# Comparing `tmp/helipad-1.5.1.tar.gz` & `tmp/helipad-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helipad-1.5.1.tar", last modified: Sat Jan 14 21:31:26 2023, max compression
+gzip compressed data, was "helipad-1.6.tar", last modified: Thu Jun 15 20:21:25 2023, max compression
```

## Comparing `helipad-1.5.1.tar` & `helipad-1.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-01-14 21:31:26.675716 helipad-1.5.1/
--rw-r--r--   0 charwick   (501) staff       (20)     1066 2023-01-08 22:00:03.000000 helipad-1.5.1/LICENSE
--rw-r--r--   0 charwick   (501) staff       (20)     5818 2023-01-14 21:31:26.675291 helipad-1.5.1/PKG-INFO
--rw-r--r--   0 charwick   (501) staff       (20)     3756 2023-01-13 17:52:45.000000 helipad-1.5.1/README.md
-drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-01-14 21:31:26.657292 helipad-1.5.1/helipad/
--rw-r--r--   0 charwick   (501) staff       (20)   379036 2022-06-27 21:28:10.000000 helipad-1.5.1/helipad/Helipad.png
--rw-r--r--   0 charwick   (501) staff       (20)      139 2023-01-14 21:30:46.000000 helipad-1.5.1/helipad/__init__.py
--rw-r--r--   0 charwick   (501) staff       (20)    16383 2023-01-14 21:25:20.000000 helipad-1.5.1/helipad/agent.py
--rw-r--r--   0 charwick   (501) staff       (20)    12783 2023-01-13 02:49:00.000000 helipad-1.5.1/helipad/cpanelJupyter.py
--rw-r--r--   0 charwick   (501) staff       (20)    25677 2023-01-13 02:53:00.000000 helipad-1.5.1/helipad/cpanelTkinter.py
--rw-r--r--   0 charwick   (501) staff       (20)     6113 2023-01-14 21:24:35.000000 helipad-1.5.1/helipad/data.py
--rw-r--r--   0 charwick   (501) staff       (20)     3191 2023-01-09 05:16:38.000000 helipad-1.5.1/helipad/helpers.py
--rw-r--r--   0 charwick   (501) staff       (20)     3414 2022-08-23 03:14:37.000000 helipad-1.5.1/helipad/ipy-styles.css
-drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-01-14 21:31:26.659626 helipad-1.5.1/helipad/locales/
-drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-01-14 21:31:26.646231 helipad-1.5.1/helipad/locales/en/
-drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-01-14 21:31:26.660230 helipad-1.5.1/helipad/locales/en/LC_MESSAGES/
--rw-r--r--   0 charwick   (501) staff       (20)      384 2022-07-16 05:19:14.000000 helipad-1.5.1/helipad/locales/en/LC_MESSAGES/helipad.mo
--rw-r--r--   0 charwick   (501) staff       (20)     7871 2023-01-10 00:00:53.000000 helipad-1.5.1/helipad/locales/helipad.pot
--rw-r--r--   0 charwick   (501) staff       (20)    34644 2023-01-14 21:24:14.000000 helipad-1.5.1/helipad/model.py
--rw-r--r--   0 charwick   (501) staff       (20)    21157 2023-01-13 02:43:26.000000 helipad-1.5.1/helipad/param.py
--rw-r--r--   0 charwick   (501) staff       (20)    13593 2023-01-11 20:40:39.000000 helipad-1.5.1/helipad/spatial.py
--rw-r--r--   0 charwick   (501) staff       (20)     4686 2022-12-11 23:47:40.000000 helipad-1.5.1/helipad/utility.py
--rw-r--r--   0 charwick   (501) staff       (20)    32301 2023-01-11 20:34:09.000000 helipad-1.5.1/helipad/visualize.py
-drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-01-14 21:31:26.659317 helipad-1.5.1/helipad.egg-info/
--rw-r--r--   0 charwick   (501) staff       (20)     5818 2023-01-14 21:31:26.000000 helipad-1.5.1/helipad.egg-info/PKG-INFO
--rw-r--r--   0 charwick   (501) staff       (20)     1047 2023-01-14 21:31:26.000000 helipad-1.5.1/helipad.egg-info/SOURCES.txt
--rw-r--r--   0 charwick   (501) staff       (20)        1 2023-01-14 21:31:26.000000 helipad-1.5.1/helipad.egg-info/dependency_links.txt
--rw-r--r--   0 charwick   (501) staff       (20)       73 2023-01-14 21:31:26.000000 helipad-1.5.1/helipad.egg-info/requires.txt
--rw-r--r--   0 charwick   (501) staff       (20)       39 2023-01-14 21:31:26.000000 helipad-1.5.1/helipad.egg-info/top_level.txt
--rw-r--r--   0 charwick   (501) staff       (20)     1189 2023-01-14 21:31:02.000000 helipad-1.5.1/pyproject.toml
-drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-01-14 21:31:26.668347 helipad-1.5.1/sample-models/
--rw-r--r--   0 charwick   (501) staff       (20)    10799 2023-01-05 00:54:39.000000 helipad-1.5.1/sample-models/Cities.py
--rw-r--r--   0 charwick   (501) staff       (20)    14233 2023-01-13 02:35:51.000000 helipad-1.5.1/sample-models/Helicopter-OMO.py
--rw-r--r--   0 charwick   (501) staff       (20)    15864 2023-01-09 04:59:13.000000 helipad-1.5.1/sample-models/Helicopter.py
--rw-r--r--   0 charwick   (501) staff       (20)     7019 2022-07-02 17:17:41.000000 helipad-1.5.1/sample-models/axelrod.py
--rw-r--r--   0 charwick   (501) staff       (20)     2747 2022-07-02 17:18:18.000000 helipad-1.5.1/sample-models/bootstrap.py
--rw-r--r--   0 charwick   (501) staff       (20)     4767 2023-01-09 05:16:42.000000 helipad-1.5.1/sample-models/cpanel-test.py
--rw-r--r--   0 charwick   (501) staff       (20)     1390 2023-01-05 02:29:26.000000 helipad-1.5.1/sample-models/crime.py
--rw-r--r--   0 charwick   (501) staff       (20)     5065 2022-07-01 18:20:40.000000 helipad-1.5.1/sample-models/criticalperiod.py
--rw-r--r--   0 charwick   (501) staff       (20)     3774 2022-07-02 17:19:30.000000 helipad-1.5.1/sample-models/demeSelection.py
--rw-r--r--   0 charwick   (501) staff       (20)     1541 2023-01-10 00:23:22.000000 helipad-1.5.1/sample-models/gameoflife.py
--rw-r--r--   0 charwick   (501) staff       (20)     5067 2023-01-11 20:49:50.000000 helipad-1.5.1/sample-models/grass.py
--rw-r--r--   0 charwick   (501) staff       (20)     3010 2022-07-02 17:20:34.000000 helipad-1.5.1/sample-models/pricediscover.py
--rw-r--r--   0 charwick   (501) staff       (20)     2484 2022-07-01 18:24:44.000000 helipad-1.5.1/sample-models/prisoners.py
-drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-01-14 21:31:26.672600 helipad-1.5.1/sample-notebooks/
--rw-r--r--   0 charwick   (501) staff       (20)    10518 2022-07-02 18:38:31.000000 helipad-1.5.1/sample-notebooks/axelrod.ipynb
--rw-r--r--   0 charwick   (501) staff       (20)     6030 2022-08-23 02:36:14.000000 helipad-1.5.1/sample-notebooks/cpanel-test.ipynb
--rw-r--r--   0 charwick   (501) staff       (20)    20989 2023-01-13 02:50:33.000000 helipad-1.5.1/sample-notebooks/helicopter.ipynb
--rw-r--r--   0 charwick   (501) staff       (20)    91586 2022-07-06 04:33:59.000000 helipad-1.5.1/sample-notebooks/pricediscover.ipynb
--rw-r--r--   0 charwick   (501) staff       (20)    86504 2022-07-01 18:52:02.000000 helipad-1.5.1/sample-notebooks/viz-tutorial.ipynb
--rw-r--r--   0 charwick   (501) staff       (20)       38 2023-01-14 21:31:26.675839 helipad-1.5.1/setup.cfg
+drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-06-15 20:21:25.900558 helipad-1.6/
+-rw-r--r--   0 charwick   (501) staff       (20)     1066 2023-01-08 22:00:03.000000 helipad-1.6/LICENSE
+-rw-r--r--   0 charwick   (501) staff       (20)     6054 2023-06-15 20:21:25.900186 helipad-1.6/PKG-INFO
+-rw-r--r--   0 charwick   (501) staff       (20)     3974 2023-06-15 19:09:24.000000 helipad-1.6/README.md
+drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-06-15 20:21:25.889691 helipad-1.6/helipad/
+-rw-r--r--   0 charwick   (501) staff       (20)   379036 2022-06-27 21:28:10.000000 helipad-1.6/helipad/Helipad.png
+-rw-r--r--   0 charwick   (501) staff       (20)      383 2023-05-29 03:23:08.000000 helipad-1.6/helipad/__init__.py
+-rw-r--r--   0 charwick   (501) staff       (20)    33987 2023-06-15 19:07:40.000000 helipad-1.6/helipad/agent.py
+-rw-r--r--   0 charwick   (501) staff       (20)    13252 2023-05-29 20:05:24.000000 helipad-1.6/helipad/cpanelJupyter.py
+-rw-r--r--   0 charwick   (501) staff       (20)    27019 2023-05-29 20:19:00.000000 helipad-1.6/helipad/cpanelTkinter.py
+-rw-r--r--   0 charwick   (501) staff       (20)     8676 2023-05-29 20:34:22.000000 helipad-1.6/helipad/data.py
+-rw-r--r--   0 charwick   (501) staff       (20)     3878 2023-06-15 19:39:17.000000 helipad-1.6/helipad/helpers.py
+-rw-r--r--   0 charwick   (501) staff       (20)     3414 2022-08-23 03:14:37.000000 helipad-1.6/helipad/ipy-styles.css
+drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-06-15 20:21:25.891778 helipad-1.6/helipad/locales/
+drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-06-15 20:21:25.884293 helipad-1.6/helipad/locales/en/
+drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-06-15 20:21:25.892171 helipad-1.6/helipad/locales/en/LC_MESSAGES/
+-rw-r--r--   0 charwick   (501) staff       (20)      434 2023-06-15 20:17:44.000000 helipad-1.6/helipad/locales/en/LC_MESSAGES/helipad.mo
+-rw-r--r--   0 charwick   (501) staff       (20)     8160 2023-06-15 20:15:08.000000 helipad-1.6/helipad/locales/helipad.pot
+-rw-r--r--   0 charwick   (501) staff       (20)    32130 2023-06-01 03:30:48.000000 helipad-1.6/helipad/model.py
+-rw-r--r--   0 charwick   (501) staff       (20)    25379 2023-05-29 21:10:59.000000 helipad-1.6/helipad/param.py
+-rw-r--r--   0 charwick   (501) staff       (20)    20367 2023-06-15 19:39:26.000000 helipad-1.6/helipad/spatial.py
+-rw-r--r--   0 charwick   (501) staff       (20)     5617 2023-05-30 03:50:59.000000 helipad-1.6/helipad/utility.py
+-rw-r--r--   0 charwick   (501) staff       (20)    41377 2023-06-15 19:49:19.000000 helipad-1.6/helipad/visualize.py
+drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-06-15 20:21:25.891381 helipad-1.6/helipad.egg-info/
+-rw-r--r--   0 charwick   (501) staff       (20)     6054 2023-06-15 20:21:25.000000 helipad-1.6/helipad.egg-info/PKG-INFO
+-rw-r--r--   0 charwick   (501) staff       (20)     1047 2023-06-15 20:21:25.000000 helipad-1.6/helipad.egg-info/SOURCES.txt
+-rw-r--r--   0 charwick   (501) staff       (20)        1 2023-06-15 20:21:25.000000 helipad-1.6/helipad.egg-info/dependency_links.txt
+-rw-r--r--   0 charwick   (501) staff       (20)       88 2023-06-15 20:21:25.000000 helipad-1.6/helipad.egg-info/requires.txt
+-rw-r--r--   0 charwick   (501) staff       (20)       39 2023-06-15 20:21:25.000000 helipad-1.6/helipad.egg-info/top_level.txt
+-rw-r--r--   0 charwick   (501) staff       (20)     1205 2023-06-15 20:01:21.000000 helipad-1.6/pyproject.toml
+drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-06-15 20:21:25.897241 helipad-1.6/sample-models/
+-rw-r--r--   0 charwick   (501) staff       (20)    10781 2023-06-01 03:41:45.000000 helipad-1.6/sample-models/Cities.py
+-rw-r--r--   0 charwick   (501) staff       (20)    14160 2023-06-01 03:38:03.000000 helipad-1.6/sample-models/Helicopter-OMO.py
+-rw-r--r--   0 charwick   (501) staff       (20)    15767 2023-06-01 03:38:38.000000 helipad-1.6/sample-models/Helicopter.py
+-rw-r--r--   0 charwick   (501) staff       (20)     7017 2023-05-21 00:37:25.000000 helipad-1.6/sample-models/axelrod.py
+-rw-r--r--   0 charwick   (501) staff       (20)     2756 2023-06-01 03:49:58.000000 helipad-1.6/sample-models/bootstrap.py
+-rw-r--r--   0 charwick   (501) staff       (20)     4937 2023-06-15 19:44:12.000000 helipad-1.6/sample-models/cpanel-test.py
+-rw-r--r--   0 charwick   (501) staff       (20)     1409 2023-05-22 22:18:00.000000 helipad-1.6/sample-models/crime.py
+-rw-r--r--   0 charwick   (501) staff       (20)     5074 2023-05-20 18:33:31.000000 helipad-1.6/sample-models/criticalperiod.py
+-rw-r--r--   0 charwick   (501) staff       (20)     3801 2023-06-01 03:40:50.000000 helipad-1.6/sample-models/demeSelection.py
+-rw-r--r--   0 charwick   (501) staff       (20)     1534 2023-06-01 03:56:20.000000 helipad-1.6/sample-models/gameoflife.py
+-rw-r--r--   0 charwick   (501) staff       (20)     5307 2023-05-30 03:17:05.000000 helipad-1.6/sample-models/grass.py
+-rw-r--r--   0 charwick   (501) staff       (20)     3011 2023-06-01 03:40:38.000000 helipad-1.6/sample-models/pricediscover.py
+-rw-r--r--   0 charwick   (501) staff       (20)     2491 2023-05-18 14:28:27.000000 helipad-1.6/sample-models/prisoners.py
+drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-06-15 20:21:25.899494 helipad-1.6/sample-notebooks/
+-rw-r--r--   0 charwick   (501) staff       (20)    10516 2023-05-18 14:28:45.000000 helipad-1.6/sample-notebooks/axelrod.ipynb
+-rw-r--r--   0 charwick   (501) staff       (20)     6015 2023-05-20 22:52:11.000000 helipad-1.6/sample-notebooks/cpanel-test.ipynb
+-rw-r--r--   0 charwick   (501) staff       (20)    20909 2023-06-01 03:39:28.000000 helipad-1.6/sample-notebooks/helicopter.ipynb
+-rw-r--r--   0 charwick   (501) staff       (20)    91616 2023-06-15 19:25:59.000000 helipad-1.6/sample-notebooks/pricediscover.ipynb
+-rw-r--r--   0 charwick   (501) staff       (20)    86511 2023-06-01 03:54:49.000000 helipad-1.6/sample-notebooks/viz-tutorial.ipynb
+-rw-r--r--   0 charwick   (501) staff       (20)       38 2023-06-15 20:21:25.900654 helipad-1.6/setup.cfg
```

### Comparing `helipad-1.5.1/LICENSE` & `helipad-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `helipad-1.5.1/PKG-INFO` & `helipad-1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helipad
-Version: 1.5.1
+Version: 1.6
 Summary: An agent-based modeling framework for Python with a shallow learning curve and powerful visualization capabilities.
 Author-email: C Harwick <cameron@cameronharwick.com>
 License: MIT License
         
         Copyright (c) 2023 C Harwick
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,17 +30,18 @@
 Project-URL: Source Code, https://github.com/charwick/helipad
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: notebook
+Provides-Extra: geo
 License-File: LICENSE
 
 # Helipad
 
 Helipad is an agent-based modeling framework for Python with powerful visualization capabilities and a shallow learning curve. Documentation and API reference can be found at [helipad.dev](https://helipad.dev).
 
 ## Features
@@ -69,32 +70,34 @@
 	
 	heli.launchCpanel()
 
 The included [bootstrap model](https://github.com/charwick/helipad/blob/master/sample-models/bootstrap.py) contains a more detailed template, and the [sample models](https://github.com/charwick/helipad/tree/master/sample-models) exemplify various use cases. The documentation also includes a complete [hook and function reference](https://helipad.dev/functions/).
 
 ## Requirements
 
-Helipad requires Python 3.7 or higher. The following libraries are also required:
+Helipad requires Python 3.8 or higher. The following libraries are also required:
 
 * [Matplotlib](https://matplotlib.org/) for visualization
 * [Pandas](https://pandas.pydata.org/) for data collection
 * [NetworkX](http://networkx.github.io/) for network analysis and spatial visualization
 * _Optional:_ [Jupyter](https://jupyter.org/), [Ipywidgets](https://pypi.org/project/ipywidgets/), and [ipympl](https://github.com/matplotlib/ipympl) to run Helipad in Jupyter notebooks
+* _Optional:_ [Shapely](https://shapely.readthedocs.io/) for geospatial models.
 
 ## How to Cite
 
 If you use Helipad in your own research, please cite as follows:
 
 > Harwick, Cameron (2021). “Helipad: A Framework for Agent-Based Modeling in Python.” Working paper available at [ssrn.com/abstract=3870501](https://ssrn.com/abstract=3870501). 
 
 ## Version History
 
+* [1.6](https://helipad.dev/2023/06/helipad-1-6/): Geospatial models, agent scatterplot visualizer, new `Agents` and `Edges` containers
 * [1.5](https://helipad.dev/2023/01/helipad-1-5/): Polar grid spatial models, various spatial improvements
 * [1.4](https://helipad.dev/2022/07/helipad-1-4/): More consistent container API, localization, miscellaneous interface improvements
 * [1.3](https://helipad.dev/2021/06/helipad-1-3/): Allow mixing time series and other plots, display networks on spatial maps, goods API improvements
 * [1.2](https://helipad.dev/2021/02/helipad-1-2/): Extensible visualization API, events, performance profiling, Jupyterlab support
 * [1.1](https://helipad.dev/2020/10/helipad-1-1/): Virtual parameters, improved Jupyter flexibility, spatial pre-alpha, misc improvements
 * [1.0](https://helipad.dev/2020/08/helipad-1-0/): Jupyter integration, hook decorators, and separated control panel from plotting
 * [0.7](https://helipad.dev/2020/06/helipad-0-7/): Ability to output stackplots, parameter sweeps, and an updated parameter identification pattern
 * [0.6](https://helipad.dev/2020/05/helipad-0-6/): Support for multi-level models
-* [0.5](https://helipad.dev/2020/03/helipad-0-5/): Support for matching models, and the checkGrid class
+* [0.5](https://helipad.dev/2020/03/helipad-0-5/): Support for matching models, and the `checkGrid` class
 * 0.4: Initial PyPI release
```

### Comparing `helipad-1.5.1/README.md` & `helipad-1.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -28,32 +28,34 @@
 	
 	heli.launchCpanel()
 
 The included [bootstrap model](https://github.com/charwick/helipad/blob/master/sample-models/bootstrap.py) contains a more detailed template, and the [sample models](https://github.com/charwick/helipad/tree/master/sample-models) exemplify various use cases. The documentation also includes a complete [hook and function reference](https://helipad.dev/functions/).
 
 ## Requirements
 
-Helipad requires Python 3.7 or higher. The following libraries are also required:
+Helipad requires Python 3.8 or higher. The following libraries are also required:
 
 * [Matplotlib](https://matplotlib.org/) for visualization
 * [Pandas](https://pandas.pydata.org/) for data collection
 * [NetworkX](http://networkx.github.io/) for network analysis and spatial visualization
 * _Optional:_ [Jupyter](https://jupyter.org/), [Ipywidgets](https://pypi.org/project/ipywidgets/), and [ipympl](https://github.com/matplotlib/ipympl) to run Helipad in Jupyter notebooks
+* _Optional:_ [Shapely](https://shapely.readthedocs.io/) for geospatial models.
 
 ## How to Cite
 
 If you use Helipad in your own research, please cite as follows:
 
 > Harwick, Cameron (2021). “Helipad: A Framework for Agent-Based Modeling in Python.” Working paper available at [ssrn.com/abstract=3870501](https://ssrn.com/abstract=3870501). 
 
 ## Version History
 
+* [1.6](https://helipad.dev/2023/06/helipad-1-6/): Geospatial models, agent scatterplot visualizer, new `Agents` and `Edges` containers
 * [1.5](https://helipad.dev/2023/01/helipad-1-5/): Polar grid spatial models, various spatial improvements
 * [1.4](https://helipad.dev/2022/07/helipad-1-4/): More consistent container API, localization, miscellaneous interface improvements
 * [1.3](https://helipad.dev/2021/06/helipad-1-3/): Allow mixing time series and other plots, display networks on spatial maps, goods API improvements
 * [1.2](https://helipad.dev/2021/02/helipad-1-2/): Extensible visualization API, events, performance profiling, Jupyterlab support
 * [1.1](https://helipad.dev/2020/10/helipad-1-1/): Virtual parameters, improved Jupyter flexibility, spatial pre-alpha, misc improvements
 * [1.0](https://helipad.dev/2020/08/helipad-1-0/): Jupyter integration, hook decorators, and separated control panel from plotting
 * [0.7](https://helipad.dev/2020/06/helipad-0-7/): Ability to output stackplots, parameter sweeps, and an updated parameter identification pattern
 * [0.6](https://helipad.dev/2020/05/helipad-0-6/): Support for multi-level models
-* [0.5](https://helipad.dev/2020/03/helipad-0-5/): Support for matching models, and the checkGrid class
+* [0.5](https://helipad.dev/2020/03/helipad-0-5/): Support for matching models, and the `checkGrid` class
 * 0.4: Initial PyPI release
```

### Comparing `helipad-1.5.1/helipad/Helipad.png` & `helipad-1.6/helipad/Helipad.png`

 * *Files identical despite different names*

### Comparing `helipad-1.5.1/helipad/cpanelJupyter.py` & `helipad-1.6/helipad/cpanelJupyter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,35 @@
+"""
+The control panel class for use in Jupyter notebooks. This module should not be imported directly; use `model.launchCpanel()` instead.
+"""
+
 import os
 from collections import ChainMap
 from ipywidgets import interactive, Layout, Accordion, HBox, VBox, HTML, Label, Button, FloatProgress
 from IPython.display import display
 from helipad.param import Param
 from helipad.helpers import ï
 
 class Cpanel(VBox):
-	def __init__(self, model, redraw=False):
+	"""The control panel class for use in Jupyter notebooks. https://helipad.dev/functions/cpanel/"""
+	def __init__(self, model, redraw: bool=False):
 		super().__init__()
 		self.model = model
 		if redraw:
 			self.children = ()
 			self.remove_class('invalid')
 		else: self.add_class('helipad_cpanel')
 		self.valid = True
 
 		#CSS niceties
 		__location__ = os.path.realpath(os.path.join(os.getcwd(), os.path.dirname(__file__)))
 		with open(os.path.join(__location__,'ipy-styles.css'), encoding='UTF-8') as c: css = c.read()
 
 		#CSS for goods and breeds, since Ipywidgets ≥8.0 oversanitizes HTML in description attributes
-		for n,c in ChainMap(*[{f'breed_{p}_{k}': v.color.hex for k,v in d.breeds.items()} for p,d in model.primitives.items()]+[{'good_'+k: v.color.hex for k,v in model.goods.items()}]).items():
+		for n,c in ChainMap(*[{f'breed_{p}_{k}': v.color.hex for k,v in d.breeds.items()} for p,d in model.agents.items()]+[{'good_'+k: v.color.hex for k,v in model.goods.items()}]).items():
 			css += f'.helipad_{n} .widget-label::before {{ background: {c} }}'
 
 		self.children += HTML(value='<style type="text/css">'+css+'</style>'),
 
 		#Callback function generator for Jupyter elements
 		def setVar(param, item=None):
 			def sv(val): #Ipywidgets bases on the function signature, so can't use more than one here…
@@ -36,15 +41,15 @@
 						pval = param.get(item) if param.type != 'checkgrid' else (item, param.get(item))
 						param.callback(self.model, param.name, pval)
 					else: param.callback(self.model, param.name, item, param.get(item))
 
 			#Consolidate value from bool and string, and toggle entry disabled state
 			#Have to return a different function since Ipywidgets bases the interactive off the function signature
 			if param.type=='checkentry':
-				def sv2(b,s):
+				def sv2(b: bool, s: str):
 					#Ipywidgets ≥8.0 runs the callback before the element is assigned
 					try:
 						els = param.element if item is None else param.elements[item]
 						els.children[1].disabled = not b
 					except (AttributeError, KeyError): return
 
 					#Coercing an int can fail, so if there's an exception, reset the textbox content
@@ -53,15 +58,15 @@
 						sv(val)
 					except: els.children[1].value = str(param.get())
 
 				return sv2
 			else: return sv
 		Param.setVar = setVar
 
-		def renderParam(param, func, title, val, circle=None):
+		def renderParam(param, func, title: str, val, circle=None):
 			i=None
 			if param.type=='slider':
 				if isinstance(param.opts, dict): i = interactive(func, val=(param.opts['low'],param.opts['high'], param.opts['step']))
 				else:
 					s = interactive(func, val=(0, len(param.opts)-1, 1))
 					s.children[0].readout = False
 					l = Label(value=str(param.opts[0]), layout=Layout(margin='0 0 0 15px'))
@@ -124,15 +129,15 @@
 					i.children[0].add_class('widget-logslider')
 					i.children[1].value = str(val)
 					if val in param.opts: val=param.opts.index(val)
 				if param.type!='checkentry': i.children[0].value = val
 
 			return i
 
-		def constructAccordion(param, itemList):
+		def constructAccordion(param, itemList: dict):
 			param.elements = {}
 			for item, good in itemList.items():
 				param.elements[item] = renderParam(param, param.setVar(item), item.title(), param.get(item), circle=good.color)
 
 			accordion = Accordion(children=[HBox(list(param.elements.values()))], selected_index=0)
 			accordion.set_title(0, param.title)
 			accordion.add_class('helipad_param_peritem helipad_paramgroup')
@@ -225,15 +230,15 @@
 		if not redraw:
 			display(self)
 
 			class progressBar(FloatProgress):
 				def __init__(self):
 					super().__init__(min=0, max=1)
 
-				def determinate(self, det):
+				def determinate(self, det: bool):
 					self.mode = 'determinate' if det else 'indeterminate'
 					if det: self.remove_class('indeterminate')
 					else:
 						self.add_class('indeterminate')
 						self.value = 1
 
 				def update(self, n): self.value = n
@@ -278,22 +283,24 @@
 				display(pbararea)
 
 			@model.hook('terminate')
 			def cpanel_terminate(model, data):
 				self.postinstruct.layout = Layout(display='inline-block')
 				self.stopbutton.layout.visibility = 'hidden'
 
-	def displayAlert(self, text, inCpanel=True):
+	def displayAlert(self, text: str, inCpanel: bool=True):
+		"""Display an alert element in the Jupyter notebook."""
 		element = HTML(value=text)
 		element.add_class('helipad_info') #Latter applies some built-in styles to the contents
 		if inCpanel: self.children += element,
 		else: display(element)
 		return element
 
-	def invalidate(self, message=ï('Model parameters changed, please re-launch the control panel with launchCpanel().')):
+	def invalidate(self, message: str=ï('Model parameters changed, please re-launch the control panel with launchCpanel().')):
+		"""Prevent the user from interacting with a control panel. A control panel is invalidated when another is launched."""
 		self.valid = False
 		self.add_class('invalid')
 		warning = Label(value=message)
 		warning.add_class('helipad_modal')
 		self.children += warning,
 		for p in self.model.params.values(): del p.element
 		return warning
```

### Comparing `helipad-1.5.1/helipad/cpanelTkinter.py` & `helipad-1.6/helipad/cpanelTkinter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# ==========
-# The standalone Tkinter-based control panel interface
-# Do not run this file; import model.py and run from your file.
-# ==========
+"""
+The Tkinter-based control panel class for use in standalone models. This module should not be imported directly; use `model.launchCpanel()` instead.
+"""
 
 import tkinter as tk
 import os, sys
 from math import ceil
 from tkinter.ttk import Progressbar
 from helipad.helpers import Color, ï
 from helipad.param import Param
 
 class Cpanel(tk.Tk):
+	"""The Tkinter-based control panel class for use in standalone models. https://helipad.dev/functions/cpanel/"""
 	def __init__(self, model):
 		self.model = model
 		super().__init__()
 		self.protocol("WM_DELETE_WINDOW", self.cpanelClose)
 
 		#Set application name
 		self.setAppIcon()
@@ -41,30 +41,30 @@
 					if param.per is None: param.callback(self.model, param.name, val)
 					else: param.callback(self.model, param.name, item, val)
 			return sv
 		Param.setVar = setVar
 
 		#For shock buttons.
 		#Can't do an inline lambda here because lambdas apparently don't preserve variable context
-		def shockCallback(name):
+		def shockCallback(name: str):
 			return lambda: self.model.shocks[name].do(self.model)
 
 		class progressBar(Progressbar):
-			def __init__(self, determinate=True, root=None):
+			def __init__(self, determinate: bool=True, root=None):
 				super().__init__(root, length=250, style="whitebg.Horizontal.TProgressbar")
 				self.determinate(determinate, False)
 				self.running = False
 
 			@property
 			def mode(self):
 				#Windows returns a string here, and MacOS returns an object
 				mode = self.cget('mode')
 				return mode if isinstance(mode, str) else self.cget('mode').string
 
-			def determinate(self2, det, refresh=True):
+			def determinate(self2, det: bool, refresh: bool=True):
 				self2.config(mode='determinate' if det else 'indeterminate')
 				if det: super().stop()
 				elif self2.running: super().start()
 				if refresh: self.update()
 			def update(self, n): self['value'] = n*100
 			def start(self):
 				if self.mode =='indeterminate': super().start()
@@ -303,40 +303,40 @@
 		cbot = self.model.doHooks('CpanelBottom', [self, bgcolors[fnum%2]])
 		if cbot:
 			cbot.pack(fill='x', side='top')
 			fnum += 1
 
 	#Separate function so we can call it again when MPL tries to override
 	def setAppIcon(self):
+		"""Set the dock/taskbar icon to the Helipad icon."""
 		try:
 			__location__ = os.path.realpath(os.path.join(os.getcwd(), os.path.dirname(__file__)))
 			icon = os.path.join(__location__, 'Helipad.png')
 			pi = tk.PhotoImage(file=icon, master=self)
 			self.tk.call('wm','iconphoto', self._w, pi)
 		except: pass
 
-	#Cleanup on cpanel close so a running model will keep running
 	def cpanelClose(self):
+		"""Cleanup on cpanel close so a running model will keep running."""
 		for p in self.model.params.values(): p.element = None
 		self.model.cpanel = None
 		self.destroy()
 
-	#Step one period at a time and update the graph
-	#For use in debugging
-	def step(self):
+	def step(self) -> int:
+		"""Step one period at a time and update the visualization. For use in debugging."""
 		t = self.model.step()
 		self.model.graph.update(self.model.data.getLast(1))
 		return t
 
 #
 # MISCELLANEOUS INTERFACE ELEMENTS
 #
 
-# A slider with defined non-linear intervals
 class logSlider(tk.Frame):
+	"""A slider with discrete specified intervals. https://helipad.dev/functions/logslider/"""
 	def __init__(self, parent=None, title=None, command=None, bg='#FFFFFF', font=('Lucida Grande',12), values=(), **kwargs):
 		tk.Frame.__init__(self, parent, bg=bg)
 		self.label = tk.Label(self, font=font, text=title, bg=bg).pack(side='top') if title else None
 		self.values = values
 		self.extCommand = command
 		self.number = values[0]
 
@@ -350,17 +350,16 @@
 			bg=bg, showvalue=0, from_=0, to=len(self.values)-1, font=font, **kwargs
 		)
 		self.text = tk.Label(self, font=font, width=4, bg=bg)
 		self.slide.pack(side='right', expand=1, fill='x')
 		self.text.pack(side='top', fill='both', padx=5)
 
 	def get(self): return self.number
-
-	#Receives a value externally and sets the slider to an index
 	def set(self, val):
+		"""Receive a value and set the slider to the corresponding index."""
 		self.number = val
 		if val in self.values: self.slide.set(self.values.index(val))
 		self.text.configure(text=val)
 
 	def enable(self): self.disabled(False)
 	def disable(self): self.disabled(True)
 	def disabled(self, val):
@@ -372,17 +371,17 @@
 			self.text.configure(fg='#333')
 			if self.label is not None: self.label.configure(fg='#333')
 			self.slide.configure(state='normal')
 
 	#Here for compatibility with other Tkinter widgets
 	def configure(self, state): self.disabled(state=='disabled')
 
-#A frame that can be expanded and collapsed by clicking on the title
 class expandableFrame(tk.Frame):
-	def __init__(self, parent=None, text="", fg='#333', bg='#FFF', padx=8, pady=None, font=None, startOpen=True):
+	"""A frame that can be expanded and collapsed by clicking on the title."""
+	def __init__(self, parent=None, text: str='', fg='#333', bg='#FFF', padx: int=8, pady=None, font=None, startOpen=True):
 		tk.Frame.__init__(self, parent, bg=bg)
 		self.columnconfigure(1, weight=1)
 
 		self.pady=pady
 		self.padx=padx
 
 		self.text = text
@@ -438,17 +437,16 @@
 			self.titleLabel['text'] = self.text+' '+'▾'
 			self._open.set(1)
 		else: #close
 			self.subframe.grid_forget()
 			self.titleLabel['text'] = self.text+' '+'▸'
 			self._open.set(0)
 
-# A checkbox-like widget whose toggle is the entire element
-# bg and fg take a two-element tuple for inactive and active states
 class textCheck(tk.Label):
+	"""A checkbox-like widget whose toggle is the entire element. `bg` and `fg` take a two-element color tuple for inactive and active states. https://helipad.dev/functions/textcheck/"""
 	def __init__(self, parent=None, text=None, bg=('#FFFFFF','#419BF9'), fg=('#333333','#FFFFFF'),
 		defaultValue=False, anchor='w', desc=None, callback=None
 	):
 		super().__init__(parent, text=text, bg=bg[defaultValue], fg=fg[defaultValue], anchor=anchor)
 		self.bg = (Color(bg[0]), Color(bg[1]))
 		self.fg = (Color(fg[0]), Color(fg[1]))
 
@@ -491,16 +489,16 @@
 		else:
 			bg = self.bg
 			fg = self.fg
 
 		self.enabled = not bool(disable)
 		self.config(bg=bg[self.value].hex, fg=fg[self.value].hex)
 
-# A checkbox that enables/disables a text box
 class checkEntry(tk.Frame):
+	"""A checkbox that enables/disables a text box. https://helipad.dev/functions/checkentry/"""
 	def __init__(self, parent=None, title=None, width=20, bg='#FFFFFF', padx=0, pady=0, default='', datatype='string', command=None, limits=(0, 10**100)):
 		tk.Frame.__init__(self, parent, bg=bg, padx=padx, pady=pady)
 		self.callback = command
 
 		#If we're enforcing int, don't allow nonnumerical input
 		self.datatype=datatype
 		def validate(code, insert, oldval, newval):
@@ -525,60 +523,66 @@
 		self.textbox.grid(row=0, column=1)
 
 		self.checkVar = tk.BooleanVar()
 		self.checkbox = tk.Checkbutton(self, text=title, bg=bg, var=self.checkVar, onvalue=True, offvalue=False, command=self.disableTextfield)
 		self.checkbox.grid(row=0, column=0)
 
 	def disableTextfield(self):
+		"""Update the enabled state of the text field to correspond to the value of the checkbox. https://helipad.dev/functions/checkentry/disabletextfield/"""
 		self.textbox.config(state='disabled' if not self.checkVar.get() else 'normal')
 		if callable(self.callback): self.callback(self.get())
 
-	#Return False or the value of the textbox
 	def get(self):
+		"""Retrieve the value of the combined input. Returns `False` if the checkbox is unchecked, and the value of the textbox otherwise. https://helipad.dev/functions/checkentry/get/"""
 		if not self.checkVar.get(): return False
 		v = self.entryValue.get()
 		if self.datatype=='int':
 			return 0 if v=='' else int(v)
 		else: return v
 
-	#Can pass a bool to turn on and off the checkbox, or a string or an int (depending on the datatype)
-	#to change the value of the textbox.
 	def set(self, val):
+		"""Set the input value. Can receive a `bool` to toggle the checkbox, or a `string` or an `int` (depending on the datatype) to change the value of the textbox. https://helipad.dev/functions/checkentry/set/"""
 		if isinstance(val, bool):
 			self.checkVar.set(val)
 		elif isinstance(val, (str, int)):
 			if self.datatype=='int' and val!='': val=int(val)
 			self.checkVar.set(True)
 			self.entryValue.set(val)
 		self.disableTextfield()
 
-	def enable(self): self.disabled(False)
-	def disable(self): self.disabled(True)
+	def enable(self):
+		"""Enable the `checkEntry` element so it can be interacted with by the user. https://helipad.dev/functions/checkentry/enable/"""
+		self.disabled(False)
+	def disable(self):
+		"""Disable the `checkEntry` element so it cannot be interacted with by the user.https://helipad.dev/functions/checkentry/disable/"""
+		self.disabled(True)
 	def disabled(self, disable):
+		"""Enables or disables the `checkEntry` element. https://helipad.dev/functions/checkentry/disabled/"""
 		self.checkbox.config(state='disabled' if disable else 'normal')
 		self.textbox.config(state='disabled' if disable or not self.checkVar.get() else 'normal')
 		self.enabled = not disable
 
 	#Here for compatibility with other Tkinter widgets
 	def configure(self, state): self.disabled(state=='disabled')
 
-#An expandableFrame full of textChecks, with setters and getters.
 class checkGrid(expandableFrame):
-	def __init__(self, parent=None, text="", columns=3, fg='#333', bg='#FFF', padx=8, pady=5, font=('Lucida Grande', 16) if sys.platform=='darwin' else ('Calibri', 14), startOpen=True, callback=None):
+	"""An `expandableFrame` full of `textCheck`s, with setters and getters. https://helipad.dev/functions/checkentry/"""
+	def __init__(self, parent=None, text: str='', columns: int=3, fg='#333', bg='#FFF', padx: int=8, pady: int=5, font=('Lucida Grande', 16) if sys.platform=='darwin' else ('Calibri', 14), startOpen=True, callback=None):
 		super().__init__(parent=parent, text=text, fg=fg, bg=bg, padx=padx, pady=pady, font=font, startOpen=startOpen)
 		self.bg = bg
 		self.columns = columns
 		self.checks = {}
 		self._index=0
 		self.callback = callback
 
 		for i in range(columns): self.subframe.columnconfigure(i, weight=1)
 		self.buttons['right'].setup('✔︎', self.toggleAll)
 
-	def addCheck(self, var, text, defaultValue=True, desc=None):
+	def addCheck(self, var, text: str, defaultValue: bool=True, desc: bool=None):
+		"""Adds a `textCheck` element to the frame. https://helipad.dev/functions/checkgrid/addcheck/"""
 		if self.callback is not None:
 			def cbWrap(val): self.callback((var, val))
 		else: cbWrap = None
 
 		self.checks[var] = textCheck(self.subframe, text=text, anchor='w', defaultValue=defaultValue, bg=(self.bg, '#419BF9'), desc=desc, callback=cbWrap)
 		self.checks[var].grid(row=int(ceil(len(self.checks)/self.columns)), column=(len(self.checks)-1)%self.columns, sticky='we')
 		return self.checks[var]
@@ -606,17 +610,16 @@
 			for c in self.values(): c.enable()
 	def disable(self, key=None):
 		if key: self.checks[key].disable()
 		else:
 			for c in self.values(): c.disable()
 	def configure(self, state): self.disabled(state=='disabled')
 
-#Replaces PMW.balloon because it's unreliably maintained
-#Modified from https://stackoverflow.com/questions/3221956/how-do-i-display-tooltips-in-tkinter
 class Tooltip:
+	"""Replaces `PMW.balloon` because it's unreliably maintained. Modified from https://stackoverflow.com/questions/3221956/how-do-i-display-tooltips-in-tkinter"""
 	def __init__(self, widget, text, bg='#FFFFEA', pad=(5, 3, 5, 3), waittime=500, wraplength=250, tip_delta=(10, 5)):
 		for v in ['text', 'widget', 'bg', 'pad', 'waittime', 'wraplength', 'tip_delta']: setattr(self, v, locals()[v]) #Populate object with arguments
 		self.widget.bind("<Enter>", self.onEnter)
 		self.widget.bind("<Leave>", self.onLeave)
 		self.widget.bind("<ButtonPress>", self.onLeave)
 		self.id = None
 		self.tw = None
```

### Comparing `helipad-1.5.1/helipad/ipy-styles.css` & `helipad-1.6/helipad/ipy-styles.css`

 * *Files identical despite different names*

### Comparing `helipad-1.5.1/helipad/locales/helipad.pot` & `helipad-1.6/helipad/locales/helipad.pot`

 * *Files 13% similar despite different names*

```diff
@@ -1,382 +1,393 @@
 # Translations template for Helipad
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: 1.4\n"
+"Project-Id-Version: 1.6\n"
 "POT-Creation-Date: 2022-07-16 01:01-0400\n"
-"PO-Revision-Date: 2022-07-16 01:01-0400\n"
+"PO-Revision-Date: 2023-06-15 16:07-0400\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
-#: agent.py:60 agent.py:66 agent.py:72 agent.py:78
+#: agent.py:67 agent.py:73 agent.py:79 agent.py:85
 msgid "{0} {1} does not have sufficient {2} to give {3} {4}."
 msgstr ""
 
-#: agent.py:62 agent.py:68 agent.py:74 agent.py:80
+#: agent.py:69 agent.py:75 agent.py:81 agent.py:87
 msgid " Continuing with available {0} of {1}…"
 msgstr ""
 
-#: agent.py:88 agent.py:144
+#: agent.py:95 agent.py:151
 msgid " Cancelling trade…"
 msgstr ""
 
-#: agent.py:108 agent.py:118
+#: agent.py:114 agent.py:124
 msgid "{} requires a monetary good to be specified."
 msgstr ""
 
-#: agent.py:129 agent.py:135
+#: agent.py:136 agent.py:142
 msgid "{0} {1} does not have sufficient funds to pay {2} {3}."
 msgstr ""
 
-#: agent.py:133 agent.py:138
+#: agent.py:140 agent.py:145
 msgid " Continuing with available balance of {}…"
 msgstr ""
 
-#: agent.py:156
+#: agent.py:164
 msgid "Balance checking requires a monetary good to be specified."
 msgstr ""
 
-#: agent.py:168
+#: agent.py:183
 msgid "Fixed primitives cannot reproduce."
 msgstr ""
 
-#: agent.py:202 data.py:112
+#: agent.py:211 data.py:118
 msgid "Invalid statistic {}."
 msgstr ""
 
-#: agent.py:229
+#: agent.py:236
 msgid "Fixed primitives cannot die."
 msgstr ""
 
-#: agent.py:254 agent.py:263
-msgid "Object must be specified either 'agent' or 'edge'."
+#: agent.py:262 agent.py:267 agent.py:272 agent.py:277
+#: agent.py:283 agent.py:593 agent.py:599 model.py:532
+#: model.py:538 model.py:544 model.py:548 model.py:553
+#: model.py:558 model.py:563 model.py:569 model.py:575
+#: model.py:579 model.py:584
+msgid "{0} is deprecated and has been replaced with {1}."
+msgstr ""
+
+#: agent.py:300
+msgid "Patches cannot rotate."
 msgstr ""
 
-#: agent.py:354
+#: agent.py:370
 msgid "Direction must select one of the agents as an endpoint."
 msgstr ""
 
-#: agent.py:357
+#: agent.py:373
 msgid "Direction must be either int, bool, or agent."
 msgstr ""
 
-#: agent.py:377
+#: agent.py:399
 msgid "Agent {} is not connected to this edge."
 msgstr ""
 
-#: cpanelJupyter.py:134 cpanelTkinter.py:199
-msgid "filename"
+#: agent.py:478
+msgid "{} is a reserved name. Please choose another."
 msgstr ""
 
-#: cpanelJupyter.py:203 cpanelTkinter.py:279
-msgid "Shocks"
+#: agent.py:507
+msgid "Breed must specify which primitive it belongs to."
+msgstr ""
+
+#: agent.py:513
+msgid "Network density must take a value between 0 and 1."
+msgstr ""
+
+#: agent.py:554
+msgid "Breed '{0}' is not registered for the '{1}' primitive."
+msgstr ""
+
+#: agent.py:620
+msgid "{0} '{1}' already defined. Overriding…"
+msgstr ""
+
+#: agent.py:670 agent.py:680
+msgid "Object must be specified either 'agent' or 'edge'."
 msgstr ""
 
-#: cpanelJupyter.py:209
+#: cpanelJupyter.py:154 cpanelTkinter.py:200
+msgid "filename"
+msgstr ""
+
+#: cpanelJupyter.py:229
 msgid ""
 "After setting parameter values, run <code>launchVisual()</code> or "
 "<code>start()</code> to start the model."
 msgstr ""
 
-#: cpanelJupyter.py:236 cpanelJupyter.py:254 cpanelTkinter.py:84
+#: cpanelJupyter.py:256 cpanelJupyter.py:274
+#: cpanelTkinter.py:85
 msgid "Pause"
 msgstr ""
 
-#: cpanelJupyter.py:241 cpanelTkinter.py:88
+#: cpanelJupyter.py:261 cpanelTkinter.py:89
 msgid "Run"
 msgstr ""
 
-#: cpanelJupyter.py:258
+#: cpanelJupyter.py:278
 msgid "Stop"
 msgstr ""
 
-#: cpanelJupyter.py:277
+#: cpanelJupyter.py:298
 msgid ""
 "Model parameters changed, please re-launch the control panel with "
 "launchCpanel()."
 msgstr ""
 
-#: cpanelTkinter.py:20
+#: cpanelTkinter.py:21
 msgid "{}Control Panel"
 msgstr ""
 
-#: cpanelTkinter.py:92
+#: cpanelTkinter.py:93
 msgid "New Model"
 msgstr ""
 
-#: cpanelTkinter.py:517
-msgid "Invalid Checkentry type. Must be either \"string\" or \"int\""
+#: cpanelTkinter.py:522
+msgid "Invalid Checkentry datatype. Must be either \"string\" or \"int\""
 msgstr ""
 
-#: data.py:26
+#: data.py:27
 msgid "Second argument of addReporter must be callable."
 msgstr ""
 
-#: data.py:33
+#: data.py:34
 msgid "removeReporter cannot be called while a model is active."
 msgstr ""
 
-#: data.py:128
+#: data.py:135
 msgid "First argument of Data.getLast() must be either a key name or an int."
 msgstr ""
 
-#: model.py:66
+#: model.py:72
 msgid "Stop on period"
 msgstr ""
 
-#: model.py:67
+#: model.py:73
 msgid "CSV?"
 msgstr ""
 
-#: model.py:68
+#: model.py:74
 msgid "Refresh Every __ Periods"
 msgstr ""
 
-#: model.py:94
+#: model.py:100
 msgid ""
 "A Helipad update is available! Use `pip install -U helipad` to upgrade to"
 " version {}."
 msgstr ""
 
-#: model.py:111
-msgid "Breed must specify which primitive it belongs to."
-msgstr ""
-
-#: model.py:129
+#: model.py:135
 msgid "Visualizations can only be registered on the top-level model."
 msgstr ""
 
-#: model.py:133
+#: model.py:139
 msgid "Visualization class must inherit from BaseVisualization."
 msgstr ""
 
-#: model.py:173
+#: model.py:179
 msgid "Monetary Base"
 msgstr ""
 
-#: model.py:183
+#: model.py:189
 msgid "Utility"
 msgstr ""
 
-#: model.py:189 model.py:773 visualize.py:121
+#: model.py:195 model.py:661 visualize.py:145
 msgid "Demand"
 msgstr ""
 
-#: model.py:212
+#: model.py:217
 msgid "nest_asyncio is required to run Helipad from Spyder."
 msgstr ""
 
-#: model.py:276
+#: model.py:282
 msgid "matchSelect did not return the correct number of agents."
 msgstr ""
 
-#: model.py:330
+#: model.py:336
 msgid "Period {0}: {1} periods/second ({2}% model, {3}% visuals)"
 msgstr ""
 
-#: model.py:383
+#: model.py:397
 msgid ""
 "Can't do a parameter sweep without the value of the 'stopafter' parameter"
 " set."
 msgstr ""
 
-#: model.py:418
-msgid "Network density must take a value between 0 and 1."
-msgstr ""
-
-#: model.py:482
-msgid "Breed '{0}' is not registered for the '{1}' primitive."
-msgstr ""
-
-#: model.py:515
-msgid "Error initializing the debug console. Make sure the `readline` and `code` modules are installed."
+#: model.py:444
+msgid ""
+"Error initializing the debug console. Make sure the `readline` and `code`"
+" modules are installed."
 msgstr ""
 
-#: model.py:549
+#: model.py:448
 msgid "Control panel can only be launched on the top-level model."
 msgstr ""
 
-#: model.py:573
+#: model.py:472
 msgid "Control panel was redrawn in another cell."
 msgstr ""
 
-#: model.py:583
+#: model.py:483
 msgid ""
 "No visualizations available. To run the model with no GUI, use "
 "model.start() instead."
 msgstr ""
 
-#: model.py:586
+#: model.py:486
 msgid ""
 "Running from the control panel with no visualization requires a stop "
 "condition, and either CSV export or a terminate hook."
 msgstr ""
 
-#: model.py:592
+#: model.py:492
 msgid "{}Data Plots"
 msgstr ""
 
-#: model.py:632 model.py:636 model.py:640 model.py:644 model.py:658
-#: model.py:667 model.py:671 model.py:675 model.py:679 model.py:683
-#: model.py:687 model.py:692 model.py:697 model.py:708 model.py:713 param.py:93
-#: param.py:525
-msgid "{0} is deprecated and has been replaced with {1}."
-msgstr ""
-
-#: model.py:650
-msgid "Breed parameter must specify which primitive it belongs to."
-msgstr ""
-
-#: model.py:663
-msgid ""
-"Model.allParams is deprecated. All parameters can be accessed using "
-"model.params."
-msgstr ""
-
-#: model.py:727
-msgid "{0} '{1}' already defined. Overriding…"
-msgstr ""
-
-#: model.py:758
+#: model.py:646
 msgid "Money good already specified as {}. Overriding…"
 msgstr ""
 
-#: model.py:764 visualize.py:122
+#: model.py:652 visualize.py:146
 msgid "Money"
 msgstr ""
 
-#: model.py:801
-msgid "{} is a reserved name. Please choose another."
-msgstr ""
-
-#: param.py:33 param.py:100 param.py:118 param.py:166
+#: param.py:36 param.py:110 param.py:129
+#: param.py:178
 msgid "A {} whose parameter value to set must be specified."
 msgstr ""
 
-#: param.py:79
+#: param.py:93
 msgid "Can't add keys to a global parameter…"
 msgstr ""
 
-#: param.py:272
+#: param.py:286
 msgid "Cannot instantiate per-item checkgrid parameter."
 msgstr ""
 
-#: param.py:318
+#: param.py:335
 msgid "Cannot add checkgrid items after control panel is drawn."
 msgstr ""
 
-#: param.py:347
+#: param.py:366
 msgid "Cannot add checkgrids or per-item parameters to groups."
 msgstr ""
 
-#: param.py:375
+#: param.py:399
 msgid "Cannot remove built-in parameters."
 msgstr ""
 
-#: param.py:396
+#: param.py:421
 msgid "Parameter '{}' already defined. Overriding…"
 msgstr ""
 
-#: param.py:418
+#: param.py:443
 msgid "Per-breed parameter must specify which primitive it belongs to."
 msgstr ""
 
-#: param.py:546
-msgid "randn() argument must be between 0 and 100."
+#: param.py:492
+msgid "Shocks"
 msgstr ""
 
-#: spatial.py:21
-msgid ""
-"Using x and y to set dimensions is deprecated. Use the dim argument "
-"instead."
+#: param.py:579
+msgid "randn() argument must be between 0 and 100."
 msgstr ""
 
 #: spatial.py:25
-msgid ""
-"The `diag` argument is deprecated. Use the `corners` argument instead."
+msgid "The `diag` argument is deprecated. Use the `corners` argument instead."
 msgstr ""
 
-#: spatial.py:40
-msgid "The {0} parameter is deprecated. Use {1} instead."
+#: spatial.py:34
+msgid "Patch number cannot be set directly. Set the dim parameter instead."
 msgstr ""
 
-#: spatial.py:27
-msgid "Map Size"
+#: spatial.py:41 spatial.py:44 spatial.py:48
+#: spatial.py:51
+msgid "The {0} parameter is deprecated. Use {1} instead."
 msgstr ""
 
-#: spatial.py:30 spatial.py:33
+#: spatial.py:54
 msgid "Map Width"
 msgstr ""
 
-#: spatial.py:31 spatial.py:34
+#: spatial.py:55
 msgid "Map Height"
 msgstr ""
 
-#: spatial.py:35
-msgid "Invalid dimension."
+#: spatial.py:56
+msgid "Wrap"
 msgstr ""
 
-#: spatial.py:142
-msgid "Invalid wrap parameter."
+#: spatial.py:65
+msgid "Agent is not on a patch."
 msgstr ""
 
-#: spatial.py:38
-msgid "Square"
+#: spatial.py:98
+msgid "There is no patch at ({0}, {1})."
 msgstr ""
 
-#: spatial.py:39
-msgid "Wrap"
+#: spatial.py:107
+msgid "Dimension is out of range."
 msgstr ""
 
-#: spatial.py:41
-msgid "Patch number cannot be set directly. Set the dim parameter instead."
+#: spatial.py:136
+msgid "Patches cannot move."
 msgstr ""
 
-#: spatial.py:59
-msgid "Patches cannot move."
+#: spatial.py:175 spatial.py:262
+msgid "Invalid wrap parameter."
 msgstr ""
 
-#: agent.py:296
-msgid "Patches cannot rotate."
+#: spatial.py:178
+msgid "Invalid dimension."
 msgstr ""
 
-#: spatial.py:92
-msgid "Dimension is out of range."
+#: spatial.py:308
+msgid "MultiPolygons are not supported as patches. Taking the first polygon…"
+msgstr ""
+
+#: spatial.py:310
+msgid "Patch with name '{0}' already exists."
+msgstr ""
+
+#: spatial.py:321
+msgid "Polygon {0} overlaps existing patch {1}."
 msgstr ""
 
-#: utility.py:26 utility.py:38
+#: utility.py:26 utility.py:35
 msgid "Quantities argument doesn't match initialized list of goods."
 msgstr ""
 
-#: visualize.py:45
+#: visualize.py:44
 msgid "Plots"
 msgstr ""
 
-#: visualize.py:219
+#: visualize.py:133
+msgid ""
+"model.visual.plots is deprecated. Plots can be accessed by indexing the "
+"visualization object directly."
+msgstr ""
+
+#: visualize.py:245 visualize.py:348
 msgid "Cannot remove plots after control panel is drawn."
 msgstr ""
 
-#: visualize.py:225 visualize.py:319
+#: visualize.py:251 visualize.py:354
 msgid "No plot '{}' to remove."
 msgstr ""
 
-#: visualize.py:304
-msgid "'{}' is not a registered plot visualizer."
+#: visualize.py:332
+msgid "The `network` plot type is deprecated. Use `agents` instead."
 msgstr ""
 
-#: visualize.py:309
-msgid "New plot types must subclass ChartPlot."
+#: visualize.py:335
+msgid "'{}' is not a registered plot visualizer."
 msgstr ""
 
-#: visualize.py:313
-msgid "Cannot remove plots after control panel is drawn."
+#: visualize.py:343
+msgid "New plot types must subclass ChartPlot."
 msgstr ""
 
-#: visualize.py:391
+#: visualize.py:430
 msgid ""
 "Reporter '{}' does not exist. Be sure to register reporters before adding"
 " series."
 msgstr ""
 
+#: visualize.py:635
+msgid "The kind= argument is deprecated and has been replaced with network=."
+msgstr ""
+
```

### Comparing `helipad-1.5.1/helipad/model.py` & `helipad-1.6/helipad/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,56 @@
-# ==========
-# Basic model infrastructure
-# Do not run this file; import it and run your file.
-# ==========
+"""
+The main model module. Import and instantiate the `Helipad` class to set up and launch a model. See https://helipad.dev for API documentation.
+"""
 
 import os, sys, warnings, asyncio, time
 import gettext
 from random import shuffle, choice
-from numpy import random
-import pandas
 #from memory_profiler import profile
 
 from helipad.visualize import BaseVisualization, Charts, TimeSeries
 from helipad.helpers import *
 from helipad.param import Params, Shocks
 from helipad.data import Data
-from helipad.agent import Agent, baseAgent
+from helipad.agent import *
 
 class Helipad:
+	"""The main model object. https://helipad.dev/functions/model/"""
 	runInit = True #for multiple inheritance. Has to be a static property
 
-	def __init__(self, locale='en'):
+	def __init__(self, locale: str='en'):
 		#Have to do this first so that i18n is available early.
-		#Put it in an obscure variable and then use helpers.ï() so we don't conflict with the REPL console.
+		#Put it in an obscure variable and then use helpers.ï() so we don't conflict with the REPL console, which overwrites _.
 		if not hasattr(self, 'breed'):
 			import builtins
 			builtins.__dict__['helipad_gettext'] = gettext.translation('helipad', localedir=os.path.realpath(os.path.join(os.getcwd(), os.path.dirname(__file__)))+'/locales', languages=[locale]).gettext
 
+		#Containers
+		self.agents = Agents(self)
 		self.data = Data(self)
 		self.params = Params(self)
 		self.shocks = Shocks(self)
 		self.events = Events()
 		self.hooks = Hooks()
-		self.primitives = Primitives(self)
-		self.goods = Goods(self)				#List of goods
+		self.goods = Goods(self)
 
 		self.name = ''
-		self.agents = {}
 		self.patches = []
 		self.stages = 1
-		self.order = 'linear'
 		self.hasModel = False		#Have we initialized?
 		self.timer = False
 		self.visual = None
 		self.cpanel = None
 
 		self.t = None
 		self.running = False
 		self._cut = False
 
 		#Default parameters
-		self.primitives.add('agent', Agent, dflt=50, low=1, high=100)
+		self.agents.addPrimitive('agent', Agent, dflt=50, low=1, high=100)
 
 		#Decorators
 		def repdec(name, fn, kwargs): self.data.addReporter(name, fn, **kwargs)
 		def hookdec(name, fn, kwargs): self.hooks.add(name, fn, **kwargs)
 		def buttondec(name, fn, kwargs): self.addButton(name, fn, **kwargs)
 		def eventdec(name, fn, kwargs): self.events.add(name, fn, **kwargs)
 		self.reporter = self.genDecorator(repdec)
@@ -103,71 +100,67 @@
 					print(ï('A Helipad update is available! Use `pip install -U helipad` to upgrade to version {}.').format(available[0]))
 			except: pass #Fail silently if we're not online
 
 	def __repr__(self):
 		if self.name: return f'<Helipad: {self.name}>'
 		else: return '<Helipad object>'
 
-	def addButton(self, text, func, desc=None):
+	def addButton(self, text: str, func, desc=None):
+		"""Add a button to the control panel, in the shocks section, that runs `func` when pressed. This method is aliased by the `@model.button` function decorator, which is preferred. https://helipad.dev/functions/model/addbutton/"""
 		self.shocks.add(text, None, func, 'button', True, desc)
 
-	#Get or set a parameter, depending on whether there are two or three arguments
 	def param(self, param, val=None):
+		"""Get or set a model parameter, depending on whether there are two or three arguments. https://helipad.dev/functions/model/param/"""
 		item = param[2] if isinstance(param, tuple) and len(param)>2 else None
 		param = self.params[param[0]] if isinstance(param, tuple) else self.params[param]
 
 		if val is not None: param.set(val, item)
 		else: return param.get(item)
 
-	def addBreed(self, name, color, prim=None):
-		if prim is None:
-			if len(self.primitives) == 1: prim = next(iter(self.primitives.keys()))
-			else: raise KeyError(ï('Breed must specify which primitive it belongs to.'))
-		return self.primitives[prim].breeds.add(name, color)
-
-	#Returns the value of the last function in the list
-	def doHooks(self, place, args):
+	def doHooks(self, place: str, args: list):
+		"""Execute registered hooks at various places in the model and return the value of the last function in the list. https://helipad.dev/functions/model/dohooks/"""
 		#Take a list of hooks; go until we get a response
 		if isinstance(place, list):
 			for f in place:
 				r = self.doHooks(f, args)
 				if r is not None: return r
 			return None
 
 		if not place in self.hooks: return None
 		for f in self.hooks[place]: r = f(*args)
 		return r
 
-	def useVisual(self, viz):
+	def useVisual(self, viz: BaseVisualization):
+		"""Register a visualization class for live model visualization. Visualization classes can be imported from `helipad.visualize`, or custom visualization classes can be subclassed from `BaseVisualization`. The visualization can then be launched later using model.launchVisual(). https://helipad.dev/functions/model/usevisual/"""
 		if hasattr(self, 'breed'):
 			warnings.warn(ï('Visualizations can only be registered on the top-level model.'), None, 2)
 			return #Doesn't matter if it's not the top-level model
 
 		if viz is not None and not issubclass(viz, BaseVisualization):
 			raise RuntimeError(ï('Visualization class must inherit from BaseVisualization.'))
 
 		self.visual = viz(self) if viz is not None else None
 		return self.visual
 
-	#Get ready to actually run the model
 	def setup(self):
+		"""Gather the control panel settings and initialize the model. This function runs when the "New Model" button is pressed, and should not be called by user code. https://helipad.dev/functions/model/setup/"""
 		if self.hasModel: self.terminate()
 		self.doHooks('modelPreSetup', [self])
 		self.t = 0
 
 		#Blank breeds for any primitives not otherwise specified
-		for p in self.primitives.values():
+		for p in self.agents.values():
 			if not p.breeds: p.breeds.add('', '#000000')
 
 		#SERIES AND REPORTERS
 		#Breeds and goods should already be registered at this point
 
 		self.data.reset()
 		for e in self.events.values(): e.reset()
-		defPrim = 'agent' if 'agent' in self.primitives else next(iter(self.primitives))
+		defPrim = 'agent' if 'agent' in self.agents else next(iter(self.agents))
 
 		def pReporter(param, item=None):
 			def reporter(model): return param.get(item)
 			return reporter
 
 		#Add reporters for parameters
 		for n,p in self.params.items():
@@ -178,38 +171,37 @@
 					self.data.addReporter(n+'-'+good, pReporter(p, good))
 			elif p.per == 'breed':
 				for breed in p.pKeys:
 					self.data.addReporter(p.prim+'-'+n+'-'+breed, pReporter(p, breed))
 
 		if self.goods.money is not None:
 			self.data.addReporter('M0', self.data.agentReporter('stocks', 'all', good=self.goods.money, stat='sum'))
-			if self.visual is not None and isinstance(self.visual, TimeSeries) and 'money' in self.visual.plots:
-				self.visual.plots['money'].addSeries('M0', ï('Monetary Base'), self.goods[self.goods.money].color)
+			if self.visual is not None and isinstance(self.visual, TimeSeries) and 'money' in self.visual:
+				self.visual['money'].addSeries('M0', ï('Monetary Base'), self.goods[self.goods.money].color)
 
 		#Unconditional variables to report
 		# self.data.addReporter('utility', self.data.agentReporter('utils', defPrim))
 
 		#Per-breed and per-good series and reporters
 		#Don't put lambda functions in here, or the variable pairs will be reported the same, for some reason.
-		for breed, b in self.primitives[defPrim].breeds.items():
+		for breed, b in self.agents[defPrim].breeds.items():
 			self.data.addReporter('utility-'+breed, self.data.agentReporter('utils', defPrim, breed=breed))
 			if self.visual is not None and self.visual.__class__.__name__=='TimeSeries':
-				self.visual.plots['utility'].addSeries('utility-'+breed, breed.title()+' '+ï('Utility'), b.color)
+				self.visual['utility'].addSeries('utility-'+breed, breed.title()+' '+ï('Utility'), b.color)
 
 		if len(self.goods) >= 2:
 			for good, g in self.goods.nonmonetary.items():
 				self.data.addReporter('demand-'+good, self.data.agentReporter('currentDemand', 'all', good=good, stat='sum'))
 				if self.visual is not None:
-					if 'demand' in self.visual.plots: self.visual.plots['demand'].addSeries('demand-'+good, good.title()+' '+ï('Demand'), g.color)
+					if 'demand' in self.visual: self.visual['demand'].addSeries('demand-'+good, good.title()+' '+ï('Demand'), g.color)
 
 		#Initialize agents
-		self.primitives = dict(sorted(self.primitives.items(), key=lambda d: d[1].priority))				#Sort by priority
-		pops = {prim: self.param('num_'+prim) for prim in self.primitives}
-		for ags in self.agents.values(): ags.clear()														#Clear any surviving agents from last run
-		for prim in self.primitives: self.nUpdater(pops[prim], prim, self, force=True)						#Force is so we can call nupdater before instantiating hasModel
+		for prim, ags in self.agents.items():
+			ags.clear()																	#Clear any surviving agents from last run
+			self.agents.initialize(self.param('num_'+prim), prim, self, force=True)		#Force is so we can call initialize() before instantiating hasModel
 
 		#Start progress bar
 		#Put this here and not in .start() because it'll flash on unpause otherwise
 		if self.cpanel:
 			st = self.param('stopafter')
 			self.cpanel.progress.determinate(st and isinstance(st, int))
 
@@ -223,57 +215,58 @@
 				nest_asyncio.apply()
 			except:
 				raise ImportError(ï('nest_asyncio is required to run Helipad from Spyder.'))
 
 		self.hasModel = True
 		self.doHooks('modelPostSetup', [self])
 
-	def cutStep(self): self._cut = True
+	def cutStep(self):
+		"""When called from inside an `agentStep` or `match` hook, skip stepping the rest of the agents that stage and proceed to the next (or to the next period in single-stage models). https://helipad.dev/functions/model/cutstep/"""
+		self._cut = True
 
-	def step(self, stage=1):
+	def step(self, stage: int=1):
+		"""Step the model, i.e. run through the `step()` functions of all the agents and increment the timer by one. This method is called automatically while the model is running, and should not generally be called in user code. https://helipad.dev/functions/model/step/"""
 		self.t += 1
 		self.doHooks('modelPreStep', [self])
 
 		#Reset per-period variables
 		#Have to do this all at once at the beginning of the period, not when each agent steps
 		for p in self.agents.values():
 			for a in p: a.currentDemand = {g:0 for g in self.goods}
 
 		self.shocks.step()
 
-		def sortFunc(model, stage, func):
+		def sortFunc(model: Helipad, stage: int, func):
 			def sf(agent): return func(agent, model, stage)
 			return sf
 
 		for self.stage in range(1, self.stages+1):
 			self._cut = False
 			self.doHooks('modelStep', [self, self.stage])
 
 			#Sort agents and step them
 			for prim, lst in self.agents.items():
-				order = self.primitives[prim].order or self.order
+				order = lst.order or self.agents.order
 				if isinstance(order, list): order = order[self.stage-1]
-
 				if order == 'random': shuffle(lst)
 
 				#Can't do our regular doHooks() here since we want to pass the function to .sort()
 				#From the user's perspective though, this doesn't matter
 				#Do the more specific sorts last
 				ordhooks = (self.hooks['order'] if 'order' in self.hooks else []) + (self.hooks[prim+'Order'] if prim+'Order' in self.hooks else [])
 				for o in ordhooks: lst.sort(key=sortFunc(self, self.stage, o))
 
-				#Keep the agent list constant for a given loop because modifying it while looping
-				#(e.g. if an agent dies or reproduces) will screw up the looping
-				agentpool = self.agents[prim].copy()
+				#Copy the agent list to keep it constant for a given loop because modifying it
+				#while looping (e.g. if an agent dies or reproduces) will screw up the looping
+				agentpool = list(lst)
 
 				#Matching model
 				if 'match' in order:
-					matchN = order.split('-')
-					matchN = int(matchN[1]) if len(matchN) > 1 else 2
-					matchpool = self.agents[prim].copy()
+					matchN = int(mn[1]) if len(mn := order.split('-')) > 1 else 2
+					matchpool = list(lst)
 					while len(matchpool) > len(agentpool) % matchN and not self._cut:
 						agents = []
 						for a in range(matchN):
 							agent = choice(matchpool)
 							matchpool.remove(agent)
 							agents.append(agent)
 
@@ -319,20 +312,20 @@
 			t = self.step()
 			st = self.param('stopafter')
 
 			if t%self.param('refresh')==0:
 				if self.timer: t2 = time.time()
 				if self.cpanel and st and isinstance(st, int): self.cpanel.progress.update(t/st)
 
-				#Update graph
+				#Update visualizations
 				if self.visual is not None and not self.visual.isNull:
 					await asyncio.sleep(0.001) #Listen for keyboard input
 					data = self.data.getLast(t - self.visual.lastUpdate)
 
-					self.visual.update(data)
+					self.visual.refresh(data)
 					self.visual.lastUpdate = t
 
 					self.doHooks('visualRefresh', [self, self.visual])
 
 				elif self.cpanel:
 					if isNotebook(): await asyncio.sleep(0.001) #Listen for keyboard input
 					else: self.cpanel.update() #Make sure we don't hang the interface if plotless
@@ -351,35 +344,37 @@
 				stop = self.events[st].triggered if isinstance(st, str) else t>=st
 				if stop: self.terminate()
 		if self.timer and isBuffered(): print('\r') #Newline on pause so the output doesn't interfere with the console
 
 	#The *args allows it to be used as an Ipywidgets callback
 	#@profile #To test memory usage
 	def start(self, *args):
-
+		"""Start a model, running `model.setup()` if `model.hasModel` is `False`, and otherwise resuming the existing model. This function is called by `model.launchVisual()`, but does not call it. Use that function to start the model instead if output plots are desired. https://helipad.dev/functions/model/start/"""
 		#Start the progress bar
 		if self.cpanel:
 			self.cpanel.progress.start()
 			self.cpanel.runButton.run()
 
 		self.doHooks('modelStart', [self, self.hasModel])
 		if not self.hasModel: self.setup()
 		self.running = True
 
 		if isNotebook(): asyncio.ensure_future(self.run()) #If Jupyter, it already has an event loop
 		else: asyncio.run(self.run())	#If Tkinter, it needs an event loop
 
 	def stop(self, *args):
+		"""Pause the model, allowing it to be subsequently resumed. https://helipad.dev/functions/model/stop/"""
 		self.running = False
 		if self.cpanel:
 			self.cpanel.progress.stop()
 			self.cpanel.runButton.pause()
 		self.doHooks('modelStop', [self])
 
 	def terminate(self, evt=False):
+		"""Terminate the running model and write the data to disk, if applicable. https://helipad.dev/functions/model/terminate/"""
 		if not self.hasModel: return
 		self.running = False
 		self.hasModel = False
 		if self.visual is not None: self.visual.terminate(self) #Clean up visualizations
 
 		remainder = int(self.t % self.param('refresh')) #For some reason this returns a float sometimes?
 		if remainder > 0 and self.visual is not None and not self.visual.isNull: self.visual.update(self.data.getLast(remainder)) #Last update at the end
@@ -394,14 +389,15 @@
 			if param.type=='checkentry' and param.event: continue
 			if not param.runtime: param.enable()
 
 		self.doHooks('terminate', [self, self.data.dataframe])
 
 	#param is a string (for a global param), a name,object,item,primitive tuple (for per-breed or per-good params), or a list of such
 	def paramSweep(self, param, reporters=None):
+		"""Repeatedly run the model while systematically varying one or more parameter values. Possible values to be swept are specified when the parameter is registered. https://helipad.dev/functions/model/paramsweep/"""
 		if not self.param('stopafter'): raise RuntimeError(ï('Can\'t do a parameter sweep without the value of the \'stopafter\' parameter set.'))
 
 		#Standardize format and get the Param objects
 		if not isinstance(param, list): param = [param]
 		params = {}
 		for p in param:
 			if not isinstance(p, tuple): p = (p,)
@@ -427,177 +423,65 @@
 			else: data = self.data.dataframe
 
 			events = [Item(name=e.name, triggered=e.triggered, data=e.data) for e in self.events.values()]
 
 			alldata.append(Item(vars=run, data=data, events=events))
 		return alldata
 
-	#Creates an unweighted and undirected network of a certain density
-	def createNetwork(self, density, kind='edge', prim=None):
-		if density < 0 or density > 1: raise ValueError(ï('Network density must take a value between 0 and 1.'))
-		from itertools import combinations
-		agents = self.allagents.values() if prim is None else self.agents[prim]
-		for c in combinations(agents, 2):
-			if random.randint(0,100) < density*100:
-				c[0].newEdge(c[1], kind)
-		return self.network(kind, prim)
-
-	def network(self, kind='edge', prim=None, excludePatches=False):
-		import networkx as nx
-
-		#Have to use DiGraph in order to draw any arrows
-		G = nx.DiGraph(name=kind)
-		agents = list(self.allagents.values()) if prim is None else self.agents[prim]
-		if excludePatches: agents = [a for a in agents if a.primitive!='patch']
-		G.add_nodes_from([(a.id, {'breed': a.breed, 'primitive': a.primitive, 'position': None if a.position is None else a.position.copy()}) for a in agents])
-		ae = self.allEdges
-		if kind in ae:
-			for e in ae[kind]:
-				if prim is None or (e.vertices[0].primitive==prim and e.vertices[1].primitive==prim): G.add_edge(
-					e.startpoint.id if e.directed else e.vertices[0].id,
-					e.endpoint.id if e.directed else e.vertices[1].id,
-					weight=e.weight, directed=e.directed
-				)
-		return G
-
-	@property
-	def allEdges(self):
-		es = {}
-		for a in self.allagents.values():
-			for e in a.alledges:
-				if not e.kind in es: es[e.kind] = []
-				if not e in es[e.kind]: es[e.kind].append(e)
-		return es
-
 	def spatial(self, *args, **kwargs):
 		from helipad.spatial import spatialSetup
 		return spatialSetup(self, *args, **kwargs)
 
-	@property
-	def allagents(self):
-		agents = {}
-		for l in self.agents.values():
-			agents.update({a.id:a for a in l})
-		return agents
-
-	#CALLBACK FOR DEFAULT PARAMETERS
-	#Model param redundant, strictly speaking, but it's necessary to make the signature match the setter callback
-	def nUpdater(self, val, prim, model, force=False):
-		if not self.hasModel and not force: return val
-
-		if 'num_' in prim: prim = prim.split('_')[1] #Because the parameter callback passes num_{prim}
-		array = self.agents[prim]
-		diff = val - len(array)
-
-		#Add agents
-		if diff > 0:
-			ids = [a.id for a in self.allagents.values()]
-			maxid = max(ids) if ids else 0 #Figure out maximum existing ID
-			for aId in range(maxid+1, maxid+int(diff)+1):
-				breed = self.doHooks([prim+'DecideBreed', 'decideBreed'], [aId, self.primitives[prim].breeds.keys(), self])
-				if breed is None: breed = list(self.primitives[prim].breeds.keys())[aId%len(self.primitives[prim].breeds)]
-				if not breed in self.primitives[prim].breeds:
-					raise ValueError(ï('Breed \'{0}\' is not registered for the \'{1}\' primitive.').format(breed, prim))
-				new = self.primitives[prim].class_(breed, aId, self)
-				array.append(new)
-
-		#Remove agents
-		elif diff < 0:
-			shuffle(array) #Delete agents at random
-
-			#Remove agents, maintaining the proportion between breeds
-			n = {x: 0 for x in self.primitives[prim].breeds.keys()}
-			for a in self.agents[prim]:
-				if n[a.breed] < -diff:
-					n[a.breed] += 1
-					a.die(updateGUI=False)
-				else: continue
-
-	#
-	# DEBUG FUNCTIONS
-	# Only call from the console, not in user code
-	#
-
-	# Requires to be run from Terminal (⌘-⇧-R in TextMate). `self` will refer to the model object
-	# Readline doesn't look like it's doing anything here, but it enables certain console features
 	# Only works on Mac. Also Gnureadline borks everything, so don't install that.
 	# Has to be called *after* Cpanel.__init__() is called, or the cpanel object won't be available.
 	def debugConsole(self):
+		"""Launch a REPL console to interact with the model after launch. Requires to be run in a buffered console. `self` will refer to the model object."""
 		if sys.platform=='darwin' and isBuffered():
 			try:
-				import code, readline
+				import code, readline # Readline doesn't look like it's doing anything here, but it enables certain console features
 				env = globals().copy()
 				env['self'] = self
 				code.interact(local=env)
 			except ModuleNotFoundError: print(ï('Error initializing the debug console. Make sure the `readline` and `code` modules are installed.'))
 
-	#Return agents of a breed if string; return specific agent with ID otherwise
-	def agent(self, var, primitive=None):
-		if primitive is None:
-			primitive = 'agent' if 'agent' in self.primitives else next(iter(self.primitives))
-		if isinstance(var, str):
-			return [a for a in self.agents[primitive] if a.breed==var]
-		else:
-			aa = self.allagents
-			return aa[var] if var in aa else None
-
-		return None #If nobody matched
-
-	#Returns summary statistics on an agent variable at a single point in time
-	def summary(self, var, prim=None, breed=None, good=False):
-		if prim is None:
-			prim = 'agent' if 'agent' in self.primitives else next(iter(self.primitives))
-		agents = self.agents[prim] if breed is None else self.agent(breed, prim)
-		if not good: data = pandas.Series([getattr(a, var) for a in agents]) #Pandas gives us nice statistical functions
-		else: data = pandas.Series([a.stocks[var] for a in agents])
-		stats = {
-			'n': data.size,
-			'Mean': data.mean(),
-			'StDev': data.std(),
-			'Variance': data.var(),
-			'Maximum': data.max(),
-			'Minimum': data.min(),
-			'Sum': data.sum()
-		}
-		for k, v in stats.items():
-			print(k+': ', v)
-
-	def launchCpanel(self):
+	def launchCpanel(self, console: bool=True):
+		"""Launch the control panel, either in a Tkinter or a Jupyter environment, as appropriate. https://helipad.dev/functions/model/launchcpanel/"""
 		if hasattr(self, 'breed'): warnings.warn(ï('Control panel can only be launched on the top-level model.'), None, 2)
 
 		self.doHooks('CpanelPreLaunch', [self])
 
 		#Set our agents slider to be a multiple of how many agent types there are
 		#Do this down here so we can have breeds registered before determining options
-		for k,p in self.primitives.items():
+		for k,p in self.agents.items():
 			if self.params['num_'+k].type != 'hidden':
 				l = len(p.breeds)
 				if not l: continue
 				self.params['num_'+k].opts['low'] = makeDivisible(self.params['num_'+k].opts['low'], l, 'max')
 				self.params['num_'+k].opts['high'] = makeDivisible(self.params['num_'+k].opts['high'], l, 'max')
 				self.params['num_'+k].opts['step'] = makeDivisible(self.params['num_'+k].opts['low'], l, 'max')
 				self.params['num_'+k].value = makeDivisible(self.params['num_'+k].value, l, 'max')
 				self.params['num_'+k].default = makeDivisible(self.params['num_'+k].default, l, 'max')
 
 		if not isNotebook():
 			from helipad.cpanelTkinter import Cpanel
 			self.cpanel = Cpanel(self)
 			self.doHooks('CpanelPostInit', [self.cpanel]) #Want the cpanel property to be available here, so don't put in cpanel.py
-			self.debugConsole()
+			if console: self.debugConsole()
 			self.cpanel.mainloop()		#Launch the control panel
 		else:
 			from helipad.cpanelJupyter import Cpanel, SilentExit
 			if self.cpanel: self.cpanel.invalidate(ï('Control panel was redrawn in another cell.'))
 			self.cpanel = Cpanel(self)
 			self.doHooks('CpanelPostInit', [self.cpanel])
 			raise SilentExit() #Don't blow past the cpanel if doing "run all"
 
 		self.doHooks('GUIClose', [self]) #This only executes after all GUI elements have closed
 
 	def launchVisual(self):
+		"""Launch the visualization window from the class registered in `model.useVisual()`, and start the model. https://helipad.dev/functions/model/launchvisual/"""
 		if self.visual is None or self.visual.isNull:
 			if not self.cpanel:
 				print(ï('No visualizations available. To run the model with no GUI, use model.start() instead.'))
 				return
 			if not self.param('stopafter') or not (self.param('csv') or 'terminate' in self.hooks):
 				print(ï('Running from the control panel with no visualization requires a stop condition, and either CSV export or a terminate hook.'))
 				return
@@ -619,266 +503,184 @@
 			root.after(1, self.start)
 			self.debugConsole()
 			root.mainloop()
 		else: self.start() #As long as we haven't already started
 
 	# Generates function decorators for hooks, reporters, etc.
 	def genDecorator(self, todo):
+		"""Return a function which can either serve as a decorator itself or return another decorator function, for use in various decorators (`@model.hook`, `@model.reporter`, and `@model.button`). https://helipad.dev/functions/model/gendecorator/"""
 		def dec(name=None, **kwargs):
 			if callable(name): func, name, isDec = (name, None, True)
 			else: isDec = False
 
 			#Is a decorator
 			def rep1(fn):
 				namn = name #If I do anything with name here, Python throws UnboundLocalError. Possibly a Python bug?
 				if namn is None: namn=fn.__name__
 				todo(namn, fn, kwargs)
 				return fn
 
 			return rep1(func) if isDec else rep1
 		return dec
 
-	#===================
-	# DEPRECATED METHODS
-	#===================
-
-	# DEPRECATED IN HELIPAD 1.4; REMOVE IN HELIPAD 1.6
-
-	def addEvent(self, name, fn, **kwargs):
-		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('Model.addEvent()', 'model.events.add()'), FutureWarning, 2)
-		return self.events.add(name, fn, **kwargs)
-
-	def removeEvent(self, name):
-		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('Model.removeEvent()', 'model.events.remove()'), FutureWarning, 2)
-		return self.events.remove(name)
-
-	def clearEvents(self):
-		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('Model.clearEvents()', 'model.events.clear()'), FutureWarning, 2)
-		self.events.clear()
-
-	def addParameter(self, *args, **kwargs):
-		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('Model.addParameter()', 'model.params.add()'), FutureWarning, 2)
-		return self.params.add(*args, **kwargs)
-
-	def addBreedParam(self, name, title, type, dflt, opts={}, prim=None, runtime=True, callback=None, desc=None, getter=None, setter=None):
-		if prim is None:
-			if len(self.primitives) == 1: prim = next(iter(self.primitives.keys()))
-			else: raise KeyError(ï('Breed parameter must specify which primitive it belongs to.'))
-		return self.addParameter(name, title, type, dflt, opts, runtime, callback, 'breed', desc, prim=prim, getter=getter, setter=setter)
-
-	def addGoodParam(self, name, title, type, dflt, opts={}, runtime=True, callback=None, desc=None, getter=None, setter=None):
-		return self.addParameter(name, title, type, dflt, opts, runtime, callback, 'good', desc, getter=getter, setter=setter)
+	#
+	#Deprecated in 1.6, remove in 1.8
+	#
 
 	@property
-	def goodParams(self):
-		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('Model.goodParams', 'model.params.perGood'), FutureWarning, 2)
-		return self.params.perGood
+	def allagents(self):
+		"""A list of all agents. This property is deprecated; use `model.agents.all` instead."""
+		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('model.allagents', 'model.agents.all'), FutureWarning, 2)
+		return self.agents.all
 
 	@property
-	def allParams(self):
-		warnings.warn(ï('Model.allParams is deprecated. All parameters can be accessed using model.params.'), FutureWarning, 2)
-		return self.params.values()
-
-	def addHook(self, place, func, prioritize=False):
-		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('Model.addHook()', 'model.hooks.add()'), FutureWarning, 2)
-		return self.hooks.add(place, func, prioritize)
-
-	def removeHook(self, place, fname, removeall=False):
-		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('Model.removeHook()', 'model.hooks.remove()'), FutureWarning, 2)
-		return self.hooks.remove(place, fname, removeall=False)
-
-	def clearHooks(self, place):
-		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('Model.clearHooks()', 'model.hooks.clear()'), FutureWarning, 2)
-		return self.hooks.remove(place)
-
-	def addPrimitive(self, *args, **kwargs):
-		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('Model.addPrimitive()', 'model.primitives.add()'), FutureWarning, 2)
-		return self.primitives.add(*args, **kwargs)
-
-	def removePrimitive(self, name):
-		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('Model.removePrimitive()', 'model.primitives.remove()'), FutureWarning, 2)
-		return self.primitives.remove(name)
-
-	def addGood(self, *args, **kwargs):
-		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('Model.addGood()', 'model.goods.add()'), FutureWarning, 2)
-		return self.goods.add(*args, **kwargs)
+	def primitives(self):
+		"""A list of primitive data. This property is deprecated; use `model.agents` instead."""
+		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('model.primitives', 'model.agents'), FutureWarning, 2)
+		return self.agents
 
 	@property
-	def moneyGood(self):
-		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('Model.moneyGood', 'model.goods.money'), FutureWarning, 2)
-		return self.goods.money
+	def order(self):
+		"""The order in which to step agents. This property is deprecated; use `model.agents.order` instead."""
+		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('model.order', 'model.agents.order'), FutureWarning, 2)
+		return self.agents.order
+	@order.setter
+	def order(self, val):
+		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('model.order', 'model.agents.order'), FutureWarning, 2)
+		self.agents.order = val
+
+	def addBreed(self, name, color, prim=None):
+		"""Add a breed to a given primitive. This method is deprecated; use `model.agents.addBreed()` instead."""
+		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('model.addBreed', 'model.agents.addBreed'), FutureWarning, 2)
+		return self.agents.addBreed(name, color, prim)
+
+	def createNetwork(self, density, kind='edge', prim=None):
+		"""Create a network of a given density among agents. This method is deprecated; use `model.agents.createNetwork()` instead."""
+		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('model.createNetwork', 'model.agents.createNetwork'), FutureWarning, 2)
+		return self.agents.createNetwork(density, kind, prim)
+
+	def network(self, kind='edge', prim=None, excludePatches=False):
+		"""Return the network structure of a set of agents. This method is deprecated; use `model.agents.network()` instead."""
+		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('model.network', 'model.agents.network'), FutureWarning, 2)
+		return self.agents.network(kind, prim, excludePatches)
 
 	@property
-	def nonMoneyGoods(self):
-		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('Model.nonMoneyGoods()', 'model.goods.nonmonetary'), FutureWarning, 2)
-		return self.goods.nonmonetary
+	def allEdges(self):
+		"""A `dict` of all network edges between agents, organized by kind. This property is deprecated; use `model.agents.edges` instead."""
+		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('model.allEdges', 'model.agents.edges'), FutureWarning, 2)
+		return self.agents.edges._dict
+
+	def agent(self, var, primitive=None):
+		"""Retrieve an agent by ID or breed. This method is deprecated; use `model.agents[primitive][breed]` or `model.agents[id]` instead."""
+		if isinstance(var, str):
+			warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('model.agent(breed)', 'model.agents[primitive][breed]'), FutureWarning, 2)
+			if primitive is None: primitive = next(iter(self.agents))
+			return self.agents[primitive][var]
+		else:
+			warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('model.agent(id)', 'model.agents[id]'), FutureWarning, 2)
+			return self.agents[var]
+
+	def summary(self, var, prim=None, breed=None, good=False):
+		"""Print summary statistics on an agent property. This method is deprecated; use `model.agents.summary()` instead."""
+		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('model.summary()', 'model.agents.summary()'), FutureWarning, 2)
+		return self.agents.summary(var, prim, breed, good)
 
 class MultiLevel(baseAgent, Helipad):
+	"""A class allowing multi-level agent-based models to be constructed, where the agents at one level are themselves full models with sub-agents. Inherits from both `baseAgent` and `Helipad`. https://helipad.dev/functions/multilevel/"""
 	def __init__(self, breed, id, parentModel):
 		super().__init__(breed, id, parentModel)
 		self.setup()
 
-	#Deprecated in Helipad 1.4; remove in Helipad 1.6
-	@property
-	def dontStepAgents(self):
-		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('MultiLevel.dontStepAgents', 'MultiLevel.cutStep()'), FutureWarning, 2)
-		return self._cut
-
-	@dontStepAgents.setter
-	def dontStepAgents(self, val):
-		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('MultiLevel.dontStepAgents', 'MultiLevel.cutStep()'), FutureWarning, 2)
-		self._cut = val
-
 #==================
 # CONTAINER CLASSES
 #==================
 
-#For adding breeds and goods. Should not be called directly
-class gandb(funcStore):
-	def __init__(self, model):
-		self.model = model
-
-	def add(self, obj, name, color, prim=None, **kwargs):
-		if name in self:
-			warnings.warn(ï('{0} \'{1}\' already defined. Overriding…').format(obj, name), None, 2)
-
-		cobj = color if isinstance(color, Color) else Color(color)
-		cobj2 = cobj.lighten()
-		self[name] = Item(color=cobj, color2=cobj2, **kwargs)
-
-		#Make sure the parameter lists keep up with our items
-		if obj=='good': paramDict = self.model.params.perGood
-		elif obj=='breed': paramDict = {k:v for k,v in self.model.params.perBreed.items() if v.prim==self.primitive}
-		for p in paramDict.values(): p.addKey(name)
-
-		return self[name]
-
-	def remove(self, name):
-		if isinstance(name, (list, tuple)): return [self.remove(n) for n in name]
-		if not name in self: return False
-
-		#Also delete per-item parameters
-		pdict = self.model.params.perBreed if isinstance(self, Breeds) else self.model.params.perGood
-		for param in pdict.values():
-			del param.value[name]
-			if getattr(param, 'elements', False):
-				if not isNotebook(): param.elements[name].destroy()
-				else: param.elements[name].close()
-				del param.elements[name]
-		return super().remove(name)
-
-class Goods(gandb):
-	def add(self, name, color, endowment=None, money=False, props={}):
-		if money:
-			if self.money is not None:
-				print(ï('Money good already specified as {}. Overriding…').format(self.money))
-				self[self.money].money = False
-
-			#Add the M0 plot once we have a money good, only if we haven't done it before
-			elif (self.model.visual is None or self.model.visual.isNull) and hasattr(self.model.visual, 'plots'):
-				try:
-					if not 'money' in self.model.visual.plots: self.model.visual.addPlot('money', ï('Money'), selected=False)
-				except: pass #Can't add plot if re-drawing the cpanel
-
-		props['quantity'] = endowment
-		item = super().add('good', name, color, money=money, props=props)
-
-		#Add demand plot once we have at least 2 goods
-		if len(self) == 2 and (self.model.visual is None or self.model.visual.isNull) and hasattr(self.model.visual, 'plots'):
-			try:
-				if not 'demand' in self.model.visual.plots: self.model.visual.addPlot('demand', ï('Demand'), selected=False)
-			except: pass
-
-		return item
-
-	@property
-	def money(self):
-		for name,good in self.items():
-			if good.money: return name
-		return None
-
-	@property
-	def nonmonetary(self):
-		return {k:v for k,v in self.items() if not v.money}
-
-class Breeds(gandb):
-	def __init__(self, model, primitive):
-		self.primitive = primitive
-		super().__init__(model)
-
-	def add(self, name, color): return super().add('breed', name, color)
-
-class Primitives(funcStore):
-	def __init__(self, model):
-		self.model = model
-		super().__init__()
-
-	def add(self, name, class_, plural=None, dflt=50, low=1, high=100, step=1, hidden=False, priority=100, order=None):
-		if name=='all': raise ValueError(ï('{} is a reserved name. Please choose another.').format(name))
-		if not plural: plural = name+'s'
-		class_.primitive = name
-		self[name] = Item(
-			class_=class_,
-			plural=plural,
-			priority=priority,
-			order=order,
-			breeds=Breeds(self.model, name)
-		)
-		def popget(name, model):
-			prim = name.split('_')[1]
-			if not model.hasModel: return None
-			else: return len(model.agents[prim])
-
-		self.model.params.add('num_'+name, 'Number of '+plural.title(), 'hidden' if hidden else 'slider', dflt=dflt, opts={'low': low, 'high': high, 'step': step} if not hidden else None, setter=self.model.nUpdater, getter=popget)
-		self.model.agents[name] = []
-
-	def remove(self, name):
-		val = super().remove(name)
-		if val:
-			del self.model.agents[name]
-			del self.model.params['num_'+name]
-		return val
-
 class Events(funcStore):
+	"""Interface to add and store events that can trigger during a model on a certain user-defined criterion. https://helipad.dev/functions/events/"""
 	def __init__(self):
 		super().__init__()
 		class Event:
-			def __init__(self, name, trigger, repeat=False, **kwargs):
+			"""An event triggers on a certain user-defined criterion. When triggered, an event stores the data output at that time and registers on the visualizer. This class should not be instantiated directly; use Events.add() or the @model.event decorator instead. https://helipad.dev/functions/event/"""
+			def __init__(self, name: str, trigger, repeat: bool=False, **kwargs):
 				self.name = name
 				self.trigger = trigger
 				self.repeat = repeat
 				self.kwargs = kwargs
 				self.data = []
 				self.triggered = []
 				self.reset()
 
-			def check(self, model):
+			def check(self, model: Helipad) -> bool:
+				"""Run the user-defined event function to determine whether the event is triggered, and record the model state if so. If `Event.repeat==False`, return `False` so long as `Event.trigger` returns `False`, `True` the first time `Event.trigger` returns `True`, and `False` thereafter. If `Event.repeat==True`, return `True` whenever `Event.trigger` returns `True`. https://helipad.dev/functions/event/check/"""
 				if self.triggered and not self.repeat: return False
 				if (isinstance(self.trigger, int) and model.t==self.trigger) or (callable(self.trigger) and self.trigger(model)):
 					data = {k: v[0] for k,v in model.data.getLast(1).items()}
 					if self.repeat:
 						self.data.append(data)
 						self.triggered.append(model.t)
 					else:
 						self.data = data
 						self.triggered = model.t
 					return True
 
 			def reset(self):
+				"""Clear `Event.data` and set `Event.triggered` to `False`. https://helipad.dev/functions/event/reset/"""
 				if self.repeat:
 					self.data.clear()
 					self.triggered.clear()
 				else:
 					self.data = None
 					self.triggered = False
 		self.Event = Event
 
-	def add(self, name, function, **kwargs):
+	def add(self, name: str, function, **kwargs):
+		"""Register an Event. When triggered, an event stores the data output at that time and registers on the visualizer. https://helipad.dev/functions/events/add/"""
 		return super().add(name, self.Event(name, function, **kwargs))
 
+class Goods(gandb):
+	"""Interface to add and store goods that agents can own. Stored in `model.goods`. https://helipad.dev/functions/goods/"""
+	def add(self, name: str, color, endowment=None, money: bool=False, props=None):
+		"""Register a good that agents can carry or trade. Agents keep track of stocks of the good in `agent.stocks`. Quantities of a good can then be accessed with `agent.stocks[good]`, and properties of the good with a two-argument index, e.g. `agent.stocks[good, 'property']`. https://helipad.dev/functions/goods/add/"""
+		if not props: props = {}
+		if money:
+			if self.money is not None:
+				print(ï('Money good already specified as {}. Overriding…').format(self.money))
+				self[self.money].money = False
+
+			#Add the M0 plot once we have a money good, only if we haven't done it before
+			elif (self.model.visual is None or self.model.visual.isNull) and hasattr(self.model.visual, 'plots'):
+				try:
+					if not 'money' in self.model.visual: self.model.visual.addPlot('money', ï('Money'), selected=False)
+				except: pass #Can't add plot if re-drawing the cpanel
+
+		props['quantity'] = endowment
+		item = super().add('good', name, color, money=money, props=props)
+
+		#Add demand plot once we have at least 2 goods
+		if len(self) == 2 and (self.model.visual is None or self.model.visual.isNull) and hasattr(self.model.visual, 'plots'):
+			try:
+				if not 'demand' in self.model.visual: self.model.visual.addPlot('demand', ï('Demand'), selected=False)
+			except: pass
+
+		return item
+
+	@property
+	def money(self):
+		"""The name of the good serving as a numeraire. This property is set by the `money` parameter of `Goods.add()`. https://helipad.dev/functions/goods/#money"""
+		for name,good in self.items():
+			if good.money: return name
+		return None
+
+	@property
+	def nonmonetary(self) -> dict:
+		"""The subset of goods minus the money good. https://helipad.dev/functions/goods/#nonmonetary"""
+		return {k:v for k,v in self.items() if not v.money}
+
 class Hooks(funcStore):
-	multi = True
+	"""Interface to add and store hooks, allowing user-defined code to be inserted into the model. https://helipad.dev/functions/hooks/"""
+	multi: bool = True
 
-	def add(self, name, function, prioritize=False):
+	def add(self, name: str, function, prioritize: bool=False):
+		"""Inserts a function into designated places in the model’s logic. See the Hooks Reference (https://helipad.dev/glossary/hooks/) for a complete list of possible hooks and the function signatures necessary to use them. This method is aliased by the `@model.hook` function decorator, which is the preferred way to hook functions. https://helipad.dev/functions/hooks/add/"""
 		if not name in self: self[name] = []
 		if prioritize: self[name].insert(0, function)
 		else: self[name].append(function)
```

### Comparing `helipad-1.5.1/helipad/param.py` & `helipad-1.6/helipad/param.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,106 +1,113 @@
-# ==========
-# Classes to abstract the interface between model parameters and GUI elements.
-# Do not run this file; import model.py and run from your file.
-# ==========
+"""
+Classes to abstract the interface between model parameters and GUI elements. This module should not be imported directly; use `model.params.add()` instead.
+"""
 
 from itertools import combinations
 import warnings
 from helipad.helpers import *
 from numpy import arange, random
 
 class Param(Item):
+	"""Base class defining a model parameter that can be set before or during runtime. https://helipad.dev/functions/param/"""
 	def __init__(self, **kwargs):
 		super().__init__(**kwargs)
 		if not hasattr(self, 'per'): self.per=None
 		if not hasattr(self, 'value'): self.value = {b:self.defaultVal for b in kwargs['pKeys']} if self.per else self.defaultVal
 		self.element = None
 		self.reset() #Populate with default values
 
 	def __repr__(self): return f'<{self.__class__.__name__}: {self.name}>'
 
-	#Set values from defaults
 	#Global generic:				int → int
 	#Per-breed universal generic:	int → dict{int}
 	#Per-breed specific generic:	dict{int} → dict{int}
 	def reset(self):
+		"""Reset the parameter to its default value. https://helipad.dev/functions/param/reset/"""
 		if self.per is None: self.setSpecific(self.default)
 		else:
 			if isinstance(self.default, dict):
 				for i in self.pKeys:
 					self.setSpecific(self.default[i] if i in self.default else self.defaultVal, i)
 			else:
 				for i in self.pKeys: self.setSpecific(self.default, i)
 
-	#Common code for the set methods
-	def setParent(self, val, item=None, updateGUI=True):
+	def setParent(self, val, item=None, updateGUI: bool=True):
+		"""Common code for subclasses' `set()` methods."""
 		if self.per is not None and item is None: raise KeyError(ï('A {} whose parameter value to set must be specified.').format(self.per))
 
 		#Jupyter requires an explicit update for all parameter types.
 		if updateGUI and isNotebook() and self.element is not None:
 			if self.per is None: self.element.children[0].value = val
 			else: self.elements[item].children[0].value = val
 
 	#Don't override this one
-	def set(self, val, item=None, updateGUI=True):
+	def set(self, val, item=None, updateGUI: bool=True):
+		"""Set the value of the parameter to `val`. Do not call directly; use `model.param()` instead. https://helipad.dev/functions/param/set/"""
 		if getattr(self, 'setter', False):
 			val = self.setter(val, item)
 			if val is not None: self.setSpecific(val, item)
 		else: self.setSpecific(val, item, updateGUI)
 
-	#A generic set method to be overridden
-	def setSpecific(self, val, item=None, updateGUI=True):
+	def setSpecific(self, val, item=None, updateGUI: bool=True):
+		"""A generic set method to be overridden by subclasses."""
 		self.setParent(val, item, updateGUI)
 		if self.per is None: self.value = val
 		else: self.value[item] = val
 
 	#Don't override this one
 	def get(self, item=None):
+		"""Retrieve the value of the parameter. Do not call directly; use `model.param()` instead. https://helipad.dev/functions/param/get/"""
 		if getattr(self, 'getter', False):
 			v = self.getter(item)
 			if v is not None: return v #Allow passing to the default getter
 		return self.getSpecific(item)
 
 	def getSpecific(self, item=None):
+		"""A generic get method to be overridden by subclasses."""
 		return self.value if self.per is None or item is None else self.value[item]
 
-	def disabled(self, disable):
+	def disabled(self, disable: bool):
+		"""Enables or disables the parameter's GUI element. https://helipad.dev/functions/param/disabled/"""
 		if self.element is None: return
 		for e in ([self.element] if self.per is None else self.elements.values()):
 			if isNotebook():
 				for i in e.children: i.disabled = disable
 			else:
 				e.configure(state='disabled' if disable else 'normal')
 
-	def disable(self): self.disabled(True)
-	def enable(self): self.disabled(False)
+	def disable(self):
+		"""Disables the parameter's control panel GUI element so that it cannot be interacted with or changed by the user. https://helipad.dev/functions/param/disable/"""
+		self.disabled(True)
+	def enable(self):
+		"""Enables the parameter's control panel GUI element so that it can be interacted with by the user. https://helipad.dev/functions/param/enable/"""
+		self.disabled(False)
 
 	@property
-	def range(self): return None
+	def range(self):
+		"""A list of possible values that the parameter can take."""
+		return None
 
 	#If a breed or good gets added after the parameter instantiation, we want to be able to keep up
-	def addKey(self, key):
+	def addKey(self, key: str):
+		"""Update a per-item parameter with a new item and assign it the default value specified at the `Param` object's instantiation. https://helipad.dev/functions/param/addkey/"""
 		if self.per is None: warnings.warn(ï('Can\'t add keys to a global parameter…'), None, 2)
 		elif not isinstance(self.default, dict):
 			self.value[key] = self.default
 		elif key in self.default:
 			self.value[key] = self.default[key]	#Forgive out-of-order specification
 		else: return True
 
-	#If there's no user-specified default value, this is what gets returned
 	@property
-	def defaultVal(self): return None
-
-	#Deprecated in Helipad 1.4, remove in Helipad 1.6
-	@property
-	def obj(self):
-		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('Param.obj', 'Param.per'), FutureWarning, 2)
-		return self.per
+	def defaultVal(self):
+		"""Fallback value in case `param.default` is not specified on init."""
+		return None
 
 class MenuParam(Param):
+	"""A parameter type that takes discrete string values. https://helipad.dev/functions/param/"""
 	type = 'menu'
 
 	def setParent(self, val, item=None, updateGUI=True):
 		if self.per is not None and item is None: raise KeyError(ï('A {} whose parameter value to set must be specified.').format(self.per))
 		if updateGUI and not isNotebook() and self.element is not None:
 			sv = self.element if self.per is None else self.elements[item]
 			sv.StringVar.set(self.opts[val]) #Saved the StringVar here
@@ -110,31 +117,33 @@
 	def range(self): return self.opts.keys()
 
 	#Choose first item of the list
 	@property
 	def defaultVal(self): return next(iter(self.opts))
 
 class CheckParam(Param):
+	"""A parameter type that takes a boolean value. https://helipad.dev/functions/param/"""
 	defaultVal = False
 	type='check'
 
-	def setParent(self, val, item=None, updateGUI=True):
+	def setParent(self, val: bool, item=None, updateGUI: bool=True):
 		if self.per is not None and item is None: raise KeyError(ï('A {} whose parameter value to set must be specified.').format(self.per))
 		if updateGUI and not isNotebook() and self.element is not None:
 			sv = self.element if self.per is None else self.elements[item]
 			sv.BooleanVar.set(val) #Saved the BooleanVar here
 		else: super().setParent(val, item, updateGUI)
 
 	@property
 	def range(self): return [False, True]
 
 class SliderParam(Param):
+	"""A parameter type that takes numerical values. https://helipad.dev/functions/param/"""
 	type='slider'
 
-	def setSpecific(self, val, item=None, updateGUI=True):
+	def setSpecific(self, val, item=None, updateGUI: bool=True):
 		#If we're receiving a value from a Jupyter logslider, it's an index and not a value
 		if not updateGUI and isNotebook() and isinstance(self.opts, list): val = self.opts[val]
 
 		self.setParent(val, item, updateGUI)
 		super().setSpecific(val, item, updateGUI)
 
 		#Because the slider tkinter widget doesn't use a Var() object like the others, we have
@@ -148,28 +157,28 @@
 		#Have sliders with an int step value return an int
 		if self.opts is not None and 'step' in self.opts and isinstance(self.opts['step'], int):
 			if isinstance(v, dict): v = {k: int(val) for k,val in v.items()}
 			else: v = int(v)
 		return v
 
 	@property
-	def range(self):
+	def range(self) -> list:
 		values = arange(self.opts['low'], self.opts['high'], self.opts['step']).tolist()
 		values.append(self.opts['high']) #arange doesn't include the high
 		return values
 
-	def addKey(self, key):
+	def addKey(self, key: str):
 		if super().addKey(key) is None: return
 		self.value[key] = 0
 
 	@property
 	def defaultVal(self): return self.opts['low'] if isinstance(self.opts, dict) else self.opts[0]
 
 	#Override in order to update log slider
-	def setParent(self, val, item=None, updateGUI=True):
+	def setParent(self, val, item=None, updateGUI: bool=True):
 		if self.per is not None and item is None: raise KeyError(ï('A {} whose parameter value to set must be specified.').format(self.per))
 
 		if isNotebook() and self.element is not None and (self.per is None or item in self.elements):
 			el = self.element if self.per is None else self.elements[item]
 
 			#Regular slider update
 			if updateGUI and isinstance(self.opts, dict): el.children[0].value = val
@@ -177,14 +186,15 @@
 			#If it's a log slider in Jupyter, update the label, even if we're receiving from the GUI
 			#And then push to the slider if we're not receiving from the GUI
 			elif isinstance(self.opts, list):
 				el.children[1].value = str(val)
 				if updateGUI and val in self.opts: el.children[0].value = self.opts.index(val)
 
 class CheckentryParam(Param):
+	"""A parameter type that takes `False` if unchecked, or a string value if checked. https://helipad.dev/functions/param/"""
 	defaultVal = ''
 	type='checkentry'
 
 	def __init__(self, **kwargs):
 		self.bvar = True if 'per' not in kwargs or kwargs['per'] is None else {k:True for k in kwargs['pKeys']}
 		self.svar = self.defaultVal if 'per' not in kwargs or kwargs['per'] is None else {k:self.defaultVal for k in kwargs['pKeys']}
 		self.value = None
@@ -203,15 +213,15 @@
 			if hasattr(self, 'elements') and not isNotebook(): return {k: v.get() for k,v in self.elements.items()}
 			else: return {k: self.svar[k] if self.bvar[k] else False for k in self.pKeys}
 		#Per-item parameter, get one
 		else:
 			if hasattr(self, 'elements') and item in self.elements and not isNotebook(): return self.elements[item].get()
 			else: return self.svar[item] if self.bvar[item] else False
 
-	def setSpecific(self, val, item=None, updateGUI=True):
+	def setSpecific(self, val, item=None, updateGUI: bool=True):
 		self.setParent(val, item, False) #Don't update the GUI because it's a complex multivar type
 		if self.per is None:
 
 			#Manage setting stopafter to an event
 			if self.name == 'stopafter':
 				if val and isinstance(val, str):
 					self.event = True
@@ -264,66 +274,68 @@
 		if self.element is not None and isNotebook() and not disable:
 			for e in ([self.element] if self.per is None else self.elements.values()):
 				e.children[0].disabled = False
 				if e.children[0].value: e.children[1].disabled = False
 		else: super().disabled(disable)
 
 class CheckgridParam(Param):
+	"""A parameter type that takes a list of boolean values. https://helipad.dev/functions/param/"""
 	defaultVal = []
 	type='checkgrid'
 
 	def __init__(self, **kwargs):
 		if kwargs['per'] is not None: raise ValueError(ï('Cannot instantiate per-item checkgrid parameter.'))
 		if 'default' not in kwargs or not isinstance(kwargs['default'], list): kwargs['default'] = []
 		if isinstance(kwargs['opts'], list): kwargs['opts'] = {k:k for k in kwargs['opts']}
 		for k,v in kwargs['opts'].items():
 			if isinstance(v, str): kwargs['opts'][k] = (v, None) #Standardized key:(name, tooltip) format
 		self.vars = {k: k in kwargs['default'] for k in kwargs['opts']}
 		super().__init__(**kwargs)
 
 	@property
-	def pKeys(self): return list(self.vars.keys())
+	def pKeys(self) -> list: return list(self.vars.keys())
 
 	def getSpecific(self, item=None):
 		useElement = self.element is not None and not isNotebook() and not isinstance(self, Shocks)
 		vals = self.element if useElement else self.vars
 		if item is not None: return vals[item]
 		else: return [k for k,v in vals.items() if (v.get() if useElement else v)]
 
-	def set(self, item, val=True, updateGUI=True):
+	def set(self, item, val=True, updateGUI: bool=True):
 		if getattr(self, 'setter', False):
 			val = self.setter(val, item)
 			if val is not None: self.setSpecific(item, val)
 		else: self.setSpecific(item, val, updateGUI)
 
 	#Takes a list of strings, or a key-bool pair
-	def setSpecific(self, item, val=True, updateGUI=True):
+	def setSpecific(self, item, val=True, updateGUI: bool=True):
 		if isinstance(item, list):
 			for i in self.pKeys: self.set(i, i in item)
 		else:
 			if self.element is not None and not isNotebook(): self.element.checks[item].set(val)
 			self.vars[item] = val
 
 			if updateGUI and isNotebook() and hasattr(self, 'elements'):
 				try: self.elements[item].children[0].value = val
 				except KeyError: return #Ipywidgets ≥8.0 runs the callback on instantiation before the element property is set
 
 	@property
-	def range(self):
+	def range(self) -> list:
 		combos = []
 		for i in range(len(self.vars)): combos += list(combinations(self.pKeys, i+1))
 		return combos
 
-	def disabled(self, disable):
+	def disabled(self, disable: bool):
 		if hasattr(self, 'elements') and isNotebook():
 			for e in self.elements.values():
 				if hasattr(e, 'children'): e.children[0].disabled = disable
 		else: super().disabled(disable)
 
-	def addItem(self, name, label, position=None, selected=False):
+	def addItem(self, name: str, label: str, position=None, selected: bool=False):
+		"""Add a new checkbox to the grid."""
 		if self.element is not None and not isNotebook(): raise RuntimeError(ï('Cannot add checkgrid items after control panel is drawn.'))
 
 		if position is None or position > len(self.vars): self.opts[name] = label
 		else:		#Reconstruct opts because there's no insert method
 			newopts, i = ({}, 1)
 			for k,v in self.opts.items():
 				if position==i: newopts[name] = label
@@ -339,46 +351,52 @@
 			if position is None or position > len(self.vars): self.containerElement.children += (self.elements[name],)
 			else: self.containerElement.children = self.containerElement.children[:position-1] + (self.elements[name],) + self.containerElement.children[position-1:]
 
 		self.vars[name] = selected
 		if selected: self.default.append(name)
 
 class ParamGroup:
-	def __init__(self, name, members, opened):
+	"""Define a collapsible group of parameters for display in the control panel. https://helipad.dev/functions/params/group/"""
+	def __init__(self, name: str, members, opened: bool):
 		self.title = name
 		self.members = members
 		self.element = None
 		self.open = opened
 
 		for p in members.values():
 			if p.per is not None or p.type=='checkgrid': raise TypeError(ï('Cannot add checkgrids or per-item parameters to groups.'))
 			p.group = name
 
-	def get(self):
+	def get(self) -> dict:
+		"""A `dict` with values for all parameters in the group."""
 		return {name: p.get() for name, p in self.members.items()}
 
-	def toggle(self): self.open = not self.open
+	def toggle(self):
+		"""Open or close the frame around the grouped parameters."""
+		self.open = not self.open
 
 	@property
-	def open(self): return self._open
+	def open(self) -> bool:
+		"""Whether the frame around the grouped parameters is currently open."""
+		return self._open
 
 	@open.setter
-	def open(self, val):
+	def open(self, val: bool):
 		self._open = val
 		if self.element is not None:
 			if isNotebook(): self.element.selected_index = 0 if val else None
 			else: self.element.open = val
 
 #==================
 # CONTAINER CLASSES
 #==================
 
-#Also delete any interface elements
 class fStoreWithInterface(funcStore):
-	def remove(self, name):
+	"""Subclass of `FuncStore` that also deletes parameter interface elements on removal. https://helipad.dev/functions/funcstore/"""
+	def remove(self, name: str):
 		if isinstance(name, (list, tuple)): return [self.remove(n) for n in name]
 
 		if name not in self: return False
 		if getattr(self[name], 'config', False): raise ValueError(ï('Cannot remove built-in parameters.'))
 		self._destroy(self[name])
 
 		del self[name]
@@ -386,22 +404,24 @@
 
 	def _destroy(self, item):
 		if item.element:
 			if not isNotebook(): item.element.forget()
 			else: item.element.close()
 
 class Params(fStoreWithInterface):
+	"""Interface for storing, adding, and accessing model parameters. Stored in `model.params`. https://helipad.dev/functions/params/"""
 	multi = False
 
 	def __init__(self, model):
 		super().__init__()
 		self.model = model
 		self.groups = []
 
-	def add(self, name, title, type, dflt, opts={}, runtime=True, callback=None, per=None, desc=None, prim=None, getter=None, setter=None, **args):
+	def add(self, name: str, title: str, type: str, dflt, opts={}, runtime: bool=True, callback=None, per=None, desc=None, prim=None, getter=None, setter=None, **args):
+		"""Register a global parameter to be displayed in the control panel. `type` can take `'menu'`, `'check'`, `'slider'`, `'checkentry'`, `'checkgrid'`, or `'hidden'`, and `opts` will depend on the parameter type. https://helipad.dev/functions/params/add/"""
 		if name in self: warnings.warn(ï('Parameter \'{}\' already defined. Overriding…').format(name), None, 2)
 
 		if callable(getter):
 			args['getter'] = lambda item=None: getter(*([name, self.model] if per is None else [name, self.model, item]))
 
 		if callable(setter):
 			args['setter'] = lambda val, item=None: setter(*([val, name, self.model] if per is None else [val, name, self.model, item]))
@@ -415,67 +435,76 @@
 			'callback': callback,
 			'desc': desc,
 			'per': per
 		})
 		if per is not None:
 			if per=='breed':
 				if prim is None:
-					if len(self.model.primitives)==1: prim = next(iter(self.model.primitives.keys()))
+					if len(list(self.model.agents.keys()))==1: prim = next(iter(self.model.agents.keys()))
 					else: raise KeyError(ï('Per-breed parameter must specify which primitive it belongs to.'))
 				args['prim'] = prim
-			args['pKeys'] = self.model.primitives[prim].breeds if per=='breed' else self.model.goods
+			args['pKeys'] = self.model.agents[prim].breeds if per=='breed' else self.model.goods
 
 		if type.title()+'Param' in globals(): pclass = globals()[type.title()+'Param']
 		else:
 			pclass = Param
 			args['type'] = type
 		self[name] = pclass(**args)
 		if self.model.cpanel and isNotebook(): self.model.cpanel.__init__(self, redraw=True) #Redraw if necessary
 		return self[name]
 
-	def group(self, name, params, opened=True):
+	def group(self, name: str, params: list, opened: bool=True):
+		"""Group parameters into a collapsible section in the control panel. https://helipad.dev/functions/params/group/"""
 		pg = ParamGroup(name, {p: self[p] for p in params}, opened)
 		self.groups.append(pg)
 		return pg
 
 	#Save the configuration parameters
 	def clear(self):
+		"""Clear all user-added parameters and removes them from the control panel if drawn. https://helipad.dev/functions/params/clear/"""
 		for p in self.values():
 			if getattr(p, 'config', False): continue
 			self._destroy(p)
 		configs = {k:v for k,v in self.items() if getattr(v, 'config', False)}
 		super().clear()
 		self.update(configs)
 
 	@property
-	def globals(self): return {k:v for k,v in self.items() if v.per is None}
+	def globals(self):
+		"""The subset of global parameters, i.e. those added with `per=None`. https://helipad.dev/functions/params/#globals"""
+		return {k:v for k,v in self.items() if v.per is None}
 
 	@property
-	def perBreed(self): return {k:v for k,v in self.items() if v.per=='breed'}
+	def perBreed(self):
+		"""The subset of per-breed parameters, i.e. those added with `per='breed'`. https://helipad.dev/functions/params/#perbreed"""
+		return {k:v for k,v in self.items() if v.per=='breed'}
 
 	@property
-	def perGood(self): return {k:v for k,v in self.items() if v.per=='good'}
+	def perGood(self):
+		"""The subset of per-good parameters, i.e. those added with `per='good'`. https://helipad.dev/functions/params/#pergood"""
+		return {k:v for k,v in self.items() if v.per=='good'}
 
-#This object is instantiated once and lives in model.shocks
 class Shocks(CheckgridParam, fStoreWithInterface):
-	multi = False
+	"""Interface for adding, storing, and executing model shocks. Stored in `model.shocks`, but also subclasses `CheckgridParam` and the same object is also located in `model.params['shocks']`. https://helipad.dev/functions/shocks/"""
+	multi: bool = False
 
 	def __init__(self, model):
 		dict.__init__(self)
 		CheckgridParam.__init__(self, name='shocks', title=ï('Shocks'), type='checkgrid', opts={}, dflt={}, runtime=True, config=True, per=None)
 		self.model = model
 
 		class Shock(Item):
+			"""Container defining a shock to a parameter that can execute during model runtime. https://helipad.dev/functions/shock/"""
 			@property
-			def selected(self2): return self.get(self2.name)
+			def selected(self2) -> bool: return self.get(self2.name)
 
 			@selected.setter
-			def selected(self, val): self.active(val)
+			def selected(self2, val: bool): self2.active(val)
 
-			def active(self2, val, updateGUI=True):
+			def active(self2, val: bool, updateGUI: bool=True):
 				self.set(self2.name, bool(val))
 				if updateGUI and not isNotebook() and self2.element is not None:
 					self2.element.BooleanVar.set(val)
 
 			def do(self, model):
 				if self.param is not None:
 					newval = self.valFunc(self.param.get(self.item))	#Pass in current value
@@ -495,21 +524,16 @@
 				self.active(val, False)
 
 				if callable(model.params['shocks'].callback): model.params['shocks'].callback(model, 'shocks', (self.name, val))
 		self.Shock = Shock
 
 	def __repr__(self): return f'<{self.__class__.__name__}: {len(self)} shocks>'
 
-	#param is the name of the variable to shock.
-	#valFunc is a function that takes the current value and returns the new value.
-	#timerFunc is a function that takes the current tick value and returns true or false
-	#    or the string 'button' in which case it draws a button in the control panel that shocks on press
-	#The variable is shocked when timerFunc returns true
-	#Can pass in param=None to run an open-ended valFunc that takes the model as an object instead
-	def add(self, name, param, valFunc, timerFunc, active=True, desc=None):
+	def add(self, name: str, param, valFunc, timerFunc, active: bool=True, desc=None):
+		"""Register a shock to parameter `param`. `valFunc` takes the current value and returns a new value. `timerFunc` is a function that takes the current model time and returns `bool` (or the string `'button'`, in which case the value is shocked when a control panel button is pressed); `valFunc` will execute whenever `timerFunc` returns `True`. `param` can also be set to `None`, in which case `valFunc` receives the model object. https://helipad.dev/functions/shocks/add/"""
 		if param is not None:
 			item = param[2] if isinstance(param, tuple) and len(param)>2 else None	#The good or breed whose parameter to shock
 			param = self.model.params[param[0]] if isinstance(param, tuple) else self.model.params[param]
 		else: item=None
 
 		super().add(name, self.Shock(
 			name=name,
@@ -521,48 +545,49 @@
 			element=None,
 			selected=active
 		))
 
 		if timerFunc != 'button': self.addItem(name, name, selected=active)
 
 	def clear(self):
+		"""Clear all registered shocks and removes the element from the control panel."""
 		if self.element is not None: self._destroy(self)
 		super().clear()
 
-	#Deprecated. Remove in Helipad 1.6
-	def register(self, *args, **kwargs):
-		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('Shocks.register()', 'Shocks.add()'), FutureWarning, 2)
-		self.add(*args, **kwargs)
-
 	def step(self):
+		"""Run through the `timerFunc`s of the registered shocks and execute the `valFunc` for any `timerFunc` that returns `True`. https://helipad.dev/functions/shocks/step/"""
 		for shock in self.values():
 			if shock.selected and callable(shock.timerFunc) and shock.timerFunc(self.model.t):
 				shock.do(self.model)
 
 	@property
-	def buttons(self): return {k:s for k,s in self.items() if s.timerFunc=='button'}
+	def buttons(self):
+		"""The subset of registered shocks where `shock.timerFunc=='button'` and therefore render as buttons in the control panel. https://helipad.dev/functions/shocks/#buttons"""
+		return {k:s for k,s in self.items() if s.timerFunc=='button'}
 
 	@property
-	def shocksExceptButtons(self): return {k:s for k,s in self.items() if callable(s.timerFunc)}
+	def shocksExceptButtons(self):
+		"""The subset of registered shocks where `shock.timerFunc` is a function and therefore render as checkboxes in the control panel. https://helipad.dev/functions/shocks/#shocksExceptButtons"""
+		return {k:s for k,s in self.items() if callable(s.timerFunc)}
 
 	# ===============
 	# TIMER FUNCTIONS
 	# The following *return* timer functions; they are not themselves timer functions.
 	# ===============
 
-	#With n% probability each period
 	def randn(self, n):
+		"""Generate a timer function that returns `True` with `n`% probability each period. https://helipad.dev/functions/shocks/randn/"""
 		if n<0 or n>100: raise ValueError(ï('randn() argument must be between 0 and 100.'))
 		def fn(t): return random.randint(0,100) < n
 		return fn
 
-	#Once at t=n. n can be an int or a list of periods
 	def atperiod(self, n):
+		"""Generate a timer function that returns `True` at one or several specified periods. https://helipad.dev/functions/shocks/atperiod/"""
 		def fn(t):
 			if isinstance(n, list): return t in n
 			else: return t==n
 		return fn
 
-	#Regularly every n periods
-	def everyn(self, n, offset=0):
+	def everyn(self, n: int, offset: int=0):
+		"""Generates a timer function that returns `True` every `n` periods. https://helipad.dev/functions/shocks/everyn/"""
 		def fn(t): return t%n-offset==0
 		return fn
```

### Comparing `helipad-1.5.1/helipad/utility.py` & `helipad-1.6/helipad/utility.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,49 @@
-# ==========
-# Utility functions
-# Do not run this file; import model.py and run your file.
-# ==========
+"""
+Classes to give agents utility functions, and a base `Utility` class to subclass new utility functions. Built-in utility functions include `CES`, `Leontief`, and `CobbDouglas`.
+"""
 
 from abc import ABC, abstractmethod
 from helipad.helpers import ï
 
-#Basic utility functions
 class Utility(ABC):
+	"""A base class defining the methods a utility class must implement. https://helipad.dev/functions/utility/"""
 
 	#Receives an array of goods.
 	#Can, but doesn't necessarily have to correspond to the registered goods
 	#i.e. you can have an abstract good like real balances
 	def __init__(self, goods):
 		self.goods = goods
 		self.utility = 0
 
-	def consume(self, quantities):
+	def consume(self, quantities: dict):
+		"""Sets `self.utility` to the value returned from `self.calculate()`. `agent.stocks` can be passed directly to this function. https://helipad.dev/functions/utility/consume/"""
 		self.utility = self.calculate(quantities)
 		return self.utility
 
-	#Receives an array of quantities
-	#Returns a scalar utility
 	@abstractmethod
-	def calculate(self, quantities):
+	def calculate(self, quantities: dict):
+		"""Calculate the agent's utility on the basis of the array of quantities entered. https://helipad.dev/functions/utility/calculate/"""
 		if len(quantities) != len(self.goods): raise KeyError(ï('Quantities argument doesn\'t match initialized list of goods.'))
 
-	#Receives a budget and an array of prices
-	#Returns an array of utility-maximizing quantities
 	@abstractmethod
-	def demand(self, budget, prices):
-		pass
+	def demand(self, budget, prices: dict):
+		"""Calculate total demand for the various goods given some income. https://helipad.dev/functions/utility/demand/"""
 
-	#Receives an array of quantities
-	#Returns a dictionary of marginal utilities
 	@abstractmethod
-	def mu(self, quantities):
+	def mu(self, quantities: dict):
+		"""Calculates the marginal utilities of the goods in question on the basis of the entered quantities. https://helipad.dev/functions/utility/mu/"""
 		if len(quantities) != len(self.goods): raise KeyError(ï('Quantities argument doesn\'t match initialized list of goods.'))
 
-	#Receives two quantities, returns a marginal rate of substitution
 	@abstractmethod
-	def mrs(self, good1, q1, good2, q2):
-		pass
+	def mrs(self, good1: str, q1, good2: str, q2):
+		"""Calculate the marginal rate of substitution between `good1` and `good2` given quantities `q1` and `q2`, respectively. https://helipad.dev/functions/utility/mrs/"""
 
-#Constant elasticity of substitution
 class CES(Utility):
+	"""A constant elasticity of substitution utility function. https://helipad.dev/functions/ces/"""
 
 	#Coefficients should add to 1, but this is not enforced
 	#Goods can be a list of goods, or a dict of goods and corresponding coefficients
 	def __init__(self, goods, elast):
 		if isinstance(goods, dict):
 			self.coeffs = goods
 			goods = goods.keys()
@@ -123,21 +118,22 @@
 			# Derivation at https://cameronharwick.com/blog/how-to-derive-a-demand-function-from-a-ces-utility-function/
 			for h, price in prices.items():
 				demand[g] += self.coeffs[h]/self.coeffs[g] * price ** (1-self.elast)
 			demand[g] = budget * prices[g] ** (-self.elast) / demand[g]
 
 		return demand
 
-#Goods can be a list of goods, or a dict of goods and corresponding exponents
 class CobbDouglas(CES):
+	"""A Cobb-Douglas utility function. `Goods` can be a list of goods, or a dict of goods and corresponding exponents. https://helipad.dev/functions/cobbdouglas/"""
 	def __init__(self, goods):
 		if isinstance(goods, list):
 			goods = {g:1/len(goods) for g in goods}
 
 		super().__init__(goods, 1)
 
 	@property
 	def exponents(self): return self.coeffs
 
 class Leontief(CES):
+	"""A Leontief utility function, where utility is equal to the minimum quantity held of any relevant good. https://helipad.dev/functions/leontief/"""
 	def __init__(self, goods):
 		super().__init__(goods, 0)
```

### Comparing `helipad-1.5.1/helipad/visualize.py` & `helipad-1.6/helipad/visualize.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,94 @@
-# ==========
-# The matplotlib interface for plotting
-# Do not run this file; import model.py and run from your file.
-# ==========
+"""
+Base classes for visualizing Helipad models with Matplotlib, to be passed to `model.useVisual()`. Main visualizers are `TimeSeries` to display diachronic data, and `Charts` to display synchronic data.
+"""
 
 import sys
 from abc import ABC, abstractmethod
-from math import sqrt, ceil, floor, pi
-from numpy import ndarray, array, asanyarray, log10, linspace, newaxis, arange, full_like
+from math import sqrt, ceil, pi, isnan
+from numpy import ndarray, array, asanyarray, log10, linspace, newaxis, arange, full_like, linalg, ones, vstack
 import matplotlib, matplotlib.pyplot as plt, matplotlib.style as mlpstyle, matplotlib.cm as cm
+from matplotlib.lines import Line2D
+from matplotlib.patches import Polygon
 from helipad.helpers import *
 mlpstyle.use('fast')
 
 #======================
 # TOP-LEVEL VISUALIZERS
 # These two use Matplotlib, but subclasses of BaseVisualization don't necessarily have to
 #======================
 
-#Used for creating an entirely new visualization window
 class BaseVisualization(ABC):
-	isNull = True
+	"""Base class defining the methods that must be implemented by any visualization. https://helipad.dev/functions/basevisualization/"""
+	isNull: bool = True
 
-	#Create the window. Mandatory to implement
 	@abstractmethod
-	def launch(self, title): pass
+	def launch(self, title: str):
+		"""Launch the visualization window (if in Tkinter) or cell (if in Jupyter). https://helipad.dev/functions/basevisualization/launch/"""
 
-	#Refresh every so many periods. Mandatory to implement
-	#data is the *incremental* data
 	@abstractmethod
-	def update(self, data): pass
+	def refresh(self, data: dict):
+		"""Update the visualization with new data and refresh the display. `data` is only data since the last visualization refresh. https://helipad.dev/functions/basevisualization/refresh/"""
 
-	#Do something when events happen. Mandatory to implement
 	@abstractmethod
-	def event(self, t, color, **kwargs): pass
+	def event(self, t: int, color, **kwargs):
+		"""Called when an event is triggered, in order to be reflected in the visualization. https://helipad.dev/functions/basevisualization/event/"""
 
-	#Called from model.terminate(). Optional to implement
-	def terminate(self, model): pass
+	def terminate(self, model):
+		"""Cleanup on model termination. Called automatically from `model.terminate()`. https://helipad.dev/functions/basevisualization/terminate/"""
 
-class MPLVisualization(BaseVisualization):
-	keys = {}
+class MPLVisualization(BaseVisualization, dict):
+	"""Base class for visualizations using Matplotlib. https://helipad.dev/functions/mplvisualization/"""
 
 	def __init__(self, model):
 		self.model = model #Unhappy with this
-		self.plots = {}
 		self.selector = model.params.add('plots', ï('Plots'), 'checkgrid', [], opts={}, runtime=False, config=True)
 		self.dim = None
 		self.pos = (400, 0)
 		self.fig = None
 		self.lastUpdate = None
+		self.keyListeners = {}
 
 		def pause(model, event):
 			if model.hasModel and event.canvas is self.fig.canvas:
 				if model.running: model.stop()
 				else: model.start()
 		self.addKeypress(' ', pause)
 
 		if isNotebook():
 			from IPython import get_ipython
 			get_ipython().magic('matplotlib widget')
 		else: matplotlib.use('TkAgg') #macosx would be preferable (Retina support), but it blocks the cpanel while running
 
-	def __repr__(self): return f'<{self.__class__.__name__} with {len(self.plots)} plots>'
+	def __repr__(self): return f'<{self.__class__.__name__} with {len(self)} plots>'
 
-	#Subclasses should call super().launch **after** the figure is created.
+	# Subclasses should call super().launch **after** the figure is created.
 	@abstractmethod
-	def launch(self, title, dim=None, pos=None):
+	def launch(self, title: str):
 		if not isNotebook():
 			self.fig.canvas.manager.set_window_title(title)
 			if self.model.cpanel: self.model.cpanel.setAppIcon()
+
+		#MPL can't take a method bound to an unhashable class (i.e. `dict`)
+		def sendEvent(event):
+			axes = event.artist.axes if hasattr(event, 'artist') else event.inaxes
+			if axes is not None:
+				for p in self.activePlots.values():
+					if axes is p.axes:
+						p.MPLEvent(event)
+						break
+
+			if event.name=='key_press_event' and event.key in self.keyListeners:
+				for f in self.keyListeners[event.key]: f(self.model, event)
+
 		self.fig.tight_layout()
 		self.fig.canvas.mpl_connect('close_event', self.model.terminate)
-		self.fig.canvas.mpl_connect('key_press_event', self.sendEvent)
-		self.fig.canvas.mpl_connect('pick_event', self.sendEvent)
-		self.fig.canvas.mpl_connect('button_press_event', self.sendEvent)
+		self.fig.canvas.mpl_connect('key_press_event', sendEvent)
+		self.fig.canvas.mpl_connect('pick_event', sendEvent)
+		self.fig.canvas.mpl_connect('button_press_event', sendEvent)
 		self.lastUpdate = 0
 
 		#Resize and position graph window if applicable
 		fm = self.fig.canvas.manager
 		if hasattr(fm, 'window'):
 			if not self.dim:
 				#This should be the window height, but MPL only allows us to set the figure height.
@@ -95,38 +108,37 @@
 	def terminate(self, model):
 		fm = self.fig.canvas.manager
 		if hasattr(fm, 'window'):
 			self.dim = list(self.fig.get_size_inches()*self.fig.dpi)
 			pos = fm.window.wm_geometry().split('+')
 			self.pos = (pos[1], pos[2])
 
-	def sendEvent(self, event):
-		axes = event.artist.axes if hasattr(event, 'artist') else event.inaxes
-		if axes is not None:
-			for p in self.activePlots.values():
-				if axes is p.axes:
-					p.MPLEvent(event)
-					break
+	def addKeypress(self, key: str, fn):
+		"""Register a function to be run when `key` is pressed in a Matplotlib visualizer. `fn` will run if `key` is pressed at any time when the plot window is in focus. To narrow the focus to a particular plot, define `catchKeypress()` in a subclass of `ChartPlot`. https://helipad.dev/functions/mplvisualization/addkeypress/"""
+		if not key in self.keyListeners: self.keyListeners[key] = []
+		self.keyListeners[key].append(fn)
 
-		if event.name=='key_press_event' and event.key in self.keys:
-			for f in self.keys[event.key]: f(self.model, event)
-
-	def addKeypress(self, key, fn):
-		if not key in self.keys: self.keys[key] = []
-		self.keys[key].append(fn)
+	@property
+	def activePlots(self) -> dict:
+		"""The subset of the plots containing the `Plot`s that are currently active. https://helipad.dev/functions/mplvisualization/#activePlots"""
+		return {k:plot for k,plot in self.items() if plot.selected}
 
 	@property
-	def activePlots(self):
-		return {k:plot for k,plot in self.plots.items() if plot.selected}
+	def isNull(self) -> bool:
+		"""`True` when the model should run as-if with no visualization, for example if all plots are unselected. `False` indicates the window can be launched. https://helipad.dev/functions/mplvisualization/#isNull"""
+		return not [plot for plot in self.values() if plot.selected]
 
 	@property
-	def isNull(self):
-		return not [plot for plot in self.plots.values() if plot.selected]
+	def plots(self):
+		"""A `dict` of plots. This property is deprecated; the visualization object can be indexed directly."""
+		warnings.warn(ï('model.visual.plots is deprecated. Plots can be accessed by indexing the visualization object directly.'), FutureWarning, 2)
+		return self
 
 class TimeSeries(MPLVisualization):
+	"""A Matplotlib-based visualizer for displaying time series data on plots so the whole history of any given variable over the model's runtime can be seen at once. https://helipad.dev/functions/timeseries/"""
 	def __init__(self, model):
 		super().__init__(model)
 		self.verticals = []
 
 		#Plot categories
 		self.addPlot('utility', 'Utility', selected=False)
 
@@ -141,32 +153,31 @@
 				leg.set_visible(not leg.get_visible())
 			event.canvas.draw_idle()
 		self.addKeypress('t', toggle)
 
 		#Delete the corresponding series when a reporter is removed
 		@model.hook('removeReporter')
 		def deleteSeries(data, key):
-			for p in self.plots.values():
+			for p in self.values():
 				for s in p.series:
 					if s.reporter==key:
 						# Remove subseries
 						for ss in s.subseries:
-							for sss in self.model.plots[s.plot].series:
+							for sss in self[s.plot].series:
 								if sss.reporter == ss:
-									self.plots[s.plot].series.remove(sss)
+									self[s.plot].series.remove(sss)
 									continue
-						self.plots[s.plot].series.remove(s)
+						self[s.plot].series.remove(s)
 
 		#Move the plots parameter to the end when the cpanel launches
 		@model.hook('CpanelPreLaunch')
 		def movePlotParam(model):
 			model.params['plots'] = model.params.pop('plots')
 
-	#listOfPlots is the trimmed model.plots list
-	def launch(self, title):
+	def launch(self, title: str):
 		if not self.activePlots: return #Windowless mode
 
 		self.resolution = 1
 		if isNotebook():
 			plt.close() #Clean up after any previous runs
 			matplotlib.rcParams['figure.figsize'] = [9, 7]
 
@@ -188,15 +199,15 @@
 
 	def terminate(self, model):
 		super().terminate(model)
 		if self.isNull:
 			model.params['csv'].enable()
 			if not isinstance(model.param('stopafter'), str): model.params['stopafter'].enable()
 
-	def update(self, data):
+	def refresh(self, data: dict):
 		newlen = len(next(data[x] for x in data))
 		if self.resolution > 1: data = {k: keepEvery(v, self.resolution) for k,v in data.items()}
 		time = newlen + len(next(iter(self.activePlots.values())).series[0].fdata)*self.resolution
 		for plot in self.activePlots.values(): plot.update(data, time) #Append new data to series
 
 		#Redo resolution at 2500, 25000, etc
 		if 10**(log10(time/2.5)-3) >= self.resolution:
@@ -206,68 +217,70 @@
 					serie.fdata = keepEvery(serie.fdata, 10)
 			if self.resolution > self.model.param('refresh'): self.model.param('refresh', self.resolution)
 
 		for plot in self.activePlots.values(): plot.draw(time) #Update the actual plots. Has to be after the new resolution is set
 		if self.fig.stale: self.fig.canvas.draw_idle()
 		self.fig.canvas.flush_events() #Listen for user input
 
-	#Position is the number you want it to be, *not* the array position
-	def addPlot(self, name, label, position=None, selected=True, logscale=False, stack=False):
+	def addPlot(self, name: str, label: str, position=None, selected: bool=True, logscale: bool=False, stack: bool=False):
+		"""Register a plot area in the `TimeSeries` plot area to which data series can be added. `position` Position is the number you want it to be, *not* the array position. https://helipad.dev/functions/timeseries/addplot/"""
 		plot = TimeSeriesPlot(viz=self, name=name, label=label, logscale=logscale, stack=stack)
 
 		self.selector.addItem(name, label, position, selected)
-		if position is None or position > len(self.plots): self.plots[name] = plot
+		if position is None or position > len(self): self[name] = plot
 		else:		#Reconstruct the dicts because there's no insert method…
 			newplots, i = ({}, 1)
-			for k,v in self.plots.items():
+			for k,v in self.items():
 				if position==i:
 					newplots[name] = plot
 				newplots[k] = v
 				i+=1
-			self.plots = newplots
+			self.clear()
+			self.update(newplots)
 
 		plot.selected = selected #Do this after CheckgridParam.addItem
 		return plot
 
 	def removePlot(self, name, reassign=None):
+		"""Remove a plot or plots and optionally reassign their series to a different plot. https://helipad.dev/functions/timeseries/removeplot/"""
 		if self.model.cpanel: raise RuntimeError(ï('Cannot remove plots after control panel is drawn.'))
 		if isinstance(name, list):
 			for p in name: self.removePlot(p, reassign)
 			return
 
-		if not name in self.plots:
+		if not name in self:
 			warnings.warn(ï('No plot \'{}\' to remove.').format(name), None, 2)
 			return False
 
-		if reassign is not None: self.plots[reassign].series += self.plots[name].series
-		del self.plots[name]
+		if reassign is not None: self[reassign].series += self[name].series
+		del self[name]
 		del self.selector.opts[name]
 		del self.selector.vars[name]
 		if name in self.selector.default: self.selector.default.remove(name)
 		return True
 
-	def event(self, t, color='#CC0000', linestyle='--', linewidth=1, **kwargs):
+	def event(self, t: int, color='#CC0000', linestyle: str='--', linewidth=1, **kwargs):
 		if self.fig is None: return
 		self.verticals.append([p.axes.axvline(x=t, color=color, linestyle=linestyle, linewidth=linewidth) for p in self.activePlots.values()])
 
 		# Problem: Need x to be in plot coordinates but y to be absolute w.r.t the figure
-		# next(iter(self.plots.values())).axes.text(t, 0, label, horizontalalignment='center')
+		# next(iter(self.values())).axes.text(t, 0, label, horizontalalignment='center')
 
 class Charts(MPLVisualization):
+	"""A Matplotlib-based visualizer for a variety of visualizations that display data that reflects a single point in time. https://helipad.dev/functions/charts/"""
 	def __init__(self, model):
 		super().__init__(model)
 		self.events = {}
 		self.plotTypes = {}
 
-		for p in [BarChart, NetworkPlot, TimeSeriesPlot]: self.addPlotType(p)
+		for p in [BarChart, AgentsPlot, TimeSeriesPlot]: self.addPlotType(p)
 		model.params['refresh'].runtime=False
-		self.refresh = model.params['refresh']
 		self.model = model # :(
 
-	def launch(self, title):
+	def launch(self, title: str):
 		if not self.activePlots: return #Windowless mode
 		from matplotlib.widgets import Slider
 
 		n = len(self.activePlots)
 		x = ceil(sqrt(n))
 		y = ceil(n/x)
 		if isNotebook():
@@ -279,134 +292,141 @@
 		plots = list(self.activePlots.values())
 		for i in range(n):
 			plots[i].launch(self.fig.add_subplot(y,x,i+1, projection=plots[i].projection))
 			plots[i].subplot_position = (y,x,i+1)
 		super().launch(title)
 
 		#Time slider
-		ref = self.refresh.get()
+		ref = self.model.params['refresh'].get()
 		self.fig.subplots_adjust(bottom=0.12) #Make room for the slider
 		sax = self.fig.add_axes([0.1,0.01,.75,0.03], facecolor='#EEF')
 		self.timeslider = Slider(sax, 't=', 0, ref, ref, valstep=ref, closedmin=False)
 		self.timeslider.on_changed(self.scrub)
 
 		self.fig.canvas.draw_idle()
 		plt.show(block=False)
 
-	def update(self, data):
+	def refresh(self, data: dict):
 		data = {k:v[-1] for k,v in data.items()}
 		t = self.model.t #cheating?
 		for c in self.activePlots.values(): c.update(data, t)
 
 		#Update slider. This calls self.scrub(), which in turn calls chart.draw()
 		self.timeslider.valmax = t
 		self.timeslider.set_val(t)
 		self.timeslider.ax.set_xlim(0,t) #Refresh
 
 		self.fig.patch.set_facecolor(self.events[t] if t in self.events else 'white')
 		if self.fig.stale: self.fig.canvas.draw_idle()
 		self.fig.canvas.flush_events() #Listen for user input
 
-	#Update the graph to a particular model time
-	def scrub(self, t):
+	def scrub(self, t: int):
+		"""Update the visualizer with the values from model time `t`."""
 		self.scrubval = t
 		for c in self.activePlots.values(): c.draw(t)
 		self.fig.patch.set_facecolor(self.events[t] if t in self.events else 'white')
 
-	def addPlot(self, name, label, type=None, position=None, selected=True, **kwargs):
+	def addPlot(self, name: str, label: str, type=None, position=None, selected=True, **kwargs):
+		"""Adds a plot area to the Chart visualizer. Defaults to a bar chart, but can be set to any subclass of ChartPlot. Kwargs are passed to the `ChartPlot` object. https://helipad.dev/functions/charts/addplot/"""
 		self.selector.addItem(name, label, position, selected)
+		if type == 'network': #Deprecated in Helipad 1.6; remove in 1.8
+			warnings.warn(ï('The `network` plot type is deprecated. Use `agents` instead.'), FutureWarning, 2)
+			type = 'agents'
 		self.type = type if type is not None else 'bar'
 		if self.type not in self.plotTypes: raise KeyError(ï('\'{}\' is not a registered plot visualizer.').format(self.type))
-		self.plots[name] = self.plotTypes[self.type](name=name, label=label, viz=self, selected=True, **kwargs)
+		self[name] = self.plotTypes[self.type](name=name, label=label, viz=self, selected=True, **kwargs)
 
-		self.plots[name].selected = selected #Do this after CheckgridParam.addItem
-		return self.plots[name]
+		self[name].selected = selected #Do this after CheckgridParam.addItem
+		return self[name]
 
 	def addPlotType(self, clss):
+		"""Registers a new plot type for the Charts visualizer. Registered plot types can then be added to the visualization area with `Charts.addPlot()`. https://helipad.dev/functions/charts/addplottype/"""
 		if not issubclass(clss, ChartPlot): raise TypeError(ï('New plot types must subclass ChartPlot.'))
 		self.plotTypes[clss.type] = clss
 
 	def removePlot(self, name):
+		"""Remove a plot or plots and optionally reassign their series to a different plot. https://helipad.dev/functions/timeseries/removeplot/"""
 		if self.model.cpanel: raise RuntimeError(ï('Cannot remove plots after control panel is drawn.'))
 		if isinstance(name, list):
 			for p in name: self.removePlot(p)
 			return
 
-		if not name in self.plots:
+		if not name in self:
 			warnings.warn(ï('No plot \'{}\' to remove.').format(name), None, 2)
 			return False
 
-		del self.plots[name]
+		del self[name]
 		return True
 
-	def event(self, t, color='#FDC', **kwargs):
-		ref = self.refresh.get()
+	def event(self, t: int, color='#FDC', **kwargs):
+		ref = self.model.params['refresh'].get()
 		self.events[ceil(t/ref)*ref] = color
 
 #======================
 # PLOT-LEVEL VISUALIZERS
 # Plug into either TimeSeries or Charts as one of the subplots
 #======================
 
-#Used for creating a synchronic plot area in the Charts visualizer. Must interface with Matplotlib and specify class.type.
-#Extra kwargs in Charts.addPlot() are passed to ChartPlot.__init__().
 class ChartPlot(Item):
+	"""Base class for creating a synchronic plot area in the Charts visualizer. Must interface with Matplotlib and specify `class.type`. Extra kwargs in `Charts.addPlot()` are passed to `ChartPlot.__init__()`. https://helipad.dev/functions/chartplot/"""
 	def __init__(self, **kwargs):
 		if 'projection' not in kwargs and not hasattr(self, 'projection'): self.projection = None
 		self.axes = None
 		super().__init__(**kwargs)
 
 	def __repr__(self): return f'<{self.__class__.__name__}: {self.name}>'
 
 	@property
-	def selected(self): return self.viz.model.params['plots'].get(self.name)
+	def selected(self):
+		"""Whether the plot is currently queued for display. Do not modify this property directly; use ChartPlot.active() to ensure consistency with the GUI state. https://helipad.dev/functions/chartplot/#selected"""
+		return self.viz.model.params['plots'].get(self.name)
 
 	@selected.setter
-	def selected(self, val): self.active(val)
+	def selected(self, val: bool): self.active(val)
 
-	def active(self, val, updateGUI=True):
+	def active(self, val: bool, updateGUI: bool=True):
+		"""Turn on or off the selected state of a plot in the control panel. https://helipad.dev/functions/chartplot/active/"""
 		self.viz.model.params['plots'].set(self.name, bool(val))
 		if updateGUI and not isNotebook() and hasattr(self, 'check'):
 			self.check.set(val)
 
-	#Receives an AxesSubplot object used for setting up the plot area. super().launch(axes) should be called from the subclass.
 	@abstractmethod
 	def launch(self, axes):
+		"""Set up the plot's `axes` object when `Charts` launches the visualization window. Subclasses should call `super().launch(axes)` at the beginning of the method. https://helipad.dev/functions/chartplot/launch/"""
 		self.axes = axes
 		axes.set_title(self.label, fontdict={'fontsize':10})
 
-	#Receives a 1-dimensional dict with only the most recent value of each column
-	#The subclass is responsible for storing the relevant data internally
 	@abstractmethod
-	def update(self, data, t): pass
+	def update(self, data: dict, t: int):
+		"""Receive current model data and store it for future scrubbing. Values of `data` should only contain the most recent value of each column. This method is only for updating plot data; drawing code happens in `draw()`. https://helipad.dev/functions/chartplot/update/"""
 
-	#Receives the time to scrub to
 	@abstractmethod
-	def draw(self, t, forceUpdate=False):
+	def draw(self, t: int, forceUpdate: bool=False):
+		"""Refresh the `axes` object to display new or historical data. This method is called after `ChartPlot.update()` when the visualizer receives new data, and when scrubbing the time bar. https://helipad.dev/functions/chartplot/draw/"""
 		if forceUpdate: self.viz.fig.canvas.draw_idle()
 
 	def remove(self):
+		"""Removes the plot from the visualizer."""
 		self.viz.removePlot(self.name)
 
-	#Override in order to catch plot-specific keypresses, clicks, or picks
-	def MPLEvent(self, event): pass
+	def MPLEvent(self, event):
+		"""Catch `pick_event`, `key_press_event`, and `button_press_event` events that occur inside a particular plot. https://helipad.dev/functions/chartplot/mplevent/"""
 
 class TimeSeriesPlot(ChartPlot):
+	"""Visualize time series data on one or more variables. Can be used in either the `TimeSeries` or `Charts` visualizer. https://helipad.dev/functions/timeseriesplot/"""
 	type = 'timeseries'
 	def __init__(self, **kwargs):
 		self.series = []
 		self.scrubline = None
 		for p in ['logscale', 'stack']:
 			if p not in kwargs: kwargs[p] = False
 		super().__init__(**kwargs)
 
-	#First arg is a reporter name registered in DataCollector, or a lambda function
-	#Second arg is the series name. Use '' to not show in the legend.
-	#Third arg is the plot's hex color, or a Color object
-	def addSeries(self, reporter, label, color, style='-', visible=True):
+	def addSeries(self, reporter, label: str, color, style: str='-', visible: bool=True):
+		"""Register a reporter to be plotted during the model's runtime. https://helipad.dev/functions/timeseriesplot/addseries/"""
 		if not isinstance(color, Color): color = Color(color)
 
 		#Check against columns and not reporters so subseries work
 		if not callable(reporter) and not reporter in self.viz.model.data.columns:
 			raise KeyError(ï('Reporter \'{}\' does not exist. Be sure to register reporters before adding series.').format(reporter))
 
 		#Add subsidiary series (e.g. percentile bars)
@@ -455,29 +475,29 @@
 					s.legtext = label
 					label.axes = axes #Necessary because an MPL bug fails to set the axes property of the text labels. Fixed in 3.5.0 (#20458)
 					break
 
 		for series in self.series: #Make sure we start out with the user-set visibility
 			if series.label and not series._visible: series.visible = False
 
-	def update(self, data, t):
+	def update(self, data: dict, t: str):
 		firstdata = next(iter(data.values()))
 		if isinstance(firstdata, list): newlen, res = len(firstdata), self.resolution
 		else:
 			newlen = 1
 			res = self.viz.model.param('refresh')
 			data = {k: [v] for k,v in data.items()}
 		for serie in self.series:
 			if callable(serie.reporter):						#Lambda functions
 				for i in range(newlen):
 					serie.fdata.append(serie.reporter(t-(newlen-1-i)*res))
 			elif serie.reporter in data: serie.fdata += data[serie.reporter] #Actual data
 			else: continue									#No data
 
-	def draw(self, t, forceUpdate=False):
+	def draw(self, t: int, forceUpdate: bool=False):
 		if self.scrubline is not None:
 			self.scrubline.remove()
 			self.scrubline = None
 
 		#Draw new data if this is a new refresh
 		if t==len(self.series[0].fdata)*self.resolution:
 			tseries = range(0, t, self.resolution)
@@ -514,26 +534,29 @@
 			c1 = event.artist					#The label or line that was clicked
 			for s in self.series:
 				if s.label and (c1 is s.legline or c1 is s.legtext):
 					s.toggle()
 					break
 
 	@property
-	def resolution(self):
+	def resolution(self) -> int:
+		"""The time elapsing between any two data points drawn to screen (not the time elapsing between two updates, which is a user-controlled parameter)."""
 		return self.viz.resolution if hasattr(self.viz, 'resolution') else int(self.viz.model.param('refresh'))
 
 class BarChart(ChartPlot):
+	"""A plot type that displays live-updating bar charts. https://helipad.dev/functions/barchart/"""
 	type = 'bar'
 	def __init__(self, **kwargs):
 		for arg in ['horizontal', 'logscale']:
 			if not arg in kwargs: kwargs[arg] = False
 		super().__init__(**kwargs)
 		self.bars = []
 
-	def addBar(self, reporter, label, color='blue', position=None):
+	def addBar(self, reporter, label: str, color='blue', position=None):
+		"""Register a data reporter as a bar on the current plot. To display error bars, use the `std` or `percentiles` arguments when creating the agent reporter. https://helipad.dev/functions/barchart/addbar/"""
 		if not isinstance(color, Color): color = Color(color)
 		bar = Item(reporter=reporter, label=label, color=color)
 
 		#Add subsidiary series (e.g. percentile bars)
 		bar.err = []
 		if reporter in self.viz.model.data.reporters and self.viz.model.data.reporters[reporter].children:
 			for p in self.viz.model.data.reporters[reporter].children:
@@ -554,28 +577,29 @@
 		errors = rects.errorbar.lines[2][0].properties()['paths'] #Hope MPL's API doesn't ever move this…!
 		for bar, rect, err in zip(self.bars, rects, errors):
 			bar.element = rect
 			bar.errPath = err.vertices
 			bar.errHist = []
 			bar.data = []
 
+		#Set bar names
 		cstlfunc, cstfunc = (axes.set_yticklabels, axes.set_yticks) if self.horizontal else (axes.set_xticklabels, axes.set_xticks)
 		cstfunc(range(len(self.bars)))
 		cstlfunc([bar.label for bar in self.bars])
 		axes.margins(x=0)
 
 		if self.logscale:
 			if self.horizontal:
 				axes.set_xscale('log')
 				axes.set_xlim(1/2, 2, auto=True)
 			else:
 				axes.set_yscale('log')
 				axes.set_ylim(1/2, 2, auto=True)
 
-	def update(self, data, t):
+	def update(self, data: dict, t: int):
 		getlim, setlim = (self.axes.get_xlim, self.axes.set_xlim) if self.horizontal else (self.axes.get_ylim, self.axes.set_ylim)
 		lims = list(getlim())
 		for b in self.bars:
 			b.data.append(data[b.reporter])
 			if data[b.reporter] < lims[0]: lims[0] = data[b.reporter]
 			if data[b.reporter] > lims[1]: lims[1] = data[b.reporter]
 
@@ -586,33 +610,39 @@
 					if errs[i] < lims[0]: lims[0] = errs[i]
 					if errs[i] > lims[1]: lims[1] = errs[i]
 				b.errHist.append(errs)
 
 		setlim(lims)
 		self.axes.autoscale_view(tight=False)
 
-	def draw(self, t=None, forceUpdate=False):
+	def draw(self, t: int=None, forceUpdate: bool=False):
 		if t is None: t=self.viz.scrubval
-		i = int(t/self.viz.refresh.get())-1
+		i = int(t/self.viz.model.param('refresh'))-1
 		for b in self.bars:
 			setbar = b.element.set_width if self.horizontal else b.element.set_height
 			setbar(b.data[i])
 
 			if b.err: #Update error bars
 				for j,cap in enumerate(b.errPath):
 					if len(b.errHist[i]) >= j+1: cap[0 if self.horizontal else 1] = b.errHist[i][j]
 		super().draw(t, forceUpdate)
 
-class NetworkPlot(ChartPlot):
-	type = 'network'
+class AgentsPlot(ChartPlot):
+	"""A plot visualizer used for displaying individual agents in various layouts. Agents can be plotted in a network structure, a spatial layout (or both at once), or a scatterplot comparing agents on two data dimensions. https://helipad.dev/functions/agentsplot/"""
+	type = 'agents'
 	def __init__(self, **kwargs):
 		if 'prim' not in kwargs: kwargs['prim'] = None
-		if 'kind' not in kwargs: kwargs['kind'] = 'edge'
-		if 'layout' not in kwargs: kwargs['layout'] = 'spring'
+		if 'kind' in kwargs:
+			warnings.warn(ï('The kind= argument is deprecated and has been replaced with network=.')) #Deprecated in Helipad 1.6; remove in Helipad 1.8
+			kwargs['network'] = kwargs['kind']
+		if 'network' not in kwargs: kwargs['network'] = 'edge'
+		if 'layout' not in kwargs: kwargs['layout'] = 'scatter' if 'scatter' in kwargs else 'spring'
+		if 'scatter' not in kwargs: kwargs['scatter'] = None
 		super().__init__(**kwargs)
+		self.scatterLims = [[0,0],[0,0]]
 		self.ndata = {}
 
 		self.params = {
 			'patchColormap': 'Blues',
 			#'patchProperty': 'mapcolor', #Don't specify, so we have a default white
 			'agentMarker': 'o',
 			'agentSize': 30,
@@ -621,179 +651,232 @@
 			'labelColor': 'k',
 			'labelFamily': 'sans-serif',
 			'labelWeight': 'normal',
 			'labelAlpha': None,
 			'labelAlign': 'center',
 			'labelVerticalAlign': 'center',
 			'lockLayout': False,
-			'patchAspect': 1
+			'patchAspect': 1,
+			'mapBg': 'black',
+			'regLine': False,
+			'regColor': 'red',
+			'regWidth': 1
 		}
 
 	def launch(self, axes):
 		import networkx as nx, networkx.drawing.layout as lay
-		def patchgrid_layout(G):
-			if not self.viz.model.patches: raise
+		self.layouts = {l: getattr(lay, l+'_layout') for l in ['spring', 'circular', 'kamada_kawai', 'random', 'shell', 'spectral', 'spiral']}
+
+		def spatial_layout(G):
 			if self.projection == 'polar': #Calculate the right angle from the x coordinate without modifying the original tuples
 				return {i: (2*pi-(2*pi/self.viz.model.patches.dim[0] * data['position'][0])+1/2*pi, data['position'][1]) for i, data in G.nodes.items()}
 			else: return {i: data['position'] for i,data in G.nodes.items()}
-		lay.patchgrid_layout = patchgrid_layout
+
+		def scatter_layout(G):
+			self.axes.set_xlabel(self.scatter[0])
+			self.axes.set_ylabel(self.scatter[1])
+			self.axes.spines['top'].set_visible(False)
+			self.axes.spines['right'].set_visible(False)
+			data = {i: [data[self.scatter[0]], data[self.scatter[1]]] for i,data in G.nodes.items()}
+
+			#Update limits if necessary
+			xs, ys = array([d[0] for d in data.values()]), array([d[1] for d in data.values()])
+			self.scatterLims[0][0] = min(self.scatterLims[0][0], xs.min())
+			self.scatterLims[0][1] = max(self.scatterLims[0][1], xs.max())
+			self.scatterLims[1][0] = min(self.scatterLims[1][0], ys.min())
+			self.scatterLims[1][1] = max(self.scatterLims[1][1], ys.max())
+			self.axes.set_xlim(*self.scatterLims[0])
+			self.axes.set_ylim(*self.scatterLims[1])
+
+			#Add regression line if applicable
+			if self.params['regLine']:
+				b0, b1 = linalg.lstsq(vstack([xs, ones(len(xs))]).T, ys, rcond=None)[0]
+				self.axes.add_line(Line2D(
+					[self.scatterLims[0][0], self.scatterLims[0][1]], [b0*self.scatterLims[0][0]+b1, b0*self.scatterLims[0][1]+b1],
+					linestyle = '--' if self.params['regLine'] is True else self.params['regLine'],
+					color = self.params['regColor'],
+					linewidth = self.params['regWidth']
+			    ))
+
+			return data
+		self.layouts['spatial'] = spatial_layout
+		self.layouts['scatter'] = scatter_layout
+
 		self.nx = nx
-		self.layClass = getattr(lay, self.layout+'_layout')
 		self.components = {}
 
 		super().launch(axes)
 
-	#Receives event from MPLVisualization.sendEvent()
 	def MPLEvent(self, event):
 		if event.name=='key_press_event' and event.key=='l': self.rotateLayout()
 
 		elif event.name=='pick_event':
 			pk = list(self.pos.keys())
-			agents = [self.viz.model.agent(pk[i]) for i in event.ind]
+			agents = [self.viz.model.agents[pk[i]] for i in event.ind]
 			self.viz.model.doHooks('agentClick', [agents, self, self.viz.scrubval])
 
-		elif event.name=='button_press_event' and self.layout=='patchgrid':
+		elif event.name=='button_press_event' and self.layout=='spatial':
 			if self.projection=='polar':
 				x = 2*pi-event.xdata+1/2*pi
 				if x > 2*pi: x-=2*pi
-				x,y = floor(x/(2*pi/self.viz.model.patches.dim[0])), floor(event.ydata)
+				x,y = x/(2*pi/self.viz.model.patches.dim[0]), event.ydata
 			else:
-				x,y = round(event.xdata), round(event.ydata)
-			if x > self.viz.model.patches.dim[0]-1 or y > self.viz.model.patches.dim[1]-1: return
-			self.viz.model.doHooks('patchClick', [self.viz.model.patches[x,y], self, self.viz.scrubval])
-
-	def update(self, data, t):
-		G = self.viz.model.network(self.kind, self.prim, excludePatches=True)
-
-		#Capture label and size data
-		if self.params['agentLabel'] and self.params['agentLabel'] is not True:
-			agents = self.viz.model.allagents
-			if 'good:' in self.params['agentLabel']:
-				for n in G.nodes: G.nodes[n]['label'] = agents[n].stocks[self.params['agentLabel'].split(':')[1]]
+				x,y = event.xdata, event.ydata
+			if x > self.viz.model.patches.boundaries[0][1] or y > self.viz.model.patches.boundaries[1][1]: return
+			self.viz.model.doHooks('patchClick', [self.viz.model.patches.at(x,y), self, self.viz.scrubval])
+
+	def update(self, data: dict, t: int):
+		G = self.viz.model.agents.network(self.network, self.prim, excludePatches=self.prim!='patch')
+
+		#Capture data for label, size, and scatterplot position
+		capture = {}
+		if self.params['agentLabel'] and self.params['agentLabel'] is not True: capture['label'] = self.params['agentLabel']
+		if self.params['agentSize'] and type(self.params['agentSize']) not in [int, float]: capture['size'] = self.params['agentSize']
+		if self.scatter:
+			for v in self.scatter: capture[v] = v
+		agents = {a.id:a for a in (self.viz.model.agents[self.prim] if self.prim else self.viz.model.agents.all)}
+		for k,v in capture.items():
+			if 'good:' in v:
+				for n in G.nodes: G.nodes[n][k] = agents[n].stocks[v.split(':')[1]]
 			else:
-				for n in G.nodes: G.nodes[n]['label'] = getattr(agents[n],self.params['agentLabel'])
-		if self.params['agentSize'] and type(self.params['agentSize']) not in [int, float]:
-			agents = self.viz.model.allagents
-			if 'good:' in self.params['agentSize']:
-				for n in G.nodes: G.nodes[n]['size'] = agents[n].stocks[self.params['agentSize'].split(':')[1]]
-			else:
-				for n in G.nodes: G.nodes[n]['size'] = getattr(agents[n],self.params['agentSize'])
-
+				for n in G.nodes: G.nodes[n][k] = getattr(agents[n],v)
 		self.ndata[t] = G
 
 		#Save spatial data even if we're on a different layout
 		if self.viz.model.patches:
-			pd = self.patchData(None if t==self.viz.model.t else t)
-			for col in self.viz.model.patches:
-				for p in col:
-					p.colorData[t] = pd[p.x][p.y]
+			lst = []
+			for p in self.viz.model.agents['patch']:
+				p.colorData[t] = self.getPatchParamValue(p, None if t==self.viz.model.t else t)
+				lst.append(p.colorData[t])
 
 			#Renormalize color scale
-			nmin, nmax = pd.min().min(), pd.max().max()
+			nmin, nmax = min(lst), max(lst)
 			self.normal = plt.cm.colors.Normalize(nmin if not hasattr(self,'normal') or nmin<self.normal.vmin else self.normal.vmin, nmax if not hasattr(self,'normal') or nmax>self.normal.vmax else self.normal.vmax)
 
-
-	def draw(self, t=None, forceUpdate=False):
+	def draw(self, t: int=None, forceUpdate: bool=False):
 		if t is None: t=self.viz.scrubval
 		self.axes.clear()
-		if self.layout != 'patchgrid' or self.projection=='polar': self.axes.axis('off')
+		if self.layout not in ['spatial', 'scatter'] or self.projection=='polar': self.axes.axis('off')
 		self.axes.set_title(self.label, fontdict={'fontsize':10})
-
-		if self.layout == 'patchgrid':
-			pd = self.patchData(t).T #Transpose because numpy is indexed col, row
+		if self.layout != 'spatial' or self.viz.model.patches.geometry != 'geo':
+			self.axes.set_facecolor('white')
+			self.axes.set_aspect('auto')
+		self.pos = self.layouts[self.layout](self.ndata[t])
+
+		if self.layout == 'spatial':
+			cmap = cm.get_cmap(self.params['patchColormap'])
+			if self.viz.model.patches.geometry == 'geo': pd = array([self.getPatchParamValue(p,t) for p in self.viz.model.patches])
+			else:
+				pd = array([[self.getPatchParamValue(p,t) for p in col] for col in self.viz.model.patches]).T #Transpose because numpy is indexed col, row
 			if self.projection=='polar':
+				self.axes.set_aspect('equal')
 				self.axes.set_ylim(0, self.viz.model.patches.dim[1])
-				norm = (pd - self.normal.vmin)/(self.normal.vmax-self.normal.vmin)
+				norm = (pd - int(self.normal.vmin))/(rng if (rng:=(self.normal.vmax-int(self.normal.vmin))) else 1)
 				space = linspace(0.0, 1.0, 100)
-				rgb = cm.get_cmap(self.params['patchColormap'])(space)[newaxis, :, :3][0]
+				rgb = cmap(space)[newaxis, :, :3][0]
 
 				x = self.viz.model.patches.dim[0]
 				for r in range(len(norm)):
 					for ti in range(len(norm[0])):
 						#Define the range going counterclockwise. The 1/4 is to make r=0 point north rather than east.
 						#Last argument is the resolution of the curve
 						theta = arange(2*pi*((1-1/x) * ti - 1/x + 1/4), 2*pi*((1-1/x) * ti + 1/4)+.04, .04)
-						cr1 = full_like(theta, r)
-						cr2 = full_like(theta, r+1)
-						self.axes.fill_between(theta, cr1, cr2, color=rgb[int(norm[r,ti]*(len(space)-1))])
+						color = self.params['mapBg'] if isnan(norm[r, ti]) else rgb[int(norm[r,ti]*(len(space)-1))]
+						self.axes.fill_between(theta, full_like(theta, r), full_like(theta, r+1), color=color)
 			else:
-				self.components['patches'] = self.axes.imshow(pd, norm=self.normal, cmap=self.params['patchColormap'], aspect=self.params['patchAspect'])
-				# self.patchmap.set_norm(self.normal)
-				# self.components['patches'].set_data(pd)
+				if self.viz.model.patches.geometry == 'rect':
+					self.axes.spines['top'].set_visible(True)
+					self.axes.spines['right'].set_visible(True)
+					cmap.set_bad(self.params['mapBg'])
+					self.components['patches'] = self.axes.imshow(pd, norm=self.normal, cmap=cmap, aspect=self.params['patchAspect'])
+					# self.patchmap.set_norm(self.normal)
+					# self.components['patches'].set_data(pd)
+				elif self.viz.model.patches.geometry == 'geo':
+					self.axes.set_aspect('equal')
+					self.axes.set_xlim(*self.viz.model.patches.boundaries[0])
+					self.axes.set_ylim(*self.viz.model.patches.boundaries[1])
+					self.axes.set_facecolor(self.params['mapBg'])
+					norm = (pd - int(self.normal.vmin))/(rng if (rng:=(self.normal.vmax-int(self.normal.vmin))) else 1)
+					space = linspace(0.0, 1.0, 100)
+					rgb = cmap(space)[newaxis, :, :3][0]
+					for i,p in enumerate(self.viz.model.patches):
+						color = self.params['mapBg'] if isnan(norm[i]) else rgb[int(norm[i]*(len(space)-1))]
+						self.axes.add_patch(Polygon(array(p.polygon.exterior.xy).T, color=color))
 
 		#Draw nodes, edges, and labels separately so we can split out the directed and undirected edges
-		self.pos = self.layClass(self.ndata[t])
 		sizes = self.params['agentSize']*10 if type(self.params['agentSize']) in [int, float] else [n[1]['size']*10 for n in self.ndata[t].nodes(data=True)]
-		self.components['nodes'] = self.nx.draw_networkx_nodes(self.ndata[t], self.pos, ax=self.axes, node_color=[self.viz.model.primitives[n[1]['primitive']].breeds[n[1]['breed']].color.hex for n in self.ndata[t].nodes(data=True)], node_size=sizes, node_shape=self.params['agentMarker'])
+		self.components['nodes'] = self.nx.draw_networkx_nodes(self.ndata[t], self.pos, ax=self.axes, node_color=[self.viz.model.agents[n[1]['primitive']].breeds[n[1]['breed']].color.hex for n in self.ndata[t].nodes(data=True)], node_size=sizes, node_shape=self.params['agentMarker'])
 		e_directed = [e for e in self.ndata[t].edges.data() if e[2]['directed']]
 		e_undirected = [e for e in self.ndata[t].edges.data() if not e[2]['directed']]
 		self.components['edges_d'] = self.nx.draw_networkx_edges(self.ndata[t], self.pos, ax=self.axes, edgelist=e_directed, width=[e[2]['weight'] for e in e_directed])
 		self.components['edges_u'] = self.nx.draw_networkx_edges(self.ndata[t], self.pos, ax=self.axes, edgelist=e_undirected, width=[e[2]['weight'] for e in e_undirected], arrows=False)
 		if self.params['agentLabel']:
 			lab = None if self.params['agentLabel'] is True else {n:self.ndata[t].nodes[n]['label'] for n in self.ndata[t].nodes}
 			self.components['labels'] = self.nx.draw_networkx_labels(self.ndata[t], self.pos, ax=self.axes, labels=lab, font_size=self.params['labelSize'], font_color=self.params['labelColor'], font_family=self.params['labelFamily'], font_weight=self.params['labelWeight'], alpha=self.params['labelAlpha'], horizontalalignment=self.params['labelAlign'], verticalalignment=self.params['labelVerticalAlign'])
+		if self.layout=='scatter': self.axes.tick_params('both', left=True, bottom=True, labelleft=True, labelbottom=True)
 
 		self.components['nodes'].set_picker(True)	#Listen for mouse events on nodes
 		self.components['nodes'].set_pickradius(5)	#Set margin of valid events in pixels
 
 		super().draw(t, forceUpdate)
 
 	def rotateLayout(self):
+		"""Rotate the layout among the several NetworkX layout classes, plus spatial and scatterplot layouts. This method is called when pressing 'l' with the mouse over the plot. https://helipad.dev/functions/agentsplot/rotatelayout/"""
 		self.axes.set_yscale('linear') #Override default logscale keypress
 		if self.params['lockLayout']: return
 
 		#Select the next layout in the list
-		import networkx.drawing.layout as lay
-		layouts = ['spring', 'circular', 'kamada_kawai', 'random', 'shell', 'spectral', 'spiral', 'patchgrid']
+		layouts = ['spatial'] if self.viz.model.patches else []
+		if self.scatter: layouts.append('scatter')
+		if self.network in self.viz.model.agents.edges or not layouts: layouts += ['spring', 'circular', 'kamada_kawai', 'random', 'shell', 'spectral', 'spiral']
 		li = layouts.index(self.layout)+1
 		while li>=len(layouts): li -= len(layouts)
 		self.layout = layouts[li]
-		self.layClass = getattr(lay, self.layout+'_layout')
 
 		#Replace the axes object if we need to switch projections
-		if self.projection == 'polar' or (self.layout=='patchgrid' and self.viz.model.patches and self.viz.model.patches.geometry=='polar'):
+		if self.projection == 'polar' or (self.layout=='spatial' and self.viz.model.patches and self.viz.model.patches.geometry=='polar'):
 			self.projection = None if self.projection=='polar' else 'polar'
 			self.viz.fig.delaxes(self.axes)
 			super().launch(self.viz.fig.add_subplot(*self.subplot_position, projection=self.projection))
 
 		#kamada_kawai requires scipy; fail silently and continue if we don't have it
 		try: self.draw(self.viz.scrubval)
 		except: self.rotateLayout()
 
-	#Helper function
-	def getPatchParamValue(self, patch, t=None):
+	def getPatchParamValue(self, patch, t: int=None):
+		"""Gather historical patch data for use in color generation. https://helipad.dev/functions/agentsplot/getpatchparamvalue/"""
 		if t is not None: return patch.colorData[t]
-		if 'patchProperty' not in self.params: return 0
+		if patch.dead: return float('nan')
+		elif 'patchProperty' not in self.params: return 0
 		elif 'good:' in self.params['patchProperty']: return patch.stocks[self.params['patchProperty'].split(':')[1]]
 		else: return getattr(patch, self.params['patchProperty'])
 
-	def patchData(self, t=None):
-		if not self.viz.model.patches: return
-		return array([[self.getPatchParamValue(p,t) for p in col] for col in self.viz.model.patches])
-
-	def config(self, param, val=None):
+	def config(self, param: str, val=None):
+		"""Sets options for the spatial plot. One argument will return the value; two arguments sets the parameter. See https://helipad.dev/functions/agentsplot/config/ for valid option names."""
 		if isinstance(param, dict):
 			for k,v in param.items(): self.config(k,v)
 		elif val is None: return self.params[param]
 		else: self.params[param] = val
 
 #======================
 # SUB-PLOT OBJECTS
 # Mostly sub-plot data will use an Item object, but some need a little more
 #======================
 
 class Series(Item):
+	"""Stores data on series, which link a reporter to a plot. https://helipad.dev/functions/series/"""
 	@property
-	def visible(self):
+	def visible(self) -> bool:
+		"""Whether the series is to be drawn when the plot window launches, or - if it has launched - whether the series is currently visible. https://helipad.dev/functions/series/#visible"""
 		if not hasattr(self, 'line'): return self._visible
 		elif hasattr(self, 'poly'): return True #If it's a stackplot
 		else: return self.line.get_visible()
 
 	@visible.setter
-	def visible(self, val):
+	def visible(self, val: bool):
 		if not hasattr(self, 'line'): #If we haven't drawn it yet
 			self._visible = val
 			return
 		elif hasattr(self, 'poly'): return	#Ignore if it's a stackplot
 
 		self.line.set_visible(val)
 		for s in self.subseries: s.line.set_visible(val) #Toggle subseries (e.g. percentile bars)
@@ -806,20 +889,22 @@
 		# 	if c1.series in g.get_lines():
 		# 		g.relim()
 		# 		g.autoscale_view(tight=True)
 
 		self.line.figure.canvas.draw_idle()
 
 	def toggle(self):
+		"""Toggles the visibility of the series. https://helipad.dev/functions/series/toggle/"""
 		self.visible = not self.visible
 
 #======================
 # HELPER FUNCTIONS
 #======================
 
-def keepEvery(lst, n):
+def keepEvery(lst: list, n: int):
+	"""Reduce the resolution of a list."""
 	i,l = (1, [])
 	for k in lst:
 		if i%n==0: l.append(k)
 		i+=1
 	# if len(lst)%n != 0: print('Original:',len(lst),'New:',len(l),'Remainder:',len(lst)%n)
 	return l
```

### Comparing `helipad-1.5.1/helipad.egg-info/PKG-INFO` & `helipad-1.6/helipad.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helipad
-Version: 1.5.1
+Version: 1.6
 Summary: An agent-based modeling framework for Python with a shallow learning curve and powerful visualization capabilities.
 Author-email: C Harwick <cameron@cameronharwick.com>
 License: MIT License
         
         Copyright (c) 2023 C Harwick
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,17 +30,18 @@
 Project-URL: Source Code, https://github.com/charwick/helipad
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: notebook
+Provides-Extra: geo
 License-File: LICENSE
 
 # Helipad
 
 Helipad is an agent-based modeling framework for Python with powerful visualization capabilities and a shallow learning curve. Documentation and API reference can be found at [helipad.dev](https://helipad.dev).
 
 ## Features
@@ -69,32 +70,34 @@
 	
 	heli.launchCpanel()
 
 The included [bootstrap model](https://github.com/charwick/helipad/blob/master/sample-models/bootstrap.py) contains a more detailed template, and the [sample models](https://github.com/charwick/helipad/tree/master/sample-models) exemplify various use cases. The documentation also includes a complete [hook and function reference](https://helipad.dev/functions/).
 
 ## Requirements
 
-Helipad requires Python 3.7 or higher. The following libraries are also required:
+Helipad requires Python 3.8 or higher. The following libraries are also required:
 
 * [Matplotlib](https://matplotlib.org/) for visualization
 * [Pandas](https://pandas.pydata.org/) for data collection
 * [NetworkX](http://networkx.github.io/) for network analysis and spatial visualization
 * _Optional:_ [Jupyter](https://jupyter.org/), [Ipywidgets](https://pypi.org/project/ipywidgets/), and [ipympl](https://github.com/matplotlib/ipympl) to run Helipad in Jupyter notebooks
+* _Optional:_ [Shapely](https://shapely.readthedocs.io/) for geospatial models.
 
 ## How to Cite
 
 If you use Helipad in your own research, please cite as follows:
 
 > Harwick, Cameron (2021). “Helipad: A Framework for Agent-Based Modeling in Python.” Working paper available at [ssrn.com/abstract=3870501](https://ssrn.com/abstract=3870501). 
 
 ## Version History
 
+* [1.6](https://helipad.dev/2023/06/helipad-1-6/): Geospatial models, agent scatterplot visualizer, new `Agents` and `Edges` containers
 * [1.5](https://helipad.dev/2023/01/helipad-1-5/): Polar grid spatial models, various spatial improvements
 * [1.4](https://helipad.dev/2022/07/helipad-1-4/): More consistent container API, localization, miscellaneous interface improvements
 * [1.3](https://helipad.dev/2021/06/helipad-1-3/): Allow mixing time series and other plots, display networks on spatial maps, goods API improvements
 * [1.2](https://helipad.dev/2021/02/helipad-1-2/): Extensible visualization API, events, performance profiling, Jupyterlab support
 * [1.1](https://helipad.dev/2020/10/helipad-1-1/): Virtual parameters, improved Jupyter flexibility, spatial pre-alpha, misc improvements
 * [1.0](https://helipad.dev/2020/08/helipad-1-0/): Jupyter integration, hook decorators, and separated control panel from plotting
 * [0.7](https://helipad.dev/2020/06/helipad-0-7/): Ability to output stackplots, parameter sweeps, and an updated parameter identification pattern
 * [0.6](https://helipad.dev/2020/05/helipad-0-6/): Support for multi-level models
-* [0.5](https://helipad.dev/2020/03/helipad-0-5/): Support for matching models, and the checkGrid class
+* [0.5](https://helipad.dev/2020/03/helipad-0-5/): Support for matching models, and the `checkGrid` class
 * 0.4: Initial PyPI release
```

### Comparing `helipad-1.5.1/helipad.egg-info/SOURCES.txt` & `helipad-1.6/helipad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helipad-1.5.1/pyproject.toml` & `helipad-1.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "helipad"
-version = "1.5.1"
+version = "1.6"
 authors = [
 	{ name="C Harwick", email="cameron@cameronharwick.com" },
 ]
 description = "An agent-based modeling framework for Python with a shallow learning curve and powerful visualization capabilities."
 readme = "README.md"
 license = { file="LICENSE" }
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
 	"Operating System :: OS Independent",
 	"Development Status :: 5 - Production/Stable",
 	"Intended Audience :: Science/Research",
 	"Topic :: Scientific/Engineering :: Visualization"
 ]
 dependencies = ["matplotlib", "pandas", "networkx"]
 
 [project.optional-dependencies]
 notebook = ["jupyterlab", "ipywidgets>=8.0", "ipympl"]
+geo = ["shapely"]
 
 [project.urls]
 "Homepage" = "https://helipad.dev"
 "Documentation" = "https://helipad.dev/functions/"
 "Source Code" = "https://github.com/charwick/helipad"
 
 [tool.setuptools.packages.find]
```

### Comparing `helipad-1.5.1/sample-models/Cities.py` & `helipad-1.6/sample-models/Cities.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from numpy import *
 heli = Helipad()
 
 #================
 # CONFIGURATION
 #================
 
-heli.addBreed('urban', '#CC0000')
-heli.addBreed('rural', '#00CC00')
+heli.agents.addBreed('urban', '#CC0000')
+heli.agents.addBreed('rural', '#00CC00')
 
 #Constrain the parameter space to values resulting in H* = 100
 def constrain(model, var, val):
 	if var=='city': model.params['rent'].disabled(val)
 	elif model.param('city'):
 		if var=='fixed':
 			model.params['rent'].enable() #Tkinter won't let you update the value of a disabled widget...
@@ -31,15 +31,15 @@
 heli.params.add('movecost', 'Moving Cost (ω)', 'slider', dflt=10, opts={'low':0, 'high': 150, 'step': 1}, desc='Cost incurred by moving location')
 heli.params.add('deathrate', 'Death Rate (θ)', 'slider', dflt=0.005, opts={'low':0, 'high': 0.05, 'step': 0.001})
 heli.params.add('rent', 'Variable cost (ρ)', 'slider', dflt=.04, opts={'low':0.01, 'high': 0.1, 'step': 0.01}, desc='Per-period cost-of-living, proportional to human capital', callback=constrain)
 heli.params.add('fixed', 'Fixed cost (χ)', 'slider', dflt=.4, opts={'low':0, 'high': 1, 'step': 0.1}, desc='Per-period cost-of-living', callback=constrain)
 
 heli.name = 'Cities'
 heli.stages = 2
-heli.order = 'linear'
+heli.agents.order = 'linear'
 
 popfactor = 10 #Multiplies the productivity and therefore the equilibrium population, without changing anything else
 burnout = 2000 #The end period, once it's equilibrated, over which to average the values
 
 class Land():
 	def __init__(self, loc):
 		self.loc = loc
@@ -49,15 +49,15 @@
 	
 	def produce(self):
 		self.product = popfactor*log(self.input) #if self.loc=='rural' else sqrt(self.input)	# = ln∑P (eq. 2)
 		self.lastInput = self.input
 		self.input = 0 #Reset productivity at the end of each period
 		return self.product
 	
-	def pop(self, model): return len(model.agent(self.loc))
+	def pop(self, model): return len(model.agents['agent'][self.loc])
 	
 	#The add argument calculates the productivity as if the agent were already there, if he's not
 	def agentProd(self, H, add=False):
 		if self.loc=='rural': return sqrt(150) * H
 		else:
 			if add:
 				return 1/sqrt(self.pop(heli)+1) * (heli.data.getLast('hsum')+H)
@@ -77,18 +77,18 @@
 # AGENT BEHAVIOR
 #================
 
 #This is here to make sure that the agents param gets reset at the beginning of each run
 #Otherwise the parameter persists between runs
 @heli.hook
 def modelPreSetup(model):
-	model.movers = {b:0 for b in heli.primitives['agent'].breeds}
-	model.births = {b:0 for b in heli.primitives['agent'].breeds}
+	model.movers = {b:0 for b in heli.agents['agent'].breeds}
+	model.births = {b:0 for b in heli.agents['agent'].breeds}
 	model.deaths = 0
-	for b in heli.primitives['agent'].breeds:
+	for b in heli.agents['agent'].breeds:
 		setattr(model, 'moverate'+b, 0)
 		setattr(model, 'birthrate'+b, 0)
 	model.deathrate = 0
 	
 	#Mark the different phases of the Malthusian model
 	model.events.clear()
 	if not model.param('city'):
@@ -97,15 +97,15 @@
 		def exp1(model):	return sum(diff(model.data.getLast('ruralPop', 20))) > 3
 		@heli.event
 		def stab2(model):	return model.events['exp1'].triggered and model.t > model.events['exp1'].triggered+1000 and sum(diff(model.data.getLast('ruralH', 3000))) < 0
 		@heli.event
 		def end3(model): return model.events['stab2'].triggered and model.t >= model.events['stab2'].triggered + burnout
 	
 	#Start with the equilibrium population
-	else: model.param('num_agent', math.floor(2.55-1.69*model.param('fixed'))*popfactor)
+	else: model.param('num_agent', floor(2.55-1.69*model.param('fixed'))*popfactor)
 
 @heli.hook
 def agentInit(agent, model):
 	agent.H = random.normal(100, 15) if model.param('city') else 10 #Human capital
 	agent.prod = 0
 	agent.wealth = model.param('breedThresh') + model.param('rent')*10
 	agent.lastWage = 0
@@ -115,15 +115,15 @@
 #modelStep executes each stage **before** any agent step functions
 @heli.hook
 def modelStep(model, stage):
 	if stage==2:
 		for l in model.land.values():
 			inp = l.input								# = ∑P
 			Y = l.produce()								# = ln∑P (eq. 2)
-			for a in model.agent(l.loc):
+			for a in model.agents['agent'][l.loc]:
 				a.lastWage = a.prod/inp * Y	# = P/∑P * Y (eq. 3)
 				a.wealth += a.lastWage
 
 @heli.hook
 def agentStep(agent, model, stage):
 	if stage==1:
 		if model.param('city'):
@@ -161,16 +161,16 @@
 		return
 
 #Organize some data and pause if all agents are dead
 @heli.hook
 def modelPostStep(model):
 	if len(model.agents['agent']) == 0: model.stop()
 	else:
-		for b in model.primitives['agent'].breeds:
-			pop = len(model.agent(b))
+		for b in model.agents['agent'].breeds:
+			pop = len(model.agents['agent'][b])
 			if pop > 0:
 				setattr(model,'moverate'+b, model.movers[b]/pop)
 				setattr(model,'birthrate'+b, model.births[b]/pop)
 				model.movers[b] = 0
 				model.births[b] = 0
 		model.deathrate = model.deaths/len(model.agents['agent'])
 		model.deaths = 0
@@ -188,15 +188,15 @@
 
 from helipad.visualize import TimeSeries
 viz = heli.useVisual(TimeSeries)
 
 # returns ln(∑H²)
 @heli.reporter
 def hsum(model, loc='urban'):
-	upop = model.agent(loc)
+	upop = model.agents['agent'][loc]
 	return sum([a.H for a in upop]) if len(upop) > 0 else 1
 
 def perCapGdp(model, loc):
 	def tmp(model):
 		pop = model.land[loc].pop(model)
 		if pop==0: return 0
 		else: return model.land[loc].product/pop
@@ -204,39 +204,39 @@
 
 viz.addPlot('pop', 'Population', 1, logscale=True)
 viz.addPlot('hcap', 'Human Capital', 2)
 viz.addPlot('wage', 'Wage', 3)
 viz.addPlot('wealth', 'Wealth', 4)
 viz.addPlot('rates', 'Rates', 5, logscale=True)
 heli.data.addReporter('theta', heli.data.modelReporter('deathrate'), smooth=0.99)
-viz.plots['rates'].addSeries('theta', 'Death Rate', '#CCCCCC')
+viz['rates'].addSeries('theta', 'Death Rate', '#CCCCCC')
 
-for breed, d in heli.primitives['agent'].breeds.items():
+for breed, d in heli.agents['agent'].breeds.items():
 	heli.data.addReporter(breed+'Pop', heli.land[breed].pop)
 	heli.data.addReporter(breed+'H', heli.data.agentReporter('H', 'agent', breed=breed, percentiles=[25,75]))
 	heli.data.addReporter(breed+'Wage', heli.data.agentReporter('lastWage', 'agent', breed=breed, percentiles=[25,75]))
 	heli.data.addReporter(breed+'ExpWage', heli.data.agentReporter('expwage', 'agent', breed=breed, percentiles=[25,75]))
 	heli.data.addReporter(breed+'Wealth', heli.data.agentReporter('wealth', 'agent', breed=breed, percentiles=[25,75]))
 	heli.data.addReporter(breed+'moveRate', heli.data.modelReporter('moverate'+breed), smooth=0.99)
 	heli.data.addReporter(breed+'birthrate', heli.data.modelReporter('birthrate'+breed), smooth=0.99)
-	viz.plots['pop'].addSeries(breed+'Pop', breed.title()+' Population', d.color)
-	viz.plots['hcap'].addSeries(breed+'H', breed.title()+' Human Capital', d.color)
-	viz.plots['wage'].addSeries(breed+'Wage', breed.title()+' Wage', d.color)
-	viz.plots['wage'].addSeries(breed+'ExpWage', breed.title()+' Expected Wage', d.color2, visible=False)
-	viz.plots['wealth'].addSeries(breed+'Wealth', breed.title()+' Wealth', d.color)
-	viz.plots['rates'].addSeries(breed+'moveRate', breed.title()+' Moveaway Rate', d.color2)
-	viz.plots['rates'].addSeries(breed+'birthrate', breed.title()+' Birthrate', d.color)
+	viz['pop'].addSeries(breed+'Pop', breed.title()+' Population', d.color)
+	viz['hcap'].addSeries(breed+'H', breed.title()+' Human Capital', d.color)
+	viz['wage'].addSeries(breed+'Wage', breed.title()+' Wage', d.color)
+	viz['wage'].addSeries(breed+'ExpWage', breed.title()+' Expected Wage', d.color2, visible=False)
+	viz['wealth'].addSeries(breed+'Wealth', breed.title()+' Wealth', d.color)
+	viz['rates'].addSeries(breed+'moveRate', breed.title()+' Moveaway Rate', d.color2)
+	viz['rates'].addSeries(breed+'birthrate', breed.title()+' Birthrate', d.color)
 
 heli.launchCpanel()
 
 #================
 # PARAM SWEEP & ANALYSIS
 #================
 
-# for p in viz.plots.values(): p.active(False) #Disable plots so Helipad doesn't try to update the visuals during param sweep
+# for p in viz.values(): p.active(False) #Disable plots so Helipad doesn't try to update the visuals during param sweep
 # #Remove superfluous columns
 # @heli.hook
 # def saveCSV(data, model):
 # 	for c in data:
 # 		if 'urban' in c or c in ['city', 'hsum'] or 'utility' in c or 'moveRate' in c or 'Unnamed' in c or 'pctile' in c:
 # 			del data[c]
 # 	print('Finished at', len(data))
```

### Comparing `helipad-1.5.1/sample-models/Helicopter-OMO.py` & `helipad-1.6/sample-models/Helicopter-OMO.py`

 * *Files 4% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 
 		self.amortizeAmt = 0
 
 #===============
 # CONFIGURATION
 #===============
 
-heli.primitives.add('bank', Bank, dflt=1, priority=1, hidden=True)
+heli.agents.addPrimitive('bank', Bank, dflt=1, priority=1, hidden=True)
 heli.name = 'Helicopter/OMO'
 
 #Disable the irrelevant checkboxes if the banking model isn't selected
 #Callback for the dist parameter
 @heli.hook('terminate') #Reset the disabled checkmarks when terminating a model
 def bankChecks(model, val=None):
 	nobank = model.param('dist')!='omo'
@@ -247,23 +247,23 @@
 		model.data.addReporter('targetRR', model.data.agentReporter('targetRR', 'bank'))
 		model.data.addReporter('i', model.data.agentReporter('i', 'bank'))
 		model.data.addReporter('r', model.data.agentReporter('realInterest', 'bank'))
 		model.data.addReporter('cashdemand', cashdemand)
 		model.data.addReporter('inflation', model.data.agentReporter('inflation', 'bank'))
 		model.data.addReporter('M2', lambda model: model.cb.M2)
 
-		model.visual.plots['money'].addSeries('defaults', 'Defaults', '#CC0000')
-		model.visual.plots['money'].addSeries('M2', 'Money Supply', '#000000')
-		model.visual.plots['debt'].addSeries('debt', 'Outstanding Debt', '#000000')
-		model.visual.plots['rr'].addSeries('targetRR', 'Target', '#777777')
-		model.visual.plots['rr'].addSeries('reserveRatio', 'Reserve Ratio', '#000000')
-		model.visual.plots['i'].addSeries('i', 'Nominal interest', '#000000')
-		model.visual.plots['i'].addSeries('r', 'Real interest', '#0000CC')
-		model.visual.plots['i'].addSeries('inflation', 'Inflation', '#CC0000')
-		model.visual.plots['i'].addSeries('cashdemand', '% cash held', '#00CC00')
+		model.visual['money'].addSeries('defaults', 'Defaults', '#CC0000')
+		model.visual['money'].addSeries('M2', 'Money Supply', '#000000')
+		model.visual['debt'].addSeries('debt', 'Outstanding Debt', '#000000')
+		model.visual['rr'].addSeries('targetRR', 'Target', '#777777')
+		model.visual['rr'].addSeries('reserveRatio', 'Reserve Ratio', '#000000')
+		model.visual['i'].addSeries('i', 'Nominal interest', '#000000')
+		model.visual['i'].addSeries('r', 'Real interest', '#0000CC')
+		model.visual['i'].addSeries('inflation', 'Inflation', '#CC0000')
+		model.visual['i'].addSeries('cashdemand', '% cash held', '#00CC00')
 
 @heli.hook
 def modelPostSetup(model):
 	if hasattr(model.agents['store'][0], 'bank'):
 		model.agents['store'][0].pavg = 0
 		model.agents['store'][0].projects = []
 		model.agents['store'][0].defaults = 0
@@ -350,31 +350,31 @@
 	if self.model.param('num_bank') > 0: expand *= self.model.agents['bank'][0].reserveRatio
 	if expand != 0: self.expand(expand)
 CentralBank.step = cbstep
 
 def expand(self, amount):
 
 	#Deposit with each bank in proportion to their liabilities
-	if 'bank' in self.model.primitives and self.model.param('num_bank') > 0:
+	if 'bank' in self.model.agents and self.model.param('num_bank') > 0:
 		self.stocks[self.model.goods.money] += amount
 		self.model.agents['bank'][0].deposit(self, amount) #Budget constraint taken care of in .pay()
 
 	elif self.model.param('dist') == 'lump':
 		amt = amount/self.model.param('num_agent')
 		for a in self.model.agents['agent']:
 			a.stocks[self.model.goods.money] += amt
 	else:
 		M0 = self.M0
-		for a in self.model.allagents.values():
+		for a in self.model.agents.all:
 			a.stocks[self.model.goods.money] += a.stocks[self.model.goods.money]/M0 * amount
 CentralBank.expand = expand
 
 def M2(self):
-	if 'bank' not in self.model.primitives or self.model.param('num_bank') == 0: return self.M0
-	return sum(a.balance for a in self.model.allagents.values())
+	if 'bank' not in self.model.agents or self.model.param('num_bank') == 0: return self.M0
+	return sum(a.balance for a in self.model.agents.all)
 CentralBank.M2 = property(M2)
 
 #Price level
 #Average good prices at each store, then average all of those together weighted by the store's sale volume
 #Figure out whether to break this out or not
 def cbP(self):
 	# denom = 0
```

### Comparing `helipad-1.5.1/sample-models/Helicopter.py` & `helipad-1.6/sample-models/Helicopter.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #===============
 
 class Store(baseAgent):
 	def __init__(self, breed, id, model):
 		super().__init__(breed, id, model)
 
 		#Start with equilibrium prices. Not strictly necessary, but it eliminates the burn-in period. See eq. A7
-		sm=sum(1/sqrt(model.param(('prod','good',g))) for g in model.goods.nonmonetary) * M0/(model.param('num_agent')*(len(model.goods.nonmonetary)+sum(1+model.param(('rbd','breed',b,'agent')) for b in model.primitives['agent'].breeds)))
+		sm=sum(1/sqrt(model.param(('prod','good',g))) for g in model.goods.nonmonetary) * M0/(model.param('num_agent')*(len(model.goods.nonmonetary)+sum(1+model.param(('rbd','breed',b,'agent')) for b in model.agents['agent'].breeds)))
 		self.price = {g:sm/(sqrt(model.param(('prod','good',g)))) for g in model.goods.nonmonetary}
 
 		self.invTarget = {g:model.param(('prod','good',g))*model.param('num_agent')*2 for g in model.goods.nonmonetary}
 		self.portion = {g:1/(len(model.goods.nonmonetary)) for g in model.goods.nonmonetary} #Capital allocation
 		self.wage = 0
 		self.cashDemand = 0
 
@@ -74,32 +74,32 @@
 #===============
 # CONFIGURATION
 #===============
 
 #Stick this here so we can build on it with the OMO model
 def setup():
 	heli = Helipad()
-	heli.primitives.add('store', Store, dflt=1, priority=2, hidden=True)
+	heli.agents.addPrimitive('store', Store, dflt=1, priority=2, hidden=True)
 
 	# Configure how many breeds there are and what good each consumes
 	# In this model, goods and breeds correspond, but they don't necessarily have to
 	breeds = [
 		('hobbit', 'jam', '#D73229'),
 		('dwarf', 'axe', '#2D8DBE'),
 		# ('elf', 'lembas', '#CCBB22')
 	]
 	AgentGoods = {}
 	for b in breeds:
-		heli.addBreed(b[0], b[2], prim='agent')
+		heli.agents.addBreed(b[0], b[2], prim='agent')
 		heli.goods.add(b[1], b[2])
 		AgentGoods[b[0]] = b[1] #Hang on to this list for future looping
 	heli.goods.add('cash', '#009900', money=True)
 
 	heli.name = 'Helicopter'
-	heli.order = 'random'
+	heli.agents.order = 'random'
 
 	# UPDATE CALLBACKS
 
 	def ngdpUpdater(model, var, val):
 		if model.hasModel: model.cb.ngdpTarget = val if not val else model.cb.ngdp
 
 	def rbalUpdater(model, var, breed, val):
@@ -153,68 +153,68 @@
 	viz.addPlot('inventory', 'Inventory', 3)
 	viz.addPlot('rbal', 'Real Balances', 5)
 	viz.addPlot('ngdp', 'NGDP', 7, selected=False)
 	viz.addPlot('capital', 'Production', 9, selected=False)
 	viz.addPlot('wage', 'Wage', 11, selected=False)
 	viz.addPlot('shortage', 'Shortages', 6, selected=False)
 
-	viz.plots['capital'].addSeries(lambda t: 1/len(heli.primitives['agent'].breeds), '', '#CCCCCC')
+	viz['capital'].addSeries(lambda t: 1/len(heli.agents['agent'].breeds), '', '#CCCCCC')
 
 	# heli.data.addReporter('rBal', heli.data.agentReporter('realBalances', 'agent', breed=True))
 	def shortageReporter(good):
 		def reporter(model): return model.shortages[good]
 		return reporter
 
-	for breed, d in heli.primitives['agent'].breeds.items():
+	for breed, d in heli.agents['agent'].breeds.items():
 		heli.data.addReporter('rbalDemand-'+breed, rbaltodemand(breed))
 		heli.data.addReporter('shortage-'+AgentGoods[breed], shortageReporter(AgentGoods[breed]))
 		heli.data.addReporter('eCons-'+breed, heli.data.agentReporter('expCons', 'agent', breed=breed, stat='sum'))
 		# heli.data.addReporter('rWage-'+breed, lambda model: heli.data.agentReporter('wage', 'store')(model) / heli.data.agentReporter('price', 'store', good=b.good)(model))
 		# heli.data.addReporter('expWage', heli.data.agentReporter('expWage', 'agent'))
 		heli.data.addReporter('rBal-'+breed, heli.data.agentReporter('realBalances', 'agent', breed=breed))
 		heli.data.addReporter('invTarget-'+AgentGoods[breed], heli.data.agentReporter('invTarget', 'store', good=AgentGoods[breed]))
 		heli.data.addReporter('portion-'+AgentGoods[breed], heli.data.agentReporter('portion', 'store', good=AgentGoods[breed]))
 
-		viz.plots['demand'].addSeries('eCons-'+breed, breed.title()+'s\' Expected Consumption', d.color2)
-		viz.plots['shortage'].addSeries('shortage-'+AgentGoods[breed], AgentGoods[breed].title()+' Shortage', d.color)
-		viz.plots['rbal'].addSeries('rbalDemand-'+breed, breed.title()+' Target Balances', d.color2)
-		viz.plots['rbal'].addSeries('rBal-'+breed, breed.title()+ 'Real Balances', d.color)
-		viz.plots['inventory'].addSeries('invTarget-'+AgentGoods[breed], AgentGoods[breed].title()+' Inventory Target', heli.goods[AgentGoods[breed]].color2)
-		viz.plots['capital'].addSeries('portion-'+AgentGoods[breed], AgentGoods[breed].title()+' Capital', heli.goods[AgentGoods[breed]].color)
-		# viz.plots['wage'].addSeries('expWage', 'Expected Wage', '#999999')
+		viz['demand'].addSeries('eCons-'+breed, breed.title()+'s\' Expected Consumption', d.color2)
+		viz['shortage'].addSeries('shortage-'+AgentGoods[breed], AgentGoods[breed].title()+' Shortage', d.color)
+		viz['rbal'].addSeries('rbalDemand-'+breed, breed.title()+' Target Balances', d.color2)
+		viz['rbal'].addSeries('rBal-'+breed, breed.title()+ 'Real Balances', d.color)
+		viz['inventory'].addSeries('invTarget-'+AgentGoods[breed], AgentGoods[breed].title()+' Inventory Target', heli.goods[AgentGoods[breed]].color2)
+		viz['capital'].addSeries('portion-'+AgentGoods[breed], AgentGoods[breed].title()+' Capital', heli.goods[AgentGoods[breed]].color)
+		# viz['wage'].addSeries('expWage', 'Expected Wage', '#999999')
 
 	#Do this one separately so it draws on top
 	for good, g in heli.goods.nonmonetary.items():
 		heli.data.addReporter('inv-'+good, heli.data.agentReporter('stocks', 'store', good=good))
-		viz.plots['inventory'].addSeries('inv-'+good, good.title()+' Inventory', g.color)
+		viz['inventory'].addSeries('inv-'+good, good.title()+' Inventory', g.color)
 		heli.data.addReporter('price-'+good, heli.data.agentReporter('price', 'store', good=good))
-		viz.plots['prices'].addSeries('price-'+good, good.title()+' Price', g.color)
+		viz['prices'].addSeries('price-'+good, good.title()+' Price', g.color)
 
 	#Price ratio plots
 	def ratioReporter(item1, item2):
 		def reporter(model):
 			return model.data.agentReporter('price', 'store', good=item1)(model)/model.data.agentReporter('price', 'store', good=item2)(model)
 		return reporter
 	viz.addPlot('ratios', 'Price Ratios', position=3, logscale=True)
-	viz.plots['ratios'].addSeries(lambda t: 1, '', '#CCCCCC')	#plots ratio of 1 for reference without recording a column of ones
+	viz['ratios'].addSeries(lambda t: 1, '', '#CCCCCC')	#plots ratio of 1 for reference without recording a column of ones
 
 	for r in combinations(heli.goods.nonmonetary.keys(), 2):
 		heli.data.addReporter('ratio-'+r[0]+'-'+r[1], ratioReporter(r[0], r[1]))
 		c1, c2 = heli.goods[r[0]].color, heli.goods[r[1]].color
-		viz.plots['ratios'].addSeries('ratio-'+r[0]+'-'+r[1], r[0].title()+'/'+r[1].title()+' Ratio', c1.blend(c2))
+		viz['ratios'].addSeries('ratio-'+r[0]+'-'+r[1], r[0].title()+'/'+r[1].title()+' Ratio', c1.blend(c2))
 
 	#Misc plots
 	heli.data.addReporter('ngdp', lambda model: model.cb.ngdp)
-	viz.plots['ngdp'].addSeries('ngdp', 'NGDP', '#000000')
+	viz['ngdp'].addSeries('ngdp', 'NGDP', '#000000')
 	heli.data.addReporter('storeCash', heli.data.agentReporter('balance', 'store'))
-	viz.plots['money'].addSeries('storeCash', 'Store Cash', '#777777')
+	viz['money'].addSeries('storeCash', 'Store Cash', '#777777')
 	heli.data.addReporter('StoreCashDemand', heli.data.agentReporter('cashDemand', 'store'))
-	viz.plots['money'].addSeries('StoreCashDemand', 'Store Cash Demand', '#CCCCCC')
+	viz['money'].addSeries('StoreCashDemand', 'Store Cash Demand', '#CCCCCC')
 	heli.data.addReporter('wage', heli.data.agentReporter('wage', 'store'))
-	viz.plots['wage'].addSeries('wage', 'Wage', '#000000')
+	viz['wage'].addSeries('wage', 'Wage', '#000000')
 
 #================
 # POST-ANALYSIS
 # Generate the appropriate impulse response functions
 #================
 
 	@heli.hook
@@ -351,15 +351,15 @@
 	def expand(self, amount):
 		if self.model.param('dist') == 'lump':
 			amt = amount/self.model.param('num_agent')
 			for a in self.model.agents['agent']:
 				a.stocks[self.model.goods.money] += amt
 		else:
 			M0 = self.M0
-			for a in self.model.allagents.values():
+			for a in self.model.agents.all:
 				a.stocks[self.model.goods.money] += a.stocks[self.model.goods.money]/M0 * amount
 
 	@property
 	def M0(self):
 		return self.model.data.agentReporter('stocks', 'all', good=self.model.goods.money, stat='sum')(self.model)
 
 	@M0.setter
```

### Comparing `helipad-1.5.1/sample-models/axelrod.py` & `helipad-1.6/sample-models/axelrod.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #===============
 
 from helipad import Helipad
 from numpy import mean, random
 
 heli = Helipad()
 heli.name = 'Axelrod Tournament'
-heli.order = 'match'
+heli.agents.order = 'match'
 
 heli.params['num_agent'].type = 'hidden' #So we can postpone breed determination until the end
 
 #Initial parameter values match the payoffs in Table 1
 heli.params.add('cc', 'C-C payoff', 'slider', dflt=3, opts={'low': 0, 'high': 10, 'step': 0.5})
 heli.params.add('dc', 'D-C payoff', 'slider', dflt=5, opts={'low': 0, 'high': 10, 'step': 0.5})
 heli.params.add('cd', 'C-D payoff', 'slider', dflt=0, opts={'low': 0, 'high': 10, 'step': 0.5})
@@ -149,24 +149,24 @@
 plot = viz.addPlot('payoffs', 'Payoffs')
 
 #Add breeds last-minute so we can toggle them in the control panel
 @heli.hook
 def modelPreSetup(model):
 
 	#Clear breeds from the previous run
-	for b in model.primitives['agent'].breeds:
+	for b in model.agents['agent'].breeds:
 		model.data.removeReporter(b+'-proportion')
-	model.primitives['agent'].breeds.clear()
+	model.agents['agent'].breeds.clear()
 
 	for k in model.param('strategies'):
-		model.addBreed(k, strategies[k][1])
+		model.agents.addBreed(k, strategies[k][1])
 
-	model.param('num_agent', len(model.primitives['agent'].breeds)*model.param('n')) #Three of each strategy, for speed
+	model.param('num_agent', len(model.agents['agent'].breeds)*model.param('n')) #Three of each strategy, for speed
 
-	for b, d in model.primitives['agent'].breeds.items():
+	for b, d in model.agents['agent'].breeds.items():
 		model.data.addReporter(b+'-proportion', proportionReporter(b))
 		plot.addSeries(b+'-proportion', b, d.color)
 
 #===============
 # CONFIGURATION
 #===============
```

### Comparing `helipad-1.5.1/sample-models/bootstrap.py` & `helipad-1.6/sample-models/bootstrap.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #===============
 
 from helipad import Helipad
 # from utility import CobbDouglas
 
 heli = Helipad()
 heli.name = 'Model Name'
-heli.order = 'random' #Can be changed to 'linear' or 'match'
+heli.agents.order = 'random' #Can be changed to 'linear' or 'match'
 heli.stages = 1 #Change to create a multi-stage model
 
 # heli.params.add('name', 'title', 'type (slider, menu, or check)', dflt=default, opts={depends on type})
 # heli.goods.add('good1','hex color', lambda breed: endowment)
-# heli.addBreed('name1', 'hex color')
-# heli.addBreed('name2', 'hex color')
+# heli.agents.addBreed('name1', 'hex color')
+# heli.agents.addBreed('name2', 'hex color')
 
 #===============
 # BEHAVIOR
 # A list of hooks and their function signatures can be found at http://helipad-docs.nfshost.com/hooks/
 #===============
 
 #Any variables or properties the agent should keep track of should have default values set here.
@@ -63,17 +63,17 @@
 # heli.data.addReporter('myReporter2', heli.data.modelReporter('myModelProperty'))
 
 #Plots are areas on the graph where series can be drawn to keep track of reporter data in real time.
 
 myplot = viz.addPlot('myplot', 'Custom Properties', logscale=False, selected=True)
 
 #Series draw reporter data on a plot. Here we draw two series on the same plot.
-#The Plot object can also be accessed later with heli.plots['myplot'], so the following two methods are identical.
+#The Plot object can also be accessed later with heli['myplot'], so the following two methods are identical.
 
 # myplot.addSeries('myplot', 'myReporter1', 'My Agent Property', 'hex color')
-# heli.plots['myplot'].addSeries('myplot', 'myReporter2', 'My Model Property', 'hex color')
+# heli['myplot'].addSeries('myplot', 'myReporter2', 'My Model Property', 'hex color')
 
 #===============
 # LAUNCH THE GUI
 #===============
 
 heli.launchCpanel()
```

### Comparing `helipad-1.5.1/sample-models/cpanel-test.py` & `helipad-1.6/sample-models/cpanel-test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #Registers parameters of every available type in order to test the rendering of the control panel, and runs a dummy model to test the Charts visualizer.
 
 #===============
 # PREAMBLE
 #===============
 
+from random import uniform
 from helipad import Helipad
 heli = Helipad()
 heli.name = 'Test'
 
 #A handful of breeds and goods
 breeds = [
 	('hobbit', 'jam', '#D73229'),
 	('dwarf', 'axe', '#2D8DBE'),
 	('elf', 'lembas', '#CCBB22')
 ]
 AgentGoods = {}
 for b in breeds:
-	heli.addBreed(b[0], b[2], prim='agent')
+	heli.agents.addBreed(b[0], b[2], prim='agent')
 	heli.goods.add(b[1], b[2])
 
 def gcallback(model, name, val):
 	print(name, '=', val)
 
 def icallback(model, name, item, val):
 	print(name, '/', item, '=', val)
@@ -63,47 +64,53 @@
 import random
 from helipad.visualize import Charts
 viz = heli.useVisual(Charts)
 
 @heli.hook
 def agentInit(agent, model):
 	for i in range(20): setattr(agent, 'prop'+str(i), 0)
+	agent.s1 = 0
+	agent.s2 = 0
 
 @heli.hook
 def agentStep(agent, model, stage):
 	for i in range(20):
 		v = getattr(agent, 'prop'+str(i))
 		setattr(agent, 'prop'+str(i), v-1 if random.randint(0, 1) else v+1)
+	
+	agent.s1 += uniform(0,agent.id+model.t**0.75)
+	agent.s2 += uniform(0,agent.id+model.t**0.75)
 
 @heli.hook
 def modelPostSetup(model):
-	model.createNetwork(0.2)
+	model.agents.createNetwork(0.2)
 
 def newedge(model):
-	a1, a2 = random.choice(list(model.agents['agent'])), random.choice(list(model.agents['agent']))
-	while a1.edgesWith(a2): a1, a2 = random.choice(list(model.agents['agent'])), random.choice(list(model.agents['agent']))
-	a1.newEdge(a2, direction=random.choice([True, False]), weight=random.choice([0.5,1,2,3]))
+	a1, a2 = random.choice(model.agents['agent']), random.choice(model.agents['agent'])
+	while a1.edges.With(a2): a1, a2 = random.choice(model.agents['agent']), random.choice(model.agents['agent'])
+	a1.edges.add(a2, direction=random.choice([True, False]), weight=random.choice([0.5,1,2,3]))
 
 #Cut one edge and create one edge
 @heli.hook
 def modelPostStep(model):
-	random.choice(model.allEdges['edge']).cut()
+	random.choice(model.agents.edges['edge']).cut()
 	newedge(model)
 
-net = viz.addPlot('net', 'Network Structure', type='network', layout='spring')
+net = viz.addPlot('net', 'Network Structure', type='agents', scatter=['s1', 's2'])
 bar1 = viz.addPlot('prop', 'Bar Chart')
 bar2 = viz.addPlot('prop2', 'Horizontal Bar Chart', horizontal=True)
 net.config({
 	'agentLabel': True,
  	'labelColor': '#FFFFFF',
 # 	'labelFamily': 'serif',
 	'agentMarker': 'H',
 	'labelAlpha': 0.75,
 	'labelWeight': 'bold',
- 	'labelSize': 8
+ 	'labelSize': 8,
+	'regLine': True
 })
 
 gcolors = ['F00', 'F03', 'F06', 'F09', 'F0C', 'C0F', '90F', '60F', '30F', '00F']
 for i in range(20):
 	heli.data.addReporter('prop'+str(i), heli.data.agentReporter('prop'+str(i), std=0.1))
 	(bar1 if i<10 else bar2).addBar('prop'+str(i), str(i), '#'+gcolors[i%10])
```

### Comparing `helipad-1.5.1/sample-models/crime.py` & `helipad-1.6/sample-models/crime.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 from helipad import Helipad, MultiLevel, Agent
 from math import floor
 from random import uniform, choice
 
 heli = Helipad()
 heli.name = 'Illicit Supply Chains'
-heli.order = 'random'
+heli.agents.order = 'random'
 
-heli.primitives.add('firm', MultiLevel, dflt=20, priority=1)
-heli.primitives.remove('agent')
+heli.agents.addPrimitive('firm', MultiLevel, dflt=20, priority=1)
+heli.agents.removePrimitive('agent')
 mapPlot = heli.spatial(dim=(5,1), wrap=False)
 mapPlot.config({
 	'patchProperty': 'x',
 	'patchAspect': 2
 })
 heli.params['x'].type = 'hidden'
 heli.params['y'].type = 'hidden'
@@ -44,15 +44,15 @@
 def modelPostSetup(model):
 	for n,a in enumerate(model.agents['firm']):
 		stage = floor(n/4)
 		a.moveTo(uniform(stage-0.4, stage+0.4), uniform(-0.5, 0.5))
 	
 	#Create links after all firms have been assigned to a stage
 	for f in model.agents['firm']:
-		if f.patch.x > 0: f.newEdge(choice(list(f.patch.left.agentsOn)))
+		if f.patch.x > 0: f.edges.add(choice(list(f.patch.left.agentsOn)))
 
 
 #===============
 # LAUNCH THE GUI
 #===============
 
 heli.launchCpanel()
```

### Comparing `helipad-1.5.1/sample-models/criticalperiod.py` & `helipad-1.6/sample-models/criticalperiod.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from helipad import Helipad, Agent
 import random
 from numpy.random import choice
 from numpy import mean
 
 heli = Helipad()
 heli.name = 'Critical Period'
-heli.order = 'random'
+heli.agents.order = 'random'
 
 heli.params.add('pleio', 'Pleiotropy', 'slider', dflt=7, opts={'low': 0, 'high': 10, 'step': 1}, runtime=False)
 heli.params.add('acq', 'Acquisition from', 'menu', dflt='mother', opts={'mother': 'Mother', 'wholepop': 'Whole Population'})
 heli.params.add('condition', 'Language affects', 'menu', dflt='rep', opts={'rep': 'Reproduction', 'srv': 'Survival'})
 
 heli.params['num_agent'].opts['step'] = 10 #Need it to be divisible by the number of life stages
 heli.params['num_agent'].opts['low'] = 10
@@ -78,16 +78,16 @@
 	#Or with equal probability in the survival condition
 	if heli.param('condition')=='rep':
 		nominees = []
 		for a in heli.agents['agent']:
 			if a.hasReproduced or a.age<=1: continue
 			for n in range(round(a.language**3+1)): nominees.append(a.id) #+1 because otherwise we start out with no one able to reproduce
 	else: nominees = [a.id for a in heli.agents['agent'] if not a.hasReproduced and a.age>1]
-	n1 = n2 = heli.agent(random.choice(nominees))
-	while n1.id == n2.id: n2 = heli.agent(random.choice(nominees))
+	n1 = n2 = heli.agents[random.choice(nominees)]
+	while n1.id == n2.id: n2 = heli.agents[random.choice(nominees)]
 	
 	#Complicated inheritance so do it manually
 	baby = n1.reproduce(partners=[n2])
 	parents = [n1, n2]
 	for n in parents:
 		n.gamete = []
 		inp = [n.dominantLap, n.recessivLap]
```

### Comparing `helipad-1.5.1/sample-models/demeSelection.py` & `helipad-1.6/sample-models/demeSelection.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from random import choice
 from math import exp
 from helipad import Helipad, MultiLevel
 import numpy.random as nprand
 
 heli = Helipad()
 heli.name = 'Deme Selection'
-heli.order = ['linear', 'linear', 'match']
+heli.agents.order = ['linear', 'linear', 'match']
 heli.stages = 3 #Stage 1 for intra-demic competition, stage 2 for reproduction, stage 3 for war
 
-heli.primitives.add('deme', MultiLevel, dflt=20, priority=1)
-heli.primitives.remove('agent')
+heli.agents.addPrimitive('deme', MultiLevel, dflt=20, priority=1)
+heli.agents.removePrimitive('agent')
 heli.params.add('b', 'Benefit conferred', 'slider', dflt=6, opts={'low': 0, 'high': 10, 'step': 1})
 heli.params.add('c', 'Cost incurred', 'slider', dflt=2, opts={'low': 0, 'high': 10, 'step': 1})
 heli.params.add('k', 'Likelihood of war', 'slider', dflt=0.25, opts={'low': 0, 'high': 1, 'step': 0.01})
 
 #===============
 # BEHAVIOR
 #===============
@@ -35,16 +35,16 @@
 		agent.stocks['payoff'] -= deme.model.param('c')
 		beneficiary.stocks['payoff'] += deme.model.param('b')
 
 #deme is the MultiLevel object, which inherits from both baseAgent and Helipad.
 @heli.hook
 def demeInit(deme, model):
 	deme.param('num_agent', 20)
-	deme.addBreed('altruist', '#009900')
-	deme.addBreed('selfish', '#990000')
+	deme.agents.addBreed('altruist', '#009900')
+	deme.agents.addBreed('selfish', '#990000')
 	deme.goods.add('payoff', '#000099', 1)
 	deme.hooks.add('agentStep', agentStep)
 
 #Odds of winning follow a sigmoid distribution in the difference in strength
 @heli.hook('demeMatch')
 def war(demes, primitive, model, stage):
 	k = model.param('k')
@@ -86,26 +86,26 @@
 
 from helipad.visualize import TimeSeries
 viz = heli.useVisual(TimeSeries)
 
 @heli.reporter
 def population(model): return sum(len(d.agents['agent']) for d in model.agents['deme'])
 @heli.reporter
-def altruists(model): return sum(len(d.agent('altruist')) for d in model.agents['deme'])/population(model)
+def altruists(model): return sum(len(d.agents['agent']['altruist']) for d in model.agents['deme'])/population(model)
 @heli.reporter
-def selfish(model): return sum(len(d.agent('selfish')) for d in model.agents['deme'])/population(model)
+def selfish(model): return sum(len(d.agents['agent']['selfish']) for d in model.agents['deme'])/population(model)
 @heli.reporter
 def fitness(model): return sum(sum(a.stocks['payoff'] for a in d.agents['agent']) for d in model.agents['deme'])/population(model)
 
 viz.addPlot('pop', 'Population', selected=False)
 viz.addPlot('pheno', 'Phenotypes', stack=True)
 viz.addPlot('fitness', 'Fitness')
-viz.plots['pop'].addSeries('population', 'Total population', '#000000')
-viz.plots['pheno'].addSeries('altruists', 'Altruists', '#33CC33')
-viz.plots['pheno'].addSeries('selfish', 'Selfish', '#BB2222')
-viz.plots['fitness'].addSeries('fitness', 'Average Fitness', '#000099')
+viz['pop'].addSeries('population', 'Total population', '#000000')
+viz['pheno'].addSeries('altruists', 'Altruists', '#33CC33')
+viz['pheno'].addSeries('selfish', 'Selfish', '#BB2222')
+viz['fitness'].addSeries('fitness', 'Average Fitness', '#000099')
 
 #===============
 # LAUNCH THE GUI
 #===============
 
 heli.launchCpanel()
```

### Comparing `helipad-1.5.1/sample-models/gameoflife.py` & `helipad-1.6/sample-models/gameoflife.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from random import getrandbits
 
 heli = Helipad()
 heli.name = 'Game of Life'
 heli.stages = 2
 heli.param('refresh', 1)
 
-heli.primitives.remove('agent')
+heli.agents.removePrimitive('agent')
 mapPlot = heli.spatial(dim=30, wrap=True, corners=True)
 mapPlot.config('patchProperty', 'active')
 
 def setdim(model, var, val): model.patches.dim = (int(val), int(val))
 heli.params.add('dim', 'Dimension', 'slider', 30, opts={'low': 4, 'high': 30, 'step': 1}, runtime=False, callback=setdim)
 
 @heli.hook
@@ -41,11 +41,11 @@
 
 @heli.button
 def Randomize(model):
 	if not model.hasModel: return
 	for p in model.agents['patch']:
 		p.active = bool(getrandbits(1))
 	if model.visual:
-		model.visual.plots['map'].update(None, model.t)
-		model.visual.plots['map'].draw(model.t, forceUpdate=True)
+		model.visual['map'].update(None, model.t)
+		model.visual['map'].draw(model.t, forceUpdate=True)
 
 heli.launchCpanel()
```

### Comparing `helipad-1.5.1/sample-models/grass.py` & `helipad-1.6/sample-models/grass.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 from random import choice, randint
 from numpy import mean
 from helipad import Helipad
 
 heli = Helipad()
 heli.name = 'Grass Eating'
-heli.order = 'random'
+heli.agents.order = 'random'
 heli.stages = 5
 
 heli.params.add('energy', 'Energy from grass', 'slider', dflt=2, opts={'low': 2, 'high': 10, 'step': 1})
 heli.params.add('smart', 'Smart consumption', 'check', dflt=True, desc='Move to the neighboring patch with the most grass, rather than randomly')
 heli.params.add('e2reproduce', 'Energy to reproduce', 'slider', dflt=25, opts={'low': 0, 'high': 100, 'step': 5})
 heli.params.add('maleportion', 'Male portion reproduction', 'slider', dflt=40, opts={'low': 0, 'high': 100, 'step': 5})
 heli.params.add('maxLife', 'Max Lifespan', 'slider', dflt=200, opts={'low': 100, 'high': 1000, 'step': 10})
 heli.params.add('grassrate', 'Grass Rate', 'slider', dflt=10, opts={'low': 1, 'high': 100, 'step': 1})
 
 heli.params['num_agent'].opts = {'low': 1, 'high': 200, 'step': 1}
 heli.param('num_agent', 200)
 
-heli.addBreed('male', 'blue')
-heli.addBreed('female', 'pink')
+heli.agents.addBreed('male', 'blue')
+heli.agents.addBreed('female', 'pink')
 heli.goods.add('energy', 'red', 5)
 
 #===============
 # BEHAVIOR
 #===============
 
 #Dividing it into stages like this (like in the NetLogo version) appears to make it more viable,
@@ -84,40 +84,44 @@
 
 @heli.hook
 def modelPostSetup(model):
 	model.deathAge = []
 
 #Stop the model when we have no more females left to reproduce
 @heli.event
-def nofemales(model): return len(model.agent('female')) <= 1
+def nofemales(model): return len(model.agents['agent']['female']) <= 1
 heli.param('stopafter', 'nofemales')
 heli.param('refresh', 1)
 
 #===============
 # DATA AND VISUALIZATION
 #===============
 
-# from helipad.visualize import TimeSeries
-# viz = heli.useVisual(TimeSeries)
-
 heli.data.addReporter('grass', heli.data.agentReporter('stocks', 'patch', good='energy', stat='sum'))
 heli.data.addReporter('age', heli.data.agentReporter('age', 'agent'))
 heli.data.addReporter('num_agent', lambda model: len(model.agents['agent']))
-heli.data.addReporter('sexratio', lambda model: len(model.agent('male', 'agent'))/len(model.agent('female', 'agent')))
+heli.data.addReporter('sexratio', lambda model: len(model.agents['agent']['male'])/len(model.agents['agent']['female']))
 heli.data.addReporter('expectancy', lambda model: mean(model.deathAge))
 heli.data.addReporter('agentenergy', heli.data.agentReporter('stocks', 'agent', good='energy', percentiles=[0,100]))
 
-mapPlot = heli.spatial(dim=(16, 8), corners=True, geometry='polar')
+mapPlot = heli.spatial(dim=16, corners=True)
+mapPlot.scatter = ['age', 'good:energy']
 mapPlot.config({
 	'patchProperty': 'good:energy',
 	'patchColormap': 'Greens',
-	'agentSize': 'good:energy',
-	'lockLayout': True
+	'agentSize': 'good:energy'
 })
 
+# # Only forward 0.368
+# import geopandas,os
+# __location__ = os.path.realpath(os.path.join(os.getcwd(), os.path.dirname(__file__)))
+# gdf = geopandas.read_file(os.path.join(__location__, 'NC_Counties.geojson'))
+# for i,county in gdf.iterrows():
+#     heli.patches.add(county['geometry'], county['CO_NAME'])
+
 pop = heli.visual.addPlot('pop', 'Population', 'timeseries', logscale=True, selected=False)
 sexratio = heli.visual.addPlot('sexratio', 'Sex Ratio', 'timeseries', logscale=True, selected=False)
 age = heli.visual.addPlot('age', 'Age', 'timeseries', selected=False)
 energy = heli.visual.addPlot('energy', 'Energy', 'timeseries', selected=False)
 
 pop.addSeries('num_agent', 'Population', 'black')
 pop.addSeries('grass', 'Grass', 'green')
@@ -128,14 +132,14 @@
 
 @heli.hook
 def agentClick(agent, plot, t):
 	print([f'Agent {a.id} at ({a.x}, {a.y})' for a in agent if a is not None])
 
 @heli.hook
 def patchClick(patch, plot, t):
-	print('Patch at',patch.position)
+	print(patch)
 
 #===============
 # LAUNCH THE GUI
 #===============
 
 heli.launchCpanel()
```

### Comparing `helipad-1.5.1/sample-models/pricediscover.py` & `helipad-1.6/sample-models/pricediscover.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from helipad import Helipad
 from helipad.utility import CobbDouglas
 from math import exp, floor
 import random
 
 heli = Helipad()
 heli.name = 'Price Discover'
-heli.order = 'match'
+heli.agents.order = 'match'
 
 heli.params.add('ratio', 'Log Endowment Ratio', 'slider', dflt=0, opts={'low': -3, 'high': 3, 'step': 0.5}, runtime=False)
 heli.params['num_agent'].opts['step'] = 2 #Make sure we don't get stray agents
 heli.params['num_agent'].opts['low'] = 2 #Make sure we don't get stray agents
 
 heli.goods.add('shmoo','#11CC00', (1, 1000))
 heli.goods.add('soma', '#CC0000', lambda breed: (1, floor(exp(heli.param('ratio'))*1000)))
@@ -71,11 +71,11 @@
 from helipad.visualize import TimeSeries
 viz = heli.useVisual(TimeSeries)
 
 heli.data.addReporter('ssprice', heli.data.agentReporter('lastPrice', 'agent', stat='gmean', percentiles=[0,100]))
 pricePlot = viz.addPlot('price', 'Price', logscale=True, selected=True)
 pricePlot.addSeries('ssprice', 'Soma/Shmoo Price', '#119900')
 
-for p in ['demand', 'utility']: viz.plots[p].active(True)
+for p in ['demand', 'utility']: viz[p].active(True)
 heli.param('refresh', 1)
 
 heli.launchCpanel()
```

### Comparing `helipad-1.5.1/sample-models/prisoners.py` & `helipad-1.6/sample-models/prisoners.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from random import shuffle, randint
 from helipad import Helipad
 from numpy import mean
 
 heli = Helipad()
 heli.name = 'Prison Escape'
-heli.order = 'random'
+heli.agents.order = 'random'
 
 heli.params.add('strategy', 'Optimal Strategy', 'check', dflt=True)
 heli.param('num_agent', 100)
 heli.params['num_agent'].type = 'hidden'
 heli.param('stopafter', 500)
 heli.cumAvg = 0
```

### Comparing `helipad-1.5.1/sample-notebooks/axelrod.ipynb` & `helipad-1.6/sample-notebooks/axelrod.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996980676328502%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(5, "heli.agents.order = \'match\'\\n")], delete: [5]}}, '*

 * *            '4: {\'source\': {insert: [(28, "\\tfor b in model.agents[\'agent\'].breeds:\\n"), '*

 * *            '(30, "\\tmodel.agents[\'agent\'].breeds.clear()\\n"), (33, '*

 * *            "'\\t\\tmodel.agents.addBreed(k, strategies[k][1])\\n'), (35, "*

 * *            '"\\tmodel.param(\'num_agent\', '*

 * *            "len(model.agents['agent'].breeds)*model.param('n')) #Three of each strategy, for "*

 * *            'speed\\n"), […]*

```diff
@@ -24,15 +24,15 @@
             "outputs": [],
             "source": [
                 "from helipad import Helipad\n",
                 "from numpy import mean, random\n",
                 "\n",
                 "heli = Helipad()\n",
                 "heli.name = 'Axelrod Tournament'\n",
-                "heli.order = 'match'\n",
+                "heli.agents.order = 'match'\n",
                 "\n",
                 "heli.params['num_agent'].type = 'hidden' #So we can postpone breed determination until the end\n",
                 "\n",
                 "#Initial parameter values match the payoffs in Table 1\n",
                 "heli.params.add('cc', 'C-C payoff', 'slider', dflt=3, opts={'low': 0, 'high': 10, 'step': 0.5})\n",
                 "heli.params.add('dc', 'D-C payoff', 'slider', dflt=5, opts={'low': 0, 'high': 10, 'step': 0.5})\n",
                 "heli.params.add('cd', 'C-D payoff', 'slider', dflt=0, opts={'low': 0, 'high': 10, 'step': 0.5})\n",
@@ -182,24 +182,24 @@
                 "plot = viz.addPlot('payoffs', 'Payoffs')\n",
                 "        \n",
                 "#Add breeds last-minute so we can toggle them in the control panel\n",
                 "@heli.hook\n",
                 "def modelPreSetup(model):\n",
                 "\t\n",
                 "\t#Clear breeds from the previous run\n",
-                "\tfor b in model.primitives['agent'].breeds:\n",
+                "\tfor b in model.agents['agent'].breeds:\n",
                 "\t\tmodel.data.removeReporter(b+'-proportion')\n",
-                "\tmodel.primitives['agent'].breeds.clear()\n",
+                "\tmodel.agents['agent'].breeds.clear()\n",
                 "\t\n",
                 "\tfor k in model.param('strategies'):\n",
-                "\t\tmodel.addBreed(k, strategies[k][1])\n",
+                "\t\tmodel.agents.addBreed(k, strategies[k][1])\n",
                 "\t\n",
-                "\tmodel.param('num_agent', len(model.primitives['agent'].breeds)*model.param('n')) #Three of each strategy, for speed\n",
+                "\tmodel.param('num_agent', len(model.agents['agent'].breeds)*model.param('n')) #Three of each strategy, for speed\n",
                 "\t\n",
-                "\tfor b, d in model.primitives['agent'].breeds.items():\n",
+                "\tfor b, d in model.agents['agent'].breeds.items():\n",
                 "\t\tmodel.data.addReporter(b+'-proportion', proportionReporter(b))\n",
                 "\t\tplot.addSeries(b+'-proportion', b, d.color)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `helipad-1.5.1/sample-notebooks/cpanel-test.ipynb` & `helipad-1.6/sample-notebooks/cpanel-test.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995205026455026%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(12, "\\theli.agents.addBreed(b[0], b[2], '*

 * *            'prim=\'agent\')\\n")], delete: [12]}}, 5: {\'source\': {insert: [(16, '*

 * *            "'\\tmodel.agents.createNetwork(0.2)\\n'), (21, "*

 * *            '"\\trandom.choice(model.agents.edges[\'edge\']).cut()\\n"), (23, "\\ta1, a2 = '*

 * *            'random.choice(model.agents[\'agent\']), random.choice(model.agents[\'agent\'])\\n"), '*

 * *            '(24, "\\twhile a1.edges.With(a2): a1, a2 = random.choice(model.agents[\'age […]*

```diff
@@ -25,15 +25,15 @@
                 "breeds = [\n",
                 "\t('hobbit', 'jam', '#D73229'),\n",
                 "\t('dwarf', 'axe', '#2D8DBE'),\n",
                 "\t('elf', 'lembas', '#CCBB22')\n",
                 "]\n",
                 "AgentGoods = {}\n",
                 "for b in breeds:\n",
-                "\theli.addBreed(b[0], b[2], prim='agent')\n",
+                "\theli.agents.addBreed(b[0], b[2], prim='agent')\n",
                 "\theli.goods.add(b[1], b[2])\n",
                 "\n",
                 "def gcallback(model, name, val):\n",
                 "\tprint(name, '=', val)\n",
                 "\n",
                 "def icallback(model, name, item, val):\n",
                 "\tprint(name, '/', item, '=', val)"
@@ -105,24 +105,24 @@
                 "def agentStep(agent, model, stage):\n",
                 "\tfor i in range(20):\n",
                 "\t\tv = getattr(agent, 'prop'+str(i))\n",
                 "\t\tsetattr(agent, 'prop'+str(i), v+1 if random.randint(0, 1) else v-1)\n",
                 "\n",
                 "@heli.hook\n",
                 "def modelPostSetup(model):\n",
-                "\tmodel.createNetwork(0.2)\n",
+                "\tmodel.agents.createNetwork(0.2)\n",
                 "\n",
                 "#Cut one edge and create one edge\n",
                 "@heli.hook\n",
                 "def modelPostStep(model):\n",
-                "\trandom.choice(model.allEdges['edge']).cut()\n",
+                "\trandom.choice(model.agents.edges['edge']).cut()\n",
                 "\t\n",
-                "\ta1, a2 = random.choice(list(model.allagents.values())), random.choice(list(model.allagents.values()))\n",
-                "\twhile a1.edgesWith(a2): a1, a2 = random.choice(list(model.allagents.values())), random.choice(list(model.allagents.values()))\n",
-                "\ta1.newEdge(a2, direction=random.choice([True, False]), weight=random.choice([0.5,1,2,3]))\n",
+                "\ta1, a2 = random.choice(model.agents['agent']), random.choice(model.agents['agent'])\n",
+                "\twhile a1.edges.With(a2): a1, a2 = random.choice(model.agents['agent']), random.choice(model.agents['agent'])\n",
+                "\ta1.edges.add(a2, direction=random.choice([True, False]), weight=random.choice([0.5,1,2,3]))\n",
                 "\n",
                 "viz.addPlot('net', 'Network Structure', type='network', layout='spring')\n",
                 "bar1 = viz.addPlot('prop', 'My Property')\n",
                 "bar2 = viz.addPlot('prop2', 'Horizontal Property', horizontal=True)\n",
                 "\n",
                 "gcolors = ['F00', 'F03', 'F06', 'F09', 'F0C', 'C0F', '90F', '60F', '30F', '00F']\n",
                 "for i in range(20):\n",
```

### Comparing `helipad-1.5.1/sample-notebooks/helicopter.ipynb` & `helipad-1.6/sample-notebooks/helicopter.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995729034565495%*

 * *Differences: {"'cells'": '{5: {\'source\': {insert: [(0, "heli.agents.addPrimitive(\'store\', Store, dflt=1, '*

 * *            'priority=2, hidden=True)\\n"), (1, "heli.agents.addPrimitive(\'agent\', Agent, '*

 * *            'dflt=50, low=1, high=100, priority=3)\\n"), (12, "\\theli.agents.addBreed(b[0], b[2], '*

 * *            'prim=\'agent\')\\n"), (19, "heli.agents.order = \'random\'\\n")], delete: [19, 12, 1, '*

 * *            '0]}}, 7: {\'source\': {insert: [(15, "viz[\'capital\'].addSeries(lambda t: '*

 * *            '1/len(heli.prim […]*

```diff
@@ -110,34 +110,34 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "heli.primitives.add('store', Store, dflt=1, priority=2, hidden=True)\n",
-                "heli.primitives.add('agent', Agent, dflt=50, low=1, high=100, priority=3)\n",
+                "heli.agents.addPrimitive('store', Store, dflt=1, priority=2, hidden=True)\n",
+                "heli.agents.addPrimitive('agent', Agent, dflt=50, low=1, high=100, priority=3)\n",
                 "\n",
                 "# Configure how many breeds there are and what good each consumes\n",
                 "# In this model, goods and breeds correspond, but they don't necessarily have to\n",
                 "breeds = [\n",
                 "\t('hobbit', 'jam', '#D73229'),\n",
                 "\t('dwarf', 'axe', '#2D8DBE'),\n",
                 "\t# ('elf', 'lembas', '#CCBB22')\n",
                 "]\n",
                 "AgentGoods = {}\n",
                 "for b in breeds:\n",
-                "\theli.addBreed(b[0], b[2], prim='agent')\n",
+                "\theli.agents.addBreed(b[0], b[2], prim='agent')\n",
                 "\theli.goods.add(b[1], b[2])\n",
                 "\tAgentGoods[b[0]] = b[1] #Hang on to this list for future looping\n",
                 "M0 = 120000\n",
                 "heli.goods.add('cash', '#009900', money=True)\n",
                 "\n",
                 "heli.name = 'Helicopter'\n",
-                "heli.order = 'random'\n",
+                "heli.agents.order = 'random'\n",
                 "\n",
                 "# UPDATE CALLBACKS\n",
                 "\n",
                 "def ngdpUpdater(model, var, val):\n",
                 "\tif model.hasModel: model.cb.ngdpTarget = val if not val else model.cb.ngdp\n",
                 "\n",
                 "def rbalUpdater(model, var, breed, val):\n",
@@ -202,62 +202,62 @@
                 "viz.addPlot('wage', 'Wage', 11, selected=False)\n",
                 "viz.addPlot('shortage', 'Shortages', 6, selected=False)\n",
                 "\n",
                 "def shortageReporter(good):\n",
                 "\tdef reporter(model): return model.shortages[good]\n",
                 "\treturn reporter\n",
                 "\n",
-                "viz.plots['capital'].addSeries(lambda t: 1/len(heli.primitives['agent'].breeds), '', '#CCCCCC')\n",
+                "viz['capital'].addSeries(lambda t: 1/len(heli.primitives['agent'].breeds), '', '#CCCCCC')\n",
                 "for breed, d in heli.primitives['agent'].breeds.items():\n",
                 "\theli.data.addReporter('rbalDemand-'+breed, rbaltodemand(breed))\n",
                 "\theli.data.addReporter('shortage-'+AgentGoods[breed], shortageReporter(AgentGoods[breed]))\n",
                 "\theli.data.addReporter('eCons-'+breed, heli.data.agentReporter('expCons', 'agent', breed=breed, stat='sum'))\n",
                 "\t# heli.data.addReporter('rWage-'+breed, lambda model: heli.data.agentReporter('wage', 'store')(model) / heli.data.agentReporter('price', 'store', good=b.good)(model))\n",
                 "\t# heli.data.addReporter('expWage', heli.data.agentReporter('expWage', 'agent'))\n",
                 "\theli.data.addReporter('rBal-'+breed, heli.data.agentReporter('realBalances', 'agent', breed=breed))\n",
                 "\theli.data.addReporter('invTarget-'+AgentGoods[breed], heli.data.agentReporter('invTarget', 'store', good=AgentGoods[breed]))\n",
                 "\theli.data.addReporter('portion-'+AgentGoods[breed], heli.data.agentReporter('portion', 'store', good=AgentGoods[breed]))\n",
                 "\n",
-                "\tviz.plots['demand'].addSeries('eCons-'+breed, breed.title()+'s\\' Expected Consumption', d.color2)\n",
-                "\tviz.plots['shortage'].addSeries('shortage-'+AgentGoods[breed], AgentGoods[breed].title()+' Shortage', d.color)\n",
-                "\tviz.plots['rbal'].addSeries('rbalDemand-'+breed, breed.title()+' Target Balances', d.color2)\n",
-                "\tviz.plots['rbal'].addSeries('rBal-'+breed, breed.title()+ 'Real Balances', d.color)\n",
-                "\tviz.plots['inventory'].addSeries('invTarget-'+AgentGoods[breed], AgentGoods[breed].title()+' Inventory Target', heli.goods[AgentGoods[breed]].color2)\n",
-                "\tviz.plots['capital'].addSeries('portion-'+AgentGoods[breed], AgentGoods[breed].title()+' Capital', heli.goods[AgentGoods[breed]].color)\n",
-                "\t# viz.plots['wage'].addSeries('expWage', 'Expected Wage', '#999999')\n",
+                "\tviz['demand'].addSeries('eCons-'+breed, breed.title()+'s\\' Expected Consumption', d.color2)\n",
+                "\tviz['shortage'].addSeries('shortage-'+AgentGoods[breed], AgentGoods[breed].title()+' Shortage', d.color)\n",
+                "\tviz['rbal'].addSeries('rbalDemand-'+breed, breed.title()+' Target Balances', d.color2)\n",
+                "\tviz['rbal'].addSeries('rBal-'+breed, breed.title()+ 'Real Balances', d.color)\n",
+                "\tviz['inventory'].addSeries('invTarget-'+AgentGoods[breed], AgentGoods[breed].title()+' Inventory Target', heli.goods[AgentGoods[breed]].color2)\n",
+                "\tviz['capital'].addSeries('portion-'+AgentGoods[breed], AgentGoods[breed].title()+' Capital', heli.goods[AgentGoods[breed]].color)\n",
+                "\t# viz['wage'].addSeries('expWage', 'Expected Wage', '#999999')\n",
                 "\n",
                 "#Do this one separately so it draws on top\n",
                 "for good, g in heli.goods.nonmonetary.items():\n",
                 "\theli.data.addReporter('inv-'+good, heli.data.agentReporter('stocks', 'store', good=good))\n",
-                "\tviz.plots['inventory'].addSeries('inv-'+good, good.title()+' Inventory', g.color)\n",
+                "\tviz['inventory'].addSeries('inv-'+good, good.title()+' Inventory', g.color)\n",
                 "\theli.data.addReporter('price-'+good, heli.data.agentReporter('price', 'store', good=good))\n",
-                "\tviz.plots['prices'].addSeries('price-'+good, good.title()+' Price', g.color)\n",
+                "\tviz['prices'].addSeries('price-'+good, good.title()+' Price', g.color)\n",
                 "\n",
                 "#Price ratio plots\n",
                 "def ratioReporter(item1, item2):\n",
                 "\tdef reporter(model):\n",
                 "\t\treturn model.data.agentReporter('price', 'store', good=item1)(model)/model.data.agentReporter('price', 'store', good=item2)(model)\n",
                 "\treturn reporter\n",
                 "viz.addPlot('ratios', 'Price Ratios', position=3, logscale=True)\n",
-                "viz.plots['ratios'].addSeries(lambda t: 1, '', '#CCCCCC')\t#plots ratio of 1 for reference without recording a column of ones\n",
+                "viz['ratios'].addSeries(lambda t: 1, '', '#CCCCCC')\t#plots ratio of 1 for reference without recording a column of ones\n",
                 "\n",
                 "for r in combinations(heli.goods.nonmonetary.keys(), 2):\n",
                 "\theli.data.addReporter('ratio-'+r[0]+'-'+r[1], ratioReporter(r[0], r[1]))\n",
                 "\tc1, c2 = heli.goods[r[0]].color, heli.goods[r[1]].color\n",
-                "\tviz.plots['ratios'].addSeries('ratio-'+r[0]+'-'+r[1], r[0].title()+'/'+r[1].title()+' Ratio', c1.blend(c2))\n",
+                "\tviz['ratios'].addSeries('ratio-'+r[0]+'-'+r[1], r[0].title()+'/'+r[1].title()+' Ratio', c1.blend(c2))\n",
                 "\n",
                 "#Misc plots\n",
                 "heli.data.addReporter('ngdp', lambda model: model.cb.ngdp)\n",
-                "viz.plots['ngdp'].addSeries('ngdp', 'NGDP', '#000000')\n",
+                "viz['ngdp'].addSeries('ngdp', 'NGDP', '#000000')\n",
                 "heli.data.addReporter('storeCash', heli.data.agentReporter('balance', 'store'))\n",
-                "viz.plots['money'].addSeries('storeCash', 'Store Cash', '#777777')\n",
+                "viz['money'].addSeries('storeCash', 'Store Cash', '#777777')\n",
                 "heli.data.addReporter('StoreCashDemand', heli.data.agentReporter('cashDemand', 'store'))\n",
-                "viz.plots['money'].addSeries('StoreCashDemand', 'Store Cash Demand', '#CCCCCC')\n",
+                "viz['money'].addSeries('StoreCashDemand', 'Store Cash Demand', '#CCCCCC')\n",
                 "heli.data.addReporter('wage', heli.data.agentReporter('wage', 'store'))\n",
-                "viz.plots['wage'].addSeries('wage', 'Wage', '#000000')"
+                "viz['wage'].addSeries('wage', 'Wage', '#000000')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Agent Behavior\n",
@@ -349,15 +349,15 @@
                 "\tdef expand(self, amount):\t\t\t\t\n",
                 "\t\tif self.model.param('dist') == 'lump':\n",
                 "\t\t\tamt = amount/self.model.param('num_agent')\n",
                 "\t\t\tfor a in self.model.agents['agent']:\n",
                 "\t\t\t\ta.stocks[self.model.goods.money] += amt\n",
                 "\t\telse:\n",
                 "\t\t\tM0 = self.M0\n",
-                "\t\t\tfor a in self.model.allagents.values():\n",
+                "\t\t\tfor a in self.model.agents.all:\n",
                 "\t\t\t\ta.stocks[self.model.goods.money] += a.stocks[self.model.goods.money]/M0 * amount\n",
                 "\t\t\t\t\n",
                 "\t@property\n",
                 "\tdef M0(self):\n",
                 "\t\treturn self.model.data.agentReporter('stocks', 'all', good=self.model.goods.money, stat='sum')(self.model)\n",
                 "\n",
                 "\t@M0.setter\n",
```

### Comparing `helipad-1.5.1/sample-notebooks/pricediscover.ipynb` & `helipad-1.6/sample-notebooks/pricediscover.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983826754385965%*

 * *Differences: {"'cells'": '{6: {\'source\': ["heli.agents.order = \'match\'"]}, 7: {\'source\': {insert: [(0, '*

 * *            '"This line configures the model to match agents each period and run them through a '*

 * *            "[`match`](https://helipad.dev/hooks/match) hook that we'll define later, rather than "*

 * *            "stepping through them individually. `'match'` is equivalent to `'match-2'`. We could "*

 * *            'also set [`heli.agents.order`](https://helipad.dev/functions/agents#order) to '*

 * *            "`'match-3' […]*

```diff
@@ -62,22 +62,23 @@
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [],
             "source": [
-                "heli.order = 'match'"
+                "heli.agents.order = 'match'"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This line configures the model to match agents each period and run them through a [`match`](https://helipad.dev/hooks/match) hook that we'll define later, rather than stepping through them individually. `'match'` is equivalent to `'match-2'`. We could also set [`heli.order`](https://helipad.dev/functions/model/#order) to `'match-3'` if we wanted it to group in triplets, or any other number. But for a trading model, and for most others, pairs are what we want.\n",
+                "This line configures the model to match agents each period and run them through a [`match`](https://helipad.dev/hooks/match) hook that we'll define later, rather than stepping through them individually. `'match'` is equivalent to `'match-2'`. We could also set [`heli.agents.order`](https://helipad.dev/functions/agents#order) to `'match-3'` if we wanted it to group in triplets, or any other number. But for a trading model, and for most others, pairs are what we want.\n",
                 "\n",
                 "For the others, we\u2019ll hook (1) and (2) into [agent initialization](https://helipad.dev/hooks/agentinit), (4) into [agent activation](https://helipad.dev/hooks/agentstep), and (5) we\u2019ll gather afterward.\n",
                 "\n",
                 "Starting with (1), we might want to control the aggregate ratio of shmoo to soma before each run. Helipad has a control panel on which we can place parameters that control the model. Before the function then, we\u2019ll tell the Helipad object to add a parameter that we can control, and whose value we can use in our agents\u2019 logic."
             ]
         },
         {
@@ -361,15 +362,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {},
             "outputs": [],
             "source": [
-                "for p in ['demand', 'utility']: viz.plots[p].active(True)"
+                "for p in ['demand', 'utility']: viz[p].active(True)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We also set the refresh rate parameter to 1 in order to see it play out live. Ordinarily this would make the model quite slow, but because it equilibrates so quickly (less than 20 periods), the default refresh rate of 20 would just show the final result."
```

### Comparing `helipad-1.5.1/sample-notebooks/viz-tutorial.ipynb` & `helipad-1.6/sample-notebooks/viz-tutorial.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998638344226579%*

 * *Differences: {"'cells'": '{2: {\'source\': {insert: [(4, "heli.agents.order = \'random\'\\n")], delete: [4]}}}'}*

```diff
@@ -29,15 +29,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "from helipad import Helipad\n",
                 "heli = Helipad()\n",
                 "\n",
                 "heli.name = '3D Spatial Visualizer'\n",
-                "heli.order = 'random'\n",
+                "heli.agents.order = 'random'\n",
                 "\n",
                 "mapPlot = heli.spatial(dim=20, diag=False, wrap=True)\n",
                 "mapPlot.remove()"
             ]
         },
         {
             "cell_type": "markdown",
```

