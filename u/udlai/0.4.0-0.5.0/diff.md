# Comparing `tmp/udlai-0.4.0.tar.gz` & `tmp/udlai-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udlai-0.4.0.tar", last modified: Thu Mar  2 10:35:26 2023, max compression
+gzip compressed data, was "udlai-0.5.0.tar", last modified: Thu Jun 15 13:34:34 2023, max compression
```

## Comparing `udlai-0.4.0.tar` & `udlai-0.5.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:35:26.891428 udlai-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-02 10:34:59.000000 udlai-0.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-03-02 10:34:59.000000 udlai-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-02 10:34:59.000000 udlai-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-02 10:34:59.000000 udlai-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-03-02 10:35:26.891428 udlai-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-03-02 10:34:59.000000 udlai-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:35:26.887428 udlai-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-02 10:34:59.000000 udlai-0.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-02 10:34:59.000000 udlai-0.4.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:35:26.887428 udlai-0.4.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:35:26.887428 udlai-0.4.0/docs/source/_static/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6148 2023-03-02 10:34:59.000000 udlai-0.4.0/docs/source/_static/favicon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    14472 2023-03-02 10:34:59.000000 udlai-0.4.0/docs/source/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-02 10:34:59.000000 udlai-0.4.0/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-03-02 10:34:59.000000 udlai-0.4.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-02 10:35:26.891428 udlai-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-03-02 10:34:59.000000 udlai-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:35:26.891428 udlai-0.4.0/udlai/
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-03-02 10:34:59.000000 udlai-0.4.0/udlai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-02 10:35:26.891428 udlai-0.4.0/udlai/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15680 2023-03-02 10:34:59.000000 udlai-0.4.0/udlai/feature_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-03-02 10:34:59.000000 udlai-0.4.0/udlai/geocoding_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:35:26.891428 udlai-0.4.0/udlai/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 10:34:59.000000 udlai-0.4.0/udlai/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-03-02 10:34:59.000000 udlai-0.4.0/udlai/tests/test_feature_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-03-02 10:34:59.000000 udlai-0.4.0/udlai/tests/test_geocoding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:35:26.891428 udlai-0.4.0/udlai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-03-02 10:35:26.000000 udlai-0.4.0/udlai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-02 10:35:26.000000 udlai-0.4.0/udlai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 10:35:26.000000 udlai-0.4.0/udlai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-02 10:35:26.000000 udlai-0.4.0/udlai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-02 10:35:26.000000 udlai-0.4.0/udlai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    70145 2023-03-02 10:34:59.000000 udlai-0.4.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:34:34.553372 udlai-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-15 13:34:20.000000 udlai-0.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-15 13:34:20.000000 udlai-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-15 13:34:20.000000 udlai-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-15 13:34:20.000000 udlai-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-15 13:34:34.557372 udlai-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-15 13:34:20.000000 udlai-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:34:34.553372 udlai-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-15 13:34:20.000000 udlai-0.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-15 13:34:20.000000 udlai-0.5.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:34:34.553372 udlai-0.5.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:34:34.553372 udlai-0.5.0/docs/source/_static/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6148 2023-06-15 13:34:20.000000 udlai-0.5.0/docs/source/_static/favicon.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14472 2023-06-15 13:34:20.000000 udlai-0.5.0/docs/source/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-15 13:34:20.000000 udlai-0.5.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-15 13:34:20.000000 udlai-0.5.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-15 13:34:34.557372 udlai-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-15 13:34:20.000000 udlai-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:34:34.557372 udlai-0.5.0/udlai/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-15 13:34:20.000000 udlai-0.5.0/udlai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-15 13:34:34.557372 udlai-0.5.0/udlai/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-06-15 13:34:20.000000 udlai-0.5.0/udlai/feature_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-15 13:34:20.000000 udlai-0.5.0/udlai/geocoding_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:34:34.553372 udlai-0.5.0/udlai/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:34:20.000000 udlai-0.5.0/udlai/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-06-15 13:34:20.000000 udlai-0.5.0/udlai/tests/test_feature_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-15 13:34:20.000000 udlai-0.5.0/udlai/tests/test_geocoding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:34:34.553372 udlai-0.5.0/udlai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-15 13:34:34.000000 udlai-0.5.0/udlai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-15 13:34:34.000000 udlai-0.5.0/udlai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:34:34.000000 udlai-0.5.0/udlai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 13:34:34.000000 udlai-0.5.0/udlai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 13:34:34.000000 udlai-0.5.0/udlai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    70145 2023-06-15 13:34:20.000000 udlai-0.5.0/versioneer.py
```

### Comparing `udlai-0.4.0/CONTRIBUTING.md` & `udlai-0.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `udlai-0.4.0/LICENSE` & `udlai-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `udlai-0.4.0/PKG-INFO` & `udlai-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udlai
-Version: 0.4.0
+Version: 0.5.0
 Summary: UDL.AI Python interface
 Home-page: https://github.com/udl-ai/udlai
 Author: Martin Fleischmann
 Author-email: m.fleischmann@urbandatalab.net
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `udlai-0.4.0/README.md` & `udlai-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `udlai-0.4.0/docs/Makefile` & `udlai-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `udlai-0.4.0/docs/make.bat` & `udlai-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `udlai-0.4.0/docs/source/_static/favicon.png` & `udlai-0.5.0/docs/source/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `udlai-0.4.0/docs/source/_static/logo.png` & `udlai-0.5.0/docs/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `udlai-0.4.0/docs/source/conf.py` & `udlai-0.5.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `udlai-0.4.0/setup.py` & `udlai-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `udlai-0.4.0/udlai/__init__.py` & `udlai-0.5.0/udlai/__init__.py`

 * *Files identical despite different names*

### Comparing `udlai-0.4.0/udlai/feature_api.py` & `udlai-0.5.0/udlai/feature_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,15 @@
     )
     if response.status_code == 200:
         return pd.Series(_flatten_dict(response.json()))
 
     _propagate_error(response)
 
 
-def features(token, latitude, longitude, attribute_id, index_by="id"):
+def features(token, latitude, longitude, attribute_id, index_by="id", grid_size=25):
     """
     An API Endpoint that will return the attributes for provided
     coordinates. The API expects the attribute IDs, that can be fetched using
     ``udlai.attributes`` function.
 
     You can pass individual coordinates or arrays of the same length.
 
@@ -193,14 +193,18 @@
     longitude : float or list-like
         longitude or list-like of longitudes denoting the location(s) for a query
     attribute_id : int or list-like
         ID(s) of the queried attribute. Use ``udlai.attributes`` to get a list of IDs.
     index_by : {"id", "name"}
         One of the ``{"id", "name"}`` denoting whether the output should be indexed
         using the original attribute ID or its name
+    grid_size : {25, 75, 225, 675}
+        Resolution of the UDL grid to be queried. Smaller resolutions are more precise
+        but may contain gaps, larger resolutions are aggregated and are more likely to
+        cover entirety of built up area.
 
     Returns
     -------
     features : pandas.Series or pandas.DataFrame
         returns Series for a single point or a DataFrame for multiple points
 
     Examples
@@ -257,27 +261,27 @@
             },
             "attributes": [
                 {
                     "id": x,
                 }
                 for x in attribute_id
             ],
+            "grid_size": f"grid{grid_size}",
         }
 
         # calling the API
         response = requests.post(
             f"{API_URL}/features/",
             headers={
                 "Authorization": f"Bearer {token}",
                 "Content-Type": "application/json",
             },
             json=json_data,
         )
         if response.status_code == 200:
-
             dict_raw = response.json()
 
             if "error" in dict_raw:
                 raise ValueError(dict_raw["details"][0])
 
             if not dict_raw["values"]:
                 warnings.warn(
@@ -303,27 +307,27 @@
         ],
         "attributes": [
             {
                 "id": x,
             }
             for x in attribute_id
         ],
+        "grid_size": f"grid{grid_size}",
     }
 
     response = requests.post(
         f"{API_URL}/features/multi/",
         headers={
             "Authorization": f"Bearer {token}",
             "Content-Type": "application/json",
         },
         json=json_data,
     )
 
     if response.status_code == 200:
-
         d = defaultdict(list)
         missing = False
         for pt in response.json()["results"]:
             d["latitude"].append(pt["coordinates"]["latitude"])
             d["longitude"].append(pt["coordinates"]["longitude"])
             if pt["values"]:
                 for attr in pt["values"]:
```

### Comparing `udlai-0.4.0/udlai/geocoding_api.py` & `udlai-0.5.0/udlai/geocoding_api.py`

 * *Files identical despite different names*

### Comparing `udlai-0.4.0/udlai/tests/test_feature_api.py` & `udlai-0.5.0/udlai/tests/test_feature_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,14 +102,21 @@
             r = udlai.features(token, lats, lons, [113, 172], index_by="name")
         assert isinstance(r, pd.DataFrame)
         assert r.shape == (3, 4)
         for c in ["latitude", "longitude", "net_betw_speed", "freiz_300"]:
             assert c in r.columns
         assert r["net_betw_speed"].notna().sum() == 2
 
+    def test_grid_size(self):
+        r25 = udlai.features(token, 47.37, 8.54, [113, 172], index_by="name")
+        r675 = udlai.features(
+            token, 47.37, 8.54, [113, 172], index_by="name", grid_size=675
+        )
+        assert r25["net_betw_speed"] != r675["net_betw_speed"]
+
 
 class TestAggregate:
     def setup_method(self):
         self.geojson = {
             "type": "Polygon",
             "coordinates": [
                 [
```

### Comparing `udlai-0.4.0/udlai/tests/test_geocoding.py` & `udlai-0.5.0/udlai/tests/test_geocoding.py`

 * *Files identical despite different names*

### Comparing `udlai-0.4.0/udlai.egg-info/PKG-INFO` & `udlai-0.5.0/udlai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udlai
-Version: 0.4.0
+Version: 0.5.0
 Summary: UDL.AI Python interface
 Home-page: https://github.com/udl-ai/udlai
 Author: Martin Fleischmann
 Author-email: m.fleischmann@urbandatalab.net
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `udlai-0.4.0/udlai.egg-info/SOURCES.txt` & `udlai-0.5.0/udlai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `udlai-0.4.0/versioneer.py` & `udlai-0.5.0/versioneer.py`

 * *Files identical despite different names*

