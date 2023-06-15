# Comparing `tmp/objtyping-0.5.3.post2.tar.gz` & `tmp/objtyping-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objtyping-0.5.3.post2.tar", last modified: Wed Jun 14 03:10:46 2023, max compression
+gzip compressed data, was "objtyping-0.5.4.tar", last modified: Thu Jun 15 09:10:28 2023, max compression
```

## Comparing `objtyping-0.5.3.post2.tar` & `objtyping-0.5.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:46.068442 objtyping-0.5.3.post2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 03:10:36.000000 objtyping-0.5.3.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-14 03:10:46.068442 objtyping-0.5.3.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-14 03:10:36.000000 objtyping-0.5.3.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:46.068442 objtyping-0.5.3.post2/objtyping/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-14 03:10:36.000000 objtyping-0.5.3.post2/objtyping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-06-14 03:10:36.000000 objtyping-0.5.3.post2/objtyping/objtyping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:46.068442 objtyping-0.5.3.post2/objtyping.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-14 03:10:46.000000 objtyping-0.5.3.post2/objtyping.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-14 03:10:46.000000 objtyping-0.5.3.post2/objtyping.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 03:10:46.000000 objtyping-0.5.3.post2/objtyping.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 03:10:46.000000 objtyping-0.5.3.post2/objtyping.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-14 03:10:36.000000 objtyping-0.5.3.post2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 03:10:46.068442 objtyping-0.5.3.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-14 03:10:36.000000 objtyping-0.5.3.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:46.068442 objtyping-0.5.3.post2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-14 03:10:36.000000 objtyping-0.5.3.post2/test/test_objtyping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:10:28.125179 objtyping-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 09:10:17.000000 objtyping-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-15 09:10:28.125179 objtyping-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-15 09:10:17.000000 objtyping-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:10:28.125179 objtyping-0.5.4/objtyping/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-15 09:10:17.000000 objtyping-0.5.4/objtyping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-06-15 09:10:17.000000 objtyping-0.5.4/objtyping/objtyping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:10:28.125179 objtyping-0.5.4/objtyping.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-15 09:10:28.000000 objtyping-0.5.4/objtyping.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-15 09:10:28.000000 objtyping-0.5.4/objtyping.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:10:28.000000 objtyping-0.5.4/objtyping.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 09:10:28.000000 objtyping-0.5.4/objtyping.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-15 09:10:17.000000 objtyping-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 09:10:28.125179 objtyping-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-15 09:10:17.000000 objtyping-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:10:28.125179 objtyping-0.5.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-15 09:10:17.000000 objtyping-0.5.4/test/test_objtyping.py
```

### Comparing `objtyping-0.5.3.post2/LICENSE` & `objtyping-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `objtyping-0.5.3.post2/PKG-INFO` & `objtyping-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objtyping
-Version: 0.5.3.post2
+Version: 0.5.4
 Summary: convert a primitive dict-list data structure to/from an instance of user-defined class.
 Author: Song Hui
 Author-email: songofhawk@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `objtyping-0.5.3.post2/README.md` & `objtyping-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `objtyping-0.5.3.post2/objtyping/objtyping.py` & `objtyping-0.5.4/objtyping/objtyping.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import inspect
 from datetime import datetime, date, timedelta
 from decimal import Decimal
+from enum import Enum
 from numbers import Number
 from typing import get_type_hints, TypeVar, Set, Any
 
 
 class DataObject(object):
     pass
 
@@ -213,15 +214,24 @@
                     attr = str(k)
                     if attr in self.ignores:
                         continue
                     dict1[attr] = self._convert(v, depth + 1, set(objs_chain))
                 return dict1
             elif type(obj).__name__ == 'Row' and callable(getattr(obj, 'keys', None)):
                 # SQLAlchemy 返回的数据行对象，直接转成dict
-                return dict(obj)
+                row_dict = dict(obj)
+                enum_value_dict = dict()
+                for k, v in row_dict.items():
+                    if isinstance(v, Enum):
+                        # 枚举类型无法直接序列化，只能取值
+                        row_dict[k] = v.name
+                        enum_value_dict[f'{k}__value'] = v.value    # 不能在遍历dict过程中，增加属性值，所以临时保存在另一个dict中
+                row_dict.update(enum_value_dict)
+                return row_dict
+
             elif hasattr(obj, '__dict__'):
                 # 如果是个自定义对象
                 dict1 = {}
                 items = list(obj.__dict__.items())  # 复制一份，避免遍历过程中改变
                 for k, v in items:
                     if self.ignore_protected and k.startswith('_'):
                         continue
```

### Comparing `objtyping-0.5.3.post2/objtyping.egg-info/PKG-INFO` & `objtyping-0.5.4/objtyping.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objtyping
-Version: 0.5.3.post2
+Version: 0.5.4
 Summary: convert a primitive dict-list data structure to/from an instance of user-defined class.
 Author: Song Hui
 Author-email: songofhawk@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `objtyping-0.5.3.post2/setup.py` & `objtyping-0.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="objtyping",
 
     # version of the module
-    version="0.5.3.r2",
+    version="0.5.4",
 
     # Name of Author
     author="Song Hui",
 
     # your Email address
     author_email="songofhawk@gmail.com",
```

### Comparing `objtyping-0.5.3.post2/test/test_objtyping.py` & `objtyping-0.5.4/test/test_objtyping.py`

 * *Files identical despite different names*

