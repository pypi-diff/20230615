# Comparing `tmp/napari_brainways-0.1.5.tar.gz` & `tmp/napari_brainways-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_brainways-0.1.5.tar", last modified: Fri Jun  9 09:41:44 2023, max compression
+gzip compressed data, was "napari_brainways-0.1.6.tar", last modified: Thu Jun 15 09:15:14 2023, max compression
```

## Comparing `napari_brainways-0.1.5.tar` & `napari_brainways-0.1.6.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.518506 napari_brainways-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.510506 napari_brainways-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.510506 napari_brainways-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.510506 napari_brainways-0.1.5/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-09 09:41:44.518506 napari_brainways-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.514506 napari_brainways-0.1.5/data/
--rw-r--r--   0 runner    (1001) docker     (123)   269441 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/data/test_data.npz
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-09 09:41:44.518506 napari_brainways-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.510506 napari_brainways-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.514506 napari_brainways-0.1.5/src/napari_brainways/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/_sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.514506 napari_brainways-0.1.5/src/napari_brainways/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-09 09:41:44.000000 napari_brainways-0.1.5/src/napari_brainways/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/brainways_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.514506 napari_brainways-0.1.5/src/napari_brainways/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.514506 napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/test_cell_detector_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/test_registration_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/test_tps_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/affine_2d_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/annotation_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/cell_3d_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/cell_detector_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/registration_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/controllers/tps_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/napari_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.518506 napari_brainways-0.1.5/src/napari_brainways/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   231054 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/resources/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.518506 napari_brainways-0.1.5/src/napari_brainways/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.518506 napari_brainways-0.1.5/src/napari_brainways/widgets/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/_tests/test_create_project_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/_tests/test_registration_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/affine_2d_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/cell_detector_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/cell_viewer_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/create_subject_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/registration_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/tps_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    22436 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/src/napari_brainways/widgets/workflow_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:41:44.514506 napari_brainways-0.1.5/src/napari_brainways.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-09 09:41:44.000000 napari_brainways-0.1.5/src/napari_brainways.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-09 09:41:44.000000 napari_brainways-0.1.5/src/napari_brainways.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:41:44.000000 napari_brainways-0.1.5/src/napari_brainways.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-09 09:41:44.000000 napari_brainways-0.1.5/src/napari_brainways.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-09 09:41:44.000000 napari_brainways-0.1.5/src/napari_brainways.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 09:41:44.000000 napari_brainways-0.1.5/src/napari_brainways.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-09 09:41:26.000000 napari_brainways-0.1.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:15:14.089362 napari_brainways-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:15:14.081362 napari_brainways-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:15:14.081362 napari_brainways-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:15:14.081362 napari_brainways-0.1.6/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-15 09:15:14.089362 napari_brainways-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:15:14.081362 napari_brainways-0.1.6/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   269441 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/data/test_data.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-15 09:15:14.089362 napari_brainways-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:15:14.081362 napari_brainways-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:15:14.085362 napari_brainways-0.1.6/src/napari_brainways/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:15:14.085362 napari_brainways-0.1.6/src/napari_brainways/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-15 09:15:14.000000 napari_brainways-0.1.6/src/napari_brainways/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/brainways_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:15:14.085362 napari_brainways-0.1.6/src/napari_brainways/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:15:14.085362 napari_brainways-0.1.6/src/napari_brainways/controllers/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/controllers/_tests/test_cell_detector_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/controllers/_tests/test_registration_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/controllers/_tests/test_tps_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/controllers/affine_2d_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/controllers/annotation_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/controllers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/controllers/cell_3d_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/controllers/cell_detector_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/controllers/registration_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/controllers/tps_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/napari_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:15:14.085362 napari_brainways-0.1.6/src/napari_brainways/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   231054 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/resources/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:15:14.089362 napari_brainways-0.1.6/src/napari_brainways/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:15:14.089362 napari_brainways-0.1.6/src/napari_brainways/widgets/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/widgets/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/widgets/_tests/test_create_project_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/widgets/_tests/test_registration_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/widgets/affine_2d_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/widgets/cell_detector_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/widgets/cell_viewer_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/widgets/create_subject_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/widgets/registration_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/widgets/tps_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22436 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/src/napari_brainways/widgets/workflow_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:15:14.085362 napari_brainways-0.1.6/src/napari_brainways.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-15 09:15:14.000000 napari_brainways-0.1.6/src/napari_brainways.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-15 09:15:14.000000 napari_brainways-0.1.6/src/napari_brainways.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:15:14.000000 napari_brainways-0.1.6/src/napari_brainways.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 09:15:14.000000 napari_brainways-0.1.6/src/napari_brainways.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-15 09:15:14.000000 napari_brainways-0.1.6/src/napari_brainways.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 09:15:14.000000 napari_brainways-0.1.6/src/napari_brainways.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-15 09:14:57.000000 napari_brainways-0.1.6/tox.ini
```

### Comparing `napari_brainways-0.1.5/.github/workflows/test_and_deploy.yml` & `napari_brainways-0.1.6/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/.gitignore` & `napari_brainways-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/.napari/DESCRIPTION.md` & `napari_brainways-0.1.6/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/.pre-commit-config.yaml` & `napari_brainways-0.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/LICENSE` & `napari_brainways-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/PKG-INFO` & `napari_brainways-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_brainways
-Version: 0.1.5
+Version: 0.1.6
 Summary: Brainways UI
 Home-page: https://github.com/bkntr/napari-brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/napari-brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/napari-brainways#README.md
```

### Comparing `napari_brainways-0.1.5/README.md` & `napari_brainways-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/data/test_data.npz` & `napari_brainways-0.1.6/data/test_data.npz`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/setup.cfg` & `napari_brainways-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/_sample_data.py` & `napari_brainways-0.1.6/src/napari_brainways/_sample_data.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/_tests/test_reader.py` & `napari_brainways-0.1.6/src/napari_brainways/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/_tests/test_widget.py` & `napari_brainways-0.1.6/src/napari_brainways/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/brainways_ui.py` & `napari_brainways-0.1.6/src/napari_brainways/brainways_ui.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/conftest.py` & `napari_brainways-0.1.6/src/napari_brainways/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
 @fixture
 def mock_atlas(test_data: Tuple[np.ndarray, AtlasSlice]) -> BrainwaysAtlas:
     test_image, test_atlas_slice = test_data
     ATLAS_SIZE = 32
     ATLAS_DEPTH = 10
     mock_atlas = create_autospec(BrainwaysAtlas)
-    mock_atlas.bounding_boxes = [(0, 0, ATLAS_SIZE, ATLAS_SIZE)] * ATLAS_DEPTH
+    mock_atlas.bounding_box = Mock(return_value=(0, 0, ATLAS_SIZE, ATLAS_SIZE))
     mock_atlas.shape = (ATLAS_DEPTH, ATLAS_SIZE, ATLAS_SIZE)
     mock_atlas.reference = torch.rand(ATLAS_DEPTH, ATLAS_SIZE, ATLAS_SIZE)
     mock_atlas.brainglobe_atlas = Mock()
     mock_atlas.brainglobe_atlas.structure_from_coords = Mock(return_value=10)
     mock_atlas.brainglobe_atlas.resolution = (1, 2, 3)
     mock_atlas.brainglobe_atlas.atlas_name = "MOCK_ATLAS"
     structures_list = [
```

### Comparing `napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py` & `napari_brainways-0.1.6/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py` & `napari_brainways-0.1.6/src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py` & `napari_brainways-0.1.6/src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/controllers/_tests/test_tps_controller.py` & `napari_brainways-0.1.6/src/napari_brainways/controllers/_tests/test_tps_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/controllers/affine_2d_controller.py` & `napari_brainways-0.1.6/src/napari_brainways/controllers/affine_2d_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/controllers/annotation_viewer_controller.py` & `napari_brainways-0.1.6/src/napari_brainways/controllers/annotation_viewer_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/controllers/base.py` & `napari_brainways-0.1.6/src/napari_brainways/controllers/base.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/controllers/cell_3d_viewer_controller.py` & `napari_brainways-0.1.6/src/napari_brainways/controllers/cell_3d_viewer_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/controllers/cell_detector_controller.py` & `napari_brainways-0.1.6/src/napari_brainways/controllers/cell_detector_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/controllers/registration_controller.py` & `napari_brainways-0.1.6/src/napari_brainways/controllers/registration_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
                 hemisphere=params.atlas.hemisphere,
             )
 
         atlas_slice = self.pipeline.get_atlas_slice(self.params).reference.numpy()
         self.atlas_slice_layer.data = atlas_slice
         update_layer_contrast_limits(self.atlas_slice_layer, (0.01, 0.98))
 
-        atlas_box = self.pipeline.atlas.bounding_boxes[int(self.params.atlas.ap)]
+        atlas_box = self.pipeline.atlas.bounding_box(int(self.params.atlas.ap))
         input_scale = atlas_box[3] / self._input_box[3]
         self.input_layer.scale = (input_scale, input_scale)
         self.mask_layer.scale = (input_scale, input_scale)
 
         tx = (self._input_box[0] + self._input_box[0] * 0.1) * input_scale
         ty = self._input_box[1] * input_scale - atlas_box[1]
         self.atlas_slice_layer.translate = (ty, tx)
```

### Comparing `napari_brainways-0.1.5/src/napari_brainways/controllers/tps_controller.py` & `napari_brainways-0.1.6/src/napari_brainways/controllers/tps_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/napari.yaml` & `napari_brainways-0.1.6/src/napari_brainways/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/napari_reader.py` & `napari_brainways-0.1.6/src/napari_brainways/napari_reader.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/resources/logo.png` & `napari_brainways-0.1.6/src/napari_brainways/resources/logo.png`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/test_utils.py` & `napari_brainways-0.1.6/src/napari_brainways/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/utils.py` & `napari_brainways-0.1.6/src/napari_brainways/utils.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/widgets/_tests/test_create_project_dialog.py` & `napari_brainways-0.1.6/src/napari_brainways/widgets/_tests/test_create_project_dialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from dataclasses import replace
 
+from aicsimageio.types import PhysicalPixelSizes
 from brainways.project.brainways_project import BrainwaysProject
 from brainways.project.info_classes import SliceInfo
 from brainways.utils.image import ImageSizeHW, get_resize_size
 from brainways.utils.io_utils import ImagePath
+from brainways.utils.io_utils.readers import QupathReader
 from pytest import fixture
 from pytestqt.qtbot import QtBot
 from qtpy.QtWidgets import QCheckBox
 
 from napari_brainways.test_utils import worker_join
 from napari_brainways.widgets.create_subject_dialog import CreateSubjectDialog
 
@@ -15,14 +17,15 @@
 @fixture
 def create_subject_dialog(
     qtbot: QtBot,
     mock_project: BrainwaysProject,
     mock_image_path: ImagePath,
     test_image_size: ImageSizeHW,
 ) -> CreateSubjectDialog:
+    QupathReader.physical_pixel_sizes = PhysicalPixelSizes(Z=None, Y=10.0, X=10.0)
     create_subject_dialog = CreateSubjectDialog(mock_project)
     create_subject_dialog.new_subject("test_subject")
     worker = create_subject_dialog.add_filenames_async([str(mock_image_path.filename)])
     worker_join(worker, qtbot)
     worker_join(create_subject_dialog._add_documents_worker, qtbot)
     return create_subject_dialog
 
@@ -33,14 +36,15 @@
 ) -> SliceInfo:
     return SliceInfo(
         path=mock_image_path,
         image_size=test_image_size,
         lowres_image_size=get_resize_size(
             test_image_size, (1024, 1024), keep_aspect=True
         ),
+        physical_pixel_sizes=(10.0, 10.0),
     )
 
 
 def test_documents(
     create_subject_dialog: CreateSubjectDialog,
     create_subject_document: SliceInfo,
 ):
```

### Comparing `napari_brainways-0.1.5/src/napari_brainways/widgets/_tests/test_registration_widget.py` & `napari_brainways-0.1.6/src/napari_brainways/widgets/_tests/test_registration_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/widgets/affine_2d_widget.py` & `napari_brainways-0.1.6/src/napari_brainways/widgets/affine_2d_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/widgets/cell_detector_widget.py` & `napari_brainways-0.1.6/src/napari_brainways/widgets/cell_detector_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/widgets/cell_viewer_widget.py` & `napari_brainways-0.1.6/src/napari_brainways/widgets/cell_viewer_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/widgets/create_subject_dialog.py` & `napari_brainways-0.1.6/src/napari_brainways/widgets/create_subject_dialog.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/widgets/registration_widget.py` & `napari_brainways-0.1.6/src/napari_brainways/widgets/registration_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/widgets/tps_widget.py` & `napari_brainways-0.1.6/src/napari_brainways/widgets/tps_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways/widgets/workflow_widget.py` & `napari_brainways-0.1.6/src/napari_brainways/widgets/workflow_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/src/napari_brainways.egg-info/PKG-INFO` & `napari_brainways-0.1.6/src/napari_brainways.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-brainways
-Version: 0.1.5
+Version: 0.1.6
 Summary: Brainways UI
 Home-page: https://github.com/bkntr/napari-brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/napari-brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/napari-brainways#README.md
```

### Comparing `napari_brainways-0.1.5/src/napari_brainways.egg-info/SOURCES.txt` & `napari_brainways-0.1.6/src/napari_brainways.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.5/tox.ini` & `napari_brainways-0.1.6/tox.ini`

 * *Files identical despite different names*

