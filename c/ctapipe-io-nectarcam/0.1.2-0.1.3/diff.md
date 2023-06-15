# Comparing `tmp/ctapipe_io_nectarcam-0.1.2.tar.gz` & `tmp/ctapipe_io_nectarcam-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctapipe_io_nectarcam-0.1.2.tar", last modified: Thu Mar 23 14:02:12 2023, max compression
+gzip compressed data, was "ctapipe_io_nectarcam-0.1.3.tar", last modified: Thu Jun 15 14:05:23 2023, max compression
```

## Comparing `ctapipe_io_nectarcam-0.1.2.tar` & `ctapipe_io_nectarcam-0.1.3.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:02:12.556382 ctapipe_io_nectarcam-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:02:12.552381 ctapipe_io_nectarcam-0.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:02:12.552381 ctapipe_io_nectarcam-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-03-23 14:02:12.556382 ctapipe_io_nectarcam-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-03-23 14:02:12.556382 ctapipe_io_nectarcam-0.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:02:12.552381 ctapipe_io_nectarcam-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:02:12.552381 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/
--rw-r--r--   0 runner    (1001) docker     (123)    28515 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-23 14:02:12.000000 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/anyarray_dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/containers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:02:12.556382 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/resources/NectarCam-003.camgeom.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    11391 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/resources/Pulse_template_nectarCam_17042020.dat
--rw-r--r--   0 runner    (1001) docker     (123)   881677 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/resources/calibrationfile_run3255_pedrun3255_gainrun3155.hdf5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:02:12.556382 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/tests/test_nectarcameventsource.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-23 14:02:08.000000 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:02:12.556382 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-03-23 14:02:12.000000 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-23 14:02:12.000000 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 14:02:12.000000 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 14:02:12.000000 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-23 14:02:12.000000 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-23 14:02:12.000000 ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:05:23.554636 ctapipe_io_nectarcam-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:05:23.546635 ctapipe_io_nectarcam-0.1.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:05:23.550636 ctapipe_io_nectarcam-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-15 14:05:23.554636 ctapipe_io_nectarcam-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-15 14:05:23.554636 ctapipe_io_nectarcam-0.1.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:05:23.546635 ctapipe_io_nectarcam-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:05:23.550636 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/
+-rw-r--r--   0 runner    (1001) docker     (123)    31424 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-15 14:05:23.000000 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/anyarray_dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/containers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:05:23.550636 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/resources/NectarCam-003.camgeom.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    11391 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/resources/Pulse_template_nectarCam_17042020.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   881677 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/resources/calibrationfile_run3255_pedrun3255_gainrun3155.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)   882754 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/resources/calibrationfile_run3255_pedrun3255_gainrun3155_ctapipe018.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:05:23.554636 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/tests/test_nectarcameventsource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-15 14:05:14.000000 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:05:23.550636 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-15 14:05:23.000000 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-15 14:05:23.000000 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:05:23.000000 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-15 14:05:23.000000 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:05:23.000000 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-15 14:05:23.000000 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 14:05:23.000000 ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam.egg-info/top_level.txt
```

### Comparing `ctapipe_io_nectarcam-0.1.2/.github/workflows/ci.yml` & `ctapipe_io_nectarcam-0.1.3/.github/workflows/ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,16 @@
   PYTEST_ADDOPTS: --color=yes
 
 jobs:
   tests:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.8]
-        ctapipe-version: [v0.12.0]
+        python-version: [3.9]
+        ctapipe-version: [v0.19.2]
 
     defaults:
       run:
         shell: bash -leo pipefail {0}
 
     steps:
       - uses: actions/checkout@v3
```

### Comparing `ctapipe_io_nectarcam-0.1.2/.github/workflows/deploy.yml` & `ctapipe_io_nectarcam-0.1.3/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.2/.gitignore` & `ctapipe_io_nectarcam-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.2/LICENSE.md` & `ctapipe_io_nectarcam-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.2/PKG-INFO` & `ctapipe_io_nectarcam-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: ctapipe_io_nectarcam
-Version: 0.1.2
+Version: 0.1.3
 Summary: ctapipe plugin for reading NectarCam files
 Author: NectarCAM collaboration
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/cta-observatory/ctapipe_io_nectarcam/issues
 Project-URL: Source Code, https://github.com/cta-observatory/ctapipe_io_nectarcam
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: ~=3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: tests
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE.md
 
 [![CI](https://github.com/cta-observatory/ctapipe_io_nectarcam/workflows/CI/badge.svg?branch=master)](https://github.com/cta-observatory/ctapipe_io_nectarcam/actions?query=workflow%3ACI+branch%3Amaster)
```

### Comparing `ctapipe_io_nectarcam-0.1.2/README.md` & `ctapipe_io_nectarcam-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.2/setup.cfg` & `ctapipe_io_nectarcam-0.1.3/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -11,28 +11,24 @@
 classifiers = 
 	Development Status :: 3 - Alpha
 	License :: OSI Approved :: BSD License
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering :: Astronomy
 	Topic :: Scientific/Engineering :: Physics
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
 
 [options]
 packages = find:
 package_dir = 
 	= src
-python_requires = ~=3.8
 zip_safe = False
 install_requires = 
-	astropy~=4.2
-	ctapipe~=0.12
-	numpy~=1.22
-	protozfits~=2.0
-	tables>=3.7
+	ctapipe~=0.19
+	protozfits # ~=2.0
 
 [options.package_data]
 * = resources/*
 
 [options.packages.find]
 where = src
 exclude = 
@@ -43,14 +39,18 @@
 	pytest
 dev = 
 	setuptools_scm[toml]
 all = 
 	%(tests)s
 	%(dev)s
 
+[options.entry_points]
+ctapipe_io = 
+	NectarCAMEventSource = ctapipe_io_nectarcam:NectarCAMEventSource
+
 [tool:pytest]
 minversion = 3.0
 addopts = -v
 
 [aliases]
 test = pytest
```

### Comparing `ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/__init__.py` & `ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,27 +9,31 @@
 import numpy as np
 import struct
 from astropy import units as u
 from astropy.io import fits
 from astropy.time import Time
 from ctapipe.containers import (
     PixelStatusContainer, EventType, R0CameraContainer, R1CameraContainer,
+    CoordinateFrameType, PointingMode, SchedulingBlockContainer, ObservationBlockContainer, # VIM : line of things in lst equivalent
 )
 from ctapipe.coordinates import CameraFrame
 from ctapipe.core import Provenance
 from ctapipe.core.traits import Int, Bool, Enum
 from ctapipe.instrument import (
     TelescopeDescription,
     SubarrayDescription,
     CameraDescription,
     CameraReadout,
     CameraGeometry,
     OpticsDescription,
+    SizeType,
+    ReflectorShape
 )
-from ctapipe.io import EventSource
+
+from ctapipe.io import EventSource, DataLevel
 from enum import IntFlag, auto
 from pkg_resources import resource_filename
 
 from .calibration import NectarCAMR0Corrections
 from .constants import (
     N_GAINS, N_PIXELS, N_SAMPLES
 )
@@ -42,15 +46,14 @@
 )
 from .version import __version__
 
 __all__ = ['NectarCAMEventSource', '__version__']
 
 S_TO_NS = np.uint64(1e9)
 
-
 class TriggerBits(IntFlag):
     '''
     See TIB User manual
     '''
     UNKNOWN = 0
     MONO = auto()
     STEREO = auto()
@@ -82,18 +85,21 @@
     BOTH_GAINS_STORED = HIGH_GAIN_STORED | LOW_GAIN_STORED
 
 
 OPTICS = OpticsDescription(
     # https://gitlab.cta-observatory.org/cta-science/simulations/simulation-model/verification/verification-process/mst-structure/-/blob/master/Appendix-MST-Structure.pdf
     # version from 20 Jan 2022
     'MST',
+    size_type=SizeType.MST,
     equivalent_focal_length=u.Quantity(16., u.m),
-    num_mirrors=1,
+    effective_focal_length=u.Quantity(16.44505,u.m), # from https://www.mpi-hd.mpg.de/hfm/CTA/MC/Prod5/Config/PSF/fov_prod4.pdf mentioned in the link above
+    n_mirrors=1,
     mirror_area=u.Quantity(106., u.m ** 2),  # no shadowing, uncertainty is 0.5 m2
-    num_mirror_tiles=86,  # Garczarczyk 2017
+    n_mirror_tiles=86,  # Garczarczyk 2017
+    reflector_shape=ReflectorShape.HYBRID #according to Dan Parsons
 )
 
 
 def load_camera_geometry(version=3):
     ''' Load camera geometry from bundled resources of this repo '''
     f = resource_filename(
         'ctapipe_io_nectarcam', f'resources/NectarCam-{version:03d}.camgeom.fits.gz'
@@ -199,30 +205,82 @@
         # the specified file mask (copied from  MAGICEventSourceROOT).
 
         if 'input_url' in kwargs.keys():
             self.file_list = glob.glob(str(kwargs['input_url']))
             self.file_list.sort()
             kwargs['input_url'] = self.file_list[0]
             super().__init__(**kwargs)
+        elif 'input_filelist' in kwargs.keys():
+            input_filelist = kwargs['input_filelist']
+            if isinstance(input_filelist,str):
+                self.file_list = [input_filelist]
+            else:
+                self.file_list = list(input_filelist)
+            self.file_list.sort()
+            kwargs['input_url'] = self.file_list[0]
+            del kwargs['input_filelist']
+            super().__init__(**kwargs)
         else:
             super().__init__(**kwargs)
             self.file_list = [self.input_url]
 
         self.multi_file = MultiFiles(self.file_list)
         self.camera_config = self.multi_file.camera_config
         self.log.info("Read {} input files".format(self.multi_file.num_inputs()))
-        self._tel_id = self.camera_config.telescope_id
+        self.run_id = self.camera_config.configuration_id
+        self.tel_id = self.camera_config.telescope_id #VIM : Change the _tel_id to tel_id to be consistent with lst
+        self.run_start = Time(self.camera_config.date, format='unix')
         self.geometry_version = 3
-        self._subarray = self.create_subarray(self.geometry_version, self._tel_id)
+        self._subarray = self.create_subarray(self.geometry_version, self.tel_id)
         self.r0_r1_calibrator = NectarCAMR0Corrections(
-            subarray=self._subarray, parent=self
-        )
-        self.nectarcam_service = self.fill_nectarcam_service_container_from_zfile(self._tel_id,
+             subarray=self._subarray, parent=self
+         )
+        self.nectarcam_service = self.fill_nectarcam_service_container_from_zfile(self.tel_id,
                                                                                   self.camera_config)
 
+        target_info = {}
+
+        # VIM : Put some pointing info to be filled as a reminder that it should be done at some point
+        #self.pointing_source = PointingSource(subarray=self.subarray, parent=self)
+        pointing_mode = PointingMode.UNKNOWN
+        #if self.pointing_information:
+        #    target = self.pointing_source.get_target(tel_id=self.tel_id, time=self.run_start)
+        #    if target is not None:
+        #        target_info["subarray_pointing_lon"] = target["ra"]
+        #        target_info["subarray_pointing_lat"] = target["dec"]
+        #        target_info["subarray_pointing_frame"] = CoordinateFrameType.ICRS
+        #        pointing_mode = PointingMode.TRACK
+
+        self._scheduling_blocks = {
+            self.run_id: SchedulingBlockContainer(
+                sb_id=np.uint64(self.run_id),
+                producer_id=f"MST-{self.tel_id}",
+                pointing_mode=pointing_mode,
+            )
+        }
+
+        self._observation_blocks = {
+            self.run_id: ObservationBlockContainer(
+                obs_id=np.uint64(self.run_id),
+                sb_id=np.uint64(self.run_id),
+                producer_id=f"MST-{self.tel_id}",
+                actual_start_time=self.run_start,
+                **target_info
+            )
+        }
+
+    def get_entries(self):
+        tot_events = 0
+        for v in self.multi_file._events_table.values():
+            tot_events += len(v)
+        return tot_events
+
+    def __len__(self):
+        return self.get_entries()
+
     @property
     def is_simulation(self):
         return False
 
     @property
     def datalevels(self):
         if self.r0_r1_calibrator.calibration_path is not None:
@@ -245,24 +303,27 @@
         # camera info from NectarCAM-[geometry_version].camgeom.fits.gz file
         camera_geom = load_camera_geometry(version=geometry_version)
 
         # get info on the camera readout:
         daq_time_per_sample, pulse_shape_time_step, pulse_shapes = read_pulse_shapes()
 
         camera_readout = CameraReadout(
-            'NectarCam',
-            1 / daq_time_per_sample,
-            pulse_shapes,
-            pulse_shape_time_step,
+            name = 'NectarCam',
+            n_pixels=N_PIXELS,
+            n_channels=N_GAINS,
+            n_samples=N_SAMPLES,
+            sampling_rate = (1 / daq_time_per_sample).to(u.GHz),
+            reference_pulse_shape = pulse_shapes,
+            reference_pulse_sample_width = pulse_shape_time_step,
         )
 
         camera = CameraDescription('NectarCam', camera_geom, camera_readout)
 
         mst_tel_descr = TelescopeDescription(
-            name='NectarCam', tel_type='MST', optics=OPTICS, camera=camera
+            name='NectarCam', optics=OPTICS, camera=camera
         )
 
         tel_descriptions = {tel_id: mst_tel_descr}
 
         # MST telescope position
         tel_positions = {tel_id: [0., 0., 0] * u.m}
 
@@ -270,29 +331,38 @@
             name=f"MST-{tel_id} subarray",
             tel_descriptions=tel_descriptions,
             tel_positions=tel_positions,
         )
 
         return subarray
 
+
+    @property
+    def observation_blocks(self):
+        return self._observation_blocks
+
+    @property
+    def scheduling_blocks(self):
+        return self._scheduling_blocks
+
     @property
     def obs_ids(self):
         # currently no obs id is available from the input files
         return [self.camera_config.configuration_id, ]
 
     def _generator(self):
 
         # container for NectarCAM data
         array_event = NectarCAMDataContainer()
         array_event.meta['input_url'] = self.input_url
         array_event.meta['max_events'] = self.max_events
         array_event.meta['origin'] = 'NectarCAM'
 
         # also add service container to the event section
-        array_event.nectarcam.tel[self._tel_id].svc = self.nectarcam_service
+        array_event.nectarcam.tel[self.tel_id].svc = self.nectarcam_service
 
         # initialize general monitoring container
         self.initialize_mon_container(array_event)
 
         # loop on events
         for count, event in enumerate(self.multi_file):
 
@@ -374,15 +444,15 @@
             idaq_version=camera_config.nectarcam.idaq_version,
             cdhs_version=camera_config.nectarcam.cdhs_version,
             algorithms=camera_config.nectarcam.algorithms,
         )
 
     def fill_nectarcam_event_container_from_zfile(self, array_event, event):
 
-        tel_id = self._tel_id
+        tel_id = self.tel_id
         event_container = NectarCAMEventContainer()
         array_event.nectarcam.tel[tel_id].evt = event_container
 
         event_container.configuration_id = event.configuration_id
         event_container.event_id = event.event_id
         event_container.tel_event_id = event.tel_event_id
         event_container.pixel_status = event.pixel_status
@@ -425,15 +495,15 @@
             event_container.ucts_num_in_bunch = unpacked_cdts[9]  # new
             event_container.cdts_version = unpacked_cdts[10]  # new
 
         # Unpack FEB counters and trigger pattern
         self.unpack_feb_data(event_container, event)
 
     def fill_trigger_info(self, array_event):
-        tel_id = self._tel_id
+        tel_id = self.tel_id
 
         nectarcam = array_event.nectarcam.tel[tel_id]
         tib_available = nectarcam.evt.extdevices_presence & 1
         ucts_available = nectarcam.evt.extdevices_presence & 2
 
         # fill trigger time using UCTS timestamp
         trigger = array_event.trigger
@@ -615,25 +685,25 @@
         return r0, r1
 
     def fill_r0r1_container(self, array_event, zfits_event):
         """
         Fill with R0Container
         """
         r0, r1 = self.fill_r0r1_camera_container(zfits_event)
-        array_event.r0.tel[self._tel_id] = r0
-        array_event.r1.tel[self._tel_id] = r1
+        array_event.r0.tel[self.tel_id] = r0
+        array_event.r1.tel[self.tel_id] = r1
 
     def initialize_mon_container(self, array_event):
         """
         Fill with MonitoringContainer.
         For the moment, initialize only the PixelStatusContainer
 
         """
         container = array_event.mon
-        mon_camera_container = container.tel[self._tel_id]
+        mon_camera_container = container.tel[self.tel_id]
 
         # initialize the container
         status_container = PixelStatusContainer()
 
         shape = (N_GAINS, N_PIXELS)
         status_container.hardware_failing_pixels = np.zeros(shape, dtype=bool)
         status_container.pedestal_failing_pixels = np.zeros(shape, dtype=bool)
@@ -644,15 +714,15 @@
     def fill_mon_container_from_zfile(self, array_event, event):
         """
         Fill with MonitoringContainer.
         For the moment, initialize only the PixelStatusContainer
 
         """
 
-        status_container = array_event.mon.tel[self._tel_id].pixel_status
+        status_container = array_event.mon.tel[self.tel_id].pixel_status
 
         # reorder the array
         pixel_status = np.zeros(N_PIXELS)
         pixel_status[self.camera_config.expected_pixels_id] = event.pixel_status
         status_container.hardware_failing_pixels[:] = pixel_status == 0
 
 class MultiFiles:
```

### Comparing `ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/anyarray_dtypes.py` & `ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/anyarray_dtypes.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/calibration.py` & `ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/calibration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import tables
 from ctapipe.calib.camera.gainselection import ThresholdGainSelector
-from ctapipe.containers import MonitoringContainer
+from ctapipe.containers import MonitoringContainer, MonitoringCameraContainer, FlatFieldContainer, WaveformCalibrationContainer
 from ctapipe.core import TelescopeComponent
 from ctapipe.core.traits import (
     Path, FloatTelescopeParameter, Bool, Float
 )
 from ctapipe.io import HDF5TableReader
 from pkg_resources import resource_filename
 
@@ -27,15 +27,15 @@
     usually performed on the raw data by the camera server.
     This calibrator exists in ctapipe_io_nectarcam for testing and prototyping purposes.
     """
 
     calibration_path = Path(
         default_value=resource_filename(
             'ctapipe_io_nectarcam',
-            'resources/calibrationfile_run3255_pedrun3255_gainrun3155.hdf5'
+            'resources/calibrationfile_run3255_pedrun3255_gainrun3155_ctapipe018.hdf5'
         ),
         exists=True, directory_ok=False, allow_none=True,
         help='Path to calibration file',
     ).tag(config=True)
 
     calib_scale_high_gain = FloatTelescopeParameter(
         default_value=1.0,
@@ -147,32 +147,32 @@
 
     @staticmethod
     def _read_calibration_file(path):
         """
         Read the correction from hdf5 calibration file
         Only calibration and flatfield containers are filled
         """
+
         mon = MonitoringContainer()
 
         with tables.open_file(path) as f:
             tel_ids = [
                 int(key[4:]) for key in f.root._v_children.keys()
                 if key.startswith('tel_')
             ]
 
         for tel_id in tel_ids:
             with HDF5TableReader(path) as h5_table:
-                base = f'/tel_{tel_id}'
-                # read the calibration data
-                table = base + '/calibration'
-                next(h5_table.read(table, mon.tel[tel_id].calibration))
-
-                # read flat-field data
-                table = base + '/flatfield'
-                next(h5_table.read(table, mon.tel[tel_id].flatfield))
+
+                mon.tel[tel_id] = MonitoringCameraContainer(
+                    calibration=next(h5_table.read(f'/tel_{tel_id}/calibration', WaveformCalibrationContainer)),
+                    flatfield=next(h5_table.read(f'/tel_{tel_id}/flatfield', FlatFieldContainer)),
+                    #pedestal=next(h5_table.read(f'/{base}/pedestal', PedestalContainer)),
+                    #pixel_status=next(h5_table.read(f"/{base}/pixel_status", PixelStatusContainer)),
+                )
 
         return mon
 
 
 def convert_to_pe(waveform, calibration, selected_gain_channel):
     if selected_gain_channel is None:
         waveform -= calibration.pedestal_per_sample
```

### Comparing `ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/containers.py` & `ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/containers.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/resources/NectarCam-003.camgeom.fits.gz` & `ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/resources/NectarCam-003.camgeom.fits.gz`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/resources/Pulse_template_nectarCam_17042020.dat` & `ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/resources/Pulse_template_nectarCam_17042020.dat`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/resources/calibrationfile_run3255_pedrun3255_gainrun3155.hdf5` & `ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/resources/calibrationfile_run3255_pedrun3255_gainrun3155.hdf5`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/tests/test_nectarcameventsource.py` & `ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/tests/test_nectarcameventsource.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam/version.py` & `ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam/version.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam.egg-info/PKG-INFO` & `ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: ctapipe-io-nectarcam
-Version: 0.1.2
+Version: 0.1.3
 Summary: ctapipe plugin for reading NectarCam files
 Author: NectarCAM collaboration
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/cta-observatory/ctapipe_io_nectarcam/issues
 Project-URL: Source Code, https://github.com/cta-observatory/ctapipe_io_nectarcam
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: ~=3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: tests
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE.md
 
 [![CI](https://github.com/cta-observatory/ctapipe_io_nectarcam/workflows/CI/badge.svg?branch=master)](https://github.com/cta-observatory/ctapipe_io_nectarcam/actions?query=workflow%3ACI+branch%3Amaster)
```

### Comparing `ctapipe_io_nectarcam-0.1.2/src/ctapipe_io_nectarcam.egg-info/SOURCES.txt` & `ctapipe_io_nectarcam-0.1.3/src/ctapipe_io_nectarcam.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 src/ctapipe_io_nectarcam/calibration.py
 src/ctapipe_io_nectarcam/constants.py
 src/ctapipe_io_nectarcam/containers.py
 src/ctapipe_io_nectarcam/version.py
 src/ctapipe_io_nectarcam.egg-info/PKG-INFO
 src/ctapipe_io_nectarcam.egg-info/SOURCES.txt
 src/ctapipe_io_nectarcam.egg-info/dependency_links.txt
+src/ctapipe_io_nectarcam.egg-info/entry_points.txt
 src/ctapipe_io_nectarcam.egg-info/not-zip-safe
 src/ctapipe_io_nectarcam.egg-info/requires.txt
 src/ctapipe_io_nectarcam.egg-info/top_level.txt
 src/ctapipe_io_nectarcam/resources/NectarCam-003.camgeom.fits.gz
 src/ctapipe_io_nectarcam/resources/Pulse_template_nectarCam_17042020.dat
 src/ctapipe_io_nectarcam/resources/calibrationfile_run3255_pedrun3255_gainrun3155.hdf5
+src/ctapipe_io_nectarcam/resources/calibrationfile_run3255_pedrun3255_gainrun3155_ctapipe018.hdf5
 src/ctapipe_io_nectarcam/tests/test_nectarcameventsource.py
 src/ctapipe_io_nectarcam/tests/test_version.py
```

