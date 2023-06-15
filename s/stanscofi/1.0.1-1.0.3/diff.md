# Comparing `tmp/stanscofi-1.0.1.tar.gz` & `tmp/stanscofi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stanscofi-1.0.1.tar", last modified: Sat Jun 10 09:57:21 2023, max compression
+gzip compressed data, was "stanscofi-1.0.3.tar", last modified: Thu Jun 15 15:37:43 2023, max compression
```

## Comparing `stanscofi-1.0.1.tar` & `stanscofi-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:57:21.872101 stanscofi-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-10 09:57:21.872101 stanscofi-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-06-10 09:57:13.000000 stanscofi-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-10 09:57:13.000000 stanscofi-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 09:57:21.872101 stanscofi-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-10 09:57:13.000000 stanscofi-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:57:21.872101 stanscofi-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:57:21.872101 stanscofi-1.0.1/src/stanscofi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:57:13.000000 stanscofi-1.0.1/src/stanscofi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25010 2023-06-10 09:57:13.000000 stanscofi-1.0.1/src/stanscofi/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-06-10 09:57:13.000000 stanscofi-1.0.1/src/stanscofi/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    15943 2023-06-10 09:57:13.000000 stanscofi-1.0.1/src/stanscofi/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-06-10 09:57:13.000000 stanscofi-1.0.1/src/stanscofi/training_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19709 2023-06-10 09:57:13.000000 stanscofi-1.0.1/src/stanscofi/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-06-10 09:57:13.000000 stanscofi-1.0.1/src/stanscofi/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:57:21.872101 stanscofi-1.0.1/src/stanscofi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-10 09:57:21.000000 stanscofi-1.0.1/src/stanscofi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-10 09:57:21.000000 stanscofi-1.0.1/src/stanscofi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 09:57:21.000000 stanscofi-1.0.1/src/stanscofi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-10 09:57:21.000000 stanscofi-1.0.1/src/stanscofi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-10 09:57:21.000000 stanscofi-1.0.1/src/stanscofi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:37:43.465273 stanscofi-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-15 15:37:43.461273 stanscofi-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-15 15:37:33.000000 stanscofi-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 15:37:33.000000 stanscofi-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 15:37:43.465273 stanscofi-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-15 15:37:33.000000 stanscofi-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:37:43.461273 stanscofi-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:37:43.461273 stanscofi-1.0.3/src/stanscofi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:37:33.000000 stanscofi-1.0.3/src/stanscofi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25010 2023-06-15 15:37:33.000000 stanscofi-1.0.3/src/stanscofi/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18449 2023-06-15 15:37:33.000000 stanscofi-1.0.3/src/stanscofi/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15943 2023-06-15 15:37:33.000000 stanscofi-1.0.3/src/stanscofi/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-06-15 15:37:33.000000 stanscofi-1.0.3/src/stanscofi/training_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19709 2023-06-15 15:37:33.000000 stanscofi-1.0.3/src/stanscofi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-06-15 15:37:33.000000 stanscofi-1.0.3/src/stanscofi/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:37:43.461273 stanscofi-1.0.3/src/stanscofi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-15 15:37:43.000000 stanscofi-1.0.3/src/stanscofi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-15 15:37:43.000000 stanscofi-1.0.3/src/stanscofi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:37:43.000000 stanscofi-1.0.3/src/stanscofi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-15 15:37:43.000000 stanscofi-1.0.3/src/stanscofi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 15:37:43.000000 stanscofi-1.0.3/src/stanscofi.egg-info/top_level.txt
```

### Comparing `stanscofi-1.0.1/PKG-INFO` & `stanscofi-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: stanscofi
-Version: 1.0.1
+Version: 1.0.3
 Summary: Package for STANdard drug Screening by COllaborative FIltering. Performs benchmarks against datasets and SotA algorithms, and implements training, validation and testing procedures.
 Home-page: https://github.com/RECeSS-EU-Project/stanscofi
 Author: Clémence Réda
 Author-email: recess-project@proton.me
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8.5
 Description-Content-Type: text/markdown
 
+![funding logo](https://raw.githubusercontent.com/RECeSS-EU-Project/RECeSS-EU-Project.github.io/main/assets/images/header%2BEU_rescale.jpg)
+
 # STANdard for drug Screening by COllaborative FIltering (stanscofi) Python Package
 
 This repository is a part of the EU-funded [RECeSS project](https://recess-eu-project.github.io) (#101102016), and hosts the code for the open-source Python package *stanscofi* for the development of collaborative filtering-based drug repurposing algorithms.
 
+[![Anaconda version](https://anaconda.org/recess/stanscofi/badges/version.svg)](https://anaconda.org/recess/stanscofi) [![PyPI version](https://badge.fury.io/py/stanscofi.svg)](https://badge.fury.io/py/stanscofi) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.8038847.svg)](https://doi.org/10.5281/zenodo.8038847)
+
 ## Statement of need
 
 As of 2022, current drug development pipelines last around 10 years, costing $2billion in average, while drug commercialization failure rates go up to 90%. These issues can be mitigated by drug repurposing, where chemical compounds are screened for new therapeutic indications in a systematic fashion. In prior works, this approach has been implemented through collaborative filtering. This semi-supervised learning framework leverages known drug-disease matchings in order to recommend new ones.
 
 The **stanscofi** package comprises method-agnostic training, validation, preprocessing and visualization procedures on several published drug repurposing datasets. The proper implementation of these steps is crucial in order to avoid data leakage, *i*.*e*., the model is learnt over information that should be unavailable at prediction time. Indeed, data leakage is the source of a major reproducibility crisis in machine learning. This will be avoided by building training and validation sets which are weakly correlated with respect to the drug and disease feature vectors. The main performance metric will be the area under the curve (AUC), which estimates the diagnostic ability of a recommender system better than accuracy in imbalanced datasets.
 
 Medium-term outcomes to this package will significantly alleviate the economic burden of drug discovery pipelines, and will help find treatments in a more sustainable manner, especially for rare or tropical neglected diseases.
@@ -74,27 +78,27 @@
 python3 -m pip install stanscofi ## or use the conda command above
 python3 -m pip install notebook>=6.5.4 markupsafe==2.0.1 ## packages for Jupyter notebook
 conda deactivate
 conda activate stanscofi_env
 cd docs/ && jupyter notebook
 ```
 
-The complete list of dependencies for *stanscofi* can be found at [requirements.txt](https://raw.githubusercontent.com/RECeSS-EU-Project/stanscofi/master/recipes/pip/requirements.txt) (pip) or [meta.yaml](https://raw.githubusercontent.com/RECeSS-EU-Project/stanscofi/master/recipes/conda/meta.yaml) (conda).
+The complete list of dependencies for *stanscofi* can be found at [requirements.txt](https://raw.githubusercontent.com/RECeSS-EU-Project/stanscofi/master/pip/requirements.txt) (pip) or [meta.yaml](https://raw.githubusercontent.com/RECeSS-EU-Project/stanscofi/master/conda/meta.yaml) (conda).
 
 ## Licence
 
 This repository is under an [OSI-approved](https://opensource.org/licenses/) [MIT license](https://raw.githubusercontent.com/RECeSS-EU-Project/stanscofi/master/LICENSE). 
 
 ## Citation
 
 If you use **stanscofi** in academic research, please cite it as follows
 
 ```
-Clémence Réda. (2023). 
-stanscofi: a Python package for the development of collaborative filtering-based drug repurposing algorithms (v1.0.0). 
-Zenodo. https://doi.org/10.5281/zenodo.8020433
+Réda, Clémence. (2023). 
+STANdard for drug Screening by COllaborative FIltering (stanscofi). 
+Zenodo. https://doi.org/10.5281/zenodo.8038847
 ```
 
 ## Community guidelines with respect to contributions, issue reporting, and support
 
-[Pull requests](https://github.com/RECeSS-EU-Project/stanscofi/pulls) and [issue flagging](https://github.com/RECeSS-EU-Project/stanscofi/issues) are welcome, and can be made through the GitHub interface. Support can be provided by reaching out to recess-project-at-proton.me. However, please note that contributors and users must abide by the [Code of Conduct](https://github.com/RECeSS-EU-Project/stanscofi/blob/master/CODE%20OF%20CONDUCT.md).
+[Pull requests](https://github.com/RECeSS-EU-Project/stanscofi/pulls) and [issue flagging](https://github.com/RECeSS-EU-Project/stanscofi/issues) are welcome, and can be made through the GitHub interface. Support can be provided by reaching out to ``recess-project[at]proton.me``. However, please note that contributors and users must abide by the [Code of Conduct](https://github.com/RECeSS-EU-Project/stanscofi/blob/master/CODE%20OF%20CONDUCT.md).
```

### Comparing `stanscofi-1.0.1/README.md` & `stanscofi-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+![funding logo](https://raw.githubusercontent.com/RECeSS-EU-Project/RECeSS-EU-Project.github.io/main/assets/images/header%2BEU_rescale.jpg)
+
 # STANdard for drug Screening by COllaborative FIltering (stanscofi) Python Package
 
 This repository is a part of the EU-funded [RECeSS project](https://recess-eu-project.github.io) (#101102016), and hosts the code for the open-source Python package *stanscofi* for the development of collaborative filtering-based drug repurposing algorithms.
 
+[![Anaconda version](https://anaconda.org/recess/stanscofi/badges/version.svg)](https://anaconda.org/recess/stanscofi) [![PyPI version](https://badge.fury.io/py/stanscofi.svg)](https://badge.fury.io/py/stanscofi) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.8038847.svg)](https://doi.org/10.5281/zenodo.8038847)
+
 ## Statement of need
 
 As of 2022, current drug development pipelines last around 10 years, costing $2billion in average, while drug commercialization failure rates go up to 90%. These issues can be mitigated by drug repurposing, where chemical compounds are screened for new therapeutic indications in a systematic fashion. In prior works, this approach has been implemented through collaborative filtering. This semi-supervised learning framework leverages known drug-disease matchings in order to recommend new ones.
 
 The **stanscofi** package comprises method-agnostic training, validation, preprocessing and visualization procedures on several published drug repurposing datasets. The proper implementation of these steps is crucial in order to avoid data leakage, *i*.*e*., the model is learnt over information that should be unavailable at prediction time. Indeed, data leakage is the source of a major reproducibility crisis in machine learning. This will be avoided by building training and validation sets which are weakly correlated with respect to the drug and disease feature vectors. The main performance metric will be the area under the curve (AUC), which estimates the diagnostic ability of a recommender system better than accuracy in imbalanced datasets.
 
 Medium-term outcomes to this package will significantly alleviate the economic burden of drug discovery pipelines, and will help find treatments in a more sustainable manner, especially for rare or tropical neglected diseases.
@@ -60,27 +64,27 @@
 python3 -m pip install stanscofi ## or use the conda command above
 python3 -m pip install notebook>=6.5.4 markupsafe==2.0.1 ## packages for Jupyter notebook
 conda deactivate
 conda activate stanscofi_env
 cd docs/ && jupyter notebook
 ```
 
-The complete list of dependencies for *stanscofi* can be found at [requirements.txt](https://raw.githubusercontent.com/RECeSS-EU-Project/stanscofi/master/recipes/pip/requirements.txt) (pip) or [meta.yaml](https://raw.githubusercontent.com/RECeSS-EU-Project/stanscofi/master/recipes/conda/meta.yaml) (conda).
+The complete list of dependencies for *stanscofi* can be found at [requirements.txt](https://raw.githubusercontent.com/RECeSS-EU-Project/stanscofi/master/pip/requirements.txt) (pip) or [meta.yaml](https://raw.githubusercontent.com/RECeSS-EU-Project/stanscofi/master/conda/meta.yaml) (conda).
 
 ## Licence
 
 This repository is under an [OSI-approved](https://opensource.org/licenses/) [MIT license](https://raw.githubusercontent.com/RECeSS-EU-Project/stanscofi/master/LICENSE). 
 
 ## Citation
 
 If you use **stanscofi** in academic research, please cite it as follows
 
 ```
-Clémence Réda. (2023). 
-stanscofi: a Python package for the development of collaborative filtering-based drug repurposing algorithms (v1.0.0). 
-Zenodo. https://doi.org/10.5281/zenodo.8020433
+Réda, Clémence. (2023). 
+STANdard for drug Screening by COllaborative FIltering (stanscofi). 
+Zenodo. https://doi.org/10.5281/zenodo.8038847
 ```
 
 ## Community guidelines with respect to contributions, issue reporting, and support
 
-[Pull requests](https://github.com/RECeSS-EU-Project/stanscofi/pulls) and [issue flagging](https://github.com/RECeSS-EU-Project/stanscofi/issues) are welcome, and can be made through the GitHub interface. Support can be provided by reaching out to recess-project-at-proton.me. However, please note that contributors and users must abide by the [Code of Conduct](https://github.com/RECeSS-EU-Project/stanscofi/blob/master/CODE%20OF%20CONDUCT.md).
+[Pull requests](https://github.com/RECeSS-EU-Project/stanscofi/pulls) and [issue flagging](https://github.com/RECeSS-EU-Project/stanscofi/issues) are welcome, and can be made through the GitHub interface. Support can be provided by reaching out to ``recess-project[at]proton.me``. However, please note that contributors and users must abide by the [Code of Conduct](https://github.com/RECeSS-EU-Project/stanscofi/blob/master/CODE%20OF%20CONDUCT.md).
```

### Comparing `stanscofi-1.0.1/setup.py` & `stanscofi-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 NAME = "stanscofi"
-VERSION = "1.0.1"
+VERSION = "1.0.3"
 
 setup(name=NAME,
     version=VERSION,
     author="Clémence Réda",
     author_email="recess-project@proton.me",
     url="https://github.com/RECeSS-EU-Project/stanscofi",
     license_files = ('LICENSE'),
@@ -27,12 +27,12 @@
         "numpy>=1.19.4",
         "scikit-learn>=0.24.0",
         "scipy>=1.5.4",
         "matplotlib>=3.3.2",
         "threadpoolctl>=3.1.0",
         "joblib>=1.0.1",
         "tqdm>=4.58.0",
-        "codecarbon>=2.2.3",
+        "codecarbon>=2.2.2",
         "seaborn>=0.11.0",
     ],
     entry_points={},
 )
```

### Comparing `stanscofi-1.0.1/src/stanscofi/datasets.py` & `stanscofi-1.0.3/src/stanscofi/datasets.py`

 * *Files identical despite different names*

### Comparing `stanscofi-1.0.1/src/stanscofi/preprocessing.py` & `stanscofi-1.0.3/src/stanscofi/preprocessing.py`

 * *Files identical despite different names*

### Comparing `stanscofi-1.0.1/src/stanscofi/training_testing.py` & `stanscofi-1.0.3/src/stanscofi/training_testing.py`

 * *Files identical despite different names*

### Comparing `stanscofi-1.0.1/src/stanscofi/utils.py` & `stanscofi-1.0.3/src/stanscofi/utils.py`

 * *Files identical despite different names*

### Comparing `stanscofi-1.0.1/src/stanscofi/validation.py` & `stanscofi-1.0.3/src/stanscofi/validation.py`

 * *Files identical despite different names*

### Comparing `stanscofi-1.0.1/src/stanscofi.egg-info/PKG-INFO` & `stanscofi-1.0.3/src/stanscofi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: stanscofi
-Version: 1.0.1
+Version: 1.0.3
 Summary: Package for STANdard drug Screening by COllaborative FIltering. Performs benchmarks against datasets and SotA algorithms, and implements training, validation and testing procedures.
 Home-page: https://github.com/RECeSS-EU-Project/stanscofi
 Author: Clémence Réda
 Author-email: recess-project@proton.me
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8.5
 Description-Content-Type: text/markdown
 
+![funding logo](https://raw.githubusercontent.com/RECeSS-EU-Project/RECeSS-EU-Project.github.io/main/assets/images/header%2BEU_rescale.jpg)
+
 # STANdard for drug Screening by COllaborative FIltering (stanscofi) Python Package
 
 This repository is a part of the EU-funded [RECeSS project](https://recess-eu-project.github.io) (#101102016), and hosts the code for the open-source Python package *stanscofi* for the development of collaborative filtering-based drug repurposing algorithms.
 
+[![Anaconda version](https://anaconda.org/recess/stanscofi/badges/version.svg)](https://anaconda.org/recess/stanscofi) [![PyPI version](https://badge.fury.io/py/stanscofi.svg)](https://badge.fury.io/py/stanscofi) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.8038847.svg)](https://doi.org/10.5281/zenodo.8038847)
+
 ## Statement of need
 
 As of 2022, current drug development pipelines last around 10 years, costing $2billion in average, while drug commercialization failure rates go up to 90%. These issues can be mitigated by drug repurposing, where chemical compounds are screened for new therapeutic indications in a systematic fashion. In prior works, this approach has been implemented through collaborative filtering. This semi-supervised learning framework leverages known drug-disease matchings in order to recommend new ones.
 
 The **stanscofi** package comprises method-agnostic training, validation, preprocessing and visualization procedures on several published drug repurposing datasets. The proper implementation of these steps is crucial in order to avoid data leakage, *i*.*e*., the model is learnt over information that should be unavailable at prediction time. Indeed, data leakage is the source of a major reproducibility crisis in machine learning. This will be avoided by building training and validation sets which are weakly correlated with respect to the drug and disease feature vectors. The main performance metric will be the area under the curve (AUC), which estimates the diagnostic ability of a recommender system better than accuracy in imbalanced datasets.
 
 Medium-term outcomes to this package will significantly alleviate the economic burden of drug discovery pipelines, and will help find treatments in a more sustainable manner, especially for rare or tropical neglected diseases.
@@ -74,27 +78,27 @@
 python3 -m pip install stanscofi ## or use the conda command above
 python3 -m pip install notebook>=6.5.4 markupsafe==2.0.1 ## packages for Jupyter notebook
 conda deactivate
 conda activate stanscofi_env
 cd docs/ && jupyter notebook
 ```
 
-The complete list of dependencies for *stanscofi* can be found at [requirements.txt](https://raw.githubusercontent.com/RECeSS-EU-Project/stanscofi/master/recipes/pip/requirements.txt) (pip) or [meta.yaml](https://raw.githubusercontent.com/RECeSS-EU-Project/stanscofi/master/recipes/conda/meta.yaml) (conda).
+The complete list of dependencies for *stanscofi* can be found at [requirements.txt](https://raw.githubusercontent.com/RECeSS-EU-Project/stanscofi/master/pip/requirements.txt) (pip) or [meta.yaml](https://raw.githubusercontent.com/RECeSS-EU-Project/stanscofi/master/conda/meta.yaml) (conda).
 
 ## Licence
 
 This repository is under an [OSI-approved](https://opensource.org/licenses/) [MIT license](https://raw.githubusercontent.com/RECeSS-EU-Project/stanscofi/master/LICENSE). 
 
 ## Citation
 
 If you use **stanscofi** in academic research, please cite it as follows
 
 ```
-Clémence Réda. (2023). 
-stanscofi: a Python package for the development of collaborative filtering-based drug repurposing algorithms (v1.0.0). 
-Zenodo. https://doi.org/10.5281/zenodo.8020433
+Réda, Clémence. (2023). 
+STANdard for drug Screening by COllaborative FIltering (stanscofi). 
+Zenodo. https://doi.org/10.5281/zenodo.8038847
 ```
 
 ## Community guidelines with respect to contributions, issue reporting, and support
 
-[Pull requests](https://github.com/RECeSS-EU-Project/stanscofi/pulls) and [issue flagging](https://github.com/RECeSS-EU-Project/stanscofi/issues) are welcome, and can be made through the GitHub interface. Support can be provided by reaching out to recess-project-at-proton.me. However, please note that contributors and users must abide by the [Code of Conduct](https://github.com/RECeSS-EU-Project/stanscofi/blob/master/CODE%20OF%20CONDUCT.md).
+[Pull requests](https://github.com/RECeSS-EU-Project/stanscofi/pulls) and [issue flagging](https://github.com/RECeSS-EU-Project/stanscofi/issues) are welcome, and can be made through the GitHub interface. Support can be provided by reaching out to ``recess-project[at]proton.me``. However, please note that contributors and users must abide by the [Code of Conduct](https://github.com/RECeSS-EU-Project/stanscofi/blob/master/CODE%20OF%20CONDUCT.md).
```

