# Comparing `tmp/chatglm-llm-1.3.4.tar.gz` & `tmp/chatglm-llm-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatglm-llm-1.3.4.tar", last modified: Mon May 15 05:57:40 2023, max compression
+gzip compressed data, was "chatglm-llm-1.3.7.tar", last modified: Thu Jun 15 08:48:43 2023, max compression
```

## Comparing `chatglm-llm-1.3.4.tar` & `chatglm-llm-1.3.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 05:57:40.268688 chatglm-llm-1.3.4/
--rw-rw-rw-   0        0        0       36 2023-05-15 05:51:20.000000 chatglm-llm-1.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0      225 2023-05-15 05:57:40.267680 chatglm-llm-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     1887 2023-05-15 05:51:20.000000 chatglm-llm-1.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 05:57:40.257685 chatglm-llm-1.3.4/chatglm_llm.egg-info/
--rw-rw-rw-   0        0        0      225 2023-05-15 05:57:39.000000 chatglm-llm-1.3.4/chatglm_llm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      480 2023-05-15 05:57:40.000000 chatglm-llm-1.3.4/chatglm_llm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 05:57:39.000000 chatglm-llm-1.3.4/chatglm_llm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-15 05:57:39.000000 chatglm-llm-1.3.4/chatglm_llm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-15 05:57:39.000000 chatglm-llm-1.3.4/chatglm_llm.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      226 2023-05-15 05:57:40.000000 chatglm-llm-1.3.4/chatglm_llm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-15 05:57:40.000000 chatglm-llm-1.3.4/chatglm_llm.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-15 05:57:40.263034 chatglm-llm-1.3.4/chatglm_src/
--rw-rw-rw-   0        0        0      680 2023-05-15 05:51:20.000000 chatglm-llm-1.3.4/chatglm_src/__init__.py
--rw-rw-rw-   0        0        0     4201 2023-05-15 05:51:20.000000 chatglm-llm-1.3.4/chatglm_src/callbacks.py
-drwxrwxrwx   0        0        0        0 2023-05-15 05:57:40.265162 chatglm-llm-1.3.4/chatglm_src/chains/
--rw-rw-rw-   0        0        0       69 2023-05-15 05:51:20.000000 chatglm-llm-1.3.4/chatglm_src/chains/__init__.py
--rw-rw-rw-   0        0        0     4402 2023-05-15 05:51:20.000000 chatglm-llm-1.3.4/chatglm_src/chains/local_qa.py
--rw-rw-rw-   0        0        0      443 2023-05-15 05:51:20.000000 chatglm-llm-1.3.4/chatglm_src/cmd.py
--rw-rw-rw-   0        0        0     3052 2023-05-15 05:51:20.000000 chatglm-llm-1.3.4/chatglm_src/embeding.py
--rw-rw-rw-   0        0        0    24286 2023-05-15 05:53:40.000000 chatglm-llm-1.3.4/chatglm_src/llm.py
-drwxrwxrwx   0        0        0        0 2023-05-15 05:57:40.265908 chatglm-llm-1.3.4/chatglm_src/loader/
--rw-rw-rw-   0        0        0     1403 2023-05-15 05:51:20.000000 chatglm-llm-1.3.4/chatglm_src/loader/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-15 05:57:40.268688 chatglm-llm-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0      997 2023-05-15 05:56:17.000000 chatglm-llm-1.3.4/setup.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-15 08:48:43.362502 chatglm-llm-1.3.7/
+-rw-r--r--   0 mroy       (501) staff       (20)       36 2023-05-10 01:48:15.000000 chatglm-llm-1.3.7/MANIFEST.in
+-rw-r--r--   0 mroy       (501) staff       (20)      212 2023-06-15 08:48:43.362354 chatglm-llm-1.3.7/PKG-INFO
+-rw-r--r--   0 mroy       (501) staff       (20)     1887 2023-05-04 01:08:28.000000 chatglm-llm-1.3.7/README.md
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-15 08:48:43.360073 chatglm-llm-1.3.7/chatglm_llm.egg-info/
+-rw-r--r--   0 mroy       (501) staff       (20)      212 2023-06-15 08:48:43.000000 chatglm-llm-1.3.7/chatglm_llm.egg-info/PKG-INFO
+-rw-r--r--   0 mroy       (501) staff       (20)      480 2023-06-15 08:48:43.000000 chatglm-llm-1.3.7/chatglm_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 mroy       (501) staff       (20)        1 2023-06-15 08:48:43.000000 chatglm-llm-1.3.7/chatglm_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 mroy       (501) staff       (20)       53 2023-06-15 08:48:43.000000 chatglm-llm-1.3.7/chatglm_llm.egg-info/entry_points.txt
+-rw-r--r--   0 mroy       (501) staff       (20)        1 2023-05-04 01:12:10.000000 chatglm-llm-1.3.7/chatglm_llm.egg-info/not-zip-safe
+-rw-r--r--   0 mroy       (501) staff       (20)      240 2023-06-15 08:48:43.000000 chatglm-llm-1.3.7/chatglm_llm.egg-info/requires.txt
+-rw-r--r--   0 mroy       (501) staff       (20)       12 2023-06-15 08:48:43.000000 chatglm-llm-1.3.7/chatglm_llm.egg-info/top_level.txt
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-15 08:48:43.361312 chatglm-llm-1.3.7/chatglm_src/
+-rw-r--r--   0 mroy       (501) staff       (20)      690 2023-05-30 04:21:32.000000 chatglm-llm-1.3.7/chatglm_src/__init__.py
+-rw-r--r--   0 mroy       (501) staff       (20)     4201 2023-05-13 02:36:58.000000 chatglm-llm-1.3.7/chatglm_src/callbacks.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-15 08:48:43.361765 chatglm-llm-1.3.7/chatglm_src/chains/
+-rw-r--r--   0 mroy       (501) staff       (20)       69 2023-05-10 01:48:15.000000 chatglm-llm-1.3.7/chatglm_src/chains/__init__.py
+-rw-r--r--   0 mroy       (501) staff       (20)     4402 2023-05-11 09:17:21.000000 chatglm-llm-1.3.7/chatglm_src/chains/local_qa.py
+-rw-r--r--   0 mroy       (501) staff       (20)      537 2023-05-30 04:20:56.000000 chatglm-llm-1.3.7/chatglm_src/cmd.py
+-rw-r--r--   0 mroy       (501) staff       (20)     3052 2023-06-15 08:48:00.000000 chatglm-llm-1.3.7/chatglm_src/embeding.py
+-rw-r--r--   0 mroy       (501) staff       (20)    36155 2023-06-01 08:59:10.000000 chatglm-llm-1.3.7/chatglm_src/llm.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-15 08:48:43.362148 chatglm-llm-1.3.7/chatglm_src/loader/
+-rw-r--r--   0 mroy       (501) staff       (20)     1403 2023-05-11 01:28:05.000000 chatglm-llm-1.3.7/chatglm_src/loader/__init__.py
+-rw-r--r--   0 mroy       (501) staff       (20)       38 2023-06-15 08:48:43.362553 chatglm-llm-1.3.7/setup.cfg
+-rw-r--r--   0 mroy       (501) staff       (20)     1026 2023-06-15 08:48:34.000000 chatglm-llm-1.3.7/setup.py
```

### Comparing `chatglm-llm-1.3.4/README.md` & `chatglm-llm-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.3.4/chatglm_src/__init__.py` & `chatglm-llm-1.3.7/chatglm_src/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pathlib
-from .llm import ChatGLMLLM
+from .llm import ChatGLMLLM,Vicuna13B
 from .chains import KnowdageQA
 from .embeding import ChatGLMEmbeding
 
 # _EMBEDDING_PATH = pathlib.Path.home() / ".cache" / "chatglm-embedding"
 
 # if not _EMBEDDING_PATH.exists():
 #     print("------ start founding embedding  ------:", _EMBEDDING_PATH)
```

### Comparing `chatglm-llm-1.3.4/chatglm_src/callbacks.py` & `chatglm-llm-1.3.7/chatglm_src/callbacks.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.3.4/chatglm_src/chains/local_qa.py` & `chatglm-llm-1.3.7/chatglm_src/chains/local_qa.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.3.4/chatglm_src/embeding.py` & `chatglm-llm-1.3.7/chatglm_src/embeding.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.3.4/chatglm_src/llm.py` & `chatglm-llm-1.3.7/chatglm_src/llm.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,31 +5,40 @@
 from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 import pathlib
 import os, json
 import asyncio
 from termcolor import colored
 
 import datetime
+import inspect
 from hashlib import md5
 import time
 import numpy as np
 from aiowebsocket.converses import AioWebSocket
 from websocket import create_connection
 import websockets
 from websockets.server import serve
-from langchain.callbacks.manager import BaseCallbackManager, CallbackManagerForLLMRun
 from langchain.embeddings import HuggingFaceEmbeddings
 import gptcache
 from gptcache.processor.pre import get_prompt
 from gptcache.manager.factory import get_data_manager
-from langchain.cache import GPTCache
+
+try:
+    from langchain.cache import GPTCache
+except:
+    pass
+
 
 try:
     from transformers import AutoTokenizer, AutoModel
+    from fastchat.serve.inference import load_model
+    from fastchat.conversation import get_default_conv_template
     from accelerate import load_checkpoint_and_dispatch
+    
+    from fastchat.serve.inference import generate_stream
     import torch, gc
     DEFAULT_CACHE_MAP_PATH = str(pathlib.Path.home() / ".cache" / "local_qa_cache_map")
     i = 0
 
     def init_gptcache_map(cache_obj: gptcache.Cache):
         global i
         cache_path = f'{DEFAULT_CACHE_MAP_PATH}_{i}.txt'
@@ -42,15 +51,16 @@
     langchain.llm_cache = GPTCache(init_gptcache_map)
     print(colored("init gptcache", "green"))
 except Exception as e:
     print("use remote ignore this / load transformers failed, please install transformers and accelerate first and torch.")
 from .callbacks import AsyncWebsocketHandler, AsyncWebSocksetCallbackManager
 
 
-
+def is_async_method(method):
+    return inspect.iscoroutinefunction(method)
 ## LLM for chatglm
 # only load from local's path
 # default path is in ~/.cache/chatglm, if not exists, will download from huggingface'url :https://huggingface.co/THUDM/chatglm-6b
 # 
 """Common utility functions for working with LLM APIs."""
 import re
 from typing import List, Dict, Any, Optional, Union
@@ -137,14 +147,285 @@
             CUDA_DEVICE = f"cuda:{i}"
             with torch.cuda.device(CUDA_DEVICE):
                 torch.cuda.empty_cache()
                 torch.cuda.ipc_collect()
     else:
         gc.collect()
 
+
+class Vicuna13B(LLM):
+    max_token: int = 2048
+    temperature: float = 0.2
+    top_p = 0.9
+    top_k = 2
+    history = []
+    history_id = "default"
+    tokenizer: Any = None
+    model: Any = None
+    history_len: int = 10
+    model: Any = None
+    tokenizer: Any = None
+    model_path: str = pathlib.Path.home() / ".cache" / "vicuna-13b-f"
+    cpu: bool = False
+    streaming: bool = False
+    verbose: bool = False
+    callbacks :Any  = [StreamingStdOutCallbackHandler()]
+    remote_host: Any = None
+    @classmethod
+    def load(cls, *args, model_path:str=None, **kwargs):
+        mo = cls(*args, **kwargs)
+        if mo.remote_host is not None:
+            return mo
+        if model_path is None:
+            model_path = cls.model_path
+        print(colored("[GPU]","green"),":",torch.cuda.device_count(), "GPUs" )
+        mo.model, mo.tokenizer = load_model(model_path, device="cuda", num_gpus="auto")
+        return mo   
+    
+    
+    def set_history(self, hist:List[str]):
+        self.history = hist
+    
+    
+    @property
+    def _llm_type(self) -> str:
+        return "Vicuna-13b"
+    
+    
+    def stream_output(self, prompt, on_llm_start,on_llm_new_token,on_llm_end):
+        st = time.time()
+        
+        params = {
+            "prompt": prompt,
+            "temperature": self.temperature,
+            "max_new_tokens": self.max_token,
+            "top_p":0.9,
+            # "top_k":k,
+            # "beams_num":4,
+            "stop": None,
+        }
+
+        # Stream output
+        if "</s>" in prompt:
+            history, input_prompt = prompt.split("</s>",1)
+            history += " "
+        else:
+            history = ""
+            input_prompt = prompt
+        on_llm_start(prompt, None, verbose=self.verbose)
+        all_text = ""
+        delta = ""
+
+        # print("AT:",prompt.encode())
+        for i,response in enumerate(generate_stream(self.model, self.tokenizer, params, device="cuda",stream_interval=4)):
+            all_text = response.encode()[len((history+input_prompt).encode()):]
+            delta = all_text[len(delta):].decode("utf-8","ignore")
+            data = {"response": response, "history": history,"query": prompt}
+            if self.verbose:
+                print(delta, end='', flush=True)
+            self.callback_manager.on_llm_new_token(
+                delta, verbose=self.verbose, **data
+            )
+        auto_gc()
+        self.history = self.history+[[input_prompt.split("USER:",1)[1], all_text.decode("utf-8","ignore")]]
+        pure_output = all_text.decode("utf-8","ignore")
+        print("usage : ", time.time() - st, "s")
+        return pure_output
+    
+
+
+    async def _acall(self, prompt: str, stop: List[str] = None):
+        assert self.remote_host is not None
+        uri = f"ws://{self.remote_host}:15000"
+
+        async with AioWebSocket(uri) as aws:
+            converse = aws.manipulator
+            
+            user_id = md5(time.asctime().encode()).hexdigest()
+            await converse.send(json.dumps({"user_id":user_id, "password":PASSWORD}).encode())
+            res = await converse.receive()
+            res = res.decode()
+            if res != "ok":
+                raise Exception("password error:"+res)
+            result = ''
+            data = json.dumps({
+                "model":"vicuna-13b",
+                "prompt":prompt,
+                "history":self.history,
+                "temperature": self.temperature,
+                }).encode()
+            await self.asend_to_remote(data, converse)
+
+            for callback in self.callbacks:
+                if is_async_method(callback.on_llm_start):
+                    await callback.on_llm_start(
+                        None,
+                        prompt,
+                        run_id=user_id,
+                        verbose=self.verbose
+                    )
+            while 1:
+                res = await converse.receive()
+                msg = json.loads(res.decode())
+                # { "new":delta,"response": response, "history": history,"query": prompt}
+                if "stop" in msg:
+                    break
+                new_token = msg["new"]
+                response = msg["response"]
+                history = msg["history"]
+                msg["verbose"] = True
+                for callback in self.callbacks:
+                    if is_async_method(callback.on_llm_new_token):
+                        await callback.on_llm_new_token(new_token, **msg)
+                result = response
+            self.history = self.history+[[prompt, result]]
+            for callback in self.callbacks:
+                if is_async_method(callback.on_llm_new_token):
+                        await callback.on_llm_end(result, verbose=self.verbose)
+            self.history = self.history+[[prompt, result]]
+            return result
+
+    def _call(self, prompt: str, stop: List[str]  = None, run_manager:Any = None) -> str:
+        if self.remote_host is not None:
+            ws = create_connection(f"ws://{self.remote_host}:15000")
+            user_id = md5(time.asctime().encode()).hexdigest()
+            # self.callback_manager =  langchain.callbacks.base.BaseCallbackManager(self.callbacks)
+            
+            # self.callback_manager =  BaseCallbackManager(self.callbacks)
+            # self.callback_manager.set_handlers(self.callbacks)
+            ws.send(json.dumps({"user_id":user_id, "password":PASSWORD}))
+            # time.sleep(0.5)
+            res = ws.recv()
+            if res != "ok":
+                print(colored("[info]:","yellow") ,res)
+                raise Exception("password error")
+            result = ''
+            data = json.dumps({
+                "model":"vicuna-13b",
+                "prompt":prompt,
+                "history":self.history,
+                "temperature": self.temperature,
+                })
+            self.send_to_remote(data, ws)
+            
+            for callback in self.callbacks:
+                if  is_async_method(callback.on_llm_start):continue
+                callback.on_llm_start(
+                    None,
+                    prompt,
+                    run_id=user_id,
+                    verbose=self.verbose
+                )
+            while 1:
+                res = ws.recv()
+                msg = json.loads(res)
+                # { "new":delta,"response": response, "history": history,"query": prompt}
+                if "stop" in msg:
+                    break
+                new_token = msg["new"]
+                response = msg["response"]
+                history = msg["history"]
+                msg["verbose"] = self.verbose
+                # self.remote_callback(new_token, history, response)
+                
+                # self.callback_manager.on_llm_new_token(new_token, **msg)
+                for callback in self.callbacks:
+                    if  is_async_method(callback.on_llm_new_token):continue
+                    callback.on_llm_new_token(
+                        new_token,
+                        **msg
+                    )
+                result = response
+            for callback in self.callbacks:
+                if  is_async_method(callback.on_llm_end):continue
+                callback.on_llm_end(result, verbose=self.verbose)
+            
+            self.history = self.history+[[prompt, result]]
+            return result
+        else:
+            current_completion = self.stream_output(prompt, run_manager.on_llm_start, run_manager.on_llm_new_token, run_manager.on_llm_end)
+            return current_completion
+    
+    async def _ncall(self, aio,prompt,history, temperature=None):
+        if history is not None and isinstance(history, list):
+            self.history = history
+
+        if "USER:" not in prompt and "ASSISTANT:" not in prompt:
+            conv = get_default_conv_template("vicuna").copy()
+            for p,o in self.history:
+                conv.append_message(conv.roles[0], p+"\n")
+                conv.append_message(conv.roles[1], o+"\n")
+            conv.append_message(conv.roles[0], prompt+"\n")
+            conv.append_message(conv.roles[1], None)
+            prompt = conv.get_prompt()
+        print(colored("prompt:", "green"),prompt, colored(" temperature:", "green"), temperature)
+        
+        params = {
+            "prompt": prompt,
+            "temperature": self.temperature,
+            "max_new_tokens": self.max_token,
+            "top_p":0.9,
+            # "top_k":k,
+            # "beams_num":4,
+            "stop": None,
+        }
+        if temperature is not None:
+            params["temperature"] = temperature
+
+        # Stream output
+        if "</s>" in prompt:
+            history, input_prompt = prompt.split("</s>",1)
+            history += " "
+        else:
+            history = ""
+            input_prompt = prompt
+        
+        all_text = ""
+        delta = ""
+
+        # print("AT:",prompt.encode())
+        old = ""
+        sended = ""
+        for i,response in enumerate(generate_stream(self.model, self.tokenizer, params, device="cuda")):
+            all_text = response[len((history+input_prompt)):]
+            
+            try:
+                if "�" in all_text:
+                    continue
+                delta = all_text[len(old):]
+                old = all_text
+                
+                data = { "new":delta,"response": all_text, "history": history,"query": prompt}
+                # print(colored("[delta]:","green"), delta)
+                # print(colored("[currt]:","yellow"), all_text,end="\n\t---- io ----\n")
+                await aio.send(json.dumps(data))
+            except :
+                continue
+        data = { "new":delta,"response": all_text, "history": history,"query": prompt, "stop":True}
+        # await aio.send(json.dumps(data))
+        auto_gc()
+        return data
+
+    def send_to_remote(self,data,ws):
+        """
+        every chunk of data is 2M
+        """
+        for i in range(0, len(data), 1024*1024*2):
+            ws.send(data[i:i+1024*1024*2])
+        ws.send("[STOP]")
+
+    async def asend_to_remote(self, data, ws):
+        """
+        every chunk of data is 2M
+        """
+        for i in range(0, len(data), 1024*1024*2):
+            await ws.send(data[i:i+1024*1024*2])
+        await ws.send("[STOP]")       
+        
+        
 class ChatGLMLLM(LLM):
     """
             Load a model from local or remote
         if want to use stream mode:
             'streaming=True'
         if want to use langchain's Callback:
             examples: 'callbacks=[StreamingStdOutCallbackHandler(), AsyncWebsocketHandler()]'
@@ -277,42 +558,48 @@
                 },
                 verbose=self.verbose
             )
             return current_completion
         elif self.remote_host is not None :
             uri = f"ws://{self.remote_host}:15000"
             result = ''
-            self.callback_manager =  BaseCallbackManager(self.callbacks)
-            self.callback_manager.set_handlers(self.callbacks)
+            # self.callback_manager =  BaseCallbackManager(self.callbacks)
+            # self.callback_manager.set_handlers(self.callbacks)
             async with AioWebSocket(uri) as aws:
                 converse = aws.manipulator
                 
                 user_id = md5(time.asctime().encode()).hexdigest()
                 await converse.send(json.dumps({"user_id":user_id, "password":PASSWORD}).encode())
                 res = await converse.receive()
                 res = res.decode()
                 if res != "ok":
                     raise Exception("password error:"+res)
-                data = json.dumps({"prompt":prompt, "history":self.history}).encode()
+                data = json.dumps({"prompt":prompt, "history":self.history,"model":"chatglm","temperature":self.temperature}).encode()
                 await self.asend_to_remote(data, converse)
 
-                self.callback_manager.on_llm_start(prompt, None, verbose=self.verbose)
+                for call in self.callbacks:
+                    if is_async_method(call.on_llm_start):
+                        await call.on_llm_start(prompt, None, verbose=self.verbose)
                 while 1:
                     res = await converse.receive()
                     msg = json.loads(res.decode())
                     # { "new":delta,"response": response, "history": history,"query": prompt}
                     if "stop" in msg:
                         break
                     new_token = msg["new"]
                     response = msg["response"]
-                    history = msg["history"]
-                    self.callback_manager.on_llm_new_token(new_token, response=response, history=history, query=prompt, verbose=self.verbose)
+                    msg["verbose"] = self.verbose
+                    for call in self.callbacks:
+                        if is_async_method(call.on_llm_start):
+                            await call.on_llm_new_token(new_token, **msg)
                     result = response
             self.history = self.history+[[prompt, result]]
-            self.callback_manager.on_llm_end(result, verbose=self.verbose)
+            for call in self.callbacks:
+                if is_async_method(call.on_llm_start):
+                    await call.on_llm_end(result, verbose=self.verbose)
             return result
 
 
                 
         else:
             response, _ = self.model.chat(
                 self.tokenizer,
@@ -338,15 +625,15 @@
         """
         every chunk of data is 2M
         """
         for i in range(0, len(data), 1024*1024*2):
             await ws.send(data[i:i+1024*1024*2])
         await ws.send("[STOP]")
     
-    def _call(self, prompt: str, stop: List[str]  = None,run_manager: Optional[CallbackManagerForLLMRun] = None) -> str:
+    def _call(self, prompt: str, stop: List[str]  = None,run_manager: Any = None) -> str:
         if self.streaming:
             current_completion = ""
             if self.verbose:
                 print("streaming")
             
             for response, history in self.model.stream_chat(self.tokenizer, prompt, self.history, max_length=self.max_token, top_p=self.top_p,
                                                temperature=self.temperature):
@@ -371,18 +658,21 @@
             ws.send(json.dumps({"user_id":user_id, "password":PASSWORD}))
             # time.sleep(0.5)
             res = ws.recv()
             if res != "ok":
                 print(colored("[info]:","yellow") ,res)
                 raise Exception("password error")
             result = ''
-            data = json.dumps({"prompt":prompt, "history":self.history})
+                
+                
+            data = json.dumps({"prompt":prompt, "history":self.history,"model":"chatglm", "temperature": self.temperature})
             self.send_to_remote(data, ws)
             
             for callback in self.callbacks:
+                if is_async_method(callback.on_llm_start):continue
                 callback.on_llm_start(
                     None,
                     prompt,
                     run_id=user_id,
                     verbose=self.verbose
                 )
             while 1:
@@ -395,20 +685,22 @@
                 response = msg["response"]
                 history = msg["history"]
                 msg["verbose"] = self.verbose
                 # self.remote_callback(new_token, history, response)
                 
                 # self.callback_manager.on_llm_new_token(new_token, **msg)
                 for callback in self.callbacks:
+                    if is_async_method(callback.on_llm_start):continue
                     callback.on_llm_new_token(
                         new_token,
                         **msg
                     )
                 result = response
             for callback in self.callbacks:
+                if is_async_method(callback.on_llm_start):continue
                 callback.on_llm_end(result, verbose=self.verbose)
             
             self.history = self.history+[[prompt, result]]
             return result
         else:
             response, _ = self.model.chat(
                 self.tokenizer,
@@ -433,31 +725,40 @@
     
     async def reply(self, data):
         await self.websocket.send(str(len(data)))
         for i in range(0,len(data), 1024*1024*2):
             await self.websocket.send(data[i:i+1024*1024*2])
         await self.websocket.send("[STOP]")
     
-    async def __call__(self, prompt=None, embed_documents=None,embed_query=None,history=None):
+    async def __call__(self, prompt=None,model=None,temperature=None, embed_documents=None,embed_query=None,history=None):
         try:
             # assert prompt is not None 
             if prompt is not None:
                 assert isinstance(prompt, str)
-                llm = self.llm
-                current_completion = ""
-                if history is not None and isinstance(history, list):
-                    llm.history = history
-                for response, history in llm.model.stream_chat(llm.tokenizer, prompt, llm.history, max_length=llm.max_token, top_p=llm.top_p,
-                                                    temperature=llm.temperature):
-                    delta = response[len(current_completion) :]
-                    current_completion = response
-                    data = { "new":delta,"response": response, "history": history,"query": prompt}
-                    await self.websocket.send(json.dumps(data))
-                data = { "new":delta,"response": response, "history": history,"query": prompt, "stop":True}
-                
+                assert model is not None
+                if model == "chatglm":
+                    llm = self.llm
+                    current_completion = ""
+                    if history is not None and isinstance(history, list):
+                        llm.history = history
+                    if temperature is not None:
+                        llm.temperature = temperature
+                    for response, history in llm.model.stream_chat(llm.tokenizer, prompt, llm.history, max_length=llm.max_token, top_p=llm.top_p,
+                                                        temperature=llm.temperature):
+                        delta = response[len(current_completion) :]
+                        current_completion = response
+                        data = { "new":delta,"response": response, "history": history,"query": prompt}
+                        await self.websocket.send(json.dumps(data))
+                    data = { "new":delta,"response": response, "history": history,"query": prompt, "stop":True}
+                elif model == "vicuna-13b":
+                    
+                    data = await self.llm._ncall(self.websocket, prompt, history,temperature=temperature)
+                    
+                else:
+                    data = { "new":"X","response": "Not Support Model !:"+model, "history": history,"query": prompt, "stop":True}
                 await self.websocket.send(json.dumps(data))
             elif embed_query is not None:
                 res = self.embeding.embed_query(embed_query)
                 data = { "embed":res} 
                 data = json.dumps(data, cls=NumpyEncoder)
                 await self.reply(data)
             elif embed_documents is not None:
@@ -578,26 +879,31 @@
     
     @classmethod
     async def del_user(cls,websocket):
         if websocket in cls.__users:
             del cls.__users[websocket]
 
     @classmethod
-    def start(cls,port=15000, model_path=None):
+    def start(cls,port=15000, model_path=None, name="chatglm"):
         cpu = False
         if not torch.cuda.is_available():
             cpu = True
         print(colored(f"[cpu:{cpu} ]","green"),":",f"listen:0.0.0.0:{port}")
         cls.embeding = HuggingFaceEmbeddings(model_name="GanymedeNil/text2vec-large-chinese")
         print(colored(f"[embedding: use cpu{cpu} ]","green"),":",f"GanymedeNil/text2vec-large-chinese")
-        cls.llm = ChatGLMLLM.load(model_path=model_path, cpu=cpu, streaming=True)
-        print(colored(f"[ starting ]","green"),":",f"listen:0.0.0.0:{port}")
+        if name == "chatglm":
+            cls.llm = ChatGLMLLM.load(model_path=model_path, cpu=cpu, streaming=True)
+            print(colored(f"[ starting chatglm]","green"),":",f"listen:0.0.0.0:{port}")
+        elif name == "vicuna-13b":
+            cls.llm = Vicuna13B.load(model_path=model_path, cpu=cpu, streaming=True)
+            print(colored(f"[ starting vicuna-13b]","green"),":",f"listen:0.0.0.0:{port}")
         asyncio.run(cls.main(port))
 
 
+
 class NumpyEncoder(json.JSONEncoder):
     """ Special json encoder for numpy types """
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         elif isinstance(obj, np.floating):
             return float(obj)
```

### Comparing `chatglm-llm-1.3.4/chatglm_src/loader/__init__.py` & `chatglm-llm-1.3.7/chatglm_src/loader/__init__.py`

 * *Files identical despite different names*

