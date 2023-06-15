# Comparing `tmp/xmlrecords-0.3.0.tar.gz` & `tmp/xmlrecords-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmlrecords-0.3.0.tar", last modified: Thu Jun 15 11:50:12 2023, max compression
+gzip compressed data, was "xmlrecords-0.3.1.tar", last modified: Thu Jun 15 12:17:33 2023, max compression
```

## Comparing `xmlrecords-0.3.0.tar` & `xmlrecords-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:50:12.345069 xmlrecords-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 11:50:01.000000 xmlrecords-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-15 11:50:12.345069 xmlrecords-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-15 11:50:01.000000 xmlrecords-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-15 11:50:01.000000 xmlrecords-0.3.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1049 2023-06-15 11:50:12.345069 xmlrecords-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-15 11:50:01.000000 xmlrecords-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:50:12.341069 xmlrecords-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:50:01.000000 xmlrecords-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-06-15 11:50:01.000000 xmlrecords-0.3.0/tests/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:50:12.341069 xmlrecords-0.3.0/xmlrecords/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-15 11:50:01.000000 xmlrecords-0.3.0/xmlrecords/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:50:12.345069 xmlrecords-0.3.0/xmlrecords/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:50:01.000000 xmlrecords-0.3.0/xmlrecords/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-06-15 11:50:01.000000 xmlrecords-0.3.0/xmlrecords/src/xmlrecords.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:50:12.345069 xmlrecords-0.3.0/xmlrecords.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-15 11:50:12.000000 xmlrecords-0.3.0/xmlrecords.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-15 11:50:12.000000 xmlrecords-0.3.0/xmlrecords.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:50:12.000000 xmlrecords-0.3.0/xmlrecords.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 11:50:12.000000 xmlrecords-0.3.0/xmlrecords.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 11:50:12.000000 xmlrecords-0.3.0/xmlrecords.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:17:33.631604 xmlrecords-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 12:17:13.000000 xmlrecords-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-15 12:17:33.631604 xmlrecords-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-15 12:17:13.000000 xmlrecords-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-15 12:17:13.000000 xmlrecords-0.3.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1049 2023-06-15 12:17:33.631604 xmlrecords-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-15 12:17:13.000000 xmlrecords-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:17:33.631604 xmlrecords-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 12:17:13.000000 xmlrecords-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-06-15 12:17:13.000000 xmlrecords-0.3.1/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:17:33.631604 xmlrecords-0.3.1/xmlrecords/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-15 12:17:13.000000 xmlrecords-0.3.1/xmlrecords/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:17:33.631604 xmlrecords-0.3.1/xmlrecords/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 12:17:13.000000 xmlrecords-0.3.1/xmlrecords/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-06-15 12:17:13.000000 xmlrecords-0.3.1/xmlrecords/src/xmlrecords.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:17:33.631604 xmlrecords-0.3.1/xmlrecords.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-15 12:17:33.000000 xmlrecords-0.3.1/xmlrecords.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-15 12:17:33.000000 xmlrecords-0.3.1/xmlrecords.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:17:33.000000 xmlrecords-0.3.1/xmlrecords.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 12:17:33.000000 xmlrecords-0.3.1/xmlrecords.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 12:17:33.000000 xmlrecords-0.3.1/xmlrecords.egg-info/top_level.txt
```

### Comparing `xmlrecords-0.3.0/LICENSE` & `xmlrecords-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xmlrecords-0.3.0/PKG-INFO` & `xmlrecords-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlrecords
-Version: 0.3.0
+Version: 0.3.1
 Summary: This package can convert an XML files to a list of records
 Home-page: UNKNOWN
 Author: Yaroslav Kopotilov
 Author-email: datascience@tuta.io
 License: Apache License, Version 2.0
 Description: # XML Records
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xmlrecords Version: 0.3.0 Summary: This package can
+Metadata-Version: 2.1 Name: xmlrecords Version: 0.3.1 Summary: This package can
 convert an XML files to a list of records Home-page: UNKNOWN Author: Yaroslav
 Kopotilov Author-email: datascience@tuta.io License: Apache License, Version
 2.0 Description: # XML Records `xmlrecords` is a user-friendly wrapper of
 `lxml` package for extraction of tabular data from XML files. >>> This data
 provider sends all his data in... XML. You know nothing about XML, except that
 it looks kind of weird and you would *definitely* never use it for tabular
 data. How could you just transform all this XML nightmare into a sensible
```

### Comparing `xmlrecords-0.3.0/README.md` & `xmlrecords-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `xmlrecords-0.3.0/pyproject.toml` & `xmlrecords-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xmlrecords-0.3.0/setup.cfg` & `xmlrecords-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `xmlrecords-0.3.0/tests/test_core.py` & `xmlrecords-0.3.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `xmlrecords-0.3.0/xmlrecords/src/xmlrecords.py` & `xmlrecords-0.3.1/xmlrecords/src/xmlrecords.py`

 * *Files identical despite different names*

### Comparing `xmlrecords-0.3.0/xmlrecords.egg-info/PKG-INFO` & `xmlrecords-0.3.1/xmlrecords.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlrecords
-Version: 0.3.0
+Version: 0.3.1
 Summary: This package can convert an XML files to a list of records
 Home-page: UNKNOWN
 Author: Yaroslav Kopotilov
 Author-email: datascience@tuta.io
 License: Apache License, Version 2.0
 Description: # XML Records
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xmlrecords Version: 0.3.0 Summary: This package can
+Metadata-Version: 2.1 Name: xmlrecords Version: 0.3.1 Summary: This package can
 convert an XML files to a list of records Home-page: UNKNOWN Author: Yaroslav
 Kopotilov Author-email: datascience@tuta.io License: Apache License, Version
 2.0 Description: # XML Records `xmlrecords` is a user-friendly wrapper of
 `lxml` package for extraction of tabular data from XML files. >>> This data
 provider sends all his data in... XML. You know nothing about XML, except that
 it looks kind of weird and you would *definitely* never use it for tabular
 data. How could you just transform all this XML nightmare into a sensible
```

