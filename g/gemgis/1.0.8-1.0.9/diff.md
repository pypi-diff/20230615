# Comparing `tmp/gemgis-1.0.8.tar.gz` & `tmp/gemgis-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemgis-1.0.8.tar", last modified: Wed Mar  1 11:23:32 2023, max compression
+gzip compressed data, was "gemgis-1.0.9.tar", last modified: Mon Mar 13 08:55:15 2023, max compression
```

## Comparing `gemgis-1.0.8.tar` & `gemgis-1.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:23:32.284960 gemgis-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-03-01 11:23:22.000000 gemgis-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-01 11:23:22.000000 gemgis-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-03-01 11:23:32.284960 gemgis-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-03-01 11:23:22.000000 gemgis-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:23:32.280960 gemgis-1.0.8/gemgis/
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-03-01 11:23:23.000000 gemgis-1.0.8/gemgis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-03-01 11:23:23.000000 gemgis-1.0.8/gemgis/download_gemgis_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    25773 2023-03-01 11:23:23.000000 gemgis-1.0.8/gemgis/gemgis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-03-01 11:23:23.000000 gemgis-1.0.8/gemgis/ipynb_to_py.py
--rw-r--r--   0 runner    (1001) docker     (123)    43487 2023-03-01 11:23:23.000000 gemgis-1.0.8/gemgis/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18917 2023-03-01 11:23:23.000000 gemgis-1.0.8/gemgis/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    97041 2023-03-01 11:23:23.000000 gemgis-1.0.8/gemgis/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)    70953 2023-03-01 11:23:23.000000 gemgis-1.0.8/gemgis/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   306834 2023-03-01 11:23:23.000000 gemgis-1.0.8/gemgis/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)   168572 2023-03-01 11:23:23.000000 gemgis-1.0.8/gemgis/visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    36545 2023-03-01 11:23:23.000000 gemgis-1.0.8/gemgis/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:23:32.284960 gemgis-1.0.8/gemgis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-03-01 11:23:32.000000 gemgis-1.0.8/gemgis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-01 11:23:32.000000 gemgis-1.0.8/gemgis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 11:23:32.000000 gemgis-1.0.8/gemgis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-01 11:23:32.000000 gemgis-1.0.8/gemgis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-01 11:23:23.000000 gemgis-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-01 11:23:23.000000 gemgis-1.0.8/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 11:23:32.284960 gemgis-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-01 11:23:23.000000 gemgis-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:23:32.284960 gemgis-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 11:23:23.000000 gemgis-1.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52875 2023-03-01 11:23:23.000000 gemgis-1.0.8/tests/test_gemgis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-03-01 11:23:23.000000 gemgis-1.0.8/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    48083 2023-03-01 11:23:23.000000 gemgis-1.0.8/tests/test_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)    49831 2023-03-01 11:23:23.000000 gemgis-1.0.8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   244522 2023-03-01 11:23:23.000000 gemgis-1.0.8/tests/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    21485 2023-03-01 11:23:23.000000 gemgis-1.0.8/tests/test_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    32196 2023-03-01 11:23:23.000000 gemgis-1.0.8/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:55:15.068968 gemgis-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-03-13 08:54:59.000000 gemgis-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-13 08:54:59.000000 gemgis-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-03-13 08:55:15.068968 gemgis-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-03-13 08:54:59.000000 gemgis-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:55:15.064968 gemgis-1.0.9/gemgis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-03-13 08:55:01.000000 gemgis-1.0.9/gemgis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-03-13 08:55:01.000000 gemgis-1.0.9/gemgis/download_gemgis_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25773 2023-03-13 08:55:01.000000 gemgis-1.0.9/gemgis/gemgis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-03-13 08:55:01.000000 gemgis-1.0.9/gemgis/ipynb_to_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43487 2023-03-13 08:55:01.000000 gemgis-1.0.9/gemgis/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34969 2023-03-13 08:55:01.000000 gemgis-1.0.9/gemgis/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97127 2023-03-13 08:55:01.000000 gemgis-1.0.9/gemgis/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70974 2023-03-13 08:55:01.000000 gemgis-1.0.9/gemgis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   306834 2023-03-13 08:55:01.000000 gemgis-1.0.9/gemgis/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)   169060 2023-03-13 08:55:01.000000 gemgis-1.0.9/gemgis/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36545 2023-03-13 08:55:01.000000 gemgis-1.0.9/gemgis/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:55:15.064968 gemgis-1.0.9/gemgis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-03-13 08:55:15.000000 gemgis-1.0.9/gemgis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-13 08:55:15.000000 gemgis-1.0.9/gemgis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 08:55:15.000000 gemgis-1.0.9/gemgis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-13 08:55:15.000000 gemgis-1.0.9/gemgis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-13 08:55:01.000000 gemgis-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-13 08:55:01.000000 gemgis-1.0.9/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 08:55:15.068968 gemgis-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-13 08:55:01.000000 gemgis-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 08:55:15.068968 gemgis-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 08:55:01.000000 gemgis-1.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52875 2023-03-13 08:55:01.000000 gemgis-1.0.9/tests/test_gemgis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-03-13 08:55:01.000000 gemgis-1.0.9/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48083 2023-03-13 08:55:01.000000 gemgis-1.0.9/tests/test_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49831 2023-03-13 08:55:01.000000 gemgis-1.0.9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   244522 2023-03-13 08:55:01.000000 gemgis-1.0.9/tests/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21485 2023-03-13 08:55:01.000000 gemgis-1.0.9/tests/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32196 2023-03-13 08:55:01.000000 gemgis-1.0.9/tests/test_web.py
```

### Comparing `gemgis-1.0.8/LICENSE` & `gemgis-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gemgis-1.0.8/PKG-INFO` & `gemgis-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemgis
-Version: 1.0.8
+Version: 1.0.9
 Summary: GemGIS is a Python-based, open-source spatial data processing library.
 Home-page: https://github.com/cgre-aachen/gemgis
 Author: Alexander Jüstel, Arthur Endlein Correia, Florian Wellmann, Marius Pischke
 Author-email: alexander.juestel@rwth-aachen.de
 License: LGPL v3
 Keywords: geology,geographic,structural geology,GIS,spatial data
 Description-Content-Type: text/markdown
```

### Comparing `gemgis-1.0.8/README.md` & `gemgis-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gemgis-1.0.8/gemgis/__init__.py` & `gemgis-1.0.9/gemgis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 __authors__ = """Alexander Jüstel, Arthur Endlein Correia, Marius Pischke, Florian Wellmann"""
 
 __correspondence_email__ = 'alexander.juestel@rwth-aachen.de'
 
 __affiliations__ = 'CGRE - RWTH Aachen University'
 
-__version_date__ = '2023-02-07'
+__version_date__ = '2023-03-13'
 
-__version__ = '1.0.8'
+__version__ = '1.0.9'
 
-__changelog__ = """What is new in version 1.0.8:
+__changelog__ = """What is new in version 1.0.9:
 
 
 
 """
```

### Comparing `gemgis-1.0.8/gemgis/download_gemgis_data.py` & `gemgis-1.0.9/gemgis/download_gemgis_data.py`

 * *Files identical despite different names*

### Comparing `gemgis-1.0.8/gemgis/gemgis.py` & `gemgis-1.0.9/gemgis/gemgis.py`

 * *Files identical despite different names*

### Comparing `gemgis-1.0.8/gemgis/ipynb_to_py.py` & `gemgis-1.0.9/gemgis/ipynb_to_py.py`

 * *Files identical despite different names*

### Comparing `gemgis-1.0.8/gemgis/misc.py` & `gemgis-1.0.9/gemgis/misc.py`

 * *Files identical despite different names*

### Comparing `gemgis-1.0.8/gemgis/raster.py` & `gemgis-1.0.9/gemgis/raster.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import rasterio
 from rasterio.merge import merge
 from rasterio.warp import calculate_default_transform, reproject, Resampling
 import pandas as pd
 import geopandas as gpd
 from typing import Union, List, Sequence, Optional, Iterable, Dict, Tuple
 from rasterio.mask import mask
-from shapely.geometry import box, Polygon
+from shapely.geometry import box, Polygon, LineString
 import shapely
 from pathlib import Path
 import affine
 import pyproj
 
 
 def sample_from_array(array: np.ndarray,
@@ -1560,15 +1560,16 @@
 
     """
 
     # Trying to import skimage but returning error if skimage is not installed
     try:
         from skimage.transform import resize
     except ModuleNotFoundError:
-        raise ModuleNotFoundError('Scikit Image package is not installed. Use pip install scikit-image to install the latest version')
+        raise ModuleNotFoundError(
+            'Scikit Image package is not installed. Use pip install scikit-image to install the latest version')
 
     # Checking if array1 is of type np.ndarray
     if not isinstance(raster, (np.ndarray, rasterio.io.DatasetReader)):
         raise TypeError('Raster must be of type np.ndarray')
 
     # Converting rasterio object to array
     if isinstance(raster, rasterio.io.DatasetReader):
@@ -1856,17 +1857,17 @@
             if line_value == 'xllcenter':
                 xllcenter = float(values[0])
             if line_value == 'yllcenter':
                 yllcenter = float(values[0])
             if line_value == 'cellsize':
                 res = float(values[0])
             if line_value == 'xllcorner':
-                xllcenter = float(values[0]) + 0.5*res
+                xllcenter = float(values[0]) + 0.5 * res
             if line_value == 'yllcorner':
-                yllcenter = float(values[0]) + 0.5*res
+                yllcenter = float(values[0]) + 0.5 * res
             if line_value == 'NODATA_value' or line_value == 'nodata_value':
                 nodata_val = float(values[0])
 
     # Load data and replace nodata_values with np.nan
     data = np.loadtxt(path, skiprows=6).reshape(nrows, ncols)
     data[data == nodata_val] = np.nan
 
@@ -1992,15 +1993,15 @@
 
 # Opening and saving Raster Data
 ################################
 
 
 def save_as_tiff(raster: np.ndarray,
                  path: str,
-                 extent: List[Union[int, float]],
+                 extent: Union[List[Union[int, float]], Tuple[Union[int, float]]],
                  crs: Union[str, pyproj.crs.crs.CRS, rasterio.crs.CRS],
                  nodata: Union[float, int] = None,
                  transform=None,
                  overwrite_file: bool = False,
                  create_directory: bool = False):
     """Saving a np.array as tif file
 
@@ -2009,15 +2010,15 @@
 
         array : np.ndarray
             Array containing the raster values
 
         path : string
             Path and name of the file, e.g. ``path='mesh.msh'``
 
-        extent : List[Union[int, float]]
+        extent : Union[List[Union[int, float]], Tuple[Union[int, float]]]
             List containing the bounds of the raster,
             e.g. ``extent=[0, 972, 0, 1069]``
 
         crs : Union[str, pyproj.crs.crs.CRS, rasterio.crs.CRS]
             CRS of the saved raster, e.g. ``crs='EPSG:4647'``
 
         nodata : Union[float, int]
@@ -2079,16 +2080,16 @@
                 "The file already exists. Pass overwrite_file=True to overwrite the existing file")
 
     # Checking if the array is of type np.ndarray
     if not isinstance(raster, np.ndarray):
         raise TypeError('array must be of type np.ndarray')
 
     # Checking if the extent is of type list
-    if not isinstance(extent, list):
-        raise TypeError('Extent must be of type list')
+    if not isinstance(extent, (list, tuple)):
+        raise TypeError('Extent must be of type list or be a tuple')
 
     # Checking that all values are either ints or floats
     if not all(isinstance(n, (int, float)) for n in extent):
         raise TypeError('Bound values must be of type int or float')
 
     # Checking if the crs is of type string
     if not isinstance(crs, (str, pyproj.crs.crs.CRS, rasterio.crs.CRS, dict)):
@@ -2538,15 +2539,16 @@
                 dst_crs=dst_crs,
                 resampling=Resampling.nearest)
 
 
 def extract_contour_lines_from_raster(raster: Union[rasterio.io.DatasetReader, np.ndarray, str],
                                       interval: int,
                                       extent: Union[Optional[Sequence[float]], Optional[Sequence[int]]] = None,
-                                      target_crs: Union[str, pyproj.crs.crs.CRS, rasterio.crs.CRS] = None) -> gpd.GeoDataFrame:
+                                      target_crs: Union[
+                                          str, pyproj.crs.crs.CRS, rasterio.crs.CRS] = None) -> gpd.GeoDataFrame:
     """Extracting contour lines from raster with a provided interval.
 
     Parameters
     __________
 
         raster: Union[rasterio.io.DatasetReader, np.ndarray, str]
             Raster from which contour lines are extracted
@@ -2578,54 +2580,54 @@
     if not isinstance(raster, (rasterio.io.DatasetReader, np.ndarray, str)):
         raise TypeError("Raster must be a raster loaded with rasterio or a path directing to a .tif file")
 
     # Checking if provided raster is of type str. If provided raster is a path (directing to a .tif file), load the file with rasterio
     if isinstance(raster, str):
         raster = rasterio.open(raster)
 
-        # Checking if provided raster is of type np.ndarray
-        if isinstance(raster, np.ndarray):
-            if extent == None:
-                raise UnboundLocalError(
-                    "For np.ndarray an extent must be provided to extract contour lines from an array")
-
-            if extent is not None and not isinstance(extent, Sequence):
-                raise TypeError("extent values must be of type float or int")
-
-            if len(extent) != 4:
-                raise TypeError("Not enough arguments in extent to extract contour lines from an array")
-
-            if target_crs == None:
-                raise UnboundLocalError("For np.ndarray a target crs must be provided")
-
-            if target_crs is not None and not isinstance(target_crs, (str, pyproj.crs.crs.CRS, rasterio.crs.CRS)):
-                raise TypeError("target_crs must be of type string, pyproj CRS or rasterio CRS")
-
-            gg.raster.save_as_tiff(raster=np.flipud(raster),
-                                   path='input_raster.tif',
-                                   extent=extent,
-                                   crs=target_crs,
-                                   overwrite_file=True)
-            raster = rasterio.open('input_raster.tif')
+    # Checking if provided raster is of type np.ndarray
+    if isinstance(raster, np.ndarray):
+        if extent is None:
+            raise UnboundLocalError(
+                "For np.ndarray an extent must be provided to extract contour lines from an array")
+
+        if extent is not None and not isinstance(extent, Sequence):
+            raise TypeError("extent values must be of type float or int")
+
+        if len(extent) != 4:
+            raise TypeError("Not enough arguments in extent to extract contour lines from an array")
+
+        if target_crs is None:
+            raise UnboundLocalError("For np.ndarray a target crs must be provided")
+
+        if target_crs is not None and not isinstance(target_crs, (str, pyproj.crs.crs.CRS, rasterio.crs.CRS)):
+            raise TypeError("target_crs must be of type string, pyproj CRS or rasterio CRS")
+
+        save_as_tiff(raster=np.flipud(raster),
+                     path='input_raster.tif',
+                     extent=extent,
+                     crs=target_crs,
+                     overwrite_file=True)
+        raster = rasterio.open('input_raster.tif')
 
     # Checking if provided interval is of type int
     if not isinstance(interval, int):
         raise TypeError("Interval must be provided as int")
 
     # Checking if provided interval is negative
     if interval <= 0:
         raise ValueError("Interval must be greater than 0")
 
     # Defining two empty lists to save contours and the corresponding values
     contours = []
     values = []
 
     # Calculating minimum and maximum value from the given raster value
-    min_val = int(interval * round(np.amin(raster.read(1)) / interval))
-    max_val = int(interval * round(np.amax(raster.read(1)) / interval))
+    min_val = int(interval * round(np.amin(raster.read(1)[~np.isnan(raster.read(1))]) / interval))
+    max_val = int(interval * round(np.amax(raster.read(1)[~np.isnan(raster.read(1))]) / interval))
 
     # Extracting contour lines and appending to lists
     for value in range(min_val,
                        max_val,
                        interval):
         contour = measure.find_contours(np.fliplr(raster.read(1).T),
                                         value)
@@ -2651,10 +2653,10 @@
                                   y_new[i]]).T) for i in range(len(x_new))]
 
     # Creating GeoDataFrame from lines
     gdf_lines = gpd.GeoDataFrame(geometry=lines,
                                  crs=raster.crs)
 
     # Adding value column to GeoDataframe
-    gdf_lines['value'] = values
+    gdf_lines['Z'] = values
 
-    return gdf_lines
+    return gdf_lines
```

### Comparing `gemgis-1.0.8/gemgis/utils.py` & `gemgis-1.0.9/gemgis/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2004,16 +2004,16 @@
     # Calculating the intersections
     intersections = [ray_trace_one_surface(surface=surface,
                                            origin=[x_value, y_value, extent[4]],
                                            end_point=[x_value, y_value, extent[5]],
                                            first_point=True) for x_value in x for y_value in y]
 
     # Extracting the height values
-    z_values = np.array([z[0][2] if len(z[0]) == 3 else nodata for z in intersections]).reshape(x_no_cells,
-                                                                                                y_no_cells).T
+    z_values = np.flipud(np.array([z[0][2] if len(z[0]) == 3 else nodata for z in intersections]).reshape(x_no_cells,
+                                                                                                          y_no_cells).T)
 
     return z_values
 
 
 def create_zmap_grid(surface: pv.core.pointset.PolyData,
                      cell_width: int,
                      comments: str = '',
```

### Comparing `gemgis-1.0.8/gemgis/vector.py` & `gemgis-1.0.9/gemgis/vector.py`

 * *Files identical despite different names*

### Comparing `gemgis-1.0.8/gemgis/visualization.py` & `gemgis-1.0.9/gemgis/visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,20 @@
     # Checking that all elements of the GeoDataFrame are of geom_type LineString
     if not all(shapely.get_type_id(gdf.geometry) == 1):
         raise TypeError('All Shapely objects of the GeoDataFrame must be LineStrings')
 
     # Creating list of points
     vertices_list = [list(gdf.geometry[i].coords) for i in range(len(gdf))]
 
+    # Extracting Z values of all points if gdf has no Z but Z value is provided for each LineString in an additional column
+    if (all(gdf.has_z == False)) and ('Z' in gdf.columns):
+        vertices_list_z = [[vertices_list[j][i] + tuple([gdf['Z'].loc[j]]) for i in range(len(vertices_list[j]))] for j
+                           in range(len(vertices_list))]
+        vertices_list = vertices_list_z
+
     # Creating array of points
     points = np.vstack(vertices_list)
 
     # Creating list with number of vertices per points and indices per lines
     lines = []
     start = 0
     for element in vertices_list:
@@ -306,18 +312,18 @@
         x = np.arange(extent[0], extent[1], res)
         y = np.arange(extent[2], extent[3], res)
 
     # Creating meshgrid
     x, y = np.meshgrid(x, y)
 
     # Creating Structured grid
-    grid = pv.StructuredGrid(x, y, dem)
+    grid = pv.StructuredGrid(x, y, np.flipud(dem))
 
     # Assigning elevation values to grid
-    grid["Elevation"] = dem.ravel(order="F")
+    grid["Elevation [m]"] = dem.ravel(order="F")
 
     return grid
 
 
 def create_points_3d(gdf: gpd.geodataframe.GeoDataFrame) -> pv.core.pointset.PolyData:
     """Plotting points in 3D with PyVista
 
@@ -4277,15 +4283,16 @@
     sel = np.round(geo_model.solutions.geological_map[0]).astype(int)[0]
 
     # Converting color values
     scalars_val = pv.convert_array(colors_rgb.loc[sel].values,
                                    array_type=3)
 
     # Creating colormap
-    cm = mcolors.ListedColormap(list(get_color_lot(is_faults=True,
+    cm = mcolors.ListedColormap(list(get_color_lot(geo_model=geo_model,
+                                                   is_faults=True,
                                                    is_basement=True)))
     rgb = True
 
     # Interpolating the polydata and assigning values
     polydata.delaunay_2d(inplace=True)
     polydata['id'] = scalars_val
     polydata['height'] = topography[:, 2]
```

### Comparing `gemgis-1.0.8/gemgis/web.py` & `gemgis-1.0.9/gemgis/web.py`

 * *Files identical despite different names*

### Comparing `gemgis-1.0.8/gemgis.egg-info/PKG-INFO` & `gemgis-1.0.9/gemgis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemgis
-Version: 1.0.8
+Version: 1.0.9
 Summary: GemGIS is a Python-based, open-source spatial data processing library.
 Home-page: https://github.com/cgre-aachen/gemgis
 Author: Alexander Jüstel, Arthur Endlein Correia, Florian Wellmann, Marius Pischke
 Author-email: alexander.juestel@rwth-aachen.de
 License: LGPL v3
 Keywords: geology,geographic,structural geology,GIS,spatial data
 Description-Content-Type: text/markdown
```

### Comparing `gemgis-1.0.8/gemgis.egg-info/SOURCES.txt` & `gemgis-1.0.9/gemgis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gemgis-1.0.8/setup.py` & `gemgis-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from os import path
 
-version = '1.0.8'
+version = '1.0.9'
 
 # Loading Readme for Description on PyPi
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
```

### Comparing `gemgis-1.0.8/tests/test_gemgis.py` & `gemgis-1.0.9/tests/test_gemgis.py`

 * *Files identical despite different names*

### Comparing `gemgis-1.0.8/tests/test_misc.py` & `gemgis-1.0.9/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `gemgis-1.0.8/tests/test_raster.py` & `gemgis-1.0.9/tests/test_raster.py`

 * *Files identical despite different names*

### Comparing `gemgis-1.0.8/tests/test_utils.py` & `gemgis-1.0.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gemgis-1.0.8/tests/test_vector.py` & `gemgis-1.0.9/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `gemgis-1.0.8/tests/test_visualization.py` & `gemgis-1.0.9/tests/test_visualization.py`

 * *Files identical despite different names*

### Comparing `gemgis-1.0.8/tests/test_web.py` & `gemgis-1.0.9/tests/test_web.py`

 * *Files identical despite different names*

