# Comparing `tmp/neqsimapi_connector-0.1.6.tar.gz` & `tmp/neqsimapi_connector-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neqsimapi_connector-0.1.6.tar", max compression
+gzip compressed data, was "neqsimapi_connector-0.1.7.tar", max compression
```

## Comparing `neqsimapi_connector-0.1.6.tar` & `neqsimapi_connector-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1039 2023-05-26 10:31:57.077727 neqsimapi_connector-0.1.6/README.md
--rw-r--r--   0        0        0     4504 2023-05-26 09:50:06.820770 neqsimapi_connector-0.1.6/neqsimapi_connector/BearerAuth.py
--rw-r--r--   0        0        0     3940 2023-05-12 10:36:51.953910 neqsimapi_connector-0.1.6/neqsimapi_connector/Connector.py
--rw-r--r--   0        0        0      597 2023-05-26 18:59:29.111747 neqsimapi_connector-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1977 1970-01-01 00:00:00.000000 neqsimapi_connector-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1039 2023-05-26 10:31:57.077727 neqsimapi_connector-0.1.7/README.md
+-rw-r--r--   0        0        0     4620 2023-06-14 13:33:15.881449 neqsimapi_connector-0.1.7/neqsimapi_connector/BearerAuth.py
+-rw-r--r--   0        0        0     4138 2023-06-14 13:24:22.875049 neqsimapi_connector-0.1.7/neqsimapi_connector/Connector.py
+-rw-r--r--   0        0        0      597 2023-06-14 13:34:57.537579 neqsimapi_connector-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1977 1970-01-01 00:00:00.000000 neqsimapi_connector-0.1.7/PKG-INFO
```

### Comparing `neqsimapi_connector-0.1.6/README.md` & `neqsimapi_connector-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `neqsimapi_connector-0.1.6/neqsimapi_connector/BearerAuth.py` & `neqsimapi_connector-0.1.7/neqsimapi_connector/BearerAuth.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,17 @@
 class BearerAuth(requests.auth.AuthBase):
     """Class for getting bearer token authentication using msal.
 
     Get BearerAuth object by calling get_bearer_token.
     """
 
     def __init__(self, token) -> None:
+        if isinstance(token,dict) and "access_result" in token:
+            token = token["access_result"]
+        
         self.token = token
 
     def __call__(self, r):
         r.headers["authorization"] = "Bearer " + self.token
         return r
 
     @staticmethod
```

### Comparing `neqsimapi_connector-0.1.6/neqsimapi_connector/Connector.py` & `neqsimapi_connector-0.1.7/neqsimapi_connector/Connector.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,14 +46,19 @@
         if url is None or len(url) == 0:
             self.base_url = get_url_NeqSimAPI()
         else:
             self.base_url = url
 
         if auth is None:
             auth = get_auth_NeqSimAPI()
+        elif isinstance(auth, str):
+            auth = BearerAuth(str)
+        elif isinstance(auth, dict) and "access_result" in auth:
+            auth = BearerAuth(auth["access_result"])
+        
         self.session = requests.Session()
         self.session.auth = auth
         if verifySSL is False:
             requests.packages.urllib3.disable_warnings(
                 requests.packages.urllib3.exceptions.InsecureRequestWarning
             )
         self.session.verify = verifySSL
```

### Comparing `neqsimapi_connector-0.1.6/pyproject.toml` & `neqsimapi_connector-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neqsimapi-connector"
-version = "0.1.6"
+version = "0.1.7"
 description = "A python package to simplify calling NeqSimAPI for end-users."
 authors = ["Åsmund Våge Fannemel <asmf@equinor.com>"]
 readme = "README.md"
 packages = [{include = "neqsimapi_connector"}]
 license = "MIT"
 repository = "https://github.com/equinor/NeqSimAPI-connector"
```

### Comparing `neqsimapi_connector-0.1.6/PKG-INFO` & `neqsimapi_connector-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neqsimapi-connector
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python package to simplify calling NeqSimAPI for end-users.
 Home-page: https://github.com/equinor/NeqSimAPI-connector
 License: MIT
 Author: Åsmund Våge Fannemel
 Author-email: asmf@equinor.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

