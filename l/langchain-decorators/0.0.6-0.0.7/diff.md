# Comparing `tmp/langchain-decorators-0.0.6.tar.gz` & `tmp/langchain-decorators-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-decorators-0.0.6.tar", last modified: Thu Jun 15 09:31:18 2023, max compression
+gzip compressed data, was "langchain-decorators-0.0.7.tar", last modified: Thu Jun 15 13:37:39 2023, max compression
```

## Comparing `langchain-decorators-0.0.6.tar` & `langchain-decorators-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-15 09:31:18.770719 langchain-decorators-0.0.6/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1066 2023-06-09 22:30:45.000000 langchain-decorators-0.0.6/LICENSE
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    16608 2023-06-15 09:31:18.769936 langchain-decorators-0.0.6/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    16253 2023-06-14 19:55:04.000000 langchain-decorators-0.0.6/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 langchain-decorators-0.0.6/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-06-15 09:31:18.770787 langchain-decorators-0.0.6/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1117 2023-06-11 12:35:54.000000 langchain-decorators-0.0.6/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-15 09:31:18.760443 langchain-decorators-0.0.6/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-15 09:31:18.767055 langchain-decorators-0.0.6/src/langchain_decorators/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      301 2023-06-15 09:29:15.000000 langchain-decorators-0.0.6/src/langchain_decorators/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5901 2023-06-14 10:52:58.000000 langchain-decorators-0.0.6/src/langchain_decorators/chains.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     6371 2023-06-15 08:38:34.000000 langchain-decorators-0.0.6/src/langchain_decorators/common.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    12845 2023-06-14 19:44:20.000000 langchain-decorators-0.0.6/src/langchain_decorators/function_decorator.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    17436 2023-06-13 08:10:19.000000 langchain-decorators-0.0.6/src/langchain_decorators/output_parsers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    19850 2023-06-15 06:53:25.000000 langchain-decorators-0.0.6/src/langchain_decorators/prompt_decorator.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    15009 2023-06-14 00:48:45.000000 langchain-decorators-0.0.6/src/langchain_decorators/prompt_template.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2572 2023-06-11 18:59:03.000000 langchain-decorators-0.0.6/src/langchain_decorators/pydantic_helpers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2088 2023-06-14 14:15:48.000000 langchain-decorators-0.0.6/src/langchain_decorators/schema.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1466 2023-06-11 11:09:42.000000 langchain-decorators-0.0.6/src/langchain_decorators/streaming_context.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-15 09:31:18.769645 langchain-decorators-0.0.6/src/langchain_decorators.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    16608 2023-06-15 09:31:18.000000 langchain-decorators-0.0.6/src/langchain_decorators.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      739 2023-06-15 09:31:18.000000 langchain-decorators-0.0.6/src/langchain_decorators.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-15 09:31:18.000000 langchain-decorators-0.0.6/src/langchain_decorators.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-08 20:09:02.000000 langchain-decorators-0.0.6/src/langchain_decorators.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       22 2023-06-15 09:31:18.000000 langchain-decorators-0.0.6/src/langchain_decorators.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       21 2023-06-15 09:31:18.000000 langchain-decorators-0.0.6/src/langchain_decorators.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-15 13:37:39.090661 langchain-decorators-0.0.7/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1066 2023-06-09 22:30:45.000000 langchain-decorators-0.0.7/LICENSE
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    16608 2023-06-15 13:37:39.090448 langchain-decorators-0.0.7/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    16253 2023-06-14 19:55:04.000000 langchain-decorators-0.0.7/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 langchain-decorators-0.0.7/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-06-15 13:37:39.090714 langchain-decorators-0.0.7/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1117 2023-06-11 12:35:54.000000 langchain-decorators-0.0.7/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-15 13:37:39.083658 langchain-decorators-0.0.7/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-15 13:37:39.088773 langchain-decorators-0.0.7/src/langchain_decorators/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      301 2023-06-15 13:37:22.000000 langchain-decorators-0.0.7/src/langchain_decorators/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5927 2023-06-15 12:29:03.000000 langchain-decorators-0.0.7/src/langchain_decorators/chains.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     7347 2023-06-15 12:40:52.000000 langchain-decorators-0.0.7/src/langchain_decorators/common.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13112 2023-06-15 12:37:50.000000 langchain-decorators-0.0.7/src/langchain_decorators/function_decorator.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    17436 2023-06-13 08:10:19.000000 langchain-decorators-0.0.7/src/langchain_decorators/output_parsers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    20072 2023-06-15 12:48:53.000000 langchain-decorators-0.0.7/src/langchain_decorators/prompt_decorator.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    15009 2023-06-14 00:48:45.000000 langchain-decorators-0.0.7/src/langchain_decorators/prompt_template.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2572 2023-06-11 18:59:03.000000 langchain-decorators-0.0.7/src/langchain_decorators/pydantic_helpers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2088 2023-06-14 14:15:48.000000 langchain-decorators-0.0.7/src/langchain_decorators/schema.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1624 2023-06-15 12:53:20.000000 langchain-decorators-0.0.7/src/langchain_decorators/streaming_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-15 13:37:39.090169 langchain-decorators-0.0.7/src/langchain_decorators.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    16608 2023-06-15 13:37:39.000000 langchain-decorators-0.0.7/src/langchain_decorators.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      739 2023-06-15 13:37:39.000000 langchain-decorators-0.0.7/src/langchain_decorators.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-15 13:37:39.000000 langchain-decorators-0.0.7/src/langchain_decorators.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-08 20:09:02.000000 langchain-decorators-0.0.7/src/langchain_decorators.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       22 2023-06-15 13:37:39.000000 langchain-decorators-0.0.7/src/langchain_decorators.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       21 2023-06-15 13:37:39.000000 langchain-decorators-0.0.7/src/langchain_decorators.egg-info/top_level.txt
```

### Comparing `langchain-decorators-0.0.6/LICENSE` & `langchain-decorators-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.6/PKG-INFO` & `langchain-decorators-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-decorators
-Version: 0.0.6
+Version: 0.0.7
 Summary: syntactic sugar for langchain
 Home-page: https://github.com/ju-bezdek/langchain-decorators
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: langchain
 Requires-Python: >=3.9
```

### Comparing `langchain-decorators-0.0.6/README.md` & `langchain-decorators-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.6/setup.py` & `langchain-decorators-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.6/src/langchain_decorators/chains.py` & `langchain-decorators-0.0.7/src/langchain_decorators/chains.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,17 +98,17 @@
         prompts, stop = await self.aprep_prompts(input_list, run_manager=run_manager)
         
     
         if self.functions:
             chat_model:BaseChatModel=self.llm
             if len(prompts)!=1:
                 raise ValueError("Only one prompt is supported when using functions")
-            messages = prompts[0].to_messages()
+            messages = [prompt.to_messages() for prompt in prompts]
              
-            return  chat_model.agenerate(messages=messages, 
+            return  await chat_model.agenerate(messages=messages, 
                                          stop=stop, callbacks=run_manager.get_child() if run_manager else None,
                                          functions=self.function_schemas)
         else:
             return await self.llm.agenerate_prompt(
                 prompts, stop, callbacks=run_manager.get_child() if run_manager else None
             )
```

### Comparing `langchain-decorators-0.0.6/src/langchain_decorators/common.py` & `langchain-decorators-0.0.7/src/langchain_decorators/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from ast import Tuple
 import inspect
 import logging
 from textwrap import dedent
 import yaml
 from enum import Enum
-from typing import Any, Coroutine, Dict, Union, Optional
+from typing import Any, Coroutine, Dict, Union, Optional, get_origin
 from pydantic import BaseConfig, BaseModel, Extra
 from pydantic.fields import ModelField
 from langchain.llms.base import BaseLanguageModel
 from langchain.chat_models import ChatOpenAI
-
+from typing_inspect import is_generic_type, is_union_type
 
 class GlobalSettings(BaseModel):
     default_llm: Optional[BaseLanguageModel] = None
     default_streaming_llm: Optional[BaseLanguageModel] = None
     logging_level: int = logging.INFO
     stdout_logging: bool = True
 
@@ -120,25 +120,43 @@
     FINAL_OUTPUT: PromptTypeSettings = PromptTypeSettings(
         color=LogColors.YELLOW, log_level=logging.INFO)
 
 
 def get_func_return_type(func: callable)->Tuple:
     return_type = func.__annotations__.get("return",None)
     if inspect.iscoroutinefunction(func):
-        if return_type and issubclass(return_type, Coroutine):
-            return_type_args = getattr(return_type, '__args__', None)
-            if return_type_args and len(return_type_args) == 3:
-                return_type = return_type_args[2]
+        if return_type:
+            if is_generic_type(return_type):
+                return_type_origin = get_origin(return_type)
+                if issubclass(return_type_origin, Coroutine):
+                    return_type_args = getattr(return_type, '__args__', None)
+                    if return_type_args and len(return_type_args) == 3:
+                        return return_type_args[2]
+                    else:
+                        raise Exception(f"Invalid Coroutine annotation {return_type}. Expected Coroutine[ any , any, <return_type>] or just <return_type>")
+                else:
+                    return return_type_origin
+            elif is_union_type(return_type):
+                return_type_args = getattr(return_type, '__args__', None)
+                if return_type_args and len(return_type_args) == 2 and return_type_args[1] == type(None):
+                    return return_type_args[0]
+                else:
+                    raise Exception(f"Invalid Union annotation {return_type}. Expected Union[ <return_type>, None] or just <return_type>")
             else:
-                raise Exception(f"Invalid Coroutine annotation {return_type}. Expected Coroutine[ any , any, <return_type>] or just <return_type>")
-        else:
-            return return_type
+                
+                if issubclass(return_type, Coroutine):
+                    return None
+                else:
+                    return return_type
+            
             
 def get_function_docs(func: callable)->Tuple:
-    fist_line, rest = func.__doc__.split('\n', 1)
+    if not func.__doc__:
+        return None
+    fist_line, rest = func.__doc__.split('\n', 1) if '\n' in func.__doc__ else (func.__doc__, "")
     # we dedent the first line separately,because its common that it often starts right after """
     fist_line = fist_line.strip()
     if fist_line:
         fist_line+="\n"
     docs = fist_line + dedent(rest)
     return docs
```

### Comparing `langchain-decorators-0.0.6/src/langchain_decorators/function_decorator.py` & `langchain-decorators-0.0.7/src/langchain_decorators/function_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,41 +144,42 @@
             args_schema =  first_param.type_.schema()
             args_schema={
                 "type":"object",
                 "properties":args_schema["properties"],
                 "required":args_schema["required"]
             }
     
-    if not args_schema and func_docs:
+    if not args_schema:
         # any other case, that function arguments are not wrapped in pydantic model
-        docsctrings_param_description = find_and_parse_params_from_docstrings(func_docs,format=format)
-        if docsctrings_param_description:
-            if validate_docstrings:
-                documented_params=set(docsctrings_param_description.keys()) 
-                implemented_params= set(arguments_fields.keys())
-                not_implemented = documented_params - implemented_params  # Set difference: keys in set1 but not in set2
-                not_documented = implemented_params - documented_params  # Set difference: keys in set2 but not in set1
-
-                if not_implemented or not_documented:
-                    errs = []
-                    if not_implemented:
-                        errs.append(f"Missing (not implemented): {not_implemented}")
-                    if not_documented:
-                        errs.append(f"Missing (not documented): {not_documented}")
-                     
-                    raise ValueError("Docstrings parameters do not match function signature. "+errs.join(", "))
-            
-            for arg_name, arg_model_field in arguments_fields.items():
-                arg_docs = docsctrings_param_description.get(arg_name)
-                if arg_docs:
-                    
-                    arg_model_field.field_info.description =arg_docs["description"]
-                    enum = parse_enum_from_docstring_param(arg_docs["type"],arg_docs["description"])
-                    if enum:
-                        arg_model_field.field_info.extra["enum"] = enum
+        if func_docs:
+            docsctrings_param_description = find_and_parse_params_from_docstrings(func_docs,format=format)
+            if docsctrings_param_description:
+                if validate_docstrings:
+                    documented_params=set(docsctrings_param_description.keys()) 
+                    implemented_params= set(arguments_fields.keys())
+                    not_implemented = documented_params - implemented_params  # Set difference: keys in set1 but not in set2
+                    not_documented = implemented_params - documented_params  # Set difference: keys in set2 but not in set1
+
+                    if not_implemented or not_documented:
+                        errs = []
+                        if not_implemented:
+                            errs.append(f"Missing (not implemented): {not_implemented}")
+                        if not_documented:
+                            errs.append(f"Missing (not documented): {not_documented}")
+                        
+                        raise ValueError("Docstrings parameters do not match function signature. "+errs.join(", "))
+                
+                for arg_name, arg_model_field in arguments_fields.items():
+                    arg_docs = docsctrings_param_description.get(arg_name)
+                    if arg_docs:
+                        
+                        arg_model_field.field_info.description =arg_docs["description"]
+                        enum = parse_enum_from_docstring_param(arg_docs["type"],arg_docs["description"])
+                        if enum:
+                            arg_model_field.field_info.extra["enum"] = enum
 
         args_schema={
             "type":"object",
             "properties":{},
             "required":[]
 
         }
@@ -196,17 +197,20 @@
     def pop_prop_title(schema):
         #title is autogenerated by pydantic and will just costs us tokens....
         if "title" in schema:
             del schema["title"]
         return schema
     args_schema["properties"] = {prop:pop_prop_title(prop_schema) for prop, prop_schema in args_schema["properties"].items()}
     
+    description = parse_function_description_from_docstrings(func_docs) if func_docs else None
+    if not description:
+        raise ValueError(f"LLM Function {func_name} has no description in docstrings")
     return {
         "name":func_name,
-        "description":parse_function_description_from_docstrings(func_docs),
+        "description":description,
         "parameters":args_schema
     }
```

### Comparing `langchain-decorators-0.0.6/src/langchain_decorators/output_parsers.py` & `langchain-decorators-0.0.7/src/langchain_decorators/output_parsers.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.6/src/langchain_decorators/prompt_decorator.py` & `langchain-decorators-0.0.7/src/langchain_decorators/prompt_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 
+from calendar import c
+from gc import callbacks
 import logging
 import inspect
 
 from functools import wraps
 from textwrap import dedent
 from typing import Callable, List, Optional, Sequence, Union
 
@@ -110,40 +112,42 @@
 
         
 
         if prompt_type:
             _capture_stream = prompt_type.capture_stream if capture_stream is None else capture_stream
         else:
             _capture_stream = capture_stream
-        if _capture_stream:
-
-            if not is_async:
-                print_log(f"Warning: capture_stream=True is only supported for async functions. Ignoring capture_stream for {full_name}", logging.WARNING, LogColors.YELLOW)
-                _capture_stream=False
-            else:
-                if not StreamingContext.get_context():
-                    print_log(f"Debug: Not inside StreamingContext. Ignoring capture_stream for {full_name}", logging.DEBUG, LogColors.DARK_GRAY)
-                    _capture_stream=False
+        if _capture_stream and not is_async:
+            print_log(f"Warning: capture_stream=True is only supported for async functions. Ignoring capture_stream for {full_name}", logging.WARNING, LogColors.YELLOW)
+            _capture_stream=False
+            
+                
                 
        
 
         def prepare_call_args(*args, **kwargs):
             global_settings = GlobalSettings.get_current_settings()
+
+            if not StreamingContext.get_context():
+                print_log(f"INFO: Not inside StreamingContext. Ignoring capture_stream for {full_name}", logging.DEBUG, LogColors.WHITE)
+                capture_stream=False
+            else:
+                capture_stream=_capture_stream
            
             if not llm:
-                if _capture_stream:
+                if capture_stream:
                     if not global_settings.default_streaming_llm:
                         print_log(f"Warning: capture_stream on {name} is on, but the default LLM {llm} doesn't seem to be supporting streaming.", logging.WARNING, LogColors.YELLOW)
                         
                     prompt_llm=global_settings.default_streaming_llm or global_settings.default_llm
                 else:
                     prompt_llm = global_settings.default_llm
             else:
                 prompt_llm=llm
-                if _capture_stream:
+                if capture_stream:
                     if  hasattr(llm,"streaming"):
                         if not getattr(llm, "streaming"):
                             print_log(f"Warning: capture_stream on {name} is on, but the provided LLM {llm} doesn't have streaming on! Stream wont be captured", logging.WARNING, LogColors.YELLOW)
                     else:
                         print_log(f"Warning: capture_stream on {name} is on, but the provided LLM {llm} doesn't seem to be supporting streaming.", logging.WARNING, LogColors.YELLOW)
                    
                 
@@ -152,51 +156,53 @@
             if len(args)==1 and hasattr(args[0],"__dict__"):
                 # is a proper object
                 input_variables_source = args[0]
 
             elif len(args)>1:
                 raise Exception(f"Positional arguments are not supported for prompt functions. Only one positional argument as an object with attributes as a source of inputs is supported. Got: {args}")
             
-            if _capture_stream:
-                if "callbacks" in kwargs:
-                    kwargs["callbacks"].append(StreamingContext.StreamingContextCallback())
-                else:
-                    kwargs["callbacks"] = [StreamingContext.StreamingContextCallback()]
-
-            if "memory" in kwargs:
-                memory = kwargs.pop("memory")
-            else:
-                memory=None
-
-            if "functions" in kwargs:
-                functions=kwargs.pop("functions")
-            else:
-                functions=None
-
-
-
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
 
+            if "callbacks" in kwargs:
+                callbacks=kwargs.pop("callbacks")
+            else:
+                callbacks=[]
+            
+            if capture_stream:
+                callbacks.append(StreamingContext.StreamingContextCallback())
+            
+
+            if "memory" in kwargs:
+                memory = kwargs.pop("memory")
+            else:
+                memory=None
+
+            if "functions" in kwargs:
+                functions=kwargs.pop("functions")
+            else:
+                functions=None
+                
             if functions:
                 llmChain = LLMChainWithFunctionSupport(llm=prompt_llm, prompt=prompt_template,  memory=memory, functions=functions)
             else:
                 llmChain = LLMChain(llm=prompt_llm, prompt=prompt_template,  memory=memory)
             other_supported_kwargs={"stop","callbacks"}
             unexpected_inputs = [key for key in kwargs if key not in prompt_template.input_variables and key not in other_supported_kwargs ]
             if unexpected_inputs:
-                raise TypeError(f"Unexpected inputs for prompt function {full_name}: {unexpected_inputs}. \nValid inputs are: {prompt_template.input_variables}")
+                raise TypeError(f"Unexpected inputs for prompt function {full_name}: {unexpected_inputs}. \nValid inputs are: {prompt_template.input_variables}\nHint: Make sure that you've used all the inputs in the template")
             
             missing_inputs = [key for key in prompt_template.input_variables if key not in kwargs ]
             if format_instructions_parameter_key in missing_inputs:
                 missing_inputs.remove(format_instructions_parameter_key)
                 kwargs[format_instructions_parameter_key]=None #init the format instructions with None... will be filled later
             if memory and memory.memory_key in missing_inputs:
                 missing_inputs.remove(memory.memory_key)
@@ -212,18 +218,18 @@
                             kwargs[key] = value
 
 
                         
                 else:
                     raise TypeError(f"{full_name}: missing 1 required keyword-only argument: {missing_inputs}")
                 
-
+            
             if stop_tokens:
                 kwargs["stop"]=stop_tokens
-            call_args = {"inputs":kwargs, "return_only_outputs":True}
+            call_args = {"inputs":kwargs, "return_only_outputs":True, "callbacks":callbacks}
             return llmChain, call_args
         
         def get_retry_parse_call_args(prompt_template:PromptDecoratorTemplate, exception:OutputParserExceptionWithOriginal, get_original_prompt:Callable):
             logging.warning(msg=f"Failed to parse output for {full_name}: {exception}\nRetrying...")
             if format_instructions_parameter_key not in prompt_str:
                 logging.warning(f"Please note that we didn't find a {format_instructions_parameter_key} parameter in the prompt string. If you don't include it in your prompt template, you need to provide your custom formatting instructions.")    
             if exception.original_prompt_needed_on_retry:
@@ -288,15 +294,15 @@
         else:
             @wraps(func)
             async def async_wrapper(*args, **kwargs):
                 
                 
                 print_log(log_object=f"> Entering {name} prompt decorator chain", log_level=prompt_type.log_level if prompt_type else logging.DEBUG,color=LogColors.WHITE_BOLD)
                 llmChain, chain_args = prepare_call_args(*args, **kwargs)
-
+                
                 try:
                     
                     result_data = await llmChain.acall(**chain_args)
                     result = result_data[llmChain.output_key]
                     is_function_call = result_data.get("function_call_info")
                     result = process_results(llmChain, result_data, result,is_function_call)
```

### Comparing `langchain-decorators-0.0.6/src/langchain_decorators/prompt_template.py` & `langchain-decorators-0.0.7/src/langchain_decorators/prompt_template.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.6/src/langchain_decorators/pydantic_helpers.py` & `langchain-decorators-0.0.7/src/langchain_decorators/pydantic_helpers.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.6/src/langchain_decorators/schema.py` & `langchain-decorators-0.0.7/src/langchain_decorators/schema.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.6/src/langchain_decorators/streaming_context.py` & `langchain-decorators-0.0.7/src/langchain_decorators/streaming_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,21 +23,25 @@
         self.token_colors = ['\033[90m', '\033[0m']
 
     def __enter__(self):
         self.__class__.context_var.set(self)
 
     @classmethod
     def get_context(cls) -> 'StreamingContext':
-        return cls.context_var.get("streaming_context")
+        return cls.context_var.get(None)
 
     def on_new_token(self, token: str):
-        if self.callback:
-            self.callback(token)
-        if self.stream_to_stdout:
-            reset_color = '\033[0m'
-            current_color = self.token_colors[0]
-            self.token_colors.reverse()
-            print('{}{}{}'.format(current_color, token if token !=
-                  "" else '\u2022', reset_color), end='')
+        if token:
+            if self.callback:
+                self.callback(token)
+            if self.stream_to_stdout:
+                reset_color = '\033[0m'
+                if token.strip() and token!="\n":
+                    current_color = self.token_colors[0]
+                    self.token_colors.reverse()
+                else:
+                    current_color='\033[40m'
+                print('{}{}{}'.format(current_color, token if token !=
+                    "" else '\u2022', reset_color), end='')
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.context_var.set(None)
```

### Comparing `langchain-decorators-0.0.6/src/langchain_decorators.egg-info/PKG-INFO` & `langchain-decorators-0.0.7/src/langchain_decorators.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-decorators
-Version: 0.0.6
+Version: 0.0.7
 Summary: syntactic sugar for langchain
 Home-page: https://github.com/ju-bezdek/langchain-decorators
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: langchain
 Requires-Python: >=3.9
```

### Comparing `langchain-decorators-0.0.6/src/langchain_decorators.egg-info/SOURCES.txt` & `langchain-decorators-0.0.7/src/langchain_decorators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

