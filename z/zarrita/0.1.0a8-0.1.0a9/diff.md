# Comparing `tmp/zarrita-0.1.0a8.tar.gz` & `tmp/zarrita-0.1.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zarrita-0.1.0a8.tar", max compression
+gzip compressed data, was "zarrita-0.1.0a9.tar", max compression
```

## Comparing `zarrita-0.1.0a8.tar` & `zarrita-0.1.0a9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1105 2023-05-09 09:12:03.956626 zarrita-0.1.0a8/LICENSE
--rw-r--r--   0        0        0     2311 2023-06-11 20:17:59.556412 zarrita-0.1.0a8/README.md
--rw-r--r--   0        0        0      736 2023-06-12 17:39:29.366212 zarrita-0.1.0a8/pyproject.toml
--rw-r--r--   0        0        0     1144 2023-06-11 20:17:59.559200 zarrita-0.1.0a8/zarrita/__init__.py
--rw-r--r--   0        0        0    19734 2023-06-12 13:32:56.555155 zarrita-0.1.0a8/zarrita/array.py
--rw-r--r--   0        0        0    13272 2023-06-12 13:33:40.509399 zarrita-0.1.0a8/zarrita/array_v2.py
--rw-r--r--   0        0        0    12363 2023-06-09 11:37:23.257106 zarrita-0.1.0a8/zarrita/codecs.py
--rw-r--r--   0        0        0     4314 2023-06-07 20:03:42.377098 zarrita-0.1.0a8/zarrita/common.py
--rw-r--r--   0        0        0     3830 2023-06-11 20:17:59.560239 zarrita-0.1.0a8/zarrita/group.py
--rw-r--r--   0        0        0     4353 2023-06-11 20:17:59.560496 zarrita-0.1.0a8/zarrita/group_v2.py
--rw-r--r--   0        0        0     7259 2023-06-07 12:49:15.942016 zarrita-0.1.0a8/zarrita/indexing.py
--rw-r--r--   0        0        0     5374 2023-06-08 07:17:39.694424 zarrita-0.1.0a8/zarrita/metadata.py
--rw-r--r--   0        0        0    20531 2023-06-08 12:06:20.763281 zarrita-0.1.0a8/zarrita/sharding.py
--rw-r--r--   0        0        0     8427 2023-06-12 13:31:41.021584 zarrita-0.1.0a8/zarrita/store.py
--rw-r--r--   0        0        0     2555 2023-06-02 09:33:41.528984 zarrita-0.1.0a8/zarrita/sync.py
--rw-r--r--   0        0        0     3783 2023-06-11 20:17:59.561195 zarrita-0.1.0a8/zarrita/value_handle.py
--rw-r--r--   0        0        0     3025 1970-01-01 00:00:00.000000 zarrita-0.1.0a8/PKG-INFO
+-rw-r--r--   0        0        0     1105 2023-05-09 09:12:03.956626 zarrita-0.1.0a9/LICENSE
+-rw-r--r--   0        0        0     2311 2023-06-11 20:17:59.556412 zarrita-0.1.0a9/README.md
+-rw-r--r--   0        0        0      736 2023-06-13 08:06:51.770379 zarrita-0.1.0a9/pyproject.toml
+-rw-r--r--   0        0        0     1144 2023-06-11 20:17:59.559200 zarrita-0.1.0a9/zarrita/__init__.py
+-rw-r--r--   0        0        0    19817 2023-06-13 07:12:01.915958 zarrita-0.1.0a9/zarrita/array.py
+-rw-r--r--   0        0        0    13272 2023-06-13 07:12:05.873448 zarrita-0.1.0a9/zarrita/array_v2.py
+-rw-r--r--   0        0        0    12363 2023-06-09 11:37:23.257106 zarrita-0.1.0a9/zarrita/codecs.py
+-rw-r--r--   0        0        0     4314 2023-06-07 20:03:42.377098 zarrita-0.1.0a9/zarrita/common.py
+-rw-r--r--   0        0        0     3830 2023-06-11 20:17:59.560239 zarrita-0.1.0a9/zarrita/group.py
+-rw-r--r--   0        0        0     4353 2023-06-11 20:17:59.560496 zarrita-0.1.0a9/zarrita/group_v2.py
+-rw-r--r--   0        0        0     7259 2023-06-07 12:49:15.942016 zarrita-0.1.0a9/zarrita/indexing.py
+-rw-r--r--   0        0        0     5374 2023-06-08 07:17:39.694424 zarrita-0.1.0a9/zarrita/metadata.py
+-rw-r--r--   0        0        0    20531 2023-06-08 12:06:20.763281 zarrita-0.1.0a9/zarrita/sharding.py
+-rw-r--r--   0        0        0     8427 2023-06-12 13:31:41.021584 zarrita-0.1.0a9/zarrita/store.py
+-rw-r--r--   0        0        0     2555 2023-06-02 09:33:41.528984 zarrita-0.1.0a9/zarrita/sync.py
+-rw-r--r--   0        0        0     3783 2023-06-11 20:17:59.561195 zarrita-0.1.0a9/zarrita/value_handle.py
+-rw-r--r--   0        0        0     3025 1970-01-01 00:00:00.000000 zarrita-0.1.0a9/PKG-INFO
```

### Comparing `zarrita-0.1.0a8/LICENSE` & `zarrita-0.1.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a8/README.md` & `zarrita-0.1.0a9/README.md`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a8/pyproject.toml` & `zarrita-0.1.0a9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zarrita"
-version = "0.1.0a8"
+version = "0.1.0a9"
 description = ""
 authors = ["Norman Rzepka <code@normanrz.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
```

### Comparing `zarrita-0.1.0a8/zarrita/__init__.py` & `zarrita-0.1.0a9/zarrita/__init__.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a8/zarrita/array.py` & `zarrita-0.1.0a9/zarrita/array.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,14 +312,18 @@
         return len(self.metadata.shape)
 
     @property
     def shape(self) -> ChunkCoords:
         return self.metadata.shape
 
     @property
+    def dtype(self) -> np.dtype:
+        return self.metadata.dtype
+
+    @property
     def _core_metadata(self) -> CoreArrayMetadata:
         return CoreArrayMetadata(
             shape=self.metadata.shape,
             chunk_shape=self.metadata.chunk_grid.configuration.chunk_shape,
             data_type=self.metadata.data_type,
             fill_value=self.metadata.fill_value,
             runtime_configuration=self.runtime_configuration,
```

### Comparing `zarrita-0.1.0a8/zarrita/array_v2.py` & `zarrita-0.1.0a9/zarrita/array_v2.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a8/zarrita/codecs.py` & `zarrita-0.1.0a9/zarrita/codecs.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a8/zarrita/common.py` & `zarrita-0.1.0a9/zarrita/common.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a8/zarrita/group.py` & `zarrita-0.1.0a9/zarrita/group.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a8/zarrita/group_v2.py` & `zarrita-0.1.0a9/zarrita/group_v2.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a8/zarrita/indexing.py` & `zarrita-0.1.0a9/zarrita/indexing.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a8/zarrita/metadata.py` & `zarrita-0.1.0a9/zarrita/metadata.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a8/zarrita/sharding.py` & `zarrita-0.1.0a9/zarrita/sharding.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a8/zarrita/store.py` & `zarrita-0.1.0a9/zarrita/store.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a8/zarrita/sync.py` & `zarrita-0.1.0a9/zarrita/sync.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a8/zarrita/value_handle.py` & `zarrita-0.1.0a9/zarrita/value_handle.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a8/PKG-INFO` & `zarrita-0.1.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zarrita
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: 
 License: MIT
 Author: Norman Rzepka
 Author-email: code@normanrz.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

