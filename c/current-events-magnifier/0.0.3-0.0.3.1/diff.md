# Comparing `tmp/current_events_magnifier-0.0.3.tar.gz` & `tmp/current_events_magnifier-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/current_events_magnifier-0.0.3.tar", last modified: Thu Jun 15 10:10:55 2023, max compression
+gzip compressed data, was "dist/current_events_magnifier-0.0.3.1.tar", last modified: Thu Jun 15 10:17:08 2023, max compression
```

## Comparing `current_events_magnifier-0.0.3.tar` & `current_events_magnifier-0.0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-15 10:10:55.004152 current_events_magnifier-0.0.3/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.0.3/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6018 2023-06-15 10:10:55.004152 current_events_magnifier-0.0.3/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5408 2023-06-14 11:16:12.000000 current_events_magnifier-0.0.3/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-15 10:10:55.004152 current_events_magnifier-0.0.3/current_events_magnifier/
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     6268 2023-06-15 02:13:38.000000 current_events_magnifier-0.0.3/current_events_magnifier/CE_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 12:01:39.000000 current_events_magnifier-0.0.3/current_events_magnifier/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 current_events_magnifier-0.0.3/current_events_magnifier/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.0.3/current_events_magnifier/cem_utils.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.0.3/current_events_magnifier/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7556 2023-06-14 11:49:38.000000 current_events_magnifier-0.0.3/current_events_magnifier/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9027 2023-06-14 10:46:36.000000 current_events_magnifier-0.0.3/current_events_magnifier/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13168 2023-06-14 12:00:50.000000 current_events_magnifier-0.0.3/current_events_magnifier/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-15 10:10:55.004152 current_events_magnifier-0.0.3/current_events_magnifier.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6018 2023-06-15 10:10:54.000000 current_events_magnifier-0.0.3/current_events_magnifier.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      600 2023-06-15 10:10:54.000000 current_events_magnifier-0.0.3/current_events_magnifier.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-15 10:10:54.000000 current_events_magnifier-0.0.3/current_events_magnifier.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       98 2023-06-15 10:10:54.000000 current_events_magnifier-0.0.3/current_events_magnifier.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-15 10:10:54.000000 current_events_magnifier-0.0.3/current_events_magnifier.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-15 10:10:55.004152 current_events_magnifier-0.0.3/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1092 2023-06-15 10:10:38.000000 current_events_magnifier-0.0.3/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-15 10:17:08.511970 current_events_magnifier-0.0.3.1/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.0.3.1/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6020 2023-06-15 10:17:08.507970 current_events_magnifier-0.0.3.1/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5408 2023-06-14 11:16:12.000000 current_events_magnifier-0.0.3.1/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-15 10:17:08.507970 current_events_magnifier-0.0.3.1/current_events_magnifier/
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     6268 2023-06-15 02:13:38.000000 current_events_magnifier-0.0.3.1/current_events_magnifier/CE_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 12:01:39.000000 current_events_magnifier-0.0.3.1/current_events_magnifier/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 current_events_magnifier-0.0.3.1/current_events_magnifier/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.0.3.1/current_events_magnifier/cem_utils.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.0.3.1/current_events_magnifier/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7556 2023-06-14 11:49:38.000000 current_events_magnifier-0.0.3.1/current_events_magnifier/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9027 2023-06-14 10:46:36.000000 current_events_magnifier-0.0.3.1/current_events_magnifier/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13168 2023-06-14 12:00:50.000000 current_events_magnifier-0.0.3.1/current_events_magnifier/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-15 10:17:08.507970 current_events_magnifier-0.0.3.1/current_events_magnifier.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6020 2023-06-15 10:17:08.000000 current_events_magnifier-0.0.3.1/current_events_magnifier.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      600 2023-06-15 10:17:08.000000 current_events_magnifier-0.0.3.1/current_events_magnifier.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-15 10:17:08.000000 current_events_magnifier-0.0.3.1/current_events_magnifier.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       83 2023-06-15 10:17:08.000000 current_events_magnifier-0.0.3.1/current_events_magnifier.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-15 10:17:08.000000 current_events_magnifier-0.0.3.1/current_events_magnifier.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-15 10:17:08.511970 current_events_magnifier-0.0.3.1/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1068 2023-06-15 10:16:49.000000 current_events_magnifier-0.0.3.1/setup.py
```

### Comparing `current_events_magnifier-0.0.3/LICENSE` & `current_events_magnifier-0.0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3/PKG-INFO` & `current_events_magnifier-0.0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: current_events_magnifier
-Version: 0.0.3
+Version: 0.0.3.1
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `current_events_magnifier-0.0.3/README.md` & `current_events_magnifier-0.0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3/current_events_magnifier/CE_magnifier.py` & `current_events_magnifier-0.0.3.1/current_events_magnifier/CE_magnifier.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3/current_events_magnifier/cem_utils.py` & `current_events_magnifier-0.0.3.1/current_events_magnifier/cem_utils.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3/current_events_magnifier/normalization.py` & `current_events_magnifier-0.0.3.1/current_events_magnifier/normalization.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3/current_events_magnifier/plot.py` & `current_events_magnifier-0.0.3.1/current_events_magnifier/plot.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3/current_events_magnifier/read_f5c_resquiggle.py` & `current_events_magnifier-0.0.3.1/current_events_magnifier/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3/current_events_magnifier/read_tombo_resquiggle.py` & `current_events_magnifier-0.0.3.1/current_events_magnifier/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3/current_events_magnifier.egg-info/PKG-INFO` & `current_events_magnifier-0.0.3.1/current_events_magnifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: current-events-magnifier
-Version: 0.0.3
+Version: 0.0.3.1
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `current_events_magnifier-0.0.3/current_events_magnifier.egg-info/SOURCES.txt` & `current_events_magnifier-0.0.3.1/current_events_magnifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3/setup.py` & `current_events_magnifier-0.0.3.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="current_events_magnifier",
-    version="0.0.3",
+    version="0.0.3.1",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle pipeline(Tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/current_events_magnifier",
@@ -22,12 +22,11 @@
     python_requires='>=3.7',
     install_requires=[
         'h5py==3.8.0',
         'numpy>=1.21.6',
         'pandas>=1.1.5',
         'plotnine>=0.8.0',
         'tqdm>=4.62.0',
-        "pyslow5==1.0.0",
         "pysam>=0.21.0"
     ],
     scripts=['current_events_magnifier/CE_magnifier.py']
 )
```

