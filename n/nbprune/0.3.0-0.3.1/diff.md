# Comparing `tmp/nbprune-0.3.0.tar.gz` & `tmp/nbprune-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbprune-0.3.0.tar", last modified: Mon Jan  9 15:55:51 2023, max compression
+gzip compressed data, was "nbprune-0.3.1.tar", last modified: Thu Jun 15 09:53:47 2023, max compression
```

## Comparing `nbprune-0.3.0.tar` & `nbprune-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-01-09 15:55:51.596778 nbprune-0.3.0/
--rw-r--r--   0 tparment (15010) diana    (200036)     2488 2023-01-09 15:55:51.596539 nbprune-0.3.0/PKG-INFO
--rw-r--r--   0 tparment (15010) diana    (200036)     2142 2022-06-07 10:12:58.000000 nbprune-0.3.0/README.md
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-01-09 15:55:51.593026 nbprune-0.3.0/nbprune/
--rw-r--r--   0 tparment (15010) diana    (200036)       32 2022-06-07 12:32:54.000000 nbprune-0.3.0/nbprune/__init__.py
--rwxr-xr-x   0 tparment (15010) diana    (200036)     8703 2023-01-09 11:30:53.000000 nbprune-0.3.0/nbprune/nbprune.py
--rw-r--r--   0 tparment (15010) diana    (200036)       22 2023-01-09 15:54:28.000000 nbprune-0.3.0/nbprune/version.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-01-09 15:55:51.596161 nbprune-0.3.0/nbprune.egg-info/
--rw-r--r--   0 tparment (15010) diana    (200036)     2488 2023-01-09 15:55:51.000000 nbprune-0.3.0/nbprune.egg-info/PKG-INFO
--rw-r--r--   0 tparment (15010) diana    (200036)      294 2023-01-09 15:55:51.000000 nbprune-0.3.0/nbprune.egg-info/SOURCES.txt
--rw-r--r--   0 tparment (15010) diana    (200036)        1 2023-01-09 15:55:51.000000 nbprune-0.3.0/nbprune.egg-info/dependency_links.txt
--rw-r--r--   0 tparment (15010) diana    (200036)       49 2023-01-09 15:55:51.000000 nbprune-0.3.0/nbprune.egg-info/entry_points.txt
--rw-r--r--   0 tparment (15010) diana    (200036)        1 2022-06-07 12:33:11.000000 nbprune-0.3.0/nbprune.egg-info/not-zip-safe
--rw-r--r--   0 tparment (15010) diana    (200036)        9 2023-01-09 15:55:51.000000 nbprune-0.3.0/nbprune.egg-info/requires.txt
--rw-r--r--   0 tparment (15010) diana    (200036)        8 2023-01-09 15:55:51.000000 nbprune-0.3.0/nbprune.egg-info/top_level.txt
--rw-r--r--   0 tparment (15010) diana    (200036)       38 2023-01-09 15:55:51.596856 nbprune-0.3.0/setup.cfg
--rwxr-xr-x   0 tparment (15010) diana    (200036)     1534 2022-06-07 12:28:54.000000 nbprune-0.3.0/setup.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-06-15 09:53:47.126527 nbprune-0.3.1/
+-rw-r--r--   0 tparment (15010) diana    (200036)     2488 2023-06-15 09:53:47.126204 nbprune-0.3.1/PKG-INFO
+-rw-r--r--   0 tparment (15010) diana    (200036)     2142 2022-06-07 10:12:58.000000 nbprune-0.3.1/README.md
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-06-15 09:53:47.123000 nbprune-0.3.1/nbprune/
+-rw-r--r--   0 tparment (15010) diana    (200036)       32 2022-06-07 12:32:54.000000 nbprune-0.3.1/nbprune/__init__.py
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     8734 2023-01-13 16:24:29.000000 nbprune-0.3.1/nbprune/nbprune.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       22 2023-01-13 16:27:45.000000 nbprune-0.3.1/nbprune/version.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-06-15 09:53:47.125769 nbprune-0.3.1/nbprune.egg-info/
+-rw-r--r--   0 tparment (15010) diana    (200036)     2488 2023-06-15 09:53:47.000000 nbprune-0.3.1/nbprune.egg-info/PKG-INFO
+-rw-r--r--   0 tparment (15010) diana    (200036)      294 2023-06-15 09:53:47.000000 nbprune-0.3.1/nbprune.egg-info/SOURCES.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)        1 2023-06-15 09:53:47.000000 nbprune-0.3.1/nbprune.egg-info/dependency_links.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)       49 2023-06-15 09:53:47.000000 nbprune-0.3.1/nbprune.egg-info/entry_points.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)        1 2022-06-07 12:33:11.000000 nbprune-0.3.1/nbprune.egg-info/not-zip-safe
+-rw-r--r--   0 tparment (15010) diana    (200036)        9 2023-06-15 09:53:47.000000 nbprune-0.3.1/nbprune.egg-info/requires.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)        8 2023-06-15 09:53:47.000000 nbprune-0.3.1/nbprune.egg-info/top_level.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)       38 2023-06-15 09:53:47.126632 nbprune-0.3.1/setup.cfg
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     1534 2022-06-07 12:28:54.000000 nbprune-0.3.1/setup.py
```

### Comparing `nbprune-0.3.0/PKG-INFO` & `nbprune-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbprune
-Version: 0.3.0
+Version: 0.3.1
 Summary: With this tool, one can define pieces of a notebook that belong to teachers and should not be exposed to students.
 Author: Thierry Parmentelat
 Author-email: thierry.parmentelat@inria.fr
 Project-URL: source, https://github.com/flotpython/nbprune
 Description-Content-Type: text/markdown
 
 # nbprune
```

### Comparing `nbprune-0.3.0/README.md` & `nbprune-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nbprune-0.3.0/nbprune/nbprune.py` & `nbprune-0.3.1/nbprune/nbprune.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,16 @@
             verbose(f"{solution} -> ", end='')
             print(student)
         return 0
 
     for solution, student in zip(solutions, students):
         if not student:
             verbose(f"ignoring {solution} - does not comply with naming conventions")
-            retcod = 1
+            # not a big deal
+            # retcod = 1
             continue
 
         p1, p2 = Path(solution), Path(student)
         if not p1.exists():
             print(f"{p1} not found")
             retcod = 1
             continue
```

### Comparing `nbprune-0.3.0/nbprune.egg-info/PKG-INFO` & `nbprune-0.3.1/nbprune.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbprune
-Version: 0.3.0
+Version: 0.3.1
 Summary: With this tool, one can define pieces of a notebook that belong to teachers and should not be exposed to students.
 Author: Thierry Parmentelat
 Author-email: thierry.parmentelat@inria.fr
 Project-URL: source, https://github.com/flotpython/nbprune
 Description-Content-Type: text/markdown
 
 # nbprune
```

### Comparing `nbprune-0.3.0/setup.py` & `nbprune-0.3.1/setup.py`

 * *Files identical despite different names*

