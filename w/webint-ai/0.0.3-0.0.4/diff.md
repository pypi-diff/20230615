# Comparing `tmp/webint_ai-0.0.3.tar.gz` & `tmp/webint_ai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webint_ai-0.0.3.tar", max compression
+gzip compressed data, was "webint_ai-0.0.4.tar", max compression
```

## Comparing `webint_ai-0.0.3.tar` & `webint_ai-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      623 2023-05-17 18:22:26.621543 webint_ai-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3865 2023-05-17 01:45:45.623398 webint_ai-0.0.3/webint_ai/__init__.py
--rw-r--r--   0        0        0      156 2023-03-21 01:32:45.174619 webint_ai-0.0.3/webint_ai/templates/__init__.py
--rw-r--r--   0        0        0       84 2023-03-20 23:10:50.085902 webint_ai-0.0.3/webint_ai/templates/chat.html
--rw-r--r--   0        0        0      433 2023-03-21 02:37:31.970964 webint_ai-0.0.3/webint_ai/templates/chat_response.html
--rw-r--r--   0        0        0      367 2023-03-22 00:34:09.529026 webint_ai-0.0.3/webint_ai/templates/index.html
--rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 webint_ai-0.0.3/setup.py
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 webint_ai-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      623 2023-06-15 00:51:58.571102 webint_ai-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3953 2023-06-14 20:05:20.564122 webint_ai-0.0.4/webint_ai/__init__.py
+-rw-r--r--   0        0        0      156 2023-03-21 01:32:45.174619 webint_ai-0.0.4/webint_ai/templates/__init__.py
+-rw-r--r--   0        0        0       84 2023-03-20 23:10:50.085902 webint_ai-0.0.4/webint_ai/templates/chat.html
+-rw-r--r--   0        0        0      433 2023-03-21 02:37:31.970964 webint_ai-0.0.4/webint_ai/templates/chat_response.html
+-rw-r--r--   0        0        0      367 2023-03-22 00:34:09.529026 webint_ai-0.0.4/webint_ai/templates/index.html
+-rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 webint_ai-0.0.4/setup.py
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 webint_ai-0.0.4/PKG-INFO
```

### Comparing `webint_ai-0.0.3/pyproject.toml` & `webint_ai-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webint-ai"
-version = "0.0.3"
+version = "0.0.4"
 description = "interface artificial intelligence"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "AGPL-3.0-or-later"
 packages = [{include = "webint_ai"}]
 
 [tool.poetry.plugins."webapps"]
 ai = "webint_ai:app"
```

### Comparing `webint_ai-0.0.3/webint_ai/__init__.py` & `webint_ai-0.0.4/webint_ai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 """Interface artificial intelligence."""
 
 import collections
+import functools
 import random
 import re
 import textwrap
 
 import black
 import openai
 import requests
 import web
 import webagt
 
 app = web.application(__name__, prefix="ai")
 ELEVENLABS_API = "https://api.elevenlabs.io/v1"
 ELEVENLABS_KEY = app.cfg.get("ELEVENLABS")
-ANGELO = [
-    v
-    for v in requests.get(
-        f"{ELEVENLABS_API}/voices",
-        headers={"Accept": "application/json", "xi-api-key": ELEVENLABS_KEY},
-    ).json()["voices"]
-    if v["name"] == "Angelo"
-][0]["voice_id"]
 openai.api_key = app.cfg.get("OPENAI")
 
 
+@functools.cache
+def get_voice():
+    return [
+        v
+        for v in requests.get(
+            f"{ELEVENLABS_API}/voices",
+            headers={"Accept": "application/json", "xi-api-key": ELEVENLABS_KEY},
+        ).json()["voices"]
+        if v["name"] == "Angelo"
+    ][0]["voice_id"]
+
+
 @app.control("")
 class AI:
     """AI."""
 
     def get(self):
         """Return an index of data sources."""
         models = openai.Model.list()
@@ -114,15 +119,15 @@
                 {"role": "user", "content": prompt},
             ],
             max_tokens=500,
         )
         response_text = response.choices[0].message.content
         print(response_text)
         audio = requests.post(
-            f"{ELEVENLABS_API}/text-to-speech/{ANGELO}/stream",
+            f"{ELEVENLABS_API}/text-to-speech/{get_voice()}/stream",
             headers={
                 "Accept": "audio/mpeg",
                 "Content-Type": "application/json",
                 "xi-api-key": ELEVENLABS_KEY,
             },
             json={
                 "text": response_text,
```

### Comparing `webint_ai-0.0.3/setup.py` & `webint_ai-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['markdown>=3.4.1,<4.0.0', 'openai>=0.27.2,<0.28.0', 'webint>=0.0']
 
 entry_points = \
 {'webapps': ['ai = webint_ai:app']}
 
 setup_kwargs = {
     'name': 'webint-ai',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'interface artificial intelligence',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `webint_ai-0.0.3/PKG-INFO` & `webint_ai-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webint-ai
-Version: 0.0.3
+Version: 0.0.4
 Summary: interface artificial intelligence
 License: AGPL-3.0-or-later
 Author: Angelo Gladding
 Author-email: angelo@ragt.ag
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

