# Comparing `tmp/bs_orm-0.8.3.post20230615.tar.gz` & `tmp/bs_orm-0.8.4.post20230615.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_orm-0.8.3.post20230615.tar", last modified: Wed Jun 14 22:30:07 2023, max compression
+gzip compressed data, was "bs_orm-0.8.4.post20230615.tar", last modified: Wed Jun 14 22:58:36 2023, max compression
```

## Comparing `bs_orm-0.8.3.post20230615.tar` & `bs_orm-0.8.4.post20230615.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 22:30:07.154329 bs_orm-0.8.3.post20230615/
--rw-rw-rw-   0        0        0      115 2023-06-14 22:30:07.154329 bs_orm-0.8.3.post20230615/PKG-INFO
--rw-rw-rw-   0        0        0     2557 2023-06-14 21:11:33.000000 bs_orm-0.8.3.post20230615/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 22:30:07.144275 bs_orm-0.8.3.post20230615/bs_orm/
--rw-rw-rw-   0        0        0     3281 2023-06-14 21:33:52.000000 bs_orm-0.8.3.post20230615/bs_orm/DataTypes.py
--rw-rw-rw-   0        0        0     9283 2023-06-14 22:24:23.000000 bs_orm-0.8.3.post20230615/bs_orm/Requests.py
--rw-rw-rw-   0        0        0        0 2023-06-14 21:11:33.000000 bs_orm-0.8.3.post20230615/bs_orm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:30:07.152329 bs_orm-0.8.3.post20230615/bs_orm.egg-info/
--rw-rw-rw-   0        0        0      115 2023-06-14 22:30:07.000000 bs_orm-0.8.3.post20230615/bs_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-06-14 22:30:07.000000 bs_orm-0.8.3.post20230615/bs_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 22:30:07.000000 bs_orm-0.8.3.post20230615/bs_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-14 22:30:07.000000 bs_orm-0.8.3.post20230615/bs_orm.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-14 22:30:07.000000 bs_orm-0.8.3.post20230615/bs_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       51 2023-06-14 22:30:07.155329 bs_orm-0.8.3.post20230615/setup.cfg
--rw-rw-rw-   0        0        0      286 2023-06-14 22:30:01.000000 bs_orm-0.8.3.post20230615/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:58:36.874572 bs_orm-0.8.4.post20230615/
+-rw-rw-rw-   0        0        0      115 2023-06-14 22:58:36.875578 bs_orm-0.8.4.post20230615/PKG-INFO
+-rw-rw-rw-   0        0        0     2557 2023-06-14 21:11:33.000000 bs_orm-0.8.4.post20230615/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 22:58:36.847978 bs_orm-0.8.4.post20230615/bs_orm/
+-rw-rw-rw-   0        0        0     3870 2023-06-14 22:57:17.000000 bs_orm-0.8.4.post20230615/bs_orm/DataTypes.py
+-rw-rw-rw-   0        0        0     9283 2023-06-14 22:24:23.000000 bs_orm-0.8.4.post20230615/bs_orm/Requests.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:11:33.000000 bs_orm-0.8.4.post20230615/bs_orm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:58:36.873571 bs_orm-0.8.4.post20230615/bs_orm.egg-info/
+-rw-rw-rw-   0        0        0      115 2023-06-14 22:58:36.000000 bs_orm-0.8.4.post20230615/bs_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-06-14 22:58:36.000000 bs_orm-0.8.4.post20230615/bs_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 22:58:36.000000 bs_orm-0.8.4.post20230615/bs_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-14 22:58:36.000000 bs_orm-0.8.4.post20230615/bs_orm.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-14 22:58:36.000000 bs_orm-0.8.4.post20230615/bs_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       51 2023-06-14 22:58:36.876611 bs_orm-0.8.4.post20230615/setup.cfg
+-rw-rw-rw-   0        0        0      286 2023-06-14 22:58:31.000000 bs_orm-0.8.4.post20230615/setup.py
```

### Comparing `bs_orm-0.8.3.post20230615/README.md` & `bs_orm-0.8.4.post20230615/README.md`

 * *Files identical despite different names*

### Comparing `bs_orm-0.8.3.post20230615/bs_orm/DataTypes.py` & `bs_orm-0.8.4.post20230615/bs_orm/DataTypes.py`

 * *Files 19% similar despite different names*

```diff
@@ -38,18 +38,23 @@
 
 class Table_Engine:
     def __init__(self, **qwargs):
         for k, v in qwargs.items():
             self.__all__.__setattr__(k, v)
     
     @classmethod
-    def read(cls):
+    def search(cls, **qwargs):
         conn = sqlite3.connect(db_settings.path)
         cur = conn.cursor()
         request  = "SELECT * FROM " + cls.__name__ # fix this line
+        if qwargs != {}:
+            request+=' WHERE'
+            for atr, val in qwargs.items():
+                request+=f' {atr}={val} AND'
+            request = request[:-4]
         cur.execute(request)
         conn.commit()
         values = cur.fetchall()
         returned = []
         obj = {}
         for line in values:
             column_names = iter(cur.description)
@@ -84,14 +89,28 @@
     @classmethod
     def create(cls, **qwargs):
         obj = qwargs
         new_cls = type(cls.__name__, (Table_Engine,), obj)
         return new_cls
     
     @classmethod
+    def add_if_not_exist(cls, **qwargs):
+        if len(cls.search(**qwargs)) != 0:
+            return False
+        obj = qwargs
+        new_cls = type(cls.__name__, (Table_Engine,), obj)
+        return new_cls
+
+    @classmethod
+    def add(cls, **qwargs):
+        obj = qwargs
+        new_cls = type(cls.__name__, (Table_Engine,), obj)
+        new_cls.save()
+
+    @classmethod
     def execute(cls, execut: str):
         conn = sqlite3.connect(db_settings.path)
         cur = conn.cursor()
         cur.execute(execut)
         conn.commit()
         return True
```

### Comparing `bs_orm-0.8.3.post20230615/bs_orm/Requests.py` & `bs_orm-0.8.4.post20230615/bs_orm/Requests.py`

 * *Files identical despite different names*

