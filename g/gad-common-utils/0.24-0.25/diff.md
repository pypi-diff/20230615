# Comparing `tmp/gad_common_utils-0.24.tar.gz` & `tmp/gad_common_utils-0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gad_common_utils-0.24.tar", last modified: Tue Jun 13 12:32:38 2023, max compression
+gzip compressed data, was "gad_common_utils-0.25.tar", last modified: Thu Jun 15 20:05:58 2023, max compression
```

## Comparing `gad_common_utils-0.24.tar` & `gad_common_utils-0.25.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:32:38.619688 gad_common_utils-0.24/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:32:38.615687 gad_common_utils-0.24/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:32:38.615687 gad_common_utils-0.24/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-13 12:32:25.000000 gad_common_utils-0.24/.github/workflows/black-format-checker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-13 12:32:25.000000 gad_common_utils-0.24/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-13 12:32:25.000000 gad_common_utils-0.24/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-13 12:32:25.000000 gad_common_utils-0.24/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-13 12:32:25.000000 gad_common_utils-0.24/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-13 12:32:38.619688 gad_common_utils-0.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-13 12:32:25.000000 gad_common_utils-0.24/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:32:38.619688 gad_common_utils-0.24/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-13 12:32:25.000000 gad_common_utils-0.24/common_utils/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:32:25.000000 gad_common_utils-0.24/common_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-13 12:32:38.000000 gad_common_utils-0.24/common_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-06-13 12:32:25.000000 gad_common_utils-0.24/common_utils/data_loading_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-13 12:32:25.000000 gad_common_utils-0.24/common_utils/data_type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-13 12:32:25.000000 gad_common_utils-0.24/common_utils/date_time_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-13 12:32:25.000000 gad_common_utils-0.24/common_utils/dynamodb_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-13 12:32:25.000000 gad_common_utils-0.24/common_utils/dynamodb_ray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-13 12:32:25.000000 gad_common_utils-0.24/common_utils/files_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-06-13 12:32:25.000000 gad_common_utils-0.24/common_utils/gad_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-06-13 12:32:25.000000 gad_common_utils-0.24/common_utils/gad_utils_additionals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-06-13 12:32:25.000000 gad_common_utils-0.24/common_utils/json_schema_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-13 12:32:25.000000 gad_common_utils-0.24/common_utils/run_athena_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-06-13 12:32:25.000000 gad_common_utils-0.24/common_utils/s3_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-13 12:32:25.000000 gad_common_utils-0.24/common_utils/sql_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-13 12:32:25.000000 gad_common_utils-0.24/common_utils/string_transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:32:38.619688 gad_common_utils-0.24/gad_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-13 12:32:38.000000 gad_common_utils-0.24/gad_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-13 12:32:38.000000 gad_common_utils-0.24/gad_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:32:38.000000 gad_common_utils-0.24/gad_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 12:32:38.000000 gad_common_utils-0.24/gad_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 12:32:38.000000 gad_common_utils-0.24/gad_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-13 12:32:25.000000 gad_common_utils-0.24/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 12:32:38.619688 gad_common_utils-0.24/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:32:38.619688 gad_common_utils-0.24/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:32:25.000000 gad_common_utils-0.24/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-13 12:32:25.000000 gad_common_utils-0.24/tests/test_json_schema_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:05:58.330087 gad_common_utils-0.25/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:05:58.326087 gad_common_utils-0.25/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:05:58.326087 gad_common_utils-0.25/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-15 20:05:46.000000 gad_common_utils-0.25/.github/workflows/black-format-checker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-15 20:05:46.000000 gad_common_utils-0.25/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-15 20:05:46.000000 gad_common_utils-0.25/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-15 20:05:46.000000 gad_common_utils-0.25/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-15 20:05:46.000000 gad_common_utils-0.25/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-15 20:05:58.330087 gad_common_utils-0.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-15 20:05:46.000000 gad_common_utils-0.25/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:05:58.326087 gad_common_utils-0.25/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-15 20:05:58.000000 gad_common_utils-0.25/common_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/data_loading_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/data_type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/date_time_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/dynamodb_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/dynamodb_ray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/files_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18069 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/gad_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/gad_utils_additionals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/json_schema_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/run_athena_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/s3_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/sql_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/string_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:05:58.326087 gad_common_utils-0.25/gad_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-15 20:05:58.000000 gad_common_utils-0.25/gad_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-15 20:05:58.000000 gad_common_utils-0.25/gad_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 20:05:58.000000 gad_common_utils-0.25/gad_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 20:05:58.000000 gad_common_utils-0.25/gad_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 20:05:58.000000 gad_common_utils-0.25/gad_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-15 20:05:46.000000 gad_common_utils-0.25/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 20:05:58.330087 gad_common_utils-0.25/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:05:58.326087 gad_common_utils-0.25/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:05:46.000000 gad_common_utils-0.25/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-15 20:05:46.000000 gad_common_utils-0.25/tests/test_json_schema_methods.py
```

### Comparing `gad_common_utils-0.24/.github/workflows/black-format-checker.yml` & `gad_common_utils-0.25/.github/workflows/black-format-checker.yml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.24/.github/workflows/publish-to-pypi.yml` & `gad_common_utils-0.25/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.24/.github/workflows/pytest.yml` & `gad_common_utils-0.25/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.24/PKG-INFO` & `gad_common_utils-0.25/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gad_common_utils
-Version: 0.24
+Version: 0.25
 Summary: gad utility
 Project-URL: Homepage, http://gad-co.ml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `gad_common_utils-0.24/common_utils/data_loading_management.py` & `gad_common_utils-0.25/common_utils/data_loading_management.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,93 +1,95 @@
-import argparse
+import ast
 import logging
+import os
 from datetime import datetime
 
 import awswrangler as wr
+import boto3
 from dateutil.relativedelta import relativedelta
 
 from common_utils.date_time_methods import dateTimeMethods
 
 
 class dataLoadingManagement:
     """
     Class to manage data loading operations. It provides functions to set the start and end timestamps for the data loading,
     validating the start and end timestamps, and creating the schema if the data is being loaded for the first time.
 
     Args:
-        app_args: An instance of argparse.Namespace, containing command line arguments passed to the application.
+        from_timestamp: A string, representing the start timestamp specified by the user.
+        to_timestamp: A string, representing the end timestamp specified by the user.
+        full_load: A string, indicating whether the data is being loaded for the first time.
+        full_load_from_timestamp: A string, representing the start timestamp to use if the data is being loaded for the first time and the start timestamp is specified by the user.
+        full_load_from_timestamp_months_back: An integer, representing the number of months to
+            go back to calculate the default start timestamp if the data is being loaded for the first time and the start timestamp is not specified by the user.
+        athena_workgroup: A string, representing the name of the Athena workgroup to use.
         timestamp_col_name: A string, representing the name of the column in the source data which contains the timestamp.
         tbl_to_check_max_timestamp: A string, representing the name of the table in the destination database to check for the max timestamp.
         from_and_to_as_dates: A boolean, indicating whether the start and end timestamps should be set as dates (midnight of the given date).
-        create_schema_if_initial_load: A boolean, indicating whether the schema should be created if the data is being loaded for the first time.
-
-    Attributes:
-        given_from_timestamp: A string, representing the start timestamp specified by the user.
-        given_to_timestamp: A string, representing the end timestamp specified by the user.
-        initial_load: A string, indicating whether the data is being loaded for the first time.
-        initial_load_from_timestamp: A string, representing the start timestamp to use if the data is being loaded for the first time and the start timestamp is specified by the user.
-        initial_load_from_timestamp_months_back: An integer, representing the number of months to go back to calculate the default start timestamp if the data is being loaded for the first time and the start timestamp is not specified by the user.
-        dest_schema: A string, representing the name of the destination database.
-        timestamp_col_name: A string, representing the name of the column in the source data which contains the timestamp.
-        tbl_to_check_max_timestamp: A string, representing the name of the table in the destination database to check for the max timestamp.
-        default_from_timestamp: A datetime object, representing the default start timestamp to use if the data is being loaded for the first time and the start timestamp is not specified by the user.
-        from_timestamp: A datetime object, representing the start timestamp to use for the data loading.
-        to_timestamp: A datetime object, representing the end timestamp to use for the data loading.
+        create_schema_if_full_load: A boolean, indicating whether the schema should be created if the data is being loaded for the first time.
     """
 
     def __init__(
         self,
-        app_args: argparse.Namespace,
-        timestamp_col_name: str,
-        tbl_to_check_max_timestamp: str,
+        from_timestamp: str = None,
+        to_timestamp: str = None,
+        full_load: bool = False,
+        full_load_from_timestamp: str = None,
+        full_load_from_timestamp_months_back: int = 3,
+        athena_workgroup: str = "primary",
+        timestamp_col_name: str = None,
+        tbl_to_check_max_timestamp: str = None,
         from_and_to_as_dates: bool = False,
-        create_schema_if_initial_load: bool = True,
+        create_schema_if_full_load: bool = True,
     ):
         """
         Initializes the class and sets the start and end timestamps, and creates the schema if the data is being loaded for the first time.
         """
-        self.given_from_timestamp = app_args.from_timestamp
-        self.given_to_timestamp = app_args.to_timestamp
-        self.initial_load = app_args.initial_load
-        self.initial_load_from_timestamp = app_args.initial_load_from_timestamp
-        self.initial_load_from_timestamp_months_back = (
-            app_args.initial_load_from_timestamp_months_back
-        )
-        self.dest_schema = app_args.destination_database_name
-        self.athena_workgroup = app_args.athena_workgroup
+        self.given_from_timestamp = from_timestamp
+        self.given_to_timestamp = to_timestamp
+        self.full_load = ast.literal_eval(full_load)
+        self.full_load_from_timestamp = full_load_from_timestamp
+        self.full_load_from_timestamp_months_back = full_load_from_timestamp_months_back
+
+        self.dest_schema = os.environ.get("ATHENA_DB")
+        self.athena_workgroup = athena_workgroup
         self.timestamp_col_name = timestamp_col_name
         self.tbl_to_check_max_timestamp = tbl_to_check_max_timestamp
 
         # to be used if nothing else is given
         self.default_from_timestamp = (
             datetime.now()
-            - relativedelta(months=self.initial_load_from_timestamp_months_back)
+            - relativedelta(months=self.full_load_from_timestamp_months_back)
         ).replace(microsecond=0)
 
         self.from_timestamp = None
         self.to_timestamp = None
 
+        # we define the session here so that it can be used by all the functions
+        boto3.setup_default_session(region_name=os.environ.get("REGION"))
+
         self.set_from_and_to_timestamps(as_dates=from_and_to_as_dates)
 
-        if create_schema_if_initial_load:
+        if create_schema_if_full_load:
             self.create_schema_if_not_exists()
 
     def set_from_and_to_timestamps(self, as_dates: bool = False):
         """
         Sets the start and end timestamps for the data loading based on the user-specified timestamps and default values.
 
         Args:
             as_dates: A boolean, indicating whether the start and end timestamps should be set as dates (midnight of the given date).
 
         Returns:
             None
         """
         # set from/to_timestamp to fetch all data when the table is recrated
-        if self.initial_load:
-            self.set_from_timestamp_initial_load()
+        if self.full_load:
+            self.set_from_timestamp_full_load()
 
             self.to_timestamp = datetime.now()
         else:
             self.set_from_timestamp_partial_load()
 
             if self.given_to_timestamp:
                 self.to_timestamp = dateTimeMethods.get_timestamp(
@@ -103,38 +105,38 @@
             )
             self.to_timestamp = self.to_timestamp.replace(
                 hour=0, minute=0, second=0, microsecond=0
             )
 
         self.validate_from_and_to_timestamp()
 
-    def set_from_timestamp_initial_load(self):
-        """Sets the from_timestamp for initial load.
+    def set_from_timestamp_full_load(self):
+        """Sets the from_timestamp for full load.
 
-        If `initial_load_from_timestamp` is given, it is used as the `from_timestamp`.
-        If not, the `from_timestamp` is calculated as `initial_load_from_timestamp_months_back` months back from today.
+        If `full_load_from_timestamp` is given, it is used as the `from_timestamp`.
+        If not, the `from_timestamp` is calculated as `full_load_from_timestamp_months_back` months back from today.
         The information about the process is logged.
 
         Returns:
             None
         """
         logging.info(
-            "initial_load is True, so from_timestamp and to_timestamp will be assigned with default values to fetch all data"
+            "full_load is True, so from_timestamp and to_timestamp will be assigned with default values to fetch all data"
         )
-        if self.initial_load_from_timestamp:
+        if self.full_load_from_timestamp:
             logging.info(
-                f"initial_load_from_timestamp is given and will be used as the from_timestamp: {self.initial_load_from_timestamp}"
+                f"full_load_from_timestamp is given and will be used as the from_timestamp: {self.full_load_from_timestamp}"
             )
             self.from_timestamp = dateTimeMethods.get_timestamp(
-                self.initial_load_from_timestamp
+                self.full_load_from_timestamp
             )
         else:
             self.from_timestamp = self.default_from_timestamp
             logging.info(
-                f"initial_load_from_timestamp was NOT given, from_timestamp will be {self.initial_load_from_timestamp_months_back} month back from today: {self.from_timestamp}"
+                f"full_load_from_timestamp was NOT given, from_timestamp will be {self.full_load_from_timestamp_months_back} month back from today: {self.from_timestamp}"
             )
 
     def set_from_timestamp_partial_load(self):
         """Sets the from_timestamp for partial load.
 
         If `given_from_timestamp` is given, it is used as the `from_timestamp`.
         If not, the `from_timestamp` is calculated as the maximum timestamp in the `tbl_to_check_max_timestamp` table in the Athena database.
@@ -172,19 +174,19 @@
         else:
             logging.info(
                 f"fetching data from: {self.from_timestamp} until: {self.to_timestamp}"
             )
 
     def create_schema_if_not_exists(self):
         """
-        Check if the "initial_load" attribute is set to True and create the destination schema if it doesn't exist yet.
+        Check if the "full_load" attribute is set to True and create the destination schema if it doesn't exist yet.
 
         Returns:
             None
         """
-        if self.initial_load:
+        if self.full_load:
             logging.info(
-                f"initial load is True. the schema {self.dest_schema} will be created if not exist yet"
+                f"full load is True. the schema {self.dest_schema} will be created if not exist yet"
             )
             wr.athena.start_query_execution(
                 f"create database if not exists {self.dest_schema}"
             )
```

### Comparing `gad_common_utils-0.24/common_utils/data_type_conversion.py` & `gad_common_utils-0.25/common_utils/data_type_conversion.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.24/common_utils/date_time_methods.py` & `gad_common_utils-0.25/common_utils/date_time_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,16 @@
 
         logging.info(f"get the max timestamp from {tbl_name}")
         try:
             df = wr.athena.read_sql_query(
                 sql=f"""select coalesce(max({col_name}), timestamp'{default_from_timestamp}') as max_timestamp from {tbl_name}""",
                 database=database,
                 workgroup=workgroup,
-                ctas_approach=False,
             )
+
             max_timestamp = df["max_timestamp"][0]
 
         except Exception as e:
             if "does not exist" in str(e):
                 if "Table" in str(e):
                     logging.warning(
                         f"the table/view {database}.{tbl_name} doesn't exist"
```

### Comparing `gad_common_utils-0.24/common_utils/dynamodb_methods.py` & `gad_common_utils-0.25/common_utils/dynamodb_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.24/common_utils/files_methods.py` & `gad_common_utils-0.25/common_utils/files_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.24/common_utils/gad_utils.py` & `gad_common_utils-0.25/common_utils/gad_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import json
+import ast
 import os
 from datetime import timedelta
 
 from airflow import DAG
 from airflow.contrib.operators.kubernetes_pod_operator import KubernetesPodOperator
 from airflow.operators.python_operator import PythonOperator
 from airflow.utils.dates import days_ago
@@ -76,14 +76,15 @@
 
 def generate_airflow_dag(
     project: str,
     dag_id: str,
     schedule_interval,
     tasks: list,
     content_path: str = "gad-deliveries",
+    dag_params: dict = {},
 ):
     """
     Creates a DAG using the specified parameters.
 
     Args:
         project (str): The name of the project.
         dag_id (str): The ID of the DAG.
@@ -148,15 +149,17 @@
                 value = (
                     "{{ ti.xcom_pull(task_ids=['"
                     + task_id
                     + "_service_task'], key='"
                     + xcom
                     + "') }}"
                 )
-                return_dict[xcom] = value
+                return_dict[xcom] = value.replace("[", "").replace(
+                    "]", ""
+                )  # this is MANDATORY to make sure we get the right value from XCOM (using [1:-1] doesn't work)
         return return_dict
 
     def return_cmds(task_dict: dict) -> list:
         """Returns a list of command-line commands based on task_dict.
 
         Args:
         task_dict: A dictionary containing information about the task to be executed.
@@ -175,99 +178,94 @@
         'executable' key of the task_dict.
         """
         if task_dict["task_type"] == "dbt":
             return ["dbt", task_dict["executable"]]
         elif task_dict["task_type"] == "python":
             return ["python", f"{paths['PYTHON_DIR']}/{task_dict['executable']}.py"]
 
-    def return_command_args(task_dict: dict, configs: dict) -> list:
+    def return_command_args(task_dict: dict, xcom_pull_task_id: str) -> list:
         """Returns a list of command-line arguments based on task_dict and configs.
 
         Args:
-        task_dict: A dictionary containing information about the task to be executed.
+        task_dict: dict
+        A dictionary containing information about the task to be executed.
                 The dictionary must have 'task_type' key with value 'dbt' or 'python'.
                 If 'task_type' is 'dbt', then the dictionary must have 'dbt_models' key
                 with a list of strings containing the names of dbt models to be executed.
 
-        configs: A dictionary containing configuration values for the task.
-                If the task is of type 'dbt', then the dictionary can have 'dbt_vars' key
-                with a string value containing the variable values to be passed to dbt.
-                If the task is of type 'python', then the dictionary can have 'python_args'
-                key with a list of strings containing command-line arguments for the python script.
+        xcom_pull_task_id: str
+        The task ID of either the digest_args_task or the last service task that pushed data to XCom.
 
         Returns:
         A list of command-line arguments based on the task and configuration values.
         If task_type is 'dbt', then the returned list will contain arguments for dbt models
         and default dbt arguments such as project-dir, profiles-dir, target-path, and log-path.
         If task_type is 'python', then the returned list will contain arguments specified
         in the 'python_args' key of the configs dictionary.
         """
 
-        xcom_val = extract_xcom_data(task_dict)
-
         if task_dict["task_type"] == "dbt":
             dbt_default_args = [
                 "--project-dir",
                 paths["DBT_DIR"],
                 "--profiles-dir",
                 paths["DBT_DIR"],
                 "--target-path",
                 paths["DBT_OUTPUT_DIR"],
                 "--log-path",
                 paths["DBT_OUTPUT_DIR"],
             ]
 
-            dbt_default_args_and_models = task_dict["dbt_models"] + dbt_default_args
+            # get the latest version of dbt vars from XCOM
+            dbt_vars = (
+                (
+                    "{{ ti.xcom_pull(task_ids=['"
+                    + xcom_pull_task_id
+                    + "'], key='dbt_vars') }}"
+                )
+                .replace(
+                    "[", ""
+                )  # this is MANDATORY to make sure we get the right value from XCOM (using [1:-1] doesn't work)
+                .replace(
+                    "]", ""
+                )  # this is MANDATORY to make sure we get the right value from XCOM (using [1:-1] doesn't work)
+            )
 
-            dbt_vars = configs.get("dbt_vars")
-            if dbt_vars:
-                dbt_vars.update(xcom_val)
-                dbt_all_args = dbt_default_args_and_models + [
-                    "--vars",
-                    json.dumps(dbt_vars),
-                ]
-            elif bool(xcom_val):
-                dbt_all_args = dbt_default_args_and_models + [
-                    "--vars",
-                    json.dumps(xcom_val),
-                ]
-            else:
-                dbt_all_args = dbt_default_args_and_models
+            dbt_all_args = (
+                task_dict["dbt_models"] + dbt_default_args + ["--vars", dbt_vars]
+            )
 
             return dbt_all_args
 
         elif task_dict["task_type"] == "python":
-            if configs.get("python_args"):
-                python_args = configs.get("python_args")
-            else:
-                python_args = {}
-            python_args.update(xcom_val)
             list_args = []
-            if python_args:
-                for key in python_args:
-                    list_args.append(f"--{key}")
-                    if python_args[key]:
-                        list_args.append(python_args[key])
-            return list_args
-
-    def return_configs() -> dict:
-        """
-        Returns the dictionary of configurations read from a JSON file.
-
-        Parameters:
-        None
-
-        Returns:
-        dict: A dictionary containing the configurations read from the JSON file located in the CONFIG_DIR directory.
+            # iterate over the non-empty dag_params, pull them from XCOM ands add them to the list
+            for key in dag_params_not_empty:
+                list_args.append(f"--{key}")
+                list_args.append(
+                    (
+                        "{{ ti.xcom_pull(task_ids=['digest_args_task'], key='"
+                        + key
+                        + "') }}"
+                    )
+                    .replace(
+                        "[", ""
+                    )  # this is MANDATORY to make sure we get the right value from XCOM (using [1:-1] doesn't work)
+                    .replace(
+                        "]", ""
+                    )  # this is MANDATORY to make sure we get the right value from XCOM (using [1:-1] doesn't work)
+                )
 
-        """
+            # get the xcom values
+            xcom_val = extract_xcom_data(task_dict)
+            for key, val in xcom_val.items():
+                list_args.append(f"--{key}")
+                list_args.append(val)
 
-        with open(f"{paths['CONFIG_DIR']}/config.json", "r") as f:
-            j = f.read()
-        return json.loads(j)
+            return list_args
 
     def parse_xcoms(task_id, **kwargs):
         """
         This function extracts XCom data from a specified task instance and pushes the data to XCom with individual keys.
 
         Parameters:
             task_id (str): The ID of the task instance from which to extract XCom data.
@@ -275,30 +273,80 @@
                     provides the task instance.
 
         Returns:
             None
         """
         task_instance = kwargs["ti"]
         value = task_instance.xcom_pull(task_ids=task_id)
-        for i in value[0][0].keys():
-            print("xcom push", "key", i, "val", value[0][0][i])
-            task_instance.xcom_push(key=i, value=value[0][0][i])
+
+        for key in value[0][0].keys():
+            print("xcom push", "key", key, "val", value[0][0][key])
+
+            # pull initial dbt_vars from xcom
+            dbt_vars_dict = task_instance.xcom_pull(
+                task_ids=["digest_args_task"], key="dbt_vars"
+            )[0]
+            # add new dbt vars from XCOM of another task to dbt_vars_dict
+            dbt_vars_dict[key] = value[0][0][key]
+
+            # push individual xcoms for python use
+            task_instance.xcom_push(key=key, value=value[0][0][key])
+
+        # push dbt_vars back to xcom
+        task_instance.xcom_push(key="dbt_vars", value=dbt_vars_dict)
+
+    def digest_args(given_args: str, default_args: str, **kwargs):
+        """
+        Process and store arguments for further use.
+
+        Args:
+            given_args (str): A string representing the given arguments.
+            default_args (str): A string representing the default arguments.
+            **kwargs: Additional keyword arguments.
+
+        Returns:
+            None
+        """
+        print(f"The given args: {given_args}")
+        print(f"The default args: {default_args}")
+
+        # convert both set of args from string to dict
+        given_args_dict = ast.literal_eval(given_args)
+        default_args_dict = ast.literal_eval(default_args)
+
+        args_to_use = {}
+        if given_args_dict:
+            print("There are some given args, using given args")
+            args_to_use = given_args_dict
+        else:
+            print("There are NO given args, using default args")
+            args_to_use = default_args_dict
+
+        # create a dict of non-empty dbt vars and push to xcom
+        dbt_vars = {key: str(val) for key, val in args_to_use.items() if val != ""}
+        kwargs["ti"].xcom_push(key="dbt_vars", value=dbt_vars)
+
+        # push each python arg to xcom
+        for arg in args_to_use:
+            if args_to_use[arg] != "":
+                kwargs["ti"].xcom_push(key=arg, value=args_to_use[arg])
+
+    # use only the params that are not empty
+    dag_params_not_empty = {key: val for key, val in dag_params.items() if val != ""}
 
     # dag creation
     dag = DAG(
         dag_id=dag_id,
         default_args=default_args,
         schedule_interval=schedule_interval,
         max_active_runs=1,
         concurrency=10,
+        params=dag_params,
     )
 
-    configs = return_configs()
-    env_vars = configs.get("env_vars")
-
     """
     This code is a loop that iterates over a list of tasks and creates a KubernetesPodOperator object for each task.
     return_command_args() function is used to obtain the command arguments for the task.
     return_image_name() function is used to get the image name based on the task type.
     return_configs() function is used to get environment variables.
     The KubernetesPodOperator object is then created using these variables and appended to a dictionary named kubernetes_tasks with the task ID as the key.
     """
@@ -325,36 +373,40 @@
         if i > 0:
             if "service" in new_tasks_list[i - 1].keys():
                 new_tasks_list[i]["upstream"] = [new_tasks_list[i - 1]["task_id"]]
 
     # Define a dictionary to store KubernetesPodOperator and PythonOperator tasks
     kubernetes_tasks = {}
 
+    # this variable is used to store the task id of the last task that updated the dbt_vars key in xcom. It can be either "digest_args_task" or a service task. If there are no service tasks - it will be "digest_args_task"
+    last_service_task_id = "digest_args_task"
+
     # Iterate through each task in the new list and create a KubernetesPodOperator or PythonOperator task based on its properties
     for task in new_tasks_list:
         # If the task is a service task, create a PythonOperator with parse_xcoms function as its callable
         if "service" in task.keys():
             service_task = PythonOperator(
                 task_id=task["task_id"],
                 python_callable=parse_xcoms,
                 op_args=[task["upstream"]],
                 dag=dag,
             )
             kubernetes_tasks[task["task_id"]] = service_task
+            last_service_task_id = task["task_id"]
 
         # If the task is not a service task, create a KubernetesPodOperator
         else:
             cmds = return_cmds(task)
-            arguments = return_command_args(task, configs)
+            arguments = return_command_args(task, last_service_task_id)
             image = return_image_name(task["task_type"])
 
             kubernetes_task = KubernetesPodOperator(
                 volumes=volumes,
                 volume_mounts=volumes_mounts,
-                env_vars=env_vars,
+                env_vars=[],
                 env_from=[envConfigMap],
                 namespace="default",
                 labels={"Task": task["task_type"]},
                 image_pull_policy="Never",
                 name=task["task_id"],
                 task_id=task["task_id"],
                 is_delete_operator_pod=True,
@@ -363,21 +415,33 @@
                 cmds=cmds,
                 arguments=arguments,
                 dag=dag,
                 do_xcom_push=is_xcom_push_task(task),
             )
             kubernetes_tasks[task["task_id"]] = kubernetes_task
 
+    # Define an empty list to store tasks without upstream dependencies, so we will set
+    # the digest_args_task as their upstream
+    tasks_without_upstream = []
+
     # using the tasks list, and the kubernetes_tasks dictionary - this loop creates the dependancies.
     # each task in tasks contains a value in the 'upstream' key that tells what is the pervious task (or tasks).
     # the kubernates operator created gets the dependancies and is configured to use them with the set_upstream setting.
-
     for task in new_tasks_list:
         if task["upstream"] is None or task["upstream"] == "" or task["upstream"] == []:
+            tasks_without_upstream.append(kubernetes_tasks[task["task_id"]])
             pass
         else:
             dependancies = []
             for t in task["upstream"]:
                 dependancies.append(kubernetes_tasks[t])
             kubernetes_tasks[task["task_id"]].set_upstream(dependancies)
 
+    # define the digest_args_task and set it as upstream for all tasks without upstream dependencies
+    digest_args_task = PythonOperator(
+        task_id="digest_args_task",
+        python_callable=digest_args,
+        op_kwargs={"given_args": "{{ dag_run.conf }}", "default_args": "{{ params }}"},
+        dag=dag,
+    ).set_downstream(tasks_without_upstream)
+
     return dag
```

### Comparing `gad_common_utils-0.24/common_utils/gad_utils_additionals.py` & `gad_common_utils-0.25/common_utils/gad_utils_additionals.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.24/common_utils/json_schema_methods.py` & `gad_common_utils-0.25/common_utils/json_schema_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.24/common_utils/run_athena_query.py` & `gad_common_utils-0.25/common_utils/run_athena_query.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.24/common_utils/s3_methods.py` & `gad_common_utils-0.25/common_utils/s3_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.24/common_utils/sql_methods.py` & `gad_common_utils-0.25/common_utils/sql_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.24/common_utils/string_transformations.py` & `gad_common_utils-0.25/common_utils/string_transformations.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.24/gad_common_utils.egg-info/PKG-INFO` & `gad_common_utils-0.25/gad_common_utils.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gad-common-utils
-Version: 0.24
+Version: 0.25
 Summary: gad utility
 Project-URL: Homepage, http://gad-co.ml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `gad_common_utils-0.24/gad_common_utils.egg-info/SOURCES.txt` & `gad_common_utils-0.25/gad_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.24/pyproject.toml` & `gad_common_utils-0.25/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.24/tests/test_json_schema_methods.py` & `gad_common_utils-0.25/tests/test_json_schema_methods.py`

 * *Files identical despite different names*

