# Comparing `tmp/computing-toolbox-0.5.1.tar.gz` & `tmp/computing-toolbox-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computing-toolbox-0.5.1.tar", last modified: Sat Jun 10 16:24:39 2023, max compression
+gzip compressed data, was "computing-toolbox-0.5.2.tar", last modified: Thu Jun 15 18:50:15 2023, max compression
```

## Comparing `computing-toolbox-0.5.1.tar` & `computing-toolbox-0.5.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:24:39.408208 computing-toolbox-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-10 16:24:27.000000 computing-toolbox-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-10 16:24:39.404208 computing-toolbox-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-10 16:24:27.000000 computing-toolbox-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-10 16:24:27.000000 computing-toolbox-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-10 16:24:27.000000 computing-toolbox-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 16:24:39.408208 computing-toolbox-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:24:39.400208 computing-toolbox-0.5.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:24:27.000000 computing-toolbox-0.5.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:24:39.400208 computing-toolbox-0.5.1/src/computing_toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-10 16:24:27.000000 computing-toolbox-0.5.1/src/computing_toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:24:39.400208 computing-toolbox-0.5.1/src/computing_toolbox/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:24:27.000000 computing-toolbox-0.5.1/src/computing_toolbox/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-10 16:24:27.000000 computing-toolbox-0.5.1/src/computing_toolbox/algorithms/split_range.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:24:39.404208 computing-toolbox-0.5.1/src/computing_toolbox/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:24:27.000000 computing-toolbox-0.5.1/src/computing_toolbox/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-10 16:24:27.000000 computing-toolbox-0.5.1/src/computing_toolbox/gcp/gs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-06-10 16:24:27.000000 computing-toolbox-0.5.1/src/computing_toolbox/gcp/gs_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-10 16:24:27.000000 computing-toolbox-0.5.1/src/computing_toolbox/gcp/secret_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:24:39.404208 computing-toolbox-0.5.1/src/computing_toolbox/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:24:27.000000 computing-toolbox-0.5.1/src/computing_toolbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-10 16:24:27.000000 computing-toolbox-0.5.1/src/computing_toolbox/utils/deep_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-10 16:24:27.000000 computing-toolbox-0.5.1/src/computing_toolbox/utils/es_long_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    22006 2023-06-10 16:24:27.000000 computing-toolbox-0.5.1/src/computing_toolbox/utils/http_async_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-10 16:24:27.000000 computing-toolbox-0.5.1/src/computing_toolbox/utils/http_fake_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-10 16:24:27.000000 computing-toolbox-0.5.1/src/computing_toolbox/utils/http_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-10 16:24:27.000000 computing-toolbox-0.5.1/src/computing_toolbox/utils/jsonl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-10 16:24:27.000000 computing-toolbox-0.5.1/src/computing_toolbox/utils/tictoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:24:39.400208 computing-toolbox-0.5.1/src/computing_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-10 16:24:39.000000 computing-toolbox-0.5.1/src/computing_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-10 16:24:39.000000 computing-toolbox-0.5.1/src/computing_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 16:24:39.000000 computing-toolbox-0.5.1/src/computing_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-10 16:24:39.000000 computing-toolbox-0.5.1/src/computing_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-10 16:24:39.000000 computing-toolbox-0.5.1/src/computing_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:15.982325 computing-toolbox-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-15 18:50:15.982325 computing-toolbox-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 18:50:15.982325 computing-toolbox-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:15.978325 computing-toolbox-0.5.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:15.978325 computing-toolbox-0.5.2/src/computing_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:15.982325 computing-toolbox-0.5.2/src/computing_toolbox/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/algorithms/split_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:15.982325 computing-toolbox-0.5.2/src/computing_toolbox/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/gcp/gs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/gcp/gs_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/gcp/secret_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:15.982325 computing-toolbox-0.5.2/src/computing_toolbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/utils/deep_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/utils/es_long_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22006 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/utils/http_async_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/utils/http_fake_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/utils/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/utils/jsonl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-15 18:50:06.000000 computing-toolbox-0.5.2/src/computing_toolbox/utils/tictoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:50:15.982325 computing-toolbox-0.5.2/src/computing_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-15 18:50:15.000000 computing-toolbox-0.5.2/src/computing_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-15 18:50:15.000000 computing-toolbox-0.5.2/src/computing_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 18:50:15.000000 computing-toolbox-0.5.2/src/computing_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-15 18:50:15.000000 computing-toolbox-0.5.2/src/computing_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 18:50:15.000000 computing-toolbox-0.5.2/src/computing_toolbox.egg-info/top_level.txt
```

### Comparing `computing-toolbox-0.5.1/LICENSE` & `computing-toolbox-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.1/PKG-INFO` & `computing-toolbox-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 0.5.1
+Version: 0.5.2
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-0.5.1/README.md` & `computing-toolbox-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.1/pyproject.toml` & `computing-toolbox-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "computing-toolbox"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
   { name="Pedro Mayorga", email="ppmayorga80@gmail.com" },
 ]
 description = "Computing Toolbox for daily computations"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `computing-toolbox-0.5.1/src/computing_toolbox/algorithms/split_range.py` & `computing-toolbox-0.5.2/src/computing_toolbox/algorithms/split_range.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.1/src/computing_toolbox/gcp/gs.py` & `computing-toolbox-0.5.2/src/computing_toolbox/gcp/gs.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.1/src/computing_toolbox/gcp/gs_async.py` & `computing-toolbox-0.5.2/src/computing_toolbox/gcp/gs_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Google Storage class with async operations"""
 import asyncio
+import gzip
 
 from gcloud.aio.storage import Storage
 from tqdm import tqdm
 
 from computing_toolbox.gcp.gs import Gs
 
 
@@ -112,15 +113,20 @@
         bucket, key = Gs.split(path)
 
         # 2. try to read the content in bytes
         try:
             async with Storage() as client:
                 content_in_bytes: bytes = await client.download(
                     bucket, key, timeout=timeout)
-                # 2.1 if success, convert to string
+                # 2.1 parse zip content if needed
+                content_in_bytes = gzip.decompress(
+                    content_in_bytes) if path.endswith(
+                        ".gz") else content_in_bytes
+
+                # 2.2 if success, convert to string.
                 content = content_in_bytes.decode("utf8")
         except Exception:
             # 2.2 if fails, set content to None
             content = None
 
         # 3. update progressbar if defined
         _ = tqdm_pbar.update() if tqdm_pbar else None
@@ -195,14 +201,16 @@
         :return: the number of bytes written
         """
         # 1. get the bucket and key
         bucket, key = Gs.split(path)
 
         # 2. try to write the content
         try:
+            content = gzip.compress(
+                content.encode("utf8")) if path.endswith(".gz") else content
             async with Storage() as client:
                 response = await client.upload(bucket,
                                                key,
                                                content,
                                                timeout=timeout)
                 # 2.1 if success get the number of bytes written
                 n_bytes = int(response["size"])
```

### Comparing `computing-toolbox-0.5.1/src/computing_toolbox/gcp/secret_manager.py` & `computing-toolbox-0.5.2/src/computing_toolbox/gcp/secret_manager.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.1/src/computing_toolbox/utils/deep_get.py` & `computing-toolbox-0.5.2/src/computing_toolbox/utils/deep_get.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.1/src/computing_toolbox/utils/es_long_search.py` & `computing-toolbox-0.5.2/src/computing_toolbox/utils/es_long_search.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.1/src/computing_toolbox/utils/http_async_request.py` & `computing-toolbox-0.5.2/src/computing_toolbox/utils/http_async_request.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.1/src/computing_toolbox/utils/http_fake_headers.py` & `computing-toolbox-0.5.2/src/computing_toolbox/utils/http_fake_headers.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.1/src/computing_toolbox/utils/http_request.py` & `computing-toolbox-0.5.2/src/computing_toolbox/utils/http_request.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.1/src/computing_toolbox/utils/jsonl.py` & `computing-toolbox-0.5.2/src/computing_toolbox/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.1/src/computing_toolbox/utils/tictoc.py` & `computing-toolbox-0.5.2/src/computing_toolbox/utils/tictoc.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-0.5.1/src/computing_toolbox.egg-info/PKG-INFO` & `computing-toolbox-0.5.2/src/computing_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 0.5.1
+Version: 0.5.2
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-0.5.1/src/computing_toolbox.egg-info/SOURCES.txt` & `computing-toolbox-0.5.2/src/computing_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

