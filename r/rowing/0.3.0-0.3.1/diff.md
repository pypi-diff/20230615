# Comparing `tmp/rowing-0.3.0.tar.gz` & `tmp/rowing-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rowing-0.3.0.tar", last modified: Wed Jun 14 19:09:20 2023, max compression
+gzip compressed data, was "rowing-0.3.1.tar", last modified: Thu Jun 15 13:56:06 2023, max compression
```

## Comparing `rowing-0.3.0.tar` & `rowing-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:09:20.852481 rowing-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-14 19:09:11.000000 rowing-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-06-14 19:09:20.852481 rowing-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-06-14 19:09:11.000000 rowing-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:09:20.852481 rowing-0.3.0/rowing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:09:11.000000 rowing-0.3.0/rowing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-14 19:09:11.000000 rowing-0.3.0/rowing/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-06-14 19:09:11.000000 rowing-0.3.0/rowing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:09:20.852481 rowing-0.3.0/rowing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-06-14 19:09:20.000000 rowing-0.3.0/rowing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-14 19:09:20.000000 rowing-0.3.0/rowing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:09:20.000000 rowing-0.3.0/rowing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 19:09:20.000000 rowing-0.3.0/rowing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-14 19:09:20.000000 rowing-0.3.0/rowing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 19:09:20.000000 rowing-0.3.0/rowing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 19:09:20.852481 rowing-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-14 19:09:11.000000 rowing-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:56:06.153976 rowing-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-15 13:55:55.000000 rowing-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-15 13:56:06.153976 rowing-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-06-15 13:55:55.000000 rowing-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:56:06.149976 rowing-0.3.1/rowing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:55:55.000000 rowing-0.3.1/rowing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-15 13:55:55.000000 rowing-0.3.1/rowing/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-06-15 13:55:55.000000 rowing-0.3.1/rowing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:56:06.153976 rowing-0.3.1/rowing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-15 13:56:06.000000 rowing-0.3.1/rowing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-15 13:56:06.000000 rowing-0.3.1/rowing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:56:06.000000 rowing-0.3.1/rowing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-15 13:56:06.000000 rowing-0.3.1/rowing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-15 13:56:06.000000 rowing-0.3.1/rowing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 13:56:06.000000 rowing-0.3.1/rowing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 13:56:06.153976 rowing-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-15 13:55:55.000000 rowing-0.3.1/setup.py
```

### Comparing `rowing-0.3.0/LICENSE` & `rowing-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rowing-0.3.0/PKG-INFO` & `rowing-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rowing
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library for loading and presenting data from the worldrowing.com
 Home-page: https://github.com/matthewghgriffiths/rowing
 Author: Matthew Griffiths
 Author-email: matthewghgriffiths@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -13,15 +13,15 @@
 Provides-Extra: GARMIN
 Provides-Extra: GPX
 License-File: LICENSE
 
 # world_rowing
 Collection of code to load, process and analyse rowing data from [World Rowing](https://worldrowing.com/).
 
-Can view the world rowing data by running `streamlit run worldrowing_app.py` or visiting https://matthewghgriffiths-worldrowing.streamlit.app/
+Can view the world rowing data by running `streamlit run world_rowing_app/home.py` or visiting https://matthewghgriffiths-worldrowing.streamlit.app/
 
 # rowing.analysis
 A python library for analysing gps data, there are two main programs, `gpx` and `garmin`. `gpx` directly processes gpx files, calculating fastest times/splits over distances and timings/splits between specified rowing landmarks. See `Garmin.ipynb` for a more direct example of how to use the library.
 
 ## Example usage
 ```
 $ gpx --help
```

### Comparing `rowing-0.3.0/README.md` & `rowing-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # world_rowing
 Collection of code to load, process and analyse rowing data from [World Rowing](https://worldrowing.com/).
 
-Can view the world rowing data by running `streamlit run worldrowing_app.py` or visiting https://matthewghgriffiths-worldrowing.streamlit.app/
+Can view the world rowing data by running `streamlit run world_rowing_app/home.py` or visiting https://matthewghgriffiths-worldrowing.streamlit.app/
 
 # rowing.analysis
 A python library for analysing gps data, there are two main programs, `gpx` and `garmin`. `gpx` directly processes gpx files, calculating fastest times/splits over distances and timings/splits between specified rowing landmarks. See `Garmin.ipynb` for a more direct example of how to use the library.
 
 ## Example usage
 ```
 $ gpx --help
```

### Comparing `rowing-0.3.0/rowing/_compat.py` & `rowing-0.3.1/rowing/_compat.py`

 * *Files identical despite different names*

### Comparing `rowing-0.3.0/rowing/utils.py` & `rowing-0.3.1/rowing/utils.py`

 * *Files identical despite different names*

### Comparing `rowing-0.3.0/rowing.egg-info/PKG-INFO` & `rowing-0.3.1/rowing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rowing
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library for loading and presenting data from the worldrowing.com
 Home-page: https://github.com/matthewghgriffiths/rowing
 Author: Matthew Griffiths
 Author-email: matthewghgriffiths@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -13,15 +13,15 @@
 Provides-Extra: GARMIN
 Provides-Extra: GPX
 License-File: LICENSE
 
 # world_rowing
 Collection of code to load, process and analyse rowing data from [World Rowing](https://worldrowing.com/).
 
-Can view the world rowing data by running `streamlit run worldrowing_app.py` or visiting https://matthewghgriffiths-worldrowing.streamlit.app/
+Can view the world rowing data by running `streamlit run world_rowing_app/home.py` or visiting https://matthewghgriffiths-worldrowing.streamlit.app/
 
 # rowing.analysis
 A python library for analysing gps data, there are two main programs, `gpx` and `garmin`. `gpx` directly processes gpx files, calculating fastest times/splits over distances and timings/splits between specified rowing landmarks. See `Garmin.ipynb` for a more direct example of how to use the library.
 
 ## Example usage
 ```
 $ gpx --help
```

### Comparing `rowing-0.3.0/setup.py` & `rowing-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='rowing',
-    version='0.3.0',
+    version='0.3.1',
     description='Library for loading and presenting data from the worldrowing.com',
     author='Matthew Griffiths',
     author_email='matthewghgriffiths@gmail.com',
     url='https://github.com/matthewghgriffiths/rowing',
     packages=['rowing'],
     entry_points={
         'console_scripts': [
```

