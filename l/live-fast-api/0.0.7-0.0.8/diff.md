# Comparing `tmp/live-fast-api-0.0.7.tar.gz` & `tmp/live-fast-api-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "live-fast-api-0.0.7.tar", last modified: Tue Jun 13 13:34:51 2023, max compression
+gzip compressed data, was "live-fast-api-0.0.8.tar", last modified: Thu Jun 15 21:46:38 2023, max compression
```

## Comparing `live-fast-api-0.0.7.tar` & `live-fast-api-0.0.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 13:34:51.769003 live-fast-api-0.0.7/
--rw-rw-rw-   0        0        0      215 2023-06-13 13:34:51.000000 live-fast-api-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2054 2023-06-13 13:34:51.768002 live-fast-api-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1245 2023-04-12 14:06:13.000000 live-fast-api-0.0.7/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:14:12.000000 live-fast-api-0.0.7/build.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:34:51.706879 live-fast-api-0.0.7/live_api/
--rw-rw-rw-   0        0        0      493 2023-03-09 10:59:51.000000 live-fast-api-0.0.7/live_api/__init__.py
--rw-rw-rw-   0        0        0     7565 2023-06-11 21:12:00.000000 live-fast-api-0.0.7/live_api/base.py
--rw-rw-rw-   0        0        0      281 2023-04-12 14:23:43.000000 live-fast-api-0.0.7/live_api/document.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:34:51.731885 live-fast-api-0.0.7/live_api/endpoints/
--rw-rw-rw-   0        0        0      182 2023-04-12 14:16:43.000000 live-fast-api-0.0.7/live_api/endpoints/__init__.py
--rw-rw-rw-   0        0        0     2599 2023-04-12 14:12:33.000000 live-fast-api-0.0.7/live_api/endpoints/data.py
--rw-rw-rw-   0        0        0    10741 2023-06-13 13:34:08.000000 live-fast-api-0.0.7/live_api/endpoints/engine.py
--rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 live-fast-api-0.0.7/live_api/endpoints/exceptions.py
--rw-rw-rw-   0        0        0     1601 2023-04-12 14:15:29.000000 live-fast-api-0.0.7/live_api/endpoints/process.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:34:51.747993 live-fast-api-0.0.7/live_api/service/
--rw-rw-rw-   0        0        0       92 2023-04-12 14:22:24.000000 live-fast-api-0.0.7/live_api/service/__init__.py
--rw-rw-rw-   0        0        0    19305 2023-06-11 21:25:12.000000 live-fast-api-0.0.7/live_api/service/rest.py
--rw-rw-rw-   0        0        0     2991 2023-04-21 18:19:24.000000 live-fast-api-0.0.7/live_api/service/sockets.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:34:51.681869 live-fast-api-0.0.7/live_api/source/
-drwxrwxrwx   0        0        0        0 2023-06-13 13:34:51.681869 live-fast-api-0.0.7/live_api/source/assets/
-drwxrwxrwx   0        0        0        0 2023-06-13 13:34:51.753001 live-fast-api-0.0.7/live_api/source/assets/icon/
--rw-rw-rw-   0        0        0     2834 2023-02-04 16:41:18.000000 live-fast-api-0.0.7/live_api/source/assets/icon/icon.ico
--rw-rw-rw-   0        0        0    27619 2023-02-04 16:40:24.000000 live-fast-api-0.0.7/live_api/source/assets/icon/icon.png
-drwxrwxrwx   0        0        0        0 2023-06-13 13:34:51.767032 live-fast-api-0.0.7/live_fast_api.egg-info/
--rw-rw-rw-   0        0        0     2054 2023-06-13 13:34:51.000000 live-fast-api-0.0.7/live_fast_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      641 2023-06-13 13:34:51.000000 live-fast-api-0.0.7/live_fast_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 13:34:51.000000 live-fast-api-0.0.7/live_fast_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-06-13 13:34:51.000000 live-fast-api-0.0.7/live_fast_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-13 13:34:51.000000 live-fast-api-0.0.7/live_fast_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      625 2023-06-13 13:34:51.000000 live-fast-api-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      100 2023-04-21 18:21:15.000000 live-fast-api-0.0.7/requirements-dev.txt
--rw-rw-rw-   0        0        0       91 2023-04-21 18:18:24.000000 live-fast-api-0.0.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 13:34:51.769003 live-fast-api-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1580 2023-06-13 13:34:24.000000 live-fast-api-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:46:38.153746 live-fast-api-0.0.8/
+-rw-rw-rw-   0        0        0      215 2023-06-15 21:46:37.000000 live-fast-api-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2054 2023-06-15 21:46:38.152746 live-fast-api-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1245 2023-04-12 14:06:13.000000 live-fast-api-0.0.8/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:14:12.000000 live-fast-api-0.0.8/build.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:46:38.082776 live-fast-api-0.0.8/live_api/
+-rw-rw-rw-   0        0        0      493 2023-03-09 10:59:51.000000 live-fast-api-0.0.8/live_api/__init__.py
+-rw-rw-rw-   0        0        0     7565 2023-06-11 21:12:00.000000 live-fast-api-0.0.8/live_api/base.py
+-rw-rw-rw-   0        0        0      281 2023-04-12 14:23:43.000000 live-fast-api-0.0.8/live_api/document.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:46:38.114776 live-fast-api-0.0.8/live_api/endpoints/
+-rw-rw-rw-   0        0        0      182 2023-04-12 14:16:43.000000 live-fast-api-0.0.8/live_api/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     2599 2023-04-12 14:12:33.000000 live-fast-api-0.0.8/live_api/endpoints/data.py
+-rw-rw-rw-   0        0        0    10741 2023-06-13 13:34:08.000000 live-fast-api-0.0.8/live_api/endpoints/engine.py
+-rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 live-fast-api-0.0.8/live_api/endpoints/exceptions.py
+-rw-rw-rw-   0        0        0     1601 2023-04-12 14:15:29.000000 live-fast-api-0.0.8/live_api/endpoints/process.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:46:38.131773 live-fast-api-0.0.8/live_api/service/
+-rw-rw-rw-   0        0        0       92 2023-04-12 14:22:24.000000 live-fast-api-0.0.8/live_api/service/__init__.py
+-rw-rw-rw-   0        0        0    19305 2023-06-11 21:25:12.000000 live-fast-api-0.0.8/live_api/service/rest.py
+-rw-rw-rw-   0        0        0     2991 2023-04-21 18:19:24.000000 live-fast-api-0.0.8/live_api/service/sockets.py
+drwxrwxrwx   0        0        0        0 2023-06-15 21:46:38.052747 live-fast-api-0.0.8/live_api/source/
+drwxrwxrwx   0        0        0        0 2023-06-15 21:46:38.052747 live-fast-api-0.0.8/live_api/source/assets/
+drwxrwxrwx   0        0        0        0 2023-06-15 21:46:38.136767 live-fast-api-0.0.8/live_api/source/assets/icon/
+-rw-rw-rw-   0        0        0     2834 2023-02-04 16:41:18.000000 live-fast-api-0.0.8/live_api/source/assets/icon/icon.ico
+-rw-rw-rw-   0        0        0    27619 2023-02-04 16:40:24.000000 live-fast-api-0.0.8/live_api/source/assets/icon/icon.png
+drwxrwxrwx   0        0        0        0 2023-06-15 21:46:38.152746 live-fast-api-0.0.8/live_fast_api.egg-info/
+-rw-rw-rw-   0        0        0     2054 2023-06-15 21:46:37.000000 live-fast-api-0.0.8/live_fast_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2023-06-15 21:46:38.000000 live-fast-api-0.0.8/live_fast_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 21:46:37.000000 live-fast-api-0.0.8/live_fast_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-06-15 21:46:37.000000 live-fast-api-0.0.8/live_fast_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 21:46:37.000000 live-fast-api-0.0.8/live_fast_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      625 2023-06-15 21:46:37.000000 live-fast-api-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      173 2023-06-15 21:46:37.000000 live-fast-api-0.0.8/requirements-dev.txt
+-rw-rw-rw-   0        0        0       69 2023-06-15 21:46:16.000000 live-fast-api-0.0.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 21:46:38.153746 live-fast-api-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1580 2023-06-15 21:46:26.000000 live-fast-api-0.0.8/setup.py
```

### Comparing `live-fast-api-0.0.7/PKG-INFO` & `live-fast-api-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: live-fast-api
-Version: 0.0.7
+Version: 0.0.8
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/live-api
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `live-fast-api-0.0.7/README.md` & `live-fast-api-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.7/build.py` & `live-fast-api-0.0.8/build.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.7/live_api/base.py` & `live-fast-api-0.0.8/live_api/base.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.7/live_api/endpoints/data.py` & `live-fast-api-0.0.8/live_api/endpoints/data.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.7/live_api/endpoints/engine.py` & `live-fast-api-0.0.8/live_api/endpoints/engine.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.7/live_api/endpoints/exceptions.py` & `live-fast-api-0.0.8/live_api/endpoints/exceptions.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.7/live_api/endpoints/process.py` & `live-fast-api-0.0.8/live_api/endpoints/process.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.7/live_api/service/rest.py` & `live-fast-api-0.0.8/live_api/service/rest.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.7/live_api/service/sockets.py` & `live-fast-api-0.0.8/live_api/service/sockets.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.7/live_api/source/assets/icon/icon.ico` & `live-fast-api-0.0.8/live_api/source/assets/icon/icon.ico`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.7/live_api/source/assets/icon/icon.png` & `live-fast-api-0.0.8/live_api/source/assets/icon/icon.png`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.7/live_fast_api.egg-info/PKG-INFO` & `live-fast-api-0.0.8/live_fast_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: live-fast-api
-Version: 0.0.7
+Version: 0.0.8
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/live-api
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `live-fast-api-0.0.7/live_fast_api.egg-info/SOURCES.txt` & `live-fast-api-0.0.8/live_fast_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.7/setup.py` & `live-fast-api-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "live_api/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='live-fast-api',
-        version='0.0.7',
+        version='0.0.8',
         description=(
             "A framework for developing responsive, "
             "live and dynamic REST APIs with python."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

