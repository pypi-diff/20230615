# Comparing `tmp/current_events_magnifier-0.0.3.2.tar.gz` & `tmp/current_events_magnifier-0.0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/current_events_magnifier-0.0.3.2.tar", last modified: Thu Jun 15 10:20:39 2023, max compression
+gzip compressed data, was "dist/current_events_magnifier-0.0.3.3.tar", last modified: Thu Jun 15 10:24:03 2023, max compression
```

## Comparing `current_events_magnifier-0.0.3.2.tar` & `current_events_magnifier-0.0.3.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-15 10:20:39.657085 current_events_magnifier-0.0.3.2/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.0.3.2/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6020 2023-06-15 10:20:39.657085 current_events_magnifier-0.0.3.2/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5408 2023-06-14 11:16:12.000000 current_events_magnifier-0.0.3.2/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-15 10:20:39.657085 current_events_magnifier-0.0.3.2/current_events_magnifier/
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     6268 2023-06-15 02:13:38.000000 current_events_magnifier-0.0.3.2/current_events_magnifier/CE_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 12:01:39.000000 current_events_magnifier-0.0.3.2/current_events_magnifier/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 current_events_magnifier-0.0.3.2/current_events_magnifier/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.0.3.2/current_events_magnifier/cem_utils.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.0.3.2/current_events_magnifier/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7556 2023-06-14 11:49:38.000000 current_events_magnifier-0.0.3.2/current_events_magnifier/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9027 2023-06-14 10:46:36.000000 current_events_magnifier-0.0.3.2/current_events_magnifier/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13168 2023-06-14 12:00:50.000000 current_events_magnifier-0.0.3.2/current_events_magnifier/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-15 10:20:39.657085 current_events_magnifier-0.0.3.2/current_events_magnifier.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6020 2023-06-15 10:20:39.000000 current_events_magnifier-0.0.3.2/current_events_magnifier.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      600 2023-06-15 10:20:39.000000 current_events_magnifier-0.0.3.2/current_events_magnifier.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-15 10:20:39.000000 current_events_magnifier-0.0.3.2/current_events_magnifier.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       91 2023-06-15 10:20:39.000000 current_events_magnifier-0.0.3.2/current_events_magnifier.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-15 10:20:39.000000 current_events_magnifier-0.0.3.2/current_events_magnifier.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-15 10:20:39.657085 current_events_magnifier-0.0.3.2/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-06-15 10:20:36.000000 current_events_magnifier-0.0.3.2/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-15 10:24:03.128273 current_events_magnifier-0.0.3.3/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.0.3.3/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6020 2023-06-15 10:24:03.128273 current_events_magnifier-0.0.3.3/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5408 2023-06-14 11:16:12.000000 current_events_magnifier-0.0.3.3/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-15 10:24:03.128273 current_events_magnifier-0.0.3.3/current_events_magnifier/
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     6268 2023-06-15 02:13:38.000000 current_events_magnifier-0.0.3.3/current_events_magnifier/CE_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 12:01:39.000000 current_events_magnifier-0.0.3.3/current_events_magnifier/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 current_events_magnifier-0.0.3.3/current_events_magnifier/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.0.3.3/current_events_magnifier/cem_utils.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.0.3.3/current_events_magnifier/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7556 2023-06-14 11:49:38.000000 current_events_magnifier-0.0.3.3/current_events_magnifier/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9027 2023-06-14 10:46:36.000000 current_events_magnifier-0.0.3.3/current_events_magnifier/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13168 2023-06-14 12:00:50.000000 current_events_magnifier-0.0.3.3/current_events_magnifier/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-15 10:24:03.128273 current_events_magnifier-0.0.3.3/current_events_magnifier.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6020 2023-06-15 10:24:03.000000 current_events_magnifier-0.0.3.3/current_events_magnifier.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      600 2023-06-15 10:24:03.000000 current_events_magnifier-0.0.3.3/current_events_magnifier.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-15 10:24:03.000000 current_events_magnifier-0.0.3.3/current_events_magnifier.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       83 2023-06-15 10:24:03.000000 current_events_magnifier-0.0.3.3/current_events_magnifier.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-15 10:24:03.000000 current_events_magnifier-0.0.3.3/current_events_magnifier.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-15 10:24:03.128273 current_events_magnifier-0.0.3.3/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1069 2023-06-15 10:24:00.000000 current_events_magnifier-0.0.3.3/setup.py
```

### Comparing `current_events_magnifier-0.0.3.2/LICENSE` & `current_events_magnifier-0.0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.2/PKG-INFO` & `current_events_magnifier-0.0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: current_events_magnifier
-Version: 0.0.3.2
+Version: 0.0.3.3
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `current_events_magnifier-0.0.3.2/README.md` & `current_events_magnifier-0.0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.2/current_events_magnifier/CE_magnifier.py` & `current_events_magnifier-0.0.3.3/current_events_magnifier/CE_magnifier.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.2/current_events_magnifier/cem_utils.py` & `current_events_magnifier-0.0.3.3/current_events_magnifier/cem_utils.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.2/current_events_magnifier/normalization.py` & `current_events_magnifier-0.0.3.3/current_events_magnifier/normalization.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.2/current_events_magnifier/plot.py` & `current_events_magnifier-0.0.3.3/current_events_magnifier/plot.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.2/current_events_magnifier/read_f5c_resquiggle.py` & `current_events_magnifier-0.0.3.3/current_events_magnifier/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.2/current_events_magnifier/read_tombo_resquiggle.py` & `current_events_magnifier-0.0.3.3/current_events_magnifier/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.2/current_events_magnifier.egg-info/PKG-INFO` & `current_events_magnifier-0.0.3.3/current_events_magnifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: current-events-magnifier
-Version: 0.0.3.2
+Version: 0.0.3.3
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `current_events_magnifier-0.0.3.2/current_events_magnifier.egg-info/SOURCES.txt` & `current_events_magnifier-0.0.3.3/current_events_magnifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.2/setup.py` & `current_events_magnifier-0.0.3.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="current_events_magnifier",
-    version="0.0.3.2",
+    version="0.0.3.3",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle pipeline(Tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/current_events_magnifier",
@@ -23,11 +23,10 @@
     install_requires=[
         'h5py==3.8.0',
         'numpy>=1.23.0',
         'pandas>=1.1.5',
         'plotnine>=0.8.0',
         'tqdm>=4.62.0',
         "pysam>=0.21.0",
-        'pyslow5'
     ],
     scripts=['current_events_magnifier/CE_magnifier.py']
 )
```

