# Comparing `tmp/articolare-0.0.7.tar.gz` & `tmp/articolare-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "articolare-0.0.7.tar", last modified: Thu Jun 15 20:09:48 2023, max compression
+gzip compressed data, was "articolare-0.0.9.tar", last modified: Thu Jun 15 20:14:34 2023, max compression
```

## Comparing `articolare-0.0.7.tar` & `articolare-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 20:09:47.932586 articolare-0.0.7/
--rw-r--r--   0 murilosilvestre   (501) staff       (20)     1905 2023-06-15 20:09:47.931540 articolare-0.0.7/PKG-INFO
--rw-r--r--   0 murilosilvestre   (501) staff       (20)     1258 2023-06-15 19:31:12.000000 articolare-0.0.7/README.md
-drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 20:09:47.800693 articolare-0.0.7/articolare/
--rw-r--r--   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 18:50:09.000000 articolare-0.0.7/articolare/__init__.py
--rw-r--r--   0 murilosilvestre   (501) staff       (20)     3294 2023-06-15 20:09:10.000000 articolare-0.0.7/articolare/translate.py
-drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 20:09:47.921483 articolare-0.0.7/articolare.egg-info/
--rw-r--r--   0 murilosilvestre   (501) staff       (20)     1905 2023-06-15 20:09:47.000000 articolare-0.0.7/articolare.egg-info/PKG-INFO
--rw-r--r--   0 murilosilvestre   (501) staff       (20)      273 2023-06-15 20:09:47.000000 articolare-0.0.7/articolare.egg-info/SOURCES.txt
--rw-r--r--   0 murilosilvestre   (501) staff       (20)        1 2023-06-15 20:09:47.000000 articolare-0.0.7/articolare.egg-info/dependency_links.txt
--rw-r--r--   0 murilosilvestre   (501) staff       (20)      196 2023-06-15 20:09:47.000000 articolare-0.0.7/articolare.egg-info/requires.txt
--rw-r--r--   0 murilosilvestre   (501) staff       (20)       17 2023-06-15 20:09:47.000000 articolare-0.0.7/articolare.egg-info/top_level.txt
--rw-r--r--   0 murilosilvestre   (501) staff       (20)       38 2023-06-15 20:09:47.932714 articolare-0.0.7/setup.cfg
--rw-r--r--   0 murilosilvestre   (501) staff       (20)     1301 2023-06-15 20:09:10.000000 articolare-0.0.7/setup.py
-drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 20:09:47.922336 articolare-0.0.7/tests/
--rw-r--r--   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 18:50:18.000000 articolare-0.0.7/tests/__init__.py
--rw-r--r--   0 murilosilvestre   (501) staff       (20)      767 2023-06-15 19:30:26.000000 articolare-0.0.7/tests/test_client.py
+drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 20:14:34.228741 articolare-0.0.9/
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)     1905 2023-06-15 20:14:34.227146 articolare-0.0.9/PKG-INFO
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)     1258 2023-06-15 19:31:12.000000 articolare-0.0.9/README.md
+drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 20:14:33.997714 articolare-0.0.9/articolare/
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 18:50:09.000000 articolare-0.0.9/articolare/__init__.py
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)     3294 2023-06-15 20:09:10.000000 articolare-0.0.9/articolare/translate.py
+drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 20:14:34.218056 articolare-0.0.9/articolare.egg-info/
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)     1905 2023-06-15 20:14:33.000000 articolare-0.0.9/articolare.egg-info/PKG-INFO
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)      273 2023-06-15 20:14:33.000000 articolare-0.0.9/articolare.egg-info/SOURCES.txt
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)        1 2023-06-15 20:14:33.000000 articolare-0.0.9/articolare.egg-info/dependency_links.txt
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)      196 2023-06-15 20:14:33.000000 articolare-0.0.9/articolare.egg-info/requires.txt
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)       17 2023-06-15 20:14:33.000000 articolare-0.0.9/articolare.egg-info/top_level.txt
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)       38 2023-06-15 20:14:34.228883 articolare-0.0.9/setup.cfg
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)     1301 2023-06-15 20:14:01.000000 articolare-0.0.9/setup.py
+drwxr-xr-x   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 20:14:34.219007 articolare-0.0.9/tests/
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)        0 2023-06-15 18:50:18.000000 articolare-0.0.9/tests/__init__.py
+-rw-r--r--   0 murilosilvestre   (501) staff       (20)      767 2023-06-15 19:30:26.000000 articolare-0.0.9/tests/test_client.py
```

### Comparing `articolare-0.0.7/PKG-INFO` & `articolare-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: articolare
-Version: 0.0.7
+Version: 0.0.9
 Summary: Python client for the Articolare API
 Author: Murilo Silvestre
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `articolare-0.0.7/README.md` & `articolare-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `articolare-0.0.7/articolare/translate.py` & `articolare-0.0.9/articolare/translate.py`

 * *Files identical despite different names*

### Comparing `articolare-0.0.7/articolare.egg-info/PKG-INFO` & `articolare-0.0.9/articolare.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: articolare
-Version: 0.0.7
+Version: 0.0.9
 Summary: Python client for the Articolare API
 Author: Murilo Silvestre
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `articolare-0.0.7/setup.py` & `articolare-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="articolare",
-    version="0.0.7",
+    version="0.0.9",
     author="Murilo Silvestre",
     description="Python client for the Articolare API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         "requests",
```

### Comparing `articolare-0.0.7/tests/test_client.py` & `articolare-0.0.9/tests/test_client.py`

 * *Files identical despite different names*

