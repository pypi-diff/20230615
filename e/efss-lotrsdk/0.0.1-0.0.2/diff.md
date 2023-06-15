# Comparing `tmp/efss-lotrsdk-0.0.1.tar.gz` & `tmp/efss-lotrsdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efss-lotrsdk-0.0.1.tar", last modified: Thu Jun 15 12:22:39 2023, max compression
+gzip compressed data, was "efss-lotrsdk-0.0.2.tar", last modified: Thu Jun 15 12:34:36 2023, max compression
```

## Comparing `efss-lotrsdk-0.0.1.tar` & `efss-lotrsdk-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 12:22:39.563769 efss-lotrsdk-0.0.1/
--rw-r--r--   0 emmanuel   (501) staff       (20)      283 2023-06-15 12:22:39.563487 efss-lotrsdk-0.0.1/PKG-INFO
--rw-r--r--   0 emmanuel   (501) staff       (20)      842 2023-06-15 10:06:54.000000 efss-lotrsdk-0.0.1/README.md
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 12:22:39.559037 efss-lotrsdk-0.0.1/efss_lotrsdk.egg-info/
--rw-r--r--   0 emmanuel   (501) staff       (20)      283 2023-06-15 12:22:39.000000 efss-lotrsdk-0.0.1/efss_lotrsdk.egg-info/PKG-INFO
--rw-r--r--   0 emmanuel   (501) staff       (20)      463 2023-06-15 12:22:39.000000 efss-lotrsdk-0.0.1/efss_lotrsdk.egg-info/SOURCES.txt
--rw-r--r--   0 emmanuel   (501) staff       (20)        1 2023-06-15 12:22:39.000000 efss-lotrsdk-0.0.1/efss_lotrsdk.egg-info/dependency_links.txt
--rw-r--r--   0 emmanuel   (501) staff       (20)       16 2023-06-15 12:22:39.000000 efss-lotrsdk-0.0.1/efss_lotrsdk.egg-info/requires.txt
--rw-r--r--   0 emmanuel   (501) staff       (20)        4 2023-06-15 12:22:39.000000 efss-lotrsdk-0.0.1/efss_lotrsdk.egg-info/top_level.txt
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 12:22:39.559933 efss-lotrsdk-0.0.1/sdk/
--rw-r--r--   0 emmanuel   (501) staff       (20)       26 2023-06-15 11:59:48.000000 efss-lotrsdk-0.0.1/sdk/__init__.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      648 2023-06-15 12:00:08.000000 efss-lotrsdk-0.0.1/sdk/client.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 12:22:39.560267 efss-lotrsdk-0.0.1/sdk/core/
--rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-14 19:00:45.000000 efss-lotrsdk-0.0.1/sdk/core/__init__.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 12:22:39.560532 efss-lotrsdk-0.0.1/sdk/core/configs/
--rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-14 20:41:43.000000 efss-lotrsdk-0.0.1/sdk/core/configs/__init__.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      105 2023-06-15 02:42:17.000000 efss-lotrsdk-0.0.1/sdk/core/configs/variables.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 12:22:39.561848 efss-lotrsdk-0.0.1/sdk/core/models/
--rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-14 19:02:00.000000 efss-lotrsdk-0.0.1/sdk/core/models/__init__.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      748 2023-06-15 05:52:56.000000 efss-lotrsdk-0.0.1/sdk/core/models/movie.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      529 2023-06-15 07:22:21.000000 efss-lotrsdk-0.0.1/sdk/core/models/quote.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 12:22:39.562981 efss-lotrsdk-0.0.1/sdk/core/utils/
--rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-14 19:01:49.000000 efss-lotrsdk-0.0.1/sdk/core/utils/__init__.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      545 2023-06-15 02:57:15.000000 efss-lotrsdk-0.0.1/sdk/core/utils/errors.py
--rw-r--r--   0 emmanuel   (501) staff       (20)     2039 2023-06-15 05:48:01.000000 efss-lotrsdk-0.0.1/sdk/core/utils/helpers.py
--rw-r--r--   0 emmanuel   (501) staff       (20)       38 2023-06-15 12:22:39.563820 efss-lotrsdk-0.0.1/setup.cfg
--rw-r--r--   0 emmanuel   (501) staff       (20)      475 2023-06-15 12:22:00.000000 efss-lotrsdk-0.0.1/setup.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 12:34:36.843587 efss-lotrsdk-0.0.2/
+-rw-r--r--   0 emmanuel   (501) staff       (20)      283 2023-06-15 12:34:36.843290 efss-lotrsdk-0.0.2/PKG-INFO
+-rw-r--r--   0 emmanuel   (501) staff       (20)      842 2023-06-15 10:06:54.000000 efss-lotrsdk-0.0.2/README.md
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 12:34:36.839233 efss-lotrsdk-0.0.2/efss_lotrsdk.egg-info/
+-rw-r--r--   0 emmanuel   (501) staff       (20)      283 2023-06-15 12:34:36.000000 efss-lotrsdk-0.0.2/efss_lotrsdk.egg-info/PKG-INFO
+-rw-r--r--   0 emmanuel   (501) staff       (20)      463 2023-06-15 12:34:36.000000 efss-lotrsdk-0.0.2/efss_lotrsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 emmanuel   (501) staff       (20)        1 2023-06-15 12:34:36.000000 efss-lotrsdk-0.0.2/efss_lotrsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 emmanuel   (501) staff       (20)       16 2023-06-15 12:34:36.000000 efss-lotrsdk-0.0.2/efss_lotrsdk.egg-info/requires.txt
+-rw-r--r--   0 emmanuel   (501) staff       (20)        4 2023-06-15 12:34:36.000000 efss-lotrsdk-0.0.2/efss_lotrsdk.egg-info/top_level.txt
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 12:34:36.839965 efss-lotrsdk-0.0.2/sdk/
+-rw-r--r--   0 emmanuel   (501) staff       (20)       26 2023-06-15 11:59:48.000000 efss-lotrsdk-0.0.2/sdk/__init__.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      648 2023-06-15 12:00:08.000000 efss-lotrsdk-0.0.2/sdk/client.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 12:34:36.840339 efss-lotrsdk-0.0.2/sdk/core/
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-14 19:00:45.000000 efss-lotrsdk-0.0.2/sdk/core/__init__.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 12:34:36.840723 efss-lotrsdk-0.0.2/sdk/core/configs/
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-14 20:41:43.000000 efss-lotrsdk-0.0.2/sdk/core/configs/__init__.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      105 2023-06-15 02:42:17.000000 efss-lotrsdk-0.0.2/sdk/core/configs/variables.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 12:34:36.841909 efss-lotrsdk-0.0.2/sdk/core/models/
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-14 19:02:00.000000 efss-lotrsdk-0.0.2/sdk/core/models/__init__.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      748 2023-06-15 05:52:56.000000 efss-lotrsdk-0.0.2/sdk/core/models/movie.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      529 2023-06-15 07:22:21.000000 efss-lotrsdk-0.0.2/sdk/core/models/quote.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2023-06-15 12:34:36.842834 efss-lotrsdk-0.0.2/sdk/core/utils/
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2023-06-14 19:01:49.000000 efss-lotrsdk-0.0.2/sdk/core/utils/__init__.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      545 2023-06-15 02:57:15.000000 efss-lotrsdk-0.0.2/sdk/core/utils/errors.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     2039 2023-06-15 05:48:01.000000 efss-lotrsdk-0.0.2/sdk/core/utils/helpers.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)       38 2023-06-15 12:34:36.843641 efss-lotrsdk-0.0.2/setup.cfg
+-rw-r--r--   0 emmanuel   (501) staff       (20)      475 2023-06-15 12:34:30.000000 efss-lotrsdk-0.0.2/setup.py
```

### Comparing `efss-lotrsdk-0.0.1/README.md` & `efss-lotrsdk-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `efss-lotrsdk-0.0.1/sdk/client.py` & `efss-lotrsdk-0.0.2/sdk/client.py`

 * *Files identical despite different names*

### Comparing `efss-lotrsdk-0.0.1/sdk/core/models/movie.py` & `efss-lotrsdk-0.0.2/sdk/core/models/movie.py`

 * *Files identical despite different names*

### Comparing `efss-lotrsdk-0.0.1/sdk/core/models/quote.py` & `efss-lotrsdk-0.0.2/sdk/core/models/quote.py`

 * *Files identical despite different names*

### Comparing `efss-lotrsdk-0.0.1/sdk/core/utils/errors.py` & `efss-lotrsdk-0.0.2/sdk/core/utils/errors.py`

 * *Files identical despite different names*

### Comparing `efss-lotrsdk-0.0.1/sdk/core/utils/helpers.py` & `efss-lotrsdk-0.0.2/sdk/core/utils/helpers.py`

 * *Files identical despite different names*

