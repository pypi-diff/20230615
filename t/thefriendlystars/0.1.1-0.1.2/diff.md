# Comparing `tmp/thefriendlystars-0.1.1.tar.gz` & `tmp/thefriendlystars-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thefriendlystars-0.1.1.tar", last modified: Wed Jun 14 07:41:06 2023, max compression
+gzip compressed data, was "thefriendlystars-0.1.2.tar", last modified: Wed Jun 14 23:28:21 2023, max compression
```

## Comparing `thefriendlystars-0.1.1.tar` & `thefriendlystars-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-14 07:41:06.271602 thefriendlystars-0.1.1/
--rw-r--r--   0 zach       (502) staff       (20)     1076 2023-06-14 03:17:18.000000 thefriendlystars-0.1.1/LICENSE
--rw-r--r--   0 zach       (502) staff       (20)      616 2023-06-14 07:41:06.271455 thefriendlystars-0.1.1/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)     2299 2023-06-14 03:19:01.000000 thefriendlystars-0.1.1/README.md
--rw-r--r--   0 zach       (502) staff       (20)       38 2023-06-14 07:41:06.271643 thefriendlystars-0.1.1/setup.cfg
--rw-r--r--   0 zach       (502) staff       (20)     3882 2023-06-14 03:23:24.000000 thefriendlystars-0.1.1/setup.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-14 07:41:06.270265 thefriendlystars-0.1.1/thefriendlystars/
--rw-r--r--   0 zach       (502) staff       (20)       19 2023-06-14 03:17:18.000000 thefriendlystars-0.1.1/thefriendlystars/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     7917 2023-06-14 03:58:43.000000 thefriendlystars-0.1.1/thefriendlystars/gaia.py
--rw-r--r--   0 zach       (502) staff       (20)      306 2023-06-14 03:17:18.000000 thefriendlystars-0.1.1/thefriendlystars/imports.py
--rwxr-xr-x   0 zach       (502) staff       (20)       62 2023-06-14 07:40:53.000000 thefriendlystars-0.1.1/thefriendlystars/version.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-14 07:41:06.271232 thefriendlystars-0.1.1/thefriendlystars.egg-info/
--rw-r--r--   0 zach       (502) staff       (20)      616 2023-06-14 07:41:06.000000 thefriendlystars-0.1.1/thefriendlystars.egg-info/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)      374 2023-06-14 07:41:06.000000 thefriendlystars-0.1.1/thefriendlystars.egg-info/SOURCES.txt
--rw-r--r--   0 zach       (502) staff       (20)        1 2023-06-14 07:41:06.000000 thefriendlystars-0.1.1/thefriendlystars.egg-info/dependency_links.txt
--rw-r--r--   0 zach       (502) staff       (20)        1 2023-06-14 03:19:56.000000 thefriendlystars-0.1.1/thefriendlystars.egg-info/not-zip-safe
--rw-r--r--   0 zach       (502) staff       (20)      204 2023-06-14 07:41:06.000000 thefriendlystars-0.1.1/thefriendlystars.egg-info/requires.txt
--rw-r--r--   0 zach       (502) staff       (20)       17 2023-06-14 07:41:06.000000 thefriendlystars-0.1.1/thefriendlystars.egg-info/top_level.txt
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-14 23:28:21.059272 thefriendlystars-0.1.2/
+-rw-r--r--   0 zach       (502) staff       (20)     1076 2023-06-14 03:17:18.000000 thefriendlystars-0.1.2/LICENSE
+-rw-r--r--   0 zach       (502) staff       (20)      616 2023-06-14 23:28:21.059031 thefriendlystars-0.1.2/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)     2299 2023-06-14 03:19:01.000000 thefriendlystars-0.1.2/README.md
+-rw-r--r--   0 zach       (502) staff       (20)       38 2023-06-14 23:28:21.059329 thefriendlystars-0.1.2/setup.cfg
+-rw-r--r--   0 zach       (502) staff       (20)     3882 2023-06-14 03:23:24.000000 thefriendlystars-0.1.2/setup.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-14 23:28:21.057121 thefriendlystars-0.1.2/thefriendlystars/
+-rw-r--r--   0 zach       (502) staff       (20)       19 2023-06-14 03:17:18.000000 thefriendlystars-0.1.2/thefriendlystars/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     8108 2023-06-14 23:27:19.000000 thefriendlystars-0.1.2/thefriendlystars/gaia.py
+-rw-r--r--   0 zach       (502) staff       (20)      306 2023-06-14 03:17:18.000000 thefriendlystars-0.1.2/thefriendlystars/imports.py
+-rwxr-xr-x   0 zach       (502) staff       (20)       62 2023-06-14 23:08:06.000000 thefriendlystars-0.1.2/thefriendlystars/version.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-14 23:28:21.058691 thefriendlystars-0.1.2/thefriendlystars.egg-info/
+-rw-r--r--   0 zach       (502) staff       (20)      616 2023-06-14 23:28:20.000000 thefriendlystars-0.1.2/thefriendlystars.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)      374 2023-06-14 23:28:21.000000 thefriendlystars-0.1.2/thefriendlystars.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (502) staff       (20)        1 2023-06-14 23:28:20.000000 thefriendlystars-0.1.2/thefriendlystars.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (502) staff       (20)        1 2023-06-14 03:19:56.000000 thefriendlystars-0.1.2/thefriendlystars.egg-info/not-zip-safe
+-rw-r--r--   0 zach       (502) staff       (20)      204 2023-06-14 23:28:20.000000 thefriendlystars-0.1.2/thefriendlystars.egg-info/requires.txt
+-rw-r--r--   0 zach       (502) staff       (20)       17 2023-06-14 23:28:20.000000 thefriendlystars-0.1.2/thefriendlystars.egg-info/top_level.txt
```

### Comparing `thefriendlystars-0.1.1/LICENSE` & `thefriendlystars-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thefriendlystars-0.1.1/PKG-INFO` & `thefriendlystars-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thefriendlystars
-Version: 0.1.1
+Version: 0.1.2
 Summary:  Python toolkit for making finder charts with catalogs that cover a small patch of the sky.
 Home-page: https://github.com/zkbt/thefriendlystars/
 Author: Zach Berta-Thompson
 Author-email: zach.bertathompson@colorado.edu
 License: MIT
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `thefriendlystars-0.1.1/README.md` & `thefriendlystars-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `thefriendlystars-0.1.1/setup.py` & `thefriendlystars-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `thefriendlystars-0.1.1/thefriendlystars/gaia.py` & `thefriendlystars-0.1.2/thefriendlystars/gaia.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from .imports import *
 from astropy.coordinates import SkyCoord
 from astroquery.gaia import Gaia
 from astropy.table import QTable
 from astropy.visualization import quantity_support
 import warnings 
 
+# for information about available queries + columns, see 
+# https://astroquery.readthedocs.io/en/latest/gaia/gaia.html
+
 # set a high row limit to allow lots of stars in crowded fields
 Gaia.ROW_LIMIT = 50000
 Gaia.MAIN_GAIA_TABLE = "gaiaedr3.gaia_source"
 gaia_epoch = 2016.0
 
 # Gaia filter transformations from
 # https://gea.esac.esa.int/archive/documentation/GDR2/Data_processing/chap_cu5pho/sec_cu5pho_calibr/ssec_cu5pho_PhotTransf.html
@@ -118,22 +121,23 @@
         raise ValueError('Sorry! `center` must be a string or SkyCoord.')
 
     # get the data from the archive
     job = Gaia.cone_search_async(
         center_skycoord,
         radius,
         columns=[
+            "source_id",
             "ra",
             "dec",
             "phot_g_mean_mag",
             "phot_rp_mean_mag",
             "phot_bp_mean_mag",
-            "parallax",
-            "pmra",
-            "pmdec",
+            "parallax", "parallax_error",
+            "pmra", "pmra_error",
+            "pmdec", "pmdec_error"
         ],
     )
     results = job.get_results()
 
     # tidy up the table and convert to quantities
     table = QTable(results)
     table.rename_columns(
```

### Comparing `thefriendlystars-0.1.1/thefriendlystars.egg-info/PKG-INFO` & `thefriendlystars-0.1.2/thefriendlystars.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thefriendlystars
-Version: 0.1.1
+Version: 0.1.2
 Summary:  Python toolkit for making finder charts with catalogs that cover a small patch of the sky.
 Home-page: https://github.com/zkbt/thefriendlystars/
 Author: Zach Berta-Thompson
 Author-email: zach.bertathompson@colorado.edu
 License: MIT
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

