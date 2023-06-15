# Comparing `tmp/topometry-0.2.0.3.tar.gz` & `tmp/topometry-0.2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topometry-0.2.0.3.tar", last modified: Thu Jun 15 12:57:40 2023, max compression
+gzip compressed data, was "topometry-0.2.0.4.tar", last modified: Thu Jun 15 17:59:22 2023, max compression
```

## Comparing `topometry-0.2.0.3.tar` & `topometry-0.2.0.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:57:40.948845 topometry-0.2.0.3/
--rwxrwxr-x   0 root         (0) root         (0)     1101 2023-06-14 21:18:44.000000 topometry-0.2.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4870 2023-06-15 12:57:40.948845 topometry-0.2.0.3/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)     4250 2023-06-14 21:18:44.000000 topometry-0.2.0.3/README.md
--rwxrwxr-x   0 root         (0) root         (0)      104 2023-06-14 21:18:44.000000 topometry-0.2.0.3/pyproject.toml
--rwxrwxr-x   0 root         (0) root         (0)      736 2023-06-15 12:57:40.948845 topometry-0.2.0.3/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)       91 2023-06-14 21:18:44.000000 topometry-0.2.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:57:40.944845 topometry-0.2.0.3/topo/
--rwxrwxr-x   0 root         (0) root         (0)      897 2023-06-14 21:18:44.000000 topometry-0.2.0.3/topo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:57:40.944845 topometry-0.2.0.3/topo/base/
--rwxrwxr-x   0 root         (0) root         (0)      179 2023-06-14 21:18:44.000000 topometry-0.2.0.3/topo/base/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    47503 2023-06-14 23:37:47.000000 topometry-0.2.0.3/topo/base/ann.py
--rwxrwxr-x   0 root         (0) root         (0)    45718 2023-06-14 22:51:02.000000 topometry-0.2.0.3/topo/base/dists.py
--rwxrwxr-x   0 root         (0) root         (0)    16721 2023-06-14 21:18:44.000000 topometry-0.2.0.3/topo/base/sparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:57:40.944845 topometry-0.2.0.3/topo/eval/
--rwxrwxr-x   0 root         (0) root         (0)      219 2023-06-14 21:27:15.000000 topometry-0.2.0.3/topo/eval/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     2218 2023-06-14 21:18:44.000000 topometry-0.2.0.3/topo/eval/global_scores.py
--rwxrwxr-x   0 root         (0) root         (0)    12721 2023-06-15 11:44:37.000000 topometry-0.2.0.3/topo/eval/local_scores.py
--rwxrwxr-x   0 root         (0) root         (0)     6058 2023-06-14 21:18:44.000000 topometry-0.2.0.3/topo/eval/rmetric.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:57:40.944845 topometry-0.2.0.3/topo/layouts/
--rwxrwxr-x   0 root         (0) root         (0)      120 2023-06-14 21:18:44.000000 topometry-0.2.0.3/topo/layouts/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    13879 2023-06-14 21:18:44.000000 topometry-0.2.0.3/topo/layouts/graph_utils.py
--rwxrwxr-x   0 root         (0) root         (0)     3366 2023-06-14 21:18:44.000000 topometry-0.2.0.3/topo/layouts/isomap.py
--rwxrwxr-x   0 root         (0) root         (0)     9251 2023-06-14 21:31:28.000000 topometry-0.2.0.3/topo/layouts/map.py
--rwxrwxr-x   0 root         (0) root         (0)    36184 2023-06-14 21:18:44.000000 topometry-0.2.0.3/topo/layouts/projector.py
--rwxrwxr-x   0 root         (0) root         (0)    19227 2023-06-14 21:25:57.000000 topometry-0.2.0.3/topo/pipes.py
--rwxrwxr-x   0 root         (0) root         (0)    22966 2023-06-14 22:04:50.000000 topometry-0.2.0.3/topo/plot.py
--rwxrwxr-x   0 root         (0) root         (0)    21289 2023-06-14 21:18:44.000000 topometry-0.2.0.3/topo/single_cell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:57:40.944845 topometry-0.2.0.3/topo/spectral/
--rwxrwxr-x   0 root         (0) root         (0)      265 2023-06-14 21:18:44.000000 topometry-0.2.0.3/topo/spectral/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    23612 2023-06-14 21:18:44.000000 topometry-0.2.0.3/topo/spectral/_spectral.py
--rwxrwxr-x   0 root         (0) root         (0)    26918 2023-06-14 21:28:18.000000 topometry-0.2.0.3/topo/spectral/eigen.py
--rw-rw-r--   0 root         (0) root         (0)      855 2023-06-14 21:18:44.000000 topometry-0.2.0.3/topo/spectral/locally.py
--rwxrwxr-x   0 root         (0) root         (0)    30671 2023-06-14 23:34:47.000000 topometry-0.2.0.3/topo/spectral/umap_layouts.py
--rwxrwxr-x   0 root         (0) root         (0)    76111 2023-06-14 23:36:41.000000 topometry-0.2.0.3/topo/topograph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:57:40.944845 topometry-0.2.0.3/topo/tpgraph/
--rwxrwxr-x   0 root         (0) root         (0)      225 2023-06-14 21:28:40.000000 topometry-0.2.0.3/topo/tpgraph/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     5110 2023-06-14 23:33:52.000000 topometry-0.2.0.3/topo/tpgraph/cknn.py
--rwxrwxr-x   0 root         (0) root         (0)    15089 2023-06-14 23:36:03.000000 topometry-0.2.0.3/topo/tpgraph/fuzzy.py
--rw-rw-r--   0 root         (0) root         (0)    14221 2023-06-14 21:29:14.000000 topometry-0.2.0.3/topo/tpgraph/intrinsic_dim.py
--rwxrwxr-x   0 root         (0) root         (0)    48044 2023-06-14 21:21:07.000000 topometry-0.2.0.3/topo/tpgraph/kernels.py
--rwxrwxr-x   0 root         (0) root         (0)    32597 2023-06-14 21:18:44.000000 topometry-0.2.0.3/topo/tpgraph/procrustes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:57:40.948845 topometry-0.2.0.3/topo/utils/
--rwxrwxr-x   0 root         (0) root         (0)       22 2023-06-14 21:18:44.000000 topometry-0.2.0.3/topo/utils/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     5710 2023-06-14 21:31:28.000000 topometry-0.2.0.3/topo/utils/_utils.py
--rwxrwxr-x   0 root         (0) root         (0)     8583 2023-06-14 21:18:44.000000 topometry-0.2.0.3/topo/utils/umap_utils.py
--rwxrwxr-x   0 root         (0) root         (0)       24 2023-06-15 11:47:12.000000 topometry-0.2.0.3/topo/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:57:40.948845 topometry-0.2.0.3/topometry.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4870 2023-06-15 12:57:40.000000 topometry-0.2.0.3/topometry.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2023-06-15 12:57:40.000000 topometry-0.2.0.3/topometry.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 12:57:40.000000 topometry-0.2.0.3/topometry.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-15 12:57:40.000000 topometry-0.2.0.3/topometry.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-15 12:57:40.000000 topometry-0.2.0.3/topometry.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:59:22.111663 topometry-0.2.0.4/
+-rwxrwxr-x   0 root         (0) root         (0)     1101 2023-06-14 21:18:44.000000 topometry-0.2.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4870 2023-06-15 17:59:22.111663 topometry-0.2.0.4/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)     4250 2023-06-14 21:18:44.000000 topometry-0.2.0.4/README.md
+-rwxrwxr-x   0 root         (0) root         (0)      104 2023-06-14 21:18:44.000000 topometry-0.2.0.4/pyproject.toml
+-rwxrwxr-x   0 root         (0) root         (0)      736 2023-06-15 17:59:22.111663 topometry-0.2.0.4/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)       91 2023-06-14 21:18:44.000000 topometry-0.2.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:59:22.107663 topometry-0.2.0.4/topo/
+-rwxrwxr-x   0 root         (0) root         (0)      897 2023-06-14 21:18:44.000000 topometry-0.2.0.4/topo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:59:22.107663 topometry-0.2.0.4/topo/base/
+-rwxrwxr-x   0 root         (0) root         (0)      179 2023-06-14 21:18:44.000000 topometry-0.2.0.4/topo/base/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    47503 2023-06-14 23:37:47.000000 topometry-0.2.0.4/topo/base/ann.py
+-rwxrwxr-x   0 root         (0) root         (0)    45718 2023-06-14 22:51:02.000000 topometry-0.2.0.4/topo/base/dists.py
+-rwxrwxr-x   0 root         (0) root         (0)    16721 2023-06-14 21:18:44.000000 topometry-0.2.0.4/topo/base/sparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:59:22.107663 topometry-0.2.0.4/topo/eval/
+-rwxrwxr-x   0 root         (0) root         (0)      219 2023-06-14 21:27:15.000000 topometry-0.2.0.4/topo/eval/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     2218 2023-06-14 21:18:44.000000 topometry-0.2.0.4/topo/eval/global_scores.py
+-rwxrwxr-x   0 root         (0) root         (0)    12721 2023-06-15 11:44:37.000000 topometry-0.2.0.4/topo/eval/local_scores.py
+-rwxrwxr-x   0 root         (0) root         (0)     6058 2023-06-14 21:18:44.000000 topometry-0.2.0.4/topo/eval/rmetric.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:59:22.107663 topometry-0.2.0.4/topo/layouts/
+-rwxrwxr-x   0 root         (0) root         (0)      120 2023-06-14 21:18:44.000000 topometry-0.2.0.4/topo/layouts/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    13879 2023-06-14 21:18:44.000000 topometry-0.2.0.4/topo/layouts/graph_utils.py
+-rwxrwxr-x   0 root         (0) root         (0)     3366 2023-06-14 21:18:44.000000 topometry-0.2.0.4/topo/layouts/isomap.py
+-rwxrwxr-x   0 root         (0) root         (0)     9251 2023-06-14 21:31:28.000000 topometry-0.2.0.4/topo/layouts/map.py
+-rwxrwxr-x   0 root         (0) root         (0)    36184 2023-06-14 21:18:44.000000 topometry-0.2.0.4/topo/layouts/projector.py
+-rwxrwxr-x   0 root         (0) root         (0)    19221 2023-06-15 17:58:12.000000 topometry-0.2.0.4/topo/pipes.py
+-rwxrwxr-x   0 root         (0) root         (0)    22966 2023-06-14 22:04:50.000000 topometry-0.2.0.4/topo/plot.py
+-rwxrwxr-x   0 root         (0) root         (0)    21289 2023-06-14 21:18:44.000000 topometry-0.2.0.4/topo/single_cell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:59:22.107663 topometry-0.2.0.4/topo/spectral/
+-rwxrwxr-x   0 root         (0) root         (0)      265 2023-06-14 21:18:44.000000 topometry-0.2.0.4/topo/spectral/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    23612 2023-06-14 21:18:44.000000 topometry-0.2.0.4/topo/spectral/_spectral.py
+-rwxrwxr-x   0 root         (0) root         (0)    26918 2023-06-14 21:28:18.000000 topometry-0.2.0.4/topo/spectral/eigen.py
+-rw-rw-r--   0 root         (0) root         (0)      855 2023-06-14 21:18:44.000000 topometry-0.2.0.4/topo/spectral/locally.py
+-rwxrwxr-x   0 root         (0) root         (0)    30671 2023-06-14 23:34:47.000000 topometry-0.2.0.4/topo/spectral/umap_layouts.py
+-rwxrwxr-x   0 root         (0) root         (0)    76111 2023-06-14 23:36:41.000000 topometry-0.2.0.4/topo/topograph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:59:22.107663 topometry-0.2.0.4/topo/tpgraph/
+-rwxrwxr-x   0 root         (0) root         (0)      225 2023-06-14 21:28:40.000000 topometry-0.2.0.4/topo/tpgraph/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     5110 2023-06-14 23:33:52.000000 topometry-0.2.0.4/topo/tpgraph/cknn.py
+-rwxrwxr-x   0 root         (0) root         (0)    15089 2023-06-14 23:36:03.000000 topometry-0.2.0.4/topo/tpgraph/fuzzy.py
+-rw-rw-r--   0 root         (0) root         (0)    14221 2023-06-14 21:29:14.000000 topometry-0.2.0.4/topo/tpgraph/intrinsic_dim.py
+-rwxrwxr-x   0 root         (0) root         (0)    48044 2023-06-14 21:21:07.000000 topometry-0.2.0.4/topo/tpgraph/kernels.py
+-rwxrwxr-x   0 root         (0) root         (0)    32597 2023-06-14 21:18:44.000000 topometry-0.2.0.4/topo/tpgraph/procrustes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:59:22.111663 topometry-0.2.0.4/topo/utils/
+-rwxrwxr-x   0 root         (0) root         (0)       22 2023-06-14 21:18:44.000000 topometry-0.2.0.4/topo/utils/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     5710 2023-06-14 21:31:28.000000 topometry-0.2.0.4/topo/utils/_utils.py
+-rwxrwxr-x   0 root         (0) root         (0)     8583 2023-06-14 21:18:44.000000 topometry-0.2.0.4/topo/utils/umap_utils.py
+-rwxrwxr-x   0 root         (0) root         (0)       24 2023-06-15 17:58:32.000000 topometry-0.2.0.4/topo/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 17:59:22.111663 topometry-0.2.0.4/topometry.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4870 2023-06-15 17:59:22.000000 topometry-0.2.0.4/topometry.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      958 2023-06-15 17:59:22.000000 topometry-0.2.0.4/topometry.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 17:59:22.000000 topometry-0.2.0.4/topometry.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-15 17:59:22.000000 topometry-0.2.0.4/topometry.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-15 17:59:22.000000 topometry-0.2.0.4/topometry.egg-info/top_level.txt
```

### Comparing `topometry-0.2.0.3/LICENSE` & `topometry-0.2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/PKG-INFO` & `topometry-0.2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topometry
-Version: 0.2.0.3
+Version: 0.2.0.4
 Summary: A comprehensive dimensional reduction framework to recover latent information from data.
 Home-page: https://github.com/davisidarta/topometry
 Author: Davi Sidarta-Oliveira
 Author-email: davi.oliveira@dpag.ox.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/davisidarta/topometry/issues
 Platform: UNKNOWN
```

### Comparing `topometry-0.2.0.3/README.md` & `topometry-0.2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/setup.cfg` & `topometry-0.2.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = topometry
-version = 0.2.0.3
+version = 0.2.0.4
 author = Davi Sidarta-Oliveira
 author_email = davi.oliveira@dpag.ox.ac.uk
 description = A comprehensive dimensional reduction framework to recover latent information from data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/davisidarta/topometry
 project_urls =
```

### Comparing `topometry-0.2.0.3/topo/__init__.py` & `topometry-0.2.0.4/topo/__init__.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/base/ann.py` & `topometry-0.2.0.4/topo/base/ann.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/base/dists.py` & `topometry-0.2.0.4/topo/base/dists.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/base/sparse.py` & `topometry-0.2.0.4/topo/base/sparse.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/eval/global_scores.py` & `topometry-0.2.0.4/topo/eval/global_scores.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/eval/local_scores.py` & `topometry-0.2.0.4/topo/eval/local_scores.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/eval/rmetric.py` & `topometry-0.2.0.4/topo/eval/rmetric.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/layouts/graph_utils.py` & `topometry-0.2.0.4/topo/layouts/graph_utils.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/layouts/isomap.py` & `topometry-0.2.0.4/topo/layouts/isomap.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/layouts/map.py` & `topometry-0.2.0.4/topo/layouts/map.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/layouts/projector.py` & `topometry-0.2.0.4/topo/layouts/projector.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/pipes.py` & `topometry-0.2.0.4/topo/pipes.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         else:
             data_pdist = pairwise_distances(X, metric=metric, n_jobs=n_jobs)
     gc.collect()
     for key in TopOGraph.EigenbasisDict.keys():
         if 'gc' in methods:
             if TopOGraph.verbosity > 0:
                 print('Computing geodesics for eigenbasis \'{}...\''.format(key))
-            emb_graph = kNN(TopOGraph.EigenbasisDict[key].transform(), n_neighbors=n_neighbors,
+            emb_graph = kNN(TopOGraph.EigenbasisDict[key].results(), n_neighbors=n_neighbors,
                             metric=metric,
                             n_jobs=n_jobs,
                             backend=TopOGraph.backend,
                             return_instance=False,
                             verbose=False, **kwargs)
             if landmarks is not None:
                 emb_graph = emb_graph[landmark_indices, :][:, landmark_indices]
@@ -185,21 +185,21 @@
             if TopOGraph.verbosity > 0:
                 print('Computing Spearman R for eigenbasis \'{}...\''.format(key))
             EigenbasisGCResults[key], _ = spearmanr(
                 base_geodesics, embedding_geodesics)
             gc.collect()
         if 'gs' in methods:
             EigenbasisGSResults[key] = global_score(
-                X, TopOGraph.EigenbasisDict[key].transform())
+                X, TopOGraph.EigenbasisDict[key].results())
             if TopOGraph.verbosity > 0:
                 print('Computed global score for eigenbasis {}'.format(key))
             gc.collect()
         if 'tw' in methods:
             EigenbasisTWResults[key] = trustworthiness(data_pdist,
-                                                        TopOGraph.EigenbasisDict[key].transform(), n_neighbors=n_neighbors,
+                                                        TopOGraph.EigenbasisDict[key].results(), n_neighbors=n_neighbors,
                                                         n_jobs=n_jobs, X_is_distance=True, metric=metric)
             gc.collect()
 
     ProjectionTWResults = {}
     ProjectionGCResults = {}
     ProjectionGSResults = {}
     for key in TopOGraph.ProjectionDict.keys():
```

### Comparing `topometry-0.2.0.3/topo/plot.py` & `topometry-0.2.0.4/topo/plot.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/single_cell.py` & `topometry-0.2.0.4/topo/single_cell.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/spectral/_spectral.py` & `topometry-0.2.0.4/topo/spectral/_spectral.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/spectral/eigen.py` & `topometry-0.2.0.4/topo/spectral/eigen.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/spectral/locally.py` & `topometry-0.2.0.4/topo/spectral/locally.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/spectral/umap_layouts.py` & `topometry-0.2.0.4/topo/spectral/umap_layouts.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/topograph.py` & `topometry-0.2.0.4/topo/topograph.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/tpgraph/cknn.py` & `topometry-0.2.0.4/topo/tpgraph/cknn.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/tpgraph/fuzzy.py` & `topometry-0.2.0.4/topo/tpgraph/fuzzy.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/tpgraph/intrinsic_dim.py` & `topometry-0.2.0.4/topo/tpgraph/intrinsic_dim.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/tpgraph/kernels.py` & `topometry-0.2.0.4/topo/tpgraph/kernels.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/tpgraph/procrustes.py` & `topometry-0.2.0.4/topo/tpgraph/procrustes.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/utils/_utils.py` & `topometry-0.2.0.4/topo/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topo/utils/umap_utils.py` & `topometry-0.2.0.4/topo/utils/umap_utils.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.3/topometry.egg-info/PKG-INFO` & `topometry-0.2.0.4/topometry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topometry
-Version: 0.2.0.3
+Version: 0.2.0.4
 Summary: A comprehensive dimensional reduction framework to recover latent information from data.
 Home-page: https://github.com/davisidarta/topometry
 Author: Davi Sidarta-Oliveira
 Author-email: davi.oliveira@dpag.ox.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/davisidarta/topometry/issues
 Platform: UNKNOWN
```

### Comparing `topometry-0.2.0.3/topometry.egg-info/SOURCES.txt` & `topometry-0.2.0.4/topometry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

