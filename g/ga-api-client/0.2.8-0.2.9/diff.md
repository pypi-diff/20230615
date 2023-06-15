# Comparing `tmp/ga-api-client-0.2.8.tar.gz` & `tmp/ga-api-client-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ga-api-client-0.2.8.tar", last modified: Wed Nov 16 06:53:53 2022, max compression
+gzip compressed data, was "ga-api-client-0.2.9.tar", last modified: Wed Jan 18 02:54:18 2023, max compression
```

## Comparing `ga-api-client-0.2.8.tar` & `ga-api-client-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 allenliao  (1000) allenliao  (1000)        0 2022-11-16 06:53:53.565200 ga-api-client-0.2.8/
--rw-r--r--   0 allenliao  (1000) allenliao  (1000)     1073 2022-10-07 09:35:51.000000 ga-api-client-0.2.8/LICENSE
--rw-r--r--   0 allenliao  (1000) allenliao  (1000)      955 2022-11-16 06:53:53.565200 ga-api-client-0.2.8/PKG-INFO
--rw-r--r--   0 allenliao  (1000) allenliao  (1000)       11 2022-09-07 06:40:46.000000 ga-api-client-0.2.8/README
-drwxr-xr-x   0 allenliao  (1000) allenliao  (1000)        0 2022-11-16 06:53:53.561200 ga-api-client-0.2.8/ga_api/
--rw-r--r--   0 allenliao  (1000) allenliao  (1000)      149 2022-10-07 09:35:51.000000 ga-api-client-0.2.8/ga_api/__init__.py
--rw-r--r--   0 allenliao  (1000) allenliao  (1000)    12131 2022-10-07 09:35:51.000000 ga-api-client-0.2.8/ga_api/field_tree.py
--rw-r--r--   0 allenliao  (1000) allenliao  (1000)    32156 2022-11-16 06:49:26.000000 ga-api-client-0.2.8/ga_api/ga_api_client.py
--rw-r--r--   0 allenliao  (1000) allenliao  (1000)     1695 2022-10-07 09:35:51.000000 ga-api-client-0.2.8/ga_api/hyper_log_log.py
-drwxr-xr-x   0 allenliao  (1000) allenliao  (1000)        0 2022-11-16 06:53:53.565200 ga-api-client-0.2.8/ga_api_client.egg-info/
--rw-r--r--   0 allenliao  (1000) allenliao  (1000)      955 2022-11-16 06:53:53.000000 ga-api-client-0.2.8/ga_api_client.egg-info/PKG-INFO
--rw-r--r--   0 allenliao  (1000) allenliao  (1000)      320 2022-11-16 06:53:53.000000 ga-api-client-0.2.8/ga_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 allenliao  (1000) allenliao  (1000)        1 2022-11-16 06:53:53.000000 ga-api-client-0.2.8/ga_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 allenliao  (1000) allenliao  (1000)       44 2022-11-16 06:53:53.000000 ga-api-client-0.2.8/ga_api_client.egg-info/requires.txt
--rw-r--r--   0 allenliao  (1000) allenliao  (1000)        7 2022-11-16 06:53:53.000000 ga-api-client-0.2.8/ga_api_client.egg-info/top_level.txt
--rw-r--r--   0 allenliao  (1000) allenliao  (1000)       84 2022-10-07 09:35:51.000000 ga-api-client-0.2.8/pyproject.toml
--rw-r--r--   0 allenliao  (1000) allenliao  (1000)      463 2022-11-16 06:53:53.565200 ga-api-client-0.2.8/setup.cfg
--rw-r--r--   0 allenliao  (1000) allenliao  (1000)       67 2022-10-07 09:38:32.000000 ga-api-client-0.2.8/setup.py
+drwxr-xr-x   0 allen     (1000) allen     (1000)        0 2023-01-18 02:54:18.660150 ga-api-client-0.2.9/
+-rw-r--r--   0 allen     (1000) allen     (1000)     1073 2022-12-20 01:26:56.000000 ga-api-client-0.2.9/LICENSE
+-rw-r--r--   0 allen     (1000) allen     (1000)      955 2023-01-18 02:54:18.660150 ga-api-client-0.2.9/PKG-INFO
+-rw-r--r--   0 allen     (1000) allen     (1000)      666 2022-12-20 01:26:56.000000 ga-api-client-0.2.9/README.md
+drwxr-xr-x   0 allen     (1000) allen     (1000)        0 2023-01-18 02:54:18.656150 ga-api-client-0.2.9/ga_api/
+-rw-r--r--   0 allen     (1000) allen     (1000)      149 2022-12-20 01:26:56.000000 ga-api-client-0.2.9/ga_api/__init__.py
+-rw-r--r--   0 allen     (1000) allen     (1000)    12131 2022-12-20 01:26:56.000000 ga-api-client-0.2.9/ga_api/field_tree.py
+-rw-r--r--   0 allen     (1000) allen     (1000)    32156 2022-12-20 01:26:56.000000 ga-api-client-0.2.9/ga_api/ga_api_client.py
+-rw-r--r--   0 allen     (1000) allen     (1000)     1695 2022-12-20 01:26:56.000000 ga-api-client-0.2.9/ga_api/hyper_log_log.py
+drwxr-xr-x   0 allen     (1000) allen     (1000)        0 2023-01-18 02:54:18.660150 ga-api-client-0.2.9/ga_api_client.egg-info/
+-rw-r--r--   0 allen     (1000) allen     (1000)      955 2023-01-18 02:54:18.000000 ga-api-client-0.2.9/ga_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 allen     (1000) allen     (1000)      323 2023-01-18 02:54:18.000000 ga-api-client-0.2.9/ga_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 allen     (1000) allen     (1000)        1 2023-01-18 02:54:18.000000 ga-api-client-0.2.9/ga_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 allen     (1000) allen     (1000)       44 2023-01-18 02:54:18.000000 ga-api-client-0.2.9/ga_api_client.egg-info/requires.txt
+-rw-r--r--   0 allen     (1000) allen     (1000)        7 2023-01-18 02:54:18.000000 ga-api-client-0.2.9/ga_api_client.egg-info/top_level.txt
+-rw-r--r--   0 allen     (1000) allen     (1000)       84 2022-12-20 01:26:56.000000 ga-api-client-0.2.9/pyproject.toml
+-rw-r--r--   0 allen     (1000) allen     (1000)      463 2023-01-18 02:54:18.660150 ga-api-client-0.2.9/setup.cfg
+-rw-r--r--   0 allen     (1000) allen     (1000)       67 2022-12-20 01:26:56.000000 ga-api-client-0.2.9/setup.py
```

### Comparing `ga-api-client-0.2.8/LICENSE` & `ga-api-client-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ga-api-client-0.2.8/PKG-INFO` & `ga-api-client-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga-api-client
-Version: 0.2.8
+Version: 0.2.9
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ga-api-client-0.2.8/ga_api/field_tree.py` & `ga-api-client-0.2.9/ga_api/field_tree.py`

 * *Files identical despite different names*

### Comparing `ga-api-client-0.2.8/ga_api/ga_api_client.py` & `ga-api-client-0.2.9/ga_api/ga_api_client.py`

 * *Files identical despite different names*

### Comparing `ga-api-client-0.2.8/ga_api/hyper_log_log.py` & `ga-api-client-0.2.9/ga_api/hyper_log_log.py`

 * *Files identical despite different names*

### Comparing `ga-api-client-0.2.8/ga_api_client.egg-info/PKG-INFO` & `ga-api-client-0.2.9/ga_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga-api-client
-Version: 0.2.8
+Version: 0.2.9
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

