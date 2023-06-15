# Comparing `tmp/kast_flow_api_python-1.0.2.tar.gz` & `tmp/kast_flow_api_python-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kast_flow_api_python-1.0.2.tar", max compression
+gzip compressed data, was "kast_flow_api_python-1.0.3.tar", max compression
```

## Comparing `kast_flow_api_python-1.0.2.tar` & `kast_flow_api_python-1.0.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-15 11:03:06.962366 kast_flow_api_python-1.0.2/kast_flow_api/__init__.py
--rw-r--r--   0        0        0     8783 2023-06-15 11:03:06.934366 kast_flow_api_python-1.0.2/kast_flow_api/v1.py
--rw-r--r--   0        0        0      528 2023-06-15 11:03:27.019413 kast_flow_api_python-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 kast_flow_api_python-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-15 11:14:06.166894 kast_flow_api_python-1.0.3/kast_flow_api/__init__.py
+-rw-r--r--   0        0        0     8864 2023-06-15 11:14:05.927894 kast_flow_api_python-1.0.3/kast_flow_api/v1.py
+-rw-r--r--   0        0        0      528 2023-06-15 11:14:26.053940 kast_flow_api_python-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 kast_flow_api_python-1.0.3/PKG-INFO
```

### Comparing `kast_flow_api_python-1.0.2/kast_flow_api/v1.py` & `kast_flow_api_python-1.0.3/kast_flow_api/v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,20 @@
     PARQUET = "parquet"
 
     @staticmethod
     def unmarshal(format: str) -> "KastFormat":
         try:
             return KastFormat(format)
         except ValueError as e:
-            raise KastFunctionInvalidArgumentsException(message=[
-                ["KastFormat", f"shoud be one of {list(map(str, KastFormat))}"],
-            ], errors=e)
+            raise KastFunctionInvalidArgumentsException(
+                message=[
+                    ["KastFormat", f"shoud be one of {list(map(str, KastFormat))}"],
+                ],
+                errors=e,
+            )
 
 
 class KastDataFrameBackend(Enum):
     NOTSET = "notset"
     PANDAS = "pandas"
     PYSPARK = "pyspark"
 
@@ -120,14 +123,15 @@
     type: str = "table"
 
 
 class KastTool(Protocol):
     def newKastDataFrame(
         self: Self,
         df: Any,
+        schema: str = "",
     ) -> KastDataFrame:
         ...
 
     def emptyKastDataFrame(self: Self) -> KastDataFrame:
         ...
```

### Comparing `kast_flow_api_python-1.0.2/pyproject.toml` & `kast_flow_api_python-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kast-flow-api-python"
-version = "1.0.2"
+version = "1.0.3"
 description = "kast python api unified processing engine"
 authors = ["kast"]
 packages = [
     { include = "kast_flow_api" }
 ]
 
 [tool.poetry.dependencies]
```

