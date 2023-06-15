# Comparing `tmp/hopeit.redis-streams-0.9.3.tar.gz` & `tmp/hopeit.redis-streams-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hopeit.redis-streams-0.9.3.tar", last modified: Mon Jul 12 23:34:12 2021, max compression
+gzip compressed data, was "hopeit.redis-streams-0.9.4.tar", last modified: Wed Jul 14 00:51:54 2021, max compression
```

## Comparing `hopeit.redis-streams-0.9.3.tar` & `hopeit.redis-streams-0.9.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:12.522150 hopeit.redis-streams-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1541 2021-07-12 23:34:12.522150 hopeit.redis-streams-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      241 2021-07-12 23:27:48.000000 hopeit.redis-streams-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-12 23:34:12.522150 hopeit.redis-streams-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1938 2021-07-12 23:27:48.000000 hopeit.redis-streams-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:12.522150 hopeit.redis-streams-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:12.522150 hopeit.redis-streams-0.9.3/src/hopeit/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:12.522150 hopeit.redis-streams-0.9.3/src/hopeit/redis_streams/
--rw-r--r--   0 runner    (1001) docker     (121)    12477 2021-07-12 23:27:48.000000 hopeit.redis-streams-0.9.3/src/hopeit/redis_streams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:12.522150 hopeit.redis-streams-0.9.3/src/hopeit.redis_streams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1541 2021-07-12 23:34:12.000000 hopeit.redis-streams-0.9.3/src/hopeit.redis_streams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-07-12 23:34:12.000000 hopeit.redis-streams-0.9.3/src/hopeit.redis_streams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-12 23:34:12.000000 hopeit.redis-streams-0.9.3/src/hopeit.redis_streams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-07-12 23:34:12.000000 hopeit.redis-streams-0.9.3/src/hopeit.redis_streams.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-07-12 23:34:12.000000 hopeit.redis-streams-0.9.3/src/hopeit.redis_streams.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:54.072910 hopeit.redis-streams-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)     1541 2021-07-14 00:51:54.072910 hopeit.redis-streams-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2021-07-14 00:45:26.000000 hopeit.redis-streams-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-14 00:51:54.072910 hopeit.redis-streams-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1938 2021-07-14 00:45:26.000000 hopeit.redis-streams-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:54.072910 hopeit.redis-streams-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:54.072910 hopeit.redis-streams-0.9.4/src/hopeit/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:54.072910 hopeit.redis-streams-0.9.4/src/hopeit/redis_streams/
+-rw-r--r--   0 runner    (1001) docker     (121)    12477 2021-07-14 00:45:26.000000 hopeit.redis-streams-0.9.4/src/hopeit/redis_streams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:54.072910 hopeit.redis-streams-0.9.4/src/hopeit.redis_streams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1541 2021-07-14 00:51:54.000000 hopeit.redis-streams-0.9.4/src/hopeit.redis_streams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2021-07-14 00:51:54.000000 hopeit.redis-streams-0.9.4/src/hopeit.redis_streams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-14 00:51:54.000000 hopeit.redis-streams-0.9.4/src/hopeit.redis_streams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-07-14 00:51:54.000000 hopeit.redis-streams-0.9.4/src/hopeit.redis_streams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-07-14 00:51:54.000000 hopeit.redis-streams-0.9.4/src/hopeit.redis_streams.egg-info/top_level.txt
```

### Comparing `hopeit.redis-streams-0.9.3/PKG-INFO` & `hopeit.redis-streams-0.9.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopeit.redis-streams
-Version: 0.9.3
+Version: 0.9.4
 Summary: Hopeit Engine Redis Streams Plugin
 Home-page: https://github.com/hopeit-git/hopeit.engine
 Author: Leo Smerling and Pablo Canto
 Author-email: contact@hopeit.com.ar
 License: Apache 2
 Project-URL: CI: GitHub Actions, https://github.com/hopeit-git/hopeit.engine/actions?query=workflow
 Project-URL: Docs: RTD, https://hopeitengine.readthedocs.io/en/latest/
```

### Comparing `hopeit.redis-streams-0.9.3/setup.py` & `hopeit.redis-streams-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `hopeit.redis-streams-0.9.3/src/hopeit/redis_streams/__init__.py` & `hopeit.redis-streams-0.9.4/src/hopeit/redis_streams/__init__.py`

 * *Files identical despite different names*

### Comparing `hopeit.redis-streams-0.9.3/src/hopeit.redis_streams.egg-info/PKG-INFO` & `hopeit.redis-streams-0.9.4/src/hopeit.redis_streams.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopeit.redis-streams
-Version: 0.9.3
+Version: 0.9.4
 Summary: Hopeit Engine Redis Streams Plugin
 Home-page: https://github.com/hopeit-git/hopeit.engine
 Author: Leo Smerling and Pablo Canto
 Author-email: contact@hopeit.com.ar
 License: Apache 2
 Project-URL: CI: GitHub Actions, https://github.com/hopeit-git/hopeit.engine/actions?query=workflow
 Project-URL: Docs: RTD, https://hopeitengine.readthedocs.io/en/latest/
```

