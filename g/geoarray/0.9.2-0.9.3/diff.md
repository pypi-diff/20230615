# Comparing `tmp/geoarray-0.9.2.tar.gz` & `tmp/geoarray-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/geoarray-0.9.2.tar", last modified: Thu Oct  8 21:18:22 2020, max compression
+gzip compressed data, was "dist/geoarray-0.9.3.tar", last modified: Mon Oct 12 10:37:48 2020, max compression
```

## Comparing `geoarray-0.9.2.tar` & `geoarray-0.9.3.tar`

### file list

```diff
@@ -1,72 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-08 21:18:22.886949 geoarray-0.9.2/
--rw-rw-rw-   0 root         (0) root         (0)      292 2020-10-08 21:18:16.000000 geoarray-0.9.2/.editorconfig
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-08 21:18:22.886949 geoarray-0.9.2/.github/
--rw-rw-rw-   0 root         (0) root         (0)      319 2020-10-08 21:18:16.000000 geoarray-0.9.2/.github/ISSUE_TEMPLATE.md
--rw-rw-rw-   0 root         (0) root         (0)      804 2020-10-08 21:18:16.000000 geoarray-0.9.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     2847 2020-10-08 21:18:16.000000 geoarray-0.9.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      442 2020-10-08 21:18:16.000000 geoarray-0.9.2/.travis.yml
--rw-rw-rw-   0 root         (0) root         (0)      270 2020-10-08 21:18:16.000000 geoarray-0.9.2/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)     3282 2020-10-08 21:18:16.000000 geoarray-0.9.2/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)    19916 2020-10-08 21:18:16.000000 geoarray-0.9.2/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1585 2020-10-08 21:18:16.000000 geoarray-0.9.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      264 2020-10-08 21:18:16.000000 geoarray-0.9.2/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     3189 2020-10-08 21:18:16.000000 geoarray-0.9.2/Makefile
--rw-r--r--   0 root         (0) root         (0)    31641 2020-10-08 21:18:22.886949 geoarray-0.9.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3523 2020-10-08 21:18:16.000000 geoarray-0.9.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-08 21:18:22.886949 geoarray-0.9.2/docs/
--rw-rw-rw-   0 root         (0) root         (0)     6773 2020-10-08 21:18:16.000000 geoarray-0.9.2/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-08 21:18:22.882949 geoarray-0.9.2/docs/_build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-08 21:18:22.882949 geoarray-0.9.2/docs/_build/html/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-08 21:18:22.886949 geoarray-0.9.2/docs/_build/html/_static/
--rw-r--r--   0 root         (0) root         (0)      286 2020-09-04 20:38:01.000000 geoarray-0.9.2/docs/_build/html/_static/file.png
--rw-r--r--   0 root         (0) root         (0)       90 2020-09-04 20:38:01.000000 geoarray-0.9.2/docs/_build/html/_static/minus.png
--rw-r--r--   0 root         (0) root         (0)       90 2020-09-04 20:38:01.000000 geoarray-0.9.2/docs/_build/html/_static/plus.png
--rw-rw-rw-   0 root         (0) root         (0)       28 2020-10-08 21:18:16.000000 geoarray-0.9.2/docs/authors.rst
--rwxrwxrwx   0 root         (0) root         (0)     8416 2020-10-08 21:18:16.000000 geoarray-0.9.2/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2020-10-08 21:18:16.000000 geoarray-0.9.2/docs/contributing.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2020-10-08 21:18:16.000000 geoarray-0.9.2/docs/history.rst
--rw-rw-rw-   0 root         (0) root         (0)      281 2020-10-08 21:18:16.000000 geoarray-0.9.2/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1216 2020-10-08 21:18:16.000000 geoarray-0.9.2/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)     6463 2020-10-08 21:18:16.000000 geoarray-0.9.2/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       27 2020-10-08 21:18:16.000000 geoarray-0.9.2/docs/readme.rst
--rw-rw-rw-   0 root         (0) root         (0)       71 2020-10-08 21:18:16.000000 geoarray-0.9.2/docs/usage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-08 21:18:22.882949 geoarray-0.9.2/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-08 21:18:22.886949 geoarray-0.9.2/examples/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)   167682 2020-10-08 21:18:16.000000 geoarray-0.9.2/examples/notebooks/features_and_usage.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-08 21:18:22.886949 geoarray-0.9.2/geoarray/
--rw-rw-rw-   0 root         (0) root         (0)     1672 2020-10-08 21:18:16.000000 geoarray-0.9.2/geoarray/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    79491 2020-10-08 21:18:16.000000 geoarray-0.9.2/geoarray/baseclasses.py
--rw-rw-rw-   0 root         (0) root         (0)     5300 2020-10-08 21:18:16.000000 geoarray-0.9.2/geoarray/masks.py
--rw-rw-rw-   0 root         (0) root         (0)    10044 2020-10-08 21:18:16.000000 geoarray-0.9.2/geoarray/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11567 2020-10-08 21:18:16.000000 geoarray-0.9.2/geoarray/subsetting.py
--rw-rw-rw-   0 root         (0) root         (0)     1073 2020-10-08 21:18:16.000000 geoarray-0.9.2/geoarray/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-08 21:18:22.886949 geoarray-0.9.2/geoarray.egg-info/
--rw-r--r--   0 root         (0) root         (0)    31641 2020-10-08 21:18:22.000000 geoarray-0.9.2/geoarray.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1272 2020-10-08 21:18:22.000000 geoarray-0.9.2/geoarray.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-10-08 21:18:22.000000 geoarray-0.9.2/geoarray.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-10-08 21:18:22.000000 geoarray-0.9.2/geoarray.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      144 2020-10-08 21:18:22.000000 geoarray-0.9.2/geoarray.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2020-10-08 21:18:22.000000 geoarray-0.9.2/geoarray.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      134 2020-10-08 21:18:16.000000 geoarray-0.9.2/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      158 2020-10-08 21:18:16.000000 geoarray-0.9.2/requirements_dev.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2020-10-08 21:18:16.000000 geoarray-0.9.2/requirements_pip.txt
--rw-rw-rw-   0 root         (0) root         (0)      380 2020-10-08 21:18:22.890949 geoarray-0.9.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3126 2020-10-08 21:18:16.000000 geoarray-0.9.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-08 21:18:22.886949 geoarray-0.9.2/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-08 21:18:22.886949 geoarray-0.9.2/tests/CI_docker/
--rw-rw-rw-   0 root         (0) root         (0)     2069 2020-10-08 21:18:16.000000 geoarray-0.9.2/tests/CI_docker/build_testsuite_image.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-08 21:18:22.886949 geoarray-0.9.2/tests/CI_docker/context/
--rw-rw-rw-   0 root         (0) root         (0)      654 2020-10-08 21:18:16.000000 geoarray-0.9.2/tests/CI_docker/context/environment_geoarray.yml
--rw-rw-rw-   0 root         (0) root         (0)      394 2020-10-08 21:18:16.000000 geoarray-0.9.2/tests/CI_docker/context/geoarray_ci.docker
--rw-rw-rw-   0 root         (0) root         (0)     1041 2020-10-08 21:18:16.000000 geoarray-0.9.2/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-08 21:18:22.886949 geoarray-0.9.2/tests/data/
--rwxrwxrwx   0 root         (0) root         (0)     1276 2020-10-08 21:18:16.000000 geoarray-0.9.2/tests/data/L8_2bands_extract10x11.tif
--rwxrwxrwx   0 root         (0) root         (0)     1760 2020-10-08 21:18:16.000000 geoarray-0.9.2/tests/data/L8_2bands_extract10x11_array.txt
--rw-rw-rw-   0 root         (0) root         (0)     1252 2020-10-08 21:18:16.000000 geoarray-0.9.2/tests/data/L8_BadDataMask10x11.tif
--rw-rw-rw-   0 root         (0) root         (0)      500 2020-10-08 21:18:16.000000 geoarray-0.9.2/tests/data/subset_metadata.bsq
--rw-rw-rw-   0 root         (0) root         (0)     1819 2020-10-08 21:18:16.000000 geoarray-0.9.2/tests/data/subset_metadata.hdr
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-08 21:18:22.886949 geoarray-0.9.2/tests/linting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-08 21:18:16.000000 geoarray-0.9.2/tests/linting/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)    36563 2020-10-08 21:18:16.000000 geoarray-0.9.2/tests/test_geoarray.py
--rw-rw-rw-   0 root         (0) root         (0)     3312 2020-10-08 21:18:16.000000 geoarray-0.9.2/tests/test_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2020-10-08 21:18:16.000000 geoarray-0.9.2/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-12 10:37:48.637199 geoarray-0.9.3/
+-rw-rw-rw-   0 root         (0) root         (0)      292 2020-10-12 10:37:42.000000 geoarray-0.9.3/.editorconfig
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-12 10:37:48.633199 geoarray-0.9.3/.github/
+-rw-rw-rw-   0 root         (0) root         (0)      319 2020-10-12 10:37:42.000000 geoarray-0.9.3/.github/ISSUE_TEMPLATE.md
+-rw-rw-rw-   0 root         (0) root         (0)      804 2020-10-12 10:37:42.000000 geoarray-0.9.3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2847 2020-10-12 10:37:42.000000 geoarray-0.9.3/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      442 2020-10-12 10:37:42.000000 geoarray-0.9.3/.travis.yml
+-rw-rw-rw-   0 root         (0) root         (0)      270 2020-10-12 10:37:42.000000 geoarray-0.9.3/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3282 2020-10-12 10:37:42.000000 geoarray-0.9.3/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    20130 2020-10-12 10:37:42.000000 geoarray-0.9.3/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2020-10-12 10:37:42.000000 geoarray-0.9.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      264 2020-10-12 10:37:42.000000 geoarray-0.9.3/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     3189 2020-10-12 10:37:42.000000 geoarray-0.9.3/Makefile
+-rw-r--r--   0 root         (0) root         (0)    31926 2020-10-12 10:37:48.637199 geoarray-0.9.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3541 2020-10-12 10:37:42.000000 geoarray-0.9.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-12 10:37:48.637199 geoarray-0.9.3/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     6773 2020-10-12 10:37:42.000000 geoarray-0.9.3/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-12 10:37:48.633199 geoarray-0.9.3/docs/_build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-12 10:37:48.633199 geoarray-0.9.3/docs/_build/html/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-12 10:37:48.637199 geoarray-0.9.3/docs/_build/html/_static/
+-rw-r--r--   0 root         (0) root         (0)      286 2020-09-04 20:38:01.000000 geoarray-0.9.3/docs/_build/html/_static/file.png
+-rw-r--r--   0 root         (0) root         (0)       90 2020-09-04 20:38:01.000000 geoarray-0.9.3/docs/_build/html/_static/minus.png
+-rw-r--r--   0 root         (0) root         (0)       90 2020-09-04 20:38:01.000000 geoarray-0.9.3/docs/_build/html/_static/plus.png
+-rw-rw-rw-   0 root         (0) root         (0)       28 2020-10-12 10:37:42.000000 geoarray-0.9.3/docs/authors.rst
+-rwxrwxrwx   0 root         (0) root         (0)     8416 2020-10-12 10:37:42.000000 geoarray-0.9.3/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2020-10-12 10:37:42.000000 geoarray-0.9.3/docs/contributing.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2020-10-12 10:37:42.000000 geoarray-0.9.3/docs/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)      281 2020-10-12 10:37:42.000000 geoarray-0.9.3/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1216 2020-10-12 10:37:42.000000 geoarray-0.9.3/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6463 2020-10-12 10:37:42.000000 geoarray-0.9.3/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       27 2020-10-12 10:37:42.000000 geoarray-0.9.3/docs/readme.rst
+-rw-rw-rw-   0 root         (0) root         (0)       71 2020-10-12 10:37:42.000000 geoarray-0.9.3/docs/usage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-12 10:37:48.633199 geoarray-0.9.3/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-12 10:37:48.637199 geoarray-0.9.3/examples/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)   167682 2020-10-12 10:37:42.000000 geoarray-0.9.3/examples/notebooks/features_and_usage.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-12 10:37:48.637199 geoarray-0.9.3/geoarray/
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2020-10-12 10:37:42.000000 geoarray-0.9.3/geoarray/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    79491 2020-10-12 10:37:42.000000 geoarray-0.9.3/geoarray/baseclasses.py
+-rw-rw-rw-   0 root         (0) root         (0)     5300 2020-10-12 10:37:42.000000 geoarray-0.9.3/geoarray/masks.py
+-rw-rw-rw-   0 root         (0) root         (0)    10044 2020-10-12 10:37:42.000000 geoarray-0.9.3/geoarray/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11567 2020-10-12 10:37:42.000000 geoarray-0.9.3/geoarray/subsetting.py
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2020-10-12 10:37:42.000000 geoarray-0.9.3/geoarray/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-12 10:37:48.637199 geoarray-0.9.3/geoarray.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    31926 2020-10-12 10:37:48.000000 geoarray-0.9.3/geoarray.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      873 2020-10-12 10:37:48.000000 geoarray-0.9.3/geoarray.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-10-12 10:37:48.000000 geoarray-0.9.3/geoarray.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-10-12 10:37:48.000000 geoarray-0.9.3/geoarray.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      144 2020-10-12 10:37:48.000000 geoarray-0.9.3/geoarray.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2020-10-12 10:37:48.000000 geoarray-0.9.3/geoarray.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      134 2020-10-12 10:37:42.000000 geoarray-0.9.3/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      158 2020-10-12 10:37:42.000000 geoarray-0.9.3/requirements_dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2020-10-12 10:37:42.000000 geoarray-0.9.3/requirements_pip.txt
+-rw-rw-rw-   0 root         (0) root         (0)      380 2020-10-12 10:37:48.637199 geoarray-0.9.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3116 2020-10-12 10:37:42.000000 geoarray-0.9.3/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      428 2020-10-12 10:37:42.000000 geoarray-0.9.3/tox.ini
```

### Comparing `geoarray-0.9.2/.gitignore` & `geoarray-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `geoarray-0.9.2/.gitlab-ci.yml` & `geoarray-0.9.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `geoarray-0.9.2/CONTRIBUTING.rst` & `geoarray-0.9.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `geoarray-0.9.2/HISTORY.rst` & `geoarray-0.9.3/HISTORY.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =======
 History
 =======
 
+0.9.3 (2020-10-12)
+------------------
+
+* Use SPDX license identifier and set all files to GLP3+ to be consistent with license headers in the source files.
+* Excluded tests from being installed via 'pip install'.
+
+
 0.9.2 (2020-10-08)
 ------------------
 
 * Bugfix for not setting nodata values transparent in GeoArray.show().
 * Moved cartopy import from module level to class level.
 * Filled HISTORY.rst.
```

### Comparing `geoarray-0.9.2/LICENSE` & `geoarray-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geoarray-0.9.2/Makefile` & `geoarray-0.9.3/Makefile`

 * *Files identical despite different names*

### Comparing `geoarray-0.9.2/PKG-INFO` & `geoarray-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: geoarray
-Version: 0.9.2
+Version: 0.9.3
 Summary: Fast Python interface for geodata - either on disk or in memory.
 Home-page: https://gitext.gfz-potsdam.de/danschef/geoarray
 Author: Daniel Scheffler
 Author-email: danschef@gfz-potsdam.de
-License: GNU General Public License v3
+License: GPL-3.0-or-later
 Description: ========
         geoarray
         ========
         
         
         Fast Python interface for geodata - either on disk or in memory.
         
         The geoarray package facilitates reading and writing of all GDAL compatible image file formats
         and provides functions for geospatial processing.
         
         
-        * Free software: GNU General Public License v3
+        * Free software: GNU General Public License v3 or later (GPLv3+)
         * Documentation: https://danschef.gitext-pages.gfz-potsdam.de/geoarray/doc/
         
         
         Status
         ------
         
         .. .. image:: https://img.shields.io/travis/danschef/geoarray.svg
@@ -103,14 +103,21 @@
         .. _here: examples/notebooks/features_and_usage.ipynb
         
         
         =======
         History
         =======
         
+        0.9.3 (2020-10-12)
+        ------------------
+        
+        * Use SPDX license identifier and set all files to GLP3+ to be consistent with license headers in the source files.
+        * Excluded tests from being installed via 'pip install'.
+        
+        
         0.9.2 (2020-10-08)
         ------------------
         
         * Bugfix for not setting nodata values transparent in GeoArray.show().
         * Moved cartopy import from module level to class level.
         * Filled HISTORY.rst.
         
@@ -913,15 +920,15 @@
         
         * Package creation.
         
 Keywords: geoarray,geoprocessing,gdal,numpy
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `geoarray-0.9.2/README.rst` & `geoarray-0.9.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 Fast Python interface for geodata - either on disk or in memory.
 
 The geoarray package facilitates reading and writing of all GDAL compatible image file formats
 and provides functions for geospatial processing.
 
 
-* Free software: GNU General Public License v3
+* Free software: GNU General Public License v3 or later (GPLv3+)
 * Documentation: https://danschef.gitext-pages.gfz-potsdam.de/geoarray/doc/
 
 
 Status
 ------
 
 .. .. image:: https://img.shields.io/travis/danschef/geoarray.svg
```

### Comparing `geoarray-0.9.2/docs/Makefile` & `geoarray-0.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `geoarray-0.9.2/docs/conf.py` & `geoarray-0.9.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `geoarray-0.9.2/docs/installation.rst` & `geoarray-0.9.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `geoarray-0.9.2/docs/make.bat` & `geoarray-0.9.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `geoarray-0.9.2/examples/notebooks/features_and_usage.ipynb` & `geoarray-0.9.3/examples/notebooks/features_and_usage.ipynb`

 * *Files identical despite different names*

### Comparing `geoarray-0.9.2/geoarray/__init__.py` & `geoarray-0.9.3/geoarray/__init__.py`

 * *Files identical despite different names*

### Comparing `geoarray-0.9.2/geoarray/baseclasses.py` & `geoarray-0.9.3/geoarray/baseclasses.py`

 * *Files identical despite different names*

### Comparing `geoarray-0.9.2/geoarray/masks.py` & `geoarray-0.9.3/geoarray/masks.py`

 * *Files identical despite different names*

### Comparing `geoarray-0.9.2/geoarray/metadata.py` & `geoarray-0.9.3/geoarray/metadata.py`

 * *Files identical despite different names*

### Comparing `geoarray-0.9.2/geoarray/subsetting.py` & `geoarray-0.9.3/geoarray/subsetting.py`

 * *Files identical despite different names*

### Comparing `geoarray-0.9.2/geoarray/version.py` & `geoarray-0.9.3/geoarray/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,9 +16,9 @@
 # FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 
-__version__ = '0.9.2'
-__versionalias__ = '20201008.01'
+__version__ = '0.9.3'
+__versionalias__ = '20201012.01'
```

### Comparing `geoarray-0.9.2/geoarray.egg-info/PKG-INFO` & `geoarray-0.9.3/geoarray.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: geoarray
-Version: 0.9.2
+Version: 0.9.3
 Summary: Fast Python interface for geodata - either on disk or in memory.
 Home-page: https://gitext.gfz-potsdam.de/danschef/geoarray
 Author: Daniel Scheffler
 Author-email: danschef@gfz-potsdam.de
-License: GNU General Public License v3
+License: GPL-3.0-or-later
 Description: ========
         geoarray
         ========
         
         
         Fast Python interface for geodata - either on disk or in memory.
         
         The geoarray package facilitates reading and writing of all GDAL compatible image file formats
         and provides functions for geospatial processing.
         
         
-        * Free software: GNU General Public License v3
+        * Free software: GNU General Public License v3 or later (GPLv3+)
         * Documentation: https://danschef.gitext-pages.gfz-potsdam.de/geoarray/doc/
         
         
         Status
         ------
         
         .. .. image:: https://img.shields.io/travis/danschef/geoarray.svg
@@ -103,14 +103,21 @@
         .. _here: examples/notebooks/features_and_usage.ipynb
         
         
         =======
         History
         =======
         
+        0.9.3 (2020-10-12)
+        ------------------
+        
+        * Use SPDX license identifier and set all files to GLP3+ to be consistent with license headers in the source files.
+        * Excluded tests from being installed via 'pip install'.
+        
+        
         0.9.2 (2020-10-08)
         ------------------
         
         * Bugfix for not setting nodata values transparent in GeoArray.show().
         * Moved cartopy import from module level to class level.
         * Filled HISTORY.rst.
         
@@ -913,15 +920,15 @@
         
         * Package creation.
         
 Keywords: geoarray,geoprocessing,gdal,numpy
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `geoarray-0.9.2/setup.py` & `geoarray-0.9.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,25 +56,25 @@
     name='geoarray',
     version=version['__version__'],
     description="Fast Python interface for geodata - either on disk or in memory.",
     long_description=readme + '\n\n' + history,
     author="Daniel Scheffler",
     author_email='danschef@gfz-potsdam.de',
     url='https://gitext.gfz-potsdam.de/danschef/geoarray',
-    packages=find_packages(),  # searches for packages with an __init__.py and returns them as properly formatted list
+    packages=find_packages(exclude=['tests*']),  # searches for packages with an __init__.py and returns a list
     package_dir={'geoarray': 'geoarray'},
     include_package_data=True,
     install_requires=requirements,
-    license="GNU General Public License v3",
+    license="GPL-3.0-or-later",
     zip_safe=False,
     keywords=['geoarray', 'geoprocessing', 'gdal', 'numpy'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
-        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
+        'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```

