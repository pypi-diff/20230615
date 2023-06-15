# Comparing `tmp/macrometa-source-collection-0.0.48.tar.gz` & `tmp/macrometa-source-collection-0.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.48.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.49.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.48.tar` & `macrometa-source-collection-0.0.49.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     9918 2023-06-14 16:01:05.350009 macrometa-source-collection-0.0.48/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0     9855 2023-06-14 16:01:05.350009 macrometa-source-collection-0.0.48/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1626 2023-06-14 16:01:05.710033 macrometa-source-collection-0.0.48/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.48/setup.py
--rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.48/PKG-INFO
+-rw-r--r--   0        0        0     9918 2023-06-15 10:03:23.878624 macrometa-source-collection-0.0.49/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0     9866 2023-06-15 10:03:23.878624 macrometa-source-collection-0.0.49/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1626 2023-06-15 10:03:24.194621 macrometa-source-collection-0.0.49/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.49/setup.py
+-rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.49/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.48/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.49/macrometa_source_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.48/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.49/macrometa_source_collection/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                     for key in rec.keys()
                 ):
                     singer_record = self.msg_to_singer_message(stream, rec, None, utils.now())
                     start_time = time.time()
                     singer.write_message(singer_record)
                     end_time = time.time()
                     if end_time - start_time > 10:
-                        LOGGER.warn(f"*** Took {end_time - start_time}seconds to write singer record:{singer_record}, rec: {rec}, stream: {stream} ***")
+                        LOGGER.warn(f"*** Count: {i} Took {end_time - start_time}seconds to write singer record:{singer_record}, rec: {rec}, stream: {stream} ***")
                     self.exported_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(rec))
                     self.exported_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                 else:
                     LOGGER.warn("The record: %s, does not match the most common schema. Skipping it..", rec)
         except Exception as e:
             time.sleep(600)
             raise e
```

### Comparing `macrometa-source-collection-0.0.48/pyproject.toml` & `macrometa-source-collection-0.0.49/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.48'
+version='0.0.49'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.48/setup.py` & `macrometa-source-collection-0.0.49/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.48',
+    'version': '0.0.49',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.48/PKG-INFO` & `macrometa-source-collection-0.0.49/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.48
+Version: 0.0.49
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

