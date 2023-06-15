# Comparing `tmp/hdlib-0.1.6.tar.gz` & `tmp/hdlib-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdlib-0.1.6.tar", last modified: Thu Jun 15 14:41:32 2023, max compression
+gzip compressed data, was "hdlib-0.1.7.tar", last modified: Thu Jun 15 20:19:48 2023, max compression
```

## Comparing `hdlib-0.1.6.tar` & `hdlib-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-15 14:41:32.697124 hdlib-0.1.6/
--rw-r--r--   0 fabio      (501) staff       (20)     1068 2022-04-25 18:30:15.000000 hdlib-0.1.6/LICENSE
--rw-r--r--   0 fabio      (501) staff       (20)     3028 2023-06-15 14:41:32.694494 hdlib-0.1.6/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)     2225 2023-06-13 01:38:11.000000 hdlib-0.1.6/README.md
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-15 14:41:32.445307 hdlib-0.1.6/hdlib/
--rw-r--r--   0 fabio      (501) staff       (20)      102 2023-06-14 21:23:08.000000 hdlib-0.1.6/hdlib/__init__.py
--rw-r--r--   0 fabio      (501) staff       (20)     2480 2023-06-01 14:38:17.000000 hdlib-0.1.6/hdlib/arithmetic.py
--rw-r--r--   0 fabio      (501) staff       (20)    29764 2023-06-15 01:29:07.000000 hdlib-0.1.6/hdlib/model.py
--rw-r--r--   0 fabio      (501) staff       (20)     2534 2023-06-08 21:27:39.000000 hdlib-0.1.6/hdlib/parser.py
--rw-r--r--   0 fabio      (501) staff       (20)    21854 2023-06-08 20:17:24.000000 hdlib-0.1.6/hdlib/space.py
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-15 14:41:32.644790 hdlib-0.1.6/hdlib.egg-info/
--rw-r--r--   0 fabio      (501) staff       (20)     3028 2023-06-15 14:41:32.000000 hdlib-0.1.6/hdlib.egg-info/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)      295 2023-06-15 14:41:32.000000 hdlib-0.1.6/hdlib.egg-info/SOURCES.txt
--rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-15 14:41:32.000000 hdlib-0.1.6/hdlib.egg-info/dependency_links.txt
--rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-15 14:41:32.000000 hdlib-0.1.6/hdlib.egg-info/not-zip-safe
--rw-r--r--   0 fabio      (501) staff       (20)       50 2023-06-15 14:41:32.000000 hdlib-0.1.6/hdlib.egg-info/requires.txt
--rw-r--r--   0 fabio      (501) staff       (20)        6 2023-06-15 14:41:32.000000 hdlib-0.1.6/hdlib.egg-info/top_level.txt
--rw-r--r--   0 fabio      (501) staff       (20)       38 2023-06-15 14:41:32.697545 hdlib-0.1.6/setup.cfg
--rw-r--r--   0 fabio      (501) staff       (20)     1462 2023-06-15 14:40:58.000000 hdlib-0.1.6/setup.py
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-15 14:41:32.648478 hdlib-0.1.6/test/
--rw-r--r--   0 fabio      (501) staff       (20)     8033 2023-06-13 01:24:19.000000 hdlib-0.1.6/test/test.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-15 20:19:48.446390 hdlib-0.1.7/
+-rw-r--r--   0 fabio      (501) staff       (20)     1068 2022-04-25 18:30:15.000000 hdlib-0.1.7/LICENSE
+-rw-r--r--   0 fabio      (501) staff       (20)     3028 2023-06-15 20:19:48.444930 hdlib-0.1.7/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)     2225 2023-06-13 01:38:11.000000 hdlib-0.1.7/README.md
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-15 20:19:48.298274 hdlib-0.1.7/hdlib/
+-rw-r--r--   0 fabio      (501) staff       (20)      102 2023-06-15 20:14:44.000000 hdlib-0.1.7/hdlib/__init__.py
+-rw-r--r--   0 fabio      (501) staff       (20)     2480 2023-06-01 14:38:17.000000 hdlib-0.1.7/hdlib/arithmetic.py
+-rw-r--r--   0 fabio      (501) staff       (20)    29987 2023-06-15 20:14:36.000000 hdlib-0.1.7/hdlib/model.py
+-rw-r--r--   0 fabio      (501) staff       (20)     2534 2023-06-08 21:27:39.000000 hdlib-0.1.7/hdlib/parser.py
+-rw-r--r--   0 fabio      (501) staff       (20)    21854 2023-06-08 20:17:24.000000 hdlib-0.1.7/hdlib/space.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-15 20:19:48.398650 hdlib-0.1.7/hdlib.egg-info/
+-rw-r--r--   0 fabio      (501) staff       (20)     3028 2023-06-15 20:19:48.000000 hdlib-0.1.7/hdlib.egg-info/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)      295 2023-06-15 20:19:48.000000 hdlib-0.1.7/hdlib.egg-info/SOURCES.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-15 20:19:48.000000 hdlib-0.1.7/hdlib.egg-info/dependency_links.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-15 20:19:48.000000 hdlib-0.1.7/hdlib.egg-info/not-zip-safe
+-rw-r--r--   0 fabio      (501) staff       (20)       50 2023-06-15 20:19:48.000000 hdlib-0.1.7/hdlib.egg-info/requires.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        6 2023-06-15 20:19:48.000000 hdlib-0.1.7/hdlib.egg-info/top_level.txt
+-rw-r--r--   0 fabio      (501) staff       (20)       38 2023-06-15 20:19:48.446735 hdlib-0.1.7/setup.cfg
+-rw-r--r--   0 fabio      (501) staff       (20)     1462 2023-06-15 14:40:58.000000 hdlib-0.1.7/setup.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-15 20:19:48.423976 hdlib-0.1.7/test/
+-rw-r--r--   0 fabio      (501) staff       (20)     8033 2023-06-13 01:24:19.000000 hdlib-0.1.7/test/test.py
```

### Comparing `hdlib-0.1.6/LICENSE` & `hdlib-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.6/PKG-INFO` & `hdlib-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdlib
-Version: 0.1.6
+Version: 0.1.7
 Summary: Hyperdimensional Computing Library for building Vector Symbolic Architectures in Python
 Home-page: http://github.com/cumbof/hdlib
 Author: Fabio Cumbo
 Author-email: fabio.cumbo@gmail.com
 License: MIT
 Project-URL: Issues, https://github.com/cumbof/hdlib/issues
 Project-URL: Source, https://github.com/cumbof/hdlib
```

### Comparing `hdlib-0.1.6/README.md` & `hdlib-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.6/hdlib/arithmetic.py` & `hdlib-0.1.7/hdlib/arithmetic.py`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.6/hdlib/model.py` & `hdlib-0.1.7/hdlib/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -685,25 +685,28 @@
 
         # Take track of the last feature selection
         # Only in case of forward variable selection
         last_selection = set()
 
         prev_score = 0.0
 
-        count_iter = 0
+        count_iter = 1
 
         while features_indices:
-            if len(features_indices) == 1:
-                break
-
             if method == "backward":
                 features_set_size = len(features_indices) - 1
 
+                if len(features_indices) == 1:
+                    break
+
             elif method == "forward":
-                features_set_size = 1
+                features_set_size = count_iter
+
+                if features_set_size >= len(features_indices):
+                    break
 
             if features_set_size > 0:
                 best_score = 0.0
                 classification_results = list()
 
                 partial_stepwise_regression_iter = partial(
                     self.stepwise_regression_iter,
@@ -794,13 +797,15 @@
 
         for feature in features_importance:
             importance[feature] = features_importance[feature]["importance"]
 
             scores[features_importance[feature]["importance"]] = features_importance[feature]["score"]
 
         if method == "backward":
-            top_importance = min(importance.values())
+            imp_values = [imp for imp in importance.values() if scores[imp] > 0.0]
+
+            top_importance = min(imp_values) if imp_values else 0
 
-        else:
+        elif method == "forward":
             top_importance = max(importance.values())
 
         return importance, scores, top_importance
```

### Comparing `hdlib-0.1.6/hdlib/parser.py` & `hdlib-0.1.7/hdlib/parser.py`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.6/hdlib/space.py` & `hdlib-0.1.7/hdlib/space.py`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.6/hdlib.egg-info/PKG-INFO` & `hdlib-0.1.7/hdlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdlib
-Version: 0.1.6
+Version: 0.1.7
 Summary: Hyperdimensional Computing Library for building Vector Symbolic Architectures in Python
 Home-page: http://github.com/cumbof/hdlib
 Author: Fabio Cumbo
 Author-email: fabio.cumbo@gmail.com
 License: MIT
 Project-URL: Issues, https://github.com/cumbof/hdlib/issues
 Project-URL: Source, https://github.com/cumbof/hdlib
```

### Comparing `hdlib-0.1.6/setup.py` & `hdlib-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.6/test/test.py` & `hdlib-0.1.7/test/test.py`

 * *Files identical despite different names*

