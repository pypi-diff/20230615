# Comparing `tmp/vastai-0.1.2.tar.gz` & `tmp/vastai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vastai-0.1.2.tar", last modified: Thu Jun 15 21:39:24 2023, max compression
+gzip compressed data, was "vastai-0.1.3.tar", last modified: Thu Jun 15 21:40:39 2023, max compression
```

## Comparing `vastai-0.1.2.tar` & `vastai-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:39:24.545748 vastai-0.1.2/
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)     1064 2023-06-15 20:54:21.000000 vastai-0.1.2/LICENSE.txt
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       38 2023-06-15 20:55:37.000000 vastai-0.1.2/MANIFEST.in
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33953 2023-06-15 21:39:24.545748 vastai-0.1.2/PKG-INFO
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33342 2023-06-15 21:37:34.000000 vastai-0.1.2/README.md
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)      641 2023-06-15 21:39:14.000000 vastai-0.1.2/pyproject.toml
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       38 2023-06-15 21:39:24.545748 vastai-0.1.2/setup.cfg
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)     1054 2023-06-15 21:20:12.000000 vastai-0.1.2/setup.py
-drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:39:24.545748 vastai-0.1.2/vastai/
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:02:15.000000 vastai-0.1.2/vastai/__init__.py
--rwxrwxr-x   0 jcannell  (1000) jcannell  (1000)    75501 2023-06-15 20:33:35.000000 vastai-0.1.2/vastai/vast.py
-drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:39:24.545748 vastai-0.1.2/vastai.egg-info/
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33953 2023-06-15 21:39:24.000000 vastai-0.1.2/vastai.egg-info/PKG-INFO
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)      283 2023-06-15 21:39:24.000000 vastai-0.1.2/vastai.egg-info/SOURCES.txt
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        1 2023-06-15 21:39:24.000000 vastai-0.1.2/vastai.egg-info/dependency_links.txt
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       44 2023-06-15 21:39:24.000000 vastai-0.1.2/vastai.egg-info/entry_points.txt
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        9 2023-06-15 21:39:24.000000 vastai-0.1.2/vastai.egg-info/requires.txt
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        7 2023-06-15 21:39:24.000000 vastai-0.1.2/vastai.egg-info/top_level.txt
+drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:40:39.157441 vastai-0.1.3/
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)     1064 2023-06-15 20:54:21.000000 vastai-0.1.3/LICENSE.txt
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       38 2023-06-15 20:55:37.000000 vastai-0.1.3/MANIFEST.in
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33954 2023-06-15 21:40:39.157441 vastai-0.1.3/PKG-INFO
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33343 2023-06-15 21:40:11.000000 vastai-0.1.3/README.md
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)      641 2023-06-15 21:40:32.000000 vastai-0.1.3/pyproject.toml
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       38 2023-06-15 21:40:39.157441 vastai-0.1.3/setup.cfg
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)     1054 2023-06-15 21:20:12.000000 vastai-0.1.3/setup.py
+drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:40:39.157441 vastai-0.1.3/vastai/
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:02:15.000000 vastai-0.1.3/vastai/__init__.py
+-rwxrwxr-x   0 jcannell  (1000) jcannell  (1000)    75501 2023-06-15 20:33:35.000000 vastai-0.1.3/vastai/vast.py
+drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:40:39.157441 vastai-0.1.3/vastai.egg-info/
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33954 2023-06-15 21:40:39.000000 vastai-0.1.3/vastai.egg-info/PKG-INFO
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)      283 2023-06-15 21:40:39.000000 vastai-0.1.3/vastai.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        1 2023-06-15 21:40:39.000000 vastai-0.1.3/vastai.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       44 2023-06-15 21:40:39.000000 vastai-0.1.3/vastai.egg-info/entry_points.txt
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        9 2023-06-15 21:40:39.000000 vastai-0.1.3/vastai.egg-info/requires.txt
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        7 2023-06-15 21:40:39.000000 vastai-0.1.3/vastai.egg-info/top_level.txt
```

### Comparing `vastai-0.1.2/LICENSE.txt` & `vastai-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vastai-0.1.2/PKG-INFO` & `vastai-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastai
-Version: 0.1.2
+Version: 0.1.3
 Summary: Vast.ai Python CLI
 Home-page: https://github.com/vast-ai/vast-python
 Author: Vast.ai
 Author-email: "vast.ai" <support@vast.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/vast-ai/vast-python
 Project-URL: Bug Tracker, https://github.com/vast-ai/vast-python/issues
@@ -25,15 +25,15 @@
 You can find usage examples and documentation for the VastAI Python library in our [API reference](https://vast.ai/docs/command-line-interface/overview-and-quickstart) and the code itself on our [github repository](https://github.com/vast-ai/vast-python).
 
 
 ## Installation
 
 To update or install the package, just run:
 
-```pip install--upgrade vastai```
+```pip install --upgrade vastai```
 
 Install from source with:
 
 ```python setup.py install```
 
 
 ## Usage
```

### Comparing `vastai-0.1.2/README.md` & `vastai-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 You can find usage examples and documentation for the VastAI Python library in our [API reference](https://vast.ai/docs/command-line-interface/overview-and-quickstart) and the code itself on our [github repository](https://github.com/vast-ai/vast-python).
 
 
 ## Installation
 
 To update or install the package, just run:
 
-```pip install--upgrade vastai```
+```pip install --upgrade vastai```
 
 Install from source with:
 
 ```python setup.py install```
 
 
 ## Usage
```

### Comparing `vastai-0.1.2/pyproject.toml` & `vastai-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vastai"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="vast.ai", email="support@vast.ai" },
 ]
 description = "Vast.ai Python CLI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `vastai-0.1.2/setup.py` & `vastai-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `vastai-0.1.2/vastai/vast.py` & `vastai-0.1.3/vastai/vast.py`

 * *Files identical despite different names*

### Comparing `vastai-0.1.2/vastai.egg-info/PKG-INFO` & `vastai-0.1.3/vastai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastai
-Version: 0.1.2
+Version: 0.1.3
 Summary: Vast.ai Python CLI
 Home-page: https://github.com/vast-ai/vast-python
 Author: Vast.ai
 Author-email: "vast.ai" <support@vast.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/vast-ai/vast-python
 Project-URL: Bug Tracker, https://github.com/vast-ai/vast-python/issues
@@ -25,15 +25,15 @@
 You can find usage examples and documentation for the VastAI Python library in our [API reference](https://vast.ai/docs/command-line-interface/overview-and-quickstart) and the code itself on our [github repository](https://github.com/vast-ai/vast-python).
 
 
 ## Installation
 
 To update or install the package, just run:
 
-```pip install--upgrade vastai```
+```pip install --upgrade vastai```
 
 Install from source with:
 
 ```python setup.py install```
 
 
 ## Usage
```

