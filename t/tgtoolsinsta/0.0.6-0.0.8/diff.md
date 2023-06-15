# Comparing `tmp/tgtoolsinsta-0.0.6.tar.gz` & `tmp/tgtoolsinsta-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgtoolsinsta-0.0.6.tar", last modified: Wed Jun 14 04:53:59 2023, max compression
+gzip compressed data, was "tgtoolsinsta-0.0.8.tar", last modified: Thu Jun 15 02:05:31 2023, max compression
```

## Comparing `tgtoolsinsta-0.0.6.tar` & `tgtoolsinsta-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-14 04:53:59.110843 tgtoolsinsta-0.0.6/
--rw-rw----   0 root         (0) everybody  (9997)     1063 2023-06-14 04:53:42.000000 tgtoolsinsta-0.0.6/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)      564 2023-06-14 04:53:59.098843 tgtoolsinsta-0.0.6/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-14 04:53:59.110843 tgtoolsinsta-0.0.6/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      853 2023-06-14 04:52:14.000000 tgtoolsinsta-0.0.6/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-14 04:53:58.990843 tgtoolsinsta-0.0.6/tgtoolsinsta/
--rw-rw----   0 root         (0) everybody  (9997)      342 2023-06-14 03:27:55.000000 tgtoolsinsta-0.0.6/tgtoolsinsta/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-14 04:53:59.086843 tgtoolsinsta-0.0.6/tgtoolsinsta.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      564 2023-06-14 04:53:58.000000 tgtoolsinsta-0.0.6/tgtoolsinsta.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      220 2023-06-14 04:53:58.000000 tgtoolsinsta-0.0.6/tgtoolsinsta.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-14 04:53:58.000000 tgtoolsinsta-0.0.6/tgtoolsinsta.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        9 2023-06-14 04:53:58.000000 tgtoolsinsta-0.0.6/tgtoolsinsta.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)       13 2023-06-14 04:53:58.000000 tgtoolsinsta-0.0.6/tgtoolsinsta.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-15 02:05:31.348620 tgtoolsinsta-0.0.8/
+-rw-rw----   0 root         (0) everybody  (9997)     1063 2023-06-14 04:53:42.000000 tgtoolsinsta-0.0.8/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)      588 2023-06-15 02:05:31.332620 tgtoolsinsta-0.0.8/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-15 02:05:31.352620 tgtoolsinsta-0.0.8/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      877 2023-06-15 02:03:34.000000 tgtoolsinsta-0.0.8/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-15 02:05:31.224620 tgtoolsinsta-0.0.8/tgtoolsinsta/
+-rw-rw----   0 root         (0) everybody  (9997)      610 2023-06-15 02:02:40.000000 tgtoolsinsta-0.0.8/tgtoolsinsta/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-15 02:05:31.320620 tgtoolsinsta-0.0.8/tgtoolsinsta.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      588 2023-06-15 02:05:30.000000 tgtoolsinsta-0.0.8/tgtoolsinsta.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      220 2023-06-15 02:05:30.000000 tgtoolsinsta-0.0.8/tgtoolsinsta.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-15 02:05:30.000000 tgtoolsinsta-0.0.8/tgtoolsinsta.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        9 2023-06-15 02:05:30.000000 tgtoolsinsta-0.0.8/tgtoolsinsta.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)       13 2023-06-15 02:05:30.000000 tgtoolsinsta-0.0.8/tgtoolsinsta.egg-info/top_level.txt
```

### Comparing `tgtoolsinsta-0.0.6/LICENSE` & `tgtoolsinsta-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tgtoolsinsta-0.0.6/PKG-INFO` & `tgtoolsinsta-0.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: tgtoolsinsta
-Version: 0.0.6
-Summary: INSTAGRAM ID SCRAPER 
+Version: 0.0.8
+Summary: INSTAGRAM ID AND POST-ID SCRAPER 
 Author: T G
 Author-email: mail2tgtools@gmail.com
 Keywords: Instagram,userid
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-A PYTHON LIBRARY THAT HELPS YOU TO SCRAPE INSTAGRAM USER-ID
+A PYTHON LIBRARY THAT HELPS YOU TO SCRAPE INSTAGRAM USER-ID AND POST-ID
```

### Comparing `tgtoolsinsta-0.0.6/setup.py` & `tgtoolsinsta-0.0.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.6'
-DESCRIPTION = 'INSTAGRAM ID SCRAPER '
-LONG_DESCRIPTION = 'A PYTHON LIBRARY THAT HELPS YOU TO SCRAPE INSTAGRAM USER-ID'
+VERSION = '0.0.8'
+DESCRIPTION = 'INSTAGRAM ID AND POST-ID SCRAPER '
+LONG_DESCRIPTION = 'A PYTHON LIBRARY THAT HELPS YOU TO SCRAPE INSTAGRAM USER-ID AND POST-ID'
 
 # Setting up
 setup(
     name="tgtoolsinsta",
     version=VERSION,
     author="T G",
     author_email="mail2tgtools@gmail.com",
```

### Comparing `tgtoolsinsta-0.0.6/tgtoolsinsta.egg-info/PKG-INFO` & `tgtoolsinsta-0.0.8/tgtoolsinsta.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: tgtoolsinsta
-Version: 0.0.6
-Summary: INSTAGRAM ID SCRAPER 
+Version: 0.0.8
+Summary: INSTAGRAM ID AND POST-ID SCRAPER 
 Author: T G
 Author-email: mail2tgtools@gmail.com
 Keywords: Instagram,userid
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-A PYTHON LIBRARY THAT HELPS YOU TO SCRAPE INSTAGRAM USER-ID
+A PYTHON LIBRARY THAT HELPS YOU TO SCRAPE INSTAGRAM USER-ID AND POST-ID
```

