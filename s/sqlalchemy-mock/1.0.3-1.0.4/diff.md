# Comparing `tmp/sqlalchemy_mock-1.0.3.tar.gz` & `tmp/sqlalchemy_mock-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_mock-1.0.3.tar", max compression
+gzip compressed data, was "sqlalchemy_mock-1.0.4.tar", max compression
```

## Comparing `sqlalchemy_mock-1.0.3.tar` & `sqlalchemy_mock-1.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1647 2023-05-13 14:38:38.650122 sqlalchemy_mock-1.0.3/README.md
--rw-r--r--   0        0        0      448 2023-06-13 08:15:28.453757 sqlalchemy_mock-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       98 2023-06-13 08:13:20.212930 sqlalchemy_mock-1.0.3/sqlalchemy_mock/__init__.py
--rw-r--r--   0        0        0      183 2023-06-13 08:13:20.213067 sqlalchemy_mock-1.0.3/sqlalchemy_mock/async_session.py
--rw-r--r--   0        0        0     4341 2023-06-13 08:13:20.213214 sqlalchemy_mock-1.0.3/sqlalchemy_mock/execute.py
--rw-r--r--   0        0        0     1427 2023-06-13 08:13:20.213390 sqlalchemy_mock-1.0.3/sqlalchemy_mock/query.py
--rw-r--r--   0        0        0     3258 2023-06-13 08:13:20.213584 sqlalchemy_mock-1.0.3/sqlalchemy_mock/session.py
--rw-r--r--   0        0        0     4407 2023-06-13 08:13:20.213788 sqlalchemy_mock-1.0.3/sqlalchemy_mock/utils.py
--rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 sqlalchemy_mock-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1647 2023-05-13 14:38:38.650122 sqlalchemy_mock-1.0.4/README.md
+-rw-r--r--   0        0        0      448 2023-06-15 17:25:10.662370 sqlalchemy_mock-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-06-13 08:13:20.212930 sqlalchemy_mock-1.0.4/sqlalchemy_mock/__init__.py
+-rw-r--r--   0        0        0      183 2023-06-13 08:13:20.213067 sqlalchemy_mock-1.0.4/sqlalchemy_mock/async_session.py
+-rw-r--r--   0        0        0     4341 2023-06-13 08:13:20.213214 sqlalchemy_mock-1.0.4/sqlalchemy_mock/execute.py
+-rw-r--r--   0        0        0     1427 2023-06-13 08:13:20.213390 sqlalchemy_mock-1.0.4/sqlalchemy_mock/query.py
+-rw-r--r--   0        0        0     3258 2023-06-13 08:13:20.213584 sqlalchemy_mock-1.0.4/sqlalchemy_mock/session.py
+-rw-r--r--   0        0        0     4575 2023-06-15 17:23:23.760224 sqlalchemy_mock-1.0.4/sqlalchemy_mock/utils.py
+-rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 sqlalchemy_mock-1.0.4/PKG-INFO
```

### Comparing `sqlalchemy_mock-1.0.3/README.md` & `sqlalchemy_mock-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.3/sqlalchemy_mock/execute.py` & `sqlalchemy_mock-1.0.4/sqlalchemy_mock/execute.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.3/sqlalchemy_mock/query.py` & `sqlalchemy_mock-1.0.4/sqlalchemy_mock/query.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.3/sqlalchemy_mock/session.py` & `sqlalchemy_mock-1.0.4/sqlalchemy_mock/session.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.3/sqlalchemy_mock/utils.py` & `sqlalchemy_mock-1.0.4/sqlalchemy_mock/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 from types import FunctionType
 import unittest.mock
 import sqlalchemy
 
 
 def set_choice_fields_to_record(record: object):
     for column in record.__table__.columns:
-        if getattr(column.type, "choices", None):
-            if isinstance(getattr(record, column.name), str):
-                setattr(record, column.name, getattr(column.type.choices, getattr(record, column.name)))
+        enum_attribute = None
+        if getattr(column.type, "enum_class", None): enum_attribute = "enum_class"
+        if getattr(column.type, "choices", None): enum_attribute = "choices"
 
+        if enum_attribute and isinstance(getattr(record, column.name), str):
+            setattr(record, column.name, getattr(getattr(column.type, enum_attribute), getattr(record, column.name)))
 
 def set_primary_key_to_record(record: object, primary_key: str, primary_key_generate: object):
     if not getattr(record, primary_key, None):
         setattr(record, primary_key, primary_key_generate())
 
 
 def set_default_fields(record: object):
```

### Comparing `sqlalchemy_mock-1.0.3/PKG-INFO` & `sqlalchemy_mock-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-mock
-Version: 1.0.3
+Version: 1.0.4
 Summary: The package for working with SQLAlchemy in unit tests
 Author: ivanostapiuk
 Author-email: ost.ivan13@gmail.com
 Requires-Python: >=3.0,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

