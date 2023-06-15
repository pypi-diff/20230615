# Comparing `tmp/hopeit.engine-0.9.3.tar.gz` & `tmp/hopeit.engine-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hopeit.engine-0.9.3.tar", last modified: Mon Jul 12 23:34:11 2021, max compression
+gzip compressed data, was "hopeit.engine-0.9.4.tar", last modified: Wed Jul 14 00:51:52 2021, max compression
```

## Comparing `hopeit.engine-0.9.3.tar` & `hopeit.engine-0.9.4.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:11.118141 hopeit.engine-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)     4379 2021-07-12 23:34:11.118141 hopeit.engine-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2832 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-12 23:34:11.118141 hopeit.engine-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4576 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:11.110141 hopeit.engine-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:11.110141 hopeit.engine-0.9.3/src/hopeit/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:11.110141 hopeit.engine-0.9.3/src/hopeit/app/
--rw-r--r--   0 runner    (1001) docker     (121)      591 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10292 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/app/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     5556 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/app/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    15111 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/app/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     7506 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/app/context.py
--rw-r--r--   0 runner    (1001) docker     (121)      592 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/app/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     4077 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/app/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/app/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:11.110141 hopeit.engine-0.9.3/src/hopeit/cli/
--rw-r--r--   0 runner    (1001) docker     (121)      271 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4928 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/cli/openapi.py
--rw-r--r--   0 runner    (1001) docker     (121)     1281 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/cli/server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:11.114141 hopeit.engine-0.9.3/src/hopeit/dataobjects/
--rw-r--r--   0 runner    (1001) docker     (121)     7905 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/dataobjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      486 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/dataobjects/jsonify.py
--rw-r--r--   0 runner    (1001) docker     (121)     6836 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/dataobjects/payload.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:11.118141 hopeit.engine-0.9.3/src/hopeit/server/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25394 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/server/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4066 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/server/collector.py
--rw-r--r--   0 runner    (1001) docker     (121)     2317 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/server/compression.py
--rw-r--r--   0 runner    (1001) docker     (121)     9102 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/server/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    28243 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/server/engine.py
--rw-r--r--   0 runner    (1001) docker     (121)      871 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/server/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     6019 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/server/events.py
--rw-r--r--   0 runner    (1001) docker     (121)      904 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/server/imports.py
--rw-r--r--   0 runner    (1001) docker     (121)    11029 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/server/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     6002 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/server/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)      809 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/server/names.py
--rw-r--r--   0 runner    (1001) docker     (121)      158 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/server/runtime.py
--rw-r--r--   0 runner    (1001) docker     (121)     1988 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/server/serialization.py
--rw-r--r--   0 runner    (1001) docker     (121)    15364 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/server/steps.py
--rw-r--r--   0 runner    (1001) docker     (121)      945 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/server/version.py
--rw-r--r--   0 runner    (1001) docker     (121)    26608 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/server/web.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:11.118141 hopeit.engine-0.9.3/src/hopeit/streams/
--rw-r--r--   0 runner    (1001) docker     (121)     8689 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/streams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:11.118141 hopeit.engine-0.9.3/src/hopeit/testing/
--rw-r--r--   0 runner    (1001) docker     (121)      380 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10163 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/testing/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      703 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/testing/encryption.py
--rw-r--r--   0 runner    (1001) docker     (121)     2689 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/testing/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:11.118141 hopeit.engine-0.9.3/src/hopeit/toolkit/
--rw-r--r--   0 runner    (1001) docker     (121)      201 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7727 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/toolkit/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)      517 2021-07-12 23:27:48.000000 hopeit.engine-0.9.3/src/hopeit/toolkit/web.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:11.110141 hopeit.engine-0.9.3/src/hopeit.engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4379 2021-07-12 23:34:11.000000 hopeit.engine-0.9.3/src/hopeit.engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2021-07-12 23:34:11.000000 hopeit.engine-0.9.3/src/hopeit.engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-12 23:34:11.000000 hopeit.engine-0.9.3/src/hopeit.engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2021-07-12 23:34:11.000000 hopeit.engine-0.9.3/src/hopeit.engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      600 2021-07-12 23:34:11.000000 hopeit.engine-0.9.3/src/hopeit.engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-07-12 23:34:11.000000 hopeit.engine-0.9.3/src/hopeit.engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:52.740911 hopeit.engine-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)     4379 2021-07-14 00:51:52.740911 hopeit.engine-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2832 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-14 00:51:52.740911 hopeit.engine-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4576 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:52.732911 hopeit.engine-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:52.732911 hopeit.engine-0.9.4/src/hopeit/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:52.736911 hopeit.engine-0.9.4/src/hopeit/app/
+-rw-r--r--   0 runner    (1001) docker     (121)      591 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10292 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/app/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5556 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/app/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15111 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/app/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7506 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/app/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)      592 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/app/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4077 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/app/events.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1136 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/app/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:52.736911 hopeit.engine-0.9.4/src/hopeit/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4928 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/cli/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1281 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/cli/server.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:52.736911 hopeit.engine-0.9.4/src/hopeit/dataobjects/
+-rw-r--r--   0 runner    (1001) docker     (121)     7905 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/dataobjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      486 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/dataobjects/jsonify.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6836 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/dataobjects/payload.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:52.740911 hopeit.engine-0.9.4/src/hopeit/server/
+-rw-r--r--   0 runner    (1001) docker     (121)     1065 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25394 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4066 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/server/collector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2317 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/server/compression.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9102 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28243 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/server/engine.py
+-rw-r--r--   0 runner    (1001) docker     (121)      871 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/server/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6019 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/server/events.py
+-rw-r--r--   0 runner    (1001) docker     (121)      904 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/server/imports.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11029 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/server/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6002 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/server/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)      809 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/server/names.py
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/server/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1988 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/server/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15364 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/server/steps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      945 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/server/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26608 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/server/web.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:52.740911 hopeit.engine-0.9.4/src/hopeit/streams/
+-rw-r--r--   0 runner    (1001) docker     (121)     8689 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/streams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:52.740911 hopeit.engine-0.9.4/src/hopeit/testing/
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10163 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/testing/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/testing/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2689 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/testing/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:52.740911 hopeit.engine-0.9.4/src/hopeit/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7727 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/toolkit/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)      517 2021-07-14 00:45:26.000000 hopeit.engine-0.9.4/src/hopeit/toolkit/web.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:52.732911 hopeit.engine-0.9.4/src/hopeit.engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4379 2021-07-14 00:51:52.000000 hopeit.engine-0.9.4/src/hopeit.engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1370 2021-07-14 00:51:52.000000 hopeit.engine-0.9.4/src/hopeit.engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-14 00:51:52.000000 hopeit.engine-0.9.4/src/hopeit.engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2021-07-14 00:51:52.000000 hopeit.engine-0.9.4/src/hopeit.engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      600 2021-07-14 00:51:52.000000 hopeit.engine-0.9.4/src/hopeit.engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-07-14 00:51:52.000000 hopeit.engine-0.9.4/src/hopeit.engine.egg-info/top_level.txt
```

### Comparing `hopeit.engine-0.9.3/PKG-INFO` & `hopeit.engine-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopeit.engine
-Version: 0.9.3
+Version: 0.9.4
 Summary: Hopeit Engine: Microservices with Streams
 Home-page: https://github.com/hopeit-git/hopeit.engine
 Author: Leo Smerling and Pablo Canto
 Author-email: contact@hopeit.com.ar
 License: Apache 2
 Project-URL: CI: GitHub Actions, https://github.com/hopeit-git/hopeit.engine/actions?query=workflow
 Project-URL: Docs: RTD, https://hopeitengine.readthedocs.io/en/latest/
```

### Comparing `hopeit.engine-0.9.3/README.md` & `hopeit.engine-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/setup.py` & `hopeit.engine-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/app/__init__.py` & `hopeit.engine-0.9.4/src/hopeit/app/__init__.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/app/api.py` & `hopeit.engine-0.9.4/src/hopeit/app/api.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/app/client.py` & `hopeit.engine-0.9.4/src/hopeit/app/client.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/app/config.py` & `hopeit.engine-0.9.4/src/hopeit/app/config.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/app/context.py` & `hopeit.engine-0.9.4/src/hopeit/app/context.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/app/errors.py` & `hopeit.engine-0.9.4/src/hopeit/app/errors.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/app/events.py` & `hopeit.engine-0.9.4/src/hopeit/app/events.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/app/logger.py` & `hopeit.engine-0.9.4/src/hopeit/app/logger.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/cli/openapi.py` & `hopeit.engine-0.9.4/src/hopeit/cli/openapi.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/cli/server.py` & `hopeit.engine-0.9.4/src/hopeit/cli/server.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/dataobjects/__init__.py` & `hopeit.engine-0.9.4/src/hopeit/dataobjects/__init__.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/dataobjects/payload.py` & `hopeit.engine-0.9.4/src/hopeit/dataobjects/payload.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/server/__init__.py` & `hopeit.engine-0.9.4/src/hopeit/server/__init__.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/server/api.py` & `hopeit.engine-0.9.4/src/hopeit/server/api.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/server/collector.py` & `hopeit.engine-0.9.4/src/hopeit/server/collector.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/server/compression.py` & `hopeit.engine-0.9.4/src/hopeit/server/compression.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/server/config.py` & `hopeit.engine-0.9.4/src/hopeit/server/config.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/server/engine.py` & `hopeit.engine-0.9.4/src/hopeit/server/engine.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/server/errors.py` & `hopeit.engine-0.9.4/src/hopeit/server/errors.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/server/events.py` & `hopeit.engine-0.9.4/src/hopeit/server/events.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/server/imports.py` & `hopeit.engine-0.9.4/src/hopeit/server/imports.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/server/logger.py` & `hopeit.engine-0.9.4/src/hopeit/server/logger.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/server/metrics.py` & `hopeit.engine-0.9.4/src/hopeit/server/metrics.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/server/names.py` & `hopeit.engine-0.9.4/src/hopeit/server/names.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/server/serialization.py` & `hopeit.engine-0.9.4/src/hopeit/server/serialization.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/server/steps.py` & `hopeit.engine-0.9.4/src/hopeit/server/steps.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/server/version.py` & `hopeit.engine-0.9.4/src/hopeit/server/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 To ensure configuration files from example apps and plugins have same version as engine,
 environment variables `HOPEIT_ENGINE_VERSION` and `HOPEIT_APPS_API_VERSION` are set.
 """
 import os
 import sys
 
 ENGINE_NAME = "hopeit.engine"
-ENGINE_VERSION = "0.9.3"
+ENGINE_VERSION = "0.9.4"
 
 # Major.Minor version to be used in App versions and Api endpoints for Apps/Plugins
 APPS_API_VERSION = '.'.join(ENGINE_VERSION.split('.')[0:2])
 APPS_ROUTE_VERSION = APPS_API_VERSION.replace('.', 'x')
 
 os.environ['HOPEIT_ENGINE_VERSION'] = ENGINE_VERSION
 os.environ['HOPEIT_APPS_API_VERSION'] = APPS_API_VERSION
```

### Comparing `hopeit.engine-0.9.3/src/hopeit/server/web.py` & `hopeit.engine-0.9.4/src/hopeit/server/web.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/streams/__init__.py` & `hopeit.engine-0.9.4/src/hopeit/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/testing/apps.py` & `hopeit.engine-0.9.4/src/hopeit/testing/apps.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/testing/encryption.py` & `hopeit.engine-0.9.4/src/hopeit/testing/encryption.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/testing/hooks.py` & `hopeit.engine-0.9.4/src/hopeit/testing/hooks.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/toolkit/auth.py` & `hopeit.engine-0.9.4/src/hopeit/toolkit/auth.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit/toolkit/web.py` & `hopeit.engine-0.9.4/src/hopeit/toolkit/web.py`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit.engine.egg-info/PKG-INFO` & `hopeit.engine-0.9.4/src/hopeit.engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopeit.engine
-Version: 0.9.3
+Version: 0.9.4
 Summary: Hopeit Engine: Microservices with Streams
 Home-page: https://github.com/hopeit-git/hopeit.engine
 Author: Leo Smerling and Pablo Canto
 Author-email: contact@hopeit.com.ar
 License: Apache 2
 Project-URL: CI: GitHub Actions, https://github.com/hopeit-git/hopeit.engine/actions?query=workflow
 Project-URL: Docs: RTD, https://hopeitengine.readthedocs.io/en/latest/
```

### Comparing `hopeit.engine-0.9.3/src/hopeit.engine.egg-info/SOURCES.txt` & `hopeit.engine-0.9.4/src/hopeit.engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hopeit.engine-0.9.3/src/hopeit.engine.egg-info/requires.txt` & `hopeit.engine-0.9.4/src/hopeit.engine.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 deepdiff>=5.5.0
 typing-inspect>=0.7.1
 multidict>=5.1.0
 dataclasses-jsonschema[fast-validation]>=2.14.1
 fastjsonschema>=2.15.1
 
 [apps-client]
-hopeit.apps-client==0.9.3
+hopeit.apps-client==0.9.4
 
 [apps-visualizer]
-hopeit.apps-visualizer==0.9.3
+hopeit.apps-visualizer==0.9.4
 
 [cli]
 click>=8.0.1
 
 [config-manager]
-hopeit.config-manager==0.9.3
+hopeit.config-manager==0.9.4
 
 [fs-storage]
-hopeit.fs-storage==0.9.3
+hopeit.fs-storage==0.9.4
 
 [log-streamer]
-hopeit.log-streamer==0.9.3
+hopeit.log-streamer==0.9.4
 
 [redis-storage]
-hopeit.redis-storage==0.9.3
+hopeit.redis-storage==0.9.4
 
 [redis-streams]
-hopeit.redis-streams==0.9.3
+hopeit.redis-streams==0.9.4
 
 [web]
 aiohttp>=3.7.4.post0
 aiohttp-cors>=0.7.0
 aiohttp-swagger3<0.6,>=0.5.6
```

