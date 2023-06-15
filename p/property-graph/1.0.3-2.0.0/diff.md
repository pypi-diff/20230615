# Comparing `tmp/property-graph-1.0.3.tar.gz` & `tmp/property-graph-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "property-graph-1.0.3.tar", last modified: Wed May 10 19:29:48 2023, max compression
+gzip compressed data, was "property-graph-2.0.0.tar", last modified: Thu Jun 15 16:54:52 2023, max compression
```

## Comparing `property-graph-1.0.3.tar` & `property-graph-2.0.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:29:48.617139 property-graph-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-10 19:29:39.000000 property-graph-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-05-10 19:29:48.617139 property-graph-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-05-10 19:29:39.000000 property-graph-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-10 19:29:39.000000 property-graph-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 19:29:48.617139 property-graph-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:29:48.613139 property-graph-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:29:48.613139 property-graph-1.0.3/src/property_graph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-05-10 19:29:48.000000 property-graph-1.0.3/src/property_graph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-10 19:29:48.000000 property-graph-1.0.3/src/property_graph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 19:29:48.000000 property-graph-1.0.3/src/property_graph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 19:29:48.000000 property-graph-1.0.3/src/property_graph.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:29:48.613139 property-graph-1.0.3/src/pypg/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/locator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16685 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/property_transcoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:29:48.613139 property-graph-1.0.3/src/pypg/traits/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/traits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/traits/allowed_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/traits/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/traits/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/traits/obligate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/traits/observable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/traits/overridable.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/traits/read_only.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/traits/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/traits/validated.py
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/transcode.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/type_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/type_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:29:48.617139 property-graph-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_allowed_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_locator.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_obligate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_observable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_overridable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_readonly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_transcoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_type_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_type_schema_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:54:52.253048 property-graph-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 16:54:42.000000 property-graph-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-06-15 16:54:52.253048 property-graph-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-15 16:54:42.000000 property-graph-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-15 16:54:42.000000 property-graph-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:54:52.253048 property-graph-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:54:52.249048 property-graph-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:54:52.253048 property-graph-2.0.0/src/property_graph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-06-15 16:54:52.000000 property-graph-2.0.0/src/property_graph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-15 16:54:52.000000 property-graph-2.0.0/src/property_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:54:52.000000 property-graph-2.0.0/src/property_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 16:54:52.000000 property-graph-2.0.0/src/property_graph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:54:52.253048 property-graph-2.0.0/src/pypg/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-15 16:54:42.000000 property-graph-2.0.0/src/pypg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-15 16:54:42.000000 property-graph-2.0.0/src/pypg/locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17061 2023-06-15 16:54:42.000000 property-graph-2.0.0/src/pypg/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-15 16:54:42.000000 property-graph-2.0.0/src/pypg/property_transcoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:54:52.253048 property-graph-2.0.0/src/pypg/traits/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-15 16:54:42.000000 property-graph-2.0.0/src/pypg/traits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-15 16:54:42.000000 property-graph-2.0.0/src/pypg/traits/allowed_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-15 16:54:42.000000 property-graph-2.0.0/src/pypg/traits/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-15 16:54:42.000000 property-graph-2.0.0/src/pypg/traits/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-15 16:54:42.000000 property-graph-2.0.0/src/pypg/traits/obligate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-15 16:54:42.000000 property-graph-2.0.0/src/pypg/traits/observable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-15 16:54:42.000000 property-graph-2.0.0/src/pypg/traits/overridable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-15 16:54:42.000000 property-graph-2.0.0/src/pypg/traits/read_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-15 16:54:42.000000 property-graph-2.0.0/src/pypg/traits/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-15 16:54:42.000000 property-graph-2.0.0/src/pypg/traits/validated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-06-15 16:54:42.000000 property-graph-2.0.0/src/pypg/transcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-15 16:54:42.000000 property-graph-2.0.0/src/pypg/type_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-15 16:54:42.000000 property-graph-2.0.0/src/pypg/type_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:54:52.253048 property-graph-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-15 16:54:42.000000 property-graph-2.0.0/tests/test_allowed_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-15 16:54:42.000000 property-graph-2.0.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-15 16:54:42.000000 property-graph-2.0.0/tests/test_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-15 16:54:42.000000 property-graph-2.0.0/tests/test_obligate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-15 16:54:42.000000 property-graph-2.0.0/tests/test_observable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-15 16:54:42.000000 property-graph-2.0.0/tests/test_overridable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-15 16:54:42.000000 property-graph-2.0.0/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-15 16:54:42.000000 property-graph-2.0.0/tests/test_readonly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-15 16:54:42.000000 property-graph-2.0.0/tests/test_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-15 16:54:42.000000 property-graph-2.0.0/tests/test_transcoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-15 16:54:42.000000 property-graph-2.0.0/tests/test_type_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-15 16:54:42.000000 property-graph-2.0.0/tests/test_type_schema_encoding.py
```

### Comparing `property-graph-1.0.3/LICENSE` & `property-graph-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.3/PKG-INFO` & `property-graph-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: property-graph
-Version: 1.0.3
+Version: 2.0.0
 Summary: python library for working with objects as graphs of property data
 Author-email: Matt Fowler <mattefowler@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `property-graph-1.0.3/README.md` & `property-graph-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.3/pyproject.toml` & `property-graph-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.3/src/property_graph.egg-info/PKG-INFO` & `property-graph-2.0.0/src/property_graph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: property-graph
-Version: 1.0.3
+Version: 2.0.0
 Summary: python library for working with objects as graphs of property data
 Author-email: Matt Fowler <mattefowler@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `property-graph-1.0.3/src/property_graph.egg-info/SOURCES.txt` & `property-graph-2.0.0/src/property_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.3/src/pypg/locator.py` & `property-graph-2.0.0/src/pypg/locator.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.3/src/pypg/property.py` & `property-graph-2.0.0/src/pypg/property.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     "PropertyClass",
     "Trait",
 ]
 
 import itertools
 from abc import ABC, abstractmethod
 from functools import cached_property, wraps
+from types import FunctionType
 from typing import Any, Callable, Generic, Iterable, Protocol, TypeVar
 
 from pypg.type_utils import get_fully_qualified_name
 
 T = TypeVar("T")
 
 
@@ -267,14 +268,18 @@
     def __subclasscheck__(cls, subclass):
         return issubclass(_Proxy, subclass) or super().__subclasscheck__(subclass)
 
 
 TraitProvider = Trait | classmethod
 
 
+def is_method(cls: type, obj: Any) -> bool:
+    return isinstance(obj, (FunctionType, classmethod, staticmethod)) and obj in cls.__dict__.values()
+
+
 class Property(Generic[T], metaclass=_PropertyMeta):
     """
     Property is a descriptor class used for instance-data storage as well as
     declaring metadata and behaviors triggered by data-access.
     """
 
     def __init__(
@@ -320,14 +325,18 @@
     @cached_property
     def value_type(self):
         return self.__orig_class__.__args__[0]
 
     def __bind__(self, name, cls: PropertyType):
         self.name = name
         self.__declaring_type = cls
+        self._default, self._getter, self._setter = (
+            MethodReference(obj) if is_method(cls, obj) else obj
+            for obj in (self._default, self._getter, self._setter)
+        )
 
     def __bind_subclass__(self, cls):
         proxy = _Proxy(self, cls)
         for t in proxy.traits:
             t.__bind__(self)
         self._subclass_proxies[cls] = proxy
```

### Comparing `property-graph-1.0.3/src/pypg/traits/allowed_range.py` & `property-graph-2.0.0/src/pypg/traits/allowed_range.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.3/src/pypg/traits/config.py` & `property-graph-2.0.0/src/pypg/traits/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pypg.property import PropertyClass, Property, PropertyType
 from pypg.property_transcoder import PropertyClassEncoder
 
 
 class ConfigEncoder(PropertyClassEncoder):
     def _encode(self, obj: PropertyClass):
         return {
-            p.name: Encoder(p.get(obj), self, self.overrides).obj_id
+            p.name: Encoder(p.get(obj), self, self.overrides).obj_data
             for p in filter(Config.has_config_data, type(obj).properties)
         }
 
 
 class Config(MetadataTrait):
     def __init__(self, include=True):
         super().__init__(include)
```

### Comparing `property-graph-1.0.3/src/pypg/traits/obligate.py` & `property-graph-2.0.0/src/pypg/traits/obligate.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.3/src/pypg/traits/observable.py` & `property-graph-2.0.0/src/pypg/traits/observable.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.3/src/pypg/traits/overridable.py` & `property-graph-2.0.0/src/pypg/traits/overridable.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.3/src/pypg/traits/read_only.py` & `property-graph-2.0.0/src/pypg/traits/read_only.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.3/src/pypg/traits/validated.py` & `property-graph-2.0.0/src/pypg/traits/validated.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.3/src/pypg/transcode.py` & `property-graph-2.0.0/src/pypg/transcode.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     "encode",
     "Encoder",
     "CollectionEncoder",
     "DictEncoder",
 ]
 
 import json
+from abc import abstractmethod
 from collections.abc import Collection, Iterable
 from types import NoneType
 from typing import Any, Union, Self
 
 from pypg.locator import Locator
 from pypg.type_registry import TypeRegistry
 from pypg.type_utils import get_fully_qualified_name
@@ -25,15 +26,17 @@
 
 
 class _Transcoder:
     root_key = "root"
 
     _registry: TypeRegistry[_Transcoder] = None
 
-    def __init_subclass__(cls, handler_for: type | Iterable[type] = (), **kwargs):
+    def __init_subclass__(
+        cls, handler_for: type | Iterable[type] = (), **kwargs
+    ):
         if isinstance(handler_for, type):
             handler_for = (handler_for,)
         if cls._registry is None:
             cls._registry = TypeRegistry()
         cls._registry.update({t: cls for t in handler_for})
 
     @classmethod
@@ -46,44 +49,44 @@
             try:
                 return TypeRegistry(overrides)[obj_type:]
             except KeyError:
                 pass
         return cls[obj_type]
 
 
-class Encoder(_Transcoder, handler_for=primitives):
+class Encoder(_Transcoder):
     """
     Encoders transform python objects into JSON-compliant data-structures for
     storage or transmission. All constituent object data is stored in a flat
     dict keyed by each object's id. The values of the data-dict are lists of
     two elements: the first node contains the fully-qualified type name of the
     object's type, and the second contains a serializable representation of its
     members. The one exception to this pattern is the 'root' node, which
     contains only the address of the object initially passed to the Encoder.
     Subclasses of Encoder transform data for specific types specified by the
     handler_for class-keyword.
     """
 
     def __new__(
-        cls, obj, parent: Encoder | None, overrides: dict[type, type[Encoder]] = None
+        cls,
+        obj,
+        parent: Encoder | None,
+        overrides: dict[type, type[Encoder]] = None,
     ):
         """
         Create a new encoder for the object. If a more-specific encoder-type
         for the object's type exists than the one specific, construct it
         instead.
         Args:
             obj: the object to be encoded.
             parent: the Encoder constructing this one, or None if obj is the
             first object to be encoded.
         """
         encoder_type = cls._resolve_handler(type(obj), overrides)
-        if encoder_type is cls:
-            return super().__new__(cls)
-        else:
-            return encoder_type(obj, parent, overrides)
+        return super().__new__(encoder_type)
 
     def __init__(
         self, obj, parent: Encoder | None, overrides: dict[type, type[Encoder]]
     ):
         """
         Initialize a new encoder for the object.
         Args:
@@ -93,15 +96,16 @@
         """
         self.parent = parent
         self.overrides = overrides
         if parent is None:
             self.data: dict[str, str | list[str, Any]] = {}
         else:
             self.data = parent.data
-        self._obj_id = self._pack(obj)
+        self._obj_id = id(obj)
+        self.obj_data = self._pack(obj)
         if parent is None:
             self.data[self.root_key] = self.obj_id
 
     @property
     def obj_id(self) -> str:
         """
         The unique identifier for the object being encoded; this should be a
@@ -111,146 +115,154 @@
         """
         return self._obj_id
 
     @classmethod
     def _get_obj_type(cls, obj):
         return type(obj)
 
-    def _pack(self, obj) -> str:
-        obj_id = str(id(obj))
+    def _pack(self, obj) -> list[str, int, Any]:
         obj_type = self._get_obj_type(obj)
-        if obj_id not in self.data:
-            encoded_data = [f"{get_fully_qualified_name(obj_type)}"]
-            # pack data in 2 stages to prevent infinite recursion when encoding self-referential objects.
-            self.data[obj_id] = encoded_data
-            encoded_data.append(self._encode(obj))
-        return obj_id
+        if self.obj_id in self.data:
+            return Encoder(
+                _ObjectReference(obj), self, self.overrides
+            ).obj_data
+        encoded_data = [
+            get_fully_qualified_name(obj_type),
+            (self._encode(obj), self.obj_id),
+        ]
+        self.data[self.obj_id] = encoded_data
+        return encoded_data
 
     def _encode(self, obj):
         return obj
 
-    @classmethod
-    def unpack(cls, data, obj_id=_Transcoder.root_key, locator=default_locator):
-        """Transform encoded data into a more readable format, expanding
-        objects into container elements instead of referencing by id, and
-        duplicating any shared references."""
-        if obj_id == _Transcoder.root_key:
-            obj_id = data[obj_id]
-        obj_type_fqn, obj_data = data[obj_id]
-        obj_type = locator(obj_type_fqn)
-        e_type = cls[obj_type]
-        return [obj_type_fqn, e_type._unpack(data, obj_data, locator)]
 
-    @classmethod
-    def _unpack(cls, data, obj_data, locator=default_locator):
-        return obj_data
+class PrimitiveEncoder(Encoder, handler_for=primitives):
+    def _pack(self, obj) -> list[str, int, Any]:
+        obj_type = self._get_obj_type(obj)
+        return [
+            get_fully_qualified_name(obj_type),
+            self._encode(obj),
+        ]
 
 
 class Decoder(_Transcoder, handler_for=primitives):
     """
     Decoders transform encoded data into instances equivalent to the originally
     encoded object.
     """
 
     def __new__(
         cls,
         encoded_data: dict,
-        obj_id: str | None,
         locator: Locator,
         parent: Decoder | None,
         overrides: dict[type, type[Decoder]] = None,
     ):
         """
         Create a new Decoder. The most appropriate Decoder for the object
         corresponding to obj_id will be resolve and constructed for non-
         primitive data.
         Args:
             encoded_data:
             obj_id:
             locator:
             parent:
         """
-        if obj_id is None:
-            obj_id = encoded_data[cls.root_key]
-        attr_type, attr_data = cls._unpack(encoded_data, obj_id, locator)
+        # if obj_id is None:
+        #     obj_id = encoded_data[cls.root_key]
+        attr_type, *_ = cls._unpack(encoded_data, locator)
         decoder_cls = cls._resolve_handler(attr_type, overrides)
-        return (
-            super().__new__(cls)
-            if decoder_cls is cls
-            else decoder_cls(encoded_data, obj_id, locator, parent, overrides=overrides)
-        )
+        return super().__new__(decoder_cls)
 
     def __init__(
         self,
         encoded_data: dict,
-        obj_id: str | None,
         locator: Locator,
         parent: Decoder | None,
         overrides: dict[type, type[Decoder]],
     ):
         self.parent = parent
         self.overrides = overrides
         if parent is None:
             self.decoded_objects = {}
         else:
             self.decoded_objects = parent.decoded_objects
         self.encoded_data = encoded_data
-        self.obj_id = obj_id if obj_id is not None else encoded_data[self.root_key]
         self.locator = locator
         self.instance = self.decode()
 
     def decode(self) -> Any:
+        member_type, (member_data, obj_id) = self._unpack(
+            self.encoded_data, self.locator
+        )
         try:
-            return self.decoded_objects[self.obj_id]
+            return self.decoded_objects[obj_id]
         except KeyError:
             pass
-
-        member_type, member_data = self._unpack(
-            self.encoded_data, self.obj_id, self.locator
-        )
         instance = self._decode(member_type, member_data)
-        self.decoded_objects[self.obj_id] = instance
+        self.decoded_objects[obj_id] = instance
         return instance
 
     @classmethod
     def _unpack(
         cls,
         encoded_data: dict[str, list[str, Any]],
-        obj_id: str,
         locator: Locator,
     ) -> tuple[type, Any]:
-        fully_qualified_name, value = encoded_data[obj_id]
+        fully_qualified_name, obj_data = encoded_data
         try:
             t = locator(fully_qualified_name)
         except TypeError:
             if fully_qualified_name != NoneType.__name__:
                 raise
             t = NoneType
-        return t, value
+        return t, obj_data
 
     def _decode(self, obj_type: type, value: Any) -> Any:
         return obj_type(value)
 
 
-class NoneTypeDecoder(Decoder, handler_for=NoneType):
+class PrimitiveDecoder(Decoder, handler_for=primitives):
+    def decode(self) -> Any:
+        member_type, value = self._unpack(self.encoded_data, self.locator)
+        return self._decode(member_type, value)
+
+
+class _ObjectReference:
+    def __init__(self, obj: Any):
+        self.obj = obj
+
+
+class _ObjectReferenceEncoder(Encoder, handler_for=_ObjectReference):
+    def _encode(self, obj_ref):
+        return id(obj_ref.obj)
+
+
+class _ObjectReferenceDecoder(Decoder, handler_for=_ObjectReference):
+    def _decode(self, obj_type: type, value: Any) -> Any:
+        return self.decoded_objects[value]
+
+
+class NoneTypeDecoder(PrimitiveDecoder, handler_for=NoneType):
     def _decode(self, obj_type: type, value: Any) -> Any:
         return None
 
 
 def encode(obj, overrides: dict[type, type[Encoder]] = None) -> Any:
     """
     A convenience function to simplify the syntax of using an Encoder to
     transform an object's data into a JSON-serializable format.
     Args:
         obj: the object to be serialized.
 
     Returns:
         transformed-data of obj
     """
-    return Encoder(obj, None, overrides).data
+    return Encoder(obj, None, overrides).obj_data
 
 
 def to_string(obj, overrides: dict[type, type[Encoder]] | None = None) -> str:
     """
     A convenience function to simplify using an Encoder to transform an
     object's data into a JSON-parseable string.
     Args:
@@ -272,18 +284,22 @@
     of encoded object data into object instances.
     Args:
         obj: the object to be stringified.
 
     Returns:
         a JSON-parseable string of the object's data.
     """
-    return decode(json.loads(encoded_object), locator=locator, overrides=overrides)
+    return decode(
+        json.loads(encoded_object), locator=locator, overrides=overrides
+    )
 
 
-def to_file(obj, path: str, overrides: dict[type, type[Encoder]]|None=None):
+def to_file(
+    obj, path: str, overrides: dict[type, type[Encoder]] | None = None
+):
     with open(path, "w") as f:
         json.dump(encode(obj, overrides=overrides), f)
 
 
 def from_file(
     path: str,
     locator=default_locator,
@@ -295,87 +311,70 @@
 
 def decode(
     obj_data,
     locator=default_locator,
     overrides: dict[type, type[Decoder]] | None = None,
 ):
     return Decoder(
-        obj_data, locator=locator, parent=None, obj_id=None, overrides=overrides
+        obj_data, locator=locator, parent=None, overrides=overrides
     ).instance
 
 
-def unpack(obj_data, obj_id=Encoder.root_key, locator=default_locator):
-    return Encoder.unpack(obj_data, obj_id, locator)
-
-
-class TypeEncoder(Encoder, handler_for=type):
+class TypeEncoder(PrimitiveEncoder, handler_for=type):
     def _encode(self, obj_type):
         return get_fully_qualified_name(obj_type)
 
 
-class TypeDecoder(Decoder, handler_for=type):
+class TypeDecoder(PrimitiveDecoder, handler_for=type):
     def _decode(self, _, fully_qualified_name: str):
         return self.locator(fully_qualified_name)
 
 
 class CollectionEncoder(Encoder, handler_for=(tuple, set, list)):
     def _encode(self, obj: Collection):
-        return [Encoder(item, self, self.overrides).obj_id for item in obj]
-
-    @classmethod
-    def _unpack(cls, data, obj_data: list[str], locator=default_locator):
-        return [Encoder.unpack(data, item, locator) for item in obj_data]
+        return [Encoder(item, self, self.overrides).obj_data for item in obj]
 
 
 class CollectionDecoder(Decoder, handler_for=(tuple, set, list)):
-    def _decode(self, obj_type, obj_ids: Collection[str]):
+    def _decode(self, obj_type, obj_data: Collection[Any]):
         return obj_type(
             (
                 Decoder(
-                    self.encoded_data,
-                    obj_id,
+                    encoded_obj_data,
                     self.locator,
                     self,
                     overrides=self.overrides,
                 ).instance
-                for obj_id in obj_ids
+                for encoded_obj_data in obj_data
             )
         )
 
 
 class DictEncoder(Encoder, handler_for=dict):
     def _encode(self, obj: dict):
-        return {
-            Encoder(key, self, self.overrides)
-            .obj_id: Encoder(value, self, self.overrides)
-            .obj_id
-            for key, value in obj.items()
-        }
-
-    @classmethod
-    def _unpack(
-        cls,
-        data: dict[str, Any],
-        obj_data: dict[str, str],
-        locator=default_locator,
-    ):
         return [
-            (
-                Encoder.unpack(data, key, locator=locator),
-                Encoder.unpack(data, value, locator=locator),
+            *zip(
+                *(
+                    (
+                        Encoder(obj, self, self.overrides).obj_data
+                        for obj in item
+                    )
+                    for item in obj.items()
+                )
             )
-            for key, value in obj_data.items()
         ]
 
 
 class DictDecoder(Decoder, handler_for=dict):
-    def _decode(self, obj_type: type, value: dict) -> Any:
-        return {
-            Decoder(
-                self.encoded_data, key, self.locator, self, overrides=self.overrides
-            )
-            .instance: Decoder(
-                self.encoded_data, value, self.locator, self, overrides=self.overrides
-            )
-            .instance
-            for key, value in value.items()
-        }
+    def _decode(self, obj_type: type, items: list[list, list]) -> Any:
+        return (
+            {
+                Decoder(key, self.locator, self, overrides=self.overrides)
+                .instance: Decoder(
+                    item, self.locator, self, overrides=self.overrides
+                )
+                .instance
+                for key, item in zip(*items)
+            }
+            if items
+            else {}
+        )
```

### Comparing `property-graph-1.0.3/src/pypg/type_registry.py` & `property-graph-2.0.0/src/pypg/type_registry.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.3/src/pypg/type_utils.py` & `property-graph-2.0.0/src/pypg/type_utils.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.3/tests/test_allowed_range.py` & `property-graph-2.0.0/tests/test_allowed_range.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.3/tests/test_config.py` & `property-graph-2.0.0/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     p1 = Property[int](default=0, traits=[Config(True)])
 
 
 class CfgDataCls(PropertyClass):
     def _make_inner(self):
         return InnerCls()
 
-    inner = Property[InnerCls](default=MethodReference(_make_inner))
+    inner = Property[InnerCls](default=_make_inner)
     excluded = Property[int](default=0, traits=[Config(False)])
     included = Property[int](default=0, traits=[Config(True)])
     excluded_inner = Property[InnerCls](traits=[Config(False)])
 
 
 class ConfigTest(TestCase):
     def test_config(self):
```

### Comparing `property-graph-1.0.3/tests/test_locator.py` & `property-graph-2.0.0/tests/test_locator.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.3/tests/test_obligate.py` & `property-graph-2.0.0/tests/test_obligate.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.3/tests/test_observable.py` & `property-graph-2.0.0/tests/test_observable.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.3/tests/test_overridable.py` & `property-graph-2.0.0/tests/test_overridable.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.3/tests/test_property.py` & `property-graph-2.0.0/tests/test_property.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     a = Property[float](default=MethodReference(default_poly, offset=1))
     a2 = Property[float](default=MethodReference(default_poly, offset=2))
 
     @classmethod
     def default_gain(cls):
         return 1
 
-    b = Property[float](default=MethodReference(default_gain))
+    b = Property[float](default=default_gain)
 
     @classmethod
     def _optional_c_traits(cls):
         pass
 
     c = Property[int](default=1, traits=_optional_c_traits)
 
@@ -32,15 +32,15 @@
         return self.a + self.b + self.c
 
     @classmethod
     def _d_traits(cls):
         return Unit("mm"), Observable[PostSet]()
 
     d = Property[float](
-        default=1, getter=MethodReference(default_sum), traits=_d_traits
+        default=1, getter=default_sum, traits=_d_traits
     )
 
 
 class PropertyTest(TestCase):
     def test_method_reference(self):
         mr = MethodReference(Example.default_poly)
         ex = Example()
```

### Comparing `property-graph-1.0.3/tests/test_readonly.py` & `property-graph-2.0.0/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.3/tests/test_traits.py` & `property-graph-2.0.0/tests/test_traits.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.3/tests/test_type_registry.py` & `property-graph-2.0.0/tests/test_type_registry.py`

 * *Files identical despite different names*

