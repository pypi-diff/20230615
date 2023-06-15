# Comparing `tmp/tephi-0.2.4.tar.gz` & `tmp/tephi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tephi-0.2.4.tar", last modified: Mon May 25 01:35:43 2020, max compression
+gzip compressed data, was "tephi-0.3.0.tar", last modified: Thu Jun 15 14:45:46 2023, max compression
```

## Comparing `tephi-0.2.4.tar` & `tephi-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,73 @@
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2020-05-25 01:35:43.676529 tephi-0.2.4/
--rw-r--r--   0 bill      (1000) bill      (1000)    35147 2020-05-21 18:37:03.000000 tephi-0.2.4/COPYING
--rw-r--r--   0 bill      (1000) bill      (1000)     7651 2020-05-21 18:37:03.000000 tephi-0.2.4/COPYING.LESSER
--rw-r--r--   0 bill      (1000) bill      (1000)       59 2020-05-23 13:57:55.000000 tephi-0.2.4/MANIFEST.in
--rw-r--r--   0 bill      (1000) bill      (1000)     3307 2020-05-25 01:35:43.676529 tephi-0.2.4/PKG-INFO
--rw-r--r--   0 bill      (1000) bill      (1000)     1680 2020-05-25 00:27:21.000000 tephi-0.2.4/README.md
--rw-r--r--   0 bill      (1000) bill      (1000)      528 2020-05-25 00:08:14.000000 tephi-0.2.4/pyproject.toml
--rw-r--r--   0 bill      (1000) bill      (1000)     1628 2020-05-25 01:35:43.676529 tephi-0.2.4/setup.cfg
--rw-r--r--   0 bill      (1000) bill      (1000)      288 2020-05-24 22:39:24.000000 tephi-0.2.4/setup.py
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2020-05-25 01:35:43.672529 tephi-0.2.4/tephi/
--rw-r--r--   0 bill      (1000) bill      (1000)    29022 2020-05-25 01:35:30.000000 tephi-0.2.4/tephi/__init__.py
--rw-r--r--   0 bill      (1000) bill      (1000)      462 2020-05-21 18:38:18.000000 tephi-0.2.4/tephi/_constants.py
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2020-05-25 01:35:43.668528 tephi-0.2.4/tephi/etc/
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2020-05-25 01:35:43.676529 tephi-0.2.4/tephi/etc/test_data/
--rw-r--r--   0 bill      (1000) bill      (1000)      550 2020-05-21 18:38:18.000000 tephi-0.2.4/tephi/etc/test_data/barbs.txt
--rw-r--r--   0 bill      (1000) bill      (1000)       92 2020-05-21 18:38:18.000000 tephi-0.2.4/tephi/etc/test_data/comma_sep.txt
--rw-r--r--   0 bill      (1000) bill      (1000)      233 2020-05-21 18:38:18.000000 tephi-0.2.4/tephi/etc/test_data/dews.txt
--rw-r--r--   0 bill      (1000) bill      (1000)      422 2020-05-21 18:38:18.000000 tephi-0.2.4/tephi/etc/test_data/temps.txt
--rw-r--r--   0 bill      (1000) bill      (1000)    14896 2020-05-21 18:38:18.000000 tephi-0.2.4/tephi/isopleths.py
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2020-05-25 01:35:43.676529 tephi-0.2.4/tephi/tests/
--rw-r--r--   0 bill      (1000) bill      (1000)    10371 2020-05-21 18:38:18.000000 tephi-0.2.4/tephi/tests/__init__.py
--rwxr-xr-x   0 bill      (1000) bill      (1000)    11194 2020-05-21 18:38:18.000000 tephi-0.2.4/tephi/tests/idiff.py
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2020-05-25 01:35:43.676529 tephi-0.2.4/tephi/tests/results/
--rw-r--r--   0 bill      (1000) bill      (1000)      356 2020-05-21 18:38:18.000000 tephi-0.2.4/tephi/tests/results/barbs.npz
--rw-r--r--   0 bill      (1000) bill      (1000)      286 2020-05-21 18:38:18.000000 tephi-0.2.4/tephi/tests/results/dews.npz
--rw-r--r--   0 bill      (1000) bill      (1000)     4571 2020-05-21 18:38:18.000000 tephi-0.2.4/tephi/tests/results/imagerepo.json
--rw-r--r--   0 bill      (1000) bill      (1000)      336 2020-05-21 18:38:18.000000 tephi-0.2.4/tephi/tests/results/temps.npz
--rw-r--r--   0 bill      (1000) bill      (1000)     2081 2020-05-21 18:38:18.000000 tephi-0.2.4/tephi/tests/test_imagerepo.py
--rw-r--r--   0 bill      (1000) bill      (1000)     8998 2020-05-21 18:38:18.000000 tephi-0.2.4/tephi/tests/test_tephigram.py
--rw-r--r--   0 bill      (1000) bill      (1000)     5934 2020-05-21 18:38:18.000000 tephi-0.2.4/tephi/transforms.py
-drwxr-xr-x   0 bill      (1000) bill      (1000)        0 2020-05-25 01:35:43.672529 tephi-0.2.4/tephi.egg-info/
--rw-r--r--   0 bill      (1000) bill      (1000)     3307 2020-05-25 01:35:43.000000 tephi-0.2.4/tephi.egg-info/PKG-INFO
--rw-r--r--   0 bill      (1000) bill      (1000)      651 2020-05-25 01:35:43.000000 tephi-0.2.4/tephi.egg-info/SOURCES.txt
--rw-r--r--   0 bill      (1000) bill      (1000)        1 2020-05-25 01:35:43.000000 tephi-0.2.4/tephi.egg-info/dependency_links.txt
--rw-r--r--   0 bill      (1000) bill      (1000)       23 2020-05-25 01:35:43.000000 tephi-0.2.4/tephi.egg-info/requires.txt
--rw-r--r--   0 bill      (1000) bill      (1000)        6 2020-05-25 01:35:43.000000 tephi-0.2.4/tephi.egg-info/top_level.txt
+drwxr-xr-x   0 esadek   (12411) users     (1000)        0 2023-06-15 14:45:46.937636 tephi-0.3.0/
+-rw-r--r--   0 esadek   (12411) users     (1000)      238 2023-06-13 08:44:41.000000 tephi-0.3.0/.coveragerc
+-rw-r--r--   0 esadek   (12411) users     (1000)      715 2023-06-08 08:30:43.000000 tephi-0.3.0/.flake8
+-rw-r--r--   0 esadek   (12411) users     (1000)       40 2023-06-08 08:30:43.000000 tephi-0.3.0/.git-blame-ignore-revs
+-rw-r--r--   0 esadek   (12411) users     (1000)      880 2023-06-08 08:30:43.000000 tephi-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 esadek   (12411) users     (1000)       92 2023-06-08 08:30:43.000000 tephi-0.3.0/.readthedocs.yml
+-rw-r--r--   0 esadek   (12411) users     (1000)      550 2023-06-15 14:40:03.000000 tephi-0.3.0/CITATION.cff
+-rw-r--r--   0 esadek   (12411) users     (1000)     1519 2023-06-08 08:30:43.000000 tephi-0.3.0/LICENSE
+-rw-r--r--   0 esadek   (12411) users     (1000)      385 2023-06-15 14:40:03.000000 tephi-0.3.0/MANIFEST.in
+-rw-r--r--   0 esadek   (12411) users     (1000)     7281 2023-06-15 14:45:46.938642 tephi-0.3.0/PKG-INFO
+-rw-r--r--   0 esadek   (12411) users     (1000)     6103 2023-06-15 14:40:03.000000 tephi-0.3.0/README.md
+drwxr-xr-x   0 esadek   (12411) users     (1000)        0 2023-06-15 14:45:46.574673 tephi-0.3.0/docs/
+drwxr-xr-x   0 esadek   (12411) users     (1000)        0 2023-06-15 14:45:46.681650 tephi-0.3.0/docs/tephi/
+-rw-r--r--   0 esadek   (12411) users     (1000)     5569 2023-06-13 08:44:41.000000 tephi-0.3.0/docs/tephi/Makefile
+-rw-r--r--   0 esadek   (12411) users     (1000)     5103 2023-06-13 08:44:41.000000 tephi-0.3.0/docs/tephi/make.bat
+drwxr-xr-x   0 esadek   (12411) users     (1000)        0 2023-06-15 14:45:46.716675 tephi-0.3.0/docs/tephi/source/
+drwxr-xr-x   0 esadek   (12411) users     (1000)        0 2023-06-15 14:45:46.723633 tephi-0.3.0/docs/tephi/source/_static/
+-rw-r--r--   0 esadek   (12411) users     (1000)     5430 2023-06-13 08:44:41.000000 tephi-0.3.0/docs/tephi/source/_static/favicon.ico
+-rw-r--r--   0 esadek   (12411) users     (1000)    43065 2023-06-13 08:44:41.000000 tephi-0.3.0/docs/tephi/source/_static/tephi-logo-200-137.png
+-rw-r--r--   0 esadek   (12411) users     (1000)     5468 2023-06-13 08:44:41.000000 tephi-0.3.0/docs/tephi/source/barbs.rst
+-rw-r--r--   0 esadek   (12411) users     (1000)     8813 2023-06-13 08:44:41.000000 tephi-0.3.0/docs/tephi/source/conf.py
+-rw-r--r--   0 esadek   (12411) users     (1000)    14299 2023-06-13 08:44:41.000000 tephi-0.3.0/docs/tephi/source/customise.rst
+drwxr-xr-x   0 esadek   (12411) users     (1000)        0 2023-06-15 14:45:46.812663 tephi-0.3.0/docs/tephi/source/figures/
+-rw-r--r--   0 esadek   (12411) users     (1000)    97473 2023-06-13 08:44:42.000000 tephi-0.3.0/docs/tephi/source/figures/tephi_axes.png
+-rw-r--r--   0 esadek   (12411) users     (1000)    95669 2023-06-13 08:44:42.000000 tephi-0.3.0/docs/tephi/source/figures/tephi_axis_dry_adiabat.png
+-rw-r--r--   0 esadek   (12411) users     (1000)    99081 2023-06-13 08:44:42.000000 tephi-0.3.0/docs/tephi/source/figures/tephi_axis_isobar.png
+-rw-r--r--   0 esadek   (12411) users     (1000)    95955 2023-06-13 08:44:42.000000 tephi-0.3.0/docs/tephi/source/figures/tephi_axis_isotherm.png
+-rw-r--r--   0 esadek   (12411) users     (1000)   103735 2023-06-13 08:44:42.000000 tephi-0.3.0/docs/tephi/source/figures/tephi_axis_mixing.png
+-rw-r--r--   0 esadek   (12411) users     (1000)   101146 2023-06-13 08:44:42.000000 tephi-0.3.0/docs/tephi/source/figures/tephi_axis_wet_adiabat.png
+-rw-r--r--   0 esadek   (12411) users     (1000)    95102 2023-06-13 08:44:42.000000 tephi-0.3.0/docs/tephi/source/figures/tephi_right_angles.png
+-rw-r--r--   0 esadek   (12411) users     (1000)     2142 2023-06-13 08:44:42.000000 tephi-0.3.0/docs/tephi/source/glossary.rst
+-rw-r--r--   0 esadek   (12411) users     (1000)      719 2023-06-13 08:44:42.000000 tephi-0.3.0/docs/tephi/source/index.rst
+-rw-r--r--   0 esadek   (12411) users     (1000)     4820 2023-06-13 08:44:42.000000 tephi-0.3.0/docs/tephi/source/introduction.rst
+drwxr-xr-x   0 esadek   (12411) users     (1000)        0 2023-06-15 14:45:46.819637 tephi-0.3.0/docs/tephi/source/plot/
+-rw-r--r--   0 esadek   (12411) users     (1000)     1368 2023-06-13 08:44:42.000000 tephi-0.3.0/docs/tephi/source/plot/barbs.py
+-rw-r--r--   0 esadek   (12411) users     (1000)     8052 2023-06-13 08:44:42.000000 tephi-0.3.0/docs/tephi/source/plotting.rst
+-rw-r--r--   0 esadek   (12411) users     (1000)       85 2023-06-08 08:30:43.000000 tephi-0.3.0/environment.yml
+-rw-r--r--   0 esadek   (12411) users     (1000)   734702 2023-06-08 08:30:43.000000 tephi-0.3.0/index.ipynb
+-rw-r--r--   0 esadek   (12411) users     (1000)      246 2023-06-08 08:30:43.000000 tephi-0.3.0/pyproject.toml
+drwxr-xr-x   0 esadek   (12411) users     (1000)        0 2023-06-15 14:45:46.833641 tephi-0.3.0/requirements/
+-rw-r--r--   0 esadek   (12411) users     (1000)       99 2023-06-08 08:30:43.000000 tephi-0.3.0/requirements/dev.yml
+-rw-r--r--   0 esadek   (12411) users     (1000)      154 2023-06-08 08:30:43.000000 tephi-0.3.0/requirements/rtd.yml
+-rw-r--r--   0 esadek   (12411) users     (1000)     1690 2023-06-15 14:45:46.941650 tephi-0.3.0/setup.cfg
+-rw-r--r--   0 esadek   (12411) users     (1000)      266 2023-06-08 08:30:43.000000 tephi-0.3.0/setup.py
+drwxr-xr-x   0 esadek   (12411) users     (1000)        0 2023-06-15 14:45:46.851641 tephi-0.3.0/tephi/
+-rw-r--r--   0 esadek   (12411) users     (1000)    29014 2023-06-15 14:08:35.000000 tephi-0.3.0/tephi/__init__.py
+-rw-r--r--   0 esadek   (12411) users     (1000)      440 2023-06-15 12:32:13.000000 tephi-0.3.0/tephi/_constants.py
+drwxr-xr-x   0 esadek   (12411) users     (1000)        0 2023-06-15 14:45:46.585670 tephi-0.3.0/tephi/etc/
+drwxr-xr-x   0 esadek   (12411) users     (1000)        0 2023-06-15 14:45:46.896649 tephi-0.3.0/tephi/etc/test_data/
+-rw-r--r--   0 esadek   (12411) users     (1000)      550 2023-06-15 12:32:13.000000 tephi-0.3.0/tephi/etc/test_data/barbs.txt
+-rw-r--r--   0 esadek   (12411) users     (1000)       92 2023-06-15 12:32:13.000000 tephi-0.3.0/tephi/etc/test_data/comma_sep.txt
+-rw-r--r--   0 esadek   (12411) users     (1000)      233 2023-06-15 12:32:13.000000 tephi-0.3.0/tephi/etc/test_data/dews.txt
+-rw-r--r--   0 esadek   (12411) users     (1000)      422 2023-06-15 12:32:13.000000 tephi-0.3.0/tephi/etc/test_data/temps.txt
+-rw-r--r--   0 esadek   (12411) users     (1000)    15062 2023-06-15 12:32:13.000000 tephi-0.3.0/tephi/isopleths.py
+drwxr-xr-x   0 esadek   (12411) users     (1000)        0 2023-06-15 14:45:46.918632 tephi-0.3.0/tephi/tests/
+-rw-r--r--   0 esadek   (12411) users     (1000)     9344 2023-06-15 12:32:13.000000 tephi-0.3.0/tephi/tests/__init__.py
+-rw-r--r--   0 esadek   (12411) users     (1000)     1024 2023-06-15 12:32:13.000000 tephi-0.3.0/tephi/tests/conftest.py
+-rwxr-xr-x   0 esadek   (12411) users     (1000)    11172 2023-06-15 12:32:13.000000 tephi-0.3.0/tephi/tests/idiff.py
+drwxr-xr-x   0 esadek   (12411) users     (1000)        0 2023-06-15 14:45:46.934638 tephi-0.3.0/tephi/tests/results/
+-rw-r--r--   0 esadek   (12411) users     (1000)      356 2023-06-15 12:32:13.000000 tephi-0.3.0/tephi/tests/results/barbs.npz
+-rw-r--r--   0 esadek   (12411) users     (1000)      286 2023-06-15 12:32:13.000000 tephi-0.3.0/tephi/tests/results/dews.npz
+-rw-r--r--   0 esadek   (12411) users     (1000)     5381 2023-06-15 12:32:13.000000 tephi-0.3.0/tephi/tests/results/imagerepo.json
+-rw-r--r--   0 esadek   (12411) users     (1000)      336 2023-06-15 12:32:13.000000 tephi-0.3.0/tephi/tests/results/temps.npz
+-rw-r--r--   0 esadek   (12411) users     (1000)     1898 2023-06-15 12:32:13.000000 tephi-0.3.0/tephi/tests/test_imagerepo.py
+-rw-r--r--   0 esadek   (12411) users     (1000)     9701 2023-06-15 12:32:13.000000 tephi-0.3.0/tephi/tests/test_tephigram.py
+-rw-r--r--   0 esadek   (12411) users     (1000)     5908 2023-06-15 12:32:13.000000 tephi-0.3.0/tephi/transforms.py
+drwxr-xr-x   0 esadek   (12411) users     (1000)        0 2023-06-15 14:45:46.876642 tephi-0.3.0/tephi.egg-info/
+-rw-r--r--   0 esadek   (12411) users     (1000)     7281 2023-06-15 14:45:46.000000 tephi-0.3.0/tephi.egg-info/PKG-INFO
+-rw-r--r--   0 esadek   (12411) users     (1000)     1547 2023-06-15 14:45:46.000000 tephi-0.3.0/tephi.egg-info/SOURCES.txt
+-rw-r--r--   0 esadek   (12411) users     (1000)        1 2023-06-15 14:45:46.000000 tephi-0.3.0/tephi.egg-info/dependency_links.txt
+-rw-r--r--   0 esadek   (12411) users     (1000)       23 2023-06-15 14:45:46.000000 tephi-0.3.0/tephi.egg-info/requires.txt
+-rw-r--r--   0 esadek   (12411) users     (1000)        6 2023-06-15 14:45:46.000000 tephi-0.3.0/tephi.egg-info/top_level.txt
+-rw-r--r--   0 esadek   (12411) users     (1000)      985 2023-06-13 08:44:42.000000 tephi-0.3.0/tox.ini
```

### Comparing `tephi-0.2.4/setup.cfg` & `tephi-0.3.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -4,48 +4,51 @@
 	docs,
 	tephi/tests/__init__.py
 	.eggs
 
 [tool:pytest]
 testpaths = 
 	tephi/
+markers = 
+	graphical: mark a test as a graphical test
 addopts = 
 	-ra
 	-v
 	--cov-config=.coveragerc
 	--cov=tephi
 	--cov-report=term-missing
+	--doctest-modules
+doctest_optionflags = NORMALIZE_WHITESPACE ELLIPSIS NUMBER
 
 [metadata]
 name = tephi
 version = attr: tephi.__version__
 author = UK Met Office
 author_email = scitools-iris-dev@googlegroups.com
 url = https://github.com/SciTools/tephi
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
-	License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+	License :: OSI Approved :: BSD License
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Topic :: Scientific/Engineering :: Atmospheric Science
 	Topic :: Scientific/Engineering :: Visualization
-license = LGPL-3.0
-license_file = COPYING.LESSER
+license_files = LICENSE
 description = Tephigram plotting in Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 project_urls = 
 	code = https://github.com/SciTools/tephi
 	issues = https://github.com/SciTools/tephi/issues
-	binder = https://mybinder.org/v2/gh/SciTools/tephi/master?filepath=index.ipynb
+	binder = https://mybinder.org/v2/gh/SciTools/tephi/main?filepath=index.ipynb
 	documentation =  https://tephi.readthedocs.io/en/latest/
 keywords = 
 	tephigram
 	radiosonde
 	meteorology
 	visualization
 
@@ -54,15 +57,15 @@
 setup_requires = 
 	setuptools>=40.8.0
 	wheel
 install_requires = 
 	matplotlib
 	numpy
 	scipy
-python_requires = >=3.6
+python_requires = >=3.8
 
 [options.package_data]
 tephi = 
 	etc/test_data/*.txt
 	tests/results/*.npz
 	tests/results/imagerepo.json
```

### Comparing `tephi-0.2.4/tephi/__init__.py` & `tephi-0.3.0/tephi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright Tephi contributors
 #
-# This file is part of Tephi and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of Tephi and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 """
 The tephi module provides tephigram plotting of pressure, temperature and wind
 barb data.
 
 .. warning::
     This is a beta release module and is liable to change.
 
@@ -24,15 +23,15 @@
 import numpy as np
 import os.path
 
 from . import isopleths
 from . import transforms
 
 
-__version__ = "0.2.4"
+__version__ = "0.3.0"
 
 
 #
 # Miscellaneous constants.
 #
 DEFAULT_WIDTH = 700  # in pixels
 
@@ -292,18 +291,17 @@
         """
         self.step = int(step)
 
     def __call__(self, start, stop):
         """Calculate the axis ticks given the provided tick range."""
 
         step = self.step
-        start = (int(start) / step) * step
-        stop = (int(stop) / step) * step
-        ticks = np.arange(start, stop + step, step)
-
+        start = (int(start) // step) * step
+        stop = (int(stop) // step) * step
+        ticks = np.arange(start, stop + step, step, dtype=int)
         return ticks, len(ticks), 1
 
 
 def _refresh_isopleths(axes):
     """
     Refresh the plot isobars, wet adiabats and mixing ratios and associated
     text labels.
@@ -593,17 +591,17 @@
         * isotherm_locator:
             A :class:`tephi.Locator` instance or a numeric step size
             for the isotherm lines.
         * dry_adiabat_locator:
             A :class:`tephi.Locator` instance or a numeric step size
             for the dry adiabat lines.
         * anchor:
-            A sequence of two pressure, temperature pairs specifying the extent
-            of the tephigram plot in terms of the bottom left hand corner and
-            the top right hand corner. Pressure data points must be in units of
+            A sequence of two (pressure, temperature) pairs specifying the extent
+            of the tephigram plot in terms of the bottom right-hand corner, and
+            the top left-hand corner. Pressure data points must be in units of
             mb or hPa, and temperature data points must be in units of degC.
 
         For example:
 
         .. plot::
             :include-source:
 
@@ -799,17 +797,17 @@
             self._anchor = np.asarray(anchor)
             if (
                 self._anchor.ndim != 2
                 or self._anchor.shape[-1] != 2
                 or len(self._anchor) != 2
             ):
                 msg = (
-                    "Invalid anchor, expecting [(bottom-left-pressure, "
-                    "bottom-left-temperature), (top-right-pressure, "
-                    "top-right-temperature)]"
+                    "Invalid anchor, expecting [(bottom-right-pressure, "
+                    "bottom-right-temperature), (top-left-pressure, "
+                    "top-left-temperature)]"
                 )
                 raise ValueError(msg)
             (
                 (bottom_pressure, bottom_temp),
                 (top_pressure, top_temp),
             ) = self._anchor
 
@@ -837,15 +835,15 @@
 
         .. warning::
             Pressure data points must be in units of mb or hPa, and temperature
             data points must be in units of degC.
 
         Args:
 
-        * data: pressure and temperature pair data points.
+        * data: (pressure, temperature) pair data points.
 
         .. note::
             All keyword arguments are passed through to
             :func:`matplotlib.pyplot.plot`.
 
         For example:
```

### Comparing `tephi-0.2.4/tephi/etc/test_data/barbs.txt` & `tephi-0.3.0/tephi/etc/test_data/barbs.txt`

 * *Files identical despite different names*

### Comparing `tephi-0.2.4/tephi/isopleths.py` & `tephi-0.3.0/tephi/isopleths.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright Tephi contributors
 #
-# This file is part of Tephi and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of Tephi and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 """
 Tephigram isopleth support for generating and plotting tephigram lines,
 environment profiles and barbs.
 
 """
 import math
 from matplotlib.collections import PathCollection
@@ -22,15 +21,15 @@
 
 # Wind barb speed (knots) ranges used since 1 January 1955.
 _BARB_BINS = np.arange(20) * 5 + 3
 _BARB_GUTTER = 0.1
 _BARB_DTYPE = np.dtype(
     dict(
         names=("speed", "angle", "pressure", "barb"),
-        formats=("f4", "f4", "f4", np.object),
+        formats=("f4", "f4", "f4", object),
     )
 )
 
 #
 # Reference: http://www-nwp/~hadaa/tephigram/tephi_plot.html
 #
 
@@ -137,15 +136,15 @@
         the gradient difference.
 
     * dp:
         The wet adiabat change in pressure, in mb or hPa, from which to
         calculate the gradient difference.
 
     Returns:
-        The gradient change as a pressure, potential temperature value pair.
+        The gradient change as a (pressure, potential-temperature) value pair.
 
     """
 
     # TODO: Discover the meaning of the magic numbers.
 
     kelvin = temperature + CONST_KELVIN
     lsbc = (CONST_L / CONST_RV) * ((1.0 / CONST_KELVIN) - (1.0 / kelvin))
@@ -212,15 +211,15 @@
 
     _, thetas = transforms.convert_pT2Tt(pressures, temps)
     (line,) = axes.plot(temps, thetas, transform=transform, **kwargs)
 
     return line
 
 
-class Barbs(object):
+class Barbs:
     """Generate a wind arrow barb."""
 
     def __init__(self, axes):
         """
         Create a wind arrow barb for the given axes.
 
         Args:
@@ -290,15 +289,15 @@
             pivot = self._kwargs.get("pivot", "tip")
             offset = pivot_points[pivot]
             verts = [(0.0, offset), (0.0, length + offset)]
             rangle = math.radians(-angle)
             verts = mtransforms.Affine2D().rotate(rangle).transform(verts)
             codes = [Path.MOVETO, Path.LINETO]
             path = Path(verts, codes)
-            size = length ** 2 / 4
+            size = length**2 / 4
             xy = np.array([[temperature, theta]])
             barb = PathCollection(
                 [path],
                 (size,),
                 offsets=xy,
                 transOffset=self._transform,
                 **self._custom_kwargs,
@@ -365,15 +364,17 @@
             Proportion offset from the right hand side axis to plot the
             barbs. Defaults to 0.1
 
             Also see :func:`matplotlib.pyplot.barbs`
 
         """
         self._gutter = kwargs.pop("gutter", _BARB_GUTTER)
-        self._kwargs = dict(length=7, zorder=10)
+        # zorder of 4.1 is higher than all MPL defaults, excluding legend. Also
+        # higher than tephi default for plot-lines.
+        self._kwargs = dict(length=7, zorder=4.1)
         self._kwargs.update(kwargs)
         self._custom_kwargs = dict(
             color=None, linewidth=1.5, zorder=self._kwargs["zorder"]
         )
         for key, values in self._custom.items():
             common = set(values).intersection(kwargs)
             if common:
@@ -389,15 +390,15 @@
             raise ValueError(msg)
         self.barbs = np.empty(barbs.shape[0], dtype=_BARB_DTYPE)
         for i, barb in enumerate(barbs):
             self.barbs[i] = tuple(barb) + (None,)
         self.refresh()
 
 
-class Profile(object):
+class Profile:
     """Generate an environmental lapse rate profile."""
 
     def __init__(self, data, axes):
         """
         Create an environmental lapse rate profile from the sequence of
         pressure and temperature point data.
 
@@ -413,15 +414,15 @@
         """
         if hasattr(data, "__next__"):
             data = list(data)
         self.data = np.asarray(data)
         if self.data.ndim != 2 or self.data.shape[-1] != 2:
             msg = (
                 "The environment profile data requires to be a sequence "
-                "of pressure, temperature value pairs."
+                "of (pressure, temperature) value pairs."
             )
             raise ValueError(msg)
         self.axes = axes
         self._transform = axes.tephigram_transform + axes.transData
         self.pressure = self.data[:, 0]
         self.temperature = self.data[:, 1]
         _, self.theta = transforms.convert_pT2Tt(
@@ -441,16 +442,17 @@
         Returns:
             The profile :class:`matplotlib.lines.Line2D`
 
         """
         if self.line is not None and self.line in self.axes.lines:
             self.axes.lines.remove(self.line)
 
+        # zorder of 4 is higher than all MPL defaults, excluding legend.
         if "zorder" not in kwargs:
-            kwargs["zorder"] = 10
+            kwargs["zorder"] = 4
 
         (self.line,) = self.axes.plot(
             self.temperature, self.theta, transform=self._transform, **kwargs
         )
         return self.line
 
     def refresh(self):
```

### Comparing `tephi-0.2.4/tephi/tests/__init__.py` & `tephi-0.3.0/tephi/tests/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright Tephi contributors
 #
-# This file is part of Tephi and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of Tephi and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 """
 Provides testing capabilities and customisations specific to tephi.
 
 .. note:: This module needs to control the matplotlib backend, so it
           **must** be imported before ``matplotlib.pyplot``.
 
 By default, this module sets the matplotlib backend to "agg". But when
@@ -18,19 +17,19 @@
 """
 import codecs
 import collections
 import io
 import json
 import os
 import sys
-import unittest
 
 import filelock
 import matplotlib
 import numpy as np
+import pytest
 import requests
 
 from tephi import DATA_DIR
 
 
 #: Basepath for test data.
 _DATA_PATH = DATA_DIR
@@ -38,15 +37,15 @@
 #: Basepath for test results.
 _RESULT_PATH = os.path.join(os.path.dirname(__file__), "results")
 
 #: Default perceptual hash size.
 _HASH_SIZE = 16
 
 #: Default maximum perceptual hash hamming distance.
-_HAMMING_DISTANCE = 2
+_HAMMING_DISTANCE = 4
 
 # Whether to display matplotlib output to the screen.
 _DISPLAY_FIGURES = False
 
 # Test images URL.
 BASE_URL = "https://scitools.github.io/test-tephi-imagehash/images"
 
@@ -56,17 +55,17 @@
     # on a platform which has restricted/no internet access.
     requests.get("https://github.com/SciTools/tephi", timeout=5.0)
     INET_AVAILABLE = True
 except requests.exceptions.ConnectionError:
     INET_AVAILABLE = False
 
 
-skip_inet = unittest.skipIf(
+requires_inet = pytest.mark.skipif(
     not INET_AVAILABLE,
-    ('Test(s) require an "internet connection", which is not available.'),
+    reason=('Test requires an "internet connection", which is not available.'),
 )
 
 
 if "-d" in sys.argv:
     sys.argv.remove("-d")
     matplotlib.use("tkagg")
     _DISPLAY_FIGURES = True
@@ -95,90 +94,70 @@
 
     """
     if isinstance(relative_path, (list, tuple)):
         relative_path = os.path.join(*relative_path)
     return os.path.abspath(os.path.join(_RESULT_PATH, relative_path))
 
 
-class TephiTest(unittest.TestCase):
+class TephiTest:
     """
-    A subclass of unittest.TestCase which provides testing functionality
-    specific to tephi.
+    Utility class containing common testing framework functionality.
 
     """
 
-    _assertion_counts = collections.defaultdict(int)
-
-    def _unique_id(self):
-        """
-        Returns the unique ID for the current assertion.
-
-        The ID is composed of two parts: a unique ID for the current test
-        (which is itself composed of the module, class, and test names), and
-        a sequential counter (specific to the current test) that is incremented
-        on each call.
-
-        For example, calls from a "test_tx" routine followed by a "test_ty"
-        routine might result in::
-            test_plot.TestContourf.test_tx.0
-            test_plot.TestContourf.test_tx.1
-            test_plot.TestContourf.test_tx.2
-            test_plot.TestContourf.test_ty.0
-
-        """
-        # Obtain a consistent ID for the current test.
-
-        # NB. unittest.TestCase.id() returns different values depending on
-        # whether the test has been run explicitly, or via test discovery.
-        # For example:
-        #   python tests/test_brand.py
-        #       => '__main__.TestBranding.test_combo'
-        #   python -m unittest discover
-        #       => 'tephi.tests.test_brand.TestBranding.test_combo'
-        bits = self.id().split(".")[-3:]
-        if bits[0] == "__main__":
-            file_name = os.path.basename(sys.modules["__main__"].__file__)
-            bits[0] = os.path.splitext(file_name)[0]
-        test_id = ".".join(bits)
-
-        # Derive the sequential assertion ID within the test
-        assertion_id = self._assertion_counts[test_id]
-        self._assertion_counts[test_id] += 1
-
-        return "{}.{}".format(test_id, assertion_id)
-
     def assertArrayEqual(self, a, b):
+        __tracebackhide__ = True
         return np.testing.assert_array_equal(a, b)
 
     def assertArrayAlmostEqual(self, a, b, *args, **kwargs):
+        __tracebackhide__ = True
         return np.testing.assert_array_almost_equal(a, b, *args, **kwargs)
 
 
 class GraphicsTest(TephiTest):
-    def tearDown(self):
-        # If a plotting test bombs out it can leave the current figure in an
-        # odd state, so we make sure it's been disposed of.
-        plt.close()
+    _assertion_count = collections.defaultdict(int)
+
+    def _unique_id(self, nodeid):
+        """Create a hashable key to represent the unique test invocation.
+
+        Construct the hashable key from the provided nodeid and a sequential
+        counter specific to the current test, that is incremented on each call.
+
+        Parameters
+        ----------
+        nodeid : str
+            Unique identifier for the current test. See :func:`nodeid` fixture.
+
+        Returns
+        -------
+        str
+            The nodeid with sequential counter.
+
+        """
+        count = self._assertion_count[nodeid]
+        self._assertion_count[nodeid] += 1
+        return f"{nodeid}.{count}"
 
-    def check_graphic(self):
+    def check_graphic(self, nodeid):
         """
         Check the hash of the current matplotlib figure matches the expected
         image hash for the current graphic test.
 
         To create missing image test results, set the TEPHI_TEST_CREATE_MISSING
         environment variable before running the tests. This will result in new
         and appropriately "<hash>.png" image files being generated in the image
         output directory, and the imagerepo.json file being updated.
 
         """
+        __tracebackhide__ = True
         import imagehash
         from PIL import Image
 
         dev_mode = os.environ.get("TEPHI_TEST_CREATE_MISSING")
-        unique_id = self._unique_id()
+        unique_id = self._unique_id(nodeid)
         repo_fname = os.path.join(_RESULT_PATH, "imagerepo.json")
         repo = {}
         if os.path.isfile(repo_fname):
             with open(repo_fname, "rb") as fi:
                 repo = json.load(codecs.getreader("utf-8")(fi))
 
         try:
```

### Comparing `tephi-0.2.4/tephi/tests/idiff.py` & `tephi-0.3.0/tephi/tests/idiff.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright Tephi contributors
 #
-# This file is part of Tephi and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of Tephi and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 # !/usr/bin/env python
 """
 Provides "diff-like" comparison of images.
 
 Currently relies on matplotlib for image processing so limited to PNG format.
 
 """
```

### Comparing `tephi-0.2.4/tephi/tests/results/imagerepo.json` & `tephi-0.3.0/tephi/tests/results/imagerepo.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9318181818181818%*

 * *Differences: {"'test_tephigram.TestTephigramPlot.test_plot_dews_locator_adiabat_numeric.0'": '{insert: [(1, '*

 * *                                                                                "'https://scitools.github.io/test-tephi-imagehash/images/e85a9f0991a76639cca53989965d98d6cf3462619b893f124c664b9c9c7b7256.png')]}",*

 * * "'test_tephigram.TestTephigramPlot.test_plot_dews_locator_adiabat_object.0'": '{insert: [(1, '*

 * *                                                                               "'https://scitools.github.io […]*

```diff
@@ -29,30 +29,36 @@
     "test_tephigram.TestTephigramPlot.test_plot_dews_custom.0": [
         "https://scitools.github.io/test-tephi-imagehash/images/e85a986d99e66631c66d698e971999a6c7966261979b7a9269668c893c7332a6.png"
     ],
     "test_tephigram.TestTephigramPlot.test_plot_dews_label.0": [
         "https://scitools.github.io/test-tephi-imagehash/images/e85a992d90c56630cced39afc6198cf6c734e26197997a9269669d8d387330e6.png"
     ],
     "test_tephigram.TestTephigramPlot.test_plot_dews_locator_adiabat_numeric.0": [
-        "https://scitools.github.io/test-tephi-imagehash/images/e85a9e0c91a3663ccda5398c965a9cf6cb3462619b9c3f134c66cd099e737346.png"
+        "https://scitools.github.io/test-tephi-imagehash/images/e85a9e0c91a3663ccda5398c965a9cf6cb3462619b9c3f134c66cd099e737346.png",
+        "https://scitools.github.io/test-tephi-imagehash/images/e85a9f0991a76639cca53989965d98d6cf3462619b893f124c664b9c9c7b7256.png"
     ],
     "test_tephigram.TestTephigramPlot.test_plot_dews_locator_adiabat_object.0": [
-        "https://scitools.github.io/test-tephi-imagehash/images/e85a9e0c91a3663ccda5398c965a9cf6cb3462619b9c3f134c66cd099e737346.png"
+        "https://scitools.github.io/test-tephi-imagehash/images/e85a9e0c91a3663ccda5398c965a9cf6cb3462619b9c3f134c66cd099e737346.png",
+        "https://scitools.github.io/test-tephi-imagehash/images/e85a9f0991a76639cca53989965d98d6cf3462619b893f124c664b9c9c7b7256.png"
     ],
     "test_tephigram.TestTephigramPlot.test_plot_dews_locator_isotherm_numeric.0": [
-        "https://scitools.github.io/test-tephi-imagehash/images/e85a8f2c90c56630cce539ad96591c96cf347a6795986a924966cd8dbc73e1e4.png"
+        "https://scitools.github.io/test-tephi-imagehash/images/e85a8f2c90c56630cce539ad96591c96cf347a6795986a924966cd8dbc73e1e4.png",
+        "https://scitools.github.io/test-tephi-imagehash/images/e85a9f2d90c56630cce539ac96599cf6c7b46a6195986a924d66cd8d1e23363e.png"
     ],
     "test_tephigram.TestTephigramPlot.test_plot_dews_locator_isotherm_object.0": [
-        "https://scitools.github.io/test-tephi-imagehash/images/e85a8f2c90c56630cce539ad96591c96cf347a6795986a924966cd8dbc73e1e4.png"
+        "https://scitools.github.io/test-tephi-imagehash/images/e85a8f2c90c56630cce539ad96591c96cf347a6795986a924966cd8dbc73e1e4.png",
+        "https://scitools.github.io/test-tephi-imagehash/images/e85a9f2d90c56630cce539ac96599cf6c7b46a6195986a924d66cd8d1e23363e.png"
     ],
     "test_tephigram.TestTephigramPlot.test_plot_dews_locator_numeric.0": [
-        "https://scitools.github.io/test-tephi-imagehash/images/e85a9e0c91e3663ccda5398c965b1cd6cb346a639a9c27334c664d099c78e3f6.png"
+        "https://scitools.github.io/test-tephi-imagehash/images/e85a9e0c91e3663ccda5398c965b1cd6cb346a639a9c27334c664d099c78e3f6.png",
+        "https://scitools.github.io/test-tephi-imagehash/images/e85a9f0991e76639c5a53989965d1cd6cf346a63939867b30c664bcc1e1b7216.png"
     ],
     "test_tephigram.TestTephigramPlot.test_plot_dews_locator_object.0": [
-        "https://scitools.github.io/test-tephi-imagehash/images/e85a9e0c91e3663ccda5398c965b1cd6cb346a639a9c27334c664d099c78e3f6.png"
+        "https://scitools.github.io/test-tephi-imagehash/images/e85a9e0c91e3663ccda5398c965b1cd6cb346a639a9c27334c664d099c78e3f6.png",
+        "https://scitools.github.io/test-tephi-imagehash/images/e85a9f0991e76639c5a53989965d1cd6cf346a63939867b30c664bcc1e1b7216.png"
     ],
     "test_tephigram.TestTephigramPlot.test_plot_dews_temps.0": [
         "https://scitools.github.io/test-tephi-imagehash/images/e969cc3992c76726cd973326c65869c6c3319e4d9c9849333c2c6399e5a7a7a4.png"
     ],
     "test_tephigram.TestTephigramPlot.test_plot_dews_temps_custom.0": [
         "https://scitools.github.io/test-tephi-imagehash/images/f1289c9996c76726cd9d333cc658cc66c731ce4c3cde499934247199b1e73326.png"
     ],
```

### Comparing `tephi-0.2.4/tephi/tests/test_imagerepo.py` & `tephi-0.3.0/tephi/tests/test_imagerepo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 # Copyright Tephi contributors
 #
-# This file is part of Tephi and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of Tephi and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 """
 Test that imagerepo.json reconciles with the images registered in the
 test-tephi-imagehash repository.
 
 """
 # Import tephi tests first so that some things can be initialised before
 # importing anything else
 import tephi.tests as tests
 
 import codecs
 import itertools
 import json
 import os
-import unittest
+import pytest
 
 import requests
 
 
 IMAGE_MANIFEST = (
     "https://raw.githubusercontent.com/SciTools/"
     "test-tephi-imagehash/gh-pages/image_manifest.txt"
 )
 
 
-@tests.skip_inet
-class TestImageRepoJSON(tests.TephiTest):
+@tests.requires_inet
+class TestImageRepoJSON:
     def test(self):
         response = requests.get(IMAGE_MANIFEST)
 
         emsg = 'Failed to download "image_manifest.txt"'
-        self.assertEqual(response.status_code, requests.codes.ok, msg=emsg)
+        assert response.status_code == requests.codes.ok, emsg
 
         image_manifest = response.content.decode("utf-8")
         image_manifest = [line.strip() for line in image_manifest.split("\n")]
         image_manifest_uris = set(
             os.path.join(tests.BASE_URL, fname) for fname in image_manifest
         )
 
@@ -55,13 +54,8 @@
         if count:
             emsg = (
                 '"imagerepo.json" references {} image URIs that are not '
                 'listed in "{}":\n\t'
             )
             emsg = emsg.format(count, IMAGE_MANIFEST)
             emsg += "\t".join(uri for uri in missing)
-            # Always fails when we get here: report the problem.
-            self.assertEqual(count, 0, msg=emsg)
-
-
-if __name__ == "__main__":
-    unittest.main()
+            pytest.fail(emsg)
```

### Comparing `tephi-0.2.4/tephi/tests/test_tephigram.py` & `tephi-0.3.0/tephi/tests/test_tephigram.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # Copyright Tephi contributors
 #
-# This file is part of Tephi and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of Tephi and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 """
 Tests the tephigram plotting capability provided by tephi.
 
 """
 # Import tephi test package first so that some things can be initialised
 # before importing anything else.
 import tephi.tests as tests
 
-import unittest
-
 import numpy as np
+import pytest
 
 import tephi
 from tephi import Tephigram
 
 
 def _load_result(filename):
     with np.load(tephi.tests.get_result_path(filename)) as f:
@@ -27,201 +25,210 @@
 
 _expected_dews = _load_result("dews.npz")
 _expected_temps = _load_result("temps.npz")
 _expected_barbs = _load_result("barbs.npz")
 
 
 class TestTephigramLoadTxt(tests.TephiTest):
-    def setUp(self):
+    @pytest.fixture(autouse=True)
+    def setup(self):
         self.filename_dews = tephi.tests.get_data_path("dews.txt")
         self.filename_temps = tephi.tests.get_data_path("temps.txt")
         self.filename_barbs = tephi.tests.get_data_path("barbs.txt")
         self.filename_comma = tephi.tests.get_data_path("comma_sep.txt")
 
     def test_is_not_file(self):
-        with self.assertRaises(OSError):
+        with pytest.raises(OSError):
             tephi.loadtxt("wibble")
 
     def test_load_data_no_column_names(self):
         dews = tephi.loadtxt(self.filename_dews)
-        self.assertEqual(dews._fields, ("pressure", "temperature"))
+        assert dews._fields == ("pressure", "temperature")
         self.assertArrayEqual(dews.pressure, _expected_dews[0])
         self.assertArrayEqual(dews, _expected_dews)
 
     def test_load_data_with_column_names(self):
         # Column titles test all valid namedtuple characters (alphanumeric, _).
         columns = ("pressure", "dewpoint2", "wind_speed", "WindDirection")
         barbs = tephi.loadtxt(self.filename_barbs, column_titles=columns)
-        self.assertEqual(barbs._fields, columns)
+        assert barbs._fields == columns
         self.assertArrayEqual(barbs.wind_speed, _expected_barbs[2])
         self.assertArrayEqual(barbs, _expected_barbs)
 
     def test_load_multiple_files_same_column_names(self):
         columns = ("foo", "bar")
         dews, temps = tephi.loadtxt(
             self.filename_dews, self.filename_temps, column_titles=columns
         )
-        self.assertEqual(dews._fields, columns)
-        self.assertEqual(temps._fields, columns)
+        assert dews._fields == columns
+        assert temps._fields == columns
 
     def test_load_data_too_many_column_iterables(self):
         columns = [
             ("pressure", "dewpoint"),
             ("pressure", "wind_speed", "wind_direction"),
         ]
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             tephi.loadtxt(self.filename_dews, column_titles=columns)
 
     def test_number_of_columns_and_titles_not_equal(self):
         columns = ("pressure", "dewpoint", "wind_speed")
-        with self.assertRaises(TypeError):
+        with pytest.raises(TypeError):
             tephi.loadtxt(self.filename_barbs, column_titles=columns)
 
     def test_invalid_column_titles(self):
         columns = ("pres-sure", "dew+point", 5)
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             tephi.loadtxt(self.filename_dews, column_titles=columns)
 
     def test_non_iterable_column_title(self):
         # For the case of column titles, strings are considered non-iterable.
         columns = "pressure"
-        with self.assertRaises(TypeError):
+        with pytest.raises(TypeError):
             tephi.loadtxt(self.filename_dews, column_titles=columns)
 
     def test_delimiter(self):
         columns = ("pressure", "temperature", "wind_direction", "wind_speed")
         data = tephi.loadtxt(
             self.filename_comma, column_titles=columns, delimiter=","
         )
-        self.assertEqual(data.pressure.shape, (2,))
+        assert data.pressure.shape == (2,)
 
     def test_dtype(self):
         dews = tephi.loadtxt(self.filename_dews, dtype="i4")
-        self.assertIsInstance(dews.pressure[0], np.int32)
-        self.assertIsInstance(dews.temperature[0], np.int32)
+        assert dews.pressure[0].dtype == np.int32
+        assert dews.temperature[0].dtype == np.int32
 
 
+@pytest.mark.graphical
+@pytest.mark.usefixtures("close_plot", "nodeid")
 class TestTephigramPlot(tests.GraphicsTest):
-    def setUp(self):
+    @pytest.fixture(autouse=True)
+    def setup(self):
         self.dews = _expected_dews.T
         self.temps = _expected_temps.T
 
-    def test_plot_dews(self):
-        tpg = Tephigram()
-        tpg.plot(self.dews)
-        self.check_graphic()
-
-    def test_plot_temps(self):
-        tpg = Tephigram()
-        tpg.plot(self.temps)
-        self.check_graphic()
-
-    def test_plot_dews_temps(self):
-        tpg = Tephigram()
-        tpg.plot(self.dews)
-        tpg.plot(self.temps)
-        self.check_graphic()
-
-    def test_plot_dews_label(self):
-        tpg = Tephigram()
-        tpg.plot(self.dews, label="Dew-point temperature")
-        self.check_graphic()
-
-    def test_plot_temps_label(self):
-        tpg = Tephigram()
-        tpg.plot(self.temps, label="Dry-bulb temperature")
-        self.check_graphic()
-
-    def test_plot_dews_custom(self):
-        tpg = Tephigram()
-        tpg.plot(
+    def test_plot_dews(self, nodeid):
+        tephigram = Tephigram()
+        tephigram.plot(self.dews)
+        self.check_graphic(nodeid)
+
+    def test_plot_temps(self, nodeid):
+        tephigram = Tephigram()
+        tephigram.plot(self.temps)
+        self.check_graphic(nodeid)
+
+    def test_plot_dews_temps(self, nodeid):
+        tephigram = Tephigram()
+        tephigram.plot(self.dews)
+        tephigram.plot(self.temps)
+        self.check_graphic(nodeid)
+
+    def test_plot_dews_label(self, nodeid):
+        tephigram = Tephigram()
+        tephigram.plot(self.dews, label="Dew-point temperature")
+        self.check_graphic(nodeid)
+
+    def test_plot_temps_label(self, nodeid):
+        tephigram = Tephigram()
+        tephigram.plot(self.temps, label="Dry-bulb temperature")
+        self.check_graphic(nodeid)
+
+    def test_plot_dews_custom(self, nodeid):
+        tephigram = Tephigram()
+        tephigram.plot(
             self.dews,
             label="Dew-point temperature",
             linewidth=2,
             color="blue",
             marker="s",
         )
-        self.check_graphic()
+        self.check_graphic(nodeid)
 
-    def test_plot_temps_custom(self):
-        tpg = Tephigram()
-        tpg.plot(
+    def test_plot_temps_custom(self, nodeid):
+        tephigram = Tephigram()
+        tephigram.plot(
             self.temps,
             label="Dry-bulb temperature",
             linewidth=2,
             color="red",
             marker="o",
         )
-        self.check_graphic()
+        self.check_graphic(nodeid)
 
-    def test_plot_dews_temps_custom(self):
-        tpg = Tephigram()
-        tpg.plot(
+    def test_plot_dews_temps_custom(self, nodeid):
+        tephigram = Tephigram()
+        tephigram.plot(
             self.dews,
             label="Dew-point temperature",
             linewidth=2,
             color="blue",
             marker="s",
         )
-        tpg.plot(
+        tephigram.plot(
             self.temps,
             label="Dry-bulb temperature",
             linewidth=2,
             color="red",
             marker="o",
         )
-        self.check_graphic()
+        self.check_graphic(nodeid)
 
-    def test_plot_dews_locator_isotherm_numeric(self):
-        tpg = Tephigram(isotherm_locator=10)
-        tpg.plot(self.dews)
-        self.check_graphic()
-
-    def test_plot_dews_locator_isotherm_object(self):
-        tpg = Tephigram(isotherm_locator=tephi.Locator(10))
-        tpg.plot(self.dews)
-        self.check_graphic()
-
-    def test_plot_dews_locator_adiabat_numeric(self):
-        tpg = Tephigram(dry_adiabat_locator=10)
-        tpg.plot(self.dews)
-        self.check_graphic()
-
-    def test_plot_dews_locator_adiabat_object(self):
-        tpg = Tephigram(dry_adiabat_locator=tephi.Locator(10))
-        tpg.plot(self.dews)
-        self.check_graphic()
-
-    def test_plot_dews_locator_numeric(self):
-        tpg = Tephigram(isotherm_locator=10, dry_adiabat_locator=10)
-        tpg.plot(self.dews)
-        self.check_graphic()
+    def test_plot_dews_locator_isotherm_numeric(self, nodeid):
+        tephigram = Tephigram(isotherm_locator=10)
+        tephigram.plot(self.dews)
+        self.check_graphic(nodeid)
+
+    def test_plot_dews_locator_isotherm_object(self, nodeid):
+        tephigram = Tephigram(isotherm_locator=tephi.Locator(10))
+        tephigram.plot(self.dews)
+        self.check_graphic(nodeid)
+
+    def test_plot_dews_locator_adiabat_numeric(self, nodeid):
+        tephigram = Tephigram(dry_adiabat_locator=10)
+        tephigram.plot(self.dews)
+        self.check_graphic(nodeid)
+
+    def test_plot_dews_locator_adiabat_object(self, nodeid):
+        tephigram = Tephigram(dry_adiabat_locator=tephi.Locator(10))
+        tephigram.plot(self.dews)
+        self.check_graphic(nodeid)
+
+    def test_plot_dews_locator_numeric(self, nodeid):
+        tephigram = Tephigram(isotherm_locator=10, dry_adiabat_locator=10)
+        tephigram.plot(self.dews)
+        self.check_graphic(nodeid)
 
-    def test_plot_dews_locator_object(self):
+    def test_plot_dews_locator_object(self, nodeid):
         locator = tephi.Locator(10)
-        tpg = Tephigram(isotherm_locator=locator, dry_adiabat_locator=locator)
-        tpg.plot(self.dews)
-        self.check_graphic()
-
-    def test_plot_anchor(self):
-        tpg = Tephigram(anchor=[(1000, 0), (300, 0)])
-        tpg.plot(self.dews)
-        self.check_graphic()
+        tephigram = Tephigram(
+            isotherm_locator=locator, dry_adiabat_locator=locator
+        )
+        tephigram.plot(self.dews)
+        self.check_graphic(nodeid)
+
+    def test_plot_anchor(self, nodeid):
+        tephigram = Tephigram(anchor=[(1000, 0), (300, 0)])
+        tephigram.plot(self.dews)
+        self.check_graphic(nodeid)
 
 
+@pytest.mark.graphical
+@pytest.mark.usefixtures("close_plot", "nodeid")
 class TestTephigramBarbs(tests.GraphicsTest):
-    def setUp(self):
+    @pytest.fixture(autouse=True)
+    def setup(self):
         self.dews = _expected_dews.T
         self.temps = _expected_temps.T
         magnitude = np.hstack(([0], np.arange(20) * 5 + 2, [102]))
         self.barbs = [(m, 45, 1000 - i * 35) for i, m in enumerate(magnitude)]
 
-    def test_rotate(self):
-        tpg = Tephigram()
-        profile = tpg.plot(self.temps)
+    def test_rotate(self, nodeid):
+        tephigram = Tephigram()
+        profile = tephigram.plot(self.temps)
         profile.barbs(
             [
                 (0, 0, 900),
                 (1, 30, 850),
                 (5, 60, 800),
                 (10, 90, 750),
                 (15, 120, 700),
@@ -232,54 +239,50 @@
                 (40, 270, 450),
                 (45, 300, 400),
                 (50, 330, 350),
                 (55, 360, 300),
             ],
             zorder=10,
         )
-        self.check_graphic()
+        self.check_graphic(nodeid)
 
-    def test_barbs(self):
-        tpg = Tephigram()
-        profile = tpg.plot(self.temps)
+    def test_barbs(self, nodeid):
+        tephigram = Tephigram()
+        profile = tephigram.plot(self.temps)
         profile.barbs(self.barbs, zorder=10)
-        self.check_graphic()
+        self.check_graphic(nodeid)
 
-    def test_barbs_from_file(self):
-        tpg = Tephigram()
+    def test_barbs_from_file(self, nodeid):
+        tephigram = Tephigram()
         dews = _expected_barbs.T[:, :2]
         barbs = np.column_stack(
             (_expected_barbs[2], _expected_barbs[3], _expected_barbs[0])
         )
-        profile = tpg.plot(dews)
+        profile = tephigram.plot(dews)
         profile.barbs(barbs, zorder=10)
-        self.check_graphic()
+        self.check_graphic(nodeid)
 
-    def test_gutter(self):
-        tpg = Tephigram()
-        profile = tpg.plot(self.temps)
+    def test_gutter(self, nodeid):
+        tephigram = Tephigram()
+        profile = tephigram.plot(self.temps)
         profile.barbs(self.barbs, gutter=0.5, zorder=10)
-        self.check_graphic()
+        self.check_graphic(nodeid)
 
-    def test_length(self):
-        tpg = Tephigram()
-        profile = tpg.plot(self.temps)
+    def test_length(self, nodeid):
+        tephigram = Tephigram()
+        profile = tephigram.plot(self.temps)
         profile.barbs(self.barbs, gutter=0.9, length=10, zorder=10)
-        self.check_graphic()
+        self.check_graphic(nodeid)
 
-    def test_color(self):
-        tpg = Tephigram()
-        profile = tpg.plot(self.temps)
+    def test_color(self, nodeid):
+        tephigram = Tephigram()
+        profile = tephigram.plot(self.temps)
         profile.barbs(self.barbs, color="green", zorder=10)
-        self.check_graphic()
+        self.check_graphic(nodeid)
 
-    def test_pivot(self):
-        tpg = Tephigram()
-        tprofile = tpg.plot(self.temps)
+    def test_pivot(self, nodeid):
+        tephigram = Tephigram()
+        tprofile = tephigram.plot(self.temps)
         tprofile.barbs(self.barbs, gutter=0.2, pivot="tip", length=8)
-        dprofile = tpg.plot(self.dews)
+        dprofile = tephigram.plot(self.dews)
         dprofile.barbs(self.barbs, gutter=0.3, pivot="middle", length=8)
-        self.check_graphic()
-
-
-if __name__ == "__main__":
-    unittest.main()
+        self.check_graphic(nodeid)
```

### Comparing `tephi-0.2.4/tephi/transforms.py` & `tephi-0.3.0/tephi/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright Tephi contributors
 #
-# This file is part of Tephi and is released under the LGPL license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
+# This file is part of Tephi and is released under the BSD license.
+# See LICENSE in the root of the repository for full licensing details.
 """
 Tephigram transform support.
 
 """
 from matplotlib.transforms import Transform
 import numpy as np
 
@@ -96,15 +95,15 @@
     pressure, theta = np.asarray(pressure), np.asarray(theta)
 
     # Convert potential temperature from degC to kelvin.
     theta = theta + CONST_KELVIN
 
     # Calculate the temperature given the pressure and
     # potential temperature.
-    kelvin = theta * (pressure ** CONST_K) / (1000.0 ** CONST_K)
+    kelvin = theta * (pressure**CONST_K) / (1000.0**CONST_K)
 
     # Convert temperature from kelvin to degC.
     return pressure, kelvin - CONST_KELVIN
 
 
 def convert_Tt2xy(temperature, theta):
     """
```

