# Comparing `tmp/connected-components-3d-3.9.0.tar.gz` & `tmp/connected-components-3d-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connected-components-3d-3.9.0.tar", last modified: Sat Feb 19 00:40:44 2022, max compression
+gzip compressed data, was "connected-components-3d-3.9.1.tar", last modified: Sun Feb 20 22:48:33 2022, max compression
```

## Comparing `connected-components-3d-3.9.0.tar` & `connected-components-3d-3.9.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-02-19 00:40:44.648984 connected-components-3d-3.9.0/
--rw-r--r--   0 wms        (501) staff       (20)       95 2021-11-22 05:57:44.000000 connected-components-3d-3.9.0/.dockerignore
--rw-r--r--   0 wms        (501) staff       (20)       90 2021-11-22 05:55:59.000000 connected-components-3d-3.9.0/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)     7346 2021-11-22 05:57:44.000000 connected-components-3d-3.9.0/ChangeLog
--rw-r--r--   0 wms        (501) staff       (20)    35147 2021-01-06 03:55:10.000000 connected-components-3d-3.9.0/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)       85 2021-11-22 22:28:03.000000 connected-components-3d-3.9.0/MANIFEST.in
--rw-r--r--   0 wms        (501) staff       (20)      223 2021-11-22 05:57:44.000000 connected-components-3d-3.9.0/Makefile
--rw-r--r--   0 wms        (501) staff       (20)    31833 2022-02-19 00:40:44.648800 connected-components-3d-3.9.0/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)    27289 2022-02-18 23:31:56.000000 connected-components-3d-3.9.0/README.md
--rw-r--r--   0 wms        (501) staff       (20)     1319 2021-12-22 17:11:28.000000 connected-components-3d-3.9.0/appveyor.yml
--rw-r--r--   0 wms        (501) staff       (20)    33263 2022-02-18 23:31:56.000000 connected-components-3d-3.9.0/automated_test.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-02-19 00:40:44.646617 connected-components-3d-3.9.0/benchmarks/
--rw-r--r--   0 wms        (501) staff       (20)    11607 2021-11-29 22:05:36.000000 connected-components-3d-3.9.0/benchmarks/README.md
--rw-r--r--   0 wms        (501) staff       (20)    31521 2021-11-22 05:57:44.000000 connected-components-3d-3.9.0/benchmarks/cc3d_vs_scipy_multilabel.png
--rw-r--r--   0 wms        (501) staff       (20)   229798 2021-11-22 05:57:44.000000 connected-components-3d-3.9.0/benchmarks/cc3d_vs_scipy_single_label_10x.png
--rwxr-xr-x   0 wms        (501) staff       (20)      711 2021-11-22 05:57:44.000000 connected-components-3d-3.9.0/build_linux.sh
--rw-r--r--   0 wms        (501) staff       (20)  2418625 2022-02-18 23:34:49.000000 connected-components-3d-3.9.0/cc3d.cpp
--rw-r--r--   0 wms        (501) staff       (20)    34838 2021-11-29 07:41:40.000000 connected-components-3d-3.9.0/cc3d.hpp
--rw-r--r--   0 wms        (501) staff       (20)    33843 2022-02-18 23:32:00.000000 connected-components-3d-3.9.0/cc3d.pyx
--rw-r--r--   0 wms        (501) staff       (20)    13401 2021-11-29 22:05:40.000000 connected-components-3d-3.9.0/cc3d_continuous.hpp
--rw-r--r--   0 wms        (501) staff       (20)    11894 2021-12-22 17:06:10.000000 connected-components-3d-3.9.0/cc3d_graphs.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-02-19 00:40:44.647794 connected-components-3d-3.9.0/connected_components_3d.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)    31833 2022-02-19 00:40:44.000000 connected-components-3d-3.9.0/connected_components_3d.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)      854 2022-02-19 00:40:44.000000 connected-components-3d-3.9.0/connected_components_3d.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2022-02-19 00:40:44.000000 connected-components-3d-3.9.0/connected_components_3d.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)       46 2021-09-15 21:50:16.000000 connected-components-3d-3.9.0/connected_components_3d.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)        6 2022-02-19 00:40:44.000000 connected-components-3d-3.9.0/connected_components_3d.egg-info/requires.txt
--rw-r--r--   0 wms        (501) staff       (20)        5 2022-02-19 00:40:44.000000 connected-components-3d-3.9.0/connected_components_3d.egg-info/top_level.txt
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-02-19 00:40:44.648490 connected-components-3d-3.9.0/manual_testing/
--rw-r--r--   0 wms        (501) staff       (20)      874 2021-11-22 05:57:44.000000 connected-components-3d-3.9.0/manual_testing/test.py
--rw-r--r--   0 wms        (501) staff       (20)    13974 2021-11-22 05:56:22.000000 connected-components-3d-3.9.0/manual_testing/test2d.png
--rw-r--r--   0 wms        (501) staff       (20)     7107 2021-11-22 05:56:22.000000 connected-components-3d-3.9.0/manual_testing/test3d-1.png
--rw-r--r--   0 wms        (501) staff       (20)     5316 2021-11-22 05:56:22.000000 connected-components-3d-3.9.0/manual_testing/test3d-2.png
--rw-r--r--   0 wms        (501) staff       (20)     7107 2021-11-22 05:56:22.000000 connected-components-3d-3.9.0/manual_testing/test3d-3.png
--rw-r--r--   0 wms        (501) staff       (20)     2181 2021-11-22 05:57:44.000000 connected-components-3d-3.9.0/manylinux1.Dockerfile
--rw-r--r--   0 wms        (501) staff       (20)     2213 2021-11-22 05:57:44.000000 connected-components-3d-3.9.0/manylinux2010.Dockerfile
--rw-r--r--   0 wms        (501) staff       (20)     2194 2021-11-22 05:57:44.000000 connected-components-3d-3.9.0/manylinux2014.Dockerfile
--rw-r--r--   0 wms        (501) staff       (20)     1794 2021-11-22 05:57:44.000000 connected-components-3d-3.9.0/perf.py
--rw-r--r--   0 wms        (501) staff       (20)       90 2022-02-18 23:39:18.000000 connected-components-3d-3.9.0/pyproject.toml
--rw-r--r--   0 wms        (501) staff       (20)        6 2021-11-22 05:56:22.000000 connected-components-3d-3.9.0/requirements.txt
--rw-r--r--   0 wms        (501) staff       (20)       12 2021-11-22 05:57:44.000000 connected-components-3d-3.9.0/requirements_dev.txt
--rw-r--r--   0 wms        (501) staff       (20)       38 2022-02-19 00:40:44.649034 connected-components-3d-3.9.0/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)     2365 2022-02-18 23:38:52.000000 connected-components-3d-3.9.0/setup.py
--rw-r--r--   0 wms        (501) staff       (20)     1735 2021-11-22 05:57:44.000000 connected-components-3d-3.9.0/test.cpp
--rw-r--r--   0 wms        (501) staff       (20)      211 2021-12-22 18:13:20.000000 connected-components-3d-3.9.0/tox.ini
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-02-20 22:48:33.374374 connected-components-3d-3.9.1/
+-rw-r--r--   0 wms        (501) staff       (20)       95 2021-11-22 05:57:44.000000 connected-components-3d-3.9.1/.dockerignore
+-rw-r--r--   0 wms        (501) staff       (20)       90 2021-11-22 05:55:59.000000 connected-components-3d-3.9.1/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)     7346 2021-11-22 05:57:44.000000 connected-components-3d-3.9.1/ChangeLog
+-rw-r--r--   0 wms        (501) staff       (20)    35147 2021-01-06 03:55:10.000000 connected-components-3d-3.9.1/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)       85 2021-11-22 22:28:03.000000 connected-components-3d-3.9.1/MANIFEST.in
+-rw-r--r--   0 wms        (501) staff       (20)      223 2021-11-22 05:57:44.000000 connected-components-3d-3.9.1/Makefile
+-rw-r--r--   0 wms        (501) staff       (20)    31833 2022-02-20 22:48:33.374183 connected-components-3d-3.9.1/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)    27289 2022-02-18 23:31:56.000000 connected-components-3d-3.9.1/README.md
+-rw-r--r--   0 wms        (501) staff       (20)     1319 2021-12-22 17:11:28.000000 connected-components-3d-3.9.1/appveyor.yml
+-rw-r--r--   0 wms        (501) staff       (20)    33263 2022-02-18 23:31:56.000000 connected-components-3d-3.9.1/automated_test.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-02-20 22:48:33.371075 connected-components-3d-3.9.1/benchmarks/
+-rw-r--r--   0 wms        (501) staff       (20)    11607 2021-11-29 22:05:36.000000 connected-components-3d-3.9.1/benchmarks/README.md
+-rw-r--r--   0 wms        (501) staff       (20)    31521 2021-11-22 05:57:44.000000 connected-components-3d-3.9.1/benchmarks/cc3d_vs_scipy_multilabel.png
+-rw-r--r--   0 wms        (501) staff       (20)   229798 2021-11-22 05:57:44.000000 connected-components-3d-3.9.1/benchmarks/cc3d_vs_scipy_single_label_10x.png
+-rwxr-xr-x   0 wms        (501) staff       (20)      711 2021-11-22 05:57:44.000000 connected-components-3d-3.9.1/build_linux.sh
+-rw-r--r--   0 wms        (501) staff       (20)  2413120 2022-02-20 22:41:55.000000 connected-components-3d-3.9.1/cc3d.cpp
+-rw-r--r--   0 wms        (501) staff       (20)    34838 2021-11-29 07:41:40.000000 connected-components-3d-3.9.1/cc3d.hpp
+-rw-r--r--   0 wms        (501) staff       (20)    33860 2022-02-20 22:41:55.000000 connected-components-3d-3.9.1/cc3d.pyx
+-rw-r--r--   0 wms        (501) staff       (20)    13401 2021-11-29 22:05:40.000000 connected-components-3d-3.9.1/cc3d_continuous.hpp
+-rw-r--r--   0 wms        (501) staff       (20)    11894 2021-12-22 17:06:10.000000 connected-components-3d-3.9.1/cc3d_graphs.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-02-20 22:48:33.372910 connected-components-3d-3.9.1/connected_components_3d.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)    31833 2022-02-20 22:48:33.000000 connected-components-3d-3.9.1/connected_components_3d.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)      854 2022-02-20 22:48:33.000000 connected-components-3d-3.9.1/connected_components_3d.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2022-02-20 22:48:33.000000 connected-components-3d-3.9.1/connected_components_3d.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)       46 2021-09-15 21:50:16.000000 connected-components-3d-3.9.1/connected_components_3d.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)        6 2022-02-20 22:48:33.000000 connected-components-3d-3.9.1/connected_components_3d.egg-info/requires.txt
+-rw-r--r--   0 wms        (501) staff       (20)        5 2022-02-20 22:48:33.000000 connected-components-3d-3.9.1/connected_components_3d.egg-info/top_level.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-02-20 22:48:33.373839 connected-components-3d-3.9.1/manual_testing/
+-rw-r--r--   0 wms        (501) staff       (20)      874 2021-11-22 05:57:44.000000 connected-components-3d-3.9.1/manual_testing/test.py
+-rw-r--r--   0 wms        (501) staff       (20)    13974 2021-11-22 05:56:22.000000 connected-components-3d-3.9.1/manual_testing/test2d.png
+-rw-r--r--   0 wms        (501) staff       (20)     7107 2021-11-22 05:56:22.000000 connected-components-3d-3.9.1/manual_testing/test3d-1.png
+-rw-r--r--   0 wms        (501) staff       (20)     5316 2021-11-22 05:56:22.000000 connected-components-3d-3.9.1/manual_testing/test3d-2.png
+-rw-r--r--   0 wms        (501) staff       (20)     7107 2021-11-22 05:56:22.000000 connected-components-3d-3.9.1/manual_testing/test3d-3.png
+-rw-r--r--   0 wms        (501) staff       (20)     2181 2021-11-22 05:57:44.000000 connected-components-3d-3.9.1/manylinux1.Dockerfile
+-rw-r--r--   0 wms        (501) staff       (20)     2213 2021-11-22 05:57:44.000000 connected-components-3d-3.9.1/manylinux2010.Dockerfile
+-rw-r--r--   0 wms        (501) staff       (20)     2194 2021-11-22 05:57:44.000000 connected-components-3d-3.9.1/manylinux2014.Dockerfile
+-rw-r--r--   0 wms        (501) staff       (20)     1794 2021-11-22 05:57:44.000000 connected-components-3d-3.9.1/perf.py
+-rw-r--r--   0 wms        (501) staff       (20)       90 2022-02-18 23:39:18.000000 connected-components-3d-3.9.1/pyproject.toml
+-rw-r--r--   0 wms        (501) staff       (20)        6 2021-11-22 05:56:22.000000 connected-components-3d-3.9.1/requirements.txt
+-rw-r--r--   0 wms        (501) staff       (20)       12 2021-11-22 05:57:44.000000 connected-components-3d-3.9.1/requirements_dev.txt
+-rw-r--r--   0 wms        (501) staff       (20)       38 2022-02-20 22:48:33.374424 connected-components-3d-3.9.1/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)     2365 2022-02-20 22:42:05.000000 connected-components-3d-3.9.1/setup.py
+-rw-r--r--   0 wms        (501) staff       (20)     1735 2021-11-22 05:57:44.000000 connected-components-3d-3.9.1/test.cpp
+-rw-r--r--   0 wms        (501) staff       (20)      215 2022-02-19 00:44:11.000000 connected-components-3d-3.9.1/tox.ini
```

### Comparing `connected-components-3d-3.9.0/ChangeLog` & `connected-components-3d-3.9.1/ChangeLog`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/LICENSE` & `connected-components-3d-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/PKG-INFO` & `connected-components-3d-3.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connected-components-3d
-Version: 3.9.0
+Version: 3.9.1
 Summary: Connected components on 2D and 3D images. Supports multiple labels.
 Home-page: https://github.com/seung-lab/connected-components-3d/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description: [![Build Status](https://travis-ci.org/seung-lab/connected-components-3d.svg?branch=master)](https://travis-ci.org/seung-lab/connected-components-3d) [![PyPI version](https://badge.fury.io/py/connected-components-3d.svg)](https://badge.fury.io/py/connected-components-3d) [![DOI](https://zenodo.org/badge/146368855.svg)](https://zenodo.org/badge/latestdoi/146368855)
```

### Comparing `connected-components-3d-3.9.0/README.md` & `connected-components-3d-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/appveyor.yml` & `connected-components-3d-3.9.1/appveyor.yml`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/automated_test.py` & `connected-components-3d-3.9.1/automated_test.py`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/benchmarks/README.md` & `connected-components-3d-3.9.1/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/benchmarks/cc3d_vs_scipy_multilabel.png` & `connected-components-3d-3.9.1/benchmarks/cc3d_vs_scipy_multilabel.png`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/benchmarks/cc3d_vs_scipy_single_label_10x.png` & `connected-components-3d-3.9.1/benchmarks/cc3d_vs_scipy_single_label_10x.png`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/build_linux.sh` & `connected-components-3d-3.9.1/build_linux.sh`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/cc3d.cpp` & `connected-components-3d-3.9.1/cc3d.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -649,17 +649,14 @@
     template <typename T> typename std::remove_reference<T>::type&& move(T&& t) noexcept { return std::move(t); }
     }
 
     #endif
     
 #include <map>
 #include "numpy/arrayobject.h"
-#include "numpy/ndarrayobject.h"
-#include "numpy/ndarraytypes.h"
-#include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
 
     /* NumPy API declarations from "numpy/__init__.pxd" */
     
 #include "cc3d.hpp"
 #include "cc3d_continuous.hpp"
 #include "cc3d_graphs.hpp"
@@ -1007,195 +1004,195 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":690
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":691
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":692
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":693
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":697
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":698
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":699
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":700
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":704
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":705
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":714
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":715
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":716
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":718
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":719
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":720
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":722
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":723
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":725
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":726
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":727
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1233,42 +1230,42 @@
 struct __pyx_obj_4cc3d___pyx_scope_struct_1___iter__;
 struct __pyx_obj_4cc3d___pyx_scope_struct_2___iter__;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":729
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":730
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":731
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":733
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2979,24 +2976,14 @@
 /* Module declarations from 'numpy' */
 
 /* Module declarations from 'numpy' */
 static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
 static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
-static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
-static PyTypeObject *__pyx_ptype_5numpy_number = 0;
-static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
-static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
-static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
-static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
 /* Module declarations from 'cc3d' */
 static PyTypeObject *__pyx_ptype_4cc3d___pyx_scope_struct__each = 0;
 static PyTypeObject *__pyx_ptype_4cc3d___pyx_scope_struct_1___iter__ = 0;
 static PyTypeObject *__pyx_ptype_4cc3d___pyx_scope_struct_2___iter__ = 0;
 static PyTypeObject *__pyx_array_type = 0;
@@ -12856,15 +12843,15 @@
   __pyx_t_1 = 0;
 
   /* "cc3d.pyx":651
  * 
  *   slices = []
  *   for xs, xe, ys, ye, zs, ze in bounding_boxes.reshape((N+1,6)):             # <<<<<<<<<<<<<<
  *     if xs < voxels and ys < voxels and zs < voxels:
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))
  */
   __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_bounding_boxes), __pyx_n_s_reshape); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 651, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_4 = __Pyx_PyInt_From_uint64_t((__pyx_v_N + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 651, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 651, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
@@ -13008,15 +12995,15 @@
     __Pyx_XDECREF_SET(__pyx_v_ze, __pyx_t_26);
     __pyx_t_26 = 0;
 
     /* "cc3d.pyx":652
  *   slices = []
  *   for xs, xe, ys, ye, zs, ze in bounding_boxes.reshape((N+1,6)):
  *     if xs < voxels and ys < voxels and zs < voxels:             # <<<<<<<<<<<<<<
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))
  *     else:
  */
     __pyx_t_1 = __Pyx_PyInt_From_uint64_t(__pyx_v_voxels); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 652, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_26 = PyObject_RichCompare(__pyx_v_xs, __pyx_t_1, Py_LT); __Pyx_XGOTREF(__pyx_t_26); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 652, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_29 = __Pyx_PyObject_IsTrue(__pyx_t_26); if (unlikely(__pyx_t_29 < 0)) __PYX_ERR(0, 652, __pyx_L1_error)
@@ -13046,59 +13033,68 @@
     __pyx_t_3 = __pyx_t_29;
     __pyx_L20_bool_binop_done:;
     if (__pyx_t_3) {
 
       /* "cc3d.pyx":653
  *   for xs, xe, ys, ye, zs, ze in bounding_boxes.reshape((N+1,6)):
  *     if xs < voxels and ys < voxels and zs < voxels:
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))             # <<<<<<<<<<<<<<
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))             # <<<<<<<<<<<<<<
  *     else:
  *       slices.append(None)
  */
       __pyx_t_26 = __Pyx_PyInt_AddObjC(__pyx_v_xe, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 653, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_26);
-      __pyx_t_1 = PySlice_New(__pyx_v_xs, __pyx_t_26, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyNumber_Int(__pyx_t_26); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 653, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
-      __pyx_t_26 = __Pyx_PyInt_AddObjC(__pyx_v_ye, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __pyx_t_26 = PySlice_New(__pyx_v_xs, __pyx_t_1, Py_None); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 653, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_26);
-      __pyx_t_25 = PySlice_New(__pyx_v_ys, __pyx_t_26, Py_None); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_ye, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_25 = __Pyx_PyNumber_Int(__pyx_t_1); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 653, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_25);
-      __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
-      __pyx_t_26 = __Pyx_PyInt_AddObjC(__pyx_v_ze, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 653, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_26);
-      __pyx_t_24 = PySlice_New(__pyx_v_zs, __pyx_t_26, Py_None); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = PySlice_New(__pyx_v_ys, __pyx_t_25, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
+      __pyx_t_25 = __Pyx_PyInt_AddObjC(__pyx_v_ze, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_25);
+      __pyx_t_24 = __Pyx_PyNumber_Int(__pyx_t_25); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 653, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_24);
-      __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
-      __pyx_t_26 = PyTuple_New(3); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 653, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_26);
+      __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
+      __pyx_t_25 = PySlice_New(__pyx_v_zs, __pyx_t_24, Py_None); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_25);
+      __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
+      __pyx_t_24 = PyTuple_New(3); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_24);
+      __Pyx_GIVEREF(__pyx_t_26);
+      PyTuple_SET_ITEM(__pyx_t_24, 0, __pyx_t_26);
       __Pyx_GIVEREF(__pyx_t_1);
-      PyTuple_SET_ITEM(__pyx_t_26, 0, __pyx_t_1);
+      PyTuple_SET_ITEM(__pyx_t_24, 1, __pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_25);
-      PyTuple_SET_ITEM(__pyx_t_26, 1, __pyx_t_25);
-      __Pyx_GIVEREF(__pyx_t_24);
-      PyTuple_SET_ITEM(__pyx_t_26, 2, __pyx_t_24);
+      PyTuple_SET_ITEM(__pyx_t_24, 2, __pyx_t_25);
+      __pyx_t_26 = 0;
       __pyx_t_1 = 0;
       __pyx_t_25 = 0;
-      __pyx_t_24 = 0;
-      __pyx_t_30 = __Pyx_PyList_Append(__pyx_v_slices, __pyx_t_26); if (unlikely(__pyx_t_30 == ((int)-1))) __PYX_ERR(0, 653, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
+      __pyx_t_30 = __Pyx_PyList_Append(__pyx_v_slices, __pyx_t_24); if (unlikely(__pyx_t_30 == ((int)-1))) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
 
       /* "cc3d.pyx":652
  *   slices = []
  *   for xs, xe, ys, ye, zs, ze in bounding_boxes.reshape((N+1,6)):
  *     if xs < voxels and ys < voxels and zs < voxels:             # <<<<<<<<<<<<<<
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))
  *     else:
  */
       goto __pyx_L19;
     }
 
     /* "cc3d.pyx":655
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))
  *     else:
  *       slices.append(None)             # <<<<<<<<<<<<<<
  * 
  *   return {
  */
     /*else*/ {
       __pyx_t_30 = __Pyx_PyList_Append(__pyx_v_slices, Py_None); if (unlikely(__pyx_t_30 == ((int)-1))) __PYX_ERR(0, 655, __pyx_L1_error)
@@ -13106,15 +13102,15 @@
     __pyx_L19:;
 
     /* "cc3d.pyx":651
  * 
  *   slices = []
  *   for xs, xe, ys, ye, zs, ze in bounding_boxes.reshape((N+1,6)):             # <<<<<<<<<<<<<<
  *     if xs < voxels and ys < voxels and zs < voxels:
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))
  */
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
   /* "cc3d.pyx":657
  *       slices.append(None)
  * 
@@ -13147,44 +13143,44 @@
   /* "cc3d.pyx":660
  *     "voxel_counts": counts,
  *     "bounding_boxes": slices,
  *     "centroids": centroids.reshape((N+1,3)),             # <<<<<<<<<<<<<<
  *   }
  * 
  */
-  __pyx_t_24 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_centroids), __pyx_n_s_reshape); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 660, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_24);
-  __pyx_t_25 = __Pyx_PyInt_From_uint64_t((__pyx_v_N + 1)); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __pyx_t_25 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_centroids), __pyx_n_s_reshape); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_25);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint64_t((__pyx_v_N + 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_25);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_25);
+  __pyx_t_26 = PyTuple_New(2); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_26);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_26, 0, __pyx_t_1);
   __Pyx_INCREF(__pyx_int_3);
   __Pyx_GIVEREF(__pyx_int_3);
-  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_3);
-  __pyx_t_25 = 0;
-  __pyx_t_25 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_24))) {
-    __pyx_t_25 = PyMethod_GET_SELF(__pyx_t_24);
-    if (likely(__pyx_t_25)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_24);
-      __Pyx_INCREF(__pyx_t_25);
+  PyTuple_SET_ITEM(__pyx_t_26, 1, __pyx_int_3);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_25))) {
+    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_25);
+    if (likely(__pyx_t_1)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_25);
+      __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_24, function);
+      __Pyx_DECREF_SET(__pyx_t_25, function);
     }
   }
-  __pyx_t_26 = (__pyx_t_25) ? __Pyx_PyObject_Call2Args(__pyx_t_24, __pyx_t_25, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_24, __pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_25); __pyx_t_25 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 660, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_26);
-  __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_centroids, __pyx_t_26) < 0) __PYX_ERR(0, 658, __pyx_L1_error)
+  __pyx_t_24 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_25, __pyx_t_1, __pyx_t_26) : __Pyx_PyObject_CallOneArg(__pyx_t_25, __pyx_t_26);
+  __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
+  if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_24);
+  __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_centroids, __pyx_t_24) < 0) __PYX_ERR(0, 658, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
   /* "cc3d.pyx":597
  * @cython.wraparound(False)
  * @cython.nonecheck(False)
@@ -13987,15 +13983,15 @@
   __pyx_t_1 = 0;
 
   /* "cc3d.pyx":651
  * 
  *   slices = []
  *   for xs, xe, ys, ye, zs, ze in bounding_boxes.reshape((N+1,6)):             # <<<<<<<<<<<<<<
  *     if xs < voxels and ys < voxels and zs < voxels:
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))
  */
   __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_bounding_boxes), __pyx_n_s_reshape); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 651, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_4 = __Pyx_PyInt_From_uint64_t((__pyx_v_N + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 651, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 651, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
@@ -14139,15 +14135,15 @@
     __Pyx_XDECREF_SET(__pyx_v_ze, __pyx_t_26);
     __pyx_t_26 = 0;
 
     /* "cc3d.pyx":652
  *   slices = []
  *   for xs, xe, ys, ye, zs, ze in bounding_boxes.reshape((N+1,6)):
  *     if xs < voxels and ys < voxels and zs < voxels:             # <<<<<<<<<<<<<<
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))
  *     else:
  */
     __pyx_t_1 = __Pyx_PyInt_From_uint64_t(__pyx_v_voxels); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 652, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_26 = PyObject_RichCompare(__pyx_v_xs, __pyx_t_1, Py_LT); __Pyx_XGOTREF(__pyx_t_26); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 652, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_29 = __Pyx_PyObject_IsTrue(__pyx_t_26); if (unlikely(__pyx_t_29 < 0)) __PYX_ERR(0, 652, __pyx_L1_error)
@@ -14177,59 +14173,68 @@
     __pyx_t_3 = __pyx_t_29;
     __pyx_L20_bool_binop_done:;
     if (__pyx_t_3) {
 
       /* "cc3d.pyx":653
  *   for xs, xe, ys, ye, zs, ze in bounding_boxes.reshape((N+1,6)):
  *     if xs < voxels and ys < voxels and zs < voxels:
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))             # <<<<<<<<<<<<<<
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))             # <<<<<<<<<<<<<<
  *     else:
  *       slices.append(None)
  */
       __pyx_t_26 = __Pyx_PyInt_AddObjC(__pyx_v_xe, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 653, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_26);
-      __pyx_t_1 = PySlice_New(__pyx_v_xs, __pyx_t_26, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyNumber_Int(__pyx_t_26); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 653, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
-      __pyx_t_26 = __Pyx_PyInt_AddObjC(__pyx_v_ye, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __pyx_t_26 = PySlice_New(__pyx_v_xs, __pyx_t_1, Py_None); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 653, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_26);
-      __pyx_t_25 = PySlice_New(__pyx_v_ys, __pyx_t_26, Py_None); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_ye, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_25 = __Pyx_PyNumber_Int(__pyx_t_1); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 653, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_25);
-      __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
-      __pyx_t_26 = __Pyx_PyInt_AddObjC(__pyx_v_ze, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 653, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_26);
-      __pyx_t_24 = PySlice_New(__pyx_v_zs, __pyx_t_26, Py_None); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = PySlice_New(__pyx_v_ys, __pyx_t_25, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
+      __pyx_t_25 = __Pyx_PyInt_AddObjC(__pyx_v_ze, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_25);
+      __pyx_t_24 = __Pyx_PyNumber_Int(__pyx_t_25); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 653, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_24);
-      __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
-      __pyx_t_26 = PyTuple_New(3); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 653, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_26);
+      __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
+      __pyx_t_25 = PySlice_New(__pyx_v_zs, __pyx_t_24, Py_None); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_25);
+      __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
+      __pyx_t_24 = PyTuple_New(3); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_24);
+      __Pyx_GIVEREF(__pyx_t_26);
+      PyTuple_SET_ITEM(__pyx_t_24, 0, __pyx_t_26);
       __Pyx_GIVEREF(__pyx_t_1);
-      PyTuple_SET_ITEM(__pyx_t_26, 0, __pyx_t_1);
+      PyTuple_SET_ITEM(__pyx_t_24, 1, __pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_25);
-      PyTuple_SET_ITEM(__pyx_t_26, 1, __pyx_t_25);
-      __Pyx_GIVEREF(__pyx_t_24);
-      PyTuple_SET_ITEM(__pyx_t_26, 2, __pyx_t_24);
+      PyTuple_SET_ITEM(__pyx_t_24, 2, __pyx_t_25);
+      __pyx_t_26 = 0;
       __pyx_t_1 = 0;
       __pyx_t_25 = 0;
-      __pyx_t_24 = 0;
-      __pyx_t_30 = __Pyx_PyList_Append(__pyx_v_slices, __pyx_t_26); if (unlikely(__pyx_t_30 == ((int)-1))) __PYX_ERR(0, 653, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
+      __pyx_t_30 = __Pyx_PyList_Append(__pyx_v_slices, __pyx_t_24); if (unlikely(__pyx_t_30 == ((int)-1))) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
 
       /* "cc3d.pyx":652
  *   slices = []
  *   for xs, xe, ys, ye, zs, ze in bounding_boxes.reshape((N+1,6)):
  *     if xs < voxels and ys < voxels and zs < voxels:             # <<<<<<<<<<<<<<
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))
  *     else:
  */
       goto __pyx_L19;
     }
 
     /* "cc3d.pyx":655
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))
  *     else:
  *       slices.append(None)             # <<<<<<<<<<<<<<
  * 
  *   return {
  */
     /*else*/ {
       __pyx_t_30 = __Pyx_PyList_Append(__pyx_v_slices, Py_None); if (unlikely(__pyx_t_30 == ((int)-1))) __PYX_ERR(0, 655, __pyx_L1_error)
@@ -14237,15 +14242,15 @@
     __pyx_L19:;
 
     /* "cc3d.pyx":651
  * 
  *   slices = []
  *   for xs, xe, ys, ye, zs, ze in bounding_boxes.reshape((N+1,6)):             # <<<<<<<<<<<<<<
  *     if xs < voxels and ys < voxels and zs < voxels:
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))
  */
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
   /* "cc3d.pyx":657
  *       slices.append(None)
  * 
@@ -14278,44 +14283,44 @@
   /* "cc3d.pyx":660
  *     "voxel_counts": counts,
  *     "bounding_boxes": slices,
  *     "centroids": centroids.reshape((N+1,3)),             # <<<<<<<<<<<<<<
  *   }
  * 
  */
-  __pyx_t_24 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_centroids), __pyx_n_s_reshape); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 660, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_24);
-  __pyx_t_25 = __Pyx_PyInt_From_uint64_t((__pyx_v_N + 1)); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __pyx_t_25 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_centroids), __pyx_n_s_reshape); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_25);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint64_t((__pyx_v_N + 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_25);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_25);
+  __pyx_t_26 = PyTuple_New(2); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_26);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_26, 0, __pyx_t_1);
   __Pyx_INCREF(__pyx_int_3);
   __Pyx_GIVEREF(__pyx_int_3);
-  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_3);
-  __pyx_t_25 = 0;
-  __pyx_t_25 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_24))) {
-    __pyx_t_25 = PyMethod_GET_SELF(__pyx_t_24);
-    if (likely(__pyx_t_25)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_24);
-      __Pyx_INCREF(__pyx_t_25);
+  PyTuple_SET_ITEM(__pyx_t_26, 1, __pyx_int_3);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_25))) {
+    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_25);
+    if (likely(__pyx_t_1)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_25);
+      __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_24, function);
+      __Pyx_DECREF_SET(__pyx_t_25, function);
     }
   }
-  __pyx_t_26 = (__pyx_t_25) ? __Pyx_PyObject_Call2Args(__pyx_t_24, __pyx_t_25, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_24, __pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_25); __pyx_t_25 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 660, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_26);
-  __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_centroids, __pyx_t_26) < 0) __PYX_ERR(0, 658, __pyx_L1_error)
+  __pyx_t_24 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_25, __pyx_t_1, __pyx_t_26) : __Pyx_PyObject_CallOneArg(__pyx_t_25, __pyx_t_26);
+  __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
+  if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_24);
+  __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_centroids, __pyx_t_24) < 0) __PYX_ERR(0, 658, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
   /* "cc3d.pyx":597
  * @cython.wraparound(False)
  * @cython.nonecheck(False)
@@ -15118,15 +15123,15 @@
   __pyx_t_1 = 0;
 
   /* "cc3d.pyx":651
  * 
  *   slices = []
  *   for xs, xe, ys, ye, zs, ze in bounding_boxes.reshape((N+1,6)):             # <<<<<<<<<<<<<<
  *     if xs < voxels and ys < voxels and zs < voxels:
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))
  */
   __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_bounding_boxes), __pyx_n_s_reshape); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 651, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_4 = __Pyx_PyInt_From_uint64_t((__pyx_v_N + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 651, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 651, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
@@ -15270,15 +15275,15 @@
     __Pyx_XDECREF_SET(__pyx_v_ze, __pyx_t_26);
     __pyx_t_26 = 0;
 
     /* "cc3d.pyx":652
  *   slices = []
  *   for xs, xe, ys, ye, zs, ze in bounding_boxes.reshape((N+1,6)):
  *     if xs < voxels and ys < voxels and zs < voxels:             # <<<<<<<<<<<<<<
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))
  *     else:
  */
     __pyx_t_1 = __Pyx_PyInt_From_uint64_t(__pyx_v_voxels); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 652, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_26 = PyObject_RichCompare(__pyx_v_xs, __pyx_t_1, Py_LT); __Pyx_XGOTREF(__pyx_t_26); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 652, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_29 = __Pyx_PyObject_IsTrue(__pyx_t_26); if (unlikely(__pyx_t_29 < 0)) __PYX_ERR(0, 652, __pyx_L1_error)
@@ -15308,59 +15313,68 @@
     __pyx_t_3 = __pyx_t_29;
     __pyx_L20_bool_binop_done:;
     if (__pyx_t_3) {
 
       /* "cc3d.pyx":653
  *   for xs, xe, ys, ye, zs, ze in bounding_boxes.reshape((N+1,6)):
  *     if xs < voxels and ys < voxels and zs < voxels:
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))             # <<<<<<<<<<<<<<
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))             # <<<<<<<<<<<<<<
  *     else:
  *       slices.append(None)
  */
       __pyx_t_26 = __Pyx_PyInt_AddObjC(__pyx_v_xe, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 653, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_26);
-      __pyx_t_1 = PySlice_New(__pyx_v_xs, __pyx_t_26, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyNumber_Int(__pyx_t_26); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 653, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
-      __pyx_t_26 = __Pyx_PyInt_AddObjC(__pyx_v_ye, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __pyx_t_26 = PySlice_New(__pyx_v_xs, __pyx_t_1, Py_None); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 653, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_26);
-      __pyx_t_25 = PySlice_New(__pyx_v_ys, __pyx_t_26, Py_None); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_ye, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_25 = __Pyx_PyNumber_Int(__pyx_t_1); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 653, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_25);
-      __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
-      __pyx_t_26 = __Pyx_PyInt_AddObjC(__pyx_v_ze, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 653, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_26);
-      __pyx_t_24 = PySlice_New(__pyx_v_zs, __pyx_t_26, Py_None); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = PySlice_New(__pyx_v_ys, __pyx_t_25, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
+      __pyx_t_25 = __Pyx_PyInt_AddObjC(__pyx_v_ze, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_25);
+      __pyx_t_24 = __Pyx_PyNumber_Int(__pyx_t_25); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 653, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_24);
-      __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
-      __pyx_t_26 = PyTuple_New(3); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 653, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_26);
+      __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
+      __pyx_t_25 = PySlice_New(__pyx_v_zs, __pyx_t_24, Py_None); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_25);
+      __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
+      __pyx_t_24 = PyTuple_New(3); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_24);
+      __Pyx_GIVEREF(__pyx_t_26);
+      PyTuple_SET_ITEM(__pyx_t_24, 0, __pyx_t_26);
       __Pyx_GIVEREF(__pyx_t_1);
-      PyTuple_SET_ITEM(__pyx_t_26, 0, __pyx_t_1);
+      PyTuple_SET_ITEM(__pyx_t_24, 1, __pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_25);
-      PyTuple_SET_ITEM(__pyx_t_26, 1, __pyx_t_25);
-      __Pyx_GIVEREF(__pyx_t_24);
-      PyTuple_SET_ITEM(__pyx_t_26, 2, __pyx_t_24);
+      PyTuple_SET_ITEM(__pyx_t_24, 2, __pyx_t_25);
+      __pyx_t_26 = 0;
       __pyx_t_1 = 0;
       __pyx_t_25 = 0;
-      __pyx_t_24 = 0;
-      __pyx_t_30 = __Pyx_PyList_Append(__pyx_v_slices, __pyx_t_26); if (unlikely(__pyx_t_30 == ((int)-1))) __PYX_ERR(0, 653, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
+      __pyx_t_30 = __Pyx_PyList_Append(__pyx_v_slices, __pyx_t_24); if (unlikely(__pyx_t_30 == ((int)-1))) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
 
       /* "cc3d.pyx":652
  *   slices = []
  *   for xs, xe, ys, ye, zs, ze in bounding_boxes.reshape((N+1,6)):
  *     if xs < voxels and ys < voxels and zs < voxels:             # <<<<<<<<<<<<<<
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))
  *     else:
  */
       goto __pyx_L19;
     }
 
     /* "cc3d.pyx":655
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))
  *     else:
  *       slices.append(None)             # <<<<<<<<<<<<<<
  * 
  *   return {
  */
     /*else*/ {
       __pyx_t_30 = __Pyx_PyList_Append(__pyx_v_slices, Py_None); if (unlikely(__pyx_t_30 == ((int)-1))) __PYX_ERR(0, 655, __pyx_L1_error)
@@ -15368,15 +15382,15 @@
     __pyx_L19:;
 
     /* "cc3d.pyx":651
  * 
  *   slices = []
  *   for xs, xe, ys, ye, zs, ze in bounding_boxes.reshape((N+1,6)):             # <<<<<<<<<<<<<<
  *     if xs < voxels and ys < voxels and zs < voxels:
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))
  */
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
   /* "cc3d.pyx":657
  *       slices.append(None)
  * 
@@ -15409,44 +15423,44 @@
   /* "cc3d.pyx":660
  *     "voxel_counts": counts,
  *     "bounding_boxes": slices,
  *     "centroids": centroids.reshape((N+1,3)),             # <<<<<<<<<<<<<<
  *   }
  * 
  */
-  __pyx_t_24 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_centroids), __pyx_n_s_reshape); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 660, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_24);
-  __pyx_t_25 = __Pyx_PyInt_From_uint64_t((__pyx_v_N + 1)); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __pyx_t_25 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_centroids), __pyx_n_s_reshape); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_25);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint64_t((__pyx_v_N + 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_25);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_25);
+  __pyx_t_26 = PyTuple_New(2); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_26);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_26, 0, __pyx_t_1);
   __Pyx_INCREF(__pyx_int_3);
   __Pyx_GIVEREF(__pyx_int_3);
-  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_3);
-  __pyx_t_25 = 0;
-  __pyx_t_25 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_24))) {
-    __pyx_t_25 = PyMethod_GET_SELF(__pyx_t_24);
-    if (likely(__pyx_t_25)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_24);
-      __Pyx_INCREF(__pyx_t_25);
+  PyTuple_SET_ITEM(__pyx_t_26, 1, __pyx_int_3);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_25))) {
+    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_25);
+    if (likely(__pyx_t_1)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_25);
+      __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_24, function);
+      __Pyx_DECREF_SET(__pyx_t_25, function);
     }
   }
-  __pyx_t_26 = (__pyx_t_25) ? __Pyx_PyObject_Call2Args(__pyx_t_24, __pyx_t_25, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_24, __pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_25); __pyx_t_25 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 660, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_26);
-  __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_centroids, __pyx_t_26) < 0) __PYX_ERR(0, 658, __pyx_L1_error)
+  __pyx_t_24 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_25, __pyx_t_1, __pyx_t_26) : __Pyx_PyObject_CallOneArg(__pyx_t_25, __pyx_t_26);
+  __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
+  if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_24);
+  __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_centroids, __pyx_t_24) < 0) __PYX_ERR(0, 658, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
   /* "cc3d.pyx":597
  * @cython.wraparound(False)
  * @cython.nonecheck(False)
@@ -16249,15 +16263,15 @@
   __pyx_t_1 = 0;
 
   /* "cc3d.pyx":651
  * 
  *   slices = []
  *   for xs, xe, ys, ye, zs, ze in bounding_boxes.reshape((N+1,6)):             # <<<<<<<<<<<<<<
  *     if xs < voxels and ys < voxels and zs < voxels:
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))
  */
   __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_bounding_boxes), __pyx_n_s_reshape); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 651, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_4 = __Pyx_PyInt_From_uint64_t((__pyx_v_N + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 651, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 651, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
@@ -16401,15 +16415,15 @@
     __Pyx_XDECREF_SET(__pyx_v_ze, __pyx_t_26);
     __pyx_t_26 = 0;
 
     /* "cc3d.pyx":652
  *   slices = []
  *   for xs, xe, ys, ye, zs, ze in bounding_boxes.reshape((N+1,6)):
  *     if xs < voxels and ys < voxels and zs < voxels:             # <<<<<<<<<<<<<<
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))
  *     else:
  */
     __pyx_t_1 = __Pyx_PyInt_From_uint64_t(__pyx_v_voxels); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 652, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_26 = PyObject_RichCompare(__pyx_v_xs, __pyx_t_1, Py_LT); __Pyx_XGOTREF(__pyx_t_26); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 652, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_29 = __Pyx_PyObject_IsTrue(__pyx_t_26); if (unlikely(__pyx_t_29 < 0)) __PYX_ERR(0, 652, __pyx_L1_error)
@@ -16439,59 +16453,68 @@
     __pyx_t_3 = __pyx_t_29;
     __pyx_L20_bool_binop_done:;
     if (__pyx_t_3) {
 
       /* "cc3d.pyx":653
  *   for xs, xe, ys, ye, zs, ze in bounding_boxes.reshape((N+1,6)):
  *     if xs < voxels and ys < voxels and zs < voxels:
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))             # <<<<<<<<<<<<<<
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))             # <<<<<<<<<<<<<<
  *     else:
  *       slices.append(None)
  */
       __pyx_t_26 = __Pyx_PyInt_AddObjC(__pyx_v_xe, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 653, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_26);
-      __pyx_t_1 = PySlice_New(__pyx_v_xs, __pyx_t_26, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyNumber_Int(__pyx_t_26); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 653, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
-      __pyx_t_26 = __Pyx_PyInt_AddObjC(__pyx_v_ye, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __pyx_t_26 = PySlice_New(__pyx_v_xs, __pyx_t_1, Py_None); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 653, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_26);
-      __pyx_t_25 = PySlice_New(__pyx_v_ys, __pyx_t_26, Py_None); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_ye, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_25 = __Pyx_PyNumber_Int(__pyx_t_1); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 653, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_25);
-      __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
-      __pyx_t_26 = __Pyx_PyInt_AddObjC(__pyx_v_ze, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 653, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_26);
-      __pyx_t_24 = PySlice_New(__pyx_v_zs, __pyx_t_26, Py_None); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = PySlice_New(__pyx_v_ys, __pyx_t_25, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
+      __pyx_t_25 = __Pyx_PyInt_AddObjC(__pyx_v_ze, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_25);
+      __pyx_t_24 = __Pyx_PyNumber_Int(__pyx_t_25); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 653, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_24);
-      __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
-      __pyx_t_26 = PyTuple_New(3); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 653, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_26);
+      __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
+      __pyx_t_25 = PySlice_New(__pyx_v_zs, __pyx_t_24, Py_None); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_25);
+      __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
+      __pyx_t_24 = PyTuple_New(3); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_24);
+      __Pyx_GIVEREF(__pyx_t_26);
+      PyTuple_SET_ITEM(__pyx_t_24, 0, __pyx_t_26);
       __Pyx_GIVEREF(__pyx_t_1);
-      PyTuple_SET_ITEM(__pyx_t_26, 0, __pyx_t_1);
+      PyTuple_SET_ITEM(__pyx_t_24, 1, __pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_25);
-      PyTuple_SET_ITEM(__pyx_t_26, 1, __pyx_t_25);
-      __Pyx_GIVEREF(__pyx_t_24);
-      PyTuple_SET_ITEM(__pyx_t_26, 2, __pyx_t_24);
+      PyTuple_SET_ITEM(__pyx_t_24, 2, __pyx_t_25);
+      __pyx_t_26 = 0;
       __pyx_t_1 = 0;
       __pyx_t_25 = 0;
-      __pyx_t_24 = 0;
-      __pyx_t_30 = __Pyx_PyList_Append(__pyx_v_slices, __pyx_t_26); if (unlikely(__pyx_t_30 == ((int)-1))) __PYX_ERR(0, 653, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
+      __pyx_t_30 = __Pyx_PyList_Append(__pyx_v_slices, __pyx_t_24); if (unlikely(__pyx_t_30 == ((int)-1))) __PYX_ERR(0, 653, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
 
       /* "cc3d.pyx":652
  *   slices = []
  *   for xs, xe, ys, ye, zs, ze in bounding_boxes.reshape((N+1,6)):
  *     if xs < voxels and ys < voxels and zs < voxels:             # <<<<<<<<<<<<<<
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))
  *     else:
  */
       goto __pyx_L19;
     }
 
     /* "cc3d.pyx":655
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))
  *     else:
  *       slices.append(None)             # <<<<<<<<<<<<<<
  * 
  *   return {
  */
     /*else*/ {
       __pyx_t_30 = __Pyx_PyList_Append(__pyx_v_slices, Py_None); if (unlikely(__pyx_t_30 == ((int)-1))) __PYX_ERR(0, 655, __pyx_L1_error)
@@ -16499,15 +16522,15 @@
     __pyx_L19:;
 
     /* "cc3d.pyx":651
  * 
  *   slices = []
  *   for xs, xe, ys, ye, zs, ze in bounding_boxes.reshape((N+1,6)):             # <<<<<<<<<<<<<<
  *     if xs < voxels and ys < voxels and zs < voxels:
- *       slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1)))
+ *       slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))
  */
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
   /* "cc3d.pyx":657
  *       slices.append(None)
  * 
@@ -16540,44 +16563,44 @@
   /* "cc3d.pyx":660
  *     "voxel_counts": counts,
  *     "bounding_boxes": slices,
  *     "centroids": centroids.reshape((N+1,3)),             # <<<<<<<<<<<<<<
  *   }
  * 
  */
-  __pyx_t_24 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_centroids), __pyx_n_s_reshape); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 660, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_24);
-  __pyx_t_25 = __Pyx_PyInt_From_uint64_t((__pyx_v_N + 1)); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __pyx_t_25 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_centroids), __pyx_n_s_reshape); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_25);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint64_t((__pyx_v_N + 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_25);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_25);
+  __pyx_t_26 = PyTuple_New(2); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_26);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_26, 0, __pyx_t_1);
   __Pyx_INCREF(__pyx_int_3);
   __Pyx_GIVEREF(__pyx_int_3);
-  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_3);
-  __pyx_t_25 = 0;
-  __pyx_t_25 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_24))) {
-    __pyx_t_25 = PyMethod_GET_SELF(__pyx_t_24);
-    if (likely(__pyx_t_25)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_24);
-      __Pyx_INCREF(__pyx_t_25);
+  PyTuple_SET_ITEM(__pyx_t_26, 1, __pyx_int_3);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_25))) {
+    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_25);
+    if (likely(__pyx_t_1)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_25);
+      __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_24, function);
+      __Pyx_DECREF_SET(__pyx_t_25, function);
     }
   }
-  __pyx_t_26 = (__pyx_t_25) ? __Pyx_PyObject_Call2Args(__pyx_t_24, __pyx_t_25, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_24, __pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_25); __pyx_t_25 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 660, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_26);
-  __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_centroids, __pyx_t_26) < 0) __PYX_ERR(0, 658, __pyx_L1_error)
+  __pyx_t_24 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_25, __pyx_t_1, __pyx_t_26) : __Pyx_PyObject_CallOneArg(__pyx_t_25, __pyx_t_26);
+  __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
+  if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_24);
+  __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_centroids, __pyx_t_24) < 0) __PYX_ERR(0, 658, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
   /* "cc3d.pyx":597
  * @cython.wraparound(False)
  * @cython.nonecheck(False)
@@ -31589,15 +31612,15 @@
  *     memset(self.data.as_chars, 0, Py_SIZE(self) * self.ob_descr.itemsize)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":735
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -31606,29 +31629,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":736
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 736, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":735
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -31639,15 +31662,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":738
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -31656,29 +31679,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":739
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 739, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":738
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -31689,15 +31712,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":741
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -31706,29 +31729,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":742
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 742, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":741
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -31739,15 +31762,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":744
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -31756,29 +31779,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":745
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 745, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":744
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -31789,15 +31812,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":747
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -31806,29 +31829,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":748
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 748, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":747
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -31839,212 +31862,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":750
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":751
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":752
+    /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":751
+    /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":754
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":750
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":929
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":868
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":930
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":869
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":931
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":870
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":929
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":868
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":933
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":872
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":934
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":873
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":935
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":874
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":936
+    /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":875
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":935
+    /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":874
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":937
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":876
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":933
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":872
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":941
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":880
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -32060,15 +32083,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":942
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -32076,84 +32099,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":943
+      /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":882
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 943, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 882, __pyx_L3_error)
 
-      /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":942
+      /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":944
+    /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":883
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 944, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 883, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":945
+      /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":884
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 945, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 884, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 945, __pyx_L5_except_error)
+      __PYX_ERR(2, 884, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":942
+    /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":881
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":941
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":880
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -32168,15 +32191,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":947
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":886
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -32192,15 +32215,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":948
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -32208,84 +32231,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":949
+      /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":888
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 949, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 888, __pyx_L3_error)
 
-      /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":948
+      /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":950
+    /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":889
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 950, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 889, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":951
+      /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":890
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 951, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 890, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 951, __pyx_L5_except_error)
+      __PYX_ERR(2, 890, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":948
+    /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":887
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":947
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":886
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -32300,15 +32323,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":953
+/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":892
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -32324,15 +32347,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":954
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -32340,84 +32363,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":955
+      /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":894
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 955, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 894, __pyx_L3_error)
 
-      /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":954
+      /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":956
+    /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":895
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 956, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 895, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":957
+      /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":896
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 957, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 896, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 957, __pyx_L5_except_error)
+      __PYX_ERR(2, 896, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":954
+    /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":893
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":953
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":892
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -32432,188 +32455,14 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":967
- * 
- * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.timedelta64)`
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
-
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":979
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
-  goto __pyx_L0;
-
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":967
- * 
- * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.timedelta64)`
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":982
- * 
- * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.datetime64)`
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
-
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":994
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
-  goto __pyx_L0;
-
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":982
- * 
- * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.datetime64)`
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":997
- * 
- * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy datetime64 object
- */
-
-static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
-  npy_datetime __pyx_r;
-
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":1004
- *     also needed.  That can be found using `get_datetime64_unit`.
- *     """
- *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":997
- * 
- * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy datetime64 object
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":1007
- * 
- * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy timedelta64 object
- */
-
-static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
-  npy_timedelta __pyx_r;
-
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":1011
- *     returns the int64 value underlying scalar numpy timedelta64 object
- *     """
- *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":1007
- * 
- * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy timedelta64 object
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
-/* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":1014
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
-
-static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
-  NPY_DATETIMEUNIT __pyx_r;
-
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":1018
- *     returns the unit part of the dtype for a numpy datetime64 object.
- *     """
- *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
- */
-  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
-  goto __pyx_L0;
-
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":1014
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
 /* "pair.from_py":145
  * 
  * @cname("__pyx_convert_pair_from_py_size_t__and_size_t")
  * cdef pair[X,Y] __pyx_convert_pair_from_py_size_t__and_size_t(object o) except *:             # <<<<<<<<<<<<<<
  *     x, y = o
  *     return pair[X,Y](<X>x, <Y>y)
  */
@@ -47879,15 +47728,15 @@
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 128, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 205, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 266, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 1070, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 109, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 945, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 884, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(3, 404, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(3, 613, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(3, 832, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
@@ -47964,33 +47813,33 @@
  *       for key, rns in all_runs.items():
  */
   __pyx_tuple__14 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_img, __pyx_n_s_key, __pyx_n_s_rns); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 959, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
   __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cc3d_pyx, __pyx_n_s_iter, 959, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 959, __pyx_L1_error)
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":945
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":884
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 945, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 884, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
-  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":951
+  /* "../../.virtualenvs/cc3d/lib/python3.9/site-packages/numpy/__init__.pxd":890
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(2, 951, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(2, 890, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
 
   /* "View.MemoryView":133
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
@@ -48618,46 +48467,26 @@
    if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("array"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_5array_array = __Pyx_ImportType(__pyx_t_1, "array", "array", sizeof(arrayobject), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(1, 58, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 200, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 200, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 223, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 227, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 787, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 789, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 827, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 764, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
```

### Comparing `connected-components-3d-3.9.0/cc3d.hpp` & `connected-components-3d-3.9.1/cc3d.hpp`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/cc3d.pyx` & `connected-components-3d-3.9.1/cc3d.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -646,15 +646,15 @@
     centroids[3 * label + 0] /= <double>counts[label]
     centroids[3 * label + 1] /= <double>counts[label]
     centroids[3 * label + 2] /= <double>counts[label]
 
   slices = []
   for xs, xe, ys, ye, zs, ze in bounding_boxes.reshape((N+1,6)):
     if xs < voxels and ys < voxels and zs < voxels:
-      slices.append((slice(xs,xe+1), slice(ys,ye+1), slice(zs,ze+1))) 
+      slices.append((slice(xs, int(xe+1)), slice(ys, int(ye+1)), slice(zs, int(ze+1))))
     else:
       slices.append(None)
   
   return {
     "voxel_counts": counts,
     "bounding_boxes": slices,
     "centroids": centroids.reshape((N+1,3)),
```

### Comparing `connected-components-3d-3.9.0/cc3d_continuous.hpp` & `connected-components-3d-3.9.1/cc3d_continuous.hpp`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/cc3d_graphs.hpp` & `connected-components-3d-3.9.1/cc3d_graphs.hpp`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/connected_components_3d.egg-info/PKG-INFO` & `connected-components-3d-3.9.1/connected_components_3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connected-components-3d
-Version: 3.9.0
+Version: 3.9.1
 Summary: Connected components on 2D and 3D images. Supports multiple labels.
 Home-page: https://github.com/seung-lab/connected-components-3d/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description: [![Build Status](https://travis-ci.org/seung-lab/connected-components-3d.svg?branch=master)](https://travis-ci.org/seung-lab/connected-components-3d) [![PyPI version](https://badge.fury.io/py/connected-components-3d.svg)](https://badge.fury.io/py/connected-components-3d) [![DOI](https://zenodo.org/badge/146368855.svg)](https://zenodo.org/badge/latestdoi/146368855)
```

### Comparing `connected-components-3d-3.9.0/connected_components_3d.egg-info/SOURCES.txt` & `connected-components-3d-3.9.1/connected_components_3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/manual_testing/test.py` & `connected-components-3d-3.9.1/manual_testing/test.py`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/manual_testing/test2d.png` & `connected-components-3d-3.9.1/manual_testing/test2d.png`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/manual_testing/test3d-1.png` & `connected-components-3d-3.9.1/manual_testing/test3d-1.png`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/manual_testing/test3d-2.png` & `connected-components-3d-3.9.1/manual_testing/test3d-2.png`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/manual_testing/test3d-3.png` & `connected-components-3d-3.9.1/manual_testing/test3d-3.png`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/manylinux1.Dockerfile` & `connected-components-3d-3.9.1/manylinux1.Dockerfile`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/manylinux2010.Dockerfile` & `connected-components-3d-3.9.1/manylinux2010.Dockerfile`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/manylinux2014.Dockerfile` & `connected-components-3d-3.9.1/manylinux2014.Dockerfile`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/perf.py` & `connected-components-3d-3.9.1/perf.py`

 * *Files identical despite different names*

### Comparing `connected-components-3d-3.9.0/setup.py` & `connected-components-3d-3.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   ]
 
 if sys.platform == 'darwin':
   extra_compile_args += [ '-stdlib=libc++', '-mmacosx-version-min=10.9' ]
 
 setuptools.setup(
   name="connected-components-3d",
-  version="3.9.0",
+  version="3.9.1",
   setup_requires=['pbr', 'numpy'],
   install_requires=['numpy'],
   python_requires="~=3.7", # >= 3.7 < 4.0
   ext_modules=[
     setuptools.Extension(
       'cc3d',
       sources=[ 'cc3d.cpp' ],
```

### Comparing `connected-components-3d-3.9.0/test.cpp` & `connected-components-3d-3.9.1/test.cpp`

 * *Files identical despite different names*

