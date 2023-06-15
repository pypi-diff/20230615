# Comparing `tmp/stax_module_sdk-0.1.6.tar.gz` & `tmp/stax_module_sdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stax_module_sdk-0.1.6.tar", last modified: Mon Sep 19 06:09:11 2022, max compression
+gzip compressed data, was "stax_module_sdk-0.1.7.tar", last modified: Thu Jun 15 02:59:28 2023, max compression
```

## Comparing `stax_module_sdk-0.1.6.tar` & `stax_module_sdk-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxr-x   0 naru      (1000) naru      (1000)        0 2022-09-19 06:09:11.488143 stax_module_sdk-0.1.6/
--rw-rw-r--   0 naru      (1000) naru      (1000)     1639 2022-09-19 05:44:44.000000 stax_module_sdk-0.1.6/LICENSE.md
--rw-rw-r--   0 naru      (1000) naru      (1000)     7182 2022-09-19 06:09:11.488143 stax_module_sdk-0.1.6/PKG-INFO
--rw-rw-r--   0 naru      (1000) naru      (1000)     6745 2022-09-19 05:44:44.000000 stax_module_sdk-0.1.6/README.md
-drwxrwxr-x   0 naru      (1000) naru      (1000)        0 2022-09-19 06:09:11.488143 stax_module_sdk-0.1.6/bin/
--rw-rw-r--   0 naru      (1000) naru      (1000)       43 2022-09-19 05:44:44.000000 stax_module_sdk-0.1.6/bin/stax_module_cli
--rw-rw-r--   0 naru      (1000) naru      (1000)      103 2022-09-19 05:44:44.000000 stax_module_sdk-0.1.6/pyproject.toml
--rw-rw-r--   0 naru      (1000) naru      (1000)       38 2022-09-19 06:09:11.488143 stax_module_sdk-0.1.6/setup.cfg
--rw-rw-r--   0 naru      (1000) naru      (1000)      753 2022-09-19 06:09:04.000000 stax_module_sdk-0.1.6/setup.py
-drwxrwxr-x   0 naru      (1000) naru      (1000)        0 2022-09-19 06:09:11.484143 stax_module_sdk-0.1.6/src/
-drwxrwxr-x   0 naru      (1000) naru      (1000)        0 2022-09-19 06:09:11.488143 stax_module_sdk-0.1.6/src/stax_module_sdk/
--rw-rw-r--   0 naru      (1000) naru      (1000)     4233 2022-09-19 06:08:47.000000 stax_module_sdk-0.1.6/src/stax_module_sdk/Stax.py
--rw-rw-r--   0 naru      (1000) naru      (1000)       54 2022-09-19 05:44:44.000000 stax_module_sdk-0.1.6/src/stax_module_sdk/__init__.py
--rw-rw-r--   0 naru      (1000) naru      (1000)     1137 2022-09-19 05:44:44.000000 stax_module_sdk-0.1.6/src/stax_module_sdk/helpers.py
--rw-rw-r--   0 naru      (1000) naru      (1000)      884 2022-09-19 05:44:44.000000 stax_module_sdk-0.1.6/src/stax_module_sdk/pytext.py
--rw-rw-r--   0 naru      (1000) naru      (1000)     3783 2022-09-19 05:44:44.000000 stax_module_sdk-0.1.6/src/stax_module_sdk/wrapper.py
-drwxrwxr-x   0 naru      (1000) naru      (1000)        0 2022-09-19 06:09:11.488143 stax_module_sdk-0.1.6/src/stax_module_sdk.egg-info/
--rw-rw-r--   0 naru      (1000) naru      (1000)     7182 2022-09-19 06:09:11.000000 stax_module_sdk-0.1.6/src/stax_module_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 naru      (1000) naru      (1000)      430 2022-09-19 06:09:11.000000 stax_module_sdk-0.1.6/src/stax_module_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 naru      (1000) naru      (1000)        1 2022-09-19 06:09:11.000000 stax_module_sdk-0.1.6/src/stax_module_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 naru      (1000) naru      (1000)       15 2022-09-19 06:09:11.000000 stax_module_sdk-0.1.6/src/stax_module_sdk.egg-info/requires.txt
--rw-rw-r--   0 naru      (1000) naru      (1000)       16 2022-09-19 06:09:11.000000 stax_module_sdk-0.1.6/src/stax_module_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 naru      (1000) naru      (1000)        0 2023-06-15 02:59:28.590089 stax_module_sdk-0.1.7/
+-rw-rw-r--   0 naru      (1000) naru      (1000)     9027 2023-06-15 02:59:28.590089 stax_module_sdk-0.1.7/PKG-INFO
+-rw-rw-r--   0 naru      (1000) naru      (1000)     6745 2023-06-15 02:56:21.000000 stax_module_sdk-0.1.7/README.md
+drwxrwxr-x   0 naru      (1000) naru      (1000)        0 2023-06-15 02:59:28.590089 stax_module_sdk-0.1.7/bin/
+-rw-rw-r--   0 naru      (1000) naru      (1000)       43 2023-06-15 02:56:21.000000 stax_module_sdk-0.1.7/bin/stax_module_cli
+-rw-rw-r--   0 naru      (1000) naru      (1000)      103 2023-06-15 02:56:21.000000 stax_module_sdk-0.1.7/pyproject.toml
+-rw-rw-r--   0 naru      (1000) naru      (1000)       38 2023-06-15 02:59:28.590089 stax_module_sdk-0.1.7/setup.cfg
+-rw-rw-r--   0 naru      (1000) naru      (1000)      753 2023-06-15 02:59:21.000000 stax_module_sdk-0.1.7/setup.py
+drwxrwxr-x   0 naru      (1000) naru      (1000)        0 2023-06-15 02:59:28.590089 stax_module_sdk-0.1.7/src/
+drwxrwxr-x   0 naru      (1000) naru      (1000)        0 2023-06-15 02:59:28.590089 stax_module_sdk-0.1.7/src/stax_module_sdk/
+-rw-rw-r--   0 naru      (1000) naru      (1000)     4274 2023-06-15 02:57:29.000000 stax_module_sdk-0.1.7/src/stax_module_sdk/Stax.py
+-rw-rw-r--   0 naru      (1000) naru      (1000)       54 2023-06-15 02:56:21.000000 stax_module_sdk-0.1.7/src/stax_module_sdk/__init__.py
+-rw-rw-r--   0 naru      (1000) naru      (1000)     1137 2023-06-15 02:56:21.000000 stax_module_sdk-0.1.7/src/stax_module_sdk/helpers.py
+-rw-rw-r--   0 naru      (1000) naru      (1000)      884 2023-06-15 02:56:21.000000 stax_module_sdk-0.1.7/src/stax_module_sdk/pytext.py
+-rw-rw-r--   0 naru      (1000) naru      (1000)     3824 2023-06-15 02:57:29.000000 stax_module_sdk-0.1.7/src/stax_module_sdk/wrapper.py
+drwxrwxr-x   0 naru      (1000) naru      (1000)        0 2023-06-15 02:59:28.590089 stax_module_sdk-0.1.7/src/stax_module_sdk.egg-info/
+-rw-rw-r--   0 naru      (1000) naru      (1000)     9027 2023-06-15 02:59:28.000000 stax_module_sdk-0.1.7/src/stax_module_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 naru      (1000) naru      (1000)      419 2023-06-15 02:59:28.000000 stax_module_sdk-0.1.7/src/stax_module_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 naru      (1000) naru      (1000)        1 2023-06-15 02:59:28.000000 stax_module_sdk-0.1.7/src/stax_module_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 naru      (1000) naru      (1000)       15 2023-06-15 02:59:28.000000 stax_module_sdk-0.1.7/src/stax_module_sdk.egg-info/requires.txt
+-rw-rw-r--   0 naru      (1000) naru      (1000)       16 2023-06-15 02:59:28.000000 stax_module_sdk-0.1.7/src/stax_module_sdk.egg-info/top_level.txt
```

### Comparing `stax_module_sdk-0.1.6/PKG-INFO` & `stax_module_sdk-0.1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: stax_module_sdk
-Version: 0.1.6
-Summary: Stax.ai Module SDK
-Home-page: https://bitbucket.org/pinetree-ai/stax-module-sdk-py/src/master/
-Author: Stax.ai, Inc. <https://stax.ai>
-Author-email: naru@stax.ai
-License: CC-BY-NC 4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # Stax.ai Module SDK
 
 This project is created and maintained by [Stax.ai, Inc.](https://stax.ai), and is licensed under the [Creative Commons Attribution-NonCommercial 4.0 International License](https://creativecommons.org/licenses/by-nc/4.0/legalcode).
 
 ## About
 
 ...coming soon...
@@ -238,8 +224,8 @@
 
 ```sh
 python setup.py sdist bdist_wheel
 twine upload --repository-url https://test.pypi.org/legacy/ dist/*
 twine upload dist/*
 ```
 
-NOTE: PyPi username is: `inventives`
+NOTE: PyPi username is: `inventives`
```

### Comparing `stax_module_sdk-0.1.6/setup.py` & `stax_module_sdk-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='stax_module_sdk',
-    version='0.1.6',
+    version='0.1.7',
     url='https://bitbucket.org/pinetree-ai/stax-module-sdk-py/src/master/',
     author='Stax.ai, Inc. <https://stax.ai>',
     author_email='naru@stax.ai',
     description='Stax.ai Module SDK',
     long_description=readme,
     long_description_content_type='text/markdown',
     classifiers=[
```

### Comparing `stax_module_sdk-0.1.6/src/stax_module_sdk/Stax.py` & `stax_module_sdk-0.1.7/src/stax_module_sdk/Stax.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # See LICENSE.md file in project root directory
 import json
-from retry_requests import retry
+from retry_requests import retry, RSession
 from .helpers import getConfigByLabel
 
 class Stax:
     def __init__(self, module_id:str, module_key:str, team_id:str=None, document:str=None, api_url:str="https://api.stax.ai"):
         # Construct API header
         self.headers = {
             'Module': module_id,
@@ -12,15 +12,15 @@
             'Team': team_id
         }
 
         self.document_id = document
         self.api_url = api_url
 
         # Create retry requests session
-        self.sess = retry()
+        self.sess = retry(RSession(timeout=30), retries=3)
 
 
     def getDocument(self, presigned:bool=True, document:str=None):
         '''
         Get document metadata.
         '''
         document_id = document if document else self.document_id
```

### Comparing `stax_module_sdk-0.1.6/src/stax_module_sdk/helpers.py` & `stax_module_sdk-0.1.7/src/stax_module_sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `stax_module_sdk-0.1.6/src/stax_module_sdk/pytext.py` & `stax_module_sdk-0.1.7/src/stax_module_sdk/pytext.py`

 * *Files identical despite different names*

### Comparing `stax_module_sdk-0.1.6/src/stax_module_sdk/wrapper.py` & `stax_module_sdk-0.1.7/src/stax_module_sdk/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import os
 import json
 import shutil
 import signal
 import traceback
 from datetime import datetime
-from retry_requests import retry
+from retry_requests import retry, RSession
 
 from .Stax import Stax
 
-sess = retry()
+sess = retry(RSession(timeout=30), retries=3)
 
 def log(*args):
     print("[" + str(datetime.now()) + "]", *args)
 
 def result(obj):
     with open('response.json', 'w') as f:
         json.dump(obj, f)
```

