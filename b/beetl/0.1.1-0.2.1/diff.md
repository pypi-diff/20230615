# Comparing `tmp/beetl-0.1.1.tar.gz` & `tmp/beetl-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beetl-0.1.1.tar", last modified: Tue Mar 14 16:05:57 2023, max compression
+gzip compressed data, was "beetl-0.2.1.tar", last modified: Thu Jun 15 11:06:25 2023, max compression
```

## Comparing `beetl-0.1.1.tar` & `beetl-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,39 @@
-drwxrwxr-x   0 larsch    (1003) larsch    (1003)        0 2023-03-14 16:05:57.980746 beetl-0.1.1/
--rw-rw-r--   0 larsch    (1003) larsch    (1003)     5808 2023-03-14 16:05:57.980746 beetl-0.1.1/PKG-INFO
--rw-rw-r--   0 larsch    (1003) larsch    (1003)     5204 2023-03-14 15:45:18.000000 beetl-0.1.1/README.md
--rw-rw-r--   0 larsch    (1003) larsch    (1003)       38 2023-03-14 16:05:57.980746 beetl-0.1.1/setup.cfg
--rw-rw-r--   0 larsch    (1003) larsch    (1003)     1626 2023-03-14 16:03:52.000000 beetl-0.1.1/setup.py
-drwxrwxr-x   0 larsch    (1003) larsch    (1003)        0 2023-03-14 16:05:57.976746 beetl-0.1.1/src/
-drwxrwxr-x   0 larsch    (1003) larsch    (1003)        0 2023-03-14 16:05:57.976746 beetl-0.1.1/src/beetl/
--rw-rw-r--   0 larsch    (1003) larsch    (1003)       36 2023-02-09 16:27:50.000000 beetl-0.1.1/src/beetl/__init__.py
--rw-rw-r--   0 larsch    (1003) larsch    (1003)      658 2023-03-14 16:05:44.000000 beetl-0.1.1/src/beetl/__version__.py
--rw-rw-r--   0 larsch    (1003) larsch    (1003)     2070 2023-03-14 15:36:40.000000 beetl-0.1.1/src/beetl/beetl.py
--rw-rw-r--   0 larsch    (1003) larsch    (1003)     3158 2023-03-14 15:51:40.000000 beetl-0.1.1/src/beetl/config.py
-drwxrwxr-x   0 larsch    (1003) larsch    (1003)        0 2023-03-14 16:05:57.980746 beetl-0.1.1/src/beetl/field_transformers/
--rw-rw-r--   0 larsch    (1003) larsch    (1003)        0 2023-03-14 15:52:38.000000 beetl-0.1.1/src/beetl/field_transformers/__init__.py
--rw-rw-r--   0 larsch    (1003) larsch    (1003)        0 2023-03-14 15:52:34.000000 beetl-0.1.1/src/beetl/field_transformers/interface.py
-drwxrwxr-x   0 larsch    (1003) larsch    (1003)        0 2023-03-14 16:05:57.980746 beetl-0.1.1/src/beetl/source_transformers/
--rw-rw-r--   0 larsch    (1003) larsch    (1003)        0 2023-03-14 15:52:43.000000 beetl-0.1.1/src/beetl/source_transformers/__init__.py
--rw-rw-r--   0 larsch    (1003) larsch    (1003)        0 2023-03-14 15:52:48.000000 beetl-0.1.1/src/beetl/source_transformers/interface.py
-drwxrwxr-x   0 larsch    (1003) larsch    (1003)        0 2023-03-14 16:05:57.980746 beetl-0.1.1/src/beetl/sources/
--rw-rw-r--   0 larsch    (1003) larsch    (1003)        0 2023-03-14 10:18:50.000000 beetl-0.1.1/src/beetl/sources/__init__.py
--rw-rw-r--   0 larsch    (1003) larsch    (1003)     3185 2023-03-14 15:37:34.000000 beetl-0.1.1/src/beetl/sources/file.py
--rw-rw-r--   0 larsch    (1003) larsch    (1003)     3587 2023-03-14 15:30:34.000000 beetl-0.1.1/src/beetl/sources/interface.py
--rw-rw-r--   0 larsch    (1003) larsch    (1003)     2632 2023-03-14 14:59:13.000000 beetl-0.1.1/src/beetl/sources/mysql.py
--rw-rw-r--   0 larsch    (1003) larsch    (1003)      940 2023-03-14 14:10:45.000000 beetl-0.1.1/src/beetl/sources/sqlserver.py
--rw-rw-r--   0 larsch    (1003) larsch    (1003)     2150 2023-03-14 10:21:37.000000 beetl-0.1.1/src/beetl/sources.py
--rw-rw-r--   0 larsch    (1003) larsch    (1003)     1718 2023-02-15 10:46:36.000000 beetl-0.1.1/src/beetl/transformers.py
-drwxrwxr-x   0 larsch    (1003) larsch    (1003)        0 2023-03-14 16:05:57.980746 beetl-0.1.1/src/beetl.egg-info/
--rw-rw-r--   0 larsch    (1003) larsch    (1003)     5808 2023-03-14 16:05:57.000000 beetl-0.1.1/src/beetl.egg-info/PKG-INFO
--rw-rw-r--   0 larsch    (1003) larsch    (1003)      692 2023-03-14 16:05:57.000000 beetl-0.1.1/src/beetl.egg-info/SOURCES.txt
--rw-rw-r--   0 larsch    (1003) larsch    (1003)        1 2023-03-14 16:05:57.000000 beetl-0.1.1/src/beetl.egg-info/dependency_links.txt
--rw-rw-r--   0 larsch    (1003) larsch    (1003)       52 2023-03-14 16:05:57.000000 beetl-0.1.1/src/beetl.egg-info/entry_points.txt
--rw-rw-r--   0 larsch    (1003) larsch    (1003)       75 2023-03-14 16:05:57.000000 beetl-0.1.1/src/beetl.egg-info/requires.txt
--rw-rw-r--   0 larsch    (1003) larsch    (1003)        6 2023-03-14 16:05:57.000000 beetl-0.1.1/src/beetl.egg-info/top_level.txt
--rw-rw-r--   0 larsch    (1003) larsch    (1003)        1 2023-03-14 10:15:51.000000 beetl-0.1.1/src/beetl.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:06:25.762860 beetl-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-15 11:06:25.762860 beetl-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-15 11:05:45.000000 beetl-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:06:25.762860 beetl-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-15 11:05:45.000000 beetl-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:06:25.750860 beetl-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:06:25.754860 beetl-0.2.1/src/beetl/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/beetl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:06:25.758860 beetl-0.2.1/src/beetl/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/sources/faker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/sources/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/sources/itop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/sources/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/sources/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/sources/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/sources/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/sources/sqlserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/sources/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:06:25.762860 beetl-0.2.1/src/beetl/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/transformers/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/transformers/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/transformers/itop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/transformers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/transformers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/transformers/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-15 11:05:45.000000 beetl-0.2.1/src/beetl/transformers/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:06:25.754860 beetl-0.2.1/src/beetl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-15 11:06:25.000000 beetl-0.2.1/src/beetl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-15 11:06:25.000000 beetl-0.2.1/src/beetl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:06:25.000000 beetl-0.2.1/src/beetl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 11:06:25.000000 beetl-0.2.1/src/beetl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-15 11:06:25.000000 beetl-0.2.1/src/beetl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 11:06:25.000000 beetl-0.2.1/src/beetl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:06:25.000000 beetl-0.2.1/src/beetl.egg-info/zip-safe
```

### Comparing `beetl-0.1.1/setup.py` & `beetl-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `beetl-0.1.1/src/beetl/__version__.py` & `beetl-0.2.1/src/beetl/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Module information."""
 import os
 
 # The title and description of the package
 __title__ = "beetl"
 __description__ = """
-    Bee ETL is a Python package for extracting data from one source, transforming it and loading it into another
+    BeETL is a Python package for extracting data from one source, transforming it and loading it into another
 """
 
 # The version and build number
 # Without specifying a unique number, you cannot overwrite packages in the PyPi repo
 __version__ = os.getenv("RELEASE_NAME", "0.1.1" + os.getenv("GITHUB_RUN_ID", ""))
 
 # Author and license information
 __author__ = "Lars Scheibling"
 __author_email__ = "lars.scheibling@hoglandet.se"
 __license__ = "GnuPG 3.0"
 
 # URL to the project
-__url__ = f"https://github.com/Hoglandets-IT/{__title__}"
+__url__ = f"https://github.com/Hoglandets-IT/{__title__}"
```

### Comparing `beetl-0.1.1/src/beetl.egg-info/SOURCES.txt` & `beetl-0.2.1/src/beetl.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 README.md
 setup.py
 src/beetl/__init__.py
 src/beetl/__version__.py
 src/beetl/beetl.py
 src/beetl/config.py
-src/beetl/sources.py
-src/beetl/transformers.py
 src/beetl.egg-info/PKG-INFO
 src/beetl.egg-info/SOURCES.txt
 src/beetl.egg-info/dependency_links.txt
 src/beetl.egg-info/entry_points.txt
 src/beetl.egg-info/requires.txt
 src/beetl.egg-info/top_level.txt
 src/beetl.egg-info/zip-safe
-src/beetl/field_transformers/__init__.py
-src/beetl/field_transformers/interface.py
-src/beetl/source_transformers/__init__.py
-src/beetl/source_transformers/interface.py
 src/beetl/sources/__init__.py
-src/beetl/sources/file.py
+src/beetl/sources/faker.py
 src/beetl/sources/interface.py
+src/beetl/sources/itop.py
+src/beetl/sources/mongodb.py
 src/beetl/sources/mysql.py
-src/beetl/sources/sqlserver.py
+src/beetl/sources/postgres.py
+src/beetl/sources/rest.py
+src/beetl/sources/sqlserver.py
+src/beetl/sources/static.py
+src/beetl/transformers/__init__.py
+src/beetl/transformers/frames.py
+src/beetl/transformers/interface.py
+src/beetl/transformers/itop.py
+src/beetl/transformers/misc.py
+src/beetl/transformers/regex.py
+src/beetl/transformers/strings.py
+src/beetl/transformers/structs.py
```

