# Comparing `tmp/articolare-0.0.4.tar.gz` & `tmp/articolare-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "articolare-0.0.4.tar", last modified: Thu Jun 15 19:39:31 2023, max compression
+gzip compressed data, was "articolare-0.0.5.tar", last modified: Thu Jun 15 19:49:58 2023, max compression
```

## Comparing `articolare-0.0.4.tar` & `articolare-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 19:39:31.069499 articolare-0.0.4/
--rw-r--r--   0 murilosilvestre   (501) staff       (20)     1905 2023-06-15 19:39:31.067862 articolare-0.0.4/PKG-INFO
--rw-r--r--   0 murilosilvestre   (501) staff       (20)     1258 2023-06-15 19:31:12.000000 articolare-0.0.4/README.md
-drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 19:39:30.876438 articolare-0.0.4/articolare/
--rw-r--r--   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 18:50:09.000000 articolare-0.0.4/articolare/__init__.py
--rw-r--r--   0 murilosilvestre   (501) staff       (20)     3300 2023-06-15 18:56:46.000000 articolare-0.0.4/articolare/translate.py
-drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 19:39:31.023364 articolare-0.0.4/articolare.egg-info/
--rw-r--r--   0 murilosilvestre   (501) staff       (20)     1905 2023-06-15 19:39:30.000000 articolare-0.0.4/articolare.egg-info/PKG-INFO
--rw-r--r--   0 murilosilvestre   (501) staff       (20)      273 2023-06-15 19:39:30.000000 articolare-0.0.4/articolare.egg-info/SOURCES.txt
--rw-r--r--   0 murilosilvestre   (501) staff       (20)        1 2023-06-15 19:39:30.000000 articolare-0.0.4/articolare.egg-info/dependency_links.txt
--rw-r--r--   0 murilosilvestre   (501) staff       (20)      196 2023-06-15 19:39:30.000000 articolare-0.0.4/articolare.egg-info/requires.txt
--rw-r--r--   0 murilosilvestre   (501) staff       (20)       17 2023-06-15 19:39:30.000000 articolare-0.0.4/articolare.egg-info/top_level.txt
--rw-r--r--   0 murilosilvestre   (501) staff       (20)       38 2023-06-15 19:39:31.069699 articolare-0.0.4/setup.cfg
--rw-r--r--   0 murilosilvestre   (501) staff       (20)     1301 2023-06-15 19:25:49.000000 articolare-0.0.4/setup.py
-drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 19:39:31.024191 articolare-0.0.4/tests/
--rw-r--r--   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 18:50:18.000000 articolare-0.0.4/tests/__init__.py
--rw-r--r--   0 murilosilvestre   (501) staff       (20)      767 2023-06-15 19:30:26.000000 articolare-0.0.4/tests/test_client.py
+drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 19:49:58.301595 articolare-0.0.5/
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)     1905 2023-06-15 19:49:58.300659 articolare-0.0.5/PKG-INFO
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)     1258 2023-06-15 19:31:12.000000 articolare-0.0.5/README.md
+drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 19:49:58.297963 articolare-0.0.5/articolare/
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 18:50:09.000000 articolare-0.0.5/articolare/__init__.py
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)     3300 2023-06-15 19:47:44.000000 articolare-0.0.5/articolare/translate.py
+drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 19:49:58.299624 articolare-0.0.5/articolare.egg-info/
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)     1905 2023-06-15 19:49:58.000000 articolare-0.0.5/articolare.egg-info/PKG-INFO
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)      273 2023-06-15 19:49:58.000000 articolare-0.0.5/articolare.egg-info/SOURCES.txt
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)        1 2023-06-15 19:49:58.000000 articolare-0.0.5/articolare.egg-info/dependency_links.txt
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)      196 2023-06-15 19:49:58.000000 articolare-0.0.5/articolare.egg-info/requires.txt
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)       17 2023-06-15 19:49:58.000000 articolare-0.0.5/articolare.egg-info/top_level.txt
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)       38 2023-06-15 19:49:58.301712 articolare-0.0.5/setup.cfg
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)     1301 2023-06-15 19:49:50.000000 articolare-0.0.5/setup.py
+drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 19:49:58.300186 articolare-0.0.5/tests/
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 18:50:18.000000 articolare-0.0.5/tests/__init__.py
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)      767 2023-06-15 19:30:26.000000 articolare-0.0.5/tests/test_client.py
```

### Comparing `articolare-0.0.4/PKG-INFO` & `articolare-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: articolare
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python client for the Articolare API
 Author: Murilo Silvestre
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `articolare-0.0.4/README.md` & `articolare-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `articolare-0.0.4/articolare/translate.py` & `articolare-0.0.5/articolare/translate.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,23 +53,23 @@
         dict: The response data.
 
         Raises:
         requests.HTTPError: If the API request fails.
         """
         if not isinstance(model, str):
             raise TypeError("model must be a string.")
-        if lang not in ["English", "Portuguese", "Spanish", "Italian"]:
+        if lang not in ["english", "portuguese", "spanish", "italian"]:
             raise ValueError("Invalid language. Supported languages are English, Portuguese, Spanish, or Italian.")
-        if style not in ["Conversation Formal", "Conversation Informal", "Documents"]:
+        if style not in ["conversation formal", "conversation informal", "documents"]:
             raise ValueError("Invalid style. Supported styles are conversation, formal, or informal.")
         if not isinstance(prompt, str):
             raise TypeError("prompt must be a string.")
         if not isinstance(max_tokens, int):
             raise TypeError("max_tokens must be an integer.")
-        if dialect not in ["Latam", "European"] :
+        if dialect not in ["latam", "european"] :
             raise ValueError("Invalid dialect. Supported dialects are Latam and European.")
 
         data = {
             "model": model,
             "lang": lang,
             "style": style,
             "dialect": dialect,
```

### Comparing `articolare-0.0.4/articolare.egg-info/PKG-INFO` & `articolare-0.0.5/articolare.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: articolare
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python client for the Articolare API
 Author: Murilo Silvestre
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `articolare-0.0.4/setup.py` & `articolare-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="articolare",
-    version="0.0.4",
+    version="0.0.5",
     author="Murilo Silvestre",
     description="Python client for the Articolare API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         "requests",
```

### Comparing `articolare-0.0.4/tests/test_client.py` & `articolare-0.0.5/tests/test_client.py`

 * *Files identical despite different names*

