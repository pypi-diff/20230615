# Comparing `tmp/threedi-modelchecker-2.2.3.tar.gz` & `tmp/threedi-modelchecker-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedi-modelchecker-2.2.3.tar", last modified: Wed Jun 14 09:05:35 2023, max compression
+gzip compressed data, was "threedi-modelchecker-2.2.4.tar", last modified: Thu Jun 15 14:02:24 2023, max compression
```

## Comparing `threedi-modelchecker-2.2.3.tar` & `threedi-modelchecker-2.2.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:05:35.454912 threedi-modelchecker-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    20385 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-14 09:05:35.454912 threedi-modelchecker-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-14 09:05:35.454912 threedi-modelchecker-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:05:35.442912 threedi-modelchecker-2.2.3/threedi_modelchecker/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:05:35.450912 threedi-modelchecker-2.2.3/threedi_modelchecker/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/checks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/checks/cross_section_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/checks/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/checks/geo_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    32998 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/checks/other.py
--rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/checks/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/checks/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    94957 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/exporters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:05:35.450912 threedi-modelchecker-2.2.3/threedi_modelchecker/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/interfaces/raster_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/interfaces/raster_interface_gdal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/interfaces/raster_interface_rasterio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/model_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:05:35.454912 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:05:35.454912 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:05:24.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-14 09:05:25.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/data/empty_v4.sqlite
--rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-06-14 09:05:25.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    27178 2023-06-14 09:05:25.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15823 2023-06-14 09:05:25.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_cross_section_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-14 09:05:25.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    22881 2023-06-14 09:05:25.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_other.py
--rw-r--r--   0 runner    (1001) docker     (123)    14685 2023-06-14 09:05:25.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-14 09:05:25.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-14 09:05:25.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-14 09:05:25.000000 threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_model_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:05:35.446912 threedi-modelchecker-2.2.3/threedi_modelchecker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-14 09:05:35.000000 threedi-modelchecker-2.2.3/threedi_modelchecker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-14 09:05:35.000000 threedi-modelchecker-2.2.3/threedi_modelchecker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:05:35.000000 threedi-modelchecker-2.2.3/threedi_modelchecker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-14 09:05:35.000000 threedi-modelchecker-2.2.3/threedi_modelchecker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:05:35.000000 threedi-modelchecker-2.2.3/threedi_modelchecker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-14 09:05:35.000000 threedi-modelchecker-2.2.3/threedi_modelchecker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-14 09:05:35.000000 threedi-modelchecker-2.2.3/threedi_modelchecker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:02:24.055057 threedi-modelchecker-2.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    20498 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-15 14:02:24.055057 threedi-modelchecker-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-15 14:02:24.055057 threedi-modelchecker-2.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:02:24.047057 threedi-modelchecker-2.2.4/threedi_modelchecker/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:02:24.051057 threedi-modelchecker-2.2.4/threedi_modelchecker/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/checks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/checks/cross_section_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/checks/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/checks/geo_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32995 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/checks/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/checks/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/checks/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94957 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/exporters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:02:24.051057 threedi-modelchecker-2.2.4/threedi_modelchecker/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/interfaces/raster_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/interfaces/raster_interface_gdal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/interfaces/raster_interface_rasterio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/model_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:02:24.051057 threedi-modelchecker-2.2.4/threedi_modelchecker/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:02:24.055057 threedi-modelchecker-2.2.4/threedi_modelchecker/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:02:11.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-15 14:02:12.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/tests/data/empty_v4.sqlite
+-rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-06-15 14:02:12.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27178 2023-06-15 14:02:12.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/tests/test_checks_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15823 2023-06-15 14:02:12.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/tests/test_checks_cross_section_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-15 14:02:12.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/tests/test_checks_factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22881 2023-06-15 14:02:12.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/tests/test_checks_other.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14685 2023-06-15 14:02:12.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/tests/test_checks_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-15 14:02:12.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/tests/test_checks_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-15 14:02:12.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/tests/test_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-15 14:02:12.000000 threedi-modelchecker-2.2.4/threedi_modelchecker/tests/test_model_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:02:24.051057 threedi-modelchecker-2.2.4/threedi_modelchecker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-15 14:02:24.000000 threedi-modelchecker-2.2.4/threedi_modelchecker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-15 14:02:24.000000 threedi-modelchecker-2.2.4/threedi_modelchecker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:02:24.000000 threedi-modelchecker-2.2.4/threedi_modelchecker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-15 14:02:24.000000 threedi-modelchecker-2.2.4/threedi_modelchecker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:02:23.000000 threedi-modelchecker-2.2.4/threedi_modelchecker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-15 14:02:24.000000 threedi-modelchecker-2.2.4/threedi_modelchecker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 14:02:24.000000 threedi-modelchecker-2.2.4/threedi_modelchecker.egg-info/top_level.txt
```

### Comparing `threedi-modelchecker-2.2.3/CHANGES.rst` & `threedi-modelchecker-2.2.4/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 Changelog of threedi-modelchecker
 =================================
 
 
+2.2.4 (2023-06-15)
+------------------
+
+- Fixed check 204; it now only applies to broad crested weirs/orifices.
+
+
 2.2.3 (2023-06-14)
 ------------------
 
 - Ignore tiny floating-point deviations in RasterGridSizeCheck (check 798).
 
 - Add check 327 to make sure vegetation drag is only used if the friction type is Chezy.
```

### Comparing `threedi-modelchecker-2.2.3/LICENSE` & `threedi-modelchecker-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/PKG-INFO` & `threedi-modelchecker-2.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-modelchecker
-Version: 2.2.3
+Version: 2.2.4
 Summary: Checks validity of a 3Di schematisation
 Home-page: https://github.com/nens/threedi-modelchecker
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `threedi-modelchecker-2.2.3/README.rst` & `threedi-modelchecker-2.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/setup.py` & `threedi-modelchecker-2.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/checks/base.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/checks/base.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/checks/cross_section_definitions.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/checks/cross_section_definitions.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/checks/factories.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/checks/factories.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/checks/geo_query.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/checks/geo_query.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/checks/other.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/checks/other.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
         self.min_distance = min_distance
         self.recommended_distance = recommended_distance
 
     def get_invalid(self, session):
         start_node = aliased(models.ConnectionNode)
         end_node = aliased(models.ConnectionNode)
         q = (
-            Query(self.column.class_)
+            self.to_check(session)
             .join(start_node, self.start_node)
             .join(end_node, self.end_node)
             .filter(
                 distance(start_node.the_geom, end_node.the_geom) < self.min_distance
             )
         )
         return list(q.with_session(session).all())
```

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/checks/raster.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/checks/raster.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/checks/timeseries.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/checks/timeseries.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/config.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/config.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/exporters.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/exporters.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/interfaces/raster_interface.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/interfaces/raster_interface.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/interfaces/raster_interface_gdal.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/interfaces/raster_interface_gdal.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/interfaces/raster_interface_rasterio.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/interfaces/raster_interface_rasterio.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/model_checks.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/model_checks.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/scripts.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/scripts.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/tests/conftest.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/tests/factories.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/tests/factories.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_base.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/tests/test_checks_base.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_cross_section_definitions.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/tests/test_checks_cross_section_definitions.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_factories.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/tests/test_checks_factories.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_other.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/tests/test_checks_other.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_raster.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/tests/test_checks_raster.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_checks_timeseries.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/tests/test_checks_timeseries.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_exporters.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker/tests/test_model_checks.py` & `threedi-modelchecker-2.2.4/threedi_modelchecker/tests/test_model_checks.py`

 * *Files identical despite different names*

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker.egg-info/PKG-INFO` & `threedi-modelchecker-2.2.4/threedi_modelchecker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-modelchecker
-Version: 2.2.3
+Version: 2.2.4
 Summary: Checks validity of a 3Di schematisation
 Home-page: https://github.com/nens/threedi-modelchecker
 Author: Nelen & Schuurmans
 Author-email: info@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `threedi-modelchecker-2.2.3/threedi_modelchecker.egg-info/SOURCES.txt` & `threedi-modelchecker-2.2.4/threedi_modelchecker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

