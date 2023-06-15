# Comparing `tmp/scrapy_arweave-0.0.1.tar.gz` & `tmp/scrapy_arweave-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy_arweave-0.0.1.tar", last modified: Tue May 16 17:41:01 2023, max compression
+gzip compressed data, was "scrapy_arweave-0.0.2.tar", last modified: Thu Jun 15 04:27:20 2023, max compression
```

## Comparing `scrapy_arweave-0.0.1.tar` & `scrapy_arweave-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 blokchainaholic   (501) staff       (20)        0 2023-05-16 17:41:01.977699 scrapy_arweave-0.0.1/
--rw-r--r--   0 blokchainaholic   (501) staff       (20)     1056 2023-05-15 03:22:58.000000 scrapy_arweave-0.0.1/LICENSE.txt
--rw-r--r--   0 blokchainaholic   (501) staff       (20)     4809 2023-05-16 17:41:01.977551 scrapy_arweave-0.0.1/PKG-INFO
--rw-r--r--   0 blokchainaholic   (501) staff       (20)     3877 2023-05-16 12:59:59.000000 scrapy_arweave-0.0.1/README.md
--rw-r--r--   0 blokchainaholic   (501) staff       (20)      297 2023-05-15 04:39:09.000000 scrapy_arweave-0.0.1/pyproject.toml
-drwxr-xr-x   0 blokchainaholic   (501) staff       (20)        0 2023-05-16 17:41:01.976471 scrapy_arweave-0.0.1/scrapy_arweave/
--rw-r--r--   0 blokchainaholic   (501) staff       (20)       22 2023-05-15 02:52:23.000000 scrapy_arweave-0.0.1/scrapy_arweave/__init__.py
--rw-r--r--   0 blokchainaholic   (501) staff       (20)     2955 2023-05-16 12:13:37.000000 scrapy_arweave-0.0.1/scrapy_arweave/client.py
--rw-r--r--   0 blokchainaholic   (501) staff       (20)     1053 2023-05-16 07:57:09.000000 scrapy_arweave-0.0.1/scrapy_arweave/feedexport.py
--rw-r--r--   0 blokchainaholic   (501) staff       (20)    12532 2023-05-16 12:51:28.000000 scrapy_arweave-0.0.1/scrapy_arweave/pipelines.py
-drwxr-xr-x   0 blokchainaholic   (501) staff       (20)        0 2023-05-16 17:41:01.977306 scrapy_arweave-0.0.1/scrapy_arweave.egg-info/
--rw-r--r--   0 blokchainaholic   (501) staff       (20)     4809 2023-05-16 17:41:01.000000 scrapy_arweave-0.0.1/scrapy_arweave.egg-info/PKG-INFO
--rw-r--r--   0 blokchainaholic   (501) staff       (20)      343 2023-05-16 17:41:01.000000 scrapy_arweave-0.0.1/scrapy_arweave.egg-info/SOURCES.txt
--rw-r--r--   0 blokchainaholic   (501) staff       (20)        1 2023-05-16 17:41:01.000000 scrapy_arweave-0.0.1/scrapy_arweave.egg-info/dependency_links.txt
--rw-r--r--   0 blokchainaholic   (501) staff       (20)       23 2023-05-16 17:41:01.000000 scrapy_arweave-0.0.1/scrapy_arweave.egg-info/requires.txt
--rw-r--r--   0 blokchainaholic   (501) staff       (20)       15 2023-05-16 17:41:01.000000 scrapy_arweave-0.0.1/scrapy_arweave.egg-info/top_level.txt
--rw-r--r--   0 blokchainaholic   (501) staff       (20)       38 2023-05-16 17:41:01.977749 scrapy_arweave-0.0.1/setup.cfg
--rw-r--r--   0 blokchainaholic   (501) staff       (20)     4614 2023-05-16 17:33:32.000000 scrapy_arweave-0.0.1/setup.py
+drwxr-xr-x   0 blokchainaholic   (501) staff       (20)        0 2023-06-15 04:27:20.882945 scrapy_arweave-0.0.2/
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     1056 2023-05-15 03:22:58.000000 scrapy_arweave-0.0.2/LICENSE.txt
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     4809 2023-06-15 04:27:20.882798 scrapy_arweave-0.0.2/PKG-INFO
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     3877 2023-06-15 04:25:39.000000 scrapy_arweave-0.0.2/README.md
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)      297 2023-05-15 04:39:09.000000 scrapy_arweave-0.0.2/pyproject.toml
+drwxr-xr-x   0 blokchainaholic   (501) staff       (20)        0 2023-06-15 04:27:20.881877 scrapy_arweave-0.0.2/scrapy_arweave/
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)       22 2023-05-15 02:52:23.000000 scrapy_arweave-0.0.2/scrapy_arweave/__init__.py
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     2955 2023-05-16 12:13:37.000000 scrapy_arweave-0.0.2/scrapy_arweave/client.py
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     1053 2023-05-16 07:57:09.000000 scrapy_arweave-0.0.2/scrapy_arweave/feedexport.py
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)    12532 2023-05-16 12:51:28.000000 scrapy_arweave-0.0.2/scrapy_arweave/pipelines.py
+drwxr-xr-x   0 blokchainaholic   (501) staff       (20)        0 2023-06-15 04:27:20.882583 scrapy_arweave-0.0.2/scrapy_arweave.egg-info/
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     4809 2023-06-15 04:27:20.000000 scrapy_arweave-0.0.2/scrapy_arweave.egg-info/PKG-INFO
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)      343 2023-06-15 04:27:20.000000 scrapy_arweave-0.0.2/scrapy_arweave.egg-info/SOURCES.txt
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)        1 2023-06-15 04:27:20.000000 scrapy_arweave-0.0.2/scrapy_arweave.egg-info/dependency_links.txt
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)       23 2023-06-15 04:27:20.000000 scrapy_arweave-0.0.2/scrapy_arweave.egg-info/requires.txt
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)       15 2023-06-15 04:27:20.000000 scrapy_arweave-0.0.2/scrapy_arweave.egg-info/top_level.txt
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)       38 2023-06-15 04:27:20.882996 scrapy_arweave-0.0.2/setup.cfg
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     4614 2023-06-15 04:25:42.000000 scrapy_arweave-0.0.2/setup.py
```

### Comparing `scrapy_arweave-0.0.1/LICENSE.txt` & `scrapy_arweave-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapy_arweave-0.0.1/PKG-INFO` & `scrapy_arweave-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy_arweave
-Version: 0.0.1
+Version: 0.0.2
 Summary: Scrapy is a popular open-source and collaborative python framework for extracting the data you need from websites. scrapy-arweave provides scrapy pipelines and feed exports to store items into Arweave.
 Home-page: https://github.com/pawanpaudel93/scrapy-arweave
 Author: Pawan Paudel
 Author-email: pawanpaudel93@gmail.com
 License: ISC
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
@@ -20,15 +20,15 @@
 License-File: LICENSE.txt
 
 
 <p align="center"><img src="logo.png" alt="original" width="100%" height="100%"></p>
 
 <h1 align="center">Welcome to Scrapy-Arweave</h1>
 <p>
-  <img alt="Version" src="https://img.shields.io/badge/version-0.0.1-blue.svg?cacheSeconds=2592000" />
+  <img alt="Version" src="https://img.shields.io/badge/version-0.0.2-blue.svg?cacheSeconds=2592000" />
 </p>
 
 Scrapy is a popular open-source and collaborative python framework for extracting the data you need from websites. scrapy-arweave provides scrapy pipelines and feed exports to store items into [Arweave](https://arweave.org/).
 
 ### 🏠 [Homepage](https://github.com/pawanpaudel93/scrapy-arweave)
 
 ## Install
```

### Comparing `scrapy_arweave-0.0.1/README.md` & `scrapy_arweave-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <p align="center"><img src="logo.png" alt="original" width="100%" height="100%"></p>
 
 <h1 align="center">Welcome to Scrapy-Arweave</h1>
 <p>
-  <img alt="Version" src="https://img.shields.io/badge/version-0.0.1-blue.svg?cacheSeconds=2592000" />
+  <img alt="Version" src="https://img.shields.io/badge/version-0.0.2-blue.svg?cacheSeconds=2592000" />
 </p>
 
 Scrapy is a popular open-source and collaborative python framework for extracting the data you need from websites. scrapy-arweave provides scrapy pipelines and feed exports to store items into [Arweave](https://arweave.org/).
 
 ### 🏠 [Homepage](https://github.com/pawanpaudel93/scrapy-arweave)
 
 ## Install
```

### Comparing `scrapy_arweave-0.0.1/scrapy_arweave/client.py` & `scrapy_arweave-0.0.2/scrapy_arweave/client.py`

 * *Files identical despite different names*

### Comparing `scrapy_arweave-0.0.1/scrapy_arweave/feedexport.py` & `scrapy_arweave-0.0.2/scrapy_arweave/feedexport.py`

 * *Files identical despite different names*

### Comparing `scrapy_arweave-0.0.1/scrapy_arweave/pipelines.py` & `scrapy_arweave-0.0.2/scrapy_arweave/pipelines.py`

 * *Files identical despite different names*

### Comparing `scrapy_arweave-0.0.1/scrapy_arweave.egg-info/PKG-INFO` & `scrapy_arweave-0.0.2/scrapy_arweave.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-arweave
-Version: 0.0.1
+Version: 0.0.2
 Summary: Scrapy is a popular open-source and collaborative python framework for extracting the data you need from websites. scrapy-arweave provides scrapy pipelines and feed exports to store items into Arweave.
 Home-page: https://github.com/pawanpaudel93/scrapy-arweave
 Author: Pawan Paudel
 Author-email: pawanpaudel93@gmail.com
 License: ISC
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
@@ -20,15 +20,15 @@
 License-File: LICENSE.txt
 
 
 <p align="center"><img src="logo.png" alt="original" width="100%" height="100%"></p>
 
 <h1 align="center">Welcome to Scrapy-Arweave</h1>
 <p>
-  <img alt="Version" src="https://img.shields.io/badge/version-0.0.1-blue.svg?cacheSeconds=2592000" />
+  <img alt="Version" src="https://img.shields.io/badge/version-0.0.2-blue.svg?cacheSeconds=2592000" />
 </p>
 
 Scrapy is a popular open-source and collaborative python framework for extracting the data you need from websites. scrapy-arweave provides scrapy pipelines and feed exports to store items into [Arweave](https://arweave.org/).
 
 ### 🏠 [Homepage](https://github.com/pawanpaudel93/scrapy-arweave)
 
 ## Install
```

### Comparing `scrapy_arweave-0.0.1/setup.py` & `scrapy_arweave-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 # Package meta-data.
 NAME = "scrapy_arweave"
 DESCRIPTION = "Scrapy is a popular open-source and collaborative python framework for extracting the data you need from websites. scrapy-arweave provides scrapy pipelines and feed exports to store items into Arweave."
 URL = "https://github.com/pawanpaudel93/scrapy-arweave"
 EMAIL = "pawanpaudel93@gmail.com"
 AUTHOR = "Pawan Paudel"
 REQUIRES_PYTHON = ">=3.0"
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 REQUIRED = [
     "python-magic",
     "pyarweave",
 ]
 
 EXTRAS = {
```

