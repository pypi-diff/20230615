# Comparing `tmp/multitrackpro-0.1.1.tar.gz` & `tmp/multitrackpro-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multitrackpro-0.1.1.tar", last modified: Fri Jun  9 22:34:21 2023, max compression
+gzip compressed data, was "multitrackpro-0.1.2.tar", last modified: Wed Jun 14 22:25:38 2023, max compression
```

## Comparing `multitrackpro-0.1.1.tar` & `multitrackpro-0.1.2.tar`

### file list

```diff
@@ -1,45 +1,69 @@
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 22:34:21.767862 multitrackpro-0.1.1/
--rw-rw-r--   0 sk        (1000) sk        (1000)      165 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/AUTHORS.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)     3611 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/CONTRIBUTING.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)      179 2023-06-09 20:51:56.000000 multitrackpro-0.1.1/HISTORY.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)     1613 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/LICENSE
--rw-rw-r--   0 sk        (1000) sk        (1000)      262 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/MANIFEST.in
--rw-rw-r--   0 sk        (1000) sk        (1000)     3242 2023-06-09 22:34:21.767862 multitrackpro-0.1.1/PKG-INFO
--rw-rw-r--   0 sk        (1000) sk        (1000)     1647 2023-06-09 21:56:44.000000 multitrackpro-0.1.1/README.rst
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 22:34:21.767862 multitrackpro-0.1.1/docs/
--rw-rw-r--   0 sk        (1000) sk        (1000)      614 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/docs/Makefile
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 22:34:21.763862 multitrackpro-0.1.1/docs/_build/
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 22:34:21.763862 multitrackpro-0.1.1/docs/_build/html/
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 22:34:21.767862 multitrackpro-0.1.1/docs/_build/html/_static/
--rw-rw-r--   0 sk        (1000) sk        (1000)      286 2023-06-09 12:32:19.000000 multitrackpro-0.1.1/docs/_build/html/_static/file.png
--rw-rw-r--   0 sk        (1000) sk        (1000)       90 2023-06-09 12:32:19.000000 multitrackpro-0.1.1/docs/_build/html/_static/minus.png
--rw-rw-r--   0 sk        (1000) sk        (1000)       90 2023-06-09 12:32:19.000000 multitrackpro-0.1.1/docs/_build/html/_static/plus.png
--rw-rw-r--   0 sk        (1000) sk        (1000)       28 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/docs/authors.rst
--rwxrwxr-x   0 sk        (1000) sk        (1000)     4868 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/docs/conf.py
--rw-rw-r--   0 sk        (1000) sk        (1000)       33 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/docs/contributing.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)       28 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/docs/history.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)      310 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/docs/index.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)     1182 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/docs/installation.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)      811 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/docs/make.bat
--rw-rw-r--   0 sk        (1000) sk        (1000)       73 2023-06-09 22:33:10.000000 multitrackpro-0.1.1/docs/modules.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)      632 2023-06-09 22:33:10.000000 multitrackpro-0.1.1/docs/multitracker.core.io.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)      645 2023-06-09 22:33:10.000000 multitrackpro-0.1.1/docs/multitracker.core.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)      374 2023-06-09 22:33:10.000000 multitrackpro-0.1.1/docs/multitracker.qt.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)      784 2023-06-09 22:33:10.000000 multitrackpro-0.1.1/docs/multitracker.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)       27 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/docs/readme.rst
--rw-rw-r--   0 sk        (1000) sk        (1000)       81 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/docs/usage.rst
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 22:34:21.767862 multitrackpro-0.1.1/multitracker/
--rw-rw-r--   0 sk        (1000) sk        (1000)     4395 2023-06-09 20:50:32.000000 multitrackpro-0.1.1/multitracker/auto_annotate_pro.py
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 22:34:21.767862 multitrackpro-0.1.1/multitrackpro.egg-info/
--rw-rw-r--   0 sk        (1000) sk        (1000)     3242 2023-06-09 22:34:21.000000 multitrackpro-0.1.1/multitrackpro.egg-info/PKG-INFO
--rw-rw-r--   0 sk        (1000) sk        (1000)      819 2023-06-09 22:34:21.000000 multitrackpro-0.1.1/multitrackpro.egg-info/SOURCES.txt
--rw-rw-r--   0 sk        (1000) sk        (1000)        1 2023-06-09 22:34:21.000000 multitrackpro-0.1.1/multitrackpro.egg-info/dependency_links.txt
--rw-rw-r--   0 sk        (1000) sk        (1000)       61 2023-06-09 22:34:21.000000 multitrackpro-0.1.1/multitrackpro.egg-info/entry_points.txt
--rw-rw-r--   0 sk        (1000) sk        (1000)        1 2023-06-09 22:34:21.000000 multitrackpro-0.1.1/multitrackpro.egg-info/not-zip-safe
--rw-rw-r--   0 sk        (1000) sk        (1000)       65 2023-06-09 22:34:21.000000 multitrackpro-0.1.1/multitrackpro.egg-info/requires.txt
--rw-rw-r--   0 sk        (1000) sk        (1000)        1 2023-06-09 22:34:21.000000 multitrackpro-0.1.1/multitrackpro.egg-info/top_level.txt
--rw-rw-r--   0 sk        (1000) sk        (1000)      407 2023-06-09 22:34:21.771862 multitrackpro-0.1.1/setup.cfg
--rw-rw-r--   0 sk        (1000) sk        (1000)     2235 2023-06-09 22:18:53.000000 multitrackpro-0.1.1/setup.py
-drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-09 22:34:21.767862 multitrackpro-0.1.1/tests/
--rw-rw-r--   0 sk        (1000) sk        (1000)       43 2023-06-09 10:59:19.000000 multitrackpro-0.1.1/tests/__init__.py
--rw-rw-r--   0 sk        (1000) sk        (1000)      376 2023-06-09 22:31:54.000000 multitrackpro-0.1.1/tests/test_multitrackpro.py
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/
+-rw-rw-r--   0 sk        (1000) sk        (1000)      165 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/AUTHORS.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)     3611 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/CONTRIBUTING.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      230 2023-06-14 22:23:47.000000 multitrackpro-0.1.2/HISTORY.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)     1613 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/LICENSE
+-rw-rw-r--   0 sk        (1000) sk        (1000)      262 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/MANIFEST.in
+-rw-rw-r--   0 sk        (1000) sk        (1000)     3304 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/PKG-INFO
+-rw-rw-r--   0 sk        (1000) sk        (1000)     1658 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/README.rst
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.094647 multitrackpro-0.1.2/docs/
+-rw-rw-r--   0 sk        (1000) sk        (1000)      613 2023-06-13 00:07:22.000000 multitrackpro-0.1.2/docs/Makefile
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.094647 multitrackpro-0.1.2/docs/_build/
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.094647 multitrackpro-0.1.2/docs/_build/html/
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.094647 multitrackpro-0.1.2/docs/_build/html/_static/
+-rw-rw-r--   0 sk        (1000) sk        (1000)      286 2023-06-09 12:32:19.000000 multitrackpro-0.1.2/docs/_build/html/_static/file.png
+-rw-rw-r--   0 sk        (1000) sk        (1000)       90 2023-06-09 12:32:19.000000 multitrackpro-0.1.2/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 sk        (1000) sk        (1000)       90 2023-06-09 12:32:19.000000 multitrackpro-0.1.2/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 sk        (1000) sk        (1000)       28 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/docs/authors.rst
+-rwxrwxr-x   0 sk        (1000) sk        (1000)     4865 2023-06-13 00:08:18.000000 multitrackpro-0.1.2/docs/conf.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)       33 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/docs/contributing.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)       28 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/docs/history.rst
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.094647 multitrackpro-0.1.2/docs/html/
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/docs/html/_static/
+-rw-rw-r--   0 sk        (1000) sk        (1000)      286 2023-06-09 12:32:19.000000 multitrackpro-0.1.2/docs/html/_static/file.png
+-rw-rw-r--   0 sk        (1000) sk        (1000)       90 2023-06-09 12:32:19.000000 multitrackpro-0.1.2/docs/html/_static/minus.png
+-rw-rw-r--   0 sk        (1000) sk        (1000)       90 2023-06-09 12:32:19.000000 multitrackpro-0.1.2/docs/html/_static/plus.png
+-rw-rw-r--   0 sk        (1000) sk        (1000)      313 2023-06-10 09:05:27.000000 multitrackpro-0.1.2/docs/index.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)     1182 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/docs/installation.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      811 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/docs/make.bat
+-rw-rw-r--   0 sk        (1000) sk        (1000)       73 2023-06-14 22:24:28.000000 multitrackpro-0.1.2/docs/modules.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      632 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/docs/multitracker.core.io.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      645 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/docs/multitracker.core.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      409 2023-06-13 00:08:47.000000 multitrackpro-0.1.2/docs/multitracker.core.tracker.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      374 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/docs/multitracker.qt.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)      784 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/docs/multitracker.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)       27 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/docs/readme.rst
+-rw-rw-r--   0 sk        (1000) sk        (1000)       81 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/docs/usage.rst
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/multitracker/
+-rw-rw-r--   0 sk        (1000) sk        (1000)      140 2023-06-14 22:24:11.000000 multitrackpro-0.1.2/multitracker/__init__.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)     6427 2023-06-14 20:58:57.000000 multitrackpro-0.1.2/multitracker/auto_annotate_pro.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)       20 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/multitracker/config.py
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/multitracker/core/
+-rw-rw-r--   0 sk        (1000) sk        (1000)        0 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/multitracker/core/__init__.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)     1997 2023-06-13 19:14:44.000000 multitrackpro-0.1.2/multitracker/core/dataset_manager.py
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/multitracker/core/io/
+-rw-rw-r--   0 sk        (1000) sk        (1000)        0 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/multitracker/core/io/__init__.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)     2267 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/multitracker/core/io/cached_video_reader.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)     1176 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/multitracker/core/io/multi_video_manager.py
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/multitracker/core/tracker/
+-rw-rw-r--   0 sk        (1000) sk        (1000)      322 2023-06-13 00:02:34.000000 multitrackpro-0.1.2/multitracker/core/tracker/Tracker.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)        0 2023-06-12 21:05:37.000000 multitrackpro-0.1.2/multitracker/core/tracker/__init__.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)      411 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/multitracker/core/video_utils.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)       19 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/multitracker/multi_track_pro.py
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/multitracker/qt/
+-rw-rw-r--   0 sk        (1000) sk        (1000)        0 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/multitracker/qt/__init__.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)     7666 2023-06-13 00:02:34.000000 multitrackpro-0.1.2/multitracker/qt/my_main_window.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)        0 2023-06-13 12:52:14.000000 multitrackpro-0.1.2/multitracker/stackoverflow.py
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/multitrackpro.egg-info/
+-rw-rw-r--   0 sk        (1000) sk        (1000)     3304 2023-06-14 22:25:38.000000 multitrackpro-0.1.2/multitrackpro.egg-info/PKG-INFO
+-rw-rw-r--   0 sk        (1000) sk        (1000)     1404 2023-06-14 22:25:38.000000 multitrackpro-0.1.2/multitrackpro.egg-info/SOURCES.txt
+-rw-rw-r--   0 sk        (1000) sk        (1000)        1 2023-06-14 22:25:38.000000 multitrackpro-0.1.2/multitrackpro.egg-info/dependency_links.txt
+-rw-rw-r--   0 sk        (1000) sk        (1000)       61 2023-06-14 22:25:38.000000 multitrackpro-0.1.2/multitrackpro.egg-info/entry_points.txt
+-rw-rw-r--   0 sk        (1000) sk        (1000)        1 2023-06-14 22:25:38.000000 multitrackpro-0.1.2/multitrackpro.egg-info/not-zip-safe
+-rw-rw-r--   0 sk        (1000) sk        (1000)       81 2023-06-14 22:25:38.000000 multitrackpro-0.1.2/multitrackpro.egg-info/requires.txt
+-rw-rw-r--   0 sk        (1000) sk        (1000)       13 2023-06-14 22:25:38.000000 multitrackpro-0.1.2/multitrackpro.egg-info/top_level.txt
+-rw-rw-r--   0 sk        (1000) sk        (1000)      407 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/setup.cfg
+-rw-rw-r--   0 sk        (1000) sk        (1000)     2342 2023-06-14 22:24:14.000000 multitrackpro-0.1.2/setup.py
+drwxrwxr-x   0 sk        (1000) sk        (1000)        0 2023-06-14 22:25:38.098647 multitrackpro-0.1.2/tests/
+-rw-rw-r--   0 sk        (1000) sk        (1000)       43 2023-06-09 10:59:19.000000 multitrackpro-0.1.2/tests/__init__.py
+-rw-rw-r--   0 sk        (1000) sk        (1000)      376 2023-06-09 22:39:14.000000 multitrackpro-0.1.2/tests/test_multitrackpro.py
```

### Comparing `multitrackpro-0.1.1/CONTRIBUTING.rst` & `multitrackpro-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.1/LICENSE` & `multitrackpro-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.1/PKG-INFO` & `multitrackpro-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multitrackpro
-Version: 0.1.1
+Version: 0.1.2
 Summary: A multi-camera multi-object tracking library with its own labelling tool to annotate datasets.
 Home-page: https://github.com/saurabheights/multitrackpro
 Author: Saurabh Khanduja
 Author-email: pixelperceive@gmail.com
 License: GNU General Public License v3
 Keywords: multitrackpro,annotation,labelling,machine-learning,deep-learning,vision,ML,DL,AI,YOLO
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -44,15 +44,15 @@
 
 
 
 A multi-camera multi-object tracking library with its own labelling tool to annotate datasets.
 
 
 * Free software: GNU General Public License v3
-* Documentation: https://multitrackpro.readthedocs.io.
+* Documentation: https://readthedocs.org/projects/multitrackpro/.
 
 
 Features
 --------
 
 * QT based media player that can play four videos at the same time.
 
@@ -97,7 +97,12 @@
 
 * First release on PyPI.
 
 0.1.1 (2023-06-09)
 ------------------
 
 * Added video player that plays exactly 4 videos.
+
+0.1.2 (2023-06-15)
+------------------
+
+* BugFixes
```

### Comparing `multitrackpro-0.1.1/README.rst` & `multitrackpro-0.1.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 
 A multi-camera multi-object tracking library with its own labelling tool to annotate datasets.
 
 
 * Free software: GNU General Public License v3
-* Documentation: https://multitrackpro.readthedocs.io.
+* Documentation: https://readthedocs.org/projects/multitrackpro/.
 
 
 Features
 --------
 
 * QT based media player that can play four videos at the same time.
```

### Comparing `multitrackpro-0.1.1/docs/Makefile` & `multitrackpro-0.1.2/docs/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Minimal makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line.
 SPHINXOPTS    =
 SPHINXBUILD   = python -msphinx
-SPHINXPROJ    = multitrackpro
+SPHINXPROJ    = multitracker
 SOURCEDIR     = .
 BUILDDIR      = _build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `multitrackpro-0.1.1/docs/conf.py` & `multitrackpro-0.1.2/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #
 import os
 import sys
 sys.path.insert(0, os.path.abspath('..'))
 
-import multitrackpro
+import multitracker
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
@@ -51,17 +51,17 @@
 author = "Saurabh Khanduja"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
-version = multitrackpro.__version__
+version = multitracker.__version__
 # The full version, including alpha/beta/rc tags.
-release = multitrackpro.__version__
+release = multitracker.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `multitrackpro-0.1.1/docs/installation.rst` & `multitrackpro-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.1/docs/make.bat` & `multitrackpro-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.1/docs/multitracker.core.io.rst` & `multitrackpro-0.1.2/docs/multitracker.core.io.rst`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.1/docs/multitracker.core.rst` & `multitrackpro-0.1.2/docs/multitracker.core.rst`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.1/docs/multitracker.rst` & `multitrackpro-0.1.2/docs/multitracker.rst`

 * *Files identical despite different names*

### Comparing `multitrackpro-0.1.1/multitrackpro.egg-info/PKG-INFO` & `multitrackpro-0.1.2/multitrackpro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multitrackpro
-Version: 0.1.1
+Version: 0.1.2
 Summary: A multi-camera multi-object tracking library with its own labelling tool to annotate datasets.
 Home-page: https://github.com/saurabheights/multitrackpro
 Author: Saurabh Khanduja
 Author-email: pixelperceive@gmail.com
 License: GNU General Public License v3
 Keywords: multitrackpro,annotation,labelling,machine-learning,deep-learning,vision,ML,DL,AI,YOLO
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -44,15 +44,15 @@
 
 
 
 A multi-camera multi-object tracking library with its own labelling tool to annotate datasets.
 
 
 * Free software: GNU General Public License v3
-* Documentation: https://multitrackpro.readthedocs.io.
+* Documentation: https://readthedocs.org/projects/multitrackpro/.
 
 
 Features
 --------
 
 * QT based media player that can play four videos at the same time.
 
@@ -97,7 +97,12 @@
 
 * First release on PyPI.
 
 0.1.1 (2023-06-09)
 ------------------
 
 * Added video player that plays exactly 4 videos.
+
+0.1.2 (2023-06-15)
+------------------
+
+* BugFixes
```

### Comparing `multitrackpro-0.1.1/setup.py` & `multitrackpro-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = [
+    "boxmot>=10.0.13",
     "linetimer>=0.1.5",
-    "numpy>=1.24.3",
-    "opencv-python>= 4.7.0",
+    "numpy==1.23.1",  # See https://github.com/mikel-brostrom/yolo_tracking/blame/master/requirements.txt
+    "opencv-python>=4.7.0",
     "pyqt6>=6.5.1",
 ]
 
 test_requirements = [ ]
 
 setup(
     author="Saurabh Khanduja",
@@ -48,16 +49,16 @@
     install_requires=requirements,
     license="GNU General Public License v3",
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/x-rst',
     include_package_data=True,
     keywords='multitrackpro, annotation, labelling, machine-learning, deep-learning, vision, ML, DL, AI, YOLO',
     name='multitrackpro',
-    packages=find_packages(include=['multitrackpro', 'multitrackpro.*']),
+    packages=find_packages(include=['multitracker', 'multitracker.*']),
     python_requires='>=3.6',
     scripts=['multitracker/auto_annotate_pro.py'],
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/saurabheights/multitrackpro',
-    version='0.1.1',
+    version='0.1.2  ',
     zip_safe=False,
 )
```

