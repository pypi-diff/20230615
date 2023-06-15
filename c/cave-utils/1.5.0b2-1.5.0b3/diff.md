# Comparing `tmp/cave_utils-1.5.0b2.tar.gz` & `tmp/cave_utils-1.5.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cave_utils-1.5.0b2.tar", last modified: Thu Jun 15 14:50:45 2023, max compression
+gzip compressed data, was "cave_utils-1.5.0b3.tar", last modified: Thu Jun 15 19:05:09 2023, max compression
```

## Comparing `cave_utils-1.5.0b2.tar` & `cave_utils-1.5.0b3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-15 14:50:45.919441 cave_utils-1.5.0b2/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    11357 2023-06-13 15:21:54.000000 cave_utils-1.5.0b2/LICENSE
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      631 2023-06-13 15:22:15.000000 cave_utils-1.5.0b2/NOTICE.md
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1606 2023-06-15 14:50:45.919441 cave_utils-1.5.0b2/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      927 2023-06-13 20:25:36.000000 cave_utils-1.5.0b2/README.md
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-15 14:50:45.915440 cave_utils-1.5.0b2/cave_utils/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        0 2023-06-13 15:24:05.000000 cave_utils-1.5.0b2/cave_utils/__init__ .py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      257 2023-06-13 15:24:47.000000 cave_utils-1.5.0b2/cave_utils/socket.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    54839 2023-06-15 14:50:12.000000 cave_utils-1.5.0b2/cave_utils/validator.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-15 14:50:45.919441 cave_utils-1.5.0b2/cave_utils.egg-info/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1606 2023-06-15 14:50:45.000000 cave_utils-1.5.0b2/cave_utils.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      319 2023-06-15 14:50:45.000000 cave_utils-1.5.0b2/cave_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-06-15 14:50:45.000000 cave_utils-1.5.0b2/cave_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       13 2023-06-15 14:50:45.000000 cave_utils-1.5.0b2/cave_utils.egg-info/requires.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2023-06-15 14:50:45.000000 cave_utils-1.5.0b2/cave_utils.egg-info/top_level.txt
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      101 2023-06-13 14:42:48.000000 cave_utils-1.5.0b2/pyproject.toml
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-06-15 14:50:45.919441 cave_utils-1.5.0b2/setup.cfg
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      997 2023-06-15 14:46:45.000000 cave_utils-1.5.0b2/setup.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-15 14:50:45.919441 cave_utils-1.5.0b2/test/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       46 2023-06-13 15:19:05.000000 cave_utils-1.5.0b2/test/test_import.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-15 19:05:09.668969 cave_utils-1.5.0b3/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    11357 2023-06-13 15:21:54.000000 cave_utils-1.5.0b3/LICENSE
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      631 2023-06-13 15:22:15.000000 cave_utils-1.5.0b3/NOTICE.md
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1606 2023-06-15 19:05:09.668969 cave_utils-1.5.0b3/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      927 2023-06-13 20:25:36.000000 cave_utils-1.5.0b3/README.md
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-15 19:05:09.664970 cave_utils-1.5.0b3/cave_utils/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        0 2023-06-13 15:24:05.000000 cave_utils-1.5.0b3/cave_utils/__init__ .py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      257 2023-06-13 15:24:47.000000 cave_utils-1.5.0b3/cave_utils/socket.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    55892 2023-06-15 19:04:19.000000 cave_utils-1.5.0b3/cave_utils/validator.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-15 19:05:09.668969 cave_utils-1.5.0b3/cave_utils.egg-info/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1606 2023-06-15 19:05:09.000000 cave_utils-1.5.0b3/cave_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      319 2023-06-15 19:05:09.000000 cave_utils-1.5.0b3/cave_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-06-15 19:05:09.000000 cave_utils-1.5.0b3/cave_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       13 2023-06-15 19:05:09.000000 cave_utils-1.5.0b3/cave_utils.egg-info/requires.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2023-06-15 19:05:09.000000 cave_utils-1.5.0b3/cave_utils.egg-info/top_level.txt
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      101 2023-06-13 14:42:48.000000 cave_utils-1.5.0b3/pyproject.toml
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-06-15 19:05:09.668969 cave_utils-1.5.0b3/setup.cfg
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      997 2023-06-15 19:03:56.000000 cave_utils-1.5.0b3/setup.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-15 19:05:09.668969 cave_utils-1.5.0b3/test/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       46 2023-06-13 15:19:05.000000 cave_utils-1.5.0b3/test/test_import.py
```

### Comparing `cave_utils-1.5.0b2/LICENSE` & `cave_utils-1.5.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.0b2/NOTICE.md` & `cave_utils-1.5.0b3/NOTICE.md`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.0b2/PKG-INFO` & `cave_utils-1.5.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cave_utils
-Version: 1.5.0b2
+Version: 1.5.0b3
 Summary: Cave utilities for the CAVE App at the MIT
 Home-page: https://github.com/mit-cave/cave_utils
-Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b2.tar.gz
+Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b3.tar.gz
 Author: Connor Makowski
 Author-email: connor.m.makowski@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cave_utils-1.5.0b2/README.md` & `cave_utils-1.5.0b3/README.md`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.0b2/cave_utils/validator.py` & `cave_utils-1.5.0b3/cave_utils/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,54 +12,54 @@
 
     def get_logs(self, level=None):
         if level is None:
             return self.log
         assert level in ["error", "warning"], "Invalid level, must be 'error' or 'warning'"
         return [i for i in self.log if i["level"] == level]
 
-    def write_logs(self, path, level=None):
-        pamda.write_json(path, self.get_logs(level=level), pretty=True)
-
     def print_logs(self, level=None):
         for i in self.get_logs(level=level):
             print("=" * 50)
             print(f"Path: {i['path']}")
             print(f"Message: {i['msg']}")
             print(f"Level: {i['level']}")
 
+    def write_logs(self, path, level=None):
+        with open(path, "w") as f:
+            for i in self.get_logs(level=level):
+                f.write("=" * 50 + "\n")
+                f.write(f"Path: {i['path']}\n")
+                f.write(f"Message: {i['msg']}\n")
+                f.write(f"Level: {i['level']}\n")
+
 
 class LogHelper:
     def __init__(self, log: LogObject, prepend_path: list):
         self.log = log
         self.prepend_path = prepend_path
 
     def add(self, path, msg, level="error"):
         self.log.add(path=self.prepend_path + path, msg=msg, level=level)
 
 
 class CoreValidator:
-    def __init__(self, data, log: LogObject, prepend_path: list = [], **kwargs):
+    def __init__(self, data, log: LogObject, prepend_path: list = list(), **kwargs):
         self.data = copy.deepcopy(data)
+        self.ignore_keys = kwargs.get("ignore_keys", set())
         self.log = LogHelper(log=log, prepend_path=prepend_path)
         self.populate_data(**kwargs)
-        self.validate()
-        try:
-            self.additional_validations(**kwargs)
-        except Exception as e:
-            self.log.add(
-                path=[],
-                msg=f"Additional validations failed (likely due to another error with your api data)",
-            )
-        # self.additional_validations(**kwargs)
+        self.validate(**kwargs)
 
-    def validate(self):
+    def validate(self, **kwargs):
         for field in self.required_fields:
             if field not in self.data:
-                self.log.add(path=[field], msg=f"Missing required field")
+                self.log.add(path=[field], msg=f"Missing required field: ({field})")
         for field, value in self.data.items():
+            if field in self.ignore_keys:
+                continue
             accepted_values = self.accepted_values.get(field, None)
             if (
                 isinstance(
                     value,
                     (
                         list,
                         dict,
@@ -94,14 +94,23 @@
             acceptable_types = self.field_types.get(field, type(None))
             if not isinstance(value, acceptable_types):
                 self.log.add(
                     path=[field],
                     msg=f"Invalid type ({type(value)}): Acceptable types are: {acceptable_types}",
                 )
 
+        # Run additional Validations
+        try:
+            self.additional_validations(**kwargs)
+        except Exception as e:
+            self.log.add(
+                path=[],
+                msg=f"Additional validations failed (likely due to another error with your api data)",
+            )
+
     def additional_validations(self, **kwargs):
         pass
 
     def is_rgb_string_valid(self, rgb_string: str):
         try:
             if "rgb(" != rgb_string[:4]:
                 return False
@@ -215,14 +224,16 @@
         self.required_fields = []
         self.optional_fields = list(self.field_types.keys())
         self.accepted_values = {}
 
 
 class ColorByOptionValidator(CoreValidator):
     def is_categorical(self):
+        if self.data == {}:
+            return False
         expected_keys = ["min", "max", "startGradientColor", "endGradientColor"]
         return len(pamda.intersection(expected_keys, list(self.data.keys()))) == 0
 
     def populate_data(self, **kwargs):
         if self.is_categorical():
             self.field_types = {i: str for i in self.data.keys()}
             self.required_fields = list(self.data.keys())
@@ -299,14 +310,15 @@
             "variant": str,
             "enabled": bool,
             "options": dict,
             "maxValue": (int, float),
             "minValue": (int, float),
             "maxRows": int,
             "minRows": int,
+            "rows": int,
             "numberFormat": dict,
         }
 
         self.allowed_variants = {
             "head": ["column", "row"],
             "text": ["textarea"],
             "num": ["slider"],
@@ -339,14 +351,15 @@
                 "help",
                 "enabled",
                 "variant",
                 "apiCommand",
                 "apiCommandKeys",
                 "minRows",
                 "maxRows",
+                "rows",
             ],
             "num": [
                 "help",
                 "enabled",
                 "variant",
                 "apiCommand",
                 "apiCommandKeys",
@@ -1219,28 +1232,29 @@
             "groupScaleWithZoom": bool,
             "groupScale": (
                 int,
                 float,
             ),
             "groupMatchCategory": str,
             "groupMatchCategoryLevel": str,
+            "order": int,
         }
 
         self.accepted_values = {
             "sizeBy": prop_options,
             "colorBy": prop_options,
             "groupCalcByColor": ["count", "sum", "mean", "median", "mode", "min", "max"],
             "groupCalcBySize": ["count", "sum", "mean", "median", "mode", "min", "max"],
             "groupMatchCategory": list(categories.keys()),
             "groupMatchCategoryLevel": categories.get(self.data.get("groupMatchCategory"), []),
         }
 
         self.required_fields = ["value", "colorBy"]
 
-        self.optional_fields = []
+        self.optional_fields = ["order"]
 
         if layer_type == "nodes":
             self.optional_fields.extend(
                 [
                     "allowGrouping",
                     "group",
                     "groupCalcByColor",
@@ -1562,15 +1576,18 @@
         self.optional_fields = []
         self.accepted_values = {}
 
     def additional_validations(self, **kwargs):
         # Validate Categories
         ## Note this happens first to give useful feedback as categories are used in other validations
         CategoriesValidator(
-            data=self.data.get("categories", {}), log=self.log, prepend_path=["categories"]
+            data=self.data.get("categories", {}),
+            log=self.log,
+            prepend_path=["categories"],
+            **kwargs,
         )
         ## Get useful categories data for future validations
         categories_data = pamda.pathOr({}, ["categories", "data"], self.data)
         categories_key_values = {
             i: list(pamda.pathOr({}, ["data"], j).keys()) for i, j in categories_data.items()
         }
         categories_key_levels = {
@@ -1580,44 +1597,48 @@
 
         # Validate Stats
         StatsValidator(
             data=self.data.get("stats", {}),
             log=self.log,
             prepend_path=["stats"],
             categories_key_values=categories_key_values,
+            **kwargs,
         )
         ## Get useful stats data for future validations
         acceptable_stats = list(pamda.pathOr({}, ["stats", "types"], self.data).keys())
 
         # Validate KPIs
-        KpisValidator(data=self.data.get("kpis", {}), log=self.log, prepend_path=["kpis"])
+        KpisValidator(data=self.data.get("kpis", {}), log=self.log, prepend_path=["kpis"], **kwargs)
         ## Get useful kpis data for future validations
         acceptable_kpis = list(pamda.pathOr({}, ["kpis", "data"], self.data).keys())
 
         # Validate Arcs nodes and Geos
         ArcsNodesGeosValidator(
             data=self.data.get("arcs", {}),
             log=self.log,
             prepend_path=["arcs"],
             top_level_key="arcs",
             categories_key_values=categories_key_values,
+            **kwargs,
         )
         ArcsNodesGeosValidator(
             data=self.data.get("nodes", {}),
             log=self.log,
             prepend_path=["nodes"],
             top_level_key="nodes",
             categories_key_values=categories_key_values,
+            **kwargs,
         )
         ArcsNodesGeosValidator(
             data=self.data.get("geos", {}),
             log=self.log,
             prepend_path=["geos"],
             top_level_key="geos",
             categories_key_values=categories_key_values,
+            **kwargs,
         )
         ## Get useful arcs, nodes, and geos data for future validations
         node_prop_options = {
             k: list(v.get("props", {}).keys())
             for k, v in pamda.pathOr({}, ["nodes", "types"], self.data).items()
         }
         arc_prop_options = {
@@ -1626,56 +1647,72 @@
         }
         geo_prop_options = {
             k: list(v.get("props", {}).keys())
             for k, v in pamda.pathOr({}, ["geos", "types"], self.data).items()
         }
 
         # Validate AppBar
-        AppBarValidator(data=self.data.get("appBar", {}), log=self.log, prepend_path=["appBar"])
+        AppBarValidator(
+            data=self.data.get("appBar", {}), log=self.log, prepend_path=["appBar"], **kwargs
+        )
 
         # Validate Dashboards
         DashboardsValidator(
             data=self.data.get("dashboards", {}),
             log=self.log,
             prepend_path=["dashboards"],
             categories_key_levels=categories_key_levels,
             acceptable_stats=acceptable_stats,
             acceptable_kpis=acceptable_kpis,
+            **kwargs,
         )
 
         # Validate Kwargs
-        KwargsValidator(data=self.data.get("kwargs", {}), log=self.log, prepend_path=["kwargs"])
+        KwargsValidator(
+            data=self.data.get("kwargs", {}), log=self.log, prepend_path=["kwargs"], **kwargs
+        )
 
         # Validate Maps
         MapsValidator(
             data=self.data.get("maps", {}),
             log=self.log,
             prepend_path=["maps"],
             categories_key_levels=categories_key_levels,
             node_prop_options=node_prop_options,
             arc_prop_options=arc_prop_options,
             geo_prop_options=geo_prop_options,
+            **kwargs,
         )
 
         # Validate Panes
         PanesValidator(
             data=self.data.get("panes", {}),
             log=self.log,
             prepend_path=["panes"],
             categories_key_values=categories_key_values,
+            **kwargs,
         )
 
         # Validate Settings
         SettingsValidator(
             data=self.data.get("settings", {}),
             log=self.log,
             prepend_path=["settings"],
             root_data=self.data,
+            **kwargs,
         )
 
 
 class Validator:
-    def __init__(self, session_data, **kwargs):
+    def __init__(self, session_data, ignore_keys: list = [], **kwargs):
         self.session_data = session_data
         self.log = LogObject()
-
-        RootValidator(data=self.session_data, log=self.log, prepend_path=[])
+        assert isinstance(
+            ignore_keys,
+            (
+                list,
+                set,
+            ),
+        ), "`ignore_keys` must be a list of strings or set of strings"
+        RootValidator(
+            data=self.session_data, log=self.log, prepend_path=[], ignore_keys=set(ignore_keys)
+        )
```

### Comparing `cave_utils-1.5.0b2/cave_utils.egg-info/PKG-INFO` & `cave_utils-1.5.0b3/cave_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cave-utils
-Version: 1.5.0b2
+Version: 1.5.0b3
 Summary: Cave utilities for the CAVE App at the MIT
 Home-page: https://github.com/mit-cave/cave_utils
-Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b2.tar.gz
+Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b3.tar.gz
 Author: Connor Makowski
 Author-email: connor.m.makowski@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cave_utils-1.5.0b2/setup.py` & `cave_utils-1.5.0b3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'cave_utils',
   packages=['cave_utils'],
-  version = '1.5.0b2',
+  version = '1.5.0b3',
   license='MIT',
   description = 'Cave utilities for the CAVE App at the MIT',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Connor Makowski',
   author_email = 'connor.m.makowski@gmail.com',
   url = 'https://github.com/mit-cave/cave_utils',
-  download_url = 'https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b2.tar.gz',
+  download_url = 'https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b3.tar.gz',
   keywords = [],
   install_requires=[
     'pamda>=2.1.2',
   ],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

