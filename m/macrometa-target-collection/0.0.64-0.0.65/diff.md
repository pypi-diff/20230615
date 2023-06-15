# Comparing `tmp/macrometa-target-collection-0.0.64.tar.gz` & `tmp/macrometa-target-collection-0.0.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.64.tar", last modified: Mon Jun  5 17:20:18 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.65.tar", last modified: Thu Jun 15 06:09:49 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.64.tar` & `macrometa-target-collection-0.0.65.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:20:18.488135 macrometa-target-collection-0.0.64/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-05 17:19:58.000000 macrometa-target-collection-0.0.64/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-05 17:20:18.488135 macrometa-target-collection-0.0.64/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-05 17:19:58.000000 macrometa-target-collection-0.0.64/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:20:18.484135 macrometa-target-collection-0.0.64/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-05 17:19:58.000000 macrometa-target-collection-0.0.64/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14466 2023-06-05 17:19:58.000000 macrometa-target-collection-0.0.64/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:20:18.488135 macrometa-target-collection-0.0.64/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-05 17:20:18.000000 macrometa-target-collection-0.0.64/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-05 17:20:18.000000 macrometa-target-collection-0.0.64/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:20:18.000000 macrometa-target-collection-0.0.64/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-05 17:20:18.000000 macrometa-target-collection-0.0.64/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-05 17:20:18.000000 macrometa-target-collection-0.0.64/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 17:20:18.000000 macrometa-target-collection-0.0.64/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-05 17:19:58.000000 macrometa-target-collection-0.0.64/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 17:20:18.488135 macrometa-target-collection-0.0.64/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:09:49.169020 macrometa-target-collection-0.0.65/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-15 06:09:28.000000 macrometa-target-collection-0.0.65/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-15 06:09:49.169020 macrometa-target-collection-0.0.65/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-15 06:09:28.000000 macrometa-target-collection-0.0.65/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:09:49.165019 macrometa-target-collection-0.0.65/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-15 06:09:28.000000 macrometa-target-collection-0.0.65/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15628 2023-06-15 06:09:28.000000 macrometa-target-collection-0.0.65/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:09:49.169020 macrometa-target-collection-0.0.65/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-15 06:09:49.000000 macrometa-target-collection-0.0.65/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-15 06:09:49.000000 macrometa-target-collection-0.0.65/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:09:49.000000 macrometa-target-collection-0.0.65/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-15 06:09:49.000000 macrometa-target-collection-0.0.65/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-15 06:09:49.000000 macrometa-target-collection-0.0.65/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 06:09:49.000000 macrometa-target-collection-0.0.65/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-15 06:09:28.000000 macrometa-target-collection-0.0.65/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 06:09:49.169020 macrometa-target-collection-0.0.65/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.64/LICENSE` & `macrometa-target-collection-0.0.65/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.64/PKG-INFO` & `macrometa-target-collection-0.0.65/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.64
+Version: 0.0.65
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.64/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.65/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.64/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.65/macrometa_target_collection/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -90,15 +90,18 @@
         logger.debug('Emitting state {}'.format(line))
         sys.stdout.write("{}\n".format(line))
         sys.stdout.flush()
 
 
 def try_upsert(collection: StandardCollection, record_batch: RecordBatch, client, force=False):
     if record_batch.length() >= record_batch.max_batch_size or force:
+        logger.info(f"*** Inside try_upsert if condition. ***")
+        start_time = time.time()
         to_insert = record_batch.flush()
+        all_records = to_insert
         to_update = []
         records_array = remove_time_extracted(to_insert)
 
         for i, r in enumerate(collection.insert_many(records_array)):
             if type(r) is DocumentInsertError:
                 to_update.append(to_insert[i])
             else:
@@ -117,16 +120,25 @@
                     ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                     logger.warn(f'Failed to insert/update record: {to_update[i]}. {r}')
                 else:
                     # Update ingest_lag metric
                     diff = datetime.now(timezone.utc) - ensure_datetime(to_update[i]["time_extracted"])
                     ingest_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(
                         diff.total_seconds())
+        start_delete = time.time()
         try_delete(client, collection)
+        end_delete = time.time()
         record_batch.last_executed_time = datetime.now(timezone.utc)
+        end_time = time.time()
+        if end_delete - start_delete > 10:
+            logger.warn(
+                f"*** Delete Took {end_delete - start_delete}seconds ***")
+        if end_time - start_time > 10:
+            logger.warn(
+                f"*** Batch Process Took {end_time - start_time}seconds to process:{all_records} ***")
 
 
 def remove_time_extracted(records):
     return [{k: v for k, v in record.items() if k != 'time_extracted'} for record in records]
 
 
 def try_delete(client, collection: StandardCollection):
@@ -141,26 +153,30 @@
 
 
 def persist_messages(collection: StandardCollection, messages: io.TextIOWrapper, record_batch: RecordBatch, client):
     state = None
     schemas = {}
     key_properties = {}
     validators = {}
+    count = 0
 
     for message in messages:
         try:
             o = json.loads(message)
         except json.decoder.JSONDecodeError as e:
             # Increment ingest_errors metric
             ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
             logger.error(f"Unable to parse:\n{message}")
             raise e
 
         message_type = o['type']
         if message_type == 'RECORD':
+            count += 1
+            if count >= 184800:
+                logger.info(f"*** Record {count} is {o['record']} ***")
             stream = o['stream']
             if stream not in schemas:
                 # Increment ingest_errors metric
                 ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                 raise Exception(f"A record for stream {stream} was encountered before a corresponding schema")
 
             try:
@@ -220,23 +236,33 @@
                 ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                 # TODO: This is temporary until json serializing issue for Decimals are fixed in pyC8
                 logger.debug("pyC8 error occurred")
 
             state = None
             try_upsert(collection, record_batch, client)
         elif message_type == 'STATE':
+            start_time = time.time()
             logger.debug('Setting state to {}'.format(o['value']))
             state = o['value']
             emit_state(state)
+            end_time = time.time()
+            if end_time - start_time > 10:
+                logger.warn(
+                    f"*** State Process Took {end_time - start_time}seconds to process:{o} ***")
         elif message_type == 'SCHEMA':
+            start_time = time.time()
             stream = o['stream']
             schemas[stream] = o['schema']
             adjust_decimal_precision_for_schema(schemas[stream])
             validators[stream] = Draft4Validator((o['schema']))
             key_properties[stream] = o['key_properties']
+            end_time = time.time()
+            if end_time - start_time > 10:
+                logger.warn(
+                    f"*** Schema Process Took {end_time - start_time}seconds to process:{o} ***")
         else:
             # Increment ingest_errors metric
             ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
             logger.warning("Unknown message type {} in message {}".format(o['type'], o))
 
     scrape_complete_flag.labels(workflow_label).inc()
     return state
```

### Comparing `macrometa-target-collection-0.0.64/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.65/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.64
+Version: 0.0.65
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.64/pyproject.toml` & `macrometa-target-collection-0.0.65/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.64"
+version = "0.0.65"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

