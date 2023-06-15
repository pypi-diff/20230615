# Comparing `tmp/data_ecosystem_services-202306.0.4.tar.gz` & `tmp/data_ecosystem_services-202306.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_services-202306.0.4.tar", max compression
+gzip compressed data, was "data_ecosystem_services-202306.0.5.tar", max compression
```

## Comparing `data_ecosystem_services-202306.0.4.tar` & `data_ecosystem_services-202306.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      857 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/__main__.py
--rw-r--r--   0        0        0      973 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/admin_service/__init__.py
--rw-r--r--   0        0        0     6323 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/admin_service/environment_logging.py
--rw-r--r--   0        0        0     6901 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/admin_service/environment_tracing.py
--rw-r--r--   0        0        0     1081 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/alation_service/__init__.py
--rw-r--r--   0        0        0     1871 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/alation_service/customfieldsendpoint.py
--rw-r--r--   0        0        0     2319 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/alation_service/datasource.py
--rw-r--r--   0        0        0     1808 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/alation_service/endpoint.py
--rw-r--r--   0        0        0     1666 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/alation_service/idfinderendpoint.py
--rw-r--r--   0        0        0    12151 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/alation_service/manifest.py
--rw-r--r--   0        0        0    17715 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/alation_service/schema.py
--rw-r--r--   0        0        0     1224 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/alation_service/tagsendpoint.py
--rw-r--r--   0        0        0    12309 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/alation_service/tokenendpoint.py
--rw-r--r--   0        0        0      971 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/az_storage_service/__init__.py
--rw-r--r--   0        0        0      790 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/az_storage_service/az_storage_queue.py
--rw-r--r--   0        0        0      908 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/security_service/__init__.py
--rw-r--r--   0        0        0    14614 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/security_service/security_core.py
--rw-r--r--   0        0        0     1115 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/self_service/__init__.py
--rw-r--r--   0        0        0    41371 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/self_service/dataset_metadata.py
--rw-r--r--   0        0        0    32805 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/self_service/environment_metadata.py
--rw-r--r--   0        0        0    36036 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/self_service/job_metadata.py
--rw-r--r--   0        0        0     2250 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/self_service/logging_metadata.py
--rw-r--r--   0        0        0    22304 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/self_service/pipeline_metadata.py
--rw-r--r--   0        0        0     1538 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/tech_environment_service/__init__.py
--rw-r--r--   0        0        0    33723 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/tech_environment_service/dataset_convert.py
--rw-r--r--   0        0        0     8716 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/tech_environment_service/dataset_core.py
--rw-r--r--   0        0        0    24955 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/tech_environment_service/dataset_crud.py
--rw-r--r--   0        0        0     3777 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/tech_environment_service/dataset_extract.py
--rw-r--r--   0        0        0     1997 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/tech_environment_service/environment_core.py
--rw-r--r--   0        0        0    27546 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/tech_environment_service/environment_file.py
--rw-r--r--   0        0        0     4589 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/tech_environment_service/environment_spark.py
--rw-r--r--   0        0        0     4648 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/tech_environment_service/job_core.py
--rw-r--r--   0        0        0    17224 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/data_ecosystem_services/tech_environment_service/repo_core.py
--rw-r--r--   0        0        0    11357 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/license.md
--rw-r--r--   0        0        0     3463 2023-06-15 15:10:09.140947 data_ecosystem_services-202306.0.4/pyproject.toml
--rw-r--r--   0        0        0    52126 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/readme.md
--rw-r--r--   0        0        0      126 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/setup.cfg
--rw-r--r--   0        0        0      127 2023-06-15 15:07:25.037860 data_ecosystem_services-202306.0.4/setup.py
--rw-r--r--   0        0        0    55003 1970-01-01 00:00:00.000000 data_ecosystem_services-202306.0.4/PKG-INFO
+-rw-r--r--   0        0        0      857 2023-06-15 15:38:55.732392 data_ecosystem_services-202306.0.5/data_ecosystem_services/__main__.py
+-rw-r--r--   0        0        0      973 2023-06-15 15:38:55.732392 data_ecosystem_services-202306.0.5/data_ecosystem_services/admin_service/__init__.py
+-rw-r--r--   0        0        0     6323 2023-06-15 15:38:55.732392 data_ecosystem_services-202306.0.5/data_ecosystem_services/admin_service/environment_logging.py
+-rw-r--r--   0        0        0     6901 2023-06-15 15:38:55.732392 data_ecosystem_services-202306.0.5/data_ecosystem_services/admin_service/environment_tracing.py
+-rw-r--r--   0        0        0     1081 2023-06-15 15:38:55.732392 data_ecosystem_services-202306.0.5/data_ecosystem_services/alation_service/__init__.py
+-rw-r--r--   0        0        0     1871 2023-06-15 15:38:55.732392 data_ecosystem_services-202306.0.5/data_ecosystem_services/alation_service/customfieldsendpoint.py
+-rw-r--r--   0        0        0     2319 2023-06-15 15:38:55.732392 data_ecosystem_services-202306.0.5/data_ecosystem_services/alation_service/datasource.py
+-rw-r--r--   0        0        0     1808 2023-06-15 15:38:55.732392 data_ecosystem_services-202306.0.5/data_ecosystem_services/alation_service/endpoint.py
+-rw-r--r--   0        0        0     1666 2023-06-15 15:38:55.732392 data_ecosystem_services-202306.0.5/data_ecosystem_services/alation_service/idfinderendpoint.py
+-rw-r--r--   0        0        0    12151 2023-06-15 15:38:55.732392 data_ecosystem_services-202306.0.5/data_ecosystem_services/alation_service/manifest.py
+-rw-r--r--   0        0        0    17715 2023-06-15 15:38:55.732392 data_ecosystem_services-202306.0.5/data_ecosystem_services/alation_service/schema.py
+-rw-r--r--   0        0        0     1224 2023-06-15 15:38:55.732392 data_ecosystem_services-202306.0.5/data_ecosystem_services/alation_service/tagsendpoint.py
+-rw-r--r--   0        0        0    12309 2023-06-15 15:38:55.732392 data_ecosystem_services-202306.0.5/data_ecosystem_services/alation_service/tokenendpoint.py
+-rw-r--r--   0        0        0      971 2023-06-15 15:38:55.732392 data_ecosystem_services-202306.0.5/data_ecosystem_services/az_storage_service/__init__.py
+-rw-r--r--   0        0        0      790 2023-06-15 15:38:55.732392 data_ecosystem_services-202306.0.5/data_ecosystem_services/az_storage_service/az_storage_queue.py
+-rw-r--r--   0        0        0      908 2023-06-15 15:38:55.732392 data_ecosystem_services-202306.0.5/data_ecosystem_services/security_service/__init__.py
+-rw-r--r--   0        0        0    14614 2023-06-15 15:38:55.732392 data_ecosystem_services-202306.0.5/data_ecosystem_services/security_service/security_core.py
+-rw-r--r--   0        0        0     1115 2023-06-15 15:38:55.732392 data_ecosystem_services-202306.0.5/data_ecosystem_services/self_service/__init__.py
+-rw-r--r--   0        0        0    41371 2023-06-15 15:38:55.732392 data_ecosystem_services-202306.0.5/data_ecosystem_services/self_service/dataset_metadata.py
+-rw-r--r--   0        0        0    32805 2023-06-15 15:38:55.732392 data_ecosystem_services-202306.0.5/data_ecosystem_services/self_service/environment_metadata.py
+-rw-r--r--   0        0        0    36036 2023-06-15 15:38:55.736392 data_ecosystem_services-202306.0.5/data_ecosystem_services/self_service/job_metadata.py
+-rw-r--r--   0        0        0     2250 2023-06-15 15:38:55.736392 data_ecosystem_services-202306.0.5/data_ecosystem_services/self_service/logging_metadata.py
+-rw-r--r--   0        0        0    22304 2023-06-15 15:38:55.736392 data_ecosystem_services-202306.0.5/data_ecosystem_services/self_service/pipeline_metadata.py
+-rw-r--r--   0        0        0     1538 2023-06-15 15:38:55.736392 data_ecosystem_services-202306.0.5/data_ecosystem_services/tech_environment_service/__init__.py
+-rw-r--r--   0        0        0    33723 2023-06-15 15:38:55.736392 data_ecosystem_services-202306.0.5/data_ecosystem_services/tech_environment_service/dataset_convert.py
+-rw-r--r--   0        0        0     8716 2023-06-15 15:38:55.736392 data_ecosystem_services-202306.0.5/data_ecosystem_services/tech_environment_service/dataset_core.py
+-rw-r--r--   0        0        0    24955 2023-06-15 15:38:55.736392 data_ecosystem_services-202306.0.5/data_ecosystem_services/tech_environment_service/dataset_crud.py
+-rw-r--r--   0        0        0     3777 2023-06-15 15:38:55.736392 data_ecosystem_services-202306.0.5/data_ecosystem_services/tech_environment_service/dataset_extract.py
+-rw-r--r--   0        0        0     1997 2023-06-15 15:38:55.736392 data_ecosystem_services-202306.0.5/data_ecosystem_services/tech_environment_service/environment_core.py
+-rw-r--r--   0        0        0    27546 2023-06-15 15:38:55.736392 data_ecosystem_services-202306.0.5/data_ecosystem_services/tech_environment_service/environment_file.py
+-rw-r--r--   0        0        0     4589 2023-06-15 15:38:55.736392 data_ecosystem_services-202306.0.5/data_ecosystem_services/tech_environment_service/environment_spark.py
+-rw-r--r--   0        0        0     4648 2023-06-15 15:38:55.736392 data_ecosystem_services-202306.0.5/data_ecosystem_services/tech_environment_service/job_core.py
+-rw-r--r--   0        0        0    17224 2023-06-15 15:38:55.736392 data_ecosystem_services-202306.0.5/data_ecosystem_services/tech_environment_service/repo_core.py
+-rw-r--r--   0        0        0    11357 2023-06-15 15:38:55.736392 data_ecosystem_services-202306.0.5/license.md
+-rw-r--r--   0        0        0     3463 2023-06-15 15:41:53.759734 data_ecosystem_services-202306.0.5/pyproject.toml
+-rw-r--r--   0        0        0    52126 2023-06-15 15:38:55.736392 data_ecosystem_services-202306.0.5/readme.md
+-rw-r--r--   0        0        0      126 2023-06-15 15:38:55.736392 data_ecosystem_services-202306.0.5/setup.cfg
+-rw-r--r--   0        0        0      127 2023-06-15 15:38:55.736392 data_ecosystem_services-202306.0.5/setup.py
+-rw-r--r--   0        0        0    55003 1970-01-01 00:00:00.000000 data_ecosystem_services-202306.0.5/PKG-INFO
```

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/__main__.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/__main__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/admin_service/__init__.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/admin_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/admin_service/environment_logging.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/admin_service/environment_logging.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/admin_service/environment_tracing.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/admin_service/environment_tracing.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/alation_service/__init__.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/alation_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/alation_service/customfieldsendpoint.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/alation_service/customfieldsendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/alation_service/datasource.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/alation_service/datasource.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/alation_service/endpoint.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/alation_service/endpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/alation_service/idfinderendpoint.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/alation_service/idfinderendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/alation_service/manifest.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/alation_service/manifest.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/alation_service/schema.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/alation_service/schema.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/alation_service/tagsendpoint.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/alation_service/tagsendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/alation_service/tokenendpoint.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/alation_service/tokenendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/az_storage_service/__init__.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/az_storage_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/az_storage_service/az_storage_queue.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/az_storage_service/az_storage_queue.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/security_service/__init__.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/security_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/security_service/security_core.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/security_service/security_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/self_service/__init__.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/self_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/self_service/dataset_metadata.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/self_service/dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/self_service/environment_metadata.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/self_service/environment_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/self_service/job_metadata.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/self_service/job_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/self_service/logging_metadata.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/self_service/logging_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/self_service/pipeline_metadata.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/self_service/pipeline_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/tech_environment_service/__init__.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/tech_environment_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/tech_environment_service/dataset_convert.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/tech_environment_service/dataset_convert.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/tech_environment_service/dataset_core.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/tech_environment_service/dataset_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/tech_environment_service/dataset_crud.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/tech_environment_service/dataset_crud.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/tech_environment_service/dataset_extract.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/tech_environment_service/dataset_extract.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/tech_environment_service/environment_core.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/tech_environment_service/environment_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/tech_environment_service/environment_file.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/tech_environment_service/environment_file.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/tech_environment_service/environment_spark.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/tech_environment_service/environment_spark.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/tech_environment_service/job_core.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/tech_environment_service/job_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/data_ecosystem_services/tech_environment_service/repo_core.py` & `data_ecosystem_services-202306.0.5/data_ecosystem_services/tech_environment_service/repo_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/license.md` & `data_ecosystem_services-202306.0.5/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/pyproject.toml` & `data_ecosystem_services-202306.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [project.urls]
 "Homepage" = "https://test.pypi.org/project/data-ecosystem-services"
 "Documentation" = "https://gift.readthedocs.io"
 "Repository" = "https://github.com/cdcent/data-ecosystem-services"
 
 [tool.poetry]
 name="data_ecosystem_services"
-version="202306.0.4"
+version="202306.0.5"
 description="Program Agnostic Data Ecosystem (PADE) - Python Services"
 authors=["John Bowyer <zfi4@cdc.gov>"]
 readme = "readme.md"
 license="Apache"
 homepage="https://test.pypi.org/project/data-ecosystem-services"
 repository="https://github.com/cdcent/data-ecosystem-services"
 classifiers=[
```

### Comparing `data_ecosystem_services-202306.0.4/readme.md` & `data_ecosystem_services-202306.0.5/readme.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.4/PKG-INFO` & `data_ecosystem_services-202306.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-services
-Version: 202306.0.4
+Version: 202306.0.5
 Summary: Program Agnostic Data Ecosystem (PADE) - Python Services
 Home-page: https://test.pypi.org/project/data-ecosystem-services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

