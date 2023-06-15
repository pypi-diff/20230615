# Comparing `tmp/configzen-0.3.6.tar.gz` & `tmp/configzen-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.3.6.tar", max compression
+gzip compressed data, was "configzen-0.3.7.tar", max compression
```

## Comparing `configzen-0.3.6.tar` & `configzen-0.3.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      979 2023-06-15 09:10:26.257090 configzen-0.3.6/configzen/__init__.py
--rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.3.6/configzen/__main__.py
--rw-r--r--   0        0        0    67816 2023-06-15 18:54:00.040515 configzen-0.3.6/configzen/config.py
--rw-r--r--   0        0        0     3232 2023-06-15 09:05:45.207916 configzen-0.3.6/configzen/decorators.py
--rw-r--r--   0        0        0     3607 2023-06-15 00:25:22.104007 configzen-0.3.6/configzen/errors.py
--rw-r--r--   0        0        0      544 2023-06-15 09:10:51.539939 configzen-0.3.6/configzen/field.py
--rw-r--r--   0        0        0    25977 2023-06-15 09:05:45.230906 configzen-0.3.6/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.3.6/configzen/py.typed
--rw-r--r--   0        0        0     4599 2023-06-15 09:11:04.738125 configzen-0.3.6/configzen/route.py
--rw-r--r--   0        0        0     1124 2023-06-15 09:10:42.331286 configzen-0.3.6/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.3.6/LICENSE
--rw-r--r--   0        0        0     1255 2023-06-15 18:54:17.172403 configzen-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     7371 2023-06-13 02:20:30.758785 configzen-0.3.6/README.md
--rw-r--r--   0        0        0     8001 1970-01-01 00:00:00.000000 configzen-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0      979 2023-06-15 09:10:26.257090 configzen-0.3.7/configzen/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.3.7/configzen/__main__.py
+-rw-r--r--   0        0        0    67816 2023-06-15 18:54:00.040515 configzen-0.3.7/configzen/config.py
+-rw-r--r--   0        0        0     3232 2023-06-15 09:05:45.207916 configzen-0.3.7/configzen/decorators.py
+-rw-r--r--   0        0        0     3607 2023-06-15 00:25:22.104007 configzen-0.3.7/configzen/errors.py
+-rw-r--r--   0        0        0      544 2023-06-15 09:10:51.539939 configzen-0.3.7/configzen/field.py
+-rw-r--r--   0        0        0    26185 2023-06-15 21:21:22.530453 configzen-0.3.7/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.3.7/configzen/py.typed
+-rw-r--r--   0        0        0     4599 2023-06-15 09:11:04.738125 configzen-0.3.7/configzen/route.py
+-rw-r--r--   0        0        0     1124 2023-06-15 09:10:42.331286 configzen-0.3.7/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.3.7/LICENSE
+-rw-r--r--   0        0        0     1255 2023-06-15 21:21:53.913600 configzen-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     7371 2023-06-13 02:20:30.758785 configzen-0.3.7/README.md
+-rw-r--r--   0        0        0     8001 1970-01-01 00:00:00.000000 configzen-0.3.7/PKG-INFO
```

### Comparing `configzen-0.3.6/configzen/__init__.py` & `configzen-0.3.7/configzen/__init__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.6/configzen/__main__.py` & `configzen-0.3.7/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.6/configzen/config.py` & `configzen-0.3.7/configzen/config.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.6/configzen/decorators.py` & `configzen-0.3.7/configzen/decorators.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.6/configzen/errors.py` & `configzen-0.3.7/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.6/configzen/field.py` & `configzen-0.3.7/configzen/field.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.6/configzen/processor.py` & `configzen-0.3.7/configzen/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -705,16 +705,18 @@
                 }
                 if overrides_for_key:
                     export_key = agent.processor_class.extension_prefix + key
                     overrides[export_key] = overrides_for_key
 
             elif is_list_like(value):
                 cls.export(value)
+                if value != counterpart_value:
+                    overrides[key] = counterpart_value
 
-            elif counterpart_value != value:
+            elif value != counterpart_value:
                 overrides[key] = counterpart_value
                 del substituted_values[key]
 
         for value in state.values():
             cls.export(value)
 
         cls._export_finalize(
@@ -779,14 +781,16 @@
                 }
                 if overrides_for_key:
                     export_key = agent.processor_class.extension_prefix + key
                     overrides[export_key] = overrides_for_key
 
             elif is_list_like(value):
                 await cls.export_async(value)
+                if value != counterpart_value:
+                    overrides[key] = counterpart_value
 
             elif counterpart_value != value:
                 overrides[key] = counterpart_value
                 del substituted_values[key]
 
         for value in state.values():
             await cls.export_async(value)
```

### Comparing `configzen-0.3.6/configzen/route.py` & `configzen-0.3.7/configzen/route.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.6/configzen/typedefs.py` & `configzen-0.3.7/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.6/LICENSE` & `configzen-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.3.6/pyproject.toml` & `configzen-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.3.6"
+version = "0.3.7"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.3.6/README.md` & `configzen-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.3.6/PKG-INFO` & `configzen-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.3.6
+Version: 0.3.7
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

