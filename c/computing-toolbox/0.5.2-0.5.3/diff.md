# Comparing `tmp/computing-toolbox-0.5.2.tar.gz` & `tmp/computing-toolbox-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computing-toolbox-0.5.2.tar", last modified: Thu Jun 15 18:50:15 2023, max compression
+gzip compressed data, was "computing-toolbox-0.5.3.tar", last modified: Thu Jun 15 18:56:37 2023, max compression
```

## Comparing `computing-toolbox-0.5.2.tar` & `computing-toolbox-0.5.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:15.982325 computing-toolbox-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-15 18:50:15.982325 computing-toolbox-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 18:50:15.982325 computing-toolbox-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:15.978325 computing-toolbox-0.5.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:15.978325 computing-toolbox-0.5.2/src/computing_toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:15.982325 computing-toolbox-0.5.2/src/computing_toolbox/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/algorithms/split_range.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:15.982325 computing-toolbox-0.5.2/src/computing_toolbox/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/gcp/gs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/gcp/gs_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/gcp/secret_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:15.982325 computing-toolbox-0.5.2/src/computing_toolbox/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/utils/deep_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/utils/es_long_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    22006 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/utils/http_async_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/utils/http_fake_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/utils/http_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/utils/jsonl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/utils/tictoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:15.982325 computing-toolbox-0.5.2/src/computing_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-15 18:50:15.000000 computing-toolbox-0.5.2/src/computing_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-15 18:50:15.000000 computing-toolbox-0.5.2/src/computing_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 18:50:15.000000 computing-toolbox-0.5.2/src/computing_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-15 18:50:15.000000 computing-toolbox-0.5.2/src/computing_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 18:50:15.000000 computing-toolbox-0.5.2/src/computing_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:56:37.366077 computing-toolbox-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-15 18:56:27.000000 computing-toolbox-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-15 18:56:37.366077 computing-toolbox-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-15 18:56:27.000000 computing-toolbox-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-15 18:56:27.000000 computing-toolbox-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-15 18:56:27.000000 computing-toolbox-0.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 18:56:37.366077 computing-toolbox-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:56:37.362077 computing-toolbox-0.5.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:56:27.000000 computing-toolbox-0.5.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:56:37.362077 computing-toolbox-0.5.3/src/computing_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 18:56:27.000000 computing-toolbox-0.5.3/src/computing_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:56:37.362077 computing-toolbox-0.5.3/src/computing_toolbox/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:56:27.000000 computing-toolbox-0.5.3/src/computing_toolbox/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-15 18:56:27.000000 computing-toolbox-0.5.3/src/computing_toolbox/algorithms/split_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:56:37.362077 computing-toolbox-0.5.3/src/computing_toolbox/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:56:27.000000 computing-toolbox-0.5.3/src/computing_toolbox/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-15 18:56:27.000000 computing-toolbox-0.5.3/src/computing_toolbox/gcp/gs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-06-15 18:56:27.000000 computing-toolbox-0.5.3/src/computing_toolbox/gcp/gs_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-15 18:56:27.000000 computing-toolbox-0.5.3/src/computing_toolbox/gcp/secret_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:56:37.366077 computing-toolbox-0.5.3/src/computing_toolbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:56:27.000000 computing-toolbox-0.5.3/src/computing_toolbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-15 18:56:27.000000 computing-toolbox-0.5.3/src/computing_toolbox/utils/deep_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-15 18:56:27.000000 computing-toolbox-0.5.3/src/computing_toolbox/utils/es_long_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22006 2023-06-15 18:56:27.000000 computing-toolbox-0.5.3/src/computing_toolbox/utils/http_async_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-15 18:56:27.000000 computing-toolbox-0.5.3/src/computing_toolbox/utils/http_fake_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-15 18:56:27.000000 computing-toolbox-0.5.3/src/computing_toolbox/utils/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-15 18:56:27.000000 computing-toolbox-0.5.3/src/computing_toolbox/utils/jsonl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-15 18:56:27.000000 computing-toolbox-0.5.3/src/computing_toolbox/utils/tictoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:56:37.362077 computing-toolbox-0.5.3/src/computing_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-15 18:56:37.000000 computing-toolbox-0.5.3/src/computing_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-15 18:56:37.000000 computing-toolbox-0.5.3/src/computing_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 18:56:37.000000 computing-toolbox-0.5.3/src/computing_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-15 18:56:37.000000 computing-toolbox-0.5.3/src/computing_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 18:56:37.000000 computing-toolbox-0.5.3/src/computing_toolbox.egg-info/top_level.txt
```

### Comparing `computing-toolbox-0.5.2/LICENSE` & `computing-toolbox-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.2/PKG-INFO` & `computing-toolbox-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 0.5.2
+Version: 0.5.3
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-0.5.2/README.md` & `computing-toolbox-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.2/pyproject.toml` & `computing-toolbox-0.5.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "computing-toolbox"
-version = "0.5.2"
+version = "0.5.3"
 authors = [
   { name="Pedro Mayorga", email="ppmayorga80@gmail.com" },
 ]
 description = "Computing Toolbox for daily computations"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `computing-toolbox-0.5.2/src/computing_toolbox/algorithms/split_range.py` & `computing-toolbox-0.5.3/src/computing_toolbox/algorithms/split_range.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.2/src/computing_toolbox/gcp/gs.py` & `computing-toolbox-0.5.3/src/computing_toolbox/gcp/gs.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.2/src/computing_toolbox/gcp/gs_async.py` & `computing-toolbox-0.5.3/src/computing_toolbox/gcp/gs_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 from gcloud.aio.storage import Storage
 from tqdm import tqdm
 
 from computing_toolbox.gcp.gs import Gs
 
 
 class GsAsync:
-    """GS async class"""
+    """GS async class
+    if you want to read/write gzip files you only need to provide *.gz extension in the path     
+    """
+
     # default timeout for read and write operations
     DEFAULT_TIMEOUT: int = 3600
 
     @classmethod
     async def _exist_one(cls,
                          path: str,
                          timeout: int,
```

### Comparing `computing-toolbox-0.5.2/src/computing_toolbox/gcp/secret_manager.py` & `computing-toolbox-0.5.3/src/computing_toolbox/gcp/secret_manager.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.2/src/computing_toolbox/utils/deep_get.py` & `computing-toolbox-0.5.3/src/computing_toolbox/utils/deep_get.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.2/src/computing_toolbox/utils/es_long_search.py` & `computing-toolbox-0.5.3/src/computing_toolbox/utils/es_long_search.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.2/src/computing_toolbox/utils/http_async_request.py` & `computing-toolbox-0.5.3/src/computing_toolbox/utils/http_async_request.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.2/src/computing_toolbox/utils/http_fake_headers.py` & `computing-toolbox-0.5.3/src/computing_toolbox/utils/http_fake_headers.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.2/src/computing_toolbox/utils/http_request.py` & `computing-toolbox-0.5.3/src/computing_toolbox/utils/http_request.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.2/src/computing_toolbox/utils/jsonl.py` & `computing-toolbox-0.5.3/src/computing_toolbox/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.2/src/computing_toolbox/utils/tictoc.py` & `computing-toolbox-0.5.3/src/computing_toolbox/utils/tictoc.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.2/src/computing_toolbox.egg-info/PKG-INFO` & `computing-toolbox-0.5.3/src/computing_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 0.5.2
+Version: 0.5.3
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-0.5.2/src/computing_toolbox.egg-info/SOURCES.txt` & `computing-toolbox-0.5.3/src/computing_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

