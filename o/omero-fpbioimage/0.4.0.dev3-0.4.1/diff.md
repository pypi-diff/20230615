# Comparing `tmp/omero-fpbioimage-0.4.0.dev3.tar.gz` & `tmp/omero-fpbioimage-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/omero-fpbioimage-0.4.0.dev3.tar", last modified: Wed Dec  4 09:01:12 2019, max compression
+gzip compressed data, was "omero-fpbioimage-0.4.1.tar", last modified: Thu Jun 15 12:57:24 2023, max compression
```

## Comparing `omero-fpbioimage-0.4.0.dev3.tar` & `omero-fpbioimage-0.4.1.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-04 09:01:12.000000 omero-fpbioimage-0.4.0.dev3/
--rw-rw-r--   0 travis    (2000) travis    (2000)       55 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2995 2019-12-04 09:01:12.000000 omero-fpbioimage-0.4.0.dev3/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-04 09:01:12.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2995 2019-12-04 09:01:12.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-12-04 09:01:12.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       17 2019-12-04 09:01:12.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-12-04 09:01:12.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)     1599 2019-12-04 09:01:12.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2019-12-04 09:01:12.000000 omero-fpbioimage-0.4.0.dev3/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-04 09:01:12.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-04 09:01:12.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/__pycache__/
--rw-rw-r--   0 travis    (2000) travis    (2000)      267 2019-12-04 09:01:12.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/__pycache__/version.cpython-36.pyc
--rw-rw-r--   0 travis    (2000) travis    (2000)      829 2019-12-04 09:01:12.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/__pycache__/utils.cpython-36.pyc
--rw-rw-r--   0 travis    (2000) travis    (2000)      215 2019-12-04 09:01:12.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/__pycache__/__init__.cpython-36.pyc
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-04 09:01:12.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-04 09:01:12.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1017 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/openwith.js
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-04 09:01:12.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/resources/
--rw-rw-r--   0 travis    (2000) travis    (2000)    43151 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/resources/cambridgeLogo.png
--rw-rw-r--   0 travis    (2000) travis    (2000)   115325 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/resources/LAGlogo.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      321 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/resources/fullscreen.png
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-04 09:01:12.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/
--rw-rw-r--   0 travis    (2000) travis    (2000)   279684 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.asm.memory.unityweb
--rw-rw-r--   0 travis    (2000) travis    (2000)    20466 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/logo.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     5840 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/download.js
--rw-rw-r--   0 travis    (2000) travis    (2000)      353 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    71504 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.asm.framework.unityweb
--rw-rw-r--   0 travis    (2000) travis    (2000)  3311819 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.data.unityweb
--rw-rw-r--   0 travis    (2000) travis    (2000)     2961 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/FPProgress.js
--rw-rw-r--   0 travis    (2000) travis    (2000)   153339 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/UnityLoader.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     3271 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/FPLoader.js
--rw-rw-r--   0 travis    (2000) travis    (2000)      179 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/empty.png
--rw-rw-r--   0 travis    (2000) travis    (2000)  2993719 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.asm.code.unityweb
--rw-rw-r--   0 travis    (2000) travis    (2000)      179 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/full.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     1677 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/urls.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-04 09:01:12.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/templates/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-04 09:01:12.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/templates/fpbioimage/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2538 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/templates/fpbioimage/viewer.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1411 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      938 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1016 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/apps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       65 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5523 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/views.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1386 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2898 2019-12-04 08:56:20.000000 omero-fpbioimage-0.4.0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:57:24.395597 omero-fpbioimage-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-15 12:57:24.395597 omero-fpbioimage-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:57:24.383597 omero-fpbioimage-0.4.1/omero_fpbioimage/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:57:24.383597 omero-fpbioimage-0.4.1/omero_fpbioimage/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-15 12:57:24.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-15 12:57:24.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-15 12:57:24.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/__pycache__/version.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:57:24.379597 omero-fpbioimage-0.4.1/omero_fpbioimage/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:57:24.383597 omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:57:24.395597 omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/
+-rw-r--r--   0 runner    (1001) docker     (123)  2993719 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.asm.code.unityweb
+-rw-r--r--   0 runner    (1001) docker     (123)    71504 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.asm.framework.unityweb
+-rw-r--r--   0 runner    (1001) docker     (123)   279684 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.asm.memory.unityweb
+-rw-r--r--   0 runner    (1001) docker     (123)  3311819 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.data.unityweb
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/FPLoader.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/FPProgress.js
+-rw-r--r--   0 runner    (1001) docker     (123)   153339 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/UnityLoader.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/download.js
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/empty.png
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/full.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20466 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/openwith.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:57:24.395597 omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   115325 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/resources/LAGlogo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    43151 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/resources/cambridgeLogo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/resources/fullscreen.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:57:24.379597 omero-fpbioimage-0.4.1/omero_fpbioimage/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:57:24.395597 omero-fpbioimage-0.4.1/omero_fpbioimage/templates/fpbioimage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/templates/fpbioimage/viewer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/omero_fpbioimage/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:57:24.383597 omero-fpbioimage-0.4.1/omero_fpbioimage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-15 12:57:24.000000 omero-fpbioimage-0.4.1/omero_fpbioimage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-15 12:57:24.000000 omero-fpbioimage-0.4.1/omero_fpbioimage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:57:24.000000 omero-fpbioimage-0.4.1/omero_fpbioimage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:57:24.000000 omero-fpbioimage-0.4.1/omero_fpbioimage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 12:57:24.000000 omero-fpbioimage-0.4.1/omero_fpbioimage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 12:57:24.000000 omero-fpbioimage-0.4.1/omero_fpbioimage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 12:57:24.395597 omero-fpbioimage-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-15 12:57:20.000000 omero-fpbioimage-0.4.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `omero-fpbioimage-0.4.0.dev3/PKG-INFO` & `omero-fpbioimage-0.4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,86 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: omero-fpbioimage
-Version: 0.4.0.dev3
+Version: 0.4.1
 Summary: A Python plugin for OMERO.web
 Home-page: https://github.com/ome/omero-fpbioimage
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: AGPL-3.0
-Download-URL: https://github.com/ome/omero-fpbioimage/archive/v0.4.0dev3.tar.gz
-Description: .. image:: https://travis-ci.org/ome/omero-fpbioimage.svg?branch=master
-            :target: https://travis-ci.org/ome/omero-fpbioimage
-        
-        .. image:: https://badge.fury.io/py/omero-fpbioimage.svg
-            :target: https://badge.fury.io/py/omero-fpbioimage
-        
-        OMERO.FPBioimage
-        ================
-        
-        `FPBioimage <http://fpb.ceb.cam.ac.uk/>`_ is a volumetric visualization tool.
-        FPBioimage as an OMERO.web app.
-        
-        Requirements
-        ============
-        
-        * OMERO 5.2.6 or newer.
-        
-        Installing from PyPI
-        ====================
-        
-        This section assumes that an OMERO.web is already installed.
-        
-        
-        Install the app using `pip <https://pip.pypa.io/en/stable/>`_:
-        
-        ::
-        
-            $ pip install -U omero-fpbioimage
-        
-        Add fpbioimage custom app to your installed web apps:
-        
-        ::
-        
-            $ bin/omero config append omero.web.apps '"omero_fpbioimage"'
-        
-        Optionally add fpbioimage to the 'Open with' config, to enable
-        open-with menu for Images in OMERO.webclient:
-        
-        ::
-        
-            $ bin/omero config append omero.web.open_with '["omero_fpbioimage", "fpbioimage_index",
-              {"script_url": "fpbioimage/openwith.js", "supported_objects": ["image"], "label": "FPBioimage"}]'
-        
-        Now restart OMERO.web as normal.
-        
-        
-        License
-        -------
-        
-        OMERO.FPBioimage is released under the AGPL. 
-        FPBioimage was originally published in `Nature
-        Photonics <https://www.nature.com/nphoton/journal/v11/n2/full/nphoton.2016.273.html>`_
-        
-        Copyright
-        ---------
-        
-        2017-2018, The Open Microscopy Environment
+Download-URL: https://github.com/ome/omero-fpbioimage/archive/v0.4.1.tar.gz
 Keywords: OMERO.web,plugin
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
-Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Text Processing :: Markup :: HTML
+Requires-Python: >=3
+
+.. image:: https://github.com/ome/omero-fpbioimage/workflows/OMERO/badge.svg
+    :target: https://github.com/ome/omero-fpbioimage/actions
+
+.. image:: https://badge.fury.io/py/omero-fpbioimage.svg
+    :target: https://badge.fury.io/py/omero-fpbioimage
+
+OMERO.FPBioimage
+================
+
+`FPBioimage <http://fpb.ceb.cam.ac.uk/>`_ is a volumetric visualization tool.
+FPBioimage as an OMERO.web app.
+
+Requirements
+============
+
+* OMERO.web 5.6 or newer.
+
+Installing from PyPI
+====================
+
+This section assumes that an OMERO.web is already installed.
+
+
+Install the app using `pip <https://pip.pypa.io/en/stable/>`_:
+
+::
+
+    $ pip install -U omero-fpbioimage
+
+Add fpbioimage custom app to your installed web apps:
+
+::
+
+    $ bin/omero config append omero.web.apps '"omero_fpbioimage"'
+
+Optionally add fpbioimage to the 'Open with' config, to enable
+open-with menu for Images in OMERO.webclient:
+
+::
+
+    $ bin/omero config append omero.web.open_with '["omero_fpbioimage", "fpbioimage_index",
+      {"script_url": "fpbioimage/openwith.js", "supported_objects": ["image"], "label": "FPBioimage"}]'
+
+Now restart OMERO.web as normal.
+
+
+License
+-------
+
+OMERO.FPBioimage is released under the AGPL. 
+FPBioimage was originally published in `Nature
+Photonics <https://www.nature.com/nphoton/journal/v11/n2/full/nphoton.2016.273.html>`_
+
+Copyright
+---------
+
+2017-2020, The Open Microscopy Environment
+
```

### Comparing `omero-fpbioimage-0.4.0.dev3/omero_fpbioimage.egg-info/PKG-INFO` & `omero-fpbioimage-0.4.1/omero_fpbioimage.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,86 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: omero-fpbioimage
-Version: 0.4.0.dev3
+Version: 0.4.1
 Summary: A Python plugin for OMERO.web
 Home-page: https://github.com/ome/omero-fpbioimage
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: AGPL-3.0
-Download-URL: https://github.com/ome/omero-fpbioimage/archive/v0.4.0dev3.tar.gz
-Description: .. image:: https://travis-ci.org/ome/omero-fpbioimage.svg?branch=master
-            :target: https://travis-ci.org/ome/omero-fpbioimage
-        
-        .. image:: https://badge.fury.io/py/omero-fpbioimage.svg
-            :target: https://badge.fury.io/py/omero-fpbioimage
-        
-        OMERO.FPBioimage
-        ================
-        
-        `FPBioimage <http://fpb.ceb.cam.ac.uk/>`_ is a volumetric visualization tool.
-        FPBioimage as an OMERO.web app.
-        
-        Requirements
-        ============
-        
-        * OMERO 5.2.6 or newer.
-        
-        Installing from PyPI
-        ====================
-        
-        This section assumes that an OMERO.web is already installed.
-        
-        
-        Install the app using `pip <https://pip.pypa.io/en/stable/>`_:
-        
-        ::
-        
-            $ pip install -U omero-fpbioimage
-        
-        Add fpbioimage custom app to your installed web apps:
-        
-        ::
-        
-            $ bin/omero config append omero.web.apps '"omero_fpbioimage"'
-        
-        Optionally add fpbioimage to the 'Open with' config, to enable
-        open-with menu for Images in OMERO.webclient:
-        
-        ::
-        
-            $ bin/omero config append omero.web.open_with '["omero_fpbioimage", "fpbioimage_index",
-              {"script_url": "fpbioimage/openwith.js", "supported_objects": ["image"], "label": "FPBioimage"}]'
-        
-        Now restart OMERO.web as normal.
-        
-        
-        License
-        -------
-        
-        OMERO.FPBioimage is released under the AGPL. 
-        FPBioimage was originally published in `Nature
-        Photonics <https://www.nature.com/nphoton/journal/v11/n2/full/nphoton.2016.273.html>`_
-        
-        Copyright
-        ---------
-        
-        2017-2018, The Open Microscopy Environment
+Download-URL: https://github.com/ome/omero-fpbioimage/archive/v0.4.1.tar.gz
 Keywords: OMERO.web,plugin
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
-Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Text Processing :: Markup :: HTML
+Requires-Python: >=3
+
+.. image:: https://github.com/ome/omero-fpbioimage/workflows/OMERO/badge.svg
+    :target: https://github.com/ome/omero-fpbioimage/actions
+
+.. image:: https://badge.fury.io/py/omero-fpbioimage.svg
+    :target: https://badge.fury.io/py/omero-fpbioimage
+
+OMERO.FPBioimage
+================
+
+`FPBioimage <http://fpb.ceb.cam.ac.uk/>`_ is a volumetric visualization tool.
+FPBioimage as an OMERO.web app.
+
+Requirements
+============
+
+* OMERO.web 5.6 or newer.
+
+Installing from PyPI
+====================
+
+This section assumes that an OMERO.web is already installed.
+
+
+Install the app using `pip <https://pip.pypa.io/en/stable/>`_:
+
+::
+
+    $ pip install -U omero-fpbioimage
+
+Add fpbioimage custom app to your installed web apps:
+
+::
+
+    $ bin/omero config append omero.web.apps '"omero_fpbioimage"'
+
+Optionally add fpbioimage to the 'Open with' config, to enable
+open-with menu for Images in OMERO.webclient:
+
+::
+
+    $ bin/omero config append omero.web.open_with '["omero_fpbioimage", "fpbioimage_index",
+      {"script_url": "fpbioimage/openwith.js", "supported_objects": ["image"], "label": "FPBioimage"}]'
+
+Now restart OMERO.web as normal.
+
+
+License
+-------
+
+OMERO.FPBioimage is released under the AGPL. 
+FPBioimage was originally published in `Nature
+Photonics <https://www.nature.com/nphoton/journal/v11/n2/full/nphoton.2016.273.html>`_
+
+Copyright
+---------
+
+2017-2020, The Open Microscopy Environment
+
```

### Comparing `omero-fpbioimage-0.4.0.dev3/omero_fpbioimage.egg-info/SOURCES.txt` & `omero-fpbioimage-0.4.1/omero_fpbioimage.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 omero_fpbioimage/utils.py
 omero_fpbioimage/version.py
 omero_fpbioimage/views.py
 omero_fpbioimage.egg-info/PKG-INFO
 omero_fpbioimage.egg-info/SOURCES.txt
 omero_fpbioimage.egg-info/dependency_links.txt
 omero_fpbioimage.egg-info/not-zip-safe
+omero_fpbioimage.egg-info/requires.txt
 omero_fpbioimage.egg-info/top_level.txt
-omero_fpbioimage/__pycache__/__init__.cpython-36.pyc
-omero_fpbioimage/__pycache__/utils.cpython-36.pyc
-omero_fpbioimage/__pycache__/version.cpython-36.pyc
+omero_fpbioimage/__pycache__/__init__.cpython-310.pyc
+omero_fpbioimage/__pycache__/utils.cpython-310.pyc
+omero_fpbioimage/__pycache__/version.cpython-310.pyc
 omero_fpbioimage/static/fpbioimage/openwith.js
 omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.asm.code.unityweb
 omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.asm.framework.unityweb
 omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.asm.memory.unityweb
 omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.data.unityweb
 omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.json
 omero_fpbioimage/static/fpbioimage/FPBioimage/FPLoader.js
```

### Comparing `omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/openwith.js` & `omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/openwith.js`

 * *Files identical despite different names*

### Comparing `omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/resources/cambridgeLogo.png` & `omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/resources/cambridgeLogo.png`

 * *Files identical despite different names*

### Comparing `omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/resources/LAGlogo.png` & `omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/resources/LAGlogo.png`

 * *Files identical despite different names*

### Comparing `omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.asm.memory.unityweb` & `omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.asm.memory.unityweb`

 * *Files identical despite different names*

### Comparing `omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/logo.png` & `omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/logo.png`

 * *Files identical despite different names*

### Comparing `omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/download.js` & `omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/download.js`

 * *Files identical despite different names*

### Comparing `omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.asm.framework.unityweb` & `omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.asm.framework.unityweb`

 * *Files identical despite different names*

### Comparing `omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.data.unityweb` & `omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.data.unityweb`

 * *Files identical despite different names*

### Comparing `omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/FPProgress.js` & `omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/FPProgress.js`

 * *Files identical despite different names*

### Comparing `omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/UnityLoader.js` & `omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/UnityLoader.js`

 * *Files identical despite different names*

### Comparing `omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/FPLoader.js` & `omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/FPLoader.js`

 * *Files identical despite different names*

### Comparing `omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.asm.code.unityweb` & `omero-fpbioimage-0.4.1/omero_fpbioimage/static/fpbioimage/FPBioimage/FPBioimage.asm.code.unityweb`

 * *Files identical despite different names*

### Comparing `omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/urls.py` & `omero-fpbioimage-0.4.1/omero_fpbioimage/urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,32 +18,32 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 # Version: 1.0
 #
 
-from django.conf.urls import url
+from django.urls import re_path
 
 from . import views
 
 
 urlpatterns = [
 
     # index placeholder
-    url(r'^$', views.index, name='fpbioimage_index'),
+    re_path(r'^$', views.index, name='fpbioimage_index'),
 
     # Viewer page
-    url(r'^viewer/(?P<image_id>[0-9]+)/', views.fpbioimage,
-        name='fpbioimage_viewer'),
+    re_path(r'^viewer/(?P<image_id>[0-9]+)/', views.fpbioimage,
+            name='fpbioimage_viewer'),
 
     # PNG plane. This is used for 'first_image'
-    url(r'^imageStacks/(?P<image_id>[0-9]+)/(?P<atlas_index>[0-9]+)\.png',
-        views.fpbioimage_png, name='fpbioimage_png'),
+    re_path(r'^imageStacks/(?P<image_id>[0-9]+)/(?P<atlas_index>[0-9]+)\.png',
+            views.fpbioimage_png, name='fpbioimage_png'),
 
     # PNG planes to load whole stack.
     # Can't seem to control how this url is generated in JavaScript from
     # the 'first_image' url above. So it's ugly but this works for now.
-    url(r'^viewer//fpbioimage/imageStacks/'
-        '(?P<image_id>[0-9]+)/(?P<atlas_index>[0-9]+)\.png',
-        views.fpbioimage_png, name='fpbioimage_png2'),
+    re_path(r'^viewer//fpbioimage/imageStacks/'
+            '(?P<image_id>[0-9]+)/(?P<atlas_index>[0-9]+)\.png',
+            views.fpbioimage_png, name='fpbioimage_png2'),
 ]
```

### Comparing `omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/templates/fpbioimage/viewer.html` & `omero-fpbioimage-0.4.1/omero_fpbioimage/templates/fpbioimage/viewer.html`

 * *Files identical despite different names*

### Comparing `omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/utils.py` & `omero-fpbioimage-0.4.1/omero_fpbioimage/utils.py`

 * *Files identical despite different names*

### Comparing `omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/version.py` & `omero-fpbioimage-0.4.1/omero_fpbioimage/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,11 +18,11 @@
 #
 # Version: 1.0
 #
 
 from .utils import get_version
 
 
-VERSION = (0, 4, 0, "dev3")
+VERSION = (0, 4, 1)
 
 
 __version__ = get_version(VERSION)
```

### Comparing `omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/apps.py` & `omero-fpbioimage-0.4.1/omero_fpbioimage/apps.py`

 * *Files identical despite different names*

### Comparing `omero-fpbioimage-0.4.0.dev3/omero_fpbioimage/views.py` & `omero-fpbioimage-0.4.1/omero_fpbioimage/views.py`

 * *Files identical despite different names*

### Comparing `omero-fpbioimage-0.4.0.dev3/README.rst` & `omero-fpbioimage-0.4.1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-.. image:: https://travis-ci.org/ome/omero-fpbioimage.svg?branch=master
-    :target: https://travis-ci.org/ome/omero-fpbioimage
+.. image:: https://github.com/ome/omero-fpbioimage/workflows/OMERO/badge.svg
+    :target: https://github.com/ome/omero-fpbioimage/actions
 
 .. image:: https://badge.fury.io/py/omero-fpbioimage.svg
     :target: https://badge.fury.io/py/omero-fpbioimage
 
 OMERO.FPBioimage
 ================
 
 `FPBioimage <http://fpb.ceb.cam.ac.uk/>`_ is a volumetric visualization tool.
 FPBioimage as an OMERO.web app.
 
 Requirements
 ============
 
-* OMERO 5.2.6 or newer.
+* OMERO.web 5.6 or newer.
 
 Installing from PyPI
 ====================
 
 This section assumes that an OMERO.web is already installed.
 
 
@@ -50,8 +50,8 @@
 OMERO.FPBioimage is released under the AGPL. 
 FPBioimage was originally published in `Nature
 Photonics <https://www.nature.com/nphoton/journal/v11/n2/full/nphoton.2016.273.html>`_
 
 Copyright
 ---------
 
-2017-2018, The Open Microscopy Environment
+2017-2020, The Open Microscopy Environment
```

### Comparing `omero-fpbioimage-0.4.0.dev3/setup.py` & `omero-fpbioimage-0.4.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,15 +53,15 @@
           'Environment :: Web Environment',
           'Framework :: Django',
           'Intended Audience :: End Users/Desktop',
           'Intended Audience :: Science/Research',
           'Natural Language :: English',
           'Operating System :: OS Independent',
           'Programming Language :: JavaScript',
-          'Programming Language :: Python :: 2',
+          'Programming Language :: Python :: 3',
           'Topic :: Internet :: WWW/HTTP',
           'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
           'Topic :: Internet :: WWW/HTTP :: WSGI',
           'Topic :: Scientific/Engineering :: Visualization',
           'Topic :: Software Development :: Libraries :: '
           'Application Frameworks',
           'Topic :: Text Processing :: Markup :: HTML'
@@ -69,10 +69,12 @@
           # http://pypi.python.org/pypi?%3Aaction=list_classifiers
       author='The Open Microscopy Team',
       author_email='ome-devel@lists.openmicroscopy.org.uk',
       license='AGPL-3.0',
       url="https://github.com/ome/omero-fpbioimage",
       download_url='https://github.com/ome/omero-fpbioimage/archive/v%s.tar.gz' % version,  # NOQA
       keywords=['OMERO.web', 'plugin'],
+      install_requires=['omero-web>=5.6.0'],
+      python_requires='>=3',
       include_package_data=True,
       zip_safe=False,
       )
```

