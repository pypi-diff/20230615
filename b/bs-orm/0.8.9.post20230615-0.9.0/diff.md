# Comparing `tmp/bs_orm-0.8.9.post20230615.tar.gz` & `tmp/bs_orm-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_orm-0.8.9.post20230615.tar", last modified: Thu Jun 15 01:07:05 2023, max compression
+gzip compressed data, was "bs_orm-0.9.0.tar", last modified: Thu Jun 15 01:35:15 2023, max compression
```

## Comparing `bs_orm-0.8.9.post20230615.tar` & `bs_orm-0.9.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 01:07:05.165182 bs_orm-0.8.9.post20230615/
--rw-rw-rw-   0        0        0      115 2023-06-15 01:07:05.165182 bs_orm-0.8.9.post20230615/PKG-INFO
--rw-rw-rw-   0        0        0     2557 2023-06-14 21:11:33.000000 bs_orm-0.8.9.post20230615/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 01:07:05.155654 bs_orm-0.8.9.post20230615/bs_orm/
--rw-rw-rw-   0        0        0     4887 2023-06-15 00:59:59.000000 bs_orm-0.8.9.post20230615/bs_orm/DataTypes.py
--rw-rw-rw-   0        0        0    10040 2023-06-15 00:31:18.000000 bs_orm-0.8.9.post20230615/bs_orm/Requests.py
--rw-rw-rw-   0        0        0        0 2023-06-14 21:11:33.000000 bs_orm-0.8.9.post20230615/bs_orm/__init__.py
--rw-rw-rw-   0        0        0       32 2023-06-15 00:01:44.000000 bs_orm-0.8.9.post20230615/bs_orm/db_settings.py
-drwxrwxrwx   0        0        0        0 2023-06-15 01:07:05.164174 bs_orm-0.8.9.post20230615/bs_orm.egg-info/
--rw-rw-rw-   0        0        0      115 2023-06-15 01:07:05.000000 bs_orm-0.8.9.post20230615/bs_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-06-15 01:07:05.000000 bs_orm-0.8.9.post20230615/bs_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 01:07:05.000000 bs_orm-0.8.9.post20230615/bs_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-15 01:07:05.000000 bs_orm-0.8.9.post20230615/bs_orm.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-15 01:07:05.000000 bs_orm-0.8.9.post20230615/bs_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       51 2023-06-15 01:07:05.167183 bs_orm-0.8.9.post20230615/setup.cfg
--rw-rw-rw-   0        0        0      286 2023-06-15 01:06:57.000000 bs_orm-0.8.9.post20230615/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:35:15.301392 bs_orm-0.9.0/
+-rw-rw-rw-   0        0        0      108 2023-06-15 01:35:15.302604 bs_orm-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2557 2023-06-14 21:11:33.000000 bs_orm-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 01:35:15.292079 bs_orm-0.9.0/bs_orm/
+-rw-rw-rw-   0        0        0     4887 2023-06-15 01:26:56.000000 bs_orm-0.9.0/bs_orm/DataTypes.py
+-rw-rw-rw-   0        0        0    10036 2023-06-15 01:26:11.000000 bs_orm-0.9.0/bs_orm/Requests.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:11:33.000000 bs_orm-0.9.0/bs_orm/__init__.py
+-rw-rw-rw-   0        0        0       32 2023-06-15 00:01:44.000000 bs_orm-0.9.0/bs_orm/db_settings.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:35:15.300381 bs_orm-0.9.0/bs_orm.egg-info/
+-rw-rw-rw-   0        0        0      108 2023-06-15 01:35:15.000000 bs_orm-0.9.0/bs_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-06-15 01:35:15.000000 bs_orm-0.9.0/bs_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 01:35:15.000000 bs_orm-0.9.0/bs_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 01:35:15.000000 bs_orm-0.9.0/bs_orm.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-15 01:35:15.000000 bs_orm-0.9.0/bs_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 01:35:15.303616 bs_orm-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      292 2023-06-15 01:35:05.000000 bs_orm-0.9.0/setup.py
```

### Comparing `bs_orm-0.8.9.post20230615/README.md` & `bs_orm-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `bs_orm-0.8.9.post20230615/bs_orm/DataTypes.py` & `bs_orm-0.9.0/bs_orm/DataTypes.py`

 * *Files identical despite different names*

### Comparing `bs_orm-0.8.9.post20230615/bs_orm/Requests.py` & `bs_orm-0.9.0/bs_orm/Requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,15 +265,15 @@
         upgrade, [add_list, remove_list, update_list_a, update_list_r])
     downgrade = '\n'
     downgrade = concatenete_data(
         downgrade, [FD_add_list, FD_remove_list, \
                     FD_update_list_a, FD_update_list_r])
 
     textFromPattern = f'''import sqlite3
-from better_orm import db_settings
+from bs_orm import db_settings
 
 def upgrade():
     upgrade_execut = """{upgrade}"""
     conn = sqlite3.connect(db_settings.path)
     cur = conn.cursor()
     cur.executescript(upgrade_execut)
```

