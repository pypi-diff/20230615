# Comparing `tmp/python-oauth-token-manager-0.2.5.tar.gz` & `tmp/python-oauth-token-manager-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-oauth-token-manager-0.2.5.tar", last modified: Thu Jun 15 15:28:29 2023, max compression
+gzip compressed data, was "python-oauth-token-manager-0.2.6.tar", last modified: Thu Jun 15 15:31:36 2023, max compression
```

## Comparing `python-oauth-token-manager-0.2.5.tar` & `python-oauth-token-manager-0.2.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-15 15:28:29.237966 python-oauth-token-manager-0.2.5/
--rw-rw-r--   0 davidharcombe (261421) primarygroup (89939)    11357 2022-07-15 13:28:45.000000 python-oauth-token-manager-0.2.5/LICENSE
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2947 2023-06-15 15:28:29.237966 python-oauth-token-manager-0.2.5/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2387 2023-06-14 15:36:29.000000 python-oauth-token-manager-0.2.5/README.md
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-15 15:28:29.233966 python-oauth-token-manager-0.2.5/auth/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      769 2023-06-15 15:27:37.000000 python-oauth-token-manager-0.2.5/auth/__init__.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     4035 2022-07-08 21:15:10.000000 python-oauth-token-manager-0.2.5/auth/abstract_datastore.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5760 2023-06-15 15:27:55.000000 python-oauth-token-manager-0.2.5/auth/credentials.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1322 2022-07-12 16:38:02.000000 python-oauth-token-manager-0.2.5/auth/credentials_helpers.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1057 2022-07-12 16:36:52.000000 python-oauth-token-manager-0.2.5/auth/credentials_helpers_test.py
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-15 15:28:29.237966 python-oauth-token-manager-0.2.5/auth/datastore/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      610 2023-05-18 18:02:08.000000 python-oauth-token-manager-0.2.5/auth/datastore/__init__.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5937 2023-06-15 15:27:04.000000 python-oauth-token-manager-0.2.5/auth/datastore/cloud_storage.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     8319 2023-05-18 14:50:53.000000 python-oauth-token-manager-0.2.5/auth/datastore/cloud_storage_test.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     4702 2023-06-15 15:27:13.000000 python-oauth-token-manager-0.2.5/auth/datastore/firestore.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5063 2023-06-15 15:27:18.000000 python-oauth-token-manager-0.2.5/auth/datastore/local_file.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     6154 2023-05-18 14:53:49.000000 python-oauth-token-manager-0.2.5/auth/datastore/local_file_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     6001 2023-06-15 15:27:21.000000 python-oauth-token-manager-0.2.5/auth/datastore/secret_manager.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1517 2022-08-17 14:18:37.000000 python-oauth-token-manager-0.2.5/auth/decorators.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1030 2022-08-09 16:45:46.000000 python-oauth-token-manager-0.2.5/auth/decorators_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      739 2022-07-08 21:14:30.000000 python-oauth-token-manager-0.2.5/auth/exceptions.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1266 2023-06-15 15:28:16.000000 python-oauth-token-manager-0.2.5/pyproject.toml
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-15 15:28:29.237966 python-oauth-token-manager-0.2.5/python_oauth_token_manager.egg-info/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2947 2023-06-15 15:28:29.000000 python-oauth-token-manager-0.2.5/python_oauth_token_manager.egg-info/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      688 2023-06-15 15:28:29.000000 python-oauth-token-manager-0.2.5/python_oauth_token_manager.egg-info/SOURCES.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-06-15 15:28:29.000000 python-oauth-token-manager-0.2.5/python_oauth_token_manager.egg-info/dependency_links.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      495 2023-06-15 15:28:29.000000 python-oauth-token-manager-0.2.5/python_oauth_token_manager.egg-info/requires.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        5 2023-06-15 15:28:29.000000 python-oauth-token-manager-0.2.5/python_oauth_token_manager.egg-info/top_level.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-06-15 15:28:29.237966 python-oauth-token-manager-0.2.5/setup.cfg
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-15 15:31:36.981621 python-oauth-token-manager-0.2.6/
+-rw-rw-r--   0 davidharcombe (261421) primarygroup (89939)    11357 2022-07-15 13:28:45.000000 python-oauth-token-manager-0.2.6/LICENSE
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2947 2023-06-15 15:31:36.981621 python-oauth-token-manager-0.2.6/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2387 2023-06-14 15:36:29.000000 python-oauth-token-manager-0.2.6/README.md
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-15 15:31:36.981621 python-oauth-token-manager-0.2.6/auth/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      769 2023-06-15 15:27:37.000000 python-oauth-token-manager-0.2.6/auth/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     4035 2023-06-15 15:30:01.000000 python-oauth-token-manager-0.2.6/auth/abstract_datastore.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5770 2023-06-15 15:29:48.000000 python-oauth-token-manager-0.2.6/auth/credentials.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1322 2022-07-12 16:38:02.000000 python-oauth-token-manager-0.2.6/auth/credentials_helpers.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1057 2022-07-12 16:36:52.000000 python-oauth-token-manager-0.2.6/auth/credentials_helpers_test.py
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-15 15:31:36.981621 python-oauth-token-manager-0.2.6/auth/datastore/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      610 2023-05-18 18:02:08.000000 python-oauth-token-manager-0.2.6/auth/datastore/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5937 2023-06-15 15:27:04.000000 python-oauth-token-manager-0.2.6/auth/datastore/cloud_storage.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     8319 2023-05-18 14:50:53.000000 python-oauth-token-manager-0.2.6/auth/datastore/cloud_storage_test.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     4702 2023-06-15 15:27:13.000000 python-oauth-token-manager-0.2.6/auth/datastore/firestore.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5063 2023-06-15 15:27:18.000000 python-oauth-token-manager-0.2.6/auth/datastore/local_file.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     6154 2023-05-18 14:53:49.000000 python-oauth-token-manager-0.2.6/auth/datastore/local_file_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     6001 2023-06-15 15:27:21.000000 python-oauth-token-manager-0.2.6/auth/datastore/secret_manager.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1517 2022-08-17 14:18:37.000000 python-oauth-token-manager-0.2.6/auth/decorators.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1030 2022-08-09 16:45:46.000000 python-oauth-token-manager-0.2.6/auth/decorators_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      739 2022-07-08 21:14:30.000000 python-oauth-token-manager-0.2.6/auth/exceptions.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1266 2023-06-15 15:29:36.000000 python-oauth-token-manager-0.2.6/pyproject.toml
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-15 15:31:36.981621 python-oauth-token-manager-0.2.6/python_oauth_token_manager.egg-info/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2947 2023-06-15 15:31:36.000000 python-oauth-token-manager-0.2.6/python_oauth_token_manager.egg-info/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      688 2023-06-15 15:31:36.000000 python-oauth-token-manager-0.2.6/python_oauth_token_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-06-15 15:31:36.000000 python-oauth-token-manager-0.2.6/python_oauth_token_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      495 2023-06-15 15:31:36.000000 python-oauth-token-manager-0.2.6/python_oauth_token_manager.egg-info/requires.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        5 2023-06-15 15:31:36.000000 python-oauth-token-manager-0.2.6/python_oauth_token_manager.egg-info/top_level.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-06-15 15:31:36.981621 python-oauth-token-manager-0.2.6/setup.cfg
```

### Comparing `python-oauth-token-manager-0.2.5/LICENSE` & `python-oauth-token-manager-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.5/PKG-INFO` & `python-oauth-token-manager-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-oauth-token-manager
-Version: 0.2.5
+Version: 0.2.6
 Summary: API for managing stored OAuth credentials.
 Author-email: David Harcombe <david.harcombe@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/googleworkspace/python-oauth-token-manager
 Project-URL: Bug Tracker, https://github.com/googleworkspace/python-oauth-token-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `python-oauth-token-manager-0.2.5/README.md` & `python-oauth-token-manager-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.5/auth/__init__.py` & `python-oauth-token-manager-0.2.6/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.5/auth/abstract_datastore.py` & `python-oauth-token-manager-0.2.6/auth/abstract_datastore.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.5/auth/credentials.py` & `python-oauth-token-manager-0.2.6/auth/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from typing import Any, Dict, Type, TypeVar
 
 import pytz
 from dateutil.relativedelta import relativedelta
 from google.auth.transport import requests
 from google.oauth2 import credentials as oauth
 
-import decorators
+from auth import decorators
 from .credentials_helpers import encode_key
 
 from .abstract_datastore import AbstractDatastore
 from .exceptions import CredentialsError
 
 
 @dataclass
```

### Comparing `python-oauth-token-manager-0.2.5/auth/credentials_helpers.py` & `python-oauth-token-manager-0.2.6/auth/credentials_helpers.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.5/auth/credentials_helpers_test.py` & `python-oauth-token-manager-0.2.6/auth/credentials_helpers_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.5/auth/datastore/__init__.py` & `python-oauth-token-manager-0.2.6/auth/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.5/auth/datastore/cloud_storage.py` & `python-oauth-token-manager-0.2.6/auth/datastore/cloud_storage.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.5/auth/datastore/cloud_storage_test.py` & `python-oauth-token-manager-0.2.6/auth/datastore/cloud_storage_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.5/auth/datastore/firestore.py` & `python-oauth-token-manager-0.2.6/auth/datastore/firestore.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.5/auth/datastore/local_file.py` & `python-oauth-token-manager-0.2.6/auth/datastore/local_file.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.5/auth/datastore/local_file_test.py` & `python-oauth-token-manager-0.2.6/auth/datastore/local_file_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.5/auth/datastore/secret_manager.py` & `python-oauth-token-manager-0.2.6/auth/datastore/secret_manager.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.5/auth/decorators.py` & `python-oauth-token-manager-0.2.6/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.5/auth/decorators_test.py` & `python-oauth-token-manager-0.2.6/auth/decorators_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.5/auth/exceptions.py` & `python-oauth-token-manager-0.2.6/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.5/pyproject.toml` & `python-oauth-token-manager-0.2.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "python-oauth-token-manager"
-version = "0.2.5"
+version = "0.2.6"
 authors = [{ name = "David Harcombe", email = "david.harcombe@gmail.com" }]
 description = "API for managing stored OAuth credentials."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
```

### Comparing `python-oauth-token-manager-0.2.5/python_oauth_token_manager.egg-info/PKG-INFO` & `python-oauth-token-manager-0.2.6/python_oauth_token_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-oauth-token-manager
-Version: 0.2.5
+Version: 0.2.6
 Summary: API for managing stored OAuth credentials.
 Author-email: David Harcombe <david.harcombe@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/googleworkspace/python-oauth-token-manager
 Project-URL: Bug Tracker, https://github.com/googleworkspace/python-oauth-token-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `python-oauth-token-manager-0.2.5/python_oauth_token_manager.egg-info/SOURCES.txt` & `python-oauth-token-manager-0.2.6/python_oauth_token_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

