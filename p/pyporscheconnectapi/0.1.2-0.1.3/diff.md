# Comparing `tmp/pyporscheconnectapi-0.1.2.tar.gz` & `tmp/pyporscheconnectapi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyporscheconnectapi-0.1.2.tar", last modified: Wed Jun 14 21:33:28 2023, max compression
+gzip compressed data, was "pyporscheconnectapi-0.1.3.tar", last modified: Thu Jun 15 11:35:55 2023, max compression
```

## Comparing `pyporscheconnectapi-0.1.2.tar` & `pyporscheconnectapi-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:33:28.456955 pyporscheconnectapi-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 21:33:18.000000 pyporscheconnectapi-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-14 21:33:28.456955 pyporscheconnectapi-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-14 21:33:18.000000 pyporscheconnectapi-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:33:28.452955 pyporscheconnectapi-0.1.2/pyporscheconnectapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 21:33:18.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10930 2023-06-14 21:33:18.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    19856 2023-06-14 21:33:18.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-06-14 21:33:18.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-14 21:33:18.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:33:28.456955 pyporscheconnectapi-0.1.2/pyporscheconnectapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-14 21:33:28.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-14 21:33:28.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:33:28.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-14 21:33:28.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-14 21:33:28.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 21:33:28.000000 pyporscheconnectapi-0.1.2/pyporscheconnectapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-14 21:33:28.456955 pyporscheconnectapi-0.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      951 2023-06-14 21:33:18.000000 pyporscheconnectapi-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:55.986906 pyporscheconnectapi-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-15 11:35:39.000000 pyporscheconnectapi-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-15 11:35:55.986906 pyporscheconnectapi-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-15 11:35:39.000000 pyporscheconnectapi-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:55.986906 pyporscheconnectapi-0.1.3/pyporscheconnectapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:39.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10930 2023-06-15 11:35:39.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19856 2023-06-15 11:35:39.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-06-15 11:35:39.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-15 11:35:39.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:55.986906 pyporscheconnectapi-0.1.3/pyporscheconnectapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-15 11:35:55.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-15 11:35:55.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:35:55.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 11:35:55.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 11:35:55.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 11:35:55.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-15 11:35:55.986906 pyporscheconnectapi-0.1.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      951 2023-06-15 11:35:39.000000 pyporscheconnectapi-0.1.3/setup.py
```

### Comparing `pyporscheconnectapi-0.1.2/LICENSE` & `pyporscheconnectapi-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyporscheconnectapi-0.1.2/PKG-INFO` & `pyporscheconnectapi-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyporscheconnectapi
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python library and CLI for communicating with Porsche Connect API.
 Home-page: https://github.com/cjne/pyporscheconnectapi
 Author: Johan Isaksson
 Author-email: johan@generatorhallen.se
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pyporscheconnectapi-0.1.2/README.md` & `pyporscheconnectapi-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyporscheconnectapi-0.1.2/pyporscheconnectapi/cli.py` & `pyporscheconnectapi-0.1.3/pyporscheconnectapi/cli.py`

 * *Files identical despite different names*

### Comparing `pyporscheconnectapi-0.1.2/pyporscheconnectapi/client.py` & `pyporscheconnectapi-0.1.3/pyporscheconnectapi/client.py`

 * *Files identical despite different names*

### Comparing `pyporscheconnectapi-0.1.2/pyporscheconnectapi/connection.py` & `pyporscheconnectapi-0.1.3/pyporscheconnectapi/connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,41 +62,31 @@
         password: Text = None,
         websession: aiohttp.ClientSession = None,
         language: Text = "de",
         country: Text = "DE",
         tokens=None,
     ) -> None:
         """Initialize connection object."""
-        self.porscheCookiedomain: Text = "https://login.porsche.com"
-        self.porscheLogin: Text = "https://login.porsche.com/auth/de/de_DE"
-        self.porscheLoginAuth: Text = (
-            "https://login.porsche.com/auth/api/v1/de/de_DE/public/login"
-        )
-        self.porscheAPIAuth: Text = "https://login.porsche.com/as/authorization.oauth2"
-        self.porscheAPIToken: Text = "https://login.porsche.com/as/token.oauth2"
-        self.porscheAPI: Text = (
-            "https://connect-portal.porsche.com/core/api/v3/de/de_DE"
-        )
         self.porscheApplications = {
             "api": {
                 "client_id": CLIENT_ID,
                 "redirect_uri": REDIRECT_URI,
                 "prefix": "https://api.porsche.com/core/api/",
             },
             "profile": {
                 "client_id": CLIENT_ID,
                 "api_key": "QPw3VOLAMfI7r0nmRY8ELq4RzZpZeXEE",
                 "redirect_uri": REDIRECT_URI,
                 "prefix": "https://api.porsche.com/profiles",
             },
-            "auth": {
-                "client_id": "4mPO3OE5Srjb1iaUGWsbqKBvvesya8oA",
-                "redirect_uri": "https://my.porsche.com/core/de/de_DE/",
-                "prefix": "https://login.porsche.com",
-            },
+            # "auth": {
+            #     "client_id": "4mPO3OE5Srjb1iaUGWsbqKBvvesya8oA",
+            #     "redirect_uri": "https://my.porsche.com/core/de/de_DE/",
+            #     "prefix": "https://login.porsche.com",
+            # },
             "carcontrol": {
                 #"client_id": "Ux8WmyzsOAGGmvmWnW7GLEjIILHEztAs",
                 "client_id": CLIENT_ID,
                 "redirect_uri": "https://my.porsche.com/myservices/auth/auth.html",
                 "prefix": "https://api.porsche.com/",
             },
         }
@@ -174,35 +164,36 @@
         auth_url = f"https://{AUTHORIZATION_SERVER}/login/callback"
         resume_url = ""
         async with self.websession.post(auth_url, headers={"Content-Type": "application/x-www-form-urlencoded"}, data=verify_body, allow_redirects=False) as resp:
             resume_url = resp.headers['Location']
             _LOGGER.debug(f"Resume at {resume_url}")
 
         _LOGGER.debug("Sleeping 2.5s...")
-        time.sleep(2.5)
+        await asyncio.sleep(2.5)
 
         # Resume auth
         auth_url = f"https://{{AUTHORIZATION_SERVER}}{resume_url}"
         async with self.websession.get(start_login_url, allow_redirects=False) as resp:
             location = resp.headers["Location"]
             params = urllib.parse.parse_qs(urllib.parse.urlparse(location).query)
             _LOGGER.debug(params)
             self.auth_state["code"] = params["code"][0]
             _LOGGER.debug(f"Got code {self.auth_state['code']}")
 
         _LOGGER.debug("Sleeping 2.5s...")
-        time.sleep(2.5)
+        await asyncio.sleep(2.5)
         
         self._isLoggedIn = True
         return True
 
     async def getAllTokens(self):
         now = calendar.timegm(datetime.datetime.now().timetuple())
         for applicationKey in self.porscheApplications:
             application = self.porscheApplications[applicationKey]
+            _LOGGER.debug(f"Get token for app {applicationKey}")
             token = self.tokens.get(application["client_id"], None)
             if token is None or token["expiration"] < now:
                 token = await self._requestToken(application)
                 self.tokens[application["client_id"]] = token
         self.isTokenRefreshed = False
         return self.tokens
 
@@ -210,15 +201,15 @@
         if not self._isLoggedIn or wasExpired:
             await self._login()
 
 
         _LOGGER.debug("POST to acces token endpoint...")
         auth_url = f"https://{AUTHORIZATION_SERVER}/oauth/token"
         auth_body = {
-                "client_id": CLIENT_ID,
+                "client_id": application['client_id'],
                 "grant_type": "authorization_code",
                 "code": self.auth_state['code'],
                 "redirect_uri": REDIRECT_URI
                 }
         _LOGGER.debug(auth_body)
         _LOGGER.debug( "Requesting access token for client id %s", application["client_id"])
         now = calendar.timegm(datetime.datetime.now().timetuple())
```

### Comparing `pyporscheconnectapi-0.1.2/pyporscheconnectapi/exceptions.py` & `pyporscheconnectapi-0.1.3/pyporscheconnectapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyporscheconnectapi-0.1.2/pyporscheconnectapi.egg-info/PKG-INFO` & `pyporscheconnectapi-0.1.3/pyporscheconnectapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyporscheconnectapi
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python library and CLI for communicating with Porsche Connect API.
 Home-page: https://github.com/cjne/pyporscheconnectapi
 Author: Johan Isaksson
 Author-email: johan@generatorhallen.se
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pyporscheconnectapi-0.1.2/setup.py` & `pyporscheconnectapi-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 
 setup(
     name="pyporscheconnectapi",
-    version="0.1.2",
+    version="0.1.3",
     author="Johan Isaksson",
     author_email="johan@generatorhallen.se",
     description="Python library and CLI for communicating with Porsche Connect API.",
     long_description=open("README.md", 'r').read(),
     long_description_content_type='text/markdown',
     include_package_data=True,
     url="https://github.com/cjne/pyporscheconnectapi",
```

