# Comparing `tmp/fastmodels-0.1.tar.gz` & `tmp/fastmodels-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastmodels-0.1.tar", last modified: Thu Jun 15 09:38:01 2023, max compression
+gzip compressed data, was "fastmodels-0.1.1.tar", last modified: Thu Jun 15 09:50:04 2023, max compression
```

## Comparing `fastmodels-0.1.tar` & `fastmodels-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 09:38:01.981246 fastmodels-0.1/
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      139 2023-06-15 09:38:01.981246 fastmodels-0.1/PKG-INFO
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      121 2023-06-15 09:26:16.000000 fastmodels-0.1/README.md
-drwxrwxr-x   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 09:38:01.981246 fastmodels-0.1/datavalidator/
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 09:01:48.000000 fastmodels-0.1/datavalidator/__init__.py
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      979 2023-06-15 09:05:15.000000 fastmodels-0.1/datavalidator/validator.py
-drwxrwxr-x   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 09:38:01.981246 fastmodels-0.1/fastmodels.egg-info/
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      139 2023-06-15 09:38:01.000000 fastmodels-0.1/fastmodels.egg-info/PKG-INFO
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      282 2023-06-15 09:38:01.000000 fastmodels-0.1/fastmodels.egg-info/SOURCES.txt
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)        1 2023-06-15 09:38:01.000000 fastmodels-0.1/fastmodels.egg-info/dependency_links.txt
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)       11 2023-06-15 09:38:01.000000 fastmodels-0.1/fastmodels.egg-info/requires.txt
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)       20 2023-06-15 09:38:01.000000 fastmodels-0.1/fastmodels.egg-info/top_level.txt
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)       38 2023-06-15 09:38:01.981246 fastmodels-0.1/setup.cfg
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      275 2023-06-15 09:26:16.000000 fastmodels-0.1/setup.py
-drwxrwxr-x   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 09:38:01.981246 fastmodels-0.1/tests/
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 09:17:25.000000 fastmodels-0.1/tests/__init__.py
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      649 2023-06-15 09:20:20.000000 fastmodels-0.1/tests/test_validator.py
+drwxrwxr-x   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 09:50:04.375805 fastmodels-0.1.1/
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      141 2023-06-15 09:50:04.371808 fastmodels-0.1.1/PKG-INFO
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      121 2023-06-15 09:26:16.000000 fastmodels-0.1.1/README.md
+drwxrwxr-x   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 09:50:04.371808 fastmodels-0.1.1/datavalidator/
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 09:01:48.000000 fastmodels-0.1.1/datavalidator/__init__.py
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      979 2023-06-15 09:05:15.000000 fastmodels-0.1.1/datavalidator/validator.py
+drwxrwxr-x   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 09:50:04.371808 fastmodels-0.1.1/fastmodels.egg-info/
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      141 2023-06-15 09:50:04.000000 fastmodels-0.1.1/fastmodels.egg-info/PKG-INFO
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      319 2023-06-15 09:50:04.000000 fastmodels-0.1.1/fastmodels.egg-info/SOURCES.txt
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)        1 2023-06-15 09:50:04.000000 fastmodels-0.1.1/fastmodels.egg-info/dependency_links.txt
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)       51 2023-06-15 09:50:04.000000 fastmodels-0.1.1/fastmodels.egg-info/entry_points.txt
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)       11 2023-06-15 09:50:04.000000 fastmodels-0.1.1/fastmodels.egg-info/requires.txt
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)       20 2023-06-15 09:50:04.000000 fastmodels-0.1.1/fastmodels.egg-info/top_level.txt
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)       38 2023-06-15 09:50:04.375805 fastmodels-0.1.1/setup.cfg
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      389 2023-06-15 09:49:46.000000 fastmodels-0.1.1/setup.py
+drwxrwxr-x   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 09:50:04.371808 fastmodels-0.1.1/tests/
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 09:17:25.000000 fastmodels-0.1.1/tests/__init__.py
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      649 2023-06-15 09:20:20.000000 fastmodels-0.1.1/tests/test_validator.py
```

### Comparing `fastmodels-0.1/datavalidator/validator.py` & `fastmodels-0.1.1/datavalidator/validator.py`

 * *Files identical despite different names*

### Comparing `fastmodels-0.1/tests/test_validator.py` & `fastmodels-0.1.1/tests/test_validator.py`

 * *Files identical despite different names*

