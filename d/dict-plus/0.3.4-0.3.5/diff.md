# Comparing `tmp/dict_plus-0.3.4.tar.gz` & `tmp/dict_plus-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dict_plus-0.3.4.tar", last modified: Fri Jun  9 17:31:06 2023, max compression
+gzip compressed data, was "dict_plus-0.3.5.tar", last modified: Thu Jun 15 21:09:45 2023, max compression
```

## Comparing `dict_plus-0.3.4.tar` & `dict_plus-0.3.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 17:31:06.355894 dict_plus-0.3.4/
--rw-rw-rw-   0        0        0    35821 2023-06-09 16:46:36.000000 dict_plus-0.3.4/LICENSE
--rw-rw-rw-   0        0        0      357 2023-06-09 17:31:06.355894 dict_plus-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0       73 2023-06-09 17:29:54.000000 dict_plus-0.3.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-09 17:31:06.342664 dict_plus-0.3.4/dict_plus/
--rw-rw-rw-   0        0        0      409 2023-06-09 16:46:36.000000 dict_plus-0.3.4/dict_plus/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 17:31:06.351424 dict_plus-0.3.4/dict_plus/dicts/
--rw-rw-rw-   0        0        0      384 2023-06-09 16:46:36.000000 dict_plus-0.3.4/dict_plus/dicts/__init__.py
--rw-rw-rw-   0        0        0      619 2023-06-09 16:46:36.000000 dict_plus-0.3.4/dict_plus/dicts/dictlist.py
--rw-rw-rw-   0        0        0     1831 2023-06-09 16:46:36.000000 dict_plus-0.3.4/dict_plus/dicts/dictplus.py
--rw-rw-rw-   0        0        0     4239 2023-06-09 16:46:36.000000 dict_plus-0.3.4/dict_plus/dicts/hooked.py
--rw-rw-rw-   0        0        0    12076 2023-06-09 16:46:36.000000 dict_plus-0.3.4/dict_plus/dicts/insensitive.py
--rw-rw-rw-   0        0        0     4363 2023-06-09 16:46:36.000000 dict_plus-0.3.4/dict_plus/dicts/ordered.py
-drwxrwxrwx   0        0        0        0 2023-06-09 17:31:06.351424 dict_plus-0.3.4/dict_plus/elements/
--rw-rw-rw-   0        0        0     1024 2023-06-09 16:46:36.000000 dict_plus-0.3.4/dict_plus/elements/__init__.py
--rw-rw-rw-   0        0        0     7575 2023-06-09 16:46:36.000000 dict_plus-0.3.4/dict_plus/elements/element.py
--rw-rw-rw-   0        0        0      435 2023-06-09 16:46:36.000000 dict_plus-0.3.4/dict_plus/etypes.py
--rw-rw-rw-   0        0        0      586 2023-06-09 16:46:36.000000 dict_plus-0.3.4/dict_plus/exceptions.py
--rw-rw-rw-   0        0        0     2026 2023-06-09 16:46:36.000000 dict_plus-0.3.4/dict_plus/funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-09 17:31:06.351424 dict_plus-0.3.4/dict_plus/indexes/
--rw-rw-rw-   0        0        0      121 2023-06-09 16:46:36.000000 dict_plus-0.3.4/dict_plus/indexes/__init__.py
--rw-rw-rw-   0        0        0     5423 2023-06-09 16:46:36.000000 dict_plus-0.3.4/dict_plus/indexes/index.py
--rw-rw-rw-   0        0        0     1156 2023-06-09 16:46:36.000000 dict_plus-0.3.4/dict_plus/indexes/ordered.py
--rw-rw-rw-   0        0        0    35082 2023-06-09 16:46:36.000000 dict_plus-0.3.4/dict_plus/iterable.py
-drwxrwxrwx   0        0        0        0 2023-06-09 17:31:06.355894 dict_plus-0.3.4/dict_plus/lists/
--rw-rw-rw-   0        0        0       94 2023-06-09 16:46:36.000000 dict_plus-0.3.4/dict_plus/lists/__init__.py
--rw-rw-rw-   0        0        0     7652 2023-06-09 16:46:36.000000 dict_plus-0.3.4/dict_plus/lists/listdict.py
--rw-rw-rw-   0        0        0     6406 2023-06-09 16:46:36.000000 dict_plus-0.3.4/dict_plus/lists/listplus.py
-drwxrwxrwx   0        0        0        0 2023-06-09 17:31:06.355894 dict_plus-0.3.4/dict_plus/utils/
--rw-rw-rw-   0        0        0        0 2023-06-09 17:29:54.000000 dict_plus-0.3.4/dict_plus/utils/__init__.py
--rw-rw-rw-   0        0        0     2414 2023-06-09 17:29:54.000000 dict_plus-0.3.4/dict_plus/utils/simpleflatten.py
-drwxrwxrwx   0        0        0        0 2023-06-09 17:31:06.348203 dict_plus-0.3.4/dict_plus.egg-info/
--rw-rw-rw-   0        0        0      357 2023-06-09 17:31:06.000000 dict_plus-0.3.4/dict_plus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      726 2023-06-09 17:31:06.000000 dict_plus-0.3.4/dict_plus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 17:31:06.000000 dict_plus-0.3.4/dict_plus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-09 17:31:06.000000 dict_plus-0.3.4/dict_plus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 17:31:06.355894 dict_plus-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1185 2023-06-09 17:31:05.000000 dict_plus-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:09:45.496898 dict_plus-0.3.5/
+-rw-rw-rw-   0        0        0    35821 2023-06-09 16:46:36.000000 dict_plus-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0      357 2023-06-15 21:09:45.496898 dict_plus-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0       73 2023-06-09 17:29:54.000000 dict_plus-0.3.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-15 21:09:45.485564 dict_plus-0.3.5/dict_plus/
+-rw-rw-rw-   0        0        0      409 2023-06-09 16:46:36.000000 dict_plus-0.3.5/dict_plus/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:09:45.492286 dict_plus-0.3.5/dict_plus/dicts/
+-rw-rw-rw-   0        0        0      384 2023-06-09 16:46:36.000000 dict_plus-0.3.5/dict_plus/dicts/__init__.py
+-rw-rw-rw-   0        0        0      619 2023-06-09 16:46:36.000000 dict_plus-0.3.5/dict_plus/dicts/dictlist.py
+-rw-rw-rw-   0        0        0     1831 2023-06-09 16:46:36.000000 dict_plus-0.3.5/dict_plus/dicts/dictplus.py
+-rw-rw-rw-   0        0        0     4239 2023-06-09 16:46:36.000000 dict_plus-0.3.5/dict_plus/dicts/hooked.py
+-rw-rw-rw-   0        0        0    12076 2023-06-09 16:46:36.000000 dict_plus-0.3.5/dict_plus/dicts/insensitive.py
+-rw-rw-rw-   0        0        0     4363 2023-06-09 16:46:36.000000 dict_plus-0.3.5/dict_plus/dicts/ordered.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:09:45.493286 dict_plus-0.3.5/dict_plus/elements/
+-rw-rw-rw-   0        0        0     1024 2023-06-09 16:46:36.000000 dict_plus-0.3.5/dict_plus/elements/__init__.py
+-rw-rw-rw-   0        0        0     7575 2023-06-09 16:46:36.000000 dict_plus-0.3.5/dict_plus/elements/element.py
+-rw-rw-rw-   0        0        0      435 2023-06-09 16:46:36.000000 dict_plus-0.3.5/dict_plus/etypes.py
+-rw-rw-rw-   0        0        0      586 2023-06-09 16:46:36.000000 dict_plus-0.3.5/dict_plus/exceptions.py
+-rw-rw-rw-   0        0        0     2026 2023-06-09 16:46:36.000000 dict_plus-0.3.5/dict_plus/funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:09:45.494285 dict_plus-0.3.5/dict_plus/indexes/
+-rw-rw-rw-   0        0        0      121 2023-06-09 16:46:36.000000 dict_plus-0.3.5/dict_plus/indexes/__init__.py
+-rw-rw-rw-   0        0        0     5423 2023-06-09 16:46:36.000000 dict_plus-0.3.5/dict_plus/indexes/index.py
+-rw-rw-rw-   0        0        0     1156 2023-06-09 16:46:36.000000 dict_plus-0.3.5/dict_plus/indexes/ordered.py
+-rw-rw-rw-   0        0        0    35082 2023-06-09 16:46:36.000000 dict_plus-0.3.5/dict_plus/iterable.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:09:45.494891 dict_plus-0.3.5/dict_plus/lists/
+-rw-rw-rw-   0        0        0       94 2023-06-09 16:46:36.000000 dict_plus-0.3.5/dict_plus/lists/__init__.py
+-rw-rw-rw-   0        0        0     7652 2023-06-09 16:46:36.000000 dict_plus-0.3.5/dict_plus/lists/listdict.py
+-rw-rw-rw-   0        0        0     6406 2023-06-09 16:46:36.000000 dict_plus-0.3.5/dict_plus/lists/listplus.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:09:45.495894 dict_plus-0.3.5/dict_plus/utils/
+-rw-rw-rw-   0        0        0       44 2023-06-15 21:09:37.000000 dict_plus-0.3.5/dict_plus/utils/__init__.py
+-rw-rw-rw-   0        0        0     2560 2023-06-15 21:05:58.000000 dict_plus-0.3.5/dict_plus/utils/simpleflatten.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:09:45.488862 dict_plus-0.3.5/dict_plus.egg-info/
+-rw-rw-rw-   0        0        0      357 2023-06-15 21:09:45.000000 dict_plus-0.3.5/dict_plus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      726 2023-06-15 21:09:45.000000 dict_plus-0.3.5/dict_plus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 21:09:45.000000 dict_plus-0.3.5/dict_plus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-15 21:09:45.000000 dict_plus-0.3.5/dict_plus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 21:09:45.496898 dict_plus-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1185 2023-06-15 21:05:58.000000 dict_plus-0.3.5/setup.py
```

### Comparing `dict_plus-0.3.4/LICENSE` & `dict_plus-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.4/dict_plus/dicts/dictlist.py` & `dict_plus-0.3.5/dict_plus/dicts/dictlist.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.4/dict_plus/dicts/dictplus.py` & `dict_plus-0.3.5/dict_plus/dicts/dictplus.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.4/dict_plus/dicts/hooked.py` & `dict_plus-0.3.5/dict_plus/dicts/hooked.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.4/dict_plus/dicts/insensitive.py` & `dict_plus-0.3.5/dict_plus/dicts/insensitive.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.4/dict_plus/dicts/ordered.py` & `dict_plus-0.3.5/dict_plus/dicts/ordered.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.4/dict_plus/elements/__init__.py` & `dict_plus-0.3.5/dict_plus/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.4/dict_plus/elements/element.py` & `dict_plus-0.3.5/dict_plus/elements/element.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.4/dict_plus/exceptions.py` & `dict_plus-0.3.5/dict_plus/exceptions.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.4/dict_plus/funcs.py` & `dict_plus-0.3.5/dict_plus/funcs.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.4/dict_plus/indexes/index.py` & `dict_plus-0.3.5/dict_plus/indexes/index.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.4/dict_plus/indexes/ordered.py` & `dict_plus-0.3.5/dict_plus/indexes/ordered.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.4/dict_plus/iterable.py` & `dict_plus-0.3.5/dict_plus/iterable.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.4/dict_plus/lists/listdict.py` & `dict_plus-0.3.5/dict_plus/lists/listdict.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.4/dict_plus/lists/listplus.py` & `dict_plus-0.3.5/dict_plus/lists/listplus.py`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.4/dict_plus/utils/simpleflatten.py` & `dict_plus-0.3.5/dict_plus/utils/simpleflatten.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,23 +15,25 @@
     class _SimpleListType(object):
         """
         Helper class to distinguish a 'Simple List' a list of simple typed data
         """
         def __init__(self, val):
             self.val = val
 
-    def __init__(self, simple_types=[], maxdepth=math.inf):
+    def __init__(self, simple_types=[], maxdepth=math.inf, delimiter="_"):
         """
         simple_types is a list of types that should be treated as simple, base cases
         maxdepth is the maximum depth within the data to traverse, defaults to no maximum
+        delimiter is the string used to separate subkeys in the flattened dict
         """
         self.simple_types = {str, bytes, int, float, bool, tuple}
         self.max_depth = maxdepth
         for s in simple_types:
             self.simple_types.add(s)
+        self.delimiter = delimiter
 
     def is_simplelist(self, val):
         """
         Check if a list is only of simple_types and also not mixed types
         """
         if isinstance(val, list):
             list_types = set()
@@ -42,15 +44,15 @@
                     return True
             return False  # Multiple types of data within the list, or data is not simple
         else:
             return False
 
     def flatten(self, data, current_depth=0, key_prefix=""):
         if key_prefix:
-            key_prefix = f"{key_prefix}_"
+            key_prefix = f"{key_prefix}{self.delimiter}"
 
         if current_depth > self.max_depth:
             return {key_prefix: data}
 
         if isinstance(data, dict):
             newdict = {}
             for key, val in data.items():
```

### Comparing `dict_plus-0.3.4/dict_plus.egg-info/SOURCES.txt` & `dict_plus-0.3.5/dict_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dict_plus-0.3.4/setup.py` & `dict_plus-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import json
 
-VERSION = "0.3.4"
+VERSION = "0.3.5"
 
 
 def check_version_info():
     try:
         with open("version.json", "r") as f:
             data = json.load(f)
             assert data["version"] == VERSION  # Assert that the versions are the same
```

