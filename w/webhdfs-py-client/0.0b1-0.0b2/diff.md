# Comparing `tmp/webhdfs-py-client-0.0b1.tar.gz` & `tmp/webhdfs-py-client-0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webhdfs-py-client-0.0b1.tar", last modified: Thu Jun 15 19:34:42 2023, max compression
+gzip compressed data, was "webhdfs-py-client-0.0b2.tar", last modified: Thu Jun 15 19:36:34 2023, max compression
```

## Comparing `webhdfs-py-client-0.0b1.tar` & `webhdfs-py-client-0.0b2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 19:34:44.000000 webhdfs-py-client-0.0b1/
--rw-rw-rw-   0        0        0     3494 2023-06-15 19:34:44.000000 webhdfs-py-client-0.0b1/PKG-INFO
--rw-rw-rw-   0        0        0     2756 2023-06-07 20:51:38.000000 webhdfs-py-client-0.0b1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 19:34:44.000000 webhdfs-py-client-0.0b1/setup.cfg
--rw-rw-rw-   0        0        0     1643 2023-06-15 19:34:32.000000 webhdfs-py-client-0.0b1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:34:44.000000 webhdfs-py-client-0.0b1/src/
-drwxrwxrwx   0        0        0        0 2023-06-15 19:34:44.000000 webhdfs-py-client-0.0b1/src/webhdfs_py/
--rw-rw-rw-   0        0        0       35 2023-06-15 16:19:56.000000 webhdfs-py-client-0.0b1/src/webhdfs_py/__init__.py
--rw-rw-rw-   0        0        0      493 2023-06-01 19:50:36.000000 webhdfs-py-client-0.0b1/src/webhdfs_py/errors.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:34:44.000000 webhdfs-py-client-0.0b1/src/webhdfs_py/example/
--rw-rw-rw-   0        0        0        0 2023-06-15 14:38:50.000000 webhdfs-py-client-0.0b1/src/webhdfs_py/example/__init__.py
--rw-rw-rw-   0        0        0     2483 2023-06-15 15:14:52.000000 webhdfs-py-client-0.0b1/src/webhdfs_py/example/example.py
--rw-rw-rw-   0        0        0     1160 2023-06-01 02:02:20.000000 webhdfs-py-client-0.0b1/src/webhdfs_py/example/hello.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:34:44.000000 webhdfs-py-client-0.0b1/src/webhdfs_py/example/pages/
--rw-rw-rw-   0        0        0     1648 2023-06-15 17:57:58.000000 webhdfs-py-client-0.0b1/src/webhdfs_py/example/pages/dataframe.py
--rw-rw-rw-   0        0        0      360 2023-06-15 14:45:00.000000 webhdfs-py-client-0.0b1/src/webhdfs_py/example/run.py
--rw-rw-rw-   0        0        0      390 2023-06-01 02:08:52.000000 webhdfs-py-client-0.0b1/src/webhdfs_py/example/utils.py
--rw-rw-rw-   0        0        0      406 2023-06-07 19:36:30.000000 webhdfs-py-client-0.0b1/src/webhdfs_py/operations.py
--rw-rw-rw-   0        0        0    27361 2023-06-15 15:14:52.000000 webhdfs-py-client-0.0b1/src/webhdfs_py/webhdfs.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:34:44.000000 webhdfs-py-client-0.0b1/src/webhdfs_py_client.egg-info/
--rw-rw-rw-   0        0        0     3494 2023-06-15 19:34:42.000000 webhdfs-py-client-0.0b1/src/webhdfs_py_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      554 2023-06-15 19:34:42.000000 webhdfs-py-client-0.0b1/src/webhdfs_py_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 19:34:42.000000 webhdfs-py-client-0.0b1/src/webhdfs_py_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-15 19:34:42.000000 webhdfs-py-client-0.0b1/src/webhdfs_py_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-15 19:34:42.000000 webhdfs-py-client-0.0b1/src/webhdfs_py_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 19:36:34.000000 webhdfs-py-client-0.0b2/
+-rw-rw-rw-   0        0        0     3494 2023-06-15 19:36:36.000000 webhdfs-py-client-0.0b2/PKG-INFO
+-rw-rw-rw-   0        0        0     2756 2023-06-07 20:51:38.000000 webhdfs-py-client-0.0b2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 19:36:36.000000 webhdfs-py-client-0.0b2/setup.cfg
+-rw-rw-rw-   0        0        0     1639 2023-06-15 19:36:14.000000 webhdfs-py-client-0.0b2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:36:34.000000 webhdfs-py-client-0.0b2/src/
+drwxrwxrwx   0        0        0        0 2023-06-15 19:36:34.000000 webhdfs-py-client-0.0b2/src/webhdfs_py/
+-rw-rw-rw-   0        0        0       35 2023-06-15 16:19:56.000000 webhdfs-py-client-0.0b2/src/webhdfs_py/__init__.py
+-rw-rw-rw-   0        0        0      493 2023-06-01 19:50:36.000000 webhdfs-py-client-0.0b2/src/webhdfs_py/errors.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:36:36.000000 webhdfs-py-client-0.0b2/src/webhdfs_py/example/
+-rw-rw-rw-   0        0        0        0 2023-06-15 14:38:50.000000 webhdfs-py-client-0.0b2/src/webhdfs_py/example/__init__.py
+-rw-rw-rw-   0        0        0     2483 2023-06-15 15:14:52.000000 webhdfs-py-client-0.0b2/src/webhdfs_py/example/example.py
+-rw-rw-rw-   0        0        0     1160 2023-06-01 02:02:20.000000 webhdfs-py-client-0.0b2/src/webhdfs_py/example/hello.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:36:36.000000 webhdfs-py-client-0.0b2/src/webhdfs_py/example/pages/
+-rw-rw-rw-   0        0        0     1648 2023-06-15 17:57:58.000000 webhdfs-py-client-0.0b2/src/webhdfs_py/example/pages/dataframe.py
+-rw-rw-rw-   0        0        0      360 2023-06-15 14:45:00.000000 webhdfs-py-client-0.0b2/src/webhdfs_py/example/run.py
+-rw-rw-rw-   0        0        0      390 2023-06-01 02:08:52.000000 webhdfs-py-client-0.0b2/src/webhdfs_py/example/utils.py
+-rw-rw-rw-   0        0        0      406 2023-06-07 19:36:30.000000 webhdfs-py-client-0.0b2/src/webhdfs_py/operations.py
+-rw-rw-rw-   0        0        0    27361 2023-06-15 15:14:52.000000 webhdfs-py-client-0.0b2/src/webhdfs_py/webhdfs.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:36:36.000000 webhdfs-py-client-0.0b2/src/webhdfs_py_client.egg-info/
+-rw-rw-rw-   0        0        0     3494 2023-06-15 19:36:34.000000 webhdfs-py-client-0.0b2/src/webhdfs_py_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-06-15 19:36:34.000000 webhdfs-py-client-0.0b2/src/webhdfs_py_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 19:36:34.000000 webhdfs-py-client-0.0b2/src/webhdfs_py_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-15 19:36:34.000000 webhdfs-py-client-0.0b2/src/webhdfs_py_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-15 19:36:34.000000 webhdfs-py-client-0.0b2/src/webhdfs_py_client.egg-info/top_level.txt
```

### Comparing `webhdfs-py-client-0.0b1/PKG-INFO` & `webhdfs-py-client-0.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webhdfs-py-client
-Version: 0.0b1
+Version: 0.0b2
 Summary: Python wrapper for the Hadoop WebHDFS REST API
 Home-page: 
 Author: Erik Alejandro Abdala
 Author-email: e.ale.abdala@gmail.com
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `webhdfs-py-client-0.0b1/README.md` & `webhdfs-py-client-0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `webhdfs-py-client-0.0b1/setup.py` & `webhdfs-py-client-0.0b2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_namespace_packages
 from pathlib import Path
 
 # Load the local files
 
 
-with open("./README.md", 'r',encoding="utf-8") as f:
+with open("README.md", 'r',encoding="utf-8") as f:
     long_description = f.read()
 
 # Read the requirements
-with open("./requirements.txt", 'r', encoding="utf8") as f:
+with open("requirements.txt", 'r', encoding="utf8") as f:
     requirements = f.readlines()
 
 try:
     version = open("VERSION", 'r').read().rstrip("\n")
 except FileNotFoundError:
     version = "0.0.beta"
 with open("VERSION", "w") as version_file:
```

### Comparing `webhdfs-py-client-0.0b1/src/webhdfs_py/example/example.py` & `webhdfs-py-client-0.0b2/src/webhdfs_py/example/example.py`

 * *Files identical despite different names*

### Comparing `webhdfs-py-client-0.0b1/src/webhdfs_py/example/hello.py` & `webhdfs-py-client-0.0b2/src/webhdfs_py/example/hello.py`

 * *Files identical despite different names*

### Comparing `webhdfs-py-client-0.0b1/src/webhdfs_py/example/pages/dataframe.py` & `webhdfs-py-client-0.0b2/src/webhdfs_py/example/pages/dataframe.py`

 * *Files identical despite different names*

### Comparing `webhdfs-py-client-0.0b1/src/webhdfs_py/webhdfs.py` & `webhdfs-py-client-0.0b2/src/webhdfs_py/webhdfs.py`

 * *Files identical despite different names*

### Comparing `webhdfs-py-client-0.0b1/src/webhdfs_py_client.egg-info/PKG-INFO` & `webhdfs-py-client-0.0b2/src/webhdfs_py_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webhdfs-py-client
-Version: 0.0b1
+Version: 0.0b2
 Summary: Python wrapper for the Hadoop WebHDFS REST API
 Home-page: 
 Author: Erik Alejandro Abdala
 Author-email: e.ale.abdala@gmail.com
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `webhdfs-py-client-0.0b1/src/webhdfs_py_client.egg-info/SOURCES.txt` & `webhdfs-py-client-0.0b2/src/webhdfs_py_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

