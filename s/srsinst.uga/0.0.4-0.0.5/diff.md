# Comparing `tmp/srsinst.uga-0.0.4.tar.gz` & `tmp/srsinst.uga-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\instrument_library\uga100\dist\.tmp-v6ddqcfs\srsinst.uga-0.0.4.tar", last modified: Thu Jun 15 19:03:45 2023, max compression
+gzip compressed data, was "C:\PyPI\instrument_library\uga100\dist\.tmp-h3cmqrk7\srsinst.uga-0.0.5.tar", last modified: Thu Jun 15 19:20:47 2023, max compression
```

## Comparing `srsinst.uga-0.0.4.tar` & `srsinst.uga-0.0.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 19:03:45.048808 srsinst.uga-0.0.4/
--rw-rw-rw-   0        0        0     1103 2023-05-19 19:35:50.000000 srsinst.uga-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     7126 2023-06-15 19:03:45.038808 srsinst.uga-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     6345 2023-06-15 19:01:04.000000 srsinst.uga-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 19:03:45.028808 srsinst.uga-0.0.4/docs/
--rw-rw-rw-   0        0        0      654 2023-05-19 21:28:14.000000 srsinst.uga-0.0.4/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-06-15 19:03:45.006676 srsinst.uga-0.0.4/docs/_static/
-drwxrwxrwx   0        0        0        0 2023-06-15 19:03:45.028808 srsinst.uga-0.0.4/docs/_static/image/
--rw-rw-rw-   0        0        0   174299 2023-05-16 16:03:57.000000 srsinst.uga-0.0.4/docs/_static/image/UGA100_composition_analysis_screenshot.png
--rwxrwxrwx   0        0        0       28 2023-05-19 21:28:14.000000 srsinst.uga-0.0.4/docs/autodoc.bat
--rw-rw-rw-   0        0        0     5458 2023-05-19 21:28:14.000000 srsinst.uga-0.0.4/docs/basic_operation.rst
--rw-rw-rw-   0        0        0       26 2023-05-19 21:28:14.000000 srsinst.uga-0.0.4/docs/changelog.rst
--rw-rw-rw-   0        0        0     1985 2023-06-13 17:27:43.000000 srsinst.uga-0.0.4/docs/conf.py
--rw-rw-rw-   0        0        0     1168 2023-05-19 21:28:14.000000 srsinst.uga-0.0.4/docs/connection.rst
--rw-rw-rw-   0        0        0     1541 2023-06-13 17:07:45.000000 srsinst.uga-0.0.4/docs/index.rst
--rw-rw-rw-   0        0        0     1246 2023-05-19 21:28:14.000000 srsinst.uga-0.0.4/docs/installation.rst
--rwxrwxrwx   0        0        0      802 2023-05-19 21:28:14.000000 srsinst.uga-0.0.4/docs/make.bat
--rw-rw-rw-   0        0        0       32 2023-05-19 21:28:14.000000 srsinst.uga-0.0.4/docs/requirements.txt
--rw-rw-rw-   0        0        0     1010 2023-05-19 21:28:14.000000 srsinst.uga-0.0.4/docs/scan_operation.rst
--rw-rw-rw-   0        0        0      329 2023-06-13 17:18:39.000000 srsinst.uga-0.0.4/docs/srsinst.uga.instruments.rst
--rw-rw-rw-   0        0        0      478 2023-06-13 17:16:42.000000 srsinst.uga-0.0.4/docs/srsinst.uga.instruments.uga100.rst
--rw-rw-rw-   0        0        0      134 2023-05-19 21:28:14.000000 srsinst.uga-0.0.4/docs/srsinst.uga.rst
--rw-rw-rw-   0        0        0      530 2023-06-13 17:33:33.000000 srsinst.uga-0.0.4/docs/srsinst.uga.tasks.rst
--rw-rw-rw-   0        0        0     1473 2023-05-19 21:28:14.000000 srsinst.uga-0.0.4/docs/troubleshooting.rst
--rw-rw-rw-   0        0        0     1231 2023-06-15 17:27:23.000000 srsinst.uga-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-15 19:03:45.048808 srsinst.uga-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsinst.uga-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:03:45.006676 srsinst.uga-0.0.4/srsinst/
-drwxrwxrwx   0        0        0        0 2023-06-15 19:03:45.038808 srsinst.uga-0.0.4/srsinst/uga/
--rw-rw-rw-   0        0        0      229 2023-06-15 19:02:35.000000 srsinst.uga-0.0.4/srsinst/uga/__init__.py
--rw-rw-rw-   0        0        0      483 2023-05-19 21:22:28.000000 srsinst.uga-0.0.4/srsinst/uga/__main__.py
--rw-rw-rw-   0        0        0    10600 2023-05-19 21:22:27.000000 srsinst.uga-0.0.4/srsinst/uga/gaslib.dat
-drwxrwxrwx   0        0        0        0 2023-06-15 19:03:45.038808 srsinst.uga-0.0.4/srsinst/uga/instruments/
--rw-rw-rw-   0        0        0       47 2023-05-19 21:22:28.000000 srsinst.uga-0.0.4/srsinst/uga/instruments/__init__.py
--rw-rw-rw-   0        0        0     1327 2023-05-19 21:32:52.000000 srsinst.uga-0.0.4/srsinst/uga/instruments/get_instruments.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:03:45.038808 srsinst.uga-0.0.4/srsinst/uga/instruments/uga100/
--rw-rw-rw-   0        0        0        0 2023-05-19 21:22:28.000000 srsinst.uga-0.0.4/srsinst/uga/instruments/uga100/__init__.py
--rw-rw-rw-   0        0        0    10643 2023-05-31 00:34:22.000000 srsinst.uga-0.0.4/srsinst/uga/instruments/uga100/components.py
--rw-rw-rw-   0        0        0     4643 2023-05-24 17:51:21.000000 srsinst.uga-0.0.4/srsinst/uga/instruments/uga100/keys.py
--rw-rw-rw-   0        0        0     5544 2023-06-15 17:42:38.000000 srsinst.uga-0.0.4/srsinst/uga/instruments/uga100/uga.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:03:45.038808 srsinst.uga-0.0.4/srsinst/uga/tasks/
--rw-rw-rw-   0        0        0        0 2023-05-19 21:22:28.000000 srsinst.uga-0.0.4/srsinst/uga/tasks/__init__.py
--rw-rw-rw-   0        0        0     4415 2023-05-24 17:26:46.000000 srsinst.uga-0.0.4/srsinst/uga/tasks/ugamodecontroltask.py
--rw-rw-rw-   0        0        0     3881 2023-05-19 21:34:42.000000 srsinst.uga-0.0.4/srsinst/uga/tasks/ugamultiplottask.py
--rw-rw-rw-   0        0        0     1949 2023-05-24 18:32:16.000000 srsinst.uga-0.0.4/srsinst/uga/tasks/ugastatemonitortask.py
--rw-rw-rw-   0        0        0     2339 2023-05-24 16:25:05.000000 srsinst.uga-0.0.4/srsinst/uga/uga.taskconfig
-drwxrwxrwx   0        0        0        0 2023-06-15 19:03:45.028808 srsinst.uga-0.0.4/srsinst.uga.egg-info/
--rw-rw-rw-   0        0        0     7126 2023-06-15 19:03:44.000000 srsinst.uga-0.0.4/srsinst.uga.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1157 2023-06-15 19:03:45.000000 srsinst.uga-0.0.4/srsinst.uga.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 19:03:44.000000 srsinst.uga-0.0.4/srsinst.uga.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-15 19:03:44.000000 srsinst.uga-0.0.4/srsinst.uga.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       79 2023-06-15 19:03:44.000000 srsinst.uga-0.0.4/srsinst.uga.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-15 19:03:44.000000 srsinst.uga-0.0.4/srsinst.uga.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 19:20:47.427008 srsinst.uga-0.0.5/
+-rw-rw-rw-   0        0        0     1103 2023-05-19 19:35:50.000000 srsinst.uga-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     7323 2023-06-15 19:20:47.427008 srsinst.uga-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6408 2023-06-15 19:19:47.000000 srsinst.uga-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 19:20:47.410714 srsinst.uga-0.0.5/docs/
+-rw-rw-rw-   0        0        0      654 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-06-15 19:20:47.393316 srsinst.uga-0.0.5/docs/_static/
+drwxrwxrwx   0        0        0        0 2023-06-15 19:20:47.410714 srsinst.uga-0.0.5/docs/_static/image/
+-rw-rw-rw-   0        0        0   174299 2023-05-16 16:03:57.000000 srsinst.uga-0.0.5/docs/_static/image/UGA100_composition_analysis_screenshot.png
+-rwxrwxrwx   0        0        0       28 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/autodoc.bat
+-rw-rw-rw-   0        0        0     5458 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/basic_operation.rst
+-rw-rw-rw-   0        0        0       26 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/changelog.rst
+-rw-rw-rw-   0        0        0     1985 2023-06-13 17:27:43.000000 srsinst.uga-0.0.5/docs/conf.py
+-rw-rw-rw-   0        0        0     1168 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/connection.rst
+-rw-rw-rw-   0        0        0     1541 2023-06-13 17:07:45.000000 srsinst.uga-0.0.5/docs/index.rst
+-rw-rw-rw-   0        0        0     1246 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/installation.rst
+-rwxrwxrwx   0        0        0      802 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/make.bat
+-rw-rw-rw-   0        0        0       32 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/requirements.txt
+-rw-rw-rw-   0        0        0     1010 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/scan_operation.rst
+-rw-rw-rw-   0        0        0      329 2023-06-13 17:18:39.000000 srsinst.uga-0.0.5/docs/srsinst.uga.instruments.rst
+-rw-rw-rw-   0        0        0      478 2023-06-13 17:16:42.000000 srsinst.uga-0.0.5/docs/srsinst.uga.instruments.uga100.rst
+-rw-rw-rw-   0        0        0      134 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/srsinst.uga.rst
+-rw-rw-rw-   0        0        0      530 2023-06-13 17:33:33.000000 srsinst.uga-0.0.5/docs/srsinst.uga.tasks.rst
+-rw-rw-rw-   0        0        0     1473 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/troubleshooting.rst
+-rw-rw-rw-   0        0        0     1363 2023-06-15 19:14:32.000000 srsinst.uga-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-15 19:20:47.427008 srsinst.uga-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsinst.uga-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:20:47.393316 srsinst.uga-0.0.5/srsinst/
+drwxrwxrwx   0        0        0        0 2023-06-15 19:20:47.417005 srsinst.uga-0.0.5/srsinst/uga/
+-rw-rw-rw-   0        0        0      229 2023-06-15 19:17:17.000000 srsinst.uga-0.0.5/srsinst/uga/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-05-19 21:22:28.000000 srsinst.uga-0.0.5/srsinst/uga/__main__.py
+-rw-rw-rw-   0        0        0    10600 2023-05-19 21:22:27.000000 srsinst.uga-0.0.5/srsinst/uga/gaslib.dat
+drwxrwxrwx   0        0        0        0 2023-06-15 19:20:47.417005 srsinst.uga-0.0.5/srsinst/uga/instruments/
+-rw-rw-rw-   0        0        0       47 2023-05-19 21:22:28.000000 srsinst.uga-0.0.5/srsinst/uga/instruments/__init__.py
+-rw-rw-rw-   0        0        0     1327 2023-05-19 21:32:52.000000 srsinst.uga-0.0.5/srsinst/uga/instruments/get_instruments.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:20:47.417005 srsinst.uga-0.0.5/srsinst/uga/instruments/uga100/
+-rw-rw-rw-   0        0        0        0 2023-05-19 21:22:28.000000 srsinst.uga-0.0.5/srsinst/uga/instruments/uga100/__init__.py
+-rw-rw-rw-   0        0        0    10643 2023-05-31 00:34:22.000000 srsinst.uga-0.0.5/srsinst/uga/instruments/uga100/components.py
+-rw-rw-rw-   0        0        0     4643 2023-05-24 17:51:21.000000 srsinst.uga-0.0.5/srsinst/uga/instruments/uga100/keys.py
+-rw-rw-rw-   0        0        0     5544 2023-06-15 17:42:38.000000 srsinst.uga-0.0.5/srsinst/uga/instruments/uga100/uga.py
+drwxrwxrwx   0        0        0        0 2023-06-15 19:20:47.427008 srsinst.uga-0.0.5/srsinst/uga/tasks/
+-rw-rw-rw-   0        0        0        0 2023-05-19 21:22:28.000000 srsinst.uga-0.0.5/srsinst/uga/tasks/__init__.py
+-rw-rw-rw-   0        0        0     4415 2023-05-24 17:26:46.000000 srsinst.uga-0.0.5/srsinst/uga/tasks/ugamodecontroltask.py
+-rw-rw-rw-   0        0        0     3881 2023-05-19 21:34:42.000000 srsinst.uga-0.0.5/srsinst/uga/tasks/ugamultiplottask.py
+-rw-rw-rw-   0        0        0     1949 2023-05-24 18:32:16.000000 srsinst.uga-0.0.5/srsinst/uga/tasks/ugastatemonitortask.py
+-rw-rw-rw-   0        0        0     2339 2023-05-24 16:25:05.000000 srsinst.uga-0.0.5/srsinst/uga/uga.taskconfig
+drwxrwxrwx   0        0        0        0 2023-06-15 19:20:47.417005 srsinst.uga-0.0.5/srsinst.uga.egg-info/
+-rw-rw-rw-   0        0        0     7323 2023-06-15 19:20:47.000000 srsinst.uga-0.0.5/srsinst.uga.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1157 2023-06-15 19:20:47.000000 srsinst.uga-0.0.5/srsinst.uga.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 19:20:47.000000 srsinst.uga-0.0.5/srsinst.uga.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-15 19:20:47.000000 srsinst.uga-0.0.5/srsinst.uga.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2023-06-15 19:20:47.000000 srsinst.uga-0.0.5/srsinst.uga.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-15 19:20:47.000000 srsinst.uga-0.0.5/srsinst.uga.egg-info/top_level.txt
```

### Comparing `srsinst.uga-0.0.4/LICENSE` & `srsinst.uga-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.4/PKG-INFO` & `srsinst.uga-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: srsinst.uga
-Version: 0.0.4
+Version: 0.0.5
 Summary: Instrument driver package for Universal Gas Analyzers (UGA) from Stanford Research Systems
 Author: Chulhoon Kim
 License: MIT license
+Project-URL: homepage, https://github.com/thinkSRS/srsinst.uga
+Project-URL: repository, https://github.com/thinkSRS/srsinst.uga.git
 Keywords: UGA,universal gas analyzer,SRS,Stanford Research Systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -181,11 +183,13 @@
      'index_dict': None}
 
 When the ion gauge is on, you can get a pressure measurement with the get_pressure() method.
 
     >>> uga.ig.get_pressure()
     1.115742e-07
 
+Commands in other components can be used in a similar way. 
+
 The most important component in a UGA is the Residual Gas Analyzer, 
 which has the separate [RGA instrument driver package](https://github.com/thinkSRS/srsinst.rga)
  for its independent usage.
 Refer to [RGA documentation](https://thinksrs.github.io/srsinst.rga/) for RGA component usage.
```

### Comparing `srsinst.uga-0.0.4/README.md` & `srsinst.uga-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -161,11 +161,13 @@
      'index_dict': None}
 
 When the ion gauge is on, you can get a pressure measurement with the get_pressure() method.
 
     >>> uga.ig.get_pressure()
     1.115742e-07
 
+Commands in other components can be used in a similar way. 
+
 The most important component in a UGA is the Residual Gas Analyzer, 
 which has the separate [RGA instrument driver package](https://github.com/thinkSRS/srsinst.rga)
  for its independent usage.
 Refer to [RGA documentation](https://thinksrs.github.io/srsinst.rga/) for RGA component usage.
```

### Comparing `srsinst.uga-0.0.4/docs/Makefile` & `srsinst.uga-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.4/docs/_static/image/UGA100_composition_analysis_screenshot.png` & `srsinst.uga-0.0.5/docs/_static/image/UGA100_composition_analysis_screenshot.png`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.4/docs/basic_operation.rst` & `srsinst.uga-0.0.5/docs/basic_operation.rst`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.4/docs/conf.py` & `srsinst.uga-0.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.4/docs/connection.rst` & `srsinst.uga-0.0.5/docs/connection.rst`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.4/docs/index.rst` & `srsinst.uga-0.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.4/docs/installation.rst` & `srsinst.uga-0.0.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.4/docs/make.bat` & `srsinst.uga-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.4/docs/scan_operation.rst` & `srsinst.uga-0.0.5/docs/scan_operation.rst`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.4/docs/srsinst.uga.tasks.rst` & `srsinst.uga-0.0.5/docs/srsinst.uga.tasks.rst`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.4/docs/troubleshooting.rst` & `srsinst.uga-0.0.5/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.4/pyproject.toml` & `srsinst.uga-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -31,9 +31,13 @@
 [tool.setuptools.dynamic]
 version = {attr = "srsinst.uga.__version__"}
 
 [project.optional-dependencies]
 full = ['matplotlib >= 3.6.2', 'pyside6']
 # For Dependency specification, Refer to PEP 631
 
+[project.urls]
+homepage = "https://github.com/thinkSRS/srsinst.uga"
+repository = "https://github.com/thinkSRS/srsinst.uga.git"
+
 [project.scripts]
 uga = "srsinst.uga.__main__:main"
```

### Comparing `srsinst.uga-0.0.4/srsinst/uga/gaslib.dat` & `srsinst.uga-0.0.5/srsinst/uga/gaslib.dat`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.4/srsinst/uga/instruments/get_instruments.py` & `srsinst.uga-0.0.5/srsinst/uga/instruments/get_instruments.py`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.4/srsinst/uga/instruments/uga100/components.py` & `srsinst.uga-0.0.5/srsinst/uga/instruments/uga100/components.py`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.4/srsinst/uga/instruments/uga100/keys.py` & `srsinst.uga-0.0.5/srsinst/uga/instruments/uga100/keys.py`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.4/srsinst/uga/instruments/uga100/uga.py` & `srsinst.uga-0.0.5/srsinst/uga/instruments/uga100/uga.py`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.4/srsinst/uga/tasks/ugamodecontroltask.py` & `srsinst.uga-0.0.5/srsinst/uga/tasks/ugamodecontroltask.py`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.4/srsinst/uga/tasks/ugamultiplottask.py` & `srsinst.uga-0.0.5/srsinst/uga/tasks/ugamultiplottask.py`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.4/srsinst/uga/tasks/ugastatemonitortask.py` & `srsinst.uga-0.0.5/srsinst/uga/tasks/ugastatemonitortask.py`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.4/srsinst/uga/uga.taskconfig` & `srsinst.uga-0.0.5/srsinst/uga/uga.taskconfig`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.4/srsinst.uga.egg-info/PKG-INFO` & `srsinst.uga-0.0.5/srsinst.uga.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: srsinst.uga
-Version: 0.0.4
+Version: 0.0.5
 Summary: Instrument driver package for Universal Gas Analyzers (UGA) from Stanford Research Systems
 Author: Chulhoon Kim
 License: MIT license
+Project-URL: homepage, https://github.com/thinkSRS/srsinst.uga
+Project-URL: repository, https://github.com/thinkSRS/srsinst.uga.git
 Keywords: UGA,universal gas analyzer,SRS,Stanford Research Systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -181,11 +183,13 @@
      'index_dict': None}
 
 When the ion gauge is on, you can get a pressure measurement with the get_pressure() method.
 
     >>> uga.ig.get_pressure()
     1.115742e-07
 
+Commands in other components can be used in a similar way. 
+
 The most important component in a UGA is the Residual Gas Analyzer, 
 which has the separate [RGA instrument driver package](https://github.com/thinkSRS/srsinst.rga)
  for its independent usage.
 Refer to [RGA documentation](https://thinksrs.github.io/srsinst.rga/) for RGA component usage.
```

### Comparing `srsinst.uga-0.0.4/srsinst.uga.egg-info/SOURCES.txt` & `srsinst.uga-0.0.5/srsinst.uga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

