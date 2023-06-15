# Comparing `tmp/turborest-0.1.3.tar.gz` & `tmp/turborest-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turborest-0.1.3.tar", last modified: Wed Jun 14 12:34:43 2023, max compression
+gzip compressed data, was "turborest-0.1.4.tar", last modified: Thu Jun 15 05:59:57 2023, max compression
```

## Comparing `turborest-0.1.3.tar` & `turborest-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:34:43.019371 turborest-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-14 12:34:43.019371 turborest-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-14 12:34:22.000000 turborest-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-14 12:34:22.000000 turborest-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 12:34:43.019371 turborest-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-14 12:34:22.000000 turborest-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:34:43.015370 turborest-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:34:43.019371 turborest-0.1.3/src/turborest/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-14 12:34:22.000000 turborest-0.1.3/src/turborest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-14 12:34:22.000000 turborest-0.1.3/src/turborest/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:34:43.019371 turborest-0.1.3/src/turborest/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-14 12:34:22.000000 turborest-0.1.3/src/turborest/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-14 12:34:22.000000 turborest-0.1.3/src/turborest/cmd/ping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:34:43.019371 turborest-0.1.3/src/turborest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-14 12:34:43.000000 turborest-0.1.3/src/turborest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-14 12:34:43.000000 turborest-0.1.3/src/turborest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:34:43.000000 turborest-0.1.3/src/turborest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 12:34:43.000000 turborest-0.1.3/src/turborest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:59:57.939832 turborest-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-15 05:59:57.939832 turborest-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-15 05:59:36.000000 turborest-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-15 05:59:36.000000 turborest-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 05:59:57.939832 turborest-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-15 05:59:36.000000 turborest-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:59:57.935832 turborest-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:59:57.935832 turborest-0.1.4/src/turborest/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-15 05:59:36.000000 turborest-0.1.4/src/turborest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-06-15 05:59:36.000000 turborest-0.1.4/src/turborest/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:59:57.939832 turborest-0.1.4/src/turborest/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-15 05:59:36.000000 turborest-0.1.4/src/turborest/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-15 05:59:36.000000 turborest-0.1.4/src/turborest/cmd/ping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:59:57.935832 turborest-0.1.4/src/turborest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-15 05:59:57.000000 turborest-0.1.4/src/turborest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-15 05:59:57.000000 turborest-0.1.4/src/turborest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 05:59:57.000000 turborest-0.1.4/src/turborest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 05:59:57.000000 turborest-0.1.4/src/turborest.egg-info/top_level.txt
```

### Comparing `turborest-0.1.3/PKG-INFO` & `turborest-0.1.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turborest
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library for monitoring files and directories for changes
 Home-page: https://github.com/bytesentinel-io/turborest
 Author: ByteSentinel.io
 Author-email: dev@bytesentinel.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -49,14 +49,32 @@
 
 def main():
     proxy = "http://localhost:8080"
     client = Client(format="json", proxy=proxy)
     client.get("https://api.bytesentinel.io/test")
 ```
 
+## Advanced Options
+
+```python
+from turborest import Client
+
+def main():
+    proxy = "http://localhost:8080"
+    endpoint = "https://api.bytesentinel.io/test"
+    auth = ("Bearer", "xyz")
+    client = Client(format="json", proxy=proxy, auth=auth)
+    client.set_user_agent("TestAgent/1.0.0")
+    client.set_success(print)
+    client.set_header("X-Test", "Test")
+    res = client.get(endpoint)
+
+    print(res.status_code)
+```
+
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 
 ### MIT License
```

### Comparing `turborest-0.1.3/README.md` & `turborest-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -36,14 +36,32 @@
 
 def main():
     proxy = "http://localhost:8080"
     client = Client(format="json", proxy=proxy)
     client.get("https://api.bytesentinel.io/test")
 ```
 
+## Advanced Options
+
+```python
+from turborest import Client
+
+def main():
+    proxy = "http://localhost:8080"
+    endpoint = "https://api.bytesentinel.io/test"
+    auth = ("Bearer", "xyz")
+    client = Client(format="json", proxy=proxy, auth=auth)
+    client.set_user_agent("TestAgent/1.0.0")
+    client.set_success(print)
+    client.set_header("X-Test", "Test")
+    res = client.get(endpoint)
+
+    print(res.status_code)
+```
+
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 
 ### MIT License
```

### Comparing `turborest-0.1.3/pyproject.toml` & `turborest-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = "turborest"
-version = "0.1.3"
+version = "0.1.4"
 description = "A library for monitoring files and directories for changes"
 long_description = """
 A library for monitoring files and directories for changes
 """
 license = "MIT"
 author = "ByteSentinel.io"
 author-email = "dev@bytesentinel.io"
```

### Comparing `turborest-0.1.3/setup.py` & `turborest-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="turborest",
-    version="0.1.3",
+    version="0.1.4",
     author="ByteSentinel.io",
     author_email="dev@bytesentinel.io",
     description="A library for monitoring files and directories for changes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bytesentinel-io/turborest",
     packages=find_packages(where="src"),
```

### Comparing `turborest-0.1.3/src/turborest/cmd/ping.py` & `turborest-0.1.4/src/turborest/cmd/ping.py`

 * *Files identical despite different names*

### Comparing `turborest-0.1.3/src/turborest.egg-info/PKG-INFO` & `turborest-0.1.4/src/turborest.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turborest
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library for monitoring files and directories for changes
 Home-page: https://github.com/bytesentinel-io/turborest
 Author: ByteSentinel.io
 Author-email: dev@bytesentinel.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -49,14 +49,32 @@
 
 def main():
     proxy = "http://localhost:8080"
     client = Client(format="json", proxy=proxy)
     client.get("https://api.bytesentinel.io/test")
 ```
 
+## Advanced Options
+
+```python
+from turborest import Client
+
+def main():
+    proxy = "http://localhost:8080"
+    endpoint = "https://api.bytesentinel.io/test"
+    auth = ("Bearer", "xyz")
+    client = Client(format="json", proxy=proxy, auth=auth)
+    client.set_user_agent("TestAgent/1.0.0")
+    client.set_success(print)
+    client.set_header("X-Test", "Test")
+    res = client.get(endpoint)
+
+    print(res.status_code)
+```
+
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 
 ### MIT License
```

