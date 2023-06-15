# Comparing `tmp/openet-sims-0.1.0rc1.tar.gz` & `tmp/openet-sims-0.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openet-sims-0.1.0rc1.tar", last modified: Wed Jun 14 20:34:39 2023, max compression
+gzip compressed data, was "openet-sims-0.1.0rc3.tar", last modified: Thu Jun 15 00:24:41 2023, max compression
```

## Comparing `openet-sims-0.1.0rc1.tar` & `openet-sims-0.1.0rc3.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-06-14 20:34:39.291262 openet-sims-0.1.0rc1/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    11357 2023-06-14 16:39:53.000000 openet-sims-0.1.0rc1/LICENSE.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      132 2023-05-01 17:38:14.000000 openet-sims-0.1.0rc1/MANIFEST.in
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    22340 2023-06-14 20:34:39.291350 openet-sims-0.1.0rc1/PKG-INFO
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     8858 2023-06-14 16:39:49.000000 openet-sims-0.1.0rc1/README.rst
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-06-14 20:34:39.288384 openet-sims-0.1.0rc1/openet/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       65 2023-05-01 17:38:14.000000 openet-sims-0.1.0rc1/openet/__init__.py
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-06-14 20:34:39.289291 openet-sims-0.1.0rc1/openet/sims/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      130 2023-05-01 17:38:14.000000 openet-sims-0.1.0rc1/openet/sims/__init__.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    36377 2023-06-07 21:15:27.000000 openet-sims-0.1.0rc1/openet/sims/collection.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    11462 2023-05-01 17:38:14.000000 openet-sims-0.1.0rc1/openet/sims/data.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    22434 2023-05-01 17:38:14.000000 openet-sims-0.1.0rc1/openet/sims/image.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    27145 2023-05-01 17:38:14.000000 openet-sims-0.1.0rc1/openet/sims/interpolate.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    21889 2023-05-01 17:38:14.000000 openet-sims-0.1.0rc1/openet/sims/model.py
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-06-14 20:34:39.290457 openet-sims-0.1.0rc1/openet/sims/tests/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     1024 2023-05-01 17:38:14.000000 openet-sims-0.1.0rc1/openet/sims/tests/conftest.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     5542 2023-05-01 17:38:14.000000 openet-sims-0.1.0rc1/openet/sims/tests/ee_wb_valid.csv
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2916 2023-05-01 17:38:14.000000 openet-sims-0.1.0rc1/openet/sims/tests/test_a_utils.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3087 2023-05-01 17:38:14.000000 openet-sims-0.1.0rc1/openet/sims/tests/test_b_data.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    23963 2023-06-07 14:31:44.000000 openet-sims-0.1.0rc1/openet/sims/tests/test_b_model.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    22566 2023-05-01 17:38:14.000000 openet-sims-0.1.0rc1/openet/sims/tests/test_c_image.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    27551 2023-06-07 15:09:29.000000 openet-sims-0.1.0rc1/openet/sims/tests/test_d_collection.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    19719 2023-05-01 17:38:14.000000 openet-sims-0.1.0rc1/openet/sims/tests/test_d_interpolate.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3194 2023-05-01 17:38:14.000000 openet-sims-0.1.0rc1/openet/sims/utils.py
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-06-14 20:34:39.291145 openet-sims-0.1.0rc1/openet_sims.egg-info/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    22340 2023-06-14 20:34:39.000000 openet-sims-0.1.0rc1/openet_sims.egg-info/PKG-INFO
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      690 2023-06-14 20:34:39.000000 openet-sims-0.1.0rc1/openet_sims.egg-info/SOURCES.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        1 2023-06-14 20:34:39.000000 openet-sims-0.1.0rc1/openet_sims.egg-info/dependency_links.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       61 2023-06-14 20:34:39.000000 openet-sims-0.1.0rc1/openet_sims.egg-info/requires.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        7 2023-06-14 20:34:39.000000 openet-sims-0.1.0rc1/openet_sims.egg-info/top_level.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     1008 2023-06-14 20:34:29.000000 openet-sims-0.1.0rc1/pyproject.toml
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       63 2023-06-14 20:34:39.291544 openet-sims-0.1.0rc1/setup.cfg
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-06-15 00:24:41.424334 openet-sims-0.1.0rc3/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    11357 2023-06-14 16:39:53.000000 openet-sims-0.1.0rc3/LICENSE.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    22361 2023-06-15 00:24:41.424198 openet-sims-0.1.0rc3/PKG-INFO
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     8858 2023-06-14 16:39:49.000000 openet-sims-0.1.0rc3/README.rst
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-06-15 00:24:41.421570 openet-sims-0.1.0rc3/openet/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       65 2023-05-01 17:38:14.000000 openet-sims-0.1.0rc3/openet/__init__.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-06-15 00:24:41.422430 openet-sims-0.1.0rc3/openet/sims/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      107 2023-06-14 20:56:10.000000 openet-sims-0.1.0rc3/openet/sims/__init__.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    36506 2023-06-14 23:08:04.000000 openet-sims-0.1.0rc3/openet/sims/collection.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    10984 2023-06-14 23:42:28.000000 openet-sims-0.1.0rc3/openet/sims/data.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    22376 2023-06-14 22:51:20.000000 openet-sims-0.1.0rc3/openet/sims/image.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    27163 2023-06-15 00:11:23.000000 openet-sims-0.1.0rc3/openet/sims/interpolate.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    21843 2023-06-14 22:45:46.000000 openet-sims-0.1.0rc3/openet/sims/model.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-06-15 00:24:41.423422 openet-sims-0.1.0rc3/openet/sims/tests/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     1024 2023-05-01 17:38:14.000000 openet-sims-0.1.0rc3/openet/sims/tests/conftest.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     5542 2023-05-01 17:38:14.000000 openet-sims-0.1.0rc3/openet/sims/tests/ee_wb_valid.csv
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2918 2023-06-14 23:06:07.000000 openet-sims-0.1.0rc3/openet/sims/tests/test_a_utils.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3087 2023-05-01 17:38:14.000000 openet-sims-0.1.0rc3/openet/sims/tests/test_b_data.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    23942 2023-06-14 23:26:42.000000 openet-sims-0.1.0rc3/openet/sims/tests/test_b_model.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    22531 2023-06-15 00:14:16.000000 openet-sims-0.1.0rc3/openet/sims/tests/test_c_image.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    27833 2023-06-14 23:50:39.000000 openet-sims-0.1.0rc3/openet/sims/tests/test_d_collection.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    19623 2023-06-14 23:22:26.000000 openet-sims-0.1.0rc3/openet/sims/tests/test_d_interpolate.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3186 2023-06-14 23:07:50.000000 openet-sims-0.1.0rc3/openet/sims/utils.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-06-15 00:24:41.423989 openet-sims-0.1.0rc3/openet_sims.egg-info/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    22361 2023-06-15 00:24:41.000000 openet-sims-0.1.0rc3/openet_sims.egg-info/PKG-INFO
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      668 2023-06-15 00:24:41.000000 openet-sims-0.1.0rc3/openet_sims.egg-info/SOURCES.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        1 2023-06-15 00:24:41.000000 openet-sims-0.1.0rc3/openet_sims.egg-info/dependency_links.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      130 2023-06-15 00:24:41.000000 openet-sims-0.1.0rc3/openet_sims.egg-info/requires.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        7 2023-06-15 00:24:41.000000 openet-sims-0.1.0rc3/openet_sims.egg-info/top_level.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     1195 2023-06-15 00:24:36.000000 openet-sims-0.1.0rc3/pyproject.toml
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       38 2023-06-15 00:24:41.424375 openet-sims-0.1.0rc3/setup.cfg
```

### Comparing `openet-sims-0.1.0rc1/LICENSE.txt` & `openet-sims-0.1.0rc3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openet-sims-0.1.0rc1/PKG-INFO` & `openet-sims-0.1.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openet-sims
-Version: 0.1.0rc1
+Version: 0.1.0rc3
 Summary: Earth Engine based SIMS Model
 Author-email: Alberto Guzman <aguzman@csumb.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -208,14 +208,15 @@
 Project-URL: Homepage, https://github.com/Open-ET/openet-sims
 Keywords: SIMS,OpenET,Earth Engine,evapotranspiration
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE.txt
 
 ===================
 OpenET - SIMS Model
 ===================
 
 |version| |build|
```

### Comparing `openet-sims-0.1.0rc1/README.rst` & `openet-sims-0.1.0rc3/README.rst`

 * *Files identical despite different names*

### Comparing `openet-sims-0.1.0rc1/openet/sims/collection.py` & `openet-sims-0.1.0rc3/openet/sims/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import copy
 import datetime
-import pprint
+# import pprint
 
-from dateutil.relativedelta import *
+from dateutil.relativedelta import relativedelta
 import ee
 import openet.core.interpolate
 # TODO: import utils from openet.core
 # import openet.core.utils as utils
 
 from . import utils
 from .image import Image
-# Importing to get version number, is there a better way?
-import openet.sims
+
+try:
+    from importlib import metadata
+except ImportError:  # for Python<3.8
+    import importlib_metadata as metadata
 
 
 def lazy_property(fn):
     """Decorator that makes a property lazy-evaluated
 
     https://stevenloria.com/lazy-properties/
     """
@@ -29,33 +32,33 @@
     return _lazy_property
 
 
 class Collection():
     """"""
 
     def __init__(
-            self,
-            collections,
-            start_date,
-            end_date,
-            geometry,
-            variables=None,
-            cloud_cover_max=70,
-            et_reference_source=None,
-            et_reference_band=None,
-            et_reference_factor=None,
-            et_reference_resample=None,
-            filter_args=None,
-            model_args=None,
-            # model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
-            #             'et_reference_band': 'eto',
-            #             'et_reference_factor': 0.85,
-            #             'et_reference_resample': 'nearest},
-            # **kwargs
-        ):
+        self,
+        collections,
+        start_date,
+        end_date,
+        geometry,
+        variables=None,
+        cloud_cover_max=70,
+        et_reference_source=None,
+        et_reference_band=None,
+        et_reference_factor=None,
+        et_reference_resample=None,
+        filter_args=None,
+        model_args=None,
+        # model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
+        #             'et_reference_band': 'eto',
+        #             'et_reference_factor': 0.85,
+        #             'et_reference_resample': 'nearest},
+        # **kwargs
+    ):
         """Earth Engine based SIMS ETcb Image Collection object
 
         Parameters
         ----------
         collections : list, str
             GEE satellite image collection IDs.
         start_date : str
@@ -531,24 +534,24 @@
         interp_start_date = interp_start_dt.date().isoformat()
         interp_end_date = interp_end_dt.date().isoformat()
 
         # Update model_args if et_reference parameters were passed to interpolate
         # Intentionally using model_args (instead of self.et_reference_source, etc.) in
         #   this function since model_args is passed to Image class in _build()
         # if 'et' in variables or 'et_reference' in variables:
-        if ('et_reference_source' in kwargs.keys() and \
+        if ('et_reference_source' in kwargs.keys() and
                 kwargs['et_reference_source'] is not None):
             self.model_args['et_reference_source'] = kwargs['et_reference_source']
-        if ('et_reference_band' in kwargs.keys() and \
+        if ('et_reference_band' in kwargs.keys() and
                 kwargs['et_reference_band'] is not None):
             self.model_args['et_reference_band'] = kwargs['et_reference_band']
-        if ('et_reference_factor' in kwargs.keys() and \
+        if ('et_reference_factor' in kwargs.keys() and
                 kwargs['et_reference_factor'] is not None):
             self.model_args['et_reference_factor'] = kwargs['et_reference_factor']
-        if ('et_reference_resample' in kwargs.keys() and \
+        if ('et_reference_resample' in kwargs.keys() and
                 kwargs['et_reference_resample'] is not None):
             self.model_args['et_reference_resample'] = kwargs['et_reference_resample']
 
         # Check that all et_reference parameters were set
         for et_reference_param in ['et_reference_source', 'et_reference_band',
                                    'et_reference_factor']:
             if et_reference_param not in self.model_args.keys():
@@ -621,15 +624,16 @@
             # The following is needed because the aggregate collection can be
             #   empty if there are no scenes in the target date range but there
             #   are scenes in the interpolation date range.
             # Without this the count image will not be built but the other
             #   bands will be which causes a non-homogenous image collection.
             aggregate_coll = aggregate_coll.merge(
                 ee.Image.constant(0).rename(['mask'])
-                    .set({'system:time_start': ee.Date(start_date).millis()}))
+                .set({'system:time_start': ee.Date(start_date).millis()})
+            )
 
         # Including count/mask causes problems in interpolate.daily() function.
         # Issues with mask being an int but the values need to be double.
         # Casting the mask band to a double would fix this problem also.
         if 'mask' in interp_vars:
             interp_vars.remove('mask')
 
@@ -656,16 +660,18 @@
             daily_coll = daily_coll.map(compute_et)
 
         interp_properties = {
             'cloud_cover_max': self.cloud_cover_max,
             'collections': ', '.join(self.collections),
             'interp_days': interp_days,
             'interp_method': interp_method,
-            'model_name': openet.sims.MODEL_NAME,
-            'model_version': openet.sims.__version__,
+            'model_name': metadata.metadata('openet-sims')['Name'],
+            'model_version': metadata.metadata('openet-sims')['Version'],
+            # 'model_name': openet.sims.MODEL_NAME,
+            # 'model_version': openet.sims.__version__,
         }
         interp_properties.update(self.model_args)
 
         def aggregate_image(agg_start_date, agg_end_date, date_format):
             """Aggregate the daily images within the target date range
 
             Parameters
```

### Comparing `openet-sims-0.1.0rc1/openet/sims/data.py` & `openet-sims-0.1.0rc3/openet/sims/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,224 +6,101 @@
     DOI 10.1007/s00271-009-0182-z
 """
 
 # Scaling factor to use in EE remap function since it only work with integers
 int_scalar = 100
 
 cdl = {
-    # Vines
-    69:  {'crop_class': 2, 'h_max': 2, 'm_l': 1.5, 'fr_mid': 0.65,
-          'fr_end': 0.43, 'ls_start': 205, 'ls_stop': 265,
-          'name': 'Wine Grapes'},
-    78:  {'crop_class': 2, 'h_max': 2, 'm_l': 1.5, 'fr_mid': 0.95,
-          'fr_end': 0.51, 'ls_start': 205, 'ls_stop': 265,
-          'name': 'Grapes (table/raisin)'},
-
-    # Trees
-    66:  {'crop_class': 3, 'h_max': 3, 'm_l': 2, 'fr_mid': 0.95,
-          'fr_end': 0.75, 'ls_start': 270, 'ls_stop': 300,
-          'name': 'Cherries'},
-    67:  {'crop_class': 3, 'h_max': 3, 'm_l': 1.5, 'fr_mid': 1.0,
-          'fr_end': 0.71, 'ls_start': 270, 'ls_stop': 300,
-          'name': 'Peaches'},
-    68:  {'crop_class': 3, 'h_max': 3, 'm_l': 2, 'fr_mid': 0.95,
-          'fr_end': 0.75, 'ls_start': 270, 'ls_stop': 300,
-          'name': 'Apples'},
-    71:  {'crop_class': 3, 'h_max': 4, 'm_l': 1.5, 'fr_mid': 0.89,
-          'fr_end': 0.63, 'ls_start': 270, 'ls_stop': 300,
-          'name': 'Other Tree Crops'},
-    72:  {'crop_class': 3, 'h_max': 2.5, 'm_l': 1.5, 'fr_mid': 0.71,
-          'fr_end': 0.94, 'ls_start': 270, 'ls_stop': 365,
-          'name': 'Citrus'},
-    74:  {'crop_class': 3, 'h_max': 4, 'm_l': 1.5, 'fr_mid': 0.89,
-          'fr_end': 0.80, 'ls_start': 270, 'ls_stop': 300,
-          'name': 'Pecans'},
-    75:  {'crop_class': 3, 'h_max': 4, 'm_l': 1.5, 'fr_mid': 0.81,
-          'fr_end': 0.59, 'ls_start': 270, 'ls_stop': 300,
-          'name': 'Almonds'},
-    76:  {'crop_class': 3, 'h_max': 5, 'm_l': 1.5, 'fr_mid': 0.9,
-          'fr_end': 0.52, 'ls_start': 250, 'ls_stop': 280,
-          'name': 'Walnuts'},
-    77:  {'crop_class': 3, 'h_max': 3, 'm_l': 2, 'fr_mid': 0.95,
-          'fr_end': 0.75, 'ls_start': 270, 'ls_stop': 300,
-          'name': 'Pears'},
-    204: {'crop_class': 3, 'h_max': 3, 'm_l': 1.5, 'fr_mid': 0.81,
-          'fr_end': 0.57, 'ls_start': 200, 'ls_stop': 240,
-          'name': 'Pistachios'},
-    210: {'crop_class': 3, 'h_max': 3, 'm_l': 1.5, 'fr_mid': 0.95,
-          'fr_end': 0.71, 'ls_start': 270, 'ls_stop': 300,
-          'name': 'Prunes'},
-    211: {'crop_class': 3, 'h_max': 4, 'm_l': 1.5, 'fr_mid': 0.48,
-          'fr_end': 0.46, 'ls_start': 240, 'ls_stop': 330,
-          'name': 'Olives'},
-    212: {'crop_class': 3, 'h_max': 2.5, 'm_l': 1.5, 'fr_mid': 0.71,
-          'fr_end': 0.94, 'ls_start': 270, 'ls_stop': 365,
-          'name': 'Oranges'},
-    215: {'crop_class': 3, 'h_max': 3, 'm_l': 2, 'fr_mid': 0.81,
-          'fr_end': 0.73, 'ls_start': 270, 'ls_stop': 365,
-          'name': 'Avocados'},
-    218: {'crop_class': 3, 'h_max': 3, 'm_l': 1.5, 'fr_mid': 0.95,
-          'fr_end': 0.75, 'ls_start': 270, 'ls_stop': 300,
-          'name': 'Nectarines'},
-    220: {'crop_class': 3, 'h_max': 3, 'm_l': 1.5, 'fr_mid': 0.95,
-          'fr_end': 0.71, 'ls_start': 270, 'ls_stop': 300,
-          'name': 'Plums'},
-    223: {'crop_class': 3, 'h_max': 3, 'm_l': 1.5, 'fr_mid': 0.95,
-          'fr_end': 0.71, 'ls_start': 270, 'ls_stop': 300,
-          'name': 'Apricots'},
-
     # Field crops
-    49:  {'crop_class': 1, 'h_max': 0.4, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Onions'},
-    206: {'crop_class': 1, 'h_max': 0.3, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Carrots'},
-    208: {'crop_class': 1, 'h_max': 0.3, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Garlic'},
-    214: {'crop_class': 1, 'h_max': 0.3, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Broccoli'},
-    227: {'crop_class': 1, 'h_max': 0.3, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Lettuce'},
-    243: {'crop_class': 1, 'h_max': 0.4, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Cabbage'},
-    244: {'crop_class': 1, 'h_max': 0.4, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Cauliflower'},
-    245: {'crop_class': 1, 'h_max': 0.6, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Celery'},
-    246: {'crop_class': 1, 'h_max': 0.3, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Radishes'},
+    49: {'crop_class': 1, 'h_max': 0.4, 'm_l': 2, 'fr_mid': 1, 'name': 'Onions'},
+    206: {'crop_class': 1, 'h_max': 0.3, 'm_l': 2, 'fr_mid': 1, 'name': 'Carrots'},
+    208: {'crop_class': 1, 'h_max': 0.3, 'm_l': 2, 'fr_mid': 1, 'name': 'Garlic'},
+    214: {'crop_class': 1, 'h_max': 0.3, 'm_l': 2, 'fr_mid': 1, 'name': 'Broccoli'},
+    227: {'crop_class': 1, 'h_max': 0.3, 'm_l': 2, 'fr_mid': 1, 'name': 'Lettuce'},
+    243: {'crop_class': 1, 'h_max': 0.4, 'm_l': 2, 'fr_mid': 1, 'name': 'Cabbage'},
+    244: {'crop_class': 1, 'h_max': 0.4, 'm_l': 2, 'fr_mid': 1, 'name': 'Cauliflower'},
+    245: {'crop_class': 1, 'h_max': 0.6, 'm_l': 2, 'fr_mid': 1, 'name': 'Celery'},
+    246: {'crop_class': 1, 'h_max': 0.3, 'm_l': 2, 'fr_mid': 1, 'name': 'Radishes'},
 
     # Vegetables, solanum family
-    54:  {'crop_class': 1, 'h_max': 0.6, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Tomatoes'},
-    248: {'crop_class': 1, 'h_max': 0.8, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Eggplants'},
+    54: {'crop_class': 1, 'h_max': 0.6, 'm_l': 2, 'fr_mid': 1, 'name': 'Tomatoes'},
+    248: {'crop_class': 1, 'h_max': 0.8, 'm_l': 2, 'fr_mid': 1, 'name': 'Eggplants'},
 
     # Vegetables, cucurb family
-    48:  {'crop_class': 1, 'h_max': 0.4, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Watermelons'},
-    209: {'crop_class': 1, 'h_max': 0.3, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Cantaloupes'},
-    213: {'crop_class': 1, 'h_max': 0.4, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Honeydew Melons'},
-    222: {'crop_class': 1, 'h_max': 0.3, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Squash'},
-    228: {'crop_class': 1, 'h_max': 0.3, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Dbl Crop Triticale/Corn'},
-    229: {'crop_class': 1, 'h_max': 0.4, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Pumpkins'},
+    48: {'crop_class': 1, 'h_max': 0.4, 'm_l': 2, 'fr_mid': 1, 'name': 'Watermelons'},
+    209: {'crop_class': 1, 'h_max': 0.3, 'm_l': 2, 'fr_mid': 1, 'name': 'Cantaloupes'},
+    213: {'crop_class': 1, 'h_max': 0.4, 'm_l': 2, 'fr_mid': 1, 'name': 'Honeydew Melons'},
+    222: {'crop_class': 1, 'h_max': 0.3, 'm_l': 2, 'fr_mid': 1, 'name': 'Squash'},
+    228: {'crop_class': 1, 'h_max': 0.3, 'm_l': 2, 'fr_mid': 1, 'name': 'Dbl Crop Triticale/Corn'},
+    229: {'crop_class': 1, 'h_max': 0.4, 'm_l': 2, 'fr_mid': 1, 'name': 'Pumpkins'},
 
     # Vegetables, other
-    47: {'crop_class': 1, 'h_max': 0.37, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Misc Vegs & Fruits'},
+    47: {'crop_class': 1, 'h_max': 0.37, 'm_l': 2, 'fr_mid': 1, 'name': 'Misc Vegs & Fruits'},
 
     # Roots & tubers
-    41:  {'crop_class': 1, 'h_max': 0.5, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Sugarbeets'},
-    43:  {'crop_class': 1, 'h_max': 0.6, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Potatoes'},
-    46:  {'crop_class': 1, 'h_max': 0.4, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Sweet Potatoes'},
-    247: {'crop_class': 1, 'h_max': 0.6, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Turnips'},
+    41: {'crop_class': 1, 'h_max': 0.5, 'm_l': 2, 'fr_mid': 1, 'name': 'Sugarbeets'},
+    43: {'crop_class': 1, 'h_max': 0.6, 'm_l': 2, 'fr_mid': 1, 'name': 'Potatoes'},
+    46: {'crop_class': 1, 'h_max': 0.4, 'm_l': 2, 'fr_mid': 1, 'name': 'Sweet Potatoes'},
+    247: {'crop_class': 1, 'h_max': 0.6, 'm_l': 2, 'fr_mid': 1, 'name': 'Turnips'},
 
     # Legumes
-    5:  {'crop_class': 1, 'h_max': 0.5, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Soybeans'},
-    10: {'crop_class': 1, 'h_max': 0.4, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Peanuts'},
-    30: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Speltz'},
-    42: {'crop_class': 1, 'h_max': 0.4, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Dry Beans'},
-    51: {'crop_class': 1, 'h_max': 0.4, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Chick Peas'},
-    52: {'crop_class': 1, 'h_max': 0.5, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Lentils'},
-    53: {'crop_class': 1, 'h_max': 0.5, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Peas'},
-    224: {'crop_class': 1, 'h_max': 0.5, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Vetch'},
+    5: {'crop_class': 1, 'h_max': 0.5, 'm_l': 2, 'fr_mid': 1, 'name': 'Soybeans'},
+    10: {'crop_class': 1, 'h_max': 0.4, 'm_l': 2, 'fr_mid': 1, 'name': 'Peanuts'},
+    30: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1, 'name': 'Speltz'},
+    42: {'crop_class': 1, 'h_max': 0.4, 'm_l': 2, 'fr_mid': 1, 'name': 'Dry Beans'},
+    51: {'crop_class': 1, 'h_max': 0.4, 'm_l': 2, 'fr_mid': 1, 'name': 'Chick Peas'},
+    52: {'crop_class': 1, 'h_max': 0.5, 'm_l': 2, 'fr_mid': 1, 'name': 'Lentils'},
+    53: {'crop_class': 1, 'h_max': 0.5, 'm_l': 2, 'fr_mid': 1, 'name': 'Peas'},
+    224: {'crop_class': 1, 'h_max': 0.5, 'm_l': 2, 'fr_mid': 1, 'name': 'Vetch'},
 
     # Perennial vegetables or fruit
-    14:  {'crop_class': 1, 'h_max': 0.7, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Mint'},
-    50:  {'crop_class': 1, 'h_max': 0.3, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Cucumbers'},
-    207: {'crop_class': 1, 'h_max': 0.5, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Asparagus'},
-    216: {'crop_class': 1, 'h_max': 0.7, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Peppers'},
-    221: {'crop_class': 1, 'h_max': 0.2, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Strawberries'},
+    14: {'crop_class': 1, 'h_max': 0.7, 'm_l': 2, 'fr_mid': 1, 'name': 'Mint'},
+    50: {'crop_class': 1, 'h_max': 0.3, 'm_l': 2, 'fr_mid': 1, 'name': 'Cucumbers'},
+    207: {'crop_class': 1, 'h_max': 0.5, 'm_l': 2, 'fr_mid': 1, 'name': 'Asparagus'},
+    216: {'crop_class': 1, 'h_max': 0.7, 'm_l': 2, 'fr_mid': 1, 'name': 'Peppers'},
+    221: {'crop_class': 1, 'h_max': 0.2, 'm_l': 2, 'fr_mid': 1, 'name': 'Strawberries'},
 
     # Fiber
-    2:  {'crop_class': 1, 'h_max': 1.35, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Cotton'},
-    6:  {'crop_class': 1, 'h_max': 2.0, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Sunflower'},
-    31: {'crop_class': 1, 'h_max': 0.6, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Canola'},
-    32: {'crop_class': 1, 'h_max': 1.2, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Flaxseed'},
-    33: {'crop_class': 1, 'h_max': 0.8, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Safflower'},
-    45: {'crop_class': 1, 'h_max': 3.0, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Sugarcane'},
+    2: {'crop_class': 1, 'h_max': 1.35, 'm_l': 2, 'fr_mid': 1, 'name': 'Cotton'},
+    6: {'crop_class': 1, 'h_max': 2.0, 'm_l': 2, 'fr_mid': 1, 'name': 'Sunflower'},
+    31: {'crop_class': 1, 'h_max': 0.6, 'm_l': 2, 'fr_mid': 1, 'name': 'Canola'},
+    32: {'crop_class': 1, 'h_max': 1.2, 'm_l': 2, 'fr_mid': 1, 'name': 'Flaxseed'},
+    33: {'crop_class': 1, 'h_max': 0.8, 'm_l': 2, 'fr_mid': 1, 'name': 'Safflower'},
+    45: {'crop_class': 1, 'h_max': 3.0, 'm_l': 2, 'fr_mid': 1, 'name': 'Sugarcane'},
 
     # Cereal
-    1:  {'crop_class': 1, 'h_max': 2.0, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Corn'},
-    4:  {'crop_class': 1, 'h_max': 1.5, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Sorghum'},
-    12: {'crop_class': 1, 'h_max': 1.5, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Sweet Corn'},
-    21: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Barley'},
-    22: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Durum Wheat'},
-    23: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Spring Wheat'},
-    24: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Winter Wheat'},
-    25: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Other Small Grains'},
-    26: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Dbl Crop WinWht/Soybeans'},
-    28: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Oats'},
-    29: {'crop_class': 1, 'h_max': 1.5, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Millet'},
-    32: {'crop_class': 1, 'h_max': 1.2, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Flaxseed'},
-    34: {'crop_class': 1, 'h_max': 0.6, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Rape Seed'},
-    35: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Mustard'},
-    39: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Buckwheat'},
-    56: {'crop_class': 1, 'h_max': 5.0, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Hops'},
+    1: {'crop_class': 1, 'h_max': 2.0, 'm_l': 2, 'fr_mid': 1,  'name': 'Corn'},
+    4: {'crop_class': 1, 'h_max': 1.5, 'm_l': 2, 'fr_mid': 1, 'name': 'Sorghum'},
+    12: {'crop_class': 1, 'h_max': 1.5, 'm_l': 2, 'fr_mid': 1, 'name': 'Sweet Corn'},
+    21: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1, 'name': 'Barley'},
+    22: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1, 'name': 'Durum Wheat'},
+    23: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1, 'name': 'Spring Wheat'},
+    24: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1, 'name': 'Winter Wheat'},
+    25: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1, 'name': 'Other Small Grains'},
+    26: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1, 'name': 'Dbl Crop WinWht/Soybeans'},
+    28: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1, 'name': 'Oats'},
+    29: {'crop_class': 1, 'h_max': 1.5, 'm_l': 2, 'fr_mid': 1, 'name': 'Millet'},
+    # CGM - Repeat of crop 32 in fiber section
+    #   Same values so commenting out for now
+    # 32: {'crop_class': 1, 'h_max': 1.2, 'm_l': 2, 'fr_mid': 1, 'name': 'Flaxseed'},
+    34: {'crop_class': 1, 'h_max': 0.6, 'm_l': 2, 'fr_mid': 1, 'name': 'Rape Seed'},
+    35: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1, 'name': 'Mustard'},
+    39: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1, 'name': 'Buckwheat'},
+    56: {'crop_class': 1, 'h_max': 5.0, 'm_l': 2, 'fr_mid': 1, 'name': 'Hops'},
 
     # Rice
-    3: {'crop_class': 5, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1,
-        'name': 'Rice'},
+    3: {'crop_class': 5, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1, 'name': 'Rice'},
 
     # Forage
-    27: {'crop_class': 1, 'h_max': 0.3, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Rye'},
-    36: {'crop_class': 1, 'h_max': 0.7, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Alfalfa'},
-    58: {'crop_class': 1, 'h_max': 0.6, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Clover/Wildflowers'},
-    37: {'crop_class': 1, 'h_max': 0.5, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Other Hay/Non Alfalfa'},
-    38: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1,
-         'name': 'Camelina'},
-    205: {'crop_class': 1, 'h_max': 0.65, 'm_l': 2, 'fr_mid': 1,
-          'name': 'Triticale'},
+    27: {'crop_class': 1, 'h_max': 0.3, 'm_l': 2, 'fr_mid': 1, 'name': 'Rye'},
+    36: {'crop_class': 1, 'h_max': 0.7, 'm_l': 2, 'fr_mid': 1, 'name': 'Alfalfa'},
+    58: {'crop_class': 1, 'h_max': 0.6, 'm_l': 2, 'fr_mid': 1, 'name': 'Clover/Wildflowers'},
+    37: {'crop_class': 1, 'h_max': 0.5, 'm_l': 2, 'fr_mid': 1, 'name': 'Other Hay/Non Alfalfa'},
+    38: {'crop_class': 1, 'h_max': 1.0, 'm_l': 2, 'fr_mid': 1, 'name': 'Camelina'},
+    205: {'crop_class': 1, 'h_max': 0.65, 'm_l': 2, 'fr_mid': 1, 'name': 'Triticale'},
 
     # Crops without custom coefficients
     11: {'crop_class': 1, 'name': 'Tobacco'},
     13: {'crop_class': 1, 'name': 'Pop or Orn Corn'},
     44: {'crop_class': 1, 'name': 'Other Crops'},
     55: {'crop_class': 1, 'name': 'Caneberries'},
     57: {'crop_class': 1, 'name': 'Herbs'},
@@ -245,14 +122,94 @@
     240: {'crop_class': 1, 'name': 'Dbl Crop Soybeans/Oats'},
     241: {'crop_class': 1, 'name': 'Dbl Crop Corn/Soybeans'},
     242: {'crop_class': 1, 'name': 'Blueberries'},
     249: {'crop_class': 1, 'name': 'Gourds'},
     250: {'crop_class': 1, 'name': 'Cranberries'},
     254: {'crop_class': 1, 'name': 'Dbl Crop Barley/Soybeans'},
 
+    # Vines
+    69: {
+        'crop_class': 2, 'h_max': 2, 'm_l': 1.5, 'fr_mid': 0.65, 'fr_end': 0.43,
+        'ls_start': 205, 'ls_stop': 265, 'name': 'Wine Grapes'
+    },
+    78: {
+        'crop_class': 2, 'h_max': 2, 'm_l': 1.5, 'fr_mid': 0.95, 'fr_end': 0.51,
+        'ls_start': 205, 'ls_stop': 265, 'name': 'Grapes (table/raisin)'
+    },
+
+    # Trees
+    66: {
+        'crop_class': 3, 'h_max': 3, 'm_l': 2, 'fr_mid': 0.95, 'fr_end': 0.75,
+        'ls_start': 270, 'ls_stop': 300, 'name': 'Cherries',
+    },
+    67: {
+        'crop_class': 3, 'h_max': 3, 'm_l': 1.5, 'fr_mid': 1.0, 'fr_end': 0.71,
+        'ls_start': 270, 'ls_stop': 300, 'name': 'Peaches',
+    },
+    68: {
+        'crop_class': 3, 'h_max': 3, 'm_l': 2, 'fr_mid': 0.95, 'fr_end': 0.75,
+        'ls_start': 270, 'ls_stop': 300, 'name': 'Apples',
+    },
+    71: {
+        'crop_class': 3, 'h_max': 4, 'm_l': 1.5, 'fr_mid': 0.89, 'fr_end': 0.63,
+        'ls_start': 270, 'ls_stop': 300, 'name': 'Other Tree Crops'
+    },
+    72: {
+        'crop_class': 3, 'h_max': 2.5, 'm_l': 1.5, 'fr_mid': 0.71, 'fr_end': 0.94,
+        'ls_start': 270, 'ls_stop': 365, 'name': 'Citrus',
+    },
+    74: {
+        'crop_class': 3, 'h_max': 4, 'm_l': 1.5, 'fr_mid': 0.89, 'fr_end': 0.80,
+        'ls_start': 270, 'ls_stop': 300, 'name': 'Pecans',
+    },
+    75: {
+        'crop_class': 3, 'h_max': 4, 'm_l': 1.5, 'fr_mid': 0.81, 'fr_end': 0.59,
+        'ls_start': 270, 'ls_stop': 300, 'name': 'Almonds',
+    },
+    76: {
+        'crop_class': 3, 'h_max': 5, 'm_l': 1.5, 'fr_mid': 0.9, 'fr_end': 0.52,
+        'ls_start': 250, 'ls_stop': 280, 'name': 'Walnuts',
+    },
+    77: {
+        'crop_class': 3, 'h_max': 3, 'm_l': 2, 'fr_mid': 0.95, 'fr_end': 0.75,
+        'ls_start': 270, 'ls_stop': 300, 'name': 'Pears',
+    },
+    204: {
+        'crop_class': 3, 'h_max': 3, 'm_l': 1.5, 'fr_mid': 0.81, 'fr_end': 0.57,
+        'ls_start': 200, 'ls_stop': 240, 'name': 'Pistachios',
+    },
+    210: {
+        'crop_class': 3, 'h_max': 3, 'm_l': 1.5, 'fr_mid': 0.95, 'fr_end': 0.71,
+        'ls_start': 270, 'ls_stop': 300, 'name': 'Prunes',
+    },
+    211: {
+        'crop_class': 3, 'h_max': 4, 'm_l': 1.5, 'fr_mid': 0.48, 'fr_end': 0.46,
+        'ls_start': 240, 'ls_stop': 330, 'name': 'Olives',
+    },
+    212: {
+        'crop_class': 3, 'h_max': 2.5, 'm_l': 1.5, 'fr_mid': 0.71, 'fr_end': 0.94,
+        'ls_start': 270, 'ls_stop': 365, 'name': 'Oranges',
+    },
+    215: {
+        'crop_class': 3, 'h_max': 3, 'm_l': 2, 'fr_mid': 0.81, 'fr_end': 0.73,
+        'ls_start': 270, 'ls_stop': 365, 'name': 'Avocados',
+    },
+    218: {
+        'crop_class': 3, 'h_max': 3, 'm_l': 1.5, 'fr_mid': 0.95, 'fr_end': 0.75,
+        'ls_start': 270, 'ls_stop': 300, 'name': 'Nectarines',
+    },
+    220: {
+        'crop_class': 3, 'h_max': 3, 'm_l': 1.5, 'fr_mid': 0.95, 'fr_end': 0.71,
+        'ls_start': 270, 'ls_stop': 300, 'name': 'Plums',
+    },
+    223: {
+        'crop_class': 3, 'h_max': 3, 'm_l': 1.5, 'fr_mid': 0.95, 'fr_end': 0.71,
+        'ls_start': 270, 'ls_stop': 300, 'name': 'Apricots',
+    },
+
     # Tree crops without custom coefficients
     70: {'crop_class': 3, 'name': 'Christmas Trees'},
     217: {'crop_class': 3, 'name': 'Pomegranates'},
 
     # Fallow
     61: {'crop_class': 6, 'name': 'Fallow/Idle Cropland'},
```

### Comparing `openet-sims-0.1.0rc1/openet/sims/image.py` & `openet-sims-0.1.0rc3/openet/sims/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,28 +35,28 @@
     return _lazy_property
 
 
 class Image():
     """GEE based model for computing SIMS ETcb"""
 
     def __init__(
-            self,
-            image,
-            crop_type_source='USDA/NASS/CDL',
-            crop_type_remap='CDL',
-            crop_type_kc_flag=False,
-            crop_type_annual_skip_flag=False,
-            et_reference_source=None,
-            et_reference_band=None,
-            et_reference_factor=None,
-            et_reference_resample=None,
-            mask_non_ag_flag=False,
-            water_kc_flag=True,
-            reflectance_type='SR',
-        ):
+        self,
+        image,
+        crop_type_source='USDA/NASS/CDL',
+        crop_type_remap='CDL',
+        crop_type_kc_flag=False,
+        crop_type_annual_skip_flag=False,
+        et_reference_source=None,
+        et_reference_band=None,
+        et_reference_factor=None,
+        et_reference_resample=None,
+        mask_non_ag_flag=False,
+        water_kc_flag=True,
+        reflectance_type='SR',
+    ):
         """Earth Engine based SIMS image object
 
         Parameters
         ----------
         image : ee.Image
             Required band: ndvi
             Required properties: system:time_start, system:index, system:id
@@ -135,15 +135,15 @@
 
         # Check reference ET parameters
         if et_reference_factor and not utils.is_number(et_reference_factor):
             raise ValueError('et_reference_factor must be a number')
         if et_reference_factor and self.et_reference_factor < 0:
             raise ValueError('et_reference_factor must be greater than zero')
         et_reference_resample_methods = ['nearest', 'bilinear', 'bicubic']
-        if (et_reference_resample and \
+        if (et_reference_resample and
                 et_reference_resample.lower() not in et_reference_resample_methods):
             raise ValueError('unsupported et_reference_resample method')
 
         self.reflectance_type = reflectance_type
 
         # CGM - Model class could inherit these from Image instead of passing them
         #   Could pass time_start instead of separate year and doy
```

### Comparing `openet-sims-0.1.0rc1/openet/sims/interpolate.py` & `openet-sims-0.1.0rc3/openet/sims/interpolate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 import datetime
 import logging
 
-from dateutil.relativedelta import *
+from dateutil.relativedelta import relativedelta
 import ee
 import openet.core.interpolate
 # TODO: import utils from openet.core
 # import openet.core.utils as utils
 
 from . import utils
 
 
-
-def from_scene_et_fraction(scene_coll, start_date, end_date, variables,
-                           interp_args, model_args, t_interval, use_joins=False,
-                           _interp_vars=['et_fraction', 'ndvi']):
+def from_scene_et_fraction(
+    scene_coll,
+    start_date,
+    end_date,
+    variables,
+    interp_args,
+    model_args,
+    t_interval,
+    use_joins=False,
+    _interp_vars=['et_fraction', 'ndvi'],
+):
     """Interpolate from a precomputed collection of Landast ET fraction scenes
 
     Parameters
     ----------
     scene_coll : ee.ImageCollection
         Non-daily 'et_fraction' images that will be interpolated.
     start_date : str
@@ -169,16 +176,16 @@
     #     # raise ValueError('et_reference_resample was not set')
 
     # check if collection already has et_reference provided
     # if not, get it from the collection
     if type(et_reference_source) is str and et_reference_source.lower() == 'provided':
         daily_et_ref_coll = scene_coll.map(lambda x: x.select('et_reference'))
     elif type(et_reference_source) is str:
-        # Assume a string source is an single image collection ID
-        #   not an list of collection IDs or ee.ImageCollection
+        # Assume a string source is a single image collection ID
+        #   not a list of collection IDs or ee.ImageCollection
         daily_et_ref_coll = ee.ImageCollection(et_reference_source) \
             .filterDate(start_date, end_date) \
             .select([et_reference_band], ['et_reference'])
     # elif isinstance(et_reference_source, computedobject.ComputedObject):
     #     # Interpret computed objects as image collections
     #     daily_et_ref_coll = ee.ImageCollection(et_reference_source) \
     #         .filterDate(self.start_date, self.end_date) \
@@ -218,32 +225,36 @@
     # Filter scene collection to the interpolation range
     # This probably isn't needed since scene_coll was built to this range
     scene_coll = scene_coll.filterDate(interp_start_date, interp_end_date)
 
     # For count, compute the composite/mosaic image for the mask band only
     if 'count' in variables:
         aggregate_coll = openet.core.interpolate.aggregate_to_daily(
-            image_coll = scene_coll.select(['mask']),
-            start_date=start_date, end_date=end_date)
+            image_coll=scene_coll.select(['mask']),
+            start_date=start_date,
+            end_date=end_date
+        )
         # The following is needed because the aggregate collection can be
         #   empty if there are no scenes in the target date range but there
         #   are scenes in the interpolation date range.
         # Without this the count image will not be built but the other
         #   bands will be which causes a non-homogeneous image collection.
         aggregate_coll = aggregate_coll.merge(
             ee.Image.constant(0).rename(['mask'])
-                .set({'system:time_start': ee.Date(start_date).millis()}))
+            .set({'system:time_start': ee.Date(start_date).millis()})
+        )
 
     # Interpolate to a daily time step
     # NOTE: the daily function is not computing ET (ETf x ETo)
     #   but is returning the target (ETo) band
     daily_coll = openet.core.interpolate.daily(
         target_coll=daily_et_ref_coll,
         source_coll=scene_coll.select(interp_vars),
-        interp_method=interp_method, interp_days=interp_days,
+        interp_method=interp_method,
+        interp_days=interp_days,
         use_joins=use_joins,
         compute_product=False,
     )
 
     if estimate_soil_evaporation:
         daily_coll = daily_ke(daily_coll, model_args, **interp_args)
 
@@ -437,19 +448,19 @@
     precip_source : str, optional
         GEE data source for gridded precipitation data, default is gridMET.
     precip_band : str, option
         GEE Image band that contains gridded precipitaiton data, default is
         'pr', which is the band for gridMET.
     fc_source : str, ee.Image
         GEE Image of soil field capacity values
-    fc_band : str 
+    fc_band : str
         Name of the band in `fc_source` that contains field capacity values
     wp_source : str, ee.Image
         GEE Image of soil permanent wilting point values
-    wp_band : str 
+    wp_band : str
         Name of the band in `wp_source` that contains wilting point values
 
     Returns
     -------
     ee.ImageCollection
 
     """
@@ -461,26 +472,25 @@
     wilting_point = ee.Image(wp_source).select(wp_band)
 
     # Available water content (mm)
     awc = field_capacity.subtract(wilting_point)
 
     # Fraction of wetting
     # Setting to 1 for now (precip), but could be lower for irrigation
-    # CGM - Not used below
-    frac_wet = ee.Image(1)
+    # CGM - Not used below, commenting out for now
+    # frac_wet = ee.Image(1)
 
     # Depth of evaporable zone
     # Set to 10 cm
     z_e = 0.1
 
     # Total evaporable water (mm)
     # Allen et al. 1998 eqn 73
     tew = field_capacity.expression(
-        '10 * (b() - 0.5 * wp) * z_e',
-        {'wp': wilting_point, 'z_e': z_e}
+        '10 * (b() - 0.5 * wp) * z_e', {'wp': wilting_point, 'z_e': z_e}
     )
 
     # Readily evaporable water (mm)
     rew = awc.expression('0.8 + 54.4 * b() / 100')
     rew = rew.where(rew.gt(tew), tew)
 
     # Coefficients for skin layer retention, Allen (2011)
@@ -495,155 +505,168 @@
     frac_day_evap = ee.Image(0.5)
 
     # Get precip collection
     daily_pr_coll = ee.ImageCollection(precip_source).select(precip_band)
 
     # Assume soil is at field capacity to start
     # i.e. depletion = 0
-    #init_de = ee.Image(ee.Image(0.0).select([0], ['de']))
-    #init_de_rew = ee.Image(ee.Image(0.0).select([0], ['de_rew']))
+    # init_de = ee.Image(ee.Image(0.0).select([0], ['de']))
+    # init_de_rew = ee.Image(ee.Image(0.0).select([0], ['de_rew']))
     init_de = tew.select([0], ['de'])
     init_de_rew = rew.select([0], ['de_rew'])
-    init_c_eff = init_de \
-        .expression(
-            "C0 + C1 * (1 - b() / TEW)",
-            {'C0': c0, 'C1': c1, 'TEW': tew}) \
-        .min(1) \
+    init_c_eff = (
+        init_de.expression("C0 + C1 * (1 - b() / TEW)", {'C0': c0, 'C1': c1, 'TEW': tew})
+        .min(1)
         .select([0], ['c_eff'])
+    )
 
     # Create list to hold water balance rasters when iterating over collection
     # Doesn't seem like you can create an empty list in ee?
     init_img = ee.Image([init_de, init_de_rew, init_c_eff])
     init_img_list = ee.ImageCollection([init_img]).toList(1)
 
     # Convert interp collection to list
     interp_list = daily_coll.toList(daily_coll.size())
     # Is list guaranteed to have right order?
     # (Seems to be fine in initial testing.)
-    #interp_list = interp_list.sort(ee.List(['system:index']))
+    # interp_list = interp_list.sort(ee.List(['system:index']))
 
     # Perform daily water balance update
     def water_balance_step(img, wb_coll):
         # Explicit cast ee.Image
         prev_img = ee.Image(ee.List(wb_coll).get(-1))
         curr_img = ee.Image(img)
 
         # Make precip image with bands for today and tomorrow
         # CGM - The current image is selected by filtering to the previous day
         #   since the Landsat image time is ~18 UTC but the precip start time
         #   is likely 0 UTC or 6 UTC (for GRIDMET)
         # CGM the
         curr_date = curr_img.date()
         curr_precip = ee.Image(
-            daily_pr_coll.filterDate(curr_date.advance(-1, 'day'), curr_date).first())
+            daily_pr_coll.filterDate(curr_date.advance(-1, 'day'), curr_date).first()
+        )
         next_precip = ee.Image(
-            daily_pr_coll.filterDate(curr_date, curr_date.advance(1, 'day')).first())
-        # curr_precip = ee.Image(daily_pr_coll
-        #     .filterDate(curr_date, curr_date.advance(1, 'day')).first()).rename('precip')
-        # next_precip = ee.Image(daily_pr_coll
-        #     .filterDate(curr_date.advance(1, 'day'), curr_date.advance(2, 'day')).first())
-        precip_img = ee.Image([curr_precip, next_precip]) \
-            .rename(['current', 'next'])
+            daily_pr_coll.filterDate(curr_date, curr_date.advance(1, 'day')).first()
+        )
+        # curr_precip = ee.Image(
+        #     daily_pr_coll.filterDate(curr_date, curr_date.advance(1, 'day')).first()
+        # )
+        # next_precip = ee.Image(
+        #     daily_pr_coll.filterDate(curr_date.advance(1, 'day'), curr_date.advance(2, 'day'))
+        #     .first()
+        # )
+        precip_img = ee.Image([curr_precip, next_precip]).rename(['current', 'next'])
 
         # Fraction of day stage 1 evap
         # Allen 2011, eq 12
-        ft = rew \
-            .expression(
+        ft = (
+            rew.expression(
                 '(b() - de_rew_prev) / (ke_max * eto)',
                 {
                     'de_rew_prev': prev_img.select('de_rew'),
                     'rew': rew,
                     'ke_max': ke_max,
                     'eto': curr_img.select('et_reference')
-                }) \
-            .clamp(0.0, 1.0) \
+                }
+            )
+            .clamp(0.0, 1.0)
             .rename('ft')
+        )
 
         # Soil evap reduction coeff, FAO 56
-        kr = tew.expression(
+        kr = (
+            tew.expression(
                 "(b() - de_prev) / (b() - rew)",
-                {'de_prev': prev_img.select('de'), 'rew': rew}) \
-            .clamp(0.0, 1.0) \
+                {'de_prev': prev_img.select('de'), 'rew': rew}
+            )
+            .clamp(0.0, 1.0)
             .rename('kr')
-        
+        )
+
         de_prev = prev_img.select('de').rename('de_prev')
 
         # precip only for now
         # irrigation might have lower f_w
         fw = prev_img.select('de').multiply(0).add(1).rename('fw')
         low_few = fw.multiply(0).add(0.01).rename('low_few')
         fc = curr_img.select('ndvi').multiply(1.26).subtract(0.18).rename('fc')
         few = fw.min(fc.multiply(-1).add(1)).max(low_few).rename('few')
 
         # Soil evap coeff, FAO 56
-        ke = ft.expression(
-                "(b() + (1 - b()) * kr) * ke_max",
-                {'kr': kr, 'ke_max': ke_max}) \
+        ke = (
+            ft.expression("(b() + (1 - b()) * kr) * ke_max", {'kr': kr, 'ke_max': ke_max})
+            .min(few.multiply(ke_max))
             .rename('ke')
-        ke = ke.min(few.multiply(ke_max))
+        )
 
         # Dual crop coefficient: Kc = Kcb + Ke
-        #kc = ke.add(curr_img.select('et_fraction')).rename('kc')
+        # kc = ke.add(curr_img.select('et_fraction')).rename('kc')
 
         # Crop ET (note that Kc in other parts of code refers to *basal*
         # crop coeff (Kcb))
-        #etc = kc.multiply(curr_img.select('et_reference')).rename('etc')
+        # etc = kc.multiply(curr_img.select('et_reference')).rename('etc')
 
         # ETe - soil evaporation
         ete = ke.multiply(curr_img.select('et_reference')).rename('ete')
 
         # CGM - Why not just add ke to et_frac and clamp the result?
         #   What does the extra .where call do?
-        et_frac = ee.Image(img).select(['et_fraction']) 
-        etof = et_frac.where(et_frac.lte(1.15), et_frac.add(ke).clamp(0, 1.15)) \
+        et_frac = ee.Image(img).select(['et_fraction'])
+        etof = (
+            et_frac.where(et_frac.lte(1.15), et_frac.add(ke).clamp(0, 1.15))
             .rename('et_fraction')
+        )
 
         # Depletion, FAO 56
-        de = prev_img.select('de') \
+        de = (
+            prev_img.select('de')
             .subtract(
                 frac_day_evap
-                    .multiply(ee.Image(precip_img.select('next')))
-                    .add(
-                        ee.Image(1)
-                            .subtract(frac_day_evap)
-                            .multiply(precip_img.select('current')))
-            ) \
-            .add(ete.divide(few.select('few'))) \
-            .select([0], ['de']).rename('de')
+                .multiply(ee.Image(precip_img.select('next')))
+                .add(
+                    ee.Image(1)
+                    .subtract(frac_day_evap)
+                    .multiply(precip_img.select('current')))
+            )
+            .add(ete.divide(few.select('few')))
+            .select([0], ['de'])
+        )
 
         # Can't have negative depletion
         de = de.min(tew).max(0)
 
         # Stage 1 depletion (REW)
         # Allen 2011
-        de_rew = prev_img.select('de_rew') \
+        de_rew = (
+            prev_img.select('de_rew')
             .subtract(
                 frac_day_evap
-                    .multiply(precip_img.select('next'))
-                    .add(
-                        ee.Image(1)
-                        .subtract(frac_day_evap)
-                        .multiply(precip_img.select('current'))
-                    )
-                    .multiply(prev_img.select('c_eff'))
-            ) \
-            .add(ete.divide(few.select('few'))) \
-            .select([0], ['de_rew']).rename('de_rew')
+                .multiply(precip_img.select('next'))
+                .add(
+                    ee.Image(1)
+                    .subtract(frac_day_evap)
+                    .multiply(precip_img.select('current'))
+                )
+                .multiply(prev_img.select('c_eff'))
+            )
+            .add(ete.divide(few.select('few')))
+            .select([0], ['de_rew'])
+        )
 
         # Can't have negative depletion
         de_rew = de_rew.min(rew).max(0)
 
         # Efficiency of skin layer
         # Allen 2011, eq 15
-        c_eff = de \
-            .expression(
-                "c0 + c1 * (1 - b() / tew)",
-                {'c0': c0, 'c1': c1, 'tew': tew}) \
-            .min(1) \
+        c_eff = (
+            de.expression("c0 + c1 * (1 - b() / tew)", {'c0': c0, 'c1': c1, 'tew': tew})
+            .min(1)
             .select([0], ['c_eff'])
+        )
 
         # Make image to add to list
         # CGM - I removed the duplicate de, de_rew, and ft bands
         #   Are they needed?
         new_day_img = ee.Image(
             curr_img.addBands(
                 ee.Image([de, de_rew, c_eff, ke, kr, ft, de_prev, ete,
```

### Comparing `openet-sims-0.1.0rc1/openet/sims/model.py` & `openet-sims-0.1.0rc3/openet/sims/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pprint
+# import pprint
 
 import ee
 
 from . import data
 from . import utils
 
 
@@ -21,26 +21,26 @@
 #     return _lazy_property
 
 
 class Model():
     """GEE based model for computing SIMS ETcb"""
 
     def __init__(
-            self,
-            # CGM - Switch to ee.Date or time_start instead?
-            year,
-            doy,
-            crop_type_source='USDA/NASS/CDL',
-            crop_type_remap='CDL',
-            crop_type_kc_flag=False,
-            crop_type_annual_skip_flag=False,
-            mask_non_ag_flag=True,
-            water_kc_flag=True,
-            reflectance_type='SR',
-        ):
+        self,
+        # CGM - Switch to ee.Date or time_start instead?
+        year,
+        doy,
+        crop_type_source='USDA/NASS/CDL',
+        crop_type_remap='CDL',
+        crop_type_kc_flag=False,
+        crop_type_annual_skip_flag=False,
+        mask_non_ag_flag=True,
+        water_kc_flag=True,
+        reflectance_type='SR',
+    ):
         """Earth Engine based SIMS model object
 
         Parameters
         ----------
         year : ee.Number
         doy : ee.Number
             Day of year
```

### Comparing `openet-sims-0.1.0rc1/openet/sims/tests/conftest.py` & `openet-sims-0.1.0rc3/openet/sims/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openet-sims-0.1.0rc1/openet/sims/tests/ee_wb_valid.csv` & `openet-sims-0.1.0rc3/openet/sims/tests/ee_wb_valid.csv`

 * *Files identical despite different names*

### Comparing `openet-sims-0.1.0rc1/openet/sims/tests/test_a_utils.py` & `openet-sims-0.1.0rc3/openet/sims/tests/test_a_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime
-import pprint
+# import pprint
 
 import ee
 import pytest
 
 import openet.sims.utils as utils
 
 
@@ -88,12 +88,12 @@
 
 
 def test_millis():
     assert utils.millis(datetime.datetime(2015, 7, 13)) == 1436745600000
 
 
 def test_valid_date():
-    assert utils.valid_date('2015-07-13') == True
-    assert utils.valid_date('2015-02-30') == False
-    assert utils.valid_date('20150713') == False
-    assert utils.valid_date('07/13/2015') == False
-    assert utils.valid_date('07-13-2015', '%m-%d-%Y') == True
+    assert utils.valid_date('2015-07-13') is True
+    assert utils.valid_date('2015-02-30') is False
+    assert utils.valid_date('20150713') is False
+    assert utils.valid_date('07/13/2015') is False
+    assert utils.valid_date('07-13-2015', '%m-%d-%Y') is True
```

### Comparing `openet-sims-0.1.0rc1/openet/sims/tests/test_b_data.py` & `openet-sims-0.1.0rc3/openet/sims/tests/test_b_data.py`

 * *Files identical despite different names*

### Comparing `openet-sims-0.1.0rc1/openet/sims/tests/test_b_model.py` & `openet-sims-0.1.0rc3/openet/sims/tests/test_b_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pprint
+# import pprint
 
 import ee
 import pytest
 
 import openet.sims.data as data
 import openet.sims.model as model
 import openet.sims.utils as utils
@@ -82,15 +82,15 @@
 
 
 def test_crop_data_image_default_nodata():
     output = utils.constant_image_value(model.crop_data_image(
         param_name='crop_class',
         crop_type=ee.Image.constant(-999).rename(['crop_class']),
         crop_data={9: {'crop_class': 10}}))
-    assert output['crop_class'] == None
+    assert output['crop_class'] is None
 
 
 def test_Model_init_default_parameters():
     m = default_model_obj()
     assert m.crop_type_source == f'USDA/NASS/CDL/{YEAR}'
     assert m.crop_type_remap == 'CDL'
     assert m.reflectance_type == 'SR'
@@ -570,17 +570,19 @@
         h = crop_profile['h_max'] * min((fc / 0.7), 1)
         fr = 1.0
     elif crop_profile['crop_class'] == 3 or crop_profile['crop_class'] == 2:
         # Set fr based on doy
         if doy < crop_profile['ls_start']:
             fr = crop_profile['fr_mid']
         elif crop_profile['ls_start'] <= doy and doy <= crop_profile['ls_stop']:
-            fr = crop_profile['fr_mid'] - ((doy - crop_profile['ls_start'])\
-                                           / (crop_profile['ls_stop'] - crop_profile['ls_start'])\
-                                           * (crop_profile['fr_mid'] - crop_profile['fr_end']))
+            fr = crop_profile["fr_mid"] - (
+                (doy - crop_profile["ls_start"])
+                / (crop_profile["ls_stop"] - crop_profile["ls_start"])
+                * (crop_profile["fr_mid"] - crop_profile["fr_end"])
+            )
         elif doy > crop_profile['ls_stop']:
             fr = crop_profile['fr_end']
 
         # Set h based on crop class
         if crop_profile['crop_class'] == 3:
             if fc > 0.5:
                 h = crop_profile['h_max']
@@ -607,17 +609,17 @@
 
 @pytest.mark.parametrize(
     'ndvi, doy, crop_type_num',
     [
         # 1.26 * 0.8 - 0.18 = 0.828
         # ((0.828 ** 2) * -0.4771) + (1.4047 * 0.828) + 0.15 = 0.9859994736
         [0.8, 174, 1],
-        #[1.0, 200, 3],
-        #[0.5, 200, 3],
-        #[0.1, 200, 3],
+        # [1.0, 200, 3],
+        # [0.5, 200, 3],
+        # [0.1, 200, 3],
         [1.0, 200, 1],
         [0.5, 200, 1],
         [0.1, 200, 1],
         [1.0, 200, 2],
         [0.5, 250, 2],
         [0.1, 300, 2],
         [1.0, 200, 69],
```

### Comparing `openet-sims-0.1.0rc1/openet/sims/tests/test_c_image.py` & `openet-sims-0.1.0rc3/openet/sims/tests/test_c_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 # import logging
-import pprint
+# import pprint
 
 import ee
 import pytest
 
 import openet.sims as sims
 import openet.sims.utils as utils
 # TODO: import utils from openet.core
@@ -95,18 +95,18 @@
         water_kc_flag=water_kc_flag,
         # reflectance_type=reflectance_type,
     ))
 
 
 def test_Image_init_default_parameters():
     m = sims.Image(image=default_image())
-    assert m.et_reference_source == None
-    assert m.et_reference_band == None
-    assert m.et_reference_factor == None
-    assert m.et_reference_resample == None
+    assert m.et_reference_source is None
+    assert m.et_reference_band is None
+    assert m.et_reference_factor is None
+    assert m.et_reference_resample is None
     # assert m.crop_type_source == 'USDA/NASS/CDL'
     # assert m.crop_type_remap == 'CDL'
     # assert m.crop_type_kc_flag == False
     # assert m.crop_type_annual_skip_flag == False
     # assert m.mask_non_ag_flag == False
     assert m.reflectance_type == 'SR'
 
@@ -337,24 +337,23 @@
 def test_Image_calculate_variables_custom():
     variables = ['ndvi']
     output = utils.getinfo(default_image_obj().calculate(variables))
     assert set([x['id'] for x in output['bands']]) == set(variables)
 
 
 def test_Image_calculate_variables_all():
-    variables = ['et', 'et_fraction', 'et_reference', 'fc', 'kc', 'mask',
-                 'ndvi', 'time']
+    variables = ['et', 'et_fraction', 'et_reference', 'fc', 'kc', 'mask', 'ndvi', 'time']
     output = utils.getinfo(default_image_obj().calculate(variables=variables))
     assert set([x['id'] for x in output['bands']]) == set(variables)
 
 
 def test_Image_from_landsat_c1_sr_default_image():
     """Test that the classmethod is returning a class object"""
     output = sims.Image.from_landsat_c1_sr(input_image())
-    assert type(output) == type(default_image_obj())
+    assert isinstance(type(output), type(default_image_obj()))
 
 
 @pytest.mark.parametrize(
     'image_id',
     [
         'LANDSAT/LC08/C01/T1_SR/LC08_044033_20170716',
         'LANDSAT/LE07/C01/T1_SR/LE07_044033_20170708',
@@ -367,16 +366,15 @@
     output = utils.getinfo(sims.Image.from_landsat_c1_sr(image_id).ndvi)
     assert output['properties']['system:index'] == image_id.split('/')[-1]
 
 
 def test_Image_from_landsat_c1_sr_image():
     """Test instantiating the class from a Landsat ee.Image"""
     image_id = 'LANDSAT/LC08/C01/T1_SR/LC08_044033_20170716'
-    output = utils.getinfo(sims.Image.from_landsat_c1_sr(
-        ee.Image(image_id)).ndvi)
+    output = utils.getinfo(sims.Image.from_landsat_c1_sr(ee.Image(image_id)).ndvi)
     assert output['properties']['system:index'] == image_id.split('/')[-1]
 
 
 def test_Image_from_landsat_c1_sr_kc():
     """Test if ET fraction can be built from a Landsat images"""
     image_id = 'LANDSAT/LC08/C01/T1_SR/LC08_044033_20170716'
     output = utils.getinfo(sims.Image.from_landsat_c1_sr(image_id).kc)
@@ -403,15 +401,15 @@
     image_id = 'LANDSAT/LC08/C01/T1_SR/LC08_044033_20170716'
     assert sims.Image.from_landsat_c1_sr(image_id).reflectance_type == 'SR'
 
 
 def test_Image_from_landsat_c1_toa_default_image():
     """Test that the classmethod is returning a class object"""
     output = sims.Image.from_landsat_c1_toa(input_image())
-    assert type(output) == type(default_image_obj())
+    assert isinstance(type(output), type(default_image_obj()))
 
 
 @pytest.mark.parametrize(
     'image_id',
     [
         'LANDSAT/LC08/C01/T1_TOA/LC08_044033_20170716',
         'LANDSAT/LE07/C01/T1_TOA/LE07_044033_20170708',
@@ -427,16 +425,15 @@
     output = utils.getinfo(sims.Image.from_landsat_c1_toa(image_id).ndvi)
     assert output['properties']['system:index'] == image_id.split('/')[-1]
 
 
 def test_Image_from_landsat_c1_toa_image():
     """Test instantiating the class from a Landsat ee.Image"""
     image_id = 'LANDSAT/LC08/C01/T1_TOA/LC08_044033_20170716'
-    output = utils.getinfo(sims.Image.from_landsat_c1_toa(
-        ee.Image(image_id)).ndvi)
+    output = utils.getinfo(sims.Image.from_landsat_c1_toa(ee.Image(image_id)).ndvi)
     assert output['properties']['system:index'] == image_id.split('/')[-1]
 
 
 def test_Image_from_landsat_c1_toa_kc():
     """Test if ET fraction can be built from a Landsat images"""
     image_id = 'LANDSAT/LC08/C01/T1_TOA/LC08_044033_20170716'
     output = utils.getinfo(sims.Image.from_landsat_c1_toa(image_id).kc)
@@ -463,15 +460,15 @@
     image_id = 'LANDSAT/LC08/C01/T1_TOA/LC08_044033_20170716'
     assert sims.Image.from_landsat_c1_toa(image_id).reflectance_type == 'TOA'
 
 
 def test_Image_from_landsat_c2_sr_default_image():
     """Test that the classmethod is returning a class object"""
     output = sims.Image.from_landsat_c2_sr(input_image())
-    assert type(output) == type(default_image_obj())
+    assert isinstance(type(output), type(default_image_obj()))
 
 
 @pytest.mark.parametrize(
     'image_id',
     [
         # 'LANDSAT/LT04/C02/T1_L2/LT04_044033_19830812',
         'LANDSAT/LT05/C02/T1_L2/LT05_044033_20110716',
@@ -485,16 +482,15 @@
     output = utils.getinfo(sims.Image.from_landsat_c2_sr(image_id).ndvi)
     assert output['properties']['system:index'] == image_id.split('/')[-1]
 
 
 def test_Image_from_landsat_c2_sr_image():
     """Test instantiating the class from a Landsat ee.Image"""
     image_id = 'LANDSAT/LC08/C02/T1_L2/LC08_044033_20170716'
-    output = utils.getinfo(sims.Image.from_landsat_c2_sr(
-        ee.Image(image_id)).ndvi)
+    output = utils.getinfo(sims.Image.from_landsat_c2_sr(ee.Image(image_id)).ndvi)
     assert output['properties']['system:index'] == image_id.split('/')[-1]
 
 
 def test_Image_from_landsat_c2_sr_kc():
     """Test if ET fraction can be built from a Landsat images"""
     image_id = 'LANDSAT/LC08/C02/T1_L2/LC08_044033_20170716'
     output = utils.getinfo(sims.Image.from_landsat_c2_sr(image_id).kc)
@@ -516,40 +512,39 @@
         utils.getinfo(sims.Image.from_landsat_c2_sr(ee.Image('FOO')).ndvi)
 
 
 def test_Image_from_landsat_c2_sr_scaling():
     """Test if Landsat SR images images are being scaled"""
     sr_img = ee.Image('LANDSAT/LC08/C02/T1_L2/LC08_044033_20170716')
     # CGM - These reflectances should correspond to 0.1 for RED and 0.2 for NIR
-    input_img = ee.Image.constant([10909, 10909, 10909, 14545, 10909, 10909,
-                                   44177.6, 21824, 0]) \
+    input_img = (
+        ee.Image.constant([10909, 10909, 10909, 14545, 10909, 10909, 44177.6, 21824, 0])
         .rename(['SR_B2', 'SR_B3', 'SR_B4', 'SR_B5', 'SR_B6', 'SR_B7',
-                 'ST_B10', 'QA_PIXEL', 'QA_RADSAT']) \
+                 'ST_B10', 'QA_PIXEL', 'QA_RADSAT'])
         .set({'SPACECRAFT_ID': ee.String(sr_img.get('SPACECRAFT_ID')),
               'system:id': ee.String(sr_img.get('system:id')),
               'system:index': ee.String(sr_img.get('system:index')),
               'system:time_start': ee.Number(sr_img.get('system:time_start'))})
-
-    output = utils.constant_image_value(
-        sims.Image.from_landsat_c2_sr(input_img).ndvi)
+    )
+    output = utils.constant_image_value(sims.Image.from_landsat_c2_sr(input_img).ndvi)
     assert abs(output['ndvi'] - 0.333) <= 0.01
 
 
 def test_Image_from_landsat_c2_sr_reflectance_type():
     """Test if reflectance_type property is being set"""
     image_id = 'LANDSAT/LC08/C02/T1_L2/LC08_044033_20170716'
     assert sims.Image.from_landsat_c2_sr(image_id).reflectance_type == 'SR'
 
 
 def test_Image_from_landsat_c2_sr_cloud_mask_args():
     """Test if the cloud_mask_args parameter can be set (not if it works)"""
     image_id = 'LANDSAT/LC08/C02/T1_L2/LC08_038031_20130828'
     output = sims.Image.from_landsat_c2_sr(
         image_id, cloudmask_args={'snow_flag': True, 'cirrus_flag': True})
-    assert type(output) == type(default_image_obj())
+    assert isinstance(type(output), type(default_image_obj()))
 
 
 @pytest.mark.parametrize(
     'image_id',
     [
         'LANDSAT/LC08/C01/T1_SR/LC08_044033_20170716',
         'LANDSAT/LC08/C01/T1_TOA/LC08_044033_20170716',
```

### Comparing `openet-sims-0.1.0rc1/openet/sims/tests/test_d_collection.py` & `openet-sims-0.1.0rc3/openet/sims/tests/test_d_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import pprint
+# import pprint
+import re
 
 import ee
 import pytest
 
 import openet.sims as sims
 import openet.sims.utils as utils
 # TODO: import utils from openet.core
@@ -33,14 +34,15 @@
     'et_reference_band': 'eto',
     'et_reference_factor': 0.85,
     'et_reference_resample': 'nearest',
     'model_args': {},
     'filter_args': {},
 }
 
+
 def default_coll_obj(**kwargs):
     args = default_coll_args.copy()
     args.update(kwargs)
     return sims.Collection(**args)
 
 
 def parse_scene_id(output_info):
@@ -56,19 +58,19 @@
     del args['et_reference_source']
     del args['et_reference_band']
     del args['et_reference_factor']
     del args['et_reference_resample']
     del args['variables']
 
     m = sims.Collection(**args)
-    assert m.variables == None
-    assert m.et_reference_source == None
-    assert m.et_reference_band == None
-    assert m.et_reference_factor == None
-    assert m.et_reference_resample == None
+    assert m.variables is None
+    assert m.et_reference_source is None
+    assert m.et_reference_band is None
+    assert m.et_reference_factor is None
+    assert m.et_reference_resample is None
     assert m.cloud_cover_max == 70
     assert m.model_args == {}
     assert m.filter_args == {}
     assert set(m._interp_vars) == {'ndvi', 'et_fraction'}
 
 
 def test_Collection_init_collection_str(coll_id='LANDSAT/LC08/C02/T1_L2'):
@@ -159,16 +161,15 @@
     assert parse_scene_id(output) == C02_SCENE_ID_LIST
     # Check that the variables being set in the default collection object are returned
     assert {y['id'] for x in output['features'] for y in x['bands']} == VARIABLES
 
 
 def test_Collection_build_variables_custom(variable='ndvi'):
     # Check that setting the build variables overrides the collection variables
-    output = utils.getinfo(default_coll_obj()._build(variables=[variable])
-                           .first().bandNames())
+    output = utils.getinfo(default_coll_obj()._build(variables=[variable]).first().bandNames())
     assert set(output) == {variable}
 
 
 def test_Collection_build_variables_none():
     """Test for exception if variables is set to None in method call"""
     with pytest.raises(ValueError):
         utils.getinfo(default_coll_obj(variables=None)._build(variables=None))
@@ -180,54 +181,51 @@
         utils.getinfo(default_coll_obj(variables=None)._build())
 
 
 def test_Collection_build_variables_empty_list():
     # Setting variables to an empty list should return the merged Landsat collection
     output = utils.getinfo(
         default_coll_obj(collections=C02_COLLECTIONS, variables=None)
-            ._build(variables=[]).first().bandNames())
+        ._build(variables=[]).first().bandNames()
+    )
     assert 'SR_B3' in output
 
 
 def test_Collection_build_invalid_variable_exception():
     """Test if Exception is raised for an invalid variable"""
     with pytest.raises(ValueError):
         utils.getinfo(default_coll_obj()._build(variables=['FOO']))
 
 
 def test_Collection_build_dates():
     """Check that dates passed to build function override Class dates"""
     coll_obj = default_coll_obj(start_date='2017-08-01', end_date='2017-09-01')
-    output = utils.getinfo(coll_obj._build(
-        start_date='2017-07-16', end_date='2017-07-17'))
+    output = utils.getinfo(coll_obj._build(start_date='2017-07-16', end_date='2017-07-17'))
     assert parse_scene_id(output) == ['LC08_044033_20170716']
 
 
 def test_Collection_build_landsat_c1_toa():
     """Test if the Landsat TOA (non RT) collections can be built"""
-    coll_obj = default_coll_obj(
-        collections=['LANDSAT/LC08/C01/T1_TOA', 'LANDSAT/LE07/C01/T1_TOA'])
+    coll_obj = default_coll_obj(collections=['LANDSAT/LC08/C01/T1_TOA', 'LANDSAT/LE07/C01/T1_TOA'])
     output = utils.getinfo(coll_obj._build())
     assert parse_scene_id(output) == C01_SCENE_ID_LIST
     assert VARIABLES == {y['id'] for x in output['features'] for y in x['bands']}
 
 
 def test_Collection_build_landsat_c1_sr():
     """Test if the Landsat SR collections can be built"""
-    coll_obj = default_coll_obj(
-        collections=['LANDSAT/LC08/C01/T1_SR', 'LANDSAT/LE07/C01/T1_SR'])
+    coll_obj = default_coll_obj(collections=['LANDSAT/LC08/C01/T1_SR', 'LANDSAT/LE07/C01/T1_SR'])
     output = utils.getinfo(coll_obj._build())
     assert parse_scene_id(output) == C01_SCENE_ID_LIST
     assert {y['id'] for x in output['features'] for y in x['bands']} == VARIABLES
 
 
 def test_Collection_build_landsat_c2_sr():
     """Test if the Landsat SR collections can be built"""
-    coll_obj = default_coll_obj(
-        collections=['LANDSAT/LC08/C02/T1_L2', 'LANDSAT/LE07/C02/T1_L2'])
+    coll_obj = default_coll_obj(collections=['LANDSAT/LC08/C02/T1_L2', 'LANDSAT/LE07/C02/T1_L2'])
     output = utils.getinfo(coll_obj._build())
     assert parse_scene_id(output) == C02_SCENE_ID_LIST
     assert {y['id'] for x in output['features'] for y in x['bands']} == VARIABLES
 
 
 # CGM - Non Landsat SR collections not currently supported
 # def test_Collection_build_sentinel_toa():
@@ -246,16 +244,15 @@
     output = utils.getinfo(default_coll_obj(end_date='2017-07-24')._build())
     assert [x for x in parse_scene_id(output) if int(x[-8:]) >= 20170724] == []
 
 
 def test_Collection_build_cloud_cover():
     """Test if the cloud cover max parameter is being applied"""
     # CGM - The filtered images should probably be looked up programmatically
-    output = utils.getinfo(default_coll_obj(cloud_cover_max=0.5)._build(
-        variables=['et']))
+    output = utils.getinfo(default_coll_obj(cloud_cover_max=0.5)._build(variables=['et']))
     assert 'LE07_044033_20170724' not in parse_scene_id(output)
 
 
 @pytest.mark.parametrize(
     'collection, start_date, end_date',
     [
         ['LANDSAT/LT05/C01/T1_TOA', '2012-01-01', '2013-01-01'],
@@ -605,19 +602,19 @@
 
 def test_Collection_interpolate_output_type_default():
     """Test if output_type parameter is defaulting to float"""
     test_vars = ['et', 'et_reference', 'et_fraction', 'ndvi', 'count']
     output = utils.getinfo(default_coll_obj(variables=test_vars).interpolate())
     output = output['features'][0]['bands']
     bands = {info['id']: i for i, info in enumerate(output)}
-    assert(output[bands['et']]['data_type']['precision'] == 'float')
-    assert(output[bands['et_reference']]['data_type']['precision'] == 'float')
-    assert(output[bands['et_fraction']]['data_type']['precision'] == 'float')
-    assert(output[bands['ndvi']]['data_type']['precision'] == 'float')
-    assert(output[bands['count']]['data_type']['precision'] == 'int')
+    assert output[bands['et']]['data_type']['precision'] == 'float'
+    assert output[bands['et_reference']]['data_type']['precision'] == 'float'
+    assert output[bands['et_fraction']]['data_type']['precision'] == 'float'
+    assert output[bands['ndvi']]['data_type']['precision'] == 'float'
+    assert output[bands['count']]['data_type']['precision'] == 'int'
 
 
 def test_Collection_interpolate_custom_model_args():
     """Test passing in a model specific parameter through model_args"""
     model_args = {'crop_type_source': 'projects/openet/crop_type/annual_provisional'}
     output = utils.getinfo(default_coll_obj(model_args=model_args).interpolate())
     output = output['features'][0]['properties']
@@ -627,24 +624,31 @@
 def test_Collection_interpolate_only_interpolate_images():
     """Test if count band is returned if no images in the date range"""
     variables = {'et', 'count'}
     output = utils.getinfo(default_coll_obj(
         collections=['LANDSAT/LC08/C02/T1_L2'],
         geometry=ee.Geometry.Point(-123.623, 44.745),
         start_date='2017-04-01', end_date='2017-04-30',
-        variables=list(variables), cloud_cover_max=70).interpolate())
+        variables=list(variables), cloud_cover_max=70
+    ).interpolate())
     assert {y['id'] for x in output['features'] for y in x['bands']} == variables
 
 
+def test_Collection_interpolate_model_properties():
+    """Check that setting the model name and version from importlib.metadata works"""
+    output = utils.getinfo(default_coll_obj().interpolate().first())
+    assert output['properties']['model_name'] == 'openet-sims'
+    assert re.match('^\\d.\\d.\\d\\w+', output['properties']['model_version'])
+
+
 @pytest.mark.parametrize(
     'collections, scene_id_list',
     [
         [['LANDSAT/LC08/C01/T1_SR', 'LANDSAT/LE07/C01/T1_SR'], C01_SCENE_ID_LIST],
         [['LANDSAT/LC08/C02/T1_L2', 'LANDSAT/LE07/C02/T1_L2'], C02_SCENE_ID_LIST],
     ]
 )
 def test_Collection_get_image_ids(collections, scene_id_list):
     # get_image_ids method makes a getInfo call internally
-    output = default_coll_obj(collections=collections, variables=None)\
-        .get_image_ids()
+    output = default_coll_obj(collections=collections, variables=None).get_image_ids()
     assert type(output) is list
     assert set(x.split('/')[-1] for x in output) == set(scene_id_list)
```

### Comparing `openet-sims-0.1.0rc1/openet/sims/tests/test_d_interpolate.py` & `openet-sims-0.1.0rc3/openet/sims/tests/test_d_interpolate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime
-import pprint
+# import pprint
 
 import ee
 import pandas as pd
 import pytest
 
 import openet.sims.interpolate as interpolate
 import openet.sims.utils as utils
@@ -28,54 +28,49 @@
 
     """
     img = ee.Image('LANDSAT/LC08/C01/T1_SR/LC08_044033_20170716') \
         .select(['B2']).double().multiply(0)
     mask = img.add(1).updateMask(1).uint8()
 
     # The time band needs to be the 0 UTC time (date)
-    date1 = ee.Number(ee.Date.fromYMD(2017, 7, 8).millis())
-    date2 = ee.Number(ee.Date.fromYMD(2017, 7, 16).millis())
-    date3 = ee.Number(ee.Date.fromYMD(2017, 7, 24).millis())
-    time1 = ee.Number(ee.Date.fromYMD(2017, 7, 8).advance(18, 'hours').millis())
-    time2 = ee.Number(ee.Date.fromYMD(2017, 7, 16).advance(18, 'hours').millis())
-    time3 = ee.Number(ee.Date.fromYMD(2017, 7, 24).advance(18, 'hours').millis())
+    d1 = ee.Number(ee.Date.fromYMD(2017, 7, 8).millis())
+    d2 = ee.Number(ee.Date.fromYMD(2017, 7, 16).millis())
+    d3 = ee.Number(ee.Date.fromYMD(2017, 7, 24).millis())
+    t1 = ee.Number(ee.Date.fromYMD(2017, 7, 8).advance(18, 'hours').millis())
+    t2 = ee.Number(ee.Date.fromYMD(2017, 7, 16).advance(18, 'hours').millis())
+    t3 = ee.Number(ee.Date.fromYMD(2017, 7, 24).advance(18, 'hours').millis())
 
     # Mask and time bands currently get added on to the scene collection
     #   and images are unscaled just before interpolating in the export tool
     scene_coll = ee.ImageCollection([
-        ee.Image([img.add(et_fraction[0]), img.add(et[0]), img.add(ndvi[0]),
-                  img.add(date1), mask])\
+        ee.Image([img.add(et_fraction[0]), img.add(et[0]), img.add(ndvi[0]), img.add(d1), mask])
             .rename(['et_fraction', 'et', 'ndvi', 'time', 'mask'])
-            .set({'system:index': 'LE07_044033_20170708',
-                  'system:time_start': time1}),
-        ee.Image([img.add(et_fraction[1]), img.add(et[1]), img.add(ndvi[1]),
-                  img.add(date2), mask])\
+            .set({'system:index': 'LE07_044033_20170708', 'system:time_start': t1}),
+        ee.Image([img.add(et_fraction[1]), img.add(et[1]), img.add(ndvi[1]), img.add(d2), mask])
             .rename(['et_fraction', 'et', 'ndvi', 'time', 'mask'])
-            .set({'system:index': 'LC08_044033_20170716',
-                  'system:time_start': time2}),
-        ee.Image([img.add(et_fraction[2]), img.add(et[2]), img.add(ndvi[2]),
-                  img.add(date3), mask])\
+            .set({'system:index': 'LC08_044033_20170716', 'system:time_start': t2}),
+        ee.Image([img.add(et_fraction[2]), img.add(et[2]), img.add(ndvi[2]), img.add(d3), mask])
             .rename(['et_fraction', 'et', 'ndvi', 'time', 'mask'])
-            .set({'system:index': 'LE07_044033_20170724',
-                  'system:time_start': time3}),
+            .set({'system:index': 'LE07_044033_20170724', 'system:time_start': t3}),
     ])
     return scene_coll.select(variables)
 
 
 def test_from_scene_et_fraction_daily_values(tol=0.0001):
     output_coll = interpolate.from_scene_et_fraction(
         scene_coll(['et_fraction', 'ndvi', 'time', 'mask'], ndvi=[0.2, 0.4, 0.6]),
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'ndvi'],
-        interp_args={'interp_method': 'linear', 'interp_days': 32,},
+        interp_args={'interp_method': 'linear', 'interp_days': 32},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                     'et_reference_band': 'eto',
                     'et_reference_factor': 1.0,
                     'et_reference_resample': 'nearest'},
-        t_interval='daily')
+        t_interval='daily',
+    )
 
     TEST_POINT = (-121.5265, 38.7399)
     output = utils.point_coll_value(output_coll, TEST_POINT, scale=10)
     assert abs(output['ndvi']['2017-07-01'] - 0.2) <= tol
     assert abs(output['ndvi']['2017-07-08'] - 0.2) <= tol
     assert abs(output['ndvi']['2017-07-10'] - 0.25) <= tol
     assert abs(output['ndvi']['2017-07-12'] - 0.3) <= tol
@@ -97,15 +92,16 @@
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'ndvi', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                     'et_reference_band': 'eto',
                     'et_reference_factor': 1.0,
                     'et_reference_resample': 'nearest'},
-        t_interval='monthly')
+        t_interval='monthly',
+    )
 
     TEST_POINT = (-121.5265, 38.7399)
     output = utils.point_coll_value(output_coll, TEST_POINT, scale=10)
     assert abs(output['ndvi']['2017-07-01'] - 0.6) <= tol
     assert abs(output['et_fraction']['2017-07-01'] - 0.4) <= tol
     assert abs(output['et_reference']['2017-07-01'] - 236.5) <= tol
     assert abs(output['et']['2017-07-01'] - (236.5 * 0.4)) <= tol
@@ -118,15 +114,16 @@
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'ndvi', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                     'et_reference_band': 'eto',
                     'et_reference_factor': 1.0,
                     'et_reference_resample': 'nearest'},
-        t_interval='custom')
+        t_interval='custom',
+    )
 
     TEST_POINT = (-121.5265, 38.7399)
     output = utils.point_coll_value(output_coll, TEST_POINT, scale=10)
     assert abs(output['ndvi']['2017-07-01'] - 0.6) <= tol
     assert abs(output['et_fraction']['2017-07-01'] - 0.4) <= tol
     assert abs(output['et_reference']['2017-07-01'] - 236.5) <= tol
     assert abs(output['et']['2017-07-01'] - (236.5 * 0.4)) <= tol
@@ -139,15 +136,16 @@
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'ndvi', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                     'et_reference_band': 'eto',
                     'et_reference_factor': 0.5,
                     'et_reference_resample': 'nearest'},
-        t_interval='monthly')
+        t_interval='monthly',
+    )
 
     TEST_POINT = (-121.5265, 38.7399)
     output = utils.point_coll_value(output_coll, TEST_POINT, scale=10)
     assert abs(output['ndvi']['2017-07-01'] - 0.6) <= tol
     assert abs(output['et_fraction']['2017-07-01'] - 0.4) <= tol
     assert abs(output['et_reference']['2017-07-01'] - 236.5 * 0.5) <= tol
     assert abs(output['et']['2017-07-01'] - (236.5 * 0.5 * 0.4)) <= tol
@@ -161,51 +159,54 @@
         start_date='2017-07-01', end_date='2017-08-01',
         variables=['et', 'et_reference', 'et_fraction', 'ndvi', 'count'],
         interp_args={'interp_method': 'linear', 'interp_days': 32},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                     'et_reference_band': 'eto',
                     'et_reference_factor': 1.0,
                     'et_reference_resample': 'bilinear'},
-        t_interval='monthly')
+        t_interval='monthly',
+    )
 
     TEST_POINT = (-121.5265, 38.7399)
     output = utils.point_coll_value(output_coll, TEST_POINT, scale=10)
     assert abs(output['ndvi']['2017-07-01'] - 0.6) <= tol
     assert abs(output['et_fraction']['2017-07-01'] - 0.4) <= tol
     assert abs(output['et_reference']['2017-07-01'] - 236.5) <= tol
     assert abs(output['et']['2017-07-01'] - (236.5 * 0.4)) <= tol
     assert output['count']['2017-07-01'] == 3
 
 
 def test_from_scene_et_fraction_t_interval_bad_value():
     # Function should raise a ValueError if t_interval is not supported
     with pytest.raises(ValueError):
-        output_coll = interpolate.from_scene_et_fraction(
+        interpolate.from_scene_et_fraction(
             scene_coll(['et', 'time', 'mask']),
             start_date='2017-07-01', end_date='2017-08-01', variables=['et'],
             interp_args={'interp_method': 'linear', 'interp_days': 32},
             model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                         'et_reference_band': 'etr',
                         'et_reference_factor': 0.5,
                         'et_reference_resample': 'nearest'},
-            t_interval='deadbeef')
+            t_interval='deadbeef',
+        )
 
 
 def test_from_scene_et_fraction_t_interval_no_value():
     # Function should raise an Exception if t_interval is not set
     with pytest.raises(TypeError):
-        output_coll = interpolate.from_scene_et_fraction(
+        interpolate.from_scene_et_fraction(
             scene_coll(['et', 'time', 'mask']),
             start_date='2017-07-01', end_date='2017-08-01',
             variables=['et', 'et_reference', 'et_fraction', 'count'],
             interp_args={'interp_method': 'linear', 'interp_days': 32},
             model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                         'et_reference_band': 'etr',
                         'et_reference_factor': 0.5,
-                        'et_reference_resample': 'nearest'})
+                        'et_reference_resample': 'nearest'},
+        )
 
 
 @pytest.mark.parametrize(
     'landsat_coll_id',
     [
         'LANDSAT/LC08/C01/T1_SR',
         'LANDSAT/LC08/C02/T1_L2',
@@ -222,23 +223,25 @@
         .filterDate(start_date, end_date)\
         .filterBounds(ee.Geometry.Point(TEST_POINT))
 
     zero = landsat_coll.first().select(1).double().multiply(0)
 
     def make_et_frac(img):
         if 'C01' in landsat_coll_id:
-            et_img = sims.Image.from_landsat_c1_sr(img,
-                    et_reference_source=et_reference_source,
-                    et_reference_band=et_reference_band)\
-                .calculate(['ndvi', 'et_reference', 'et_fraction', 'et'])
+            et_img = sims.Image.from_landsat_c1_sr(
+                img,
+                et_reference_source=et_reference_source,
+                et_reference_band=et_reference_band,
+            ).calculate(['ndvi', 'et_reference', 'et_fraction', 'et'])
         elif 'C02' in landsat_coll_id:
-            et_img = sims.Image.from_landsat_c2_sr(img,
-                    et_reference_source=et_reference_source,
-                    et_reference_band=et_reference_band)\
-                .calculate(['ndvi', 'et_reference', 'et_fraction', 'et'])
+            et_img = sims.Image.from_landsat_c2_sr(
+                img,
+                et_reference_source=et_reference_source,
+                et_reference_band=et_reference_band,
+            ).calculate(['ndvi', 'et_reference', 'et_fraction', 'et'])
 
         time = ee.Number(img.get('system:time_start'))
         et_img = et_img.addBands([zero.add(time).rename('time')])
         return et_img
 
     test_imgs = landsat_coll.map(make_et_frac)
     normal_coll = interpolate.from_scene_et_fraction(
@@ -247,28 +250,30 @@
         end_date=end_date,
         variables=['et_reference', 'et_fraction', 'et'],
         interp_args={'interp_method': 'linear', 'interp_days': 14},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                     'et_reference_band': 'eto',
                     'et_reference_factor': 1.0,
                     'et_reference_resample': 'nearest'},
-        t_interval='daily')
+        t_interval='daily',
+    )
 
     wb_coll = interpolate.from_scene_et_fraction(
         test_imgs,
         start_date=start_date,
         end_date=end_date,
         variables=['et_reference', 'et_fraction', 'ke', 'et', 'ndvi'],
         interp_args={'interp_method': 'linear', 'interp_days': 14,
                      'estimate_soil_evaporation': True},
         model_args={'et_reference_source': 'IDAHO_EPSCOR/GRIDMET',
                     'et_reference_band': 'eto',
                     'et_reference_factor': 1.0,
                     'et_reference_resample': 'nearest'},
-        t_interval='daily')
+        t_interval='daily',
+    )
 
     normal = utils.point_coll_value(normal_coll, TEST_POINT, scale=30)
     wb = utils.point_coll_value(wb_coll, TEST_POINT, scale=30)
 
     for date in normal['et'].keys():
         # check that ET with soil evap >= ET without soil evap
         assert wb['et'][date] >= normal['et'][date]
@@ -277,17 +282,18 @@
 # Global constants for soil evap tests
 TEST_POINT = (-120.201, 36.1696)
 start_date = '2018-02-10'
 end_date = '2018-03-14'
 comp_df = pd.read_csv('openet/sims/tests/ee_wb_valid.csv')
 comp_df['et_fraction'] = comp_df['etc'] / comp_df['eto']
 
+
 @pytest.fixture
 def synth_test_imgs():
-    landsat_coll_id = f'LANDSAT/LC08/C01/T1_SR'
+    landsat_coll_id = 'LANDSAT/LC08/C01/T1_SR'
     landsat_coll = ee.ImageCollection(landsat_coll_id)\
         .filterDate(start_date, end_date)\
         .filterBounds(ee.Geometry.Point(TEST_POINT))
     mask = landsat_coll.first().select(['B2']).double().multiply(0)
 
     test_imgs = []
     for index, row in comp_df.iterrows():
@@ -345,15 +351,15 @@
         wp_source='projects/eeflux/soils/gsmsoil_mu_a_wp_10cm_albers_100',
         wp_band='b1',
     )
 
     base_ts = utils.point_coll_value(synth_test_imgs, TEST_POINT, scale=30)
     base_df = pd.DataFrame(base_ts).reset_index()
     base_df['et'] = base_df['et_fraction'] * base_df['et_reference']
-    
+
     evap_ts = utils.point_coll_value(evap_imgs, TEST_POINT, scale=30)
     evap_df = pd.DataFrame(evap_ts).reset_index()
     evap_df['et'] = evap_df['et_fraction'] * evap_df['et_reference']
 
     # Iterate through time series, stop one before end to avoid out of bounds
     # in "check next day state variable" tests
     for i in range(evap_df.shape[0]-1):
@@ -378,29 +384,30 @@
         if evap_df.loc[i, 'de'] == evap_df.de.max():
             assert evap_df.loc[i+1, 'kr'] == 0
 
 
 def test_soil_evap_fails_without_ndvi(synth_test_imgs):
     """Test that daily_ke raises exception if `ndvi` band not present"""
     try:
-        wb_coll = interpolate.from_scene_et_fraction(
+        interpolate.from_scene_et_fraction(
             synth_test_imgs,
             start_date=start_date,
             end_date=end_date,
             variables=['et_reference', 'et_fraction', 'ke', 'et', 'precip'],
             interp_args={'interp_method': 'linear', 'interp_days': 10,
                          'estimate_soil_evaporation': True},
             model_args={'et_reference_source': 'provided',
                         'et_reference_band': 'eto',
                         'et_reference_factor': 1.0,
                         'et_reference_resample': 'nearest'},
-            t_interval='daily')
+            t_interval='daily',
+        )
         # if from_scene_et_fraction doesn't raise, assert False
         assert False
-    except:
+    except Exception:
         pass
 
 
 def test_soil_evaporation_synthetic(synth_test_imgs, synth_precip_imgs, tol=0.001):
     """Test that setting 'estimate_soil_evaporation' flag runs SWB"""
     normal_coll = interpolate.from_scene_et_fraction(
         scene_coll=synth_test_imgs,
```

### Comparing `openet-sims-0.1.0rc1/openet/sims/utils.py` & `openet-sims-0.1.0rc3/openet/sims/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,15 @@
     # First key is band name, second key is the date string
     col_dict = {}
     info_dict = {}
     for i, k in enumerate(output[0][4:]):
         col_dict[k] = i + 4
         info_dict[k] = {}
     for row in output[1:]:
-        date = datetime.datetime.utcfromtimestamp(row[3] / 1000.0).strftime(
-            '%Y-%m-%d')
+        date = datetime.datetime.utcfromtimestamp(row[3] / 1000.0).strftime('%Y-%m-%d')
         for k, v in col_dict.items():
             info_dict[k][date] = row[col_dict[k]]
     return info_dict
     # return pd.DataFrame.from_dict(info_dict)
 
 
 def date_to_time_0utc(date):
@@ -83,15 +82,15 @@
     #     .divide(1000).floor().multiply(1000)
 
 
 def is_number(x):
     try:
         float(x)
         return True
-    except:
+    except Exception:
         return False
 
 
 def millis(input_dt):
     """Convert datetime to milliseconds since epoch
 
     Parameters
@@ -107,9 +106,9 @@
 
 
 def valid_date(date_str, date_fmt='%Y-%m-%d'):
     """Check if a datetime can be built from a date string and if it is valid"""
     try:
         datetime.datetime.strptime(date_str, date_fmt)
         return True
-    except Exception as e:
+    except Exception:
         return False
```

### Comparing `openet-sims-0.1.0rc1/openet_sims.egg-info/PKG-INFO` & `openet-sims-0.1.0rc3/openet_sims.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openet-sims
-Version: 0.1.0rc1
+Version: 0.1.0rc3
 Summary: Earth Engine based SIMS Model
 Author-email: Alberto Guzman <aguzman@csumb.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -208,14 +208,15 @@
 Project-URL: Homepage, https://github.com/Open-ET/openet-sims
 Keywords: SIMS,OpenET,Earth Engine,evapotranspiration
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE.txt
 
 ===================
 OpenET - SIMS Model
 ===================
 
 |version| |build|
```

### Comparing `openet-sims-0.1.0rc1/openet_sims.egg-info/SOURCES.txt` & `openet-sims-0.1.0rc3/openet_sims.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 LICENSE.txt
-MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
 openet/__init__.py
 openet/sims/__init__.py
 openet/sims/collection.py
 openet/sims/data.py
 openet/sims/image.py
 openet/sims/interpolate.py
 openet/sims/model.py
```

### Comparing `openet-sims-0.1.0rc1/pyproject.toml` & `openet-sims-0.1.0rc3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "openet-sims"
-version = "0.1.0-rc.1"
+version = "0.1.0-rc.3"
 authors = [
   { name="Alberto Guzman", email="aguzman@csumb.edu" },
 ]
 description = "Earth Engine based SIMS Model"
 readme = "README.rst"
 requires-python = ">=3.7"
 keywords = ["SIMS", "OpenET", "Earth Engine", "evapotranspiration"]
@@ -15,19 +15,29 @@
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "earthengine-api>=0.1.310",
     "openet-core>=0.0.16",
     "python-dateutil",
+    "importlib-metadata; python_version <= '3.7'",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Open-ET/openet-sims"
 #"Repository" = "https://github.com/Open-ET/openet-sims.git"
 #"Documentation" = "https://github.com/Open-ET/openet-sims"
 #"Bug Tracker" = "https://github.com/Open-ET/openet-sims"
 #"Changelog" = "https://github.com/Open-ET/openet-sims"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
+
+[project.optional-dependencies]
+test = [
+    "pytest",
+    "pandas",
+]
+
+[tool.setuptools.package-data]
+"openet.sims.tests" = ["*.csv"]
```

