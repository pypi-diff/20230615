# Comparing `tmp/gad_common_utils-0.25.tar.gz` & `tmp/gad_common_utils-0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gad_common_utils-0.25.tar", last modified: Thu Jun 15 20:05:58 2023, max compression
+gzip compressed data, was "gad_common_utils-0.26.tar", last modified: Thu Jun 15 21:13:38 2023, max compression
```

## Comparing `gad_common_utils-0.25.tar` & `gad_common_utils-0.26.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:05:58.330087 gad_common_utils-0.25/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:05:58.326087 gad_common_utils-0.25/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:05:58.326087 gad_common_utils-0.25/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-15 20:05:46.000000 gad_common_utils-0.25/.github/workflows/black-format-checker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-15 20:05:46.000000 gad_common_utils-0.25/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-15 20:05:46.000000 gad_common_utils-0.25/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-15 20:05:46.000000 gad_common_utils-0.25/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-15 20:05:46.000000 gad_common_utils-0.25/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-15 20:05:58.330087 gad_common_utils-0.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-15 20:05:46.000000 gad_common_utils-0.25/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:05:58.326087 gad_common_utils-0.25/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-15 20:05:58.000000 gad_common_utils-0.25/common_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/data_loading_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/data_type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/date_time_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/dynamodb_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/dynamodb_ray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/files_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    18069 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/gad_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/gad_utils_additionals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/json_schema_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/run_athena_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/s3_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/sql_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-15 20:05:46.000000 gad_common_utils-0.25/common_utils/string_transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:05:58.326087 gad_common_utils-0.25/gad_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-15 20:05:58.000000 gad_common_utils-0.25/gad_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-15 20:05:58.000000 gad_common_utils-0.25/gad_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 20:05:58.000000 gad_common_utils-0.25/gad_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 20:05:58.000000 gad_common_utils-0.25/gad_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 20:05:58.000000 gad_common_utils-0.25/gad_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-15 20:05:46.000000 gad_common_utils-0.25/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 20:05:58.330087 gad_common_utils-0.25/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:05:58.326087 gad_common_utils-0.25/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:05:46.000000 gad_common_utils-0.25/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-15 20:05:46.000000 gad_common_utils-0.25/tests/test_json_schema_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:13:38.305853 gad_common_utils-0.26/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:13:38.297853 gad_common_utils-0.26/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:13:38.297853 gad_common_utils-0.26/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-15 21:13:25.000000 gad_common_utils-0.26/.github/workflows/black-format-checker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-15 21:13:25.000000 gad_common_utils-0.26/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-15 21:13:25.000000 gad_common_utils-0.26/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-15 21:13:25.000000 gad_common_utils-0.26/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-15 21:13:25.000000 gad_common_utils-0.26/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-15 21:13:38.305853 gad_common_utils-0.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-15 21:13:25.000000 gad_common_utils-0.26/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:13:38.301853 gad_common_utils-0.26/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-15 21:13:25.000000 gad_common_utils-0.26/common_utils/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:13:25.000000 gad_common_utils-0.26/common_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-15 21:13:38.000000 gad_common_utils-0.26/common_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-06-15 21:13:25.000000 gad_common_utils-0.26/common_utils/data_loading_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-15 21:13:25.000000 gad_common_utils-0.26/common_utils/data_type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-15 21:13:25.000000 gad_common_utils-0.26/common_utils/date_time_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-15 21:13:25.000000 gad_common_utils-0.26/common_utils/dynamodb_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-15 21:13:25.000000 gad_common_utils-0.26/common_utils/dynamodb_ray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-15 21:13:25.000000 gad_common_utils-0.26/common_utils/files_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18069 2023-06-15 21:13:25.000000 gad_common_utils-0.26/common_utils/gad_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-06-15 21:13:25.000000 gad_common_utils-0.26/common_utils/gad_utils_additionals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-06-15 21:13:25.000000 gad_common_utils-0.26/common_utils/json_schema_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-15 21:13:25.000000 gad_common_utils-0.26/common_utils/run_athena_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-06-15 21:13:25.000000 gad_common_utils-0.26/common_utils/s3_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-15 21:13:25.000000 gad_common_utils-0.26/common_utils/sql_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-15 21:13:25.000000 gad_common_utils-0.26/common_utils/string_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:13:38.305853 gad_common_utils-0.26/gad_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-15 21:13:38.000000 gad_common_utils-0.26/gad_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-15 21:13:38.000000 gad_common_utils-0.26/gad_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:13:38.000000 gad_common_utils-0.26/gad_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 21:13:38.000000 gad_common_utils-0.26/gad_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 21:13:38.000000 gad_common_utils-0.26/gad_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-15 21:13:25.000000 gad_common_utils-0.26/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 21:13:38.305853 gad_common_utils-0.26/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:13:38.305853 gad_common_utils-0.26/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:13:25.000000 gad_common_utils-0.26/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-15 21:13:25.000000 gad_common_utils-0.26/tests/test_json_schema_methods.py
```

### Comparing `gad_common_utils-0.25/.github/workflows/black-format-checker.yml` & `gad_common_utils-0.26/.github/workflows/black-format-checker.yml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.25/.github/workflows/publish-to-pypi.yml` & `gad_common_utils-0.26/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.25/.github/workflows/pytest.yml` & `gad_common_utils-0.26/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.25/PKG-INFO` & `gad_common_utils-0.26/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gad_common_utils
-Version: 0.25
+Version: 0.26
 Summary: gad utility
 Project-URL: Homepage, http://gad-co.ml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `gad_common_utils-0.25/common_utils/data_loading_management.py` & `gad_common_utils-0.26/common_utils/data_loading_management.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.25/common_utils/data_type_conversion.py` & `gad_common_utils-0.26/common_utils/data_type_conversion.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.25/common_utils/date_time_methods.py` & `gad_common_utils-0.26/common_utils/date_time_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,16 @@
 
         logging.info(f"get the max timestamp from {tbl_name}")
         try:
             df = wr.athena.read_sql_query(
                 sql=f"""select coalesce(max({col_name}), timestamp'{default_from_timestamp}') as max_timestamp from {tbl_name}""",
                 database=database,
                 workgroup=workgroup,
+                ctas_approach=False,
             )
-
             max_timestamp = df["max_timestamp"][0]
 
         except Exception as e:
             if "does not exist" in str(e):
                 if "Table" in str(e):
                     logging.warning(
                         f"the table/view {database}.{tbl_name} doesn't exist"
```

### Comparing `gad_common_utils-0.25/common_utils/dynamodb_methods.py` & `gad_common_utils-0.26/common_utils/dynamodb_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.25/common_utils/files_methods.py` & `gad_common_utils-0.26/common_utils/files_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.25/common_utils/gad_utils.py` & `gad_common_utils-0.26/common_utils/gad_utils.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.25/common_utils/gad_utils_additionals.py` & `gad_common_utils-0.26/common_utils/gad_utils_additionals.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.25/common_utils/json_schema_methods.py` & `gad_common_utils-0.26/common_utils/json_schema_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.25/common_utils/run_athena_query.py` & `gad_common_utils-0.26/common_utils/run_athena_query.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.25/common_utils/s3_methods.py` & `gad_common_utils-0.26/common_utils/s3_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.25/common_utils/sql_methods.py` & `gad_common_utils-0.26/common_utils/sql_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.25/common_utils/string_transformations.py` & `gad_common_utils-0.26/common_utils/string_transformations.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.25/gad_common_utils.egg-info/PKG-INFO` & `gad_common_utils-0.26/gad_common_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gad-common-utils
-Version: 0.25
+Version: 0.26
 Summary: gad utility
 Project-URL: Homepage, http://gad-co.ml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `gad_common_utils-0.25/gad_common_utils.egg-info/SOURCES.txt` & `gad_common_utils-0.26/gad_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.25/pyproject.toml` & `gad_common_utils-0.26/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.25/tests/test_json_schema_methods.py` & `gad_common_utils-0.26/tests/test_json_schema_methods.py`

 * *Files identical despite different names*

