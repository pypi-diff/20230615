# Comparing `tmp/configzen-0.3.3.tar.gz` & `tmp/configzen-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.3.3.tar", max compression
+gzip compressed data, was "configzen-0.3.4.tar", max compression
```

## Comparing `configzen-0.3.3.tar` & `configzen-0.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      979 2023-06-15 09:10:26.257090 configzen-0.3.3/configzen/__init__.py
--rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.3.3/configzen/__main__.py
--rw-r--r--   0        0        0    67651 2023-06-15 09:09:10.106723 configzen-0.3.3/configzen/config.py
--rw-r--r--   0        0        0     3232 2023-06-15 09:05:45.207916 configzen-0.3.3/configzen/decorators.py
--rw-r--r--   0        0        0     3607 2023-06-15 00:25:22.104007 configzen-0.3.3/configzen/errors.py
--rw-r--r--   0        0        0      544 2023-06-15 09:10:51.539939 configzen-0.3.3/configzen/field.py
--rw-r--r--   0        0        0    25977 2023-06-15 09:05:45.230906 configzen-0.3.3/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.3.3/configzen/py.typed
--rw-r--r--   0        0        0     4599 2023-06-15 09:11:04.738125 configzen-0.3.3/configzen/route.py
--rw-r--r--   0        0        0     1124 2023-06-15 09:10:42.331286 configzen-0.3.3/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.3.3/LICENSE
--rw-r--r--   0        0        0     1255 2023-06-15 09:11:56.327727 configzen-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     7371 2023-06-13 02:20:30.758785 configzen-0.3.3/README.md
--rw-r--r--   0        0        0     8001 1970-01-01 00:00:00.000000 configzen-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      979 2023-06-15 09:10:26.257090 configzen-0.3.4/configzen/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.3.4/configzen/__main__.py
+-rw-r--r--   0        0        0    67481 2023-06-15 09:13:30.986779 configzen-0.3.4/configzen/config.py
+-rw-r--r--   0        0        0     3232 2023-06-15 09:05:45.207916 configzen-0.3.4/configzen/decorators.py
+-rw-r--r--   0        0        0     3607 2023-06-15 00:25:22.104007 configzen-0.3.4/configzen/errors.py
+-rw-r--r--   0        0        0      544 2023-06-15 09:10:51.539939 configzen-0.3.4/configzen/field.py
+-rw-r--r--   0        0        0    25977 2023-06-15 09:05:45.230906 configzen-0.3.4/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.3.4/configzen/py.typed
+-rw-r--r--   0        0        0     4599 2023-06-15 09:11:04.738125 configzen-0.3.4/configzen/route.py
+-rw-r--r--   0        0        0     1124 2023-06-15 09:10:42.331286 configzen-0.3.4/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.3.4/LICENSE
+-rw-r--r--   0        0        0     1255 2023-06-15 09:13:54.886814 configzen-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     7371 2023-06-13 02:20:30.758785 configzen-0.3.4/README.md
+-rw-r--r--   0        0        0     8001 1970-01-01 00:00:00.000000 configzen-0.3.4/PKG-INFO
```

### Comparing `configzen-0.3.3/configzen/__init__.py` & `configzen-0.3.4/configzen/__init__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.3/configzen/__main__.py` & `configzen-0.3.4/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.3/configzen/config.py` & `configzen-0.3.4/configzen/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1673,20 +1673,15 @@
 
 
 class ConfigModel(
     pydantic.BaseSettings,
     metaclass=ConfigModelMetaclass,
     root=True,
 ):
-    """
-    The base class for configuration models.
-
-    It is not recommended to inherit from this class directly for basic usage.
-    Instead, use either :class:`ConfigModel` or :class:`AsyncConfigModel`.
-    """
+    """The base class for configuration models."""
 
     def __init__(self, **kwargs: Any) -> None:
         # Set private attributes via the constructor
         # to allow preprocessor-related instances to exist.
         missing = object()
         for private_attr in self.__private_attributes__:
             value = kwargs.pop(private_attr, missing)
```

### Comparing `configzen-0.3.3/configzen/decorators.py` & `configzen-0.3.4/configzen/decorators.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.3/configzen/errors.py` & `configzen-0.3.4/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.3/configzen/field.py` & `configzen-0.3.4/configzen/field.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.3/configzen/processor.py` & `configzen-0.3.4/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.3/configzen/route.py` & `configzen-0.3.4/configzen/route.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.3/configzen/typedefs.py` & `configzen-0.3.4/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.3/LICENSE` & `configzen-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.3.3/pyproject.toml` & `configzen-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.3.3"
+version = "0.3.4"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.3.3/README.md` & `configzen-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.3.3/PKG-INFO` & `configzen-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.3.3
+Version: 0.3.4
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

