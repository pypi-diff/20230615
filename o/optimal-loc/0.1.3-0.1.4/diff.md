# Comparing `tmp/optimal_loc-0.1.3.tar.gz` & `tmp/optimal_loc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimal_loc-0.1.3.tar", max compression
+gzip compressed data, was "optimal_loc-0.1.4.tar", max compression
```

## Comparing `optimal_loc-0.1.3.tar` & `optimal_loc-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.1.3/LICENSE
--rw-r--r--   0        0        0      552 2023-05-01 00:14:15.114286 optimal_loc-0.1.3/README.md
--rw-r--r--   0        0        0   125580 2023-05-07 13:18:02.614960 optimal_loc-0.1.3/optimal_loc/Modelling Algorithm.png
--rw-r--r--   0        0        0       87 2023-05-30 23:50:43.751464 optimal_loc-0.1.3/optimal_loc/__init__.py
--rw-r--r--   0        0        0    19115 2023-05-30 23:50:23.788871 optimal_loc-0.1.3/optimal_loc/app.py
--rw-r--r--   0        0        0      696 2023-05-28 22:37:44.186978 optimal_loc-0.1.3/optimal_loc/app_constants.py
--rw-r--r--   0        0        0      410 2023-05-28 23:21:17.917732 optimal_loc-0.1.3/optimal_loc/bash_command.py
--rw-r--r--   0        0        0     2691 2023-05-30 23:49:41.453579 optimal_loc-0.1.3/optimal_loc/st_app.py
--rw-r--r--   0        0        0      857 2023-05-30 23:50:47.906822 optimal_loc-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 optimal_loc-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.1.4/LICENSE
+-rw-r--r--   0        0        0     5263 2023-06-14 22:49:17.827797 optimal_loc-0.1.4/README.md
+-rw-r--r--   0        0        0   125580 2023-05-07 13:18:02.614960 optimal_loc-0.1.4/optimal_loc/Modelling Algorithm.png
+-rw-r--r--   0        0        0       87 2023-06-14 22:50:34.078058 optimal_loc-0.1.4/optimal_loc/__init__.py
+-rw-r--r--   0        0        0    19115 2023-05-30 23:50:23.788871 optimal_loc-0.1.4/optimal_loc/app.py
+-rw-r--r--   0        0        0      696 2023-05-28 22:37:44.186978 optimal_loc-0.1.4/optimal_loc/app_constants.py
+-rw-r--r--   0        0        0      410 2023-05-28 23:21:17.917732 optimal_loc-0.1.4/optimal_loc/bash_command.py
+-rw-r--r--   0        0        0     2691 2023-05-30 23:49:41.453579 optimal_loc-0.1.4/optimal_loc/st_app.py
+-rw-r--r--   0        0        0      857 2023-06-14 22:50:05.641385 optimal_loc-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6483 1970-01-01 00:00:00.000000 optimal_loc-0.1.4/PKG-INFO
```

### Comparing `optimal_loc-0.1.3/LICENSE` & `optimal_loc-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.3/optimal_loc/Modelling Algorithm.png` & `optimal_loc-0.1.4/optimal_loc/Modelling Algorithm.png`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.3/optimal_loc/app.py` & `optimal_loc-0.1.4/optimal_loc/app.py`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.3/optimal_loc/app_constants.py` & `optimal_loc-0.1.4/optimal_loc/app_constants.py`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.3/optimal_loc/st_app.py` & `optimal_loc-0.1.4/optimal_loc/st_app.py`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.3/pyproject.toml` & `optimal_loc-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optimal-loc"
-version = "0.1.3"
+version = "0.1.4"
 description = "A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs."
 
 authors = ["Sinan Demirhan <sdemirhan1320@gmail.com>"]
 readme = "README.md"
 packages = [{include = "optimal_loc"}]
 license = "MIT"
 homepage = "https://github.com/sinan-demirhan/optimal-loc"
```

