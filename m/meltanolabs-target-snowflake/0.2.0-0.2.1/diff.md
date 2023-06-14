# Comparing `tmp/meltanolabs_target_snowflake-0.2.0.tar.gz` & `tmp/meltanolabs_target_snowflake-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meltanolabs_target_snowflake-0.2.0.tar", max compression
+gzip compressed data, was "meltanolabs_target_snowflake-0.2.1.tar", max compression
```

## Comparing `meltanolabs_target_snowflake-0.2.0.tar` & `meltanolabs_target_snowflake-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     3860 2023-06-14 14:59:00.277687 meltanolabs_target_snowflake-0.2.0/LICENSE
--rw-r--r--   0        0        0     3924 2023-06-14 14:59:00.277687 meltanolabs_target_snowflake-0.2.0/README.md
--rw-r--r--   0        0        0     1282 2023-06-14 14:59:23.657910 meltanolabs_target_snowflake-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       89 2023-06-14 14:59:23.657910 meltanolabs_target_snowflake-0.2.0/target_snowflake/__init__.py
--rw-r--r--   0        0        0    16204 2023-06-14 14:59:00.281687 meltanolabs_target_snowflake-0.2.0/target_snowflake/connector.py
--rw-r--r--   0        0        0     7060 2023-06-14 14:59:00.281687 meltanolabs_target_snowflake-0.2.0/target_snowflake/sinks.py
--rw-r--r--   0        0        0     4057 2023-06-14 14:59:00.281687 meltanolabs_target_snowflake-0.2.0/target_snowflake/target.py
--rw-r--r--   0        0        0     4671 1970-01-01 00:00:00.000000 meltanolabs_target_snowflake-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3860 2023-06-14 22:10:42.781383 meltanolabs_target_snowflake-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3924 2023-06-14 22:10:42.781383 meltanolabs_target_snowflake-0.2.1/README.md
+-rw-r--r--   0        0        0     1282 2023-06-14 22:11:02.493650 meltanolabs_target_snowflake-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       89 2023-06-14 22:11:02.493650 meltanolabs_target_snowflake-0.2.1/target_snowflake/__init__.py
+-rw-r--r--   0        0        0    16397 2023-06-14 22:10:42.785383 meltanolabs_target_snowflake-0.2.1/target_snowflake/connector.py
+-rw-r--r--   0        0        0     7060 2023-06-14 22:10:42.785383 meltanolabs_target_snowflake-0.2.1/target_snowflake/sinks.py
+-rw-r--r--   0        0        0      724 2023-06-14 22:10:42.785383 meltanolabs_target_snowflake-0.2.1/target_snowflake/snowflake_types.py
+-rw-r--r--   0        0        0     4057 2023-06-14 22:10:42.785383 meltanolabs_target_snowflake-0.2.1/target_snowflake/target.py
+-rw-r--r--   0        0        0     4671 1970-01-01 00:00:00.000000 meltanolabs_target_snowflake-0.2.1/PKG-INFO
```

### Comparing `meltanolabs_target_snowflake-0.2.0/LICENSE` & `meltanolabs_target_snowflake-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.2.0/README.md` & `meltanolabs_target_snowflake-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.2.0/pyproject.toml` & `meltanolabs_target_snowflake-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meltanolabs-target-snowflake"
-version = "0.2.0"
+version = "0.2.1"
 description = "`target-snowflake` is a Singer target for Snowflake, built with the Meltano SDK for Singer Targets."
 readme = "README.md"
 authors = ["Ken Payne"]
 keywords = [
     "ELT",
     "Snowflake",
 ]
```

### Comparing `meltanolabs_target_snowflake-0.2.0/target_snowflake/connector.py` & `meltanolabs_target_snowflake-0.2.1/target_snowflake/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from operator import contains, eq
-from typing import Sequence, Tuple, cast, Union, List, Dict
+from typing import Dict, List, Sequence, Tuple, Union, cast
 
-import snowflake.sqlalchemy.custom_types as sct
 import sqlalchemy
 from singer_sdk import typing as th
 from singer_sdk.connectors import SQLConnector
 from snowflake.sqlalchemy import URL
 from snowflake.sqlalchemy.base import SnowflakeIdentifierPreparer
 from snowflake.sqlalchemy.snowdialect import SnowflakeDialect
 from sqlalchemy.engine import Engine
 from sqlalchemy.sql import text
 
+from target_snowflake.snowflake_types import NUMBER, TIMESTAMP_NTZ, VARIANT
+
 
 class TypeMap:
     def __init__(self, operator, map_value, match_value=None):
         self.operator = operator
         self.map_value = map_value
         self.match_value = match_value
 
@@ -193,23 +194,23 @@
         # start with default implementation
         target_type = SQLConnector.to_sql_type(jsonschema_type)
         # snowflake max and default varchar length
         # https://docs.snowflake.com/en/sql-reference/intro-summary-data-types.html
         maxlength = jsonschema_type.get("maxLength", 16777216)
         # define type maps
         string_submaps = [
-            TypeMap(eq, sct.TIMESTAMP_NTZ(), "date-time"),
+            TypeMap(eq, TIMESTAMP_NTZ(), "date-time"),
             TypeMap(contains, sqlalchemy.types.TIME(), "time"),
             TypeMap(eq, sqlalchemy.types.DATE(), "date"),
             TypeMap(eq, sqlalchemy.types.VARCHAR(maxlength), None),
         ]
         type_maps = [
-            TypeMap(th._jsonschema_type_check, sct.NUMBER(), ("integer",)),
-            TypeMap(th._jsonschema_type_check, sct.VARIANT(), ("object",)),
-            TypeMap(th._jsonschema_type_check, sct.VARIANT(), ("array",)),
+            TypeMap(th._jsonschema_type_check, NUMBER(), ("integer",)),
+            TypeMap(th._jsonschema_type_check, VARIANT(), ("object",)),
+            TypeMap(th._jsonschema_type_check, VARIANT(), ("array",)),
         ]
         # apply type maps
         if th._jsonschema_type_check(jsonschema_type, ("string",)):
             datelike_type = th.get_datelike_property_type(jsonschema_type)
             target_type = evaluate_typemaps(string_submaps, datelike_type, target_type)
         else:
             target_type = evaluate_typemaps(type_maps, jsonschema_type, target_type)
@@ -265,19 +266,21 @@
         matched_clause = ", ".join(
             [f'd.{col} = s.{col}' for col in formatted_properties]
         )
         not_matched_insert_cols = ", ".join(formatted_properties)
         not_matched_insert_values = ", ".join(
             [f's.{col}' for col in formatted_properties]
         )
+        dedup_cols = ", ".join([key for key in formatted_key_properties])
+        dedup = f"QUALIFY ROW_NUMBER() OVER (PARTITION BY {dedup_cols} ORDER BY SEQ8() DESC) = 1"
         return (
             text(
                 f"merge into {full_table_name} d using "
                 + f"(select {', '.join(column_selections)} from '@~/target-snowflake/{sync_id}'"
-                + f"(file_format => {file_format})) s "
+                + f"(file_format => {file_format}) {dedup}) s "
                 + f"on {join_expr} "
                 + f"when matched then update set {matched_clause} "
                 + f"when not matched then insert ({not_matched_insert_cols}) "
                 + f"values ({not_matched_insert_values})"
             ),
             {},
         )
```

### Comparing `meltanolabs_target_snowflake-0.2.0/target_snowflake/sinks.py` & `meltanolabs_target_snowflake-0.2.1/target_snowflake/sinks.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.2.0/target_snowflake/target.py` & `meltanolabs_target_snowflake-0.2.1/target_snowflake/target.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.2.0/PKG-INFO` & `meltanolabs_target_snowflake-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meltanolabs-target-snowflake
-Version: 0.2.0
+Version: 0.2.1
 Summary: `target-snowflake` is a Singer target for Snowflake, built with the Meltano SDK for Singer Targets.
 License: Apache 2.0
 Keywords: ELT,Snowflake
 Author: Ken Payne
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

