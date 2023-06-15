# Comparing `tmp/torchquad-0.3.0.tar.gz` & `tmp/torchquad-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchquad-0.3.0.tar", last modified: Thu May  5 17:04:38 2022, max compression
+gzip compressed data, was "torchquad-0.4.0.tar", last modified: Thu Jun 15 08:26:48 2023, max compression
```

## Comparing `torchquad-0.3.0.tar` & `torchquad-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 17:04:38.372408 torchquad-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-05-05 17:04:17.000000 torchquad-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16650 2022-05-05 17:04:38.372408 torchquad-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13631 2022-05-05 17:04:17.000000 torchquad-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-05 17:04:38.372408 torchquad-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1332 2022-05-05 17:04:17.000000 torchquad-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 17:04:38.368407 torchquad-0.3.0/torchquad/
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-05-05 17:04:17.000000 torchquad-0.3.0/torchquad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 17:04:38.368407 torchquad-0.3.0/torchquad/integration/
--rw-r--r--   0 runner    (1001) docker     (121)     3602 2022-05-05 17:04:17.000000 torchquad-0.3.0/torchquad/integration/base_integrator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3695 2022-05-05 17:04:17.000000 torchquad-0.3.0/torchquad/integration/boole.py
--rw-r--r--   0 runner    (1001) docker     (121)     3719 2022-05-05 17:04:17.000000 torchquad-0.3.0/torchquad/integration/integration_grid.py
--rw-r--r--   0 runner    (1001) docker     (121)    11367 2022-05-05 17:04:17.000000 torchquad-0.3.0/torchquad/integration/monte_carlo.py
--rw-r--r--   0 runner    (1001) docker     (121)     9184 2022-05-05 17:04:17.000000 torchquad-0.3.0/torchquad/integration/newton_cotes.py
--rw-r--r--   0 runner    (1001) docker     (121)     6202 2022-05-05 17:04:17.000000 torchquad-0.3.0/torchquad/integration/rng.py
--rw-r--r--   0 runner    (1001) docker     (121)     3368 2022-05-05 17:04:17.000000 torchquad-0.3.0/torchquad/integration/simpson.py
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-05-05 17:04:17.000000 torchquad-0.3.0/torchquad/integration/trapezoid.py
--rw-r--r--   0 runner    (1001) docker     (121)     9177 2022-05-05 17:04:17.000000 torchquad-0.3.0/torchquad/integration/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    14940 2022-05-05 17:04:17.000000 torchquad-0.3.0/torchquad/integration/vegas.py
--rw-r--r--   0 runner    (1001) docker     (121)    11123 2022-05-05 17:04:17.000000 torchquad-0.3.0/torchquad/integration/vegas_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     6580 2022-05-05 17:04:17.000000 torchquad-0.3.0/torchquad/integration/vegas_stratification.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 17:04:38.372408 torchquad-0.3.0/torchquad/plots/
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-05-05 17:04:17.000000 torchquad-0.3.0/torchquad/plots/plot_convergence.py
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-05-05 17:04:17.000000 torchquad-0.3.0/torchquad/plots/plot_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 17:04:38.372408 torchquad-0.3.0/torchquad/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     1899 2022-05-05 17:04:17.000000 torchquad-0.3.0/torchquad/utils/deployment_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1021 2022-05-05 17:04:17.000000 torchquad-0.3.0/torchquad/utils/enable_cuda.py
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-05-05 17:04:17.000000 torchquad-0.3.0/torchquad/utils/set_log_level.py
--rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-05-05 17:04:17.000000 torchquad-0.3.0/torchquad/utils/set_precision.py
--rw-r--r--   0 runner    (1001) docker     (121)     1898 2022-05-05 17:04:17.000000 torchquad-0.3.0/torchquad/utils/set_up_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 17:04:38.368407 torchquad-0.3.0/torchquad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16650 2022-05-05 17:04:37.000000 torchquad-0.3.0/torchquad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      875 2022-05-05 17:04:38.000000 torchquad-0.3.0/torchquad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-05 17:04:37.000000 torchquad-0.3.0/torchquad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-05-05 17:04:37.000000 torchquad-0.3.0/torchquad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-05-05 17:04:37.000000 torchquad-0.3.0/torchquad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:26:48.693371 torchquad-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 08:26:23.000000 torchquad-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16478 2023-06-15 08:26:48.693371 torchquad-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13475 2023-06-15 08:26:23.000000 torchquad-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 08:26:48.693371 torchquad-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-15 08:26:24.000000 torchquad-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:26:48.689370 torchquad-0.4.0/torchquad/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:26:48.689370 torchquad-0.4.0/torchquad/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/integration/base_integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/integration/boole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/integration/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/integration/grid_integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/integration/integration_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/integration/monte_carlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/integration/newton_cotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/integration/rng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/integration/simpson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/integration/trapezoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/integration/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15087 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/integration/vegas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/integration/vegas_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/integration/vegas_stratification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:26:48.689370 torchquad-0.4.0/torchquad/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/plots/plot_convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/plots/plot_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:26:48.693371 torchquad-0.4.0/torchquad/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/utils/deployment_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/utils/enable_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/utils/set_log_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/utils/set_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-15 08:26:24.000000 torchquad-0.4.0/torchquad/utils/set_up_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:26:48.689370 torchquad-0.4.0/torchquad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16478 2023-06-15 08:26:48.000000 torchquad-0.4.0/torchquad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-15 08:26:48.000000 torchquad-0.4.0/torchquad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 08:26:48.000000 torchquad-0.4.0/torchquad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-15 08:26:48.000000 torchquad-0.4.0/torchquad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 08:26:48.000000 torchquad-0.4.0/torchquad.egg-info/top_level.txt
```

### Comparing `torchquad-0.3.0/LICENSE` & `torchquad-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchquad-0.3.0/PKG-INFO` & `torchquad-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: torchquad
-Version: 0.3.0
+Version: 0.4.0
 Summary: Package providing torch-based numerical integration methods.
 Home-page: https://github.com/esa/torchquad
 Author: ESA Advanced Concepts Team
 Author-email: pablo.gomez@esa.int
 License: UNKNOWN
 Project-URL: Source, https://github.com/esa/torchquad/
 Description: # torchquad
         <!--
         *** Based on https://github.com/othneildrew/Best-README-Template
         -->
         
-        ![Read the Docs (version)](https://img.shields.io/readthedocs/torchquad/main?style=flat-square) ![GitHub Workflow Status (branch)](https://img.shields.io/github/workflow/status/esa/torchquad/Running%20tests/main?style=flat-square) ![GitHub last commit](https://img.shields.io/github/last-commit/esa/torchquad?style=flat-square)
+        ![Read the Docs (version)](https://img.shields.io/readthedocs/torchquad/main?style=flat-square) [![Tests](https://github.com/esa/torchquad/actions/workflows/run_tests.yml/badge.svg)](https://github.com/esa/torchquad/actions/workflows/run_tests.yml) ![GitHub last commit](https://img.shields.io/github/last-commit/esa/torchquad?style=flat-square)
         ![GitHub](https://img.shields.io/github/license/esa/torchquad?style=flat-square) ![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/torchquad?style=flat-square) ![PyPI](https://img.shields.io/pypi/v/torchquad?style=flat-square) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/torchquad?style=flat-square)
         
         ![GitHub contributors](https://img.shields.io/github/contributors/esa/torchquad?style=flat-square)
         ![GitHub issues](https://img.shields.io/github/issues/esa/torchquad?style=flat-square) ![GitHub pull requests](https://img.shields.io/github/issues-pr/esa/torchquad?style=flat-square)
         ![Conda](https://img.shields.io/conda/dn/conda-forge/torchquad?style=flat-square) ![PyPI - Downloads](https://img.shields.io/pypi/dm/torchquad?style=flat-square)
         [![JOSS](https://joss.theoj.org/papers/d6f22f83f1a889ddf83b3c2e0cd0919c/status.svg)](https://joss.theoj.org/papers/d6f22f83f1a889ddf83b3c2e0cd0919c?style=flat-square)
         
@@ -28,16 +28,14 @@
           </a>
           <p align="center">
             High-performance numerical integration on the GPU with PyTorch, JAX and Tensorflow
             <br />
             <a href="https://torchquad.readthedocs.io"><strong>Explore the docs »</strong></a>
             <br />
             <br />
-            <a href="https://github.com/esa/torchquad/blob/master/notebooks/Torchquad%20-%20Example%20notebook.ipynb">View Example notebook</a>
-            ·
             <a href="https://github.com/esa/torchquad/issues">Report Bug</a>
             ·
             <a href="https://github.com/esa/torchquad/issues">Request Feature</a>
           </p>
         </p>
         
         
@@ -132,15 +130,15 @@
         
         Note that since PyTorch is not yet on *conda-forge* for Windows, we have explicitly included it here using `-c pytorch`.
         Note also that installing PyTorch with *pip* may **not** set it up with CUDA support. Therefore, we recommend to use *conda*.
         
         Here are installation instructions for other numerical backends:
            ```sh
            conda install "tensorflow>=2.6.0=cuda*" -c conda-forge
-           pip install "jax[cuda]>=0.2.22" --find-links https://storage.googleapis.com/jax-releases/jax_releases.html # linux only
+           pip install "jax[cuda]>=0.2.22" --find-links https://storage.googleapis.com/jax-releases/jax_cuda_releases.html # linux only
            conda install "numpy>=1.19.5" -c conda-forge
            ```
         
         More installation instructions for numerical backends can be found in
         [environment_all_backends.yml](/environment_all_backends.yml) and at the
         backend documentations, for example
         https://pytorch.org/get-started/locally/,
@@ -280,15 +278,15 @@
         <!-- CONTACT -->
         ## Contact
         
         Created by ESA's [Advanced Concepts Team](https://www.esa.int/gsp/ACT/index.html)
         
         - Pablo Gómez - `pablo.gomez at esa.int`
         - Gabriele Meoni - `gabriele.meoni at esa.int`
-        - Håvard Hem Toftevaag - `havard.hem.toftevaag at esa.int`
+        - Håvard Hem Toftevaag
         
         Project Link: [https://github.com/esa/torchquad](https://github.com/esa/torchquad)
         
         
         
         <!-- ACKNOWLEDGEMENTS
         This README was based on https://github.com/othneildrew/Best-README-Template
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: torchquad Version: 0.3.0 Summary: Package providing
+Metadata-Version: 2.1 Name: torchquad Version: 0.4.0 Summary: Package providing
 torch-based numerical integration methods. Home-page: https://github.com/esa/
 torchquad Author: ESA Advanced Concepts Team Author-email: pablo.gomez@esa.int
 License: UNKNOWN Project-URL: Source, https://github.com/esa/torchquad/
 Description: # torchquad  ![Read the Docs (version)](https://img.shields.io/
-readthedocs/torchquad/main?style=flat-square) ![GitHub Workflow Status
-(branch)](https://img.shields.io/github/workflow/status/esa/torchquad/
-Running%20tests/main?style=flat-square) ![GitHub last commit](https://
+readthedocs/torchquad/main?style=flat-square) [![Tests](https://github.com/esa/
+torchquad/actions/workflows/run_tests.yml/badge.svg)](https://github.com/esa/
+torchquad/actions/workflows/run_tests.yml) ![GitHub last commit](https://
 img.shields.io/github/last-commit/esa/torchquad?style=flat-square) ![GitHub]
 (https://img.shields.io/github/license/esa/torchquad?style=flat-square) ![Conda
 (channel only)](https://img.shields.io/conda/vn/conda-forge/
 torchquad?style=flat-square) ![PyPI](https://img.shields.io/pypi/v/
 torchquad?style=flat-square) ![PyPI - Python Version](https://img.shields.io/
 pypi/pyversions/torchquad?style=flat-square) ![GitHub contributors](https://
 img.shields.io/github/contributors/esa/torchquad?style=flat-square) ![GitHub
@@ -21,15 +21,15 @@
 d6f22f83f1a889ddf83b3c2e0cd0919c/status.svg)](https://joss.theoj.org/papers/
 d6f22f83f1a889ddf83b3c2e0cd0919c?style=flat-square)
                                     [Logo]
     High-performance numerical integration on the GPU with PyTorch, JAX and
                                   Tensorflow
                              Explore_the_docs_Â»
 
-            View_Example_notebook Â· Report_Bug Â· Request_Feature
+                         Report_Bug Â· Request_Feature
   Table of Contents
    1. About_The_Project
           o Built_With
    2. Goals
    3. Getting_Started
           o Prerequisites
           o Installation
@@ -90,16 +90,16 @@
 "cudatoolkit>=11.1" "pytorch>=1.9=*cuda*" -c conda-forge -c pytorch ``` Note
 that since PyTorch is not yet on *conda-forge* for Windows, we have explicitly
 included it here using `-c pytorch`. Note also that installing PyTorch with
 *pip* may **not** set it up with CUDA support. Therefore, we recommend to use
 *conda*. Here are installation instructions for other numerical backends: ```sh
 conda install "tensorflow>=2.6.0=cuda*" -c conda-forge pip install "jax
 [cuda]>=0.2.22" --find-links https://storage.googleapis.com/jax-releases/
-jax_releases.html # linux only conda install "numpy>=1.19.5" -c conda-forge ```
-More installation instructions for numerical backends can be found in
+jax_cuda_releases.html # linux only conda install "numpy>=1.19.5" -c conda-
+forge ``` More installation instructions for numerical backends can be found in
 [environment_all_backends.yml](/environment_all_backends.yml) and at the
 backend documentations, for example https://pytorch.org/get-started/locally/,
 https://github.com/google/jax/#installation and https://www.tensorflow.org/
 install/gpu, and often there are multiple ways to install them. ### Test After
 installing `torchquad` and PyTorch through `conda` or `pip`, users can test
 `torchquad`'s correct installation with: ```py import torchquad
 torchquad._deployment_test() ``` After cloning the repository, developers can
@@ -170,15 +170,15 @@
 A: This error indicates that PyTorch could not find a CUDA-compatible GPU.
 Either you have no compatible GPU or the necessary CUDA requirements are
 missing. Using `conda`, you can install them with `conda install cudatoolkit`.
 For more detailed installation instructions, please refer to the [PyTorch
 documentation](https://pytorch.org/get-started/locally/).  ## Contact Created
 by ESA's [Advanced Concepts Team](https://www.esa.int/gsp/ACT/index.html) -
 Pablo GÃ³mez - `pablo.gomez at esa.int` - Gabriele Meoni - `gabriele.meoni at
-esa.int` - HÃ¥vard Hem Toftevaag - `havard.hem.toftevaag at esa.int` Project
-Link: [https://github.com/esa/torchquad](https://github.com/esa/torchquad)
-Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: Science/
-Research Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier:
-License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
-Programming Language :: Python :: 3.8 Requires-Python: >=3.8, <4 Description-
-Content-Type: text/markdown
+esa.int` - HÃ¥vard Hem Toftevaag Project Link: [https://github.com/esa/
+torchquad](https://github.com/esa/torchquad)  Platform: UNKNOWN Classifier:
+Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research Classifier: Topic ::
+Scientific/Engineering :: Mathematics Classifier: License :: OSI Approved ::
+GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
+Python :: 3.8 Requires-Python: >=3.8, <4 Description-Content-Type: text/
+markdown
```

### Comparing `torchquad-0.3.0/README.md` & `torchquad-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # torchquad
 <!--
 *** Based on https://github.com/othneildrew/Best-README-Template
 -->
 
-![Read the Docs (version)](https://img.shields.io/readthedocs/torchquad/main?style=flat-square) ![GitHub Workflow Status (branch)](https://img.shields.io/github/workflow/status/esa/torchquad/Running%20tests/main?style=flat-square) ![GitHub last commit](https://img.shields.io/github/last-commit/esa/torchquad?style=flat-square)
+![Read the Docs (version)](https://img.shields.io/readthedocs/torchquad/main?style=flat-square) [![Tests](https://github.com/esa/torchquad/actions/workflows/run_tests.yml/badge.svg)](https://github.com/esa/torchquad/actions/workflows/run_tests.yml) ![GitHub last commit](https://img.shields.io/github/last-commit/esa/torchquad?style=flat-square)
 ![GitHub](https://img.shields.io/github/license/esa/torchquad?style=flat-square) ![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/torchquad?style=flat-square) ![PyPI](https://img.shields.io/pypi/v/torchquad?style=flat-square) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/torchquad?style=flat-square)
 
 ![GitHub contributors](https://img.shields.io/github/contributors/esa/torchquad?style=flat-square)
 ![GitHub issues](https://img.shields.io/github/issues/esa/torchquad?style=flat-square) ![GitHub pull requests](https://img.shields.io/github/issues-pr/esa/torchquad?style=flat-square)
 ![Conda](https://img.shields.io/conda/dn/conda-forge/torchquad?style=flat-square) ![PyPI - Downloads](https://img.shields.io/pypi/dm/torchquad?style=flat-square)
 [![JOSS](https://joss.theoj.org/papers/d6f22f83f1a889ddf83b3c2e0cd0919c/status.svg)](https://joss.theoj.org/papers/d6f22f83f1a889ddf83b3c2e0cd0919c?style=flat-square)
 
@@ -19,16 +19,14 @@
   </a>
   <p align="center">
     High-performance numerical integration on the GPU with PyTorch, JAX and Tensorflow
     <br />
     <a href="https://torchquad.readthedocs.io"><strong>Explore the docs »</strong></a>
     <br />
     <br />
-    <a href="https://github.com/esa/torchquad/blob/master/notebooks/Torchquad%20-%20Example%20notebook.ipynb">View Example notebook</a>
-    ·
     <a href="https://github.com/esa/torchquad/issues">Report Bug</a>
     ·
     <a href="https://github.com/esa/torchquad/issues">Request Feature</a>
   </p>
 </p>
 
 
@@ -123,15 +121,15 @@
 
 Note that since PyTorch is not yet on *conda-forge* for Windows, we have explicitly included it here using `-c pytorch`.
 Note also that installing PyTorch with *pip* may **not** set it up with CUDA support. Therefore, we recommend to use *conda*.
 
 Here are installation instructions for other numerical backends:
    ```sh
    conda install "tensorflow>=2.6.0=cuda*" -c conda-forge
-   pip install "jax[cuda]>=0.2.22" --find-links https://storage.googleapis.com/jax-releases/jax_releases.html # linux only
+   pip install "jax[cuda]>=0.2.22" --find-links https://storage.googleapis.com/jax-releases/jax_cuda_releases.html # linux only
    conda install "numpy>=1.19.5" -c conda-forge
    ```
 
 More installation instructions for numerical backends can be found in
 [environment_all_backends.yml](/environment_all_backends.yml) and at the
 backend documentations, for example
 https://pytorch.org/get-started/locally/,
@@ -271,15 +269,15 @@
 <!-- CONTACT -->
 ## Contact
 
 Created by ESA's [Advanced Concepts Team](https://www.esa.int/gsp/ACT/index.html)
 
 - Pablo Gómez - `pablo.gomez at esa.int`
 - Gabriele Meoni - `gabriele.meoni at esa.int`
-- Håvard Hem Toftevaag - `havard.hem.toftevaag at esa.int`
+- Håvard Hem Toftevaag
 
 Project Link: [https://github.com/esa/torchquad](https://github.com/esa/torchquad)
 
 
 
 <!-- ACKNOWLEDGEMENTS
 This README was based on https://github.com/othneildrew/Best-README-Template
```

#### html2text {}

```diff
@@ -1,31 +1,31 @@
 # torchquad  ![Read the Docs (version)](https://img.shields.io/readthedocs/
-torchquad/main?style=flat-square) ![GitHub Workflow Status (branch)](https://
-img.shields.io/github/workflow/status/esa/torchquad/Running%20tests/
-main?style=flat-square) ![GitHub last commit](https://img.shields.io/github/
-last-commit/esa/torchquad?style=flat-square) ![GitHub](https://img.shields.io/
-github/license/esa/torchquad?style=flat-square) ![Conda (channel only)](https:/
-/img.shields.io/conda/vn/conda-forge/torchquad?style=flat-square) ![PyPI]
-(https://img.shields.io/pypi/v/torchquad?style=flat-square) ![PyPI - Python
-Version](https://img.shields.io/pypi/pyversions/torchquad?style=flat-square) !
-[GitHub contributors](https://img.shields.io/github/contributors/esa/
+torchquad/main?style=flat-square) [![Tests](https://github.com/esa/torchquad/
+actions/workflows/run_tests.yml/badge.svg)](https://github.com/esa/torchquad/
+actions/workflows/run_tests.yml) ![GitHub last commit](https://img.shields.io/
+github/last-commit/esa/torchquad?style=flat-square) ![GitHub](https://
+img.shields.io/github/license/esa/torchquad?style=flat-square) ![Conda (channel
+only)](https://img.shields.io/conda/vn/conda-forge/torchquad?style=flat-square)
+![PyPI](https://img.shields.io/pypi/v/torchquad?style=flat-square) ![PyPI -
+Python Version](https://img.shields.io/pypi/pyversions/torchquad?style=flat-
+square) ![GitHub contributors](https://img.shields.io/github/contributors/esa/
 torchquad?style=flat-square) ![GitHub issues](https://img.shields.io/github/
 issues/esa/torchquad?style=flat-square) ![GitHub pull requests](https://
 img.shields.io/github/issues-pr/esa/torchquad?style=flat-square) ![Conda]
 (https://img.shields.io/conda/dn/conda-forge/torchquad?style=flat-square) !
 [PyPI - Downloads](https://img.shields.io/pypi/dm/torchquad?style=flat-square)
 [![JOSS](https://joss.theoj.org/papers/d6f22f83f1a889ddf83b3c2e0cd0919c/
 status.svg)](https://joss.theoj.org/papers/
 d6f22f83f1a889ddf83b3c2e0cd0919c?style=flat-square)
                                     [Logo]
     High-performance numerical integration on the GPU with PyTorch, JAX and
                                   Tensorflow
                              Explore_the_docs_Â»
 
-            View_Example_notebook Â· Report_Bug Â· Request_Feature
+                         Report_Bug Â· Request_Feature
   Table of Contents
    1. About_The_Project
           o Built_With
    2. Goals
    3. Getting_Started
           o Prerequisites
           o Installation
@@ -86,16 +86,16 @@
 "cudatoolkit>=11.1" "pytorch>=1.9=*cuda*" -c conda-forge -c pytorch ``` Note
 that since PyTorch is not yet on *conda-forge* for Windows, we have explicitly
 included it here using `-c pytorch`. Note also that installing PyTorch with
 *pip* may **not** set it up with CUDA support. Therefore, we recommend to use
 *conda*. Here are installation instructions for other numerical backends: ```sh
 conda install "tensorflow>=2.6.0=cuda*" -c conda-forge pip install "jax
 [cuda]>=0.2.22" --find-links https://storage.googleapis.com/jax-releases/
-jax_releases.html # linux only conda install "numpy>=1.19.5" -c conda-forge ```
-More installation instructions for numerical backends can be found in
+jax_cuda_releases.html # linux only conda install "numpy>=1.19.5" -c conda-
+forge ``` More installation instructions for numerical backends can be found in
 [environment_all_backends.yml](/environment_all_backends.yml) and at the
 backend documentations, for example https://pytorch.org/get-started/locally/,
 https://github.com/google/jax/#installation and https://www.tensorflow.org/
 install/gpu, and often there are multiple ways to install them. ### Test After
 installing `torchquad` and PyTorch through `conda` or `pip`, users can test
 `torchquad`'s correct installation with: ```py import torchquad
 torchquad._deployment_test() ``` After cloning the repository, developers can
@@ -166,9 +166,9 @@
 A: This error indicates that PyTorch could not find a CUDA-compatible GPU.
 Either you have no compatible GPU or the necessary CUDA requirements are
 missing. Using `conda`, you can install them with `conda install cudatoolkit`.
 For more detailed installation instructions, please refer to the [PyTorch
 documentation](https://pytorch.org/get-started/locally/).  ## Contact Created
 by ESA's [Advanced Concepts Team](https://www.esa.int/gsp/ACT/index.html) -
 Pablo GÃ³mez - `pablo.gomez at esa.int` - Gabriele Meoni - `gabriele.meoni at
-esa.int` - HÃ¥vard Hem Toftevaag - `havard.hem.toftevaag at esa.int` Project
-Link: [https://github.com/esa/torchquad](https://github.com/esa/torchquad)
+esa.int` - HÃ¥vard Hem Toftevaag Project Link: [https://github.com/esa/
+torchquad](https://github.com/esa/torchquad)
```

### Comparing `torchquad-0.3.0/setup.py` & `torchquad-0.4.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 """
 
 # Always prefer setuptools over distutils
 from setuptools import setup
 
 setup(
     name="torchquad",
-    version="0.3.0",
+    version="0.4.0",
     description="Package providing torch-based numerical integration methods.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/esa/torchquad",
     author="ESA Advanced Concepts Team",
     author_email="pablo.gomez@esa.int",
     install_requires=[
         "loguru>=0.5.3",
         "matplotlib>=3.3.3",
         "scipy>=1.6.0",
         "tqdm>=4.56.1",
-        "autoray>=0.2.5",
+        "autoray>=0.5.0",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Mathematics",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `torchquad-0.3.0/torchquad/__init__.py` & `torchquad-0.4.0/torchquad/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,33 +5,41 @@
 # hopefully changes with setup.py
 from .integration.integration_grid import IntegrationGrid
 from .integration.monte_carlo import MonteCarlo
 from .integration.trapezoid import Trapezoid
 from .integration.simpson import Simpson
 from .integration.boole import Boole
 from .integration.vegas import VEGAS
+from .integration.gaussian import GaussLegendre
+from .integration.gaussian import Gaussian
+from .integration.grid_integrator import GridIntegrator
+from .integration.base_integrator import BaseIntegrator
 
 from .integration.rng import RNG
 
 from .plots.plot_convergence import plot_convergence
 from .plots.plot_runtime import plot_runtime
 
 from .utils.set_log_level import set_log_level
 from .utils.enable_cuda import enable_cuda
 from .utils.set_precision import set_precision
 from .utils.set_up_backend import set_up_backend
 from .utils.deployment_test import _deployment_test
 
 __all__ = [
+    "GridIntegrator",
+    "BaseIntegrator",
     "IntegrationGrid",
     "MonteCarlo",
     "Trapezoid",
     "Simpson",
     "Boole",
     "VEGAS",
+    "GaussLegendre",
+    "Gaussian",
     "RNG",
     "plot_convergence",
     "plot_runtime",
     "enable_cuda",
     "set_precision",
     "set_log_level",
     "set_up_backend",
```

### Comparing `torchquad-0.3.0/torchquad/integration/base_integrator.py` & `torchquad-0.4.0/torchquad/integration/boole.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,98 +1,88 @@
-import warnings
 from autoray import numpy as anp
-from autoray import infer_backend
+import warnings
 from loguru import logger
 
-from .utils import _check_integration_domain
-
-
-class BaseIntegrator:
-    """The (abstract) integrator that all other integrators inherit from. Provides no explicit definitions for methods."""
+from .newton_cotes import NewtonCotes
 
-    # Function to evaluate
-    _fn = None
 
-    # Dimensionality of function to evaluate
-    _dim = None
+class Boole(NewtonCotes):
 
-    # Integration domain
-    _integration_domain = None
-
-    # Number of function evaluations
-    _nr_of_fevals = None
+    """Boole's rule. See https://en.wikipedia.org/wiki/Newton%E2%80%93Cotes_formulas#Closed_Newton%E2%80%93Cotes_formulas ."""
 
     def __init__(self):
-        self._nr_of_fevals = 0
-
-    def integrate(self):
-        raise (
-            NotImplementedError("This is an abstract base class. Should not be called.")
-        )
+        super().__init__()
 
-    def _eval(self, points):
-        """Call evaluate_integrand to evaluate self._fn function at the passed points and update self._nr_of_evals
+    def integrate(self, fn, dim, N=None, integration_domain=None, backend=None):
+        """Integrates the passed function on the passed domain using Boole's rule.
 
         Args:
-            points (backend tensor): Integration points
-        """
-        result, num_points = self.evaluate_integrand(self._fn, points)
-        self._nr_of_fevals += num_points
-        return result
-
-    @staticmethod
-    def evaluate_integrand(fn, points):
-        """Evaluate the integrand function at the passed points
-
-        Args:
-            fn (function): Integrand function
-            points (backend tensor): Integration points
+            fn (func): The function to integrate over.
+            dim (int): Dimensionality of the integration domain.
+            N (int, optional): Total number of sample points to use for the integration. N has to be such that N^(1/dim) - 1 % 4 == 0. Defaults to 5 points per dimension if None is given.
+            integration_domain (list or backend tensor, optional): Integration domain, e.g. [[-1,1],[0,1]]. Defaults to [-1,1]^dim. It can also determine the numerical backend.
+            backend (string, optional): Numerical backend. Defaults to integration_domain's backend if it is a tensor and otherwise to the backend from the latest call to set_up_backend or "torch" for backwards compatibility.
 
         Returns:
-            backend tensor: Integrand function output
-            int: Number of evaluated points
+            backend-specific number: Integral value
         """
-        num_points = points.shape[0]
-        result = fn(points)
-        if infer_backend(result) != infer_backend(points):
-            warnings.warn(
-                "The passed function's return value has a different numerical backend than the passed points. Will try to convert. Note that this may be slow as it results in memory transfers between CPU and GPU, if torchquad uses the GPU."
-            )
-            result = anp.array(result, like=points)
+        return super().integrate(fn, dim, N, integration_domain, backend)
 
-        num_results = result.shape[0]
-        if num_results != num_points:
-            raise ValueError(
-                f"The passed function was given {num_points} points but only returned {num_results} value(s)."
-                f"Please ensure that your function is vectorized, i.e. can be called with multiple evaluation points at once. It should return a tensor "
-                f"where first dimension matches length of passed elements. "
+    @staticmethod
+    def _apply_composite_rule(cur_dim_areas, dim, hs, domain):
+        """Apply composite Boole quadrature.
+        cur_dim_areas will contain the areas per dimension
+        """
+        # We collapse dimension by dimension
+        for cur_dim in range(dim):
+            cur_dim_areas = (
+                hs[cur_dim]
+                / 22.5
+                * (
+                    7 * cur_dim_areas[..., 0:-4][..., ::4]
+                    + 32 * cur_dim_areas[..., 1:-3][..., ::4]
+                    + 12 * cur_dim_areas[..., 2:-2][..., ::4]
+                    + 32 * cur_dim_areas[..., 3:-1][..., ::4]
+                    + 7 * cur_dim_areas[..., 4:][..., ::4]
+                )
             )
+            cur_dim_areas = anp.sum(cur_dim_areas, axis=len(cur_dim_areas.shape) - 1)
+        return cur_dim_areas
 
-        return result, num_points
+    @staticmethod
+    def _get_minimal_N(dim):
+        """Get the minimal number of points N for the integrator rule"""
+        return 5**dim
 
     @staticmethod
-    def _check_inputs(dim=None, N=None, integration_domain=None):
-        """Used to check input validity
+    def _adjust_N(dim, N):
+        """Adjusts the total number of points to a valid number, i.e. N satisfies N^(1/dim) - 1 % 4 == 0.
 
         Args:
-            dim (int, optional): Dimensionality of function to integrate. Defaults to None.
-            N (int, optional): Total number of integration points. Defaults to None.
-            integration_domain (list or backend tensor, optional): Integration domain, e.g. [[0,1],[1,2]]. Defaults to None.
+            dim (int): Dimensionality of the integration domain.
+            N (int): Total number of sample points to use for the integration.
 
-        Raises:
-            ValueError: if inputs are not compatible with each other.
+        Returns:
+            int: An N satisfying N^(1/dim) - 1 % 4 == 0.
         """
-        logger.debug("Checking inputs to Integrator.")
-        if dim is not None:
-            if dim < 1:
-                raise ValueError("Dimension needs to be 1 or larger.")
-
-        if N is not None:
-            if N < 1 or type(N) is not int:
-                raise ValueError("N has to be a positive integer.")
-
-        if integration_domain is not None:
-            dim_domain = _check_integration_domain(integration_domain)
-            if dim is not None and dim != dim_domain:
-                raise ValueError(
-                    "The dimension of the integration domain must match the passed function dimensionality dim."
-                )
+        n_per_dim = int(N ** (1.0 / dim) + 1e-8)
+        logger.debug(
+            "Checking if N per dim is >=5 and N = 1 + 4n, where n is a positive integer."
+        )
+
+        # Boole's rule requires N per dim >=5 and N = 1 + 4n,
+        # where n is a positive integer, for correctness.
+        if n_per_dim < 5:
+            warnings.warn(
+                "N per dimension cannot be lower than 5. "
+                "N per dim will now be changed to 5."
+            )
+            N = 5**dim
+        elif (n_per_dim - 1) % 4 != 0:
+            new_n_per_dim = n_per_dim - ((n_per_dim - 1) % 4)
+            warnings.warn(
+                "N per dimension must be N = 1 + 4n with n a positive integer due to necessary subdivisions. "
+                "N per dim will now be changed to the next lower N satisfying this, i.e. "
+                f"{n_per_dim} -> {new_n_per_dim}."
+            )
+            N = (new_n_per_dim) ** (dim)
+        return N
```

### Comparing `torchquad-0.3.0/torchquad/integration/boole.py` & `torchquad-0.4.0/torchquad/integration/simpson.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,88 +1,83 @@
 from autoray import numpy as anp
-import warnings
 from loguru import logger
+import warnings
 
 from .newton_cotes import NewtonCotes
 
 
-class Boole(NewtonCotes):
+class Simpson(NewtonCotes):
 
-    """Boole's rule. See https://en.wikipedia.org/wiki/Newton%E2%80%93Cotes_formulas#Closed_Newton%E2%80%93Cotes_formulas ."""
+    """Simpson's rule. See https://en.wikipedia.org/wiki/Newton%E2%80%93Cotes_formulas#Closed_Newton%E2%80%93Cotes_formulas ."""
 
     def __init__(self):
         super().__init__()
 
     def integrate(self, fn, dim, N=None, integration_domain=None, backend=None):
-        """Integrates the passed function on the passed domain using Boole's rule.
+        """Integrates the passed function on the passed domain using Simpson's rule.
 
         Args:
             fn (func): The function to integrate over.
             dim (int): Dimensionality of the integration domain.
-            N (int, optional): Total number of sample points to use for the integration. N has to be such that N^(1/dim) - 1 % 4 == 0. Defaults to 5 points per dimension if None is given.
-            integration_domain (list or backend tensor, optional): Integration domain, e.g. [[-1,1],[0,1]]. Defaults to [-1,1]^dim. It also determines the numerical backend if possible.
-            backend (string, optional): Numerical backend. This argument is ignored if the backend can be inferred from integration_domain. Defaults to the backend from the latest call to set_up_backend or "torch" for backwards compatibility.
+            N (int, optional): Total number of sample points to use for the integration. Should be odd. Defaults to 3 points per dimension if None is given.
+            integration_domain (list or backend tensor, optional): Integration domain, e.g. [[-1,1],[0,1]]. Defaults to [-1,1]^dim. It can also determine the numerical backend.
+            backend (string, optional): Numerical backend. Defaults to integration_domain's backend if it is a tensor and otherwise to the backend from the latest call to set_up_backend or "torch" for backwards compatibility.
 
         Returns:
             backend-specific number: Integral value
         """
         return super().integrate(fn, dim, N, integration_domain, backend)
 
     @staticmethod
-    def _apply_composite_rule(cur_dim_areas, dim, hs):
-        """Apply composite Boole quadrature.
+    def _apply_composite_rule(cur_dim_areas, dim, hs, domain):
+        """Apply composite Simpson quadrature.
         cur_dim_areas will contain the areas per dimension
         """
         # We collapse dimension by dimension
         for cur_dim in range(dim):
             cur_dim_areas = (
                 hs[cur_dim]
-                / 22.5
+                / 3.0
                 * (
-                    7 * cur_dim_areas[..., 0:-4][..., ::4]
-                    + 32 * cur_dim_areas[..., 1:-3][..., ::4]
-                    + 12 * cur_dim_areas[..., 2:-2][..., ::4]
-                    + 32 * cur_dim_areas[..., 3:-1][..., ::4]
-                    + 7 * cur_dim_areas[..., 4:][..., ::4]
+                    cur_dim_areas[..., 0:-2][..., ::2]
+                    + 4 * cur_dim_areas[..., 1:-1][..., ::2]
+                    + cur_dim_areas[..., 2:][..., ::2]
                 )
             )
-            cur_dim_areas = anp.sum(cur_dim_areas, axis=dim - cur_dim - 1)
+            cur_dim_areas = anp.sum(cur_dim_areas, axis=len(cur_dim_areas.shape) - 1)
         return cur_dim_areas
 
     @staticmethod
     def _get_minimal_N(dim):
         """Get the minimal number of points N for the integrator rule"""
-        return 5**dim
+        return 3**dim
 
     @staticmethod
     def _adjust_N(dim, N):
-        """Adjusts the total number of points to a valid number, i.e. N satisfies N^(1/dim) - 1 % 4 == 0.
+        """Adjusts the current N to an odd integer >=3, if N is not that already.
 
         Args:
             dim (int): Dimensionality of the integration domain.
             N (int): Total number of sample points to use for the integration.
 
         Returns:
-            int: An N satisfying N^(1/dim) - 1 % 4 == 0.
+            int: An odd N >3.
         """
         n_per_dim = int(N ** (1.0 / dim) + 1e-8)
-        logger.debug(
-            "Checking if N per dim is >=5 and N = 1 + 4n, where n is a positive integer."
-        )
-
-        # Boole's rule requires N per dim >=5 and N = 1 + 4n,
-        # where n is a positive integer, for correctness.
-        if n_per_dim < 5:
+        logger.debug("Checking if N per dim is >=3 and odd.")
+
+        # Simpson's rule requires odd N per dim >3 for correctness. There is a more
+        # complex rule that works for even N as well but it is not implemented here.
+        if n_per_dim < 3:
             warnings.warn(
-                "N per dimension cannot be lower than 5. "
-                "N per dim will now be changed to 5."
+                "N per dimension cannot be lower than 3. "
+                "N per dim will now be changed to 3."
             )
-            N = 5**dim
-        elif (n_per_dim - 1) % 4 != 0:
-            new_n_per_dim = n_per_dim - ((n_per_dim - 1) % 4)
+            N = 3**dim
+        elif n_per_dim % 2 != 1:
             warnings.warn(
-                "N per dimension must be N = 1 + 4n with n a positive integer due to necessary subdivisions. "
-                "N per dim will now be changed to the next lower N satisfying this, i.e. "
-                f"{n_per_dim} -> {new_n_per_dim}."
+                "N per dimension cannot be even due to necessary subdivisions. "
+                "N per dim will now be changed to the next lower integer, i.e. "
+                f"{n_per_dim} -> {n_per_dim - 1}."
             )
-            N = (new_n_per_dim) ** (dim)
+            N = (n_per_dim - 1) ** (dim)
         return N
```

### Comparing `torchquad-0.3.0/torchquad/integration/integration_grid.py` & `torchquad-0.4.0/torchquad/integration/integration_grid.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,64 @@
 from autoray import numpy as anp
-from autoray import infer_backend
+from autoray import infer_backend, astype, to_backend_dtype
 from time import perf_counter
 from loguru import logger
 
 from .utils import (
-    _linspace_with_grads,
     _check_integration_domain,
     _setup_integration_domain,
+    _linspace_with_grads,
 )
 
 
+def grid_func(integration_domain, N, requires_grad=False, backend=None):
+    a = integration_domain[0]
+    b = integration_domain[1]
+    return _linspace_with_grads(a, b, N, requires_grad=requires_grad)
+
+
 class IntegrationGrid:
     """This class is used to store the integration grid for methods like Trapezoid or Simpsons, which require a grid."""
 
     points = None  # integration points
     h = None  # mesh width
     _N = None  # number of mesh points
     _dim = None  # dimensionality of the grid
     _runtime = None  # runtime for the creation of the integration grid
 
-    def __init__(self, N, integration_domain):
+    def __init__(
+        self,
+        N,
+        integration_domain,
+        grid_func=grid_func,
+        disable_integration_domain_check=False,
+    ):
         """Creates an integration grid of N points in the passed domain. Dimension will be len(integration_domain)
 
         Args:
             N (int): Total desired number of points in the grid (will take next lower root depending on dim)
             integration_domain (list or backend tensor): Domain to choose points in, e.g. [[-1,1],[0,1]]. It also determines the numerical backend (if it is a list, the backend is "torch").
+            grid_func (function): function for generating a grid of points over which to integrate (arguments: integration_domain, N, requires_grad, backend)
+            disable_integration_domain_check (bool): Disbaling integration domain checks (default False)
         """
         start = perf_counter()
-        self._check_inputs(N, integration_domain)
-        if infer_backend(integration_domain) == "builtins":
+        self._check_inputs(N, integration_domain, disable_integration_domain_check)
+        backend = infer_backend(integration_domain)
+        if backend == "builtins":
+            backend = "torch"
             integration_domain = _setup_integration_domain(
-                len(integration_domain), integration_domain, backend="torch"
+                len(integration_domain), integration_domain, backend=backend
             )
+        else:
+            # Convert the grid domain to float64 if it was int32/64
+            # will cause problems otherwise as in issue #180
+            if "int" in str(integration_domain.dtype):
+                dtype = to_backend_dtype("float64", like=backend)
+                integration_domain = astype(integration_domain, dtype)
+
         self._dim = integration_domain.shape[0]
 
         # TODO Add that N can be different for each dimension
         # A rounding error occurs for certain numbers with certain powers,
         # e.g. (4**3)**(1/3) = 3.99999... Because int() floors the number,
         # i.e. int(3.99999...) -> 3, a little error term is useful
         self._N = int(N ** (1.0 / self._dim) + 1e-8)  # convert to points per dim
@@ -53,19 +76,19 @@
         else:
             requires_grad = False
 
         grid_1d = []
         # Determine for each dimension grid points and mesh width
         for dim in range(self._dim):
             grid_1d.append(
-                _linspace_with_grads(
-                    integration_domain[dim][0],
-                    integration_domain[dim][1],
+                grid_func(
+                    integration_domain[dim],
                     self._N,
                     requires_grad=requires_grad,
+                    backend=backend,
                 )
             )
         self.h = anp.stack(
             [grid_1d[dim][1] - grid_1d[dim][0] for dim in range(self._dim)],
             like=integration_domain,
         )
 
@@ -77,19 +100,22 @@
             [mg.ravel() for mg in points], axis=1, like=integration_domain
         )
 
         logger.info("Integration grid created.")
 
         self._runtime = perf_counter() - start
 
-    def _check_inputs(self, N, integration_domain):
+    def _check_inputs(self, N, integration_domain, disable_integration_domain_check):
         """Used to check input validity"""
 
         logger.debug("Checking inputs to IntegrationGrid.")
-        dim = _check_integration_domain(integration_domain)
+        if disable_integration_domain_check:
+            dim = len(integration_domain)
+        else:
+            dim = _check_integration_domain(integration_domain)
 
         if N < 2:
             raise ValueError("N has to be > 1.")
 
         if N ** (1.0 / dim) < 2:
             raise ValueError(
                 "Cannot create a ",
```

### Comparing `torchquad-0.3.0/torchquad/integration/monte_carlo.py` & `torchquad-0.4.0/torchquad/integration/monte_carlo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from autoray import numpy as anp
 from autoray import infer_backend
 from loguru import logger
 
 from .base_integrator import BaseIntegrator
-from .utils import _setup_integration_domain
+from .utils import _setup_integration_domain, expand_func_values_and_squeeze_integral
 from .rng import RNG
 
 
 class MonteCarlo(BaseIntegrator):
     """Monte Carlo integration"""
 
     def __init__(self):
@@ -23,20 +23,20 @@
         rng=None,
         backend=None,
     ):
         """Integrates the passed function on the passed domain using vanilla Monte Carlo Integration.
 
         Args:
             fn (func): The function to integrate over.
-            dim (int): Dimensionality of the function to integrate.
+            dim (int): Dimensionality of the function's domain over which to integrate.
             N (int, optional): Number of sample points to use for the integration. Defaults to 1000.
-            integration_domain (list or backend tensor, optional): Integration domain, e.g. [[-1,1],[0,1]]. Defaults to [-1,1]^dim. It also determines the numerical backend if possible.
+            integration_domain (list or backend tensor, optional): Integration domain, e.g. [[-1,1],[0,1]]. Defaults to [-1,1]^dim. It can also determine the numerical backend.
             seed (int, optional): Random number generation seed to the sampling point creation, only set if provided. Defaults to None.
             rng (RNG, optional): An initialised RNG; this can be used when compiling the function for Tensorflow
-            backend (string, optional): Numerical backend. This argument is ignored if the backend can be inferred from integration_domain. Defaults to the backend from the latest call to set_up_backend or "torch" for backwards compatibility.
+            backend (string, optional): Numerical backend. Defaults to integration_domain's backend if it is a tensor and otherwise to the backend from the latest call to set_up_backend or "torch" for backwards compatibility.
 
         Raises:
             ValueError: If len(integration_domain) != dim
 
         Returns:
             backend-specific number: Integral value
         """
@@ -49,14 +49,15 @@
         )
         integration_domain = _setup_integration_domain(dim, integration_domain, backend)
         sample_points = self.calculate_sample_points(N, integration_domain, seed, rng)
         logger.debug("Evaluating integrand")
         function_values, self._nr_of_fevals = self.evaluate_integrand(fn, sample_points)
         return self.calculate_result(function_values, integration_domain)
 
+    @expand_func_values_and_squeeze_integral
     def calculate_result(self, function_values, integration_domain):
         """Calculate an integral result from the function evaluations
 
         Args:
             function_values (backend tensor): Output of the integrand
             integration_domain (backend tensor): Integration domain
 
@@ -65,15 +66,15 @@
         """
         logger.debug("Computing integration domain volume")
         scales = integration_domain[:, 1] - integration_domain[:, 0]
         volume = anp.prod(scales)
 
         # Integral = V / N * sum(func values)
         N = function_values.shape[0]
-        integral = volume * anp.sum(function_values) / N
+        integral = volume * anp.sum(function_values, axis=0) / N
         # NumPy automatically casts to float64 when dividing by N
         if (
             infer_backend(integration_domain) == "numpy"
             and function_values.dtype != integral.dtype
         ):
             integral = integral.astype(function_values.dtype)
         logger.opt(lazy=True).info(
@@ -115,17 +116,17 @@
         Use this method only if the integrand cannot be compiled.
         The compilation happens when the function is executed the first time.
         With PyTorch, return values of different integrands passed to the compiled function must all have the same format, e.g. precision.
 
         Args:
             dim (int): Dimensionality of the integration domain.
             N (int, optional): Number of sample points to use for the integration. Defaults to 1000.
-            integration_domain (list or backend tensor, optional): Integration domain, e.g. [[-1,1],[0,1]]. Defaults to [-1,1]^dim. It also determines the numerical backend if possible.
+            integration_domain (list or backend tensor, optional): Integration domain, e.g. [[-1,1],[0,1]]. Defaults to [-1,1]^dim. It can also determine the numerical backend.
             seed (int, optional): Random number generation seed for the sequence of sampling point calculations, only set if provided. The returned integrate function calculates different points in each invocation with and without specified seed. Defaults to None.
-            backend (string, optional): Numerical backend. This argument is ignored if the backend can be inferred from integration_domain. Defaults to the backend from the latest call to set_up_backend or "torch" for backwards compatibility.
+            backend (string, optional): Numerical backend. Defaults to integration_domain's backend if it is a tensor and otherwise to the backend from the latest call to set_up_backend or "torch" for backwards compatibility.
 
         Returns:
             function(fn, integration_domain): JIT compiled integrate function where all parameters except the integrand and domain are fixed
         """
         self._check_inputs(dim=dim, N=N, integration_domain=integration_domain)
         integration_domain = _setup_integration_domain(dim, integration_domain, backend)
         backend = infer_backend(integration_domain)
```

### Comparing `torchquad-0.3.0/torchquad/integration/newton_cotes.py` & `torchquad-0.4.0/torchquad/integration/grid_integrator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,73 +1,118 @@
 from loguru import logger
-from autoray import infer_backend
+from autoray import numpy as anp, infer_backend
 
 from .base_integrator import BaseIntegrator
 from .integration_grid import IntegrationGrid
-from .utils import _setup_integration_domain
+from .utils import (
+    _linspace_with_grads,
+    expand_func_values_and_squeeze_integral,
+    _setup_integration_domain,
+)
 
 
-class NewtonCotes(BaseIntegrator):
-    """The abstract integrator that Composite Newton Cotes integrators inherit from"""
+class GridIntegrator(BaseIntegrator):
+    """The abstract integrator that grid-like integrators (Newton-Cotes and Gaussian) integrators inherit from"""
 
     def __init__(self):
         super().__init__()
 
+    @property
+    def _grid_func(self):
+        def f(integration_domain, N, requires_grad=False, backend=None):
+            a = integration_domain[0]
+            b = integration_domain[1]
+            return _linspace_with_grads(a, b, N, requires_grad=requires_grad)
+
+        return f
+
+    def _weights(self, N, dim, backend, requires_grad=False):
+        return None
+
     def integrate(self, fn, dim, N, integration_domain, backend):
         """Integrate the passed function on the passed domain using a Composite Newton Cotes rule.
         The argument meanings are explained in the sub-classes.
 
         Returns:
             float: integral value
         """
         # If N is None, use the minimal required number of points per dimension
         if N is None:
             N = self._get_minimal_N(dim)
 
         integration_domain = _setup_integration_domain(dim, integration_domain, backend)
+        backend = infer_backend(integration_domain)
         self._check_inputs(dim=dim, N=N, integration_domain=integration_domain)
 
         grid_points, hs, n_per_dim = self.calculate_grid(N, integration_domain)
 
         logger.debug("Evaluating integrand on the grid.")
-        function_values, num_points = self.evaluate_integrand(fn, grid_points)
+        function_values, num_points = self.evaluate_integrand(
+            fn, grid_points, weights=self._weights(n_per_dim, dim, backend)
+        )
         self._nr_of_fevals = num_points
 
-        return self.calculate_result(function_values, dim, n_per_dim, hs)
+        return self.calculate_result(
+            function_values, dim, n_per_dim, hs, integration_domain
+        )
 
-    def calculate_result(self, function_values, dim, n_per_dim, hs):
-        """Apply the Composite Newton Cotes rule to calculate a result from the evaluated integrand.
+    @expand_func_values_and_squeeze_integral
+    def calculate_result(self, function_values, dim, n_per_dim, hs, integration_domain):
+        """Apply the "composite rule" to calculate a result from the evaluated integrand.
 
         Args:
             function_values (backend tensor): Output of the integrand
             dim (int): Dimensionality
             n_per_dim (int): Number of grid slices per dimension
             hs (backend tensor): Distances between grid slices for each dimension
 
         Returns:
             backend tensor: Quadrature result
         """
-        # Reshape the output to be [N,N,...] points instead of [dim*N] points
-        function_values = function_values.reshape([n_per_dim] * dim)
-
+        # Reshape the output to be [integrand_dim,N,N,...] points instead of [integrand_dim,dim*N] points
+        integrand_shape = function_values.shape[1:]
+        dim_shape = [n_per_dim] * dim
+        new_shape = [*integrand_shape, *dim_shape]
+        # We need to use einsum instead of just reshape here because reshape does not move the axis - it only reshapes.
+        # So the first line generates a character string for einsum, followed by moving the first dimension i.e `dim*N`
+        # to the end.  Finally we reshape the resulting object so that instead of the last dimension being `dim*N`, it is
+        # `N,N,...` as desired.
+        einsum = "".join(
+            [chr(i + 65) for i in range(len(function_values.shape))]
+        )  # chr(i + 65) generates an alphabetical character
+        reshaped_function_values = anp.einsum(
+            f"{einsum}->{einsum[1:]}{einsum[0]}", function_values
+        )
+        reshaped_function_values = reshaped_function_values.reshape(new_shape)
+        assert new_shape == list(
+            reshaped_function_values.shape
+        ), f"reshaping produced shape {reshaped_function_values.shape}, expected shape was {new_shape}"
         logger.debug("Computing areas.")
 
-        result = self._apply_composite_rule(function_values, dim, hs)
+        result = self._apply_composite_rule(
+            reshaped_function_values, dim, hs, integration_domain
+        )
 
         logger.opt(lazy=True).info(
             "Computed integral: {result}", result=lambda: str(result)
         )
         return result
 
-    def calculate_grid(self, N, integration_domain):
+    def calculate_grid(
+        self,
+        N,
+        integration_domain,
+        disable_integration_domain_check=False,
+    ):
         """Calculate grid points, widths and N per dim
 
         Args:
             N (int): Number of points
             integration_domain (backend tensor): Integration domain
+            disable_integration_domain_check (bool): Disbaling integration domain checks (default False)
 
         Returns:
             backend tensor: Grid points
             backend tensor: Grid widths
             int: Number of grid slices per dimension
         """
         N = self._adjust_N(dim=integration_domain.shape[0], N=N)
@@ -78,31 +123,38 @@
             "Creating a grid for {name} to integrate a function with {N} points over {d}.",
             name=lambda: type(self).__name__,
             N=lambda: str(N),
             d=lambda: str(integration_domain),
         )
 
         # Create grid and assemble evaluation points
-        grid = IntegrationGrid(N, integration_domain)
+        grid = IntegrationGrid(
+            N, integration_domain, self._grid_func, disable_integration_domain_check
+        )
 
         return grid.points, grid.h, grid._N
 
+    @staticmethod
+    def _adjust_N(dim, N):
+        # Nothing to do by default
+        return N
+
     def get_jit_compiled_integrate(
         self, dim, N=None, integration_domain=None, backend=None
     ):
         """Create an integrate function where the performance-relevant steps except the integrand evaluation are JIT compiled.
         Use this method only if the integrand cannot be compiled.
         The compilation happens when the function is executed the first time.
         With PyTorch, return values of different integrands passed to the compiled function must all have the same format, e.g. precision.
 
         Args:
             dim (int): Dimensionality of the integration domain.
             N (int, optional): Total number of sample points to use for the integration. See the integrate method documentation for more details.
-            integration_domain (list or backend tensor, optional): Integration domain, e.g. [[-1,1],[0,1]]. Defaults to [-1,1]^dim. It also determines the numerical backend if possible.
-            backend (string, optional): Numerical backend. This argument is ignored if the backend can be inferred from integration_domain. Defaults to the backend from the latest call to set_up_backend or "torch" for backwards compatibility.
+            integration_domain (list or backend tensor, optional): Integration domain, e.g. [[-1,1],[0,1]]. Defaults to [-1,1]^dim. It can also determine the numerical backend.
+            backend (string, optional): Numerical backend. Defaults to integration_domain's backend if it is a tensor and otherwise to the backend from the latest call to set_up_backend or "torch" for backwards compatibility.
 
         Returns:
             function(fn, integration_domain): JIT compiled integrate function where all parameters except the integrand and domain are fixed
         """
         # If N is None, use the minimal required number of points per dimension
         if N is None:
             N = self._get_minimal_N(dim)
@@ -129,23 +181,31 @@
                 if not hasattr(self, "_jax_jit_calculate_grid"):
                     import jax
 
                     self._jax_jit_calculate_grid = jax.jit(
                         self.calculate_grid, static_argnames=["N"]
                     )
                     self._jax_jit_calculate_result = jax.jit(
-                        self.calculate_result, static_argnames=["dim", "n_per_dim"]
+                        self.calculate_result,
+                        static_argnums=(
+                            1,
+                            2,
+                        ),  # dim and n_per_dim
                     )
                 jit_calculate_grid = self._jax_jit_calculate_grid
                 jit_calculate_result = self._jax_jit_calculate_result
 
             def compiled_integrate(fn, integration_domain):
                 grid_points, hs, n_per_dim = jit_calculate_grid(N, integration_domain)
-                function_values, _ = self.evaluate_integrand(fn, grid_points)
-                return jit_calculate_result(function_values, dim, int(n_per_dim), hs)
+                function_values, _ = self.evaluate_integrand(
+                    fn, grid_points, weights=self._weights(n_per_dim, dim, backend)
+                )
+                return jit_calculate_result(
+                    function_values, dim, int(n_per_dim), hs, integration_domain
+                )
 
             return compiled_integrate
 
         elif backend == "torch":
             # Torch requires explicit tracing with example inputs.
             def do_compile(example_integrand):
                 import torch
@@ -159,43 +219,51 @@
                         grid_points,
                         hs,
                         torch.Tensor([n_per_dim]),
                     )  # n_per_dim is constant
 
                 dim = int(integration_domain.shape[0])
 
-                def step3(function_values, hs):
-                    return self.calculate_result(function_values, dim, n_per_dim, hs)
+                def step3(function_values, hs, integration_domain):
+                    return self.calculate_result(
+                        function_values, dim, n_per_dim, hs, integration_domain
+                    )
 
                 # Trace the first step
                 step1 = torch.jit.trace(step1, (integration_domain,))
 
                 # Get example input for the third step
                 grid_points, hs, n_per_dim = step1(integration_domain)
                 n_per_dim = int(n_per_dim)
                 function_values, _ = self.evaluate_integrand(
-                    example_integrand, grid_points
+                    example_integrand,
+                    grid_points,
+                    weights=self._weights(n_per_dim, dim, backend),
                 )
 
                 # Trace the third step
                 # Avoid the warnings about a .grad attribute access of a
                 # non-leaf Tensor
                 if hs.requires_grad:
                     hs = hs.detach()
                     hs.requires_grad = True
                 if function_values.requires_grad:
                     function_values = function_values.detach()
                     function_values.requires_grad = True
-                step3 = torch.jit.trace(step3, (function_values, hs))
+                step3 = torch.jit.trace(
+                    step3, (function_values, hs, integration_domain)
+                )
 
                 # Define a compiled integrate function
                 def compiled_integrate(fn, integration_domain):
                     grid_points, hs, _ = step1(integration_domain)
-                    function_values, _ = self.evaluate_integrand(fn, grid_points)
-                    result = step3(function_values, hs)
+                    function_values, _ = self.evaluate_integrand(
+                        fn, grid_points, weights=self._weights(n_per_dim, dim, backend)
+                    )
+                    result = step3(function_values, hs, integration_domain)
                     return result
 
                 return compiled_integrate
 
             # Do the compilation when the returned function is executed the
             # first time
             compiled_func = [None]
```

### Comparing `torchquad-0.3.0/torchquad/integration/rng.py` & `torchquad-0.4.0/torchquad/integration/rng.py`

 * *Files identical despite different names*

### Comparing `torchquad-0.3.0/torchquad/integration/trapezoid.py` & `torchquad-0.4.0/torchquad/integration/trapezoid.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,33 +12,28 @@
     def integrate(self, fn, dim, N=1000, integration_domain=None, backend=None):
         """Integrates the passed function on the passed domain using the trapezoid rule.
 
         Args:
             fn (func): The function to integrate over.
             dim (int): Dimensionality of the function to integrate.
             N (int, optional): Total number of sample points to use for the integration. Defaults to 1000.
-            integration_domain (list or backend tensor, optional): Integration domain, e.g. [[-1,1],[0,1]]. Defaults to [-1,1]^dim. It also determines the numerical backend if possible.
-            backend (string, optional): Numerical backend. This argument is ignored if the backend can be inferred from integration_domain. Defaults to the backend from the latest call to set_up_backend or "torch" for backwards compatibility.
+            integration_domain (list or backend tensor, optional): Integration domain, e.g. [[-1,1],[0,1]]. Defaults to [-1,1]^dim. It can also determine the numerical backend.
+            backend (string, optional): Numerical backend. Defaults to integration_domain's backend if it is a tensor and otherwise to the backend from the latest call to set_up_backend or "torch" for backwards compatibility.
 
         Returns:
             backend-specific number: Integral value
         """
         return super().integrate(fn, dim, N, integration_domain, backend)
 
     @staticmethod
-    def _apply_composite_rule(cur_dim_areas, dim, hs):
+    def _apply_composite_rule(cur_dim_areas, dim, hs, domain):
         """Apply composite Trapezoid quadrature.
 
         cur_dim_areas will contain the areas per dimension
         """
         # We collapse dimension by dimension
         for cur_dim in range(dim):
             cur_dim_areas = (
                 hs[cur_dim] / 2.0 * (cur_dim_areas[..., 0:-1] + cur_dim_areas[..., 1:])
             )
-            cur_dim_areas = anp.sum(cur_dim_areas, axis=dim - cur_dim - 1)
+            cur_dim_areas = anp.sum(cur_dim_areas, axis=len(cur_dim_areas.shape) - 1)
         return cur_dim_areas
-
-    @staticmethod
-    def _adjust_N(dim, N):
-        # Nothing to do for Trapezoid
-        return N
```

### Comparing `torchquad-0.3.0/torchquad/integration/utils.py` & `torchquad-0.4.0/torchquad/integration/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # A relative import currently does not work when executing the tests.
 sys.path.append(str(Path(__file__).absolute().parent.parent))
 
 from autoray import numpy as anp
 from autoray import infer_backend, register_function
 from functools import partial
 from loguru import logger
+import warnings
 
 # from ..utils.set_precision import _get_precision
 from utils.set_precision import _get_precision
 from utils.set_up_backend import _get_default_backend
 
 
 def _linspace_with_grads(start, stop, N, requires_grad):
@@ -99,27 +100,39 @@
         raise NotImplementedError(f"Unsupported numerical backend: {backend}")
 
 
 def _setup_integration_domain(dim, integration_domain, backend):
     """Sets up the integration domain if unspecified by the user.
     Args:
         dim (int): Dimensionality of the integration domain.
-        integration_domain (list or backend tensor, optional): Integration domain, e.g. [[-1,1],[0,1]]. Defaults to [-1,1]^dim. It also determines the numerical backend if possible.
-        backend (string or None): Numerical backend. This argument is ignored if the backend can be inferred from integration_domain. If set to None, use the backend from the latest call to set_up_backend or "torch" for backwards compatibility.
+        integration_domain (list or backend tensor or None): Integration domain, e.g. [[-1,1],[0,1]]. Defaults to [-1,1]^dim. It can also determine the numerical backend.
+        backend (string or None): Numerical backend. If set to None, use integration_domain's backend if it is a tensor and otherwise use the backend from the latest call to set_up_backend or "torch" for backwards compatibility.
     Returns:
         backend tensor: Integration domain.
     """
     logger.debug("Setting up integration domain.")
 
     # If no integration_domain is specified, create [-1,1]^d bounds
     if integration_domain is None:
         integration_domain = [[-1.0, 1.0]] * dim
 
+    # Give an explicitly set backend argument higher precedence than
+    # integration_domain's backend.
+    # If the backend argument is not None, the dtype of integration_domain is
+    # ignored unless its backend and the backend argument are the same.
+    domain_arg_backend = infer_backend(integration_domain)
+    convert_to_tensor = domain_arg_backend == "builtins"
+    if not convert_to_tensor and backend is not None and domain_arg_backend != backend:
+        logger.warning(
+            "integration_domain should be a list when the backend argument is set."
+        )
+        convert_to_tensor = True
+
     # Convert integration_domain to a tensor if needed
-    if infer_backend(integration_domain) == "builtins":
+    if convert_to_tensor:
         # Cast all integration domain values to Python3 float because
         # some numerical backends create a tensor based on the Python3 types
         integration_domain = [
             [float(b) for b in bounds] for bounds in integration_domain
         ]
         if backend is None:
             # Get a globally default backend
@@ -160,15 +173,15 @@
             if len(bounds) != 2:
                 raise ValueError(
                     bounds,
                     " in ",
                     integration_domain,
                     " does not specify a valid integration bound.",
                 )
-            if bounds[0] > bounds[1]:
+            if anp.any(bounds[0] > bounds[1]):
                 raise ValueError(
                     bounds,
                     " in ",
                     integration_domain,
                     " does not specify a valid integration bound.",
                 )
         return dim
@@ -202,7 +215,49 @@
 @partial(register_function, "torch", "repeat")
 def _torch_repeat(a, repeats, axis=None):
     import torch
 
     # torch.repeat_interleave corresponds to np.repeat and should not be
     # confused with torch.Tensor.repeat.
     return torch.repeat_interleave(a, repeats, dim=axis)
+
+
+@partial(register_function, "torch", "expand_dims")
+def _torch_expand_dims(a, axis):
+    """torch is missing `expand_dims` which appears to exist on all other libraries used.
+
+    Args:
+        a (torch.Tensor): Tensor to be expanded along axis
+        axis (int): the axis along which to expand the dimensions
+
+    Returns:
+        torch.Tensor: a Tensor with an extra dimension.
+    """
+    import torch
+
+    return torch.unsqueeze(a, axis)
+
+
+def expand_func_values_and_squeeze_integral(f):
+    """This decorator ensures that the trailing dimension of integrands is indeed the integrand dimension.
+    This is pertinent in the 1d case when the sampled values are often of shape `(N,)`.  Then, to maintain backward
+    consistency, we squeeze the result in the 1d case so it does not have any trailing dimensions.
+
+    Args:
+        f (Callable): the wrapped function
+    """
+
+    def wrap(*args, **kwargs):
+        # i.e we only have one dimension, or the second dimension (that of the integrand) is 1
+        is_1d = len(args[1].shape) == 1 or (
+            len(args[1].shape) == 2 and args[1].shape[1] == 1
+        )
+        if is_1d:
+            warnings.warn(
+                "DEPRECATION WARNING: In future versions of torchquad, an array-like object will be returned."
+            )
+            return anp.squeeze(
+                f(args[0], anp.expand_dims(args[1], axis=1), *args[2:], **kwargs)
+            )
+        return f(*args, **kwargs)
+
+    return wrap
```

### Comparing `torchquad-0.3.0/torchquad/integration/vegas.py` & `torchquad-0.4.0/torchquad/integration/vegas.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,28 +41,29 @@
         max_iterations=20,
         use_warmup=True,
         backend=None,
     ):
         """Integrates the passed function on the passed domain using VEGAS.
 
         If the integrand output is far away from zero, i.e. lies within [b, b+c] for a constant b with large absolute value and small constant c, VEGAS does not adapt well to the integrand. Shifting the integrand so that it is close to zero may improve the accuracy of the calculated integral in this case.
+        This method does not support multi-dimensional/vectorized integrands (i.e., integrating an integrand repeatedly over a grid of points).
 
         Args:
             fn (func): The function to integrate over.
-            dim (int): Dimensionality of the function to integrate.
+            dim (int): Dimensionality of the function's domain over which to integrate.
             N (int, optional): Approximate maximum number of function evaluations to use for the integration. This value can be exceeded if the vegas stratification distributes evaluations per hypercube very unevenly. Defaults to 10000.
             integration_domain (list, optional): Integration domain, e.g. [[-1,1],[0,1]]. Defaults to [-1,1]^dim.
             seed (int, optional): Random number generation seed for the sampling point creation; only set if provided. Defaults to None.
             rng (RNG, optional): An initialised RNG; this can be used as alternative to the seed argument and to avoid problems with integrand functions which reset PyTorch's RNG seed.
             use_grid_improve (bool, optional): If True, improve the vegas map after each iteration. Defaults to True.
             eps_rel (float, optional): Relative error to abort at. Defaults to 0.
             eps_abs (float, optional): Absolute error to abort at. Defaults to 0.
             max_iterations (int, optional): Maximum number of vegas iterations to perform. The number of performed iterations is usually lower than this value because the number of sample points per iteration increases every fifth iteration. Defaults to 20.
             use_warmup (bool, optional): If True, execute a warmup to initialize the vegas map. Defaults to True.
-            backend (string, optional): Numerical backend. This argument is ignored if the backend can be inferred from integration_domain. "jax" and "tensorflow" are unsupported. Defaults to the backend from the latest call to set_up_backend or "torch" for backwards compatibility.
+            backend (string, optional): Numerical backend. "jax" and "tensorflow" are unsupported. Defaults to integration_domain's backend if it is a tensor and otherwise to the backend from the latest call to set_up_backend or "torch" for backwards compatibility.
 
         Raises:
             ValueError: If the integration_domain or backend argument is invalid
 
         Returns:
             backend-specific float: Integral value
         """
```

### Comparing `torchquad-0.3.0/torchquad/integration/vegas_map.py` & `torchquad-0.4.0/torchquad/integration/vegas_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """
 
     def __init__(self, N_intervals, dim, backend, dtype, alpha=0.5) -> None:
         """Initializes VEGAS Enhanced's adaptive map
 
         Args:
             N_intervals (int): Number of intervals per dimension to split the domain in.
-            dim (int): Dimensionality of the integrand.
+            dim (int): Dimensionality of the integration domain.
             backend (string): Numerical backend
             dtype (backend dtype): dtype used for the calculations
             alpha (float, optional): Alpha from the paper, EQ 19. Defaults to 0.5.
         """
         self.dim = dim
         self.N_intervals = N_intervals  # # of subdivisions
         N_edges = self.N_intervals + 1  # # of subdivsion boundaries
```

### Comparing `torchquad-0.3.0/torchquad/integration/vegas_stratification.py` & `torchquad-0.4.0/torchquad/integration/vegas_stratification.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """
 
     def __init__(self, N_increment, dim, rng, backend, dtype, beta=0.75):
         """Initialize the VEGAS stratification.
 
         Args:
             N_increment (int): Number of evaluations per iteration.
-            dim (int): Dimensionality
+            dim (int): Dimensionality of the integration domain
             rng (RNG): Random number generator
             backend (string): Numerical backend
             dtype (backend dtype): dtype used for the calculations
             beta (float, optional): Beta parameter from VEGAS Enhanced. Defaults to 0.75.
         """
         self.rng = rng
         self.dim = dim
```

### Comparing `torchquad-0.3.0/torchquad/plots/plot_convergence.py` & `torchquad-0.4.0/torchquad/plots/plot_convergence.py`

 * *Files identical despite different names*

### Comparing `torchquad-0.3.0/torchquad/plots/plot_runtime.py` & `torchquad-0.4.0/torchquad/plots/plot_runtime.py`

 * *Files identical despite different names*

### Comparing `torchquad-0.3.0/torchquad/utils/deployment_test.py` & `torchquad-0.4.0/torchquad/utils/deployment_test.py`

 * *Files identical despite different names*

### Comparing `torchquad-0.3.0/torchquad/utils/enable_cuda.py` & `torchquad-0.4.0/torchquad/utils/enable_cuda.py`

 * *Files identical despite different names*

### Comparing `torchquad-0.3.0/torchquad/utils/set_log_level.py` & `torchquad-0.4.0/torchquad/utils/set_log_level.py`

 * *Files identical despite different names*

### Comparing `torchquad-0.3.0/torchquad/utils/set_precision.py` & `torchquad-0.4.0/torchquad/utils/set_precision.py`

 * *Files identical despite different names*

### Comparing `torchquad-0.3.0/torchquad/utils/set_up_backend.py` & `torchquad-0.4.0/torchquad/utils/set_up_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 from .set_precision import set_precision
 from .enable_cuda import enable_cuda
 
 
 def _get_default_backend():
     """Get the latest backend which was passed to set_up_backend.
-    If set_up_backend has never been executed, return "torch" for backwards compatibility"""
+    If set_up_backend has never been executed, return "torch" for backwards compatibility
+    """
     return os.environ.get("TORCHQUAD_DEFAULT_BACKEND", "torch")
 
 
 def set_up_backend(backend, data_type=None, torch_enable_cuda=True):
     """Configure a numerical backend for torchquad.
 
     With the torch backend, this function calls torchquad.enable_cuda unless torch_enable_cuda is False.
```

### Comparing `torchquad-0.3.0/torchquad.egg-info/PKG-INFO` & `torchquad-0.4.0/torchquad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: torchquad
-Version: 0.3.0
+Version: 0.4.0
 Summary: Package providing torch-based numerical integration methods.
 Home-page: https://github.com/esa/torchquad
 Author: ESA Advanced Concepts Team
 Author-email: pablo.gomez@esa.int
 License: UNKNOWN
 Project-URL: Source, https://github.com/esa/torchquad/
 Description: # torchquad
         <!--
         *** Based on https://github.com/othneildrew/Best-README-Template
         -->
         
-        ![Read the Docs (version)](https://img.shields.io/readthedocs/torchquad/main?style=flat-square) ![GitHub Workflow Status (branch)](https://img.shields.io/github/workflow/status/esa/torchquad/Running%20tests/main?style=flat-square) ![GitHub last commit](https://img.shields.io/github/last-commit/esa/torchquad?style=flat-square)
+        ![Read the Docs (version)](https://img.shields.io/readthedocs/torchquad/main?style=flat-square) [![Tests](https://github.com/esa/torchquad/actions/workflows/run_tests.yml/badge.svg)](https://github.com/esa/torchquad/actions/workflows/run_tests.yml) ![GitHub last commit](https://img.shields.io/github/last-commit/esa/torchquad?style=flat-square)
         ![GitHub](https://img.shields.io/github/license/esa/torchquad?style=flat-square) ![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/torchquad?style=flat-square) ![PyPI](https://img.shields.io/pypi/v/torchquad?style=flat-square) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/torchquad?style=flat-square)
         
         ![GitHub contributors](https://img.shields.io/github/contributors/esa/torchquad?style=flat-square)
         ![GitHub issues](https://img.shields.io/github/issues/esa/torchquad?style=flat-square) ![GitHub pull requests](https://img.shields.io/github/issues-pr/esa/torchquad?style=flat-square)
         ![Conda](https://img.shields.io/conda/dn/conda-forge/torchquad?style=flat-square) ![PyPI - Downloads](https://img.shields.io/pypi/dm/torchquad?style=flat-square)
         [![JOSS](https://joss.theoj.org/papers/d6f22f83f1a889ddf83b3c2e0cd0919c/status.svg)](https://joss.theoj.org/papers/d6f22f83f1a889ddf83b3c2e0cd0919c?style=flat-square)
         
@@ -28,16 +28,14 @@
           </a>
           <p align="center">
             High-performance numerical integration on the GPU with PyTorch, JAX and Tensorflow
             <br />
             <a href="https://torchquad.readthedocs.io"><strong>Explore the docs »</strong></a>
             <br />
             <br />
-            <a href="https://github.com/esa/torchquad/blob/master/notebooks/Torchquad%20-%20Example%20notebook.ipynb">View Example notebook</a>
-            ·
             <a href="https://github.com/esa/torchquad/issues">Report Bug</a>
             ·
             <a href="https://github.com/esa/torchquad/issues">Request Feature</a>
           </p>
         </p>
         
         
@@ -132,15 +130,15 @@
         
         Note that since PyTorch is not yet on *conda-forge* for Windows, we have explicitly included it here using `-c pytorch`.
         Note also that installing PyTorch with *pip* may **not** set it up with CUDA support. Therefore, we recommend to use *conda*.
         
         Here are installation instructions for other numerical backends:
            ```sh
            conda install "tensorflow>=2.6.0=cuda*" -c conda-forge
-           pip install "jax[cuda]>=0.2.22" --find-links https://storage.googleapis.com/jax-releases/jax_releases.html # linux only
+           pip install "jax[cuda]>=0.2.22" --find-links https://storage.googleapis.com/jax-releases/jax_cuda_releases.html # linux only
            conda install "numpy>=1.19.5" -c conda-forge
            ```
         
         More installation instructions for numerical backends can be found in
         [environment_all_backends.yml](/environment_all_backends.yml) and at the
         backend documentations, for example
         https://pytorch.org/get-started/locally/,
@@ -280,15 +278,15 @@
         <!-- CONTACT -->
         ## Contact
         
         Created by ESA's [Advanced Concepts Team](https://www.esa.int/gsp/ACT/index.html)
         
         - Pablo Gómez - `pablo.gomez at esa.int`
         - Gabriele Meoni - `gabriele.meoni at esa.int`
-        - Håvard Hem Toftevaag - `havard.hem.toftevaag at esa.int`
+        - Håvard Hem Toftevaag
         
         Project Link: [https://github.com/esa/torchquad](https://github.com/esa/torchquad)
         
         
         
         <!-- ACKNOWLEDGEMENTS
         This README was based on https://github.com/othneildrew/Best-README-Template
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: torchquad Version: 0.3.0 Summary: Package providing
+Metadata-Version: 2.1 Name: torchquad Version: 0.4.0 Summary: Package providing
 torch-based numerical integration methods. Home-page: https://github.com/esa/
 torchquad Author: ESA Advanced Concepts Team Author-email: pablo.gomez@esa.int
 License: UNKNOWN Project-URL: Source, https://github.com/esa/torchquad/
 Description: # torchquad  ![Read the Docs (version)](https://img.shields.io/
-readthedocs/torchquad/main?style=flat-square) ![GitHub Workflow Status
-(branch)](https://img.shields.io/github/workflow/status/esa/torchquad/
-Running%20tests/main?style=flat-square) ![GitHub last commit](https://
+readthedocs/torchquad/main?style=flat-square) [![Tests](https://github.com/esa/
+torchquad/actions/workflows/run_tests.yml/badge.svg)](https://github.com/esa/
+torchquad/actions/workflows/run_tests.yml) ![GitHub last commit](https://
 img.shields.io/github/last-commit/esa/torchquad?style=flat-square) ![GitHub]
 (https://img.shields.io/github/license/esa/torchquad?style=flat-square) ![Conda
 (channel only)](https://img.shields.io/conda/vn/conda-forge/
 torchquad?style=flat-square) ![PyPI](https://img.shields.io/pypi/v/
 torchquad?style=flat-square) ![PyPI - Python Version](https://img.shields.io/
 pypi/pyversions/torchquad?style=flat-square) ![GitHub contributors](https://
 img.shields.io/github/contributors/esa/torchquad?style=flat-square) ![GitHub
@@ -21,15 +21,15 @@
 d6f22f83f1a889ddf83b3c2e0cd0919c/status.svg)](https://joss.theoj.org/papers/
 d6f22f83f1a889ddf83b3c2e0cd0919c?style=flat-square)
                                     [Logo]
     High-performance numerical integration on the GPU with PyTorch, JAX and
                                   Tensorflow
                              Explore_the_docs_Â»
 
-            View_Example_notebook Â· Report_Bug Â· Request_Feature
+                         Report_Bug Â· Request_Feature
   Table of Contents
    1. About_The_Project
           o Built_With
    2. Goals
    3. Getting_Started
           o Prerequisites
           o Installation
@@ -90,16 +90,16 @@
 "cudatoolkit>=11.1" "pytorch>=1.9=*cuda*" -c conda-forge -c pytorch ``` Note
 that since PyTorch is not yet on *conda-forge* for Windows, we have explicitly
 included it here using `-c pytorch`. Note also that installing PyTorch with
 *pip* may **not** set it up with CUDA support. Therefore, we recommend to use
 *conda*. Here are installation instructions for other numerical backends: ```sh
 conda install "tensorflow>=2.6.0=cuda*" -c conda-forge pip install "jax
 [cuda]>=0.2.22" --find-links https://storage.googleapis.com/jax-releases/
-jax_releases.html # linux only conda install "numpy>=1.19.5" -c conda-forge ```
-More installation instructions for numerical backends can be found in
+jax_cuda_releases.html # linux only conda install "numpy>=1.19.5" -c conda-
+forge ``` More installation instructions for numerical backends can be found in
 [environment_all_backends.yml](/environment_all_backends.yml) and at the
 backend documentations, for example https://pytorch.org/get-started/locally/,
 https://github.com/google/jax/#installation and https://www.tensorflow.org/
 install/gpu, and often there are multiple ways to install them. ### Test After
 installing `torchquad` and PyTorch through `conda` or `pip`, users can test
 `torchquad`'s correct installation with: ```py import torchquad
 torchquad._deployment_test() ``` After cloning the repository, developers can
@@ -170,15 +170,15 @@
 A: This error indicates that PyTorch could not find a CUDA-compatible GPU.
 Either you have no compatible GPU or the necessary CUDA requirements are
 missing. Using `conda`, you can install them with `conda install cudatoolkit`.
 For more detailed installation instructions, please refer to the [PyTorch
 documentation](https://pytorch.org/get-started/locally/).  ## Contact Created
 by ESA's [Advanced Concepts Team](https://www.esa.int/gsp/ACT/index.html) -
 Pablo GÃ³mez - `pablo.gomez at esa.int` - Gabriele Meoni - `gabriele.meoni at
-esa.int` - HÃ¥vard Hem Toftevaag - `havard.hem.toftevaag at esa.int` Project
-Link: [https://github.com/esa/torchquad](https://github.com/esa/torchquad)
-Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: Science/
-Research Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier:
-License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
-Programming Language :: Python :: 3.8 Requires-Python: >=3.8, <4 Description-
-Content-Type: text/markdown
+esa.int` - HÃ¥vard Hem Toftevaag Project Link: [https://github.com/esa/
+torchquad](https://github.com/esa/torchquad)  Platform: UNKNOWN Classifier:
+Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research Classifier: Topic ::
+Scientific/Engineering :: Mathematics Classifier: License :: OSI Approved ::
+GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
+Python :: 3.8 Requires-Python: >=3.8, <4 Description-Content-Type: text/
+markdown
```

### Comparing `torchquad-0.3.0/torchquad.egg-info/SOURCES.txt` & `torchquad-0.4.0/torchquad.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 torchquad.egg-info/PKG-INFO
 torchquad.egg-info/SOURCES.txt
 torchquad.egg-info/dependency_links.txt
 torchquad.egg-info/requires.txt
 torchquad.egg-info/top_level.txt
 torchquad/integration/base_integrator.py
 torchquad/integration/boole.py
+torchquad/integration/gaussian.py
+torchquad/integration/grid_integrator.py
 torchquad/integration/integration_grid.py
 torchquad/integration/monte_carlo.py
 torchquad/integration/newton_cotes.py
 torchquad/integration/rng.py
 torchquad/integration/simpson.py
 torchquad/integration/trapezoid.py
 torchquad/integration/utils.py
```

