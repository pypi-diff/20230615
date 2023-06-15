# Comparing `tmp/pyramm-1.8.tar.gz` & `tmp/pyramm-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyramm-1.8.tar", max compression
+gzip compressed data, was "pyramm-1.9.tar", max compression
```

## Comparing `pyramm-1.8.tar` & `pyramm-1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1068 2021-07-15 04:17:39.667177 pyramm-1.8/LICENSE
--rw-r--r--   0        0        0     3371 2021-07-15 04:17:39.667177 pyramm-1.8/README.md
--rw-r--r--   0        0        0      643 2021-07-15 04:17:39.667177 pyramm-1.8/pyproject.toml
--rw-r--r--   0        0        0      371 2021-07-15 04:17:39.667177 pyramm-1.8/pyramm/__init__.py
--rw-r--r--   0        0        0     7584 2021-07-15 04:17:39.667177 pyramm-1.8/pyramm/api.py
--rw-r--r--   0        0        0     1440 2021-07-15 04:17:39.667177 pyramm-1.8/pyramm/cache.py
--rw-r--r--   0        0        0      206 2021-07-15 04:17:39.667177 pyramm-1.8/pyramm/config.py
--rw-r--r--   0        0        0    12226 2021-07-15 04:17:39.667177 pyramm-1.8/pyramm/geometry.py
--rw-r--r--   0        0        0      235 2021-07-15 04:17:39.667177 pyramm-1.8/pyramm/helpers.py
--rw-r--r--   0        0        0       34 2021-07-15 04:17:39.667177 pyramm-1.8/pyramm/ops/__init__.py
--rw-r--r--   0        0        0     4788 2021-07-15 04:17:39.667177 pyramm-1.8/pyramm/ops/top_surface.py
--rw-r--r--   0        0        0     4944 2021-07-15 04:17:39.667177 pyramm-1.8/pyramm/tables.py
--rw-r--r--   0        0        0     4360 2021-07-15 04:17:42.842567 pyramm-1.8/setup.py
--rw-r--r--   0        0        0     4209 2021-07-15 04:17:42.843025 pyramm-1.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-03-22 00:36:19.810015 pyramm-1.9/LICENSE
+-rw-r--r--   0        0        0     3371 2022-03-22 00:36:19.810015 pyramm-1.9/README.md
+-rw-r--r--   0        0        0      665 2022-03-22 00:36:19.810015 pyramm-1.9/pyproject.toml
+-rw-r--r--   0        0        0      570 2022-03-22 00:36:19.810015 pyramm-1.9/pyramm/__init__.py
+-rw-r--r--   0        0        0     7584 2022-03-22 00:36:19.810015 pyramm-1.9/pyramm/api.py
+-rw-r--r--   0        0        0     1440 2022-03-22 00:36:19.810015 pyramm-1.9/pyramm/cache.py
+-rw-r--r--   0        0        0      206 2022-03-22 00:36:19.810015 pyramm-1.9/pyramm/config.py
+-rw-r--r--   0        0        0    12226 2022-03-22 00:36:19.810015 pyramm-1.9/pyramm/geometry.py
+-rw-r--r--   0        0        0      235 2022-03-22 00:36:19.810015 pyramm-1.9/pyramm/helpers.py
+-rw-r--r--   0        0        0       34 2022-03-22 00:36:19.810015 pyramm-1.9/pyramm/ops/__init__.py
+-rw-r--r--   0        0        0     4788 2022-03-22 00:36:19.810015 pyramm-1.9/pyramm/ops/top_surface.py
+-rw-r--r--   0        0        0     5072 2022-03-22 00:36:19.810015 pyramm-1.9/pyramm/tables.py
+-rw-r--r--   0        0        0     4360 2022-03-22 00:36:24.189505 pyramm-1.9/setup.py
+-rw-r--r--   0        0        0     4260 2022-03-22 00:36:24.190015 pyramm-1.9/PKG-INFO
```

### Comparing `pyramm-1.8/LICENSE` & `pyramm-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyramm-1.8/README.md` & `pyramm-1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyramm-1.8/pyproject.toml` & `pyramm-1.9/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyramm"
-version = "1.8"
+version = "1.9"
 description = "Provides a wrapper to the RAMM API and additional tools for positional referencing"
 authors = ["John Bull"]
 homepage = "https://github.com/captif-nz/pyramm"
 license = "MIT"
 readme = "README.md"
 keywords = ["CAPTIF", "RAMM"]
 
@@ -18,11 +18,12 @@
 scipy = "^1.5.4"
 pyproj = "^3.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.1.2"
 pre-commit = "^2.9.2"
 black = "^20.8b1"
+pytest-cov = "^3.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyramm-1.8/pyramm/api.py` & `pyramm-1.9/pyramm/api.py`

 * *Files identical despite different names*

### Comparing `pyramm-1.8/pyramm/cache.py` & `pyramm-1.9/pyramm/cache.py`

 * *Files identical despite different names*

### Comparing `pyramm-1.8/pyramm/geometry.py` & `pyramm-1.9/pyramm/geometry.py`

 * *Files identical despite different names*

### Comparing `pyramm-1.8/pyramm/ops/top_surface.py` & `pyramm-1.9/pyramm/ops/top_surface.py`

 * *Files identical despite different names*

### Comparing `pyramm-1.8/pyramm/tables.py` & `pyramm-1.9/pyramm/tables.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from pandas import DataFrame, to_datetime, read_csv, notnull
 
 from pyramm.helpers import _map_json
 from pyramm.geometry import transform, loads
 
 
 DEFAULT_DATE_COLUMNS = ["added_on", "chgd_on"]
@@ -27,16 +28,17 @@
             self.df.set_index(self.index_name, drop=True, inplace=True)
 
     def _get_data(self, ramm, road_id, latest):
         self.df = ramm.get_data(
             self.table_name, road_id, latest, self.get_geometry
         ).copy()
         if "wkt" in self.df.columns:
-            # self.df["geometry"] = transform([loads(ww) for ww in self.df["wkt"]])
-            self.df["geometry"] = [transform(loads(ww)) for ww in self.df["wkt"]]
+            with warnings.catch_warnings():
+                warnings.filterwarnings("ignore")
+                self.df["geometry"] = [transform(loads(ww)) for ww in self.df["wkt"]]
 
     def _convert_dates(self):
         date_columns = set(self.date_columns + DEFAULT_DATE_COLUMNS)
         for cc in date_columns:
             try:
                 self.df[cc] = to_datetime(self.df[cc])
             except KeyError:
@@ -46,15 +48,17 @@
         self.df = self.df.where(notnull(self.df), None)
 
     @classmethod
     def from_csv(cls, path):
         new = cls(None)
         new.df = read_csv(path, index_col=cls.index_name, float_precision="%g")
         if "wkt" in new.df.columns:
-            new.df["geometry"] = [transform(loads(ww)) for ww in new.df["wkt"]]
+            with warnings.catch_warnings():
+                warnings.filterwarnings("ignore")
+                new.df["geometry"] = [transform(loads(ww)) for ww in new.df["wkt"]]
         new._convert_dates()
         new._replace_nan()
         return new.df
 
     @classmethod
     def from_frame(cls, df):
         new = cls(None)
```

### Comparing `pyramm-1.8/setup.py` & `pyramm-1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'pandas>=1.1.4,<2.0.0',
  'pyproj>=3.0.0,<4.0.0',
  'requests>=2.25.0,<3.0.0',
  'scipy>=1.5.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'pyramm',
-    'version': '1.8',
+    'version': '1.9',
     'description': 'Provides a wrapper to the RAMM API and additional tools for positional referencing',
     'long_description': '# pyramm\n\nPython wrapper for RAMM API.\n\n**Users must have their own login for the RAMM database.**\n\n## Issues\n\nPlease submit an issue if you find a bug or have an idea for an improvement.\n\n## Installation\n\n```\npip install pyramm\n```\n\n## Initialise\n\nYou must first initialise the connection to the RAMM API as follows. Note that the\n`database` argument defaults to `"SH New Zealand"` if it is not provided.\n\n```\nfrom pyramm.api import Connection\nconn = Connection(username, password, database="SH New Zealand")\n```\n\nAlternatively the username and password can be stored in file called `.pyramm.ini`. This\nfile must be saved in the users home directory (`"~"` on linux) and contain the following:\n\n```\n[RAMM]\nUSERNAME = username\nPASSWORD = password\n```\n\nYou are then able to initialise the RAMM API connection without providing your login\ncredentials each time.\n\n```\nfrom pyramm.api import Connection\nconn = Connection()\n```\n\n## Table and column names\n\nA list of available tables can be accessed using:\n\n```\ntable_names = conn.table_names()\n```\n\nA list of columns for a given table can be accessed using:\n\n```\ncolumn_names = conn.column_names(table_name)\n```\n\n## Table data\n\nSome methods are attached to the `Connection` object to provide convenient access to\nselected RAMM tables. These helper methods implement some additional filtering (exposed\nas method arguments) and automatically set the DataFrame index to the correct table\ncolumn(s).\n\nTables not listed in the sections below can be accessed using the general `get_data()`\nmethod:\n\n```\ndf = conn.get_data(table_name)\n```\n\n### General tables:\n```\nroadnames = conn.roadnames()\n```\n```\ncarrway = conn.carr_way(road_id=None)\n```\n```\nc_surface = conn.c_surface(road_id=None)\n```\n```\ntop_surface = conn.top_surface()\n```\n```\nsurf_material = conn.surf_material()\n```\n```\nsurf_category = conn.surf_category()\n```\n```\nminor_structure = conn.minor_structure()\n```\n\n### HSD tables:\n\n```\nhsd_roughness = conn.hsd_roughness(road_id, latest=True, survey_year=None)\n```\n```\nhsd_roughness_hdr = conn.hsd_roughness_hdr()\n```\n```\nhsd_rutting = conn.hsd_rutting(road_id, latest=True, survey_year=None)\n```\n```\nhsd_rutting_hdr = conn.hsd_rutting_hdr()\n```\n```\nhsd_texture = conn.hsd_texture(road_id, latest=True, survey_year=None)\n```\n```\nhsd_texture_hdr = conn.hsd_texture_hdr()\n```\n\n## Centreline\n\nThe `Centreline` object is provided to:\n - assist with generating geometry for table entries (based on `road_id`, `start_m` and\n`end_m` values),\n <!-- - find the nearest geometry element to give a point (`latitude`, `longitude`),\n - find the displacement (in metres) along the nearest geometry element given a point\n(`latitude`, `longitude`). -->\n\nThe base geometry used by the `Centreline` object is derived from the `carr_way` table.\n\n### Create a Centreline instance:\n\n```\ncentreline = conn.centreline()\n```\n\n### Append geometry to table:\n\nFor a table containing `road_id`, `start_m` and `end_m` columns, the geometry can be\nappended using the `append_geometry()` method:\n\n```\ndf = centreline.append_geometry(df, geometry_type="wkt")\n```\n\nThe `geometry_type` argument defaults to `"wkt"`. This will provide a\n[WKT](https://en.wikipedia.org/wiki/Well-known_text_representation_of_geometry)\nLineString for each row.\n\nAlternatively, `geometry_type` can be set to `"coord"` to append\na `northing` and `easting` column to the DataFrame.\n',
     'author': 'John Bull',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/captif-nz/pyramm',
```

### Comparing `pyramm-1.8/PKG-INFO` & `pyramm-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pyramm
-Version: 1.8
+Version: 1.9
 Summary: Provides a wrapper to the RAMM API and additional tools for positional referencing
 Home-page: https://github.com/captif-nz/pyramm
 License: MIT
 Keywords: CAPTIF,RAMM
 Author: John Bull
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Shapely (>=1.7.1,<2.0.0)
 Requires-Dist: geopandas (>=0.8.1,<0.9.0)
 Requires-Dist: numpy (>=1.19.4,<2.0.0)
 Requires-Dist: pandas (>=1.1.4,<2.0.0)
```

