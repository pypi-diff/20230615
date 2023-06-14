# Comparing `tmp/topometry-0.2.0.1.tar.gz` & `tmp/topometry-0.2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topometry-0.2.0.1.tar", last modified: Wed Jun 14 22:46:04 2023, max compression
+gzip compressed data, was "topometry-0.2.0.2.tar", last modified: Wed Jun 14 23:46:03 2023, max compression
```

## Comparing `topometry-0.2.0.1.tar` & `topometry-0.2.0.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:46:04.820172 topometry-0.2.0.1/
--rwxrwxr-x   0 root         (0) root         (0)     1101 2023-06-14 21:18:44.000000 topometry-0.2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4870 2023-06-14 22:46:04.820172 topometry-0.2.0.1/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)     4250 2023-06-14 21:18:44.000000 topometry-0.2.0.1/README.md
--rwxrwxr-x   0 root         (0) root         (0)      104 2023-06-14 21:18:44.000000 topometry-0.2.0.1/pyproject.toml
--rwxrwxr-x   0 root         (0) root         (0)      736 2023-06-14 22:46:04.820172 topometry-0.2.0.1/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)       91 2023-06-14 21:18:44.000000 topometry-0.2.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:46:04.816172 topometry-0.2.0.1/topo/
--rwxrwxr-x   0 root         (0) root         (0)      897 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:46:04.816172 topometry-0.2.0.1/topo/base/
--rwxrwxr-x   0 root         (0) root         (0)      179 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/base/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    47503 2023-06-14 21:26:44.000000 topometry-0.2.0.1/topo/base/ann.py
--rwxrwxr-x   0 root         (0) root         (0)    45676 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/base/dists.py
--rwxrwxr-x   0 root         (0) root         (0)    16721 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/base/sparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:46:04.816172 topometry-0.2.0.1/topo/eval/
--rwxrwxr-x   0 root         (0) root         (0)      219 2023-06-14 21:27:15.000000 topometry-0.2.0.1/topo/eval/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     2218 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/eval/global_scores.py
--rwxrwxr-x   0 root         (0) root         (0)    12754 2023-06-14 21:27:15.000000 topometry-0.2.0.1/topo/eval/local_scores.py
--rwxrwxr-x   0 root         (0) root         (0)     6058 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/eval/rmetric.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:46:04.816172 topometry-0.2.0.1/topo/layouts/
--rwxrwxr-x   0 root         (0) root         (0)      120 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/layouts/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    13879 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/layouts/graph_utils.py
--rwxrwxr-x   0 root         (0) root         (0)     3366 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/layouts/isomap.py
--rwxrwxr-x   0 root         (0) root         (0)     9251 2023-06-14 21:31:28.000000 topometry-0.2.0.1/topo/layouts/map.py
--rwxrwxr-x   0 root         (0) root         (0)    36184 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/layouts/projector.py
--rwxrwxr-x   0 root         (0) root         (0)    19227 2023-06-14 21:25:57.000000 topometry-0.2.0.1/topo/pipes.py
--rwxrwxr-x   0 root         (0) root         (0)    22966 2023-06-14 22:04:50.000000 topometry-0.2.0.1/topo/plot.py
--rwxrwxr-x   0 root         (0) root         (0)    21289 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/single_cell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:46:04.816172 topometry-0.2.0.1/topo/spectral/
--rwxrwxr-x   0 root         (0) root         (0)      265 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/spectral/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    23612 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/spectral/_spectral.py
--rwxrwxr-x   0 root         (0) root         (0)    26918 2023-06-14 21:28:18.000000 topometry-0.2.0.1/topo/spectral/eigen.py
--rw-rw-r--   0 root         (0) root         (0)      855 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/spectral/locally.py
--rwxrwxr-x   0 root         (0) root         (0)    30671 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/spectral/umap_layouts.py
--rwxrwxr-x   0 root         (0) root         (0)    76100 2023-06-14 21:22:09.000000 topometry-0.2.0.1/topo/topograph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:46:04.820172 topometry-0.2.0.1/topo/tpgraph/
--rwxrwxr-x   0 root         (0) root         (0)      225 2023-06-14 21:28:40.000000 topometry-0.2.0.1/topo/tpgraph/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     5089 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/tpgraph/cknn.py
--rwxrwxr-x   0 root         (0) root         (0)    15089 2023-06-14 21:29:14.000000 topometry-0.2.0.1/topo/tpgraph/fuzzy.py
--rw-rw-r--   0 root         (0) root         (0)    14221 2023-06-14 21:29:14.000000 topometry-0.2.0.1/topo/tpgraph/intrinsic_dim.py
--rwxrwxr-x   0 root         (0) root         (0)    48044 2023-06-14 21:21:07.000000 topometry-0.2.0.1/topo/tpgraph/kernels.py
--rwxrwxr-x   0 root         (0) root         (0)    32597 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/tpgraph/procrustes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:46:04.820172 topometry-0.2.0.1/topo/utils/
--rwxrwxr-x   0 root         (0) root         (0)       22 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/utils/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     5710 2023-06-14 21:31:28.000000 topometry-0.2.0.1/topo/utils/_utils.py
--rwxrwxr-x   0 root         (0) root         (0)     8583 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/utils/umap_utils.py
--rwxrwxr-x   0 root         (0) root         (0)       24 2023-06-14 22:45:36.000000 topometry-0.2.0.1/topo/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:46:04.820172 topometry-0.2.0.1/topometry.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4870 2023-06-14 22:46:04.000000 topometry-0.2.0.1/topometry.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2023-06-14 22:46:04.000000 topometry-0.2.0.1/topometry.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 22:46:04.000000 topometry-0.2.0.1/topometry.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-14 22:46:04.000000 topometry-0.2.0.1/topometry.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-14 22:46:04.000000 topometry-0.2.0.1/topometry.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 23:46:03.360502 topometry-0.2.0.2/
+-rwxrwxr-x   0 root         (0) root         (0)     1101 2023-06-14 21:18:44.000000 topometry-0.2.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4870 2023-06-14 23:46:03.360502 topometry-0.2.0.2/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)     4250 2023-06-14 21:18:44.000000 topometry-0.2.0.2/README.md
+-rwxrwxr-x   0 root         (0) root         (0)      104 2023-06-14 21:18:44.000000 topometry-0.2.0.2/pyproject.toml
+-rwxrwxr-x   0 root         (0) root         (0)      736 2023-06-14 23:46:03.360502 topometry-0.2.0.2/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)       91 2023-06-14 21:18:44.000000 topometry-0.2.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 23:46:03.356502 topometry-0.2.0.2/topo/
+-rwxrwxr-x   0 root         (0) root         (0)      897 2023-06-14 21:18:44.000000 topometry-0.2.0.2/topo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 23:46:03.356502 topometry-0.2.0.2/topo/base/
+-rwxrwxr-x   0 root         (0) root         (0)      179 2023-06-14 21:18:44.000000 topometry-0.2.0.2/topo/base/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    47503 2023-06-14 23:37:47.000000 topometry-0.2.0.2/topo/base/ann.py
+-rwxrwxr-x   0 root         (0) root         (0)    45718 2023-06-14 22:51:02.000000 topometry-0.2.0.2/topo/base/dists.py
+-rwxrwxr-x   0 root         (0) root         (0)    16721 2023-06-14 21:18:44.000000 topometry-0.2.0.2/topo/base/sparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 23:46:03.356502 topometry-0.2.0.2/topo/eval/
+-rwxrwxr-x   0 root         (0) root         (0)      219 2023-06-14 21:27:15.000000 topometry-0.2.0.2/topo/eval/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     2218 2023-06-14 21:18:44.000000 topometry-0.2.0.2/topo/eval/global_scores.py
+-rwxrwxr-x   0 root         (0) root         (0)    12754 2023-06-14 21:27:15.000000 topometry-0.2.0.2/topo/eval/local_scores.py
+-rwxrwxr-x   0 root         (0) root         (0)     6058 2023-06-14 21:18:44.000000 topometry-0.2.0.2/topo/eval/rmetric.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 23:46:03.356502 topometry-0.2.0.2/topo/layouts/
+-rwxrwxr-x   0 root         (0) root         (0)      120 2023-06-14 21:18:44.000000 topometry-0.2.0.2/topo/layouts/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    13879 2023-06-14 21:18:44.000000 topometry-0.2.0.2/topo/layouts/graph_utils.py
+-rwxrwxr-x   0 root         (0) root         (0)     3366 2023-06-14 21:18:44.000000 topometry-0.2.0.2/topo/layouts/isomap.py
+-rwxrwxr-x   0 root         (0) root         (0)     9251 2023-06-14 21:31:28.000000 topometry-0.2.0.2/topo/layouts/map.py
+-rwxrwxr-x   0 root         (0) root         (0)    36184 2023-06-14 21:18:44.000000 topometry-0.2.0.2/topo/layouts/projector.py
+-rwxrwxr-x   0 root         (0) root         (0)    19227 2023-06-14 21:25:57.000000 topometry-0.2.0.2/topo/pipes.py
+-rwxrwxr-x   0 root         (0) root         (0)    22966 2023-06-14 22:04:50.000000 topometry-0.2.0.2/topo/plot.py
+-rwxrwxr-x   0 root         (0) root         (0)    21289 2023-06-14 21:18:44.000000 topometry-0.2.0.2/topo/single_cell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 23:46:03.356502 topometry-0.2.0.2/topo/spectral/
+-rwxrwxr-x   0 root         (0) root         (0)      265 2023-06-14 21:18:44.000000 topometry-0.2.0.2/topo/spectral/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    23612 2023-06-14 21:18:44.000000 topometry-0.2.0.2/topo/spectral/_spectral.py
+-rwxrwxr-x   0 root         (0) root         (0)    26918 2023-06-14 21:28:18.000000 topometry-0.2.0.2/topo/spectral/eigen.py
+-rw-rw-r--   0 root         (0) root         (0)      855 2023-06-14 21:18:44.000000 topometry-0.2.0.2/topo/spectral/locally.py
+-rwxrwxr-x   0 root         (0) root         (0)    30671 2023-06-14 23:34:47.000000 topometry-0.2.0.2/topo/spectral/umap_layouts.py
+-rwxrwxr-x   0 root         (0) root         (0)    76111 2023-06-14 23:36:41.000000 topometry-0.2.0.2/topo/topograph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 23:46:03.360502 topometry-0.2.0.2/topo/tpgraph/
+-rwxrwxr-x   0 root         (0) root         (0)      225 2023-06-14 21:28:40.000000 topometry-0.2.0.2/topo/tpgraph/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     5110 2023-06-14 23:33:52.000000 topometry-0.2.0.2/topo/tpgraph/cknn.py
+-rwxrwxr-x   0 root         (0) root         (0)    15089 2023-06-14 23:36:03.000000 topometry-0.2.0.2/topo/tpgraph/fuzzy.py
+-rw-rw-r--   0 root         (0) root         (0)    14221 2023-06-14 21:29:14.000000 topometry-0.2.0.2/topo/tpgraph/intrinsic_dim.py
+-rwxrwxr-x   0 root         (0) root         (0)    48044 2023-06-14 21:21:07.000000 topometry-0.2.0.2/topo/tpgraph/kernels.py
+-rwxrwxr-x   0 root         (0) root         (0)    32597 2023-06-14 21:18:44.000000 topometry-0.2.0.2/topo/tpgraph/procrustes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 23:46:03.360502 topometry-0.2.0.2/topo/utils/
+-rwxrwxr-x   0 root         (0) root         (0)       22 2023-06-14 21:18:44.000000 topometry-0.2.0.2/topo/utils/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     5710 2023-06-14 21:31:28.000000 topometry-0.2.0.2/topo/utils/_utils.py
+-rwxrwxr-x   0 root         (0) root         (0)     8583 2023-06-14 21:18:44.000000 topometry-0.2.0.2/topo/utils/umap_utils.py
+-rwxrwxr-x   0 root         (0) root         (0)       24 2023-06-14 22:56:32.000000 topometry-0.2.0.2/topo/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 23:46:03.360502 topometry-0.2.0.2/topometry.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4870 2023-06-14 23:46:03.000000 topometry-0.2.0.2/topometry.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      958 2023-06-14 23:46:03.000000 topometry-0.2.0.2/topometry.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 23:46:03.000000 topometry-0.2.0.2/topometry.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-14 23:46:03.000000 topometry-0.2.0.2/topometry.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-14 23:46:03.000000 topometry-0.2.0.2/topometry.egg-info/top_level.txt
```

### Comparing `topometry-0.2.0.1/LICENSE` & `topometry-0.2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/PKG-INFO` & `topometry-0.2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topometry
-Version: 0.2.0.1
+Version: 0.2.0.2
 Summary: A comprehensive dimensional reduction framework to recover latent information from data.
 Home-page: https://github.com/davisidarta/topometry
 Author: Davi Sidarta-Oliveira
 Author-email: davi.oliveira@dpag.ox.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/davisidarta/topometry/issues
 Platform: UNKNOWN
```

### Comparing `topometry-0.2.0.1/README.md` & `topometry-0.2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/setup.cfg` & `topometry-0.2.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = topometry
-version = 0.2.0.1
+version = 0.2.0.2
 author = Davi Sidarta-Oliveira
 author_email = davi.oliveira@dpag.ox.ac.uk
 description = A comprehensive dimensional reduction framework to recover latent information from data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/davisidarta/topometry
 project_urls =
```

### Comparing `topometry-0.2.0.1/topo/__init__.py` & `topometry-0.2.0.2/topo/__init__.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/base/ann.py` & `topometry-0.2.0.2/topo/base/ann.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/base/dists.py` & `topometry-0.2.0.2/topo/base/dists.py`

 * *Files 0% similar despite different names*

```diff
@@ -1049,35 +1049,35 @@
             normalisation = max_dist / 2.0  # heuristic
             # heuristic
             return {"normalisation": normalisation, "max_dist": max_dist / 2.0}
 
         else:
             return {}
 
-    @numba.jit()
+    @numba.jit(nopython=False)
     def categorical_distance(x, y):
         if x == y:
             return 0.0
         else:
             return 1.0
 
-    @numba.jit()
+    @numba.jit(nopython=False)
     def hierarchical_categorical_distance(x, y, cat_hierarchy=[{}]):
         n_levels = float(len(cat_hierarchy))
         for level, cats in enumerate(cat_hierarchy):
             if cats[x] == cats[y]:
                 return float(level) / n_levels
         else:
             return 1.0
 
     @numba.njit()
     def ordinal_distance(x, y, support_size=1.0):
         return abs(x - y) / support_size
 
-    @numba.jit()
+    @numba.jit(nopython=False)
     def count_distance(x, y, poisson_lambda=1.0, normalisation=1.0):
         lo = int(min(x, y))
         hi = int(max(x, y))
 
         log_lambda = np.log(poisson_lambda)
 
         if lo < 2:
```

### Comparing `topometry-0.2.0.1/topo/base/sparse.py` & `topometry-0.2.0.2/topo/base/sparse.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/eval/global_scores.py` & `topometry-0.2.0.2/topo/eval/global_scores.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/eval/local_scores.py` & `topometry-0.2.0.2/topo/eval/local_scores.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/eval/rmetric.py` & `topometry-0.2.0.2/topo/eval/rmetric.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/layouts/graph_utils.py` & `topometry-0.2.0.2/topo/layouts/graph_utils.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/layouts/isomap.py` & `topometry-0.2.0.2/topo/layouts/isomap.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/layouts/map.py` & `topometry-0.2.0.2/topo/layouts/map.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/layouts/projector.py` & `topometry-0.2.0.2/topo/layouts/projector.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/pipes.py` & `topometry-0.2.0.2/topo/pipes.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/plot.py` & `topometry-0.2.0.2/topo/plot.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/single_cell.py` & `topometry-0.2.0.2/topo/single_cell.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/spectral/_spectral.py` & `topometry-0.2.0.2/topo/spectral/_spectral.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/spectral/eigen.py` & `topometry-0.2.0.2/topo/spectral/eigen.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/spectral/locally.py` & `topometry-0.2.0.2/topo/spectral/locally.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/spectral/umap_layouts.py` & `topometry-0.2.0.2/topo/spectral/umap_layouts.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/topograph.py` & `topometry-0.2.0.2/topo/topograph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1048,15 +1048,15 @@
     #     self.EigenbasisDict = {}
     #     self.GraphKernelDict = {}
     #     self.ProjectionDict = {}
 
 
 
 
-    def _compute_kernel_from_version_knn(self, knn, n_neighbors, kernel_version, results_dict, prefix='', suffix='', low_memory=False, data_for_expansion=None):
+    def _compute_kernel_from_version_knn(self, knn, n_neighbors, kernel_version, results_dict, prefix='', suffix='', low_memory=False, base=True, data_for_expansion=None):
         import gc
         gc.collect()
         kernel_key = kernel_version
         if prefix is not None:
             kernel_key = prefix + kernel_key
         if suffix is not None:
             kernel_key = kernel_key + suffix
```

### Comparing `topometry-0.2.0.1/topo/tpgraph/cknn.py` & `topometry-0.2.0.2/topo/tpgraph/cknn.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         knn = kNN(X, n_neighbors=n_neighbors,
                   metric=metric,
                   n_jobs=n_jobs,
                   backend=backend,
                   verbose=verbose,
                   **kwargs)
 
-    median_k = np.floor(n_neighbors / 2).astype(int)
+    median_k = np.floor(n_neighbors / 2).astype(np.int32)
     adap_sd = np.zeros(N)
     for i in np.arange(len(adap_sd)):
         adap_sd[i] = np.sort(knn.data[knn.indptr[i]: knn.indptr[i + 1]])[
             median_k - 1
         ]
 
     x, y, dists = find(knn)
@@ -105,23 +105,23 @@
     dd = np.arange(N)
     if include_self:
         A[dd, dd] = True
     else:
         A[dd, dd] = False
     if weighted is None:
         if return_densities:
-            return A.astype(np.int), A.astype(np.float), adap_sd
+            return A.astype(np.int32), A.astype(np.float32), adap_sd
         else:
-            return A.astype(np.int), A.astype(np.float)
+            return A.astype(np.int32), A.astype(np.float32)
     else:
         if weighted:
             if return_densities:
-                return A.astype(np.float), adap_sd
+                return A.astype(np.float32), adap_sd
             else:
-                return A.astype(np.float)
+                return A.astype(np.float32)
         else:
             if return_densities:
-                return A.astype(np.int), adap_sd
+                return A.astype(np.int32), adap_sd
             else:
-                return A.astype(np.int)
+                return A.astype(np.int32)
```

### Comparing `topometry-0.2.0.1/topo/tpgraph/fuzzy.py` & `topometry-0.2.0.2/topo/tpgraph/fuzzy.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/tpgraph/intrinsic_dim.py` & `topometry-0.2.0.2/topo/tpgraph/intrinsic_dim.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/tpgraph/kernels.py` & `topometry-0.2.0.2/topo/tpgraph/kernels.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/tpgraph/procrustes.py` & `topometry-0.2.0.2/topo/tpgraph/procrustes.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/utils/_utils.py` & `topometry-0.2.0.2/topo/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topo/utils/umap_utils.py` & `topometry-0.2.0.2/topo/utils/umap_utils.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.1/topometry.egg-info/PKG-INFO` & `topometry-0.2.0.2/topometry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topometry
-Version: 0.2.0.1
+Version: 0.2.0.2
 Summary: A comprehensive dimensional reduction framework to recover latent information from data.
 Home-page: https://github.com/davisidarta/topometry
 Author: Davi Sidarta-Oliveira
 Author-email: davi.oliveira@dpag.ox.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/davisidarta/topometry/issues
 Platform: UNKNOWN
```

### Comparing `topometry-0.2.0.1/topometry.egg-info/SOURCES.txt` & `topometry-0.2.0.2/topometry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

