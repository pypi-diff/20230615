# Comparing `tmp/FastWAPI-0.1.0.tar.gz` & `tmp/fastwapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastWAPI-0.1.0.tar", last modified: Thu Jun 15 10:44:08 2023, max compression
+gzip compressed data, was "fastwapi-0.1.1.tar", last modified: Thu Jun 15 10:59:41 2023, max compression
```

## Comparing `FastWAPI-0.1.0.tar` & `fastwapi-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 10:44:08.913417 FastWAPI-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-06-15 10:44:08.897418 FastWAPI-0.1.0/FastWAPI/
--rw-rw-rw-   0        0        0        0 2023-06-15 09:10:09.000000 FastWAPI-0.1.0/FastWAPI/__init__.py
--rw-rw-rw-   0        0        0     1364 2023-06-15 10:40:00.000000 FastWAPI-0.1.0/FastWAPI/fastwapi.py
-drwxrwxrwx   0        0        0        0 2023-06-15 10:44:08.911417 FastWAPI-0.1.0/FastWAPI.egg-info/
--rw-rw-rw-   0        0        0     4417 2023-06-15 10:44:08.000000 FastWAPI-0.1.0/FastWAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-15 10:44:08.000000 FastWAPI-0.1.0/FastWAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 10:44:08.000000 FastWAPI-0.1.0/FastWAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-15 10:44:08.000000 FastWAPI-0.1.0/FastWAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-15 10:44:08.000000 FastWAPI-0.1.0/FastWAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1062 2023-06-15 09:10:09.000000 FastWAPI-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4417 2023-06-15 10:44:08.912417 FastWAPI-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1710 2023-06-15 10:30:10.000000 FastWAPI-0.1.0/README.md
--rw-rw-rw-   0        0        0     1529 2023-06-15 10:38:57.000000 FastWAPI-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-15 10:44:08.913417 FastWAPI-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-15 10:59:41.962462 fastwapi-0.1.1/
+-rw-rw-rw-   0        0        0     1062 2023-06-15 09:10:09.000000 fastwapi-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4421 2023-06-15 10:59:41.962462 fastwapi-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1710 2023-06-15 10:30:10.000000 fastwapi-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 10:59:41.950461 fastwapi-0.1.1/fastwapi/
+-rw-rw-rw-   0        0        0        0 2023-06-15 09:10:09.000000 fastwapi-0.1.1/fastwapi/__init__.py
+-rw-rw-rw-   0        0        0     1364 2023-06-15 10:40:00.000000 fastwapi-0.1.1/fastwapi/fastwapi.py
+drwxrwxrwx   0        0        0        0 2023-06-15 10:59:41.961461 fastwapi-0.1.1/fastwapi.egg-info/
+-rw-rw-rw-   0        0        0     4421 2023-06-15 10:59:41.000000 fastwapi-0.1.1/fastwapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-06-15 10:59:41.000000 fastwapi-0.1.1/fastwapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 10:59:41.000000 fastwapi-0.1.1/fastwapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-15 10:59:41.000000 fastwapi-0.1.1/fastwapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 10:59:41.000000 fastwapi-0.1.1/fastwapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1533 2023-06-15 10:59:29.000000 fastwapi-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-15 10:59:41.962462 fastwapi-0.1.1/setup.cfg
```

### Comparing `FastWAPI-0.1.0/FastWAPI/fastwapi.py` & `fastwapi-0.1.1/fastwapi/fastwapi.py`

 * *Files identical despite different names*

### Comparing `FastWAPI-0.1.0/FastWAPI.egg-info/PKG-INFO` & `fastwapi-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: FastWAPI
-Version: 0.1.0
+Name: fastwapi
+Version: 0.1.1
 Summary: A simple API Websocket server to easily parse JSON
 Author-email: lonode <lonode-git@proton.me>
 License: MIT License
         
         Copyright (c) 2023 lonode
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -20,15 +20,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: Homepage, https://github.com/lonode/wapi
+Project-URL: Homepage, https://github.com/lonode/FastWAPI
 Keywords: websocket,api,json
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet
```

### Comparing `FastWAPI-0.1.0/LICENSE` & `fastwapi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FastWAPI-0.1.0/PKG-INFO` & `fastwapi-0.1.1/fastwapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: FastWAPI
-Version: 0.1.0
+Name: fastwapi
+Version: 0.1.1
 Summary: A simple API Websocket server to easily parse JSON
 Author-email: lonode <lonode-git@proton.me>
 License: MIT License
         
         Copyright (c) 2023 lonode
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -20,15 +20,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: Homepage, https://github.com/lonode/wapi
+Project-URL: Homepage, https://github.com/lonode/FastWAPI
 Keywords: websocket,api,json
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet
```

### Comparing `FastWAPI-0.1.0/README.md` & `fastwapi-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `FastWAPI-0.1.0/pyproject.toml` & `fastwapi-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # pyproject.toml
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "FastWAPI"
-version = "0.1.0"
+name = "fastwapi"
+version = "0.1.1"
 description = "A simple API Websocket server to easily parse JSON"
 readme = "README.md"
 authors = [{ name = "lonode", email = "lonode-git@proton.me" }]
 license = { file = "LICENSE" }
 classifiers = [
  "Intended Audience :: Information Technology",
     "Intended Audience :: System Administrators",
@@ -39,8 +39,8 @@
 dependencies = [
     "starlette",
     "pydantic"
 ]
 requires-python = ">=3.7"
 
 [project.urls]
-Homepage = "https://github.com/lonode/wapi"
+Homepage = "https://github.com/lonode/FastWAPI"
```

