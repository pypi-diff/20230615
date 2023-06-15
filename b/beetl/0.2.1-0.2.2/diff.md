# Comparing `tmp/beetl-0.2.1.tar.gz` & `tmp/beetl-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beetl-0.2.1.tar", last modified: Thu Jun 15 11:06:25 2023, max compression
+gzip compressed data, was "beetl-0.2.2.tar", last modified: Thu Jun 15 12:27:35 2023, max compression
```

## Comparing `beetl-0.2.1.tar` & `beetl-0.2.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:06:25.762860 beetl-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-15 11:06:25.762860 beetl-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-15 11:05:45.000000 beetl-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:06:25.762860 beetl-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-15 11:05:45.000000 beetl-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:06:25.750860 beetl-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:06:25.754860 beetl-0.2.1/src/beetl/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/beetl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:06:25.758860 beetl-0.2.1/src/beetl/sources/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/sources/faker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/sources/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/sources/itop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/sources/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/sources/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/sources/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/sources/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/sources/sqlserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/sources/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:06:25.762860 beetl-0.2.1/src/beetl/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/transformers/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/transformers/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/transformers/itop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/transformers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/transformers/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/transformers/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/transformers/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:06:25.754860 beetl-0.2.1/src/beetl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-15 11:06:25.000000 beetl-0.2.1/src/beetl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-15 11:06:25.000000 beetl-0.2.1/src/beetl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:06:25.000000 beetl-0.2.1/src/beetl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 11:06:25.000000 beetl-0.2.1/src/beetl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-15 11:06:25.000000 beetl-0.2.1/src/beetl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 11:06:25.000000 beetl-0.2.1/src/beetl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:06:25.000000 beetl-0.2.1/src/beetl.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:27:35.888885 beetl-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-06-15 12:27:35.888885 beetl-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-06-15 12:26:44.000000 beetl-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 12:27:35.888885 beetl-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-15 12:26:44.000000 beetl-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:27:35.880884 beetl-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:27:35.880884 beetl-0.2.2/src/beetl/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/beetl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:27:35.884884 beetl-0.2.2/src/beetl/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/sources/faker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/sources/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/sources/itop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/sources/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/sources/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/sources/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/sources/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/sources/sqlserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/sources/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:27:35.884884 beetl-0.2.2/src/beetl/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/transformers/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/transformers/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/transformers/itop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/transformers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/transformers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/transformers/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-15 12:26:44.000000 beetl-0.2.2/src/beetl/transformers/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:27:35.880884 beetl-0.2.2/src/beetl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-06-15 12:27:35.000000 beetl-0.2.2/src/beetl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-15 12:27:35.000000 beetl-0.2.2/src/beetl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:27:35.000000 beetl-0.2.2/src/beetl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 12:27:35.000000 beetl-0.2.2/src/beetl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-15 12:27:35.000000 beetl-0.2.2/src/beetl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 12:27:35.000000 beetl-0.2.2/src/beetl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:27:35.000000 beetl-0.2.2/src/beetl.egg-info/zip-safe
```

### Comparing `beetl-0.2.1/PKG-INFO` & `beetl-0.2.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beetl
-Version: 0.2.1
+Version: 0.2.2
 Summary: BeETL is a Python package for extracting data from one source, transforming it and loading it into another
 Home-page: https://github.com/Hoglandets-IT/beetl
 Author: Lars Scheibling
 Author-email: lars.scheibling@hoglandet.se
 License: GnuPG 3.0
 Keywords: python template package module cli
 Classifier: Programming Language :: Python :: 3
@@ -151,7 +151,70 @@
             },
             "sourceTransformers": {},
             "insertionTransformers": {}
         }
     ]
 }
 ```
+
+### Secrets from Environment Variables
+In case you want to save your secrets in environment variables instead of in the yaml configuration file, you can save them as a json object to an environment variable and replace the "sources"-section with sourcesFromEnv setting.
+
+Note that the "sources" and "sourcesFromEnv" options are mutually exclusive.
+
+```python
+sync_config = {
+    # The version of the config file, currently V1
+    "version": "V1",
+
+    # Fetch source configuration from environment variable BEETL_SOURCES
+    "sourcesFromEnv": "BEETL_SOURCES",
+
+    # The datasources to move data between
+    "sync": [
+        .....
+```
+
+```yaml
+version: "V1"
+sourcesFromEnv: "BEETL_SOURCES"
+sync:
+  - ......
+```
+
+```json
+{
+    "version": "V1",
+    "sourcesFromEnv": "BEETL_SOURCES",
+    "sync": [
+        ......
+```
+
+The format of the sources configuration is the same as the one normally under the "sources"-section:
+
+```python
+[
+    {
+        # The identifier for the datasource
+        "name": "mysql_db",
+
+        # The type (ex. Sqlserver, Rest, Itop)
+        "type": "Mysql",
+
+        # The connection settings for the datasource (connection string or host/user/password)
+        "connection": {
+            "settings": {
+            "connection_string": "mysql://user:password@host:3306/database"
+            }
+        }
+    },
+    {
+        "name": "postgres_db",
+        "type": "Postgres",
+        "connection": {
+            "settings": {
+            "connection_string": "postgresql://user:password@host:5432/database"
+            }
+        }
+    }
+]
+```
```

### Comparing `beetl-0.2.1/README.md` & `beetl-0.2.2/src/beetl.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: beetl
+Version: 0.2.2
+Summary: BeETL is a Python package for extracting data from one source, transforming it and loading it into another
+Home-page: https://github.com/Hoglandets-IT/beetl
+Author: Lars Scheibling
+Author-email: lars.scheibling@hoglandet.se
+License: GnuPG 3.0
+Keywords: python template package module cli
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 <h1 style="width: 100%; text-align: center; margin-bottom: 20px; border-bottom: 0px;">BeETL: Extensible Python/Polars-based ETL Framework</h1>
 <p style="text-align: center; margin-bottom: 30px;"><img src="./_static/BeETL.png" style="max-width: 400px;"><img src="./docs/_static/BeETL.png" style="max-width: 400px;"><br/></p>
 BeETL was born from a job as Integration Developer where a majority of the integrations we develop follow the same pattern - get here, transform a little, put there (with the middle step frequently missing altogether). 
 
 After building our 16th integration between the same two systems with another manual template, we decided to build BeETL. BeETL is currently limited to one datasource per source and destination per sync, but this will be expanded in the future. One configuration can contain multiple syncs.
 
 Note: Even though most of the configuration below is in YAML format, you can also use JSON or a python dictionary.
@@ -135,8 +150,71 @@
                 ]
             },
             "sourceTransformers": {},
             "insertionTransformers": {}
         }
     ]
 }
-```
+```
+
+### Secrets from Environment Variables
+In case you want to save your secrets in environment variables instead of in the yaml configuration file, you can save them as a json object to an environment variable and replace the "sources"-section with sourcesFromEnv setting.
+
+Note that the "sources" and "sourcesFromEnv" options are mutually exclusive.
+
+```python
+sync_config = {
+    # The version of the config file, currently V1
+    "version": "V1",
+
+    # Fetch source configuration from environment variable BEETL_SOURCES
+    "sourcesFromEnv": "BEETL_SOURCES",
+
+    # The datasources to move data between
+    "sync": [
+        .....
+```
+
+```yaml
+version: "V1"
+sourcesFromEnv: "BEETL_SOURCES"
+sync:
+  - ......
+```
+
+```json
+{
+    "version": "V1",
+    "sourcesFromEnv": "BEETL_SOURCES",
+    "sync": [
+        ......
+```
+
+The format of the sources configuration is the same as the one normally under the "sources"-section:
+
+```python
+[
+    {
+        # The identifier for the datasource
+        "name": "mysql_db",
+
+        # The type (ex. Sqlserver, Rest, Itop)
+        "type": "Mysql",
+
+        # The connection settings for the datasource (connection string or host/user/password)
+        "connection": {
+            "settings": {
+            "connection_string": "mysql://user:password@host:3306/database"
+            }
+        }
+    },
+    {
+        "name": "postgres_db",
+        "type": "Postgres",
+        "connection": {
+            "settings": {
+            "connection_string": "postgresql://user:password@host:5432/database"
+            }
+        }
+    }
+]
+```
```

### Comparing `beetl-0.2.1/setup.py` & `beetl-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `beetl-0.2.1/src/beetl/__version__.py` & `beetl-0.2.2/src/beetl/__version__.py`

 * *Files identical despite different names*

### Comparing `beetl-0.2.1/src/beetl/beetl.py` & `beetl-0.2.2/src/beetl/beetl.py`

 * *Files identical despite different names*

### Comparing `beetl-0.2.1/src/beetl/config.py` & `beetl-0.2.2/src/beetl/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import yaml
 import json
 from typing import List, Dict
 from dataclasses import dataclass
 import copy
 from .sources.interface import (
     SourceInterfaceConfiguration,
@@ -118,18 +119,40 @@
 
 class BeetlConfigV1(BeetlConfig):
     """Version 1 of the Beetl Configuration Interface"""
 
     def __init__(self, config: dict):
         self.sources, self.sync_list = {}, []
 
-        if len(config.get("sources", "")) == 0 or len(config.get("sync", "")) == 0:
+        if len(config.get("sync", "")) == 0:
             raise Exception(
-                "The configuration file is missing the 'sources' or 'sync' section."
+                "The configuration file is missing the 'sync' section."
             )
+        
+        if len(config.get("sources", "")) == 0:
+            if config.get("sourcesFromEnv", "") in [None, ""]:
+                raise Exception(
+                    "The configuration file is missing the 'sources' section."
+                    "If you are using environment variables to configure your sources, "
+                    "please set the 'sourcesFromEnv' property to the name"
+                    "of the environment variable."
+                )
+            
+            sourcesFromEnv = config.pop("sourcesFromEnv")
+            envJson = os.environ.get(sourcesFromEnv)
+            try:
+                envConfig = json.loads(envJson)
+            except Exception as e:
+                raise Exception(
+                    "The environment variable specified in 'sourcesFromEnv' "
+                    "is not a valid JSON string or does not exist."
+                ) from e
+            
+            config["sources"] = envConfig
+            
 
         for source in config["sources"]:
             name = source.pop("name")
             source_type = source.pop("type")
             source_module = __import__(
                 ".".join(
                     self.__module__.split(".")[0:-1]
```

### Comparing `beetl-0.2.1/src/beetl/sources/faker.py` & `beetl-0.2.2/src/beetl/sources/faker.py`

 * *Files identical despite different names*

### Comparing `beetl-0.2.1/src/beetl/sources/interface.py` & `beetl-0.2.2/src/beetl/sources/interface.py`

 * *Files identical despite different names*

### Comparing `beetl-0.2.1/src/beetl/sources/itop.py` & `beetl-0.2.2/src/beetl/sources/itop.py`

 * *Files identical despite different names*

### Comparing `beetl-0.2.1/src/beetl/sources/mongodb.py` & `beetl-0.2.2/src/beetl/sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `beetl-0.2.1/src/beetl/sources/mysql.py` & `beetl-0.2.2/src/beetl/sources/mysql.py`

 * *Files identical despite different names*

### Comparing `beetl-0.2.1/src/beetl/sources/postgres.py` & `beetl-0.2.2/src/beetl/sources/postgres.py`

 * *Files identical despite different names*

### Comparing `beetl-0.2.1/src/beetl/sources/rest.py` & `beetl-0.2.2/src/beetl/sources/rest.py`

 * *Files identical despite different names*

### Comparing `beetl-0.2.1/src/beetl/sources/sqlserver.py` & `beetl-0.2.2/src/beetl/sources/sqlserver.py`

 * *Files identical despite different names*

### Comparing `beetl-0.2.1/src/beetl/sources/static.py` & `beetl-0.2.2/src/beetl/sources/static.py`

 * *Files identical despite different names*

### Comparing `beetl-0.2.1/src/beetl/transformers/frames.py` & `beetl-0.2.2/src/beetl/transformers/frames.py`

 * *Files identical despite different names*

### Comparing `beetl-0.2.1/src/beetl/transformers/interface.py` & `beetl-0.2.2/src/beetl/transformers/interface.py`

 * *Files identical despite different names*

### Comparing `beetl-0.2.1/src/beetl/transformers/itop.py` & `beetl-0.2.2/src/beetl/transformers/itop.py`

 * *Files identical despite different names*

### Comparing `beetl-0.2.1/src/beetl/transformers/misc.py` & `beetl-0.2.2/src/beetl/transformers/misc.py`

 * *Files identical despite different names*

### Comparing `beetl-0.2.1/src/beetl/transformers/regex.py` & `beetl-0.2.2/src/beetl/transformers/regex.py`

 * *Files identical despite different names*

### Comparing `beetl-0.2.1/src/beetl/transformers/strings.py` & `beetl-0.2.2/src/beetl/transformers/strings.py`

 * *Files identical despite different names*

### Comparing `beetl-0.2.1/src/beetl/transformers/structs.py` & `beetl-0.2.2/src/beetl/transformers/structs.py`

 * *Files identical despite different names*

### Comparing `beetl-0.2.1/src/beetl.egg-info/SOURCES.txt` & `beetl-0.2.2/src/beetl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

