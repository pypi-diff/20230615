# Comparing `tmp/kast_flow_api_python-1.0.1.tar.gz` & `tmp/kast_flow_api_python-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kast_flow_api_python-1.0.1.tar", max compression
+gzip compressed data, was "kast_flow_api_python-1.0.2.tar", max compression
```

## Comparing `kast_flow_api_python-1.0.1.tar` & `kast_flow_api_python-1.0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-11 06:36:38.862227 kast_flow_api_python-1.0.1/kast_flow_api/__init__.py
--rw-r--r--   0        0        0     8347 2023-06-11 06:33:21.816761 kast_flow_api_python-1.0.1/kast_flow_api/v1.py
--rw-r--r--   0        0        0      528 2023-06-11 06:36:57.487179 kast_flow_api_python-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 kast_flow_api_python-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-15 11:03:06.962366 kast_flow_api_python-1.0.2/kast_flow_api/__init__.py
+-rw-r--r--   0        0        0     8783 2023-06-15 11:03:06.934366 kast_flow_api_python-1.0.2/kast_flow_api/v1.py
+-rw-r--r--   0        0        0      528 2023-06-15 11:03:27.019413 kast_flow_api_python-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 kast_flow_api_python-1.0.2/PKG-INFO
```

### Comparing `kast_flow_api_python-1.0.1/kast_flow_api/v1.py` & `kast_flow_api_python-1.0.2/kast_flow_api/v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,32 @@
 import time
 from dataclasses import asdict, dataclass, field, fields
-from enum import Enum
+from enum import Enum, StrEnum
 from functools import wraps
 from typing import Any, Callable, Protocol, Self, Tuple, Type, TypeVar, cast
 
 from dacite import Config, from_dict
 
 
+class KastFormat(StrEnum):
+    AVRO = "avro"
+    JSON = "json"
+    CSV = "csv"
+    PARQUET = "parquet"
+
+    @staticmethod
+    def unmarshal(format: str) -> "KastFormat":
+        try:
+            return KastFormat(format)
+        except ValueError as e:
+            raise KastFunctionInvalidArgumentsException(message=[
+                ["KastFormat", f"shoud be one of {list(map(str, KastFormat))}"],
+            ], errors=e)
+
+
 class KastDataFrameBackend(Enum):
     NOTSET = "notset"
     PANDAS = "pandas"
     PYSPARK = "pyspark"
 
     @staticmethod
     def from_string(s: str) -> "KastDataFrameBackend":
```

### Comparing `kast_flow_api_python-1.0.1/pyproject.toml` & `kast_flow_api_python-1.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kast-flow-api-python"
-version = "1.0.1"
+version = "1.0.2"
 description = "kast python api unified processing engine"
 authors = ["kast"]
 packages = [
     { include = "kast_flow_api" }
 ]
 
 [tool.poetry.dependencies]
```

