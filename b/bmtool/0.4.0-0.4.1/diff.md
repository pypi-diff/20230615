# Comparing `tmp/bmtool-0.4.0.tar.gz` & `tmp/bmtool-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmtool-0.4.0.tar", last modified: Tue Jun  6 18:06:08 2023, max compression
+gzip compressed data, was "bmtool-0.4.1.tar", last modified: Thu Jun 15 00:32:22 2023, max compression
```

## Comparing `bmtool-0.4.0.tar` & `bmtool-0.4.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 18:06:08.312708 bmtool-0.4.0/
--rw-rw-rw-   0        0        0     1089 2022-09-11 17:13:05.000000 bmtool-0.4.0/LICENSE
--rw-rw-rw-   0        0        0    17751 2023-06-06 18:06:08.312708 bmtool-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    17006 2023-05-31 22:34:19.000000 bmtool-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 18:06:08.268740 bmtool-0.4.0/bmtool/
--rw-rw-rw-   0        0        0      141 2023-03-17 15:08:47.000000 bmtool-0.4.0/bmtool/__init__.py
--rw-rw-rw-   0        0        0      676 2023-03-17 15:09:21.000000 bmtool-0.4.0/bmtool/__main__.py
--rw-rw-rw-   0        0        0    29723 2023-06-01 20:21:45.000000 bmtool-0.4.0/bmtool/bmplot.py
-drwxrwxrwx   0        0        0        0 2023-06-06 18:06:08.297710 bmtool-0.4.0/bmtool/debug/
--rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.4.0/bmtool/debug/__init__.py
--rw-rw-rw-   0        0        0      602 2022-09-11 17:13:05.000000 bmtool-0.4.0/bmtool/debug/commands.py
--rw-rw-rw-   0        0        0      218 2023-03-17 14:52:10.000000 bmtool-0.4.0/bmtool/debug/debug.py
--rw-rw-rw-   0        0        0      688 2023-03-17 15:12:53.000000 bmtool-0.4.0/bmtool/manage.py
--rw-rw-rw-   0        0        0    12528 2023-06-01 14:19:08.000000 bmtool-0.4.0/bmtool/plot_commands.py
--rw-rw-rw-   0        0        0    22524 2023-06-06 18:05:24.000000 bmtool-0.4.0/bmtool/singlecell.py
-drwxrwxrwx   0        0        0        0 2023-06-06 18:06:08.305706 bmtool-0.4.0/bmtool/util/
--rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.4.0/bmtool/util/__init__.py
--rw-rw-rw-   0        0        0    65882 2023-03-17 15:09:19.000000 bmtool-0.4.0/bmtool/util/commands.py
-drwxrwxrwx   0        0        0        0 2023-06-06 18:06:08.309745 bmtool-0.4.0/bmtool/util/neuron/
--rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.4.0/bmtool/util/neuron/__init__.py
--rw-rw-rw-   0        0        0    89259 2023-03-17 14:53:16.000000 bmtool-0.4.0/bmtool/util/neuron/celltuner.py
--rw-rw-rw-   0        0        0    51814 2023-05-29 23:57:07.000000 bmtool-0.4.0/bmtool/util/util.py
-drwxrwxrwx   0        0        0        0 2023-06-06 18:06:08.292734 bmtool-0.4.0/bmtool.egg-info/
--rw-rw-rw-   0        0        0    17751 2023-06-06 18:06:06.000000 bmtool-0.4.0/bmtool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-06-06 18:06:06.000000 bmtool-0.4.0/bmtool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 18:06:06.000000 bmtool-0.4.0/bmtool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-06 18:06:06.000000 bmtool-0.4.0/bmtool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       76 2023-06-06 18:06:06.000000 bmtool-0.4.0/bmtool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-06 18:06:06.000000 bmtool-0.4.0/bmtool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 18:06:08.313708 bmtool-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1348 2023-06-06 18:05:36.000000 bmtool-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 00:32:22.056233 bmtool-0.4.1/
+-rw-rw-rw-   0        0        0     1089 2022-09-11 17:13:05.000000 bmtool-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0    18106 2023-06-15 00:32:22.056233 bmtool-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0    17361 2023-06-15 00:31:36.000000 bmtool-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 00:32:22.009329 bmtool-0.4.1/bmtool/
+-rw-rw-rw-   0        0        0      141 2023-03-17 15:08:47.000000 bmtool-0.4.1/bmtool/__init__.py
+-rw-rw-rw-   0        0        0      676 2023-03-17 15:09:21.000000 bmtool-0.4.1/bmtool/__main__.py
+-rw-rw-rw-   0        0        0    29723 2023-06-01 20:21:45.000000 bmtool-0.4.1/bmtool/bmplot.py
+-rw-rw-rw-   0        0        0    61181 2023-06-15 00:31:36.000000 bmtool-0.4.1/bmtool/connectors.py
+drwxrwxrwx   0        0        0        0 2023-06-15 00:32:22.040576 bmtool-0.4.1/bmtool/debug/
+-rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.4.1/bmtool/debug/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-09-11 17:13:05.000000 bmtool-0.4.1/bmtool/debug/commands.py
+-rw-rw-rw-   0        0        0      218 2023-03-17 14:52:10.000000 bmtool-0.4.1/bmtool/debug/debug.py
+-rw-rw-rw-   0        0        0      688 2023-03-17 15:12:53.000000 bmtool-0.4.1/bmtool/manage.py
+-rw-rw-rw-   0        0        0    12528 2023-06-01 14:19:08.000000 bmtool-0.4.1/bmtool/plot_commands.py
+-rw-rw-rw-   0        0        0    22524 2023-06-06 18:05:24.000000 bmtool-0.4.1/bmtool/singlecell.py
+drwxrwxrwx   0        0        0        0 2023-06-15 00:32:22.056233 bmtool-0.4.1/bmtool/util/
+-rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.4.1/bmtool/util/__init__.py
+-rw-rw-rw-   0        0        0    65882 2023-03-17 15:09:19.000000 bmtool-0.4.1/bmtool/util/commands.py
+drwxrwxrwx   0        0        0        0 2023-06-15 00:32:22.056233 bmtool-0.4.1/bmtool/util/neuron/
+-rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.4.1/bmtool/util/neuron/__init__.py
+-rw-rw-rw-   0        0        0    89259 2023-03-17 14:53:16.000000 bmtool-0.4.1/bmtool/util/neuron/celltuner.py
+-rw-rw-rw-   0        0        0    51814 2023-05-29 23:57:07.000000 bmtool-0.4.1/bmtool/util/util.py
+drwxrwxrwx   0        0        0        0 2023-06-15 00:32:22.024955 bmtool-0.4.1/bmtool.egg-info/
+-rw-rw-rw-   0        0        0    18106 2023-06-15 00:32:20.000000 bmtool-0.4.1/bmtool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-06-15 00:32:20.000000 bmtool-0.4.1/bmtool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 00:32:20.000000 bmtool-0.4.1/bmtool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-15 00:32:20.000000 bmtool-0.4.1/bmtool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       76 2023-06-15 00:32:20.000000 bmtool-0.4.1/bmtool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-15 00:32:20.000000 bmtool-0.4.1/bmtool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 00:32:22.056233 bmtool-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1348 2023-06-15 00:31:49.000000 bmtool-0.4.1/setup.py
```

### Comparing `bmtool-0.4.0/LICENSE` & `bmtool-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bmtool-0.4.0/PKG-INFO` & `bmtool-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmtool
-Version: 0.4.0
+Version: 0.4.1
 Summary: BMTool
 Home-page: https://github.com/tjbanks/bmtool
 Download-URL: 
 Author: Tyler Banks
 Author-email: tbanks@mail.missouri.edu
 License: MIT
 Classifier: Intended Audience :: Developers
@@ -389,14 +389,21 @@
 ### Simulation Summary
 
 Using previous functions, plots connection probability as a function of distance, total connections, cell information, current clamp information, input spike train information, and a 3D plot of the network if specified. 
 ```
 bmtool plot --config simulation_config_foo.json summary
 ```
 
+### Connectors Module
+
+This module contains helper functions and classes that work with BMTK's NetworkBuilder module in building networks. It facilitates building reciprocal connections, distance dependent connections, afferent connections, etc. See documentation inside the script `connectors.py` for usage.
+```
+from bmtool import connectors
+```
+
 ## Cell Tuning
 
 ### Python/Jupyter
 
 Single Cell Profiler
 
 ```
```

### Comparing `bmtool-0.4.0/README.md` & `bmtool-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -368,14 +368,21 @@
 ### Simulation Summary
 
 Using previous functions, plots connection probability as a function of distance, total connections, cell information, current clamp information, input spike train information, and a 3D plot of the network if specified. 
 ```
 bmtool plot --config simulation_config_foo.json summary
 ```
 
+### Connectors Module
+
+This module contains helper functions and classes that work with BMTK's NetworkBuilder module in building networks. It facilitates building reciprocal connections, distance dependent connections, afferent connections, etc. See documentation inside the script `connectors.py` for usage.
+```
+from bmtool import connectors
+```
+
 ## Cell Tuning
 
 ### Python/Jupyter
 
 Single Cell Profiler
 
 ```
```

### Comparing `bmtool-0.4.0/bmtool/__main__.py` & `bmtool-0.4.1/bmtool/__main__.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.4.0/bmtool/bmplot.py` & `bmtool-0.4.1/bmtool/bmplot.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.4.0/bmtool/debug/commands.py` & `bmtool-0.4.1/bmtool/debug/commands.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.4.0/bmtool/manage.py` & `bmtool-0.4.1/bmtool/manage.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.4.0/bmtool/plot_commands.py` & `bmtool-0.4.1/bmtool/plot_commands.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.4.0/bmtool/singlecell.py` & `bmtool-0.4.1/bmtool/singlecell.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.4.0/bmtool/util/commands.py` & `bmtool-0.4.1/bmtool/util/commands.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.4.0/bmtool/util/neuron/celltuner.py` & `bmtool-0.4.1/bmtool/util/neuron/celltuner.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.4.0/bmtool/util/util.py` & `bmtool-0.4.1/bmtool/util/util.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.4.0/bmtool.egg-info/PKG-INFO` & `bmtool-0.4.1/bmtool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmtool
-Version: 0.4.0
+Version: 0.4.1
 Summary: BMTool
 Home-page: https://github.com/tjbanks/bmtool
 Download-URL: 
 Author: Tyler Banks
 Author-email: tbanks@mail.missouri.edu
 License: MIT
 Classifier: Intended Audience :: Developers
@@ -389,14 +389,21 @@
 ### Simulation Summary
 
 Using previous functions, plots connection probability as a function of distance, total connections, cell information, current clamp information, input spike train information, and a 3D plot of the network if specified. 
 ```
 bmtool plot --config simulation_config_foo.json summary
 ```
 
+### Connectors Module
+
+This module contains helper functions and classes that work with BMTK's NetworkBuilder module in building networks. It facilitates building reciprocal connections, distance dependent connections, afferent connections, etc. See documentation inside the script `connectors.py` for usage.
+```
+from bmtool import connectors
+```
+
 ## Cell Tuning
 
 ### Python/Jupyter
 
 Single Cell Profiler
 
 ```
```

### Comparing `bmtool-0.4.0/bmtool.egg-info/SOURCES.txt` & `bmtool-0.4.1/bmtool.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 bmtool/__init__.py
 bmtool/__main__.py
 bmtool/bmplot.py
+bmtool/connectors.py
 bmtool/manage.py
 bmtool/plot_commands.py
 bmtool/singlecell.py
 bmtool.egg-info/PKG-INFO
 bmtool.egg-info/SOURCES.txt
 bmtool.egg-info/dependency_links.txt
 bmtool.egg-info/entry_points.txt
```

### Comparing `bmtool-0.4.0/setup.py` & `bmtool-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="bmtool",
-    version="0.4.0",
+    version="0.4.1",
     author="Tyler Banks",
     author_email="tbanks@mail.missouri.edu",
     description="BMTool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tjbanks/bmtool",
     download_url='',
```

