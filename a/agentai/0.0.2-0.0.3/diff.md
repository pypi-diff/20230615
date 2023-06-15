# Comparing `tmp/agentai-0.0.2.tar.gz` & `tmp/agentai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentai-0.0.2.tar", max compression
+gzip compressed data, was "agentai-0.0.3.tar", max compression
```

## Comparing `agentai-0.0.2.tar` & `agentai-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-06-14 06:59:05.040089 agentai-0.0.2/LICENSE
--rw-r--r--   0        0        0     6256 2023-06-14 12:03:47.969750 agentai-0.0.2/README.md
--rw-r--r--   0        0        0     2650 2023-06-14 11:08:25.532465 agentai-0.0.2/agentai/api.py
--rw-r--r--   0        0        0      839 2023-06-14 10:22:15.497178 agentai-0.0.2/agentai/conversation.py
--rw-r--r--   0        0        0     3072 2023-06-14 11:57:13.062510 agentai-0.0.2/agentai/function_parser.py
--rw-r--r--   0        0        0     1195 2023-06-14 09:16:58.758374 agentai-0.0.2/agentai/sqlite_utils.py
--rw-r--r--   0        0        0      703 2023-06-14 12:05:36.790354 agentai-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     7202 1970-01-01 00:00:00.000000 agentai-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-14 06:59:05.040089 agentai-0.0.3/LICENSE
+-rw-r--r--   0        0        0     6610 2023-06-14 17:27:44.494698 agentai-0.0.3/README.md
+-rw-r--r--   0        0        0      264 2023-06-14 20:24:51.745667 agentai-0.0.3/agentai/__init__.py
+-rw-r--r--   0        0        0     3305 2023-06-15 14:41:20.843471 agentai-0.0.3/agentai/api.py
+-rw-r--r--   0        0        0      946 2023-06-15 14:08:03.475616 agentai-0.0.3/agentai/conversation.py
+-rw-r--r--   0        0        0     5291 2023-06-15 13:30:10.589581 agentai-0.0.3/agentai/openai_function.py
+-rw-r--r--   0        0        0     2039 2023-06-15 04:45:49.214722 agentai-0.0.3/agentai/sqlite_utils.py
+-rw-r--r--   0        0        0      740 2023-06-15 14:42:35.979896 agentai-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7637 1970-01-01 00:00:00.000000 agentai-0.0.3/PKG-INFO
```

### Comparing `agentai-0.0.2/LICENSE` & `agentai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `agentai-0.0.2/README.md` & `agentai-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -20,44 +20,50 @@
 ## Features
 
 - **API Calls**: Use AgentAI to decorate your Python functions and make them magical!
 - **SQL Database Interaction**: Seamlessly extract and utilize data from SQL databases.
 - **Function Execution**: Generate and execute function calls based on conversation context.
 - **Conversation Management**: Effectively manage and track the state of conversations. Easily define your own functions which can use messages, functions, and conversation history.
 
+### Next Week
+
+- _Multiple Functions_: Call multiple functions in a single conversation with a DSL/DAG.
+- _Retrieval_: Use AgentAI to retrieve information from a vector Database -- but only when needed!
+- _Rich Media_: Support for rich media types e.g. images, audio
+- _Function Generation_: Generate Python functions based on conversation context
+
 ## Installation
 
 Install AgentAI using pip:
 
 ```bash
 pip install agentai
 ```
 
-## Usage
-
-### Getting Started: Asking User for Missing Inputs till all inputs are available
+## Getting Started: Asking User for Missing Inputs till all inputs are available
 
 1. **Import required classes and functions**
 
 ```python
-from agentai.api import chat_complete
+from agentai.api import chat_complete, chat_complete_execute_fn
+from agentai.openai_function import tool, ToolRegistry
 from agentai.conversation import Conversation
-from agentai.function_parser import tool
+from enum import Enum
+weather_registry = ToolRegistry()
 ```
 
 2. **Define a function with `@tool` decorator**
 
 ```python
-
-from enum import Enum
 class TemperatureUnit(Enum):
     celsius = "celsius"
     fahrenheit = "fahrenheit"
 
-@tool
+
+@tool(regsitry=weather_registry)
 def get_current_weather(location: str, format: TemperatureUnit) -> str:
     """
     Get the current weather
 
     Args:
         location (str): The city and state, e.g. San Francisco, CA
         format (str): The temperature unit to use. Infer this from the users location.
@@ -77,50 +83,49 @@
 conversation = Conversation()
 conversation.add_message("user", "what is the weather like today?")
 ```
 
 4. **Use the `chat_complete` function to get a response from the model**
 
 ```python
-registered_functions = [get_current_weather]
-functions = [json.loads(func.json_info) for func in registered_functions]
-chat_response = chat_complete(conversation.conversation_history, functions=functions)
+chat_response = chat_complete(conversation.conversation_history, function_registry=weather_registry, model=GPT_MODEL)
 ```
 
 Output:
 
 ```javascript
 {'role': 'assistant',
 'content': 'In which city would you like to know the current weather?'}
 ```
 
 5. **Add user response to conversation and call `chat_complete` again**
 
 Once the user provides the required information, the model can generate the function arguments:
 
 ```python
-
 conversation.add_message("user", "I'm in Bengaluru, India")
-chat_response = chat_complete(conversation.conversation_history, functions=functions, model=GPT_MODEL)
+chat_response = chat_complete(conversation.conversation_history, function_registry=weather_registry, model=GPT_MODEL)
 
-chat_response.json()["choices"][0]["message"]["function_call"]["arguments"]
+eval(chat_response.json()["choices"][0]["message"]["function_call"]["arguments"])
 ```
 
 Output:
 
 ```python
 {'location': 'Bengaluru, India', 'format': 'celsius'}
 ```
 
-### Ramping up Usage: Implement function execution logic (e.g., a database query)
+## Example: Doing a Database Query with Generated SQL
 
 1. **Define a function with `@tool` decorator**
 
 ```python
-@tool
+db_registry = ToolRegistry()
+
+@tool(registry=db_registry)
 def ask_database(query: str) -> List[Tuple[str, str]]:
     """
     Use this function to answer user questions about music. Input should be a fully formed SQL query.
 
     Args:
         query (str): SQL query extracting info to answer the user's question.
                     SQL should be written using this database schema: <database_schema_string>
@@ -175,18 +180,18 @@
 3. Led Zeppelin - 114 tracks
 4. Metallica - 112 tracks
 5. Lost - 92 tracks
 ```
 
 ## Detailed Examples
 
-Check out our detailed [notebooks with examples](https://github.com/NirantK/agentai/docs/) where we demonstrate how to integrate AgentAI with a chatbot to create a powerful conversational assistant that can answer questions using a SQLite database.
+Check out our detailed [notebooks with examples](./docs/) where we demonstrate how to integrate AgentAI with a chatbot to create a powerful conversational assistant that can answer questions using a SQLite database.
 
 ## Contributing
 
-We welcome contributions! Please see our [contributing guidelines](https://github.com/NirantK/agentai) for more details.
+We welcome contributions! Please see our [contributing guidelines](./.github/CONTRIBUTING.md) for more details.
 
 ## Support
 
 If you encounter any issues or require further assistance, please raise an issue on our [GitHub repository](https://github.com/NirantK/agentai/issues).
 
 We hope you enjoy using AgentAI and find it helpful in powering up your AI models. Happy coding!
```

### Comparing `agentai-0.0.2/agentai/api.py` & `agentai-0.0.3/agentai/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,104 @@
 """
 API functions for the agentai package
 """
-import openai
-import requests
-from tenacity import retry, stop_after_attempt, wait_random_exponential
-
-
-@retry(wait=wait_random_exponential(min=1, max=40), stop=stop_after_attempt(3))
-def chat_complete(messages, model, functions=None, debug=False):
-    headers = {
-        "Content-Type": "application/json",
-        "Authorization": "Bearer " + openai.api_key,
-    }
-    if debug:
-        print("Generating ChatCompletion response")
-        print(f"messages: {messages}")
-    if not len(messages) > 0:
-        raise ValueError("messages must be a list of strings")
-    json_data = {"model": model, "messages": messages}
-    if functions is not None:
-        json_data.update({"functions": functions})
-        if debug:
-            print(f"functions: {functions}")
-
-    try:
-        response = requests.post(
-            "https://api.openai.com/v1/chat/completions",
-            headers=headers,
-            json=json_data,
-        )
-        return response
-    except Exception as e:
-        print("Unable to generate ChatCompletion response")
-        print(f"Exception: {e}")
-        return e
-
-
-def get_function_arguments(message, conversation, functions, model):
-    function_arguments = {}
-    if message["finish_reason"] == "function_call":
-        arguments = message["message"]["function_call"]["arguments"]
-        try:
-            function_arguments = eval(arguments)
-        except SyntaxError:
-            print("Syntax error, trying again")
-            response = chat_complete(conversation.conversation_history, functions=functions, model=model)
-            message = response.json()["choices"][0]
-            function_arguments = get_function_arguments(message, conversation, functions, model)
-    else:
-        print("Function not required, responding to user")
-    return function_arguments
-
-
-def chat_complete_execute_fn(conversation, functions, model, callable_function):
-    response = chat_complete(conversation.conversation_history, functions=functions, model=model)
-    message = response.json()["choices"][0]
-    function_arguments = get_function_arguments(
-        message=message, conversation=conversation, functions=functions, model=model
+import json
+from typing import Any, Callable, Tuple
+
+from loguru import logger
+from openai import ChatCompletion
+from tenacity import retry, retry_if_exception_type, stop_after_attempt, wait_random
+
+from .conversation import Conversation
+from .openai_function import ToolRegistry
+
+logger.disable(__name__)
+
+
+@retry(
+    retry=retry_if_exception_type(ValueError),
+    stop=stop_after_attempt(5),
+)
+def chat_complete(
+    conversation: Conversation,
+    model,
+    tool_registry: ToolRegistry = None,
+    return_function_params: bool = False,
+):
+    messages = [message.dict(exclude_unset=True) for message in conversation.history]
+    if len(messages) == 0:
+        raise UserWarning("Conversation history is empty")
+
+    functions = (
+        tool_registry.get_all_function_information()
+        if tool_registry is not None
+        else []
+    )
+
+    if len(functions) == 0 and return_function_params:
+        raise UserWarning("No functions registered but expecting function parameters")
+
+    completion = ChatCompletion.create(
+        model=model,
+        messages=messages,
+        functions=functions,
+    )
+
+    message = completion.choices[0].message
+    logger.info(f"OpenAI API returned: {message}")
+    # When function params are expected
+    if return_function_params:
+        finish_reason = completion.choices[0].get("finish_reason", None)
+        if finish_reason is not None and finish_reason == "function_call":
+            logger.info(f"Got Function Call: {completion}")
+            return completion
+        raise ValueError(f"Expected function parameters, but received: {completion}")
+
+    # When a message is expected
+    if message["content"] is not None:
+        logger.info(f"Got Message: {completion}")
+        return completion
+
+    raise ValueError(
+        f"Expected a message, but received function parameters: {completion}"
+    )
+
+
+@retry(
+    retry=retry_if_exception_type(ValueError),
+    stop=stop_after_attempt(3),
+    wait=wait_random(min=1, max=3),
+    # wait=wait_exponential(multiplier=1, min=4, max=10),
+)
+def chat_complete_execute_fn(
+    conversation: Conversation,
+    tool_registry: ToolRegistry,
+    model: str,
+) -> Tuple[Any, Callable]:
+    """
+    Generate Argument and Execute a function from the Registry by the OpenAI API
+
+    Args:
+        conversation (Conversation): _description_
+        tool_registry (ToolRegistry): _description_
+        model (str): _description_
+
+    Returns:
+        Tuple[Any, Callable]: Results, Callable Function
+    """
+    completion = chat_complete(
+        conversation=conversation,
+        tool_registry=tool_registry,
+        model=model,
+        return_function_params=True,
     )
+    message = completion.choices[0].message
+    function_call = message["function_call"]
+    function_arguments = json.loads(function_call["arguments"])
+    logger.info(f"function_arguments: {function_arguments}")
+    callable_function = tool_registry.get(function_call["name"])
+    logger.info(f"callable_function: {callable_function}")
+    callable_function.validate(**function_arguments)
+    logger.info("Validated function arguments")
     results = callable_function(**function_arguments)
-    conversation.add_message(role="function", name=callable_function.__name__, content=str(results))
-    response = chat_complete(conversation.conversation_history, functions=functions, model=model)
-    assistant_message = response.json()["choices"][0]["message"]["content"]
-    conversation.add_message(role="assistant", content=assistant_message)
-    return assistant_message
+    logger.info(f"results: {results}")
+    return results, function_arguments, callable_function
```

### Comparing `agentai-0.0.2/pyproject.toml` & `agentai-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agentai"
-version = "0.0.2"
+version = "0.0.3"
 description = "Python library which wraps OpenAI Functions and makes them easier to use"
 authors = ["NirantK <nirant.bits@gmail.com>"]
 license = "Apache"
 readme = "README.md"
 packages = [{include = "agentai"}]
 
 [tool.poetry.dependencies]
@@ -15,21 +15,23 @@
 requests = "^2.31.0"
 tenacity = "^8.2.2"
 ruff = "^0.0.272"
 isort = "^5.12.0"
 pandas = "^2.0.2"
 termcolor = "^2.3.0"
 typing-extensions = "^4.6.3"
+loguru = "^0.7.0"
+pydantic = "^1.10.9"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
-line-length = 120
+line-length = 88
 
 [tool.isort]
 profile = "black"
 
 [tool.ruff]
-line-length = 120
+line-length = 88
```

### Comparing `agentai-0.0.2/PKG-INFO` & `agentai-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: agentai
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python library which wraps OpenAI Functions and makes them easier to use
 License: Apache
 Author: NirantK
 Author-email: nirant.bits@gmail.com
 Requires-Python: >=3.8.16,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docstring-parser (>=0.15,<0.16)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
+Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: ruff (>=0.0.272,<0.0.273)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: termcolor (>=2.3.0,<3.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Description-Content-Type: text/markdown
@@ -45,44 +47,50 @@
 ## Features
 
 - **API Calls**: Use AgentAI to decorate your Python functions and make them magical!
 - **SQL Database Interaction**: Seamlessly extract and utilize data from SQL databases.
 - **Function Execution**: Generate and execute function calls based on conversation context.
 - **Conversation Management**: Effectively manage and track the state of conversations. Easily define your own functions which can use messages, functions, and conversation history.
 
+### Next Week
+
+- _Multiple Functions_: Call multiple functions in a single conversation with a DSL/DAG.
+- _Retrieval_: Use AgentAI to retrieve information from a vector Database -- but only when needed!
+- _Rich Media_: Support for rich media types e.g. images, audio
+- _Function Generation_: Generate Python functions based on conversation context
+
 ## Installation
 
 Install AgentAI using pip:
 
 ```bash
 pip install agentai
 ```
 
-## Usage
-
-### Getting Started: Asking User for Missing Inputs till all inputs are available
+## Getting Started: Asking User for Missing Inputs till all inputs are available
 
 1. **Import required classes and functions**
 
 ```python
-from agentai.api import chat_complete
+from agentai.api import chat_complete, chat_complete_execute_fn
+from agentai.openai_function import tool, ToolRegistry
 from agentai.conversation import Conversation
-from agentai.function_parser import tool
+from enum import Enum
+weather_registry = ToolRegistry()
 ```
 
 2. **Define a function with `@tool` decorator**
 
 ```python
-
-from enum import Enum
 class TemperatureUnit(Enum):
     celsius = "celsius"
     fahrenheit = "fahrenheit"
 
-@tool
+
+@tool(regsitry=weather_registry)
 def get_current_weather(location: str, format: TemperatureUnit) -> str:
     """
     Get the current weather
 
     Args:
         location (str): The city and state, e.g. San Francisco, CA
         format (str): The temperature unit to use. Infer this from the users location.
@@ -102,50 +110,49 @@
 conversation = Conversation()
 conversation.add_message("user", "what is the weather like today?")
 ```
 
 4. **Use the `chat_complete` function to get a response from the model**
 
 ```python
-registered_functions = [get_current_weather]
-functions = [json.loads(func.json_info) for func in registered_functions]
-chat_response = chat_complete(conversation.conversation_history, functions=functions)
+chat_response = chat_complete(conversation.conversation_history, function_registry=weather_registry, model=GPT_MODEL)
 ```
 
 Output:
 
 ```javascript
 {'role': 'assistant',
 'content': 'In which city would you like to know the current weather?'}
 ```
 
 5. **Add user response to conversation and call `chat_complete` again**
 
 Once the user provides the required information, the model can generate the function arguments:
 
 ```python
-
 conversation.add_message("user", "I'm in Bengaluru, India")
-chat_response = chat_complete(conversation.conversation_history, functions=functions, model=GPT_MODEL)
+chat_response = chat_complete(conversation.conversation_history, function_registry=weather_registry, model=GPT_MODEL)
 
-chat_response.json()["choices"][0]["message"]["function_call"]["arguments"]
+eval(chat_response.json()["choices"][0]["message"]["function_call"]["arguments"])
 ```
 
 Output:
 
 ```python
 {'location': 'Bengaluru, India', 'format': 'celsius'}
 ```
 
-### Ramping up Usage: Implement function execution logic (e.g., a database query)
+## Example: Doing a Database Query with Generated SQL
 
 1. **Define a function with `@tool` decorator**
 
 ```python
-@tool
+db_registry = ToolRegistry()
+
+@tool(registry=db_registry)
 def ask_database(query: str) -> List[Tuple[str, str]]:
     """
     Use this function to answer user questions about music. Input should be a fully formed SQL query.
 
     Args:
         query (str): SQL query extracting info to answer the user's question.
                     SQL should be written using this database schema: <database_schema_string>
@@ -200,19 +207,19 @@
 3. Led Zeppelin - 114 tracks
 4. Metallica - 112 tracks
 5. Lost - 92 tracks
 ```
 
 ## Detailed Examples
 
-Check out our detailed [notebooks with examples](https://github.com/NirantK/agentai/docs/) where we demonstrate how to integrate AgentAI with a chatbot to create a powerful conversational assistant that can answer questions using a SQLite database.
+Check out our detailed [notebooks with examples](./docs/) where we demonstrate how to integrate AgentAI with a chatbot to create a powerful conversational assistant that can answer questions using a SQLite database.
 
 ## Contributing
 
-We welcome contributions! Please see our [contributing guidelines](https://github.com/NirantK/agentai) for more details.
+We welcome contributions! Please see our [contributing guidelines](./.github/CONTRIBUTING.md) for more details.
 
 ## Support
 
 If you encounter any issues or require further assistance, please raise an issue on our [GitHub repository](https://github.com/NirantK/agentai/issues).
 
 We hope you enjoy using AgentAI and find it helpful in powering up your AI models. Happy coding!
```

