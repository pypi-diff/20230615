# Comparing `tmp/data_ecosystem_services-202304.0.9.tar.gz` & `tmp/data_ecosystem_services-202306.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_services-202304.0.9.tar", max compression
+gzip compressed data, was "data_ecosystem_services-202306.0.1.tar", max compression
```

## Comparing `data_ecosystem_services-202304.0.9.tar` & `data_ecosystem_services-202306.0.1.tar`

### file list

```diff
@@ -1,29 +1,37 @@
--rw-r--r--   0        0        0      857 2023-04-11 00:20:25.877581 data_ecosystem_services-202304.0.9/data_ecosystem_services/__main__.py
--rw-r--r--   0        0        0      916 2023-04-11 00:20:25.877581 data_ecosystem_services-202304.0.9/data_ecosystem_services/admin_service/__init__.py
--rw-r--r--   0        0        0     4670 2023-04-11 00:20:25.877581 data_ecosystem_services-202304.0.9/data_ecosystem_services/admin_service/environment_logging.py
--rw-r--r--   0        0        0      958 2023-04-11 00:20:25.877581 data_ecosystem_services-202304.0.9/data_ecosystem_services/security_service/__init__.py
--rw-r--r--   0        0        0     3431 2023-04-11 00:20:25.877581 data_ecosystem_services-202304.0.9/data_ecosystem_services/security_service/security_alation.py
--rw-r--r--   0        0        0    14614 2023-04-11 00:20:25.877581 data_ecosystem_services-202304.0.9/data_ecosystem_services/security_service/security_core.py
--rw-r--r--   0        0        0     1115 2023-04-11 00:20:25.877581 data_ecosystem_services-202304.0.9/data_ecosystem_services/self_service/__init__.py
--rw-r--r--   0        0        0    41371 2023-04-11 00:20:25.877581 data_ecosystem_services-202304.0.9/data_ecosystem_services/self_service/dataset_metadata.py
--rw-r--r--   0        0        0    32651 2023-04-11 00:20:25.881581 data_ecosystem_services-202304.0.9/data_ecosystem_services/self_service/environment_metadata.py
--rw-r--r--   0        0        0    36036 2023-04-11 00:20:25.881581 data_ecosystem_services-202304.0.9/data_ecosystem_services/self_service/job_metadata.py
--rw-r--r--   0        0        0     2261 2023-04-11 00:20:25.881581 data_ecosystem_services-202304.0.9/data_ecosystem_services/self_service/logging_metadata.py
--rw-r--r--   0        0        0    22304 2023-04-11 00:20:25.881581 data_ecosystem_services-202304.0.9/data_ecosystem_services/self_service/pipeline_metadata.py
--rw-r--r--   0        0        0     1472 2023-04-11 00:20:25.881581 data_ecosystem_services-202304.0.9/data_ecosystem_services/tech_environment_service/__init__.py
--rw-r--r--   0        0        0    33731 2023-04-11 00:20:25.881581 data_ecosystem_services-202304.0.9/data_ecosystem_services/tech_environment_service/dataset_convert.py
--rw-r--r--   0        0        0     8716 2023-04-11 00:20:25.881581 data_ecosystem_services-202304.0.9/data_ecosystem_services/tech_environment_service/dataset_core.py
--rw-r--r--   0        0        0    24963 2023-04-11 00:20:25.881581 data_ecosystem_services-202304.0.9/data_ecosystem_services/tech_environment_service/dataset_crud.py
--rw-r--r--   0        0        0     3777 2023-04-11 00:20:25.881581 data_ecosystem_services-202304.0.9/data_ecosystem_services/tech_environment_service/dataset_extract.py
--rw-r--r--   0        0        0     1997 2023-04-11 00:20:25.881581 data_ecosystem_services-202304.0.9/data_ecosystem_services/tech_environment_service/environment_core.py
--rw-r--r--   0        0        0    26185 2023-04-11 00:20:25.881581 data_ecosystem_services-202304.0.9/data_ecosystem_services/tech_environment_service/environment_file.py
--rw-r--r--   0        0        0     4589 2023-04-11 00:20:25.881581 data_ecosystem_services-202304.0.9/data_ecosystem_services/tech_environment_service/environment_spark.py
--rw-r--r--   0        0        0     4648 2023-04-11 00:20:25.881581 data_ecosystem_services-202304.0.9/data_ecosystem_services/tech_environment_service/job_core.py
--rw-r--r--   0        0        0    17224 2023-04-11 00:20:25.881581 data_ecosystem_services-202304.0.9/data_ecosystem_services/tech_environment_service/repo_core.py
--rw-r--r--   0        0        0    10094 2023-04-11 00:20:25.881581 data_ecosystem_services-202304.0.9/data_ecosystem_services/tech_schema/manifest.py
--rw-r--r--   0        0        0    11357 2023-04-11 00:20:25.881581 data_ecosystem_services-202304.0.9/license.md
--rw-r--r--   0        0        0     3345 2023-04-11 00:24:01.390857 data_ecosystem_services-202304.0.9/pyproject.toml
--rw-r--r--   0        0        0    46691 2023-04-11 00:20:25.881581 data_ecosystem_services-202304.0.9/readme.md
--rw-r--r--   0        0        0      118 2023-04-11 00:20:25.881581 data_ecosystem_services-202304.0.9/setup.cfg
--rw-r--r--   0        0        0      127 2023-04-11 00:20:25.881581 data_ecosystem_services-202304.0.9/setup.py
--rw-r--r--   0        0        0    49502 1970-01-01 00:00:00.000000 data_ecosystem_services-202304.0.9/PKG-INFO
+-rw-r--r--   0        0        0      857 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/__main__.py
+-rw-r--r--   0        0        0      973 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/admin_service/__init__.py
+-rw-r--r--   0        0        0     6323 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/admin_service/environment_logging.py
+-rw-r--r--   0        0        0     6901 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/admin_service/environment_tracing.py
+-rw-r--r--   0        0        0     1081 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/alation_service/__init__.py
+-rw-r--r--   0        0        0     1871 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/alation_service/customfieldsendpoint.py
+-rw-r--r--   0        0        0     2319 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/alation_service/datasource.py
+-rw-r--r--   0        0        0     1808 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/alation_service/endpoint.py
+-rw-r--r--   0        0        0     1666 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/alation_service/idfinderendpoint.py
+-rw-r--r--   0        0        0    12151 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/alation_service/manifest.py
+-rw-r--r--   0        0        0    17699 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/alation_service/schema.py
+-rw-r--r--   0        0        0     1224 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/alation_service/tagsendpoint.py
+-rw-r--r--   0        0        0    12309 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/alation_service/tokenendpoint.py
+-rw-r--r--   0        0        0      908 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/security_service/__init__.py
+-rw-r--r--   0        0        0    14614 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/security_service/security_core.py
+-rw-r--r--   0        0        0     1115 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/self_service/__init__.py
+-rw-r--r--   0        0        0    41371 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/self_service/dataset_metadata.py
+-rw-r--r--   0        0        0    32805 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/self_service/environment_metadata.py
+-rw-r--r--   0        0        0    36036 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/self_service/job_metadata.py
+-rw-r--r--   0        0        0     2250 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/self_service/logging_metadata.py
+-rw-r--r--   0        0        0    22304 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/self_service/pipeline_metadata.py
+-rw-r--r--   0        0        0     1472 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/tech_environment_service/__init__.py
+-rw-r--r--   0        0        0    33723 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/tech_environment_service/dataset_convert.py
+-rw-r--r--   0        0        0     8716 2023-06-15 04:26:32.540635 data_ecosystem_services-202306.0.1/data_ecosystem_services/tech_environment_service/dataset_core.py
+-rw-r--r--   0        0        0    24955 2023-06-15 04:26:32.544635 data_ecosystem_services-202306.0.1/data_ecosystem_services/tech_environment_service/dataset_crud.py
+-rw-r--r--   0        0        0     3777 2023-06-15 04:26:32.544635 data_ecosystem_services-202306.0.1/data_ecosystem_services/tech_environment_service/dataset_extract.py
+-rw-r--r--   0        0        0     1997 2023-06-15 04:26:32.544635 data_ecosystem_services-202306.0.1/data_ecosystem_services/tech_environment_service/environment_core.py
+-rw-r--r--   0        0        0    27546 2023-06-15 04:26:32.544635 data_ecosystem_services-202306.0.1/data_ecosystem_services/tech_environment_service/environment_file.py
+-rw-r--r--   0        0        0     4589 2023-06-15 04:26:32.544635 data_ecosystem_services-202306.0.1/data_ecosystem_services/tech_environment_service/environment_spark.py
+-rw-r--r--   0        0        0     4648 2023-06-15 04:26:32.544635 data_ecosystem_services-202306.0.1/data_ecosystem_services/tech_environment_service/job_core.py
+-rw-r--r--   0        0        0    17224 2023-06-15 04:26:32.544635 data_ecosystem_services-202306.0.1/data_ecosystem_services/tech_environment_service/repo_core.py
+-rw-r--r--   0        0        0    11357 2023-06-15 04:26:32.544635 data_ecosystem_services-202306.0.1/license.md
+-rw-r--r--   0        0        0     3463 2023-06-15 04:28:27.965865 data_ecosystem_services-202306.0.1/pyproject.toml
+-rw-r--r--   0        0        0    52126 2023-06-15 04:26:32.544635 data_ecosystem_services-202306.0.1/readme.md
+-rw-r--r--   0        0        0      117 2023-06-15 04:26:32.544635 data_ecosystem_services-202306.0.1/setup.cfg
+-rw-r--r--   0        0        0      127 2023-06-15 04:26:32.544635 data_ecosystem_services-202306.0.1/setup.py
+-rw-r--r--   0        0        0    55003 1970-01-01 00:00:00.000000 data_ecosystem_services-202306.0.1/PKG-INFO
```

### Comparing `data_ecosystem_services-202304.0.9/data_ecosystem_services/__main__.py` & `data_ecosystem_services-202306.0.1/data_ecosystem_services/__main__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.9/data_ecosystem_services/admin_service/__init__.py` & `data_ecosystem_services-202306.0.1/data_ecosystem_services/security_service/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Initialize the admin_service subpackage of data_ecosystem_services package"""
+"""Initialize the security_service subpackage of data_ecosystem_services package"""
 # allow absolute import from the root folder
 # whatever its name is.
 import sys  # don't remove required for error handling
 import os
 
 # Import from sibling directory ..\developer_service
 OS_NAME = os.name
@@ -15,10 +15,10 @@
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..\\..\\..")))
 else:
     print("non windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../../..")))
 
-from . import environment_logging
+from . import security_core
 
-__all__ = ['environment_logging']
+__all__ = [ 'security_core']
```

### Comparing `data_ecosystem_services-202304.0.9/data_ecosystem_services/security_service/__init__.py` & `data_ecosystem_services-202306.0.1/data_ecosystem_services/admin_service/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Initialize the security_service subpackage of data_ecosystem_services package"""
+"""Initialize the admin_service subpackage of data_ecosystem_services package"""
 # allow absolute import from the root folder
 # whatever its name is.
 import sys  # don't remove required for error handling
 import os
 
 # Import from sibling directory ..\developer_service
 OS_NAME = os.name
@@ -15,11 +15,11 @@
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..\\..\\..")))
 else:
     print("non windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../../..")))
 
-from . import security_alation
-from . import security_core
+from . import environment_logging
+from . import environment_tracing
 
-__all__ = ['security_alation', 'security_core']
+__all__ = ['environment_logging', 'environment_tracing']
```

### Comparing `data_ecosystem_services-202304.0.9/data_ecosystem_services/security_service/security_core.py` & `data_ecosystem_services-202306.0.1/data_ecosystem_services/security_service/security_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.9/data_ecosystem_services/self_service/__init__.py` & `data_ecosystem_services-202306.0.1/data_ecosystem_services/self_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.9/data_ecosystem_services/self_service/dataset_metadata.py` & `data_ecosystem_services-202306.0.1/data_ecosystem_services/self_service/dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.9/data_ecosystem_services/self_service/environment_metadata.py` & `data_ecosystem_services-202306.0.1/data_ecosystem_services/self_service/environment_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import logging.config
 
 # data
 import uuid
 from datetime import datetime
 
 # davt
-from data_ecosystem_services.tech_environment_service \
+from data_ecosystem_services.security_service \
     import security_core as davt_sec_core
 from data_ecosystem_services.tech_environment_service \
     import environment_file as davt_env_file
 from data_ecosystem_services.self_service \
     import logging_metadata as davt_log_metadata
 
 from dotenv import load_dotenv, find_dotenv, set_key
@@ -335,17 +335,24 @@
         Args:
             parameters (dict): global parameters dictionary
 
         Returns:
             dict: update global configuration dictionary
         """
 
+
+
+        parameters.setdefault('running_local', False)
+        parameters.setdefault('dataset_name', 'na')
+        parameters.setdefault('cicd_action', 'na')
+
+
         if isinstance(parameters['running_local'], (bool)) is False:
             running_local = parameters['running_local'].lower() in ['true', '1', 't', 'y', 'yes']
-        else:
+        else: 
             running_local = parameters['running_local']
 
         project_id = parameters["project_id"]
         print(f"running_local: {running_local}")
         azure_client_secret_key = parameters['azure_client_secret_key']
         environment = parameters["environment"]
         project_id_root = parameters["project_id_root"]
```

### Comparing `data_ecosystem_services-202304.0.9/data_ecosystem_services/self_service/job_metadata.py` & `data_ecosystem_services-202306.0.1/data_ecosystem_services/self_service/job_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.9/data_ecosystem_services/self_service/logging_metadata.py` & `data_ecosystem_services-202306.0.1/data_ecosystem_services/self_service/logging_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Module to log warning, debug, error and info messages based on project metadata
 """
 import sys
 import os
 
-import data_ecosystem_services.tech_environment_service.environment_logging as davt_env_log
+import data_ecosystem_services.admin_service.environment_logging as davt_env_log
 
 class LoggingMetaData:
     """
     Class to log warning, debug, error and info messages based on project metadata
     """
 
     @staticmethod
```

### Comparing `data_ecosystem_services-202304.0.9/data_ecosystem_services/self_service/pipeline_metadata.py` & `data_ecosystem_services-202306.0.1/data_ecosystem_services/self_service/pipeline_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.9/data_ecosystem_services/tech_environment_service/__init__.py` & `data_ecosystem_services-202306.0.1/data_ecosystem_services/tech_environment_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.9/data_ecosystem_services/tech_environment_service/dataset_convert.py` & `data_ecosystem_services-202306.0.1/data_ecosystem_services/tech_environment_service/dataset_convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # file excel
 import openpyxl
 import openpyxl.utils.cell
 
 # PADE
 import data_ecosystem_services.tech_environment_service.environment_file as pade_env_file
 import data_ecosystem_services.tech_environment_service.dataset_core as pade_ds_core
-import data_ecosystem_services.tech_environment_service.security_core as pade_sec_core
+import data_ecosystem_services.security_service.security_core as pade_sec_core
 import data_ecosystem_services.tech_environment_service.environment_core as pade_env_core
 
 
 # data
 import numpy as np
 
 # spark / data
```

### Comparing `data_ecosystem_services-202304.0.9/data_ecosystem_services/tech_environment_service/dataset_core.py` & `data_ecosystem_services-202306.0.1/data_ecosystem_services/tech_environment_service/dataset_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.9/data_ecosystem_services/tech_environment_service/dataset_crud.py` & `data_ecosystem_services-202306.0.1/data_ecosystem_services/tech_environment_service/dataset_crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # file excel
 import openpyxl
 import openpyxl.utils.cell
 
 # PADE
 import data_ecosystem_services.tech_environment_service.dataset_core as pade_ds_core
 import data_ecosystem_services.tech_environment_service.environment_file as pade_env_file
-import data_ecosystem_services.tech_environment_service.security_core as pade_sec_core
+import data_ecosystem_services.security_service.security_core as pade_sec_core
 import data_ecosystem_services.tech_environment_service.environment_core as pade_env_core
 
 # spark / data
 import uuid
 from pyspark.sql import SparkSession, DataFrame
 import pyspark.sql.utils
 import pyspark.sql.functions as f
```

### Comparing `data_ecosystem_services-202304.0.9/data_ecosystem_services/tech_environment_service/dataset_extract.py` & `data_ecosystem_services-202306.0.1/data_ecosystem_services/tech_environment_service/dataset_extract.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.9/data_ecosystem_services/tech_environment_service/environment_core.py` & `data_ecosystem_services-202306.0.1/data_ecosystem_services/tech_environment_service/environment_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.9/data_ecosystem_services/tech_environment_service/environment_file.py` & `data_ecosystem_services-202306.0.1/data_ecosystem_services/tech_environment_service/environment_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -159,14 +159,52 @@
                 for chunk in request_result.iter_content(chunk_size=8192):
                     # If you have chunk encoded response uncomment if
                     # and set chunk_size parameter to None.
                     # if chunk:
                     file_result.write(chunk)
         return local_filename
 
+    @staticmethod
+    def scrub_file_name(original_file_name: str) -> str:
+        """Scrubs characters in object to rename
+
+        Args:
+            original_file_name (str): original column name
+
+        Returns:
+            str: new object name
+        """
+
+        if original_file_name is None:
+            original_file_name = "object_name_is_missing"
+
+        c_renamed = original_file_name
+        c_renamed = c_renamed.replace("†", "_")
+        c_renamed = c_renamed.replace(",", "_")
+        c_renamed = c_renamed.replace("*", "_")
+        c_renamed = c_renamed.replace(" ", "_")
+        c_renamed = c_renamed.replace("\r", "_")
+        c_renamed = c_renamed.replace("\n", "_")
+        c_renamed = c_renamed.replace(";", "")
+        c_renamed = c_renamed.replace(".", "")
+        c_renamed = c_renamed.replace("}", "")
+        c_renamed = c_renamed.replace("{", "")
+        c_renamed = c_renamed.replace("(", "")
+        c_renamed = c_renamed.replace(")", "")
+        c_renamed = c_renamed.replace("?", "")
+        c_renamed = c_renamed.replace("-", "")
+        c_renamed = c_renamed.replace("/", "")
+        c_renamed = c_renamed.replace("//", "")
+        c_renamed = c_renamed.replace("=", "_")
+        c_renamed = c_renamed.replace("&", "w")
+        c_renamed = c_renamed.lower()
+        c_renamed = c_renamed.strip()
+
+        return c_renamed
+
     @classmethod
     def prepend_line_to_file(cls, source_path: str, destination_path: str,
                              line_to_prepend: str) -> str:
         """Add line to the beginning of a file
 
         Args:
             source_path (str): _description_
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `data_ecosystem_services-202304.0.9/data_ecosystem_services/tech_environment_service/environment_spark.py` & `data_ecosystem_services-202306.0.1/data_ecosystem_services/tech_environment_service/environment_spark.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.9/data_ecosystem_services/tech_environment_service/job_core.py` & `data_ecosystem_services-202306.0.1/data_ecosystem_services/tech_environment_service/job_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.9/data_ecosystem_services/tech_environment_service/repo_core.py` & `data_ecosystem_services-202306.0.1/data_ecosystem_services/tech_environment_service/repo_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.9/license.md` & `data_ecosystem_services-202306.0.1/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202304.0.9/pyproject.toml` & `data_ecosystem_services-202306.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [project.urls]
 "Homepage" = "https://test.pypi.org/project/data-ecosystem-services"
 "Documentation" = "https://gift.readthedocs.io"
 "Repository" = "https://github.com/cdcent/data-ecosystem-services"
 
 [tool.poetry]
 name="data_ecosystem_services"
-version="202304.0.9"
+version="202306.0.1"
 description="Program Agnostic Data Ecosystem (PADE) - Python Services"
 authors=["John Bowyer <zfi4@cdc.gov>"]
 readme = "readme.md"
 license="Apache"
 homepage="https://test.pypi.org/project/data-ecosystem-services"
 repository="https://github.com/cdcent/data-ecosystem-services"
 classifiers=[
@@ -52,15 +52,15 @@
 azure-identity = "^1.10.0"
 azure-storage-file-datalake = "^12.8.0"
 openpyxl = "^3.0.4"
 numpy = "^1.23.0"
 botocore = "1.24.18"
 boto3 = "1.21.18"
 setuptools = "65.6.3"
-requests = "^2.28.1"
+requests = "2.31.0"
 myst-parser = "^0.18.0"
 sphinx-markdown-tables = "^0.0.17"
 Sphinx = "^5.2.1"
 sphinx-markdown-builder = "^0.5.5"
 pathlib = "^1.0.1"
 opencensus-ext-azure = "^1.1.7"
 opencensus = "^0.11.0"
@@ -82,14 +82,16 @@
 chardet = "^5.0.0"
 nbconvert = "^6.5.1"
 pip-system-certs = "^4.0"
 style = "^1.1.6"
 azure-keyvault = "^4.2.0"
 azure-mgmt-monitor = "^5.0.1"
 jinja2 = "^3.1.2"
+opentelemetry-sdk = "^1.17.0"
+azure-monitor-opentelemetry-exporter = {version = "^1.0.0b14", allow-prereleases = true}
 
 [tool.poetry.dev-dependencies]
 pandas = "^1.4.2"
 wheel = "^0.38.1"
 check-wheel-contents = "^0.3.4"
 flake8 = "^4.0.1"
 flake8-bugbear = "^22.6.22"
```

### Comparing `data_ecosystem_services-202304.0.9/readme.md` & `data_ecosystem_services-202306.0.1/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PADE-Python Project Documentation
 
-- Point of contact: [John Bowyer](mailto:zfo4@cdc.gov)
+- Point of contact: [John Bowyer](mailto:zfi4@cdc.gov)
 - Organizational unit: OCIO
 - Related projects: EDC
 - Related investments:  Pending Public Release
 - Governance status: Pending Public Release
 - Program official:  [Erik Knudsen](mailto:egk1@cdc.gov)
 
 ## Getting Started
@@ -33,16 +33,15 @@
 Update Path
 
         ```sh
         nano ~/.bashrc
         export PATH="/usr/bin/python3.9:$PATH"
         source ~/.bashrc
         ```
-        
-
+  
 #### Run Install Python on windows
 
 Run Application
 
         ```sh
         C:\Users\zfi4\OneDrive - CDC\DAVT Analytics\davt-analytics-software\python\python-3.9.0-amd64
         ```
@@ -201,15 +200,15 @@
 npm -v
 npm install npm@9.1.1
 pip install --upgrade pip
 pip install nodeenv
 cd $VIRTUAL_ENV/lib/node_modules/npm
 nodeenv -p
 cd $VIRTUAL_ENV/lib
-npm install mermaid.cli@latest
+npm install @mermaid-js/mermaid-cli --registry=https://registry.npmjs.org
 cdvirtualenv bin
 echo "export PATH='$PATH:$VIRTUAL_ENV/lib/node_modules/.bin'" | sudo tee -a activate
 source activate
 # Test client
 mmdc -h
 ```
 
@@ -232,15 +231,14 @@
 
 For local
 
 ```sh
 rm -rf OCIO_PADE_DEV
 ```
 
-
 ## Set up Local development environment for Docker
 
 ### Install Docker without License on Ubuntu or WSL (Primary)
 
 Reference 1: [Install Docker Engine without Docker Desktop](https://dev.to/bowmanjd/install-docker-on-windows-wsl-without-docker-desktop-34m9)
 Reference 2: [Install Docker for WSL](https://docs.docker.com/engine/install/ubuntu/)
 
@@ -850,15 +848,15 @@
 
 Symptom: Receive error: git push origin dev-zfi4:dev-zfi4
 remote: warning: File pade/pade_ocio_ingress/ehr/encounters.csv is 87.59 MB; this is larger than GitHub's recommended maximum file size of 50.00 MB
 remote: error: Trace: 2c8fbfed93d4f4c52468dde090cd8d14a1a311d13a6aa58ea35cb9cb8c5d2577
 remote: error: See http://git.io/iEPt8g for more information.
 remote: error: File pade/pade_ocio_ingress/ehr/observations.csv is 296.35 MB; this exceeds GitHub's file size limit of 100.00 MB
 remote: error: GH001: Large files detected. You may want to try Git Large File Storage - https://git-lfs.github.com.
-To https://github.com/cdcent/davt_pade_ocio.git
+To https://github.com/cdcent/data-ecosystem-services.git
  ! [remote rejected] dev-zfi4 -> dev-zfi4 (pre-receive hook declined)
 
 Reference: [Stack Overflow](https://stackoverflow.com/questions/33330771/git-lfs-this-exceeds-githubs-file-size-limit-of-100-00-mb)
 
 Solution:
 
 ```sh
@@ -1281,14 +1279,118 @@
 First, ensure that python is included in the PATH variable, then run
 Then run the following
 
 ```sh
 python -m ensurepip
 ```
 
+### Error: Ubuntu: Failed to call method: org.freedesktop.DBus.Properties.Get: object_path= /org/freedesktop/UPower: org.freedesktop.DBus.Error.ServiceUnknown
+
+Problem: When browsing https://127.0.0.1:5000 receive error: SSL: Handshake failed. while not logged into ZScaler
+
+Solution: 
+
+Here are the steps you can follow to fix this error:
+
+1. Check if the UPower daemon is installed on your system by running the following command in the terminal:
+
+```bash
+systemctl status upower.service
+```
+
+If the command output shows that the UPower service is not running or is not installed, you can install it using the package manager for your system (e.g. apt-get for Ubuntu/Debian, dnf for Fedora, pacman for Arch Linux, etc.).
+
+2. Install the UPower daemon using the package manager. For example, on Ubuntu/Debian, you can run the following command:
+
+```bash
+sudo apt-get install upower
+```
+
+This command installs the upower package, which provides the UPower daemon.
+
+3. After installing the UPower daemon, start the service using the following command:
+
+```bash
+sudo systemctl start upower.service
+```
+
+4. Verify that the UPower daemon is now running by checking the status using the following command:
+
+```bash
+systemctl status upower.service
+```
+
+5. Restart your Flask application and try again. The error message should no longer appear.
+
+Note that the specific steps for installing and starting the UPower daemon may vary depending on your system and distribution. You may need to consult the documentation or package manager for your system to find the appropriate package and commands to install and start the UPower daemon.
+
+### Error: Ubuntu: SSL: Handshake failed error when browsing local web site in google-chrome from Ubuntu
+
+Problem:  When browsing https://127.0.0.1:5000 receive error: SSL: Handshake failed. when logged into ZScaler
+
+[39102:39117:0503/091443.791015:ERROR:ssl_client_socket_impl.cc(992)] handshake failed; returned -1, SSL error code 1, net_error -202
+[39102:39117:0503/091447.197078:ERROR:ssl_client_socket_impl.cc(992)] handshake failed; returned -1, SSL error code 1, net_error -202
+[39102:39117:0503/091447.998238:ERROR:ssl_client_socket_impl.cc(992)] handshake failed; returned -1, SSL error code 1, net_error -202
+[39062:39086:0503/091448.177119:ERROR:cert_issuer_source_aia.cc(134)] AiaRequest::OnFetchCompleted got error -301
+[39062:39086:0503/091448.178211:ERROR:cert_issuer_source_aia.cc(134)] AiaRequest::OnFetchCompleted got error -301
+[42678:42704:0503/093402.088689:ERROR:cert_verify_proc_builtin.cc(677)] CertVerifyProcBuiltin for clientservices.googleapis.com failed:
+----- Certificate i=2 (CN=NCA-DPI1,OU=ITSO,O=Centers for Disease Control and Prevention,L=Atlanta,ST=Georgia,C=US) -----
+ERROR: No matching issuer found
+
+[39062:39086:0503/091448.178351:ERROR:cert_verify_proc_builtin.cc(677)] CertVerifyProcBuiltin for optimizationguide-pa.googleapis.com failed:
+----- Certificate i=2 (CN=NCA-DPI1,OU=ITSO,O=Centers for Disease Control and Prevention,L=Atlanta,ST=Georgia,C=US) -----
+ERROR: No matching issuer found
+
+Solution:  
+
+1. Verify that your Python installation has a valid CA bundle that can be used to verify the SSL/TLS certificate. You can do this by running the following command in your terminal:
+
+```bash
+python -c "import ssl; print(ssl.get_default_verify_paths())"
+```
+
+This should print out the paths to the CA bundle and the OpenSSL configuration file used by Python. If the paths are not found or are invalid, you may need to update your Python installation or install a valid CA bundle.
+
+Path should return
+
+```bash
+/usr/lib/ssl/certs
+```
+
+2. Download the missing CA certificate from the server that issued the certificate. You can use the openssl s_client command to retrieve the certificate, like this:
+
+```bash
+cd $HOME
+openssl s_client -showcerts -connect clientservices.googleapis.com:443 </dev/null 2>/dev/null | openssl x509 -outform PEM > clientservices.googleapis.com.crt
+openssl s_client -showcerts -connect optimizationguide-pa.googleapis.com:443 </dev/null 2>/dev/null | openssl x509 -outform PEM >  optimizationguide-pa.googleapis.com.crt
+openssl s_client -showcerts -connect safebrowsing.googleapis.com.com:443 </dev/null 2>/dev/null | openssl x509 -outform PEM >  safebrowsing.googleapis.com.crt
+openssl s_client -showcerts -connect accounts.google.com:443 </dev/null 2>/dev/null | openssl x509 -outform PEM >  accounts.google.com.crt
+openssl s_client -showcerts -connect update.googleapis.com:443 </dev/null 2>/dev/null | openssl x509 -outform PEM >  update.googleapis.com.crt
+openssl s_client -showcerts -connect www.google.com:443 </dev/null 2>/dev/null | openssl x509 -outform PEM >  www.google.com.crt
+ dns.google
+```
+
+3. Install the CA certificate in your system's trusted CA store by copying it to the /usr/local/share/ca-certificates/ directory:
+    
+```bash
+sudo cp clientservices.googleapis.com.crt /usr/local/share/ca-certificates/
+sudo cp optimizationguide-pa.googleapis.com.crt /usr/local/share/ca-certificates/
+sudo cp  safebrowsing.googleapis.com.crt /usr/local/share/ca-certificates/
+sudo cp accounts.google.com.crt /usr/local/share/ca-certificates/
+sudo cp update.googleapis.com.crt /usr/local/share/ca-certificates/
+sudo cp www.google.com.crt /usr/local/share/ca-certificates/
+```
+
+4. Update the CA bundle by running the following command:
+
+```bash
+sudo update-ca-certificates
+```
+
+
 ### Error: Ubuntu: CURL: SSL: Certificate problem: unable to get local issuer certificate when installing docker
 
 Symptom:  Receive error: curl: (60) SSL certificate problem: unable to get local issuer certificate when installing docker
 
 Reference: [Stack Overflow](https://stackoverflow.com/questions/72167566/wsl-docker-curl-60-ssl-certificate-problem-unable-to-get-local-issuer-certi)
 
 Details:
@@ -1423,15 +1525,15 @@
 3. Search for CRLF
 4. Change Files: EOL Setting to LF
 
 Solution for All Existing Files
 
 1. Download VS Code Exntension: [Change LF to CRLF](https://marketplace.visualstudio.com/items?itemName=stkb.rewrap)
 
-### Problem: WSL: Github clone fails: "fatal: unable to access 'https://github.com/cdcent/davt_pade_ocio.git/': Could not resolve host: github.com':"
+### Problem: WSL: Github clone fails: "fatal: unable to access 'https://github.com/cdcent/data-ecosystem-services.git': Could not resolve host: github.com':"
 
 Symptom: Trying to clone a github repository and receive error: "fatal: unable to access Could not resolve host: github.com "
 
 Reference: [Stack Overflow](https://stackoverflow.com/questions/20370294/git-could-not-resolve-host-github-com-error-while-cloning-remote-repository-in)
 
 Resolution:
```

### Comparing `data_ecosystem_services-202304.0.9/PKG-INFO` & `data_ecosystem_services-202306.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-services
-Version: 202304.0.9
+Version: 202306.0.1
 Summary: Program Agnostic Data Ecosystem (PADE) - Python Services
 Home-page: https://test.pypi.org/project/data-ecosystem-services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -13,45 +13,46 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Sphinx (>=5.2.1,<6.0.0)
 Requires-Dist: adal (>=1.2.7,<2.0.0)
 Requires-Dist: azure-common (>=1.1.28,<2.0.0)
 Requires-Dist: azure-identity (>=1.10.0,<2.0.0)
 Requires-Dist: azure-keyvault (>=4.2.0,<5.0.0)
 Requires-Dist: azure-keyvault-secrets (>=4.5.0,<5.0.0)
 Requires-Dist: azure-mgmt-monitor (>=5.0.1,<6.0.0)
+Requires-Dist: azure-monitor-opentelemetry-exporter (>=1.0.0b14,<2.0.0)
 Requires-Dist: azure-storage-file-datalake (>=12.8.0,<13.0.0)
 Requires-Dist: boto3 (==1.21.18)
 Requires-Dist: botocore (==1.24.18)
 Requires-Dist: chardet (>=5.0.0,<6.0.0)
 Requires-Dist: docutils (==0.17.1)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: markdown (>=3.4.1,<4.0.0)
 Requires-Dist: myst-parser (>=0.18.0,<0.19.0)
 Requires-Dist: nbconvert (>=6.5.1,<7.0.0)
 Requires-Dist: numpy (>=1.23.0,<2.0.0)
 Requires-Dist: opencensus (>=0.11.0,<0.12.0)
 Requires-Dist: opencensus-ext-azure (>=1.1.7,<2.0.0)
 Requires-Dist: openpyxl (>=3.0.4,<4.0.0)
+Requires-Dist: opentelemetry-sdk (>=1.17.0,<2.0.0)
 Requires-Dist: pathlib (>=1.0.1,<2.0.0)
 Requires-Dist: pip-system-certs (>=4.0,<5.0)
 Requires-Dist: pyarrow (>=10.0.1,<11.0.0)
 Requires-Dist: pygments (>=2.13.0,<3.0.0)
 Requires-Dist: pyreadstat (>=1.1.9,<2.0.0)
 Requires-Dist: pytest (>=7.1.2,<8.0.0)
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: requests (==2.31.0)
 Requires-Dist: rsconnect-jupyter (>=1.6.0,<2.0.0)
 Requires-Dist: setuptools (==65.6.3)
 Requires-Dist: sphinx-autoapi (>=2.0.0,<3.0.0)
 Requires-Dist: sphinx-autodoc-typehints (>=1.19.5,<2.0.0)
 Requires-Dist: sphinx-markdown-builder (>=0.5.5,<0.6.0)
 Requires-Dist: sphinx-markdown-tables (>=0.0.17,<0.0.18)
 Requires-Dist: sphinx-rtd-theme (>=1.1.1,<2.0.0)
@@ -61,15 +62,15 @@
 Requires-Dist: style (>=1.1.6,<2.0.0)
 Requires-Dist: testresources (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://github.com/cdcent/data-ecosystem-services
 Description-Content-Type: text/markdown
 
 # PADE-Python Project Documentation
 
-- Point of contact: [John Bowyer](mailto:zfo4@cdc.gov)
+- Point of contact: [John Bowyer](mailto:zfi4@cdc.gov)
 - Organizational unit: OCIO
 - Related projects: EDC
 - Related investments:  Pending Public Release
 - Governance status: Pending Public Release
 - Program official:  [Erik Knudsen](mailto:egk1@cdc.gov)
 
 ## Getting Started
@@ -98,16 +99,15 @@
 Update Path
 
         ```sh
         nano ~/.bashrc
         export PATH="/usr/bin/python3.9:$PATH"
         source ~/.bashrc
         ```
-        
-
+  
 #### Run Install Python on windows
 
 Run Application
 
         ```sh
         C:\Users\zfi4\OneDrive - CDC\DAVT Analytics\davt-analytics-software\python\python-3.9.0-amd64
         ```
@@ -266,15 +266,15 @@
 npm -v
 npm install npm@9.1.1
 pip install --upgrade pip
 pip install nodeenv
 cd $VIRTUAL_ENV/lib/node_modules/npm
 nodeenv -p
 cd $VIRTUAL_ENV/lib
-npm install mermaid.cli@latest
+npm install @mermaid-js/mermaid-cli --registry=https://registry.npmjs.org
 cdvirtualenv bin
 echo "export PATH='$PATH:$VIRTUAL_ENV/lib/node_modules/.bin'" | sudo tee -a activate
 source activate
 # Test client
 mmdc -h
 ```
 
@@ -297,15 +297,14 @@
 
 For local
 
 ```sh
 rm -rf OCIO_PADE_DEV
 ```
 
-
 ## Set up Local development environment for Docker
 
 ### Install Docker without License on Ubuntu or WSL (Primary)
 
 Reference 1: [Install Docker Engine without Docker Desktop](https://dev.to/bowmanjd/install-docker-on-windows-wsl-without-docker-desktop-34m9)
 Reference 2: [Install Docker for WSL](https://docs.docker.com/engine/install/ubuntu/)
 
@@ -915,15 +914,15 @@
 
 Symptom: Receive error: git push origin dev-zfi4:dev-zfi4
 remote: warning: File pade/pade_ocio_ingress/ehr/encounters.csv is 87.59 MB; this is larger than GitHub's recommended maximum file size of 50.00 MB
 remote: error: Trace: 2c8fbfed93d4f4c52468dde090cd8d14a1a311d13a6aa58ea35cb9cb8c5d2577
 remote: error: See http://git.io/iEPt8g for more information.
 remote: error: File pade/pade_ocio_ingress/ehr/observations.csv is 296.35 MB; this exceeds GitHub's file size limit of 100.00 MB
 remote: error: GH001: Large files detected. You may want to try Git Large File Storage - https://git-lfs.github.com.
-To https://github.com/cdcent/davt_pade_ocio.git
+To https://github.com/cdcent/data-ecosystem-services.git
  ! [remote rejected] dev-zfi4 -> dev-zfi4 (pre-receive hook declined)
 
 Reference: [Stack Overflow](https://stackoverflow.com/questions/33330771/git-lfs-this-exceeds-githubs-file-size-limit-of-100-00-mb)
 
 Solution:
 
 ```sh
@@ -1346,14 +1345,118 @@
 First, ensure that python is included in the PATH variable, then run
 Then run the following
 
 ```sh
 python -m ensurepip
 ```
 
+### Error: Ubuntu: Failed to call method: org.freedesktop.DBus.Properties.Get: object_path= /org/freedesktop/UPower: org.freedesktop.DBus.Error.ServiceUnknown
+
+Problem: When browsing https://127.0.0.1:5000 receive error: SSL: Handshake failed. while not logged into ZScaler
+
+Solution: 
+
+Here are the steps you can follow to fix this error:
+
+1. Check if the UPower daemon is installed on your system by running the following command in the terminal:
+
+```bash
+systemctl status upower.service
+```
+
+If the command output shows that the UPower service is not running or is not installed, you can install it using the package manager for your system (e.g. apt-get for Ubuntu/Debian, dnf for Fedora, pacman for Arch Linux, etc.).
+
+2. Install the UPower daemon using the package manager. For example, on Ubuntu/Debian, you can run the following command:
+
+```bash
+sudo apt-get install upower
+```
+
+This command installs the upower package, which provides the UPower daemon.
+
+3. After installing the UPower daemon, start the service using the following command:
+
+```bash
+sudo systemctl start upower.service
+```
+
+4. Verify that the UPower daemon is now running by checking the status using the following command:
+
+```bash
+systemctl status upower.service
+```
+
+5. Restart your Flask application and try again. The error message should no longer appear.
+
+Note that the specific steps for installing and starting the UPower daemon may vary depending on your system and distribution. You may need to consult the documentation or package manager for your system to find the appropriate package and commands to install and start the UPower daemon.
+
+### Error: Ubuntu: SSL: Handshake failed error when browsing local web site in google-chrome from Ubuntu
+
+Problem:  When browsing https://127.0.0.1:5000 receive error: SSL: Handshake failed. when logged into ZScaler
+
+[39102:39117:0503/091443.791015:ERROR:ssl_client_socket_impl.cc(992)] handshake failed; returned -1, SSL error code 1, net_error -202
+[39102:39117:0503/091447.197078:ERROR:ssl_client_socket_impl.cc(992)] handshake failed; returned -1, SSL error code 1, net_error -202
+[39102:39117:0503/091447.998238:ERROR:ssl_client_socket_impl.cc(992)] handshake failed; returned -1, SSL error code 1, net_error -202
+[39062:39086:0503/091448.177119:ERROR:cert_issuer_source_aia.cc(134)] AiaRequest::OnFetchCompleted got error -301
+[39062:39086:0503/091448.178211:ERROR:cert_issuer_source_aia.cc(134)] AiaRequest::OnFetchCompleted got error -301
+[42678:42704:0503/093402.088689:ERROR:cert_verify_proc_builtin.cc(677)] CertVerifyProcBuiltin for clientservices.googleapis.com failed:
+----- Certificate i=2 (CN=NCA-DPI1,OU=ITSO,O=Centers for Disease Control and Prevention,L=Atlanta,ST=Georgia,C=US) -----
+ERROR: No matching issuer found
+
+[39062:39086:0503/091448.178351:ERROR:cert_verify_proc_builtin.cc(677)] CertVerifyProcBuiltin for optimizationguide-pa.googleapis.com failed:
+----- Certificate i=2 (CN=NCA-DPI1,OU=ITSO,O=Centers for Disease Control and Prevention,L=Atlanta,ST=Georgia,C=US) -----
+ERROR: No matching issuer found
+
+Solution:  
+
+1. Verify that your Python installation has a valid CA bundle that can be used to verify the SSL/TLS certificate. You can do this by running the following command in your terminal:
+
+```bash
+python -c "import ssl; print(ssl.get_default_verify_paths())"
+```
+
+This should print out the paths to the CA bundle and the OpenSSL configuration file used by Python. If the paths are not found or are invalid, you may need to update your Python installation or install a valid CA bundle.
+
+Path should return
+
+```bash
+/usr/lib/ssl/certs
+```
+
+2. Download the missing CA certificate from the server that issued the certificate. You can use the openssl s_client command to retrieve the certificate, like this:
+
+```bash
+cd $HOME
+openssl s_client -showcerts -connect clientservices.googleapis.com:443 </dev/null 2>/dev/null | openssl x509 -outform PEM > clientservices.googleapis.com.crt
+openssl s_client -showcerts -connect optimizationguide-pa.googleapis.com:443 </dev/null 2>/dev/null | openssl x509 -outform PEM >  optimizationguide-pa.googleapis.com.crt
+openssl s_client -showcerts -connect safebrowsing.googleapis.com.com:443 </dev/null 2>/dev/null | openssl x509 -outform PEM >  safebrowsing.googleapis.com.crt
+openssl s_client -showcerts -connect accounts.google.com:443 </dev/null 2>/dev/null | openssl x509 -outform PEM >  accounts.google.com.crt
+openssl s_client -showcerts -connect update.googleapis.com:443 </dev/null 2>/dev/null | openssl x509 -outform PEM >  update.googleapis.com.crt
+openssl s_client -showcerts -connect www.google.com:443 </dev/null 2>/dev/null | openssl x509 -outform PEM >  www.google.com.crt
+ dns.google
+```
+
+3. Install the CA certificate in your system's trusted CA store by copying it to the /usr/local/share/ca-certificates/ directory:
+    
+```bash
+sudo cp clientservices.googleapis.com.crt /usr/local/share/ca-certificates/
+sudo cp optimizationguide-pa.googleapis.com.crt /usr/local/share/ca-certificates/
+sudo cp  safebrowsing.googleapis.com.crt /usr/local/share/ca-certificates/
+sudo cp accounts.google.com.crt /usr/local/share/ca-certificates/
+sudo cp update.googleapis.com.crt /usr/local/share/ca-certificates/
+sudo cp www.google.com.crt /usr/local/share/ca-certificates/
+```
+
+4. Update the CA bundle by running the following command:
+
+```bash
+sudo update-ca-certificates
+```
+
+
 ### Error: Ubuntu: CURL: SSL: Certificate problem: unable to get local issuer certificate when installing docker
 
 Symptom:  Receive error: curl: (60) SSL certificate problem: unable to get local issuer certificate when installing docker
 
 Reference: [Stack Overflow](https://stackoverflow.com/questions/72167566/wsl-docker-curl-60-ssl-certificate-problem-unable-to-get-local-issuer-certi)
 
 Details:
@@ -1488,15 +1591,15 @@
 3. Search for CRLF
 4. Change Files: EOL Setting to LF
 
 Solution for All Existing Files
 
 1. Download VS Code Exntension: [Change LF to CRLF](https://marketplace.visualstudio.com/items?itemName=stkb.rewrap)
 
-### Problem: WSL: Github clone fails: "fatal: unable to access 'https://github.com/cdcent/davt_pade_ocio.git/': Could not resolve host: github.com':"
+### Problem: WSL: Github clone fails: "fatal: unable to access 'https://github.com/cdcent/data-ecosystem-services.git': Could not resolve host: github.com':"
 
 Symptom: Trying to clone a github repository and receive error: "fatal: unable to access Could not resolve host: github.com "
 
 Reference: [Stack Overflow](https://stackoverflow.com/questions/20370294/git-could-not-resolve-host-github-com-error-while-cloning-remote-repository-in)
 
 Resolution:
```

