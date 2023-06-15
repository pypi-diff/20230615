# Comparing `tmp/viadot-2.0a8.tar.gz` & `tmp/viadot-2.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viadot-2.0a8.tar", last modified: Wed Oct 19 19:12:47 2022, max compression
+gzip compressed data, was "viadot-2.0a9.tar", last modified: Wed Oct 19 20:51:40 2022, max compression
```

## Comparing `viadot-2.0a8.tar` & `viadot-2.0a9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 19:12:47.288920 viadot-2.0a8/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-10-19 19:12:33.000000 viadot-2.0a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7683 2022-10-19 19:12:47.288920 viadot-2.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7191 2022-10-19 19:12:33.000000 viadot-2.0a8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-10-19 19:12:33.000000 viadot-2.0a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-19 19:12:47.288920 viadot-2.0a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-10-19 19:12:33.000000 viadot-2.0a8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 19:12:47.272915 viadot-2.0a8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 19:12:33.000000 viadot-2.0a8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-10-19 19:12:33.000000 viadot-2.0a8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 19:12:47.272915 viadot-2.0a8/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 19:12:33.000000 viadot-2.0a8/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1604 2022-10-19 19:12:33.000000 viadot-2.0a8/tests/integration/test_azure_data_lake.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 19:12:47.276916 viadot-2.0a8/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 19:12:33.000000 viadot-2.0a8/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1980 2022-10-19 19:12:33.000000 viadot-2.0a8/tests/unit/test_exchange_rates.py
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-10-19 19:12:33.000000 viadot-2.0a8/tests/unit/test_sharepoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-10-19 19:12:33.000000 viadot-2.0a8/tests/unit/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 19:12:47.280918 viadot-2.0a8/viadot/
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-10-19 19:12:33.000000 viadot-2.0a8/viadot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-10-19 19:12:33.000000 viadot-2.0a8/viadot/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 19:12:47.280918 viadot-2.0a8/viadot/examples/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 19:12:33.000000 viadot-2.0a8/viadot/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-10-19 19:12:33.000000 viadot-2.0a8/viadot/examples/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-10-19 19:12:33.000000 viadot-2.0a8/viadot/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-10-19 19:12:33.000000 viadot-2.0a8/viadot/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 19:12:47.284919 viadot-2.0a8/viadot/sources/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-19 19:12:33.000000 viadot-2.0a8/viadot/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8843 2022-10-19 19:12:33.000000 viadot-2.0a8/viadot/sources/azure_data_lake.py
--rw-r--r--   0 runner    (1001) docker     (121)    11002 2022-10-19 19:12:33.000000 viadot-2.0a8/viadot/sources/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    16982 2022-10-19 19:12:33.000000 viadot-2.0a8/viadot/sources/databricks.py
--rw-r--r--   0 runner    (1001) docker     (121)     4393 2022-10-19 19:12:33.000000 viadot-2.0a8/viadot/sources/exchange_rates.py
--rw-r--r--   0 runner    (1001) docker     (121)     4410 2022-10-19 19:12:33.000000 viadot-2.0a8/viadot/sources/sharepoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     1537 2022-10-19 19:12:33.000000 viadot-2.0a8/viadot/sources/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (121)     2581 2022-10-19 19:12:33.000000 viadot-2.0a8/viadot/sources/uk_carbon_intensity.py
--rw-r--r--   0 runner    (1001) docker     (121)    14599 2022-10-19 19:12:33.000000 viadot-2.0a8/viadot/task_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    12795 2022-10-19 19:12:33.000000 viadot-2.0a8/viadot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 19:12:47.280918 viadot-2.0a8/viadot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7683 2022-10-19 19:12:47.000000 viadot-2.0a8/viadot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-10-19 19:12:47.000000 viadot-2.0a8/viadot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 19:12:47.000000 viadot-2.0a8/viadot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-10-19 19:12:47.000000 viadot-2.0a8/viadot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-19 19:12:47.000000 viadot-2.0a8/viadot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 20:51:40.801757 viadot-2.0a9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-10-19 20:51:31.000000 viadot-2.0a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     7683 2022-10-19 20:51:40.801757 viadot-2.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7191 2022-10-19 20:51:31.000000 viadot-2.0a9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      327 2022-10-19 20:51:31.000000 viadot-2.0a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-19 20:51:40.801757 viadot-2.0a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-10-19 20:51:31.000000 viadot-2.0a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 20:51:40.801757 viadot-2.0a9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 20:51:31.000000 viadot-2.0a9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-10-19 20:51:31.000000 viadot-2.0a9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 20:51:40.801757 viadot-2.0a9/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 20:51:31.000000 viadot-2.0a9/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1604 2022-10-19 20:51:31.000000 viadot-2.0a9/tests/integration/test_azure_data_lake.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 20:51:40.801757 viadot-2.0a9/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 20:51:31.000000 viadot-2.0a9/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1980 2022-10-19 20:51:31.000000 viadot-2.0a9/tests/unit/test_exchange_rates.py
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2022-10-19 20:51:31.000000 viadot-2.0a9/tests/unit/test_sharepoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-10-19 20:51:31.000000 viadot-2.0a9/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 20:51:40.801757 viadot-2.0a9/viadot/
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2022-10-19 20:51:31.000000 viadot-2.0a9/viadot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-10-19 20:51:31.000000 viadot-2.0a9/viadot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 20:51:40.801757 viadot-2.0a9/viadot/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 20:51:31.000000 viadot-2.0a9/viadot/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-10-19 20:51:31.000000 viadot-2.0a9/viadot/examples/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (121)      917 2022-10-19 20:51:31.000000 viadot-2.0a9/viadot/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-10-19 20:51:31.000000 viadot-2.0a9/viadot/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 20:51:40.801757 viadot-2.0a9/viadot/sources/
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-19 20:51:31.000000 viadot-2.0a9/viadot/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8869 2022-10-19 20:51:31.000000 viadot-2.0a9/viadot/sources/azure_data_lake.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11002 2022-10-19 20:51:31.000000 viadot-2.0a9/viadot/sources/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16982 2022-10-19 20:51:31.000000 viadot-2.0a9/viadot/sources/databricks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4393 2022-10-19 20:51:31.000000 viadot-2.0a9/viadot/sources/exchange_rates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4410 2022-10-19 20:51:31.000000 viadot-2.0a9/viadot/sources/sharepoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1537 2022-10-19 20:51:31.000000 viadot-2.0a9/viadot/sources/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2581 2022-10-19 20:51:31.000000 viadot-2.0a9/viadot/sources/uk_carbon_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14599 2022-10-19 20:51:31.000000 viadot-2.0a9/viadot/task_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12795 2022-10-19 20:51:31.000000 viadot-2.0a9/viadot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 20:51:40.801757 viadot-2.0a9/viadot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7683 2022-10-19 20:51:40.000000 viadot-2.0a9/viadot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      819 2022-10-19 20:51:40.000000 viadot-2.0a9/viadot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 20:51:40.000000 viadot-2.0a9/viadot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-10-19 20:51:40.000000 viadot-2.0a9/viadot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-19 20:51:40.000000 viadot-2.0a9/viadot.egg-info/top_level.txt
```

### Comparing `viadot-2.0a8/LICENSE` & `viadot-2.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `viadot-2.0a8/PKG-INFO` & `viadot-2.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viadot
-Version: 2.0a8
+Version: 2.0a9
 Summary: A simple data ingestion library to guide data flows from some places to other places
 Home-page: https://github.com/dyvenia/viadot
 Author: Alessio Civitillo
 Maintainer: Michal Zawadzki
 Maintainer-email: mzawadzki@dyvenia.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: viadot Version: 2.0a8 Summary: A simple data
+Metadata-Version: 2.1 Name: viadot Version: 2.0a9 Summary: A simple data
 ingestion library to guide data flows from some places to other places Home-
 page: https://github.com/dyvenia/viadot Author: Alessio Civitillo Maintainer:
 Michal Zawadzki Maintainer-email: mzawadzki@dyvenia.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE # Viadot [![build status](https://github.com/
 dyvenia/viadot/actions/workflows/build.yml/badge.svg)](https://github.com/
```

### Comparing `viadot-2.0a8/README.md` & `viadot-2.0a9/README.md`

 * *Files identical despite different names*

### Comparing `viadot-2.0a8/setup.py` & `viadot-2.0a9/setup.py`

 * *Files identical despite different names*

### Comparing `viadot-2.0a8/tests/conftest.py` & `viadot-2.0a9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `viadot-2.0a8/tests/integration/test_azure_data_lake.py` & `viadot-2.0a9/tests/integration/test_azure_data_lake.py`

 * *Files identical despite different names*

### Comparing `viadot-2.0a8/tests/unit/test_exchange_rates.py` & `viadot-2.0a9/tests/unit/test_exchange_rates.py`

 * *Files identical despite different names*

### Comparing `viadot-2.0a8/tests/unit/test_utils.py` & `viadot-2.0a9/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `viadot-2.0a8/viadot/config.py` & `viadot-2.0a9/viadot/config.py`

 * *Files identical despite different names*

### Comparing `viadot-2.0a8/viadot/examples/hello_world.py` & `viadot-2.0a9/viadot/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `viadot-2.0a8/viadot/exceptions.py` & `viadot-2.0a9/viadot/exceptions.py`

 * *Files identical despite different names*

### Comparing `viadot-2.0a8/viadot/sources/azure_data_lake.py` & `viadot-2.0a9/viadot/sources/azure_data_lake.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,14 +264,14 @@
             raise ValueError(msg)
 
         file_name = path.split("/")[-1]
         if extension == "csv":
             # Can do it simply like this if ADLS accesses are set up correctly
             # url = os.path.join(self.base_url, path)
             # df.to_csv(url, storage_options=self.storage_options)
-            df.to_csv(file_name)
+            df.to_csv(file_name, index=False)
         else:
-            df.to_parquet(file_name)
+            df.to_parquet(file_name, index=False)
 
         self.upload(from_path=file_name, to_path=path, overwrite=overwrite)
 
         os.remove(file_name)
```

### Comparing `viadot-2.0a8/viadot/sources/base.py` & `viadot-2.0a9/viadot/sources/base.py`

 * *Files identical despite different names*

### Comparing `viadot-2.0a8/viadot/sources/databricks.py` & `viadot-2.0a9/viadot/sources/databricks.py`

 * *Files identical despite different names*

### Comparing `viadot-2.0a8/viadot/sources/exchange_rates.py` & `viadot-2.0a9/viadot/sources/exchange_rates.py`

 * *Files identical despite different names*

### Comparing `viadot-2.0a8/viadot/sources/sharepoint.py` & `viadot-2.0a9/viadot/sources/sharepoint.py`

 * *Files identical despite different names*

### Comparing `viadot-2.0a8/viadot/sources/sqlite.py` & `viadot-2.0a9/viadot/sources/sqlite.py`

 * *Files identical despite different names*

### Comparing `viadot-2.0a8/viadot/sources/uk_carbon_intensity.py` & `viadot-2.0a9/viadot/sources/uk_carbon_intensity.py`

 * *Files identical despite different names*

### Comparing `viadot-2.0a8/viadot/task_utils.py` & `viadot-2.0a9/viadot/task_utils.py`

 * *Files identical despite different names*

### Comparing `viadot-2.0a8/viadot/utils.py` & `viadot-2.0a9/viadot/utils.py`

 * *Files identical despite different names*

### Comparing `viadot-2.0a8/viadot.egg-info/PKG-INFO` & `viadot-2.0a9/viadot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viadot
-Version: 2.0a8
+Version: 2.0a9
 Summary: A simple data ingestion library to guide data flows from some places to other places
 Home-page: https://github.com/dyvenia/viadot
 Author: Alessio Civitillo
 Maintainer: Michal Zawadzki
 Maintainer-email: mzawadzki@dyvenia.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: viadot Version: 2.0a8 Summary: A simple data
+Metadata-Version: 2.1 Name: viadot Version: 2.0a9 Summary: A simple data
 ingestion library to guide data flows from some places to other places Home-
 page: https://github.com/dyvenia/viadot Author: Alessio Civitillo Maintainer:
 Michal Zawadzki Maintainer-email: mzawadzki@dyvenia.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE # Viadot [![build status](https://github.com/
 dyvenia/viadot/actions/workflows/build.yml/badge.svg)](https://github.com/
```

### Comparing `viadot-2.0a8/viadot.egg-info/SOURCES.txt` & `viadot-2.0a9/viadot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

