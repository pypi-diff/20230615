# Comparing `tmp/fastwapi-0.1.2.tar.gz` & `tmp/fastwapi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastwapi-0.1.2.tar", last modified: Thu Jun 15 11:15:58 2023, max compression
+gzip compressed data, was "fastwapi-0.1.3.tar", last modified: Thu Jun 15 11:29:37 2023, max compression
```

## Comparing `fastwapi-0.1.2.tar` & `fastwapi-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 11:15:58.277582 fastwapi-0.1.2/
--rw-rw-rw-   0        0        0     1062 2023-06-15 09:10:09.000000 fastwapi-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     4421 2023-06-15 11:15:58.277582 fastwapi-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1710 2023-06-15 10:30:10.000000 fastwapi-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 11:15:58.261583 fastwapi-0.1.2/fastwapi/
--rw-rw-rw-   0        0        0       43 2023-06-15 11:15:22.000000 fastwapi-0.1.2/fastwapi/__init__.py
--rw-rw-rw-   0        0        0     1364 2023-06-15 10:40:00.000000 fastwapi-0.1.2/fastwapi/fastwapi.py
-drwxrwxrwx   0        0        0        0 2023-06-15 11:15:58.276582 fastwapi-0.1.2/fastwapi.egg-info/
--rw-rw-rw-   0        0        0     4421 2023-06-15 11:15:58.000000 fastwapi-0.1.2/fastwapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-15 11:15:58.000000 fastwapi-0.1.2/fastwapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 11:15:58.000000 fastwapi-0.1.2/fastwapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-15 11:15:58.000000 fastwapi-0.1.2/fastwapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-15 11:15:58.000000 fastwapi-0.1.2/fastwapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1533 2023-06-15 11:15:34.000000 fastwapi-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-15 11:15:58.277582 fastwapi-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-15 11:29:37.835605 fastwapi-0.1.3/
+-rw-rw-rw-   0        0        0     1062 2023-06-15 09:10:09.000000 fastwapi-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     4370 2023-06-15 11:29:37.835605 fastwapi-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1659 2023-06-15 11:29:09.000000 fastwapi-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 11:29:37.828604 fastwapi-0.1.3/fastwapi/
+-rw-rw-rw-   0        0        0       43 2023-06-15 11:15:22.000000 fastwapi-0.1.3/fastwapi/__init__.py
+-rw-rw-rw-   0        0        0     1376 2023-06-15 11:28:15.000000 fastwapi-0.1.3/fastwapi/fastwapi.py
+-rw-rw-rw-   0        0        0      571 2023-06-15 11:27:20.000000 fastwapi-0.1.3/fastwapi/main.py
+drwxrwxrwx   0        0        0        0 2023-06-15 11:29:37.834605 fastwapi-0.1.3/fastwapi.egg-info/
+-rw-rw-rw-   0        0        0     4370 2023-06-15 11:29:37.000000 fastwapi-0.1.3/fastwapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-06-15 11:29:37.000000 fastwapi-0.1.3/fastwapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 11:29:37.000000 fastwapi-0.1.3/fastwapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-15 11:29:37.000000 fastwapi-0.1.3/fastwapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 11:29:37.000000 fastwapi-0.1.3/fastwapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1533 2023-06-15 11:29:22.000000 fastwapi-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-15 11:29:37.836605 fastwapi-0.1.3/setup.cfg
```

### Comparing `fastwapi-0.1.2/LICENSE` & `fastwapi-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastwapi-0.1.2/PKG-INFO` & `fastwapi-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastwapi
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple API Websocket server to easily parse JSON
 Author-email: lonode <lonode-git@proton.me>
 License: MIT License
         
         Copyright (c) 2023 lonode
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,21 +50,23 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Description
 
-A simple lightweight Websocket framework based on Starlette, which provide easy-to-use Python decorator to parse JSON incoming message.  
+FastWAPI is a simple lightweight Websocket framework based on Starlette, which provide easy-to-use Python decorator to parse JSON incoming message.  
 
-It's in the same spirit as FastAPI, where each decorator map to a path. But here, each decorator map to a Pydantic object, so it is easy to map each incoming JSON message to a function. 
+It's in the same spirit as _FastAPI_, where each decorator map to an HTTP path. But here, each decorator map to a Pydantic object, and each object map to a function. 
 
+# Installation
+
+`pip install fastwapi`
 # Disclaimer
 
- - The project is not yet available on pip due to a name conflict with a previous wapi project.
  - The module is available, but far from finished & polished, please do not use it in production.
 
 # Roadmap 
 
 - Add authent middleware
 - Add background job to asynchrounosly send JSON to the client
 
@@ -74,18 +76,18 @@
 
 Getting started in three steps :
 
 #### Instanciates the framework and declare the Websocket HTTP endpoint.  
 
 ```python
 import uvicorn
-from wapi import WAPI, WebSocket
+from fastwapi import FastWAPI, WebSocket
 from pydantic import BaseModel
 
-app = WAPI(endpoint="/ws")
+app = FastWAPI(endpoint="/ws")
 
 ```
 
 #### Define Pyndantic model, for incoming and outgoing messages.
 
 ```python
 class CM(BaseModel):
```

### Comparing `fastwapi-0.1.2/README.md` & `fastwapi-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Description
 
-A simple lightweight Websocket framework based on Starlette, which provide easy-to-use Python decorator to parse JSON incoming message.  
+FastWAPI is a simple lightweight Websocket framework based on Starlette, which provide easy-to-use Python decorator to parse JSON incoming message.  
 
-It's in the same spirit as FastAPI, where each decorator map to a path. But here, each decorator map to a Pydantic object, so it is easy to map each incoming JSON message to a function. 
+It's in the same spirit as _FastAPI_, where each decorator map to an HTTP path. But here, each decorator map to a Pydantic object, and each object map to a function. 
 
+# Installation
+
+`pip install fastwapi`
 # Disclaimer
 
- - The project is not yet available on pip due to a name conflict with a previous wapi project.
  - The module is available, but far from finished & polished, please do not use it in production.
 
 # Roadmap 
 
 - Add authent middleware
 - Add background job to asynchrounosly send JSON to the client
 
@@ -20,18 +22,18 @@
 
 Getting started in three steps :
 
 #### Instanciates the framework and declare the Websocket HTTP endpoint.  
 
 ```python
 import uvicorn
-from wapi import WAPI, WebSocket
+from fastwapi import FastWAPI, WebSocket
 from pydantic import BaseModel
 
-app = WAPI(endpoint="/ws")
+app = FastWAPI(endpoint="/ws")
 
 ```
 
 #### Define Pyndantic model, for incoming and outgoing messages.
 
 ```python
 class CM(BaseModel):
```

### Comparing `fastwapi-0.1.2/fastwapi/fastwapi.py` & `fastwapi-0.1.3/fastwapi/fastwapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     encoding = 'json'
     
     async def on_connect(self, websocket):
         await websocket.accept()
 
     async def on_receive(self, websocket, data):
         try:
-            decoded, func = WAPI.decode_incoming(data)
+            decoded, func = FastWAPI.decode_incoming(data)
         except:
             await websocket.send_json({"error":"invalid JSON"})
             return -1
         
         await func(websocket, decoded)
 
     async def on_disconnect(self, websocket, close_code):
@@ -24,18 +24,18 @@
 
 class FastWAPI(Starlette):
 
     mapping_class = {}
 
 
     def decode_incoming(data: dict):
-        for model in WAPI.mapping_class:
+        for model in FastWAPI.mapping_class:
             try:
                 decoded = model(**data)
-                return decoded, WAPI.mapping_class[model]
+                return decoded, FastWAPI.mapping_class[model]
             except:
                 print("error")
 
 
     def __init__(self,endpoint: str):
         super().__init__(routes=[WebSocketRoute(endpoint, WSEndpoint)])
```

### Comparing `fastwapi-0.1.2/fastwapi.egg-info/PKG-INFO` & `fastwapi-0.1.3/fastwapi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastwapi
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple API Websocket server to easily parse JSON
 Author-email: lonode <lonode-git@proton.me>
 License: MIT License
         
         Copyright (c) 2023 lonode
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,21 +50,23 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Description
 
-A simple lightweight Websocket framework based on Starlette, which provide easy-to-use Python decorator to parse JSON incoming message.  
+FastWAPI is a simple lightweight Websocket framework based on Starlette, which provide easy-to-use Python decorator to parse JSON incoming message.  
 
-It's in the same spirit as FastAPI, where each decorator map to a path. But here, each decorator map to a Pydantic object, so it is easy to map each incoming JSON message to a function. 
+It's in the same spirit as _FastAPI_, where each decorator map to an HTTP path. But here, each decorator map to a Pydantic object, and each object map to a function. 
 
+# Installation
+
+`pip install fastwapi`
 # Disclaimer
 
- - The project is not yet available on pip due to a name conflict with a previous wapi project.
  - The module is available, but far from finished & polished, please do not use it in production.
 
 # Roadmap 
 
 - Add authent middleware
 - Add background job to asynchrounosly send JSON to the client
 
@@ -74,18 +76,18 @@
 
 Getting started in three steps :
 
 #### Instanciates the framework and declare the Websocket HTTP endpoint.  
 
 ```python
 import uvicorn
-from wapi import WAPI, WebSocket
+from fastwapi import FastWAPI, WebSocket
 from pydantic import BaseModel
 
-app = WAPI(endpoint="/ws")
+app = FastWAPI(endpoint="/ws")
 
 ```
 
 #### Define Pyndantic model, for incoming and outgoing messages.
 
 ```python
 class CM(BaseModel):
```

### Comparing `fastwapi-0.1.2/pyproject.toml` & `fastwapi-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastwapi"
-version = "0.1.2"
+version = "0.1.3"
 description = "A simple API Websocket server to easily parse JSON"
 readme = "README.md"
 authors = [{ name = "lonode", email = "lonode-git@proton.me" }]
 license = { file = "LICENSE" }
 classifiers = [
  "Intended Audience :: Information Technology",
     "Intended Audience :: System Administrators",
```

