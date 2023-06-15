# Comparing `tmp/pylusat-0.5.7.tar.gz` & `tmp/pylusat-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylusat-0.5.7.tar", last modified: Thu Oct 20 21:21:03 2022, max compression
+gzip compressed data, was "pylusat-0.5.8.tar", last modified: Thu Jun 15 19:35:00 2023, max compression
```

## Comparing `pylusat-0.5.7.tar` & `pylusat-0.5.8.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2022-10-20 21:21:03.553769 pylusat-0.5.7/
--rw-r--r--   0 changjiechen   (501) staff       (20)     1498 2022-09-29 14:35:28.000000 pylusat-0.5.7/LICENSE.txt
--rw-r--r--   0 changjiechen   (501) staff       (20)     1981 2022-10-20 21:21:03.553559 pylusat-0.5.7/PKG-INFO
--rw-r--r--   0 changjiechen   (501) staff       (20)     1038 2022-09-29 14:35:28.000000 pylusat-0.5.7/README.md
-drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2022-10-20 21:21:03.502174 pylusat-0.5.7/pylusat/
--rw-r--r--   0 changjiechen   (501) staff       (20)       41 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/__init__.py
--rw-r--r--   0 changjiechen   (501) staff       (20)       22 2022-10-20 21:15:21.000000 pylusat-0.5.7/pylusat/_version.py
--rw-r--r--   0 changjiechen   (501) staff       (20)    11007 2022-10-20 20:46:31.000000 pylusat-0.5.7/pylusat/base.py
-drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2022-10-20 21:21:03.503268 pylusat-0.5.7/pylusat/datasets/
--rw-r--r--   0 changjiechen   (501) staff       (20)     1476 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/__init__.py
-drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2022-10-20 21:21:03.507070 pylusat-0.5.7/pylusat/datasets/acs2016/
--rw-r--r--   0 changjiechen   (501) staff       (20)        5 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/acs2016/acs2016.CPG
--rw-r--r--   0 changjiechen   (501) staff       (20)    46559 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/acs2016/acs2016.dbf
--rw-r--r--   0 changjiechen   (501) staff       (20)      501 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/acs2016/acs2016.prj
--rw-r--r--   0 changjiechen   (501) staff       (20)     1692 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/acs2016/acs2016.sbn
--rw-r--r--   0 changjiechen   (501) staff       (20)      228 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/acs2016/acs2016.sbx
--rw-r--r--   0 changjiechen   (501) staff       (20)   521324 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/acs2016/acs2016.shp
--rw-r--r--   0 changjiechen   (501) staff       (20)   216105 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/acs2016/acs2016.shp.xml
--rw-r--r--   0 changjiechen   (501) staff       (20)     1340 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/acs2016/acs2016.shx
-drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2022-10-20 21:21:03.516217 pylusat-0.5.7/pylusat/datasets/habitat/
--rw-r--r--   0 changjiechen   (501) staff       (20)       91 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/habitat/habitat.tfw
--rw-r--r--   0 changjiechen   (501) staff       (20)  4201504 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/habitat/habitat.tif
--rw-r--r--   0 changjiechen   (501) staff       (20)     1481 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/habitat/habitat.tif.aux.xml
--rw-r--r--   0 changjiechen   (501) staff       (20)   313777 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/habitat/habitat.tif.ovr
--rw-r--r--   0 changjiechen   (501) staff       (20)        5 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/habitat/habitat.tif.vat.cpg
--rw-r--r--   0 changjiechen   (501) staff       (20)      908 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/habitat/habitat.tif.vat.dbf
-drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2022-10-20 21:21:03.519900 pylusat-0.5.7/pylusat/datasets/habitat_fl_stateplane/
--rw-r--r--   0 changjiechen   (501) staff       (20)       92 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tfw
--rw-r--r--   0 changjiechen   (501) staff       (20)   759776 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif
--rw-r--r--   0 changjiechen   (501) staff       (20)     1599 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif.aux.xml
--rw-r--r--   0 changjiechen   (501) staff       (20)   315409 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif.ovr
--rw-r--r--   0 changjiechen   (501) staff       (20)        5 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif.vat.cpg
--rw-r--r--   0 changjiechen   (501) staff       (20)      908 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif.vat.dbf
--rw-r--r--   0 changjiechen   (501) staff       (20)     8412 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif.xml
-drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2022-10-20 21:21:03.524648 pylusat-0.5.7/pylusat/datasets/habitat_shift/
--rw-r--r--   0 changjiechen   (501) staff       (20)       91 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/habitat_shift/habitat_shift.tfw
--rw-r--r--   0 changjiechen   (501) staff       (20)   755954 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/habitat_shift/habitat_shift.tif
--rw-r--r--   0 changjiechen   (501) staff       (20)     1479 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/habitat_shift/habitat_shift.tif.aux.xml
--rw-r--r--   0 changjiechen   (501) staff       (20)   314738 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/habitat_shift/habitat_shift.tif.ovr
--rw-r--r--   0 changjiechen   (501) staff       (20)        5 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/habitat_shift/habitat_shift.tif.vat.cpg
--rw-r--r--   0 changjiechen   (501) staff       (20)      968 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/habitat_shift/habitat_shift.tif.vat.dbf
--rw-r--r--   0 changjiechen   (501) staff       (20)     7091 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/habitat_shift/habitat_shift.tif.xml
-drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2022-10-20 21:21:03.527604 pylusat-0.5.7/pylusat/datasets/highway/
--rw-r--r--   0 changjiechen   (501) staff       (20)        5 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/highway/highway.cpg
--rw-r--r--   0 changjiechen   (501) staff       (20)     8348 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/highway/highway.dbf
--rw-r--r--   0 changjiechen   (501) staff       (20)      501 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/highway/highway.prj
--rw-r--r--   0 changjiechen   (501) staff       (20)      628 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/highway/highway.sbn
--rw-r--r--   0 changjiechen   (501) staff       (20)      164 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/highway/highway.sbx
--rw-r--r--   0 changjiechen   (501) staff       (20)    25276 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/highway/highway.shp
--rw-r--r--   0 changjiechen   (501) staff       (20)   136966 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/highway/highway.shp.xml
--rw-r--r--   0 changjiechen   (501) staff       (20)      508 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/highway/highway.shx
-drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2022-10-20 21:21:03.530180 pylusat-0.5.7/pylusat/datasets/schools/
--rw-r--r--   0 changjiechen   (501) staff       (20)        5 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/schools/schools.CPG
--rw-r--r--   0 changjiechen   (501) staff       (20)    37743 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/schools/schools.dbf
--rw-r--r--   0 changjiechen   (501) staff       (20)      501 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/schools/schools.prj
--rw-r--r--   0 changjiechen   (501) staff       (20)     1396 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/schools/schools.sbn
--rw-r--r--   0 changjiechen   (501) staff       (20)      196 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/schools/schools.sbx
--rw-r--r--   0 changjiechen   (501) staff       (20)     3488 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/schools/schools.shp
--rw-r--r--   0 changjiechen   (501) staff       (20)   263975 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/schools/schools.shp.xml
--rw-r--r--   0 changjiechen   (501) staff       (20)     1068 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/schools/schools.shx
-drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2022-10-20 21:21:03.550730 pylusat-0.5.7/pylusat/datasets/streets/
--rw-r--r--   0 changjiechen   (501) staff       (20)        5 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/streets/streets.CPG
--rw-r--r--   0 changjiechen   (501) staff       (20)  8317235 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/streets/streets.dbf
--rw-r--r--   0 changjiechen   (501) staff       (20)      501 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/streets/streets.prj
--rw-r--r--   0 changjiechen   (501) staff       (20)   214284 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/streets/streets.sbn
--rw-r--r--   0 changjiechen   (501) staff       (20)    12588 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/streets/streets.sbx
--rw-r--r--   0 changjiechen   (501) staff       (20)  3467420 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/streets/streets.shp
--rw-r--r--   0 changjiechen   (501) staff       (20)    38406 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/streets/streets.shp.xml
--rw-r--r--   0 changjiechen   (501) staff       (20)   169388 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/datasets/streets/streets.shx
--rw-r--r--   0 changjiechen   (501) staff       (20)     7527 2022-10-20 21:03:25.000000 pylusat-0.5.7/pylusat/density.py
--rw-r--r--   0 changjiechen   (501) staff       (20)     7055 2022-10-20 21:03:25.000000 pylusat-0.5.7/pylusat/distance.py
--rw-r--r--   0 changjiechen   (501) staff       (20)    12574 2022-10-20 21:06:02.000000 pylusat-0.5.7/pylusat/geotools.py
--rw-r--r--   0 changjiechen   (501) staff       (20)     4464 2022-10-20 21:03:25.000000 pylusat-0.5.7/pylusat/interpolate.py
--rw-r--r--   0 changjiechen   (501) staff       (20)     7186 2022-10-20 21:03:25.000000 pylusat-0.5.7/pylusat/rescale.py
-drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2022-10-20 21:21:03.553236 pylusat-0.5.7/pylusat/tests/
--rw-r--r--   0 changjiechen   (501) staff       (20)        0 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/tests/__init__.py
--rw-r--r--   0 changjiechen   (501) staff       (20)     1060 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/tests/test_base.py
--rw-r--r--   0 changjiechen   (501) staff       (20)      971 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/tests/test_density.py
--rw-r--r--   0 changjiechen   (501) staff       (20)      820 2022-09-29 18:54:56.000000 pylusat-0.5.7/pylusat/tests/test_distance.py
--rw-r--r--   0 changjiechen   (501) staff       (20)     1292 2022-10-20 20:44:19.000000 pylusat-0.5.7/pylusat/tests/test_geotools.py
--rw-r--r--   0 changjiechen   (501) staff       (20)      475 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/tests/test_interpolate.py
--rw-r--r--   0 changjiechen   (501) staff       (20)      338 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/tests/test_rescale.py
--rw-r--r--   0 changjiechen   (501) staff       (20)       34 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/tests/test_utils.py
--rw-r--r--   0 changjiechen   (501) staff       (20)     1026 2022-09-29 14:35:28.000000 pylusat-0.5.7/pylusat/tests/test_zonal.py
--rw-r--r--   0 changjiechen   (501) staff       (20)     7596 2022-10-20 21:03:25.000000 pylusat-0.5.7/pylusat/utils.py
--rw-r--r--   0 changjiechen   (501) staff       (20)     3748 2022-10-20 21:03:25.000000 pylusat-0.5.7/pylusat/zonal.py
-drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2022-10-20 21:21:03.503052 pylusat-0.5.7/pylusat.egg-info/
--rw-r--r--   0 changjiechen   (501) staff       (20)     1981 2022-10-20 21:21:03.000000 pylusat-0.5.7/pylusat.egg-info/PKG-INFO
--rw-r--r--   0 changjiechen   (501) staff       (20)     2981 2022-10-20 21:21:03.000000 pylusat-0.5.7/pylusat.egg-info/SOURCES.txt
--rw-r--r--   0 changjiechen   (501) staff       (20)        1 2022-10-20 21:21:03.000000 pylusat-0.5.7/pylusat.egg-info/dependency_links.txt
--rw-r--r--   0 changjiechen   (501) staff       (20)       37 2022-10-20 21:21:03.000000 pylusat-0.5.7/pylusat.egg-info/requires.txt
--rw-r--r--   0 changjiechen   (501) staff       (20)        8 2022-10-20 21:21:03.000000 pylusat-0.5.7/pylusat.egg-info/top_level.txt
--rw-r--r--   0 changjiechen   (501) staff       (20)       38 2022-10-20 21:21:03.554144 pylusat-0.5.7/setup.cfg
--rw-r--r--   0 changjiechen   (501) staff       (20)     1488 2022-09-29 19:59:10.000000 pylusat-0.5.7/setup.py
+drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2023-06-15 19:35:00.722341 pylusat-0.5.8/
+-rw-r--r--   0 changjiechen   (501) staff       (20)     1498 2022-09-29 14:35:28.000000 pylusat-0.5.8/LICENSE.txt
+-rw-r--r--   0 changjiechen   (501) staff       (20)     1981 2023-06-15 19:35:00.722144 pylusat-0.5.8/PKG-INFO
+-rw-r--r--   0 changjiechen   (501) staff       (20)     1038 2022-09-29 14:35:28.000000 pylusat-0.5.8/README.md
+drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2023-06-15 19:35:00.669373 pylusat-0.5.8/pylusat/
+-rw-r--r--   0 changjiechen   (501) staff       (20)       41 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/__init__.py
+-rw-r--r--   0 changjiechen   (501) staff       (20)       22 2023-06-15 19:25:27.000000 pylusat-0.5.8/pylusat/_version.py
+-rw-r--r--   0 changjiechen   (501) staff       (20)    11007 2023-06-15 17:45:03.000000 pylusat-0.5.8/pylusat/base.py
+drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2023-06-15 19:35:00.670376 pylusat-0.5.8/pylusat/datasets/
+-rw-r--r--   0 changjiechen   (501) staff       (20)     1476 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/__init__.py
+drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2023-06-15 19:35:00.673776 pylusat-0.5.8/pylusat/datasets/acs2016/
+-rw-r--r--   0 changjiechen   (501) staff       (20)        5 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/acs2016/acs2016.CPG
+-rw-r--r--   0 changjiechen   (501) staff       (20)    46559 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/acs2016/acs2016.dbf
+-rw-r--r--   0 changjiechen   (501) staff       (20)      501 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/acs2016/acs2016.prj
+-rw-r--r--   0 changjiechen   (501) staff       (20)     1692 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/acs2016/acs2016.sbn
+-rw-r--r--   0 changjiechen   (501) staff       (20)      228 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/acs2016/acs2016.sbx
+-rw-r--r--   0 changjiechen   (501) staff       (20)   521324 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/acs2016/acs2016.shp
+-rw-r--r--   0 changjiechen   (501) staff       (20)   216105 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/acs2016/acs2016.shp.xml
+-rw-r--r--   0 changjiechen   (501) staff       (20)     1340 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/acs2016/acs2016.shx
+drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2023-06-15 19:35:00.680810 pylusat-0.5.8/pylusat/datasets/habitat/
+-rw-r--r--   0 changjiechen   (501) staff       (20)       91 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/habitat/habitat.tfw
+-rw-r--r--   0 changjiechen   (501) staff       (20)  4201504 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/habitat/habitat.tif
+-rw-r--r--   0 changjiechen   (501) staff       (20)     1481 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/habitat/habitat.tif.aux.xml
+-rw-r--r--   0 changjiechen   (501) staff       (20)   313777 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/habitat/habitat.tif.ovr
+-rw-r--r--   0 changjiechen   (501) staff       (20)        5 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/habitat/habitat.tif.vat.cpg
+-rw-r--r--   0 changjiechen   (501) staff       (20)      908 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/habitat/habitat.tif.vat.dbf
+drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2023-06-15 19:35:00.684031 pylusat-0.5.8/pylusat/datasets/habitat_fl_stateplane/
+-rw-r--r--   0 changjiechen   (501) staff       (20)       92 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tfw
+-rw-r--r--   0 changjiechen   (501) staff       (20)   759776 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif
+-rw-r--r--   0 changjiechen   (501) staff       (20)     1599 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif.aux.xml
+-rw-r--r--   0 changjiechen   (501) staff       (20)   315409 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif.ovr
+-rw-r--r--   0 changjiechen   (501) staff       (20)        5 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif.vat.cpg
+-rw-r--r--   0 changjiechen   (501) staff       (20)      908 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif.vat.dbf
+-rw-r--r--   0 changjiechen   (501) staff       (20)     8412 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif.xml
+drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2023-06-15 19:35:00.686984 pylusat-0.5.8/pylusat/datasets/habitat_shift/
+-rw-r--r--   0 changjiechen   (501) staff       (20)       91 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/habitat_shift/habitat_shift.tfw
+-rw-r--r--   0 changjiechen   (501) staff       (20)   755954 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/habitat_shift/habitat_shift.tif
+-rw-r--r--   0 changjiechen   (501) staff       (20)     1479 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/habitat_shift/habitat_shift.tif.aux.xml
+-rw-r--r--   0 changjiechen   (501) staff       (20)   314738 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/habitat_shift/habitat_shift.tif.ovr
+-rw-r--r--   0 changjiechen   (501) staff       (20)        5 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/habitat_shift/habitat_shift.tif.vat.cpg
+-rw-r--r--   0 changjiechen   (501) staff       (20)      968 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/habitat_shift/habitat_shift.tif.vat.dbf
+-rw-r--r--   0 changjiechen   (501) staff       (20)     7091 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/habitat_shift/habitat_shift.tif.xml
+drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2023-06-15 19:35:00.688810 pylusat-0.5.8/pylusat/datasets/highway/
+-rw-r--r--   0 changjiechen   (501) staff       (20)        5 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/highway/highway.cpg
+-rw-r--r--   0 changjiechen   (501) staff       (20)     8348 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/highway/highway.dbf
+-rw-r--r--   0 changjiechen   (501) staff       (20)      501 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/highway/highway.prj
+-rw-r--r--   0 changjiechen   (501) staff       (20)      628 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/highway/highway.sbn
+-rw-r--r--   0 changjiechen   (501) staff       (20)      164 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/highway/highway.sbx
+-rw-r--r--   0 changjiechen   (501) staff       (20)    25276 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/highway/highway.shp
+-rw-r--r--   0 changjiechen   (501) staff       (20)   136966 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/highway/highway.shp.xml
+-rw-r--r--   0 changjiechen   (501) staff       (20)      508 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/highway/highway.shx
+drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2023-06-15 19:35:00.691251 pylusat-0.5.8/pylusat/datasets/schools/
+-rw-r--r--   0 changjiechen   (501) staff       (20)        5 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/schools/schools.CPG
+-rw-r--r--   0 changjiechen   (501) staff       (20)    37743 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/schools/schools.dbf
+-rw-r--r--   0 changjiechen   (501) staff       (20)      501 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/schools/schools.prj
+-rw-r--r--   0 changjiechen   (501) staff       (20)     1396 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/schools/schools.sbn
+-rw-r--r--   0 changjiechen   (501) staff       (20)      196 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/schools/schools.sbx
+-rw-r--r--   0 changjiechen   (501) staff       (20)     3488 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/schools/schools.shp
+-rw-r--r--   0 changjiechen   (501) staff       (20)   263975 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/schools/schools.shp.xml
+-rw-r--r--   0 changjiechen   (501) staff       (20)     1068 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/schools/schools.shx
+drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2023-06-15 19:35:00.719144 pylusat-0.5.8/pylusat/datasets/streets/
+-rw-r--r--   0 changjiechen   (501) staff       (20)        5 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/streets/streets.CPG
+-rw-r--r--   0 changjiechen   (501) staff       (20)  8317235 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/streets/streets.dbf
+-rw-r--r--   0 changjiechen   (501) staff       (20)      501 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/streets/streets.prj
+-rw-r--r--   0 changjiechen   (501) staff       (20)   214284 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/streets/streets.sbn
+-rw-r--r--   0 changjiechen   (501) staff       (20)    12588 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/streets/streets.sbx
+-rw-r--r--   0 changjiechen   (501) staff       (20)  3467420 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/streets/streets.shp
+-rw-r--r--   0 changjiechen   (501) staff       (20)    38406 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/streets/streets.shp.xml
+-rw-r--r--   0 changjiechen   (501) staff       (20)   169388 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/datasets/streets/streets.shx
+-rw-r--r--   0 changjiechen   (501) staff       (20)     7527 2022-10-20 21:03:25.000000 pylusat-0.5.8/pylusat/density.py
+-rw-r--r--   0 changjiechen   (501) staff       (20)     7055 2022-10-20 21:03:25.000000 pylusat-0.5.8/pylusat/distance.py
+-rw-r--r--   0 changjiechen   (501) staff       (20)    13007 2023-06-15 17:38:40.000000 pylusat-0.5.8/pylusat/geotools.py
+-rw-r--r--   0 changjiechen   (501) staff       (20)     4464 2022-10-20 21:03:25.000000 pylusat-0.5.8/pylusat/interpolate.py
+-rw-r--r--   0 changjiechen   (501) staff       (20)     7186 2022-10-20 21:03:25.000000 pylusat-0.5.8/pylusat/rescale.py
+drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2023-06-15 19:35:00.721828 pylusat-0.5.8/pylusat/tests/
+-rw-r--r--   0 changjiechen   (501) staff       (20)        0 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/tests/__init__.py
+-rw-r--r--   0 changjiechen   (501) staff       (20)     1060 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/tests/test_base.py
+-rw-r--r--   0 changjiechen   (501) staff       (20)      971 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/tests/test_density.py
+-rw-r--r--   0 changjiechen   (501) staff       (20)      820 2022-09-29 18:54:56.000000 pylusat-0.5.8/pylusat/tests/test_distance.py
+-rw-r--r--   0 changjiechen   (501) staff       (20)     1439 2023-06-15 17:59:38.000000 pylusat-0.5.8/pylusat/tests/test_geotools.py
+-rw-r--r--   0 changjiechen   (501) staff       (20)      475 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/tests/test_interpolate.py
+-rw-r--r--   0 changjiechen   (501) staff       (20)      338 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/tests/test_rescale.py
+-rw-r--r--   0 changjiechen   (501) staff       (20)       34 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/tests/test_utils.py
+-rw-r--r--   0 changjiechen   (501) staff       (20)     1026 2022-09-29 14:35:28.000000 pylusat-0.5.8/pylusat/tests/test_zonal.py
+-rw-r--r--   0 changjiechen   (501) staff       (20)     7596 2022-10-20 21:03:25.000000 pylusat-0.5.8/pylusat/utils.py
+-rw-r--r--   0 changjiechen   (501) staff       (20)     3748 2022-10-20 21:03:25.000000 pylusat-0.5.8/pylusat/zonal.py
+drwxr-xr-x   0 changjiechen   (501) staff       (20)        0 2023-06-15 19:35:00.670212 pylusat-0.5.8/pylusat.egg-info/
+-rw-r--r--   0 changjiechen   (501) staff       (20)     1981 2023-06-15 19:35:00.000000 pylusat-0.5.8/pylusat.egg-info/PKG-INFO
+-rw-r--r--   0 changjiechen   (501) staff       (20)     2981 2023-06-15 19:35:00.000000 pylusat-0.5.8/pylusat.egg-info/SOURCES.txt
+-rw-r--r--   0 changjiechen   (501) staff       (20)        1 2023-06-15 19:35:00.000000 pylusat-0.5.8/pylusat.egg-info/dependency_links.txt
+-rw-r--r--   0 changjiechen   (501) staff       (20)       37 2023-06-15 19:35:00.000000 pylusat-0.5.8/pylusat.egg-info/requires.txt
+-rw-r--r--   0 changjiechen   (501) staff       (20)        8 2023-06-15 19:35:00.000000 pylusat-0.5.8/pylusat.egg-info/top_level.txt
+-rw-r--r--   0 changjiechen   (501) staff       (20)       38 2023-06-15 19:35:00.722409 pylusat-0.5.8/setup.cfg
+-rw-r--r--   0 changjiechen   (501) staff       (20)     1488 2022-09-29 19:59:10.000000 pylusat-0.5.8/setup.py
```

### Comparing `pylusat-0.5.7/LICENSE.txt` & `pylusat-0.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/PKG-INFO` & `pylusat-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylusat
-Version: 0.5.7
+Version: 0.5.8
 Summary: Python for Land-use suitability analysis tools
 Home-page: https://github.com/chjch/pylusat
 Author: Changjie Chen
 Author-email: chj.chen@hotmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pylusat-0.5.7/README.md` & `pylusat-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/base.py` & `pylusat-0.5.8/pylusat/base.py`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/__init__.py` & `pylusat-0.5.8/pylusat/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/acs2016/acs2016.dbf` & `pylusat-0.5.8/pylusat/datasets/acs2016/acs2016.dbf`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/acs2016/acs2016.sbn` & `pylusat-0.5.8/pylusat/datasets/acs2016/acs2016.sbn`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/acs2016/acs2016.shp` & `pylusat-0.5.8/pylusat/datasets/acs2016/acs2016.shp`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/acs2016/acs2016.shp.xml` & `pylusat-0.5.8/pylusat/datasets/acs2016/acs2016.shp.xml`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/acs2016/acs2016.shx` & `pylusat-0.5.8/pylusat/datasets/acs2016/acs2016.shx`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/habitat/habitat.tif` & `pylusat-0.5.8/pylusat/datasets/habitat/habitat.tif`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/habitat/habitat.tif.aux.xml` & `pylusat-0.5.8/pylusat/datasets/habitat/habitat.tif.aux.xml`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/habitat/habitat.tif.ovr` & `pylusat-0.5.8/pylusat/datasets/habitat/habitat.tif.ovr`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/habitat/habitat.tif.vat.dbf` & `pylusat-0.5.8/pylusat/datasets/habitat/habitat.tif.vat.dbf`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif` & `pylusat-0.5.8/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif.aux.xml` & `pylusat-0.5.8/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif.aux.xml`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif.ovr` & `pylusat-0.5.8/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif.ovr`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif.vat.dbf` & `pylusat-0.5.8/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif.vat.dbf`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif.xml` & `pylusat-0.5.8/pylusat/datasets/habitat_fl_stateplane/habitat_fl_stateplane.tif.xml`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/habitat_shift/habitat_shift.tif` & `pylusat-0.5.8/pylusat/datasets/habitat_shift/habitat_shift.tif`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/habitat_shift/habitat_shift.tif.aux.xml` & `pylusat-0.5.8/pylusat/datasets/habitat_shift/habitat_shift.tif.aux.xml`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/habitat_shift/habitat_shift.tif.ovr` & `pylusat-0.5.8/pylusat/datasets/habitat_shift/habitat_shift.tif.ovr`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/habitat_shift/habitat_shift.tif.vat.dbf` & `pylusat-0.5.8/pylusat/datasets/habitat_shift/habitat_shift.tif.vat.dbf`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/habitat_shift/habitat_shift.tif.xml` & `pylusat-0.5.8/pylusat/datasets/habitat_shift/habitat_shift.tif.xml`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/highway/highway.dbf` & `pylusat-0.5.8/pylusat/datasets/highway/highway.dbf`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/highway/highway.sbn` & `pylusat-0.5.8/pylusat/datasets/highway/highway.sbn`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/highway/highway.shp` & `pylusat-0.5.8/pylusat/datasets/highway/highway.shp`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/highway/highway.shp.xml` & `pylusat-0.5.8/pylusat/datasets/highway/highway.shp.xml`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/schools/schools.dbf` & `pylusat-0.5.8/pylusat/datasets/schools/schools.dbf`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/schools/schools.sbn` & `pylusat-0.5.8/pylusat/datasets/schools/schools.sbn`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/schools/schools.shp` & `pylusat-0.5.8/pylusat/datasets/schools/schools.shp`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/schools/schools.shp.xml` & `pylusat-0.5.8/pylusat/datasets/schools/schools.shp.xml`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/schools/schools.shx` & `pylusat-0.5.8/pylusat/datasets/schools/schools.shx`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/streets/streets.dbf` & `pylusat-0.5.8/pylusat/datasets/streets/streets.dbf`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/streets/streets.sbn` & `pylusat-0.5.8/pylusat/datasets/streets/streets.sbn`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/streets/streets.sbx` & `pylusat-0.5.8/pylusat/datasets/streets/streets.sbx`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/streets/streets.shp` & `pylusat-0.5.8/pylusat/datasets/streets/streets.shp`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/streets/streets.shp.xml` & `pylusat-0.5.8/pylusat/datasets/streets/streets.shp.xml`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/datasets/streets/streets.shx` & `pylusat-0.5.8/pylusat/datasets/streets/streets.shx`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/density.py` & `pylusat-0.5.8/pylusat/density.py`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/distance.py` & `pylusat-0.5.8/pylusat/distance.py`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/geotools.py` & `pylusat-0.5.8/pylusat/geotools.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 import geopandas as gpd
-from geopandas import GeoDataFrame
 import pandas as pd
 from typing import Dict
 from shapely.geometry import Polygon
 from rasterio.io import MemoryFile
 from pylusat.base import RasterManager
 
 
@@ -268,47 +267,57 @@
                            crs=out_crs, width=out_width, height=out_height,
                            transform=geo_tform, nodata=out_nd, tiled=False)
         rst.write(output_arr, indexes=1)
         rst.close()
         return memfile.open(driver="GTiff"), attr
 
 
-def gridify(input_gdf, width=None, height=None, num_cols=None, num_rows=None):
+def gridify(input_gdf, cell_x=None, cell_y=None, n_cols=None, n_rows=None):
     """
-    Create a grid based on the input_gdf by specifying width and/or height of
-    the cells of the grid.
+    Create a grid covering the extent of the input_gdf based on either
+    (cell_x, celly_y) or (n_cols, n_rows).
 
-    num_cols and num_rows can be used to define the grid as well. If nothing
-    specified, the cell size of the grid will be the span on x axis (width)
-    divided by 30.
+    If both are specified, (cell_x, cell_y) will be used.
+
+    If neither are specified, the cell size will be calcualted based on the
+    input_gdf's width (length of x-axis) divided by 30.
 
     Parameters
     ----------
     input_gdf : geopandas.GeoDataFrame
         Input GeoDataFrame based on which the grid is created.
-    width : int or float
-        Cell width.
-    height : int or float
-        Cell height.
-    num_cols : int
-        Number of columns. When specified, this number will determine cell
-        width.
-    num_rows : int
-        Number of rows. When specified, this number will determine cell height.
+    cell_x : int or float
+        Cell size on the x-axis.
+    cell_y : int or float
+        Cell cell_y.
+    n_cols : int
+        Number of columns. When specified, this number will determine cell_x
+        (i.e., input_gdf's width divided by `n_cols`).
+    n_rows : int
+        Number of rows. When specified, this number will determine cell_y
+        (input_gdf's height divided by `n_rows`).
 
     Returns
     -------
     geopandas.GeoDataFrame
         The output grid (polygons).
 
+    Notes
+    _____
+    `cell_x` and `cell_y` are in the same unit as the input_gdf's CRS.
+
+    The output grid will have the same CRS as the input_gdf. The CRS of the
+    input_gdf must be projected (not geographic).
+
     Examples
     --------
-    Create grid of polygons from the schools GeoDataFrame with a width of 1000
+    Create grid of polygons from the schools GeoDataFrame with a cell size
+    of 1000 (meters).
 
-    >>> pylusat.geotools.gridify(schools_gdf, width=1000)
+    >>> pylusat.geotools.gridify(schools_gdf, cell_x=1000)
     0       POLYGON ((533359.960 611556.855, 534359.960...))
     1       POLYGON ((534359.960 611556.855, 535359.960...))
     2       POLYGON ((535359.960 611556.855, 536359.960...))
     3       POLYGON ((536359.960 611556.855, 537359.960...))
     4       POLYGON ((537359.960 611556.855, 538359.960...))
     ...
     2491    POLYGON ((580359.960 658556.855, 581359.960...))
@@ -316,45 +325,43 @@
     2493    POLGYON ((582359.960 658556.855, 583359.960...))
     2494    POLYGON ((583359.960 658556.855, 584359.960...))
     2495    POLGYON ((584359.960 658556.855, 585359.960...))
     
     """
     xmin, ymin, xmax, ymax = input_gdf.total_bounds
 
-    if width and height:
-        pass
-    else:
-        if not width and not height:
-            width = height = (xmax - xmin) / 30
-        else:
-            if width:
-                height = width
-            elif height:
-                width = height
-
-    if num_cols and num_rows:
-        # width and height are calculated based on num_cols and num_rows
-        width = (xmax - xmin) / num_cols
-        height = (ymax - ymin) / num_rows
-    else:
-        if num_cols:
-            width = height = (xmax - xmin) / num_cols
-        elif num_rows:
-            height = width = (ymax - ymin) / num_rows
+    if not cell_x and not cell_y:
+        if n_cols and n_rows:
+            # cell_x and cell_y are calculated based on n_cols and n_rows
+            cell_x = (xmax - xmin) / n_cols
+            cell_y = (ymax - ymin) / n_rows
+        elif n_cols and not n_rows:
+            cell_y = cell_x = (xmax - xmin) / n_cols
+        elif n_rows and not n_cols:
+            cell_y = cell_x = (ymax - ymin) / n_rows
         else:
-            pass
+            cell_x = cell_y = (xmax - xmin) / 30
+    elif not cell_x and cell_y:
+        cell_x = cell_y
+    elif cell_x and not cell_y:
+        cell_y = cell_x
+
+    new_xmin = xmin//cell_x*cell_x
+    new_xmax = xmax//cell_x*cell_x + cell_x
+    new_ymin = ymin//cell_y*cell_y
+    new_ymax = ymax//cell_y*cell_y + cell_y
 
-    cols = np.arange(xmin - width/2, xmax + width/2, width)
-    rows = np.arange(ymin - height/2, ymax + height/2, height)
+    cols = np.arange(new_xmin, new_xmax + cell_x, cell_x)
+    rows = np.arange(new_ymin, new_ymax + cell_y, cell_y)
 
     polygons = [
         Polygon([
             (x, y),
-            (x+width, y),
-            (x+width, y+height),
-            (x, y+height)
+            (x + cell_x, y),
+            (x + cell_x, y + cell_y),
+            (x, y + cell_y)
         ])
         for y in rows
         for x in cols
     ]
 
-    return GeoDataFrame({'geometry': polygons}, crs=input_gdf.crs)
+    return gpd.GeoDataFrame({'geometry': polygons}, crs=input_gdf.crs)
```

### Comparing `pylusat-0.5.7/pylusat/interpolate.py` & `pylusat-0.5.8/pylusat/interpolate.py`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/rescale.py` & `pylusat-0.5.8/pylusat/rescale.py`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/tests/test_base.py` & `pylusat-0.5.8/pylusat/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/tests/test_density.py` & `pylusat-0.5.8/pylusat/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/tests/test_distance.py` & `pylusat-0.5.8/pylusat/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/tests/test_geotools.py` & `pylusat-0.5.8/pylusat/tests/test_geotools.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,9 +45,12 @@
 def test_combine_rio_ds(habitat_rio):
     rast_obj, attr = combine(habitat_rio, habitat_rio)
     assert len(attr) == 29
     assert attr['count'][attr.value == 1][0] == 618688
 
 
 def test_gridify(schools_gdf):
-    result = gridify(schools_gdf, width=1000)
-    assert len(result) == 2496
+    cell_x = 1000
+    result = gridify(schools_gdf, cell_x=cell_x)
+    assert len(result) == 2544
+    assert abs(result.total_bounds[0] - schools_gdf.total_bounds[0]) < cell_x
+    assert result.total_bounds[0] % cell_x == 0
```

### Comparing `pylusat-0.5.7/pylusat/tests/test_zonal.py` & `pylusat-0.5.8/pylusat/tests/test_zonal.py`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/utils.py` & `pylusat-0.5.8/pylusat/utils.py`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat/zonal.py` & `pylusat-0.5.8/pylusat/zonal.py`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/pylusat.egg-info/PKG-INFO` & `pylusat-0.5.8/pylusat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylusat
-Version: 0.5.7
+Version: 0.5.8
 Summary: Python for Land-use suitability analysis tools
 Home-page: https://github.com/chjch/pylusat
 Author: Changjie Chen
 Author-email: chj.chen@hotmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pylusat-0.5.7/pylusat.egg-info/SOURCES.txt` & `pylusat-0.5.8/pylusat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylusat-0.5.7/setup.py` & `pylusat-0.5.8/setup.py`

 * *Files identical despite different names*

