# Comparing `tmp/hearthstone_data-93849.1.tar.gz` & `tmp/hearthstone_data-95431.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hearthstone_data-93849.1.tar", last modified: Tue Sep 21 19:01:04 2021, max compression
+gzip compressed data, was "hearthstone_data-95431.1.tar", last modified: Tue Oct 12 19:31:57 2021, max compression
```

## Comparing `hearthstone_data-93849.1.tar` & `hearthstone_data-95431.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 benedict  (1000) benedict  (1000)        0 2021-09-21 19:01:04.056617 hearthstone_data-93849.1/
--rw-r--r--   0 benedict  (1000) benedict  (1000)      743 2021-09-21 19:01:04.056617 hearthstone_data-93849.1/PKG-INFO
-drwxr-xr-x   0 benedict  (1000) benedict  (1000)        0 2021-09-21 19:01:04.056617 hearthstone_data-93849.1/hearthstone_data/
--rw-r--r--   0 benedict  (1000) benedict  (1000)      382 2021-09-21 18:54:14.000000 hearthstone_data-93849.1/hearthstone_data/__init__.py
-drwxr-xr-x   0 benedict  (1000) benedict  (1000)        0 2021-09-21 19:01:04.056617 hearthstone_data-93849.1/hearthstone_data.egg-info/
--rw-r--r--   0 benedict  (1000) benedict  (1000)      743 2021-09-21 19:01:04.000000 hearthstone_data-93849.1/hearthstone_data.egg-info/PKG-INFO
--rw-r--r--   0 benedict  (1000) benedict  (1000)      242 2021-09-21 19:01:04.000000 hearthstone_data-93849.1/hearthstone_data.egg-info/SOURCES.txt
--rw-r--r--   0 benedict  (1000) benedict  (1000)        1 2021-09-21 19:01:04.000000 hearthstone_data-93849.1/hearthstone_data.egg-info/dependency_links.txt
--rw-r--r--   0 benedict  (1000) benedict  (1000)       17 2021-09-21 19:01:04.000000 hearthstone_data-93849.1/hearthstone_data.egg-info/top_level.txt
--rw-r--r--   0 benedict  (1000) benedict  (1000)        1 2021-09-21 18:55:21.000000 hearthstone_data-93849.1/hearthstone_data.egg-info/zip-safe
--rw-r--r--   0 benedict  (1000) benedict  (1000)      752 2021-09-21 19:01:04.059950 hearthstone_data-93849.1/setup.cfg
--rwxr-xr-x   0 benedict  (1000) benedict  (1000)      650 2021-09-21 18:54:14.000000 hearthstone_data-93849.1/setup.py
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2021-10-12 19:31:57.628826 hearthstone_data-95431.1/
+-rw-rw-r--   0 julian    (1000) julian    (1000)      754 2021-10-12 19:31:57.628826 hearthstone_data-95431.1/PKG-INFO
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2021-10-12 19:31:57.628826 hearthstone_data-95431.1/hearthstone_data/
+-rw-rw-r--   0 julian    (1000) julian    (1000)      382 2021-10-12 19:30:44.000000 hearthstone_data-95431.1/hearthstone_data/__init__.py
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2021-10-12 19:31:57.628826 hearthstone_data-95431.1/hearthstone_data.egg-info/
+-rw-rw-r--   0 julian    (1000) julian    (1000)      754 2021-10-12 19:31:57.000000 hearthstone_data-95431.1/hearthstone_data.egg-info/PKG-INFO
+-rw-rw-r--   0 julian    (1000) julian    (1000)      242 2021-10-12 19:31:57.000000 hearthstone_data-95431.1/hearthstone_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)        1 2021-10-12 19:31:57.000000 hearthstone_data-95431.1/hearthstone_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)       17 2021-10-12 19:31:57.000000 hearthstone_data-95431.1/hearthstone_data.egg-info/top_level.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)        1 2021-10-12 19:31:57.000000 hearthstone_data-95431.1/hearthstone_data.egg-info/zip-safe
+-rw-rw-r--   0 julian    (1000) julian    (1000)      752 2021-10-12 19:31:57.628826 hearthstone_data-95431.1/setup.cfg
+-rwxrwxr-x   0 julian    (1000) julian    (1000)      650 2021-10-12 19:30:44.000000 hearthstone_data-95431.1/setup.py
```

### Comparing `hearthstone_data-93849.1/PKG-INFO` & `hearthstone_data-95431.1/hearthstone_data.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-Metadata-Version: 2.1
-Name: hearthstone_data
-Version: 93849.1
+Metadata-Version: 1.1
+Name: hearthstone-data
+Version: 95431.1
 Summary: CardDefs.xml and Strings for Hearthstone
 Home-page: https://github.com/HearthSim/python-hearthstone-data/
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 License: UNKNOWN
 Download-URL: https://github.com/HearthSim/python-hearthstone-data/tarball/master
+Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Games/Entertainment
-
-UNKNOWN
-
```

### Comparing `hearthstone_data-93849.1/hearthstone_data.egg-info/PKG-INFO` & `hearthstone_data-95431.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-Metadata-Version: 2.1
-Name: hearthstone-data
-Version: 93849.1
+Metadata-Version: 1.1
+Name: hearthstone_data
+Version: 95431.1
 Summary: CardDefs.xml and Strings for Hearthstone
 Home-page: https://github.com/HearthSim/python-hearthstone-data/
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 License: UNKNOWN
 Download-URL: https://github.com/HearthSim/python-hearthstone-data/tarball/master
+Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Games/Entertainment
-
-UNKNOWN
-
```

### Comparing `hearthstone_data-93849.1/setup.cfg` & `hearthstone_data-95431.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `hearthstone_data-93849.1/setup.py` & `hearthstone_data-95431.1/setup.py`

 * *Files identical despite different names*

