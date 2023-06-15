# Comparing `tmp/databaseRestoreIntegrity-1.0.8.tar.gz` & `tmp/databaseRestoreIntegrity-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databaseRestoreIntegrity-1.0.8.tar", last modified: Thu Jun 15 13:10:54 2023, max compression
+gzip compressed data, was "databaseRestoreIntegrity-1.0.9.tar", last modified: Thu Jun 15 14:21:19 2023, max compression
```

## Comparing `databaseRestoreIntegrity-1.0.8.tar` & `databaseRestoreIntegrity-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 13:10:54.601181 databaseRestoreIntegrity-1.0.8/
--rw-r--r--   0 mhasan     (502) staff       (20)     1073 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.8/LICENSE.txt
--rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.8/MANIFEST.in
--rw-r--r--   0 mhasan     (502) staff       (20)     3727 2023-06-15 13:10:54.601290 databaseRestoreIntegrity-1.0.8/PKG-INFO
--rw-r--r--   0 mhasan     (502) staff       (20)     2035 2023-06-08 12:12:36.000000 databaseRestoreIntegrity-1.0.8/README.md
--rw-r--r--   0 mhasan     (502) staff       (20)       84 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.8/pyproject.toml
--rw-r--r--   0 mhasan     (502) staff       (20)      740 2023-06-15 13:10:54.602948 databaseRestoreIntegrity-1.0.8/setup.cfg
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 13:10:54.558061 databaseRestoreIntegrity-1.0.8/src/
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 13:10:54.597720 databaseRestoreIntegrity-1.0.8/src/databaseRestoreIntegrity/
--rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.8/src/databaseRestoreIntegrity/__init__.py
--rw-r--r--   0 mhasan     (502) staff       (20)     2970 2023-06-07 12:36:19.000000 databaseRestoreIntegrity-1.0.8/src/databaseRestoreIntegrity/mysql.py
--rw-r--r--   0 mhasan     (502) staff       (20)     2872 2023-06-15 13:02:54.000000 databaseRestoreIntegrity-1.0.8/src/databaseRestoreIntegrity/postgres.py
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 13:10:54.600805 databaseRestoreIntegrity-1.0.8/src/databaseRestoreIntegrity.egg-info/
--rw-r--r--   0 mhasan     (502) staff       (20)     3727 2023-06-15 13:10:54.000000 databaseRestoreIntegrity-1.0.8/src/databaseRestoreIntegrity.egg-info/PKG-INFO
--rw-r--r--   0 mhasan     (502) staff       (20)      386 2023-06-15 13:10:54.000000 databaseRestoreIntegrity-1.0.8/src/databaseRestoreIntegrity.egg-info/SOURCES.txt
--rw-r--r--   0 mhasan     (502) staff       (20)        1 2023-06-15 13:10:54.000000 databaseRestoreIntegrity-1.0.8/src/databaseRestoreIntegrity.egg-info/dependency_links.txt
--rw-r--r--   0 mhasan     (502) staff       (20)       25 2023-06-15 13:10:54.000000 databaseRestoreIntegrity-1.0.8/src/databaseRestoreIntegrity.egg-info/top_level.txt
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 14:21:19.169314 databaseRestoreIntegrity-1.0.9/
+-rw-r--r--   0 mhasan     (502) staff       (20)     1073 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.9/LICENSE.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.9/MANIFEST.in
+-rw-r--r--   0 mhasan     (502) staff       (20)     6223 2023-06-15 14:21:19.169491 databaseRestoreIntegrity-1.0.9/PKG-INFO
+-rw-r--r--   0 mhasan     (502) staff       (20)     4531 2023-06-15 14:19:55.000000 databaseRestoreIntegrity-1.0.9/README.md
+-rw-r--r--   0 mhasan     (502) staff       (20)       84 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.9/pyproject.toml
+-rw-r--r--   0 mhasan     (502) staff       (20)      740 2023-06-15 14:21:19.171057 databaseRestoreIntegrity-1.0.9/setup.cfg
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 14:21:19.147468 databaseRestoreIntegrity-1.0.9/src/
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 14:21:19.165862 databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity/
+-rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity/__init__.py
+-rw-r--r--   0 mhasan     (502) staff       (20)     2970 2023-06-07 12:36:19.000000 databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity/mysql.py
+-rw-r--r--   0 mhasan     (502) staff       (20)     2872 2023-06-15 13:02:54.000000 databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity/postgres.py
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 14:21:19.168775 databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity.egg-info/
+-rw-r--r--   0 mhasan     (502) staff       (20)     6223 2023-06-15 14:21:19.000000 databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity.egg-info/PKG-INFO
+-rw-r--r--   0 mhasan     (502) staff       (20)      386 2023-06-15 14:21:19.000000 databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity.egg-info/SOURCES.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)        1 2023-06-15 14:21:19.000000 databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity.egg-info/dependency_links.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)       25 2023-06-15 14:21:19.000000 databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity.egg-info/top_level.txt
```

### Comparing `databaseRestoreIntegrity-1.0.8/LICENSE.txt` & `databaseRestoreIntegrity-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `databaseRestoreIntegrity-1.0.8/README.md` & `databaseRestoreIntegrity-1.0.9/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 # MySQL restore integrity check
 Module can be used to test the database integrigity after restore the database. It will compare tables and show the only that tables in tabular format, Which had diffrencial records in after restore. 
 
-## Requirements
+## Requirements 
+### MySQL
 - python3.6 or above
 - tablular and os python plugin should be installed using pip3
 
-## How to use
+### PostgreSQL
+- python3.6 or above
+- tablular, os, Psycopg2 or Psycopg2-binary python plugin should be installed using pip3
+
+### How to use MySQL
 ```
 $ pip3 install databaseRestoreIntegrity
 $ export SRC_DB_HOST='origin_database_hostname'
 $ export SRC_DB_USER='origin_database_username'
 $ export SRC_DB_PASS='origin_database_password'
 $ export DST_DB_HOST='restored_database_hostname'
 $ export DST_DB_USER='restored_database_username'
 $ export DST_DB_PASS='restored_database_password'
 ```
 
-### Now create and run a python scrip using the content below
+### MySQL python script (Create and run on your local or from the host which can connect both db -- restored and active)
 ```
 from databaseRestoreIntegrity import mysql
 from tabulate import tabulate
 import os
 
 src_db_host = os.environ['SRC_DB_HOST']
 src_db_pass = os.environ['SRC_DB_PASS']
 src_db_user = os.environ['SRC_DB_USER']
-
-
 dst_db_host = os.environ['DST_DB_HOST']
 dst_db_pass = os.environ['DST_DB_PASS']
 dst_db_user = os.environ['DST_DB_USER']
 
 
 
 restored_db = mysql.mysqlReadData(dst_db_host, dst_db_user, dst_db_pass)
@@ -50,10 +53,72 @@
     check_consistency.execute("select tables_name, records_count, hostname from (select tables_name, hostname, records_count from active_db union all select tables_name, hostname, records_count from restored_db) temp group by tables_name, records_count having count(*) = 1")
     result = check_consistency.fetchall()
     print(tabulate(result, headers=['tables_name', 'records_count'], tablefmt='psql'))
     conn.close()
 check_consistency()
 ```
 
+### How to use PostgreSQL
+```
+$ pip3 install databaseRestoreIntegrity
+$ export SRC_DB_HOST='origin_database_hostname'
+$ export SRC_DB_USER='origin_database_username'
+$ export SRC_DB_PASS='origin_database_password'
+$ export DST_DB_HOST='restored_database_hostname'
+$ export DST_DB_USER='restored_database_username'
+$ export DST_DB_PASS='restored_database_password'
+$ export DB_NAME='database_name' 
+```
+
+**Note:** Postgres need databsebase name to connectivity
+
+
+### PostgreSQL python script (Create and run on your local or from the host which can connect both db -- restored and active)
+```
+from databaseRestoreIntegrity import postgres
+from tabulate import tabulate
+import os
+
+src_db_host = os.environ['SRC_DB_HOST']
+src_db_pass = os.environ['SRC_DB_PASS']
+src_db_user = os.environ['SRC_DB_USER']
+dst_db_host = os.environ['DST_DB_HOST']
+dst_db_pass = os.environ['DST_DB_PASS']
+dst_db_user = os.environ['DST_DB_USER']
+db_name = os.environ['DB_NAME']
+
+
+
+restored_db = postgres.pgsqlReadData(dst_db_host, dst_db_user, dst_db_pass, db_name)
+active_db = postgres.pgsqlReadData(src_db_host, src_db_user, src_db_pass, db_name)
+
+restored_db._create_tmp_file('restored_db')
+active_db._create_tmp_file('active_db')
+restored_db._insert_data('restored_db')
+restored_db._insert_data('active_db')
+
+
+def check_consistency():
+    unconsistent_tabels = []
+    sql_query = "SELECT COALESCE(s.tables_name,t.tables_name) id, \
+                s.records_count records_count, t.records_count records_count, \
+                CASE WHEN s.records_count = t.records_count THEN 'equal' \
+                    WHEN s.tables_name IS NULL THEN 'Table not on source' \
+                    WHEN t.tables_name IS NULL THEN 'Table not on target' \
+                    ELSE 'difference' \
+                END compare_result \
+                FROM CheckDBsTableConsistency.active_db s \
+                FULL JOIN CheckDBsTableConsistency.restored_db t ON s.tables_name=t.tables_name"
+    conn = restored_db.connection()
+    check_consistency = conn.cursor()
+    check_consistency.execute(sql_query)
+    result = check_consistency.fetchall()
+    print(tabulate(result, headers=['tables_name', 'records_count_active_db', 'records_count_restored_db', 'compare_result'], tablefmt='psql'))
+    conn.close()
+check_consistency()
+```
+
+
+
```

### Comparing `databaseRestoreIntegrity-1.0.8/setup.cfg` & `databaseRestoreIntegrity-1.0.9/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = databaseRestoreIntegrity
-version = 1.0.8
+version = 1.0.9
 author = Maihraj Hasan
 author_email = maihrajhasan@gmail.com
 description = A package to check mysql restore integrity check
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = 
 project_urls =
```

### Comparing `databaseRestoreIntegrity-1.0.8/src/databaseRestoreIntegrity/mysql.py` & `databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity/mysql.py`

 * *Files identical despite different names*

### Comparing `databaseRestoreIntegrity-1.0.8/src/databaseRestoreIntegrity/postgres.py` & `databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity/postgres.py`

 * *Files identical despite different names*

