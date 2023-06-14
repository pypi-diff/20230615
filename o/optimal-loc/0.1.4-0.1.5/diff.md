# Comparing `tmp/optimal_loc-0.1.4.tar.gz` & `tmp/optimal_loc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimal_loc-0.1.4.tar", max compression
+gzip compressed data, was "optimal_loc-0.1.5.tar", max compression
```

## Comparing `optimal_loc-0.1.4.tar` & `optimal_loc-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.1.4/LICENSE
--rw-r--r--   0        0        0     5263 2023-06-14 22:49:17.827797 optimal_loc-0.1.4/README.md
--rw-r--r--   0        0        0   125580 2023-05-07 13:18:02.614960 optimal_loc-0.1.4/optimal_loc/Modelling Algorithm.png
--rw-r--r--   0        0        0       87 2023-06-14 22:50:34.078058 optimal_loc-0.1.4/optimal_loc/__init__.py
--rw-r--r--   0        0        0    19115 2023-05-30 23:50:23.788871 optimal_loc-0.1.4/optimal_loc/app.py
--rw-r--r--   0        0        0      696 2023-05-28 22:37:44.186978 optimal_loc-0.1.4/optimal_loc/app_constants.py
--rw-r--r--   0        0        0      410 2023-05-28 23:21:17.917732 optimal_loc-0.1.4/optimal_loc/bash_command.py
--rw-r--r--   0        0        0     2691 2023-05-30 23:49:41.453579 optimal_loc-0.1.4/optimal_loc/st_app.py
--rw-r--r--   0        0        0      857 2023-06-14 22:50:05.641385 optimal_loc-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     6483 1970-01-01 00:00:00.000000 optimal_loc-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.1.5/LICENSE
+-rw-r--r--   0        0        0     5240 2023-06-14 22:54:07.375334 optimal_loc-0.1.5/README.md
+-rw-r--r--   0        0        0   125580 2023-05-07 13:18:02.614960 optimal_loc-0.1.5/optimal_loc/Modelling Algorithm.png
+-rw-r--r--   0        0        0       87 2023-06-14 22:54:07.370490 optimal_loc-0.1.5/optimal_loc/__init__.py
+-rw-r--r--   0        0        0    19115 2023-05-30 23:50:23.788871 optimal_loc-0.1.5/optimal_loc/app.py
+-rw-r--r--   0        0        0      696 2023-05-28 22:37:44.186978 optimal_loc-0.1.5/optimal_loc/app_constants.py
+-rw-r--r--   0        0        0      410 2023-05-28 23:21:17.917732 optimal_loc-0.1.5/optimal_loc/bash_command.py
+-rw-r--r--   0        0        0     2691 2023-05-30 23:49:41.453579 optimal_loc-0.1.5/optimal_loc/st_app.py
+-rw-r--r--   0        0        0      857 2023-06-14 22:54:07.372554 optimal_loc-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6460 1970-01-01 00:00:00.000000 optimal_loc-0.1.5/PKG-INFO
```

### Comparing `optimal_loc-0.1.4/LICENSE` & `optimal_loc-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.4/README.md` & `optimal_loc-0.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# Project Description
-
 ## What is it?
 
 The OptimalLoc package is a Python library designed to provide a solution for finding optimal locations based on various needs such as transportation and logistics, urban planning, retail, healthcare, and emergency services. The package utilizes a mixed integer linear optimization algorithm to calculate the optimal locations based on input demands and a specified number of location points.
 
 ## Main Features
 
 - Hexagon mapping: The package uses the Uber h3 library to map locations onto hexagons on a map. This allows for efficient optimization calculations by reducing the number of data points involved.
```

### Comparing `optimal_loc-0.1.4/optimal_loc/Modelling Algorithm.png` & `optimal_loc-0.1.5/optimal_loc/Modelling Algorithm.png`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.4/optimal_loc/app.py` & `optimal_loc-0.1.5/optimal_loc/app.py`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.4/optimal_loc/app_constants.py` & `optimal_loc-0.1.5/optimal_loc/app_constants.py`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.4/optimal_loc/st_app.py` & `optimal_loc-0.1.5/optimal_loc/st_app.py`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.4/pyproject.toml` & `optimal_loc-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optimal-loc"
-version = "0.1.4"
+version = "0.1.5"
 description = "A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs."
 
 authors = ["Sinan Demirhan <sdemirhan1320@gmail.com>"]
 readme = "README.md"
 packages = [{include = "optimal_loc"}]
 license = "MIT"
 homepage = "https://github.com/sinan-demirhan/optimal-loc"
```

### Comparing `optimal_loc-0.1.4/PKG-INFO` & `optimal_loc-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimal-loc
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs.
 Home-page: https://github.com/sinan-demirhan/optimal-loc
 License: MIT
 Keywords: optimalLoc,optimal_loc,optimal-loc,optimal,optimal location,optimal location finder
 Author: Sinan Demirhan
 Author-email: sdemirhan1320@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -21,16 +21,14 @@
 Requires-Dist: pandas (>=1.2.4,<2.0.0)
 Requires-Dist: pulp (>=2.4,<3.0)
 Requires-Dist: pymongo (>=3.11.0,<4.0.0)
 Requires-Dist: streamlit (>=1.21.0,<2.0.0)
 Project-URL: Repository, https://github.com/sinan-demirhan/optimal-loc
 Description-Content-Type: text/markdown
 
-# Project Description
-
 ## What is it?
 
 The OptimalLoc package is a Python library designed to provide a solution for finding optimal locations based on various needs such as transportation and logistics, urban planning, retail, healthcare, and emergency services. The package utilizes a mixed integer linear optimization algorithm to calculate the optimal locations based on input demands and a specified number of location points.
 
 ## Main Features
 
 - Hexagon mapping: The package uses the Uber h3 library to map locations onto hexagons on a map. This allows for efficient optimization calculations by reducing the number of data points involved.
```

