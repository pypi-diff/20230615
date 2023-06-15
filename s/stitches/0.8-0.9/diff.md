# Comparing `tmp/stitches-0.8.tar.gz` & `tmp/stitches-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stitches-0.8.tar", last modified: Fri Sep 12 12:24:54 2014, max compression
+gzip compressed data, was "dist/stitches-0.9.tar", last modified: Mon Mar 16 11:35:27 2015, max compression
```

## Comparing `stitches-0.8.tar` & `stitches-0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2014-09-12 12:24:54.000000 stitches-0.8/
--rw-rw-r--   0 mkovacik  (1000) mkovacik  (1000)      793 2014-09-12 12:24:20.000000 stitches-0.8/setup.py
--rw-r--r--   0 root         (0) root         (0)      579 2014-09-12 12:24:54.000000 stitches-0.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2014-09-12 12:24:54.000000 stitches-0.8/stitches/
--rw-rw-r--   0 mkovacik  (1000) mkovacik  (1000)     3076 2014-05-22 12:30:01.000000 stitches-0.8/stitches/structure.py
--rw-rw-r--   0 mkovacik  (1000) mkovacik  (1000)    10672 2014-09-12 12:16:33.000000 stitches-0.8/stitches/connection.py
--rw-rw-r--   0 mkovacik  (1000) mkovacik  (1000)      285 2014-05-22 12:30:01.000000 stitches-0.8/stitches/__init__.py
--rw-rw-r--   0 mkovacik  (1000) mkovacik  (1000)     6190 2014-05-22 12:30:01.000000 stitches-0.8/stitches/expect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2014-09-12 12:24:54.000000 stitches-0.8/stitches.egg-info/
--rw-r--r--   0 root         (0) root         (0)        9 2014-09-12 12:24:54.000000 stitches-0.8/stitches.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      579 2014-09-12 12:24:54.000000 stitches-0.8/stitches.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       34 2014-09-12 12:24:54.000000 stitches-0.8/stitches.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      252 2014-09-12 12:24:54.000000 stitches-0.8/stitches.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2014-09-12 12:24:54.000000 stitches-0.8/stitches.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2014-09-12 12:24:54.000000 stitches-0.8/setup.cfg
+drwxrwxr-x   0 mkovacik   (501) mkovacik    (20)        0 2015-03-16 11:35:42.000000 stitches-0.9/
+-rw-rw-r--   0 mkovacik   (501) mkovacik    (20)      579 2015-03-16 11:35:42.000000 stitches-0.9/PKG-INFO
+-rw-rw-r--   0 mkovacik   (501) mkovacik    (20)       59 2015-03-16 11:35:42.000000 stitches-0.9/setup.cfg
+-rw-rw-r--   0 mkovacik   (501) mkovacik    (20)      801 2015-03-16 11:32:58.000000 stitches-0.9/setup.py
+drwxrwxr-x   0 mkovacik   (501) mkovacik    (20)        0 2015-03-16 11:35:08.000000 stitches-0.9/stitches/
+-rw-rw-r--   0 mkovacik   (501) mkovacik    (20)      285 2014-05-22 12:30:01.000000 stitches-0.9/stitches/__init__.py
+-rw-rw-r--   0 mkovacik   (501) mkovacik    (20)    10672 2014-09-12 12:16:33.000000 stitches-0.9/stitches/connection.py
+-rw-rw-r--   0 mkovacik   (501) mkovacik    (20)     6190 2014-05-22 12:30:01.000000 stitches-0.9/stitches/expect.py
+-rw-rw-r--   0 mkovacik   (501) mkovacik    (20)     3076 2014-05-22 12:30:01.000000 stitches-0.9/stitches/structure.py
+drwxrwxr-x   0 mkovacik   (501) mkovacik    (20)        0 2015-03-16 11:35:08.000000 stitches-0.9/stitches.egg-info/
+-rw-r--r--   0 mkovacik   (501) mkovacik    (20)        1 2015-03-16 11:35:42.000000 stitches-0.9/stitches.egg-info/dependency_links.txt
+-rw-r--r--   0 mkovacik   (501) mkovacik    (20)      579 2015-03-16 11:35:42.000000 stitches-0.9/stitches.egg-info/PKG-INFO
+-rw-r--r--   0 mkovacik   (501) mkovacik    (20)       41 2015-03-16 11:35:42.000000 stitches-0.9/stitches.egg-info/requires.txt
+-rw-r--r--   0 mkovacik   (501) mkovacik    (20)      252 2015-03-16 11:35:42.000000 stitches-0.9/stitches.egg-info/SOURCES.txt
+-rw-r--r--   0 mkovacik   (501) mkovacik    (20)        9 2015-03-16 11:35:42.000000 stitches-0.9/stitches.egg-info/top_level.txt
```

### Comparing `stitches-0.8/setup.py` & `stitches-0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 
 """ setup.py """
 
 from setuptools import setup
 
 setup(name='stitches',
-    version='0.8',
+    version='0.9',
     description='Multihost actions toolbox',
     author='Vitaly Kuznetsov',
     author_email='vitty@redhat.com',
     url='https://github.com/RedHatQE/python-stitches',
     license="GPLv3+",
-    install_requires=['paramiko', 'nose', 'PyYAML', 'plumbum', 'rpyc'],
+    install_requires=['paramiko >= 1.10', 'nose', 'PyYAML', 'plumbum', 'rpyc'],
     packages=[
         'stitches'
         ],
     classifiers=[
             'License :: OSI Approved :: GNU General Public\
  License v3 or later (GPLv3+)',
             'Programming Language :: Python',
```

### Comparing `stitches-0.8/PKG-INFO` & `stitches-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: stitches
-Version: 0.8
+Version: 0.9
 Summary: Multihost actions toolbox
 Home-page: https://github.com/RedHatQE/python-stitches
 Author: Vitaly Kuznetsov
 Author-email: vitty@redhat.com
 License: GPLv3+
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `stitches-0.8/stitches/structure.py` & `stitches-0.9/stitches/structure.py`

 * *Files identical despite different names*

### Comparing `stitches-0.8/stitches/connection.py` & `stitches-0.9/stitches/connection.py`

 * *Files identical despite different names*

### Comparing `stitches-0.8/stitches/expect.py` & `stitches-0.9/stitches/expect.py`

 * *Files identical despite different names*

### Comparing `stitches-0.8/stitches.egg-info/PKG-INFO` & `stitches-0.9/stitches.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: stitches
-Version: 0.8
+Version: 0.9
 Summary: Multihost actions toolbox
 Home-page: https://github.com/RedHatQE/python-stitches
 Author: Vitaly Kuznetsov
 Author-email: vitty@redhat.com
 License: GPLv3+
 Description: UNKNOWN
 Platform: UNKNOWN
```

