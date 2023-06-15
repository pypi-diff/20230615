# Comparing `tmp/data_ecosystem_services-202306.0.6.tar.gz` & `tmp/data_ecosystem_services-202306.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_services-202306.0.6.tar", max compression
+gzip compressed data, was "data_ecosystem_services-202306.0.7.tar", max compression
```

## Comparing `data_ecosystem_services-202306.0.6.tar` & `data_ecosystem_services-202306.0.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      857 2023-06-15 15:53:45.998345 data_ecosystem_services-202306.0.6/data_ecosystem_services/__main__.py
--rw-r--r--   0        0        0      973 2023-06-15 15:53:45.998345 data_ecosystem_services-202306.0.6/data_ecosystem_services/admin_service/__init__.py
--rw-r--r--   0        0        0     6323 2023-06-15 15:53:45.998345 data_ecosystem_services-202306.0.6/data_ecosystem_services/admin_service/environment_logging.py
--rw-r--r--   0        0        0     6901 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/admin_service/environment_tracing.py
--rw-r--r--   0        0        0     1081 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/alation_service/__init__.py
--rw-r--r--   0        0        0     1871 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/alation_service/customfieldsendpoint.py
--rw-r--r--   0        0        0     2319 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/alation_service/datasource.py
--rw-r--r--   0        0        0     1808 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/alation_service/endpoint.py
--rw-r--r--   0        0        0     1666 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/alation_service/idfinderendpoint.py
--rw-r--r--   0        0        0    12151 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/alation_service/manifest.py
--rw-r--r--   0        0        0    17715 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/alation_service/schema.py
--rw-r--r--   0        0        0     1224 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/alation_service/tagsendpoint.py
--rw-r--r--   0        0        0    12309 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/alation_service/tokenendpoint.py
--rw-r--r--   0        0        0      971 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/az_storage_service/__init__.py
--rw-r--r--   0        0        0      790 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/az_storage_service/az_storage_queue.py
--rw-r--r--   0        0        0      908 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/security_service/__init__.py
--rw-r--r--   0        0        0    14614 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/security_service/security_core.py
--rw-r--r--   0        0        0     1115 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/self_service/__init__.py
--rw-r--r--   0        0        0    41371 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/self_service/dataset_metadata.py
--rw-r--r--   0        0        0    32805 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/self_service/environment_metadata.py
--rw-r--r--   0        0        0    36036 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/self_service/job_metadata.py
--rw-r--r--   0        0        0     2250 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/self_service/logging_metadata.py
--rw-r--r--   0        0        0    22304 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/self_service/pipeline_metadata.py
--rw-r--r--   0        0        0     1538 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/tech_environment_service/__init__.py
--rw-r--r--   0        0        0    33723 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/tech_environment_service/dataset_convert.py
--rw-r--r--   0        0        0     8716 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/tech_environment_service/dataset_core.py
--rw-r--r--   0        0        0    24955 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/tech_environment_service/dataset_crud.py
--rw-r--r--   0        0        0     3777 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/tech_environment_service/dataset_extract.py
--rw-r--r--   0        0        0     1997 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/tech_environment_service/environment_core.py
--rw-r--r--   0        0        0    27546 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/tech_environment_service/environment_file.py
--rw-r--r--   0        0        0     4589 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/tech_environment_service/environment_spark.py
--rw-r--r--   0        0        0     4648 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/tech_environment_service/job_core.py
--rw-r--r--   0        0        0    17224 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/data_ecosystem_services/tech_environment_service/repo_core.py
--rw-r--r--   0        0        0    11357 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/license.md
--rw-r--r--   0        0        0     3495 2023-06-15 15:56:46.223780 data_ecosystem_services-202306.0.6/pyproject.toml
--rw-r--r--   0        0        0    52126 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/readme.md
--rw-r--r--   0        0        0      126 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/setup.cfg
--rw-r--r--   0        0        0      127 2023-06-15 15:53:46.002345 data_ecosystem_services-202306.0.6/setup.py
--rw-r--r--   0        0        0    55057 1970-01-01 00:00:00.000000 data_ecosystem_services-202306.0.6/PKG-INFO
+-rw-r--r--   0        0        0      857 2023-06-15 16:17:12.374575 data_ecosystem_services-202306.0.7/data_ecosystem_services/__main__.py
+-rw-r--r--   0        0        0      973 2023-06-15 16:17:12.374575 data_ecosystem_services-202306.0.7/data_ecosystem_services/admin_service/__init__.py
+-rw-r--r--   0        0        0     6323 2023-06-15 16:17:12.374575 data_ecosystem_services-202306.0.7/data_ecosystem_services/admin_service/environment_logging.py
+-rw-r--r--   0        0        0     6901 2023-06-15 16:17:12.374575 data_ecosystem_services-202306.0.7/data_ecosystem_services/admin_service/environment_tracing.py
+-rw-r--r--   0        0        0     1081 2023-06-15 16:17:12.374575 data_ecosystem_services-202306.0.7/data_ecosystem_services/alation_service/__init__.py
+-rw-r--r--   0        0        0     1871 2023-06-15 16:17:12.374575 data_ecosystem_services-202306.0.7/data_ecosystem_services/alation_service/customfieldsendpoint.py
+-rw-r--r--   0        0        0     2319 2023-06-15 16:17:12.374575 data_ecosystem_services-202306.0.7/data_ecosystem_services/alation_service/datasource.py
+-rw-r--r--   0        0        0     1808 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/alation_service/endpoint.py
+-rw-r--r--   0        0        0     1666 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/alation_service/idfinderendpoint.py
+-rw-r--r--   0        0        0    12151 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/alation_service/manifest.py
+-rw-r--r--   0        0        0    17715 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/alation_service/schema.py
+-rw-r--r--   0        0        0     1224 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/alation_service/tagsendpoint.py
+-rw-r--r--   0        0        0    12309 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/alation_service/tokenendpoint.py
+-rw-r--r--   0        0        0      971 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/az_storage_service/__init__.py
+-rw-r--r--   0        0        0      750 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/az_storage_service/az_storage_queue.py
+-rw-r--r--   0        0        0      908 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/security_service/__init__.py
+-rw-r--r--   0        0        0    14614 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/security_service/security_core.py
+-rw-r--r--   0        0        0     1115 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/self_service/__init__.py
+-rw-r--r--   0        0        0    41371 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/self_service/dataset_metadata.py
+-rw-r--r--   0        0        0    32805 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/self_service/environment_metadata.py
+-rw-r--r--   0        0        0    36036 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/self_service/job_metadata.py
+-rw-r--r--   0        0        0     2250 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/self_service/logging_metadata.py
+-rw-r--r--   0        0        0    22304 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/self_service/pipeline_metadata.py
+-rw-r--r--   0        0        0     1538 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/tech_environment_service/__init__.py
+-rw-r--r--   0        0        0    33723 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/tech_environment_service/dataset_convert.py
+-rw-r--r--   0        0        0     8716 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/tech_environment_service/dataset_core.py
+-rw-r--r--   0        0        0    24955 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/tech_environment_service/dataset_crud.py
+-rw-r--r--   0        0        0     3777 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/tech_environment_service/dataset_extract.py
+-rw-r--r--   0        0        0     1997 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/tech_environment_service/environment_core.py
+-rw-r--r--   0        0        0    27546 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/tech_environment_service/environment_file.py
+-rw-r--r--   0        0        0     4589 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/tech_environment_service/environment_spark.py
+-rw-r--r--   0        0        0     4648 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/tech_environment_service/job_core.py
+-rw-r--r--   0        0        0    17224 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/data_ecosystem_services/tech_environment_service/repo_core.py
+-rw-r--r--   0        0        0    11357 2023-06-15 16:17:12.378576 data_ecosystem_services-202306.0.7/license.md
+-rw-r--r--   0        0        0     3495 2023-06-15 16:21:41.123740 data_ecosystem_services-202306.0.7/pyproject.toml
+-rw-r--r--   0        0        0    52126 2023-06-15 16:17:12.382576 data_ecosystem_services-202306.0.7/readme.md
+-rw-r--r--   0        0        0      126 2023-06-15 16:17:12.382576 data_ecosystem_services-202306.0.7/setup.cfg
+-rw-r--r--   0        0        0      127 2023-06-15 16:17:12.382576 data_ecosystem_services-202306.0.7/setup.py
+-rw-r--r--   0        0        0    55057 1970-01-01 00:00:00.000000 data_ecosystem_services-202306.0.7/PKG-INFO
```

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/__main__.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/__main__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/admin_service/__init__.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/admin_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/admin_service/environment_logging.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/admin_service/environment_logging.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/admin_service/environment_tracing.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/admin_service/environment_tracing.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/alation_service/__init__.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/alation_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/alation_service/customfieldsendpoint.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/alation_service/customfieldsendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/alation_service/datasource.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/alation_service/datasource.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/alation_service/endpoint.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/alation_service/endpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/alation_service/idfinderendpoint.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/alation_service/idfinderendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/alation_service/manifest.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/alation_service/manifest.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/alation_service/schema.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/alation_service/schema.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/alation_service/tagsendpoint.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/alation_service/tagsendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/alation_service/tokenendpoint.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/alation_service/tokenendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/az_storage_service/__init__.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/az_storage_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/az_storage_service/az_storage_queue.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/az_storage_service/az_storage_queue.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from azure.storage.queue import QueueService
+from azure.storage.queue import QueueClient
 
 class AzureStorageQueue:
     def __init__(self, connection_string, queue_name):
-        self.queue_service = QueueService(connection_string=connection_string)
+        self.queue_service = QueueClient.from_connection_string(connection_string, queue_name)
         self.queue_name = queue_name
-        self.queue_service.create_queue(queue_name)
+        self.queue_service.create_queue()
 
     def enqueue_task(self, message):
-        self.queue_service.put_message(self.queue_name, message)
+        self.queue_service.send_message(message)
 
     def dequeue_task(self):
-        messages = self.queue_service.get_messages(self.queue_name, num_messages=1)
+        messages = self.queue_service.receive_messages(num_messages=1)
         if messages:
             message = messages[0]
             return message.content, message.id, message.pop_receipt
         return None
 
     def delete_task(self, message_id, pop_receipt):
-        self.queue_service.delete_message(self.queue_name, message_id, pop_receipt)
+        self.queue_service.delete_message( message_id, pop_receipt)
```

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/security_service/__init__.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/security_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/security_service/security_core.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/security_service/security_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/self_service/__init__.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/self_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/self_service/dataset_metadata.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/self_service/dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/self_service/environment_metadata.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/self_service/environment_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/self_service/job_metadata.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/self_service/job_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/self_service/logging_metadata.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/self_service/logging_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/self_service/pipeline_metadata.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/self_service/pipeline_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/tech_environment_service/__init__.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/tech_environment_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/tech_environment_service/dataset_convert.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/tech_environment_service/dataset_convert.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/tech_environment_service/dataset_core.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/tech_environment_service/dataset_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/tech_environment_service/dataset_crud.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/tech_environment_service/dataset_crud.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/tech_environment_service/dataset_extract.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/tech_environment_service/dataset_extract.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/tech_environment_service/environment_core.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/tech_environment_service/environment_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/tech_environment_service/environment_file.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/tech_environment_service/environment_file.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/tech_environment_service/environment_spark.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/tech_environment_service/environment_spark.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/tech_environment_service/job_core.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/tech_environment_service/job_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/data_ecosystem_services/tech_environment_service/repo_core.py` & `data_ecosystem_services-202306.0.7/data_ecosystem_services/tech_environment_service/repo_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/license.md` & `data_ecosystem_services-202306.0.7/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/pyproject.toml` & `data_ecosystem_services-202306.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [project.urls]
 "Homepage" = "https://test.pypi.org/project/data-ecosystem-services"
 "Documentation" = "https://gift.readthedocs.io"
 "Repository" = "https://github.com/cdcent/data-ecosystem-services"
 
 [tool.poetry]
 name="data_ecosystem_services"
-version="202306.0.6"
+version="202306.0.7"
 description="Program Agnostic Data Ecosystem (PADE) - Python Services"
 authors=["John Bowyer <zfi4@cdc.gov>"]
 readme = "readme.md"
 license="Apache"
 homepage="https://test.pypi.org/project/data-ecosystem-services"
 repository="https://github.com/cdcent/data-ecosystem-services"
 classifiers=[
```

### Comparing `data_ecosystem_services-202306.0.6/readme.md` & `data_ecosystem_services-202306.0.7/readme.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202306.0.6/PKG-INFO` & `data_ecosystem_services-202306.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-services
-Version: 202306.0.6
+Version: 202306.0.7
 Summary: Program Agnostic Data Ecosystem (PADE) - Python Services
 Home-page: https://test.pypi.org/project/data-ecosystem-services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

