# Comparing `tmp/databaseRestoreIntegrity-1.0.6.tar.gz` & `tmp/databaseRestoreIntegrity-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databaseRestoreIntegrity-1.0.6.tar", last modified: Thu Jun 15 09:06:19 2023, max compression
+gzip compressed data, was "databaseRestoreIntegrity-1.0.7.tar", last modified: Thu Jun 15 13:05:21 2023, max compression
```

## Comparing `databaseRestoreIntegrity-1.0.6.tar` & `databaseRestoreIntegrity-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 09:06:19.615181 databaseRestoreIntegrity-1.0.6/
--rw-r--r--   0 mhasan     (502) staff       (20)     1073 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.6/LICENSE.txt
--rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.6/MANIFEST.in
--rw-r--r--   0 mhasan     (502) staff       (20)     3727 2023-06-15 09:06:19.615285 databaseRestoreIntegrity-1.0.6/PKG-INFO
--rw-r--r--   0 mhasan     (502) staff       (20)     2035 2023-06-08 12:12:36.000000 databaseRestoreIntegrity-1.0.6/README.md
--rw-r--r--   0 mhasan     (502) staff       (20)       84 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.6/pyproject.toml
--rw-r--r--   0 mhasan     (502) staff       (20)      740 2023-06-15 09:06:19.622489 databaseRestoreIntegrity-1.0.6/setup.cfg
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 09:06:19.605893 databaseRestoreIntegrity-1.0.6/src/
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 09:06:19.609875 databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity/
--rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity/__init__.py
--rw-r--r--   0 mhasan     (502) staff       (20)     2970 2023-06-07 12:36:19.000000 databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity/mysql.py
--rw-r--r--   0 mhasan     (502) staff       (20)     2873 2023-06-11 12:26:37.000000 databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity/postgres.py
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 09:06:19.614537 databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity.egg-info/
--rw-r--r--   0 mhasan     (502) staff       (20)     3727 2023-06-15 09:06:19.000000 databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity.egg-info/PKG-INFO
--rw-r--r--   0 mhasan     (502) staff       (20)      386 2023-06-15 09:06:19.000000 databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity.egg-info/SOURCES.txt
--rw-r--r--   0 mhasan     (502) staff       (20)        1 2023-06-15 09:06:19.000000 databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity.egg-info/dependency_links.txt
--rw-r--r--   0 mhasan     (502) staff       (20)       25 2023-06-15 09:06:19.000000 databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity.egg-info/top_level.txt
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 13:05:21.875875 databaseRestoreIntegrity-1.0.7/
+-rw-r--r--   0 mhasan     (502) staff       (20)     1073 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.7/LICENSE.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.7/MANIFEST.in
+-rw-r--r--   0 mhasan     (502) staff       (20)     3727 2023-06-15 13:05:21.876004 databaseRestoreIntegrity-1.0.7/PKG-INFO
+-rw-r--r--   0 mhasan     (502) staff       (20)     2035 2023-06-08 12:12:36.000000 databaseRestoreIntegrity-1.0.7/README.md
+-rw-r--r--   0 mhasan     (502) staff       (20)       84 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.7/pyproject.toml
+-rw-r--r--   0 mhasan     (502) staff       (20)      740 2023-06-15 13:05:21.882928 databaseRestoreIntegrity-1.0.7/setup.cfg
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 13:05:21.866936 databaseRestoreIntegrity-1.0.7/src/
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 13:05:21.871316 databaseRestoreIntegrity-1.0.7/src/databaseRestoreIntegrity/
+-rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.7/src/databaseRestoreIntegrity/__init__.py
+-rw-r--r--   0 mhasan     (502) staff       (20)     2970 2023-06-07 12:36:19.000000 databaseRestoreIntegrity-1.0.7/src/databaseRestoreIntegrity/mysql.py
+-rw-r--r--   0 mhasan     (502) staff       (20)     2872 2023-06-15 13:02:54.000000 databaseRestoreIntegrity-1.0.7/src/databaseRestoreIntegrity/postgres.py
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 13:05:21.874604 databaseRestoreIntegrity-1.0.7/src/databaseRestoreIntegrity.egg-info/
+-rw-r--r--   0 mhasan     (502) staff       (20)     3727 2023-06-15 13:05:21.000000 databaseRestoreIntegrity-1.0.7/src/databaseRestoreIntegrity.egg-info/PKG-INFO
+-rw-r--r--   0 mhasan     (502) staff       (20)      386 2023-06-15 13:05:21.000000 databaseRestoreIntegrity-1.0.7/src/databaseRestoreIntegrity.egg-info/SOURCES.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)        1 2023-06-15 13:05:21.000000 databaseRestoreIntegrity-1.0.7/src/databaseRestoreIntegrity.egg-info/dependency_links.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)       25 2023-06-15 13:05:21.000000 databaseRestoreIntegrity-1.0.7/src/databaseRestoreIntegrity.egg-info/top_level.txt
```

### Comparing `databaseRestoreIntegrity-1.0.6/LICENSE.txt` & `databaseRestoreIntegrity-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `databaseRestoreIntegrity-1.0.6/PKG-INFO` & `databaseRestoreIntegrity-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databaseRestoreIntegrity
-Version: 1.0.6
+Version: 1.0.7
 Summary: A package to check mysql restore integrity check
 Home-page: 
 Author: Maihraj Hasan
 Author-email: maihrajhasan@gmail.com
 Project-URL: Bug Tracker, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck/-/issues
 Project-URL: repository, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck
 Classifier: Programming Language :: Python :: 3
```

### Comparing `databaseRestoreIntegrity-1.0.6/README.md` & `databaseRestoreIntegrity-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `databaseRestoreIntegrity-1.0.6/setup.cfg` & `databaseRestoreIntegrity-1.0.7/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = databaseRestoreIntegrity
-version = 1.0.6
+version = 1.0.7
 author = Maihraj Hasan
 author_email = maihrajhasan@gmail.com
 description = A package to check mysql restore integrity check
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = 
 project_urls =
```

### Comparing `databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity/mysql.py` & `databaseRestoreIntegrity-1.0.7/src/databaseRestoreIntegrity/mysql.py`

 * *Files identical despite different names*

### Comparing `databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity/postgres.py` & `databaseRestoreIntegrity-1.0.7/src/databaseRestoreIntegrity/postgres.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,32 +24,31 @@
         return mydb
     
     def _get_tables_raw_data(self):
         raw_tables_data = []
         # sql_query = "\dt *.*"
         conn = self.connection()
         mycursor = conn.cursor()
-        mycursor.execute("SELECT schemaname,tablename FROM pg_catalog.pg_tables")
+        mycursor.execute("SELECT schemaname,tablename FROM pg_catalog.pg_tables WHERE schemaname != 'pg_catalog' AND schemaname != 'information_schema'")
         for x in mycursor:
             raw_tables_data.append(str("{}.{}".format(*x)))
         return raw_tables_data
 
     
     def _get_count(self):
         records_count = []
         raw_tables = self._get_tables_raw_data()
         try:
             conn = self.connection()
-            for x in raw_tables:
-                if x.split('.')[0] not in 'pg_catalog':
-                    sql_query = ("{} {}".format("SELECT COUNT(*) FROM", x))
-                    mycursor = conn.cursor()
-                    mycursor.execute(sql_query)
-                    for c in mycursor:
-                        records_count.append("{},{}".format(x, *c))
+            for x in raw_tables:   
+                sql_query = ("{} {}".format("SELECT COUNT(*) FROM", x))
+                mycursor = conn.cursor()
+                mycursor.execute(sql_query)
+                for c in mycursor:
+                    records_count.append("{},{}".format(x, *c))
         except:
             print(f'database list not succedd')
         return records_count
 
     def _create_tmp_file(self, name):
         self.name = name
         records = self._get_count()
```

### Comparing `databaseRestoreIntegrity-1.0.6/src/databaseRestoreIntegrity.egg-info/PKG-INFO` & `databaseRestoreIntegrity-1.0.7/src/databaseRestoreIntegrity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databaseRestoreIntegrity
-Version: 1.0.6
+Version: 1.0.7
 Summary: A package to check mysql restore integrity check
 Home-page: 
 Author: Maihraj Hasan
 Author-email: maihrajhasan@gmail.com
 Project-URL: Bug Tracker, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck/-/issues
 Project-URL: repository, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck
 Classifier: Programming Language :: Python :: 3
```

