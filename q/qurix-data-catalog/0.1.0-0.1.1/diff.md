# Comparing `tmp/qurix-data-catalog-0.1.0.tar.gz` & `tmp/qurix-data-catalog-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qurix-data-catalog-0.1.0.tar", last modified: Wed Jun 14 09:11:00 2023, max compression
+gzip compressed data, was "qurix-data-catalog-0.1.1.tar", last modified: Thu Jun 15 10:42:45 2023, max compression
```

## Comparing `qurix-data-catalog-0.1.0.tar` & `qurix-data-catalog-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:11:00.829995 qurix-data-catalog-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-06-14 09:10:51.000000 qurix-data-catalog-0.1.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-14 09:11:00.829995 qurix-data-catalog-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-14 09:10:51.000000 qurix-data-catalog-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:11:00.825995 qurix-data-catalog-0.1.0/qurix/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:11:00.825995 qurix-data-catalog-0.1.0/qurix/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:11:00.825995 qurix-data-catalog-0.1.0/qurix/data/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-14 09:10:51.000000 qurix-data-catalog-0.1.0/qurix/data/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-14 09:10:51.000000 qurix-data-catalog-0.1.0/qurix/data/catalog/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-14 09:10:51.000000 qurix-data-catalog-0.1.0/qurix/data/catalog/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:11:00.829995 qurix-data-catalog-0.1.0/qurix_data_catalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-14 09:11:00.000000 qurix-data-catalog-0.1.0/qurix_data_catalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-14 09:11:00.000000 qurix-data-catalog-0.1.0/qurix_data_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:11:00.000000 qurix-data-catalog-0.1.0/qurix_data_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-14 09:11:00.000000 qurix-data-catalog-0.1.0/qurix_data_catalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 09:11:00.000000 qurix-data-catalog-0.1.0/qurix_data_catalog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:11:00.829995 qurix-data-catalog-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-14 09:10:51.000000 qurix-data-catalog-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:11:00.829995 qurix-data-catalog-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:10:51.000000 qurix-data-catalog-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-14 09:10:51.000000 qurix-data-catalog-0.1.0/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:42:45.530789 qurix-data-catalog-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-06-15 10:42:18.000000 qurix-data-catalog-0.1.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-15 10:42:45.530789 qurix-data-catalog-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-15 10:42:18.000000 qurix-data-catalog-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:42:45.526789 qurix-data-catalog-0.1.1/qurix/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:42:45.526789 qurix-data-catalog-0.1.1/qurix/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:42:45.530789 qurix-data-catalog-0.1.1/qurix/data/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-15 10:42:18.000000 qurix-data-catalog-0.1.1/qurix/data/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-15 10:42:18.000000 qurix-data-catalog-0.1.1/qurix/data/catalog/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-15 10:42:18.000000 qurix-data-catalog-0.1.1/qurix/data/catalog/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:42:45.530789 qurix-data-catalog-0.1.1/qurix_data_catalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-15 10:42:45.000000 qurix-data-catalog-0.1.1/qurix_data_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-15 10:42:45.000000 qurix-data-catalog-0.1.1/qurix_data_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:42:45.000000 qurix-data-catalog-0.1.1/qurix_data_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-15 10:42:45.000000 qurix-data-catalog-0.1.1/qurix_data_catalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 10:42:45.000000 qurix-data-catalog-0.1.1/qurix_data_catalog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 10:42:45.530789 qurix-data-catalog-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-15 10:42:18.000000 qurix-data-catalog-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:42:45.530789 qurix-data-catalog-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:42:18.000000 qurix-data-catalog-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-15 10:42:18.000000 qurix-data-catalog-0.1.1/tests/test_client.py
```

### Comparing `qurix-data-catalog-0.1.0/LICENCE` & `qurix-data-catalog-0.1.1/LICENCE`

 * *Files identical despite different names*

