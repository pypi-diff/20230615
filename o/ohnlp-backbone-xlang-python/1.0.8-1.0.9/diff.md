# Comparing `tmp/ohnlp-backbone-xlang-python-1.0.8.tar.gz` & `tmp/ohnlp-backbone-xlang-python-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohnlp-backbone-xlang-python-1.0.8.tar", last modified: Wed Jun  7 21:29:26 2023, max compression
+gzip compressed data, was "ohnlp-backbone-xlang-python-1.0.9.tar", last modified: Mon Jun 12 19:40:08 2023, max compression
```

## Comparing `ohnlp-backbone-xlang-python-1.0.8.tar` & `ohnlp-backbone-xlang-python-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:26.987375 ohnlp-backbone-xlang-python-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 21:29:24.000000 ohnlp-backbone-xlang-python-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-07 21:29:26.987375 ohnlp-backbone-xlang-python-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-07 21:29:24.000000 ohnlp-backbone-xlang-python-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:26.987375 ohnlp-backbone-xlang-python-1.0.8/ohnlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:24.000000 ohnlp-backbone-xlang-python-1.0.8/ohnlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:26.987375 ohnlp-backbone-xlang-python-1.0.8/ohnlp/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:24.000000 ohnlp-backbone-xlang-python-1.0.8/ohnlp/toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:26.987375 ohnlp-backbone-xlang-python-1.0.8/ohnlp/toolkit/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:24.000000 ohnlp-backbone-xlang-python-1.0.8/ohnlp/toolkit/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-06-07 21:29:24.000000 ohnlp-backbone-xlang-python-1.0.8/ohnlp/toolkit/backbone/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-07 21:29:24.000000 ohnlp-backbone-xlang-python-1.0.8/ohnlp/toolkit/backbone/backbone_module_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:26.987375 ohnlp-backbone-xlang-python-1.0.8/ohnlp_backbone_xlang_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-07 21:29:26.000000 ohnlp-backbone-xlang-python-1.0.8/ohnlp_backbone_xlang_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-07 21:29:26.000000 ohnlp-backbone-xlang-python-1.0.8/ohnlp_backbone_xlang_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:29:26.000000 ohnlp-backbone-xlang-python-1.0.8/ohnlp_backbone_xlang_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-07 21:29:26.000000 ohnlp-backbone-xlang-python-1.0.8/ohnlp_backbone_xlang_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 21:29:26.000000 ohnlp-backbone-xlang-python-1.0.8/ohnlp_backbone_xlang_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 21:29:26.987375 ohnlp-backbone-xlang-python-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-07 21:29:24.000000 ohnlp-backbone-xlang-python-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:40:08.060664 ohnlp-backbone-xlang-python-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 19:40:01.000000 ohnlp-backbone-xlang-python-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-12 19:40:08.060664 ohnlp-backbone-xlang-python-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-12 19:40:01.000000 ohnlp-backbone-xlang-python-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:40:08.060664 ohnlp-backbone-xlang-python-1.0.9/ohnlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:40:01.000000 ohnlp-backbone-xlang-python-1.0.9/ohnlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:40:08.060664 ohnlp-backbone-xlang-python-1.0.9/ohnlp/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:40:01.000000 ohnlp-backbone-xlang-python-1.0.9/ohnlp/toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:40:08.060664 ohnlp-backbone-xlang-python-1.0.9/ohnlp/toolkit/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:40:01.000000 ohnlp-backbone-xlang-python-1.0.9/ohnlp/toolkit/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-06-12 19:40:01.000000 ohnlp-backbone-xlang-python-1.0.9/ohnlp/toolkit/backbone/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-12 19:40:01.000000 ohnlp-backbone-xlang-python-1.0.9/ohnlp/toolkit/backbone/backbone_module_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:40:08.060664 ohnlp-backbone-xlang-python-1.0.9/ohnlp_backbone_xlang_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-12 19:40:08.000000 ohnlp-backbone-xlang-python-1.0.9/ohnlp_backbone_xlang_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-12 19:40:08.000000 ohnlp-backbone-xlang-python-1.0.9/ohnlp_backbone_xlang_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:40:08.000000 ohnlp-backbone-xlang-python-1.0.9/ohnlp_backbone_xlang_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-12 19:40:08.000000 ohnlp-backbone-xlang-python-1.0.9/ohnlp_backbone_xlang_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 19:40:08.000000 ohnlp-backbone-xlang-python-1.0.9/ohnlp_backbone_xlang_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 19:40:08.060664 ohnlp-backbone-xlang-python-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 19:40:01.000000 ohnlp-backbone-xlang-python-1.0.9/setup.py
```

### Comparing `ohnlp-backbone-xlang-python-1.0.8/LICENSE` & `ohnlp-backbone-xlang-python-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ohnlp-backbone-xlang-python-1.0.8/README.md` & `ohnlp-backbone-xlang-python-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ohnlp-backbone-xlang-python-1.0.8/ohnlp/toolkit/backbone/api.py` & `ohnlp-backbone-xlang-python-1.0.9/ohnlp/toolkit/backbone/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,14 +78,29 @@
     def get_values(self) -> List[object]:
         return self.values
 
     class Java:
         implements = ["org.ohnlp.backbone.api.components.xlang.python.PythonRow"]
 
 
+class TaggedRow(object):
+    def __init__(self, tag: str, row: Row):
+        self.tag: str = tag
+        self.row: Row = row
+
+    def get_tag(self) -> str:
+        return self.tag
+
+    def get_row(self) -> Row:
+        return self.row
+
+    class Java:
+        implements = ["org.ohnlp.backbone.api.components.xlang.python.PythonTaggedRow"]
+
+
 class BridgedInterfaceWithConvertableDataTypes(object):
     def python_schema_from_json_string(self, json_schema: str) -> Schema:
         schema_def: dict = json.loads(json_schema)
         return self.parse_schema_from_json(schema_def)
 
     def parse_schema_from_json(self, schema_def: dict) -> Schema:
         schema_fields: List[SchemaField] = []
@@ -227,8 +242,32 @@
         pass
 
     @abstractmethod
     def apply(self, input_row: Row) -> List[Row]:
         pass
 
     class Java:
-        implements = ["org.ohnlp.backbone.api.components.xlang.python.PythonOneToOneTransformDoFn"]
+        implements = ["org.ohnlp.backbone.api.components.xlang.python.PythonOneToOneTransformDoFn"]
+
+
+class BackboneComponentOneToManyDoFn(ABC, BridgedInterfaceWithConvertableDataTypes):
+    def __init__(self):
+        pass
+
+    @abstractmethod
+    def init_from_driver(self, config_json_str: str) -> None:
+        pass
+
+    @abstractmethod
+    def on_bundle_start(self) -> None:
+        pass
+
+    @abstractmethod
+    def on_bundle_end(self) -> None:
+        pass
+
+    @abstractmethod
+    def apply(self, input_row: Row) -> List[TaggedRow]:
+        pass
+
+    class Java:
+        implements = ["org.ohnlp.backbone.api.components.xlang.python.PythonOneToManyTransformDoFn"]
```

### Comparing `ohnlp-backbone-xlang-python-1.0.8/ohnlp/toolkit/backbone/backbone_module_launcher.py` & `ohnlp-backbone-xlang-python-1.0.9/ohnlp/toolkit/backbone/backbone_module_launcher.py`

 * *Files identical despite different names*

### Comparing `ohnlp-backbone-xlang-python-1.0.8/setup.py` & `ohnlp-backbone-xlang-python-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ohnlp-backbone-xlang-python",
-    version="1.0.8",
+    version="1.0.9",
     description="Python support for OHNLP Toolkit Backbone Components",
     author="Andrew Wen",
     author_email="contact@ohnlp.org",
     packages=find_packages(),
     python_requires='>3.7',
     install_requires=[
         'certifi==2023.5.7',
```

