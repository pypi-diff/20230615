# Comparing `tmp/bs_orm-0.8.7.post20230615.tar.gz` & `tmp/bs_orm-0.8.8.post20230615.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_orm-0.8.7.post20230615.tar", last modified: Thu Jun 15 00:14:03 2023, max compression
+gzip compressed data, was "bs_orm-0.8.8.post20230615.tar", last modified: Thu Jun 15 00:41:29 2023, max compression
```

## Comparing `bs_orm-0.8.7.post20230615.tar` & `bs_orm-0.8.8.post20230615.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 00:14:03.194411 bs_orm-0.8.7.post20230615/
--rw-rw-rw-   0        0        0      115 2023-06-15 00:14:03.195411 bs_orm-0.8.7.post20230615/PKG-INFO
--rw-rw-rw-   0        0        0     2557 2023-06-14 21:11:33.000000 bs_orm-0.8.7.post20230615/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 00:14:03.184859 bs_orm-0.8.7.post20230615/bs_orm/
--rw-rw-rw-   0        0        0     4578 2023-06-15 00:13:24.000000 bs_orm-0.8.7.post20230615/bs_orm/DataTypes.py
--rw-rw-rw-   0        0        0     9223 2023-06-15 00:04:30.000000 bs_orm-0.8.7.post20230615/bs_orm/Requests.py
--rw-rw-rw-   0        0        0        0 2023-06-14 21:11:33.000000 bs_orm-0.8.7.post20230615/bs_orm/__init__.py
--rw-rw-rw-   0        0        0       32 2023-06-15 00:01:44.000000 bs_orm-0.8.7.post20230615/bs_orm/db_settings.py
-drwxrwxrwx   0        0        0        0 2023-06-15 00:14:03.193405 bs_orm-0.8.7.post20230615/bs_orm.egg-info/
--rw-rw-rw-   0        0        0      115 2023-06-15 00:14:03.000000 bs_orm-0.8.7.post20230615/bs_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-06-15 00:14:03.000000 bs_orm-0.8.7.post20230615/bs_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 00:14:03.000000 bs_orm-0.8.7.post20230615/bs_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-15 00:14:03.000000 bs_orm-0.8.7.post20230615/bs_orm.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-15 00:14:03.000000 bs_orm-0.8.7.post20230615/bs_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       51 2023-06-15 00:14:03.196411 bs_orm-0.8.7.post20230615/setup.cfg
--rw-rw-rw-   0        0        0      286 2023-06-15 00:13:56.000000 bs_orm-0.8.7.post20230615/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 00:41:29.440976 bs_orm-0.8.8.post20230615/
+-rw-rw-rw-   0        0        0      115 2023-06-15 00:41:29.440976 bs_orm-0.8.8.post20230615/PKG-INFO
+-rw-rw-rw-   0        0        0     2557 2023-06-14 21:11:33.000000 bs_orm-0.8.8.post20230615/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 00:41:29.426326 bs_orm-0.8.8.post20230615/bs_orm/
+-rw-rw-rw-   0        0        0     4821 2023-06-15 00:39:00.000000 bs_orm-0.8.8.post20230615/bs_orm/DataTypes.py
+-rw-rw-rw-   0        0        0    10040 2023-06-15 00:31:18.000000 bs_orm-0.8.8.post20230615/bs_orm/Requests.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:11:33.000000 bs_orm-0.8.8.post20230615/bs_orm/__init__.py
+-rw-rw-rw-   0        0        0       32 2023-06-15 00:01:44.000000 bs_orm-0.8.8.post20230615/bs_orm/db_settings.py
+drwxrwxrwx   0        0        0        0 2023-06-15 00:41:29.438974 bs_orm-0.8.8.post20230615/bs_orm.egg-info/
+-rw-rw-rw-   0        0        0      115 2023-06-15 00:41:29.000000 bs_orm-0.8.8.post20230615/bs_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-06-15 00:41:29.000000 bs_orm-0.8.8.post20230615/bs_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 00:41:29.000000 bs_orm-0.8.8.post20230615/bs_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 00:41:29.000000 bs_orm-0.8.8.post20230615/bs_orm.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-15 00:41:29.000000 bs_orm-0.8.8.post20230615/bs_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       51 2023-06-15 00:41:29.442563 bs_orm-0.8.8.post20230615/setup.cfg
+-rw-rw-rw-   0        0        0      286 2023-06-15 00:41:23.000000 bs_orm-0.8.8.post20230615/setup.py
```

### Comparing `bs_orm-0.8.7.post20230615/README.md` & `bs_orm-0.8.8.post20230615/README.md`

 * *Files identical despite different names*

### Comparing `bs_orm-0.8.7.post20230615/bs_orm/DataTypes.py` & `bs_orm-0.8.8.post20230615/bs_orm/DataTypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,28 +112,35 @@
         conn = sqlite3.connect(db_settings.path)
         cur = conn.cursor()
         cur.execute(execut)
         conn.commit()
         return True
     
     @classmethod
-    def update(cls, **qwargs):
-        request = f'UPDATE {cls.__name__} SET'
-        for atr, val in qwargs.items():
-            request+=cls.__check_type__(atr, val) + ','
-        request = request[:-1] + ' WHERE'
-        flag = False
-        for atr, val in cls.__dict__.items():
-            if not atr.startswith('__') and val != None:
-                request+=cls.__check_type__(atr, val) + ' AND'
-                flag = True
-        if flag: request = request[:-4]
+    def update(cls, objects:list = None, **qwargs):
+        request = ''
+        if objects != None:
+            cls_s = objects
+        else:
+            cls_s = [cls]
+        for cls in cls_s:
+            request += f'UPDATE {cls.__name__} SET'
+            for atr, val in qwargs.items():
+                request+=cls.__check_type__(atr, val) + ','
+            request = request[:-1] + ' WHERE'
+            flag = False
+            for atr, val in cls.__dict__.items():
+                if not atr.startswith('__') and val != None:
+                    request+=cls.__check_type__(atr, val) + ' AND'
+                    flag = True
+            if flag: request = request[:-4]
+            request+'\n'
         conn = sqlite3.connect(db_settings.path)
         cur = conn.cursor()
-        cur.execute(request)
+        cur.executescript(request)
         conn.commit()
         return True
     
     def __check_type__(atr, val):
         if type(val) == str: 
             return f' [{atr}] = "{val}"'
         else:
```

### Comparing `bs_orm-0.8.7.post20230615/bs_orm/Requests.py` & `bs_orm-0.8.8.post20230615/bs_orm/Requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -157,14 +157,35 @@
                 conn.commit()
                 conn.close()
                 return True
     except Exception as ex:
         raise Exception(
             f'well congratulations your father goes fucking you with a chair on the head with these words: {ex}')
 
+def update(cls_s, **qwargs):
+        request = ''
+        if type(cls_s) != list:
+            cls_s = [cls_s]
+        for cls in cls_s:
+            request += f'UPDATE {cls.__name__} SET'
+            for atr, val in qwargs.items():
+                request+=cls.__check_type__(atr, val) + ','
+            request = request[:-1] + ' WHERE'
+            flag = False
+            for atr, val in cls.__dict__.items():
+                if not atr.startswith('__') and val != None:
+                    request+=cls.__check_type__(atr, val) + ' AND'
+                    flag = True
+            if flag: request = request[:-4]
+            request+'\n'
+        conn = sqlite3.connect(db_settings.path)
+        cur = conn.cursor()
+        cur.executescript(request)
+        conn.commit()
+        return True
 
 def migrate():
     conn = sqlite3.connect(db_settings.path)
     cur = conn.cursor()
     cur.execute('SELECT sql FROM sqlite_master WHERE type="table"')
     old_data = ';\n'.join([x[0] for x in cur.fetchall()])
     new_data = create_execute()
```

