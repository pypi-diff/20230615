# Comparing `tmp/kaki-0.1.8.tar.gz` & `tmp/kaki-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaki-0.1.8.tar", last modified: Fri Dec 23 09:24:36 2022, max compression
+gzip compressed data, was "kaki-0.1.9.tar", last modified: Thu Jun 15 15:25:29 2023, max compression
```

## Comparing `kaki-0.1.8.tar` & `kaki-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 tito      (1000) tito       (100)        0 2022-12-23 09:24:36.567979 kaki-0.1.8/
--rw-r--r--   0 tito      (1000) tito       (100)       63 2019-07-19 20:34:59.000000 kaki-0.1.8/.gitignore
--rw-r--r--   0 tito      (1000) tito       (100)       19 2019-07-19 20:34:59.000000 kaki-0.1.8/MANIFEST.in
--rw-r--r--   0 tito      (1000) tito       (100)     3977 2022-12-23 09:24:36.567979 kaki-0.1.8/PKG-INFO
--rw-r--r--   0 tito      (1000) tito       (100)     3035 2022-12-23 09:23:55.000000 kaki-0.1.8/README.md
-drwxr-xr-x   0 tito      (1000) tito       (100)        0 2022-12-23 09:24:36.567979 kaki-0.1.8/examples/
-drwxr-xr-x   0 tito      (1000) tito       (100)        0 2022-12-23 09:24:36.567979 kaki-0.1.8/examples/livedemo/
--rw-r--r--   0 tito      (1000) tito       (100)      177 2022-03-10 16:44:26.000000 kaki-0.1.8/examples/livedemo/README.md
-drwxr-xr-x   0 tito      (1000) tito       (100)        0 2022-12-23 09:24:36.567979 kaki-0.1.8/examples/livedemo/live/
--rw-r--r--   0 tito      (1000) tito       (100)        0 2019-07-19 20:34:59.000000 kaki-0.1.8/examples/livedemo/live/__init__.py
--rw-r--r--   0 tito      (1000) tito       (100)     1329 2019-07-19 20:34:59.000000 kaki-0.1.8/examples/livedemo/live/test.py
--rw-r--r--   0 tito      (1000) tito       (100)      249 2019-07-19 20:34:59.000000 kaki-0.1.8/examples/livedemo/live/ui.py
--rw-r--r--   0 tito      (1000) tito       (100)      283 2019-07-19 20:34:59.000000 kaki-0.1.8/examples/livedemo/main.py
-drwxr-xr-x   0 tito      (1000) tito       (100)        0 2022-12-23 09:24:36.567979 kaki-0.1.8/kaki/
--rw-r--r--   0 tito      (1000) tito       (100)       47 2022-12-23 09:24:36.000000 kaki-0.1.8/kaki/__init__.py
--rw-r--r--   0 tito      (1000) tito       (100)    14293 2022-12-23 09:11:07.000000 kaki-0.1.8/kaki/app.py
-drwxr-xr-x   0 tito      (1000) tito       (100)        0 2022-12-23 09:24:36.567979 kaki-0.1.8/kaki.egg-info/
--rw-r--r--   0 tito      (1000) tito       (100)     3977 2022-12-23 09:24:36.000000 kaki-0.1.8/kaki.egg-info/PKG-INFO
--rw-r--r--   0 tito      (1000) tito       (100)      368 2022-12-23 09:24:36.000000 kaki-0.1.8/kaki.egg-info/SOURCES.txt
--rw-r--r--   0 tito      (1000) tito       (100)        1 2022-12-23 09:24:36.000000 kaki-0.1.8/kaki.egg-info/dependency_links.txt
--rw-r--r--   0 tito      (1000) tito       (100)       14 2022-12-23 09:24:36.000000 kaki-0.1.8/kaki.egg-info/requires.txt
--rw-r--r--   0 tito      (1000) tito       (100)        5 2022-12-23 09:24:36.000000 kaki-0.1.8/kaki.egg-info/top_level.txt
--rw-r--r--   0 tito      (1000) tito       (100)       67 2022-12-23 09:24:36.567979 kaki-0.1.8/setup.cfg
--rw-r--r--   0 tito      (1000) tito       (100)     1527 2022-12-23 09:10:24.000000 kaki-0.1.8/setup.py
+drwxr-xr-x   0 tito      (1000) tito      (1000)        0 2023-06-15 15:25:29.763895 kaki-0.1.9/
+-rw-r--r--   0 tito      (1000) tito      (1000)       63 2019-07-19 20:34:59.000000 kaki-0.1.9/.gitignore
+-rw-r--r--   0 tito      (1000) tito      (1000)       19 2019-07-19 20:34:59.000000 kaki-0.1.9/MANIFEST.in
+-rw-r--r--   0 tito      (1000) tito      (1000)     3977 2023-06-15 15:25:29.763895 kaki-0.1.9/PKG-INFO
+-rw-r--r--   0 tito      (1000) tito      (1000)     3035 2022-12-23 09:23:55.000000 kaki-0.1.9/README.md
+drwxr-xr-x   0 tito      (1000) tito      (1000)        0 2023-06-15 15:25:29.763895 kaki-0.1.9/examples/
+drwxr-xr-x   0 tito      (1000) tito      (1000)        0 2023-06-15 15:25:29.763895 kaki-0.1.9/examples/livedemo/
+-rw-r--r--   0 tito      (1000) tito      (1000)      177 2022-03-10 16:44:26.000000 kaki-0.1.9/examples/livedemo/README.md
+drwxr-xr-x   0 tito      (1000) tito      (1000)        0 2023-06-15 15:25:29.763895 kaki-0.1.9/examples/livedemo/live/
+-rw-r--r--   0 tito      (1000) tito      (1000)        0 2019-07-19 20:34:59.000000 kaki-0.1.9/examples/livedemo/live/__init__.py
+-rw-r--r--   0 tito      (1000) tito      (1000)     1329 2019-07-19 20:34:59.000000 kaki-0.1.9/examples/livedemo/live/test.py
+-rw-r--r--   0 tito      (1000) tito      (1000)      249 2019-07-19 20:34:59.000000 kaki-0.1.9/examples/livedemo/live/ui.py
+-rw-r--r--   0 tito      (1000) tito      (1000)      283 2019-07-19 20:34:59.000000 kaki-0.1.9/examples/livedemo/main.py
+drwxr-xr-x   0 tito      (1000) tito      (1000)        0 2023-06-15 15:25:29.763895 kaki-0.1.9/kaki/
+-rw-r--r--   0 tito      (1000) tito      (1000)       47 2023-06-15 15:25:29.000000 kaki-0.1.9/kaki/__init__.py
+-rw-r--r--   0 tito      (1000) tito      (1000)    14289 2023-06-15 15:22:05.000000 kaki-0.1.9/kaki/app.py
+drwxr-xr-x   0 tito      (1000) tito      (1000)        0 2023-06-15 15:25:29.763895 kaki-0.1.9/kaki.egg-info/
+-rw-r--r--   0 tito      (1000) tito      (1000)     3977 2023-06-15 15:25:29.000000 kaki-0.1.9/kaki.egg-info/PKG-INFO
+-rw-r--r--   0 tito      (1000) tito      (1000)      368 2023-06-15 15:25:29.000000 kaki-0.1.9/kaki.egg-info/SOURCES.txt
+-rw-r--r--   0 tito      (1000) tito      (1000)        1 2023-06-15 15:25:29.000000 kaki-0.1.9/kaki.egg-info/dependency_links.txt
+-rw-r--r--   0 tito      (1000) tito      (1000)       14 2023-06-15 15:25:29.000000 kaki-0.1.9/kaki.egg-info/requires.txt
+-rw-r--r--   0 tito      (1000) tito      (1000)        5 2023-06-15 15:25:29.000000 kaki-0.1.9/kaki.egg-info/top_level.txt
+-rw-r--r--   0 tito      (1000) tito      (1000)       67 2023-06-15 15:25:29.763895 kaki-0.1.9/setup.cfg
+-rw-r--r--   0 tito      (1000) tito      (1000)     1527 2022-12-23 09:10:24.000000 kaki-0.1.9/setup.py
```

### Comparing `kaki-0.1.8/PKG-INFO` & `kaki-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaki
-Version: 0.1.8
+Version: 0.1.9
 Summary: Kivy application library on steroids
 Home-page: https://github.com/tito/kaki
 Author: Mathieu Virbel
 Author-email: mat@meltingrocks.com
 Project-URL: Bug Reports, https://github.com/tito/kaki/issues
 Project-URL: Source, https://github.com/tito/kaki/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `kaki-0.1.8/README.md` & `kaki-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `kaki-0.1.8/examples/livedemo/live/test.py` & `kaki-0.1.9/examples/livedemo/live/test.py`

 * *Files identical despite different names*

### Comparing `kaki-0.1.8/kaki/app.py` & `kaki-0.1.9/kaki/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 class E(ExceptionHandler):
     def handle_exception(self, inst):
         if isinstance(inst, (KeyboardInterrupt, SystemExit)):
             return ExceptionManager.RAISE
         app = App.get_running_app()
-        if not app.DEBUG and not app.RAISE_ERROR:
+        if not app.DEBUG and app.RAISE_ERROR:
             return ExceptionManager.RAISE
         app.set_error(inst, tb=traceback.format_exc())
         traceback.print_exc()
         return ExceptionManager.PASS
 
 
 ExceptionManager.add_handler(E())
```

### Comparing `kaki-0.1.8/kaki.egg-info/PKG-INFO` & `kaki-0.1.9/kaki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaki
-Version: 0.1.8
+Version: 0.1.9
 Summary: Kivy application library on steroids
 Home-page: https://github.com/tito/kaki
 Author: Mathieu Virbel
 Author-email: mat@meltingrocks.com
 Project-URL: Bug Reports, https://github.com/tito/kaki/issues
 Project-URL: Source, https://github.com/tito/kaki/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `kaki-0.1.8/setup.py` & `kaki-0.1.9/setup.py`

 * *Files identical despite different names*

