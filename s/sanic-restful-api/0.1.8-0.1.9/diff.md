# Comparing `tmp/sanic-restful-api-0.1.8.tar.gz` & `tmp/sanic-restful-api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanic-restful-api-0.1.8.tar", last modified: Fri Apr 28 04:24:51 2023, max compression
+gzip compressed data, was "sanic-restful-api-0.1.9.tar", last modified: Thu Jun 15 08:44:53 2023, max compression
```

## Comparing `sanic-restful-api-0.1.8.tar` & `sanic-restful-api-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 linzhiming   (502) staff       (20)        0 2023-04-28 04:24:51.850692 sanic-restful-api-0.1.8/
--rw-r--r--   0 linzhiming   (502) staff       (20)     1071 2022-11-22 07:22:12.000000 sanic-restful-api-0.1.8/LICENSE
--rw-r--r--   0 linzhiming   (502) staff       (20)     2414 2023-04-28 04:24:51.850772 sanic-restful-api-0.1.8/PKG-INFO
--rw-r--r--   0 linzhiming   (502) staff       (20)     1958 2022-11-22 07:22:12.000000 sanic-restful-api-0.1.8/README.md
-drwxr-xr-x   0 linzhiming   (502) staff       (20)        0 2023-04-28 04:24:51.845428 sanic-restful-api-0.1.8/sanic_restful_api/
--rw-r--r--   0 linzhiming   (502) staff       (20)    16345 2023-03-29 00:56:02.000000 sanic-restful-api-0.1.8/sanic_restful_api/__init__.py
--rw-r--r--   0 linzhiming   (502) staff       (20)       45 2023-04-28 04:19:27.000000 sanic-restful-api-0.1.8/sanic_restful_api/__version__.py
--rw-r--r--   0 linzhiming   (502) staff       (20)    11785 2022-11-22 07:22:12.000000 sanic-restful-api-0.1.8/sanic_restful_api/fields.py
--rw-r--r--   0 linzhiming   (502) staff       (20)     9104 2022-11-22 07:22:12.000000 sanic-restful-api-0.1.8/sanic_restful_api/inputs.py
-drwxr-xr-x   0 linzhiming   (502) staff       (20)        0 2023-04-28 04:24:51.849971 sanic-restful-api-0.1.8/sanic_restful_api/representations/
--rw-r--r--   0 linzhiming   (502) staff       (20)        0 2022-11-22 07:22:12.000000 sanic-restful-api-0.1.8/sanic_restful_api/representations/__init__.py
--rw-r--r--   0 linzhiming   (502) staff       (20)      334 2023-04-14 11:23:58.000000 sanic-restful-api-0.1.8/sanic_restful_api/representations/json.py
--rw-r--r--   0 linzhiming   (502) staff       (20)    14413 2023-04-28 04:19:03.000000 sanic-restful-api-0.1.8/sanic_restful_api/reqparse.py
-drwxr-xr-x   0 linzhiming   (502) staff       (20)        0 2023-04-28 04:24:51.850511 sanic-restful-api-0.1.8/sanic_restful_api/utils/
--rw-r--r--   0 linzhiming   (502) staff       (20)     1355 2022-11-22 07:22:12.000000 sanic-restful-api-0.1.8/sanic_restful_api/utils/__init__.py
--rw-r--r--   0 linzhiming   (502) staff       (20)      746 2022-11-22 07:22:12.000000 sanic-restful-api-0.1.8/sanic_restful_api/utils/accept_mimetypes.py
--rw-r--r--   0 linzhiming   (502) staff       (20)      996 2022-11-22 07:22:12.000000 sanic-restful-api-0.1.8/sanic_restful_api/utils/crypto.py
-drwxr-xr-x   0 linzhiming   (502) staff       (20)        0 2023-04-28 04:24:51.849771 sanic-restful-api-0.1.8/sanic_restful_api.egg-info/
--rw-r--r--   0 linzhiming   (502) staff       (20)     2414 2023-04-28 04:24:51.000000 sanic-restful-api-0.1.8/sanic_restful_api.egg-info/PKG-INFO
--rw-r--r--   0 linzhiming   (502) staff       (20)      631 2023-04-28 04:24:51.000000 sanic-restful-api-0.1.8/sanic_restful_api.egg-info/SOURCES.txt
--rw-r--r--   0 linzhiming   (502) staff       (20)        1 2023-04-28 04:24:51.000000 sanic-restful-api-0.1.8/sanic_restful_api.egg-info/dependency_links.txt
--rw-r--r--   0 linzhiming   (502) staff       (20)        1 2022-11-22 08:16:58.000000 sanic-restful-api-0.1.8/sanic_restful_api.egg-info/not-zip-safe
--rw-r--r--   0 linzhiming   (502) staff       (20)       71 2023-04-28 04:24:51.000000 sanic-restful-api-0.1.8/sanic_restful_api.egg-info/requires.txt
--rw-r--r--   0 linzhiming   (502) staff       (20)       18 2023-04-28 04:24:51.000000 sanic-restful-api-0.1.8/sanic_restful_api.egg-info/top_level.txt
--rw-r--r--   0 linzhiming   (502) staff       (20)       70 2023-04-28 04:24:51.851174 sanic-restful-api-0.1.8/setup.cfg
--rwxr-xr-x   0 linzhiming   (502) staff       (20)     1225 2023-04-28 04:24:41.000000 sanic-restful-api-0.1.8/setup.py
+drwxr-xr-x   0 linzhiming   (502) staff       (20)        0 2023-06-15 08:44:53.469032 sanic-restful-api-0.1.9/
+-rw-r--r--   0 linzhiming   (502) staff       (20)     1071 2022-11-22 07:22:12.000000 sanic-restful-api-0.1.9/LICENSE
+-rw-r--r--   0 linzhiming   (502) staff       (20)     2414 2023-06-15 08:44:53.469104 sanic-restful-api-0.1.9/PKG-INFO
+-rw-r--r--   0 linzhiming   (502) staff       (20)     1958 2022-11-22 07:22:12.000000 sanic-restful-api-0.1.9/README.md
+drwxr-xr-x   0 linzhiming   (502) staff       (20)        0 2023-06-15 08:44:53.464801 sanic-restful-api-0.1.9/sanic_restful_api/
+-rw-r--r--   0 linzhiming   (502) staff       (20)    16345 2023-03-29 00:56:02.000000 sanic-restful-api-0.1.9/sanic_restful_api/__init__.py
+-rw-r--r--   0 linzhiming   (502) staff       (20)       45 2023-06-15 08:43:50.000000 sanic-restful-api-0.1.9/sanic_restful_api/__version__.py
+-rw-r--r--   0 linzhiming   (502) staff       (20)    11785 2022-11-22 07:22:12.000000 sanic-restful-api-0.1.9/sanic_restful_api/fields.py
+-rw-r--r--   0 linzhiming   (502) staff       (20)     9104 2022-11-22 07:22:12.000000 sanic-restful-api-0.1.9/sanic_restful_api/inputs.py
+drwxr-xr-x   0 linzhiming   (502) staff       (20)        0 2023-06-15 08:44:53.466617 sanic-restful-api-0.1.9/sanic_restful_api/representations/
+-rw-r--r--   0 linzhiming   (502) staff       (20)        0 2022-11-22 07:22:12.000000 sanic-restful-api-0.1.9/sanic_restful_api/representations/__init__.py
+-rw-r--r--   0 linzhiming   (502) staff       (20)      425 2023-06-15 08:13:49.000000 sanic-restful-api-0.1.9/sanic_restful_api/representations/json.py
+-rw-r--r--   0 linzhiming   (502) staff       (20)    14413 2023-04-28 04:19:03.000000 sanic-restful-api-0.1.9/sanic_restful_api/reqparse.py
+drwxr-xr-x   0 linzhiming   (502) staff       (20)        0 2023-06-15 08:44:53.468488 sanic-restful-api-0.1.9/sanic_restful_api/utils/
+-rw-r--r--   0 linzhiming   (502) staff       (20)     1355 2022-11-22 07:22:12.000000 sanic-restful-api-0.1.9/sanic_restful_api/utils/__init__.py
+-rw-r--r--   0 linzhiming   (502) staff       (20)      746 2022-11-22 07:22:12.000000 sanic-restful-api-0.1.9/sanic_restful_api/utils/accept_mimetypes.py
+-rw-r--r--   0 linzhiming   (502) staff       (20)      996 2022-11-22 07:22:12.000000 sanic-restful-api-0.1.9/sanic_restful_api/utils/crypto.py
+drwxr-xr-x   0 linzhiming   (502) staff       (20)        0 2023-06-15 08:44:53.466328 sanic-restful-api-0.1.9/sanic_restful_api.egg-info/
+-rw-r--r--   0 linzhiming   (502) staff       (20)     2414 2023-06-15 08:44:53.000000 sanic-restful-api-0.1.9/sanic_restful_api.egg-info/PKG-INFO
+-rw-r--r--   0 linzhiming   (502) staff       (20)      631 2023-06-15 08:44:53.000000 sanic-restful-api-0.1.9/sanic_restful_api.egg-info/SOURCES.txt
+-rw-r--r--   0 linzhiming   (502) staff       (20)        1 2023-06-15 08:44:53.000000 sanic-restful-api-0.1.9/sanic_restful_api.egg-info/dependency_links.txt
+-rw-r--r--   0 linzhiming   (502) staff       (20)        1 2022-11-22 08:16:58.000000 sanic-restful-api-0.1.9/sanic_restful_api.egg-info/not-zip-safe
+-rw-r--r--   0 linzhiming   (502) staff       (20)       71 2023-06-15 08:44:53.000000 sanic-restful-api-0.1.9/sanic_restful_api.egg-info/requires.txt
+-rw-r--r--   0 linzhiming   (502) staff       (20)       18 2023-06-15 08:44:53.000000 sanic-restful-api-0.1.9/sanic_restful_api.egg-info/top_level.txt
+-rw-r--r--   0 linzhiming   (502) staff       (20)       70 2023-06-15 08:44:53.469427 sanic-restful-api-0.1.9/setup.cfg
+-rwxr-xr-x   0 linzhiming   (502) staff       (20)     1225 2023-04-28 04:24:41.000000 sanic-restful-api-0.1.9/setup.py
```

### Comparing `sanic-restful-api-0.1.8/LICENSE` & `sanic-restful-api-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sanic-restful-api-0.1.8/PKG-INFO` & `sanic-restful-api-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanic-restful-api
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simple framework for creating REST APIs
 Home-page: https://github.com/linzhiming0826/sanic-restful
 Author: TuoX
 Author-email: 120549827@qq.com
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `sanic-restful-api-0.1.8/README.md` & `sanic-restful-api-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `sanic-restful-api-0.1.8/sanic_restful_api/__init__.py` & `sanic-restful-api-0.1.9/sanic_restful_api/__init__.py`

 * *Files identical despite different names*

### Comparing `sanic-restful-api-0.1.8/sanic_restful_api/fields.py` & `sanic-restful-api-0.1.9/sanic_restful_api/fields.py`

 * *Files identical despite different names*

### Comparing `sanic-restful-api-0.1.8/sanic_restful_api/inputs.py` & `sanic-restful-api-0.1.9/sanic_restful_api/inputs.py`

 * *Files identical despite different names*

### Comparing `sanic-restful-api-0.1.8/sanic_restful_api/reqparse.py` & `sanic-restful-api-0.1.9/sanic_restful_api/reqparse.py`

 * *Files identical despite different names*

### Comparing `sanic-restful-api-0.1.8/sanic_restful_api/utils/__init__.py` & `sanic-restful-api-0.1.9/sanic_restful_api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sanic-restful-api-0.1.8/sanic_restful_api/utils/accept_mimetypes.py` & `sanic-restful-api-0.1.9/sanic_restful_api/utils/accept_mimetypes.py`

 * *Files identical despite different names*

### Comparing `sanic-restful-api-0.1.8/sanic_restful_api/utils/crypto.py` & `sanic-restful-api-0.1.9/sanic_restful_api/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `sanic-restful-api-0.1.8/sanic_restful_api.egg-info/PKG-INFO` & `sanic-restful-api-0.1.9/sanic_restful_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanic-restful-api
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simple framework for creating REST APIs
 Home-page: https://github.com/linzhiming0826/sanic-restful
 Author: TuoX
 Author-email: 120549827@qq.com
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `sanic-restful-api-0.1.8/sanic_restful_api.egg-info/SOURCES.txt` & `sanic-restful-api-0.1.9/sanic_restful_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sanic-restful-api-0.1.8/setup.py` & `sanic-restful-api-0.1.9/setup.py`

 * *Files identical despite different names*

