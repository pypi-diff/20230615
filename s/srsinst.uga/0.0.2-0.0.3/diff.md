# Comparing `tmp/srsinst.uga-0.0.2.tar.gz` & `tmp/srsinst.uga-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\instrument drivers to GIT\uga100\dist\.tmp-6qykfqwj\srsinst.uga-0.0.2.tar", last modified: Wed May 24 20:48:23 2023, max compression
+gzip compressed data, was "C:\PyPI\instrument_library\uga100\dist\.tmp-603afvxg\srsinst.uga-0.0.3.tar", last modified: Thu Jun 15 18:54:39 2023, max compression
```

## Comparing `srsinst.uga-0.0.2.tar` & `srsinst.uga-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 20:48:23.927017 srsinst.uga-0.0.2/
--rw-rw-rw-   0        0        0     1356 2023-05-15 17:35:24.000000 srsinst.uga-0.0.2/.gitignore
--rw-rw-rw-   0        0        0     1103 2023-05-19 19:35:50.000000 srsinst.uga-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     7000 2023-05-24 20:48:23.927017 srsinst.uga-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6219 2023-05-19 20:11:28.000000 srsinst.uga-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 20:48:23.897064 srsinst.uga-0.0.2/docs/
-drwxrwxrwx   0        0        0        0 2023-05-24 20:48:23.897064 srsinst.uga-0.0.2/docs/_static/
-drwxrwxrwx   0        0        0        0 2023-05-24 20:48:23.907027 srsinst.uga-0.0.2/docs/_static/image/
--rw-rw-rw-   0        0        0   174299 2023-05-16 16:03:57.000000 srsinst.uga-0.0.2/docs/_static/image/UGA100_composition_analysis_screenshot.png
--rw-rw-rw-   0        0        0     1181 2023-05-12 21:56:47.000000 srsinst.uga-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 20:48:23.927017 srsinst.uga-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsinst.uga-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 20:48:23.897064 srsinst.uga-0.0.2/srsinst/
-drwxrwxrwx   0        0        0        0 2023-05-24 20:48:23.917023 srsinst.uga-0.0.2/srsinst/uga/
--rw-rw-rw-   0        0        0      229 2023-05-24 20:48:10.000000 srsinst.uga-0.0.2/srsinst/uga/__init__.py
--rw-rw-rw-   0        0        0      483 2023-05-19 21:22:28.000000 srsinst.uga-0.0.2/srsinst/uga/__main__.py
--rw-rw-rw-   0        0        0    10600 2023-05-19 21:22:27.000000 srsinst.uga-0.0.2/srsinst/uga/gaslib.dat
-drwxrwxrwx   0        0        0        0 2023-05-24 20:48:23.917023 srsinst.uga-0.0.2/srsinst/uga/instruments/
--rw-rw-rw-   0        0        0       47 2023-05-19 21:22:28.000000 srsinst.uga-0.0.2/srsinst/uga/instruments/__init__.py
--rw-rw-rw-   0        0        0     1327 2023-05-19 21:32:52.000000 srsinst.uga-0.0.2/srsinst/uga/instruments/get_instruments.py
-drwxrwxrwx   0        0        0        0 2023-05-24 20:48:23.917023 srsinst.uga-0.0.2/srsinst/uga/instruments/uga100/
--rw-rw-rw-   0        0        0        0 2023-05-19 21:22:28.000000 srsinst.uga-0.0.2/srsinst/uga/instruments/uga100/__init__.py
--rw-rw-rw-   0        0        0    10643 2023-05-24 18:25:35.000000 srsinst.uga-0.0.2/srsinst/uga/instruments/uga100/components.py
--rw-rw-rw-   0        0        0     4643 2023-05-24 17:51:21.000000 srsinst.uga-0.0.2/srsinst/uga/instruments/uga100/keys.py
--rw-rw-rw-   0        0        0     5544 2023-05-19 21:34:11.000000 srsinst.uga-0.0.2/srsinst/uga/instruments/uga100/uga.py
-drwxrwxrwx   0        0        0        0 2023-05-24 20:48:23.927017 srsinst.uga-0.0.2/srsinst/uga/tasks/
--rw-rw-rw-   0        0        0        0 2023-05-19 21:22:28.000000 srsinst.uga-0.0.2/srsinst/uga/tasks/__init__.py
--rw-rw-rw-   0        0        0     4415 2023-05-24 17:26:46.000000 srsinst.uga-0.0.2/srsinst/uga/tasks/ugamodecontroltask.py
--rw-rw-rw-   0        0        0     3881 2023-05-19 21:34:42.000000 srsinst.uga-0.0.2/srsinst/uga/tasks/ugamultiplottask.py
--rw-rw-rw-   0        0        0     1949 2023-05-24 18:32:16.000000 srsinst.uga-0.0.2/srsinst/uga/tasks/ugastatemonitortask.py
--rw-rw-rw-   0        0        0     2339 2023-05-24 16:25:05.000000 srsinst.uga-0.0.2/srsinst/uga/uga.taskconfig
-drwxrwxrwx   0        0        0        0 2023-05-24 20:48:23.917023 srsinst.uga-0.0.2/srsinst.uga.egg-info/
--rw-rw-rw-   0        0        0     7000 2023-05-24 20:48:23.000000 srsinst.uga-0.0.2/srsinst.uga.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      817 2023-05-24 20:48:23.000000 srsinst.uga-0.0.2/srsinst.uga.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 20:48:23.000000 srsinst.uga-0.0.2/srsinst.uga.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-24 20:48:23.000000 srsinst.uga-0.0.2/srsinst.uga.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       81 2023-05-24 20:48:23.000000 srsinst.uga-0.0.2/srsinst.uga.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-24 20:48:23.000000 srsinst.uga-0.0.2/srsinst.uga.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 18:54:39.247864 srsinst.uga-0.0.3/
+-rw-rw-rw-   0        0        0     1103 2023-05-19 19:35:50.000000 srsinst.uga-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     7117 2023-06-15 18:54:39.247864 srsinst.uga-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6336 2023-06-15 18:39:17.000000 srsinst.uga-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 18:54:39.227864 srsinst.uga-0.0.3/docs/
+-rw-rw-rw-   0        0        0      654 2023-05-19 21:28:14.000000 srsinst.uga-0.0.3/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-06-15 18:54:39.212422 srsinst.uga-0.0.3/docs/_static/
+drwxrwxrwx   0        0        0        0 2023-06-15 18:54:39.227864 srsinst.uga-0.0.3/docs/_static/image/
+-rw-rw-rw-   0        0        0   174299 2023-05-16 16:03:57.000000 srsinst.uga-0.0.3/docs/_static/image/UGA100_composition_analysis_screenshot.png
+-rwxrwxrwx   0        0        0       28 2023-05-19 21:28:14.000000 srsinst.uga-0.0.3/docs/autodoc.bat
+-rw-rw-rw-   0        0        0     5458 2023-05-19 21:28:14.000000 srsinst.uga-0.0.3/docs/basic_operation.rst
+-rw-rw-rw-   0        0        0       26 2023-05-19 21:28:14.000000 srsinst.uga-0.0.3/docs/changelog.rst
+-rw-rw-rw-   0        0        0     1985 2023-06-13 17:27:43.000000 srsinst.uga-0.0.3/docs/conf.py
+-rw-rw-rw-   0        0        0     1168 2023-05-19 21:28:14.000000 srsinst.uga-0.0.3/docs/connection.rst
+-rw-rw-rw-   0        0        0     1541 2023-06-13 17:07:45.000000 srsinst.uga-0.0.3/docs/index.rst
+-rw-rw-rw-   0        0        0     1246 2023-05-19 21:28:14.000000 srsinst.uga-0.0.3/docs/installation.rst
+-rwxrwxrwx   0        0        0      802 2023-05-19 21:28:14.000000 srsinst.uga-0.0.3/docs/make.bat
+-rw-rw-rw-   0        0        0       32 2023-05-19 21:28:14.000000 srsinst.uga-0.0.3/docs/requirements.txt
+-rw-rw-rw-   0        0        0     1010 2023-05-19 21:28:14.000000 srsinst.uga-0.0.3/docs/scan_operation.rst
+-rw-rw-rw-   0        0        0      329 2023-06-13 17:18:39.000000 srsinst.uga-0.0.3/docs/srsinst.uga.instruments.rst
+-rw-rw-rw-   0        0        0      478 2023-06-13 17:16:42.000000 srsinst.uga-0.0.3/docs/srsinst.uga.instruments.uga100.rst
+-rw-rw-rw-   0        0        0      134 2023-05-19 21:28:14.000000 srsinst.uga-0.0.3/docs/srsinst.uga.rst
+-rw-rw-rw-   0        0        0      530 2023-06-13 17:33:33.000000 srsinst.uga-0.0.3/docs/srsinst.uga.tasks.rst
+-rw-rw-rw-   0        0        0     1473 2023-05-19 21:28:14.000000 srsinst.uga-0.0.3/docs/troubleshooting.rst
+-rw-rw-rw-   0        0        0     1231 2023-06-15 17:27:23.000000 srsinst.uga-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-15 18:54:39.247864 srsinst.uga-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsinst.uga-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 18:54:39.212422 srsinst.uga-0.0.3/srsinst/
+drwxrwxrwx   0        0        0        0 2023-06-15 18:54:39.237864 srsinst.uga-0.0.3/srsinst/uga/
+-rw-rw-rw-   0        0        0      229 2023-06-15 18:52:48.000000 srsinst.uga-0.0.3/srsinst/uga/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-05-19 21:22:28.000000 srsinst.uga-0.0.3/srsinst/uga/__main__.py
+-rw-rw-rw-   0        0        0    10600 2023-05-19 21:22:27.000000 srsinst.uga-0.0.3/srsinst/uga/gaslib.dat
+drwxrwxrwx   0        0        0        0 2023-06-15 18:54:39.237864 srsinst.uga-0.0.3/srsinst/uga/instruments/
+-rw-rw-rw-   0        0        0       47 2023-05-19 21:22:28.000000 srsinst.uga-0.0.3/srsinst/uga/instruments/__init__.py
+-rw-rw-rw-   0        0        0     1327 2023-05-19 21:32:52.000000 srsinst.uga-0.0.3/srsinst/uga/instruments/get_instruments.py
+drwxrwxrwx   0        0        0        0 2023-06-15 18:54:39.237864 srsinst.uga-0.0.3/srsinst/uga/instruments/uga100/
+-rw-rw-rw-   0        0        0        0 2023-05-19 21:22:28.000000 srsinst.uga-0.0.3/srsinst/uga/instruments/uga100/__init__.py
+-rw-rw-rw-   0        0        0    10643 2023-05-31 00:34:22.000000 srsinst.uga-0.0.3/srsinst/uga/instruments/uga100/components.py
+-rw-rw-rw-   0        0        0     4643 2023-05-24 17:51:21.000000 srsinst.uga-0.0.3/srsinst/uga/instruments/uga100/keys.py
+-rw-rw-rw-   0        0        0     5544 2023-06-15 17:42:38.000000 srsinst.uga-0.0.3/srsinst/uga/instruments/uga100/uga.py
+drwxrwxrwx   0        0        0        0 2023-06-15 18:54:39.247864 srsinst.uga-0.0.3/srsinst/uga/tasks/
+-rw-rw-rw-   0        0        0        0 2023-05-19 21:22:28.000000 srsinst.uga-0.0.3/srsinst/uga/tasks/__init__.py
+-rw-rw-rw-   0        0        0     4415 2023-05-24 17:26:46.000000 srsinst.uga-0.0.3/srsinst/uga/tasks/ugamodecontroltask.py
+-rw-rw-rw-   0        0        0     3881 2023-05-19 21:34:42.000000 srsinst.uga-0.0.3/srsinst/uga/tasks/ugamultiplottask.py
+-rw-rw-rw-   0        0        0     1949 2023-05-24 18:32:16.000000 srsinst.uga-0.0.3/srsinst/uga/tasks/ugastatemonitortask.py
+-rw-rw-rw-   0        0        0     2339 2023-05-24 16:25:05.000000 srsinst.uga-0.0.3/srsinst/uga/uga.taskconfig
+drwxrwxrwx   0        0        0        0 2023-06-15 18:54:39.227864 srsinst.uga-0.0.3/srsinst.uga.egg-info/
+-rw-rw-rw-   0        0        0     7117 2023-06-15 18:54:39.000000 srsinst.uga-0.0.3/srsinst.uga.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1157 2023-06-15 18:54:39.000000 srsinst.uga-0.0.3/srsinst.uga.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 18:54:39.000000 srsinst.uga-0.0.3/srsinst.uga.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-15 18:54:39.000000 srsinst.uga-0.0.3/srsinst.uga.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2023-06-15 18:54:39.000000 srsinst.uga-0.0.3/srsinst.uga.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-15 18:54:39.000000 srsinst.uga-0.0.3/srsinst.uga.egg-info/top_level.txt
```

### Comparing `srsinst.uga-0.0.2/LICENSE` & `srsinst.uga-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.2/PKG-INFO` & `srsinst.uga-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsinst.uga
-Version: 0.0.2
+Version: 0.0.3
 Summary: Instrument driver package for Universal Gas Analyzers (UGA) from Stanford Research Systems
 Author: Chulhoon Kim
 License: MIT license
 Keywords: UGA,universal gas analyzer,SRS,Stanford Research Systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -18,23 +18,24 @@
 Provides-Extra: full
 License-File: LICENSE
 
 # `srsinst.uga`
 
 `srsinst.uga` contains a Python instrument driver to control and acquire 
 mass spectra of atmospheric gas samples from 
-[Stanford Research Systems (SRS) Universal Gas Analyzer (UGA)](https://thinksrs.com/products/uga.html). It also has a collection of Python scripts 
-that runs on a graphic user interface (GUI) based on [srsgui](https://thinksrs.github.io/srsgui/).
-
+[Stanford Research Systems (SRS) Universal Gas Analyzer (UGA)](https://thinksrs.com/products/uga.html).
+It also provides a collection of Python scripts that runs on a graphic user interface (GUI) based on
+[srsgui](https://thinksrs.github.io/srsgui/) and 
+[srsinst.rga](https://thinksrs.github.io/srsinst.rga/). 
 
 ![screenshot](https://github.com/thinkSRS/srsinst.uga/blob/main/docs/_static/image/UGA100_composition_analysis_screenshot.png " ")
 
 ## Installation
-You need a working Python with `pip` (Python package installer) installed. If you don't,
-[install Python 3](https://realpython.com/installing-python/) to your system.
+You need a working Python version 3.7 or later with `pip` (Python package installer) installed.
+If you don't, [install Python 3](https://www.python.org/) to your system.
 
 To install `srsinst.uga` as an instrument driver only, use Python package installer `pip` 
 from the command line.
 
     python -m pip install srsinst.uga
 
 To use its full GUI application, create a virtual environment, if necessary,
@@ -180,10 +181,11 @@
      'index_dict': None}
 
 When the ion gauge is on, you can get a pressure measurement with the get_pressure() method.
 
     >>> uga.ig.get_pressure()
     1.115742e-07
 
-The most important component in a UGA is the Residual Gas Analyzer (RGA). 
-It has a separate [instrument driver package](https://pypi.org/project/srsinst.rga/) 
-to use an independent RGA. Refer to its documentation for RGA component usage.  
+The most important component in a UGA is the Residual Gas Analyzer, 
+which has the separate [RGA instrument driver package](https://github.com/thinkSRS/srsinst.rga)
+ for its independent usage.
+Refer to [RGA documentation](https://thinksrs.github.io/srsinst.rga/) for RGA component usage.
```

### Comparing `srsinst.uga-0.0.2/README.md` & `srsinst.uga-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # `srsinst.uga`
 
 `srsinst.uga` contains a Python instrument driver to control and acquire 
 mass spectra of atmospheric gas samples from 
-[Stanford Research Systems (SRS) Universal Gas Analyzer (UGA)](https://thinksrs.com/products/uga.html). It also has a collection of Python scripts 
-that runs on a graphic user interface (GUI) based on [srsgui](https://thinksrs.github.io/srsgui/).
-
+[Stanford Research Systems (SRS) Universal Gas Analyzer (UGA)](https://thinksrs.com/products/uga.html).
+It also provides a collection of Python scripts that runs on a graphic user interface (GUI) based on
+[srsgui](https://thinksrs.github.io/srsgui/) and 
+[srsinst.rga](https://thinksrs.github.io/srsinst.rga/). 
 
 ![screenshot](https://github.com/thinkSRS/srsinst.uga/blob/main/docs/_static/image/UGA100_composition_analysis_screenshot.png " ")
 
 ## Installation
-You need a working Python with `pip` (Python package installer) installed. If you don't,
-[install Python 3](https://realpython.com/installing-python/) to your system.
+You need a working Python version 3.7 or later with `pip` (Python package installer) installed.
+If you don't, [install Python 3](https://www.python.org/) to your system.
 
 To install `srsinst.uga` as an instrument driver only, use Python package installer `pip` 
 from the command line.
 
     python -m pip install srsinst.uga
 
 To use its full GUI application, create a virtual environment, if necessary,
@@ -160,10 +161,11 @@
      'index_dict': None}
 
 When the ion gauge is on, you can get a pressure measurement with the get_pressure() method.
 
     >>> uga.ig.get_pressure()
     1.115742e-07
 
-The most important component in a UGA is the Residual Gas Analyzer (RGA). 
-It has a separate [instrument driver package](https://pypi.org/project/srsinst.rga/) 
-to use an independent RGA. Refer to its documentation for RGA component usage.  
+The most important component in a UGA is the Residual Gas Analyzer, 
+which has the separate [RGA instrument driver package](https://github.com/thinkSRS/srsinst.rga)
+ for its independent usage.
+Refer to [RGA documentation](https://thinksrs.github.io/srsinst.rga/) for RGA component usage.
```

### Comparing `srsinst.uga-0.0.2/docs/_static/image/UGA100_composition_analysis_screenshot.png` & `srsinst.uga-0.0.3/docs/_static/image/UGA100_composition_analysis_screenshot.png`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.2/pyproject.toml` & `srsinst.uga-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -20,19 +20,20 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Topic :: Scientific/Engineering"
 ]
 dependencies = [
-    "numpy", "scipy", "srsgui>=0.2.16", "srsinst.rga>=0.2.11"
+    "numpy", "scipy", "srsgui>=0.3.3", "srsinst.rga>=0.3.3"
 ]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = {attr = "srsinst.uga.__version__"}
 
 [project.optional-dependencies]
-full = ['matplotlib>=3.6.2', 'pyside6']
+full = ['matplotlib >= 3.6.2', 'pyside6']
+# For Dependency specification, Refer to PEP 631
 
 [project.scripts]
 uga = "srsinst.uga.__main__:main"
```

### Comparing `srsinst.uga-0.0.2/srsinst/uga/gaslib.dat` & `srsinst.uga-0.0.3/srsinst/uga/gaslib.dat`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.2/srsinst/uga/instruments/get_instruments.py` & `srsinst.uga-0.0.3/srsinst/uga/instruments/get_instruments.py`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.2/srsinst/uga/instruments/uga100/components.py` & `srsinst.uga-0.0.3/srsinst/uga/instruments/uga100/components.py`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.2/srsinst/uga/instruments/uga100/keys.py` & `srsinst.uga-0.0.3/srsinst/uga/instruments/uga100/keys.py`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.2/srsinst/uga/instruments/uga100/uga.py` & `srsinst.uga-0.0.3/srsinst/uga/instruments/uga100/uga.py`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.2/srsinst/uga/tasks/ugamodecontroltask.py` & `srsinst.uga-0.0.3/srsinst/uga/tasks/ugamodecontroltask.py`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.2/srsinst/uga/tasks/ugamultiplottask.py` & `srsinst.uga-0.0.3/srsinst/uga/tasks/ugamultiplottask.py`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.2/srsinst/uga/tasks/ugastatemonitortask.py` & `srsinst.uga-0.0.3/srsinst/uga/tasks/ugastatemonitortask.py`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.2/srsinst/uga/uga.taskconfig` & `srsinst.uga-0.0.3/srsinst/uga/uga.taskconfig`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.2/srsinst.uga.egg-info/PKG-INFO` & `srsinst.uga-0.0.3/srsinst.uga.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsinst.uga
-Version: 0.0.2
+Version: 0.0.3
 Summary: Instrument driver package for Universal Gas Analyzers (UGA) from Stanford Research Systems
 Author: Chulhoon Kim
 License: MIT license
 Keywords: UGA,universal gas analyzer,SRS,Stanford Research Systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -18,23 +18,24 @@
 Provides-Extra: full
 License-File: LICENSE
 
 # `srsinst.uga`
 
 `srsinst.uga` contains a Python instrument driver to control and acquire 
 mass spectra of atmospheric gas samples from 
-[Stanford Research Systems (SRS) Universal Gas Analyzer (UGA)](https://thinksrs.com/products/uga.html). It also has a collection of Python scripts 
-that runs on a graphic user interface (GUI) based on [srsgui](https://thinksrs.github.io/srsgui/).
-
+[Stanford Research Systems (SRS) Universal Gas Analyzer (UGA)](https://thinksrs.com/products/uga.html).
+It also provides a collection of Python scripts that runs on a graphic user interface (GUI) based on
+[srsgui](https://thinksrs.github.io/srsgui/) and 
+[srsinst.rga](https://thinksrs.github.io/srsinst.rga/). 
 
 ![screenshot](https://github.com/thinkSRS/srsinst.uga/blob/main/docs/_static/image/UGA100_composition_analysis_screenshot.png " ")
 
 ## Installation
-You need a working Python with `pip` (Python package installer) installed. If you don't,
-[install Python 3](https://realpython.com/installing-python/) to your system.
+You need a working Python version 3.7 or later with `pip` (Python package installer) installed.
+If you don't, [install Python 3](https://www.python.org/) to your system.
 
 To install `srsinst.uga` as an instrument driver only, use Python package installer `pip` 
 from the command line.
 
     python -m pip install srsinst.uga
 
 To use its full GUI application, create a virtual environment, if necessary,
@@ -180,10 +181,11 @@
      'index_dict': None}
 
 When the ion gauge is on, you can get a pressure measurement with the get_pressure() method.
 
     >>> uga.ig.get_pressure()
     1.115742e-07
 
-The most important component in a UGA is the Residual Gas Analyzer (RGA). 
-It has a separate [instrument driver package](https://pypi.org/project/srsinst.rga/) 
-to use an independent RGA. Refer to its documentation for RGA component usage.  
+The most important component in a UGA is the Residual Gas Analyzer, 
+which has the separate [RGA instrument driver package](https://github.com/thinkSRS/srsinst.rga)
+ for its independent usage.
+Refer to [RGA documentation](https://thinksrs.github.io/srsinst.rga/) for RGA component usage.
```

