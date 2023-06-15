# Comparing `tmp/lanarky-0.7.8.tar.gz` & `tmp/lanarky-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanarky-0.7.8.tar", max compression
+gzip compressed data, was "lanarky-0.7.9.tar", max compression
```

## Comparing `lanarky-0.7.8.tar` & `lanarky-0.7.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1073 2023-06-04 20:29:47.738920 lanarky-0.7.8/LICENSE
--rw-r--r--   0        0        0     4746 2023-06-04 20:29:47.738920 lanarky-0.7.8/README.md
--rw-r--r--   0        0        0      130 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/__init__.py
--rw-r--r--   0        0        0     2874 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/callbacks/__init__.py
--rw-r--r--   0        0        0     3082 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/callbacks/agents.py
--rw-r--r--   0        0        0     2204 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/callbacks/base.py
--rw-r--r--   0        0        0     1685 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/callbacks/llm.py
--rw-r--r--   0        0        0     3515 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/callbacks/retrieval_qa.py
--rw-r--r--   0        0        0      422 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/register/__init__.py
--rw-r--r--   0        0        0     1171 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/register/base.py
--rw-r--r--   0        0        0     1074 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/register/callbacks.py
--rw-r--r--   0        0        0       74 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/responses/__init__.py
--rw-r--r--   0        0        0     5980 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/responses/streaming.py
--rw-r--r--   0        0        0      150 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/routing/__init__.py
--rw-r--r--   0        0        0     5591 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/routing/langchain.py
--rw-r--r--   0        0        0     7467 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/routing/utils.py
--rw-r--r--   0        0        0      316 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/schemas/__init__.py
--rw-r--r--   0        0        0      335 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/schemas/callbacks.py
--rw-r--r--   0        0        0      707 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/schemas/websockets.py
--rw-r--r--   0        0        0       69 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/testing/__init__.py
--rw-r--r--   0        0        0     3212 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/testing/gradio.py
--rw-r--r--   0        0        0      391 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/testing/settings.py
--rw-r--r--   0        0        0       73 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/websockets/__init__.py
--rw-r--r--   0        0        0     4793 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/websockets/base.py
--rw-r--r--   0        0        0     1419 2023-06-04 20:29:47.918933 lanarky-0.7.8/pyproject.toml
--rw-r--r--   0        0        0     5884 1970-01-01 00:00:00.000000 lanarky-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-10 08:13:42.713097 lanarky-0.7.9/LICENSE
+-rw-r--r--   0        0        0     5525 2023-06-10 08:13:42.713097 lanarky-0.7.9/README.md
+-rw-r--r--   0        0        0      130 2023-06-10 08:13:42.889099 lanarky-0.7.9/lanarky/__init__.py
+-rw-r--r--   0        0        0     2874 2023-06-10 08:13:42.893099 lanarky-0.7.9/lanarky/callbacks/__init__.py
+-rw-r--r--   0        0        0     3082 2023-06-10 08:13:42.893099 lanarky-0.7.9/lanarky/callbacks/agents.py
+-rw-r--r--   0        0        0     2204 2023-06-10 08:13:42.893099 lanarky-0.7.9/lanarky/callbacks/base.py
+-rw-r--r--   0        0        0     1685 2023-06-10 08:13:42.893099 lanarky-0.7.9/lanarky/callbacks/llm.py
+-rw-r--r--   0        0        0     3515 2023-06-10 08:13:42.893099 lanarky-0.7.9/lanarky/callbacks/retrieval_qa.py
+-rw-r--r--   0        0        0      422 2023-06-10 08:13:42.893099 lanarky-0.7.9/lanarky/register/__init__.py
+-rw-r--r--   0        0        0     1171 2023-06-10 08:13:42.893099 lanarky-0.7.9/lanarky/register/base.py
+-rw-r--r--   0        0        0     1074 2023-06-10 08:13:42.893099 lanarky-0.7.9/lanarky/register/callbacks.py
+-rw-r--r--   0        0        0       74 2023-06-10 08:13:42.893099 lanarky-0.7.9/lanarky/responses/__init__.py
+-rw-r--r--   0        0        0     5980 2023-06-10 08:13:42.893099 lanarky-0.7.9/lanarky/responses/streaming.py
+-rw-r--r--   0        0        0      150 2023-06-10 08:13:42.893099 lanarky-0.7.9/lanarky/routing/__init__.py
+-rw-r--r--   0        0        0     5591 2023-06-10 08:13:42.893099 lanarky-0.7.9/lanarky/routing/langchain.py
+-rw-r--r--   0        0        0     7467 2023-06-10 08:13:42.893099 lanarky-0.7.9/lanarky/routing/utils.py
+-rw-r--r--   0        0        0      316 2023-06-10 08:13:42.893099 lanarky-0.7.9/lanarky/schemas/__init__.py
+-rw-r--r--   0        0        0      335 2023-06-10 08:13:42.893099 lanarky-0.7.9/lanarky/schemas/callbacks.py
+-rw-r--r--   0        0        0      707 2023-06-10 08:13:42.893099 lanarky-0.7.9/lanarky/schemas/websockets.py
+-rw-r--r--   0        0        0       69 2023-06-10 08:13:42.893099 lanarky-0.7.9/lanarky/testing/__init__.py
+-rw-r--r--   0        0        0     3212 2023-06-10 08:13:42.893099 lanarky-0.7.9/lanarky/testing/gradio.py
+-rw-r--r--   0        0        0      391 2023-06-10 08:13:42.893099 lanarky-0.7.9/lanarky/testing/settings.py
+-rw-r--r--   0        0        0       73 2023-06-10 08:13:42.893099 lanarky-0.7.9/lanarky/websockets/__init__.py
+-rw-r--r--   0        0        0     5076 2023-06-10 08:13:42.893099 lanarky-0.7.9/lanarky/websockets/base.py
+-rw-r--r--   0        0        0     1419 2023-06-10 08:13:42.893099 lanarky-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0     6663 1970-01-01 00:00:00.000000 lanarky-0.7.9/PKG-INFO
```

### Comparing `lanarky-0.7.8/LICENSE` & `lanarky-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.8/README.md` & `lanarky-0.7.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,30 @@
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/lanarky.svg)](https://pypi.org/project/lanarky/)
 
 </div>
 
 Lanarky is an open-source framework to deploy LLM applications in production. It is built on top of [FastAPI](https://github.com/tiangolo/fastapi)
 and comes with batteries included.
 
+</div>
+<details>
+<summary><strong>Table of Contents</strong></summary>
+
+- [🚀 Features](#-features)
+- [❓ Why?](#-why)
+- [💾 Installation](#-installation)
+- [🔥 Build your first LLM app](#-build-your-first-llm-app)
+- [📍 Roadmap](#-roadmap)
+- [🤩 Stargazers](#-stargazers)
+- [🤝 Contributing](#-contributing)
+- [📝 License](#-license)
+- [✨ Want to build LLM applications with us?](#-want-to-build-llm-applications-with-us)
+
+</details>
+
 ## 🚀 Features
 
 - 🌐 multi-mode token streaming
 - 💬 simple gradio chatbot UI for fast prototyping
 - 🔗 supports [LangChain](https://github.com/hwchase17/langchain) applications
 - 🗄️ multiple LLM caching strategies
 
@@ -109,7 +125,14 @@
 <a href="https://github.com/ajndkr/lanarky/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=ajndkr/lanarky" />
 </a>
 
 ## ⚖️ License
 
 The library is released under the [MIT License](https://github.com/ajndkr/lanarky/blob/main/LICENSE).
+
+## ✨ Want to build LLM applications with us?
+
+Are you interested in building LLM applications with us? We would love to hear from you! Reach out to us on
+Twitter [@lanarky_io](https://twitter.com/lanarky_io).
+
+Let's connect and explore the possibilities of working together to create amazing LLM applications with Lanarky!
```

### Comparing `lanarky-0.7.8/lanarky/callbacks/__init__.py` & `lanarky-0.7.9/lanarky/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.8/lanarky/callbacks/agents.py` & `lanarky-0.7.9/lanarky/callbacks/agents.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.8/lanarky/callbacks/base.py` & `lanarky-0.7.9/lanarky/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.8/lanarky/callbacks/llm.py` & `lanarky-0.7.9/lanarky/callbacks/llm.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.8/lanarky/callbacks/retrieval_qa.py` & `lanarky-0.7.9/lanarky/callbacks/retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.8/lanarky/register/base.py` & `lanarky-0.7.9/lanarky/register/base.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.8/lanarky/register/callbacks.py` & `lanarky-0.7.9/lanarky/register/callbacks.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.8/lanarky/responses/streaming.py` & `lanarky-0.7.9/lanarky/responses/streaming.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.8/lanarky/routing/langchain.py` & `lanarky-0.7.9/lanarky/routing/langchain.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.8/lanarky/routing/utils.py` & `lanarky-0.7.9/lanarky/routing/utils.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.8/lanarky/schemas/websockets.py` & `lanarky-0.7.9/lanarky/schemas/websockets.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.8/lanarky/testing/gradio.py` & `lanarky-0.7.9/lanarky/testing/gradio.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.8/lanarky/websockets/base.py` & `lanarky-0.7.9/lanarky/websockets/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,21 +18,28 @@
 
 
 class BaseWebsocketConnection(BaseModel):
     """Base class for websocket connections."""
 
     websocket: WebSocket = Field(...)
     chain_executor: Callable[[str], Awaitable[Any]] = Field(...)
+    connection_accepted: bool = Field(False)
 
     class Config:
         arbitrary_types_allowed = True
 
-    async def connect(self):
-        """Connect to websocket."""
-        await self.websocket.accept()
+    async def connect(self, accept_connection: bool = True):
+        if accept_connection and self.connection_accepted:
+            raise RuntimeError("Connection already accepted.")
+
+        if accept_connection:
+            """Connect to websocket."""
+            await self.websocket.accept()
+            self.connection_accepted = True
+
         while True:
             try:
                 user_message = await self.websocket.receive_text()
                 await self.websocket.send_json(
                     WebsocketResponse(
                         sender=Sender.HUMAN,
                         message=user_message,
```

### Comparing `lanarky-0.7.8/pyproject.toml` & `lanarky-0.7.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lanarky"
-version = "0.7.8"
+version = "0.7.9"
 description = "Ship production-ready LLM projects with FastAPI"
 authors = ["Ajinkya Indulkar <26824103+ajndkr@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/ajndkr/lanarky"
 repository = "https://github.com/ajndkr/lanarky"
 license = "MIT"
 packages = [{include = "lanarky"}]
```

### Comparing `lanarky-0.7.8/PKG-INFO` & `lanarky-0.7.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanarky
-Version: 0.7.8
+Version: 0.7.9
 Summary: Ship production-ready LLM projects with FastAPI
 Home-page: https://github.com/ajndkr/lanarky
 License: MIT
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -44,14 +44,30 @@
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/lanarky.svg)](https://pypi.org/project/lanarky/)
 
 </div>
 
 Lanarky is an open-source framework to deploy LLM applications in production. It is built on top of [FastAPI](https://github.com/tiangolo/fastapi)
 and comes with batteries included.
 
+</div>
+<details>
+<summary><strong>Table of Contents</strong></summary>
+
+- [🚀 Features](#-features)
+- [❓ Why?](#-why)
+- [💾 Installation](#-installation)
+- [🔥 Build your first LLM app](#-build-your-first-llm-app)
+- [📍 Roadmap](#-roadmap)
+- [🤩 Stargazers](#-stargazers)
+- [🤝 Contributing](#-contributing)
+- [📝 License](#-license)
+- [✨ Want to build LLM applications with us?](#-want-to-build-llm-applications-with-us)
+
+</details>
+
 ## 🚀 Features
 
 - 🌐 multi-mode token streaming
 - 💬 simple gradio chatbot UI for fast prototyping
 - 🔗 supports [LangChain](https://github.com/hwchase17/langchain) applications
 - 🗄️ multiple LLM caching strategies
 
@@ -139,7 +155,14 @@
   <img src="https://contrib.rocks/image?repo=ajndkr/lanarky" />
 </a>
 
 ## ⚖️ License
 
 The library is released under the [MIT License](https://github.com/ajndkr/lanarky/blob/main/LICENSE).
 
+## ✨ Want to build LLM applications with us?
+
+Are you interested in building LLM applications with us? We would love to hear from you! Reach out to us on
+Twitter [@lanarky_io](https://twitter.com/lanarky_io).
+
+Let's connect and explore the possibilities of working together to create amazing LLM applications with Lanarky!
+
```

