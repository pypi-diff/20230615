# Comparing `tmp/dagster-mysql-0.19.9.tar.gz` & `tmp/dagster-mysql-0.19.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-mysql-0.19.9.tar", last modified: Thu Jun  8 18:52:04 2023, max compression
+gzip compressed data, was "dagster-mysql-0.19.9rc0.tar", last modified: Thu Jun  8 18:28:57 2023, max compression
```

## Comparing `dagster-mysql-0.19.9.tar` & `dagster-mysql-0.19.9rc0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:03.995170 dagster-mysql-0.19.9/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:43:17.000000 dagster-mysql-0.19.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      126 2023-06-08 18:43:17.000000 dagster-mysql-0.19.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      602 2023-06-08 18:52:03.995170 dagster-mysql-0.19.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      125 2023-06-08 18:43:17.000000 dagster-mysql-0.19.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:03.995170 dagster-mysql-0.19.9/dagster_mysql/
--rw-r--r--   0 root         (0) root         (0)      434 2023-06-08 18:43:17.000000 dagster-mysql-0.19.9/dagster_mysql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:03.995170 dagster-mysql-0.19.9/dagster_mysql/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-mysql-0.19.9/dagster_mysql/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-08 18:43:17.000000 dagster-mysql-0.19.9/dagster_mysql/alembic/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:03.995170 dagster-mysql-0.19.9/dagster_mysql/event_log/
--rw-r--r--   0 root         (0) root         (0)       68 2023-06-08 18:43:17.000000 dagster-mysql-0.19.9/dagster_mysql/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8792 2023-06-08 18:43:17.000000 dagster-mysql-0.19.9/dagster_mysql/event_log/event_log.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:43:17.000000 dagster-mysql-0.19.9/dagster_mysql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:03.995170 dagster-mysql-0.19.9/dagster_mysql/run_storage/
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-08 18:43:17.000000 dagster-mysql-0.19.9/dagster_mysql/run_storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7883 2023-06-08 18:43:17.000000 dagster-mysql-0.19.9/dagster_mysql/run_storage/run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:03.995170 dagster-mysql-0.19.9/dagster_mysql/schedule_storage/
--rw-r--r--   0 root         (0) root         (0)       75 2023-06-08 18:43:17.000000 dagster-mysql-0.19.9/dagster_mysql/schedule_storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6277 2023-06-08 18:43:17.000000 dagster-mysql-0.19.9/dagster_mysql/schedule_storage/schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     3730 2023-06-08 18:43:17.000000 dagster-mysql-0.19.9/dagster_mysql/storage.py
--rw-r--r--   0 root         (0) root         (0)     6404 2023-06-08 18:43:17.000000 dagster-mysql-0.19.9/dagster_mysql/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 18:43:17.000000 dagster-mysql-0.19.9/dagster_mysql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:03.995170 dagster-mysql-0.19.9/dagster_mysql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      602 2023-06-08 18:52:03.000000 dagster-mysql-0.19.9/dagster_mysql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      704 2023-06-08 18:52:03.000000 dagster-mysql-0.19.9/dagster_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:52:03.000000 dagster-mysql-0.19.9/dagster_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:52:03.000000 dagster-mysql-0.19.9/dagster_mysql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 18:52:03.000000 dagster-mysql-0.19.9/dagster_mysql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-08 18:52:03.000000 dagster-mysql-0.19.9/dagster_mysql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      148 2023-06-08 18:52:03.999170 dagster-mysql-0.19.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1293 2023-06-08 18:43:17.000000 dagster-mysql-0.19.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      126 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      605 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      125 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:57.567206 dagster-mysql-0.19.9rc0/dagster_mysql/
+-rw-r--r--   0 root         (0) root         (0)      434 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/dagster_mysql/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/alembic/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/dagster_mysql/event_log/
+-rw-r--r--   0 root         (0) root         (0)       68 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8792 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/event_log/event_log.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/dagster_mysql/run_storage/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/run_storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7883 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/run_storage/run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/dagster_mysql/schedule_storage/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/schedule_storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6277 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/schedule_storage/schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3730 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/storage.py
+-rw-r--r--   0 root         (0) root         (0)     6404 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/utils.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      605 2023-06-08 18:28:57.000000 dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      704 2023-06-08 18:28:57.000000 dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:57.000000 dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:57.000000 dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       41 2023-06-08 18:28:57.000000 dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-08 18:28:57.000000 dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/setup.py
```

### Comparing `dagster-mysql-0.19.9/LICENSE` & `dagster-mysql-0.19.9rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.19.9/PKG-INFO` & `dagster-mysql-0.19.9rc0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mysql
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: A Dagster integration for MySQL
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mysql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-mysql-0.19.9/dagster_mysql/alembic/alembic.ini` & `dagster-mysql-0.19.9rc0/dagster_mysql/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.19.9/dagster_mysql/event_log/event_log.py` & `dagster-mysql-0.19.9rc0/dagster_mysql/event_log/event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.19.9/dagster_mysql/run_storage/run_storage.py` & `dagster-mysql-0.19.9rc0/dagster_mysql/run_storage/run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.19.9/dagster_mysql/schedule_storage/schedule_storage.py` & `dagster-mysql-0.19.9rc0/dagster_mysql/schedule_storage/schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.19.9/dagster_mysql/storage.py` & `dagster-mysql-0.19.9rc0/dagster_mysql/storage.py`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.19.9/dagster_mysql/utils.py` & `dagster-mysql-0.19.9rc0/dagster_mysql/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.19.9/dagster_mysql.egg-info/PKG-INFO` & `dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mysql
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: A Dagster integration for MySQL
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mysql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-mysql-0.19.9/dagster_mysql.egg-info/SOURCES.txt` & `dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.19.9/setup.py` & `dagster-mysql-0.19.9rc0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,10 +33,10 @@
     packages=find_packages(exclude=["dagster_mysql_tests*"]),
     package_data={
         "dagster-mysql": [
             "dagster_mysql/alembic/*",
         ]
     },
     include_package_data=True,
-    install_requires=["dagster==1.3.9", "mysql-connector-python"],
+    install_requires=["dagster==1.3.9rc0", "mysql-connector-python"],
     zip_safe=False,
 )
```

