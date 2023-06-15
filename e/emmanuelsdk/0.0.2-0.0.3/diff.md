# Comparing `tmp/emmanuelsdk-0.0.2.tar.gz` & `tmp/emmanuelsdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmanuelsdk-0.0.2.tar", last modified: Thu Jun 15 11:34:25 2023, max compression
+gzip compressed data, was "emmanuelsdk-0.0.3.tar", last modified: Thu Jun 15 12:01:01 2023, max compression
```

## Comparing `emmanuelsdk-0.0.2.tar` & `emmanuelsdk-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 11:34:25.267992 emmanuelsdk-0.0.2/
--rw-r--r--   0 emmanuel   (501) staff       (20)      282 2023-06-15 11:34:25.267626 emmanuelsdk-0.0.2/PKG-INFO
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 11:34:25.259398 emmanuelsdk-0.0.2/core/
--rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-14 19:00:45.000000 emmanuelsdk-0.0.2/core/__init__.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 11:34:25.259691 emmanuelsdk-0.0.2/core/configs/
--rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-14 20:41:43.000000 emmanuelsdk-0.0.2/core/configs/__init__.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      105 2023-06-15 02:42:17.000000 emmanuelsdk-0.0.2/core/configs/variables.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 11:34:25.261146 emmanuelsdk-0.0.2/core/models/
--rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-14 19:02:00.000000 emmanuelsdk-0.0.2/core/models/__init__.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      748 2023-06-15 05:52:56.000000 emmanuelsdk-0.0.2/core/models/movie.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      529 2023-06-15 07:22:21.000000 emmanuelsdk-0.0.2/core/models/quote.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 11:34:25.262651 emmanuelsdk-0.0.2/core/utils/
--rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-14 19:01:49.000000 emmanuelsdk-0.0.2/core/utils/__init__.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      545 2023-06-15 02:57:15.000000 emmanuelsdk-0.0.2/core/utils/errors.py
--rw-r--r--   0 emmanuel   (501) staff       (20)     2039 2023-06-15 05:48:01.000000 emmanuelsdk-0.0.2/core/utils/helpers.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 11:34:25.266809 emmanuelsdk-0.0.2/emmanuelsdk.egg-info/
--rw-r--r--   0 emmanuel   (501) staff       (20)      282 2023-06-15 11:34:25.000000 emmanuelsdk-0.0.2/emmanuelsdk.egg-info/PKG-INFO
--rw-r--r--   0 emmanuel   (501) staff       (20)      403 2023-06-15 11:34:25.000000 emmanuelsdk-0.0.2/emmanuelsdk.egg-info/SOURCES.txt
--rw-r--r--   0 emmanuel   (501) staff       (20)        1 2023-06-15 11:34:25.000000 emmanuelsdk-0.0.2/emmanuelsdk.egg-info/dependency_links.txt
--rw-r--r--   0 emmanuel   (501) staff       (20)       16 2023-06-15 11:34:25.000000 emmanuelsdk-0.0.2/emmanuelsdk.egg-info/requires.txt
--rw-r--r--   0 emmanuel   (501) staff       (20)        5 2023-06-15 11:34:25.000000 emmanuelsdk-0.0.2/emmanuelsdk.egg-info/top_level.txt
--rw-r--r--   0 emmanuel   (501) staff       (20)       38 2023-06-15 11:34:25.268198 emmanuelsdk-0.0.2/setup.cfg
--rw-r--r--   0 emmanuel   (501) staff       (20)      474 2023-06-15 11:33:10.000000 emmanuelsdk-0.0.2/setup.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 11:34:25.266981 emmanuelsdk-0.0.2/tests/
--rw-r--r--   0 emmanuel   (501) staff       (20)     1133 2023-06-15 07:37:27.000000 emmanuelsdk-0.0.2/tests/test_client.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 12:01:01.464635 emmanuelsdk-0.0.3/
+-rw-r--r--   0 emmanuel   (501) staff       (20)      282 2023-06-15 12:01:01.464296 emmanuelsdk-0.0.3/PKG-INFO
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 12:01:01.459562 emmanuelsdk-0.0.3/core/
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-14 19:00:45.000000 emmanuelsdk-0.0.3/core/__init__.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 12:01:01.459802 emmanuelsdk-0.0.3/core/configs/
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-14 20:41:43.000000 emmanuelsdk-0.0.3/core/configs/__init__.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      105 2023-06-15 02:42:17.000000 emmanuelsdk-0.0.3/core/configs/variables.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 12:01:01.461072 emmanuelsdk-0.0.3/core/models/
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-14 19:02:00.000000 emmanuelsdk-0.0.3/core/models/__init__.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      748 2023-06-15 05:52:56.000000 emmanuelsdk-0.0.3/core/models/movie.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      529 2023-06-15 07:22:21.000000 emmanuelsdk-0.0.3/core/models/quote.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 12:01:01.462441 emmanuelsdk-0.0.3/core/utils/
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-14 19:01:49.000000 emmanuelsdk-0.0.3/core/utils/__init__.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      545 2023-06-15 02:57:15.000000 emmanuelsdk-0.0.3/core/utils/errors.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     2039 2023-06-15 05:48:01.000000 emmanuelsdk-0.0.3/core/utils/helpers.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 12:01:01.463712 emmanuelsdk-0.0.3/emmanuelsdk.egg-info/
+-rw-r--r--   0 emmanuel   (501) staff       (20)      282 2023-06-15 12:01:01.000000 emmanuelsdk-0.0.3/emmanuelsdk.egg-info/PKG-INFO
+-rw-r--r--   0 emmanuel   (501) staff       (20)      403 2023-06-15 12:01:01.000000 emmanuelsdk-0.0.3/emmanuelsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 emmanuel   (501) staff       (20)        1 2023-06-15 12:01:01.000000 emmanuelsdk-0.0.3/emmanuelsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 emmanuel   (501) staff       (20)       16 2023-06-15 12:01:01.000000 emmanuelsdk-0.0.3/emmanuelsdk.egg-info/requires.txt
+-rw-r--r--   0 emmanuel   (501) staff       (20)        5 2023-06-15 12:01:01.000000 emmanuelsdk-0.0.3/emmanuelsdk.egg-info/top_level.txt
+-rw-r--r--   0 emmanuel   (501) staff       (20)       38 2023-06-15 12:01:01.464713 emmanuelsdk-0.0.3/setup.cfg
+-rw-r--r--   0 emmanuel   (501) staff       (20)      474 2023-06-15 12:00:42.000000 emmanuelsdk-0.0.3/setup.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 12:01:01.463874 emmanuelsdk-0.0.3/tests/
+-rw-r--r--   0 emmanuel   (501) staff       (20)     1133 2023-06-15 07:37:27.000000 emmanuelsdk-0.0.3/tests/test_client.py
```

### Comparing `emmanuelsdk-0.0.2/core/models/movie.py` & `emmanuelsdk-0.0.3/core/models/movie.py`

 * *Files identical despite different names*

### Comparing `emmanuelsdk-0.0.2/core/models/quote.py` & `emmanuelsdk-0.0.3/core/models/quote.py`

 * *Files identical despite different names*

### Comparing `emmanuelsdk-0.0.2/core/utils/errors.py` & `emmanuelsdk-0.0.3/core/utils/errors.py`

 * *Files identical despite different names*

### Comparing `emmanuelsdk-0.0.2/core/utils/helpers.py` & `emmanuelsdk-0.0.3/core/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `emmanuelsdk-0.0.2/tests/test_client.py` & `emmanuelsdk-0.0.3/tests/test_client.py`

 * *Files identical despite different names*

