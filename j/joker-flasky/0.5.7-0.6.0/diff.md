# Comparing `tmp/joker-flasky-0.5.7.tar.gz` & `tmp/joker-flasky-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joker-flasky-0.5.7.tar", last modified: Fri Apr  7 03:11:50 2023, max compression
+gzip compressed data, was "joker-flasky-0.6.0.tar", last modified: Thu Jun 15 02:12:33 2023, max compression
```

## Comparing `joker-flasky-0.5.7.tar` & `joker-flasky-0.6.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-04-07 03:11:50.623055 joker-flasky-0.5.7/
--rw-r--r--   0 Hailong    (502) staff       (20)    35149 2018-11-06 12:36:13.000000 joker-flasky-0.5.7/LICENSE
--rw-r--r--   0 Hailong    (502) staff       (20)      106 2022-05-11 15:56:47.000000 joker-flasky-0.5.7/MANIFEST.in
--rw-r--r--   0 Hailong    (502) staff       (20)     1473 2023-04-07 03:11:50.622749 joker-flasky-0.5.7/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)      986 2022-05-24 12:19:22.000000 joker-flasky-0.5.7/README.md
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-04-07 03:11:50.610207 joker-flasky-0.5.7/joker/
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-04-07 03:11:50.616874 joker-flasky-0.5.7/joker/flasky/
--rw-r--r--   0 Hailong    (502) staff       (20)       98 2023-04-07 03:09:34.000000 joker-flasky-0.5.7/joker/flasky/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1315 2022-01-21 14:04:10.000000 joker-flasky-0.5.7/joker/flasky/app.py
--rw-r--r--   0 Hailong    (502) staff       (20)     5275 2022-05-06 15:22:35.000000 joker-flasky-0.5.7/joker/flasky/auth.py
--rw-r--r--   0 Hailong    (502) staff       (20)      919 2022-05-05 06:06:00.000000 joker-flasky-0.5.7/joker/flasky/context.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1524 2021-09-04 07:05:32.000000 joker-flasky-0.5.7/joker/flasky/develop.py
--rw-r--r--   0 Hailong    (502) staff       (20)      699 2022-05-13 10:17:47.000000 joker-flasky-0.5.7/joker/flasky/environ.py
--rw-r--r--   0 Hailong    (502) staff       (20)      384 2022-05-06 15:22:35.000000 joker-flasky-0.5.7/joker/flasky/loggers.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1348 2022-05-11 13:11:04.000000 joker-flasky-0.5.7/joker/flasky/pages.py
--rw-r--r--   0 Hailong    (502) staff       (20)      330 2022-03-04 12:46:49.000000 joker-flasky-0.5.7/joker/flasky/security.py
--rw-r--r--   0 Hailong    (502) staff       (20)      644 2021-09-04 16:31:12.000000 joker-flasky-0.5.7/joker/flasky/serialize.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-04-07 03:11:50.617865 joker-flasky-0.5.7/joker/flasky/templates/
--rw-r--r--   0 Hailong    (502) staff       (20)     1842 2022-05-24 11:30:42.000000 joker-flasky-0.5.7/joker/flasky/templates/help.html
--rw-r--r--   0 Hailong    (502) staff       (20)     2168 2022-05-11 12:26:38.000000 joker-flasky-0.5.7/joker/flasky/templates/helplist.html
--rw-r--r--   0 Hailong    (502) staff       (20)     1730 2022-05-13 12:40:19.000000 joker-flasky-0.5.7/joker/flasky/templates/login.html
--rw-r--r--   0 Hailong    (502) staff       (20)      583 2022-05-11 15:54:35.000000 joker-flasky-0.5.7/joker/flasky/templates/upload.html
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-04-07 03:11:50.618593 joker-flasky-0.5.7/joker/flasky/tools/
--rw-r--r--   0 Hailong    (502) staff       (20)       39 2021-09-04 16:34:51.000000 joker-flasky-0.5.7/joker/flasky/tools/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1032 2022-05-09 15:09:48.000000 joker-flasky-0.5.7/joker/flasky/tools/docs.py
--rw-r--r--   0 Hailong    (502) staff       (20)     2056 2022-01-21 14:04:37.000000 joker-flasky-0.5.7/joker/flasky/tools/validation.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-04-07 03:11:50.619726 joker-flasky-0.5.7/joker/flasky/views/
--rw-r--r--   0 Hailong    (502) staff       (20)       39 2021-09-04 10:56:53.000000 joker-flasky-0.5.7/joker/flasky/views/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)     2223 2021-12-08 12:08:11.000000 joker-flasky-0.5.7/joker/flasky/views/admin_views.py
--rw-r--r--   0 Hailong    (502) staff       (20)      549 2021-09-19 09:52:20.000000 joker-flasky-0.5.7/joker/flasky/views/ctxmap_views.py
--rw-r--r--   0 Hailong    (502) staff       (20)     9846 2023-04-07 03:08:51.000000 joker-flasky-0.5.7/joker/flasky/viewutils.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-04-07 03:11:50.622341 joker-flasky-0.5.7/joker_flasky.egg-info/
--rw-r--r--   0 Hailong    (502) staff       (20)     1473 2023-04-07 03:11:50.000000 joker-flasky-0.5.7/joker_flasky.egg-info/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)      905 2023-04-07 03:11:50.000000 joker-flasky-0.5.7/joker_flasky.egg-info/SOURCES.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2023-04-07 03:11:50.000000 joker-flasky-0.5.7/joker_flasky.egg-info/dependency_links.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        6 2023-04-07 03:11:50.000000 joker-flasky-0.5.7/joker_flasky.egg-info/namespace_packages.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2022-05-24 12:20:10.000000 joker-flasky-0.5.7/joker_flasky.egg-info/not-zip-safe
--rw-r--r--   0 Hailong    (502) staff       (20)       93 2023-04-07 03:11:50.000000 joker-flasky-0.5.7/joker_flasky.egg-info/requires.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        6 2023-04-07 03:11:50.000000 joker-flasky-0.5.7/joker_flasky.egg-info/top_level.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       92 2023-04-07 03:06:12.000000 joker-flasky-0.5.7/requirements.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       38 2023-04-07 03:11:50.623152 joker-flasky-0.5.7/setup.cfg
--rw-r--r--   0 Hailong    (502) staff       (20)     1688 2022-05-07 13:29:28.000000 joker-flasky-0.5.7/setup.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-06-15 02:12:33.077060 joker-flasky-0.6.0/
+-rw-r--r--   0 Hailong    (502) staff       (20)    35149 2018-11-06 12:36:13.000000 joker-flasky-0.6.0/LICENSE
+-rw-r--r--   0 Hailong    (502) staff       (20)      106 2022-05-11 15:56:47.000000 joker-flasky-0.6.0/MANIFEST.in
+-rw-r--r--   0 Hailong    (502) staff       (20)     1473 2023-06-15 02:12:33.076650 joker-flasky-0.6.0/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)      986 2022-05-24 12:19:22.000000 joker-flasky-0.6.0/README.md
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-06-15 02:12:33.063310 joker-flasky-0.6.0/joker/
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-06-15 02:12:33.069295 joker-flasky-0.6.0/joker/flasky/
+-rw-r--r--   0 Hailong    (502) staff       (20)       98 2023-06-15 02:10:41.000000 joker-flasky-0.6.0/joker/flasky/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1315 2022-01-21 14:04:10.000000 joker-flasky-0.6.0/joker/flasky/app.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     5275 2022-05-06 15:22:35.000000 joker-flasky-0.6.0/joker/flasky/auth.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      919 2022-05-05 06:06:00.000000 joker-flasky-0.6.0/joker/flasky/context.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1524 2021-09-04 07:05:32.000000 joker-flasky-0.6.0/joker/flasky/develop.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      699 2022-05-13 10:17:47.000000 joker-flasky-0.6.0/joker/flasky/environ.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      384 2022-05-06 15:22:35.000000 joker-flasky-0.6.0/joker/flasky/loggers.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1348 2022-05-11 13:11:04.000000 joker-flasky-0.6.0/joker/flasky/pages.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      330 2022-03-04 12:46:49.000000 joker-flasky-0.6.0/joker/flasky/security.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      644 2021-09-04 16:31:12.000000 joker-flasky-0.6.0/joker/flasky/serialize.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-06-15 02:12:33.070997 joker-flasky-0.6.0/joker/flasky/templates/
+-rw-r--r--   0 Hailong    (502) staff       (20)     1842 2022-05-24 11:30:42.000000 joker-flasky-0.6.0/joker/flasky/templates/help.html
+-rw-r--r--   0 Hailong    (502) staff       (20)     2168 2022-05-11 12:26:38.000000 joker-flasky-0.6.0/joker/flasky/templates/helplist.html
+-rw-r--r--   0 Hailong    (502) staff       (20)     1730 2022-05-13 12:40:19.000000 joker-flasky-0.6.0/joker/flasky/templates/login.html
+-rw-r--r--   0 Hailong    (502) staff       (20)      583 2022-05-11 15:54:35.000000 joker-flasky-0.6.0/joker/flasky/templates/upload.html
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-06-15 02:12:33.072388 joker-flasky-0.6.0/joker/flasky/tools/
+-rw-r--r--   0 Hailong    (502) staff       (20)       39 2021-09-04 16:34:51.000000 joker-flasky-0.6.0/joker/flasky/tools/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1032 2022-05-09 15:09:48.000000 joker-flasky-0.6.0/joker/flasky/tools/docs.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     2056 2022-01-21 14:04:37.000000 joker-flasky-0.6.0/joker/flasky/tools/validation.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-06-15 02:12:33.073569 joker-flasky-0.6.0/joker/flasky/views/
+-rw-r--r--   0 Hailong    (502) staff       (20)       39 2021-09-04 10:56:53.000000 joker-flasky-0.6.0/joker/flasky/views/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     2223 2021-12-08 12:08:11.000000 joker-flasky-0.6.0/joker/flasky/views/admin_views.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      549 2021-09-19 09:52:20.000000 joker-flasky-0.6.0/joker/flasky/views/ctxmap_views.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     9911 2023-06-15 02:10:21.000000 joker-flasky-0.6.0/joker/flasky/viewutils.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-06-15 02:12:33.076152 joker-flasky-0.6.0/joker_flasky.egg-info/
+-rw-r--r--   0 Hailong    (502) staff       (20)     1473 2023-06-15 02:12:33.000000 joker-flasky-0.6.0/joker_flasky.egg-info/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)      905 2023-06-15 02:12:33.000000 joker-flasky-0.6.0/joker_flasky.egg-info/SOURCES.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2023-06-15 02:12:33.000000 joker-flasky-0.6.0/joker_flasky.egg-info/dependency_links.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        6 2023-06-15 02:12:33.000000 joker-flasky-0.6.0/joker_flasky.egg-info/namespace_packages.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2023-06-15 02:12:33.000000 joker-flasky-0.6.0/joker_flasky.egg-info/not-zip-safe
+-rw-r--r--   0 Hailong    (502) staff       (20)       93 2023-06-15 02:12:33.000000 joker-flasky-0.6.0/joker_flasky.egg-info/requires.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        6 2023-06-15 02:12:33.000000 joker-flasky-0.6.0/joker_flasky.egg-info/top_level.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       92 2023-04-07 03:06:12.000000 joker-flasky-0.6.0/requirements.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       38 2023-06-15 02:12:33.077172 joker-flasky-0.6.0/setup.cfg
+-rw-r--r--   0 Hailong    (502) staff       (20)     1688 2022-05-07 13:29:28.000000 joker-flasky-0.6.0/setup.py
```

### Comparing `joker-flasky-0.5.7/LICENSE` & `joker-flasky-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `joker-flasky-0.5.7/PKG-INFO` & `joker-flasky-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joker-flasky
-Version: 0.5.7
+Version: 0.6.0
 Summary: reusable components for flask-based web development
 License: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `joker-flasky-0.5.7/README.md` & `joker-flasky-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `joker-flasky-0.5.7/joker/flasky/app.py` & `joker-flasky-0.6.0/joker/flasky/app.py`

 * *Files identical despite different names*

### Comparing `joker-flasky-0.5.7/joker/flasky/auth.py` & `joker-flasky-0.6.0/joker/flasky/auth.py`

 * *Files identical despite different names*

### Comparing `joker-flasky-0.5.7/joker/flasky/context.py` & `joker-flasky-0.6.0/joker/flasky/context.py`

 * *Files identical despite different names*

### Comparing `joker-flasky-0.5.7/joker/flasky/develop.py` & `joker-flasky-0.6.0/joker/flasky/develop.py`

 * *Files identical despite different names*

### Comparing `joker-flasky-0.5.7/joker/flasky/environ.py` & `joker-flasky-0.6.0/joker/flasky/environ.py`

 * *Files identical despite different names*

### Comparing `joker-flasky-0.5.7/joker/flasky/pages.py` & `joker-flasky-0.6.0/joker/flasky/pages.py`

 * *Files identical despite different names*

### Comparing `joker-flasky-0.5.7/joker/flasky/serialize.py` & `joker-flasky-0.6.0/joker/flasky/serialize.py`

 * *Files identical despite different names*

### Comparing `joker-flasky-0.5.7/joker/flasky/templates/help.html` & `joker-flasky-0.6.0/joker/flasky/templates/help.html`

 * *Files identical despite different names*

### Comparing `joker-flasky-0.5.7/joker/flasky/templates/helplist.html` & `joker-flasky-0.6.0/joker/flasky/templates/helplist.html`

 * *Files identical despite different names*

### Comparing `joker-flasky-0.5.7/joker/flasky/templates/login.html` & `joker-flasky-0.6.0/joker/flasky/templates/login.html`

 * *Files identical despite different names*

### Comparing `joker-flasky-0.5.7/joker/flasky/templates/upload.html` & `joker-flasky-0.6.0/joker/flasky/templates/upload.html`

 * *Files identical despite different names*

### Comparing `joker-flasky-0.5.7/joker/flasky/tools/docs.py` & `joker-flasky-0.6.0/joker/flasky/tools/docs.py`

 * *Files identical despite different names*

### Comparing `joker-flasky-0.5.7/joker/flasky/tools/validation.py` & `joker-flasky-0.6.0/joker/flasky/tools/validation.py`

 * *Files identical despite different names*

### Comparing `joker-flasky-0.5.7/joker/flasky/views/admin_views.py` & `joker-flasky-0.6.0/joker/flasky/views/admin_views.py`

 * *Files identical despite different names*

### Comparing `joker-flasky-0.5.7/joker/flasky/views/ctxmap_views.py` & `joker-flasky-0.6.0/joker/flasky/views/ctxmap_views.py`

 * *Files identical despite different names*

### Comparing `joker-flasky-0.5.7/joker/flasky/viewutils.py` & `joker-flasky-0.6.0/joker/flasky/viewutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,22 +180,25 @@
     return call_json_default_functions(o, funcs)
 
 
 def chain_json_default_functions(*funcs):
     return functools.partial(call_json_default_functions, funcs=funcs)
 
 
-class JSONEncoderPlus(flask.json.JSONEncoder):
-    json_default_funcs = [json_default_strict, str]
-
-    def default(self, o):
-        try:
-            return call_json_default_functions(o, self.json_default_funcs)
-        except TypeError:
-            return super().default(o)
+try:
+    class JSONEncoderPlus(flask.json.JSONEncoder):
+        json_default_funcs = [json_default_strict, str]
+
+        def default(self, o):
+            try:
+                return call_json_default_functions(o, self.json_default_funcs)
+            except TypeError:
+                return super().default(o)
+except AttributeError:
+    pass
 
 
 def get_json_encoder(*json_default_funcs):
     # bases should be a tuple
     bases = JSONEncoderPlus,
     attrs = {'json_default_funcs': list(json_default_funcs)}
     return type('JSONEncoderExtended', bases, attrs)
```

### Comparing `joker-flasky-0.5.7/joker_flasky.egg-info/PKG-INFO` & `joker-flasky-0.6.0/joker_flasky.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joker-flasky
-Version: 0.5.7
+Version: 0.6.0
 Summary: reusable components for flask-based web development
 License: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `joker-flasky-0.5.7/joker_flasky.egg-info/SOURCES.txt` & `joker-flasky-0.6.0/joker_flasky.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joker-flasky-0.5.7/setup.py` & `joker-flasky-0.6.0/setup.py`

 * *Files identical despite different names*

