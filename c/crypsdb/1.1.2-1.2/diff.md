# Comparing `tmp/crypsdb-1.1.2.tar.gz` & `tmp/crypsdb-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypsdb-1.1.2.tar", last modified: Thu Jun 15 16:56:58 2023, max compression
+gzip compressed data, was "crypsdb-1.2.tar", last modified: Thu Jun 15 16:50:12 2023, max compression
```

## Comparing `crypsdb-1.1.2.tar` & `crypsdb-1.2.tar`

### file list

```diff
@@ -1,12 +1,10 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-15 16:56:58.095967 crypsdb-1.1.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      656 2023-06-15 16:56:58.095967 crypsdb-1.1.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2023-06-15 16:49:42.000000 crypsdb-1.1.2/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-15 16:56:58.091967 crypsdb-1.1.2/crypsdb/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15979 2023-06-15 16:48:21.000000 crypsdb-1.1.2/crypsdb/crypsdb.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-15 16:56:58.095967 crypsdb-1.1.2/crypsdb.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      656 2023-06-15 16:56:58.000000 crypsdb-1.1.2/crypsdb.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      161 2023-06-15 16:56:58.000000 crypsdb-1.1.2/crypsdb.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-15 16:56:58.000000 crypsdb-1.1.2/crypsdb.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       16 2023-06-15 16:56:58.000000 crypsdb-1.1.2/crypsdb.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-15 16:56:58.095967 crypsdb-1.1.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      667 2023-06-15 16:56:20.000000 crypsdb-1.1.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-15 16:50:12.085212 crypsdb-1.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      654 2023-06-15 16:50:12.085212 crypsdb-1.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2023-06-15 16:49:42.000000 crypsdb-1.2/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-15 16:50:12.085212 crypsdb-1.2/crypsdb.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      654 2023-06-15 16:50:12.000000 crypsdb-1.2/crypsdb.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      142 2023-06-15 16:50:12.000000 crypsdb-1.2/crypsdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-15 16:50:12.000000 crypsdb-1.2/crypsdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-06-15 16:50:12.000000 crypsdb-1.2/crypsdb.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-15 16:50:12.085212 crypsdb-1.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      657 2023-06-15 16:49:47.000000 crypsdb-1.2/setup.py
```

### Comparing `crypsdb-1.1.2/PKG-INFO` & `crypsdb-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypsdb
-Version: 1.1.2
+Version: 1.2
 Summary: A lightweight JSON-based database system for Python
 Home-page: https://github.com/E491K8/crypsDb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `crypsdb-1.1.2/crypsdb.egg-info/PKG-INFO` & `crypsdb-1.2/crypsdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypsdb
-Version: 1.1.2
+Version: 1.2
 Summary: A lightweight JSON-based database system for Python
 Home-page: https://github.com/E491K8/crypsDb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `crypsdb-1.1.2/setup.py` & `crypsdb-1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="crypsdb",
-    version="1.1.2",
+    version="1.2",
     author="Pawan kumar",
     author_email="control@vvfin.in",
     description="A lightweight JSON-based database system for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/E491K8/crypsDb",
     packages=find_packages(),
-    py_modules=['crypsdb/crypsdb'],
+    py_modules=['crypsdb'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

