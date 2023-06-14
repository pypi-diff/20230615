# Comparing `tmp/sixth-sense-0.0.3.tar.gz` & `tmp/sixth-sense-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sixth-sense-0.0.3.tar", last modified: Mon Jun 12 03:13:52 2023, max compression
+gzip compressed data, was "dist/sixth-sense-0.0.4.tar", last modified: Wed Jun 14 23:28:02 2023, max compression
```

## Comparing `sixth-sense-0.0.3.tar` & `sixth-sense-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 03:13:52.000000 sixth-sense-0.0.3/
--rw-r--r--   0 mac        (501) staff       (20)      759 2023-06-12 03:13:52.000000 sixth-sense-0.0.3/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)       20 2023-06-09 19:50:05.000000 sixth-sense-0.0.3/README.md
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-12 03:13:52.000000 sixth-sense-0.0.3/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     2014 2023-06-12 03:13:50.000000 sixth-sense-0.0.3/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 03:13:52.000000 sixth-sense-0.0.3/sixth_sense/
--rw-r--r--   0 mac        (501) staff       (20)       46 2023-06-12 01:09:39.000000 sixth-sense-0.0.3/sixth_sense/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 03:13:52.000000 sixth-sense-0.0.3/sixth_sense/middlewares/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-sense-0.0.3/sixth_sense/middlewares/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3715 2023-06-12 02:56:19.000000 sixth-sense-0.0.3/sixth_sense/middlewares/encryption_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-sense-0.0.3/sixth_sense/middlewares/six_base_http_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     3930 2023-06-12 02:55:48.000000 sixth-sense-0.0.3/sixth_sense/middlewares/six_independent_rate_limiter.py
--rw-r--r--   0 mac        (501) staff       (20)     3881 2023-06-12 02:56:04.000000 sixth-sense-0.0.3/sixth_sense/middlewares/six_rate_limiter_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)      624 2023-06-10 23:02:11.000000 sixth-sense-0.0.3/sixth_sense/schemas.py
--rw-r--r--   0 mac        (501) staff       (20)     4126 2023-06-12 03:06:15.000000 sixth-sense-0.0.3/sixth_sense/sixth_sense.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 03:13:52.000000 sixth-sense-0.0.3/sixth_sense/utils/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-sense-0.0.3/sixth_sense/utils/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-sense-0.0.3/sixth_sense/utils/encryption_utils.py
--rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-sense-0.0.3/sixth_sense/utils/time_utils.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 03:13:52.000000 sixth-sense-0.0.3/sixth_sense.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      759 2023-06-12 03:13:52.000000 sixth-sense-0.0.3/sixth_sense.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      614 2023-06-12 03:13:52.000000 sixth-sense-0.0.3/sixth_sense.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-12 03:13:52.000000 sixth-sense-0.0.3/sixth_sense.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      610 2023-06-12 03:13:52.000000 sixth-sense-0.0.3/sixth_sense.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       12 2023-06-12 03:13:52.000000 sixth-sense-0.0.3/sixth_sense.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/
+-rw-r--r--   0 mac        (501) staff       (20)      759 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)       20 2023-06-09 19:50:05.000000 sixth-sense-0.0.4/README.md
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     2014 2023-06-14 23:08:33.000000 sixth-sense-0.0.4/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/sixth_sense/
+-rw-r--r--   0 mac        (501) staff       (20)       46 2023-06-12 01:09:39.000000 sixth-sense-0.0.4/sixth_sense/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/sixth_sense/middlewares/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-sense-0.0.4/sixth_sense/middlewares/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3715 2023-06-12 02:56:19.000000 sixth-sense-0.0.4/sixth_sense/middlewares/encryption_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-sense-0.0.4/sixth_sense/middlewares/six_base_http_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     3930 2023-06-12 02:55:48.000000 sixth-sense-0.0.4/sixth_sense/middlewares/six_independent_rate_limiter.py
+-rw-r--r--   0 mac        (501) staff       (20)     4204 2023-06-14 03:49:11.000000 sixth-sense-0.0.4/sixth_sense/middlewares/six_rate_limiter_middleware.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/sixth_sense/pen_test/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-12 15:04:45.000000 sixth-sense-0.0.4/sixth_sense/pen_test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      165 2023-06-14 20:44:10.000000 sixth-sense-0.0.4/sixth_sense/pen_test/auto_pen_test.py
+-rw-r--r--   0 mac        (501) staff       (20)      624 2023-06-10 23:02:11.000000 sixth-sense-0.0.4/sixth_sense/schemas.py
+-rw-r--r--   0 mac        (501) staff       (20)     4191 2023-06-14 20:44:16.000000 sixth-sense-0.0.4/sixth_sense/sixth_sense.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/sixth_sense/utils/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-sense-0.0.4/sixth_sense/utils/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-sense-0.0.4/sixth_sense/utils/encryption_utils.py
+-rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-sense-0.0.4/sixth_sense/utils/time_utils.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/sixth_sense.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      759 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/sixth_sense.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      685 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/sixth_sense.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/sixth_sense.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      610 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/sixth_sense.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       12 2023-06-14 23:28:02.000000 sixth-sense-0.0.4/sixth_sense.egg-info/top_level.txt
```

### Comparing `sixth-sense-0.0.3/PKG-INFO` & `sixth-sense-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sixth-sense
-Version: 0.0.3
+Version: 0.0.4
 Summary: Six offical python ackage
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: Six is a package that helps you automate pen testing and also helps you protect your API from cybersecurity threats. Visit https://withsix.co to get started.
 Keywords: python,cybersecurity,pentesting,encryption,rate limiting,xss prevention
```

### Comparing `sixth-sense-0.0.3/setup.py` & `sixth-sense-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from pip._internal.req import parse_requirements
 
 
 
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Six offical python ackage'
 LONG_DESCRIPTION = 'Six is a package that helps you automate pen testing and also helps you protect your API from cybersecurity threats. Visit https://withsix.co to get started.'
 
 # Setting up
 setup(
     name="sixth-sense",
     version=VERSION,
```

### Comparing `sixth-sense-0.0.3/sixth_sense/middlewares/encryption_middleware.py` & `sixth-sense-0.0.4/sixth_sense/middlewares/encryption_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-sense-0.0.3/sixth_sense/middlewares/six_base_http_middleware.py` & `sixth-sense-0.0.4/sixth_sense/middlewares/six_base_http_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-sense-0.0.3/sixth_sense/middlewares/six_independent_rate_limiter.py` & `sixth-sense-0.0.4/sixth_sense/middlewares/six_independent_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `sixth-sense-0.0.3/sixth_sense/middlewares/six_rate_limiter_middleware.py` & `sixth-sense-0.0.4/sixth_sense/middlewares/six_rate_limiter_middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,23 @@
 class SixRateLimiterMiddleware(BaseHTTPMiddleware):
     def __init__(self, app: ASGIApp, apikey: str, fastapi_app: FastAPI, project_config: schemas.ProjectConfig):
         super().__init__(app)
         self._config = project_config
         self._log_dict = {}
         self._app = app
         self._apikey = apikey
-        for route in fastapi_app.routes:
-            new_route = re.sub(r'\W+', '~', route.path)
-            self._log_dict[str(new_route)] = {}
+        for route in fastapi_app.router.routes:
+            if type(route.app )== FastAPI:
+                for new_route in route.app.routes:
+                    path = "/v"+str(route.app.version)+new_route.path
+                    edited_route = re.sub(r'\W+', '~', path)
+                    self._log_dict[str(edited_route)] = {}
+            else:
+                edited_route = re.sub(r'\W+', '~', route.path)
+                self._log_dict[str(edited_route)] = {}
 
     async def set_body(self, request: Request, body: bytes):
         async def receive() -> Message:
             return {'type': 'http.request', 'body': body}
         request._receive = receive
         
     def _is_rate_limit_reached(self, uid, route):
```

### Comparing `sixth-sense-0.0.3/sixth_sense/schemas.py` & `sixth-sense-0.0.4/sixth_sense/schemas.py`

 * *Files identical despite different names*

### Comparing `sixth-sense-0.0.3/sixth_sense/sixth_sense.py` & `sixth-sense-0.0.4/sixth_sense/sixth_sense.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,16 @@
         
     def _sync_project_route(self, config: schemas.ProjectConfig = None)-> schemas.ProjectConfig:
         #sync the config with db
         _rl_configs = {}
         for route in self._app.router.routes:
             if type(route.app )== FastAPI:
                 for new_route in route.app.routes:
-                    edited_route = re.sub(r'\W+', '~', new_route)
+                    path = "/v"+str(route.app.version)+new_route.path
+                    edited_route = re.sub(r'\W+', '~', path)
                     if config and edited_route in config.rate_limiter.keys():
                         #default config has been set earlier on so skip
                         _rl_configs[edited_route] = config.rate_limiter[edited_route]
                         continue
                     #set the default values
                     _rl_config = schemas.RateLimiter(id = edited_route, route=edited_route, interval=60, rate_limit=10, last_updated=get_time_now(), created_at=get_time_now(), unique_id="host")
                     _rl_configs[edited_route] = _rl_config
```

### Comparing `sixth-sense-0.0.3/sixth_sense/utils/encryption_utils.py` & `sixth-sense-0.0.4/sixth_sense/utils/encryption_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-sense-0.0.3/sixth_sense/utils/time_utils.py` & `sixth-sense-0.0.4/sixth_sense/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-sense-0.0.3/sixth_sense.egg-info/PKG-INFO` & `sixth-sense-0.0.4/sixth_sense.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sixth-sense
-Version: 0.0.3
+Version: 0.0.4
 Summary: Six offical python ackage
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: Six is a package that helps you automate pen testing and also helps you protect your API from cybersecurity threats. Visit https://withsix.co to get started.
 Keywords: python,cybersecurity,pentesting,encryption,rate limiting,xss prevention
```

### Comparing `sixth-sense-0.0.3/sixth_sense.egg-info/SOURCES.txt` & `sixth-sense-0.0.4/sixth_sense.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,10 +9,12 @@
 sixth_sense.egg-info/requires.txt
 sixth_sense.egg-info/top_level.txt
 sixth_sense/middlewares/__init__.py
 sixth_sense/middlewares/encryption_middleware.py
 sixth_sense/middlewares/six_base_http_middleware.py
 sixth_sense/middlewares/six_independent_rate_limiter.py
 sixth_sense/middlewares/six_rate_limiter_middleware.py
+sixth_sense/pen_test/__init__.py
+sixth_sense/pen_test/auto_pen_test.py
 sixth_sense/utils/__init__.py
 sixth_sense/utils/encryption_utils.py
 sixth_sense/utils/time_utils.py
```

### Comparing `sixth-sense-0.0.3/sixth_sense.egg-info/requires.txt` & `sixth-sense-0.0.4/sixth_sense.egg-info/requires.txt`

 * *Files identical despite different names*

