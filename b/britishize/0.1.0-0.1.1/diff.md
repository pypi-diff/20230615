# Comparing `tmp/britishize-0.1.0.tar.gz` & `tmp/britishize-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "britishize-0.1.0.tar", max compression
+gzip compressed data, was "britishize-0.1.1.tar", max compression
```

## Comparing `britishize-0.1.0.tar` & `britishize-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      318 2023-06-15 14:17:19.133936 britishize-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       21 2023-06-15 14:17:08.439865 britishize-0.1.0/readme.md
--rw-r--r--   0        0        0     1539 2023-06-15 14:10:53.321684 britishize-0.1.0/src/britishize/britishize.py
--rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 britishize-0.1.0/setup.py
--rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 britishize-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      318 2023-06-15 14:23:55.092237 britishize-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-15 14:17:08.439865 britishize-0.1.1/readme.md
+-rw-r--r--   0        0        0     1539 2023-06-15 14:10:53.321684 britishize-0.1.1/src/britishize/britishize.py
+-rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 britishize-0.1.1/setup.py
+-rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 britishize-0.1.1/PKG-INFO
```

### Comparing `britishize-0.1.0/src/britishize/britishize.py` & `britishize-0.1.1/src/britishize/britishize.py`

 * *Files identical despite different names*

### Comparing `britishize-0.1.0/setup.py` & `britishize-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['britishize']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'britishize',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Write poorer english',
     'long_description': 'Write proper english\n',
     'author': 'Antonio Feregrino',
     'author_email': 'antonio.feregrino@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `britishize-0.1.0/PKG-INFO` & `britishize-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: britishize
-Version: 0.1.0
+Version: 0.1.1
 Summary: Write poorer english
 License: MIT
 Author: Antonio Feregrino
 Author-email: antonio.feregrino@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

