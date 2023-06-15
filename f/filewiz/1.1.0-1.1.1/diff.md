# Comparing `tmp/filewiz-1.1.0.tar.gz` & `tmp/filewiz-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filewiz-1.1.0.tar", last modified: Thu Jun 15 00:21:04 2023, max compression
+gzip compressed data, was "filewiz-1.1.1.tar", last modified: Thu Jun 15 16:10:17 2023, max compression
```

## Comparing `filewiz-1.1.0.tar` & `filewiz-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-15 00:21:04.097095 filewiz-1.1.0/
--rw-r--r--   0 francispotter   (501) staff       (20)     1873 2023-06-15 00:21:04.096248 filewiz-1.1.0/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)     1618 2023-04-10 05:40:23.000000 filewiz-1.1.0/README.md
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-15 00:21:03.956085 filewiz-1.1.0/filewiz/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-06-15 00:15:58.000000 filewiz-1.1.0/filewiz/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)       74 2023-04-10 05:20:07.000000 filewiz-1.1.0/filewiz/__main__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      935 2023-06-15 00:15:58.000000 filewiz-1.1.0/filewiz/_watchdog.py
--rw-r--r--   0 francispotter   (501) staff       (20)      725 2023-06-15 00:15:58.000000 filewiz-1.1.0/filewiz/directory_scanner.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2365 2023-06-15 00:15:58.000000 filewiz-1.1.0/filewiz/file_mover.py
--rw-r--r--   0 francispotter   (501) staff       (20)      522 2023-06-15 00:15:58.000000 filewiz-1.1.0/filewiz/handler.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1283 2023-04-05 00:32:38.000000 filewiz-1.1.0/filewiz/readline_util.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-15 00:21:04.095389 filewiz-1.1.0/filewiz.egg-info/
--rw-r--r--   0 francispotter   (501) staff       (20)     1873 2023-06-15 00:21:03.000000 filewiz-1.1.0/filewiz.egg-info/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)      376 2023-06-15 00:21:03.000000 filewiz-1.1.0/filewiz.egg-info/SOURCES.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-06-15 00:21:03.000000 filewiz-1.1.0/filewiz.egg-info/dependency_links.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       49 2023-06-15 00:21:03.000000 filewiz-1.1.0/filewiz.egg-info/entry_points.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       14 2023-06-15 00:21:03.000000 filewiz-1.1.0/filewiz.egg-info/requires.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        8 2023-06-15 00:21:03.000000 filewiz-1.1.0/filewiz.egg-info/top_level.txt
--rw-r--r--   0 francispotter   (501) staff       (20)      562 2023-04-22 17:30:53.000000 filewiz-1.1.0/pyproject.toml
--rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-06-15 00:21:04.097300 filewiz-1.1.0/setup.cfg
--rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-06-15 00:20:15.000000 filewiz-1.1.0/version
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-15 16:10:17.484603 filewiz-1.1.1/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1873 2023-06-15 16:10:17.484068 filewiz-1.1.1/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)     1618 2023-04-10 05:40:23.000000 filewiz-1.1.1/README.md
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-15 16:10:17.436049 filewiz-1.1.1/filewiz/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-06-15 00:15:58.000000 filewiz-1.1.1/filewiz/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)       74 2023-04-10 05:20:07.000000 filewiz-1.1.1/filewiz/__main__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      935 2023-06-15 00:15:58.000000 filewiz-1.1.1/filewiz/_watchdog.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      725 2023-06-15 00:15:58.000000 filewiz-1.1.1/filewiz/directory_scanner.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2365 2023-06-15 00:15:58.000000 filewiz-1.1.1/filewiz/file_mover.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      522 2023-06-15 00:15:58.000000 filewiz-1.1.1/filewiz/handler.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1283 2023-04-05 00:32:38.000000 filewiz-1.1.1/filewiz/readline_util.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-15 16:10:17.483422 filewiz-1.1.1/filewiz.egg-info/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1873 2023-06-15 16:10:17.000000 filewiz-1.1.1/filewiz.egg-info/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)      376 2023-06-15 16:10:17.000000 filewiz-1.1.1/filewiz.egg-info/SOURCES.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-06-15 16:10:17.000000 filewiz-1.1.1/filewiz.egg-info/dependency_links.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       49 2023-06-15 16:10:17.000000 filewiz-1.1.1/filewiz.egg-info/entry_points.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       28 2023-06-15 16:10:17.000000 filewiz-1.1.1/filewiz.egg-info/requires.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        8 2023-06-15 16:10:17.000000 filewiz-1.1.1/filewiz.egg-info/top_level.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)      584 2023-06-15 16:08:45.000000 filewiz-1.1.1/pyproject.toml
+-rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-06-15 16:10:17.484742 filewiz-1.1.1/setup.cfg
+-rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-06-15 16:09:17.000000 filewiz-1.1.1/version
```

### Comparing `filewiz-1.1.0/PKG-INFO` & `filewiz-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filewiz
-Version: 1.1.0
+Version: 1.1.1
 Summary: Quickly rename and move new files into structured folders
 Author-email: Francis Potter <filewiz@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 
 # FileWiz
```

### Comparing `filewiz-1.1.0/README.md` & `filewiz-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `filewiz-1.1.0/filewiz/_watchdog.py` & `filewiz-1.1.1/filewiz/_watchdog.py`

 * *Files identical despite different names*

### Comparing `filewiz-1.1.0/filewiz/directory_scanner.py` & `filewiz-1.1.1/filewiz/directory_scanner.py`

 * *Files identical despite different names*

### Comparing `filewiz-1.1.0/filewiz/file_mover.py` & `filewiz-1.1.1/filewiz/file_mover.py`

 * *Files identical despite different names*

### Comparing `filewiz-1.1.0/filewiz/handler.py` & `filewiz-1.1.1/filewiz/handler.py`

 * *Files identical despite different names*

### Comparing `filewiz-1.1.0/filewiz/readline_util.py` & `filewiz-1.1.1/filewiz/readline_util.py`

 * *Files identical despite different names*

### Comparing `filewiz-1.1.0/filewiz.egg-info/PKG-INFO` & `filewiz-1.1.1/filewiz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filewiz
-Version: 1.1.0
+Version: 1.1.1
 Summary: Quickly rename and move new files into structured folders
 Author-email: Francis Potter <filewiz@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 
 # FileWiz
```

