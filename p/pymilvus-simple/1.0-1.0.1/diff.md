# Comparing `tmp/pymilvus_simple-1.0.tar.gz` & `tmp/pymilvus_simple-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/filiphaltmayer/Documents/packages_clean/pymilvus-simple/dist/.tmp-2wchgfx4/pymilvus_simple-1.0.tar", last modified: Mon Jun 12 20:59:10 2023, max compression
+gzip compressed data, was "/Users/filiphaltmayer/Documents/packages_clean/pymilvus-simple/dist/.tmp-13rohxag/pymilvus_simple-1.0.1.tar", last modified: Wed Jun 14 22:54:03 2023, max compression
```

## Comparing `pymilvus_simple-1.0.tar` & `pymilvus_simple-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 filiphaltmayer   (501) staff       (20)        0 2023-06-12 20:59:10.339100 pymilvus_simple-1.0/
--rw-r--r--   0 filiphaltmayer   (501) staff       (20)      249 2023-06-12 20:59:10.338695 pymilvus_simple-1.0/PKG-INFO
--rw-r--r--   0 filiphaltmayer   (501) staff       (20)       18 2023-06-12 20:45:08.000000 pymilvus_simple-1.0/README.md
-drwxr-xr-x   0 filiphaltmayer   (501) staff       (20)        0 2023-06-12 20:59:10.332873 pymilvus_simple-1.0/pymilvus_simple/
--rw-r--r--   0 filiphaltmayer   (501) staff       (20)        0 2023-06-12 20:21:15.000000 pymilvus_simple-1.0/pymilvus_simple/__init__.py
--rw-r--r--   0 filiphaltmayer   (501) staff       (20)    31129 2023-06-12 20:53:45.000000 pymilvus_simple-1.0/pymilvus_simple/simple_api.py
--rw-r--r--   0 filiphaltmayer   (501) staff       (20)      572 2023-06-12 20:21:15.000000 pymilvus_simple-1.0/pymilvus_simple/simple_api_exceptions.py
-drwxr-xr-x   0 filiphaltmayer   (501) staff       (20)        0 2023-06-12 20:59:10.336974 pymilvus_simple-1.0/pymilvus_simple.egg-info/
--rw-r--r--   0 filiphaltmayer   (501) staff       (20)      249 2023-06-12 20:59:10.000000 pymilvus_simple-1.0/pymilvus_simple.egg-info/PKG-INFO
--rw-r--r--   0 filiphaltmayer   (501) staff       (20)      340 2023-06-12 20:59:10.000000 pymilvus_simple-1.0/pymilvus_simple.egg-info/SOURCES.txt
--rw-r--r--   0 filiphaltmayer   (501) staff       (20)        1 2023-06-12 20:59:10.000000 pymilvus_simple-1.0/pymilvus_simple.egg-info/dependency_links.txt
--rw-r--r--   0 filiphaltmayer   (501) staff       (20)       16 2023-06-12 20:59:10.000000 pymilvus_simple-1.0/pymilvus_simple.egg-info/requires.txt
--rw-r--r--   0 filiphaltmayer   (501) staff       (20)       16 2023-06-12 20:59:10.000000 pymilvus_simple-1.0/pymilvus_simple.egg-info/top_level.txt
--rw-r--r--   0 filiphaltmayer   (501) staff       (20)      117 2023-06-12 20:54:50.000000 pymilvus_simple-1.0/pyproject.toml
--rw-r--r--   0 filiphaltmayer   (501) staff       (20)       38 2023-06-12 20:59:10.339243 pymilvus_simple-1.0/setup.cfg
--rw-r--r--   0 filiphaltmayer   (501) staff       (20)      439 2023-06-12 20:46:25.000000 pymilvus_simple-1.0/setup.py
-drwxr-xr-x   0 filiphaltmayer   (501) staff       (20)        0 2023-06-12 20:59:10.337574 pymilvus_simple-1.0/tests/
--rw-r--r--   0 filiphaltmayer   (501) staff       (20)     7516 2023-06-12 20:53:28.000000 pymilvus_simple-1.0/tests/test.py
+drwxr-xr-x   0 filiphaltmayer   (501) staff       (20)        0 2023-06-14 22:54:03.269438 pymilvus_simple-1.0.1/
+-rw-r--r--   0 filiphaltmayer   (501) staff       (20)      251 2023-06-14 22:54:03.268820 pymilvus_simple-1.0.1/PKG-INFO
+-rw-r--r--   0 filiphaltmayer   (501) staff       (20)       18 2023-06-12 20:45:08.000000 pymilvus_simple-1.0.1/README.md
+drwxr-xr-x   0 filiphaltmayer   (501) staff       (20)        0 2023-06-14 22:54:03.263962 pymilvus_simple-1.0.1/pymilvus_simple/
+-rw-r--r--   0 filiphaltmayer   (501) staff       (20)        0 2023-06-12 20:21:15.000000 pymilvus_simple-1.0.1/pymilvus_simple/__init__.py
+-rw-r--r--   0 filiphaltmayer   (501) staff       (20)    31343 2023-06-14 22:48:34.000000 pymilvus_simple-1.0.1/pymilvus_simple/simple_api.py
+-rw-r--r--   0 filiphaltmayer   (501) staff       (20)      572 2023-06-12 20:21:15.000000 pymilvus_simple-1.0.1/pymilvus_simple/simple_api_exceptions.py
+drwxr-xr-x   0 filiphaltmayer   (501) staff       (20)        0 2023-06-14 22:54:03.267204 pymilvus_simple-1.0.1/pymilvus_simple.egg-info/
+-rw-r--r--   0 filiphaltmayer   (501) staff       (20)      251 2023-06-14 22:54:03.000000 pymilvus_simple-1.0.1/pymilvus_simple.egg-info/PKG-INFO
+-rw-r--r--   0 filiphaltmayer   (501) staff       (20)      340 2023-06-14 22:54:03.000000 pymilvus_simple-1.0.1/pymilvus_simple.egg-info/SOURCES.txt
+-rw-r--r--   0 filiphaltmayer   (501) staff       (20)        1 2023-06-14 22:54:03.000000 pymilvus_simple-1.0.1/pymilvus_simple.egg-info/dependency_links.txt
+-rw-r--r--   0 filiphaltmayer   (501) staff       (20)       16 2023-06-14 22:54:03.000000 pymilvus_simple-1.0.1/pymilvus_simple.egg-info/requires.txt
+-rw-r--r--   0 filiphaltmayer   (501) staff       (20)       16 2023-06-14 22:54:03.000000 pymilvus_simple-1.0.1/pymilvus_simple.egg-info/top_level.txt
+-rw-r--r--   0 filiphaltmayer   (501) staff       (20)      117 2023-06-14 22:48:34.000000 pymilvus_simple-1.0.1/pyproject.toml
+-rw-r--r--   0 filiphaltmayer   (501) staff       (20)       38 2023-06-14 22:54:03.269622 pymilvus_simple-1.0.1/setup.cfg
+-rw-r--r--   0 filiphaltmayer   (501) staff       (20)      441 2023-06-14 22:53:32.000000 pymilvus_simple-1.0.1/setup.py
+drwxr-xr-x   0 filiphaltmayer   (501) staff       (20)        0 2023-06-14 22:54:03.267682 pymilvus_simple-1.0.1/tests/
+-rw-r--r--   0 filiphaltmayer   (501) staff       (20)     7517 2023-06-14 22:48:34.000000 pymilvus_simple-1.0.1/tests/test.py
```

### Comparing `pymilvus_simple-1.0/pymilvus_simple/simple_api.py` & `pymilvus_simple-1.0.1/pymilvus_simple/simple_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -499,15 +499,17 @@
             output_fields.remove(vec_field)
             include_vectors = True
         except ValueError:
             pass
 
         expr = []
 
-        if partition_keys is not None and len(partition_keys) != 0:
+        partition_keys = [] if partition_keys is None else partition_keys
+
+        if len(partition_keys) != 0:
             partition_field = schema["partition_key_field"]
             expr.append(self._fetch_formatter(partition_field, partition_keys))
 
         if filter_expression is not None:
             expr.append(filter_expression)
 
         expr = " and ".join(expr)
@@ -557,15 +559,15 @@
                     count += 1
 
         return ret
 
     def query(
         self,
         collection_name: str,
-        filter_expression: str,
+        filter_expression: str = None,
         output_fields: List[str] = None,
         include_vectors: bool = False,
         partition_keys: List[Union[str, int]] = None,
         timeout: int = None,
         consistency_level: str = None,
     ) -> List[dict]:
         """Query the collection for values based on an expression.
@@ -600,21 +602,25 @@
         # Grab necessary schema info
         schema = self.describe_collection(collection_name)
         primary_field = schema["primary_field"]
         vec_field = schema["vector_field"]
 
         expr = []
 
+        partition_keys = [] if partition_keys is None else partition_keys
+
         # Check if we are performing a partition search
-        if partition_keys is not None and len(partition_keys) != 0:
+        if len(partition_keys) != 0:
             partition_field = schema["partition_key_field"]
             expr.append(self._fetch_formatter(partition_field, partition_keys))
 
         # Combine the filter expression with filter for partition
-        expr.append(filter_expression)
+        if filter_expression is not None:
+            expr.append(filter_expression)
+
         expr = " and ".join(expr)
 
         # Check if returning all data
         if output_fields is None or len(output_fields) == 0:
             output_fields = ["*"]
 
         # Change logic to avoid two output_field searches
@@ -680,22 +686,24 @@
 
         schema = self.describe_collection(collection_name, extra=True)
 
         primary_field = schema["primary_field"]
 
         expr = []
 
-        if partition_keys is not None and len(partition_keys) != 0:
+        partition_keys = [] if partition_keys is None else partition_keys
+
+        if len(partition_keys) != 0:
             partition_field = schema["partition_key_field"]
             expr.append(self._fetch_formatter(partition_field, partition_keys))
 
         expr.append(self._fetch_formatter(field=field_name, values=values))
         expr = " and ".join(expr)
 
-        if field_name != primary_field:
+        if field_name != primary_field or len(partition_keys) != 0:
             pks = self.conn.query(
                 collection_name=collection_name,
                 expr=expr,
                 timeout=timeout,
                 consistency_level=consistency_level,
             )
             field_name = primary_field
```

### Comparing `pymilvus_simple-1.0/pymilvus_simple/simple_api_exceptions.py` & `pymilvus_simple-1.0.1/pymilvus_simple/simple_api_exceptions.py`

 * *Files identical despite different names*

### Comparing `pymilvus_simple-1.0/tests/test.py` & `pymilvus_simple-1.0.1/tests/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     Collection,
     CollectionSchema,
     DataType,
     utility,
 )
 
 from pymilvus_simple.simple_api import SimpleAPI
+
 connections.connect()
 
 for x in utility.list_collections():
     utility.drop_collection(x)
 
 z = SimpleAPI()
```

