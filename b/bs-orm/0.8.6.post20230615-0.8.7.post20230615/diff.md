# Comparing `tmp/bs_orm-0.8.6.post20230615.tar.gz` & `tmp/bs_orm-0.8.7.post20230615.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_orm-0.8.6.post20230615.tar", last modified: Wed Jun 14 23:56:02 2023, max compression
+gzip compressed data, was "bs_orm-0.8.7.post20230615.tar", last modified: Thu Jun 15 00:14:03 2023, max compression
```

## Comparing `bs_orm-0.8.6.post20230615.tar` & `bs_orm-0.8.7.post20230615.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 23:56:02.950685 bs_orm-0.8.6.post20230615/
--rw-rw-rw-   0        0        0      115 2023-06-14 23:56:02.950685 bs_orm-0.8.6.post20230615/PKG-INFO
--rw-rw-rw-   0        0        0     2557 2023-06-14 21:11:33.000000 bs_orm-0.8.6.post20230615/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 23:56:02.940160 bs_orm-0.8.6.post20230615/bs_orm/
--rw-rw-rw-   0        0        0     4727 2023-06-14 23:54:37.000000 bs_orm-0.8.6.post20230615/bs_orm/DataTypes.py
--rw-rw-rw-   0        0        0     9283 2023-06-14 22:24:23.000000 bs_orm-0.8.6.post20230615/bs_orm/Requests.py
--rw-rw-rw-   0        0        0        0 2023-06-14 21:11:33.000000 bs_orm-0.8.6.post20230615/bs_orm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:56:02.948719 bs_orm-0.8.6.post20230615/bs_orm.egg-info/
--rw-rw-rw-   0        0        0      115 2023-06-14 23:56:02.000000 bs_orm-0.8.6.post20230615/bs_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-06-14 23:56:02.000000 bs_orm-0.8.6.post20230615/bs_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 23:56:02.000000 bs_orm-0.8.6.post20230615/bs_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-14 23:56:02.000000 bs_orm-0.8.6.post20230615/bs_orm.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-14 23:56:02.000000 bs_orm-0.8.6.post20230615/bs_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       51 2023-06-14 23:56:02.951685 bs_orm-0.8.6.post20230615/setup.cfg
--rw-rw-rw-   0        0        0      286 2023-06-14 23:55:57.000000 bs_orm-0.8.6.post20230615/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 00:14:03.194411 bs_orm-0.8.7.post20230615/
+-rw-rw-rw-   0        0        0      115 2023-06-15 00:14:03.195411 bs_orm-0.8.7.post20230615/PKG-INFO
+-rw-rw-rw-   0        0        0     2557 2023-06-14 21:11:33.000000 bs_orm-0.8.7.post20230615/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 00:14:03.184859 bs_orm-0.8.7.post20230615/bs_orm/
+-rw-rw-rw-   0        0        0     4578 2023-06-15 00:13:24.000000 bs_orm-0.8.7.post20230615/bs_orm/DataTypes.py
+-rw-rw-rw-   0        0        0     9223 2023-06-15 00:04:30.000000 bs_orm-0.8.7.post20230615/bs_orm/Requests.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:11:33.000000 bs_orm-0.8.7.post20230615/bs_orm/__init__.py
+-rw-rw-rw-   0        0        0       32 2023-06-15 00:01:44.000000 bs_orm-0.8.7.post20230615/bs_orm/db_settings.py
+drwxrwxrwx   0        0        0        0 2023-06-15 00:14:03.193405 bs_orm-0.8.7.post20230615/bs_orm.egg-info/
+-rw-rw-rw-   0        0        0      115 2023-06-15 00:14:03.000000 bs_orm-0.8.7.post20230615/bs_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-06-15 00:14:03.000000 bs_orm-0.8.7.post20230615/bs_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 00:14:03.000000 bs_orm-0.8.7.post20230615/bs_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 00:14:03.000000 bs_orm-0.8.7.post20230615/bs_orm.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-15 00:14:03.000000 bs_orm-0.8.7.post20230615/bs_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       51 2023-06-15 00:14:03.196411 bs_orm-0.8.7.post20230615/setup.cfg
+-rw-rw-rw-   0        0        0      286 2023-06-15 00:13:56.000000 bs_orm-0.8.7.post20230615/setup.py
```

### Comparing `bs_orm-0.8.6.post20230615/README.md` & `bs_orm-0.8.7.post20230615/README.md`

 * *Files identical despite different names*

### Comparing `bs_orm-0.8.6.post20230615/bs_orm/DataTypes.py` & `bs_orm-0.8.7.post20230615/bs_orm/DataTypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import sqlite3
+from . import db_settings
 
 
 class empty():
     pass
 class DataType:
     def __init__(self, size=0, nullable=False, default=None, primary_key=False, check=None, unique=None):
         if primary_key and nullable:
@@ -32,39 +33,39 @@
     def __init__(self, table_column, on_delete=None, on_update=None, size=0, nullable=False, default=None, primary_key=False, check=None, unique=None):
         self.column = ' ('.join(table_column.split('.'))+')'
         if on_delete != None:
             self.column += ' ON DELETE ' + on_delete
         if on_update != None:
             self.column += ' ON UPDATE ' + on_update
 
-class Table_Engine:
+class Table:
     def __init__(self, **qwargs):
         for k, v in qwargs.items():
             self.__all__.__setattr__(k, v)
     
     @classmethod
     def search(cls, **qwargs):
         conn = sqlite3.connect(db_settings.path)
         cur = conn.cursor()
-        request  = f'SELECT * FROM [{cls.__name__}]' # fix this line
+        request  = f'SELECT * FROM [{cls.__name__}]'
         if qwargs != {}:
             request+=' WHERE'
             for atr, val in qwargs.items():
-                request+=cls.__check_type__(atr, val) + 'AND'
+                request+=cls.__check_type__(atr, val) + ' AND'
             request = request[:-4]
         cur.execute(request)
         conn.commit()
         values = cur.fetchall()
         returned = []
         obj = {}
         for line in values:
             column_names = iter(cur.description)
             for val in line:
                 obj[next(column_names)[0]] = val
-            returned.append(type(cls.__name__, (Table_Engine,), obj))
+            returned.append(type(cls.__name__, (Table,), obj))
         conn.commit()
         return returned
 
     @classmethod
     def save(cls):
         conn = sqlite3.connect(db_settings.path)
         cur = conn.cursor()
@@ -85,29 +86,29 @@
             return True
         except Exception as ex:
             raise Exception(f'well congratulations your father goes fucking you with a chair on the head with these words: {ex}')
 
     @classmethod
     def create(cls, **qwargs):
         obj = qwargs
-        new_cls = type(cls.__name__, (Table_Engine,), obj)
+        new_cls = type(cls.__name__, (Table,), obj)
         return new_cls
     
     @classmethod
     def add_if_not_exist(cls, **qwargs):
         if len(cls.search(**qwargs)) != 0:
             return False
         obj = qwargs
-        new_cls = type(cls.__name__, (Table_Engine,), obj)
+        new_cls = type(cls.__name__, (Table,), obj)
         new_cls.save()
 
     @classmethod
     def add(cls, **qwargs):
         obj = qwargs
-        new_cls = type(cls.__name__, (Table_Engine,), obj)
+        new_cls = type(cls.__name__, (Table,), obj)
         new_cls.save()
 
     @classmethod
     def execute(cls, execut: str):
         conn = sqlite3.connect(db_settings.path)
         cur = conn.cursor()
         cur.execute(execut)
@@ -119,25 +120,21 @@
         request = f'UPDATE {cls.__name__} SET'
         for atr, val in qwargs.items():
             request+=cls.__check_type__(atr, val) + ','
         request = request[:-1] + ' WHERE'
         flag = False
         for atr, val in cls.__dict__.items():
             if not atr.startswith('__') and val != None:
-                request+=cls.__check_type__(atr, val) + 'AND'
+                request+=cls.__check_type__(atr, val) + ' AND'
                 flag = True
         if flag: request = request[:-4]
         conn = sqlite3.connect(db_settings.path)
         cur = conn.cursor()
         cur.execute(request)
         conn.commit()
         return True
     
     def __check_type__(atr, val):
         if type(val) == str: 
             return f' [{atr}] = "{val}"'
         else:
-            return f' [{atr}] = {val}'
-
-class db_settings:
-    path = 'database.db'
-    debug = False # добавить возможность с дебагом
+            return f' [{atr}] = {val}'
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bs_orm-0.8.6.post20230615/bs_orm/Requests.py` & `bs_orm-0.8.7.post20230615/bs_orm/Requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 from .DataTypes import *
 import sqlite3
 import os
 import datetime
-
+from . import db_settings
 
 class empty:
     pass
 
 
-class db_settings:
-    path = 'database.db'
-    models = 0
-
-
 def for_size(content, request):
     try:
         if content.size:
             request += f'({content.size})'
         return ['ok', request]
     except Exception as ex:
         return ['error', ex]
@@ -276,9 +271,7 @@
     with open(f'./migrations/{fileName}.py', 'w') as f:
         f.write(textFromPattern)
 
     cur.execute(f'INSERT INTO migrations (filename) VALUES({fileName})')
     cur.executescript(upgrade)
     conn.commit()
     conn.close()
-
-    # debugging
```

