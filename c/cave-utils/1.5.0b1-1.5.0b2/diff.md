# Comparing `tmp/cave_utils-1.5.0b1.tar.gz` & `tmp/cave_utils-1.5.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cave_utils-1.5.0b1.tar", last modified: Tue Jun 13 20:29:42 2023, max compression
+gzip compressed data, was "cave_utils-1.5.0b2.tar", last modified: Thu Jun 15 14:50:45 2023, max compression
```

## Comparing `cave_utils-1.5.0b1.tar` & `cave_utils-1.5.0b2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 conmak    (1000) docker     (999)        0 2023-06-13 20:29:42.218368 cave_utils-1.5.0b1/
--rw-rw-r--   0 conmak    (1000) docker     (999)    11357 2023-06-13 15:21:54.000000 cave_utils-1.5.0b1/LICENSE
--rw-rw-r--   0 conmak    (1000) docker     (999)      631 2023-06-13 15:22:15.000000 cave_utils-1.5.0b1/NOTICE.md
--rw-rw-r--   0 conmak    (1000) docker     (999)     1608 2023-06-13 20:29:42.218368 cave_utils-1.5.0b1/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) docker     (999)      927 2023-06-13 20:25:36.000000 cave_utils-1.5.0b1/README.md
-drwxrwxr-x   0 conmak    (1000) docker     (999)        0 2023-06-13 20:29:42.218368 cave_utils-1.5.0b1/cave_utils/
--rw-rw-r--   0 conmak    (1000) docker     (999)        0 2023-06-13 15:24:05.000000 cave_utils-1.5.0b1/cave_utils/__init__ .py
--rw-rw-r--   0 conmak    (1000) docker     (999)      257 2023-06-13 15:24:47.000000 cave_utils-1.5.0b1/cave_utils/socket.py
--rw-rw-r--   0 conmak    (1000) docker     (999)    53736 2023-06-13 19:58:25.000000 cave_utils-1.5.0b1/cave_utils/validator.py
-drwxrwxr-x   0 conmak    (1000) docker     (999)        0 2023-06-13 20:29:42.218368 cave_utils-1.5.0b1/cave_utils.egg-info/
--rw-rw-r--   0 conmak    (1000) docker     (999)     1608 2023-06-13 20:29:42.000000 cave_utils-1.5.0b1/cave_utils.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) docker     (999)      319 2023-06-13 20:29:42.000000 cave_utils-1.5.0b1/cave_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) docker     (999)        1 2023-06-13 20:29:42.000000 cave_utils-1.5.0b1/cave_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) docker     (999)       13 2023-06-13 20:29:42.000000 cave_utils-1.5.0b1/cave_utils.egg-info/requires.txt
--rw-rw-r--   0 conmak    (1000) docker     (999)       11 2023-06-13 20:29:42.000000 cave_utils-1.5.0b1/cave_utils.egg-info/top_level.txt
--rwxrwxr-x   0 conmak    (1000) docker     (999)      101 2023-06-13 14:42:48.000000 cave_utils-1.5.0b1/pyproject.toml
--rwxrwxr-x   0 conmak    (1000) docker     (999)       79 2023-06-13 20:29:42.218368 cave_utils-1.5.0b1/setup.cfg
--rwxrwxr-x   0 conmak    (1000) docker     (999)      999 2023-06-13 20:27:46.000000 cave_utils-1.5.0b1/setup.py
-drwxrwxr-x   0 conmak    (1000) docker     (999)        0 2023-06-13 20:29:42.218368 cave_utils-1.5.0b1/test/
--rw-rw-r--   0 conmak    (1000) docker     (999)       46 2023-06-13 15:19:05.000000 cave_utils-1.5.0b1/test/test_import.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-15 14:50:45.919441 cave_utils-1.5.0b2/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    11357 2023-06-13 15:21:54.000000 cave_utils-1.5.0b2/LICENSE
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      631 2023-06-13 15:22:15.000000 cave_utils-1.5.0b2/NOTICE.md
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1606 2023-06-15 14:50:45.919441 cave_utils-1.5.0b2/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      927 2023-06-13 20:25:36.000000 cave_utils-1.5.0b2/README.md
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-15 14:50:45.915440 cave_utils-1.5.0b2/cave_utils/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        0 2023-06-13 15:24:05.000000 cave_utils-1.5.0b2/cave_utils/__init__ .py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      257 2023-06-13 15:24:47.000000 cave_utils-1.5.0b2/cave_utils/socket.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    54839 2023-06-15 14:50:12.000000 cave_utils-1.5.0b2/cave_utils/validator.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-15 14:50:45.919441 cave_utils-1.5.0b2/cave_utils.egg-info/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1606 2023-06-15 14:50:45.000000 cave_utils-1.5.0b2/cave_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      319 2023-06-15 14:50:45.000000 cave_utils-1.5.0b2/cave_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-06-15 14:50:45.000000 cave_utils-1.5.0b2/cave_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       13 2023-06-15 14:50:45.000000 cave_utils-1.5.0b2/cave_utils.egg-info/requires.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2023-06-15 14:50:45.000000 cave_utils-1.5.0b2/cave_utils.egg-info/top_level.txt
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      101 2023-06-13 14:42:48.000000 cave_utils-1.5.0b2/pyproject.toml
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-06-15 14:50:45.919441 cave_utils-1.5.0b2/setup.cfg
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      997 2023-06-15 14:46:45.000000 cave_utils-1.5.0b2/setup.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-06-15 14:50:45.919441 cave_utils-1.5.0b2/test/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       46 2023-06-13 15:19:05.000000 cave_utils-1.5.0b2/test/test_import.py
```

### Comparing `cave_utils-1.5.0b1/LICENSE` & `cave_utils-1.5.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.0b1/NOTICE.md` & `cave_utils-1.5.0b2/NOTICE.md`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.0b1/PKG-INFO` & `cave_utils-1.5.0b2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cave_utils
-Version: 1.5.0b1
+Version: 1.5.0b2
 Summary: Cave utilities for the CAVE App at the MIT
 Home-page: https://github.com/mit-cave/cave_utils
-Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b1.1.tar.gz
+Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b2.tar.gz
 Author: Connor Makowski
 Author-email: connor.m.makowski@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cave_utils-1.5.0b1/README.md` & `cave_utils-1.5.0b2/README.md`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.0b1/cave_utils/validator.py` & `cave_utils-1.5.0b2/cave_utils/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,54 +1,64 @@
 from pamda import pamda
-import re, copy, json
+import re
+import copy
 
 
 class LogObject:
-    def __init__(self, errors: dict = dict(), warnings: dict = dict()):
-        self.errors = errors
-        self.warnings = warnings
-
-    def add(self, path, error, level="error"):
-        assert level in ["error", "warning"], "level must be one of `error` or `warning`"
-        data = self.warnings if level == "warning" else self.errors
-        path = path + [level]
-        pamda.assocPath(path=path, value=pamda.pathOr([], path, data) + [error], data=data)
+    def __init__(self):
+        self.log = []
+
+    def add(self, path, msg, level="error"):
+        self.log.append({"path": path, "msg": msg, "level": level})
+
+    def get_logs(self, level=None):
+        if level is None:
+            return self.log
+        assert level in ["error", "warning"], "Invalid level, must be 'error' or 'warning'"
+        return [i for i in self.log if i["level"] == level]
+
+    def write_logs(self, path, level=None):
+        pamda.write_json(path, self.get_logs(level=level), pretty=True)
+
+    def print_logs(self, level=None):
+        for i in self.get_logs(level=level):
+            print("=" * 50)
+            print(f"Path: {i['path']}")
+            print(f"Message: {i['msg']}")
+            print(f"Level: {i['level']}")
 
 
 class LogHelper:
     def __init__(self, log: LogObject, prepend_path: list):
         self.log = log
         self.prepend_path = prepend_path
 
-    def add(self, path, error, level="error"):
-        self.log.add(path=self.prepend_path + path, error=error, level=level)
-
-    def show(self):
-        self.log.show()
+    def add(self, path, msg, level="error"):
+        self.log.add(path=self.prepend_path + path, msg=msg, level=level)
 
 
 class CoreValidator:
     def __init__(self, data, log: LogObject, prepend_path: list = [], **kwargs):
         self.data = copy.deepcopy(data)
         self.log = LogHelper(log=log, prepend_path=prepend_path)
         self.populate_data(**kwargs)
         self.validate()
         try:
             self.additional_validations(**kwargs)
         except Exception as e:
             self.log.add(
                 path=[],
-                error=f"Additional validations failed (likely due to another error with your api data)",
+                msg=f"Additional validations failed (likely due to another error with your api data)",
             )
         # self.additional_validations(**kwargs)
 
     def validate(self):
         for field in self.required_fields:
             if field not in self.data:
-                self.log.add(path=[field], error=f"Missing required field")
+                self.log.add(path=[field], msg=f"Missing required field")
         for field, value in self.data.items():
             accepted_values = self.accepted_values.get(field, None)
             if (
                 isinstance(
                     value,
                     (
                         list,
@@ -60,35 +70,36 @@
                 check_value = value
                 if isinstance(value, dict):
                     check_value = list(value.keys())
                 value_diff = pamda.difference(check_value, accepted_values)
                 if len(value_diff) > 0:
                     self.log.add(
                         path=[field],
-                        error=f"Invalid values ({value_diff}): Acceptable values are: {accepted_values}",
+                        msg=f"Invalid values ({value_diff}): Acceptable values are: {accepted_values}",
                     )
                     continue
             else:
                 if accepted_values is not None and value not in accepted_values:
                     self.log.add(
                         path=[field],
-                        error=f"Invalid value ({value}): Acceptable values are: {accepted_values}",
+                        msg=f"Invalid value ({value}): Acceptable values are: {accepted_values}",
                     )
                     continue
             if field not in self.required_fields + self.optional_fields:
                 self.log.add(
                     path=[field],
-                    error=f"Unknown field: Acceptable fields are: {self.required_fields + self.optional_fields}",
+                    msg=f"Unknown field ({field}): Acceptable fields are: {self.required_fields + self.optional_fields}",
+                    level="warning",
                 )
                 continue
             acceptable_types = self.field_types.get(field, type(None))
             if not isinstance(value, acceptable_types):
                 self.log.add(
                     path=[field],
-                    error=f"Invalid type ({type(value)}): Acceptable types are: {acceptable_types}",
+                    msg=f"Invalid type ({type(value)}): Acceptable types are: {acceptable_types}",
                 )
 
     def additional_validations(self, **kwargs):
         pass
 
     def is_rgb_string_valid(self, rgb_string: str):
         try:
@@ -104,15 +115,15 @@
                     return False
         except:
             return False
         return True
 
     def validate_rgb_string(self, rgb_string: str, prepend_path: list = []):
         if not self.is_rgb_string_valid(rgb_string):
-            self.log.add(path=prepend_path, error=f"Invalid rgb string: {rgb_string}")
+            self.log.add(path=prepend_path, msg=f"Invalid rgb string: {rgb_string}")
 
     def is_url_valid(self, url: str):
         # Use Django regex for URL validation
         # See https://stackoverflow.com/a/7160778/12014156
         regex = re.compile(
             r"^(?:http|ftp)s?://"  # http:// or https://
             r"(?:(?:[A-Z0-9](?:[A-Z0-9-]{0,61}[A-Z0-9])?\.)+(?:[A-Z]{2,6}\.?|[A-Z0-9-]{2,}\.?)|"  # domain...
@@ -123,26 +134,52 @@
             re.IGNORECASE,
         )
         is_valid = re.match(regex, url) is not None
         return re.match(regex, url) is not None
 
     def validate_url(self, url: str, prepend_path: list = []):
         if not self.is_url_valid(url):
-            self.log.add(path=prepend_path, error=f"Invalid URL: {url}")
+            self.log.add(path=prepend_path, msg=f"Invalid URL: {url}")
 
     def error(self, error: str, prepend_path: list = []):
-        self.log.add(path=prepend_path, error=error)
+        self.log.add(path=prepend_path, msg=error)
 
     def warn(self, error: str, prepend_path: list = []):
-        self.log.add(path=prepend_path, error=error, level="warning")
+        self.log.add(path=prepend_path, msg=error, level="warning")
 
     def validate_subset(self, subset: list, valid_values: list, prepend_path: list = []):
         invalid_values = pamda.difference(subset, valid_values)
         if len(invalid_values) > 0:
-            self.log.add(path=prepend_path, error=f"Invalid subset values: {invalid_values}")
+            self.log.add(path=prepend_path, msg=f"Invalid subset values: {invalid_values}")
+
+    def is_coord_path_valid(self, coord_path: list):
+        try:
+            if len(coord_path) < 2:
+                return False
+            for coord in coord_path:
+                # Ensure coord is less than 3 items (longitude, latitude, altitude)
+                if len(coord) > 3:
+                    return False
+                # Check Longitude
+                if coord[0] < -180 or coord[0] > 180:
+                    return False
+                # Check Latitude
+                if coord[1] < -90 or coord[1] > 90:
+                    return False
+                # Check Altitude (if present)
+                if len(coord) == 3:
+                    if coord[2] < 0:
+                        return False
+        except:
+            return False
+        return True
+
+    def validate_coord_path(self, coord_path: list, prepend_path: list = []):
+        if not self.is_coord_path_valid(coord_path):
+            self.log.add(path=prepend_path, msg=f"Invalid coordinate path")
 
 
 class NumericDictValidator(CoreValidator):
     def populate_data(self, **kwargs):
         self.field_types = {i: (int, float) for i in self.data.keys()}
         self.required_fields = list(self.data.keys())
         self.optional_fields = []
@@ -269,17 +306,25 @@
             "numberFormat": dict,
         }
 
         self.allowed_variants = {
             "head": ["column", "row"],
             "text": ["textarea"],
             "num": ["slider"],
-            "selector": ["dropdown", "checkbox", "radio", "combobox", "hstepper", "vstepper", "hradio"],
+            "selector": [
+                "dropdown",
+                "checkbox",
+                "radio",
+                "combobox",
+                "hstepper",
+                "vstepper",
+                "hradio",
+            ],
             "date": ["date", "time", "datetime"],
-            "media": ["picture", "video"]
+            "media": ["picture", "video"],
         }
 
         self.accepted_values = {
             "type": ["head", "num", "toggle", "button", "text", "selector", "date", "media"],
             "variant": self.allowed_variants.get(validation_type, None),
             "views": ["year", "day", "hours", "minutes"],
         }
@@ -576,14 +621,15 @@
             "startAltitude": (float, int),
             "startClick": int,
             "endLatitude": (float, int),
             "endLongitude": (float, int),
             "endAltitude": (float, int),
             "endClick": int,
             "category": dict,
+            "path": list,
             # Overlapping fields
             "props": dict,
             "layout": dict,
         }
 
         self.required_fields = {
             "nodes": ["props", "type", "latitude", "longitude"],
@@ -604,26 +650,28 @@
                 "name",
                 "layout",
                 "startClick",
                 "endClick",
                 "category",
                 "startAltitude",
                 "endAltitude",
+                "path",
             ],
             "geos": ["name", "layout", "startClick", "endClick", "category"],
         }.get(self.top_level_key, [])
 
         self.accepted_values = {
             "type": list(self.types_data.keys()),
         }
 
     def additional_validations(self, **kwargs):
         props = self.data.get("props")
         layout = self.data.get("layout")
         category = self.data.get("category")
+        path = self.data.get("path")
         if props is not None:
             CustomKeyValidator(
                 data=props, log=self.log, prepend_path=["props"], validator=PropValidator, **kwargs
             )
         if layout is not None:
             acceptable_keys = list(props.keys()) if props is not None else []
             LayoutValidator(
@@ -631,14 +679,16 @@
                 log=self.log,
                 prepend_path=["layout"],
                 acceptable_keys=acceptable_keys,
                 **kwargs,
             )
         if category is not None:
             CategoryValidator(data=category, log=self.log, prepend_path=["category"], **kwargs)
+        if path is not None:
+            self.validate_coord_path(coord_path=path, prepend_path=["path"])
 
 
 class CategoriesValidator(CoreValidator):
     def populate_data(self, **kwargs):
         self.field_types = {
             "data": dict,
             "allowModification": bool,
@@ -1468,19 +1518,19 @@
 
         self.accepted_values = {}
 
         self.required_fields = ["name", "showToggle", "value", "data"]
 
         self.optional_fields = []
 
-    def additional_validations(self, **kwargs):
-        root_data = kwargs.get("root_data", {})
-        for key, path in self.data.get("data", {}).items():
-            if not pamda.hasPath(path, root_data):
-                self.warn(f"Path {path} does not exist.", prepend_path=["data", key])
+    # def additional_validations(self, **kwargs):
+    #     root_data = kwargs.get("root_data", {})
+    #     for key, path in self.data.get("data", {}).items():
+    #         if not pamda.hasPath(path, root_data):
+    #             self.warn(f"Path {path} does not exist.", prepend_path=["data", key])
 
 
 class RootValidator(CoreValidator):
     def populate_data(self, **kwargs):
         self.field_types = {
             "appBar": dict,
             "arcs": dict,
@@ -1625,24 +1675,7 @@
 
 class Validator:
     def __init__(self, session_data, **kwargs):
         self.session_data = session_data
         self.log = LogObject()
 
         RootValidator(data=self.session_data, log=self.log, prepend_path=[])
-
-        self.errors = self.log.errors
-        self.warnings = self.log.warnings
-
-    def print_errors(self):
-        print("Errors:")
-        print(json.dumps(self.errors, indent=2))
-
-    def print_warnings(self):
-        print("Warnings:")
-        print(json.dumps(self.warnings, indent=2))
-
-    def write_errors(self, path):
-        pamda.write_json(path, self.errors, pretty=True)
-
-    def write_warnings(self, path):
-        pamda.write_json(path, self.warnings, pretty=True)
```

### Comparing `cave_utils-1.5.0b1/cave_utils.egg-info/PKG-INFO` & `cave_utils-1.5.0b2/cave_utils.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cave-utils
-Version: 1.5.0b1
+Version: 1.5.0b2
 Summary: Cave utilities for the CAVE App at the MIT
 Home-page: https://github.com/mit-cave/cave_utils
-Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b1.1.tar.gz
+Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b2.tar.gz
 Author: Connor Makowski
 Author-email: connor.m.makowski@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cave_utils-1.5.0b1/setup.py` & `cave_utils-1.5.0b2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'cave_utils',
   packages=['cave_utils'],
-  version = '1.5.0b1',
+  version = '1.5.0b2',
   license='MIT',
   description = 'Cave utilities for the CAVE App at the MIT',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Connor Makowski',
   author_email = 'connor.m.makowski@gmail.com',
   url = 'https://github.com/mit-cave/cave_utils',
-  download_url = 'https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b1.1.tar.gz',
+  download_url = 'https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.0b2.tar.gz',
   keywords = [],
   install_requires=[
     'pamda>=2.1.2',
   ],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

