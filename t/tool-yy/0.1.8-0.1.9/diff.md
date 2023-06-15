# Comparing `tmp/tool-yy-0.1.8.tar.gz` & `tmp/tool-yy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tool-yy-0.1.8.tar", last modified: Thu Jan  2 15:40:12 2020, max compression
+gzip compressed data, was "dist/tool-yy-0.1.9.tar", last modified: Fri Feb 21 07:29:37 2020, max compression
```

## Comparing `tool-yy-0.1.8.tar` & `tool-yy-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 cpx        (501) staff       (20)        0 2020-01-02 15:40:12.000000 tool-yy-0.1.8/
--rw-r--r--   0 cpx        (501) staff       (20)      868 2020-01-02 15:40:12.000000 tool-yy-0.1.8/PKG-INFO
-drwxr-xr-x   0 cpx        (501) staff       (20)        0 2020-01-02 15:40:12.000000 tool-yy-0.1.8/test/
--rw-r--r--   0 cpx        (501) staff       (20)      550 2019-08-28 06:36:54.000000 tool-yy-0.1.8/test/helper_test.py
--rw-r--r--   0 cpx        (501) staff       (20)       22 2019-04-24 01:46:27.000000 tool-yy-0.1.8/test/__init__.py
--rw-r--r--   0 cpx        (501) staff       (20)      228 2019-09-23 05:09:47.000000 tool-yy-0.1.8/test/settings.py
-drwxr-xr-x   0 cpx        (501) staff       (20)        0 2020-01-02 15:40:12.000000 tool-yy-0.1.8/tool_yy/
-drwxr-xr-x   0 cpx        (501) staff       (20)        0 2020-01-02 15:40:12.000000 tool-yy-0.1.8/tool_yy/config/
--rwxr-xr-x   0 cpx        (501) staff       (20)      214 2019-04-24 01:58:44.000000 tool-yy-0.1.8/tool_yy/config/dbconfig.py
--rwxr-xr-x   0 cpx        (501) staff       (20)        0 2019-04-09 05:31:03.000000 tool-yy-0.1.8/tool_yy/config/__init__.py
--rw-r--r--   0 cpx        (501) staff       (20)       18 2019-04-10 05:12:40.000000 tool-yy-0.1.8/tool_yy/config/settings.py
--rwxr-xr-x   0 cpx        (501) staff       (20)      150 2019-04-09 05:31:03.000000 tool-yy-0.1.8/tool_yy/config/phoenix_db_config.py
--rw-r--r--   0 cpx        (501) staff       (20)      125 2019-07-25 09:29:53.000000 tool-yy-0.1.8/tool_yy/__init__.py
--rw-r--r--   0 cpx        (501) staff       (20)      572 2020-01-02 15:39:28.000000 tool-yy-0.1.8/tool_yy/__about__.py
-drwxr-xr-x   0 cpx        (501) staff       (20)        0 2020-01-02 15:40:12.000000 tool-yy-0.1.8/tool_yy/lib/
--rwxr-xr-x   0 cpx        (501) staff       (20)    12612 2020-01-02 15:37:43.000000 tool-yy-0.1.8/tool_yy/lib/db.py
--rwxr-xr-x   0 cpx        (501) staff       (20)    13205 2019-07-25 06:12:13.000000 tool-yy-0.1.8/tool_yy/lib/phoenix_db.py
--rw-r--r--   0 cpx        (501) staff       (20)      853 2019-08-28 03:19:09.000000 tool-yy-0.1.8/tool_yy/lib/thread.py
--rw-r--r--   0 cpx        (501) staff       (20)     9447 2019-07-25 07:15:32.000000 tool-yy-0.1.8/tool_yy/lib/config.py
--rw-r--r--   0 cpx        (501) staff       (20)      915 2019-07-25 06:25:16.000000 tool-yy-0.1.8/tool_yy/lib/helper_context.py
--rw-r--r--   0 cpx        (501) staff       (20)       22 2019-04-24 01:50:08.000000 tool-yy-0.1.8/tool_yy/lib/__init__.py
--rw-r--r--   0 cpx        (501) staff       (20)      297 2019-09-21 16:17:50.000000 tool-yy-0.1.8/tool_yy/lib/helper.py
--rw-r--r--   0 cpx        (501) staff       (20)     2987 2019-07-25 06:37:19.000000 tool-yy-0.1.8/tool_yy/lib/_compat.py
--rw-r--r--   0 cpx        (501) staff       (20)     2085 2019-12-26 06:23:23.000000 tool-yy-0.1.8/tool_yy/lib/helper_config.py
--rw-r--r--   0 cpx        (501) staff       (20)     2286 2019-07-25 06:32:02.000000 tool-yy-0.1.8/tool_yy/lib/json.py
--rwxr-xr-x   0 cpx        (501) staff       (20)    14724 2019-11-22 01:28:25.000000 tool-yy-0.1.8/tool_yy/lib/function.py
--rw-r--r--   0 cpx        (501) staff       (20)     1221 2019-12-26 03:52:12.000000 tool-yy-0.1.8/README.md
--rw-r--r--   0 cpx        (501) staff       (20)     1191 2019-07-25 08:00:04.000000 tool-yy-0.1.8/setup.py
--rw-r--r--   0 cpx        (501) staff       (20)       38 2020-01-02 15:40:12.000000 tool-yy-0.1.8/setup.cfg
-drwxr-xr-x   0 cpx        (501) staff       (20)        0 2020-01-02 15:40:12.000000 tool-yy-0.1.8/tool_yy.egg-info/
--rw-r--r--   0 cpx        (501) staff       (20)      868 2020-01-02 15:40:12.000000 tool-yy-0.1.8/tool_yy.egg-info/PKG-INFO
--rw-r--r--   0 cpx        (501) staff       (20)      644 2020-01-02 15:40:12.000000 tool-yy-0.1.8/tool_yy.egg-info/SOURCES.txt
--rw-r--r--   0 cpx        (501) staff       (20)       97 2020-01-02 15:40:12.000000 tool-yy-0.1.8/tool_yy.egg-info/requires.txt
--rw-r--r--   0 cpx        (501) staff       (20)       13 2020-01-02 15:40:12.000000 tool-yy-0.1.8/tool_yy.egg-info/top_level.txt
--rw-r--r--   0 cpx        (501) staff       (20)        1 2020-01-02 15:40:12.000000 tool-yy-0.1.8/tool_yy.egg-info/dependency_links.txt
+drwxr-xr-x   0 cpx        (501) staff       (20)        0 2020-02-21 07:29:37.000000 tool-yy-0.1.9/
+-rw-r--r--   0 cpx        (501) staff       (20)      868 2020-02-21 07:29:37.000000 tool-yy-0.1.9/PKG-INFO
+drwxr-xr-x   0 cpx        (501) staff       (20)        0 2020-02-21 07:29:37.000000 tool-yy-0.1.9/test/
+-rw-r--r--   0 cpx        (501) staff       (20)      550 2019-08-28 06:36:54.000000 tool-yy-0.1.9/test/helper_test.py
+-rw-r--r--   0 cpx        (501) staff       (20)       22 2019-04-24 01:46:27.000000 tool-yy-0.1.9/test/__init__.py
+-rw-r--r--   0 cpx        (501) staff       (20)      228 2019-09-23 05:09:47.000000 tool-yy-0.1.9/test/settings.py
+drwxr-xr-x   0 cpx        (501) staff       (20)        0 2020-02-21 07:29:37.000000 tool-yy-0.1.9/tool_yy/
+drwxr-xr-x   0 cpx        (501) staff       (20)        0 2020-02-21 07:29:37.000000 tool-yy-0.1.9/tool_yy/config/
+-rwxr-xr-x   0 cpx        (501) staff       (20)      214 2019-04-24 01:58:44.000000 tool-yy-0.1.9/tool_yy/config/dbconfig.py
+-rwxr-xr-x   0 cpx        (501) staff       (20)        0 2019-04-09 05:31:03.000000 tool-yy-0.1.9/tool_yy/config/__init__.py
+-rw-r--r--   0 cpx        (501) staff       (20)       18 2019-04-10 05:12:40.000000 tool-yy-0.1.9/tool_yy/config/settings.py
+-rwxr-xr-x   0 cpx        (501) staff       (20)      150 2019-04-09 05:31:03.000000 tool-yy-0.1.9/tool_yy/config/phoenix_db_config.py
+-rw-r--r--   0 cpx        (501) staff       (20)      125 2019-07-25 09:29:53.000000 tool-yy-0.1.9/tool_yy/__init__.py
+-rw-r--r--   0 cpx        (501) staff       (20)      572 2020-02-21 07:22:38.000000 tool-yy-0.1.9/tool_yy/__about__.py
+drwxr-xr-x   0 cpx        (501) staff       (20)        0 2020-02-21 07:29:37.000000 tool-yy-0.1.9/tool_yy/lib/
+-rwxr-xr-x   0 cpx        (501) staff       (20)    12830 2020-02-21 07:27:56.000000 tool-yy-0.1.9/tool_yy/lib/db.py
+-rwxr-xr-x   0 cpx        (501) staff       (20)    13205 2019-07-25 06:12:13.000000 tool-yy-0.1.9/tool_yy/lib/phoenix_db.py
+-rw-r--r--   0 cpx        (501) staff       (20)      853 2019-08-28 03:19:09.000000 tool-yy-0.1.9/tool_yy/lib/thread.py
+-rw-r--r--   0 cpx        (501) staff       (20)     9447 2019-07-25 07:15:32.000000 tool-yy-0.1.9/tool_yy/lib/config.py
+-rw-r--r--   0 cpx        (501) staff       (20)      915 2019-07-25 06:25:16.000000 tool-yy-0.1.9/tool_yy/lib/helper_context.py
+-rw-r--r--   0 cpx        (501) staff       (20)       22 2019-04-24 01:50:08.000000 tool-yy-0.1.9/tool_yy/lib/__init__.py
+-rw-r--r--   0 cpx        (501) staff       (20)      297 2019-09-21 16:17:50.000000 tool-yy-0.1.9/tool_yy/lib/helper.py
+-rw-r--r--   0 cpx        (501) staff       (20)     2987 2019-07-25 06:37:19.000000 tool-yy-0.1.9/tool_yy/lib/_compat.py
+-rw-r--r--   0 cpx        (501) staff       (20)     2085 2019-12-26 06:23:23.000000 tool-yy-0.1.9/tool_yy/lib/helper_config.py
+-rw-r--r--   0 cpx        (501) staff       (20)     2286 2019-07-25 06:32:02.000000 tool-yy-0.1.9/tool_yy/lib/json.py
+-rwxr-xr-x   0 cpx        (501) staff       (20)    14724 2019-11-22 01:28:25.000000 tool-yy-0.1.9/tool_yy/lib/function.py
+-rw-r--r--   0 cpx        (501) staff       (20)     1221 2019-12-26 03:52:12.000000 tool-yy-0.1.9/README.md
+-rw-r--r--   0 cpx        (501) staff       (20)     1191 2019-07-25 08:00:04.000000 tool-yy-0.1.9/setup.py
+-rw-r--r--   0 cpx        (501) staff       (20)       38 2020-02-21 07:29:37.000000 tool-yy-0.1.9/setup.cfg
+drwxr-xr-x   0 cpx        (501) staff       (20)        0 2020-02-21 07:29:37.000000 tool-yy-0.1.9/tool_yy.egg-info/
+-rw-r--r--   0 cpx        (501) staff       (20)      868 2020-02-21 07:29:37.000000 tool-yy-0.1.9/tool_yy.egg-info/PKG-INFO
+-rw-r--r--   0 cpx        (501) staff       (20)      644 2020-02-21 07:29:37.000000 tool-yy-0.1.9/tool_yy.egg-info/SOURCES.txt
+-rw-r--r--   0 cpx        (501) staff       (20)       97 2020-02-21 07:29:37.000000 tool-yy-0.1.9/tool_yy.egg-info/requires.txt
+-rw-r--r--   0 cpx        (501) staff       (20)       13 2020-02-21 07:29:37.000000 tool-yy-0.1.9/tool_yy.egg-info/top_level.txt
+-rw-r--r--   0 cpx        (501) staff       (20)        1 2020-02-21 07:29:37.000000 tool-yy-0.1.9/tool_yy.egg-info/dependency_links.txt
```

### Comparing `tool-yy-0.1.8/PKG-INFO` & `tool-yy-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tool-yy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Util tools, designed by yy
 Home-page: https://github.com/guaidashu/python3_tool_myself
 Author: guaidashu
 Author-email: song42960@gmail.com
 License: MIT
 Description: 
         tool-yy
```

### Comparing `tool-yy-0.1.8/test/helper_test.py` & `tool-yy-0.1.9/test/helper_test.py`

 * *Files identical despite different names*

### Comparing `tool-yy-0.1.8/tool_yy/__about__.py` & `tool-yy-0.1.9/tool_yy/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Create by yy on 2019-07-25
 """
 
 __title__ = 'tool-yy'
 __description__ = 'Util tools, designed by yy'
 __url__ = 'https://github.com/guaidashu/python3_tool_myself'
-__version_info__ = ('0', '1', '8')
+__version_info__ = ('0', '1', '9')
 __version__ = '.'.join(__version_info__)
 __author__ = 'guaidashu'
 __author_email__ = 'song42960@gmail.com'
 __maintainer__ = 'YY blog'
 __license__ = 'MIT'
 __copyright__ = '(c) 2019 by guaidashu'
 __install_requires__ = [
```

### Comparing `tool-yy-0.1.8/tool_yy/lib/db.py` & `tool-yy-0.1.9/tool_yy/lib/db.py`

 * *Files 5% similar despite different names*

```diff
@@ -286,15 +286,16 @@
             sql = sql + s
         except:
             pass
         if is_close_db:
             self.closeDB()
         return sql
 
-    def getInsertSql(self, data, table, is_close_db=False, table_columns=False, table_auto_increment=False):
+    def getInsertSql(self, data, table, is_close_db=False, table_columns=False, table_auto_increment=False,
+                     ignore_column_type=None):
         # 构造插入查询语句，此函数传入参数data必须为dict()类型
         s = "insert into " + self.table_prefix + table + "("
         columns = ""
         value = ""
         # get table's columns name
         table_sql = {
             "table": "information_schema.columns",
@@ -304,19 +305,24 @@
         }
         if not table_columns:
             table_columns = self.getColumns(table_sql)
         table_sql['condition'].append("and EXTRA like '%auto_increment%'")
         if not table_auto_increment:
             table_auto_increment = self.getColumns(table_sql)
         table_columns_dict = dict()
-        str_dict = {"text": "text", "varchar": "varchar", "longtext": "longtext", "datetime": "datetime",
+        str_dict = {"text": "text", "varchar": "varchar", "longtext": "longtext",
                     "char": "char"}
         ignore_dict = {
-            "timestamp": "timestamp"
+            "timestamp": "timestamp",
+            "datetime": "datetime",
         }
+        # merge two ignore_dict
+        if ignore_column_type:
+            ignore_dict = ignore_dict.copy()
+            ignore_dict.update(ignore_column_type)
         # int_dict = {"int": "int", "bigint": "bigint", "decimal": "decimal", "double": "double", "float": "float"}
         try:
             for v in table_columns:
                 table_columns_dict[v[0]] = v[1]
         except:
             pass
         length = len(data)
```

### Comparing `tool-yy-0.1.8/tool_yy/lib/phoenix_db.py` & `tool-yy-0.1.9/tool_yy/lib/phoenix_db.py`

 * *Files identical despite different names*

### Comparing `tool-yy-0.1.8/tool_yy/lib/thread.py` & `tool-yy-0.1.9/tool_yy/lib/thread.py`

 * *Files identical despite different names*

### Comparing `tool-yy-0.1.8/tool_yy/lib/config.py` & `tool-yy-0.1.9/tool_yy/lib/config.py`

 * *Files identical despite different names*

### Comparing `tool-yy-0.1.8/tool_yy/lib/helper_context.py` & `tool-yy-0.1.9/tool_yy/lib/helper_context.py`

 * *Files identical despite different names*

### Comparing `tool-yy-0.1.8/tool_yy/lib/_compat.py` & `tool-yy-0.1.9/tool_yy/lib/_compat.py`

 * *Files identical despite different names*

### Comparing `tool-yy-0.1.8/tool_yy/lib/helper_config.py` & `tool-yy-0.1.9/tool_yy/lib/helper_config.py`

 * *Files identical despite different names*

### Comparing `tool-yy-0.1.8/tool_yy/lib/json.py` & `tool-yy-0.1.9/tool_yy/lib/json.py`

 * *Files identical despite different names*

### Comparing `tool-yy-0.1.8/tool_yy/lib/function.py` & `tool-yy-0.1.9/tool_yy/lib/function.py`

 * *Files identical despite different names*

### Comparing `tool-yy-0.1.8/README.md` & `tool-yy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `tool-yy-0.1.8/setup.py` & `tool-yy-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `tool-yy-0.1.8/tool_yy.egg-info/PKG-INFO` & `tool-yy-0.1.9/tool_yy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tool-yy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Util tools, designed by yy
 Home-page: https://github.com/guaidashu/python3_tool_myself
 Author: guaidashu
 Author-email: song42960@gmail.com
 License: MIT
 Description: 
         tool-yy
```

### Comparing `tool-yy-0.1.8/tool_yy.egg-info/SOURCES.txt` & `tool-yy-0.1.9/tool_yy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

