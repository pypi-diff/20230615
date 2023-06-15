# Comparing `tmp/filewiz-1.1.1.tar.gz` & `tmp/filewiz-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filewiz-1.1.1.tar", last modified: Thu Jun 15 16:10:17 2023, max compression
+gzip compressed data, was "filewiz-1.1.2.tar", last modified: Thu Jun 15 16:18:41 2023, max compression
```

## Comparing `filewiz-1.1.1.tar` & `filewiz-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-15 16:10:17.484603 filewiz-1.1.1/
--rw-r--r--   0 francispotter   (501) staff       (20)     1873 2023-06-15 16:10:17.484068 filewiz-1.1.1/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)     1618 2023-04-10 05:40:23.000000 filewiz-1.1.1/README.md
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-15 16:10:17.436049 filewiz-1.1.1/filewiz/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-06-15 00:15:58.000000 filewiz-1.1.1/filewiz/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)       74 2023-04-10 05:20:07.000000 filewiz-1.1.1/filewiz/__main__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      935 2023-06-15 00:15:58.000000 filewiz-1.1.1/filewiz/_watchdog.py
--rw-r--r--   0 francispotter   (501) staff       (20)      725 2023-06-15 00:15:58.000000 filewiz-1.1.1/filewiz/directory_scanner.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2365 2023-06-15 00:15:58.000000 filewiz-1.1.1/filewiz/file_mover.py
--rw-r--r--   0 francispotter   (501) staff       (20)      522 2023-06-15 00:15:58.000000 filewiz-1.1.1/filewiz/handler.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1283 2023-04-05 00:32:38.000000 filewiz-1.1.1/filewiz/readline_util.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-15 16:10:17.483422 filewiz-1.1.1/filewiz.egg-info/
--rw-r--r--   0 francispotter   (501) staff       (20)     1873 2023-06-15 16:10:17.000000 filewiz-1.1.1/filewiz.egg-info/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)      376 2023-06-15 16:10:17.000000 filewiz-1.1.1/filewiz.egg-info/SOURCES.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-06-15 16:10:17.000000 filewiz-1.1.1/filewiz.egg-info/dependency_links.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       49 2023-06-15 16:10:17.000000 filewiz-1.1.1/filewiz.egg-info/entry_points.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       28 2023-06-15 16:10:17.000000 filewiz-1.1.1/filewiz.egg-info/requires.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        8 2023-06-15 16:10:17.000000 filewiz-1.1.1/filewiz.egg-info/top_level.txt
--rw-r--r--   0 francispotter   (501) staff       (20)      584 2023-06-15 16:08:45.000000 filewiz-1.1.1/pyproject.toml
--rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-06-15 16:10:17.484742 filewiz-1.1.1/setup.cfg
--rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-06-15 16:09:17.000000 filewiz-1.1.1/version
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-15 16:18:41.223183 filewiz-1.1.2/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1873 2023-06-15 16:18:41.207730 filewiz-1.1.2/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)     1618 2023-04-10 05:40:23.000000 filewiz-1.1.2/README.md
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-15 16:18:41.142317 filewiz-1.1.2/filewiz/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-06-15 00:15:58.000000 filewiz-1.1.2/filewiz/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)       74 2023-04-10 05:20:07.000000 filewiz-1.1.2/filewiz/__main__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      935 2023-06-15 00:15:58.000000 filewiz-1.1.2/filewiz/_watchdog.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      725 2023-06-15 00:15:58.000000 filewiz-1.1.2/filewiz/directory_scanner.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2365 2023-06-15 00:15:58.000000 filewiz-1.1.2/filewiz/file_mover.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      522 2023-06-15 00:15:58.000000 filewiz-1.1.2/filewiz/handler.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1283 2023-04-05 00:32:38.000000 filewiz-1.1.2/filewiz/readline_util.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-15 16:18:41.206437 filewiz-1.1.2/filewiz.egg-info/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1873 2023-06-15 16:18:40.000000 filewiz-1.1.2/filewiz.egg-info/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)      376 2023-06-15 16:18:40.000000 filewiz-1.1.2/filewiz.egg-info/SOURCES.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-06-15 16:18:40.000000 filewiz-1.1.2/filewiz.egg-info/dependency_links.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       49 2023-06-15 16:18:40.000000 filewiz-1.1.2/filewiz.egg-info/entry_points.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       30 2023-06-15 16:18:40.000000 filewiz-1.1.2/filewiz.egg-info/requires.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        8 2023-06-15 16:18:40.000000 filewiz-1.1.2/filewiz.egg-info/top_level.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)      586 2023-06-15 16:17:01.000000 filewiz-1.1.2/pyproject.toml
+-rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-06-15 16:18:41.223354 filewiz-1.1.2/setup.cfg
+-rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-06-15 16:17:08.000000 filewiz-1.1.2/version
```

### Comparing `filewiz-1.1.1/PKG-INFO` & `filewiz-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filewiz
-Version: 1.1.1
+Version: 1.1.2
 Summary: Quickly rename and move new files into structured folders
 Author-email: Francis Potter <filewiz@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 
 # FileWiz
```

### Comparing `filewiz-1.1.1/README.md` & `filewiz-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `filewiz-1.1.1/filewiz/_watchdog.py` & `filewiz-1.1.2/filewiz/_watchdog.py`

 * *Files identical despite different names*

### Comparing `filewiz-1.1.1/filewiz/directory_scanner.py` & `filewiz-1.1.2/filewiz/directory_scanner.py`

 * *Files identical despite different names*

### Comparing `filewiz-1.1.1/filewiz/file_mover.py` & `filewiz-1.1.2/filewiz/file_mover.py`

 * *Files identical despite different names*

### Comparing `filewiz-1.1.1/filewiz/handler.py` & `filewiz-1.1.2/filewiz/handler.py`

 * *Files identical despite different names*

### Comparing `filewiz-1.1.1/filewiz/readline_util.py` & `filewiz-1.1.2/filewiz/readline_util.py`

 * *Files identical despite different names*

### Comparing `filewiz-1.1.1/filewiz.egg-info/PKG-INFO` & `filewiz-1.1.2/filewiz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filewiz
-Version: 1.1.1
+Version: 1.1.2
 Summary: Quickly rename and move new files into structured folders
 Author-email: Francis Potter <filewiz@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 
 # FileWiz
```

### Comparing `filewiz-1.1.1/pyproject.toml` & `filewiz-1.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ]
 description = "Quickly rename and move new files into structured folders"
 readme = "README.md"
 requires-python = ">=3.6.5"
 license = {text = "MIT"}
 dependencies = [
     "wizlib >=0.2.3",
-    "vernum >=2.2.2"
+    "watchdog >=3.0.0"
 ]
 dynamic = ["version"]
 
 [tool.setuptools.package-dir]
 filewiz = "filewiz"
 
 [project.scripts]
```

