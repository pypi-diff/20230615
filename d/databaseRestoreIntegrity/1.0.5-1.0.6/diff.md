# Comparing `tmp/databaseRestoreIntegrity-1.0.5.tar.gz` & `tmp/databaseRestoreIntegrity-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databaseRestoreIntegrity-1.0.5.tar", last modified: Wed Jun  7 15:03:06 2023, max compression
+gzip compressed data, was "databaseRestoreIntegrity-1.0.6.tar", last modified: Thu Jun 15 09:06:19 2023, max compression
```

## Comparing `databaseRestoreIntegrity-1.0.5.tar` & `databaseRestoreIntegrity-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-07 15:03:06.273056 databaseRestoreIntegrity-1.0.5/
--rw-r--r--   0 mhasan     (502) staff       (20)     1073 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.5/LICENSE.txt
--rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.5/MANIFEST.in
--rw-r--r--   0 mhasan     (502) staff       (20)     3651 2023-06-07 15:03:06.273154 databaseRestoreIntegrity-1.0.5/PKG-INFO
--rw-r--r--   0 mhasan     (502) staff       (20)     1959 2023-06-05 09:52:54.000000 databaseRestoreIntegrity-1.0.5/README.md
--rw-r--r--   0 mhasan     (502) staff       (20)       84 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.5/pyproject.toml
--rw-r--r--   0 mhasan     (502) staff       (20)      740 2023-06-07 15:03:06.278064 databaseRestoreIntegrity-1.0.5/setup.cfg
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-07 15:03:06.263358 databaseRestoreIntegrity-1.0.5/src/
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-07 15:03:06.266918 databaseRestoreIntegrity-1.0.5/src/databaseRestoreIntegrity/
--rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.5/src/databaseRestoreIntegrity/__init__.py
--rw-r--r--   0 mhasan     (502) staff       (20)     2970 2023-06-07 12:36:19.000000 databaseRestoreIntegrity-1.0.5/src/databaseRestoreIntegrity/mysql.py
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-07 15:03:06.272654 databaseRestoreIntegrity-1.0.5/src/databaseRestoreIntegrity.egg-info/
--rw-r--r--   0 mhasan     (502) staff       (20)     3651 2023-06-07 15:03:06.000000 databaseRestoreIntegrity-1.0.5/src/databaseRestoreIntegrity.egg-info/PKG-INFO
--rw-r--r--   0 mhasan     (502) staff       (20)      345 2023-06-07 15:03:06.000000 databaseRestoreIntegrity-1.0.5/src/databaseRestoreIntegrity.egg-info/SOURCES.txt
--rw-r--r--   0 mhasan     (502) staff       (20)        1 2023-06-07 15:03:06.000000 databaseRestoreIntegrity-1.0.5/src/databaseRestoreIntegrity.egg-info/dependency_links.txt
--rw-r--r--   0 mhasan     (502) staff       (20)       25 2023-06-07 15:03:06.000000 databaseRestoreIntegrity-1.0.5/src/databaseRestoreIntegrity.egg-info/top_level.txt
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 09:06:19.615181 databaseRestoreIntegrity-1.0.6/
+-rw-r--r--   0 mhasan     (502) staff       (20)     1073 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.6/LICENSE.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.6/MANIFEST.in
+-rw-r--r--   0 mhasan     (502) staff       (20)     3727 2023-06-15 09:06:19.615285 databaseRestoreIntegrity-1.0.6/PKG-INFO
+-rw-r--r--   0 mhasan     (502) staff       (20)     2035 2023-06-08 12:12:36.000000 databaseRestoreIntegrity-1.0.6/README.md
+-rw-r--r--   0 mhasan     (502) staff       (20)       84 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.6/pyproject.toml
+-rw-r--r--   0 mhasan     (502) staff       (20)      740 2023-06-15 09:06:19.622489 databaseRestoreIntegrity-1.0.6/setup.cfg
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 09:06:19.605893 databaseRestoreIntegrity-1.0.6/src/
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 09:06:19.609875 databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity/
+-rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity/__init__.py
+-rw-r--r--   0 mhasan     (502) staff       (20)     2970 2023-06-07 12:36:19.000000 databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity/mysql.py
+-rw-r--r--   0 mhasan     (502) staff       (20)     2873 2023-06-11 12:26:37.000000 databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity/postgres.py
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 09:06:19.614537 databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity.egg-info/
+-rw-r--r--   0 mhasan     (502) staff       (20)     3727 2023-06-15 09:06:19.000000 databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity.egg-info/PKG-INFO
+-rw-r--r--   0 mhasan     (502) staff       (20)      386 2023-06-15 09:06:19.000000 databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity.egg-info/SOURCES.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)        1 2023-06-15 09:06:19.000000 databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity.egg-info/dependency_links.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)       25 2023-06-15 09:06:19.000000 databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity.egg-info/top_level.txt
```

### Comparing `databaseRestoreIntegrity-1.0.5/LICENSE.txt` & `databaseRestoreIntegrity-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `databaseRestoreIntegrity-1.0.5/PKG-INFO` & `databaseRestoreIntegrity-1.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databaseRestoreIntegrity
-Version: 1.0.5
+Version: 1.0.6
 Summary: A package to check mysql restore integrity check
 Home-page: 
 Author: Maihraj Hasan
 Author-email: maihrajhasan@gmail.com
 Project-URL: Bug Tracker, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck/-/issues
 Project-URL: repository, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck
 Classifier: Programming Language :: Python :: 3
@@ -38,33 +38,39 @@
 from tabulate import tabulate
 import os
 
 src_db_host = os.environ['SRC_DB_HOST']
 src_db_pass = os.environ['SRC_DB_PASS']
 src_db_user = os.environ['SRC_DB_USER']
 
+
 dst_db_host = os.environ['DST_DB_HOST']
 dst_db_pass = os.environ['DST_DB_PASS']
 dst_db_user = os.environ['DST_DB_USER']
 
 
-database = mysql.mysqlRestroeCheck(src_db_host, src_db_user, src_db_pass)
-database1 = mysql.mysqlRestroeCheck(dst_db_host, dst_db_user, dst_db_pass)
-database._create_tmp_table('restore_rds')
-database1._create_tmp_table('actual_rds')
+
+restored_db = mysql.mysqlReadData(dst_db_host, dst_db_user, dst_db_pass)
+active_db = mysql.mysqlReadData(src_db_host, src_db_user, src_db_pass)
+
+restored_db._create_tmp_file('restored_db')
+active_db._create_tmp_file('active_db')
+restored_db._insert_data('restored_db')
+restored_db._insert_data('active_db')
+
 
 def check_consistency():
     unconsistent_tabels = []
-    conn = database.connection()
+    conn = restored_db.connection()
     check_consistency = conn.cursor()
-    check_consistency.execute("USE restore_consistency")
-    check_consistency.execute("SELECT tables_name,records_count,hostname FROM (SELECT tables_name,records_count,hostname FROM restore_rds UNION ALL SELECT tables_name,records_count,hostname FROM actual_rds) tbl GROUP BY tables_name, hostname, records_count HAVING count(*) = 1 ORDER BY tables_name")
-
+    check_consistency.execute("USE CheckDBsTableConsistency")
+    check_consistency.execute("select tables_name, records_count, hostname from (select tables_name, hostname, records_count from active_db union all select tables_name, hostname, records_count from restored_db) temp group by tables_name, records_count having count(*) = 1")
     result = check_consistency.fetchall()
     print(tabulate(result, headers=['tables_name', 'records_count'], tablefmt='psql'))
+    conn.close()
 check_consistency()
 ```
```

### Comparing `databaseRestoreIntegrity-1.0.5/setup.cfg` & `databaseRestoreIntegrity-1.0.6/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = databaseRestoreIntegrity
-version = 1.0.5
+version = 1.0.6
 author = Maihraj Hasan
 author_email = maihrajhasan@gmail.com
 description = A package to check mysql restore integrity check
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = 
 project_urls =
```

### Comparing `databaseRestoreIntegrity-1.0.5/src/databaseRestoreIntegrity/mysql.py` & `databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity/mysql.py`

 * *Files identical despite different names*

### Comparing `databaseRestoreIntegrity-1.0.5/src/databaseRestoreIntegrity.egg-info/PKG-INFO` & `databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databaseRestoreIntegrity
-Version: 1.0.5
+Version: 1.0.6
 Summary: A package to check mysql restore integrity check
 Home-page: 
 Author: Maihraj Hasan
 Author-email: maihrajhasan@gmail.com
 Project-URL: Bug Tracker, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck/-/issues
 Project-URL: repository, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck
 Classifier: Programming Language :: Python :: 3
@@ -38,33 +38,39 @@
 from tabulate import tabulate
 import os
 
 src_db_host = os.environ['SRC_DB_HOST']
 src_db_pass = os.environ['SRC_DB_PASS']
 src_db_user = os.environ['SRC_DB_USER']
 
+
 dst_db_host = os.environ['DST_DB_HOST']
 dst_db_pass = os.environ['DST_DB_PASS']
 dst_db_user = os.environ['DST_DB_USER']
 
 
-database = mysql.mysqlRestroeCheck(src_db_host, src_db_user, src_db_pass)
-database1 = mysql.mysqlRestroeCheck(dst_db_host, dst_db_user, dst_db_pass)
-database._create_tmp_table('restore_rds')
-database1._create_tmp_table('actual_rds')
+
+restored_db = mysql.mysqlReadData(dst_db_host, dst_db_user, dst_db_pass)
+active_db = mysql.mysqlReadData(src_db_host, src_db_user, src_db_pass)
+
+restored_db._create_tmp_file('restored_db')
+active_db._create_tmp_file('active_db')
+restored_db._insert_data('restored_db')
+restored_db._insert_data('active_db')
+
 
 def check_consistency():
     unconsistent_tabels = []
-    conn = database.connection()
+    conn = restored_db.connection()
     check_consistency = conn.cursor()
-    check_consistency.execute("USE restore_consistency")
-    check_consistency.execute("SELECT tables_name,records_count,hostname FROM (SELECT tables_name,records_count,hostname FROM restore_rds UNION ALL SELECT tables_name,records_count,hostname FROM actual_rds) tbl GROUP BY tables_name, hostname, records_count HAVING count(*) = 1 ORDER BY tables_name")
-
+    check_consistency.execute("USE CheckDBsTableConsistency")
+    check_consistency.execute("select tables_name, records_count, hostname from (select tables_name, hostname, records_count from active_db union all select tables_name, hostname, records_count from restored_db) temp group by tables_name, records_count having count(*) = 1")
     result = check_consistency.fetchall()
     print(tabulate(result, headers=['tables_name', 'records_count'], tablefmt='psql'))
+    conn.close()
 check_consistency()
 ```
```

