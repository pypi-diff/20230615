# Comparing `tmp/nomspectra-0.3.12.tar.gz` & `tmp/nomspectra-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomspectra-0.3.12.tar", last modified: Sat Apr  1 14:55:13 2023, max compression
+gzip compressed data, was "nomspectra-1.0.0.tar", last modified: Thu Jun 15 12:18:04 2023, max compression
```

## Comparing `nomspectra-0.3.12.tar` & `nomspectra-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 av         (501) staff       (20)        0 2023-04-01 14:55:13.346347 nomspectra-0.3.12/
--rw-r--r--   0 av         (501) staff       (20)    35121 2022-10-26 04:38:04.000000 nomspectra-0.3.12/LICENSE.txt
--rw-r--r--   0 av         (501) staff       (20)     3492 2023-04-01 14:55:13.346447 nomspectra-0.3.12/PKG-INFO
--rw-r--r--   0 av         (501) staff       (20)     2934 2023-03-21 07:22:31.000000 nomspectra-0.3.12/README.md
-drwxr-xr-x   0 av         (501) staff       (20)        0 2023-04-01 14:55:13.345257 nomspectra-0.3.12/nomspectra/
--rw-r--r--   0 av         (501) staff       (20)        0 2023-03-21 07:22:31.000000 nomspectra-0.3.12/nomspectra/__init__.py
--rw-r--r--   0 av         (501) staff       (20)      162 2023-03-21 07:22:31.000000 nomspectra-0.3.12/nomspectra/__main__.py
--rw-r--r--   0 av         (501) staff       (20)       22 2023-04-01 12:35:20.000000 nomspectra-0.3.12/nomspectra/__version__.py
--rw-r--r--   0 av         (501) staff       (20)    22061 2023-03-21 07:22:31.000000 nomspectra-0.3.12/nomspectra/brutto.py
--rw-r--r--   0 av         (501) staff       (20)    11874 2023-03-21 07:22:31.000000 nomspectra-0.3.12/nomspectra/diff.py
--rw-r--r--   0 av         (501) staff       (20)    17187 2023-03-21 07:22:31.000000 nomspectra-0.3.12/nomspectra/draw.py
--rw-r--r--   0 av         (501) staff       (20)    45694 2023-04-01 14:08:17.000000 nomspectra-0.3.12/nomspectra/gui.py
--rw-r--r--   0 av         (501) staff       (20)    63747 2023-04-01 14:05:36.000000 nomspectra-0.3.12/nomspectra/gui_design.py
--rw-r--r--   0 av         (501) staff       (20)     3898 2023-03-21 07:22:31.000000 nomspectra-0.3.12/nomspectra/gui_dialog.py
--rw-r--r--   0 av         (501) staff       (20)     3223 2023-03-21 07:22:31.000000 nomspectra-0.3.12/nomspectra/metadata.py
--rw-r--r--   0 av         (501) staff       (20)    14097 2023-03-31 07:34:04.000000 nomspectra-0.3.12/nomspectra/recal.py
--rw-r--r--   0 av         (501) staff       (20)    11378 2023-03-21 07:22:31.000000 nomspectra-0.3.12/nomspectra/spectra.py
--rw-r--r--   0 av         (501) staff       (20)    56128 2023-04-01 14:55:00.000000 nomspectra-0.3.12/nomspectra/spectrum.py
-drwxr-xr-x   0 av         (501) staff       (20)        0 2023-04-01 14:55:13.346186 nomspectra-0.3.12/nomspectra.egg-info/
--rw-r--r--   0 av         (501) staff       (20)     3492 2023-04-01 14:55:12.000000 nomspectra-0.3.12/nomspectra.egg-info/PKG-INFO
--rw-r--r--   0 av         (501) staff       (20)      496 2023-04-01 14:55:13.000000 nomspectra-0.3.12/nomspectra.egg-info/SOURCES.txt
--rw-r--r--   0 av         (501) staff       (20)        1 2023-04-01 14:55:12.000000 nomspectra-0.3.12/nomspectra.egg-info/dependency_links.txt
--rw-r--r--   0 av         (501) staff       (20)      218 2023-04-01 14:55:13.000000 nomspectra-0.3.12/nomspectra.egg-info/requires.txt
--rw-r--r--   0 av         (501) staff       (20)       11 2023-04-01 14:55:13.000000 nomspectra-0.3.12/nomspectra.egg-info/top_level.txt
--rw-r--r--   0 av         (501) staff       (20)       79 2023-04-01 14:55:13.346740 nomspectra-0.3.12/setup.cfg
--rw-r--r--   0 av         (501) staff       (20)     1470 2023-03-21 07:22:31.000000 nomspectra-0.3.12/setup.py
+drwxr-xr-x   0 av         (501) staff       (20)        0 2023-06-15 12:18:04.941666 nomspectra-1.0.0/
+-rw-r--r--   0 av         (501) staff       (20)    35121 2022-10-26 04:38:04.000000 nomspectra-1.0.0/LICENSE.txt
+-rw-r--r--   0 av         (501) staff       (20)     3735 2023-06-15 12:18:04.941728 nomspectra-1.0.0/PKG-INFO
+-rw-r--r--   0 av         (501) staff       (20)     3178 2023-06-15 12:16:36.000000 nomspectra-1.0.0/README.md
+drwxr-xr-x   0 av         (501) staff       (20)        0 2023-06-15 12:18:04.940893 nomspectra-1.0.0/nomspectra/
+-rw-r--r--   0 av         (501) staff       (20)        0 2023-03-21 07:22:31.000000 nomspectra-1.0.0/nomspectra/__init__.py
+-rw-r--r--   0 av         (501) staff       (20)      162 2023-03-21 07:22:31.000000 nomspectra-1.0.0/nomspectra/__main__.py
+-rw-r--r--   0 av         (501) staff       (20)       21 2023-06-15 12:16:47.000000 nomspectra-1.0.0/nomspectra/__version__.py
+-rw-r--r--   0 av         (501) staff       (20)    22061 2023-03-21 07:22:31.000000 nomspectra-1.0.0/nomspectra/brutto.py
+-rw-r--r--   0 av         (501) staff       (20)    11874 2023-03-21 07:22:31.000000 nomspectra-1.0.0/nomspectra/diff.py
+-rw-r--r--   0 av         (501) staff       (20)    17187 2023-03-21 07:22:31.000000 nomspectra-1.0.0/nomspectra/draw.py
+-rw-r--r--   0 av         (501) staff       (20)    45689 2023-06-15 12:16:43.000000 nomspectra-1.0.0/nomspectra/gui.py
+-rw-r--r--   0 av         (501) staff       (20)    63747 2023-04-01 14:05:36.000000 nomspectra-1.0.0/nomspectra/gui_design.py
+-rw-r--r--   0 av         (501) staff       (20)     3898 2023-03-21 07:22:31.000000 nomspectra-1.0.0/nomspectra/gui_dialog.py
+-rw-r--r--   0 av         (501) staff       (20)     3223 2023-03-21 07:22:31.000000 nomspectra-1.0.0/nomspectra/metadata.py
+-rw-r--r--   0 av         (501) staff       (20)    14097 2023-03-31 07:34:04.000000 nomspectra-1.0.0/nomspectra/recal.py
+-rw-r--r--   0 av         (501) staff       (20)    11378 2023-03-21 07:22:31.000000 nomspectra-1.0.0/nomspectra/spectra.py
+-rw-r--r--   0 av         (501) staff       (20)    56128 2023-04-02 08:55:35.000000 nomspectra-1.0.0/nomspectra/spectrum.py
+drwxr-xr-x   0 av         (501) staff       (20)        0 2023-06-15 12:18:04.941560 nomspectra-1.0.0/nomspectra.egg-info/
+-rw-r--r--   0 av         (501) staff       (20)     3735 2023-06-15 12:18:04.000000 nomspectra-1.0.0/nomspectra.egg-info/PKG-INFO
+-rw-r--r--   0 av         (501) staff       (20)      496 2023-06-15 12:18:04.000000 nomspectra-1.0.0/nomspectra.egg-info/SOURCES.txt
+-rw-r--r--   0 av         (501) staff       (20)        1 2023-06-15 12:18:04.000000 nomspectra-1.0.0/nomspectra.egg-info/dependency_links.txt
+-rw-r--r--   0 av         (501) staff       (20)      218 2023-06-15 12:18:04.000000 nomspectra-1.0.0/nomspectra.egg-info/requires.txt
+-rw-r--r--   0 av         (501) staff       (20)       11 2023-06-15 12:18:04.000000 nomspectra-1.0.0/nomspectra.egg-info/top_level.txt
+-rw-r--r--   0 av         (501) staff       (20)       79 2023-06-15 12:18:04.941922 nomspectra-1.0.0/setup.cfg
+-rw-r--r--   0 av         (501) staff       (20)     1470 2023-03-21 07:22:31.000000 nomspectra-1.0.0/setup.py
```

### Comparing `nomspectra-0.3.12/LICENSE.txt` & `nomspectra-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nomspectra-0.3.12/PKG-INFO` & `nomspectra-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomspectra
-Version: 0.3.12
+Version: 1.0.0
 Summary: Lib for working with high resolution mass spectra
 Home-page: https://github.com/nomspectra/nomspectra
 Author: Volikov Alexander, Rukhovich Gleb
 Author-email: ab.volikov@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -15,22 +15,23 @@
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 
 [![PyPI](https://img.shields.io/pypi/v/nomspectra)](https://pypi.org/project/nomspectra/)
 [![Documentation Status](https://readthedocs.org/projects/nomspectra/badge/?version=latest)](https://nomspectra.readthedocs.io/en/latest/?badge=latest)
 [![Python package](https://github.com/nomspectra/nomspectra/actions/workflows/python-package.yml/badge.svg)](https://github.com/nomspectra/nomspectra/actions/workflows/python-package.yml)
+[![DOI](https://img.shields.io/badge/DOI-10.1021%2Fjasms.3c00003-blue)](https://doi.org/10.1021/jasms.3c00003)
 
 # nomspectra
 
 ![logo](https://github.com/nomspectra/nomspectra/raw/master/docs/_static/nomspectra_logo.png)
 
 nomspectra is an open-source Python package for processing high resolution mass spectra. The name is an acronym for Natural Organic Matter & Humic Substances Mass Spectrometry, so package designed for analysis natural organic matter (NOM) which are represent such substances as dissolve organic matter (DOM), humic substances, lignin, biochar and other objects of oxidative destruction of natural compounds which are characterized by thousands of signals in the mass spectrum and require special methods for analysis. The package implements a full-fledged workflow for processing, analysis and visualization of mass spectrum. Various algorithms for filtering spectra, recalibrating and assignment of elemental composition to ions are presented. The package implements methods for calculating different molecular descriptors and methods for data visualization. A graphical user interface (GUI) for package has been implemented, which makes this package convenient for a wide range of users.
 
-Main operation:
+## Main operation
 
 - Assigning element composition to signal by mass with desirable ranges of elements (include isotopes)
 - Fine recalibrate spectrum
 - Working with spectra as with sets (intersection, union, etc.)
 - Plot spectrum and different kind of scatter and density diagram such as Van Krevelen diagram
 - Calculate similarity metrics between spectra
 - Calculate molecular descriptors (DBE, AI, NOSC, CRAM and other) for spectra
@@ -67,7 +68,11 @@
 
 If you want to ask question or contribute to the development of nomspectra, have a look at the [contribution guidelines](https://github.com/nomspectra/nomspectra/blob/master/CONTRIBUTING.md).
 
 ## License
 
 Distributed under [license GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html)
 
+## Citate us
+
+When using NOMspectra, please cite : [https://doi.org/10.1021/jasms.3c00003](https://doi.org/10.1021/jasms.3c00003)
+
```

### Comparing `nomspectra-0.3.12/README.md` & `nomspectra-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 
 [![PyPI](https://img.shields.io/pypi/v/nomspectra)](https://pypi.org/project/nomspectra/)
 [![Documentation Status](https://readthedocs.org/projects/nomspectra/badge/?version=latest)](https://nomspectra.readthedocs.io/en/latest/?badge=latest)
 [![Python package](https://github.com/nomspectra/nomspectra/actions/workflows/python-package.yml/badge.svg)](https://github.com/nomspectra/nomspectra/actions/workflows/python-package.yml)
+[![DOI](https://img.shields.io/badge/DOI-10.1021%2Fjasms.3c00003-blue)](https://doi.org/10.1021/jasms.3c00003)
 
 # nomspectra
 
 ![logo](https://github.com/nomspectra/nomspectra/raw/master/docs/_static/nomspectra_logo.png)
 
 nomspectra is an open-source Python package for processing high resolution mass spectra. The name is an acronym for Natural Organic Matter & Humic Substances Mass Spectrometry, so package designed for analysis natural organic matter (NOM) which are represent such substances as dissolve organic matter (DOM), humic substances, lignin, biochar and other objects of oxidative destruction of natural compounds which are characterized by thousands of signals in the mass spectrum and require special methods for analysis. The package implements a full-fledged workflow for processing, analysis and visualization of mass spectrum. Various algorithms for filtering spectra, recalibrating and assignment of elemental composition to ions are presented. The package implements methods for calculating different molecular descriptors and methods for data visualization. A graphical user interface (GUI) for package has been implemented, which makes this package convenient for a wide range of users.
 
-Main operation:
+## Main operation
 
 - Assigning element composition to signal by mass with desirable ranges of elements (include isotopes)
 - Fine recalibrate spectrum
 - Working with spectra as with sets (intersection, union, etc.)
 - Plot spectrum and different kind of scatter and density diagram such as Van Krevelen diagram
 - Calculate similarity metrics between spectra
 - Calculate molecular descriptors (DBE, AI, NOSC, CRAM and other) for spectra
@@ -48,8 +49,12 @@
 
 ## How to contribute or ask question
 
 If you want to ask question or contribute to the development of nomspectra, have a look at the [contribution guidelines](https://github.com/nomspectra/nomspectra/blob/master/CONTRIBUTING.md).
 
 ## License
 
-Distributed under [license GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html)
+Distributed under [license GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html)
+
+## Citate us
+
+When using NOMspectra, please cite : [https://doi.org/10.1021/jasms.3c00003](https://doi.org/10.1021/jasms.3c00003)
```

### Comparing `nomspectra-0.3.12/nomspectra/brutto.py` & `nomspectra-1.0.0/nomspectra/brutto.py`

 * *Files identical despite different names*

### Comparing `nomspectra-0.3.12/nomspectra/diff.py` & `nomspectra-1.0.0/nomspectra/diff.py`

 * *Files identical despite different names*

### Comparing `nomspectra-0.3.12/nomspectra/draw.py` & `nomspectra-1.0.0/nomspectra/draw.py`

 * *Files identical despite different names*

### Comparing `nomspectra-0.3.12/nomspectra/gui.py` & `nomspectra-1.0.0/nomspectra/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,16 @@
 
 about =f'''nomspectra. Version {version["__version__"]}
 
 Graphical user interface for nomspectra package: https://github.com/nomspectra/nomspectra
 
 Tutorial: https://nomspectra.readthedocs.io/en/latest/gui_tutorial.html
 
-Distributed under license GPLv3 http://www.gnu.org/licenses/
+Cite NOMspectra: https://doi.org/10.1021/jasms.3c00003
+
 '''
 
 def_colors = ['blue','red','green','orange','purple','brown','pink','gray','olive','cyan']
 
 class ListDialog(QtWidgets.QDialog, Ui_Dialog):
     def __init__(self, spec = None):
         super().__init__()
```

### Comparing `nomspectra-0.3.12/nomspectra/gui_design.py` & `nomspectra-1.0.0/nomspectra/gui_design.py`

 * *Files identical despite different names*

### Comparing `nomspectra-0.3.12/nomspectra/gui_dialog.py` & `nomspectra-1.0.0/nomspectra/gui_dialog.py`

 * *Files identical despite different names*

### Comparing `nomspectra-0.3.12/nomspectra/metadata.py` & `nomspectra-1.0.0/nomspectra/metadata.py`

 * *Files identical despite different names*

### Comparing `nomspectra-0.3.12/nomspectra/recal.py` & `nomspectra-1.0.0/nomspectra/recal.py`

 * *Files identical despite different names*

### Comparing `nomspectra-0.3.12/nomspectra/spectra.py` & `nomspectra-1.0.0/nomspectra/spectra.py`

 * *Files identical despite different names*

### Comparing `nomspectra-0.3.12/nomspectra/spectrum.py` & `nomspectra-1.0.0/nomspectra/spectrum.py`

 * *Files identical despite different names*

### Comparing `nomspectra-0.3.12/nomspectra.egg-info/PKG-INFO` & `nomspectra-1.0.0/nomspectra.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomspectra
-Version: 0.3.12
+Version: 1.0.0
 Summary: Lib for working with high resolution mass spectra
 Home-page: https://github.com/nomspectra/nomspectra
 Author: Volikov Alexander, Rukhovich Gleb
 Author-email: ab.volikov@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -15,22 +15,23 @@
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 
 [![PyPI](https://img.shields.io/pypi/v/nomspectra)](https://pypi.org/project/nomspectra/)
 [![Documentation Status](https://readthedocs.org/projects/nomspectra/badge/?version=latest)](https://nomspectra.readthedocs.io/en/latest/?badge=latest)
 [![Python package](https://github.com/nomspectra/nomspectra/actions/workflows/python-package.yml/badge.svg)](https://github.com/nomspectra/nomspectra/actions/workflows/python-package.yml)
+[![DOI](https://img.shields.io/badge/DOI-10.1021%2Fjasms.3c00003-blue)](https://doi.org/10.1021/jasms.3c00003)
 
 # nomspectra
 
 ![logo](https://github.com/nomspectra/nomspectra/raw/master/docs/_static/nomspectra_logo.png)
 
 nomspectra is an open-source Python package for processing high resolution mass spectra. The name is an acronym for Natural Organic Matter & Humic Substances Mass Spectrometry, so package designed for analysis natural organic matter (NOM) which are represent such substances as dissolve organic matter (DOM), humic substances, lignin, biochar and other objects of oxidative destruction of natural compounds which are characterized by thousands of signals in the mass spectrum and require special methods for analysis. The package implements a full-fledged workflow for processing, analysis and visualization of mass spectrum. Various algorithms for filtering spectra, recalibrating and assignment of elemental composition to ions are presented. The package implements methods for calculating different molecular descriptors and methods for data visualization. A graphical user interface (GUI) for package has been implemented, which makes this package convenient for a wide range of users.
 
-Main operation:
+## Main operation
 
 - Assigning element composition to signal by mass with desirable ranges of elements (include isotopes)
 - Fine recalibrate spectrum
 - Working with spectra as with sets (intersection, union, etc.)
 - Plot spectrum and different kind of scatter and density diagram such as Van Krevelen diagram
 - Calculate similarity metrics between spectra
 - Calculate molecular descriptors (DBE, AI, NOSC, CRAM and other) for spectra
@@ -67,7 +68,11 @@
 
 If you want to ask question or contribute to the development of nomspectra, have a look at the [contribution guidelines](https://github.com/nomspectra/nomspectra/blob/master/CONTRIBUTING.md).
 
 ## License
 
 Distributed under [license GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html)
 
+## Citate us
+
+When using NOMspectra, please cite : [https://doi.org/10.1021/jasms.3c00003](https://doi.org/10.1021/jasms.3c00003)
+
```

### Comparing `nomspectra-0.3.12/setup.py` & `nomspectra-1.0.0/setup.py`

 * *Files identical despite different names*

