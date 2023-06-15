# Comparing `tmp/haralyzer-2.2.0.tar.gz` & `tmp/haralyzer-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haralyzer-2.2.0.tar", last modified: Mon Jan  2 20:54:33 2023, max compression
+gzip compressed data, was "haralyzer-2.3.0.tar", last modified: Thu Jun 15 07:40:00 2023, max compression
```

## Comparing `haralyzer-2.2.0.tar` & `haralyzer-2.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 20:54:33.229492 haralyzer-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-01-02 20:54:25.000000 haralyzer-2.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-01-02 20:54:33.229492 haralyzer-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-01-02 20:54:25.000000 haralyzer-2.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 20:54:33.225492 haralyzer-2.2.0/haralyzer/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-02 20:54:25.000000 haralyzer-2.2.0/haralyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33811 2023-01-02 20:54:25.000000 haralyzer-2.2.0/haralyzer/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-01-02 20:54:25.000000 haralyzer-2.2.0/haralyzer/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-01-02 20:54:25.000000 haralyzer-2.2.0/haralyzer/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-01-02 20:54:25.000000 haralyzer-2.2.0/haralyzer/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-01-02 20:54:25.000000 haralyzer-2.2.0/haralyzer/multihar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 20:54:33.229492 haralyzer-2.2.0/haralyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-01-02 20:54:33.000000 haralyzer-2.2.0/haralyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-01-02 20:54:33.000000 haralyzer-2.2.0/haralyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-02 20:54:33.000000 haralyzer-2.2.0/haralyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-02 20:54:33.000000 haralyzer-2.2.0/haralyzer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-02 20:54:33.000000 haralyzer-2.2.0/haralyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-02 20:54:33.000000 haralyzer-2.2.0/haralyzer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-02 20:54:33.229492 haralyzer-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-01-02 20:54:25.000000 haralyzer-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:40:00.141870 haralyzer-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-15 07:39:49.000000 haralyzer-2.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-15 07:40:00.141870 haralyzer-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-15 07:39:49.000000 haralyzer-2.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:40:00.141870 haralyzer-2.3.0/haralyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-15 07:39:49.000000 haralyzer-2.3.0/haralyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33811 2023-06-15 07:39:49.000000 haralyzer-2.3.0/haralyzer/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-15 07:39:49.000000 haralyzer-2.3.0/haralyzer/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-06-15 07:39:49.000000 haralyzer-2.3.0/haralyzer/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-15 07:39:49.000000 haralyzer-2.3.0/haralyzer/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-06-15 07:39:49.000000 haralyzer-2.3.0/haralyzer/multihar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:40:00.141870 haralyzer-2.3.0/haralyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-15 07:39:59.000000 haralyzer-2.3.0/haralyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-15 07:40:00.000000 haralyzer-2.3.0/haralyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:39:59.000000 haralyzer-2.3.0/haralyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:39:59.000000 haralyzer-2.3.0/haralyzer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 07:39:59.000000 haralyzer-2.3.0/haralyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 07:39:59.000000 haralyzer-2.3.0/haralyzer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 07:40:00.141870 haralyzer-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-15 07:39:49.000000 haralyzer-2.3.0/setup.py
```

### Comparing `haralyzer-2.2.0/LICENSE.txt` & `haralyzer-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `haralyzer-2.2.0/PKG-INFO` & `haralyzer-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haralyzer
-Version: 2.2.0
+Version: 2.3.0
 Summary: A python framework for getting useful stuff out of HAR files
 Home-page: https://github.com/haralyzer/haralyzer
 Author: Justin Crown
 Author-email: justincrown1@gmail.com
 License: MIT
 Download-URL: https://github.com/haralyzer/haralyzer/releases/latest
 Project-URL: Changelog, https://github.com/haralyzer/haralyzer/blob/master/HISTORY.rst
```

### Comparing `haralyzer-2.2.0/README.rst` & `haralyzer-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `haralyzer-2.2.0/haralyzer/assets.py` & `haralyzer-2.3.0/haralyzer/assets.py`

 * *Files identical despite different names*

### Comparing `haralyzer-2.2.0/haralyzer/http.py` & `haralyzer-2.3.0/haralyzer/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 
     def __str__(self):
         return f"HarEntry.Request for {self.url}"
 
     def __repr__(self):
         return f"HarEntry.Request for {self.url}"
 
+    def _start_line(self) -> str:
+        """
+        :return: Request specific start line
+        :rtype: str
+        """
+        return f"{self.method} {self.url} {self.httpVersion}"
+
     # Root Level values
 
     @cached_property
     def bodySize(self) -> int:
         """
         :return: Body size of the request
         :rtype: int
@@ -157,14 +164,21 @@
 
     def __str__(self) -> str:
         return f"HarEntry.Response for {self.url}"
 
     def __repr__(self) -> str:
         return f"HarEntry.Response for {self.url}"
 
+    def _start_line(self) -> str:
+        """
+        :return: Response specific start line (status-line)
+        :rtype: str
+        """
+        return f"{self.httpVersion} {self.status} {self.statusText}"
+
     # Root Level values
 
     @cached_property
     def bodySize(self) -> int:
         """
         :return: Body Size
         :rtype: int
```

### Comparing `haralyzer-2.2.0/haralyzer/mixins.py` & `haralyzer-2.3.0/haralyzer/mixins.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Mixin Objects that allow for shared methods"""
+import abc
 from collections.abc import MutableMapping
 from typing import Any, Optional
+
 from cached_property import cached_property
 
 
 class GetHeaders:
     # pylint: disable=R0903
     """Mixin to get a header"""
 
@@ -18,14 +20,30 @@
         :rtype: Optional[str]
         """
         for header in self.raw_entry["headers"]:
             if header["name"].lower() == name.lower():
                 return header["value"]
         return None
 
+    @cached_property
+    def _formatted_headers(self) -> str:
+        """
+        Returns a formatted string of the headers in `KEY: VALUE` format
+
+        :return: string of all headers
+        :rtype: str
+        """
+        formatted_headers = ""
+
+        for header in self.raw_entry["headers"]:
+            name, value = header["name"], header["value"]
+            formatted_headers += f"{name}: {value}\n"
+
+        return formatted_headers
+
 
 class MimicDict(MutableMapping):
     """Mixin for functions to mimic a dictionary for backward compatibility"""
 
     def __getitem__(self, item: str) -> Any:
         return self.raw_entry[item]
 
@@ -55,7 +73,22 @@
         """
         Headers from the entry
 
         :return: Headers from both request and response
         :rtype: list
         """
         return self.raw_entry["headers"]
+
+    @cached_property
+    def formatted(self) -> str:
+        """
+        Formatted HttpTransaction string for pretty print.
+
+        :return: formatted string
+        :rtype: str
+        """
+        body = self.text if self.text else ""
+        return f"{self._start_line()}\n{self._formatted_headers}\n{body}"
+
+    @abc.abstractmethod
+    def _start_line(self) -> str:
+        pass
```

### Comparing `haralyzer-2.2.0/haralyzer/multihar.py` & `haralyzer-2.3.0/haralyzer/multihar.py`

 * *Files identical despite different names*

### Comparing `haralyzer-2.2.0/haralyzer.egg-info/PKG-INFO` & `haralyzer-2.3.0/haralyzer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haralyzer
-Version: 2.2.0
+Version: 2.3.0
 Summary: A python framework for getting useful stuff out of HAR files
 Home-page: https://github.com/haralyzer/haralyzer
 Author: Justin Crown
 Author-email: justincrown1@gmail.com
 License: MIT
 Download-URL: https://github.com/haralyzer/haralyzer/releases/latest
 Project-URL: Changelog, https://github.com/haralyzer/haralyzer/blob/master/HISTORY.rst
```

### Comparing `haralyzer-2.2.0/setup.py` & `haralyzer-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 test_reqs = open("requirements-dev.txt").readlines()
 
 
 readme = open('README.rst').read()
 
 setup(
         name='haralyzer',
-        version='2.2.0',
+        version='2.3.0',
         description='A python framework for getting useful stuff out of HAR files',
         long_description=readme,
         long_description_content_type="text/x-rst",
         author='Justin Crown',
         author_email='justincrown1@gmail.com',
         url='https://github.com/haralyzer/haralyzer',
         download_url='https://github.com/haralyzer/haralyzer/releases/latest',
```

