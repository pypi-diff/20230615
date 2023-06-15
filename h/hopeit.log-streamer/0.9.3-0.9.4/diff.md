# Comparing `tmp/hopeit.log-streamer-0.9.3.tar.gz` & `tmp/hopeit.log-streamer-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hopeit.log-streamer-0.9.3.tar", last modified: Mon Jul 12 23:34:17 2021, max compression
+gzip compressed data, was "hopeit.log-streamer-0.9.4.tar", last modified: Wed Jul 14 00:51:58 2021, max compression
```

## Comparing `hopeit.log-streamer-0.9.3.tar` & `hopeit.log-streamer-0.9.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:17.642179 hopeit.log-streamer-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1983 2021-07-12 23:34:17.642179 hopeit.log-streamer-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      685 2021-07-12 23:27:48.000000 hopeit.log-streamer-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-12 23:34:17.642179 hopeit.log-streamer-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1943 2021-07-12 23:27:48.000000 hopeit.log-streamer-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:17.638179 hopeit.log-streamer-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:17.638179 hopeit.log-streamer-0.9.3/src/hopeit/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:17.642179 hopeit.log-streamer-0.9.3/src/hopeit/log_streamer/
--rw-r--r--   0 runner    (1001) docker     (121)     8804 2021-07-12 23:27:48.000000 hopeit.log-streamer-0.9.3/src/hopeit/log_streamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4454 2021-07-12 23:27:48.000000 hopeit.log-streamer-0.9.3/src/hopeit/log_streamer/log_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:17.642179 hopeit.log-streamer-0.9.3/src/hopeit.log_streamer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1983 2021-07-12 23:34:17.000000 hopeit.log-streamer-0.9.3/src/hopeit.log_streamer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      326 2021-07-12 23:34:17.000000 hopeit.log-streamer-0.9.3/src/hopeit.log_streamer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-12 23:34:17.000000 hopeit.log-streamer-0.9.3/src/hopeit.log_streamer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-07-12 23:34:17.000000 hopeit.log-streamer-0.9.3/src/hopeit.log_streamer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-07-12 23:34:17.000000 hopeit.log-streamer-0.9.3/src/hopeit.log_streamer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:58.892906 hopeit.log-streamer-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)     1983 2021-07-14 00:51:58.892906 hopeit.log-streamer-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      685 2021-07-14 00:45:26.000000 hopeit.log-streamer-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-14 00:51:58.892906 hopeit.log-streamer-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1943 2021-07-14 00:45:26.000000 hopeit.log-streamer-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:58.888906 hopeit.log-streamer-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:58.892906 hopeit.log-streamer-0.9.4/src/hopeit/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:58.892906 hopeit.log-streamer-0.9.4/src/hopeit/log_streamer/
+-rw-r--r--   0 runner    (1001) docker     (121)     8804 2021-07-14 00:45:26.000000 hopeit.log-streamer-0.9.4/src/hopeit/log_streamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4422 2021-07-14 00:45:26.000000 hopeit.log-streamer-0.9.4/src/hopeit/log_streamer/log_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:58.892906 hopeit.log-streamer-0.9.4/src/hopeit.log_streamer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1983 2021-07-14 00:51:58.000000 hopeit.log-streamer-0.9.4/src/hopeit.log_streamer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2021-07-14 00:51:58.000000 hopeit.log-streamer-0.9.4/src/hopeit.log_streamer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-14 00:51:58.000000 hopeit.log-streamer-0.9.4/src/hopeit.log_streamer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2021-07-14 00:51:58.000000 hopeit.log-streamer-0.9.4/src/hopeit.log_streamer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-07-14 00:51:58.000000 hopeit.log-streamer-0.9.4/src/hopeit.log_streamer.egg-info/top_level.txt
```

### Comparing `hopeit.log-streamer-0.9.3/PKG-INFO` & `hopeit.log-streamer-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopeit.log-streamer
-Version: 0.9.3
+Version: 0.9.4
 Summary: Hopeit Engine Log Streamer Plugin
 Home-page: https://github.com/hopeit-git/hopeit.engine
 Author: Leo Smerling and Pablo Canto
 Author-email: contact@hopeit.com.ar
 License: Apache 2
 Project-URL: CI: GitHub Actions, https://github.com/hopeit-git/hopeit.engine/actions?query=workflow
 Project-URL: Docs: RTD, https://hopeitengine.readthedocs.io/en/latest/
```

### Comparing `hopeit.log-streamer-0.9.3/README.md` & `hopeit.log-streamer-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `hopeit.log-streamer-0.9.3/setup.py` & `hopeit.log-streamer-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `hopeit.log-streamer-0.9.3/src/hopeit/log_streamer/__init__.py` & `hopeit.log-streamer-0.9.4/src/hopeit/log_streamer/__init__.py`

 * *Files identical despite different names*

### Comparing `hopeit.log-streamer-0.9.3/src/hopeit/log_streamer/log_reader.py` & `hopeit.log-streamer-0.9.4/src/hopeit/log_streamer/log_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     LogFileHandler, start_observer
 
 logger, extra = app_extra_logger()
 
 __steps__ = ['process_log_data']
 
 
-async def __service__(context: EventContext) -> Spawn[LogRawBatch]:  # pylint: disable=invalid-name
+async def __service__(context: EventContext) -> Spawn[LogRawBatch]:
     config = LogReaderConfig.from_dict(context.env['log_reader'])  # type: ignore
     event_handler = LogFileHandler(config, context)
     logger.info(context, "Starting LogFileHandler...", extra=extra(
         logs_path=config.logs_path,
         checkpoint_path=config.checkpoint_path
     ))
     observer = start_observer(event_handler, config.logs_path)
```

### Comparing `hopeit.log-streamer-0.9.3/src/hopeit.log_streamer.egg-info/PKG-INFO` & `hopeit.log-streamer-0.9.4/src/hopeit.log_streamer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopeit.log-streamer
-Version: 0.9.3
+Version: 0.9.4
 Summary: Hopeit Engine Log Streamer Plugin
 Home-page: https://github.com/hopeit-git/hopeit.engine
 Author: Leo Smerling and Pablo Canto
 Author-email: contact@hopeit.com.ar
 License: Apache 2
 Project-URL: CI: GitHub Actions, https://github.com/hopeit-git/hopeit.engine/actions?query=workflow
 Project-URL: Docs: RTD, https://hopeitengine.readthedocs.io/en/latest/
```

