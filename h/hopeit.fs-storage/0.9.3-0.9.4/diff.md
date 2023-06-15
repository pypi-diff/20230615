# Comparing `tmp/hopeit.fs-storage-0.9.3.tar.gz` & `tmp/hopeit.fs-storage-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hopeit.fs-storage-0.9.3.tar", last modified: Mon Jul 12 23:34:15 2021, max compression
+gzip compressed data, was "hopeit.fs-storage-0.9.4.tar", last modified: Wed Jul 14 00:51:56 2021, max compression
```

## Comparing `hopeit.fs-storage-0.9.3.tar` & `hopeit.fs-storage-0.9.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:15.050166 hopeit.fs-storage-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1538 2021-07-12 23:34:15.050166 hopeit.fs-storage-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      234 2021-07-12 23:27:48.000000 hopeit.fs-storage-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-12 23:34:15.050166 hopeit.fs-storage-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2021-07-12 23:27:48.000000 hopeit.fs-storage-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:15.050166 hopeit.fs-storage-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:15.050166 hopeit.fs-storage-0.9.3/src/hopeit/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:15.050166 hopeit.fs-storage-0.9.3/src/hopeit/fs_storage/
--rw-r--r--   0 runner    (1001) docker     (121)     3249 2021-07-12 23:27:48.000000 hopeit.fs-storage-0.9.3/src/hopeit/fs_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:15.050166 hopeit.fs-storage-0.9.3/src/hopeit.fs_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1538 2021-07-12 23:34:15.000000 hopeit.fs-storage-0.9.3/src/hopeit.fs_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      276 2021-07-12 23:34:15.000000 hopeit.fs-storage-0.9.3/src/hopeit.fs_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-12 23:34:15.000000 hopeit.fs-storage-0.9.3/src/hopeit.fs_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-07-12 23:34:15.000000 hopeit.fs-storage-0.9.3/src/hopeit.fs_storage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-07-12 23:34:15.000000 hopeit.fs-storage-0.9.3/src/hopeit.fs_storage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:56.504908 hopeit.fs-storage-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)     1538 2021-07-14 00:51:56.504908 hopeit.fs-storage-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      234 2021-07-14 00:45:26.000000 hopeit.fs-storage-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-14 00:51:56.504908 hopeit.fs-storage-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1929 2021-07-14 00:45:26.000000 hopeit.fs-storage-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:56.500908 hopeit.fs-storage-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:56.500908 hopeit.fs-storage-0.9.4/src/hopeit/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:56.504908 hopeit.fs-storage-0.9.4/src/hopeit/fs_storage/
+-rw-r--r--   0 runner    (1001) docker     (121)     3249 2021-07-14 00:45:26.000000 hopeit.fs-storage-0.9.4/src/hopeit/fs_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:56.504908 hopeit.fs-storage-0.9.4/src/hopeit.fs_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1538 2021-07-14 00:51:56.000000 hopeit.fs-storage-0.9.4/src/hopeit.fs_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2021-07-14 00:51:56.000000 hopeit.fs-storage-0.9.4/src/hopeit.fs_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-14 00:51:56.000000 hopeit.fs-storage-0.9.4/src/hopeit.fs_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2021-07-14 00:51:56.000000 hopeit.fs-storage-0.9.4/src/hopeit.fs_storage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-07-14 00:51:56.000000 hopeit.fs-storage-0.9.4/src/hopeit.fs_storage.egg-info/top_level.txt
```

### Comparing `hopeit.fs-storage-0.9.3/PKG-INFO` & `hopeit.fs-storage-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopeit.fs-storage
-Version: 0.9.3
+Version: 0.9.4
 Summary: Hopeit Engine File System Storage Toolkit
 Home-page: https://github.com/hopeit-git/hopeit.engine
 Author: Leo Smerling and Pablo Canto
 Author-email: contact@hopeit.com.ar
 License: Apache 2
 Project-URL: CI: GitHub Actions, https://github.com/hopeit-git/hopeit.engine/actions?query=workflow
 Project-URL: Docs: RTD, https://hopeitengine.readthedocs.io/en/latest/
```

### Comparing `hopeit.fs-storage-0.9.3/setup.py` & `hopeit.fs-storage-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `hopeit.fs-storage-0.9.3/src/hopeit/fs_storage/__init__.py` & `hopeit.fs-storage-0.9.4/src/hopeit/fs_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `hopeit.fs-storage-0.9.3/src/hopeit.fs_storage.egg-info/PKG-INFO` & `hopeit.fs-storage-0.9.4/src/hopeit.fs_storage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopeit.fs-storage
-Version: 0.9.3
+Version: 0.9.4
 Summary: Hopeit Engine File System Storage Toolkit
 Home-page: https://github.com/hopeit-git/hopeit.engine
 Author: Leo Smerling and Pablo Canto
 Author-email: contact@hopeit.com.ar
 License: Apache 2
 Project-URL: CI: GitHub Actions, https://github.com/hopeit-git/hopeit.engine/actions?query=workflow
 Project-URL: Docs: RTD, https://hopeitengine.readthedocs.io/en/latest/
```

