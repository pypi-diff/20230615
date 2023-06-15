# Comparing `tmp/langchain-decorators-0.0.4.tar.gz` & `tmp/langchain-decorators-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-decorators-0.0.4.tar", last modified: Tue Jun 13 09:49:27 2023, max compression
+gzip compressed data, was "langchain-decorators-0.0.6.tar", last modified: Thu Jun 15 09:31:18 2023, max compression
```

## Comparing `langchain-decorators-0.0.4.tar` & `langchain-decorators-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-13 09:49:27.993785 langchain-decorators-0.0.4/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1066 2023-06-09 22:30:45.000000 langchain-decorators-0.0.4/LICENSE
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    12625 2023-06-13 09:49:27.993512 langchain-decorators-0.0.4/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    12270 2023-06-10 13:45:12.000000 langchain-decorators-0.0.4/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 langchain-decorators-0.0.4/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-06-13 09:49:27.993879 langchain-decorators-0.0.4/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1117 2023-06-11 12:35:54.000000 langchain-decorators-0.0.4/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-13 09:49:27.985615 langchain-decorators-0.0.4/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-13 09:49:27.990276 langchain-decorators-0.0.4/src/langchain_decorators/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      252 2023-06-13 09:48:35.000000 langchain-decorators-0.0.4/src/langchain_decorators/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4368 2023-06-13 08:52:49.000000 langchain-decorators-0.0.4/src/langchain_decorators/common.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    17436 2023-06-13 08:10:19.000000 langchain-decorators-0.0.4/src/langchain_decorators/output_parsers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    15882 2023-06-13 09:46:48.000000 langchain-decorators-0.0.4/src/langchain_decorators/prompt_decorator.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    15765 2023-06-13 08:26:41.000000 langchain-decorators-0.0.4/src/langchain_decorators/prompt_template.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2572 2023-06-11 18:59:03.000000 langchain-decorators-0.0.4/src/langchain_decorators/pydantic_helpers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1466 2023-06-11 11:09:42.000000 langchain-decorators-0.0.4/src/langchain_decorators/streaming_context.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-13 09:49:27.993026 langchain-decorators-0.0.4/src/langchain_decorators.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    12625 2023-06-13 09:49:27.000000 langchain-decorators-0.0.4/src/langchain_decorators.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      622 2023-06-13 09:49:27.000000 langchain-decorators-0.0.4/src/langchain_decorators.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-13 09:49:27.000000 langchain-decorators-0.0.4/src/langchain_decorators.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-08 20:09:02.000000 langchain-decorators-0.0.4/src/langchain_decorators.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       22 2023-06-13 09:49:27.000000 langchain-decorators-0.0.4/src/langchain_decorators.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       21 2023-06-13 09:49:27.000000 langchain-decorators-0.0.4/src/langchain_decorators.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-15 09:31:18.770719 langchain-decorators-0.0.6/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1066 2023-06-09 22:30:45.000000 langchain-decorators-0.0.6/LICENSE
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    16608 2023-06-15 09:31:18.769936 langchain-decorators-0.0.6/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    16253 2023-06-14 19:55:04.000000 langchain-decorators-0.0.6/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 langchain-decorators-0.0.6/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-06-15 09:31:18.770787 langchain-decorators-0.0.6/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1117 2023-06-11 12:35:54.000000 langchain-decorators-0.0.6/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-15 09:31:18.760443 langchain-decorators-0.0.6/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-15 09:31:18.767055 langchain-decorators-0.0.6/src/langchain_decorators/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      301 2023-06-15 09:29:15.000000 langchain-decorators-0.0.6/src/langchain_decorators/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5901 2023-06-14 10:52:58.000000 langchain-decorators-0.0.6/src/langchain_decorators/chains.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     6371 2023-06-15 08:38:34.000000 langchain-decorators-0.0.6/src/langchain_decorators/common.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    12845 2023-06-14 19:44:20.000000 langchain-decorators-0.0.6/src/langchain_decorators/function_decorator.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    17436 2023-06-13 08:10:19.000000 langchain-decorators-0.0.6/src/langchain_decorators/output_parsers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    19850 2023-06-15 06:53:25.000000 langchain-decorators-0.0.6/src/langchain_decorators/prompt_decorator.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    15009 2023-06-14 00:48:45.000000 langchain-decorators-0.0.6/src/langchain_decorators/prompt_template.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2572 2023-06-11 18:59:03.000000 langchain-decorators-0.0.6/src/langchain_decorators/pydantic_helpers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2088 2023-06-14 14:15:48.000000 langchain-decorators-0.0.6/src/langchain_decorators/schema.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1466 2023-06-11 11:09:42.000000 langchain-decorators-0.0.6/src/langchain_decorators/streaming_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-15 09:31:18.769645 langchain-decorators-0.0.6/src/langchain_decorators.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    16608 2023-06-15 09:31:18.000000 langchain-decorators-0.0.6/src/langchain_decorators.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      739 2023-06-15 09:31:18.000000 langchain-decorators-0.0.6/src/langchain_decorators.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-15 09:31:18.000000 langchain-decorators-0.0.6/src/langchain_decorators.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-08 20:09:02.000000 langchain-decorators-0.0.6/src/langchain_decorators.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       22 2023-06-15 09:31:18.000000 langchain-decorators-0.0.6/src/langchain_decorators.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       21 2023-06-15 09:31:18.000000 langchain-decorators-0.0.6/src/langchain_decorators.egg-info/top_level.txt
```

### Comparing `langchain-decorators-0.0.4/LICENSE` & `langchain-decorators-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.4/PKG-INFO` & `langchain-decorators-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-decorators
-Version: 0.0.4
+Version: 0.0.6
 Summary: syntactic sugar for langchain
 Home-page: https://github.com/ju-bezdek/langchain-decorators
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: langchain
 Requires-Python: >=3.9
@@ -55,131 +55,15 @@
 
 ## Examples
 
 Good idea on how to start is to review the examples here:
  - [jupyter notebook](example_notebook.ipynb)
  - [colab notebook](https://colab.research.google.com/drive/1no-8WfeP6JaLD9yUtkPgym6x0G9ZYZOG#scrollTo=N4cf__D0E2Yk)
 
-# Defining other parameters
-Here we are just marking a function as a prompt with `llm_prompt` decorator, turning it effectively into a LLMChain. Instead of running it 
-
-
-Standard LLMchain takes much more init parameter than just inputs_variables and prompt... here is this implementation detail hidden in the decorator.
-Here is how it works:
-
-1. Using **Global settings**:
-
-``` python
-# define global settings for all prompty (if not set - chatGPT is the current default)
-from langchain_decorators import GlobalSettings
-
-GlobalSettings.define_settings(
-    default_llm=ChatOpenAI(temperature=0.0), this is default... can change it here globally
-    default_streaming_llm=ChatOpenAI(temperature=0.0,streaming=True), this is default... can change it here for all ... will be used for streaming
-)
-```
-
-2. Using predefined **prompt types**
-
-``` python
-#You can change the default prompt types
-from langchain_decorators import PromptTypes, PromptTypeSettings
-
-PromptTypes.AGENT_REASONING.llm = ChatOpenAI()
-
-# Or you can just define your own ones:
-class MyCustomPromptTypes(PromptTypes):
-    GPT4=PromptTypeSettings(llm=ChatOpenAI(model="gpt-4"))
-
-@llm_prompt(prompt_type=MyCustomPromptTypes.GPT4) 
-def write_a_complicated_code(app_idea:str)->str:
-    ...
-
-```
-
-3.  Define the settings **directly in the decorator**
-
-``` python
-from langchain.llms import OpenAI
-
-@llm_prompt(
-    llm=OpenAI(temperature=0.7),
-    stop_tokens=["\nObservation"],
-    ...
-    )
-def creative_writer(book_title:str)->str:
-    ...
-```
-
-## Passing a memory and/or callbacks:
-
-To pass any of these, just declare them in the function (or use kwargs to pass anything)
-
-```python
-
-@llm_prompt()
-async def write_me_short_post(topic:str, platform:str="twitter", memory:SimpleMemory = None):
-    """
-    {history_key}
-    Write me a short header for my post about {topic} for {platform} platform. 
-    It should be for {audience} audience.
-    (Max 15 words)
-    """
-    pass
-
-await write_me_short_post(topic="old movies")
-
-```
-
-# Simplified streaming
-
-If we wan't to leverage streaming:
- - we need to define prompt as async function 
- - turn on the streaming on the decorator, or we can define PromptType with streaming on
- - capture the stream using StreamingContext
-
-This way we just mark which prompt should be streamed, not needing to tinker with what LLM should we use, passing around the creating and distribute streaming handler into particular part of our chain... just turn the streaming on/off on prompt/prompt type...
 
-The streaming will happen only if we call it in streaming context ... there we can define a simple function to handle the stream
-
-``` python
-# this code example is complete and should run as it is
-
-from langchain_decorators import StreamingContext, llm_prompt
-
-# this will mark the prompt for streaming (useful if we want stream just some prompts in our app... but don't want to pass distribute the callback handlers)
-# note that only async functions can be streamed (will get an error if it's not)
-@llm_prompt(capture_stream=True) 
-async def write_me_short_post(topic:str, platform:str="twitter", audience:str = "developers"):
-    """
-    Write me a short header for my post about {topic} for {platform} platform. 
-    It should be for {audience} audience.
-    (Max 15 words)
-    """
-    pass
-
-
-
-# just an arbitrary  function to demonstrate the streaming... wil be some websockets code in the real world
-tokens=[]
-def capture_stream_func(new_token:str):
-    tokens.append(new_token)
-
-# if we want to capture the stream, we need to wrap the execution into StreamingContext... 
-# this will allow us to capture the stream even if the prompt call is hidden inside higher level method
-# only the prompts marked with capture_stream will be captured here
-with StreamingContext(stream_to_stdout=True, callback=capture_stream_func):
-    result = await run_prompt()
-    print("Stream finished ... we can distinguish tokens thanks to alternating colors")
-
-
-print("\nWe've captured",len(tokens),"tokens🎉\n")
-print("Here is the result:")
-print(result)
-```
 
 
 # Prompt declarations
 By default the prompt is is the whole function docs, unless you mark your prompt 
 
 ## Documenting your prompt
 
@@ -295,18 +179,262 @@
     """ Write me {count} good name suggestions for company that {company_business}
     """
     pass
 
 write_name_suggestions(company_business="sells cookies", count=5)
 ```
 
+## LLM functions
+- currently supported only for the latest OpenAI chat models
+
+- all you need to do is annotate your function with @llm_function decorator. 
+- This will parse the description for LLM (first coherent paragraph is considered as function description) 
+- and aso parameter descriptions (Google, Numpy and Spihnx notations are supported for now)
+
+- by default the docstring format is automatically resolved, but setting the format of the docstring can speed things up a bit.
+        -  `auto` (default): the format is automatically inferred from the docstring
+        -  `google`: the docstring is parsed as markdown (see [Google docstring format](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html))
+        -  `numpy`: the docstring is parsed as markdown (see [Numpy docstring format](https://numpydoc.readthedocs.io/en/latest/format.html))
+        -  `sphinx`: the docstring is parsed as sphinx format (see [Sphinx docstring format](https://sphinx-rtd-tutorial.readthedocs.io/en/latest/docstrings.html))
+
+
+To annotate an *"enum"* like argument, you can use this "typescript" like format: `["value_a" | "value_b"]` ... if will be parsed out.
+This text will be a part of a description too... if you dont want it, you can use this notation as a type notation. 
+Example:
+```
+Args:
+    message_type (["email" | "sms"]): type of a message  / channel how to send the message
+        
+```
+
+
+Then you pass these functions as arguments to and  `@llm_prompt` (the argument must be named `functions` ‼️)
+here you can pass any @llm_function there or a native LangChain tool 
+
+
+here is how to use it:
+
+```python
+from langchain.agents import load_tools
+from langchian_decorators import llm_function, llm_prompt, GlobalSettings
+
+@llm_function
+def send_message(message:str, addressee:str=None, message_type:str="email"):
+    """ Use this if user asks to send some message
+
+    Args:
+        message (str): message text to send
+        addressee (str): email of the adressese... in format firstName.lastName@company.com
+        message_type (str, optional): enum: ["email"|"whatsapp"]
+    """
+
+    if message_type=="email":
+        send_email(addressee, message)
+    elif message_type=="whatsapp":
+        send_whatsapp(addressee, message)
+        
+
+# load some other tools from langchain
+list_of_other_tools = load_tools(
+    tool_names=[...], 
+    llm=GlobalSettings.get_current_settings().default_llm)
+
+@llm_prompt
+def do_what_user_asks_for(user_input:str, functions:List[Union[Callable,BaseTool]]):
+    """ 
+    ``` <prompt:system>
+    Your role is to be a helpfull asistant.
+    ```
+    ``` <prompt:user>
+    {user_input}
+    ```
+    """
+
+user_input="Yo, send an email to John Smith that I will be late for the meeting"
+result = do_what_user_asks_for(
+        user_input=user_input, 
+        functions=[send_message, *list_of_other_tools]
+    )
+
+if result.is_function_call:
+    result.execute()
+else:
+    print(result.output_text)
+
+```
+
+
+If you use functions argument, the output will be always `OutputWithFunctionCall`
+
+``` python
+class OutputWithFunctionCall(BaseModel):
+    output_text:str
+    output:T
+    function_name:str =None
+    function_arguments:Union[Dict[str,Any],str,None]
+    function:Callable = None
+    function_async:Callable = None
+    
+    @property
+    def is_function_call(self):
+        ...
+    
+    @property
+    def support_async(self):
+        ...
+    
+    @property
+    def support_sync(self):
+        ...
+
+    async def execute_async(self):
+       """Executes the function asynchronously."""
+       ...
+        
+    def execute(self):
+        """ Executes the function synchronously. 
+        If the function is async, it will be executed in a event loop.
+        """
+        ...
+```
+
+If you want to see how to schema has been build, you can use `get_function_schema` method that is added to the function by the decorator:
+```python
+@llm_function
+def my_func(arg1:str):
+    ...
+
+print(my_func.get_function_schema())
+
+```
+
+
+# Defining other parameters
+Here we are just marking a function as a prompt with `llm_prompt` decorator, turning it effectively into a LLMChain. Instead of running it 
+
+
+Standard LLMchain takes much more init parameter than just inputs_variables and prompt... here is this implementation detail hidden in the decorator.
+Here is how it works:
+
+1. Using **Global settings**:
+
+``` python
+# define global settings for all prompty (if not set - chatGPT is the current default)
+from langchain_decorators import GlobalSettings
+
+GlobalSettings.define_settings(
+    default_llm=ChatOpenAI(temperature=0.0), this is default... can change it here globally
+    default_streaming_llm=ChatOpenAI(temperature=0.0,streaming=True), this is default... can change it here for all ... will be used for streaming
+)
+```
+
+2. Using predefined **prompt types**
+
+``` python
+#You can change the default prompt types
+from langchain_decorators import PromptTypes, PromptTypeSettings
+
+PromptTypes.AGENT_REASONING.llm = ChatOpenAI()
+
+# Or you can just define your own ones:
+class MyCustomPromptTypes(PromptTypes):
+    GPT4=PromptTypeSettings(llm=ChatOpenAI(model="gpt-4"))
+
+@llm_prompt(prompt_type=MyCustomPromptTypes.GPT4) 
+def write_a_complicated_code(app_idea:str)->str:
+    ...
+
+```
+
+3.  Define the settings **directly in the decorator**
+
+``` python
+from langchain.llms import OpenAI
+
+@llm_prompt(
+    llm=OpenAI(temperature=0.7),
+    stop_tokens=["\nObservation"],
+    ...
+    )
+def creative_writer(book_title:str)->str:
+    ...
+```
+
+## Passing a memory and/or callbacks:
+
+To pass any of these, just declare them in the function (or use kwargs to pass anything)
+
+```python
+
+@llm_prompt()
+async def write_me_short_post(topic:str, platform:str="twitter", memory:SimpleMemory = None):
+    """
+    {history_key}
+    Write me a short header for my post about {topic} for {platform} platform. 
+    It should be for {audience} audience.
+    (Max 15 words)
+    """
+    pass
+
+await write_me_short_post(topic="old movies")
+
+```
+
+# Simplified streaming
+
+If we wan't to leverage streaming:
+ - we need to define prompt as async function 
+ - turn on the streaming on the decorator, or we can define PromptType with streaming on
+ - capture the stream using StreamingContext
+
+This way we just mark which prompt should be streamed, not needing to tinker with what LLM should we use, passing around the creating and distribute streaming handler into particular part of our chain... just turn the streaming on/off on prompt/prompt type...
+
+The streaming will happen only if we call it in streaming context ... there we can define a simple function to handle the stream
+
+``` python
+# this code example is complete and should run as it is
+
+from langchain_decorators import StreamingContext, llm_prompt
+
+# this will mark the prompt for streaming (useful if we want stream just some prompts in our app... but don't want to pass distribute the callback handlers)
+# note that only async functions can be streamed (will get an error if it's not)
+@llm_prompt(capture_stream=True) 
+async def write_me_short_post(topic:str, platform:str="twitter", audience:str = "developers"):
+    """
+    Write me a short header for my post about {topic} for {platform} platform. 
+    It should be for {audience} audience.
+    (Max 15 words)
+    """
+    pass
+
+
+
+# just an arbitrary  function to demonstrate the streaming... wil be some websockets code in the real world
+tokens=[]
+def capture_stream_func(new_token:str):
+    tokens.append(new_token)
+
+# if we want to capture the stream, we need to wrap the execution into StreamingContext... 
+# this will allow us to capture the stream even if the prompt call is hidden inside higher level method
+# only the prompts marked with capture_stream will be captured here
+with StreamingContext(stream_to_stdout=True, callback=capture_stream_func):
+    result = await run_prompt()
+    print("Stream finished ... we can distinguish tokens thanks to alternating colors")
+
+
+print("\nWe've captured",len(tokens),"tokens🎉\n")
+print("Here is the result:")
+print(result)
+```
+
+
 ## More complex structures
 
 for dict / pydantic you need to specify the formatting instructions... 
-this can be tedious, that's why you can let the output parser gegnerate you the instructions based on the model (pydantic)
+this can be tedious, that's why you can let the output parser generate you the instructions based on the model (pydantic)
 
 ``` python
 from langchain_decorators import llm_prompt
 from pydantic import BaseModel, Field
 
 
 class TheOutputStructureWeExpect(BaseModel):
```

### Comparing `langchain-decorators-0.0.4/README.md` & `langchain-decorators-0.0.6/src/langchain_decorators.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: langchain-decorators
+Version: 0.0.6
+Summary: syntactic sugar for langchain
+Home-page: https://github.com/ju-bezdek/langchain-decorators
+Author: Juraj Bezdek
+Author-email: juraj.bezdek@blip.solutions
+License: MIT License
+Keywords: langchain
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # LangChain Decorators ✨
 
 lanchchain decorators is a layer on the top op LangChain that provides syntactic sugar 🍭 for writing custom langchain prompts and chains
 
 > **Note:** This is an unofficial addon to langchain library. It's not trying to compete, just to make using it easier. Lot's of ideas here are totally opinionated 
 
 Main principles and benefits:
@@ -42,131 +55,15 @@
 
 ## Examples
 
 Good idea on how to start is to review the examples here:
  - [jupyter notebook](example_notebook.ipynb)
  - [colab notebook](https://colab.research.google.com/drive/1no-8WfeP6JaLD9yUtkPgym6x0G9ZYZOG#scrollTo=N4cf__D0E2Yk)
 
-# Defining other parameters
-Here we are just marking a function as a prompt with `llm_prompt` decorator, turning it effectively into a LLMChain. Instead of running it 
-
-
-Standard LLMchain takes much more init parameter than just inputs_variables and prompt... here is this implementation detail hidden in the decorator.
-Here is how it works:
-
-1. Using **Global settings**:
-
-``` python
-# define global settings for all prompty (if not set - chatGPT is the current default)
-from langchain_decorators import GlobalSettings
-
-GlobalSettings.define_settings(
-    default_llm=ChatOpenAI(temperature=0.0), this is default... can change it here globally
-    default_streaming_llm=ChatOpenAI(temperature=0.0,streaming=True), this is default... can change it here for all ... will be used for streaming
-)
-```
-
-2. Using predefined **prompt types**
-
-``` python
-#You can change the default prompt types
-from langchain_decorators import PromptTypes, PromptTypeSettings
-
-PromptTypes.AGENT_REASONING.llm = ChatOpenAI()
-
-# Or you can just define your own ones:
-class MyCustomPromptTypes(PromptTypes):
-    GPT4=PromptTypeSettings(llm=ChatOpenAI(model="gpt-4"))
 
-@llm_prompt(prompt_type=MyCustomPromptTypes.GPT4) 
-def write_a_complicated_code(app_idea:str)->str:
-    ...
-
-```
-
-3.  Define the settings **directly in the decorator**
-
-``` python
-from langchain.llms import OpenAI
-
-@llm_prompt(
-    llm=OpenAI(temperature=0.7),
-    stop_tokens=["\nObservation"],
-    ...
-    )
-def creative_writer(book_title:str)->str:
-    ...
-```
-
-## Passing a memory and/or callbacks:
-
-To pass any of these, just declare them in the function (or use kwargs to pass anything)
-
-```python
-
-@llm_prompt()
-async def write_me_short_post(topic:str, platform:str="twitter", memory:SimpleMemory = None):
-    """
-    {history_key}
-    Write me a short header for my post about {topic} for {platform} platform. 
-    It should be for {audience} audience.
-    (Max 15 words)
-    """
-    pass
-
-await write_me_short_post(topic="old movies")
-
-```
-
-# Simplified streaming
-
-If we wan't to leverage streaming:
- - we need to define prompt as async function 
- - turn on the streaming on the decorator, or we can define PromptType with streaming on
- - capture the stream using StreamingContext
-
-This way we just mark which prompt should be streamed, not needing to tinker with what LLM should we use, passing around the creating and distribute streaming handler into particular part of our chain... just turn the streaming on/off on prompt/prompt type...
-
-The streaming will happen only if we call it in streaming context ... there we can define a simple function to handle the stream
-
-``` python
-# this code example is complete and should run as it is
-
-from langchain_decorators import StreamingContext, llm_prompt
-
-# this will mark the prompt for streaming (useful if we want stream just some prompts in our app... but don't want to pass distribute the callback handlers)
-# note that only async functions can be streamed (will get an error if it's not)
-@llm_prompt(capture_stream=True) 
-async def write_me_short_post(topic:str, platform:str="twitter", audience:str = "developers"):
-    """
-    Write me a short header for my post about {topic} for {platform} platform. 
-    It should be for {audience} audience.
-    (Max 15 words)
-    """
-    pass
-
-
-
-# just an arbitrary  function to demonstrate the streaming... wil be some websockets code in the real world
-tokens=[]
-def capture_stream_func(new_token:str):
-    tokens.append(new_token)
-
-# if we want to capture the stream, we need to wrap the execution into StreamingContext... 
-# this will allow us to capture the stream even if the prompt call is hidden inside higher level method
-# only the prompts marked with capture_stream will be captured here
-with StreamingContext(stream_to_stdout=True, callback=capture_stream_func):
-    result = await run_prompt()
-    print("Stream finished ... we can distinguish tokens thanks to alternating colors")
-
-
-print("\nWe've captured",len(tokens),"tokens🎉\n")
-print("Here is the result:")
-print(result)
-```
 
 
 # Prompt declarations
 By default the prompt is is the whole function docs, unless you mark your prompt 
 
 ## Documenting your prompt
 
@@ -282,18 +179,262 @@
     """ Write me {count} good name suggestions for company that {company_business}
     """
     pass
 
 write_name_suggestions(company_business="sells cookies", count=5)
 ```
 
+## LLM functions
+- currently supported only for the latest OpenAI chat models
+
+- all you need to do is annotate your function with @llm_function decorator. 
+- This will parse the description for LLM (first coherent paragraph is considered as function description) 
+- and aso parameter descriptions (Google, Numpy and Spihnx notations are supported for now)
+
+- by default the docstring format is automatically resolved, but setting the format of the docstring can speed things up a bit.
+        -  `auto` (default): the format is automatically inferred from the docstring
+        -  `google`: the docstring is parsed as markdown (see [Google docstring format](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html))
+        -  `numpy`: the docstring is parsed as markdown (see [Numpy docstring format](https://numpydoc.readthedocs.io/en/latest/format.html))
+        -  `sphinx`: the docstring is parsed as sphinx format (see [Sphinx docstring format](https://sphinx-rtd-tutorial.readthedocs.io/en/latest/docstrings.html))
+
+
+To annotate an *"enum"* like argument, you can use this "typescript" like format: `["value_a" | "value_b"]` ... if will be parsed out.
+This text will be a part of a description too... if you dont want it, you can use this notation as a type notation. 
+Example:
+```
+Args:
+    message_type (["email" | "sms"]): type of a message  / channel how to send the message
+        
+```
+
+
+Then you pass these functions as arguments to and  `@llm_prompt` (the argument must be named `functions` ‼️)
+here you can pass any @llm_function there or a native LangChain tool 
+
+
+here is how to use it:
+
+```python
+from langchain.agents import load_tools
+from langchian_decorators import llm_function, llm_prompt, GlobalSettings
+
+@llm_function
+def send_message(message:str, addressee:str=None, message_type:str="email"):
+    """ Use this if user asks to send some message
+
+    Args:
+        message (str): message text to send
+        addressee (str): email of the adressese... in format firstName.lastName@company.com
+        message_type (str, optional): enum: ["email"|"whatsapp"]
+    """
+
+    if message_type=="email":
+        send_email(addressee, message)
+    elif message_type=="whatsapp":
+        send_whatsapp(addressee, message)
+        
+
+# load some other tools from langchain
+list_of_other_tools = load_tools(
+    tool_names=[...], 
+    llm=GlobalSettings.get_current_settings().default_llm)
+
+@llm_prompt
+def do_what_user_asks_for(user_input:str, functions:List[Union[Callable,BaseTool]]):
+    """ 
+    ``` <prompt:system>
+    Your role is to be a helpfull asistant.
+    ```
+    ``` <prompt:user>
+    {user_input}
+    ```
+    """
+
+user_input="Yo, send an email to John Smith that I will be late for the meeting"
+result = do_what_user_asks_for(
+        user_input=user_input, 
+        functions=[send_message, *list_of_other_tools]
+    )
+
+if result.is_function_call:
+    result.execute()
+else:
+    print(result.output_text)
+
+```
+
+
+If you use functions argument, the output will be always `OutputWithFunctionCall`
+
+``` python
+class OutputWithFunctionCall(BaseModel):
+    output_text:str
+    output:T
+    function_name:str =None
+    function_arguments:Union[Dict[str,Any],str,None]
+    function:Callable = None
+    function_async:Callable = None
+    
+    @property
+    def is_function_call(self):
+        ...
+    
+    @property
+    def support_async(self):
+        ...
+    
+    @property
+    def support_sync(self):
+        ...
+
+    async def execute_async(self):
+       """Executes the function asynchronously."""
+       ...
+        
+    def execute(self):
+        """ Executes the function synchronously. 
+        If the function is async, it will be executed in a event loop.
+        """
+        ...
+```
+
+If you want to see how to schema has been build, you can use `get_function_schema` method that is added to the function by the decorator:
+```python
+@llm_function
+def my_func(arg1:str):
+    ...
+
+print(my_func.get_function_schema())
+
+```
+
+
+# Defining other parameters
+Here we are just marking a function as a prompt with `llm_prompt` decorator, turning it effectively into a LLMChain. Instead of running it 
+
+
+Standard LLMchain takes much more init parameter than just inputs_variables and prompt... here is this implementation detail hidden in the decorator.
+Here is how it works:
+
+1. Using **Global settings**:
+
+``` python
+# define global settings for all prompty (if not set - chatGPT is the current default)
+from langchain_decorators import GlobalSettings
+
+GlobalSettings.define_settings(
+    default_llm=ChatOpenAI(temperature=0.0), this is default... can change it here globally
+    default_streaming_llm=ChatOpenAI(temperature=0.0,streaming=True), this is default... can change it here for all ... will be used for streaming
+)
+```
+
+2. Using predefined **prompt types**
+
+``` python
+#You can change the default prompt types
+from langchain_decorators import PromptTypes, PromptTypeSettings
+
+PromptTypes.AGENT_REASONING.llm = ChatOpenAI()
+
+# Or you can just define your own ones:
+class MyCustomPromptTypes(PromptTypes):
+    GPT4=PromptTypeSettings(llm=ChatOpenAI(model="gpt-4"))
+
+@llm_prompt(prompt_type=MyCustomPromptTypes.GPT4) 
+def write_a_complicated_code(app_idea:str)->str:
+    ...
+
+```
+
+3.  Define the settings **directly in the decorator**
+
+``` python
+from langchain.llms import OpenAI
+
+@llm_prompt(
+    llm=OpenAI(temperature=0.7),
+    stop_tokens=["\nObservation"],
+    ...
+    )
+def creative_writer(book_title:str)->str:
+    ...
+```
+
+## Passing a memory and/or callbacks:
+
+To pass any of these, just declare them in the function (or use kwargs to pass anything)
+
+```python
+
+@llm_prompt()
+async def write_me_short_post(topic:str, platform:str="twitter", memory:SimpleMemory = None):
+    """
+    {history_key}
+    Write me a short header for my post about {topic} for {platform} platform. 
+    It should be for {audience} audience.
+    (Max 15 words)
+    """
+    pass
+
+await write_me_short_post(topic="old movies")
+
+```
+
+# Simplified streaming
+
+If we wan't to leverage streaming:
+ - we need to define prompt as async function 
+ - turn on the streaming on the decorator, or we can define PromptType with streaming on
+ - capture the stream using StreamingContext
+
+This way we just mark which prompt should be streamed, not needing to tinker with what LLM should we use, passing around the creating and distribute streaming handler into particular part of our chain... just turn the streaming on/off on prompt/prompt type...
+
+The streaming will happen only if we call it in streaming context ... there we can define a simple function to handle the stream
+
+``` python
+# this code example is complete and should run as it is
+
+from langchain_decorators import StreamingContext, llm_prompt
+
+# this will mark the prompt for streaming (useful if we want stream just some prompts in our app... but don't want to pass distribute the callback handlers)
+# note that only async functions can be streamed (will get an error if it's not)
+@llm_prompt(capture_stream=True) 
+async def write_me_short_post(topic:str, platform:str="twitter", audience:str = "developers"):
+    """
+    Write me a short header for my post about {topic} for {platform} platform. 
+    It should be for {audience} audience.
+    (Max 15 words)
+    """
+    pass
+
+
+
+# just an arbitrary  function to demonstrate the streaming... wil be some websockets code in the real world
+tokens=[]
+def capture_stream_func(new_token:str):
+    tokens.append(new_token)
+
+# if we want to capture the stream, we need to wrap the execution into StreamingContext... 
+# this will allow us to capture the stream even if the prompt call is hidden inside higher level method
+# only the prompts marked with capture_stream will be captured here
+with StreamingContext(stream_to_stdout=True, callback=capture_stream_func):
+    result = await run_prompt()
+    print("Stream finished ... we can distinguish tokens thanks to alternating colors")
+
+
+print("\nWe've captured",len(tokens),"tokens🎉\n")
+print("Here is the result:")
+print(result)
+```
+
+
 ## More complex structures
 
 for dict / pydantic you need to specify the formatting instructions... 
-this can be tedious, that's why you can let the output parser gegnerate you the instructions based on the model (pydantic)
+this can be tedious, that's why you can let the output parser generate you the instructions based on the model (pydantic)
 
 ``` python
 from langchain_decorators import llm_prompt
 from pydantic import BaseModel, Field
 
 
 class TheOutputStructureWeExpect(BaseModel):
@@ -367,8 +508,8 @@
 
 # Contributing
 feedback, contributions and PR are welcomed 🙏
 
 
 # Others
 - this project is dependant on [langchain](https://github.com/hwchase17/langchain) (obviously) 
-- as well as on promptwatch [promptwatch](https://github.com/blip-solutions/promptwatch-client), which make it easy to track and store to logs, track changes in prompts and compare them by running unit tests over the prompts... 
+- as well as on promptwatch [promptwatch](https://github.com/blip-solutions/promptwatch-client), which make it easy to track and store to logs, track changes in prompts and compare them by running unit tests over the prompts...
```

### Comparing `langchain-decorators-0.0.4/setup.py` & `langchain-decorators-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.4/src/langchain_decorators/output_parsers.py` & `langchain-decorators-0.0.6/src/langchain_decorators/output_parsers.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.4/src/langchain_decorators/prompt_decorator.py` & `langchain-decorators-0.0.6/src/langchain_decorators/prompt_decorator.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,29 +4,32 @@
 
 from functools import wraps
 from textwrap import dedent
 from typing import Callable, List, Optional, Sequence, Union
 
 
 from langchain import LLMChain,  PromptTemplate
-
+from langchain.tools.base import BaseTool
 from langchain.schema import BaseOutputParser
 from langchain.llms.base import BaseLanguageModel
 
 from promptwatch import register_prompt_template
 
+from .schema import OutputWithFunctionCall
+
+from .chains import LLMChainWithFunctionSupport
+
 
 
 from .common import *
 from .prompt_template import PromptDecoratorTemplate
 from .output_parsers import *
 from .streaming_context import StreamingContext
 
 
-
 def llm_prompt(
         prompt_type:PromptTypeSettings=PromptTypes.UNDEFINED, # do not change the order of this first parameter unless you will change also the fist few lines... since we are handling cases when decorator is used with and without arguments too, than this will be the func
         template_format:str = "f-string-extra",
         output_parser:Union[str,None, BaseOutputParser]="auto", 
         stop_tokens:List[str]=None, 
         template_name:str=None, 
         template_version:str=None, 
@@ -93,20 +96,24 @@
     if verbose:
         if prompt_type:
             prompt_type = prompt_type.as_verbose()
         else:
             prompt_type = PromptTypeSettings(color=LogColors.DARK_GRAY,log_level=100, capture_stream=capture_stream)
             
     
-        
+    
     def decorator(func):
         prompt_str = dedent(func.__doc__)
         name=func.__name__
         full_name=f"{func.__module__}.{name}" if func.__module__!="__main__" else name
         is_async = inspect.iscoroutinefunction(func)
+
+
+        
+
         if prompt_type:
             _capture_stream = prompt_type.capture_stream if capture_stream is None else capture_stream
         else:
             _capture_stream = capture_stream
         if _capture_stream:
 
             if not is_async:
@@ -156,35 +163,48 @@
                     kwargs["callbacks"] = [StreamingContext.StreamingContextCallback()]
 
             if "memory" in kwargs:
                 memory = kwargs.pop("memory")
             else:
                 memory=None
 
+            if "functions" in kwargs:
+                functions=kwargs.pop("functions")
+            else:
+                functions=None
+
+
+
             prompt_template = PromptDecoratorTemplate.from_func(func, 
                                                             template_format=template_format, 
                                                             output_parser=output_parser, 
                                                             format_instructions_parameter_key=format_instructions_parameter_key,
                                                             template_name=template_name,
                                                             template_version=template_version,
                                                             prompt_type=prompt_type,
                                                             )
             if prompt_template.default_values:
                 kwargs = {**prompt_template.default_values, **kwargs}
 
-            llmChain = LLMChain(llm=prompt_llm, prompt=prompt_template,  memory=memory)
+            if functions:
+                llmChain = LLMChainWithFunctionSupport(llm=prompt_llm, prompt=prompt_template,  memory=memory, functions=functions)
+            else:
+                llmChain = LLMChain(llm=prompt_llm, prompt=prompt_template,  memory=memory)
             other_supported_kwargs={"stop","callbacks"}
             unexpected_inputs = [key for key in kwargs if key not in prompt_template.input_variables and key not in other_supported_kwargs ]
             if unexpected_inputs:
                 raise TypeError(f"Unexpected inputs for prompt function {full_name}: {unexpected_inputs}. \nValid inputs are: {prompt_template.input_variables}")
             
             missing_inputs = [key for key in prompt_template.input_variables if key not in kwargs ]
             if format_instructions_parameter_key in missing_inputs:
                 missing_inputs.remove(format_instructions_parameter_key)
                 kwargs[format_instructions_parameter_key]=None #init the format instructions with None... will be filled later
+            if memory and memory.memory_key in missing_inputs:
+                missing_inputs.remove(memory.memory_key)
+
             if missing_inputs:
                 if input_variables_source:
                     missing_value={}
                     for key in missing_inputs:
                         value= getattr(input_variables_source, key,missing_value)
                         if value is missing_value:
                             raise TypeError(f"Missing a input for prompt function {full_name}: {key}.")
@@ -195,16 +215,16 @@
                         
                 else:
                     raise TypeError(f"{full_name}: missing 1 required keyword-only argument: {missing_inputs}")
                 
 
             if stop_tokens:
                 kwargs["stop"]=stop_tokens
-            chain_args = kwargs
-            return llmChain, chain_args
+            call_args = {"inputs":kwargs, "return_only_outputs":True}
+            return llmChain, call_args
         
         def get_retry_parse_call_args(prompt_template:PromptDecoratorTemplate, exception:OutputParserExceptionWithOriginal, get_original_prompt:Callable):
             logging.warning(msg=f"Failed to parse output for {full_name}: {exception}\nRetrying...")
             if format_instructions_parameter_key not in prompt_str:
                 logging.warning(f"Please note that we didn't find a {format_instructions_parameter_key} parameter in the prompt string. If you don't include it in your prompt template, you need to provide your custom formatting instructions.")    
             if exception.original_prompt_needed_on_retry:
                 original_prompt=get_original_prompt()
@@ -215,61 +235,74 @@
             prompt_llm=llm or GlobalSettings.get_current_settings().default_llm
             retryChain = LLMChain(llm=prompt_llm, prompt=retry_parse_template)
             format_instructions = prompt_template.output_parser.get_format_instructions()
             if not format_instructions:
                 raise Exception(f"Failed to get format instructions for {full_name} from output parser {prompt_template.output_parser}.")
             call_kwargs = {"original_prompt":original_prompt, "original":exception.original, "format_instructions":format_instructions}
             return retryChain, call_kwargs
-
+        
+        def process_results(llmChain, result_data, result, is_function_call):
+            log_results(result_data, result, is_function_call, verbose, prompt_type)
+            if llmChain.prompt.output_parser:
+                if result or not is_function_call:
+                    result = llmChain.prompt.output_parser.parse(result)
+            return result
 
         if not is_async:
 
             @wraps(func)
             def wrapper(*args, **kwargs):
                 
                 print_log(log_object=f"> Entering {name} prompt decorator chain", log_level=prompt_type.log_level if prompt_type else logging.DEBUG,color=LogColors.WHITE_BOLD)
                 llmChain, chain_args = prepare_call_args(*args, **kwargs)
 
                 try:
-                    result = llmChain.predict(**chain_args)
-                    if verbose or prompt_type:
-                        print_log(log_object=f"\nResult:\n{result}", log_level=prompt_type.log_level if verbose else 100,color=prompt_type.color if prompt_type else LogColors.BLUE)
-                    if llmChain.prompt.output_parser:
-                        result = llmChain.prompt.output_parser.parse(result)
+                    result_data = llmChain(**chain_args)
+
+                    result = result_data[llmChain.output_key]
+                    is_function_call = result_data.get("function_call_info")
+                    result = process_results(llmChain, result_data, result,is_function_call)
+                        
                     
                 except OutputParserException as e:
                     if retry_on_output_parsing_error and isinstance(e, OutputParserExceptionWithOriginal):
                         prompt_template = llmChain.prompt 
                         retryChain, call_kwargs = get_retry_parse_call_args(prompt_template, e, lambda: llmChain.prompt.format(**chain_args))
                         result = retryChain.predict(**call_kwargs)
                         if verbose or prompt_type:
                             print_log(log_object=f"\nResult:\n{result}", log_level=prompt_type.log_level if not verbose else 100,color=prompt_type.color if prompt_type else LogColors.BLUE)
                         parsed = prompt_template.output_parser.parse(result)
                         return parsed
                     else: 
                         raise e
 
                 print_log(log_object=f"> Finished chain", log_level=prompt_type.log_level if prompt_type else logging.DEBUG,color=LogColors.WHITE_BOLD)
+                if "function_call_info" in result_data:
+                    return _generate_output_with_function_call(result=result, result_data=result_data, verbose=verbose,callbacks=kwargs.get("callbacks"))
                 return result
+
+            
+
+            
             return wrapper
         
         else:
             @wraps(func)
             async def async_wrapper(*args, **kwargs):
                 
                 
                 print_log(log_object=f"> Entering {name} prompt decorator chain", log_level=prompt_type.log_level if prompt_type else logging.DEBUG,color=LogColors.WHITE_BOLD)
                 llmChain, chain_args = prepare_call_args(*args, **kwargs)
 
                 try:
-                    result = await llmChain.apredict(**chain_args)
-                    if verbose or prompt_type:
-                        print_log(log_object=f"\nResult:\n{result}", log_level=prompt_type.log_level if not verbose else 100,color=prompt_type.color if prompt_type else LogColors.BLUE)
-                    if llmChain.prompt.output_parser:
-                        result = llmChain.prompt.output_parser.parse(result)
+                    
+                    result_data = await llmChain.acall(**chain_args)
+                    result = result_data[llmChain.output_key]
+                    is_function_call = result_data.get("function_call_info")
+                    result = process_results(llmChain, result_data, result,is_function_call)
                     
                     
                 except OutputParserException as e:
                     if retry_on_output_parsing_error and isinstance(e, OutputParserExceptionWithOriginal):
                         prompt_template = llmChain.prompt 
                         retryChain, call_kwargs = get_retry_parse_call_args(prompt_template, e, lambda: llmChain.prompt.format(**chain_args))
                         result = await retryChain.apredict(**call_kwargs)
@@ -277,16 +310,74 @@
                             print_log(log_object=f"\nResult:\n{result}", log_level=prompt_type.log_level if not verbose else 100,color=prompt_type.color if prompt_type else LogColors.BLUE)
                         parsed = prompt_template.output_parser.parse(result)
                         return parsed
                     else: 
                         raise e
 
                 print_log(log_object=f"> Finished chain", log_level=prompt_type.log_level if prompt_type else logging.DEBUG,color=LogColors.WHITE_BOLD)
+                if "function_call_info" in result_data:
+                    return _generate_output_with_function_call(result=result, result_data=result_data, verbose=verbose,callbacks=kwargs.get("callbacks"))
                 return result
             return async_wrapper
-        
     if func:
         return decorator(func)
     else:
         return decorator
 
 
+
+
+def _generate_output_with_function_call(result:Any, result_data:dict, verbose, callbacks):
+    """ get parsed result, function call data from llm and list of functions and build  OutputWithFunctionCall """
+    # find the function first:
+    
+    _function = result_data["function"]
+    if result_data.get("function_call_info"):
+        _tool_arguments = result_data["function_call_info"]["arguments"]
+        if isinstance(_function, BaseTool):
+            # langchain hack >> "__arg1" as a single argument hack
+            _is_single_arg_hack="__arg1" in _tool_arguments and len(_tool_arguments)==1
+            tool_input= _tool_arguments["__arg1"] if _is_single_arg_hack else _tool_arguments
+            _tool_arguments = tool_input
+            def _sync_function(arguments=tool_input):
+                return _function.run(tool_input=arguments, verbose=verbose, callbacks=callbacks)
+            
+            async def _async_function(arguments=tool_input):
+                return await _function.arun(tool_input=arguments, verbose=verbose, callbacks=callbacks)
+                
+            
+
+        elif callable(_function):
+            # TODO: add support for verbose and callbacks
+            
+            is_async = inspect.iscoroutinefunction(_function)
+            
+            if is_async:
+                _async_function = _function
+                _sync_function = None
+            else:
+                _sync_function = _function
+                _async_function = None
+        else:
+            raise TypeError(f"Invalid function type: {_function} of type {type(_function)}")
+
+        return OutputWithFunctionCall(
+                output=result,
+                output_text=result_data["text"],
+                function=_sync_function,
+                function_async=_async_function,
+                function_name=result_data["function_call_info"]["name"],
+                function_args=result_data["function_call_info"]["arguments"],
+                function_arguments=_tool_arguments
+            )
+    else:
+        return OutputWithFunctionCall(
+                output=result,
+                output_text=result_data["text"],
+            )
+
+def log_results(result_data, result, is_function_call, verbose, prompt_type=None):
+    if verbose or prompt_type:
+        print_log(log_object=f"\nResult:\n{result}", log_level=prompt_type.log_level if verbose else 100,color=prompt_type.color if prompt_type else LogColors.BLUE)
+        if is_function_call:
+            function_call_info_str = json.dumps(result_data.get('function_call_info'),indent=4)
+            print_log(log_object=f"\nFunction call:\n{function_call_info_str}", log_level=prompt_type.log_level if verbose else 100,color=prompt_type.color if prompt_type else LogColors.BLUE)
```

### Comparing `langchain-decorators-0.0.4/src/langchain_decorators/prompt_template.py` & `langchain-decorators-0.0.6/src/langchain_decorators/prompt_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from langchain import PromptTemplate
 from langchain.prompts import StringPromptTemplate
 from langchain.prompts.chat import  MessagesPlaceholder, ChatMessagePromptTemplate, ChatPromptTemplate, ChatPromptValue
 from langchain.schema import PromptValue, BaseOutputParser
 
 from promptwatch import register_prompt_template
 
-from .common import LogColors, PromptTypeSettings, print_log
+from .common import LogColors, PromptTypeSettings, get_func_return_type, get_function_docs, get_function_full_name, print_log
 from .output_parsers import *
 
 
 def parse_prompts_from_docs(docs:str):
     prompts = []
     for i, prompt_block in enumerate(re.finditer(r"```[^\S\n]*<prompt(?P<role>:\w+)?>\n(?P<prompt>.*?)\n```[ |\t]*\n", docs, re.MULTILINE | re.DOTALL)):
         role = prompt_block.group("role")
@@ -205,32 +205,18 @@
                   template_version:str=None, 
                   output_parser:Union[str,None, BaseOutputParser]="auto", 
                   template_format:str = "f-string-extra",
                   format_instructions_parameter_key:str="FORMAT_INSTRUCTIONS",
                   prompt_type:PromptTypeSettings = None
                   )->"PromptDecoratorTemplate":
         
-        
-        fist_line, rest = func.__doc__.split('\n', 1)
-        # we dedent the first line separately,because its common that it often starts right after """
-        fist_line = fist_line.strip()
-        if fist_line:
-            fist_line+="\n"
-        template_string = fist_line + dedent(rest)
-        
-        
-        template_name=template_name or f"{func.__module__}.{func.__name__}" if not func.__module__=="__main__" else func.__name__
-        return_type = func.__annotations__.get("return",None)
-        if inspect.iscoroutinefunction(func):
-            if return_type and issubclass(return_type, Coroutine):
-                return_type_args = getattr(return_type, '__args__', None)
-                if return_type_args and len(return_type_args) == 3:
-                    return_type = return_type_args[2]
-                else:
-                    raise Exception(f"Invalid Coroutine annotation {return_type}. Expected Coroutine[ any , any, <return_type>] or just <return_type>")
+        template_string = get_function_docs(func)  
+        template_name=template_name or get_function_full_name(func)
+        return_type = get_func_return_type(func)
+      
         if output_parser=="auto":
             if return_type==str or return_type==None:
                 output_parser = "str"
             elif return_type==dict:
                 output_parser = "json"
             elif return_type==list:
                 output_parser = "list"
```

### Comparing `langchain-decorators-0.0.4/src/langchain_decorators/pydantic_helpers.py` & `langchain-decorators-0.0.6/src/langchain_decorators/pydantic_helpers.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.4/src/langchain_decorators/streaming_context.py` & `langchain-decorators-0.0.6/src/langchain_decorators/streaming_context.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.4/src/langchain_decorators.egg-info/PKG-INFO` & `langchain-decorators-0.0.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: langchain-decorators
-Version: 0.0.4
-Summary: syntactic sugar for langchain
-Home-page: https://github.com/ju-bezdek/langchain-decorators
-Author: Juraj Bezdek
-Author-email: juraj.bezdek@blip.solutions
-License: MIT License
-Keywords: langchain
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # LangChain Decorators ✨
 
 lanchchain decorators is a layer on the top op LangChain that provides syntactic sugar 🍭 for writing custom langchain prompts and chains
 
 > **Note:** This is an unofficial addon to langchain library. It's not trying to compete, just to make using it easier. Lot's of ideas here are totally opinionated 
 
 Main principles and benefits:
@@ -55,131 +42,15 @@
 
 ## Examples
 
 Good idea on how to start is to review the examples here:
  - [jupyter notebook](example_notebook.ipynb)
  - [colab notebook](https://colab.research.google.com/drive/1no-8WfeP6JaLD9yUtkPgym6x0G9ZYZOG#scrollTo=N4cf__D0E2Yk)
 
-# Defining other parameters
-Here we are just marking a function as a prompt with `llm_prompt` decorator, turning it effectively into a LLMChain. Instead of running it 
-
-
-Standard LLMchain takes much more init parameter than just inputs_variables and prompt... here is this implementation detail hidden in the decorator.
-Here is how it works:
-
-1. Using **Global settings**:
-
-``` python
-# define global settings for all prompty (if not set - chatGPT is the current default)
-from langchain_decorators import GlobalSettings
-
-GlobalSettings.define_settings(
-    default_llm=ChatOpenAI(temperature=0.0), this is default... can change it here globally
-    default_streaming_llm=ChatOpenAI(temperature=0.0,streaming=True), this is default... can change it here for all ... will be used for streaming
-)
-```
-
-2. Using predefined **prompt types**
-
-``` python
-#You can change the default prompt types
-from langchain_decorators import PromptTypes, PromptTypeSettings
-
-PromptTypes.AGENT_REASONING.llm = ChatOpenAI()
-
-# Or you can just define your own ones:
-class MyCustomPromptTypes(PromptTypes):
-    GPT4=PromptTypeSettings(llm=ChatOpenAI(model="gpt-4"))
 
-@llm_prompt(prompt_type=MyCustomPromptTypes.GPT4) 
-def write_a_complicated_code(app_idea:str)->str:
-    ...
-
-```
-
-3.  Define the settings **directly in the decorator**
-
-``` python
-from langchain.llms import OpenAI
-
-@llm_prompt(
-    llm=OpenAI(temperature=0.7),
-    stop_tokens=["\nObservation"],
-    ...
-    )
-def creative_writer(book_title:str)->str:
-    ...
-```
-
-## Passing a memory and/or callbacks:
-
-To pass any of these, just declare them in the function (or use kwargs to pass anything)
-
-```python
-
-@llm_prompt()
-async def write_me_short_post(topic:str, platform:str="twitter", memory:SimpleMemory = None):
-    """
-    {history_key}
-    Write me a short header for my post about {topic} for {platform} platform. 
-    It should be for {audience} audience.
-    (Max 15 words)
-    """
-    pass
-
-await write_me_short_post(topic="old movies")
-
-```
-
-# Simplified streaming
-
-If we wan't to leverage streaming:
- - we need to define prompt as async function 
- - turn on the streaming on the decorator, or we can define PromptType with streaming on
- - capture the stream using StreamingContext
-
-This way we just mark which prompt should be streamed, not needing to tinker with what LLM should we use, passing around the creating and distribute streaming handler into particular part of our chain... just turn the streaming on/off on prompt/prompt type...
-
-The streaming will happen only if we call it in streaming context ... there we can define a simple function to handle the stream
-
-``` python
-# this code example is complete and should run as it is
-
-from langchain_decorators import StreamingContext, llm_prompt
-
-# this will mark the prompt for streaming (useful if we want stream just some prompts in our app... but don't want to pass distribute the callback handlers)
-# note that only async functions can be streamed (will get an error if it's not)
-@llm_prompt(capture_stream=True) 
-async def write_me_short_post(topic:str, platform:str="twitter", audience:str = "developers"):
-    """
-    Write me a short header for my post about {topic} for {platform} platform. 
-    It should be for {audience} audience.
-    (Max 15 words)
-    """
-    pass
-
-
-
-# just an arbitrary  function to demonstrate the streaming... wil be some websockets code in the real world
-tokens=[]
-def capture_stream_func(new_token:str):
-    tokens.append(new_token)
-
-# if we want to capture the stream, we need to wrap the execution into StreamingContext... 
-# this will allow us to capture the stream even if the prompt call is hidden inside higher level method
-# only the prompts marked with capture_stream will be captured here
-with StreamingContext(stream_to_stdout=True, callback=capture_stream_func):
-    result = await run_prompt()
-    print("Stream finished ... we can distinguish tokens thanks to alternating colors")
-
-
-print("\nWe've captured",len(tokens),"tokens🎉\n")
-print("Here is the result:")
-print(result)
-```
 
 
 # Prompt declarations
 By default the prompt is is the whole function docs, unless you mark your prompt 
 
 ## Documenting your prompt
 
@@ -295,18 +166,262 @@
     """ Write me {count} good name suggestions for company that {company_business}
     """
     pass
 
 write_name_suggestions(company_business="sells cookies", count=5)
 ```
 
+## LLM functions
+- currently supported only for the latest OpenAI chat models
+
+- all you need to do is annotate your function with @llm_function decorator. 
+- This will parse the description for LLM (first coherent paragraph is considered as function description) 
+- and aso parameter descriptions (Google, Numpy and Spihnx notations are supported for now)
+
+- by default the docstring format is automatically resolved, but setting the format of the docstring can speed things up a bit.
+        -  `auto` (default): the format is automatically inferred from the docstring
+        -  `google`: the docstring is parsed as markdown (see [Google docstring format](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html))
+        -  `numpy`: the docstring is parsed as markdown (see [Numpy docstring format](https://numpydoc.readthedocs.io/en/latest/format.html))
+        -  `sphinx`: the docstring is parsed as sphinx format (see [Sphinx docstring format](https://sphinx-rtd-tutorial.readthedocs.io/en/latest/docstrings.html))
+
+
+To annotate an *"enum"* like argument, you can use this "typescript" like format: `["value_a" | "value_b"]` ... if will be parsed out.
+This text will be a part of a description too... if you dont want it, you can use this notation as a type notation. 
+Example:
+```
+Args:
+    message_type (["email" | "sms"]): type of a message  / channel how to send the message
+        
+```
+
+
+Then you pass these functions as arguments to and  `@llm_prompt` (the argument must be named `functions` ‼️)
+here you can pass any @llm_function there or a native LangChain tool 
+
+
+here is how to use it:
+
+```python
+from langchain.agents import load_tools
+from langchian_decorators import llm_function, llm_prompt, GlobalSettings
+
+@llm_function
+def send_message(message:str, addressee:str=None, message_type:str="email"):
+    """ Use this if user asks to send some message
+
+    Args:
+        message (str): message text to send
+        addressee (str): email of the adressese... in format firstName.lastName@company.com
+        message_type (str, optional): enum: ["email"|"whatsapp"]
+    """
+
+    if message_type=="email":
+        send_email(addressee, message)
+    elif message_type=="whatsapp":
+        send_whatsapp(addressee, message)
+        
+
+# load some other tools from langchain
+list_of_other_tools = load_tools(
+    tool_names=[...], 
+    llm=GlobalSettings.get_current_settings().default_llm)
+
+@llm_prompt
+def do_what_user_asks_for(user_input:str, functions:List[Union[Callable,BaseTool]]):
+    """ 
+    ``` <prompt:system>
+    Your role is to be a helpfull asistant.
+    ```
+    ``` <prompt:user>
+    {user_input}
+    ```
+    """
+
+user_input="Yo, send an email to John Smith that I will be late for the meeting"
+result = do_what_user_asks_for(
+        user_input=user_input, 
+        functions=[send_message, *list_of_other_tools]
+    )
+
+if result.is_function_call:
+    result.execute()
+else:
+    print(result.output_text)
+
+```
+
+
+If you use functions argument, the output will be always `OutputWithFunctionCall`
+
+``` python
+class OutputWithFunctionCall(BaseModel):
+    output_text:str
+    output:T
+    function_name:str =None
+    function_arguments:Union[Dict[str,Any],str,None]
+    function:Callable = None
+    function_async:Callable = None
+    
+    @property
+    def is_function_call(self):
+        ...
+    
+    @property
+    def support_async(self):
+        ...
+    
+    @property
+    def support_sync(self):
+        ...
+
+    async def execute_async(self):
+       """Executes the function asynchronously."""
+       ...
+        
+    def execute(self):
+        """ Executes the function synchronously. 
+        If the function is async, it will be executed in a event loop.
+        """
+        ...
+```
+
+If you want to see how to schema has been build, you can use `get_function_schema` method that is added to the function by the decorator:
+```python
+@llm_function
+def my_func(arg1:str):
+    ...
+
+print(my_func.get_function_schema())
+
+```
+
+
+# Defining other parameters
+Here we are just marking a function as a prompt with `llm_prompt` decorator, turning it effectively into a LLMChain. Instead of running it 
+
+
+Standard LLMchain takes much more init parameter than just inputs_variables and prompt... here is this implementation detail hidden in the decorator.
+Here is how it works:
+
+1. Using **Global settings**:
+
+``` python
+# define global settings for all prompty (if not set - chatGPT is the current default)
+from langchain_decorators import GlobalSettings
+
+GlobalSettings.define_settings(
+    default_llm=ChatOpenAI(temperature=0.0), this is default... can change it here globally
+    default_streaming_llm=ChatOpenAI(temperature=0.0,streaming=True), this is default... can change it here for all ... will be used for streaming
+)
+```
+
+2. Using predefined **prompt types**
+
+``` python
+#You can change the default prompt types
+from langchain_decorators import PromptTypes, PromptTypeSettings
+
+PromptTypes.AGENT_REASONING.llm = ChatOpenAI()
+
+# Or you can just define your own ones:
+class MyCustomPromptTypes(PromptTypes):
+    GPT4=PromptTypeSettings(llm=ChatOpenAI(model="gpt-4"))
+
+@llm_prompt(prompt_type=MyCustomPromptTypes.GPT4) 
+def write_a_complicated_code(app_idea:str)->str:
+    ...
+
+```
+
+3.  Define the settings **directly in the decorator**
+
+``` python
+from langchain.llms import OpenAI
+
+@llm_prompt(
+    llm=OpenAI(temperature=0.7),
+    stop_tokens=["\nObservation"],
+    ...
+    )
+def creative_writer(book_title:str)->str:
+    ...
+```
+
+## Passing a memory and/or callbacks:
+
+To pass any of these, just declare them in the function (or use kwargs to pass anything)
+
+```python
+
+@llm_prompt()
+async def write_me_short_post(topic:str, platform:str="twitter", memory:SimpleMemory = None):
+    """
+    {history_key}
+    Write me a short header for my post about {topic} for {platform} platform. 
+    It should be for {audience} audience.
+    (Max 15 words)
+    """
+    pass
+
+await write_me_short_post(topic="old movies")
+
+```
+
+# Simplified streaming
+
+If we wan't to leverage streaming:
+ - we need to define prompt as async function 
+ - turn on the streaming on the decorator, or we can define PromptType with streaming on
+ - capture the stream using StreamingContext
+
+This way we just mark which prompt should be streamed, not needing to tinker with what LLM should we use, passing around the creating and distribute streaming handler into particular part of our chain... just turn the streaming on/off on prompt/prompt type...
+
+The streaming will happen only if we call it in streaming context ... there we can define a simple function to handle the stream
+
+``` python
+# this code example is complete and should run as it is
+
+from langchain_decorators import StreamingContext, llm_prompt
+
+# this will mark the prompt for streaming (useful if we want stream just some prompts in our app... but don't want to pass distribute the callback handlers)
+# note that only async functions can be streamed (will get an error if it's not)
+@llm_prompt(capture_stream=True) 
+async def write_me_short_post(topic:str, platform:str="twitter", audience:str = "developers"):
+    """
+    Write me a short header for my post about {topic} for {platform} platform. 
+    It should be for {audience} audience.
+    (Max 15 words)
+    """
+    pass
+
+
+
+# just an arbitrary  function to demonstrate the streaming... wil be some websockets code in the real world
+tokens=[]
+def capture_stream_func(new_token:str):
+    tokens.append(new_token)
+
+# if we want to capture the stream, we need to wrap the execution into StreamingContext... 
+# this will allow us to capture the stream even if the prompt call is hidden inside higher level method
+# only the prompts marked with capture_stream will be captured here
+with StreamingContext(stream_to_stdout=True, callback=capture_stream_func):
+    result = await run_prompt()
+    print("Stream finished ... we can distinguish tokens thanks to alternating colors")
+
+
+print("\nWe've captured",len(tokens),"tokens🎉\n")
+print("Here is the result:")
+print(result)
+```
+
+
 ## More complex structures
 
 for dict / pydantic you need to specify the formatting instructions... 
-this can be tedious, that's why you can let the output parser gegnerate you the instructions based on the model (pydantic)
+this can be tedious, that's why you can let the output parser generate you the instructions based on the model (pydantic)
 
 ``` python
 from langchain_decorators import llm_prompt
 from pydantic import BaseModel, Field
 
 
 class TheOutputStructureWeExpect(BaseModel):
@@ -380,8 +495,8 @@
 
 # Contributing
 feedback, contributions and PR are welcomed 🙏
 
 
 # Others
 - this project is dependant on [langchain](https://github.com/hwchase17/langchain) (obviously) 
-- as well as on promptwatch [promptwatch](https://github.com/blip-solutions/promptwatch-client), which make it easy to track and store to logs, track changes in prompts and compare them by running unit tests over the prompts... 
+- as well as on promptwatch [promptwatch](https://github.com/blip-solutions/promptwatch-client), which make it easy to track and store to logs, track changes in prompts and compare them by running unit tests over the prompts...
```

### Comparing `langchain-decorators-0.0.4/src/langchain_decorators.egg-info/SOURCES.txt` & `langchain-decorators-0.0.6/src/langchain_decorators.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/langchain_decorators/__init__.py
+src/langchain_decorators/chains.py
 src/langchain_decorators/common.py
+src/langchain_decorators/function_decorator.py
 src/langchain_decorators/output_parsers.py
 src/langchain_decorators/prompt_decorator.py
 src/langchain_decorators/prompt_template.py
 src/langchain_decorators/pydantic_helpers.py
+src/langchain_decorators/schema.py
 src/langchain_decorators/streaming_context.py
 src/langchain_decorators.egg-info/PKG-INFO
 src/langchain_decorators.egg-info/SOURCES.txt
 src/langchain_decorators.egg-info/dependency_links.txt
 src/langchain_decorators.egg-info/not-zip-safe
 src/langchain_decorators.egg-info/requires.txt
 src/langchain_decorators.egg-info/top_level.txt
```

