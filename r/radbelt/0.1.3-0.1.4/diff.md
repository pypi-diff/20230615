# Comparing `tmp/radbelt-0.1.3.tar.gz` & `tmp/radbelt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radbelt-0.1.3.tar", last modified: Mon May  1 14:02:38 2023, max compression
+gzip compressed data, was "radbelt-0.1.4.tar", last modified: Thu Jun 15 02:48:05 2023, max compression
```

## Comparing `radbelt-0.1.3.tar` & `radbelt-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:02:38.213750 radbelt-0.1.3/
--rw-r--r--   0 root         (0) root         (0)    12693 2023-05-01 14:02:23.000000 radbelt-0.1.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     3380 2023-05-01 14:02:38.213750 radbelt-0.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2606 2023-05-01 14:02:23.000000 radbelt-0.1.3/README.md
--rw-r--r--   0 root         (0) root         (0)     1485 2023-05-01 14:02:23.000000 radbelt-0.1.3/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:02:38.213750 radbelt-0.1.3/radbelt/
--rw-r--r--   0 root         (0) root         (0)     2590 2023-05-01 14:02:23.000000 radbelt-0.1.3/radbelt/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-01 14:02:38.000000 radbelt-0.1.3/radbelt/_version.py
--rw-r--r--   0 root         (0) root         (0)     1849 2023-05-01 14:02:23.000000 radbelt-0.1.3/radbelt/core.f
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:02:38.209750 radbelt-0.1.3/radbelt/extern/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:02:38.213750 radbelt-0.1.3/radbelt/extern/aep8/
--rw-r--r--   0 root         (0) root         (0)    14732 2023-05-01 14:02:23.000000 radbelt-0.1.3/radbelt/extern/aep8/trmfun.f
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:02:38.213750 radbelt-0.1.3/radbelt/extern/igrf/
--rw-r--r--   0 root         (0) root         (0)    43035 2023-05-01 14:02:23.000000 radbelt-0.1.3/radbelt/extern/igrf/shellig.f
--rw-r--r--   0 root         (0) root         (0)      611 2023-05-01 14:02:23.000000 radbelt-0.1.3/radbelt/paths.py
--rw-r--r--   0 root         (0) root         (0)      493 2023-05-01 14:02:23.000000 radbelt-0.1.3/radbelt/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:02:38.213750 radbelt-0.1.3/radbelt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3380 2023-05-01 14:02:38.000000 radbelt-0.1.3/radbelt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      346 2023-05-01 14:02:38.000000 radbelt-0.1.3/radbelt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 14:02:38.000000 radbelt-0.1.3/radbelt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-01 14:02:38.000000 radbelt-0.1.3/radbelt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-01 14:02:38.000000 radbelt-0.1.3/radbelt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 14:02:38.213750 radbelt-0.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      322 2023-05-01 14:02:23.000000 radbelt-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 02:48:05.139757 radbelt-0.1.4/
+-rw-r--r--   0 root         (0) root         (0)    12693 2023-06-15 02:47:52.000000 radbelt-0.1.4/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     3431 2023-06-15 02:48:05.139757 radbelt-0.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2606 2023-06-15 02:47:52.000000 radbelt-0.1.4/README.md
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-15 02:47:52.000000 radbelt-0.1.4/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 02:48:05.135757 radbelt-0.1.4/radbelt/
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/core.f
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 02:48:05.135757 radbelt-0.1.4/radbelt/extern/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 02:48:05.135757 radbelt-0.1.4/radbelt/extern/aep8/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/aep8/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    83596 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/aep8/ae8max.asc
+-rw-r--r--   0 root         (0) root         (0)    81254 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/aep8/ae8min.asc
+-rw-r--r--   0 root         (0) root         (0)   100542 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/aep8/ap8max.asc
+-rw-r--r--   0 root         (0) root         (0)   102318 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/aep8/ap8min.asc
+-rw-r--r--   0 root         (0) root         (0)    14732 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/aep8/trmfun.f
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 02:48:05.139757 radbelt-0.1.4/radbelt/extern/igrf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1945.dat
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1950.dat
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1955.dat
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1960.dat
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1965.dat
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1970.dat
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1975.dat
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1980.dat
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1985.dat
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1990.dat
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1995.dat
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf2000.dat
+-rw-r--r--   0 root         (0) root         (0)     1785 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf2005.dat
+-rw-r--r--   0 root         (0) root         (0)     1785 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf2010.dat
+-rw-r--r--   0 root         (0) root         (0)     1785 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf2015.dat
+-rw-r--r--   0 root         (0) root         (0)     1785 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/igrf2020.dat
+-rw-r--r--   0 root         (0) root         (0)     1786 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/igrf2020s.dat
+-rw-r--r--   0 root         (0) root         (0)    43035 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/shellig.f
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 02:48:05.135757 radbelt-0.1.4/radbelt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3431 2023-06-15 02:48:05.000000 radbelt-0.1.4/radbelt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-06-15 02:48:05.000000 radbelt-0.1.4/radbelt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 02:48:05.000000 radbelt-0.1.4/radbelt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-15 02:48:05.000000 radbelt-0.1.4/radbelt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-15 02:48:05.000000 radbelt-0.1.4/radbelt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 02:48:05.139757 radbelt-0.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      322 2023-06-15 02:47:52.000000 radbelt-0.1.4/setup.py
```

### Comparing `radbelt-0.1.3/LICENSE.txt` & `radbelt-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.3/PKG-INFO` & `radbelt-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: radbelt
-Version: 0.1.3
+Version: 0.1.4
 Summary: Astropy-friendly wrapper for the AE-8/AP-8 Van Allen belt model
 Author-email: Leo Singer <leo.p.singer@nasa.gov>
 License: NOSA
 Project-URL: source, https://github.com/nasa/radbelt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # radbelt: An Astropy-friendly wrapper for the AE-8/AP-8 Van Allen belt model
```

### Comparing `radbelt-0.1.3/README.md` & `radbelt-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.3/pyproject.toml` & `radbelt-0.1.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -17,26 +17,27 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Astronomy"
 ]
 license = { text = "NOSA" }
 requires-python = ">=3.7"
 dependencies = ["astropy", "numpy"]
 dynamic = [ "version" ]
 
 [project.urls]
 source = "https://github.com/nasa/radbelt"
 
 [tool.setuptools.packages.find]
-include = ["radbelt"]
+include = ["radbelt.*"]
 
 [tool.setuptools.package-data]
 "radbelt.extern.igrf" = ["*.dat"]
 "radbelt.extern.aep8" = ["*.asc"]
 
 [tool.setuptools_scm]
 write_to = "radbelt/_version.py"
```

### Comparing `radbelt-0.1.3/radbelt/core.f` & `radbelt-0.1.4/radbelt/core.f`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.3/radbelt/extern/aep8/trmfun.f` & `radbelt-0.1.4/radbelt/extern/aep8/trmfun.f`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.3/radbelt/extern/igrf/shellig.f` & `radbelt-0.1.4/radbelt/extern/igrf/shellig.f`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.3/radbelt.egg-info/PKG-INFO` & `radbelt-0.1.4/radbelt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: radbelt
-Version: 0.1.3
+Version: 0.1.4
 Summary: Astropy-friendly wrapper for the AE-8/AP-8 Van Allen belt model
 Author-email: Leo Singer <leo.p.singer@nasa.gov>
 License: NOSA
 Project-URL: source, https://github.com/nasa/radbelt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # radbelt: An Astropy-friendly wrapper for the AE-8/AP-8 Van Allen belt model
```

