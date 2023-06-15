# Comparing `tmp/resotodatalink-1.0.0.tar.gz` & `tmp/resotodatalink-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotodatalink-1.0.0.tar", last modified: Tue Jun 13 13:35:49 2023, max compression
+gzip compressed data, was "resotodatalink-1.0.1.tar", last modified: Thu Jun 15 06:49:02 2023, max compression
```

## Comparing `resotodatalink-1.0.0.tar` & `resotodatalink-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:35:49.359760 resotodatalink-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 13:30:42.000000 resotodatalink-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-06-13 13:35:49.359760 resotodatalink-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-13 13:30:42.000000 resotodatalink-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-13 13:30:42.000000 resotodatalink-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:35:49.359760 resotodatalink-1.0.0/resotodatalink/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:30:42.000000 resotodatalink-1.0.0/resotodatalink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-13 13:30:42.000000 resotodatalink-1.0.0/resotodatalink/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:35:49.359760 resotodatalink-1.0.0/resotodatalink/arrow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:30:42.000000 resotodatalink-1.0.0/resotodatalink/arrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-13 13:30:42.000000 resotodatalink-1.0.0/resotodatalink/arrow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-13 13:30:42.000000 resotodatalink-1.0.0/resotodatalink/arrow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-13 13:30:42.000000 resotodatalink-1.0.0/resotodatalink/arrow/type_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-06-13 13:30:42.000000 resotodatalink-1.0.0/resotodatalink/arrow/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-06-13 13:30:42.000000 resotodatalink-1.0.0/resotodatalink/collect_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-13 13:30:42.000000 resotodatalink-1.0.0/resotodatalink/remote_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-13 13:30:42.000000 resotodatalink-1.0.0/resotodatalink/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-13 13:30:42.000000 resotodatalink-1.0.0/resotodatalink/show_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-13 13:30:42.000000 resotodatalink-1.0.0/resotodatalink/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-06-13 13:30:42.000000 resotodatalink-1.0.0/resotodatalink/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:35:49.359760 resotodatalink-1.0.0/resotodatalink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-06-13 13:35:49.000000 resotodatalink-1.0.0/resotodatalink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-13 13:35:49.000000 resotodatalink-1.0.0/resotodatalink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:35:49.000000 resotodatalink-1.0.0/resotodatalink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-13 13:35:49.000000 resotodatalink-1.0.0/resotodatalink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-13 13:35:49.000000 resotodatalink-1.0.0/resotodatalink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-13 13:35:49.359760 resotodatalink-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:49:02.466517 resotodatalink-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-06-15 06:49:02.466517 resotodatalink-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:49:02.466517 resotodatalink-1.0.1/resotodatalink/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:49:02.466517 resotodatalink-1.0.1/resotodatalink/arrow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/arrow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/arrow/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/arrow/type_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/arrow/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/collect_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/remote_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/show_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:49:02.466517 resotodatalink-1.0.1/resotodatalink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-06-15 06:49:02.000000 resotodatalink-1.0.1/resotodatalink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-15 06:49:02.000000 resotodatalink-1.0.1/resotodatalink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:49:02.000000 resotodatalink-1.0.1/resotodatalink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-15 06:49:02.000000 resotodatalink-1.0.1/resotodatalink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 06:49:02.000000 resotodatalink-1.0.1/resotodatalink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-15 06:49:02.466517 resotodatalink-1.0.1/setup.cfg
```

### Comparing `resotodatalink-1.0.0/LICENSE` & `resotodatalink-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.0.0/PKG-INFO` & `resotodatalink-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotodatalink
-Version: 1.0.0
+Version: 1.0.1
 Summary: Data Pipelines for Resoto infrastructure data.
 Author: Some Engineering Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -221,14 +221,15 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: snowflake
 Provides-Extra: mysql
 Provides-Extra: parquet
 Provides-Extra: postgres
+Provides-Extra: extra
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # resotodatalink
 Data Pipelines for Resoto infrastructure data
```

### Comparing `resotodatalink-1.0.0/pyproject.toml` & `resotodatalink-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resotodatalink"
-version = "1.0.0"
+version = "1.0.1"
 authors = [{name="Some Engineering Inc."}]
 description = "Data Pipelines for Resoto infrastructure data."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -39,14 +39,24 @@
 
 # The different database backends we have tested explicitly
 snowflake = [ "snowflake-sqlalchemy" ]
 mysql = [ "pymysql" ]
 parquet = [ "pyarrow", "boto3", "google-cloud-storage" ]
 postgres = [ "psycopg2-binary" ]
 
+# All extra dependencies
+extra = [
+    "boto3",
+    "google-cloud-storage",
+    "pymysql",
+    "psycopg2-binary",
+    "pyarrow",
+    "snowflake-sqlalchemy",
+]
+
 # All dev dependencies
 dev = [ "pip-tools" ]
 
 # All test dependencies
 test = [
     "black",
     "coverage",
@@ -69,7 +79,9 @@
 Documentation = "https://resoto.com"
 Source = "https://github.com/someengineering/resotodatalink"
 
 [build-system]
 requires = ["setuptools>=67.8.0", "wheel>=0.40.0", "build>=0.10.0"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools.package-data]
+resotodatalink = ["py.typed"]
```

### Comparing `resotodatalink-1.0.0/resotodatalink/analytics.py` & `resotodatalink-1.0.1/resotodatalink/analytics.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.0.0/resotodatalink/arrow/config.py` & `resotodatalink-1.0.1/resotodatalink/arrow/config.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.0.0/resotodatalink/arrow/model.py` & `resotodatalink-1.0.1/resotodatalink/arrow/model.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.0.0/resotodatalink/arrow/type_converter.py` & `resotodatalink-1.0.1/resotodatalink/arrow/type_converter.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.0.0/resotodatalink/arrow/writer.py` & `resotodatalink-1.0.1/resotodatalink/arrow/writer.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.0.0/resotodatalink/collect_plugins.py` & `resotodatalink-1.0.1/resotodatalink/collect_plugins.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from collections import defaultdict
 from logging import getLogger
 from typing import Dict, List, Tuple, Set
 
+import jsons
 from resotoclient import Kind, Model
 from resotolib.baseplugin import BaseCollectorPlugin
 from resotolib.baseresources import BaseResource, EdgeType
 from resotolib.core.actions import CoreFeedback
 from resotolib.core.model_export import node_to_dict
-from resotolib.json import from_json
 from resotolib.types import Json
 from sqlalchemy.engine import Engine
 
 from resotodatalink.arrow.config import ArrowOutputConfig
 from resotodatalink.sql import sql_updater
 
 try:
@@ -40,15 +40,16 @@
 def collect_to_file(
     collector: BaseCollectorPlugin, feedback: CoreFeedback, output_config: ArrowOutputConfig
 ) -> Tuple[str, int, int]:
     # collect cloud data
     feedback.progress_done(collector.cloud, 0, 1)
     collector.collect()
     # read the kinds created from this collector
-    kinds = [from_json(m, Kind) for m in collector.graph.export_model(walk_subclasses=False)]
+    # Note: Kind is a dataclass - from_json can only handle attrs
+    kinds = [jsons.load(m, Kind) for m in collector.graph.export_model(walk_subclasses=False)]
     model = ArrowModel(Model({k.fqn: k for k in kinds}), output_config.format)
     node_edge_count = len(collector.graph.nodes) + len(collector.graph.edges)
     ne_current = 0
     progress_update = max(node_edge_count // 100, 1)
     feedback.progress_done("sync_db", 0, node_edge_count, context=[collector.cloud])
 
     # group all edges by kind of from/to
@@ -97,15 +98,16 @@
     edges_by_kind: Dict[Tuple[str, str], List[Json]] = defaultdict(list)
     for from_node, to_node, key in collector.graph.edges:
         if key.edge_type == EdgeType.default:
             edge_node = {"from": from_node.chksum, "to": to_node.chksum, "type": "edge"}
             edges_by_kind[(from_node.kind, to_node.kind)].append(edge_node)
 
     # read the kinds created from this collector
-    kinds = [from_json(m, Kind) for m in collector.graph.export_model(walk_subclasses=False)]
+    # Note: Kind is a dataclass - from_json can only handle attrs
+    kinds = [jsons.load(m, Kind) for m in collector.graph.export_model(walk_subclasses=False)]
     updater = sql_updater(Model({k.fqn: k for k in kinds}), engine)
     node_edge_count = len(collector.graph.nodes) + len(collector.graph.edges)
     ne_count = 0
     schema = f"create temp tables {engine.dialect.name}"
     syncdb = f"synchronize {engine.dialect.name}"
     feedback.progress_done(schema, 0, 1, context=[collector.cloud])
     feedback.progress_done(syncdb, 0, node_edge_count, context=[collector.cloud])
```

### Comparing `resotodatalink-1.0.0/resotodatalink/remote_graph.py` & `resotodatalink-1.0.1/resotodatalink/remote_graph.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.0.0/resotodatalink/schema_utils.py` & `resotodatalink-1.0.1/resotodatalink/schema_utils.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.0.0/resotodatalink/show_progress.py` & `resotodatalink-1.0.1/resotodatalink/show_progress.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.0.0/resotodatalink/snowflake.py` & `resotodatalink-1.0.1/resotodatalink/snowflake.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.0.0/resotodatalink/sql.py` & `resotodatalink-1.0.1/resotodatalink/sql.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.0.0/resotodatalink.egg-info/PKG-INFO` & `resotodatalink-1.0.1/resotodatalink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotodatalink
-Version: 1.0.0
+Version: 1.0.1
 Summary: Data Pipelines for Resoto infrastructure data.
 Author: Some Engineering Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -221,14 +221,15 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: snowflake
 Provides-Extra: mysql
 Provides-Extra: parquet
 Provides-Extra: postgres
+Provides-Extra: extra
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # resotodatalink
 Data Pipelines for Resoto infrastructure data
```

