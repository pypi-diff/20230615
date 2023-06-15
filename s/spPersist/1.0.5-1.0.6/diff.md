# Comparing `tmp/spPersist-1.0.5.tar.gz` & `tmp/spPersist-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spPersist-1.0.5.tar", last modified: Thu Jun 15 04:15:04 2023, max compression
+gzip compressed data, was "spPersist-1.0.6.tar", last modified: Thu Jun 15 05:26:04 2023, max compression
```

## Comparing `spPersist-1.0.5.tar` & `spPersist-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:15:04.160978 spPersist-1.0.5/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-06-15 04:00:09.000000 spPersist-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-15 04:15:04.160978 spPersist-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1207 2023-06-15 04:00:09.000000 spPersist-1.0.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 04:15:04.160978 spPersist-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8134 2023-06-15 04:14:41.000000 spPersist-1.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:15:04.156977 spPersist-1.0.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:15:04.158978 spPersist-1.0.5/src/spPersist/
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-15 03:59:24.000000 spPersist-1.0.5/src/spPersist/DTM_filtrations.py
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-15 03:59:24.000000 spPersist-1.0.5/src/spPersist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9595 2023-06-15 04:14:16.000000 spPersist-1.0.5/src/spPersist/dp.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-06-15 03:59:24.000000 spPersist-1.0.5/src/spPersist/hc.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-06-15 03:59:24.000000 spPersist-1.0.5/src/spPersist/persistence_statistics.py
--rw-r--r--   0 root         (0) root         (0)     4454 2023-06-15 03:59:24.000000 spPersist-1.0.5/src/spPersist/ph.py
--rw-r--r--   0 root         (0) root         (0)     6690 2023-06-15 03:59:24.000000 spPersist-1.0.5/src/spPersist/pp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:15:04.160978 spPersist-1.0.5/src/spPersist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-15 04:15:04.000000 spPersist-1.0.5/src/spPersist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-06-15 04:15:04.000000 spPersist-1.0.5/src/spPersist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 04:15:04.000000 spPersist-1.0.5/src/spPersist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-15 04:15:04.000000 spPersist-1.0.5/src/spPersist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-15 04:15:04.000000 spPersist-1.0.5/src/spPersist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 05:26:04.774878 spPersist-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-15 05:25:44.000000 spPersist-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-15 05:26:04.773878 spPersist-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-06-15 05:25:44.000000 spPersist-1.0.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 05:26:04.774878 spPersist-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8134 2023-06-15 05:25:44.000000 spPersist-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 05:26:04.768877 spPersist-1.0.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 05:26:04.771878 spPersist-1.0.6/src/spPersist/
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-15 05:23:44.000000 spPersist-1.0.6/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-15 05:23:42.000000 spPersist-1.0.6/src/spPersist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9595 2023-06-15 05:23:42.000000 spPersist-1.0.6/src/spPersist/dp.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-15 05:23:42.000000 spPersist-1.0.6/src/spPersist/hc.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-06-15 05:23:43.000000 spPersist-1.0.6/src/spPersist/persistence_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2023-06-15 05:23:42.000000 spPersist-1.0.6/src/spPersist/ph.py
+-rw-r--r--   0 root         (0) root         (0)     6742 2023-06-15 05:25:11.000000 spPersist-1.0.6/src/spPersist/pp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 05:26:04.773878 spPersist-1.0.6/src/spPersist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-15 05:26:04.000000 spPersist-1.0.6/src/spPersist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-15 05:26:04.000000 spPersist-1.0.6/src/spPersist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 05:26:04.000000 spPersist-1.0.6/src/spPersist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-15 05:26:04.000000 spPersist-1.0.6/src/spPersist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-15 05:26:04.000000 spPersist-1.0.6/src/spPersist.egg-info/top_level.txt
```

### Comparing `spPersist-1.0.5/LICENSE` & `spPersist-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.5/PKG-INFO` & `spPersist-1.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 1.0.5
+Version: 1.0.6
 Summary: Spatial transcriptomics with Persistent Homology
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spPersist-1.0.5/README.md` & `spPersist-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.5/setup.py` & `spPersist-1.0.6/setup.py`

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
-    version="1.0.5",  # Required
+    version="1.0.6",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Spatial transcriptomics with Persistent Homology",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `spPersist-1.0.5/src/spPersist/DTM_filtrations.py` & `spPersist-1.0.6/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.5/src/spPersist/dp.py` & `spPersist-1.0.6/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.5/src/spPersist/hc.py` & `spPersist-1.0.6/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.5/src/spPersist/persistence_statistics.py` & `spPersist-1.0.6/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.5/src/spPersist/ph.py` & `spPersist-1.0.6/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.5/src/spPersist/pp.py` & `spPersist-1.0.6/src/spPersist/pp.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,15 @@
     int(p)
   except:
     p = None
     print('Empty entry or the parameter is invalid.')
   else:
     p = int(p)
     adata = adata[adata.obs["pct_counts_mt"] < p]
+    print(f"#cells after MT filter: {adata.n_obs}")
 
 
 
 def extract_reference_data(adata_ref):
   '''
   extract_reference_data takes a single-cell reference data adata_ref
   as annotated data object, and returns the estimated reference expression
```

### Comparing `spPersist-1.0.5/src/spPersist.egg-info/PKG-INFO` & `spPersist-1.0.6/src/spPersist.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 1.0.5
+Version: 1.0.6
 Summary: Spatial transcriptomics with Persistent Homology
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

