# Comparing `tmp/bs_orm-0.8.8.post20230615.tar.gz` & `tmp/bs_orm-0.8.9.post20230615.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_orm-0.8.8.post20230615.tar", last modified: Thu Jun 15 00:41:29 2023, max compression
+gzip compressed data, was "bs_orm-0.8.9.post20230615.tar", last modified: Thu Jun 15 01:07:05 2023, max compression
```

## Comparing `bs_orm-0.8.8.post20230615.tar` & `bs_orm-0.8.9.post20230615.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 00:41:29.440976 bs_orm-0.8.8.post20230615/
--rw-rw-rw-   0        0        0      115 2023-06-15 00:41:29.440976 bs_orm-0.8.8.post20230615/PKG-INFO
--rw-rw-rw-   0        0        0     2557 2023-06-14 21:11:33.000000 bs_orm-0.8.8.post20230615/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 00:41:29.426326 bs_orm-0.8.8.post20230615/bs_orm/
--rw-rw-rw-   0        0        0     4821 2023-06-15 00:39:00.000000 bs_orm-0.8.8.post20230615/bs_orm/DataTypes.py
--rw-rw-rw-   0        0        0    10040 2023-06-15 00:31:18.000000 bs_orm-0.8.8.post20230615/bs_orm/Requests.py
--rw-rw-rw-   0        0        0        0 2023-06-14 21:11:33.000000 bs_orm-0.8.8.post20230615/bs_orm/__init__.py
--rw-rw-rw-   0        0        0       32 2023-06-15 00:01:44.000000 bs_orm-0.8.8.post20230615/bs_orm/db_settings.py
-drwxrwxrwx   0        0        0        0 2023-06-15 00:41:29.438974 bs_orm-0.8.8.post20230615/bs_orm.egg-info/
--rw-rw-rw-   0        0        0      115 2023-06-15 00:41:29.000000 bs_orm-0.8.8.post20230615/bs_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-06-15 00:41:29.000000 bs_orm-0.8.8.post20230615/bs_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 00:41:29.000000 bs_orm-0.8.8.post20230615/bs_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-15 00:41:29.000000 bs_orm-0.8.8.post20230615/bs_orm.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-15 00:41:29.000000 bs_orm-0.8.8.post20230615/bs_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       51 2023-06-15 00:41:29.442563 bs_orm-0.8.8.post20230615/setup.cfg
--rw-rw-rw-   0        0        0      286 2023-06-15 00:41:23.000000 bs_orm-0.8.8.post20230615/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:07:05.165182 bs_orm-0.8.9.post20230615/
+-rw-rw-rw-   0        0        0      115 2023-06-15 01:07:05.165182 bs_orm-0.8.9.post20230615/PKG-INFO
+-rw-rw-rw-   0        0        0     2557 2023-06-14 21:11:33.000000 bs_orm-0.8.9.post20230615/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 01:07:05.155654 bs_orm-0.8.9.post20230615/bs_orm/
+-rw-rw-rw-   0        0        0     4887 2023-06-15 00:59:59.000000 bs_orm-0.8.9.post20230615/bs_orm/DataTypes.py
+-rw-rw-rw-   0        0        0    10040 2023-06-15 00:31:18.000000 bs_orm-0.8.9.post20230615/bs_orm/Requests.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:11:33.000000 bs_orm-0.8.9.post20230615/bs_orm/__init__.py
+-rw-rw-rw-   0        0        0       32 2023-06-15 00:01:44.000000 bs_orm-0.8.9.post20230615/bs_orm/db_settings.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:07:05.164174 bs_orm-0.8.9.post20230615/bs_orm.egg-info/
+-rw-rw-rw-   0        0        0      115 2023-06-15 01:07:05.000000 bs_orm-0.8.9.post20230615/bs_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-06-15 01:07:05.000000 bs_orm-0.8.9.post20230615/bs_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 01:07:05.000000 bs_orm-0.8.9.post20230615/bs_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 01:07:05.000000 bs_orm-0.8.9.post20230615/bs_orm.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-15 01:07:05.000000 bs_orm-0.8.9.post20230615/bs_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       51 2023-06-15 01:07:05.167183 bs_orm-0.8.9.post20230615/setup.cfg
+-rw-rw-rw-   0        0        0      286 2023-06-15 01:06:57.000000 bs_orm-0.8.9.post20230615/setup.py
```

### Comparing `bs_orm-0.8.8.post20230615/README.md` & `bs_orm-0.8.9.post20230615/README.md`

 * *Files identical despite different names*

### Comparing `bs_orm-0.8.8.post20230615/bs_orm/DataTypes.py` & `bs_orm-0.8.9.post20230615/bs_orm/DataTypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,9 +139,11 @@
         cur.executescript(request)
         conn.commit()
         return True
     
     def __check_type__(atr, val):
         if type(val) == str: 
             return f' [{atr}] = "{val}"'
+        elif val == None:
+            return f' [{atr}] = NULL'
         else:
             return f' [{atr}] = {val}'
```

### Comparing `bs_orm-0.8.8.post20230615/bs_orm/Requests.py` & `bs_orm-0.8.9.post20230615/bs_orm/Requests.py`

 * *Files identical despite different names*

