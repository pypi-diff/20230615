# Comparing `tmp/nteu_corporate_engine-0.1.8.tar.gz` & `tmp/nteu_corporate_engine-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nteu_corporate_engine-0.1.8.tar", last modified: Thu Mar 11 16:05:18 2021, max compression
+gzip compressed data, was "nteu_corporate_engine-0.1.9.tar", max compression
```

## Comparing `nteu_corporate_engine-0.1.8.tar` & `nteu_corporate_engine-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-10-20 13:55:48.276578 nteu_corporate_engine-0.1.8/nteu_corporate_engine/__init__.py
--rw-r--r--   0        0        0     4709 2020-11-24 10:05:35.202408 nteu_corporate_engine-0.1.8/nteu_corporate_engine/engine.py
--rw-r--r--   0        0        0     5690 2021-02-05 12:44:10.189802 nteu_corporate_engine-0.1.8/nteu_corporate_engine/pipeline.py
--rw-r--r--   0        0        0     3512 2020-11-24 10:05:35.206408 nteu_corporate_engine-0.1.8/nteu_corporate_engine/server.py
--rw-r--r--   0        0        0      547 2021-03-11 16:03:55.460724 nteu_corporate_engine-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      783 2021-03-11 16:05:18.145953 nteu_corporate_engine-0.1.8/setup.py
--rw-r--r--   0        0        0      637 2021-03-11 16:05:18.146314 nteu_corporate_engine-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2021-12-29 15:02:17.636250 nteu_corporate_engine-0.1.9/nteu_corporate_engine/__init__.py
+-rw-r--r--   0        0        0     5621 2022-01-20 15:39:53.128527 nteu_corporate_engine-0.1.9/nteu_corporate_engine/engine.py
+-rw-r--r--   0        0        0     5690 2021-12-29 15:02:17.636250 nteu_corporate_engine-0.1.9/nteu_corporate_engine/pipeline.py
+-rw-r--r--   0        0        0     3512 2021-12-29 15:02:17.636250 nteu_corporate_engine-0.1.9/nteu_corporate_engine/server.py
+-rw-r--r--   0        0        0      547 2022-01-20 15:40:21.304529 nteu_corporate_engine-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      783 2022-01-20 15:54:11.241761 nteu_corporate_engine-0.1.9/setup.py
+-rw-r--r--   0        0        0      688 2022-01-20 15:54:11.241944 nteu_corporate_engine-0.1.9/PKG-INFO
```

### Comparing `nteu_corporate_engine-0.1.8/nteu_corporate_engine/engine.py` & `nteu_corporate_engine-0.1.9/nteu_corporate_engine/engine.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,19 +31,35 @@
         else:
             msg = f"Loading Model -> {name} with arguments {args}."
         logging.info(msg)
         translation_model = TranslationModelFactory.get_class(name)
         return translation_model(model_path, **args)
 
     async def translate(self, srcs: List, n_best: int = 1):
-        translations = self._model.translate(srcs, n_best=n_best)
-        result = []
-        for translation in translations:
-            self.log_translation(translation)
-            result.append(translation.pred_sents[0].sentence)
+        if self._config["translation_model"]["name"] == "onmt":
+            translations = self._model.translate(srcs, n_best=n_best)
+            result = []
+            for translation in translations:
+                self.log_translation(translation)
+                result.append(translation.pred_sents[0].sentence)
+        elif self._config["translation_model"]["name"] == "marianmt":
+            args_dec = self._config["translation_model"]["args_decoding"]
+            if not args_dec["in_training_servers"]:
+                result = self._model.translate(srcs, n_best=n_best)
+            else:
+                model_path = self._config["translation_engine_server"]["model_path"]
+                marian_path = self._config["translation_model"]["marian_path"]
+                if self._config["translation_engine_server"]["gpu"]:
+                    gpu = "0"
+                else:
+                    gpu = None
+                result = self._model.translate_training_servers(srcs,\
+                                        model_path, marian_path, gpu)
+            for translation in result:
+                self.log_translation(translation)
         return result
 
     async def process_batch(self, batch: List, lock: Lock = None):
         srcs = []
         segs = []
         ans = []
         for src in batch:
```

### Comparing `nteu_corporate_engine-0.1.8/nteu_corporate_engine/pipeline.py` & `nteu_corporate_engine-0.1.9/nteu_corporate_engine/pipeline.py`

 * *Files identical despite different names*

### Comparing `nteu_corporate_engine-0.1.8/nteu_corporate_engine/server.py` & `nteu_corporate_engine-0.1.9/nteu_corporate_engine/server.py`

 * *Files identical despite different names*

### Comparing `nteu_corporate_engine-0.1.8/pyproject.toml` & `nteu_corporate_engine-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nteu_corporate_engine"
-version = "0.1.8"
+version = "0.1.9"
 description = "NTEU model wrapper for corporate injection"
 authors = ["Your Name <you@example.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 aiohttp = "^3.6.3"
 pangeamt-nlp = "^1.0.0"
```

### Comparing `nteu_corporate_engine-0.1.8/setup.py` & `nteu_corporate_engine-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'pangeamt-nlp>=1.0.0,<2.0.0',
  'pangeamt-toolkit>=3.57.0,<4.0.0',
  'prettytable>=1.0.1,<2.0.0',
  'torch==1.5.0']
 
 setup_kwargs = {
     'name': 'nteu-corporate-engine',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'NTEU model wrapper for corporate injection',
     'long_description': None,
     'author': 'Your Name',
     'author_email': 'you@example.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `nteu_corporate_engine-0.1.8/PKG-INFO` & `nteu_corporate_engine-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: nteu-corporate-engine
-Version: 0.1.8
+Version: 0.1.9
 Summary: NTEU model wrapper for corporate injection
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: OpenNMT-py (==1.1.0)
 Requires-Dist: aiohttp (>=3.6.3,<4.0.0)
 Requires-Dist: pangeamt-nlp (>=1.0.0,<2.0.0)
 Requires-Dist: pangeamt-toolkit (>=3.57.0,<4.0.0)
```

