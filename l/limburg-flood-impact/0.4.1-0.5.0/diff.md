# Comparing `tmp/limburg_flood_impact-0.4.1.tar.gz` & `tmp/limburg_flood_impact-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limburg_flood_impact-0.4.1.tar", last modified: Tue Feb 28 08:44:30 2023, max compression
+gzip compressed data, was "limburg_flood_impact-0.5.0.tar", last modified: Thu Jun 15 08:26:53 2023, max compression
```

## Comparing `limburg_flood_impact-0.4.1.tar` & `limburg_flood_impact-0.5.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxrwxr-x   0 cahik     (1000) cahik     (1000)        0 2023-02-28 08:44:30.954445 limburg_flood_impact-0.4.1/
--rw-rw-r--   0 cahik     (1000) cahik     (1000)    12858 2023-02-28 08:44:30.954445 limburg_flood_impact-0.4.1/PKG-INFO
--rw-rw-r--   0 cahik     (1000) cahik     (1000)    12509 2023-02-28 08:44:24.000000 limburg_flood_impact-0.4.1/README.rst
--rw-rw-r--   0 cahik     (1000) cahik     (1000)      149 2023-01-11 11:33:08.000000 limburg_flood_impact-0.4.1/pyproject.toml
--rwxrwxr-x   0 cahik     (1000) cahik     (1000)     1080 2023-02-28 08:44:30.954445 limburg_flood_impact-0.4.1/setup.cfg
--rw-rw-r--   0 cahik     (1000) cahik     (1000)       69 2022-03-23 16:23:16.000000 limburg_flood_impact-0.4.1/setup.py
-drwxrwxr-x   0 cahik     (1000) cahik     (1000)        0 2023-02-28 08:44:30.946445 limburg_flood_impact-0.4.1/src/
-drwxrwxr-x   0 cahik     (1000) cahik     (1000)        0 2023-02-28 08:44:30.950445 limburg_flood_impact-0.4.1/src/limburg_flood_impact/
--rw-rw-r--   0 cahik     (1000) cahik     (1000)      103 2023-02-02 08:42:26.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact/__init__.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)    12384 2023-02-28 07:45:36.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact/_functions.py
-drwxrwxr-x   0 cahik     (1000) cahik     (1000)        0 2023-02-28 08:44:30.954445 limburg_flood_impact-0.4.1/src/limburg_flood_impact/bin/
--rw-rw-r--   0 cahik     (1000) cahik     (1000)        0 2023-01-11 11:38:20.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact/bin/__init__.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     1189 2023-02-28 07:45:36.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact/bin/check_address.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     1286 2023-02-28 07:45:36.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact/bin/classify_area_wide_rain.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     1267 2023-02-28 07:45:36.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact/bin/classify_rural_rain.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     1267 2023-02-28 07:45:36.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact/bin/classify_urban_rain.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)      865 2023-02-28 07:45:36.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact/bin/combine_classification.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     1308 2023-02-28 07:45:36.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact/bin/test_against_flood_protection_norm.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     2053 2023-02-02 08:42:26.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact/check_address.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     8809 2023-02-28 08:19:54.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact/classify_area_wide_rain.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     1635 2023-02-28 07:45:36.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact/classify_rural_rain.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     6122 2023-02-28 08:09:14.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact/classify_urban_rain.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     2983 2023-01-18 10:31:03.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact/combine_classification.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     4155 2023-02-28 08:37:34.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact/test_against_flood_protection_norm.py
-drwxrwxr-x   0 cahik     (1000) cahik     (1000)        0 2023-02-28 08:44:30.950445 limburg_flood_impact-0.4.1/src/limburg_flood_impact.egg-info/
--rw-rw-r--   0 cahik     (1000) cahik     (1000)    12858 2023-02-28 08:44:30.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact.egg-info/PKG-INFO
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     1130 2023-02-28 08:44:30.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact.egg-info/SOURCES.txt
--rw-rw-r--   0 cahik     (1000) cahik     (1000)        1 2023-02-28 08:44:30.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact.egg-info/dependency_links.txt
--rw-rw-r--   0 cahik     (1000) cahik     (1000)      482 2023-02-28 08:44:30.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact.egg-info/entry_points.txt
--rw-rw-r--   0 cahik     (1000) cahik     (1000)        1 2023-02-08 17:43:18.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact.egg-info/not-zip-safe
--rw-rw-r--   0 cahik     (1000) cahik     (1000)       11 2023-02-28 08:44:30.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact.egg-info/requires.txt
--rw-rw-r--   0 cahik     (1000) cahik     (1000)       21 2023-02-28 08:44:30.000000 limburg_flood_impact-0.4.1/src/limburg_flood_impact.egg-info/top_level.txt
+drwxrwxr-x   0 cahik     (1000) cahik     (1000)        0 2023-06-15 08:26:53.232552 limburg_flood_impact-0.5.0/
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)    12858 2023-06-15 08:26:53.232552 limburg_flood_impact-0.5.0/PKG-INFO
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)    12509 2023-06-15 08:26:47.000000 limburg_flood_impact-0.5.0/README.rst
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)      149 2023-01-11 11:33:08.000000 limburg_flood_impact-0.5.0/pyproject.toml
+-rwxrwxr-x   0 cahik     (1000) cahik     (1000)     1080 2023-06-15 08:26:53.236552 limburg_flood_impact-0.5.0/setup.cfg
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)       69 2022-03-23 16:23:16.000000 limburg_flood_impact-0.5.0/setup.py
+drwxrwxr-x   0 cahik     (1000) cahik     (1000)        0 2023-06-15 08:26:52.936552 limburg_flood_impact-0.5.0/src/
+drwxrwxr-x   0 cahik     (1000) cahik     (1000)        0 2023-06-15 08:26:52.968552 limburg_flood_impact-0.5.0/src/limburg_flood_impact/
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)      103 2023-02-02 08:42:26.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact/__init__.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)    14467 2023-06-15 07:00:42.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact/_functions.py
+drwxrwxr-x   0 cahik     (1000) cahik     (1000)        0 2023-06-15 08:26:53.232552 limburg_flood_impact-0.5.0/src/limburg_flood_impact/bin/
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)        0 2023-01-11 11:38:20.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact/bin/__init__.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     1189 2023-02-28 07:45:36.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact/bin/check_address.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     1286 2023-02-28 07:45:36.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact/bin/classify_area_wide_rain.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     1267 2023-02-28 07:45:36.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact/bin/classify_rural_rain.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     1267 2023-02-28 07:45:36.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact/bin/classify_urban_rain.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)      865 2023-02-28 07:45:36.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact/bin/combine_classification.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     1308 2023-02-28 07:45:36.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact/bin/test_against_flood_protection_norm.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     2053 2023-02-02 08:42:26.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact/check_address.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)    10663 2023-06-15 08:21:50.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact/classify_area_wide_rain.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     1635 2023-02-28 07:45:36.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact/classify_rural_rain.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     6375 2023-05-19 20:19:49.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact/classify_urban_rain.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     2983 2023-01-18 10:31:03.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact/combine_classification.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     2231 2023-06-14 09:52:33.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact/extent_tile.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     8634 2023-06-14 15:23:44.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact/test.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     4155 2023-02-28 08:37:34.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact/test_against_flood_protection_norm.py
+drwxrwxr-x   0 cahik     (1000) cahik     (1000)        0 2023-06-15 08:26:53.228552 limburg_flood_impact-0.5.0/src/limburg_flood_impact.egg-info/
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)    12858 2023-06-15 08:26:52.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact.egg-info/PKG-INFO
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     1203 2023-06-15 08:26:52.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact.egg-info/SOURCES.txt
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)        1 2023-06-15 08:26:52.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact.egg-info/dependency_links.txt
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)      482 2023-06-15 08:26:52.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact.egg-info/entry_points.txt
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)        1 2023-02-08 17:43:18.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact.egg-info/not-zip-safe
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)       11 2023-06-15 08:26:52.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact.egg-info/requires.txt
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)       21 2023-06-15 08:26:52.000000 limburg_flood_impact-0.5.0/src/limburg_flood_impact.egg-info/top_level.txt
```

### Comparing `limburg_flood_impact-0.4.1/PKG-INFO` & `limburg_flood_impact-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limburg_flood_impact
-Version: 0.4.1
+Version: 0.5.0
 Summary: Libmurg Flood Impact Package.
 Home-page: https://github.com/
 Author: Lutra Consulting Ltd.
 Author-email: jan.caha@lutraconsulting.co.uk
 License: MIT
 Project-URL: Documentation, https://
 Platform: any
```

### Comparing `limburg_flood_impact-0.4.1/README.rst` & `limburg_flood_impact-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.4.1/setup.cfg` & `limburg_flood_impact-0.5.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = limburg_flood_impact
-version = 0.4.1
+version = 0.5.0
 description = Libmurg Flood Impact Package.
 url = https://github.com/
 project_urls = 
 	Documentation = https://
 author = Lutra Consulting Ltd.
 author_email = jan.caha@lutraconsulting.co.uk
 platforms = any
```

### Comparing `limburg_flood_impact-0.4.1/src/limburg_flood_impact/_functions.py` & `limburg_flood_impact-0.5.0/src/limburg_flood_impact/_functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,32 @@
 from pathlib import Path
 import argparse
+import tempfile
+import uuid
+import shutil
+import sys
 
 import numpy as np
 
 from osgeo import ogr, gdal
 
+TIFF_DRIVER: gdal.Driver = gdal.GetDriverByName("GTiff")
 RASTER_DRIVER: gdal.Driver = gdal.GetDriverByName("MEM")
 VECTOR_DRIVER: ogr.Driver = ogr.GetDriverByName("MEMORY")
 COLUMN_RASTER_VALUE = "rasterValue"
+TMP_FOLDER = f"{tempfile.gettempdir()}/{str(uuid.uuid4()).split('-')[0]}"
+
+TILE_SIZE = 1000.0
+TILE_OVERLAP = 50.0
+
+
+def remove_tmp_folder():
+    folder = Path(TMP_FOLDER)
+    if folder.exists():
+        shutil.rmtree(folder)
 
 
 def convert_to_binary_raster(ds: gdal.Dataset, values_below_as_zero: float = None) -> gdal.Dataset:
     """
     Converts input ds into binary raster (mask). All values besides NoData are converted to 1, NoData is 0.
     If values_below_as_zero parameter is specified, values < values_below_as_zero are also converted to 0.
 
@@ -63,14 +78,16 @@
         by default gdal.GDT_Byte
 
     Returns
     -------
     gdal.Dataset
         Dataset with single band.
     """
+
+    # TIFF_DRIVER.Create(f"{TMP_FOLDER}/{name}.tiff",
     ds: gdal.Dataset = RASTER_DRIVER.Create(name,
                                             template_raster.RasterXSize,
                                             template_raster.RasterYSize,
                                             bands=1,
                                             eType=data_type)
     ds.SetGeoTransform(template_raster.GetGeoTransform())
     ds.SetProjection(template_raster.GetProjection())
@@ -166,24 +183,24 @@
     sql_layer = None
 
     return vector_ds
 
 
 def rasterize_layer_mask(ds: ogr.DataSource,
                          template_raster: gdal.Dataset,
-                         data_type=gdal.GDT_Float64) -> np.ndarray:
+                         data_type=gdal.GDT_Float32) -> np.ndarray:
     """
     Converts ds into binary raster mask according to template raster.
 
     Parameters
     ----------
     ds : ogr.DataSource
     template_raster : gdal.Dataset
     data_type : _type_, optional
-        by default gdal.GDT_Float64
+        by default gdal.GDT_Float32
 
     Returns
     -------
     np.ndarray
     """
     layer: ogr.Layer = ds.GetLayer()
 
@@ -218,15 +235,15 @@
     -------
     gdal.Dataset
     """
     ds_path = Path(raster_ds.GetDescription())
 
     file_name = "with_mask" + ds_path.stem
 
-    new_raster_ds = create_empty_raster(file_name, raster_ds, gdal.GDT_Float64)
+    new_raster_ds = create_empty_raster(file_name, raster_ds, raster_ds.GetRasterBand(1).DataType)
 
     band: gdal.Band = new_raster_ds.GetRasterBand(1)
 
     band.WriteArray(raster_ds.GetRasterBand(1).ReadAsArray() * mask)
 
     band = None
 
@@ -267,18 +284,23 @@
 
     vectorized_raster_ds = vectorize_raster(binary_raster_ds)
 
     selected_areas_ds = select_features(vectorized_raster_ds,
                                         value_to_select=1,
                                         min_area=minimal_area_of_water_pond)
 
-    rasterized_mask = rasterize_layer_mask(selected_areas_ds, flood_raster_ds)
+    rasterized_mask = rasterize_layer_mask(selected_areas_ds, flood_raster_ds, flood_raster_ds.GetRasterBand(1).DataType)
 
     raster = multiply_raster_by_mask(flood_raster_ds, rasterized_mask)
 
+    binary_raster_ds = None
+    vectorized_raster_ds = None
+    selected_areas_ds = None
+    rasterized_mask = None
+
     return raster
 
 
 def raster_coordinates(inputX: float,
                        inputY: float,
                        inv_gt,
                        minimal_cell_coordinate: bool = True) -> tuple:
@@ -326,17 +348,16 @@
         raster.GetGeoTransform()
 
     Returns
     -------
     tuple
         x, y
     """
-    x, y = \
-        (gt[0] + gt[1] * inputX + gt[2] * inputY), \
-        (gt[3] + gt[4] * inputX + gt[5] * inputY)
+    x = (gt[0] + gt[1] * inputX + gt[2] * inputY)
+    y = (gt[3] + gt[4] * inputX + gt[5] * inputY)
     return x, y
 
 
 def get_water_height_array(water_band: gdal.Band, minX: float, maxX: float, minY: float,
                            maxY: float) -> np.ndarray:
     """
     Extract small part of the band as an array, with NoDataValues replaced by 0.
@@ -349,15 +370,15 @@
     minY : float
     maxY : float
 
     Returns
     -------
     np.ndarray
     """
-    water_array = water_band.ReadAsArray(minX, maxY, int(maxX - minX), int(minY - maxY))
+    water_array = water_band.ReadAsArray(minX, minY, int(maxX - minX), int(maxY - minY))
     water_array[water_array == water_band.GetNoDataValue()] = 0
     # cannot be below 0 so filter out
     water_array[water_array < 0] = 0
     # filter out unreasonably large values -> most likely no data not set correctly
     water_array[water_array > 1000] = 0
     return water_array
 
@@ -441,7 +462,60 @@
     index = layer.FindFieldIndex(field_name, True)
 
     if index == -1:
         layer.CreateField(ogr.FieldDefn(field_name, field_type))
         index = layer.FindFieldIndex(field_name, True)
 
     return index
+
+
+def get_extent(ds: gdal.Dataset) -> ogr.Geometry:
+    """ Return list of corner coordinates from a gdal Dataset """
+    xmin, xpixel, _, ymax, _, ypixel = ds.GetGeoTransform()
+    width, height = ds.RasterXSize, ds.RasterYSize
+    xmax = xmin + width * xpixel
+    ymin = ymax + height * ypixel
+
+    ring = ogr.Geometry(ogr.wkbLinearRing)
+    ring.AddPoint(xmin, ymin)
+    ring.AddPoint(xmax, ymin)
+    ring.AddPoint(xmax, ymax)
+    ring.AddPoint(xmin, ymax)
+    ring.AddPoint(xmin, ymin)
+
+    polygon = ogr.Geometry(ogr.wkbPolygon)
+    polygon.AddGeometry(ring)
+
+    return polygon
+
+
+def set_field_if_higher(feature: ogr.Feature, field_index: int, new_value: float) -> bool:
+    """
+    Sets value of field index if the new value is higher then previously stored value. 
+    Returns `True` if the field has changed and `False` if it has not.
+
+    Parameters
+    ----------
+    feature : ogr.Feature
+    field_index : int
+    new_value : float
+
+    Returns
+    -------
+    bool
+    """
+    old_value = feature.GetFieldAsDouble(field_index)
+
+    if new_value > old_value:
+        feature.SetField(field_index, new_value)
+        return True
+
+    return False
+
+
+def print_progress_bar(count_value, total, suffix=''):
+    bar_length = 100
+    filled_up_Length = int(round(bar_length * count_value / float(total)))
+    percentage = round(100.0 * count_value / float(total), 1)
+    bar = '=' * filled_up_Length + '-' * (bar_length - filled_up_Length)
+    sys.stdout.write(f'[{bar}] {percentage}%   {suffix}\r')
+    sys.stdout.flush()
```

### Comparing `limburg_flood_impact-0.4.1/src/limburg_flood_impact/bin/check_address.py` & `limburg_flood_impact-0.5.0/src/limburg_flood_impact/bin/check_address.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.4.1/src/limburg_flood_impact/bin/classify_area_wide_rain.py` & `limburg_flood_impact-0.5.0/src/limburg_flood_impact/bin/classify_area_wide_rain.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.4.1/src/limburg_flood_impact/bin/classify_rural_rain.py` & `limburg_flood_impact-0.5.0/src/limburg_flood_impact/bin/classify_rural_rain.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.4.1/src/limburg_flood_impact/bin/classify_urban_rain.py` & `limburg_flood_impact-0.5.0/src/limburg_flood_impact/bin/classify_urban_rain.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.4.1/src/limburg_flood_impact/bin/combine_classification.py` & `limburg_flood_impact-0.5.0/src/limburg_flood_impact/bin/combine_classification.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.4.1/src/limburg_flood_impact/bin/test_against_flood_protection_norm.py` & `limburg_flood_impact-0.5.0/src/limburg_flood_impact/bin/test_against_flood_protection_norm.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.4.1/src/limburg_flood_impact/check_address.py` & `limburg_flood_impact-0.5.0/src/limburg_flood_impact/check_address.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.4.1/src/limburg_flood_impact/classify_area_wide_rain.py` & `limburg_flood_impact-0.5.0/src/limburg_flood_impact/classify_area_wide_rain.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-from typing import Callable
 from pathlib import Path
 
 import numpy as np
 
 from osgeo import ogr, gdal
 
-from ._functions import RASTER_DRIVER, VECTOR_DRIVER
+from ._functions import RASTER_DRIVER, VECTOR_DRIVER, TILE_SIZE, TILE_OVERLAP
 from ._functions import (flood_mask, delete_all_features_from_layer, raster_coordinates,
-                         world_coordinates, get_water_height_array, find_or_create_field)
+                         world_coordinates, get_water_height_array, find_or_create_field, remove_tmp_folder,
+                         get_extent, set_field_if_higher, print_progress_bar)
+from .extent_tile import Extent
 
 
 def field_name_with_puddles(type: str) -> str:
     return f"max_waterdiepte_gebiedsbreed_incl_kleine_plassen_{type}"
 
 
 def field_name_without_puddles(type: str) -> str:
     return f"max_waterdiepte_gebiedsbreed_excl_kleine_plassen_{type}"
 
 
-def classify_water_height(buildings_ds: gdal.Dataset,
+def classify_water_height(buildings_layer: ogr.Layer,
                           t10_with_puddles: gdal.Dataset,
                           t25_with_puddles: gdal.Dataset,
                           t100_with_puddles: gdal.Dataset,
                           t10: gdal.Dataset,
                           t25: gdal.Dataset,
                           t100: gdal.Dataset,
                           field_name: str = "gebiedsbreed",
-                          callback_function: Callable[[float], None] = None,
                           qgis_feedback=None):
 
-    buildings_layer: ogr.Layer = buildings_ds.GetLayer()
-
     t10_index = find_or_create_field(buildings_layer, f"{field_name}_t10", ogr.OFTString)
     t25_index = find_or_create_field(buildings_layer, f"{field_name}_t25", ogr.OFTString)
     t100_index = find_or_create_field(buildings_layer, f"{field_name}_t100", ogr.OFTString)
 
     wdp_t10_index = find_or_create_field(buildings_layer, field_name_with_puddles("t10"), ogr.OFTReal)
     wdp_t25_index = find_or_create_field(buildings_layer, field_name_with_puddles("t25"), ogr.OFTReal)
     wdp_t100_index = find_or_create_field(buildings_layer, field_name_with_puddles("t100"), ogr.OFTReal)
@@ -55,40 +53,51 @@
     t100_band: gdal.Band = t100.GetRasterBand(1)
 
     memory_ds: ogr.DataSource = VECTOR_DRIVER.CreateDataSource("ds")
     memory_layer: ogr.Layer = memory_ds.CreateLayer("geometry_layer",
                                                     buildings_layer.GetSpatialRef(),
                                                     ogr.wkbPolygon)
 
+    raster_bbox = get_extent(t10)
+
+    buildings_layer.SetSpatialFilter(raster_bbox)
+
     feature: ogr.Feature
     i = 0
     for feature in buildings_layer:
 
         if qgis_feedback is not None:
             if qgis_feedback.isCanceled():
                 break
 
         delete_all_features_from_layer(memory_layer)
 
         geom: ogr.Geometry = feature.GetGeometryRef().Buffer(1)
+
+        if not raster_bbox.Intersect(geom):
+            continue
+
+        if not geom.Within(raster_bbox):
+            geom = geom.Intersection(raster_bbox)
+
         minX, maxX, minY, maxY = geom.GetEnvelope()
 
         new_feature: ogr.Feature = ogr.Feature(memory_layer.GetLayerDefn())
         new_feature.SetGeometry(geom)
         memory_layer.SetFeature(new_feature)
 
-        rMinX, rMaxY = raster_coordinates(minX, maxY, inv_gt)
-        rMaxX, rMinY = raster_coordinates(maxX, minY, inv_gt, False)
+        rMinX, rMaxY = raster_coordinates(minX, minY, inv_gt)
+        rMaxX, rMinY = raster_coordinates(maxX, maxY, inv_gt, False)
 
         feature_raster_ds: gdal.Dataset = RASTER_DRIVER.Create("geom_raster",
                                                                int(rMaxX - rMinX),
-                                                               int(rMinY - rMaxY),
+                                                               int(rMaxY - rMinY),
                                                                bands=1,
                                                                eType=gdal.GDT_Float64)
-        t_coords = world_coordinates(rMinX, rMaxY, gt)
+        t_coords = world_coordinates(rMinX, rMinY, gt)
         feature_raster_ds.SetGeoTransform([t_coords[0], gt[1], gt[2], t_coords[1], gt[4], gt[5]])
         feature_raster_ds.SetProjection(t10.GetProjection())
 
         gdal.RasterizeLayer(feature_raster_ds, [1],
                             memory_layer,
                             burn_values=[1],
                             options=["ALL_TOUCHED=TRUE"])
@@ -102,43 +111,46 @@
         t100_water_with_puddles = get_water_height_array(t100_band_with_puddles, rMinX, rMaxX,
                                                          rMinY, rMaxY)
 
         t10_water = get_water_height_array(t10_band, rMinX, rMaxX, rMinY, rMaxY)
         t25_water = get_water_height_array(t25_band, rMinX, rMaxX, rMinY, rMaxY)
         t100_water = get_water_height_array(t100_band, rMinX, rMaxX, rMinY, rMaxY)
 
-        feature.SetField(wdp_t10_index, np.max(t10_water_with_puddles))
-        feature.SetField(wdp_t25_index, np.max(t25_water_with_puddles))
-        feature.SetField(wdp_t100_index, np.max(t100_water_with_puddles))
-
-        feature.SetField(wd_t10_index, np.max(t10_water))
-        feature.SetField(wd_t25_index, np.max(t25_water))
-        feature.SetField(wd_t100_index, np.max(t100_water))
-
-        feature.SetField(
-            t10_index,
-            column_value(np.max(feature_rasterized * t10_water_with_puddles),
-                         np.max(feature_rasterized * t10_water)))
-        feature.SetField(
-            t25_index,
-            column_value(np.max(feature_rasterized * t25_water_with_puddles),
-                         np.max(feature_rasterized * t25_water)))
-        feature.SetField(
-            t100_index,
-            column_value(np.max(feature_rasterized * t100_water_with_puddles),
-                         np.max(feature_rasterized * t100_water)))
+        wdp_t10_changed = set_field_if_higher(feature, wdp_t10_index, float(np.max(t10_water_with_puddles * feature_rasterized)))
+        wdp_t25_changed = set_field_if_higher(feature, wdp_t25_index, float(np.max(t25_water_with_puddles * feature_rasterized)))
+        wdp_t100_changed = set_field_if_higher(feature, wdp_t100_index, float(np.max(t100_water_with_puddles * feature_rasterized)))
+
+        wd_t10_changed = set_field_if_higher(feature, wd_t10_index, float(np.max(t10_water * feature_rasterized)))
+        wd_t25_changed = set_field_if_higher(feature, wd_t25_index, float(np.max(t25_water * feature_rasterized)))
+        wd_t100_changed = set_field_if_higher(feature, wd_t100_index, float(np.max(t100_water * feature_rasterized)))
+
+        if wdp_t10_changed or wd_t10_changed:
+            feature.SetField(
+                t10_index,
+                column_value(np.max(feature_rasterized * t10_water_with_puddles),
+                             np.max(feature_rasterized * t10_water)))
+
+        if wdp_t25_changed or wd_t25_changed:
+            feature.SetField(
+                t25_index,
+                column_value(np.max(feature_rasterized * t25_water_with_puddles),
+                             np.max(feature_rasterized * t25_water)))
+
+        if wdp_t100_changed or wd_t100_changed:
+            feature.SetField(
+                t100_index,
+                column_value(np.max(feature_rasterized * t100_water_with_puddles),
+                             np.max(feature_rasterized * t100_water)))
 
         buildings_layer.SetFeature(feature)
 
-        if callback_function:
-            callback_function((i / buildings_layer.GetFeatureCount()) * 100)
-
         i += 1
 
-    buildings_layer = None
+    memory_layer = None
+    memory_ds = None
 
 
 def column_value(value_with_puddles: float, value_without_puddles: float) -> str:
     if 0.15 < value_with_puddles and value_without_puddles <= 0.15:
         return "Risico, lokale herkomst"
     elif 0.15 < value_without_puddles:
         return "Risico, regionale herkomst"
@@ -148,67 +160,102 @@
     return "Geen risico"
 
 
 def classify_area_wide_rain(buildings_path: Path,
                             t10: Path,
                             t25: Path,
                             t100: Path,
-                            callback_function: Callable[[float], None] = None,
                             qgis_feedback=None):
 
     buildings_ds: ogr.DataSource = ogr.Open(buildings_path.as_posix(), True)
+    buildings_layer: ogr.Layer = buildings_ds.GetLayer()
 
-    t10_ds: gdal.Dataset = gdal.Open(t10.as_posix())
-    t25_ds: gdal.Dataset = gdal.Open(t25.as_posix())
-    t100_ds: gdal.Dataset = gdal.Open(t100.as_posix())
+    t10_ds_whole: gdal.Dataset = gdal.Open(t10.as_posix())
+    t25_ds_whole: gdal.Dataset = gdal.Open(t25.as_posix())
+    t100_ds_whole: gdal.Dataset = gdal.Open(t100.as_posix())
 
-    t10_masked_including_puddles = flood_mask(t10_ds, only_water_height_above=0.02)
+    rasterExtent = Extent.from_gdal_ds(t10_ds_whole)
 
-    if qgis_feedback:
-        if qgis_feedback.isCanceled():
-            return
+    tiles = rasterExtent.create_tiles(TILE_SIZE)
 
-    t25_masked_including_puddles = flood_mask(t25_ds, only_water_height_above=0.02)
+    gdal.UseExceptions()
 
-    if qgis_feedback:
-        if qgis_feedback.isCanceled():
-            return
+    for i, tile in enumerate(tiles):
 
-    t100_masked_including_puddles = flood_mask(t100_ds, only_water_height_above=0.02)
+        print_progress_bar(i + 1, len(tiles), "Tiles processed.")
 
-    if qgis_feedback:
-        if qgis_feedback.isCanceled():
-            return
+        tile.buffer_by(TILE_OVERLAP)
 
-    t10_masked = flood_mask(t10_ds, only_water_height_above=0.02, minimal_area_of_water_pond=200)
+        t10_ds = tile.extract_from(t10_ds_whole)
+        t25_ds = tile.extract_from(t25_ds_whole)
+        t100_ds = tile.extract_from(t100_ds_whole)
 
-    if qgis_feedback:
-        if qgis_feedback.isCanceled():
-            return
+        t10_masked_including_puddles = flood_mask(t10_ds, only_water_height_above=0.02)
 
-    t25_masked = flood_mask(t25_ds, only_water_height_above=0.02, minimal_area_of_water_pond=200)
+        if qgis_feedback:
+            if qgis_feedback.isCanceled():
+                return
+
+        t25_masked_including_puddles = flood_mask(t25_ds, only_water_height_above=0.02)
 
-    if qgis_feedback:
-        if qgis_feedback.isCanceled():
-            return
+        if qgis_feedback:
+            if qgis_feedback.isCanceled():
+                return
 
-    t100_masked = flood_mask(t100_ds, only_water_height_above=0.02, minimal_area_of_water_pond=200)
+        t100_masked_including_puddles = flood_mask(t100_ds, only_water_height_above=0.02)
+
+        if qgis_feedback:
+            if qgis_feedback.isCanceled():
+                return
+
+        t10_masked = flood_mask(t10_ds, only_water_height_above=0.02, minimal_area_of_water_pond=200)
+
+        if qgis_feedback:
+            if qgis_feedback.isCanceled():
+                return
+
+        t25_masked = flood_mask(t25_ds, only_water_height_above=0.02, minimal_area_of_water_pond=200)
+
+        if qgis_feedback:
+            if qgis_feedback.isCanceled():
+                return
+
+        t100_masked = flood_mask(t100_ds, only_water_height_above=0.02, minimal_area_of_water_pond=200)
+
+        if qgis_feedback:
+            if qgis_feedback.isCanceled():
+                return
 
-    if qgis_feedback:
-        if qgis_feedback.isCanceled():
-            return
+        classify_water_height(buildings_layer,
+                              t10_masked_including_puddles,
+                              t25_masked_including_puddles,
+                              t100_masked_including_puddles,
+                              t10_masked,
+                              t25_masked,
+                              t100_masked,
+                              field_name="gebiedsbreed",
+                              qgis_feedback=qgis_feedback)
 
-    classify_water_height(buildings_ds,
-                          t10_masked_including_puddles,
-                          t25_masked_including_puddles,
-                          t100_masked_including_puddles,
-                          t10_masked,
-                          t25_masked,
-                          t100_masked,
-                          field_name="gebiedsbreed",
-                          callback_function=callback_function,
-                          qgis_feedback=qgis_feedback)
+        if qgis_feedback:
+            qgis_feedback.setProgress((i + 1 / len(tiles)) * 100)
 
     buildings_ds = None
     t10_ds = None
     t25_ds = None
     t100_ds = None
+    t10_masked_including_puddles = None
+    t25_masked_including_puddles = None
+    t100_masked_including_puddles = None
+    t10_masked = None
+    t25_masked = None
+    t100_masked = None
+
+    remove_tmp_folder()
+
+
+if __name__ == "__main__":
+
+    classify_area_wide_rain(
+        Path("/home/cahik/Lutra/Floods/New_Data/Overig benodigde data/BAG_panden.gpkg"),
+        Path("/home/cahik/Lutra/Floods/New_Data/rasters/T10Compleet.tif"),
+        Path("/home/cahik/Lutra/Floods/New_Data/rasters/T25Compleet.tif"),
+        Path("/home/cahik/Lutra/Floods/New_Data/rasters/T100Compleet.tif"))
```

### Comparing `limburg_flood_impact-0.4.1/src/limburg_flood_impact/classify_rural_rain.py` & `limburg_flood_impact-0.5.0/src/limburg_flood_impact/classify_rural_rain.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.4.1/src/limburg_flood_impact/classify_urban_rain.py` & `limburg_flood_impact-0.5.0/src/limburg_flood_impact/classify_urban_rain.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 import numpy as np
 
 from osgeo import ogr, gdal
 
 from ._functions import RASTER_DRIVER, VECTOR_DRIVER
 from ._functions import (flood_mask, delete_all_features_from_layer, raster_coordinates,
-                         world_coordinates, get_water_height_array, find_or_create_field)
+                         world_coordinates, get_water_height_array, find_or_create_field,
+                         get_extent)
 
 
 def classify_water_height(buildings_ds: gdal.Dataset,
                           t10: gdal.Dataset,
                           t25: gdal.Dataset,
                           t100: gdal.Dataset,
                           field_name: str = "stedelijk",
@@ -35,25 +36,35 @@
     t25_band: gdal.Band = t25.GetRasterBand(1)
     t100_band: gdal.Band = t100.GetRasterBand(1)
 
     memory_ds: ogr.DataSource = VECTOR_DRIVER.CreateDataSource("ds")
     memory_layer: ogr.Layer = memory_ds.CreateLayer("geometry_layer",
                                                     buildings_layer.GetSpatialRef(),
                                                     ogr.wkbPolygon)
+
+    raster_bbox = get_extent(t10)
+
     feature: ogr.Feature
     i = 0
     for feature in buildings_layer:
 
         if qgis_feedback is not None:
             if qgis_feedback.isCanceled():
                 break
 
         delete_all_features_from_layer(memory_layer)
 
         geom: ogr.Geometry = feature.GetGeometryRef().Buffer(1)
+
+        if not raster_bbox.Intersect(geom):
+            continue
+
+        if not geom.Within(raster_bbox):
+            geom = geom.Intersection(raster_bbox)
+
         minX, maxX, minY, maxY = geom.GetEnvelope()
 
         new_feature: ogr.Feature = ogr.Feature(memory_layer.GetLayerDefn())
         new_feature.SetGeometry(geom)
         memory_layer.SetFeature(new_feature)
 
         rMinX, rMaxY = raster_coordinates(minX, maxY, inv_gt)
@@ -79,17 +90,17 @@
         t25_water = get_water_height_array(t25_band, rMinX, rMaxX, rMinY, rMaxY)
         t100_water = get_water_height_array(t100_band, rMinX, rMaxX, rMinY, rMaxY)
 
         t10_max_water_height = np.max(feature_rasterized * t10_water)
         t25_max_water_height = np.max(feature_rasterized * t25_water)
         t100_max_water_height = np.max(feature_rasterized * t100_water)
 
-        feature.SetField(water_depth_t10_index, t10_max_water_height)
-        feature.SetField(water_depth_t25_index, t25_max_water_height)
-        feature.SetField(water_depth_t100_index, t100_max_water_height)
+        feature.SetField(water_depth_t10_index, float(t10_max_water_height))
+        feature.SetField(water_depth_t25_index, float(t25_max_water_height))
+        feature.SetField(water_depth_t100_index, float(t100_max_water_height))
 
         feature.SetField(t10_index, column_value(t10_max_water_height))
         feature.SetField(t25_index, column_value(t25_max_water_height))
         feature.SetField(t100_index, column_value(t100_max_water_height))
 
         buildings_layer.SetFeature(feature)
```

### Comparing `limburg_flood_impact-0.4.1/src/limburg_flood_impact/combine_classification.py` & `limburg_flood_impact-0.5.0/src/limburg_flood_impact/combine_classification.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.4.1/src/limburg_flood_impact/test_against_flood_protection_norm.py` & `limburg_flood_impact-0.5.0/src/limburg_flood_impact/test_against_flood_protection_norm.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.4.1/src/limburg_flood_impact.egg-info/PKG-INFO` & `limburg_flood_impact-0.5.0/src/limburg_flood_impact.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limburg-flood-impact
-Version: 0.4.1
+Version: 0.5.0
 Summary: Libmurg Flood Impact Package.
 Home-page: https://github.com/
 Author: Lutra Consulting Ltd.
 Author-email: jan.caha@lutraconsulting.co.uk
 License: MIT
 Project-URL: Documentation, https://
 Platform: any
```

### Comparing `limburg_flood_impact-0.4.1/src/limburg_flood_impact.egg-info/SOURCES.txt` & `limburg_flood_impact-0.5.0/src/limburg_flood_impact.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 src/limburg_flood_impact/__init__.py
 src/limburg_flood_impact/_functions.py
 src/limburg_flood_impact/check_address.py
 src/limburg_flood_impact/classify_area_wide_rain.py
 src/limburg_flood_impact/classify_rural_rain.py
 src/limburg_flood_impact/classify_urban_rain.py
 src/limburg_flood_impact/combine_classification.py
+src/limburg_flood_impact/extent_tile.py
+src/limburg_flood_impact/test.py
 src/limburg_flood_impact/test_against_flood_protection_norm.py
 src/limburg_flood_impact.egg-info/PKG-INFO
 src/limburg_flood_impact.egg-info/SOURCES.txt
 src/limburg_flood_impact.egg-info/dependency_links.txt
 src/limburg_flood_impact.egg-info/entry_points.txt
 src/limburg_flood_impact.egg-info/not-zip-safe
 src/limburg_flood_impact.egg-info/requires.txt
```

