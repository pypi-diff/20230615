# Comparing `tmp/gratin-0.1.8.tar.gz` & `tmp/gratin-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gratin-0.1.8.tar", last modified: Fri Jan 13 11:30:22 2023, max compression
+gzip compressed data, was "gratin-0.1.9.tar", last modified: Fri Jan 13 12:58:07 2023, max compression
```

## Comparing `gratin-0.1.8.tar` & `gratin-0.1.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 11:30:22.138080 gratin-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-01-13 11:30:09.000000 gratin-0.1.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 11:30:22.114080 gratin-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 11:30:22.122079 gratin-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-01-13 11:30:09.000000 gratin-0.1.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-01-13 11:30:09.000000 gratin-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-01-13 11:30:09.000000 gratin-0.1.8/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-01-13 11:30:09.000000 gratin-0.1.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-01-13 11:30:09.000000 gratin-0.1.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-13 11:30:09.000000 gratin-0.1.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-01-13 11:30:09.000000 gratin-0.1.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-01-13 11:30:09.000000 gratin-0.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-01-13 11:30:22.138080 gratin-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-01-13 11:30:09.000000 gratin-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 11:30:22.126080 gratin-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-01-13 11:30:09.000000 gratin-0.1.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 11:30:22.126080 gratin-0.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-13 11:30:09.000000 gratin-0.1.8/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-13 11:30:09.000000 gratin-0.1.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-13 11:30:09.000000 gratin-0.1.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-01-13 11:30:09.000000 gratin-0.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-13 11:30:09.000000 gratin-0.1.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-01-13 11:30:09.000000 gratin-0.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-13 11:30:09.000000 gratin-0.1.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-13 11:30:09.000000 gratin-0.1.8/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-01-13 11:30:09.000000 gratin-0.1.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-13 11:30:09.000000 gratin-0.1.8/docs/sbi.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 11:30:22.130080 gratin-0.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)   266489 2023-01-13 11:30:09.000000 gratin-0.1.8/examples/Check_MSD.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1045416 2023-01-13 11:30:09.000000 gratin-0.1.8/examples/Example Trajectories.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   295381 2023-01-13 11:30:09.000000 gratin-0.1.8/examples/MMD.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   589491 2023-01-13 11:30:09.000000 gratin-0.1.8/examples/Train.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-01-13 11:30:09.000000 gratin-0.1.8/examples/train_lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-01-13 11:30:09.000000 gratin-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-01-13 11:30:22.142080 gratin-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 11:30:22.118080 gratin-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 11:30:22.130080 gratin-0.1.8/src/gratin/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 11:30:22.134080 gratin-0.1.8/src/gratin/data/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/data/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/data/data_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)    10682 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/data/rep_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/data/skeleton_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 11:30:22.138080 gratin-0.1.8/src/gratin/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/layers/InvNet.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/layers/diverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/layers/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/layers/fBMGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/layers/features_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/layers/minimal_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/layers/mmd_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 11:30:22.138080 gratin-0.1.8/src/gratin/models/
--rw-r--r--   0 runner    (1001) docker     (123)    25998 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/models/BFlowDiffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    14322 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/models/BFlow_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/models/MMD_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/models/SelfSup.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 11:30:22.138080 gratin-0.1.8/src/gratin/models/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)    10025 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/models/__pycache__/BFlow.cpython-38.pyc.140382539799328
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/models/main_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/models/main_net_versatile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 11:30:22.138080 gratin-0.1.8/src/gratin/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/simulation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28921 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/simulation/diffusion_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/simulation/traj_tools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2366 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/simulation/utils_andi.py
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 11:30:22.138080 gratin-0.1.8/src/gratin/training/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/training/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/training/network_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-01-13 11:30:09.000000 gratin-0.1.8/src/gratin/training/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 11:30:22.134080 gratin-0.1.8/src/gratin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-01-13 11:30:22.000000 gratin-0.1.8/src/gratin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-01-13 11:30:22.000000 gratin-0.1.8/src/gratin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 11:30:22.000000 gratin-0.1.8/src/gratin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 11:30:21.000000 gratin-0.1.8/src/gratin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-01-13 11:30:22.000000 gratin-0.1.8/src/gratin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-13 11:30:22.000000 gratin-0.1.8/src/gratin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 11:30:22.138080 gratin-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-01-13 11:30:09.000000 gratin-0.1.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-01-13 11:30:09.000000 gratin-0.1.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:58:07.340008 gratin-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-01-13 12:57:55.000000 gratin-0.1.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:58:07.328008 gratin-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:58:07.332008 gratin-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-01-13 12:57:55.000000 gratin-0.1.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-01-13 12:57:55.000000 gratin-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-01-13 12:57:55.000000 gratin-0.1.9/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-01-13 12:57:55.000000 gratin-0.1.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-01-13 12:57:55.000000 gratin-0.1.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-13 12:57:55.000000 gratin-0.1.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-01-13 12:57:55.000000 gratin-0.1.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-01-13 12:57:55.000000 gratin-0.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-01-13 12:58:07.340008 gratin-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-01-13 12:57:55.000000 gratin-0.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:58:07.332008 gratin-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-01-13 12:57:55.000000 gratin-0.1.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:58:07.332008 gratin-0.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-13 12:57:55.000000 gratin-0.1.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-13 12:57:55.000000 gratin-0.1.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-13 12:57:55.000000 gratin-0.1.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-01-13 12:57:55.000000 gratin-0.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-13 12:57:55.000000 gratin-0.1.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-01-13 12:57:55.000000 gratin-0.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-13 12:57:55.000000 gratin-0.1.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-13 12:57:55.000000 gratin-0.1.9/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-01-13 12:57:55.000000 gratin-0.1.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-13 12:57:55.000000 gratin-0.1.9/docs/sbi.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:58:07.336008 gratin-0.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   266489 2023-01-13 12:57:55.000000 gratin-0.1.9/examples/Check_MSD.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1045416 2023-01-13 12:57:55.000000 gratin-0.1.9/examples/Example Trajectories.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   295381 2023-01-13 12:57:55.000000 gratin-0.1.9/examples/MMD.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   589491 2023-01-13 12:57:55.000000 gratin-0.1.9/examples/Train.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-01-13 12:57:55.000000 gratin-0.1.9/examples/train_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-01-13 12:57:55.000000 gratin-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-01-13 12:58:07.340008 gratin-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:58:07.332008 gratin-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:58:07.336008 gratin-0.1.9/src/gratin/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:58:07.336008 gratin-0.1.9/src/gratin/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/data/data_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10682 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/data/rep_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/data/skeleton_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:58:07.340008 gratin-0.1.9/src/gratin/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/layers/InvNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/layers/diverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/layers/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/layers/fBMGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/layers/features_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/layers/minimal_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/layers/mmd_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:58:07.340008 gratin-0.1.9/src/gratin/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    25998 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/models/BFlowDiffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14322 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/models/BFlow_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/models/MMD_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/models/SelfSup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:58:07.340008 gratin-0.1.9/src/gratin/models/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)    10025 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/models/__pycache__/BFlow.cpython-38.pyc.140382539799328
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/models/main_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/models/main_net_versatile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:58:07.340008 gratin-0.1.9/src/gratin/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/simulation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28921 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/simulation/diffusion_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/simulation/traj_tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2366 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/simulation/utils_andi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:58:07.340008 gratin-0.1.9/src/gratin/training/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/training/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/training/network_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-01-13 12:57:55.000000 gratin-0.1.9/src/gratin/training/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:58:07.336008 gratin-0.1.9/src/gratin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-01-13 12:58:07.000000 gratin-0.1.9/src/gratin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-01-13 12:58:07.000000 gratin-0.1.9/src/gratin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 12:58:07.000000 gratin-0.1.9/src/gratin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 12:58:06.000000 gratin-0.1.9/src/gratin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-01-13 12:58:07.000000 gratin-0.1.9/src/gratin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-13 12:58:07.000000 gratin-0.1.9/src/gratin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:58:07.340008 gratin-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-01-13 12:57:55.000000 gratin-0.1.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-01-13 12:57:55.000000 gratin-0.1.9/tox.ini
```

### Comparing `gratin-0.1.8/.coveragerc` & `gratin-0.1.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/.github/workflows/python-publish.yml` & `gratin-0.1.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/.gitignore` & `gratin-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/.gitlab-ci.yml` & `gratin-0.1.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/CONTRIBUTING.rst` & `gratin-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/LICENSE.txt` & `gratin-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/PKG-INFO` & `gratin-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gratin
-Version: 0.1.8
+Version: 0.1.9
 Summary: Random walk analysis tool using graph neural networks
 Home-page: https://github.com/hippover/gratin/
 Author: Hippolyte Verdier
 Author-email: hverdier@pasteur.fr
 License: mit
 Project-URL: Documentation, https://gratin.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `gratin-0.1.8/README.rst` & `gratin-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/docs/Makefile` & `gratin-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/docs/conf.py` & `gratin-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/docs/index.rst` & `gratin-0.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/examples/Check_MSD.ipynb` & `gratin-0.1.9/examples/Check_MSD.ipynb`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/examples/Example Trajectories.ipynb` & `gratin-0.1.9/examples/Example Trajectories.ipynb`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/examples/MMD.ipynb` & `gratin-0.1.9/examples/MMD.ipynb`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/examples/Train.ipynb` & `gratin-0.1.9/examples/Train.ipynb`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/examples/train_lightning.py` & `gratin-0.1.9/examples/train_lightning.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/setup.cfg` & `gratin-0.1.9/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gratin
-version = 0.1.8
+version = 0.1.9
 metadata_version = 2.3
 description = Random walk analysis tool using graph neural networks
 author = Hippolyte Verdier
 author_email = hverdier@pasteur.fr
 license = mit
 long_description = file: README.rst
 long_description_content_type = text/x-rst
@@ -26,16 +26,17 @@
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	setuptools==59.5.0
 	sphinx>=3.2.1
 	torch >= 1.12
 	torchmetrics >= 0.11
 	pytorch-lightning>=1.5.10
-	umap-learn[parametric_umap]>=0.5.2
-	tensorflow >= 2.6
+	umap-learn[parametric_umap]>=0.5.2;platform_system!='Darwin'
+	tensorflow >= 2.6;platform_system=='Linux'
+	tensorflow-macos;platform_system=='Darwin'
 	keras
 	tqdm
 	matplotlib
 	numpy
 	fbm
 	scipy
 	pandas
```

### Comparing `gratin-0.1.8/src/gratin/__init__.py` & `gratin-0.1.9/src/gratin/__init__.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/data/data.py` & `gratin-0.1.9/src/gratin/data/data.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/data/data_tools.py` & `gratin-0.1.9/src/gratin/data/data_tools.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/data/datamodule.py` & `gratin-0.1.9/src/gratin/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/data/dataset.py` & `gratin-0.1.9/src/gratin/data/dataset.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/data/rep_dataset.py` & `gratin-0.1.9/src/gratin/data/rep_dataset.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/data/skeleton_data.py` & `gratin-0.1.9/src/gratin/data/skeleton_data.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/layers/InvNet.py` & `gratin-0.1.9/src/gratin/layers/InvNet.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/layers/diverse.py` & `gratin-0.1.9/src/gratin/layers/diverse.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/layers/encoders.py` & `gratin-0.1.9/src/gratin/layers/encoders.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/layers/fBMGenerator.py` & `gratin-0.1.9/src/gratin/layers/fBMGenerator.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/layers/features_init.py` & `gratin-0.1.9/src/gratin/layers/features_init.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/layers/minimal_conv.py` & `gratin-0.1.9/src/gratin/layers/minimal_conv.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/layers/mmd_pytorch.py` & `gratin-0.1.9/src/gratin/layers/mmd_pytorch.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/models/BFlowDiffusion.py` & `gratin-0.1.9/src/gratin/models/BFlowDiffusion.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/models/BFlow_old.py` & `gratin-0.1.9/src/gratin/models/BFlow_old.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/models/MMD_net.py` & `gratin-0.1.9/src/gratin/models/MMD_net.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/models/SelfSup.py` & `gratin-0.1.9/src/gratin/models/SelfSup.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/models/__pycache__/BFlow.cpython-38.pyc.140382539799328` & `gratin-0.1.9/src/gratin/models/__pycache__/BFlow.cpython-38.pyc.140382539799328`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/models/main_net.py` & `gratin-0.1.9/src/gratin/models/main_net.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/models/main_net_versatile.py` & `gratin-0.1.9/src/gratin/models/main_net_versatile.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/models/utils.py` & `gratin-0.1.9/src/gratin/models/utils.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/simulation/diffusion_models.py` & `gratin-0.1.9/src/gratin/simulation/diffusion_models.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/simulation/traj_tools.py` & `gratin-0.1.9/src/gratin/simulation/traj_tools.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/simulation/utils_andi.py` & `gratin-0.1.9/src/gratin/simulation/utils_andi.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/standard.py` & `gratin-0.1.9/src/gratin/standard.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/training/callbacks.py` & `gratin-0.1.9/src/gratin/training/callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             pred = torch.cat(self.preds[param], dim=0).cpu()
 
             if param == "model":
                 # info = info
                 pred = torch.argmax(pred, dim=1)
                 n_models = len(pl_module.hparams["RW_types"])
                 CM = (
-                    confusion_matrix(pred, info, n_models, normalize="true")
+                    confusion_matrix(pred, info, task='multiclass',num_classes=n_models, normalize="true")
                     .detach()
                     .cpu()
                 )
 
                 fig = plt.figure()
                 ax = fig.add_subplot(111)
                 ax.imshow(CM, cmap="Blues", vmin=0.0, vmax=1.0)
```

### Comparing `gratin-0.1.8/src/gratin/training/network_tools.py` & `gratin-0.1.9/src/gratin/training/network_tools.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin/training/utils.py` & `gratin-0.1.9/src/gratin/training/utils.py`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/src/gratin.egg-info/PKG-INFO` & `gratin-0.1.9/src/gratin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gratin
-Version: 0.1.8
+Version: 0.1.9
 Summary: Random walk analysis tool using graph neural networks
 Home-page: https://github.com/hippover/gratin/
 Author: Hippolyte Verdier
 Author-email: hverdier@pasteur.fr
 License: mit
 Project-URL: Documentation, https://gratin.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `gratin-0.1.8/src/gratin.egg-info/SOURCES.txt` & `gratin-0.1.9/src/gratin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gratin-0.1.8/tox.ini` & `gratin-0.1.9/tox.ini`

 * *Files identical despite different names*

