# Comparing `tmp/small_world_propensity-0.0.0.tar.gz` & `tmp/small_world_propensity-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "small_world_propensity-0.0.0.tar", max compression
+gzip compressed data, was "small_world_propensity-0.0.2.tar", max compression
```

## Comparing `small_world_propensity-0.0.0.tar` & `small_world_propensity-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2134 2023-06-15 10:44:48.448372 small_world_propensity-0.0.0/README.md
--rw-r--r--   0        0        0     1710 2023-06-15 11:53:40.458427 small_world_propensity-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      284 2023-06-14 19:44:11.768065 small_world_propensity-0.0.0/small_world_propensity/__init__.py
--rw-r--r--   0        0        0     7058 2023-06-15 09:46:05.238869 small_world_propensity-0.0.0/small_world_propensity/small_world_propensity.py
--rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 small_world_propensity-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2344 2023-06-15 13:13:34.958452 small_world_propensity-0.0.2/README.md
+-rw-r--r--   0        0        0     1710 2023-06-15 13:13:51.418575 small_world_propensity-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      284 2023-06-15 13:13:34.974452 small_world_propensity-0.0.2/small_world_propensity/__init__.py
+-rw-r--r--   0        0        0     7058 2023-06-15 13:13:34.974452 small_world_propensity-0.0.2/small_world_propensity/small_world_propensity.py
+-rw-r--r--   0        0        0     3117 1970-01-01 00:00:00.000000 small_world_propensity-0.0.2/PKG-INFO
```

### Comparing `small_world_propensity-0.0.0/README.md` & `small_world_propensity-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,36 @@
+Metadata-Version: 2.1
+Name: small-world-propensity
+Version: 0.0.2
+Summary: A package designed to calculate the small-world propensity of a weighted, undirected network. Translated from the MATLAB version featured in Muldoon et al.
+License: GPL-3.0-only
+Author: Ryan Daniels
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: networkx (>=3.1,<4.0)
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
+Requires-Dist: pandas (>=2.0.2,<3.0.0)
+Requires-Dist: python-igraph (>=0.10.4,<0.11.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Description-Content-Type: text/markdown
+
 # Small World Propensity
 
 This python package was adapted from the MATLAB package as first presented in [Small-World Propensity and Weighted Brain Networks](https://www.nature.com/articles/srep22057) (2016) by Sarah Feldt Muldoon, Eric W. Bridgeford & Danielle S. Bassett. Their original MATLAB implementation can be found [here](https://kk1995.github.io/BauerLab/BauerLab/MATLAB/lib/+mouse/+graph/smallWorldPropensity.html).
 
 ## Use
 The small-world propensity package can be installed using pip
 ```
 python -m pip install small-world-propensity
 ```
 `small_world_propensity` can be called in two ways: either with a single adjacency matrix, or with a list of adjacency matrices and a boolean list denoting whether each matrix is binary or not. In either case, `small_world_propensity` will return a `pandas` dataframe similar to the following:
-![Dataframe](img/dataframe.png "Dataframe")
+![Dataframe](https://github.com/rkdan/small_world_propensity/blob/main/img/dataframe.png?raw=True)
 
 ## Generation of regular and random matrices
 Using the structural network of the cat cortex obtained from tract-tracing studies between 52 brain regions, we can visualize the process behind the calculation of $\phi$. The matrix is loaded using
 
 ```
 cat = sio.loadmat('data/cat.mat')['CIJctx']
 ```
@@ -25,17 +43,18 @@
 r = swp.get_avg_rad_eff(symm_cat)
 cat_reg = swp.regular_matrix_generator(symm_cat, r)
 ```
 Finally we produce the randomized cat matrix:
 ```
 cat_rand = swp.randomize_matrix(cat_symm)
 ```
-![Cat matrices](img/cat.png "Cat matrices")
+![Cat matrices](https://github.com/rkdan/small_world_propensity/blob/main/img/cat.png?raw=True)
 
 ## Comparison of $\phi$ in real networks
 We can take the networks used in _Muldoon et al_ and plot $\phi$, $\Delta_L$, $\Delta_C$, and $\delta$. Note that these networks are not the exact same as the ones used in _Muldoon et al_, and due to differences in how Numpy performs permutations, and the use of NetworkX and iGraph libraries, the results are not identical, but still match closely.
 
 The adjacency matrices:
-![Adjacency matrices](img/matrices.png "Adjacency matrices")
+![Adjacency matrices](https://github.com/rkdan/small_world_propensity/blob/main/img/matrices.png?raw=True)
 
 And the results:
-![Summary](img/summary.png "Summary")
+![Summary](https://github.com/rkdan/small_world_propensity/blob/main/img/summary.png?raw=True)
+
```

### Comparing `small_world_propensity-0.0.0/pyproject.toml` & `small_world_propensity-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "small-world-propensity"
-version = "0.0.0"
+version = "0.0.2"
 description = "A package designed to calculate the small-world propensity of a weighted, undirected network. Translated from the MATLAB version featured in Muldoon et al."
 authors = ["Ryan Daniels"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [{include = "small_world_propensity"}]
 
 [tool.poetry.dependencies]
```

### Comparing `small_world_propensity-0.0.0/small_world_propensity/small_world_propensity.py` & `small_world_propensity-0.0.2/small_world_propensity/small_world_propensity.py`

 * *Files identical despite different names*

### Comparing `small_world_propensity-0.0.0/PKG-INFO` & `small_world_propensity-0.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,18 @@
-Metadata-Version: 2.1
-Name: small-world-propensity
-Version: 0.0.0
-Summary: A package designed to calculate the small-world propensity of a weighted, undirected network. Translated from the MATLAB version featured in Muldoon et al.
-License: GPL-3.0-only
-Author: Ryan Daniels
-Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: networkx (>=3.1,<4.0)
-Requires-Dist: numpy (>=1.24.3,<2.0.0)
-Requires-Dist: pandas (>=2.0.2,<3.0.0)
-Requires-Dist: python-igraph (>=0.10.4,<0.11.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Description-Content-Type: text/markdown
-
 # Small World Propensity
 
 This python package was adapted from the MATLAB package as first presented in [Small-World Propensity and Weighted Brain Networks](https://www.nature.com/articles/srep22057) (2016) by Sarah Feldt Muldoon, Eric W. Bridgeford & Danielle S. Bassett. Their original MATLAB implementation can be found [here](https://kk1995.github.io/BauerLab/BauerLab/MATLAB/lib/+mouse/+graph/smallWorldPropensity.html).
 
 ## Use
 The small-world propensity package can be installed using pip
 ```
 python -m pip install small-world-propensity
 ```
 `small_world_propensity` can be called in two ways: either with a single adjacency matrix, or with a list of adjacency matrices and a boolean list denoting whether each matrix is binary or not. In either case, `small_world_propensity` will return a `pandas` dataframe similar to the following:
-![Dataframe](img/dataframe.png "Dataframe")
+![Dataframe](https://github.com/rkdan/small_world_propensity/blob/main/img/dataframe.png?raw=True)
 
 ## Generation of regular and random matrices
 Using the structural network of the cat cortex obtained from tract-tracing studies between 52 brain regions, we can visualize the process behind the calculation of $\phi$. The matrix is loaded using
 
 ```
 cat = sio.loadmat('data/cat.mat')['CIJctx']
 ```
@@ -43,18 +25,17 @@
 r = swp.get_avg_rad_eff(symm_cat)
 cat_reg = swp.regular_matrix_generator(symm_cat, r)
 ```
 Finally we produce the randomized cat matrix:
 ```
 cat_rand = swp.randomize_matrix(cat_symm)
 ```
-![Cat matrices](img/cat.png "Cat matrices")
+![Cat matrices](https://github.com/rkdan/small_world_propensity/blob/main/img/cat.png?raw=True)
 
 ## Comparison of $\phi$ in real networks
 We can take the networks used in _Muldoon et al_ and plot $\phi$, $\Delta_L$, $\Delta_C$, and $\delta$. Note that these networks are not the exact same as the ones used in _Muldoon et al_, and due to differences in how Numpy performs permutations, and the use of NetworkX and iGraph libraries, the results are not identical, but still match closely.
 
 The adjacency matrices:
-![Adjacency matrices](img/matrices.png "Adjacency matrices")
+![Adjacency matrices](https://github.com/rkdan/small_world_propensity/blob/main/img/matrices.png?raw=True)
 
 And the results:
-![Summary](img/summary.png "Summary")
-
+![Summary](https://github.com/rkdan/small_world_propensity/blob/main/img/summary.png?raw=True)
```

