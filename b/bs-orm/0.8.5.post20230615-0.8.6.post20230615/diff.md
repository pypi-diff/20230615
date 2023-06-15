# Comparing `tmp/bs_orm-0.8.5.post20230615.tar.gz` & `tmp/bs_orm-0.8.6.post20230615.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_orm-0.8.5.post20230615.tar", last modified: Wed Jun 14 23:02:48 2023, max compression
+gzip compressed data, was "bs_orm-0.8.6.post20230615.tar", last modified: Wed Jun 14 23:56:02 2023, max compression
```

## Comparing `bs_orm-0.8.5.post20230615.tar` & `bs_orm-0.8.6.post20230615.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 23:02:48.828035 bs_orm-0.8.5.post20230615/
--rw-rw-rw-   0        0        0      115 2023-06-14 23:02:48.828035 bs_orm-0.8.5.post20230615/PKG-INFO
--rw-rw-rw-   0        0        0     2557 2023-06-14 21:11:33.000000 bs_orm-0.8.5.post20230615/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 23:02:48.817517 bs_orm-0.8.5.post20230615/bs_orm/
--rw-rw-rw-   0        0        0     3870 2023-06-14 23:02:33.000000 bs_orm-0.8.5.post20230615/bs_orm/DataTypes.py
--rw-rw-rw-   0        0        0     9283 2023-06-14 22:24:23.000000 bs_orm-0.8.5.post20230615/bs_orm/Requests.py
--rw-rw-rw-   0        0        0        0 2023-06-14 21:11:33.000000 bs_orm-0.8.5.post20230615/bs_orm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:02:48.827036 bs_orm-0.8.5.post20230615/bs_orm.egg-info/
--rw-rw-rw-   0        0        0      115 2023-06-14 23:02:48.000000 bs_orm-0.8.5.post20230615/bs_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-06-14 23:02:48.000000 bs_orm-0.8.5.post20230615/bs_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 23:02:48.000000 bs_orm-0.8.5.post20230615/bs_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-14 23:02:48.000000 bs_orm-0.8.5.post20230615/bs_orm.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-14 23:02:48.000000 bs_orm-0.8.5.post20230615/bs_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       51 2023-06-14 23:02:48.829033 bs_orm-0.8.5.post20230615/setup.cfg
--rw-rw-rw-   0        0        0      286 2023-06-14 23:02:42.000000 bs_orm-0.8.5.post20230615/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:56:02.950685 bs_orm-0.8.6.post20230615/
+-rw-rw-rw-   0        0        0      115 2023-06-14 23:56:02.950685 bs_orm-0.8.6.post20230615/PKG-INFO
+-rw-rw-rw-   0        0        0     2557 2023-06-14 21:11:33.000000 bs_orm-0.8.6.post20230615/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 23:56:02.940160 bs_orm-0.8.6.post20230615/bs_orm/
+-rw-rw-rw-   0        0        0     4727 2023-06-14 23:54:37.000000 bs_orm-0.8.6.post20230615/bs_orm/DataTypes.py
+-rw-rw-rw-   0        0        0     9283 2023-06-14 22:24:23.000000 bs_orm-0.8.6.post20230615/bs_orm/Requests.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:11:33.000000 bs_orm-0.8.6.post20230615/bs_orm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:56:02.948719 bs_orm-0.8.6.post20230615/bs_orm.egg-info/
+-rw-rw-rw-   0        0        0      115 2023-06-14 23:56:02.000000 bs_orm-0.8.6.post20230615/bs_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-06-14 23:56:02.000000 bs_orm-0.8.6.post20230615/bs_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 23:56:02.000000 bs_orm-0.8.6.post20230615/bs_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-14 23:56:02.000000 bs_orm-0.8.6.post20230615/bs_orm.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-14 23:56:02.000000 bs_orm-0.8.6.post20230615/bs_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       51 2023-06-14 23:56:02.951685 bs_orm-0.8.6.post20230615/setup.cfg
+-rw-rw-rw-   0        0        0      286 2023-06-14 23:55:57.000000 bs_orm-0.8.6.post20230615/setup.py
```

### Comparing `bs_orm-0.8.5.post20230615/README.md` & `bs_orm-0.8.6.post20230615/README.md`

 * *Files identical despite different names*

### Comparing `bs_orm-0.8.5.post20230615/bs_orm/DataTypes.py` & `bs_orm-0.8.6.post20230615/bs_orm/DataTypes.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,39 +41,39 @@
         for k, v in qwargs.items():
             self.__all__.__setattr__(k, v)
     
     @classmethod
     def search(cls, **qwargs):
         conn = sqlite3.connect(db_settings.path)
         cur = conn.cursor()
-        request  = "SELECT * FROM " + cls.__name__ # fix this line
+        request  = f'SELECT * FROM [{cls.__name__}]' # fix this line
         if qwargs != {}:
             request+=' WHERE'
             for atr, val in qwargs.items():
-                request+=f' {atr}={val} AND'
+                request+=cls.__check_type__(atr, val) + 'AND'
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
-            returned.append(type(cls.__name__, (), obj))
+            returned.append(type(cls.__name__, (Table_Engine,), obj))
         conn.commit()
         return returned
 
     @classmethod
     def save(cls):
         conn = sqlite3.connect(db_settings.path)
         cur = conn.cursor()
         try:
-            request = 'INSERT INTO '+ cls.__name__ + ' ('
+            request = f'INSERT INTO [{cls.__name__}] ('
             values = 'VALUES ('
             for k, v in cls.__dict__.items():
                 if k not in empty.__dict__.keys():
                     request+=f'{k}, '
                     if v.__class__ == str:
                         values+=f'"{v}", '
                     else:
@@ -109,11 +109,35 @@
     @classmethod
     def execute(cls, execut: str):
         conn = sqlite3.connect(db_settings.path)
         cur = conn.cursor()
         cur.execute(execut)
         conn.commit()
         return True
+    
+    @classmethod
+    def update(cls, **qwargs):
+        request = f'UPDATE {cls.__name__} SET'
+        for atr, val in qwargs.items():
+            request+=cls.__check_type__(atr, val) + ','
+        request = request[:-1] + ' WHERE'
+        flag = False
+        for atr, val in cls.__dict__.items():
+            if not atr.startswith('__') and val != None:
+                request+=cls.__check_type__(atr, val) + 'AND'
+                flag = True
+        if flag: request = request[:-4]
+        conn = sqlite3.connect(db_settings.path)
+        cur = conn.cursor()
+        cur.execute(request)
+        conn.commit()
+        return True
+    
+    def __check_type__(atr, val):
+        if type(val) == str: 
+            return f' [{atr}] = "{val}"'
+        else:
+            return f' [{atr}] = {val}'
 
 class db_settings:
     path = 'database.db'
     debug = False # добавить возможность с дебагом
```

### Comparing `bs_orm-0.8.5.post20230615/bs_orm/Requests.py` & `bs_orm-0.8.6.post20230615/bs_orm/Requests.py`

 * *Files identical despite different names*

