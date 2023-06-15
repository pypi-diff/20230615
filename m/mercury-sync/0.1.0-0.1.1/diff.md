# Comparing `tmp/mercury-sync-0.1.0.tar.gz` & `tmp/mercury-sync-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-sync-0.1.0.tar", last modified: Thu Jun 15 05:45:46 2023, max compression
+gzip compressed data, was "mercury-sync-0.1.1.tar", last modified: Thu Jun 15 05:48:53 2023, max compression
```

## Comparing `mercury-sync-0.1.0.tar` & `mercury-sync-0.1.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:46.768195 mercury-sync-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 05:45:46.768195 mercury-sync-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:46.764195 mercury-sync-0.1.0/mercury_sync/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:46.764195 mercury-sync-0.1.0/mercury_sync/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:46.764195 mercury-sync-0.1.0/mercury_sync/connection/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/connection/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:46.768195 mercury-sync-0.1.0/mercury_sync/connection/tcp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/connection/tcp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:46.768195 mercury-sync-0.1.0/mercury_sync/connection/udp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/connection/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/connection/udp/mercury_sync_udp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:46.768195 mercury-sync-0.1.0/mercury_sync/connection/udp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/connection/udp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:46.768195 mercury-sync-0.1.0/mercury_sync/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/hooks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/hooks/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/hooks/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:46.768195 mercury-sync-0.1.0/mercury_sync/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/models/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:46.768195 mercury-sync-0.1.0/mercury_sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/service/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/service/service_set.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/service/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/service/test_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:46.768195 mercury-sync-0.1.0/mercury_sync/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/snowflake/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/snowflake/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/mercury_sync/snowflake/snowflake_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:45:46.764195 mercury-sync-0.1.0/mercury_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 05:45:46.000000 mercury-sync-0.1.0/mercury_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-15 05:45:46.000000 mercury-sync-0.1.0/mercury_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 05:45:46.000000 mercury-sync-0.1.0/mercury_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 05:45:46.000000 mercury-sync-0.1.0/mercury_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 05:45:46.768195 mercury-sync-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-15 05:45:42.000000 mercury-sync-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:48:53.336430 mercury-sync-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 05:48:53.336430 mercury-sync-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:48:53.332430 mercury-sync-0.1.1/mercury_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:48:53.332430 mercury-sync-0.1.1/mercury_sync/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:48:53.332430 mercury-sync-0.1.1/mercury_sync/connection/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/connection/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:48:53.332430 mercury-sync-0.1.1/mercury_sync/connection/tcp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/connection/tcp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:48:53.332430 mercury-sync-0.1.1/mercury_sync/connection/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/connection/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/connection/udp/mercury_sync_udp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:48:53.332430 mercury-sync-0.1.1/mercury_sync/connection/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/connection/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:48:53.332430 mercury-sync-0.1.1/mercury_sync/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/hooks/client_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/hooks/server_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/hooks/stream_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:48:53.332430 mercury-sync-0.1.1/mercury_sync/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/models/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:48:53.336430 mercury-sync-0.1.1/mercury_sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/service/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/service/service_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/service/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/service/test_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:48:53.336430 mercury-sync-0.1.1/mercury_sync/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/snowflake/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/snowflake/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/mercury_sync/snowflake/snowflake_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:48:53.332430 mercury-sync-0.1.1/mercury_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 05:48:53.000000 mercury-sync-0.1.1/mercury_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-15 05:48:53.000000 mercury-sync-0.1.1/mercury_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 05:48:53.000000 mercury-sync-0.1.1/mercury_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 05:48:53.000000 mercury-sync-0.1.1/mercury_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 05:48:53.336430 mercury-sync-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-15 05:48:49.000000 mercury-sync-0.1.1/setup.py
```

### Comparing `mercury-sync-0.1.0/LICENSE` & `mercury-sync-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.0/PKG-INFO` & `mercury-sync-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.1.0
+Version: 0.1.1
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.1.0/README.md` & `mercury-sync-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.0/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py` & `mercury-sync-0.1.1/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py` & `mercury-sync-0.1.1/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py` & `mercury-sync-0.1.1/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.0/mercury_sync/connection/udp/mercury_sync_udp_connection.py` & `mercury-sync-0.1.1/mercury_sync/connection/udp/mercury_sync_udp_connection.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.0/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py` & `mercury-sync-0.1.1/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.0/mercury_sync/hooks/client.py` & `mercury-sync-0.1.1/mercury_sync/hooks/client_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.0/mercury_sync/hooks/stream.py` & `mercury-sync-0.1.1/mercury_sync/hooks/stream_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.0/mercury_sync/service/service.py` & `mercury-sync-0.1.1/mercury_sync/service/service.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.0/mercury_sync/service/service_set.py` & `mercury-sync-0.1.1/mercury_sync/service/service_set.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.0/mercury_sync/snowflake/snowflake.py` & `mercury-sync-0.1.1/mercury_sync/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.0/mercury_sync/snowflake/snowflake_generator.py` & `mercury-sync-0.1.1/mercury_sync/snowflake/snowflake_generator.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.0/mercury_sync.egg-info/PKG-INFO` & `mercury-sync-0.1.1/mercury_sync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.1.0
+Version: 0.1.1
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.1.0/mercury_sync.egg-info/SOURCES.txt` & `mercury-sync-0.1.1/mercury_sync.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
 mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
 mercury_sync/connection/udp/__init__.py
 mercury_sync/connection/udp/mercury_sync_udp_connection.py
 mercury_sync/connection/udp/protocols/__init__.py
 mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
 mercury_sync/hooks/__init__.py
-mercury_sync/hooks/client.py
-mercury_sync/hooks/server.py
-mercury_sync/hooks/stream.py
+mercury_sync/hooks/client_hook.py
+mercury_sync/hooks/server_hook.py
+mercury_sync/hooks/stream_hook.py
 mercury_sync/models/__init__.py
 mercury_sync/models/message.py
 mercury_sync/service/__init__.py
 mercury_sync/service/service.py
 mercury_sync/service/service_set.py
 mercury_sync/service/test.py
 mercury_sync/service/test_message.py
```

### Comparing `mercury-sync-0.1.0/setup.py` & `mercury-sync-0.1.1/setup.py`

 * *Files identical despite different names*

