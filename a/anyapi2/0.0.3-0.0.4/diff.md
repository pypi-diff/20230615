# Comparing `tmp/anyapi2-0.0.3.tar.gz` & `tmp/anyapi2-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyapi2-0.0.3.tar", last modified: Fri Jun  9 16:48:36 2023, max compression
+gzip compressed data, was "anyapi2-0.0.4.tar", last modified: Thu Jun 15 14:06:34 2023, max compression
```

## Comparing `anyapi2-0.0.3.tar` & `anyapi2-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwx---   0 user      (1000) user      (1000)        0 2023-06-09 16:48:36.882136 anyapi2-0.0.3/
--rw-r--r--   0 user      (1000) user      (1000)     1084 2019-11-22 22:26:36.000000 anyapi2-0.0.3/LICENSE
--rw-rw----   0 user      (1000) user      (1000)     1210 2023-06-09 16:48:36.882136 anyapi2-0.0.3/PKG-INFO
--rw-rw----   0 user      (1000) user      (1000)      582 2022-09-26 21:27:44.000000 anyapi2-0.0.3/README.md
-drwxrwx---   0 user      (1000) user      (1000)        0 2023-06-09 16:48:36.882136 anyapi2-0.0.3/anyapi/
--rw-rw----   0 user      (1000) user      (1000)     2123 2023-06-09 16:46:01.000000 anyapi2-0.0.3/anyapi/__init__.py
--rw-rw----   0 user      (1000) user      (1000)      533 2022-09-27 14:24:22.000000 anyapi2-0.0.3/anyapi/cookies.py
-drwxrwx---   0 user      (1000) user      (1000)        0 2023-06-09 16:48:36.882136 anyapi2-0.0.3/anyapi2.egg-info/
--rw-rw----   0 user      (1000) user      (1000)     1210 2023-06-09 16:48:36.000000 anyapi2-0.0.3/anyapi2.egg-info/PKG-INFO
--rw-rw----   0 user      (1000) user      (1000)      217 2023-06-09 16:48:36.000000 anyapi2-0.0.3/anyapi2.egg-info/SOURCES.txt
--rw-rw----   0 user      (1000) user      (1000)        1 2023-06-09 16:48:36.000000 anyapi2-0.0.3/anyapi2.egg-info/dependency_links.txt
--rw-rw----   0 user      (1000) user      (1000)       33 2023-06-09 16:48:36.000000 anyapi2-0.0.3/anyapi2.egg-info/requires.txt
--rw-rw----   0 user      (1000) user      (1000)        7 2023-06-09 16:48:36.000000 anyapi2-0.0.3/anyapi2.egg-info/top_level.txt
--rw-rw----   0 user      (1000) user      (1000)       38 2023-06-09 16:48:36.882136 anyapi2-0.0.3/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1045 2023-06-09 16:47:23.000000 anyapi2-0.0.3/setup.py
+drwxrwx---   0 user      (1000) user      (1000)        0 2023-06-15 14:06:34.921685 anyapi2-0.0.4/
+-rw-r--r--   0 user      (1000) user      (1000)     1084 2019-11-22 22:26:36.000000 anyapi2-0.0.4/LICENSE
+-rw-rw----   0 user      (1000) user      (1000)     1210 2023-06-15 14:06:34.921685 anyapi2-0.0.4/PKG-INFO
+-rw-rw----   0 user      (1000) user      (1000)      582 2022-09-26 21:27:44.000000 anyapi2-0.0.4/README.md
+drwxrwx---   0 user      (1000) user      (1000)        0 2023-06-15 14:06:34.921685 anyapi2-0.0.4/anyapi/
+-rw-rw----   0 user      (1000) user      (1000)     2194 2023-06-15 14:00:34.000000 anyapi2-0.0.4/anyapi/__init__.py
+-rw-rw----   0 user      (1000) user      (1000)      533 2022-09-27 14:24:22.000000 anyapi2-0.0.4/anyapi/cookies.py
+-rw-rw----   0 user      (1000) user      (1000)       38 2023-06-15 13:53:47.000000 anyapi2-0.0.4/anyapi/exceptions.py
+drwxrwx---   0 user      (1000) user      (1000)        0 2023-06-15 14:06:34.921685 anyapi2-0.0.4/anyapi2.egg-info/
+-rw-rw----   0 user      (1000) user      (1000)     1210 2023-06-15 14:06:34.000000 anyapi2-0.0.4/anyapi2.egg-info/PKG-INFO
+-rw-rw----   0 user      (1000) user      (1000)      238 2023-06-15 14:06:34.000000 anyapi2-0.0.4/anyapi2.egg-info/SOURCES.txt
+-rw-rw----   0 user      (1000) user      (1000)        1 2023-06-15 14:06:34.000000 anyapi2-0.0.4/anyapi2.egg-info/dependency_links.txt
+-rw-rw----   0 user      (1000) user      (1000)       33 2023-06-15 14:06:34.000000 anyapi2-0.0.4/anyapi2.egg-info/requires.txt
+-rw-rw----   0 user      (1000) user      (1000)        7 2023-06-15 14:06:34.000000 anyapi2-0.0.4/anyapi2.egg-info/top_level.txt
+-rw-rw----   0 user      (1000) user      (1000)       38 2023-06-15 14:06:34.921685 anyapi2-0.0.4/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1045 2023-06-15 14:06:01.000000 anyapi2-0.0.4/setup.py
```

### Comparing `anyapi2-0.0.3/LICENSE` & `anyapi2-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anyapi2-0.0.3/PKG-INFO` & `anyapi2-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyapi2
-Version: 0.0.3
+Version: 0.0.4
 Summary: Boilerplate code for api integrations
 Home-page: https://github.com/c0ntribut0r/anyapi
 License: MIT
 Keywords: requests api
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `anyapi2-0.0.3/README.md` & `anyapi2-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `anyapi2-0.0.3/anyapi/__init__.py` & `anyapi2-0.0.4/anyapi/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,39 +22,42 @@
     adapter: requests.adapters.HTTPAdapter = requests.adapters.HTTPAdapter(
         pool_maxsize=8,
     )
     cookies: Path | None = None
 
     API_URL: ClassVar[str]
     TIMEOUT: ClassVar[int] = 10
-    DEFAULT_USER_AGENT: str = 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.126 Safari/537.36'
+    USER_AGENT: ClassVar[str] = 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.126 Safari/537.36'
+    HEADERS: ClassVar[dict] = {}
 
     def __post_init__(self):
         self.session.mount('http://', self.adapter)
         self.session.mount('https://', self.adapter)
         if self.cookies:
             self.session.cookies = load_cookies(self.cookies)
-        self.session.headers.update({
-            'user-agent': self.get_user_agent(),
-        })
 
-    def get_user_agent(self) -> str:
-        return self.DEFAULT_USER_AGENT
+    @property
+    def user_agent(self) -> str:
+        return self.USER_AGENT
 
     @retry(
         reraise=True,
         retry=retry_if_exception_type((TryAgain, requests.exceptions.ReadTimeout)),
         wait=wait_incrementing(start=1, increment=2),
         stop=stop_after_attempt(20),
     )
     def request(self, method: str, path: str, check: bool = True, **kwargs) -> requests.Response:
         if path.startswith('/'):
             path = self.API_URL + path
 
         kwargs.setdefault('timeout', self.TIMEOUT)
+        kwargs.setdefault('headers', {}).update({
+            'user-agent': self.user_agent,
+            **self.HEADERS,
+        })
         response = self.session.request(method, path, **kwargs)
 
         if response.status_code == requests.codes.too_many_requests:
             raise TryAgain()
 
         if check:
             response.raise_for_status()
```

### Comparing `anyapi2-0.0.3/anyapi/cookies.py` & `anyapi2-0.0.4/anyapi/cookies.py`

 * *Files identical despite different names*

### Comparing `anyapi2-0.0.3/anyapi2.egg-info/PKG-INFO` & `anyapi2-0.0.4/anyapi2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyapi2
-Version: 0.0.3
+Version: 0.0.4
 Summary: Boilerplate code for api integrations
 Home-page: https://github.com/c0ntribut0r/anyapi
 License: MIT
 Keywords: requests api
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `anyapi2-0.0.3/setup.py` & `anyapi2-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 # # allow setup.py to be run from any path
 # os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='anyapi2',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     include_package_data=True,
     install_requires=['requests==2.28.1', 'tenacity==8.1.0'],
     license='MIT',
     description='Boilerplate code for api integrations',
     long_description=(Path(__file__).parent / 'README.md').read_text(),
     long_description_content_type="text/markdown",
```

