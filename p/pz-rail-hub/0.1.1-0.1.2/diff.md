# Comparing `tmp/pz-rail-hub-0.1.1.tar.gz` & `tmp/pz-rail-hub-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-hub-0.1.1.tar", last modified: Thu Jun 15 01:43:28 2023, max compression
+gzip compressed data, was "pz-rail-hub-0.1.2.tar", last modified: Thu Jun 15 20:53:06 2023, max compression
```

## Comparing `pz-rail-hub-0.1.1.tar` & `pz-rail-hub-0.1.2.tar`

### file list

```diff
@@ -1,98 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.991762 pz-rail-hub-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.983761 pz-rail-hub-0.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.983761 pz-rail-hub-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-15 01:43:28.991762 pz-rail-hub-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.983761 pz-rail-hub-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.979761 pz-rail-hub-0.1.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.983761 pz-rail-hub-0.1.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/_static/css/notebooks.css
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/demos.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/nbconvert-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.983761 pz-rail-hub-0.1.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/source/citing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/source/futureplans.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/source/immediateplans.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10864 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/docs/source/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.983761 pz-rail-hub-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.987761 pz-rail-hub-0.1.1/examples/core_examples/
--rw-r--r--   0 runner    (1001) docker     (123)    14973 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/core_examples/FileIO_DataStore.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/core_examples/Pipe_Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/core_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/core_examples/Run_Pipe.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/core_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/core_examples/hyperbolic_magnitude_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/core_examples/iterator_test.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.987761 pz-rail-hub-0.1.1/examples/creation_examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/creation_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/creation_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/creation_examples/degradation-demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15718 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/creation_examples/dsps_sed_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11808 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/creation_examples/example_GridSelection_for_HSC.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/creation_examples/example_ObsConditions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/creation_examples/photometric_realization_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    24628 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/creation_examples/posterior-demo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.987761 pz-rail-hub-0.1.1/examples/estimation_examples/
--rw-r--r--   0 runner    (1001) docker     (123)    19368 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/estimation_examples/NZDir.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    24800 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/estimation_examples/RAIL_estimation_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/estimation_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    28480 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/estimation_examples/SimpleSOM_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/estimation_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/estimation_examples/nzdir_as_pipeline.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    30673 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/estimation_examples/somocluSOM_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    37053 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/estimation_examples/somocluSOMcluster_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20698 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/estimation_examples/test_sampled_summarizers.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.987761 pz-rail-hub-0.1.1/examples/evaluation_examples/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/evaluation_examples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/evaluation_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/evaluation_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/evaluation_examples/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19193 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/evaluation_examples/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.991762 pz-rail-hub-0.1.1/examples/goldenspike_examples/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/goldenspike_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/goldenspike_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/goldenspike_examples/cleanup_pipeline.sh
--rw-r--r--   0 runner    (1001) docker     (123)    25570 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/examples/goldenspike_examples/goldenspike.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/rail_packages.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 01:43:28.991762 pz-rail-hub-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.979761 pz-rail-hub-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.991762 pz-rail-hub-0.1.1/src/pz_rail_hub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-15 01:43:28.000000 pz-rail-hub-0.1.1/src/pz_rail_hub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-15 01:43:28.000000 pz-rail-hub-0.1.1/src/pz_rail_hub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 01:43:28.000000 pz-rail-hub-0.1.1/src/pz_rail_hub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 01:43:28.000000 pz-rail-hub-0.1.1/src/pz_rail_hub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-15 01:43:28.000000 pz-rail-hub-0.1.1/src/pz_rail_hub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 01:43:28.000000 pz-rail-hub-0.1.1/src/pz_rail_hub.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.979761 pz-rail-hub-0.1.1/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.991762 pz-rail-hub-0.1.1/src/rail/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/src/rail/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-15 01:43:28.000000 pz-rail-hub-0.1.1/src/rail/hub/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/src/rail/hub/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/src/rail/hub/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/src/rail/hub/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:43:28.991762 pz-rail-hub-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-15 01:43:16.000000 pz-rail-hub-0.1.1/tests/test_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:53:06.966290 pz-rail-hub-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:53:06.958290 pz-rail-hub-0.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:53:06.958290 pz-rail-hub-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/.github/workflows/build_documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-15 20:53:06.966290 pz-rail-hub-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/conda-reqs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:53:06.962290 pz-rail-hub-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:53:06.954290 pz-rail-hub-0.1.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:53:06.962290 pz-rail-hub-0.1.2/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/docs/_static/css/notebooks.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/docs/demos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/docs/nbconvert-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:53:06.962290 pz-rail-hub-0.1.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/docs/source/citing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/docs/source/futureplans.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/docs/source/immediateplans.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13710 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10864 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/docs/source/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:53:06.962290 pz-rail-hub-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:53:06.962290 pz-rail-hub-0.1.2/examples/core_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    14973 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/core_examples/FileIO_DataStore.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/core_examples/Pipe_Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/core_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/core_examples/Run_Pipe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/core_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/core_examples/hyperbolic_magnitude_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/core_examples/iterator_test.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:53:06.962290 pz-rail-hub-0.1.2/examples/creation_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/creation_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/creation_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/creation_examples/degradation-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15718 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/creation_examples/dsps_sed_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11808 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/creation_examples/example_GridSelection_for_HSC.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/creation_examples/example_ObsConditions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/creation_examples/photometric_realization_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    24628 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/creation_examples/posterior-demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:53:06.966290 pz-rail-hub-0.1.2/examples/estimation_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    19368 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/estimation_examples/NZDir.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    24800 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/estimation_examples/RAIL_estimation_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/estimation_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    28480 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/estimation_examples/SimpleSOM_demo.ipynb.fixme
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/estimation_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/estimation_examples/nzdir_as_pipeline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    30673 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/estimation_examples/somocluSOM_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    37053 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/estimation_examples/somocluSOMcluster_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20698 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/estimation_examples/test_sampled_summarizers.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:53:06.966290 pz-rail-hub-0.1.2/examples/evaluation_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/evaluation_examples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/evaluation_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/evaluation_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/evaluation_examples/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19193 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/evaluation_examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:53:06.966290 pz-rail-hub-0.1.2/examples/goldenspike_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/goldenspike_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/goldenspike_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/goldenspike_examples/cleanup_pipeline.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    25570 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/examples/goldenspike_examples/goldenspike.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/rail_packages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 20:53:06.966290 pz-rail-hub-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:53:06.954290 pz-rail-hub-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:53:06.966290 pz-rail-hub-0.1.2/src/pz_rail_hub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-15 20:53:06.000000 pz-rail-hub-0.1.2/src/pz_rail_hub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-15 20:53:06.000000 pz-rail-hub-0.1.2/src/pz_rail_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 20:53:06.000000 pz-rail-hub-0.1.2/src/pz_rail_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 20:53:06.000000 pz-rail-hub-0.1.2/src/pz_rail_hub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-15 20:53:06.000000 pz-rail-hub-0.1.2/src/pz_rail_hub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 20:53:06.000000 pz-rail-hub-0.1.2/src/pz_rail_hub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:53:06.954290 pz-rail-hub-0.1.2/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:53:06.966290 pz-rail-hub-0.1.2/src/rail/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/src/rail/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-15 20:53:06.000000 pz-rail-hub-0.1.2/src/rail/hub/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/src/rail/hub/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/src/rail/hub/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/src/rail/hub/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:53:06.966290 pz-rail-hub-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-15 20:52:54.000000 pz-rail-hub-0.1.2/tests/test_scripts.py
```

### Comparing `pz-rail-hub-0.1.1/.github/pull_request_template.md` & `pz-rail-hub-0.1.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/.github/workflows/linting.yml` & `pz-rail-hub-0.1.2/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/.github/workflows/publish-to-pypi.yml` & `pz-rail-hub-0.1.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/.github/workflows/smoke-test.yml` & `pz-rail-hub-0.1.2/.github/workflows/smoke-test.yml`

 * *Files 20% similar despite different names*

```diff
@@ -3,30 +3,25 @@
 
 name: Unit test smoke test
 
 on:
   schedule:
     - cron: 45 6 * * *
   workflow_dispatch:
-    inputs:
-      logLevel:
-        description: 'Log level'     
-        required: true
-        default: 'warning'
-      tags:
-        description: 'smoke tests' 
+    inputs: {}
 
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.8', '3.9', '3.10']
+        python-version: ['3.10']
+        notebook-dir: ['core', 'creation', 'estimation', 'evaluation', 'goldenspike']
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
@@ -39,10 +34,10 @@
         pip install .[dev]
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
     - name: Run unit tests with pytest
       run: |
         python -m pytest tests
     - name: Run notebooks
       run: |
-        rail render-nb examples/*_examples/*.ipynb
-
+        rail render-nb examples/${{ matrix.notebook-dir }}_examples/*.ipynb
+      continue-on-error: true
```

### Comparing `pz-rail-hub-0.1.1/.github/workflows/testing-and-coverage.yml` & `pz-rail-hub-0.1.2/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/.gitignore` & `pz-rail-hub-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/.pre-commit-config.yaml` & `pz-rail-hub-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/LICENSE` & `pz-rail-hub-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/PKG-INFO` & `pz-rail-hub-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-hub
-Version: 0.1.1
+Version: 0.1.2
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -27,15 +27,18 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
+Provides-Extra: algos
+Provides-Extra: nb
 Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE
 
 # pz-rail-hub
 
 [![Template](https://img.shields.io/badge/Template-LINCC%20Frameworks%20Python%20Project%20Template-brightgreen)](https://lincc-ppt.readthedocs.io/en/latest/)
 [![codecov](https://codecov.io/gh/LSSTDESC/pz-rail-hub/branch/main/graph/badge.svg)](https://codecov.io/gh/LSSTDESC/pz-rail-hub)
 [![PyPI](https://img.shields.io/pypi/v/hub?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/hub/)
```

### Comparing `pz-rail-hub-0.1.1/README.md` & `pz-rail-hub-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/docs/Makefile` & `pz-rail-hub-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/docs/_static/css/notebooks.css` & `pz-rail-hub-0.1.2/docs/_static/css/notebooks.css`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/docs/conf.py` & `pz-rail-hub-0.1.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
 
 
 # -- Options for Autodoc--------------------------------------------------
 # Autodoc collects docstrings and builds API pages
 # from sphinxcontrib.apidoc import main as apidoc_main
 
 def run_apidoc(_):
-    os.system('ln -s ../examples')
+    #os.system('ln -s ../examples')
 
     from sphinx.ext.apidoc import main as apidoc_main
     cur_dir = os.path.normpath(os.path.dirname(__file__))
     output_path = os.path.join(cur_dir, 'api')
 
     for full_path in rail.__path__:
         paramlist = ['--separate', '--implicit-namespaces', '--no-toc', '-M', '-o', output_path, '-f', full_path]
```

### Comparing `pz-rail-hub-0.1.1/docs/demos.rst` & `pz-rail-hub-0.1.2/docs/demos.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/docs/index.rst` & `pz-rail-hub-0.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/docs/source/citing.rst` & `pz-rail-hub-0.1.2/docs/source/citing.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/docs/source/contributing.rst` & `pz-rail-hub-0.1.2/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/docs/source/futureplans.rst` & `pz-rail-hub-0.1.2/docs/source/futureplans.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/docs/source/immediateplans.rst` & `pz-rail-hub-0.1.2/docs/source/immediateplans.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/docs/source/overview.rst` & `pz-rail-hub-0.1.2/docs/source/overview.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/core_examples/FileIO_DataStore.ipynb` & `pz-rail-hub-0.1.2/examples/core_examples/FileIO_DataStore.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb` & `pz-rail-hub-0.1.2/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/core_examples/Pipe_Example.ipynb` & `pz-rail-hub-0.1.2/examples/core_examples/Pipe_Example.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/core_examples/README.md` & `pz-rail-hub-0.1.2/examples/core_examples/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/core_examples/Run_Pipe.ipynb` & `pz-rail-hub-0.1.2/examples/core_examples/Run_Pipe.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/core_examples/hyperbolic_magnitude_test.ipynb` & `pz-rail-hub-0.1.2/examples/core_examples/hyperbolic_magnitude_test.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/core_examples/iterator_test.ipynb` & `pz-rail-hub-0.1.2/examples/core_examples/iterator_test.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/creation_examples/README.md` & `pz-rail-hub-0.1.2/examples/creation_examples/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/creation_examples/degradation-demo.ipynb` & `pz-rail-hub-0.1.2/examples/creation_examples/degradation-demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/creation_examples/dsps_sed_demo.ipynb` & `pz-rail-hub-0.1.2/examples/creation_examples/dsps_sed_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/creation_examples/example_GridSelection_for_HSC.ipynb` & `pz-rail-hub-0.1.2/examples/creation_examples/example_GridSelection_for_HSC.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/creation_examples/example_ObsConditions.ipynb` & `pz-rail-hub-0.1.2/examples/creation_examples/example_ObsConditions.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb` & `pz-rail-hub-0.1.2/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/creation_examples/photometric_realization_demo.ipynb` & `pz-rail-hub-0.1.2/examples/creation_examples/photometric_realization_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/creation_examples/posterior-demo.ipynb` & `pz-rail-hub-0.1.2/examples/creation_examples/posterior-demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/estimation_examples/NZDir.ipynb` & `pz-rail-hub-0.1.2/examples/estimation_examples/NZDir.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/estimation_examples/RAIL_estimation_demo.ipynb` & `pz-rail-hub-0.1.2/examples/estimation_examples/RAIL_estimation_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/estimation_examples/README.md` & `pz-rail-hub-0.1.2/examples/estimation_examples/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/estimation_examples/SimpleSOM_demo.ipynb` & `pz-rail-hub-0.1.2/examples/estimation_examples/SimpleSOM_demo.ipynb.fixme`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/estimation_examples/nzdir_as_pipeline.ipynb` & `pz-rail-hub-0.1.2/examples/estimation_examples/nzdir_as_pipeline.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/estimation_examples/somocluSOM_demo.ipynb` & `pz-rail-hub-0.1.2/examples/estimation_examples/somocluSOM_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/estimation_examples/somocluSOMcluster_demo.ipynb` & `pz-rail-hub-0.1.2/examples/estimation_examples/somocluSOMcluster_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/estimation_examples/test_sampled_summarizers.ipynb` & `pz-rail-hub-0.1.2/examples/estimation_examples/test_sampled_summarizers.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/evaluation_examples/demo.ipynb` & `pz-rail-hub-0.1.2/examples/evaluation_examples/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/evaluation_examples/utils.py` & `pz-rail-hub-0.1.2/examples/evaluation_examples/utils.py`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/goldenspike_examples/cleanup.sh` & `pz-rail-hub-0.1.2/examples/goldenspike_examples/cleanup.sh`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/examples/goldenspike_examples/goldenspike.ipynb` & `pz-rail-hub-0.1.2/examples/goldenspike_examples/goldenspike.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/pyproject.toml` & `pz-rail-hub-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -19,25 +19,42 @@
     "pz-rail-base",
     "click",
     "pyaml",
 ]
 
 # On a mac, install optional dependencies with `pip install '.[dev]'` (include the single quotes)
 [project.optional-dependencies]
+algos = [
+    "pz-rail-pipelines[full]",
+]
+
+nb = [
+    "pz-rail-pipelines[full]",
+    "jupyter",
+    "seaborn",
+]
+
 dev = [
     "pz-rail-pipelines[full]",
     "jupyter",
     "seaborn",
     "coverage",
     "pytest",
     "pytest-cov", # Used to report total code coverage
     "pre-commit", # Used to run checks before finalizing a git commit
     "pylint", # Used for static linting of files
 ]
 
+docs = [
+    "nbsphinx",
+    "sphinx==6.1.3", # Used to automatically generate documentation
+    "sphinx_rtd_theme==1.2.0", # Used to render documentation
+    "sphinx-autoapi==2.0.1", # Used to automatically generate api documentation    
+]
+
 [project.scripts]
 rail = "rail.hub.commands:cli"
 
 [build-system]
 requires = [
     "setuptools>=62", # Used to build and package the Python project
     "setuptools_scm>=6.2", # Gets release version from git. Makes it available programmatically
```

### Comparing `pz-rail-hub-0.1.1/src/pz_rail_hub.egg-info/PKG-INFO` & `pz-rail-hub-0.1.2/src/pz_rail_hub.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-hub
-Version: 0.1.1
+Version: 0.1.2
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -27,15 +27,18 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
+Provides-Extra: algos
+Provides-Extra: nb
 Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE
 
 # pz-rail-hub
 
 [![Template](https://img.shields.io/badge/Template-LINCC%20Frameworks%20Python%20Project%20Template-brightgreen)](https://lincc-ppt.readthedocs.io/en/latest/)
 [![codecov](https://codecov.io/gh/LSSTDESC/pz-rail-hub/branch/main/graph/badge.svg)](https://codecov.io/gh/LSSTDESC/pz-rail-hub)
 [![PyPI](https://img.shields.io/pypi/v/hub?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/hub/)
```

### Comparing `pz-rail-hub-0.1.1/src/pz_rail_hub.egg-info/SOURCES.txt` & `pz-rail-hub-0.1.2/src/pz_rail_hub.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 .copier-answers.yml
 .flake8
 .gitignore
 .pre-commit-config.yaml
+.readthedocs.yaml
 LICENSE
 README.md
+conda-reqs.txt
+environment.yml
 pyproject.toml
 rail_packages.yml
 requirements.txt
 setup.py
 .github/pull_request_template.md
 .github/workflows/add-issue-to-project-tracker.yml
+.github/workflows/build_documentation.yml
 .github/workflows/linting.yml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/smoke-test.yml
 .github/workflows/testing-and-coverage.yml
 docs/Makefile
 docs/conf.py
 docs/demos.rst
@@ -44,15 +48,15 @@
 examples/creation_examples/example_ObsConditions.ipynb
 examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb
 examples/creation_examples/photometric_realization_demo.ipynb
 examples/creation_examples/posterior-demo.ipynb
 examples/estimation_examples/NZDir.ipynb
 examples/estimation_examples/RAIL_estimation_demo.ipynb
 examples/estimation_examples/README.md
-examples/estimation_examples/SimpleSOM_demo.ipynb
+examples/estimation_examples/SimpleSOM_demo.ipynb.fixme
 examples/estimation_examples/cleanup.sh
 examples/estimation_examples/nzdir_as_pipeline.ipynb
 examples/estimation_examples/somocluSOM_demo.ipynb
 examples/estimation_examples/somocluSOMcluster_demo.ipynb
 examples/estimation_examples/test_sampled_summarizers.ipynb
 examples/evaluation_examples/.gitignore
 examples/evaluation_examples/README.md
```

### Comparing `pz-rail-hub-0.1.1/src/rail/hub/commands.py` & `pz-rail-hub-0.1.2/src/rail/hub/commands.py`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/src/rail/hub/options.py` & `pz-rail-hub-0.1.2/src/rail/hub/options.py`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/src/rail/hub/scripts.py` & `pz-rail-hub-0.1.2/src/rail/hub/scripts.py`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.1.1/tests/test_scripts.py` & `pz-rail-hub-0.1.2/tests/test_scripts.py`

 * *Files identical despite different names*

