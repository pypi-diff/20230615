# Comparing `tmp/ValiotWorker-5.3.4.tar.gz` & `tmp/ValiotWorker-5.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ValiotWorker-5.3.4.tar", last modified: Wed May 24 16:29:59 2023, max compression
+gzip compressed data, was "ValiotWorker-5.3.5.tar", last modified: Thu Jun 15 14:28:52 2023, max compression
```

## Comparing `ValiotWorker-5.3.4.tar` & `ValiotWorker-5.3.5.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-05-24 16:29:59.976430 ValiotWorker-5.3.4/
--rw-r--r--   0 baruc      (501) staff       (20)     1074 2021-04-26 22:17:35.000000 ValiotWorker-5.3.4/LICENCE
--rw-r--r--   0 baruc      (501) staff       (20)       37 2023-02-24 03:38:26.000000 ValiotWorker-5.3.4/MANIFEST.in
--rw-r--r--   0 baruc      (501) staff       (20)     2158 2023-05-24 16:29:59.976199 ValiotWorker-5.3.4/PKG-INFO
--rw-r--r--   0 baruc      (501) staff       (20)     1811 2021-04-26 22:17:35.000000 ValiotWorker-5.3.4/README.md
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-05-24 16:29:59.970623 ValiotWorker-5.3.4/ValiotWorker/
--rw-r--r--   0 baruc      (501) staff       (20)     3486 2023-04-19 23:58:36.000000 ValiotWorker-5.3.4/ValiotWorker/Logging.py
--rw-r--r--   0 baruc      (501) staff       (20)    13430 2021-12-23 22:44:57.000000 ValiotWorker-5.3.4/ValiotWorker/Notifications.py
--rw-r--r--   0 baruc      (501) staff       (20)      294 2023-03-27 19:36:21.000000 ValiotWorker-5.3.4/ValiotWorker/__init__.py
--rw-r--r--   0 baruc      (501) staff       (20)     3450 2023-05-24 13:52:21.000000 ValiotWorker-5.3.4/ValiotWorker/__main__.py
--rw-r--r--   0 baruc      (501) staff       (20)       22 2023-05-24 16:28:35.000000 ValiotWorker-5.3.4/ValiotWorker/__version__.py
--rw-r--r--   0 baruc      (501) staff       (20)      276 2023-02-21 21:58:52.000000 ValiotWorker-5.3.4/ValiotWorker/croniterHelpers.py
--rw-r--r--   0 baruc      (501) staff       (20)      218 2023-02-21 21:58:52.000000 ValiotWorker-5.3.4/ValiotWorker/dateHelpers.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-05-24 16:29:59.975151 ValiotWorker-5.3.4/ValiotWorker/healthCheckProbe/
--rw-r--r--   0 baruc      (501) staff       (20)       41 2023-02-24 03:33:56.000000 ValiotWorker-5.3.4/ValiotWorker/healthCheckProbe/__init__.py
--rw-r--r--   0 baruc      (501) staff       (20)      963 2023-03-07 23:36:56.000000 ValiotWorker-5.3.4/ValiotWorker/healthCheckProbe/__main__.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-05-24 16:29:59.975448 ValiotWorker-5.3.4/ValiotWorker/healthCheckProbe/modules/
--rw-r--r--   0 baruc      (501) staff       (20)     1593 2023-02-24 03:33:56.000000 ValiotWorker-5.3.4/ValiotWorker/healthCheckProbe/modules/http_server.py
--rw-r--r--   0 baruc      (501) staff       (20)     7019 2023-05-24 16:25:39.000000 ValiotWorker-5.3.4/ValiotWorker/mutations.py
--rw-r--r--   0 baruc      (501) staff       (20)     4394 2023-03-07 23:36:56.000000 ValiotWorker-5.3.4/ValiotWorker/queries.py
--rw-r--r--   0 baruc      (501) staff       (20)     5885 2023-05-24 13:52:21.000000 ValiotWorker-5.3.4/ValiotWorker/redis.py
--rw-r--r--   0 baruc      (501) staff       (20)     1244 2023-03-27 19:36:21.000000 ValiotWorker-5.3.4/ValiotWorker/subscriptions.py
--rw-r--r--   0 baruc      (501) staff       (20)      182 2021-12-23 22:44:57.000000 ValiotWorker-5.3.4/ValiotWorker/uploaders.py
--rw-r--r--   0 baruc      (501) staff       (20)    69826 2023-05-24 16:27:13.000000 ValiotWorker-5.3.4/ValiotWorker/worker.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-05-24 16:29:59.974637 ValiotWorker-5.3.4/ValiotWorker.egg-info/
--rw-r--r--   0 baruc      (501) staff       (20)     2158 2023-05-24 16:29:59.000000 ValiotWorker-5.3.4/ValiotWorker.egg-info/PKG-INFO
--rw-r--r--   0 baruc      (501) staff       (20)      791 2023-05-24 16:29:59.000000 ValiotWorker-5.3.4/ValiotWorker.egg-info/SOURCES.txt
--rw-r--r--   0 baruc      (501) staff       (20)        1 2023-05-24 16:29:59.000000 ValiotWorker-5.3.4/ValiotWorker.egg-info/dependency_links.txt
--rw-r--r--   0 baruc      (501) staff       (20)       60 2023-05-24 16:29:59.000000 ValiotWorker-5.3.4/ValiotWorker.egg-info/entry_points.txt
--rw-r--r--   0 baruc      (501) staff       (20)        1 2023-02-17 23:30:14.000000 ValiotWorker-5.3.4/ValiotWorker.egg-info/not-zip-safe
--rw-r--r--   0 baruc      (501) staff       (20)      237 2023-05-24 16:29:59.000000 ValiotWorker-5.3.4/ValiotWorker.egg-info/requires.txt
--rw-r--r--   0 baruc      (501) staff       (20)       13 2023-05-24 16:29:59.000000 ValiotWorker-5.3.4/ValiotWorker.egg-info/top_level.txt
--rw-r--r--   0 baruc      (501) staff       (20)       38 2023-05-24 16:29:59.976492 ValiotWorker-5.3.4/setup.cfg
--rw-r--r--   0 baruc      (501) staff       (20)     2289 2023-02-22 19:57:08.000000 ValiotWorker-5.3.4/setup.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-05-24 16:29:59.975793 ValiotWorker-5.3.4/tests/
--rw-r--r--   0 baruc      (501) staff       (20)      106 2023-05-24 13:52:21.000000 ValiotWorker-5.3.4/tests/test_dummy.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-15 14:28:52.398371 ValiotWorker-5.3.5/
+-rw-r--r--   0 baruc      (501) staff       (20)     1074 2021-04-26 22:17:35.000000 ValiotWorker-5.3.5/LICENCE
+-rw-r--r--   0 baruc      (501) staff       (20)       37 2023-02-24 03:38:26.000000 ValiotWorker-5.3.5/MANIFEST.in
+-rw-r--r--   0 baruc      (501) staff       (20)     2158 2023-06-15 14:28:52.398170 ValiotWorker-5.3.5/PKG-INFO
+-rw-r--r--   0 baruc      (501) staff       (20)     1811 2021-04-26 22:17:35.000000 ValiotWorker-5.3.5/README.md
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-15 14:28:52.394583 ValiotWorker-5.3.5/ValiotWorker/
+-rw-r--r--   0 baruc      (501) staff       (20)     3486 2023-04-19 23:58:36.000000 ValiotWorker-5.3.5/ValiotWorker/Logging.py
+-rw-r--r--   0 baruc      (501) staff       (20)    13430 2021-12-23 22:44:57.000000 ValiotWorker-5.3.5/ValiotWorker/Notifications.py
+-rw-r--r--   0 baruc      (501) staff       (20)      294 2023-06-15 04:30:39.000000 ValiotWorker-5.3.5/ValiotWorker/__init__.py
+-rw-r--r--   0 baruc      (501) staff       (20)     3450 2023-06-15 04:30:39.000000 ValiotWorker-5.3.5/ValiotWorker/__main__.py
+-rw-r--r--   0 baruc      (501) staff       (20)       22 2023-06-15 04:32:45.000000 ValiotWorker-5.3.5/ValiotWorker/__version__.py
+-rw-r--r--   0 baruc      (501) staff       (20)      276 2023-02-21 21:58:52.000000 ValiotWorker-5.3.5/ValiotWorker/croniterHelpers.py
+-rw-r--r--   0 baruc      (501) staff       (20)      218 2023-02-21 21:58:52.000000 ValiotWorker-5.3.5/ValiotWorker/dateHelpers.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-15 14:28:52.396978 ValiotWorker-5.3.5/ValiotWorker/healthCheckProbe/
+-rw-r--r--   0 baruc      (501) staff       (20)       41 2023-02-24 03:33:56.000000 ValiotWorker-5.3.5/ValiotWorker/healthCheckProbe/__init__.py
+-rw-r--r--   0 baruc      (501) staff       (20)      963 2023-03-07 23:36:56.000000 ValiotWorker-5.3.5/ValiotWorker/healthCheckProbe/__main__.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-15 14:28:52.397475 ValiotWorker-5.3.5/ValiotWorker/healthCheckProbe/modules/
+-rw-r--r--   0 baruc      (501) staff       (20)        0 2023-06-15 04:43:52.000000 ValiotWorker-5.3.5/ValiotWorker/healthCheckProbe/modules/__init__.py
+-rw-r--r--   0 baruc      (501) staff       (20)     1593 2023-02-24 03:33:56.000000 ValiotWorker-5.3.5/ValiotWorker/healthCheckProbe/modules/http_server.py
+-rw-r--r--   0 baruc      (501) staff       (20)     7019 2023-06-15 04:30:39.000000 ValiotWorker-5.3.5/ValiotWorker/mutations.py
+-rw-r--r--   0 baruc      (501) staff       (20)     4394 2023-03-07 23:36:56.000000 ValiotWorker-5.3.5/ValiotWorker/queries.py
+-rw-r--r--   0 baruc      (501) staff       (20)     5885 2023-06-15 04:30:39.000000 ValiotWorker-5.3.5/ValiotWorker/redis.py
+-rw-r--r--   0 baruc      (501) staff       (20)     1244 2023-06-15 04:30:39.000000 ValiotWorker-5.3.5/ValiotWorker/subscriptions.py
+-rw-r--r--   0 baruc      (501) staff       (20)      182 2021-12-23 22:44:57.000000 ValiotWorker-5.3.5/ValiotWorker/uploaders.py
+-rw-r--r--   0 baruc      (501) staff       (20)    69826 2023-06-15 04:30:39.000000 ValiotWorker-5.3.5/ValiotWorker/worker.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-15 14:28:52.396473 ValiotWorker-5.3.5/ValiotWorker.egg-info/
+-rw-r--r--   0 baruc      (501) staff       (20)     2158 2023-06-15 14:28:52.000000 ValiotWorker-5.3.5/ValiotWorker.egg-info/PKG-INFO
+-rw-r--r--   0 baruc      (501) staff       (20)      841 2023-06-15 14:28:52.000000 ValiotWorker-5.3.5/ValiotWorker.egg-info/SOURCES.txt
+-rw-r--r--   0 baruc      (501) staff       (20)        1 2023-06-15 14:28:52.000000 ValiotWorker-5.3.5/ValiotWorker.egg-info/dependency_links.txt
+-rw-r--r--   0 baruc      (501) staff       (20)       60 2023-06-15 14:28:52.000000 ValiotWorker-5.3.5/ValiotWorker.egg-info/entry_points.txt
+-rw-r--r--   0 baruc      (501) staff       (20)        1 2023-02-17 23:30:14.000000 ValiotWorker-5.3.5/ValiotWorker.egg-info/not-zip-safe
+-rw-r--r--   0 baruc      (501) staff       (20)      233 2023-06-15 14:28:52.000000 ValiotWorker-5.3.5/ValiotWorker.egg-info/requires.txt
+-rw-r--r--   0 baruc      (501) staff       (20)       13 2023-06-15 14:28:52.000000 ValiotWorker-5.3.5/ValiotWorker.egg-info/top_level.txt
+-rw-r--r--   0 baruc      (501) staff       (20)       38 2023-06-15 14:28:52.398425 ValiotWorker-5.3.5/setup.cfg
+-rw-r--r--   0 baruc      (501) staff       (20)     2607 2023-06-15 04:31:00.000000 ValiotWorker-5.3.5/setup.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-06-15 14:28:52.397805 ValiotWorker-5.3.5/tests/
+-rw-r--r--   0 baruc      (501) staff       (20)      106 2023-06-15 03:50:01.000000 ValiotWorker-5.3.5/tests/test_dummy.py
```

### Comparing `ValiotWorker-5.3.4/LICENCE` & `ValiotWorker-5.3.5/LICENCE`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.4/PKG-INFO` & `ValiotWorker-5.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ValiotWorker
-Version: 5.3.4
+Version: 5.3.5
 Summary: Enables running Python functions as standalone jobs based on interaction with valiot-jobs API
 Home-page: https://github.com/valiot/python-gql-worker
 Author: Valiot
 Author-email: hiring@valiot.io
 Keywords: ValiotWorker
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `ValiotWorker-5.3.4/README.md` & `ValiotWorker-5.3.5/README.md`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.4/ValiotWorker/Logging.py` & `ValiotWorker-5.3.5/ValiotWorker/Logging.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.4/ValiotWorker/Notifications.py` & `ValiotWorker-5.3.5/ValiotWorker/Notifications.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.4/ValiotWorker/__main__.py` & `ValiotWorker-5.3.5/ValiotWorker/__main__.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.4/ValiotWorker/healthCheckProbe/__main__.py` & `ValiotWorker-5.3.5/ValiotWorker/healthCheckProbe/__main__.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.4/ValiotWorker/healthCheckProbe/modules/http_server.py` & `ValiotWorker-5.3.5/ValiotWorker/healthCheckProbe/modules/http_server.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.4/ValiotWorker/mutations.py` & `ValiotWorker-5.3.5/ValiotWorker/mutations.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.4/ValiotWorker/queries.py` & `ValiotWorker-5.3.5/ValiotWorker/queries.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.4/ValiotWorker/redis.py` & `ValiotWorker-5.3.5/ValiotWorker/redis.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.4/ValiotWorker/subscriptions.py` & `ValiotWorker-5.3.5/ValiotWorker/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.4/ValiotWorker/worker.py` & `ValiotWorker-5.3.5/ValiotWorker/worker.py`

 * *Files identical despite different names*

### Comparing `ValiotWorker-5.3.4/ValiotWorker.egg-info/PKG-INFO` & `ValiotWorker-5.3.5/ValiotWorker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ValiotWorker
-Version: 5.3.4
+Version: 5.3.5
 Summary: Enables running Python functions as standalone jobs based on interaction with valiot-jobs API
 Home-page: https://github.com/valiot/python-gql-worker
 Author: Valiot
 Author-email: hiring@valiot.io
 Keywords: ValiotWorker
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `ValiotWorker-5.3.4/ValiotWorker.egg-info/SOURCES.txt` & `ValiotWorker-5.3.5/ValiotWorker.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -20,9 +20,10 @@
 ValiotWorker.egg-info/dependency_links.txt
 ValiotWorker.egg-info/entry_points.txt
 ValiotWorker.egg-info/not-zip-safe
 ValiotWorker.egg-info/requires.txt
 ValiotWorker.egg-info/top_level.txt
 ValiotWorker/healthCheckProbe/__init__.py
 ValiotWorker/healthCheckProbe/__main__.py
+ValiotWorker/healthCheckProbe/modules/__init__.py
 ValiotWorker/healthCheckProbe/modules/http_server.py
 tests/test_dummy.py
```

### Comparing `ValiotWorker-5.3.4/setup.py` & `ValiotWorker-5.3.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,26 +21,25 @@
             "Unable to find version string in %s." % (version_file,))
 
 
 __version__ = get_package_version("ValiotWorker/__version__.py")
 
 requirements = [
     # TODO: put package requirements here
-    'colorama>=0.4, <0.5',
+    'colorama>=0.4, <0.5',  # Must be aligned with the version at gstorm
     'croniter>=1.3, <2.0',
-    'pydash>=5.0, <6.0',
-    'pygqlc>=3.0.1, <4.0.0',
-    'python-dateutil>=2.8.2, <3.0',
-    'pytz==2022.2.1',
-    'redis>=4.3.4, <5.0',
+    'pydash>=5.0, <7.0',  # Must be aligned with the version at gstorm
+    'pygqlc>=3.0, <4.0',  # Must be aligned with the version at gstorm
+    'python-dateutil>=2.8, <3.0',  # Must be aligned with the version at gstorm
+    'pytz>=2022.2, <2022.8',  # Must be aligned with the version at gstorm
+    'redis>=4.3, <5.0',
     'singleton-decorator>=1.0, <2.0',
-    'termcolor>=2.0.1, <3.0',
-    'tzlocal>=4.2, <5.0',
+    'termcolor>=2.0, <3.0',  # Must be aligned with the version at gstorm
+    'tzlocal>=4.2, <5.0',  # Must be aligned with the version at gstorm
     'velebit-useful-logs>=1.0, <2.0'
-
 ]
 
 setup_requirements = [
     # TODO(alanbato): put setup requirements (distutils extensions, etc.) here
     'twine',
 ]
```

