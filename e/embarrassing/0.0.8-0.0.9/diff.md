# Comparing `tmp/embarrassing-0.0.8.tar.gz` & `tmp/embarrassing-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embarrassing-0.0.8.tar", last modified: Thu Jun 15 02:58:52 2023, max compression
+gzip compressed data, was "embarrassing-0.0.9.tar", last modified: Thu Jun 15 03:05:10 2023, max compression
```

## Comparing `embarrassing-0.0.8.tar` & `embarrassing-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 02:58:52.512090 embarrassing-0.0.8/
--rw-rw-rw-   0        0        0     2006 2023-06-15 02:58:52.511136 embarrassing-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1567 2023-06-15 02:58:14.000000 embarrassing-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 02:58:52.498134 embarrassing-0.0.8/embarrassing/
--rw-rw-rw-   0        0        0       60 2023-06-15 02:39:01.000000 embarrassing-0.0.8/embarrassing/__init__.py
--rw-rw-rw-   0        0        0      399 2023-06-15 01:44:17.000000 embarrassing-0.0.8/embarrassing/main.py
-drwxrwxrwx   0        0        0        0 2023-06-15 02:58:52.509144 embarrassing-0.0.8/embarrassing.egg-info/
--rw-rw-rw-   0        0        0     2006 2023-06-15 02:58:52.000000 embarrassing-0.0.8/embarrassing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-15 02:58:52.000000 embarrassing-0.0.8/embarrassing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 02:58:52.000000 embarrassing-0.0.8/embarrassing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-15 02:58:52.000000 embarrassing-0.0.8/embarrassing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-15 02:58:52.000000 embarrassing-0.0.8/embarrassing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 02:58:52.513094 embarrassing-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      804 2023-06-15 02:58:21.000000 embarrassing-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 03:05:10.774525 embarrassing-0.0.9/
+-rw-rw-rw-   0        0        0     2008 2023-06-15 03:05:10.773525 embarrassing-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1569 2023-06-15 03:04:51.000000 embarrassing-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 03:05:10.760553 embarrassing-0.0.9/embarrassing/
+-rw-rw-rw-   0        0        0       60 2023-06-15 02:39:01.000000 embarrassing-0.0.9/embarrassing/__init__.py
+-rw-rw-rw-   0        0        0      399 2023-06-15 01:44:17.000000 embarrassing-0.0.9/embarrassing/main.py
+drwxrwxrwx   0        0        0        0 2023-06-15 03:05:10.771528 embarrassing-0.0.9/embarrassing.egg-info/
+-rw-rw-rw-   0        0        0     2008 2023-06-15 03:05:10.000000 embarrassing-0.0.9/embarrassing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-15 03:05:10.000000 embarrassing-0.0.9/embarrassing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 03:05:10.000000 embarrassing-0.0.9/embarrassing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-15 03:05:10.000000 embarrassing-0.0.9/embarrassing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-15 03:05:10.000000 embarrassing-0.0.9/embarrassing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 03:05:10.774525 embarrassing-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      804 2023-06-15 03:05:08.000000 embarrassing-0.0.9/setup.py
```

### Comparing `embarrassing-0.0.8/PKG-INFO` & `embarrassing-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: embarrassing
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package to embarrassingly parallelize your code
 Author: Raphaël Côté
 Author-email: cotlarrc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Embarrassing
 
-[![PyPI version](https://badge.fury.io/py/embarrassing.svg)](https://badge.fury.io/py/my_package)
+[![PyPI version](https://badge.fury.io/py/embarrassing.svg)](https://badge.fury.io/py/embarrassing)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 A brief description of your package.
 
 ## Installation
 
 You can install embarrassing using pip:
```

### Comparing `embarrassing-0.0.8/README.md` & `embarrassing-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Embarrassing
 
-[![PyPI version](https://badge.fury.io/py/embarrassing.svg)](https://badge.fury.io/py/my_package)
+[![PyPI version](https://badge.fury.io/py/embarrassing.svg)](https://badge.fury.io/py/embarrassing)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 A brief description of your package.
 
 ## Installation
 
 You can install embarrassing using pip:
```

### Comparing `embarrassing-0.0.8/embarrassing.egg-info/PKG-INFO` & `embarrassing-0.0.9/embarrassing.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: embarrassing
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package to embarrassingly parallelize your code
 Author: Raphaël Côté
 Author-email: cotlarrc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Embarrassing
 
-[![PyPI version](https://badge.fury.io/py/embarrassing.svg)](https://badge.fury.io/py/my_package)
+[![PyPI version](https://badge.fury.io/py/embarrassing.svg)](https://badge.fury.io/py/embarrassing)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 A brief description of your package.
 
 ## Installation
 
 You can install embarrassing using pip:
```

### Comparing `embarrassing-0.0.8/setup.py` & `embarrassing-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="embarrassing",
-    version="0.0.8",
+    version="0.0.9",
     description="A package to embarrassingly parallelize your code",
     author="Raphaël Côté",
     author_email="cotlarrc@gmail.com",
     long_description=long_description,
     long_description_content_type='text/markdown',
     # url="<package-url>",
     packages=find_packages(),
```

