# Comparing `tmp/chainmapping-0.1.2.tar.gz` & `tmp/chainmapping-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainmapping-0.1.2.tar", max compression
+gzip compressed data, was "chainmapping-0.1.3.tar", max compression
```

## Comparing `chainmapping-0.1.2.tar` & `chainmapping-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-06-15 11:06:34.673850 chainmapping-0.1.2/LICENSE
--rw-r--r--   0        0        0       80 2023-06-15 11:06:34.673850 chainmapping-0.1.2/README.md
--rw-r--r--   0        0        0     2183 2023-06-15 11:06:34.673850 chainmapping-0.1.2/chainmapping/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 11:06:34.673850 chainmapping-0.1.2/chainmapping/py.typed
--rw-r--r--   0        0        0      589 2023-06-15 11:06:34.673850 chainmapping-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 chainmapping-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-15 11:28:31.868889 chainmapping-0.1.3/LICENSE
+-rw-r--r--   0        0        0       80 2023-06-15 11:28:31.868889 chainmapping-0.1.3/README.md
+-rw-r--r--   0        0        0     2207 2023-06-15 11:28:31.868889 chainmapping-0.1.3/chainmapping/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 11:28:31.868889 chainmapping-0.1.3/chainmapping/py.typed
+-rw-r--r--   0        0        0      619 2023-06-15 11:28:31.868889 chainmapping-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 chainmapping-0.1.3/PKG-INFO
```

### Comparing `chainmapping-0.1.2/LICENSE` & `chainmapping-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chainmapping-0.1.2/chainmapping/__init__.py` & `chainmapping-0.1.3/chainmapping/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-from typing import (
-    Mapping,
-    TypeVar,
-    overload,
-)
+from typing import Mapping, TypeVar, overload
 
 _Key_T = TypeVar("_Key_T")
 _Value_U = TypeVar("_Value_U")
 _Default_V = TypeVar("_Default_V")
 
 
 class ChainMapping(Mapping[_Key_T, _Value_U]):
@@ -14,15 +10,15 @@
     to create a single, readonly view.
 
     The underlying mappings are stored in a list.  That list is public and can
     be accessed or updated using the *maps* attribute.  There is no other
     state.
 
     Lookups search the underlying mappings successively until a key is found.
-   
+
 
     """
 
     def __init__(self, *maps: Mapping[_Key_T, _Value_U]):
         """Initialize a ChainMap by setting *maps* to the given mappings.
         If no mappings are provided, a single empty dictionary is used.
 
@@ -37,22 +33,28 @@
             try:
                 return mapping[key]  # can't use 'key in mapping' with defaultdict
             except KeyError:
                 pass
         return self.__missing__(key)  # support subclasses that define __missing__
 
     @overload
-    def get(self, key: _Key_T, default: None = ...) -> _Value_U | None: # pragma: no cover
+    def get(
+        self, key: _Key_T, default: None = ...
+    ) -> _Value_U | None:  # pragma: no cover
         ...
 
     @overload
-    def get(self, key: _Key_T, default: _Default_V) -> _Value_U | _Default_V: # pragma: no cover
+    def get(
+        self, key: _Key_T, default: _Default_V
+    ) -> _Value_U | _Default_V:  # pragma: no cover
         ...
 
-    def get(self, key: _Key_T, default: _Default_V | None = None) -> _Default_V | _Value_U | None:
+    def get(
+        self, key: _Key_T, default: _Default_V | None = None
+    ) -> _Default_V | _Value_U | None:
         return self[key] if key in self else default
 
     def new_child(self, map: Mapping[_Key_T, _Value_U]):
         return ChainMapping(map, *self.maps)
 
     def __len__(self):
         s: set[_Key_T] = set()
```

### Comparing `chainmapping-0.1.2/pyproject.toml` & `chainmapping-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainmapping"
-version = "0.1.2"
+version = "0.1.3"
 description = "Simple class to create readonly ChainMaps that support typing.Mapping"
 authors = ["Kalle M. Aagaard <km@conscia.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
@@ -12,15 +12,16 @@
 black = "^23.3.0"
 isort = "^5.12.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.1.0"
 
-
-
 [tool.pytest.ini_options]
 addopts = "-v --cov=chainmapping --cov-report=xml --cov-report=term"
 
+[tool.isort]
+profile = "black"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `chainmapping-0.1.2/PKG-INFO` & `chainmapping-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainmapping
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple class to create readonly ChainMaps that support typing.Mapping
 Author: Kalle M. Aagaard
 Author-email: km@conscia.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

