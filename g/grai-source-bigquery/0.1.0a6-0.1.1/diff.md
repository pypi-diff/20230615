# Comparing `tmp/grai_source_bigquery-0.1.0a6.tar.gz` & `tmp/grai_source_bigquery-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_bigquery-0.1.0a6.tar", max compression
+gzip compressed data, was "grai_source_bigquery-0.1.1.tar", max compression
```

## Comparing `grai_source_bigquery-0.1.0a6.tar` & `grai_source_bigquery-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      141 2023-05-02 08:01:59.695304 grai_source_bigquery-0.1.0a6/README.md
--rw-r--r--   0        0        0      971 2023-06-06 09:38:34.393417 grai_source_bigquery-0.1.0a6/pyproject.toml
--rw-r--r--   0        0        0      145 2023-02-14 12:06:39.088033 grai_source_bigquery-0.1.0a6/src/grai_source_bigquery/__init__.py
--rw-r--r--   0        0        0     8578 2023-06-02 08:26:06.787907 grai_source_bigquery-0.1.0a6/src/grai_source_bigquery/adapters.py
--rw-r--r--   0        0        0     2078 2023-06-06 09:08:28.709689 grai_source_bigquery-0.1.0a6/src/grai_source_bigquery/base.py
--rw-r--r--   0        0        0    13806 2023-06-06 09:38:20.206271 grai_source_bigquery-0.1.0a6/src/grai_source_bigquery/loader.py
--rw-r--r--   0        0        0     6222 2023-06-06 09:35:00.282149 grai_source_bigquery-0.1.0a6/src/grai_source_bigquery/models.py
--rw-r--r--   0        0        0      199 2023-06-02 08:26:06.789100 grai_source_bigquery-0.1.0a6/src/grai_source_bigquery/package_definitions.py
--rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 grai_source_bigquery-0.1.0a6/PKG-INFO
+-rw-r--r--   0        0        0      141 2023-05-19 11:07:12.920740 grai_source_bigquery-0.1.1/README.md
+-rw-r--r--   0        0        0     1037 2023-06-14 22:17:28.774356 grai_source_bigquery-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-06-14 22:11:02.218790 grai_source_bigquery-0.1.1/src/grai_source_bigquery/__init__.py
+-rw-r--r--   0        0        0     8650 2023-06-14 22:10:38.534667 grai_source_bigquery-0.1.1/src/grai_source_bigquery/adapters.py
+-rw-r--r--   0        0        0     2078 2023-06-14 21:10:34.436953 grai_source_bigquery-0.1.1/src/grai_source_bigquery/base.py
+-rw-r--r--   0        0        0    13790 2023-06-14 21:10:34.437255 grai_source_bigquery-0.1.1/src/grai_source_bigquery/loader.py
+-rw-r--r--   0        0        0     6222 2023-06-14 21:10:34.437405 grai_source_bigquery-0.1.1/src/grai_source_bigquery/models.py
+-rw-r--r--   0        0        0      199 2023-06-01 16:01:43.257500 grai_source_bigquery-0.1.1/src/grai_source_bigquery/package_definitions.py
+-rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 grai_source_bigquery-0.1.1/PKG-INFO
```

### Comparing `grai_source_bigquery-0.1.0a6/pyproject.toml` & `grai_source_bigquery-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "grai_source_bigquery"
-version = "0.1.0-alpha6"
+version = "0.1.1"
 description = ""
 authors = ["Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_bigquery", from = "src" },
 ]
 readme = "README.md"
 homepage = "https://www.grai.io/"
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-bigquery"
 documentation = "https://docs.grai.io/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
-grai-client = "^0.2.0"
+grai-client = "^0.2.18"
 multimethod = "^1.8"
-grai-schemas = "^0.1.9"
+grai-schemas = "^0.1.15"
 google-cloud-bigquery = "^3.5.0"
 setuptools = "^67.1.0"
 google-cloud-logging = "^3.5.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 mypy = "^0.971"
@@ -35,7 +35,9 @@
 
 [tool.black]
 line-length = 120
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry_bumpversion.file."src/grai_source_bigquery/__init__.py"]
```

### Comparing `grai_source_bigquery-0.1.0a6/src/grai_source_bigquery/adapters.py` & `grai_source_bigquery-0.1.1/src/grai_source_bigquery/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 from grai_client.schemas.schema import Schema
 from grai_schemas import config as base_config
 from grai_schemas.generics import DefaultValue
 from grai_schemas.v1 import EdgeV1, NodeV1
 from grai_schemas.v1.metadata.edges import (
     ColumnToColumnMetadata,
-    EdgeTypeLabels,
+    EdgeMetadataTypeLabels,
     GenericEdgeMetadataV1,
     TableToColumnMetadata,
     TableToTableMetadata,
 )
-from grai_schemas.v1.metadata.nodes import ColumnMetadata, NodeTypeLabels, TableMetadata
+from grai_schemas.v1.metadata.nodes import ColumnMetadata, NodeMetadataTypeLabels, TableMetadata
 from multimethod import multimethod
 from pydantic import BaseModel
 
 from grai_source_bigquery.models import (
     ID,
     Column,
     ColumnID,
@@ -62,15 +62,15 @@
             has_default_value=True,
             default_value=current.default_value,
             data_type=current.data_type,
         )
 
     data = {
         "version": version,
-        "node_type": NodeTypeLabels.column.value,
+        "node_type": NodeMetadataTypeLabels.column.value,
         "node_attributes": {
             "data_type": current.data_type,
             "default_value": default_value,
             "is_nullable": None if current.is_nullable else False,  # Only not-nullable is definitive.
             # "is_primary_key": current.is_pk, # This is getting a default value right now
             # "is_unique": # Not support in BQ
         },
@@ -90,15 +90,15 @@
     Returns:
 
     Raises:
 
     """
     data = {
         "version": version,
-        "node_type": NodeTypeLabels.table.value,
+        "node_type": NodeMetadataTypeLabels.table.value,
         "node_attributes": {},
         "tags": [config.metadata_id],
     }
 
     return TableMetadata(**data)
 
 
@@ -115,25 +115,25 @@
     Raises:
 
     """
     data = {"version": version, "tags": [config.metadata_id]}
 
     if isinstance(current.source, TableID):
         if isinstance(current.destination, ColumnID):
-            data["edge_type"] = EdgeTypeLabels.table_to_column.value
+            data["edge_type"] = EdgeMetadataTypeLabels.table_to_column.value
             return TableToColumnMetadata(**data)
         elif isinstance(current.destination, TableID):
-            data["edge_type"] = EdgeTypeLabels.table_to_table.value
+            data["edge_type"] = EdgeMetadataTypeLabels.table_to_table.value
             return TableToTableMetadata(**data)
     elif isinstance(current.source, ColumnID):
         if isinstance(current.destination, ColumnID):
-            data["edge_type"] = EdgeTypeLabels.column_to_column.value
+            data["edge_type"] = EdgeMetadataTypeLabels.column_to_column.value
             return ColumnToColumnMetadata(**data)
 
-    data["edge_type"] = EdgeTypeLabels.generic.value
+    data["edge_type"] = EdgeMetadataTypeLabels.generic.value
     return GenericEdgeMetadataV1(**data)
 
 
 # ---
 
 
 @multimethod
@@ -289,15 +289,15 @@
 
     Returns:
 
     Raises:
 
     """
     metadata = {
-        "node_type": NodeTypeLabels.table.value,
+        "node_type": NodeMetadataTypeLabels.table.value,
         "schema": current.table_schema,
     }
     spec_dict = {
         "name": current.full_name,
         "namespace": current.namespace,
         "display_name": current.name,
         "data_source": config.integration_name,
```

### Comparing `grai_source_bigquery-0.1.0a6/src/grai_source_bigquery/base.py` & `grai_source_bigquery-0.1.1/src/grai_source_bigquery/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.1.0a6/src/grai_source_bigquery/loader.py` & `grai_source_bigquery-0.1.1/src/grai_source_bigquery/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,15 +392,15 @@
             filter_str += (
                 f' AND NOT protoPayload.metadata.jobChange.job.jobStats.queryStats.referencedTables="projects/grai-demo/datasets/{dataset}/tables/INFORMATION_SCHEMA.TABLES"'
                 f' AND NOT protoPayload.metadata.jobInsertion.job.jobStats.queryStats.referencedTables="projects/grai-demo/datasets/{dataset}/tables/INFORMATION_SCHEMA.TABLES"'
                 f' AND NOT protoPayload.metadata.jobChange.job.jobStats.queryStats.referencedTables="projects/grai-demo/datasets/{dataset}/tables/INFORMATION_SCHEMA.COLUMNS"'
                 f' AND NOT protoPayload.metadata.jobInsertion.job.jobStats.queryStats.referencedTables="projects/grai-demo/datasets/{dataset}/tables/INFORMATION_SCHEMA.COLUMNS"'
             )
 
-        return self.logging_connection.list_entries(filter_=filter_str, page_size=1000)
+        return self.logging_connection.list_entries(filter_=filter_str)
 
     def get_bigquery_edges(self, existing_nodes: List[BigqueryNode]) -> List[Edge]:
         """
 
         Args:
 
         Returns:
```

### Comparing `grai_source_bigquery-0.1.0a6/src/grai_source_bigquery/models.py` & `grai_source_bigquery-0.1.1/src/grai_source_bigquery/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.1.0a6/PKG-INFO` & `grai_source_bigquery-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: grai-source-bigquery
-Version: 0.1.0a6
+Version: 0.1.1
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Edward Louth
 Author-email: edward@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: google-cloud-bigquery (>=3.5.0,<4.0.0)
 Requires-Dist: google-cloud-logging (>=3.5.0,<4.0.0)
-Requires-Dist: grai-client (>=0.2.0,<0.3.0)
-Requires-Dist: grai-schemas (>=0.1.9,<0.2.0)
+Requires-Dist: grai-client (>=0.2.18,<0.3.0)
+Requires-Dist: grai-schemas (>=0.1.15,<0.2.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: setuptools (>=67.1.0,<68.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-bigquery
 Description-Content-Type: text/markdown
```

