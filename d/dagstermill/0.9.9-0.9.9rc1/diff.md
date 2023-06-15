# Comparing `tmp/dagstermill-0.9.9.tar.gz` & `tmp/dagstermill-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagstermill-0.9.9.tar", last modified: Thu Sep 17 21:28:23 2020, max compression
+gzip compressed data, was "dist/dagstermill-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:42 2020, max compression
```

## Comparing `dagstermill-0.9.9.tar` & `dagstermill-0.9.9rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:23.000000 dagstermill-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:24:45.000000 dagstermill-0.9.9/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       16 2020-09-17 21:24:45.000000 dagstermill-0.9.9/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      510 2020-09-17 21:28:23.000000 dagstermill-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      119 2020-09-17 21:24:45.000000 dagstermill-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:23.000000 dagstermill-0.9.9/dagstermill/
--rw-r--r--   0 bobchen    (501) staff       (20)      796 2020-09-17 21:24:45.000000 dagstermill-0.9.9/dagstermill/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)       30 2020-09-17 21:24:45.000000 dagstermill-0.9.9/dagstermill/__main__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4514 2020-09-17 21:24:45.000000 dagstermill-0.9.9/dagstermill/cli.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4189 2020-09-17 21:24:45.000000 dagstermill-0.9.9/dagstermill/context.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2554 2020-09-17 21:24:45.000000 dagstermill-0.9.9/dagstermill/engine.py
--rw-r--r--   0 bobchen    (501) staff       (20)      323 2020-09-17 21:24:45.000000 dagstermill-0.9.9/dagstermill/errors.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:23.000000 dagstermill-0.9.9/dagstermill/examples/
--rw-r--r--   0 bobchen    (501) staff       (20)       38 2020-09-17 21:24:45.000000 dagstermill-0.9.9/dagstermill/examples/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    12664 2020-09-17 21:24:45.000000 dagstermill-0.9.9/dagstermill/examples/repository.py
--rw-r--r--   0 bobchen    (501) staff       (20)    12003 2020-09-17 21:24:45.000000 dagstermill-0.9.9/dagstermill/manager.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1307 2020-09-17 21:24:45.000000 dagstermill-0.9.9/dagstermill/serialize.py
--rw-r--r--   0 bobchen    (501) staff       (20)    14021 2020-09-17 21:24:45.000000 dagstermill-0.9.9/dagstermill/solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2026 2020-09-17 21:24:45.000000 dagstermill-0.9.9/dagstermill/translator.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagstermill-0.9.9/dagstermill/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:23.000000 dagstermill-0.9.9/dagstermill.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      510 2020-09-17 21:28:23.000000 dagstermill-0.9.9/dagstermill.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      581 2020-09-17 21:28:23.000000 dagstermill-0.9.9/dagstermill.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:23.000000 dagstermill-0.9.9/dagstermill.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       54 2020-09-17 21:28:23.000000 dagstermill-0.9.9/dagstermill.egg-info/entry_points.txt
--rw-r--r--   0 bobchen    (501) staff       (20)      102 2020-09-17 21:28:23.000000 dagstermill-0.9.9/dagstermill.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       12 2020-09-17 21:28:23.000000 dagstermill-0.9.9/dagstermill.egg-info/top_level.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:28:23.000000 dagstermill-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1163 2020-09-17 21:24:45.000000 dagstermill-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/LICENSE
+-rw-r--r--   0 bobchen    (501) staff       (20)       16 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/MANIFEST.in
+-rw-r--r--   0 bobchen    (501) staff       (20)      513 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      119 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/dagstermill/
+-rw-r--r--   0 bobchen    (501) staff       (20)      796 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       30 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/__main__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     4514 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/cli.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     4189 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/context.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2554 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/engine.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      323 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/errors.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/dagstermill/examples/
+-rw-r--r--   0 bobchen    (501) staff       (20)       38 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/examples/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    12664 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/examples/repository.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    12003 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/manager.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1307 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/serialize.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    14021 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/solids.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2026 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/translator.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/dagstermill/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/dagstermill.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      513 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/dagstermill.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      581 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/dagstermill.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/dagstermill.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       54 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/dagstermill.egg-info/entry_points.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)      102 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/dagstermill.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       12 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/dagstermill.egg-info/top_level.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:42.000000 dagstermill-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1163 2020-09-17 21:04:59.000000 dagstermill-0.9.9rc1/setup.py
```

### Comparing `dagstermill-0.9.9/LICENSE` & `dagstermill-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagstermill-0.9.9/dagstermill/__init__.py` & `dagstermill-0.9.9rc1/dagstermill/__init__.py`

 * *Files identical despite different names*

### Comparing `dagstermill-0.9.9/dagstermill/cli.py` & `dagstermill-0.9.9rc1/dagstermill/cli.py`

 * *Files identical despite different names*

### Comparing `dagstermill-0.9.9/dagstermill/context.py` & `dagstermill-0.9.9rc1/dagstermill/context.py`

 * *Files identical despite different names*

### Comparing `dagstermill-0.9.9/dagstermill/engine.py` & `dagstermill-0.9.9rc1/dagstermill/engine.py`

 * *Files identical despite different names*

### Comparing `dagstermill-0.9.9/dagstermill/examples/repository.py` & `dagstermill-0.9.9rc1/dagstermill/examples/repository.py`

 * *Files identical despite different names*

### Comparing `dagstermill-0.9.9/dagstermill/manager.py` & `dagstermill-0.9.9rc1/dagstermill/manager.py`

 * *Files identical despite different names*

### Comparing `dagstermill-0.9.9/dagstermill/serialize.py` & `dagstermill-0.9.9rc1/dagstermill/serialize.py`

 * *Files identical despite different names*

### Comparing `dagstermill-0.9.9/dagstermill/solids.py` & `dagstermill-0.9.9rc1/dagstermill/solids.py`

 * *Files identical despite different names*

### Comparing `dagstermill-0.9.9/dagstermill/translator.py` & `dagstermill-0.9.9rc1/dagstermill/translator.py`

 * *Files identical despite different names*

### Comparing `dagstermill-0.9.9/dagstermill.egg-info/SOURCES.txt` & `dagstermill-0.9.9rc1/dagstermill.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagstermill-0.9.9/setup.py` & `dagstermill-0.9.9rc1/setup.py`

 * *Files identical despite different names*

