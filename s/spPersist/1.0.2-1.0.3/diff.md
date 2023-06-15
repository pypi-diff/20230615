# Comparing `tmp/spPersist-1.0.2.tar.gz` & `tmp/spPersist-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spPersist-1.0.2.tar", last modified: Mon Jun 12 07:25:18 2023, max compression
+gzip compressed data, was "spPersist-1.0.3.tar", last modified: Thu Jun 15 04:00:34 2023, max compression
```

## Comparing `spPersist-1.0.2.tar` & `spPersist-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:25:18.345485 spPersist-1.0.2/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-06-12 06:52:13.000000 spPersist-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 07:25:18.339484 spPersist-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1207 2023-06-12 06:52:13.000000 spPersist-1.0.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 07:25:18.345485 spPersist-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8134 2023-06-12 07:24:24.000000 spPersist-1.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:25:18.333484 spPersist-1.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:25:18.338484 spPersist-1.0.2/src/spPersist/
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-12 06:49:31.000000 spPersist-1.0.2/src/spPersist/DTM_filtrations.py
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-12 06:49:31.000000 spPersist-1.0.2/src/spPersist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9403 2023-06-12 06:49:31.000000 spPersist-1.0.2/src/spPersist/dp.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-06-12 06:49:31.000000 spPersist-1.0.2/src/spPersist/hc.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-06-12 06:49:31.000000 spPersist-1.0.2/src/spPersist/persistence_statistics.py
--rw-r--r--   0 root         (0) root         (0)     4454 2023-06-12 06:49:31.000000 spPersist-1.0.2/src/spPersist/ph.py
--rw-r--r--   0 root         (0) root         (0)     6375 2023-06-12 07:24:05.000000 spPersist-1.0.2/src/spPersist/pp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:25:18.339484 spPersist-1.0.2/src/spPersist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 07:25:18.000000 spPersist-1.0.2/src/spPersist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-06-12 07:25:18.000000 spPersist-1.0.2/src/spPersist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 07:25:18.000000 spPersist-1.0.2/src/spPersist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-12 07:25:18.000000 spPersist-1.0.2/src/spPersist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 07:25:18.000000 spPersist-1.0.2/src/spPersist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:34.956160 spPersist-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-15 04:00:09.000000 spPersist-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-15 04:00:34.956160 spPersist-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-06-15 04:00:09.000000 spPersist-1.0.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 04:00:34.957160 spPersist-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8134 2023-06-15 04:00:09.000000 spPersist-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:34.943159 spPersist-1.0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:34.953159 spPersist-1.0.3/src/spPersist/
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-15 03:59:24.000000 spPersist-1.0.3/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-15 03:59:24.000000 spPersist-1.0.3/src/spPersist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9480 2023-06-15 03:59:24.000000 spPersist-1.0.3/src/spPersist/dp.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-15 03:59:24.000000 spPersist-1.0.3/src/spPersist/hc.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-06-15 03:59:24.000000 spPersist-1.0.3/src/spPersist/persistence_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2023-06-15 03:59:24.000000 spPersist-1.0.3/src/spPersist/ph.py
+-rw-r--r--   0 root         (0) root         (0)     6690 2023-06-15 03:59:24.000000 spPersist-1.0.3/src/spPersist/pp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:34.956160 spPersist-1.0.3/src/spPersist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-15 04:00:34.000000 spPersist-1.0.3/src/spPersist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-15 04:00:34.000000 spPersist-1.0.3/src/spPersist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 04:00:34.000000 spPersist-1.0.3/src/spPersist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-15 04:00:34.000000 spPersist-1.0.3/src/spPersist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-15 04:00:34.000000 spPersist-1.0.3/src/spPersist.egg-info/top_level.txt
```

### Comparing `spPersist-1.0.2/LICENSE` & `spPersist-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.2/PKG-INFO` & `spPersist-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 1.0.2
+Version: 1.0.3
 Summary: Spatial transcriptomics with Persistent Homology
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spPersist-1.0.2/README.md` & `spPersist-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.2/setup.py` & `spPersist-1.0.3/setup.py`

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
-    version="1.0.2",  # Required
+    version="1.0.3",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Spatial transcriptomics with Persistent Homology",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `spPersist-1.0.2/src/spPersist/DTM_filtrations.py` & `spPersist-1.0.3/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.2/src/spPersist/dp.py` & `spPersist-1.0.3/src/spPersist/dp.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,18 @@
   url_pos = 'https://cf.10xgenomics.com/samples/spatial-exp/1.3.0/Visium_FFPE_Mouse_Brain/Visium_FFPE_Mouse_Brain_spatial.tar.gz'
   open(gex, 'wb').write(requests.get(url_gex).content)
   open('spatial.tar','wb').write(requests.get(url_pos).content)
 
   tar = tarfile.open('spatial.tar')
   posfile = tar.getmembers()[1] # 1 is the index of the coordinate file.
   tar.extract(posfile)
+
+  shutil.rmtree('spatial/')
+  os.remove(gex)
+  os.remove('spatial.tar')
   return visium(gex, posfile.name)
 
 
 def V1_Adult_Mouse_Brain():
   '''
   Returns annotated data object of the Mouse Brain Section (Coronal) dataset
   from Visium, 10x Genomics.
```

### Comparing `spPersist-1.0.2/src/spPersist/hc.py` & `spPersist-1.0.3/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.2/src/spPersist/persistence_statistics.py` & `spPersist-1.0.3/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.2/src/spPersist/ph.py` & `spPersist-1.0.3/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.2/src/spPersist/pp.py` & `spPersist-1.0.3/src/spPersist/pp.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   prompts the user to enter quality control parameters,
   and filters the expression matrix.
   '''
   
   # setting scanpy verbosity for filtering notice
   sc.settings.verbosity = 3
 
-  print('Filtering cells...\nPress Enter to skip the parameter.')
+  print('Filtering cells...\nPress Enter to skip a parameter.')
   p = input('Enter min_counts:')
   print('min_counts: ' + p)
   try:
     int(p)
   except:
     p = None
     print('Empty entry or the parameter is invalid.')
@@ -63,15 +63,15 @@
   except:
     p = None
     print('Empty entry or the parameter is invalid.')
   else:
     p = int(p)
     sc.pp.filter_cells(adata, max_genes=p)
 
-  print('Filtering genes...\nPress Enter to skip the parameter.')
+  print('Filtering genes...\nPress Enter to skip a parameter.')
   p = input('Enter min_counts:')
   print('min_counts: ' + p)
   try:
     int(p)
   except:
     p = None
     print('Empty entry or the parameter is invalid.')
@@ -108,14 +108,27 @@
   except:
     p = None
     print('Empty entry or the parameter is invalid.')
   else:
     p = int(p)
     sc.pp.filter_genes(adata, max_cells=p)
 
+  print('Mitochondrial filtering...\nPress Enter to skip the parameter.')
+  p = input('Enter min_pct_counts_mt:')
+  print('min_pct_counts_mt: ' + p)
+  try:
+    int(p)
+  except:
+    p = None
+    print('Empty entry or the parameter is invalid.')
+  else:
+    p = int(p)
+    adata = adata[adata.obs["pct_counts_mt"] < p]
+
+
 
 def extract_reference_data(adata_ref):
   '''
   extract_reference_data takes a single-cell reference data adata_ref
   as annotated data object, and returns the estimated reference expression
   as a pandas dataframe.
   '''
```

### Comparing `spPersist-1.0.2/src/spPersist.egg-info/PKG-INFO` & `spPersist-1.0.3/src/spPersist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 1.0.2
+Version: 1.0.3
 Summary: Spatial transcriptomics with Persistent Homology
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

