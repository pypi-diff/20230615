# Comparing `tmp/mtmtool-1.2.4.tar.gz` & `tmp/mtmtool-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtmtool-1.2.4.tar", last modified: Mon May  1 08:42:10 2023, max compression
+gzip compressed data, was "mtmtool-1.2.5.tar", last modified: Thu Jun 15 07:07:12 2023, max compression
```

## Comparing `mtmtool-1.2.4.tar` & `mtmtool-1.2.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 08:42:10.429465 mtmtool-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (122)    11324 2023-05-01 08:41:56.000000 mtmtool-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-05-01 08:41:56.000000 mtmtool-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-05-01 08:42:10.429465 mtmtool-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-05-01 08:41:56.000000 mtmtool-1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-01 08:42:10.429465 mtmtool-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2026 2023-05-01 08:41:56.000000 mtmtool-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 08:42:10.425464 mtmtool-1.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 08:42:10.429465 mtmtool-1.2.4/src/mtmtool/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 08:41:56.000000 mtmtool-1.2.4/src/mtmtool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      685 2023-05-01 08:41:56.000000 mtmtool-1.2.4/src/mtmtool/functool.py
--rw-r--r--   0 runner    (1001) docker     (122)     1687 2023-05-01 08:41:56.000000 mtmtool-1.2.4/src/mtmtool/io.py
--rw-r--r--   0 runner    (1001) docker     (122)      436 2023-05-01 08:41:56.000000 mtmtool-1.2.4/src/mtmtool/itertools.py
--rw-r--r--   0 runner    (1001) docker     (122)     2097 2023-05-01 08:41:56.000000 mtmtool-1.2.4/src/mtmtool/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     2448 2023-05-01 08:41:56.000000 mtmtool-1.2.4/src/mtmtool/pool.py
--rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-05-01 08:41:56.000000 mtmtool-1.2.4/src/mtmtool/projection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1540 2023-05-01 08:41:56.000000 mtmtool-1.2.4/src/mtmtool/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     2393 2023-05-01 08:41:56.000000 mtmtool-1.2.4/src/mtmtool/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 08:42:10.429465 mtmtool-1.2.4/src/mtmtool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-05-01 08:42:10.000000 mtmtool-1.2.4/src/mtmtool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-01 08:42:10.000000 mtmtool-1.2.4/src/mtmtool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 08:42:10.000000 mtmtool-1.2.4/src/mtmtool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 08:42:10.000000 mtmtool-1.2.4/src/mtmtool.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-01 08:42:10.000000 mtmtool-1.2.4/src/mtmtool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-01 08:42:10.000000 mtmtool-1.2.4/src/mtmtool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 08:42:10.429465 mtmtool-1.2.4/test/
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-05-01 08:41:56.000000 mtmtool-1.2.4/test/test_args2kwargs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 07:07:12.093884 mtmtool-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (122)    11324 2023-06-15 07:07:02.000000 mtmtool-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-06-15 07:07:02.000000 mtmtool-1.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-15 07:07:12.089884 mtmtool-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-06-15 07:07:02.000000 mtmtool-1.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-15 07:07:12.093884 mtmtool-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2026 2023-06-15 07:07:02.000000 mtmtool-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 07:07:12.089884 mtmtool-1.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 07:07:12.089884 mtmtool-1.2.5/src/mtmtool/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 07:07:02.000000 mtmtool-1.2.5/src/mtmtool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-06-15 07:07:02.000000 mtmtool-1.2.5/src/mtmtool/functool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1687 2023-06-15 07:07:02.000000 mtmtool-1.2.5/src/mtmtool/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)      436 2023-06-15 07:07:02.000000 mtmtool-1.2.5/src/mtmtool/itertools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2097 2023-06-15 07:07:02.000000 mtmtool-1.2.5/src/mtmtool/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2448 2023-06-15 07:07:02.000000 mtmtool-1.2.5/src/mtmtool/pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-06-15 07:07:02.000000 mtmtool-1.2.5/src/mtmtool/projection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1540 2023-06-15 07:07:02.000000 mtmtool-1.2.5/src/mtmtool/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2393 2023-06-15 07:07:02.000000 mtmtool-1.2.5/src/mtmtool/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 07:07:12.089884 mtmtool-1.2.5/src/mtmtool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-15 07:07:12.000000 mtmtool-1.2.5/src/mtmtool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-06-15 07:07:12.000000 mtmtool-1.2.5/src/mtmtool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 07:07:12.000000 mtmtool-1.2.5/src/mtmtool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 07:07:11.000000 mtmtool-1.2.5/src/mtmtool.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-15 07:07:12.000000 mtmtool-1.2.5/src/mtmtool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-15 07:07:12.000000 mtmtool-1.2.5/src/mtmtool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 07:07:12.089884 mtmtool-1.2.5/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-06-15 07:07:02.000000 mtmtool-1.2.5/test/test_args2kwargs.py
```

### Comparing `mtmtool-1.2.4/LICENSE` & `mtmtool-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.4/PKG-INFO` & `mtmtool-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmtool
-Version: 1.2.4
+Version: 1.2.5
 Summary:  A Personal Python Tool Library.
 Home-page: https://github.com/imutum/imutum_python_tool
 Author: imutum
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
```

### Comparing `mtmtool-1.2.4/setup.py` & `mtmtool-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os, shutil, sys, glob
 
 package_name = "imutum_python_tool"
 abbreviation_name = "mtmtool"
 description = " A Personal Python Tool Library."
-version = "1.2.4"
+version = "1.2.5"
 
 
 def check_requires(requires: list):
     pip_file = "pip.exe" if "win" in sys.platform else "pip"
     pip_paths = [
         os.path.join(os.path.dirname(sys.executable), "Scripts", pip_file),
         os.path.join(os.path.dirname(sys.executable), pip_file),
```

### Comparing `mtmtool-1.2.4/src/mtmtool/functool.py` & `mtmtool-1.2.5/src/mtmtool/functool.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.4/src/mtmtool/io.py` & `mtmtool-1.2.5/src/mtmtool/io.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.4/src/mtmtool/log.py` & `mtmtool-1.2.5/src/mtmtool/log.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.4/src/mtmtool/pool.py` & `mtmtool-1.2.5/src/mtmtool/pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,12 +71,12 @@
         self.function = func
 
     def worker_wrapper(self, arg):
         args, kwargs = arg
         return self.function(*args, **kwargs)
 
     def result(self):
-        logger.info("Start running with {} workers, {} tasks".format(self.max_workers), len(self.buffer))
+        logger.info("Start running with {} workers, {} tasks".format(self.max_workers, len(self.buffer)))
         with ProcessPoolExecutor(max_workers=self.max_workers) as executor:
             res = executor.map(self.worker_wrapper, self.buffer)
         self.buffer = []
         return res
```

### Comparing `mtmtool-1.2.4/src/mtmtool/projection.py` & `mtmtool-1.2.5/src/mtmtool/projection.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.4/src/mtmtool/time.py` & `mtmtool-1.2.5/src/mtmtool/time.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.4/src/mtmtool/webhook.py` & `mtmtool-1.2.5/src/mtmtool/webhook.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.2.4/src/mtmtool.egg-info/PKG-INFO` & `mtmtool-1.2.5/src/mtmtool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmtool
-Version: 1.2.4
+Version: 1.2.5
 Summary:  A Personal Python Tool Library.
 Home-page: https://github.com/imutum/imutum_python_tool
 Author: imutum
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
```

### Comparing `mtmtool-1.2.4/test/test_args2kwargs.py` & `mtmtool-1.2.5/test/test_args2kwargs.py`

 * *Files identical despite different names*

