# Comparing `tmp/spPersist-1.0.3.tar.gz` & `tmp/spPersist-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spPersist-1.0.3.tar", last modified: Thu Jun 15 04:00:34 2023, max compression
+gzip compressed data, was "spPersist-1.0.4.tar", last modified: Thu Jun 15 04:06:28 2023, max compression
```

## Comparing `spPersist-1.0.3.tar` & `spPersist-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:34.956160 spPersist-1.0.3/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-06-15 04:00:09.000000 spPersist-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-15 04:00:34.956160 spPersist-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1207 2023-06-15 04:00:09.000000 spPersist-1.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 04:00:34.957160 spPersist-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8134 2023-06-15 04:00:09.000000 spPersist-1.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:34.943159 spPersist-1.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:34.953159 spPersist-1.0.3/src/spPersist/
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-15 03:59:24.000000 spPersist-1.0.3/src/spPersist/DTM_filtrations.py
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-15 03:59:24.000000 spPersist-1.0.3/src/spPersist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9480 2023-06-15 03:59:24.000000 spPersist-1.0.3/src/spPersist/dp.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-06-15 03:59:24.000000 spPersist-1.0.3/src/spPersist/hc.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-06-15 03:59:24.000000 spPersist-1.0.3/src/spPersist/persistence_statistics.py
--rw-r--r--   0 root         (0) root         (0)     4454 2023-06-15 03:59:24.000000 spPersist-1.0.3/src/spPersist/ph.py
--rw-r--r--   0 root         (0) root         (0)     6690 2023-06-15 03:59:24.000000 spPersist-1.0.3/src/spPersist/pp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:34.956160 spPersist-1.0.3/src/spPersist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-15 04:00:34.000000 spPersist-1.0.3/src/spPersist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-06-15 04:00:34.000000 spPersist-1.0.3/src/spPersist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 04:00:34.000000 spPersist-1.0.3/src/spPersist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-15 04:00:34.000000 spPersist-1.0.3/src/spPersist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-15 04:00:34.000000 spPersist-1.0.3/src/spPersist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:06:28.780628 spPersist-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-15 04:00:09.000000 spPersist-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-15 04:06:28.779628 spPersist-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-06-15 04:00:09.000000 spPersist-1.0.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 04:06:28.780628 spPersist-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8134 2023-06-15 04:06:02.000000 spPersist-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:06:28.776628 spPersist-1.0.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:06:28.778628 spPersist-1.0.4/src/spPersist/
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-15 03:59:24.000000 spPersist-1.0.4/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-15 03:59:24.000000 spPersist-1.0.4/src/spPersist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9557 2023-06-15 04:05:03.000000 spPersist-1.0.4/src/spPersist/dp.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-15 03:59:24.000000 spPersist-1.0.4/src/spPersist/hc.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-06-15 03:59:24.000000 spPersist-1.0.4/src/spPersist/persistence_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2023-06-15 03:59:24.000000 spPersist-1.0.4/src/spPersist/ph.py
+-rw-r--r--   0 root         (0) root         (0)     6690 2023-06-15 03:59:24.000000 spPersist-1.0.4/src/spPersist/pp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:06:28.779628 spPersist-1.0.4/src/spPersist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-15 04:06:28.000000 spPersist-1.0.4/src/spPersist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-15 04:06:28.000000 spPersist-1.0.4/src/spPersist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 04:06:28.000000 spPersist-1.0.4/src/spPersist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-15 04:06:28.000000 spPersist-1.0.4/src/spPersist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-15 04:06:28.000000 spPersist-1.0.4/src/spPersist.egg-info/top_level.txt
```

### Comparing `spPersist-1.0.3/LICENSE` & `spPersist-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.3/PKG-INFO` & `spPersist-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 1.0.3
+Version: 1.0.4
 Summary: Spatial transcriptomics with Persistent Homology
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spPersist-1.0.3/README.md` & `spPersist-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.3/setup.py` & `spPersist-1.0.4/setup.py`

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
-    version="1.0.3",  # Required
+    version="1.0.4",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Spatial transcriptomics with Persistent Homology",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `spPersist-1.0.3/src/spPersist/DTM_filtrations.py` & `spPersist-1.0.4/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.3/src/spPersist/dp.py` & `spPersist-1.0.4/src/spPersist/dp.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,18 @@
   url_pos = 'https://cf.10xgenomics.com/samples/spatial-exp/1.0.0/V1_Adult_Mouse_Brain/V1_Adult_Mouse_Brain_spatial.tar.gz'
   open(gex, 'wb').write(requests.get(url_gex).content)
   open('spatial.tar','wb').write(requests.get(url_pos).content)
 
   tar = tarfile.open('spatial.tar')
   posfile = tar.getmembers()[3] # 3 is the index of the coordinate file.
   tar.extract(posfile)
+
+  shutil.rmtree('spatial/')
+  os.remove(gex)
+  os.remove('spatial.tar')
   return visium(gex, posfile.name)
 
 
 def Vizgen_V1_S2R1():
   '''
   Returns annotated data object of Slice 2 Replicate 1
   of the MERFISH Mouse Brain Receptor Map datasets from
```

### Comparing `spPersist-1.0.3/src/spPersist/hc.py` & `spPersist-1.0.4/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.3/src/spPersist/persistence_statistics.py` & `spPersist-1.0.4/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.3/src/spPersist/ph.py` & `spPersist-1.0.4/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.3/src/spPersist/pp.py` & `spPersist-1.0.4/src/spPersist/pp.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.3/src/spPersist.egg-info/PKG-INFO` & `spPersist-1.0.4/src/spPersist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 1.0.3
+Version: 1.0.4
 Summary: Spatial transcriptomics with Persistent Homology
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

