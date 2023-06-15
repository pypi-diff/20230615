# Comparing `tmp/lodestone-python-sdk-1.0.6.tar.gz` & `tmp/lodestone-python-sdk-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lodestone-python-sdk-1.0.6.tar", last modified: Wed Jun 14 09:32:08 2023, max compression
+gzip compressed data, was "lodestone-python-sdk-1.0.7.tar", last modified: Thu Jun 15 09:39:20 2023, max compression
```

## Comparing `lodestone-python-sdk-1.0.6.tar` & `lodestone-python-sdk-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-14 09:32:08.091626 lodestone-python-sdk-1.0.6/
--rw-r--r--   0 bocai      (501) staff       (20)      518 2023-06-14 09:32:08.091511 lodestone-python-sdk-1.0.6/PKG-INFO
--rw-r--r--   0 bocai      (501) staff       (20)      248 2023-06-13 08:22:58.000000 lodestone-python-sdk-1.0.6/README.md
-drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-14 09:32:08.090752 lodestone-python-sdk-1.0.6/lodestone_python_sdk/
--rw-r--r--   0 bocai      (501) staff       (20)        0 2023-06-13 09:41:00.000000 lodestone-python-sdk-1.0.6/lodestone_python_sdk/__init__.py
--rw-r--r--   0 bocai      (501) staff       (20)      697 2023-06-13 09:41:00.000000 lodestone-python-sdk-1.0.6/lodestone_python_sdk/auth_client.py
--rw-r--r--   0 bocai      (501) staff       (20)       42 2023-06-13 09:41:00.000000 lodestone-python-sdk-1.0.6/lodestone_python_sdk/exceptions.py
-drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-14 09:32:08.091357 lodestone-python-sdk-1.0.6/lodestone_python_sdk.egg-info/
--rw-r--r--   0 bocai      (501) staff       (20)      518 2023-06-14 09:32:08.000000 lodestone-python-sdk-1.0.6/lodestone_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 bocai      (501) staff       (20)      341 2023-06-14 09:32:08.000000 lodestone-python-sdk-1.0.6/lodestone_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 bocai      (501) staff       (20)        1 2023-06-14 09:32:08.000000 lodestone-python-sdk-1.0.6/lodestone_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 bocai      (501) staff       (20)       21 2023-06-14 09:32:08.000000 lodestone-python-sdk-1.0.6/lodestone_python_sdk.egg-info/requires.txt
--rw-r--r--   0 bocai      (501) staff       (20)       21 2023-06-14 09:32:08.000000 lodestone-python-sdk-1.0.6/lodestone_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 bocai      (501) staff       (20)       38 2023-06-14 09:32:08.091671 lodestone-python-sdk-1.0.6/setup.cfg
--rw-r--r--   0 bocai      (501) staff       (20)      502 2023-06-14 09:31:58.000000 lodestone-python-sdk-1.0.6/setup.py
+drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-15 09:39:20.644107 lodestone-python-sdk-1.0.7/
+-rw-r--r--   0 bocai      (501) staff       (20)      518 2023-06-15 09:39:20.643993 lodestone-python-sdk-1.0.7/PKG-INFO
+-rw-r--r--   0 bocai      (501) staff       (20)      248 2023-06-13 08:22:58.000000 lodestone-python-sdk-1.0.7/README.md
+drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-15 09:39:20.643288 lodestone-python-sdk-1.0.7/lodestone_python_sdk/
+-rw-r--r--   0 bocai      (501) staff       (20)        0 2023-06-13 09:41:00.000000 lodestone-python-sdk-1.0.7/lodestone_python_sdk/__init__.py
+-rw-r--r--   0 bocai      (501) staff       (20)     1356 2023-06-15 09:34:24.000000 lodestone-python-sdk-1.0.7/lodestone_python_sdk/auth_client.py
+-rw-r--r--   0 bocai      (501) staff       (20)      140 2023-06-15 09:00:23.000000 lodestone-python-sdk-1.0.7/lodestone_python_sdk/exceptions.py
+drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-15 09:39:20.643839 lodestone-python-sdk-1.0.7/lodestone_python_sdk.egg-info/
+-rw-r--r--   0 bocai      (501) staff       (20)      518 2023-06-15 09:39:20.000000 lodestone-python-sdk-1.0.7/lodestone_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 bocai      (501) staff       (20)      341 2023-06-15 09:39:20.000000 lodestone-python-sdk-1.0.7/lodestone_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 bocai      (501) staff       (20)        1 2023-06-15 09:39:20.000000 lodestone-python-sdk-1.0.7/lodestone_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 bocai      (501) staff       (20)       21 2023-06-15 09:39:20.000000 lodestone-python-sdk-1.0.7/lodestone_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 bocai      (501) staff       (20)       21 2023-06-15 09:39:20.000000 lodestone-python-sdk-1.0.7/lodestone_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 bocai      (501) staff       (20)       38 2023-06-15 09:39:20.644150 lodestone-python-sdk-1.0.7/setup.cfg
+-rw-r--r--   0 bocai      (501) staff       (20)      493 2023-06-15 09:27:47.000000 lodestone-python-sdk-1.0.7/setup.py
```

### Comparing `lodestone-python-sdk-1.0.6/PKG-INFO` & `lodestone-python-sdk-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lodestone-python-sdk
-Version: 1.0.6
+Version: 1.0.7
 Summary: Auth to tuyoo's Lodestone
 Home-page: UNKNOWN
 Author: bocai
 Author-email: peijianbo@tuyoogame.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >3.2
```

### Comparing `lodestone-python-sdk-1.0.6/lodestone_python_sdk/auth_client.py` & `lodestone-python-sdk-1.0.7/lodestone_python_sdk/auth_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,43 @@
 import json
 from urllib.parse import urljoin
 
 from requests import request
 
-from .exceptions import AuthException
+from .exceptions import AppAuthException, UserAuthException
 
 
-class AuthClient:
+class AppAuthClient:
     def __init__(self, auth_host, app_key, app_secret, auth_path='account/api/v1/access-token'):
         self.auth_url = urljoin(auth_host, auth_path)
         self.app_key = app_key
         self.app_secret = app_secret
 
     def get_token(self):
         response = request(
             method='post',
             url=self.auth_url,
             data={'app_key': self.app_key, 'app_secret': self.app_secret}
         )
         try:
             return json.loads(response.content)['token']
         except Exception as e:
-            raise AuthException(response.text)
+            raise AppAuthException(response.text)
+
+
+class UserAuthClient:
+    def __init__(self, auth_host, username, password, auth_path='account/api/v1/login', cate=1):
+        self.auth_url = urljoin(auth_host, auth_path)
+        self.username = username
+        self.password = password
+        self.cate = cate
+
+    def get_token(self):
+        response = request(
+            method='post',
+            url=self.auth_url,
+            data={'cate': self.cate, 'username': self.username, 'password': self.password}
+        )
+        try:
+            return json.loads(response.content)['token']
+        except Exception as e:
+            raise UserAuthException(response.text)
```

### Comparing `lodestone-python-sdk-1.0.6/lodestone_python_sdk.egg-info/PKG-INFO` & `lodestone-python-sdk-1.0.7/lodestone_python_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lodestone-python-sdk
-Version: 1.0.6
+Version: 1.0.7
 Summary: Auth to tuyoo's Lodestone
 Home-page: UNKNOWN
 Author: bocai
 Author-email: peijianbo@tuyoogame.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >3.2
```

