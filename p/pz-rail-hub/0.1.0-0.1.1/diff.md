# Comparing `tmp/pz-rail-hub-0.1.0.tar.gz` & `tmp/pz-rail-hub-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-hub-0.1.0.tar", last modified: Tue Jun 13 21:17:45 2023, max compression
+gzip compressed data, was "pz-rail-hub-0.1.1.tar", last modified: Thu Jun 15 01:43:28 2023, max compression
```

## Comparing `pz-rail-hub-0.1.0.tar` & `pz-rail-hub-0.1.1.tar`

### file list

```diff
@@ -1,92 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.065173 pz-rail-hub-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.053173 pz-rail-hub-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.057173 pz-rail-hub-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2043 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (122)      548 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1863 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1950 2023-06-13 21:17:45.065173 pz-rail-hub-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.057173 pz-rail-hub-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      655 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.053173 pz-rail-hub-0.1.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.057173 pz-rail-hub-0.1.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (122)      749 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/_static/css/notebooks.css
--rw-r--r--   0 runner    (1001) docker     (122)     6008 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/demos.rst
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/nbconvert-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      164 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.061173 pz-rail-hub-0.1.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/citing.rst
--rw-r--r--   0 runner    (1001) docker     (122)    12909 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/core-notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/creation-notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (122)      426 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/demos.rst
--rw-r--r--   0 runner    (1001) docker     (122)      769 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/estimation-notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/futureplans.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2150 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/immediateplans.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/index_body.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8876 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      455 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/other-notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10864 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.061173 pz-rail-hub-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.061173 pz-rail-hub-0.1.0/examples/core_examples/
--rw-r--r--   0 runner    (1001) docker     (122)    14973 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/core_examples/FileIO_DataStore.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     6372 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    10490 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/core_examples/Pipe_Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/core_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/core_examples/Run_Pipe.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/core_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (122)     8478 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/core_examples/hyperbolic_magnitude_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     5159 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/core_examples/iterator_test.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.061173 pz-rail-hub-0.1.0/examples/creation_examples/
--rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/creation_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/creation_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (122)    17822 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/creation_examples/degradation-demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    15718 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/creation_examples/dsps_sed_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    11808 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/creation_examples/example_GridSelection_for_HSC.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    14596 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/creation_examples/example_ObsConditions.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     9326 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    11982 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/creation_examples/photometric_realization_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    24628 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/creation_examples/posterior-demo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.061173 pz-rail-hub-0.1.0/examples/estimation_examples/
--rw-r--r--   0 runner    (1001) docker     (122)    19368 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/estimation_examples/NZDir.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    24800 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/estimation_examples/RAIL_estimation_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)      848 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/estimation_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    28480 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/estimation_examples/SimpleSOM_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)      459 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/estimation_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (122)     5238 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/estimation_examples/nzdir_as_pipeline.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    30673 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/estimation_examples/somocluSOM_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    37053 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/estimation_examples/somocluSOMcluster_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    20698 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/estimation_examples/test_sampled_summarizers.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.065173 pz-rail-hub-0.1.0/examples/evaluation_examples/
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/evaluation_examples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      340 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/evaluation_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/evaluation_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (122)    19239 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/evaluation_examples/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    19193 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/evaluation_examples/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.065173 pz-rail-hub-0.1.0/examples/goldenspike_examples/
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/goldenspike_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/goldenspike_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/goldenspike_examples/cleanup_pipeline.sh
--rw-r--r--   0 runner    (1001) docker     (122)    25570 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/goldenspike_examples/goldenspike.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     2964 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/render_nb.py
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 21:17:45.065173 pz-rail-hub-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.057173 pz-rail-hub-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.065173 pz-rail-hub-0.1.0/src/pz_rail_hub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1950 2023-06-13 21:17:44.000000 pz-rail-hub-0.1.0/src/pz_rail_hub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2548 2023-06-13 21:17:45.000000 pz-rail-hub-0.1.0/src/pz_rail_hub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 21:17:44.000000 pz-rail-hub-0.1.0/src/pz_rail_hub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-13 21:17:44.000000 pz-rail-hub-0.1.0/src/pz_rail_hub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-13 21:17:44.000000 pz-rail-hub-0.1.0/src/pz_rail_hub.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.057173 pz-rail-hub-0.1.0/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.065173 pz-rail-hub-0.1.0/src/rail/hub/
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/src/rail/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-13 21:17:44.000000 pz-rail-hub-0.1.0/src/rail/hub/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.065173 pz-rail-hub-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.991762 pz-rail-hub-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.983761 pz-rail-hub-0.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.983761 pz-rail-hub-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-15 01:43:28.991762 pz-rail-hub-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.983761 pz-rail-hub-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.979761 pz-rail-hub-0.1.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.983761 pz-rail-hub-0.1.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/_static/css/notebooks.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/demos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/nbconvert-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.983761 pz-rail-hub-0.1.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/source/citing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/source/futureplans.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/source/immediateplans.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10864 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/source/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.983761 pz-rail-hub-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.987761 pz-rail-hub-0.1.1/examples/core_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    14973 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/core_examples/FileIO_DataStore.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/core_examples/Pipe_Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/core_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/core_examples/Run_Pipe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/core_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/core_examples/hyperbolic_magnitude_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/core_examples/iterator_test.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.987761 pz-rail-hub-0.1.1/examples/creation_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/creation_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/creation_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/creation_examples/degradation-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15718 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/creation_examples/dsps_sed_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11808 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/creation_examples/example_GridSelection_for_HSC.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/creation_examples/example_ObsConditions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/creation_examples/photometric_realization_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    24628 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/creation_examples/posterior-demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.987761 pz-rail-hub-0.1.1/examples/estimation_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    19368 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/estimation_examples/NZDir.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    24800 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/estimation_examples/RAIL_estimation_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/estimation_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    28480 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/estimation_examples/SimpleSOM_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/estimation_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/estimation_examples/nzdir_as_pipeline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    30673 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/estimation_examples/somocluSOM_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    37053 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/estimation_examples/somocluSOMcluster_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20698 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/estimation_examples/test_sampled_summarizers.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.987761 pz-rail-hub-0.1.1/examples/evaluation_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/evaluation_examples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/evaluation_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/evaluation_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/evaluation_examples/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19193 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/evaluation_examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.991762 pz-rail-hub-0.1.1/examples/goldenspike_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/goldenspike_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/goldenspike_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/goldenspike_examples/cleanup_pipeline.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    25570 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/goldenspike_examples/goldenspike.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/rail_packages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 01:43:28.991762 pz-rail-hub-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.979761 pz-rail-hub-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.991762 pz-rail-hub-0.1.1/src/pz_rail_hub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-15 01:43:28.000000 pz-rail-hub-0.1.1/src/pz_rail_hub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-15 01:43:28.000000 pz-rail-hub-0.1.1/src/pz_rail_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 01:43:28.000000 pz-rail-hub-0.1.1/src/pz_rail_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 01:43:28.000000 pz-rail-hub-0.1.1/src/pz_rail_hub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-15 01:43:28.000000 pz-rail-hub-0.1.1/src/pz_rail_hub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 01:43:28.000000 pz-rail-hub-0.1.1/src/pz_rail_hub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.979761 pz-rail-hub-0.1.1/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.991762 pz-rail-hub-0.1.1/src/rail/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/src/rail/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-15 01:43:28.000000 pz-rail-hub-0.1.1/src/rail/hub/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/src/rail/hub/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/src/rail/hub/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/src/rail/hub/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.991762 pz-rail-hub-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/tests/test_scripts.py
```

### Comparing `pz-rail-hub-0.1.0/.gitignore` & `pz-rail-hub-0.1.1/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 *$py.class
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
-_version.py
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
 .eggs/
 lib/
@@ -23,14 +22,15 @@
 wheels/
 pip-wheel-metadata/
 share/python-wheels/
 *.egg-info/
 .installed.cfg
 *.egg
 MANIFEST
+_version.py
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
 
@@ -67,19 +67,15 @@
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
 docs/_build/
-docs/api.rst
-docs/api
-docs/index.rst
-docs/examples
-
+_readthedocs/
 
 # PyBuilder
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
 
@@ -129,7 +125,16 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+# vscode
+.vscode/
+
+# dask
+dask-worker-space/
+
+# tmp directory
+tmp/
```

### Comparing `pz-rail-hub-0.1.0/LICENSE` & `pz-rail-hub-0.1.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
+Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pz-rail-hub-0.1.0/docs/Makefile` & `pz-rail-hub-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/docs/_static/css/notebooks.css` & `pz-rail-hub-0.1.1/docs/_static/css/notebooks.css`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/docs/conf.py` & `pz-rail-hub-0.1.1/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import subprocess
 import sys
 sys.path.insert(0, os.path.abspath('..'))
 import rail
+from rail.core import RailEnv
 
 for rail_path in rail.__path__:
     sys.path.insert(0, rail_path)
 
 print(sys.path)
     
 
@@ -33,20 +34,29 @@
     'qp.factory',
     'qp.pdf_gen',
     'qp.metrics',
     'qp.metrics.pit',
     'qp.plotting',
     'qp.utils',
     'flexcode',
+    'flexcode.helpers',
     'flexzboost',
     'flexcode.regression_models',
     'flexcode.loss_functions',
     'flexcode.basis_functions',
     'fsps',
+    'dsps',
+    'dsps.cosmology',
+    'pzflow',
+    'pzflow.bijectors',
+    'sklearn',
+    'sklearn.cluster',
+    'sklearn.decomposition',
     'gal_pop_model_components',
+    'qp_flexzboost',
 ]
 for mod_name in MOCK_MODULES:
     sys.modules[mod_name] = MagicMock()
 
 sys.modules['flexcode'].regression_models.XGBoost = MagicMock
 sys.modules['flexcode'].loss_functions.cde_loss = MagicMock
 
@@ -173,17 +183,14 @@
 # -- Options for Autodoc--------------------------------------------------
 # Autodoc collects docstrings and builds API pages
 # from sphinxcontrib.apidoc import main as apidoc_main
 
 def run_apidoc(_):
     os.system('ln -s ../examples')
 
-    import rail
-    from rail.core import RailEnv
-    
     from sphinx.ext.apidoc import main as apidoc_main
     cur_dir = os.path.normpath(os.path.dirname(__file__))
     output_path = os.path.join(cur_dir, 'api')
 
     for full_path in rail.__path__:
         paramlist = ['--separate', '--implicit-namespaces', '--no-toc', '-M', '-o', output_path, '-f', full_path]
         print(f"running {paramlist}")
```

### Comparing `pz-rail-hub-0.1.0/docs/demos.rst` & `pz-rail-hub-0.1.1/docs/demos.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/docs/source/citing.rst` & `pz-rail-hub-0.1.1/docs/source/citing.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/docs/source/contributing.rst` & `pz-rail-hub-0.1.1/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/docs/source/futureplans.rst` & `pz-rail-hub-0.1.1/docs/source/futureplans.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/docs/source/immediateplans.rst` & `pz-rail-hub-0.1.1/docs/source/immediateplans.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/docs/source/index_body.rst` & `pz-rail-hub-0.1.1/docs/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -29,11 +29,14 @@
    source/immediateplans
    source/futureplans
    
 .. toctree::
    :maxdepth: 1
    :caption: Usage Demos
 
-   source/core-notebooks
-   source/creation-notebooks
-   source/estimation-notebooks
-   source/other-notebooks
+   demos
+
+.. toctree::
+   :maxdepth: 1
+   :caption: API
+
+   api
```

### Comparing `pz-rail-hub-0.1.0/docs/source/installation.rst` & `pz-rail-hub-0.1.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/docs/source/overview.rst` & `pz-rail-hub-0.1.1/docs/source/overview.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/core_examples/FileIO_DataStore.ipynb` & `pz-rail-hub-0.1.1/examples/core_examples/FileIO_DataStore.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb` & `pz-rail-hub-0.1.1/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/core_examples/Pipe_Example.ipynb` & `pz-rail-hub-0.1.1/examples/core_examples/Pipe_Example.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/core_examples/README.md` & `pz-rail-hub-0.1.1/examples/core_examples/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/core_examples/Run_Pipe.ipynb` & `pz-rail-hub-0.1.1/examples/core_examples/Run_Pipe.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/core_examples/hyperbolic_magnitude_test.ipynb` & `pz-rail-hub-0.1.1/examples/core_examples/hyperbolic_magnitude_test.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/core_examples/iterator_test.ipynb` & `pz-rail-hub-0.1.1/examples/core_examples/iterator_test.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/creation_examples/README.md` & `pz-rail-hub-0.1.1/examples/creation_examples/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/creation_examples/degradation-demo.ipynb` & `pz-rail-hub-0.1.1/examples/creation_examples/degradation-demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/creation_examples/dsps_sed_demo.ipynb` & `pz-rail-hub-0.1.1/examples/creation_examples/dsps_sed_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/creation_examples/example_GridSelection_for_HSC.ipynb` & `pz-rail-hub-0.1.1/examples/creation_examples/example_GridSelection_for_HSC.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/creation_examples/example_ObsConditions.ipynb` & `pz-rail-hub-0.1.1/examples/creation_examples/example_ObsConditions.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb` & `pz-rail-hub-0.1.1/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/creation_examples/photometric_realization_demo.ipynb` & `pz-rail-hub-0.1.1/examples/creation_examples/photometric_realization_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/creation_examples/posterior-demo.ipynb` & `pz-rail-hub-0.1.1/examples/creation_examples/posterior-demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/estimation_examples/NZDir.ipynb` & `pz-rail-hub-0.1.1/examples/estimation_examples/NZDir.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/estimation_examples/RAIL_estimation_demo.ipynb` & `pz-rail-hub-0.1.1/examples/estimation_examples/RAIL_estimation_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/estimation_examples/README.md` & `pz-rail-hub-0.1.1/examples/estimation_examples/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/estimation_examples/SimpleSOM_demo.ipynb` & `pz-rail-hub-0.1.1/examples/estimation_examples/SimpleSOM_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/estimation_examples/nzdir_as_pipeline.ipynb` & `pz-rail-hub-0.1.1/examples/estimation_examples/nzdir_as_pipeline.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/estimation_examples/somocluSOM_demo.ipynb` & `pz-rail-hub-0.1.1/examples/estimation_examples/somocluSOM_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/estimation_examples/somocluSOMcluster_demo.ipynb` & `pz-rail-hub-0.1.1/examples/estimation_examples/somocluSOMcluster_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/estimation_examples/test_sampled_summarizers.ipynb` & `pz-rail-hub-0.1.1/examples/estimation_examples/test_sampled_summarizers.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/evaluation_examples/demo.ipynb` & `pz-rail-hub-0.1.1/examples/evaluation_examples/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/evaluation_examples/utils.py` & `pz-rail-hub-0.1.1/examples/evaluation_examples/utils.py`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/goldenspike_examples/cleanup.sh` & `pz-rail-hub-0.1.1/examples/goldenspike_examples/cleanup.sh`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/examples/goldenspike_examples/goldenspike.ipynb` & `pz-rail-hub-0.1.1/examples/goldenspike_examples/goldenspike.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.0/src/pz_rail_hub.egg-info/SOURCES.txt` & `pz-rail-hub-0.1.1/src/pz_rail_hub.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+.copier-answers.yml
 .flake8
 .gitignore
+.pre-commit-config.yaml
 LICENSE
 README.md
 pyproject.toml
-render_nb.py
+rail_packages.yml
 requirements.txt
 setup.py
-.github/workflows/main.yml
-.github/workflows/pypi.yaml
+.github/pull_request_template.md
+.github/workflows/add-issue-to-project-tracker.yml
+.github/workflows/linting.yml
+.github/workflows/publish-to-pypi.yml
+.github/workflows/smoke-test.yml
+.github/workflows/testing-and-coverage.yml
 docs/Makefile
 docs/conf.py
 docs/demos.rst
+docs/index.rst
 docs/nbconvert-requirements.txt
 docs/requirements.txt
 docs/_static/css/notebooks.css
 docs/source/citing.rst
 docs/source/contributing.rst
-docs/source/core-notebooks.rst
-docs/source/creation-notebooks.rst
-docs/source/demos.rst
-docs/source/estimation-notebooks.rst
 docs/source/futureplans.rst
 docs/source/immediateplans.rst
-docs/source/index_body.rst
 docs/source/installation.rst
-docs/source/other-notebooks.rst
 docs/source/overview.rst
 examples/.gitignore
 examples/core_examples/FileIO_DataStore.ipynb
 examples/core_examples/FluxtoMag_and_Deredden_example.ipynb
 examples/core_examples/Pipe_Example.ipynb
 examples/core_examples/README.md
 examples/core_examples/Run_Pipe.ipynb
@@ -61,12 +62,17 @@
 examples/goldenspike_examples/README.md
 examples/goldenspike_examples/cleanup.sh
 examples/goldenspike_examples/cleanup_pipeline.sh
 examples/goldenspike_examples/goldenspike.ipynb
 src/pz_rail_hub.egg-info/PKG-INFO
 src/pz_rail_hub.egg-info/SOURCES.txt
 src/pz_rail_hub.egg-info/dependency_links.txt
+src/pz_rail_hub.egg-info/entry_points.txt
 src/pz_rail_hub.egg-info/requires.txt
 src/pz_rail_hub.egg-info/top_level.txt
 src/rail/hub/__init__.py
 src/rail/hub/_version.py
-tests/test_import.py
+src/rail/hub/commands.py
+src/rail/hub/options.py
+src/rail/hub/scripts.py
+tests/test_import.py
+tests/test_scripts.py
```

