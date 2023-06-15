# Comparing `tmp/macrometa-target-collection-0.0.65.tar.gz` & `tmp/macrometa-target-collection-0.0.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.65.tar", last modified: Thu Jun 15 06:09:49 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.66.tar", last modified: Thu Jun 15 10:03:19 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.65.tar` & `macrometa-target-collection-0.0.66.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:09:49.169020 macrometa-target-collection-0.0.65/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-15 06:09:28.000000 macrometa-target-collection-0.0.65/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-15 06:09:49.169020 macrometa-target-collection-0.0.65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-15 06:09:28.000000 macrometa-target-collection-0.0.65/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:09:49.165019 macrometa-target-collection-0.0.65/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-15 06:09:28.000000 macrometa-target-collection-0.0.65/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15628 2023-06-15 06:09:28.000000 macrometa-target-collection-0.0.65/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:09:49.169020 macrometa-target-collection-0.0.65/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-15 06:09:49.000000 macrometa-target-collection-0.0.65/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-15 06:09:49.000000 macrometa-target-collection-0.0.65/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:09:49.000000 macrometa-target-collection-0.0.65/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-15 06:09:49.000000 macrometa-target-collection-0.0.65/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-15 06:09:49.000000 macrometa-target-collection-0.0.65/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 06:09:49.000000 macrometa-target-collection-0.0.65/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-15 06:09:28.000000 macrometa-target-collection-0.0.65/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 06:09:49.169020 macrometa-target-collection-0.0.65/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:03:19.398758 macrometa-target-collection-0.0.66/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-15 10:02:54.000000 macrometa-target-collection-0.0.66/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-15 10:03:19.398758 macrometa-target-collection-0.0.66/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-15 10:02:54.000000 macrometa-target-collection-0.0.66/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:03:19.394757 macrometa-target-collection-0.0.66/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-15 10:02:54.000000 macrometa-target-collection-0.0.66/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15683 2023-06-15 10:02:54.000000 macrometa-target-collection-0.0.66/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:03:19.398758 macrometa-target-collection-0.0.66/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-15 10:03:19.000000 macrometa-target-collection-0.0.66/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-15 10:03:19.000000 macrometa-target-collection-0.0.66/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:03:19.000000 macrometa-target-collection-0.0.66/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-15 10:03:19.000000 macrometa-target-collection-0.0.66/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-15 10:03:19.000000 macrometa-target-collection-0.0.66/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 10:03:19.000000 macrometa-target-collection-0.0.66/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-15 10:02:54.000000 macrometa-target-collection-0.0.66/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 10:03:19.398758 macrometa-target-collection-0.0.66/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.65/LICENSE` & `macrometa-target-collection-0.0.66/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.65/PKG-INFO` & `macrometa-target-collection-0.0.66/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.65
+Version: 0.0.66
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.65/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.66/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.65/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.66/macrometa_target_collection/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
             ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
             logger.error(f"Unable to parse:\n{message}")
             raise e
 
         message_type = o['type']
         if message_type == 'RECORD':
             count += 1
-            if count >= 184800:
+            if count >= 30000:
                 logger.info(f"*** Record {count} is {o['record']} ***")
             stream = o['stream']
             if stream not in schemas:
                 # Increment ingest_errors metric
                 ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                 raise Exception(f"A record for stream {stream} was encountered before a corresponding schema")
 
@@ -284,14 +284,15 @@
     Thread(target=start_background_loop, args=(event_loop,), daemon=True).start()
     asyncio.run_coroutine_threadsafe(process_batch(collection, record_batch, client), event_loop)
     return event_loop
 
 
 async def process_batch(collection: StandardCollection, record_batch: RecordBatch, client) -> None:
     while True:
+        logger.info("***** Entered process batch.....")
         await asyncio.sleep(record_batch.interval)
         timedelta = datetime.now(timezone.utc) - ensure_datetime(record_batch.last_executed_time)
         if timedelta.total_seconds() >= record_batch.min_time_gap:
             # if batch has records that need to be processed but haven't reached batch size then process them.
             try_upsert(collection, record_batch, client, force=True)
```

### Comparing `macrometa-target-collection-0.0.65/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.66/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.65
+Version: 0.0.66
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.65/pyproject.toml` & `macrometa-target-collection-0.0.66/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.65"
+version = "0.0.66"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

