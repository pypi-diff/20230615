# Comparing `tmp/houtu-0.0.1.tar.gz` & `tmp/houtu-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "houtu-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "houtu-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `houtu-0.0.1.tar` & `houtu-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1075 2023-06-14 17:31:06.528173 houtu-0.0.1/LICENSE
--rw-r--r--   0        0        0      183 2023-06-14 17:31:06.528173 houtu-0.0.1/houtu/__init__.py
--rw-r--r--   0        0        0  6170036 2023-06-14 17:31:06.536173 houtu-0.0.1/houtu/data/cities1000.txt.xz
--rw-r--r--   0        0        0    14366 2023-06-14 17:31:06.540173 houtu-0.0.1/houtu/geocoding.py
--rw-r--r--   0        0        0      402 2023-06-14 17:31:06.540173 houtu-0.0.1/houtu/utils.py
--rw-r--r--   0        0        0     1312 2023-06-14 17:31:06.540173 houtu-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3119 2023-06-14 17:31:06.540173 houtu-0.0.1/readme.md
--rw-r--r--   0        0        0     4138 1970-01-01 00:00:00.000000 houtu-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-15 13:50:34.614586 houtu-0.0.2/LICENSE
+-rw-r--r--   0        0        0      183 2023-06-15 13:50:34.614586 houtu-0.0.2/houtu/__init__.py
+-rw-r--r--   0        0        0  6170036 2023-06-15 13:50:34.622586 houtu-0.0.2/houtu/data/cities1000.txt.xz
+-rw-r--r--   0        0        0    15063 2023-06-15 13:50:34.626586 houtu-0.0.2/houtu/geocoding.py
+-rw-r--r--   0        0        0      402 2023-06-15 13:50:34.626586 houtu-0.0.2/houtu/utils.py
+-rw-r--r--   0        0        0     1312 2023-06-15 13:50:34.626586 houtu-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3264 2023-06-15 13:50:34.626586 houtu-0.0.2/readme.md
+-rw-r--r--   0        0        0     4283 1970-01-01 00:00:00.000000 houtu-0.0.2/PKG-INFO
```

### Comparing `houtu-0.0.1/LICENSE` & `houtu-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `houtu-0.0.1/houtu/data/cities1000.txt.xz` & `houtu-0.0.2/houtu/data/cities1000.txt.xz`

 * *Files identical despite different names*

### Comparing `houtu-0.0.1/houtu/geocoding.py` & `houtu-0.0.2/houtu/geocoding.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import csv
 import lzma
-from typing import List, Literal, NamedTuple, Optional, Tuple, overload
+from typing import List, Literal, NamedTuple, Optional, Set, Tuple, overload
 
 import numpy as np
 from importlib_resources import files
 from sklearn.metrics.pairwise import euclidean_distances, haversine_distances
 
 
 class City(NamedTuple):
@@ -146,30 +146,42 @@
 def toint(s: str) -> Optional[int]:
     if s:
         return int(s)
     else:
         return None
 
 
-def get_data(path: str) -> Cities:
+def get_data(path: str, keep_dups: bool = False) -> Cities:
     """Read data from tsv file. Expect the following columns:
 
     cols = ("geonameid", "name", "asciiname", "alternatenames", "latitude", "longitude", "feature class",
         "feature code", "country code", "cc2", "admin1 code", "admin2", "admin3", "admin4", "population",
         "elevation", "dem", "timezone", "modification date"
     )
+
+    When keep_dups is False (the default) cities with the exact same coordinates as a previous one are skipped.
+    This ensures more consistent results and should probably be fixed in the source data file.
     """
 
     with lzma.open(path, "rt", encoding="utf-8", newline="") as fr:
         lats = []
         lons = []
         cities = []
+
+        known: Set[Tuple[float, float]] = set()
         for row in csv.reader(fr, delimiter="\t", quoting=csv.QUOTE_NONE):
             lat = float(row[4])
             lon = float(row[5])
+
+            if not keep_dups:
+                if (lat, lon) in known:
+                    continue
+                else:
+                    known.add((lat, lon))
+
             city = City(
                 row[1],
                 row[6],
                 row[7],
                 row[8],
                 row[10],
                 row[11],
@@ -186,17 +198,20 @@
 
     arr = np.array([lats, lons], dtype=np.float32).T
     arr = np.ascontiguousarray(np.deg2rad(arr))
 
     return Cities(arr, cities)
 
 
-def _check_input(arr: np.ndarray, in_form: str, out_form: str) -> np.ndarray:
-    if arr.ndim != 2 or arr.shape[-1] != 2 or arr.dtype != np.float32:
-        raise ValueError("Expected numpy array of radians with shape (x, 2) and dtype float32")
+def _check_input(arr: np.ndarray, k: int, in_form: str, out_form: str) -> np.ndarray:
+    if arr.ndim != 2 or arr.shape[0] < 1 or arr.shape[1] != 2 or arr.dtype != np.float32:
+        raise ValueError("Expected numpy array of radians with shape (x>0, 2) and dtype float32")
+
+    if k < 1:
+        raise ValueError(f"k must >= 1, not {k}")
 
     if in_form == out_form:
         pass
     elif in_form == "radians" and out_form == "degrees":
         arr = np.rad2deg(arr)
     elif in_form == "degrees" and out_form == "radians":
         arr = np.deg2rad(arr)
@@ -209,16 +224,16 @@
         raise ValueError(f"Invalid input form: {in_form} or output form {out_form}")
 
     return arr
 
 
 def _select_cities(cities: List[City], indices: np.ndarray) -> List[List[City]]:
     out = []
-    for sample in indices:
-        out.append([cities[i] for i in sample])
+    for i in range(indices.shape[0]):
+        out.append([cities[idx] for idx in indices[i]])
     return out
 
 
 class ReverseGeocodeKdScipy:
     def __init__(self, path: Optional[str] = None) -> None:
         from scipy.spatial import KDTree
 
@@ -239,17 +254,20 @@
     @overload
     def query(
         self, query_arr: np.ndarray, k: int, form: str, return_distance: Literal[False]
     ) -> Tuple[np.ndarray, List[List[City]]]:
         ...
 
     def query(self, query_arr, k=2, form="radians", return_distance=True):
-        query_arr = _check_input(query_arr, form, "ecef")
+        query_arr = _check_input(query_arr, k, form, "ecef")
 
         distances, indices = self.tree.query(query_arr, k)
+        if k == 1:
+            distances = distances[..., None]
+            indices = indices[..., None]
         cities = _select_cities(self.cities, indices)
 
         coords = self.tree.data[indices].astype(np.float32)
         coords = WGS84.ecef2geodetic(coords)
         coords = coords[..., :2]  # ignore altitude
 
         if return_distance:
@@ -280,15 +298,15 @@
     @overload
     def query(
         self, query_arr: np.ndarray, k: int, form: str, return_distance: Literal[False]
     ) -> Tuple[np.ndarray, List[List[City]]]:
         ...
 
     def query(self, query_arr, k=2, form="radians", return_distance=True):
-        query_arr = _check_input(query_arr, form, "ecef")
+        query_arr = _check_input(query_arr, k, form, "ecef")
 
         if return_distance:
             distances, indices = self.tree.query(query_arr, k, return_distance)
         else:
             indices = self.tree.query(query_arr, k, return_distance)
 
         cities = _select_cities(self.cities, indices)
@@ -323,25 +341,25 @@
     @overload
     def query(
         self, query_arr: np.ndarray, k: int, form: str, return_distance: Literal[False]
     ) -> Tuple[np.ndarray, List[List[City]]]:
         ...
 
     def query(self, query_arr, k=2, form="radians", return_distance=True):
-        query_arr = _check_input(query_arr, form, "ecef")
+        query_arr = _check_input(query_arr, k, form, "ecef")
 
-        distances = euclidean_distances(self.arr, query_arr, squared=True)
+        distances = euclidean_distances(query_arr, self.arr, squared=True)
 
-        indices = np.argpartition(distances, k, axis=0)[:k]
-        cities = _select_cities(self.cities, indices.T)
+        indices = np.argpartition(distances, range(k), axis=-1)[:, :k]
+        cities = _select_cities(self.cities, indices)
         if return_distance:
-            distances = np.take_along_axis(distances, indices, axis=0).T
+            distances = np.take_along_axis(distances, indices, axis=-1)
             distances = np.sqrt(distances)  # distance matrix is squared
 
-        coords = self.arr[indices.T]
+        coords = self.arr[indices]
         coords = WGS84.ecef2geodetic(coords)
         coords = coords[..., :2]  # ignore altitude
 
         if return_distance:
             return coords, distances, cities
         else:
             return coords, cities
@@ -365,24 +383,24 @@
     @overload
     def query(
         self, query_arr: np.ndarray, k: int, form: str, return_distance: Literal[False]
     ) -> Tuple[np.ndarray, List[List[City]]]:
         ...
 
     def query(self, query_arr, k=2, form="radians", return_distance=True):
-        query_arr = _check_input(query_arr, form, "radians")
+        query_arr = _check_input(query_arr, k, form, "radians")
 
-        distances = haversine_distances(self.arr, query_arr)
-        indices = np.argpartition(distances, k, axis=0)[:k]
-        cities = _select_cities(self.cities, indices.T)
+        distances = haversine_distances(query_arr, self.arr)
+        indices = np.argpartition(distances, range(k), axis=-1)[:, :k]
+        cities = _select_cities(self.cities, indices)
         if return_distance:
-            distances = np.take_along_axis(distances, indices, axis=0).T
+            distances = np.take_along_axis(distances, indices, axis=-1)
             distances *= self.radius
 
-        coords = self.arr[indices.T]
+        coords = self.arr[indices]
 
         if return_distance:
             return coords, distances, cities
         else:
             return coords, cities
 
 
@@ -407,15 +425,15 @@
     @overload
     def query(
         self, query_arr: np.ndarray, k: int, form: str, return_distance: Literal[False]
     ) -> Tuple[np.ndarray, List[List[City]]]:
         ...
 
     def query(self, query_arr, k=2, form="radians", return_distance=True):
-        query_arr = _check_input(query_arr, form, "radians")
+        query_arr = _check_input(query_arr, k, form, "radians")
 
         if return_distance:
             distances, indices = self.bt.query(query_arr, k, return_distance)
         else:
             indices = self.bt.query(query_arr, k, return_distance)
         cities = _select_cities(self.cities, indices)
```

### Comparing `houtu-0.0.1/pyproject.toml` & `houtu-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `houtu-0.0.1/readme.md` & `houtu-0.0.2/readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 - Naive computation of haversine distance matrix. Coordinates are not converted.
 - Using ball-tree with haversine metric. Coordinates are not converted.
 - Naive computation of euclidic distance matrix. Coordinates are converted from geodetic to ECEF and back.
 - Using kd-tree with euclidic metric. Coordinates are converted from geodetic to ECEF and back.
 
 ## Install
 
-- requires Python 3.7+
+- requires Python 3.8+
 - run `pip install houtu`
 
 ## Use
 
 ```python
 import numpy as np
 from houtu import ReverseGeocode
@@ -47,15 +47,15 @@
 | ----- | ------ |
 |ReverseGeocodeBruteHaversine | 35.674 |
 |ReverseGeocodeBallHaversine | 0.192 |
 |ReverseGeocodeBruteEuclidic | 22.110 |
 |ReverseGeocodeKdLearn | 0.392 |
 |ReverseGeocodeKdScipy | 0.317 |
 
-### Batch of 5000
+### Batch of 100
 
 | class | time/s |
 | ----- | ------ |
 |ReverseGeocodeBruteHaversine | 193.119 |
 |ReverseGeocodeBallHaversine | 0.918 |
 |ReverseGeocodeBruteEuclidic | 86.881 |
 |ReverseGeocodeKdLearn | 0.122 |
@@ -77,7 +77,11 @@
 ## Development
 
 - run tests `python -m unittest discover -s tests`
 
 ## Sources
 
 Cities database file `houtu/data/cities1000.txt.xz` is downloaded and recompressed from <http://download.geonames.org/export/dump/cities1000.zip> (Creative Commons Attribution 4.0 License).
+
+### GeoNames issues
+
+There are about 50 pairs of cities which have the exact same coordinates, for example `Fajã de Baixo` and `Rosto de Cão`.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `houtu-0.0.1/PKG-INFO` & `houtu-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: houtu
-Version: 0.0.1
+Version: 0.0.2
 Summary: Offline fast reverse geocoding. Named after the Chinese Goddess of the Earth Houtu. 
 Author-email: Dobatymo <dobatymo@users.noreply.github.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -32,15 +32,15 @@
 - Naive computation of haversine distance matrix. Coordinates are not converted.
 - Using ball-tree with haversine metric. Coordinates are not converted.
 - Naive computation of euclidic distance matrix. Coordinates are converted from geodetic to ECEF and back.
 - Using kd-tree with euclidic metric. Coordinates are converted from geodetic to ECEF and back.
 
 ## Install
 
-- requires Python 3.7+
+- requires Python 3.8+
 - run `pip install houtu`
 
 ## Use
 
 ```python
 import numpy as np
 from houtu import ReverseGeocode
@@ -73,15 +73,15 @@
 | ----- | ------ |
 |ReverseGeocodeBruteHaversine | 35.674 |
 |ReverseGeocodeBallHaversine | 0.192 |
 |ReverseGeocodeBruteEuclidic | 22.110 |
 |ReverseGeocodeKdLearn | 0.392 |
 |ReverseGeocodeKdScipy | 0.317 |
 
-### Batch of 5000
+### Batch of 100
 
 | class | time/s |
 | ----- | ------ |
 |ReverseGeocodeBruteHaversine | 193.119 |
 |ReverseGeocodeBallHaversine | 0.918 |
 |ReverseGeocodeBruteEuclidic | 86.881 |
 |ReverseGeocodeKdLearn | 0.122 |
@@ -104,7 +104,11 @@
 
 - run tests `python -m unittest discover -s tests`
 
 ## Sources
 
 Cities database file `houtu/data/cities1000.txt.xz` is downloaded and recompressed from <http://download.geonames.org/export/dump/cities1000.zip> (Creative Commons Attribution 4.0 License).
 
+### GeoNames issues
+
+There are about 50 pairs of cities which have the exact same coordinates, for example `Fajã de Baixo` and `Rosto de Cão`.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

