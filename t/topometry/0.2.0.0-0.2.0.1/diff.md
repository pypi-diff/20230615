# Comparing `tmp/topometry-0.2.0.0.tar.gz` & `tmp/topometry-0.2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topometry-0.2.0.0.tar", last modified: Wed Jun 14 19:12:35 2023, max compression
+gzip compressed data, was "topometry-0.2.0.1.tar", last modified: Wed Jun 14 22:46:04 2023, max compression
```

## Comparing `topometry-0.2.0.0.tar` & `topometry-0.2.0.1.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 19:12:35.967403 topometry-0.2.0.0/
--rwxrwxrwx   0 root         (0) root         (0)     1101 2022-07-09 04:50:40.000000 topometry-0.2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4059 2023-06-14 19:12:35.967403 topometry-0.2.0.0/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)     3439 2023-03-30 03:29:56.000000 topometry-0.2.0.0/README.md
--rwxrwxrwx   0 root         (0) root         (0)      104 2022-07-09 04:50:40.000000 topometry-0.2.0.0/pyproject.toml
--rwxrwxr-x   0 root         (0) root         (0)      736 2023-06-14 19:12:35.967403 topometry-0.2.0.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)       91 2022-07-09 04:50:40.000000 topometry-0.2.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 19:12:35.963403 topometry-0.2.0.0/topo/
--rwxrwxr-x   0 root         (0) root         (0)      897 2023-03-25 15:07:52.000000 topometry-0.2.0.0/topo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 19:12:35.967403 topometry-0.2.0.0/topo/base/
--rwxrwxrwx   0 root         (0) root         (0)      179 2022-08-31 12:30:15.000000 topometry-0.2.0.0/topo/base/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    47501 2023-06-12 00:26:05.000000 topometry-0.2.0.0/topo/base/ann.py
--rwxrwxr-x   0 root         (0) root         (0)    45676 2023-04-12 15:07:45.000000 topometry-0.2.0.0/topo/base/dists.py
--rwxrwxrwx   0 root         (0) root         (0)    16721 2022-07-09 04:35:01.000000 topometry-0.2.0.0/topo/base/sparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 19:12:35.967403 topometry-0.2.0.0/topo/eval/
--rwxrwxr-x   0 root         (0) root         (0)      218 2023-04-20 20:32:57.000000 topometry-0.2.0.0/topo/eval/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     2218 2023-03-25 15:07:52.000000 topometry-0.2.0.0/topo/eval/global_scores.py
--rwxrwxr-x   0 root         (0) root         (0)    11376 2023-06-12 06:37:03.000000 topometry-0.2.0.0/topo/eval/local_scores.py
--rwxrwxr-x   0 root         (0) root         (0)     6268 2023-04-20 20:32:57.000000 topometry-0.2.0.0/topo/eval/rmetric.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 19:12:35.967403 topometry-0.2.0.0/topo/layouts/
--rwxrwxr-x   0 root         (0) root         (0)      120 2023-03-25 15:07:52.000000 topometry-0.2.0.0/topo/layouts/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    13879 2023-03-25 15:07:52.000000 topometry-0.2.0.0/topo/layouts/graph_utils.py
--rwxrwxr-x   0 root         (0) root         (0)     3366 2023-04-02 09:18:04.000000 topometry-0.2.0.0/topo/layouts/isomap.py
--rwxrwxr-x   0 root         (0) root         (0)     9252 2023-06-13 19:12:15.000000 topometry-0.2.0.0/topo/layouts/map.py
--rwxrwxr-x   0 root         (0) root         (0)    36184 2023-06-12 17:19:13.000000 topometry-0.2.0.0/topo/layouts/projector.py
--rwxrwxr-x   0 root         (0) root         (0)    19272 2023-06-13 20:24:14.000000 topometry-0.2.0.0/topo/pipes.py
--rwxrwxr-x   0 root         (0) root         (0)    22866 2023-06-12 07:51:47.000000 topometry-0.2.0.0/topo/plot.py
--rwxrwxr-x   0 root         (0) root         (0)    21289 2023-06-13 23:22:35.000000 topometry-0.2.0.0/topo/single_cell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 19:12:35.967403 topometry-0.2.0.0/topo/spectral/
--rwxrwxr-x   0 root         (0) root         (0)      265 2023-03-25 15:07:52.000000 topometry-0.2.0.0/topo/spectral/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    23612 2023-04-12 16:16:27.000000 topometry-0.2.0.0/topo/spectral/_spectral.py
--rwxrwxr-x   0 root         (0) root         (0)    26919 2023-06-14 00:30:26.000000 topometry-0.2.0.0/topo/spectral/eigen.py
--rwxrwxrwx   0 root         (0) root         (0)    30671 2022-07-09 04:35:01.000000 topometry-0.2.0.0/topo/spectral/umap_layouts.py
--rwxrwxr-x   0 root         (0) root         (0)    74873 2023-06-14 17:51:28.000000 topometry-0.2.0.0/topo/topograph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 19:12:35.967403 topometry-0.2.0.0/topo/tpgraph/
--rwxrwxr-x   0 root         (0) root         (0)      225 2023-06-04 15:19:29.000000 topometry-0.2.0.0/topo/tpgraph/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     5089 2023-03-25 15:07:52.000000 topometry-0.2.0.0/topo/tpgraph/cknn.py
--rwxrwxr-x   0 root         (0) root         (0)    15089 2023-04-02 09:18:04.000000 topometry-0.2.0.0/topo/tpgraph/fuzzy.py
--rw-rw-r--   0 root         (0) root         (0)    14222 2023-06-04 15:38:27.000000 topometry-0.2.0.0/topo/tpgraph/intrinsic_dim.py
--rwxrwxr-x   0 root         (0) root         (0)    48045 2023-06-14 01:51:30.000000 topometry-0.2.0.0/topo/tpgraph/kernels.py
--rwxrwxr-x   0 root         (0) root         (0)    32597 2023-03-25 15:07:52.000000 topometry-0.2.0.0/topo/tpgraph/procrustes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 19:12:35.967403 topometry-0.2.0.0/topo/utils/
--rwxrwxr-x   0 root         (0) root         (0)       22 2023-03-25 15:07:52.000000 topometry-0.2.0.0/topo/utils/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     5709 2023-06-11 21:38:13.000000 topometry-0.2.0.0/topo/utils/_utils.py
--rwxrwxr-x   0 root         (0) root         (0)     8583 2023-03-25 15:07:52.000000 topometry-0.2.0.0/topo/utils/umap_utils.py
--rwxrwxr-x   0 root         (0) root         (0)       24 2023-06-14 19:07:21.000000 topometry-0.2.0.0/topo/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 19:12:35.967403 topometry-0.2.0.0/topometry.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4059 2023-06-14 19:12:35.000000 topometry-0.2.0.0/topometry.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      933 2023-06-14 19:12:35.000000 topometry-0.2.0.0/topometry.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 19:12:35.000000 topometry-0.2.0.0/topometry.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-14 19:12:35.000000 topometry-0.2.0.0/topometry.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-14 19:12:35.000000 topometry-0.2.0.0/topometry.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:46:04.820172 topometry-0.2.0.1/
+-rwxrwxr-x   0 root         (0) root         (0)     1101 2023-06-14 21:18:44.000000 topometry-0.2.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4870 2023-06-14 22:46:04.820172 topometry-0.2.0.1/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)     4250 2023-06-14 21:18:44.000000 topometry-0.2.0.1/README.md
+-rwxrwxr-x   0 root         (0) root         (0)      104 2023-06-14 21:18:44.000000 topometry-0.2.0.1/pyproject.toml
+-rwxrwxr-x   0 root         (0) root         (0)      736 2023-06-14 22:46:04.820172 topometry-0.2.0.1/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)       91 2023-06-14 21:18:44.000000 topometry-0.2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:46:04.816172 topometry-0.2.0.1/topo/
+-rwxrwxr-x   0 root         (0) root         (0)      897 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:46:04.816172 topometry-0.2.0.1/topo/base/
+-rwxrwxr-x   0 root         (0) root         (0)      179 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/base/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    47503 2023-06-14 21:26:44.000000 topometry-0.2.0.1/topo/base/ann.py
+-rwxrwxr-x   0 root         (0) root         (0)    45676 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/base/dists.py
+-rwxrwxr-x   0 root         (0) root         (0)    16721 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/base/sparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:46:04.816172 topometry-0.2.0.1/topo/eval/
+-rwxrwxr-x   0 root         (0) root         (0)      219 2023-06-14 21:27:15.000000 topometry-0.2.0.1/topo/eval/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     2218 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/eval/global_scores.py
+-rwxrwxr-x   0 root         (0) root         (0)    12754 2023-06-14 21:27:15.000000 topometry-0.2.0.1/topo/eval/local_scores.py
+-rwxrwxr-x   0 root         (0) root         (0)     6058 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/eval/rmetric.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:46:04.816172 topometry-0.2.0.1/topo/layouts/
+-rwxrwxr-x   0 root         (0) root         (0)      120 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/layouts/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    13879 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/layouts/graph_utils.py
+-rwxrwxr-x   0 root         (0) root         (0)     3366 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/layouts/isomap.py
+-rwxrwxr-x   0 root         (0) root         (0)     9251 2023-06-14 21:31:28.000000 topometry-0.2.0.1/topo/layouts/map.py
+-rwxrwxr-x   0 root         (0) root         (0)    36184 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/layouts/projector.py
+-rwxrwxr-x   0 root         (0) root         (0)    19227 2023-06-14 21:25:57.000000 topometry-0.2.0.1/topo/pipes.py
+-rwxrwxr-x   0 root         (0) root         (0)    22966 2023-06-14 22:04:50.000000 topometry-0.2.0.1/topo/plot.py
+-rwxrwxr-x   0 root         (0) root         (0)    21289 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/single_cell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:46:04.816172 topometry-0.2.0.1/topo/spectral/
+-rwxrwxr-x   0 root         (0) root         (0)      265 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/spectral/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    23612 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/spectral/_spectral.py
+-rwxrwxr-x   0 root         (0) root         (0)    26918 2023-06-14 21:28:18.000000 topometry-0.2.0.1/topo/spectral/eigen.py
+-rw-rw-r--   0 root         (0) root         (0)      855 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/spectral/locally.py
+-rwxrwxr-x   0 root         (0) root         (0)    30671 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/spectral/umap_layouts.py
+-rwxrwxr-x   0 root         (0) root         (0)    76100 2023-06-14 21:22:09.000000 topometry-0.2.0.1/topo/topograph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:46:04.820172 topometry-0.2.0.1/topo/tpgraph/
+-rwxrwxr-x   0 root         (0) root         (0)      225 2023-06-14 21:28:40.000000 topometry-0.2.0.1/topo/tpgraph/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     5089 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/tpgraph/cknn.py
+-rwxrwxr-x   0 root         (0) root         (0)    15089 2023-06-14 21:29:14.000000 topometry-0.2.0.1/topo/tpgraph/fuzzy.py
+-rw-rw-r--   0 root         (0) root         (0)    14221 2023-06-14 21:29:14.000000 topometry-0.2.0.1/topo/tpgraph/intrinsic_dim.py
+-rwxrwxr-x   0 root         (0) root         (0)    48044 2023-06-14 21:21:07.000000 topometry-0.2.0.1/topo/tpgraph/kernels.py
+-rwxrwxr-x   0 root         (0) root         (0)    32597 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/tpgraph/procrustes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:46:04.820172 topometry-0.2.0.1/topo/utils/
+-rwxrwxr-x   0 root         (0) root         (0)       22 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/utils/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     5710 2023-06-14 21:31:28.000000 topometry-0.2.0.1/topo/utils/_utils.py
+-rwxrwxr-x   0 root         (0) root         (0)     8583 2023-06-14 21:18:44.000000 topometry-0.2.0.1/topo/utils/umap_utils.py
+-rwxrwxr-x   0 root         (0) root         (0)       24 2023-06-14 22:45:36.000000 topometry-0.2.0.1/topo/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:46:04.820172 topometry-0.2.0.1/topometry.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4870 2023-06-14 22:46:04.000000 topometry-0.2.0.1/topometry.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      958 2023-06-14 22:46:04.000000 topometry-0.2.0.1/topometry.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 22:46:04.000000 topometry-0.2.0.1/topometry.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-14 22:46:04.000000 topometry-0.2.0.1/topometry.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-14 22:46:04.000000 topometry-0.2.0.1/topometry.egg-info/top_level.txt
```

### Comparing `topometry-0.2.0.0/LICENSE` & `topometry-0.2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.0/PKG-INFO` & `topometry-0.2.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topometry
-Version: 0.2.0.0
+Version: 0.2.0.1
 Summary: A comprehensive dimensional reduction framework to recover latent information from data.
 Home-page: https://github.com/davisidarta/topometry
 Author: Davi Sidarta-Oliveira
 Author-email: davi.oliveira@dpag.ox.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/davisidarta/topometry/issues
 Platform: UNKNOWN
@@ -22,29 +22,38 @@
 [![Downloads](https://static.pepy.tech/personalized-badge/topometry?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/topometry)
 [![CodeFactor](https://www.codefactor.io/repository/github/davisidarta/topometry/badge)](https://www.codefactor.io/repository/github/davisidarta/topometry)
 [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/DaviSidarta.svg?style=social&label=Follow%20%40davisidarta)](https://twitter.com/davisidarta)
 
 # TopOMetry - Topologically Optimized geoMetry
 
 
-## A global framework for dimensionality reduction: learning topologic metrics, orthonormal bases and graph layouts
-
 TopOMetry is a high-level python library to explore data topology through manifold learning. It is compatible with scikit-learn, meaning most of its operators can be easily pipelined.
 
 Its main idea is to approximate the [Laplace-Beltrami Operator (LBO)](https://en.wikipedia.org/wiki/Laplace%E2%80%93Beltrami_operator). This is done by learning properly weighted similarity graphs and their Laplacian and Diffusion operators. By definition, the eigenfunctions of these operators describe all underlying data topology in an set of orthonormal eigenbases (classically named the spectral or diffusion components). New topological operators are then learned from such eigenbases and can be used for clustering and graph-layout optimization (visualization). 
 
+There are many different ways to computationally approximate the LBO. TopOMetry tests a wide array of possible algorithmic combinations, combines them with existing graph-layout algorithm and scores them aftwerwards. This way, users do not have to choose a fixed method _a priori_, and can instead decide what works best for each use case. It also includes various utilities for scoring the performance of similarity kernels and dimensional reductions of high-dimensional data. It includes methods for the estimation of intrinsic dimensionalities (global and local), and implements the [Riemann metric]() to qualitatively visualize distortions in 2-D embeddings.
+
 For more information, see the [manuscript](https://doi.org/10.1101/2022.03.14.484134).
 
-TopOMetry was designed to handle large-scale data matrices containing extreme sample diversity, such as those generated from [single-cell omics](https://en.wikipedia.org/wiki/Single_cell_sequencing). It includes wrappers to deal with [AnnData](https://anndata.readthedocs.io/en/latest/index.html) objects using [scanpy](https://scanpy.readthedocs.io/en/stable/).
+
+## Single-cell analysis
+
+TopOMetry was designed to handle large-scale data matrices containing extreme sample diversity, such as those generated from high-throughput [single-cell experiments](https://en.wikipedia.org/wiki/Single_cell_sequencing). It includes wrappers to deal with [AnnData](https://anndata.readthedocs.io/en/latest/index.html) objects using [scanpy](https://scanpy.readthedocs.io/en/stable/) and integrates well with tools in the [scverse](https://scverse.org/) python suite for single-cell analysis.
 
 -------------------
 
 ## Documentation
 
-Documentation is available at [Read The Docs](https://topometry.readthedocs.io/en/latest/). There you'll find installation instructions, tutorials, walkthroughs and a detailed API for reference.
+Instalation can be quickly done with pip:
+
+```
+pip install topometry
+```
+
+Further installation instructions such as optional dependencies, information about the implemented methods tutorials and a detailed API are available at the available at the [documentation](https://topometry.readthedocs.io/en/latest/). 
 
 -------------------
 
 ## Contributing
 
 Contributions are very welcome! If you're interested in adding a new feature, just let me know in the Issues section.
 
@@ -54,15 +63,15 @@
 
 [MIT License](https://github.com/davisidarta/topometry/blob/master/LICENSE)
 
 -------------------
 
 ## Citation
 
-If you find TopOMetry useful for your work, please cite our manuscript:
+If you use TopOMetry for your work, please cite the manuscript:
 
 ``` bibtex
 @article {Sidarta-Oliveira2022.03.14.484134,
 	author = {Sidarta-Oliveira, Davi and Velloso, Licio A},
 	title = {A comprehensive dimensional reduction framework to learn single-cell phenotypic topology uncovers T cell diversity},
 	elocation-id = {2022.03.14.484134},
 	year = {2022},
```

### Comparing `topometry-0.2.0.0/README.md` & `topometry-0.2.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -5,29 +5,38 @@
 [![Downloads](https://static.pepy.tech/personalized-badge/topometry?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/topometry)
 [![CodeFactor](https://www.codefactor.io/repository/github/davisidarta/topometry/badge)](https://www.codefactor.io/repository/github/davisidarta/topometry)
 [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/DaviSidarta.svg?style=social&label=Follow%20%40davisidarta)](https://twitter.com/davisidarta)
 
 # TopOMetry - Topologically Optimized geoMetry
 
 
-## A global framework for dimensionality reduction: learning topologic metrics, orthonormal bases and graph layouts
-
 TopOMetry is a high-level python library to explore data topology through manifold learning. It is compatible with scikit-learn, meaning most of its operators can be easily pipelined.
 
 Its main idea is to approximate the [Laplace-Beltrami Operator (LBO)](https://en.wikipedia.org/wiki/Laplace%E2%80%93Beltrami_operator). This is done by learning properly weighted similarity graphs and their Laplacian and Diffusion operators. By definition, the eigenfunctions of these operators describe all underlying data topology in an set of orthonormal eigenbases (classically named the spectral or diffusion components). New topological operators are then learned from such eigenbases and can be used for clustering and graph-layout optimization (visualization). 
 
+There are many different ways to computationally approximate the LBO. TopOMetry tests a wide array of possible algorithmic combinations, combines them with existing graph-layout algorithm and scores them aftwerwards. This way, users do not have to choose a fixed method _a priori_, and can instead decide what works best for each use case. It also includes various utilities for scoring the performance of similarity kernels and dimensional reductions of high-dimensional data. It includes methods for the estimation of intrinsic dimensionalities (global and local), and implements the [Riemann metric]() to qualitatively visualize distortions in 2-D embeddings.
+
 For more information, see the [manuscript](https://doi.org/10.1101/2022.03.14.484134).
 
-TopOMetry was designed to handle large-scale data matrices containing extreme sample diversity, such as those generated from [single-cell omics](https://en.wikipedia.org/wiki/Single_cell_sequencing). It includes wrappers to deal with [AnnData](https://anndata.readthedocs.io/en/latest/index.html) objects using [scanpy](https://scanpy.readthedocs.io/en/stable/).
+
+## Single-cell analysis
+
+TopOMetry was designed to handle large-scale data matrices containing extreme sample diversity, such as those generated from high-throughput [single-cell experiments](https://en.wikipedia.org/wiki/Single_cell_sequencing). It includes wrappers to deal with [AnnData](https://anndata.readthedocs.io/en/latest/index.html) objects using [scanpy](https://scanpy.readthedocs.io/en/stable/) and integrates well with tools in the [scverse](https://scverse.org/) python suite for single-cell analysis.
 
 -------------------
 
 ## Documentation
 
-Documentation is available at [Read The Docs](https://topometry.readthedocs.io/en/latest/). There you'll find installation instructions, tutorials, walkthroughs and a detailed API for reference.
+Instalation can be quickly done with pip:
+
+```
+pip install topometry
+```
+
+Further installation instructions such as optional dependencies, information about the implemented methods tutorials and a detailed API are available at the available at the [documentation](https://topometry.readthedocs.io/en/latest/). 
 
 -------------------
 
 ## Contributing
 
 Contributions are very welcome! If you're interested in adding a new feature, just let me know in the Issues section.
 
@@ -37,15 +46,15 @@
 
 [MIT License](https://github.com/davisidarta/topometry/blob/master/LICENSE)
 
 -------------------
 
 ## Citation
 
-If you find TopOMetry useful for your work, please cite our manuscript:
+If you use TopOMetry for your work, please cite the manuscript:
 
 ``` bibtex
 @article {Sidarta-Oliveira2022.03.14.484134,
 	author = {Sidarta-Oliveira, Davi and Velloso, Licio A},
 	title = {A comprehensive dimensional reduction framework to learn single-cell phenotypic topology uncovers T cell diversity},
 	elocation-id = {2022.03.14.484134},
 	year = {2022},
```

### Comparing `topometry-0.2.0.0/setup.cfg` & `topometry-0.2.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = topometry
-version = 0.2.0.0
+version = 0.2.0.1
 author = Davi Sidarta-Oliveira
 author_email = davi.oliveira@dpag.ox.ac.uk
 description = A comprehensive dimensional reduction framework to recover latent information from data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/davisidarta/topometry
 project_urls =
```

### Comparing `topometry-0.2.0.0/topo/__init__.py` & `topometry-0.2.0.1/topo/__init__.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.0/topo/base/ann.py` & `topometry-0.2.0.1/topo/base/ann.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,17 +302,17 @@
 
     def __init__(self,
                  n_neighbors=15,
                  metric='cosine',
                  method='hnsw',
                  n_jobs=-1,
                  p=None,
-                 M=15,
-                 efC=50,
-                 efS=50,
+                 M=30,
+                 efC=100,
+                 efS=100,
                  dense=False,
                  verbose=False
                  ):
 
         self.n_neighbors = n_neighbors
         self.method = method
         self.metric = metric
```

### Comparing `topometry-0.2.0.0/topo/base/dists.py` & `topometry-0.2.0.1/topo/base/dists.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.0/topo/base/sparse.py` & `topometry-0.2.0.1/topo/base/sparse.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.0/topo/eval/global_scores.py` & `topometry-0.2.0.1/topo/eval/global_scores.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.0/topo/eval/local_scores.py` & `topometry-0.2.0.1/topo/eval/local_scores.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,19 +6,52 @@
 from topo.utils._utils import get_landmark_indices
 from topo.base.ann import kNN
 from sklearn.neighbors import NearestNeighbors
 from sklearn.metrics import pairwise_distances
 
 def geodesic_distance(adjacency, method='D', unweighted=False, directed=False, indices=None, n_jobs=-1, random_state=None):
     """
-    Compute the geodesic distance matrix from an adjacency matrix.
+    Subsets the geodesic distance matrix to only include distances up to the k-th
+    nearest neighbor distance for each point.
+
+    Parameters:
+    -----------
+    knn_dists: scipy.sparse.csr_matrix
+        Precomputed k-nearest-neighbors distances matrix.
+    geodesic_dists: scipy.sparse.csr_matrix
+        Geodesic distances matrix.
+
+    Returns:
+    --------
+    subset_geodesics: scipy.sparse.csr_matrix
+        Subsetted geodesic distances matrix.
+    """
+    n_points = knn_dists.shape[0]
+    # Compute the maximum distance to consider for each point
+    max_dist = knn_dists.max(axis=1).toarray()
+    # Subset the geodesic distances matrix
+    subset_geodesics = lil_matrix(geodesic_dists.shape, dtype=np.float32)
+    for i in range(n_points):
+        mask = (geodesic_dists[i,:] <= max_dist[i,:]).flatten()
+        subset_geodesics[i,mask] = geodesic_dists[i,mask]
+    subset_geodesics = subset_geodesics.tocsr()
+    return subset_geodesics
+
+
+def geodesic_distance(A, method='D', unweighted=False, directed=False, indices=None, n_jobs=-1, subset_to_knn=True, random_state=None):
+    """
+    Compute the geodesic distance matrix from an adjacency (or an affinity) matrix.
+    The default behavior is to subset the geodesic distance matrix to only include distances up
+    to the k-th nearest neighbor distance for each point. This is to ensure we are only assessing
+    the performance of the embedding on the local structure of the data.
+
     Parameters
     ----------
-    adjacency : array-like, shape (n_vertices, n_vertices)
-        Adjacency matrix of a graph.
+    A : array-like, shape (n_vertices, n_vertices)
+        Adjacency or affinity matrix of a graph.
 
     method : string, optional, default: 'D'
         Method to compute the shortest path.
         - 'D': Dijkstra's algorithm.
         - 'FW': Floyd-Warshall algorithm.
         - 'B': Bellman-Ford algorithm.
         - 'J': Johnson algorithm.
@@ -57,15 +90,15 @@
             from joblib import cpu_count
             n_jobs = cpu_count()
         if not isinstance(n_jobs, int):
             n_jobs = 1
         if method == 'FW':
             raise ValueError('The Floyd-Warshall algorithm cannot be used with parallel computations.')
         if indices is None:
-            indices = np.arange(adjacency.shape[0])
+            indices = np.arange(A.shape[0])
         elif np.issubdtype(type(indices), np.integer):
             indices = np.array([indices])
         n = len(indices)
         local_function = partial(csgraph.shortest_path,
                                 adjacency, method, directed, False, unweighted, False)
         if n_jobs == 1 or n == 1:
             try:
```

### Comparing `topometry-0.2.0.0/topo/eval/rmetric.py` & `topometry-0.2.0.1/topo/eval/rmetric.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,18 +43,15 @@
 
 class RiemannMetric(object):
     """
     RiemannMetric computes and stores the Riemannian metric and its dual
     associated with an embedding Y. The Riemannian metric is currently denoted
     by G, its dual by H, and the Laplacian by L. G at each point is the
     matrix inverse of H.
-    For performance, the following choices have been made:
-    * the class makes no defensive copies of L, Y
-    * no defensive copies of the array attributes H, G, Hvv, ....
-    * G is computed on request only
+
     In the future, this class will be extended to compute H only once,
     for mdimY dimensions, but to store multiple G's, with different dimensions.
     In the near future plans is also a "lazy" implementation, which will
     compute G (and maybe even H) only at the requested points.
 
     This implementation is from megaman, by Marina Meila (License simplified BSD), with
     adaptations from Davi Sidarta-Oliveira as included in TopOMetry for performance and
```

### Comparing `topometry-0.2.0.0/topo/layouts/graph_utils.py` & `topometry-0.2.0.1/topo/layouts/graph_utils.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.0/topo/layouts/isomap.py` & `topometry-0.2.0.1/topo/layouts/isomap.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.0/topo/layouts/map.py` & `topometry-0.2.0.1/topo/layouts/map.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                     verbose=False,
                     a=None,
                     b=None,
                     densmap=False,
                     densmap_kwds={},
                     output_dens=False,
                     ):
-    """\
+    """
     Perform a fuzzy simplicial set embedding, using a specified
     initialisation method and then minimizing the fuzzy set cross entropy
     between the 1-skeletons of the high and low dimensional fuzzy simplicial
     sets. The fuzzy simplicial set embedding was proposed and implemented by
     Leland McInnes in UMAP (see `umap-learn <https://github.com/lmcinnes/umap>`).
     Here we're using it only for the projection (layout optimization).
```

### Comparing `topometry-0.2.0.0/topo/layouts/projector.py` & `topometry-0.2.0.1/topo/layouts/projector.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.0/topo/pipes.py` & `topometry-0.2.0.1/topo/pipes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-from sklearn.utils import check_random_state
 from scipy.sparse import issparse, csr_matrix
 from scipy.stats import spearmanr, kendalltau
 from scipy.spatial.distance import squareform
 from topo.utils._utils import get_landmark_indices
 from topo.base.ann import kNN
 from topo.topograph import TopOGraph
 from topo.eval.global_scores import global_score_pca
```

### Comparing `topometry-0.2.0.0/topo/plot.py` & `topometry-0.2.0.1/topo/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -388,22 +388,23 @@
                         labels=None, pt_size=1, cmap='Spectral',  figsize=(8,8), random_state=None, **kwargs):
     """
     Plot Riemannian metric using ellipses. Adapted from Megaman (https://github.com/mmp2/megaman).
 
     Parameters
     ----------
     
-    emb: numpy.ndarray
+    emb: numpy.ndarray, shape = (n, n_dim)
         Embedding matrix.
     
-    laplacian: numpy.ndarray
+    L: numpy.ndarray
        Graph Laplacian matrix. Should be provided if H_emb is not provided.
     
-    H_emb: numpy.ndarray
-        Embedding matrix of the H. Should be provided if laplacian is not provided.
+    H : Dual Riemann metric, shape = (n, n_dim, n_dim)
+        The inverse (dual) Riemann metric matrix at each point. Should be provided if Laplacian is not provided.
+        Computed with the class `topo.eval.rmetric.RiemannMetric`.
 
     n_plot: int (optional, default 50)
         Number of ellipses to plot.
 
     std: int (optional, default 1)
         Standard deviation of the ellipses. This should be adjusted by hand for visualization purposes.
 
@@ -414,15 +415,15 @@
         Size of the points.
     
     cmap: str (optional, default 'Spectral')
         Color map for the points.
 
     figsize: tuple (optional, default (8,8))
         Figure size.
-    
+
     random_state: int (optional, default None)
         Random state for sampling points to plot ellipses of.
 
     kwargs: dict
         Additional arguments for matplotlib.
 
     References
@@ -432,16 +433,16 @@
     Dominique Perraul-Joncas, Marina Meila, arXiv:1305.7255
 
 
     """
 
     if H_emb is None:
         from topo.eval import RiemannMetric
-        rmetric = RiemannMetric(emb, laplacian)
-        H_emb = rmetric.get_dual_rmetric()
+        rmetric = RiemannMetric(emb, L)
+        H = rmetric.get_dual_rmetric()
 
     N = np.shape(emb)[0]
     rng = check_random_state(random_state)
     sample_points = rng.choice(range(N), n_plot, replace=False)
     if ax == None:
         f, ax = plt.subplots(figsize=figsize)
     # ax.grid(False)
@@ -453,15 +454,15 @@
     if labels is not None:
         colors = plt.get_cmap(cmap)(np.linspace(0, 1, np.shape(np.unique(labels))[0]))
         ax.scatter(emb[:, 0], emb[:, 1], s=pt_size, c=labels, cmap=cmap)
     else:
         ax.scatter(emb[:, 0], emb[:, 1], s=pt_size)
     for i in range(n_plot):
         ii = sample_points[i]
-        cov = H_emb[ii, :, :]
+        cov = H[ii, :, :]
         if labels is not None:
             plot_cov_ellipse(cov, emb[ii, :], nstd=std, ax=ax, edgecolor='none', color=colors[labels[ii]],
                              alpha=alpha)
         else:
             plot_cov_ellipse(cov, emb[ii, :], nstd=std, ax=ax, edgecolor='none',
                              alpha=alpha)
     return ax
@@ -473,15 +474,15 @@
             affinity = kernel[i,j]
             if affinity > 0:
                 ax.plot(data[[i,j],0], data[[i,j],1],
                         color=color, alpha=affinity, zorder=0, **kwargs)
     
 
 
-def plot_scores(scores, return_plot=True, log=False, figsize=(20,8), fontsize=15, title='Eigenbasis local scores'):
+def plot_scores(scores, return_plot=True, log=True, figsize=(8,3), fontsize=12, title='Scores'):
     keys = scores.keys()
     values = scores.values()
     cmap = get_cmap(len(keys), name='tab20')
     k_color = list()
     for k in np.arange(len(keys)):
         k_color.append(cmap(k))
     fig, (ax1) = plt.subplots(1, 1, figsize=figsize)
@@ -674,8 +675,8 @@
     texts = []
     for i in range(data.shape[0]):
         for j in range(data.shape[1]):
             kw.update(color=textcolors[int(im.norm(data[i, j]) > threshold)])
             text = im.axes.text(j, i, valfmt(data[i, j], None), fontsize=an_fontsize, **kw)
             texts.append(text)
 
-    return texts
+    return texts
```

### Comparing `topometry-0.2.0.0/topo/single_cell.py` & `topometry-0.2.0.1/topo/single_cell.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.0/topo/spectral/_spectral.py` & `topometry-0.2.0.1/topo/spectral/_spectral.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.0/topo/spectral/eigen.py` & `topometry-0.2.0.1/topo/spectral/eigen.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,14 @@
                     eigs_idx = list(range(1, int(use_eigs)))
                     eig_vals = np.ravel(evals[eigs_idx])
                     self.embedding = evecs[:, eigs_idx] * (eig_vals / (1 - eig_vals))
         else:
             self.embedding = evecs
         self.eigenvectors = evecs
         self.eigenvalues = evals
-
         return self
 
     def rescale(self, use_eigs=50):
         """
         If using multiscale diffusion maps, this rescales the mapping to a new number of eigenvectors.
         """
         if self.method != 'msDM':
```

### Comparing `topometry-0.2.0.0/topo/spectral/umap_layouts.py` & `topometry-0.2.0.1/topo/spectral/umap_layouts.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.0/topo/topograph.py` & `topometry-0.2.0.1/topo/topograph.py`

 * *Files 4% similar despite different names*

```diff
@@ -526,15 +526,17 @@
         else:
             start = time.time()
             self.base_kernel, self.BaseKernelDict = self._compute_kernel_from_version_knn(self.base_knn_graph,
                                                                                           self.base_knn,
                                                                                           self.base_kernel_version,
                                                                                           self.BaseKernelDict,
                                                                                           suffix='',
-                                                                                          low_memory=self.low_memory)
+                                                                                          low_memory=self.low_memory,
+                                                                                          data_for_expansion=X,
+                                                                                          base=True)
             end = time.time()
             gc.collect()
             if self.verbosity >= 1:
                 print(' Fitted the ' + (self.base_kernel_version) +
                       ' kernel in %f (sec)' % (end - start))
 
         if self.verbosity >= 1:
@@ -755,16 +757,17 @@
             eigenbasis = self.eigenbasis
         else:
             raise ValueError('No eigenbasis computed. Call .fit() first.')
         if self.verbosity >= 1:
             print('    Building topological graph from eigenbasis...')
         if self.verbosity >= 1:
             print('        Computing neighborhood graph...')
+        target = eigenbasis.transform(X=None)[:, 0:eigenbasis.eigengap]
         start = time.time()
-        self.eigenbasis_knn_graph = kNN(eigenbasis.transform(X=None), n_neighbors=self.graph_knn,
+        self.eigenbasis_knn_graph = kNN(target, n_neighbors=self.graph_knn,
                                         metric=self.graph_metric,
                                         n_jobs=self.n_jobs,
                                         backend=self.backend,
                                         return_instance=False,
                                         verbose=self.bases_graph_verbose, **kwargs)
         end = time.time()
         gc.collect()
@@ -773,15 +776,17 @@
             print(' Computed in %f (sec)' % (end - start))
         start = time.time()
         self.graph_kernel, self.GraphKernelDict = self._compute_kernel_from_version_knn(self.eigenbasis_knn_graph,
                                                                                         self.graph_knn,
                                                                                         self.graph_kernel_version,
                                                                                         self.GraphKernelDict,
                                                                                         suffix=' from ' + self.current_eigenbasis,
-                                                                                        low_memory=self.low_memory)
+                                                                                        low_memory=self.low_memory,
+                                                                                        data_for_expansion=eigenbasis.transform(X=None),
+                                                                                        base=False)
         
         end = time.time()
         gc.collect()
         self.current_graphkernel = self.graph_kernel_version + \
             ' from ' + self.current_eigenbasis
         if self.verbosity >= 1:
             print(' Fitted the ' + str(self.graph_kernel_version) +
@@ -1043,15 +1048,15 @@
     #     self.EigenbasisDict = {}
     #     self.GraphKernelDict = {}
     #     self.ProjectionDict = {}
 
 
 
 
-    def _compute_kernel_from_version_knn(self, knn, n_neighbors, kernel_version, results_dict, prefix='', suffix='', low_memory=False):
+    def _compute_kernel_from_version_knn(self, knn, n_neighbors, kernel_version, results_dict, prefix='', suffix='', low_memory=False, data_for_expansion=None):
         import gc
         gc.collect()
         kernel_key = kernel_version
         if prefix is not None:
             kernel_key = prefix + kernel_key
         if suffix is not None:
             kernel_key = kernel_key + suffix
@@ -1140,15 +1145,21 @@
                                 cache_input=False,
                                 verbose=self.bases_graph_verbose,
                                 random_state=self.random_state).fit(knn)
                 gc.collect()
                 results_dict[kernel_key] = kernel
 
             elif kernel_version == 'bw_adaptive_nbr_expansion':
-                kernel = Kernel(metric="precomputed",
+                if data_for_expansion is None:
+                    raise ValueError('data_for_expansion is None. Please provide data for neighborhood expansion when using the `bw_adaptive_nbr_expansion`.')
+                if base:
+                    use_metric = self.base_metric
+                else:
+                    use_metric = self.graph_metric
+                kernel = Kernel(metric=use_metric,
                                 n_neighbors=n_neighbors,
                                 fuzzy=False,
                                 cknn=False,
                                 pairwise=False,
                                 sigma=None,
                                 adaptive_bw=True,
                                 expand_nbr_search=True,
@@ -1161,15 +1172,21 @@
                                 cache_input=False,
                                 verbose=self.bases_graph_verbose,
                                 random_state=self.random_state).fit(knn)
                 gc.collect()
                 results_dict[kernel_key] = kernel
 
             elif kernel_version == 'bw_adaptive_alpha_decaying_nbr_expansion':
-                kernel = Kernel(metric="precomputed",
+                if data_for_expansion is None:
+                    raise ValueError('data_for_expansion is None. Please provide data for neighborhood expansion when using the `bw_adaptive_nbr_expansion`.')
+                if base:
+                    use_metric = self.base_metric
+                else:
+                    use_metric = self.graph_metric
+                kernel = Kernel(metric=use_metric,
                                 n_neighbors=n_neighbors,
                                 fuzzy=False,
                                 cknn=False,
                                 pairwise=False,
                                 sigma=None,
                                 adaptive_bw=True,
                                 expand_nbr_search=True,
```

### Comparing `topometry-0.2.0.0/topo/tpgraph/cknn.py` & `topometry-0.2.0.1/topo/tpgraph/cknn.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.0/topo/tpgraph/fuzzy.py` & `topometry-0.2.0.1/topo/tpgraph/fuzzy.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.0/topo/tpgraph/intrinsic_dim.py` & `topometry-0.2.0.1/topo/tpgraph/intrinsic_dim.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 ## Algorithms intrinsic dimensionality estimation
-
 import numpy as np
 from scipy.sparse.linalg import eigsh
 from topo.spectral import diffusion_operator
 from topo.base.ann import kNN
 from sklearn.base import BaseEstimator, TransformerMixin
 from topo.utils._utils import get_indices_distances_from_sparse_matrix
```

### Comparing `topometry-0.2.0.0/topo/tpgraph/kernels.py` & `topometry-0.2.0.1/topo/tpgraph/kernels.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,14 @@
                 if sigma == 0:
                     sigma = 1e-10
                 dists = (dists / sigma) ** 2
         W = csr_matrix((np.abs(np.exp(-dists)), (x, y)), shape=[N, N])
     if symmetrize:
         W = (W + W.T) / 2
     #W[(np.arange(N), np.arange(N))] = 0
-
     # handle nan
     W.data = np.where(np.isnan(W.data), 1, W.data)
     if not return_densities:
         return W
     else:
         return W, dens_dict
```

### Comparing `topometry-0.2.0.0/topo/tpgraph/procrustes.py` & `topometry-0.2.0.1/topo/tpgraph/procrustes.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.0/topo/utils/_utils.py` & `topometry-0.2.0.1/topo/utils/_utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -142,8 +142,8 @@
         width, height = np.sqrt(np.absolute(vals))
         if width > height:
             R = width / height
         else:
             R = height / width
         ecc = np.sqrt(np.abs(1 - R))
         ecc_list.append(ecc)
-    return ecc_list
+    return ecc_list
```

### Comparing `topometry-0.2.0.0/topo/utils/umap_utils.py` & `topometry-0.2.0.1/topo/utils/umap_utils.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.0/topometry.egg-info/PKG-INFO` & `topometry-0.2.0.1/topometry.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topometry
-Version: 0.2.0.0
+Version: 0.2.0.1
 Summary: A comprehensive dimensional reduction framework to recover latent information from data.
 Home-page: https://github.com/davisidarta/topometry
 Author: Davi Sidarta-Oliveira
 Author-email: davi.oliveira@dpag.ox.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/davisidarta/topometry/issues
 Platform: UNKNOWN
@@ -22,29 +22,38 @@
 [![Downloads](https://static.pepy.tech/personalized-badge/topometry?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/topometry)
 [![CodeFactor](https://www.codefactor.io/repository/github/davisidarta/topometry/badge)](https://www.codefactor.io/repository/github/davisidarta/topometry)
 [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/DaviSidarta.svg?style=social&label=Follow%20%40davisidarta)](https://twitter.com/davisidarta)
 
 # TopOMetry - Topologically Optimized geoMetry
 
 
-## A global framework for dimensionality reduction: learning topologic metrics, orthonormal bases and graph layouts
-
 TopOMetry is a high-level python library to explore data topology through manifold learning. It is compatible with scikit-learn, meaning most of its operators can be easily pipelined.
 
 Its main idea is to approximate the [Laplace-Beltrami Operator (LBO)](https://en.wikipedia.org/wiki/Laplace%E2%80%93Beltrami_operator). This is done by learning properly weighted similarity graphs and their Laplacian and Diffusion operators. By definition, the eigenfunctions of these operators describe all underlying data topology in an set of orthonormal eigenbases (classically named the spectral or diffusion components). New topological operators are then learned from such eigenbases and can be used for clustering and graph-layout optimization (visualization). 
 
+There are many different ways to computationally approximate the LBO. TopOMetry tests a wide array of possible algorithmic combinations, combines them with existing graph-layout algorithm and scores them aftwerwards. This way, users do not have to choose a fixed method _a priori_, and can instead decide what works best for each use case. It also includes various utilities for scoring the performance of similarity kernels and dimensional reductions of high-dimensional data. It includes methods for the estimation of intrinsic dimensionalities (global and local), and implements the [Riemann metric]() to qualitatively visualize distortions in 2-D embeddings.
+
 For more information, see the [manuscript](https://doi.org/10.1101/2022.03.14.484134).
 
-TopOMetry was designed to handle large-scale data matrices containing extreme sample diversity, such as those generated from [single-cell omics](https://en.wikipedia.org/wiki/Single_cell_sequencing). It includes wrappers to deal with [AnnData](https://anndata.readthedocs.io/en/latest/index.html) objects using [scanpy](https://scanpy.readthedocs.io/en/stable/).
+
+## Single-cell analysis
+
+TopOMetry was designed to handle large-scale data matrices containing extreme sample diversity, such as those generated from high-throughput [single-cell experiments](https://en.wikipedia.org/wiki/Single_cell_sequencing). It includes wrappers to deal with [AnnData](https://anndata.readthedocs.io/en/latest/index.html) objects using [scanpy](https://scanpy.readthedocs.io/en/stable/) and integrates well with tools in the [scverse](https://scverse.org/) python suite for single-cell analysis.
 
 -------------------
 
 ## Documentation
 
-Documentation is available at [Read The Docs](https://topometry.readthedocs.io/en/latest/). There you'll find installation instructions, tutorials, walkthroughs and a detailed API for reference.
+Instalation can be quickly done with pip:
+
+```
+pip install topometry
+```
+
+Further installation instructions such as optional dependencies, information about the implemented methods tutorials and a detailed API are available at the available at the [documentation](https://topometry.readthedocs.io/en/latest/). 
 
 -------------------
 
 ## Contributing
 
 Contributions are very welcome! If you're interested in adding a new feature, just let me know in the Issues section.
 
@@ -54,15 +63,15 @@
 
 [MIT License](https://github.com/davisidarta/topometry/blob/master/LICENSE)
 
 -------------------
 
 ## Citation
 
-If you find TopOMetry useful for your work, please cite our manuscript:
+If you use TopOMetry for your work, please cite the manuscript:
 
 ``` bibtex
 @article {Sidarta-Oliveira2022.03.14.484134,
 	author = {Sidarta-Oliveira, Davi and Velloso, Licio A},
 	title = {A comprehensive dimensional reduction framework to learn single-cell phenotypic topology uncovers T cell diversity},
 	elocation-id = {2022.03.14.484134},
 	year = {2022},
```

### Comparing `topometry-0.2.0.0/topometry.egg-info/SOURCES.txt` & `topometry-0.2.0.1/topometry.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 topo/layouts/graph_utils.py
 topo/layouts/isomap.py
 topo/layouts/map.py
 topo/layouts/projector.py
 topo/spectral/__init__.py
 topo/spectral/_spectral.py
 topo/spectral/eigen.py
+topo/spectral/locally.py
 topo/spectral/umap_layouts.py
 topo/tpgraph/__init__.py
 topo/tpgraph/cknn.py
 topo/tpgraph/fuzzy.py
 topo/tpgraph/intrinsic_dim.py
 topo/tpgraph/kernels.py
 topo/tpgraph/procrustes.py
```

