# Comparing `tmp/dagster-gcp-0.9.9.tar.gz` & `tmp/dagster-gcp-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-gcp-0.9.9.tar", last modified: Thu Sep 17 21:28:43 2020, max compression
+gzip compressed data, was "dist/dagster-gcp-0.9.9rc1.tar", last modified: Thu Sep 17 21:07:28 2020, max compression
```

## Comparing `dagster-gcp-0.9.9.tar` & `dagster-gcp-0.9.9rc1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:43.000000 dagster-gcp-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       16 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      629 2020-09-17 21:28:43.000000 dagster-gcp-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      119 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:43.000000 dagster-gcp-0.9.9/dagster_gcp/
--rw-r--r--   0 bobchen    (501) staff       (20)      877 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:43.000000 dagster-gcp-0.9.9/dagster_gcp/bigquery/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/bigquery/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    14635 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/bigquery/configs.py
--rw-r--r--   0 bobchen    (501) staff       (20)      304 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/bigquery/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)     6066 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/bigquery/solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4405 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/bigquery/types.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:43.000000 dagster-gcp-0.9.9/dagster_gcp/dataproc/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/dataproc/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1280 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/dataproc/configs.py
--rw-r--r--   0 bobchen    (501) staff       (20)    42391 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/dataproc/configs_dataproc_cluster.py
--rw-r--r--   0 bobchen    (501) staff       (20)    30599 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/dataproc/configs_dataproc_job.py
--rw-r--r--   0 bobchen    (501) staff       (20)     5167 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/dataproc/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1537 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/dataproc/solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)       41 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/dataproc/types.py
--rw-r--r--   0 bobchen    (501) staff       (20)      692 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/dataproc/types_dataproc_cluster.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1735 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/dataproc/types_dataproc_job.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:43.000000 dagster-gcp-0.9.9/dagster_gcp/gcs/
--rw-r--r--   0 bobchen    (501) staff       (20)      170 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/gcs/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3367 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/gcs/file_manager.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1270 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/gcs/intermediate_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4495 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/gcs/object_store.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1244 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/gcs/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2563 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/gcs/system_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:43.000000 dagster-gcp-0.9.9/dagster_gcp.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      629 2020-09-17 21:28:43.000000 dagster-gcp-0.9.9/dagster_gcp.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)     1587 2020-09-17 21:28:43.000000 dagster-gcp-0.9.9/dagster_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:43.000000 dagster-gcp-0.9.9/dagster_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:43.000000 dagster-gcp-0.9.9/dagster_gcp.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)      165 2020-09-17 21:28:43.000000 dagster-gcp-0.9.9/dagster_gcp.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       30 2020-09-17 21:28:43.000000 dagster-gcp-0.9.9/dagster_gcp.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:43.000000 dagster-gcp-0.9.9/dagster_gcp_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp_tests/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:43.000000 dagster-gcp-0.9.9/dagster_gcp_tests/bigquery_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp_tests/bigquery_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    11092 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp_tests/bigquery_tests/test_solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1972 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp_tests/bigquery_tests/test_types.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:43.000000 dagster-gcp-0.9.9/dagster_gcp_tests/dataproc_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp_tests/dataproc_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4826 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp_tests/dataproc_tests/test_resources.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:43.000000 dagster-gcp-0.9.9/dagster_gcp_tests/gcs_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp_tests/gcs_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      103 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp_tests/gcs_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2506 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp_tests/gcs_tests/test_gcs_file_manager.py
--rw-r--r--   0 bobchen    (501) staff       (20)    16628 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp_tests/gcs_tests/test_intermediate_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)      961 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp_tests/gcs_tests/test_object_store.py
--rw-r--r--   0 bobchen    (501) staff       (20)      566 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp_tests/gcs_tests/test_resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       89 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/dagster_gcp_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:28:43.000000 dagster-gcp-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1431 2020-09-17 21:24:45.000000 dagster-gcp-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/LICENSE
+-rw-r--r--   0 bobchen    (501) staff       (20)       16 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/MANIFEST.in
+-rw-r--r--   0 bobchen    (501) staff       (20)      632 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      119 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp/
+-rw-r--r--   0 bobchen    (501) staff       (20)      877 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/__init__.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp/bigquery/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/bigquery/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    14635 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/bigquery/configs.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      304 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/bigquery/resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     6066 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/bigquery/solids.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     4405 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/bigquery/types.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1280 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/configs.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    42391 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/configs_dataproc_cluster.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    30599 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/configs_dataproc_job.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     5167 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1537 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/solids.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       41 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/types.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      692 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/types_dataproc_cluster.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1735 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/types_dataproc_job.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp/gcs/
+-rw-r--r--   0 bobchen    (501) staff       (20)      170 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/gcs/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     3367 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/gcs/file_manager.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1270 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/gcs/intermediate_storage.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     4495 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/gcs/object_store.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1244 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/gcs/resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2563 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/gcs/system_storage.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      632 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)     1587 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)      165 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       30 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/__init__.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/bigquery_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/bigquery_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    11092 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/bigquery_tests/test_solids.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1972 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/bigquery_tests/test_types.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/dataproc_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/dataproc_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     4826 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/dataproc_tests/test_resources.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/gcs_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/gcs_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      103 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/gcs_tests/conftest.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2506 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/gcs_tests/test_gcs_file_manager.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    16628 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/gcs_tests/test_intermediate_storage.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      961 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/gcs_tests/test_object_store.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      566 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/gcs_tests/test_resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       89 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/dagster_gcp_tests/test_version.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:07:28.000000 dagster-gcp-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1431 2020-09-17 21:04:59.000000 dagster-gcp-0.9.9rc1/setup.py
```

### Comparing `dagster-gcp-0.9.9/LICENSE` & `dagster-gcp-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/PKG-INFO` & `dagster-gcp-0.9.9rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-gcp
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for GCP-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-gcp-0.9.9/dagster_gcp/__init__.py` & `dagster-gcp-0.9.9rc1/dagster_gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp/bigquery/configs.py` & `dagster-gcp-0.9.9rc1/dagster_gcp/bigquery/configs.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp/bigquery/solids.py` & `dagster-gcp-0.9.9rc1/dagster_gcp/bigquery/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp/bigquery/types.py` & `dagster-gcp-0.9.9rc1/dagster_gcp/bigquery/types.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp/dataproc/configs.py` & `dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/configs.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp/dataproc/configs_dataproc_cluster.py` & `dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/configs_dataproc_cluster.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp/dataproc/configs_dataproc_job.py` & `dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/configs_dataproc_job.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp/dataproc/resources.py` & `dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp/dataproc/solids.py` & `dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp/dataproc/types_dataproc_cluster.py` & `dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/types_dataproc_cluster.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp/dataproc/types_dataproc_job.py` & `dagster-gcp-0.9.9rc1/dagster_gcp/dataproc/types_dataproc_job.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp/gcs/file_manager.py` & `dagster-gcp-0.9.9rc1/dagster_gcp/gcs/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp/gcs/intermediate_storage.py` & `dagster-gcp-0.9.9rc1/dagster_gcp/gcs/intermediate_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp/gcs/object_store.py` & `dagster-gcp-0.9.9rc1/dagster_gcp/gcs/object_store.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp/gcs/resources.py` & `dagster-gcp-0.9.9rc1/dagster_gcp/gcs/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp/gcs/system_storage.py` & `dagster-gcp-0.9.9rc1/dagster_gcp/gcs/system_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp.egg-info/PKG-INFO` & `dagster-gcp-0.9.9rc1/dagster_gcp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-gcp
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for GCP-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-gcp-0.9.9/dagster_gcp.egg-info/SOURCES.txt` & `dagster-gcp-0.9.9rc1/dagster_gcp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp_tests/bigquery_tests/test_solids.py` & `dagster-gcp-0.9.9rc1/dagster_gcp_tests/bigquery_tests/test_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp_tests/bigquery_tests/test_types.py` & `dagster-gcp-0.9.9rc1/dagster_gcp_tests/bigquery_tests/test_types.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp_tests/dataproc_tests/test_resources.py` & `dagster-gcp-0.9.9rc1/dagster_gcp_tests/dataproc_tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp_tests/gcs_tests/test_gcs_file_manager.py` & `dagster-gcp-0.9.9rc1/dagster_gcp_tests/gcs_tests/test_gcs_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp_tests/gcs_tests/test_intermediate_storage.py` & `dagster-gcp-0.9.9rc1/dagster_gcp_tests/gcs_tests/test_intermediate_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp_tests/gcs_tests/test_object_store.py` & `dagster-gcp-0.9.9rc1/dagster_gcp_tests/gcs_tests/test_object_store.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/dagster_gcp_tests/gcs_tests/test_resources.py` & `dagster-gcp-0.9.9rc1/dagster_gcp_tests/gcs_tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-0.9.9/setup.py` & `dagster-gcp-0.9.9rc1/setup.py`

 * *Files identical despite different names*

