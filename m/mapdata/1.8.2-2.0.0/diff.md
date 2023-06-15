# Comparing `tmp/mapdata-1.8.2.tar.gz` & `tmp/mapdata-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapdata-1.8.2.tar", last modified: Thu May 25 02:00:57 2023, max compression
+gzip compressed data, was "mapdata-2.0.0.tar", last modified: Thu Jun 15 04:38:32 2023, max compression
```

## Comparing `mapdata-1.8.2.tar` & `mapdata-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-05-25 02:00:57.572999 mapdata-1.8.2/
--rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-1.8.2/LICENSE.txt
--rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-1.8.2/MANIFEST.in
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     3009 2023-05-25 02:00:57.572999 mapdata-1.8.2/PKG-INFO
--rw-r--r--   0 dreas     (1000) dreas     (1000)     1866 2023-05-15 01:02:57.000000 mapdata-1.8.2/README.md
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-05-25 02:00:57.568999 mapdata-1.8.2/mapdata/
--rwxr-xr-x   0 dreas     (1000) dreas     (1000)    86410 2023-05-25 01:40:23.000000 mapdata-1.8.2/mapdata/mapdata.py
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-05-25 02:00:57.572999 mapdata-1.8.2/mapdata.egg-info/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     3009 2023-05-25 02:00:57.000000 mapdata-1.8.2/mapdata.egg-info/PKG-INFO
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-05-25 02:00:57.000000 mapdata-1.8.2/mapdata.egg-info/SOURCES.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-05-25 02:00:57.000000 mapdata-1.8.2/mapdata.egg-info/dependency_links.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-05-25 02:00:57.000000 mapdata-1.8.2/mapdata.egg-info/top_level.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-05-25 02:00:57.572999 mapdata-1.8.2/setup.cfg
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     1279 2023-05-25 02:00:53.000000 mapdata-1.8.2/setup.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-15 04:38:32.639052 mapdata-2.0.0/
+-rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-2.0.0/LICENSE.txt
+-rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-2.0.0/MANIFEST.in
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     3583 2023-06-15 04:38:32.639052 mapdata-2.0.0/PKG-INFO
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     2385 2023-06-15 03:39:51.000000 mapdata-2.0.0/README.md
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-15 04:38:32.639052 mapdata-2.0.0/mapdata/
+-rwxrwxr-x   0 dreas     (1000) dreas     (1000)   157904 2023-06-15 03:33:47.000000 mapdata-2.0.0/mapdata/mapdata.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-15 04:38:32.639052 mapdata-2.0.0/mapdata.egg-info/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     3583 2023-06-15 04:38:32.000000 mapdata-2.0.0/mapdata.egg-info/PKG-INFO
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-06-15 04:38:32.000000 mapdata-2.0.0/mapdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-15 04:38:32.000000 mapdata-2.0.0/mapdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-15 04:38:32.000000 mapdata-2.0.0/mapdata.egg-info/top_level.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-06-15 04:38:32.639052 mapdata-2.0.0/setup.cfg
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     1313 2023-06-15 04:38:26.000000 mapdata-2.0.0/setup.py
```

### Comparing `mapdata-1.8.2/LICENSE.txt` & `mapdata-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapdata-1.8.2/PKG-INFO` & `mapdata-2.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 1.8.2
+Version: 2.0.0
 Summary: An interactive map and table explorer for geographic coordinates in a CSV file
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,PNG,JPG,Postscript
 Platform: UNKNOWN
@@ -21,22 +21,27 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Scientific/Engineering
 Requires: tkintermapview
 Requires: pyproj
 Requires: odfpy
+Requires: openpyxl
+Requires: xlrd
+Requires: matplotlib
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
-*mapdata.py* is a viewer for geographic coordinate data read from a CSV file.  Both a map and a data
+*mapdata.py* is a viewer for geographic coordinate data read from a CSV file, spreadsheet,
+or database.  Both a map and a data
 table are displayed.  When a location is selected on the map, the same location is highlighted in the
-table, and *vice-versa*.  Single or multiple selections may be enabled.
+table, and *vice-versa*.  Single or multiple selections may be enabled.  Locations may also
+be selected and highlighted by writing a query expression to select rows of the data table.
 
 Coordinates should be in decimal degrees, in WGS84 (coordinate reference system [CRS] 4326), however,
 coordinates in other CRSs can be converted to 4326.
 
 The map display can be customized in several ways:
 
   * Different raster tile servers may be used for the basemap.  The default is
@@ -53,15 +58,21 @@
   * Locations may be unlabeled or labeled with data values from the data file
     The label font, size, color, and location can all be customized.
 
 The map can be exported to a Postscript, PNG, or JPEG file.  Using command-line options,
 *mapdata* can be directed to load a data file and display location markers and then to
 export the map to an image file, and quit.
 
-Selected rows in the data table can be exported to a CSV file.
+Selected rows in the data table can be exported to a CSV or spreadsheet file.
+
+Data can also be displayed in several different types of plots: box plots, scatter
+plots, line charts, and counts of categorical and quantitative variables.  Plots
+can use either all data or only data values that are selected in the map and
+table.  Plots have a live connection to the data table, so when selections are
+changed the plots are automatically updated.
 
 
 Complete documentation is at [https://mapdata.osdn.io](https://mapdata.osdn.io).
 
 A configuration file template, application icons for Linux and Windows, a .desktop
 file for Linux, and additional bitmap symbols, are available for download from
 [OSDN](https://osdn.net/projects/mapdata/releases/).
```

### Comparing `mapdata-1.8.2/README.md` & `mapdata-2.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
-*mapdata.py* is a viewer for geographic coordinate data read from a CSV file.  Both a map and a data
+*mapdata.py* is a viewer for geographic coordinate data read from a CSV file, spreadsheet,
+or database.  Both a map and a data
 table are displayed.  When a location is selected on the map, the same location is highlighted in the
-table, and *vice-versa*.  Single or multiple selections may be enabled.
+table, and *vice-versa*.  Single or multiple selections may be enabled.  Locations may also
+be selected and highlighted by writing a query expression to select rows of the data table.
 
 Coordinates should be in decimal degrees, in WGS84 (coordinate reference system [CRS] 4326), however,
 coordinates in other CRSs can be converted to 4326.
 
 The map display can be customized in several ways:
 
   * Different raster tile servers may be used for the basemap.  The default is
@@ -22,15 +24,21 @@
   * Locations may be unlabeled or labeled with data values from the data file
     The label font, size, color, and location can all be customized.
 
 The map can be exported to a Postscript, PNG, or JPEG file.  Using command-line options,
 *mapdata* can be directed to load a data file and display location markers and then to
 export the map to an image file, and quit.
 
-Selected rows in the data table can be exported to a CSV file.
+Selected rows in the data table can be exported to a CSV or spreadsheet file.
+
+Data can also be displayed in several different types of plots: box plots, scatter
+plots, line charts, and counts of categorical and quantitative variables.  Plots
+can use either all data or only data values that are selected in the map and
+table.  Plots have a live connection to the data table, so when selections are
+changed the plots are automatically updated.
 
 
 Complete documentation is at [https://mapdata.osdn.io](https://mapdata.osdn.io).
 
 A configuration file template, application icons for Linux and Windows, a .desktop
 file for Linux, and additional bitmap symbols, are available for download from
 [OSDN](https://osdn.net/projects/mapdata/releases/).
```

### Comparing `mapdata-1.8.2/mapdata.egg-info/PKG-INFO` & `mapdata-2.0.0/mapdata.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 1.8.2
+Version: 2.0.0
 Summary: An interactive map and table explorer for geographic coordinates in a CSV file
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,PNG,JPG,Postscript
 Platform: UNKNOWN
@@ -21,22 +21,27 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Scientific/Engineering
 Requires: tkintermapview
 Requires: pyproj
 Requires: odfpy
+Requires: openpyxl
+Requires: xlrd
+Requires: matplotlib
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
-*mapdata.py* is a viewer for geographic coordinate data read from a CSV file.  Both a map and a data
+*mapdata.py* is a viewer for geographic coordinate data read from a CSV file, spreadsheet,
+or database.  Both a map and a data
 table are displayed.  When a location is selected on the map, the same location is highlighted in the
-table, and *vice-versa*.  Single or multiple selections may be enabled.
+table, and *vice-versa*.  Single or multiple selections may be enabled.  Locations may also
+be selected and highlighted by writing a query expression to select rows of the data table.
 
 Coordinates should be in decimal degrees, in WGS84 (coordinate reference system [CRS] 4326), however,
 coordinates in other CRSs can be converted to 4326.
 
 The map display can be customized in several ways:
 
   * Different raster tile servers may be used for the basemap.  The default is
@@ -53,15 +58,21 @@
   * Locations may be unlabeled or labeled with data values from the data file
     The label font, size, color, and location can all be customized.
 
 The map can be exported to a Postscript, PNG, or JPEG file.  Using command-line options,
 *mapdata* can be directed to load a data file and display location markers and then to
 export the map to an image file, and quit.
 
-Selected rows in the data table can be exported to a CSV file.
+Selected rows in the data table can be exported to a CSV or spreadsheet file.
+
+Data can also be displayed in several different types of plots: box plots, scatter
+plots, line charts, and counts of categorical and quantitative variables.  Plots
+can use either all data or only data values that are selected in the map and
+table.  Plots have a live connection to the data table, so when selections are
+changed the plots are automatically updated.
 
 
 Complete documentation is at [https://mapdata.osdn.io](https://mapdata.osdn.io).
 
 A configuration file template, application icons for Linux and Windows, a .desktop
 file for Linux, and additional bitmap symbols, are available for download from
 [OSDN](https://osdn.net/projects/mapdata/releases/).
```

### Comparing `mapdata-1.8.2/setup.py` & `mapdata-2.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 import io
 
 with io.open('README.md', encoding='utf-8') as f:
 	long_description = f.read()
 
 setuptools.setup(name='mapdata',
-	version='1.8.2',
+	version='2.0.0',
 	description="An interactive map and table explorer for geographic coordinates in a CSV file",
 	author='Dreas Nielsen',
 	author_email='dreas.nielsen@gmail.com',
     url='https://osdn.net/project/mapdata/',
 	scripts=['mapdata/mapdata.py'],
     license='GPL',
-	requires=['tkintermapview', 'pyproj', 'odfpy'],
+	requires=['tkintermapview', 'pyproj', 'odfpy', 'openpyxl', 'xlrd', 'matplotlib'],
 	python_requires = '>=3.8',
 	classifiers=[
 		'Development Status :: 5 - Production/Stable',
 		'Environment :: Console',
 		'Environment :: X11 Applications',
 		'Environment :: Win32 (MS Windows)',
 		'Intended Audience :: End Users/Desktop',
```

