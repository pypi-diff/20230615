# Comparing `tmp/dagster-azure-0.9.9.tar.gz` & `tmp/dagster-azure-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-azure-0.9.9.tar", last modified: Thu Sep 17 21:28:27 2020, max compression
+gzip compressed data, was "dist/dagster-azure-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:31 2020, max compression
```

## Comparing `dagster-azure-0.9.9.tar` & `dagster-azure-0.9.9rc1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:27.000000 dagster-azure-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)      173 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      611 2020-09-17 21:28:27.000000 dagster-azure-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      125 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:27.000000 dagster-azure-0.9.9/dagster_azure/
--rw-r--r--   0 bobchen    (501) staff       (20)      156 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:27.000000 dagster-azure-0.9.9/dagster_azure/adls2/
--rw-r--r--   0 bobchen    (501) staff       (20)      629 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure/adls2/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4669 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure/adls2/fake_adls2_resource.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2881 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure/adls2/file_cache.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3744 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure/adls2/file_manager.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1525 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure/adls2/intermediate_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)     5880 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure/adls2/object_store.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4200 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure/adls2/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)     5236 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure/adls2/system_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1154 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure/adls2/utils.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:27.000000 dagster-azure-0.9.9/dagster_azure/blob/
--rw-r--r--   0 bobchen    (501) staff       (20)      150 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure/blob/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     7816 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure/blob/compute_log_manager.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4805 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure/blob/fake_blob_client.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1258 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure/blob/utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:27.000000 dagster-azure-0.9.9/dagster_azure.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      611 2020-09-17 21:28:27.000000 dagster-azure-0.9.9/dagster_azure.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)     1210 2020-09-17 21:28:27.000000 dagster-azure-0.9.9/dagster_azure.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:27.000000 dagster-azure-0.9.9/dagster_azure.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       62 2020-09-17 21:28:27.000000 dagster-azure-0.9.9/dagster_azure.egg-info/entry_points.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:27.000000 dagster-azure-0.9.9/dagster_azure.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       71 2020-09-17 21:28:27.000000 dagster-azure-0.9.9/dagster_azure.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:28:27.000000 dagster-azure-0.9.9/dagster_azure.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:27.000000 dagster-azure-0.9.9/dagster_azure_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure_tests/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:27.000000 dagster-azure-0.9.9/dagster_azure_tests/adls2_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure_tests/adls2_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      307 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure_tests/adls2_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1881 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure_tests/adls2_tests/test_adls2_file_cache.py
--rw-r--r--   0 bobchen    (501) staff       (20)     7518 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure_tests/adls2_tests/test_adls2_file_manager.py
--rw-r--r--   0 bobchen    (501) staff       (20)    18490 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure_tests/adls2_tests/test_intermediate_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1636 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure_tests/adls2_tests/test_object_store.py
--rw-r--r--   0 bobchen    (501) staff       (20)       91 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/dagster_azure_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:28:27.000000 dagster-azure-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1295 2020-09-17 21:24:45.000000 dagster-azure-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/LICENSE
+-rw-r--r--   0 bobchen    (501) staff       (20)      173 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/MANIFEST.in
+-rw-r--r--   0 bobchen    (501) staff       (20)      614 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      125 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure/
+-rw-r--r--   0 bobchen    (501) staff       (20)      156 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/__init__.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure/adls2/
+-rw-r--r--   0 bobchen    (501) staff       (20)      629 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/adls2/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     4669 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/adls2/fake_adls2_resource.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2881 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/adls2/file_cache.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     3744 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/adls2/file_manager.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1525 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/adls2/intermediate_storage.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     5880 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/adls2/object_store.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     4200 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/adls2/resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     5236 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/adls2/system_storage.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1154 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/adls2/utils.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure/blob/
+-rw-r--r--   0 bobchen    (501) staff       (20)      150 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/blob/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     7816 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/blob/compute_log_manager.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     4805 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/blob/fake_blob_client.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1258 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/blob/utils.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      614 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)     1210 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       62 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure.egg-info/entry_points.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)       71 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure_tests/__init__.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure_tests/adls2_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure_tests/adls2_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      307 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure_tests/adls2_tests/conftest.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1881 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure_tests/adls2_tests/test_adls2_file_cache.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     7518 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure_tests/adls2_tests/test_adls2_file_manager.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    18490 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure_tests/adls2_tests/test_intermediate_storage.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1636 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure_tests/adls2_tests/test_object_store.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       91 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure_tests/test_version.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1295 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/setup.py
```

### Comparing `dagster-azure-0.9.9/LICENSE` & `dagster-azure-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-azure-0.9.9/PKG-INFO` & `dagster-azure-0.9.9rc1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-azure
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for Azure-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-azure
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-azure-0.9.9/dagster_azure/adls2/__init__.py` & `dagster-azure-0.9.9rc1/dagster_azure/adls2/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-azure-0.9.9/dagster_azure/adls2/fake_adls2_resource.py` & `dagster-azure-0.9.9rc1/dagster_azure/adls2/fake_adls2_resource.py`

 * *Files identical despite different names*

### Comparing `dagster-azure-0.9.9/dagster_azure/adls2/file_cache.py` & `dagster-azure-0.9.9rc1/dagster_azure/adls2/file_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-azure-0.9.9/dagster_azure/adls2/file_manager.py` & `dagster-azure-0.9.9rc1/dagster_azure/adls2/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-azure-0.9.9/dagster_azure/adls2/intermediate_storage.py` & `dagster-azure-0.9.9rc1/dagster_azure/adls2/intermediate_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-azure-0.9.9/dagster_azure/adls2/object_store.py` & `dagster-azure-0.9.9rc1/dagster_azure/adls2/object_store.py`

 * *Files identical despite different names*

### Comparing `dagster-azure-0.9.9/dagster_azure/adls2/resources.py` & `dagster-azure-0.9.9rc1/dagster_azure/adls2/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-azure-0.9.9/dagster_azure/adls2/system_storage.py` & `dagster-azure-0.9.9rc1/dagster_azure/adls2/system_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-azure-0.9.9/dagster_azure/adls2/utils.py` & `dagster-azure-0.9.9rc1/dagster_azure/adls2/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-azure-0.9.9/dagster_azure/blob/compute_log_manager.py` & `dagster-azure-0.9.9rc1/dagster_azure/blob/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-azure-0.9.9/dagster_azure/blob/fake_blob_client.py` & `dagster-azure-0.9.9rc1/dagster_azure/blob/fake_blob_client.py`

 * *Files identical despite different names*

### Comparing `dagster-azure-0.9.9/dagster_azure/blob/utils.py` & `dagster-azure-0.9.9rc1/dagster_azure/blob/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-azure-0.9.9/dagster_azure.egg-info/PKG-INFO` & `dagster-azure-0.9.9rc1/dagster_azure.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-azure
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for Azure-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-azure
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-azure-0.9.9/dagster_azure.egg-info/SOURCES.txt` & `dagster-azure-0.9.9rc1/dagster_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-azure-0.9.9/dagster_azure_tests/adls2_tests/test_adls2_file_cache.py` & `dagster-azure-0.9.9rc1/dagster_azure_tests/adls2_tests/test_adls2_file_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-azure-0.9.9/dagster_azure_tests/adls2_tests/test_adls2_file_manager.py` & `dagster-azure-0.9.9rc1/dagster_azure_tests/adls2_tests/test_adls2_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-azure-0.9.9/dagster_azure_tests/adls2_tests/test_intermediate_storage.py` & `dagster-azure-0.9.9rc1/dagster_azure_tests/adls2_tests/test_intermediate_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-azure-0.9.9/dagster_azure_tests/adls2_tests/test_object_store.py` & `dagster-azure-0.9.9rc1/dagster_azure_tests/adls2_tests/test_object_store.py`

 * *Files identical despite different names*

### Comparing `dagster-azure-0.9.9/setup.py` & `dagster-azure-0.9.9rc1/setup.py`

 * *Files identical despite different names*

