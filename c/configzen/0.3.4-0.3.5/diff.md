# Comparing `tmp/configzen-0.3.4.tar.gz` & `tmp/configzen-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.3.4.tar", max compression
+gzip compressed data, was "configzen-0.3.5.tar", max compression
```

## Comparing `configzen-0.3.4.tar` & `configzen-0.3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      979 2023-06-15 09:10:26.257090 configzen-0.3.4/configzen/__init__.py
--rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.3.4/configzen/__main__.py
--rw-r--r--   0        0        0    67481 2023-06-15 09:13:30.986779 configzen-0.3.4/configzen/config.py
--rw-r--r--   0        0        0     3232 2023-06-15 09:05:45.207916 configzen-0.3.4/configzen/decorators.py
--rw-r--r--   0        0        0     3607 2023-06-15 00:25:22.104007 configzen-0.3.4/configzen/errors.py
--rw-r--r--   0        0        0      544 2023-06-15 09:10:51.539939 configzen-0.3.4/configzen/field.py
--rw-r--r--   0        0        0    25977 2023-06-15 09:05:45.230906 configzen-0.3.4/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.3.4/configzen/py.typed
--rw-r--r--   0        0        0     4599 2023-06-15 09:11:04.738125 configzen-0.3.4/configzen/route.py
--rw-r--r--   0        0        0     1124 2023-06-15 09:10:42.331286 configzen-0.3.4/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.3.4/LICENSE
--rw-r--r--   0        0        0     1255 2023-06-15 09:13:54.886814 configzen-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     7371 2023-06-13 02:20:30.758785 configzen-0.3.4/README.md
--rw-r--r--   0        0        0     8001 1970-01-01 00:00:00.000000 configzen-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      979 2023-06-15 09:10:26.257090 configzen-0.3.5/configzen/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.3.5/configzen/__main__.py
+-rw-r--r--   0        0        0    67715 2023-06-15 09:41:13.289857 configzen-0.3.5/configzen/config.py
+-rw-r--r--   0        0        0     3232 2023-06-15 09:05:45.207916 configzen-0.3.5/configzen/decorators.py
+-rw-r--r--   0        0        0     3607 2023-06-15 00:25:22.104007 configzen-0.3.5/configzen/errors.py
+-rw-r--r--   0        0        0      544 2023-06-15 09:10:51.539939 configzen-0.3.5/configzen/field.py
+-rw-r--r--   0        0        0    25977 2023-06-15 09:05:45.230906 configzen-0.3.5/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.3.5/configzen/py.typed
+-rw-r--r--   0        0        0     4599 2023-06-15 09:11:04.738125 configzen-0.3.5/configzen/route.py
+-rw-r--r--   0        0        0     1124 2023-06-15 09:10:42.331286 configzen-0.3.5/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1255 2023-06-15 09:41:45.898880 configzen-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     7371 2023-06-13 02:20:30.758785 configzen-0.3.5/README.md
+-rw-r--r--   0        0        0     8001 1970-01-01 00:00:00.000000 configzen-0.3.5/PKG-INFO
```

### Comparing `configzen-0.3.4/configzen/__init__.py` & `configzen-0.3.5/configzen/__init__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.4/configzen/__main__.py` & `configzen-0.3.5/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.4/configzen/config.py` & `configzen-0.3.5/configzen/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1768,30 +1768,34 @@
 
     def _iter(  # type: ignore[override]
         self, **kwargs: Any
     ) -> collections.abc.Iterator[tuple[str, Any]]:
         if kwargs.get("to_dict", False) and _exporting.get():
             state = {}
             for key, value in super()._iter(**kwargs):
-                state[key] = value
+                field = self.__fields__.get(key)
+                actual_key = field.alias if field else key
+                state[actual_key] = value
             metadata = getattr(self, EXPORT, None)
             if metadata:
                 context = get_context(self)
                 context.agent.processor_class.export(state, metadata=metadata)
             yield from state.items()
         else:
             yield from super()._iter(**kwargs)
 
     async def _iter_async(
         self, **kwargs: Any
     ) -> collections.abc.Iterator[tuple[str, Any]]:
         if kwargs.get("to_dict", False) and _exporting.get():
             state = {}
             for key, value in super()._iter(**kwargs):
-                state[key] = value
+                field = self.__fields__.get(key)
+                actual_key = field.alias if field else key
+                state[actual_key] = value
             metadata = getattr(self, EXPORT, None)
             if metadata:
                 context = get_context(self)
                 await context.agent.processor_class.export_async(
                     state, metadata=metadata
                 )
             return ((key, value) for key, value in state.items())
```

### Comparing `configzen-0.3.4/configzen/decorators.py` & `configzen-0.3.5/configzen/decorators.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.4/configzen/errors.py` & `configzen-0.3.5/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.4/configzen/field.py` & `configzen-0.3.5/configzen/field.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.4/configzen/processor.py` & `configzen-0.3.5/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.4/configzen/route.py` & `configzen-0.3.5/configzen/route.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.4/configzen/typedefs.py` & `configzen-0.3.5/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.3.4/LICENSE` & `configzen-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.3.4/pyproject.toml` & `configzen-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.3.4"
+version = "0.3.5"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.3.4/README.md` & `configzen-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.3.4/PKG-INFO` & `configzen-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.3.4
+Version: 0.3.5
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

