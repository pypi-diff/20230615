# Comparing `tmp/sppersist-1.0.7.tar.gz` & `tmp/spPersist-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "spPersist-1.0.8.tar", last modified: Thu Jun 15 13:35:37 2023, max compression
```

## Comparing `sppersist-1.0.7.tar` & `spPersist-1.0.8.tar`

### file list

```diff
@@ -1,12 +1,21 @@
--rw-r--r--   0        0        0     8134 2020-02-02 00:00:00.000000 sppersist-1.0.7/setup.py
--rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-1.0.7/src/spPersist/DTM_filtrations.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sppersist-1.0.7/src/spPersist/__init__.py
--rw-r--r--   0        0        0     9595 2020-02-02 00:00:00.000000 sppersist-1.0.7/src/spPersist/dp.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sppersist-1.0.7/src/spPersist/hc.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-1.0.7/src/spPersist/persistence_statistics.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sppersist-1.0.7/src/spPersist/ph.py
--rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 sppersist-1.0.7/src/spPersist/pp.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-1.0.7/LICENSE
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sppersist-1.0.7/README.md
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 sppersist-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 sppersist-1.0.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:35:37.654169 spPersist-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-15 13:35:17.000000 spPersist-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-15 13:35:37.654169 spPersist-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-06-15 13:35:17.000000 spPersist-1.0.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 13:35:37.654169 spPersist-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8133 2023-06-15 13:35:17.000000 spPersist-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:35:37.650169 spPersist-1.0.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:35:37.652169 spPersist-1.0.8/src/spPersist/
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-15 13:32:56.000000 spPersist-1.0.8/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-15 13:32:56.000000 spPersist-1.0.8/src/spPersist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9595 2023-06-15 13:32:56.000000 spPersist-1.0.8/src/spPersist/dp.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-15 13:32:56.000000 spPersist-1.0.8/src/spPersist/hc.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-06-15 13:32:56.000000 spPersist-1.0.8/src/spPersist/persistence_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2023-06-15 13:32:56.000000 spPersist-1.0.8/src/spPersist/ph.py
+-rw-r--r--   0 root         (0) root         (0)     6742 2023-06-15 13:32:56.000000 spPersist-1.0.8/src/spPersist/pp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:35:37.654169 spPersist-1.0.8/src/spPersist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-15 13:35:37.000000 spPersist-1.0.8/src/spPersist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-15 13:35:37.000000 spPersist-1.0.8/src/spPersist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 13:35:37.000000 spPersist-1.0.8/src/spPersist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-15 13:35:37.000000 spPersist-1.0.8/src/spPersist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-15 13:35:37.000000 spPersist-1.0.8/src/spPersist.egg-info/top_level.txt
```

### Comparing `sppersist-1.0.7/setup.py` & `spPersist-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="spPersist",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="1.0.7",  # Required
+    version="1.0.8",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Spatial transcriptomics with Persistent Homology",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
@@ -125,15 +125,15 @@
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/discussions/install-requires-vs-requirements/
     install_requires=[
       'gcsfs', 
-      'squidpy',
+      'scanpy',
       'cell2location',
       'gudhi'
       ],  # Optional
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
```

### Comparing `sppersist-1.0.7/src/spPersist/DTM_filtrations.py` & `spPersist-1.0.8/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.0.7/src/spPersist/dp.py` & `spPersist-1.0.8/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.0.7/src/spPersist/hc.py` & `spPersist-1.0.8/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.0.7/src/spPersist/persistence_statistics.py` & `spPersist-1.0.8/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.0.7/src/spPersist/ph.py` & `spPersist-1.0.8/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.0.7/src/spPersist/pp.py` & `spPersist-1.0.8/src/spPersist/pp.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.0.7/LICENSE` & `spPersist-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-1.0.7/README.md` & `spPersist-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `sppersist-1.0.7/PKG-INFO` & `spPersist-1.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 1.0.7
+Version: 1.0.8
 Summary: Spatial transcriptomics with Persistent Homology
-Author-email: Lirong Yang <lirong.yang@outlook.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
+Author: Lirong Yang
+Author-email: lirong.yang@outlook.com
 Requires-Python: >=3.7
-Requires-Dist: cell2location
-Requires-Dist: gcsfs
-Requires-Dist: gudhi
-Requires-Dist: squidpy
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Spatial transcriptomics with Persistent Homology
 
 This is a package for classifying Spatial transcriptomics data according to its 
 spatial topology. The specific mathematical foundation for the classification is
 the theory of Persistent Homology and persistence diagram. The package 
 contains a data processing module, called dp, allowing users to load either the
@@ -33,8 +27,8 @@
 
 The persistent homology module contains functions for computing simplicial 
 complexes of point clouds (See data structures in the gudhi package.) and their
 topological measures. It also includes plotting features of the persistence 
 diagram.
 
 The homological classification module computes the number of holes and connected
-components as a dictionary.
+components as a dictionary.
```

