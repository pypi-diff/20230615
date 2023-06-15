# Comparing `tmp/macrometa-target-collection-0.0.66.tar.gz` & `tmp/macrometa-target-collection-0.0.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.66.tar", last modified: Thu Jun 15 10:03:19 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.67.tar", last modified: Thu Jun 15 17:19:54 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.66.tar` & `macrometa-target-collection-0.0.67.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:03:19.398758 macrometa-target-collection-0.0.66/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-15 10:02:54.000000 macrometa-target-collection-0.0.66/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-15 10:03:19.398758 macrometa-target-collection-0.0.66/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-15 10:02:54.000000 macrometa-target-collection-0.0.66/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:03:19.394757 macrometa-target-collection-0.0.66/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-15 10:02:54.000000 macrometa-target-collection-0.0.66/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15683 2023-06-15 10:02:54.000000 macrometa-target-collection-0.0.66/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:03:19.398758 macrometa-target-collection-0.0.66/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-15 10:03:19.000000 macrometa-target-collection-0.0.66/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-15 10:03:19.000000 macrometa-target-collection-0.0.66/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:03:19.000000 macrometa-target-collection-0.0.66/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-15 10:03:19.000000 macrometa-target-collection-0.0.66/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-15 10:03:19.000000 macrometa-target-collection-0.0.66/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 10:03:19.000000 macrometa-target-collection-0.0.66/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-15 10:02:54.000000 macrometa-target-collection-0.0.66/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 10:03:19.398758 macrometa-target-collection-0.0.66/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:19:54.643947 macrometa-target-collection-0.0.67/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-15 17:19:33.000000 macrometa-target-collection-0.0.67/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-15 17:19:54.643947 macrometa-target-collection-0.0.67/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-15 17:19:33.000000 macrometa-target-collection-0.0.67/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:19:54.639946 macrometa-target-collection-0.0.67/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-15 17:19:33.000000 macrometa-target-collection-0.0.67/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15889 2023-06-15 17:19:33.000000 macrometa-target-collection-0.0.67/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:19:54.643947 macrometa-target-collection-0.0.67/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-15 17:19:54.000000 macrometa-target-collection-0.0.67/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-15 17:19:54.000000 macrometa-target-collection-0.0.67/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 17:19:54.000000 macrometa-target-collection-0.0.67/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-15 17:19:54.000000 macrometa-target-collection-0.0.67/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-15 17:19:54.000000 macrometa-target-collection-0.0.67/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 17:19:54.000000 macrometa-target-collection-0.0.67/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-15 17:19:34.000000 macrometa-target-collection-0.0.67/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 17:19:54.643947 macrometa-target-collection-0.0.67/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.66/LICENSE` & `macrometa-target-collection-0.0.67/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.66/PKG-INFO` & `macrometa-target-collection-0.0.67/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.66
+Version: 0.0.67
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.66/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.67/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.66/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.67/macrometa_target_collection/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,27 +88,29 @@
     if state is not None:
         line = json.dumps(state)
         logger.debug('Emitting state {}'.format(line))
         sys.stdout.write("{}\n".format(line))
         sys.stdout.flush()
 
 
-def try_upsert(collection: StandardCollection, record_batch: RecordBatch, client, force=False):
-    if record_batch.length() >= record_batch.max_batch_size or force:
+def try_upsert(collection: StandardCollection, record_batch: RecordBatch, client, force=False, count=0):
+    if record_batch.length() > 0 and (record_batch.length() >= record_batch.max_batch_size or force):
         logger.info(f"*** Inside try_upsert if condition. ***")
         start_time = time.time()
+        insert_end_time = None
         to_insert = record_batch.flush()
         all_records = to_insert
         to_update = []
         records_array = remove_time_extracted(to_insert)
 
         for i, r in enumerate(collection.insert_many(records_array)):
             if type(r) is DocumentInsertError:
                 to_update.append(to_insert[i])
             else:
+                insert_end_time = time.time()
                 # Update ingested_documents and ingested_bytes metrics
                 ingested_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                 ingested_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(json.dumps(r)))
                 # Update ingest_lag metric
                 diff = datetime.now(timezone.utc) - ensure_datetime(to_insert[i]["time_extracted"])
                 ingest_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(diff.total_seconds())
 
@@ -125,29 +127,28 @@
                     ingest_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(
                         diff.total_seconds())
         start_delete = time.time()
         try_delete(client, collection)
         end_delete = time.time()
         record_batch.last_executed_time = datetime.now(timezone.utc)
         end_time = time.time()
-        if end_delete - start_delete > 10:
+        if end_delete - start_delete > 10 or count == 50000:
             logger.warn(
-                f"*** Delete Took {end_delete - start_delete}seconds ***")
-        if end_time - start_time > 10:
+                f"*** Delete Took {end_delete - start_delete}seconds, Insert took {start_time - insert_end_time} ***")
+        if end_time - start_time > 10 or count == 50000:
             logger.warn(
                 f"*** Batch Process Took {end_time - start_time}seconds to process:{all_records} ***")
 
 
 def remove_time_extracted(records):
     return [{k: v for k, v in record.items() if k != 'time_extracted'} for record in records]
 
 
 def try_delete(client, collection: StandardCollection):
     try:
-    
         client.execute_query(f"FOR d IN @@collection FILTER d._sdc_deleted_at != null REMOVE d._key IN @@collection",
                                   bind_vars={"@collection": collection.name})
     except Exception as e:
         # Increment ingest_errors metric
         ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
         logger.warn(f'Failed to delete records. {e}')
 
@@ -234,15 +235,15 @@
             except TypeError as e:
                 # Increment ingest_errors metric
                 ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                 # TODO: This is temporary until json serializing issue for Decimals are fixed in pyC8
                 logger.debug("pyC8 error occurred")
 
             state = None
-            try_upsert(collection, record_batch, client)
+            try_upsert(collection, record_batch, client, count=count)
         elif message_type == 'STATE':
             start_time = time.time()
             logger.debug('Setting state to {}'.format(o['value']))
             state = o['value']
             emit_state(state)
             end_time = time.time()
             if end_time - start_time > 10:
```

### Comparing `macrometa-target-collection-0.0.66/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.67/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.66
+Version: 0.0.67
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.66/pyproject.toml` & `macrometa-target-collection-0.0.67/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.66"
+version = "0.0.67"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

