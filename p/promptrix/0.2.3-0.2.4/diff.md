# Comparing `tmp/promptrix-0.2.3.tar.gz` & `tmp/promptrix-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptrix-0.2.3.tar", last modified: Wed Jun 14 15:57:19 2023, max compression
+gzip compressed data, was "promptrix-0.2.4.tar", last modified: Thu Jun 15 20:06:44 2023, max compression
```

## Comparing `promptrix-0.2.3.tar` & `promptrix-0.2.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 15:57:19.440941 promptrix-0.2.3/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-01 23:37:06.000000 promptrix-0.2.3/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2225 2023-06-14 15:57:19.440941 promptrix-0.2.3/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1655 2023-06-14 03:06:34.000000 promptrix-0.2.3/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      777 2023-06-14 15:57:13.000000 promptrix-0.2.3/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-14 15:57:19.440941 promptrix-0.2.3/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 15:57:19.436941 promptrix-0.2.3/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 15:57:19.440941 promptrix-0.2.3/src/promptrix/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      763 2023-06-12 20:40:27.000000 promptrix-0.2.3/src/promptrix/AssistantMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2571 2023-06-08 00:11:30.000000 promptrix-0.2.3/src/promptrix/ConversationHistory.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1164 2023-06-05 23:10:10.000000 promptrix-0.2.3/src/promptrix/FunctionRegistry.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      679 2023-06-12 20:15:31.000000 promptrix-0.2.3/src/promptrix/GPT3Tokenizer.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1181 2023-06-09 04:09:26.000000 promptrix-0.2.3/src/promptrix/GroupSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5159 2023-06-13 18:46:29.000000 promptrix-0.2.3/src/promptrix/LayoutEngine.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      421 2023-06-02 18:46:08.000000 promptrix-0.2.3/src/promptrix/Prompt.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2491 2023-06-12 21:39:17.000000 promptrix-0.2.3/src/promptrix/PromptSectionBase.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      475 2023-06-02 18:46:08.000000 promptrix-0.2.3/src/promptrix/SystemMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5351 2023-06-12 21:38:53.000000 promptrix-0.2.3/src/promptrix/TemplateSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      821 2023-06-02 18:46:08.000000 promptrix-0.2.3/src/promptrix/TextSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      640 2023-06-12 20:39:59.000000 promptrix-0.2.3/src/promptrix/UserMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      985 2023-06-08 00:11:43.000000 promptrix-0.2.3/src/promptrix/Utilities.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      936 2023-06-02 18:46:08.000000 promptrix-0.2.3/src/promptrix/VolatileMemory.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:55.000000 promptrix-0.2.3/src/promptrix/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1494 2023-06-02 18:46:08.000000 promptrix-0.2.3/src/promptrix/promptrixTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 15:57:19.440941 promptrix-0.2.3/src/promptrix.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2225 2023-06-14 15:57:19.000000 promptrix-0.2.3/src/promptrix.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      710 2023-06-14 15:57:19.000000 promptrix-0.2.3/src/promptrix.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-14 15:57:19.000000 promptrix-0.2.3/src/promptrix.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       71 2023-06-14 15:57:19.000000 promptrix-0.2.3/src/promptrix.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-06-14 15:57:19.000000 promptrix-0.2.3/src/promptrix.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-15 20:06:44.845356 promptrix-0.2.4/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-01 23:37:06.000000 promptrix-0.2.4/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2225 2023-06-15 20:06:44.845356 promptrix-0.2.4/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1655 2023-06-14 03:06:34.000000 promptrix-0.2.4/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      777 2023-06-15 20:06:35.000000 promptrix-0.2.4/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-15 20:06:44.845356 promptrix-0.2.4/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-15 20:06:44.841356 promptrix-0.2.4/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-15 20:06:44.845356 promptrix-0.2.4/src/promptrix/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      763 2023-06-12 20:40:27.000000 promptrix-0.2.4/src/promptrix/AssistantMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2900 2023-06-15 03:37:36.000000 promptrix-0.2.4/src/promptrix/ConversationHistory.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1164 2023-06-05 23:10:10.000000 promptrix-0.2.4/src/promptrix/FunctionRegistry.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      607 2023-06-14 17:33:19.000000 promptrix-0.2.4/src/promptrix/GPT3Tokenizer.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1187 2023-06-15 17:06:46.000000 promptrix-0.2.4/src/promptrix/GroupSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5159 2023-06-15 17:06:10.000000 promptrix-0.2.4/src/promptrix/LayoutEngine.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      421 2023-06-02 18:46:08.000000 promptrix-0.2.4/src/promptrix/Prompt.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2445 2023-06-15 17:06:28.000000 promptrix-0.2.4/src/promptrix/PromptSectionBase.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      475 2023-06-02 18:46:08.000000 promptrix-0.2.4/src/promptrix/SystemMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5738 2023-06-14 19:26:14.000000 promptrix-0.2.4/src/promptrix/TemplateSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      821 2023-06-02 18:46:08.000000 promptrix-0.2.4/src/promptrix/TextSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      636 2023-06-14 17:01:45.000000 promptrix-0.2.4/src/promptrix/UserMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      985 2023-06-14 19:25:22.000000 promptrix-0.2.4/src/promptrix/Utilities.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      936 2023-06-14 20:55:08.000000 promptrix-0.2.4/src/promptrix/VolatileMemory.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:55.000000 promptrix-0.2.4/src/promptrix/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1494 2023-06-02 18:46:08.000000 promptrix-0.2.4/src/promptrix/promptrixTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-15 20:06:44.845356 promptrix-0.2.4/src/promptrix.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2225 2023-06-15 20:06:44.000000 promptrix-0.2.4/src/promptrix.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      710 2023-06-15 20:06:44.000000 promptrix-0.2.4/src/promptrix.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-15 20:06:44.000000 promptrix-0.2.4/src/promptrix.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       71 2023-06-15 20:06:44.000000 promptrix-0.2.4/src/promptrix.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-06-15 20:06:44.000000 promptrix-0.2.4/src/promptrix.egg-info/top_level.txt
```

### Comparing `promptrix-0.2.3/LICENSE` & `promptrix-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.3/PKG-INFO` & `promptrix-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptrix
-Version: 0.2.3
+Version: 0.2.4
 Summary: Promptrix. A prompt layout manager for LLMs
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://github.com/Stevenic/promptrix-py
 Project-URL: Bug Tracker, https://github.com/Stevenic/promptrix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `promptrix-0.2.3/README.md` & `promptrix-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.3/pyproject.toml` & `promptrix-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "promptrix"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "Promptrix. A prompt layout manager for LLMs"
```

### Comparing `promptrix-0.2.3/src/promptrix/AssistantMessage.py` & `promptrix-0.2.4/src/promptrix/AssistantMessage.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.3/src/promptrix/ConversationHistory.py` & `promptrix-0.2.4/src/promptrix/ConversationHistory.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
         self.variable = variable
         self.userPrefix = userPrefix
         self.assistantPrefix = assistantPrefix
 
     async def renderAsText(self, memory, functions, tokenizer, maxTokens):
         history = memory.get(self.variable)
         if history is None: history=[]
+        #print(f'*****ConversationHistory renderAsText {len(history)}')
         tokens = 0
         budget = min(self.tokens, maxTokens) if self.tokens > 1.0 else maxTokens
         separatorLength = len(tokenizer.encode(self.separator))
         lines = []
         for i in range(len(history)-1, -1, -1):
             msg = history[i]
             message = Utilities.to_string(tokenizer, msg['content'])
@@ -26,28 +27,32 @@
                 tokens += length
                 lines.insert(0, line)
                 continue
             if tokens + length > budget:
                 break
             tokens += length
             lines.insert(0, line)
+        #print(f'*****ConversationHistory renderAsText exit lines {len(lines)}')
         return RenderedPromptSection(output=self.separator.join(lines), length=tokens, tooLong=tokens > maxTokens)
 
     async def renderAsMessages(self, memory, functions, tokenizer, maxTokens):
         history = memory.get(self.variable)
         if history is None: history = []
+        #print(f'*****ConversationHistory renderAsMessages {len(history)}')
         tokens = 0
         budget = min(self.tokens, maxTokens) if self.tokens > 1.0 else maxTokens
         messages = []
         for i in range(len(history)-1, -1, -1):
             msg = history[i]
-            message = Message(role=msg['role'], content=Utilities.to_string(tokenizer, msg['content']))
-            length = len(tokenizer.encode(message.content))
+            message = {'role':msg['role'], 'content':Utilities.to_string(tokenizer, msg['content'])}
+            length = len(tokenizer.encode(message['content']))
             if len(messages) == 0 and self.required:
                 tokens += length
                 messages.insert(0, message)
                 continue
             if tokens + length > budget:
                 break
             tokens += length
             messages.insert(0, message)
+        #print(f'*****ConversationHistory renderAsMessages exit messages {len(messages)}')
+        
         return RenderedPromptSection(output=messages, length=tokens, tooLong=tokens > maxTokens)
```

### Comparing `promptrix-0.2.3/src/promptrix/FunctionRegistry.py` & `promptrix-0.2.4/src/promptrix/FunctionRegistry.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.3/src/promptrix/GroupSection.py` & `promptrix-0.2.4/src/promptrix/GroupSection.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,12 +8,12 @@
         super().__init__(tokens, required, separator, textPrefix)
         self._layoutEngine = LayoutEngine(sections, tokens, required, separator)
         self.sections = sections
         self.role = role
 
     async def renderAsMessages(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, maxTokens: int):
         # Render sections to text
-        print(f'*****group section entry')
-        output, length, tooLong = await self._layoutEngine.renderAsText(memory, functions, tokenizer, maxTokens)
-        print(f'*****group section exit')
+        renderedPromptSection = await self._layoutEngine.renderAsText(memory, functions, tokenizer, maxTokens)
+        output = renderedPromptSection.output
+        length = renderedPromptSection.length
         # Return output as a single message
-        return self.returnMessages([{'role': self.role, 'content': output}], length, tokenizer, maxTokens)
+        return self.return_messages([{'role': self.role, 'content': output}], length, tokenizer, maxTokens)
```

### Comparing `promptrix-0.2.3/src/promptrix/LayoutEngine.py` & `promptrix-0.2.4/src/promptrix/LayoutEngine.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.3/src/promptrix/PromptSectionBase.py` & `promptrix-0.2.4/src/promptrix/PromptSectionBase.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,35 +17,36 @@
     @abstractmethod
     async def renderAsMessages(self, memory, functions, tokenizer, max_tokens):
         pass
 
     async def renderAsText(self, memory, functions, tokenizer, max_tokens):
         as_messages = await self.renderAsMessages(memory, functions, tokenizer, max_tokens)
         messages = as_messages.output
-        #print(f'***** PromptSectionBase renderAsText messages len {len(messages)}')
-        #print(f"***** PromptSectionBase renderAsText message {messages[0]['content']}")
         text = ''
         for message in messages:
             text += message['content']+'\n'
         #text = self.separator.join([message['content'] for message in messages])
         prefix_length = len(tokenizer.encode(self.text_prefix))
         separator_length = len(tokenizer.encode(self.separator))
         length = prefix_length + as_messages.length + ((len(as_messages.output) - 1) * separator_length)
         text = self.text_prefix + text
         if self.tokens > 1.0 and length > self.tokens:
             encoded = tokenizer.encode(text)
             text = tokenizer.decode(encoded[:self.tokens])
             length = self.tokens
+        if text.endswith('\n'):
+            text = text[:-1]
         return RenderedPromptSection(output=text, length=length, tooLong=length > max_tokens)
 
     def return_messages(self, output, length, tokenizer, max_tokens):
         if self.tokens > 1.0:
             while length > self.tokens:
                 msg = output.pop()
                 encoded = tokenizer.encode(msg['content'])
                 length -= len(encoded)
                 if length < self.tokens:
                     delta = self.tokens - length
                     truncated = tokenizer.decode(encoded[:delta])
-                    output.append(Message(role=msg.role, content=truncated))
+                    role = msg['role'] if type(msg) == dict else msg.role
+                    output.append({'role':role, 'content':truncated})
                     length += delta
         return RenderedPromptSection(output=output, length=length, tooLong=length > max_tokens)
```

### Comparing `promptrix-0.2.3/src/promptrix/TemplateSection.py` & `promptrix-0.2.4/src/promptrix/TemplateSection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 #from promptrixTypes import *
 from promptrix.PromptSectionBase import PromptSectionBase
 from promptrix.Utilities import Utilities
 from typing import List, Callable, Any
 from enum import Enum
 import asyncio
 
+def get_mem_str(memory, value):
+    #print (f'***** TemplateSection create_variable_renderer memory {memory}, value {value}')
+    return value
+
 class ParseState(Enum):
     IN_TEXT = 1
     IN_PARAMETER = 2
     IN_STRING = 3
 
 class TemplateSection(PromptSectionBase):
     def __init__(self, template, role, tokens = -1, required = True, separator='\n', text_prefix = ''):
         super().__init__(tokens, required, separator, text_prefix)
         self.template = template
         self.role = role
         self._parts = []
         self.parse_template()
     
     async def renderAsMessages(self, memory: 'PromptMemory', functions: 'PromptFunctions', tokenizer: 'Tokenizer', max_tokens: int) -> 'RenderedPromptSection[List[Message]]':
+        #print(f'***** TemplateSection entry {self._parts}')
         rendered_parts = [part(memory, functions, tokenizer, max_tokens) for part in self._parts]
         text = ''.join(rendered_parts)
+        #print(f'***** TemplateSection rendered parts {rendered_parts}')
         length = len(tokenizer.encode(text))
         return self.return_messages([{'role': self.role, 'content': text}], length, tokenizer, max_tokens)
 
     """
     async def renderAsMessages(self, memory: 'PromptMemory', functions: 'PromptFunctions', tokenizer: 'Tokenizer', max_tokens: int) -> 'RenderedPromptSection[List[Message]]':
         rendered_parts = await asyncio.gather(*(part(memory, functions, tokenizer, max_tokens) for part in self._parts))
         text = ''.join(rendered_parts)
@@ -71,21 +77,22 @@
                 if char == string_delim:
                     state = ParseState.IN_PARAMETER
         if state != ParseState.IN_TEXT:
             raise ValueError(f"Invalid template: {self.template}")
         if len(part) > 0:
             self._parts.append(self.create_text_renderer(part))
         
-
+        
     def create_text_renderer(self, text: str) -> Callable[['PromptMemory', 'PromptFunctions', 'Tokenizer', int], 'Promise[str]']:
         return lambda memory, functions, tokenizer, max_tokens: text
 
     def create_variable_renderer(self, name: str) -> Callable[['PromptMemory', 'PromptFunctions', 'Tokenizer', int], 'Promise[str]']:
-        return lambda memory, functions, tokenizer, max_tokens: Utilities.to_string(tokenizer, memory.get(name))
-
+        #print (f'***** TemplateSection create_variable_renderer name {name}')
+        return lambda memory, functions, tokenizer, max_tokens: get_mem_str(memory, Utilities.to_string(tokenizer, memory.get(name)))
+ 
     def create_function_renderer(self, param: str) -> Callable[['PromptMemory', 'PromptFunctions', 'Tokenizer', int], 'Promise[str]']:
         name = None
         args = []
         part = ''
         def save_part():
             nonlocal part, name, args
             if len(part) > 0:
```

### Comparing `promptrix-0.2.3/src/promptrix/TextSection.py` & `promptrix-0.2.4/src/promptrix/TextSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.3/src/promptrix/UserMessage.py` & `promptrix-0.2.4/src/promptrix/UserMessage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from promptrix.TemplateSection import TemplateSection
 
 class UserMessage(TemplateSection):
     """
     A user message.
     """
-    def __init__(self, template: str, tokens: int = -1, user_prefix: str = 'user: '):
+    def __init__(self, template: str, tokens: int = -1, user_prefix: str = 'user'):
         """
         Creates a new 'UserMessage' instance.
         :param template: Template to use for this section.
         :param tokens: Optional. Sizing strategy for this section. Defaults to `auto`.
-        :param user_prefix: Optional. Prefix to use for user messages when rendering as text. Defaults to `user: `.
+        :param user_prefix: Optional. Prefix to use for user messages when rendering as text. Defaults to `user`.
         """
         super().__init__(template, user_prefix, tokens, True, '\n', text_prefix = user_prefix)
```

### Comparing `promptrix-0.2.3/src/promptrix/Utilities.py` & `promptrix-0.2.4/src/promptrix/Utilities.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.3/src/promptrix/VolatileMemory.py` & `promptrix-0.2.4/src/promptrix/VolatileMemory.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.3/src/promptrix/promptrixTypes.py` & `promptrix-0.2.4/src/promptrix/promptrixTypes.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.3/src/promptrix.egg-info/PKG-INFO` & `promptrix-0.2.4/src/promptrix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptrix
-Version: 0.2.3
+Version: 0.2.4
 Summary: Promptrix. A prompt layout manager for LLMs
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://github.com/Stevenic/promptrix-py
 Project-URL: Bug Tracker, https://github.com/Stevenic/promptrix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `promptrix-0.2.3/src/promptrix.egg-info/SOURCES.txt` & `promptrix-0.2.4/src/promptrix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

