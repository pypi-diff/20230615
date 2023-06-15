# Comparing `tmp/brainways-0.1.5.tar.gz` & `tmp/brainways-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainways-0.1.5.tar", last modified: Fri Jun  9 09:31:57 2023, max compression
+gzip compressed data, was "brainways-0.1.6.tar", last modified: Thu Jun 15 09:13:26 2023, max compression
```

## Comparing `brainways-0.1.5.tar` & `brainways-0.1.6.tar`

### file list

```diff
@@ -1,187 +1,188 @@
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.298109 brainways-0.1.5/
--rw-rw-r--   0 ben       (1001) ben       (1001)      292 2022-07-13 13:47:58.000000 brainways-0.1.5/.editorconfig
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.282109 brainways-0.1.5/.github/
--rw-rw-r--   0 ben       (1001) ben       (1001)      320 2022-07-13 13:47:58.000000 brainways-0.1.5/.github/ISSUE_TEMPLATE.md
--rw-rw-r--   0 ben       (1001) ben       (1001)     1248 2022-07-13 14:46:16.000000 brainways-0.1.5/.gitignore
--rw-rw-r--   0 ben       (1001) ben       (1001)     1194 2022-07-14 13:50:01.000000 brainways-0.1.5/.pre-commit-config.yaml
--rw-rw-r--   0 ben       (1001) ben       (1001)      681 2022-07-13 13:47:58.000000 brainways-0.1.5/.travis.yml
--rw-rw-r--   0 ben       (1001) ben       (1001)      160 2022-07-13 13:47:58.000000 brainways-0.1.5/AUTHORS.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     3523 2022-07-13 13:47:58.000000 brainways-0.1.5/CONTRIBUTING.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)       89 2022-07-13 13:47:58.000000 brainways-0.1.5/HISTORY.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)    35148 2022-08-24 08:26:24.000000 brainways-0.1.5/LICENSE
--rw-rw-r--   0 ben       (1001) ben       (1001)      262 2022-07-13 13:47:58.000000 brainways-0.1.5/MANIFEST.in
--rw-rw-r--   0 ben       (1001) ben       (1001)     2430 2023-05-26 08:21:13.000000 brainways-0.1.5/Makefile
--rw-rw-r--   0 ben       (1001) ben       (1001)     2343 2023-06-09 09:31:57.298109 brainways-0.1.5/PKG-INFO
--rw-rw-r--   0 ben       (1001) ben       (1001)      962 2023-05-26 08:25:05.000000 brainways-0.1.5/README.rst
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.282109 brainways-0.1.5/data/
--rw-rw-r--   0 ben       (1001) ben       (1001)   269441 2022-03-11 09:30:01.000000 brainways-0.1.5/data/test_data.npz
--rw-rw-r--   0 ben       (1001) ben       (1001)    47973 2022-06-30 11:17:43.000000 brainways-0.1.5/data/test_image.jpg
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.286109 brainways-0.1.5/docs/
--rw-rw-r--   0 ben       (1001) ben       (1001)      610 2022-07-13 13:47:58.000000 brainways-0.1.5/docs/Makefile
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.278109 brainways-0.1.5/docs/_build/
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.278109 brainways-0.1.5/docs/_build/html/
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.286109 brainways-0.1.5/docs/_build/html/_static/
--rw-rw-r--   0 ben       (1001) ben       (1001)      286 2022-10-06 11:03:00.000000 brainways-0.1.5/docs/_build/html/_static/file.png
--rw-rw-r--   0 ben       (1001) ben       (1001)       90 2022-10-06 11:03:00.000000 brainways-0.1.5/docs/_build/html/_static/minus.png
--rw-rw-r--   0 ben       (1001) ben       (1001)       90 2022-10-06 11:03:00.000000 brainways-0.1.5/docs/_build/html/_static/plus.png
--rw-rw-r--   0 ben       (1001) ben       (1001)       28 2022-07-13 13:47:58.000000 brainways-0.1.5/docs/authors.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      361 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.elastix.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1317 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.pipeline.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      770 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.project.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      500 2023-05-26 08:26:43.000000 brainways-0.1.5/docs/brainways.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     2137 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.scripts.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1387 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.transforms.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      601 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.utils.atlas.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1405 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.utils.cell_detection_importer.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      386 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.utils.czi.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      971 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.utils.io_utils.file_iterators.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1145 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.utils.io_utils.readers.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      553 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.utils.io_utils.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1833 2023-05-26 08:18:55.000000 brainways-0.1.5/docs/brainways.utils.rst
--rwxrwxr-x   0 ben       (1001) ben       (1001)     4967 2023-05-26 08:17:55.000000 brainways-0.1.5/docs/conf.py
--rw-rw-r--   0 ben       (1001) ben       (1001)       33 2022-07-13 13:47:58.000000 brainways-0.1.5/docs/contributing.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)       28 2022-07-13 13:47:58.000000 brainways-0.1.5/docs/history.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      306 2022-07-13 13:47:58.000000 brainways-0.1.5/docs/index.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1118 2022-07-13 13:47:58.000000 brainways-0.1.5/docs/installation.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      807 2022-07-13 13:47:58.000000 brainways-0.1.5/docs/make.bat
--rw-rw-r--   0 ben       (1001) ben       (1001)       64 2023-05-26 08:26:43.000000 brainways-0.1.5/docs/modules.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)       27 2022-07-13 13:47:58.000000 brainways-0.1.5/docs/readme.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)       73 2022-07-13 13:47:58.000000 brainways-0.1.5/docs/usage.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      383 2023-05-26 08:03:19.000000 brainways-0.1.5/pyproject.toml
--rw-rw-r--   0 ben       (1001) ben       (1001)      165 2022-07-13 14:08:33.000000 brainways-0.1.5/requirements_dev.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)     1967 2023-06-09 09:31:57.298109 brainways-0.1.5/setup.cfg
--rw-rw-r--   0 ben       (1001) ben       (1001)       60 2023-05-26 07:59:05.000000 brainways-0.1.5/setup.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.278109 brainways-0.1.5/src/
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.286109 brainways-0.1.5/src/brainways/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-13 14:28:10.000000 brainways-0.1.5/src/brainways/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      160 2023-06-09 09:31:57.000000 brainways-0.1.5/src/brainways/_version.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     7423 2023-06-09 09:30:50.000000 brainways-0.1.5/src/brainways/conftest.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.286109 brainways-0.1.5/src/brainways/elastix/
--rw-rw-r--   0 ben       (1001) ben       (1001)     2596 2022-07-14 13:40:58.000000 brainways-0.1.5/src/brainways/elastix/Par0033bspline.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)     2316 2022-07-14 13:40:58.000000 brainways-0.1.5/src/brainways/elastix/Par0033similarity.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-12-09 12:20:50.000000 brainways-0.1.5/src/brainways/elastix/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.286109 brainways-0.1.5/src/brainways/elastix/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)      592 2022-10-27 09:03:02.000000 brainways-0.1.5/src/brainways/elastix/_tests/test_elastix.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2649 2022-09-08 14:32:33.000000 brainways-0.1.5/src/brainways/elastix/elastix.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.286109 brainways-0.1.5/src/brainways/pipeline/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-07 09:39:04.000000 brainways-0.1.5/src/brainways/pipeline/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.286109 brainways-0.1.5/src/brainways/pipeline/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)      430 2022-10-27 09:03:02.000000 brainways-0.1.5/src/brainways/pipeline/_tests/test_atlas_registration.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      552 2022-11-23 11:34:52.000000 brainways-0.1.5/src/brainways/pipeline/_tests/test_brainways_pipeline.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      370 2023-06-09 09:30:50.000000 brainways-0.1.5/src/brainways/pipeline/_tests/test_cell_detector.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1097 2022-11-30 13:23:46.000000 brainways-0.1.5/src/brainways/pipeline/affine_2d.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2339 2023-05-24 12:27:57.000000 brainways-0.1.5/src/brainways/pipeline/atlas_registration.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1165 2023-06-07 14:11:19.000000 brainways-0.1.5/src/brainways/pipeline/brainways_params.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3712 2022-11-30 13:35:53.000000 brainways-0.1.5/src/brainways/pipeline/brainways_pipeline.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     5186 2023-06-09 09:29:12.000000 brainways-0.1.5/src/brainways/pipeline/cell_detector.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1596 2022-11-30 13:25:23.000000 brainways-0.1.5/src/brainways/pipeline/tps.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.290109 brainways-0.1.5/src/brainways/project/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-07 09:39:04.000000 brainways-0.1.5/src/brainways/project/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.290109 brainways-0.1.5/src/brainways/project/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.5/src/brainways/project/_tests/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2139 2023-06-09 09:23:33.000000 brainways-0.1.5/src/brainways/project/_tests/conftest.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3207 2023-06-09 09:25:09.000000 brainways-0.1.5/src/brainways/project/_tests/test_brainways_project.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     8662 2023-06-09 09:09:06.000000 brainways-0.1.5/src/brainways/project/_tests/test_brainways_subject.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.278109 brainways-0.1.5/src/brainways/project/_tests/test_projects/
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.290109 brainways-0.1.5/src/brainways/project/_tests/test_projects/v0.1.1/
--rw-rw-r--   0 ben       (1001) ben       (1001)       38 2023-06-07 15:59:39.000000 brainways-0.1.5/src/brainways/project/_tests/test_projects/v0.1.1/project.bwp
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.290109 brainways-0.1.5/src/brainways/project/_tests/test_projects/v0.1.1/subject1/
--rw-rw-r--   0 ben       (1001) ben       (1001)     2016 2023-06-09 09:23:59.000000 brainways-0.1.5/src/brainways/project/_tests/test_projects/v0.1.1/subject1/brainways.bin
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.290109 brainways-0.1.5/src/brainways/project/_tests/test_projects/v0.1.4/
--rw-rw-r--   0 ben       (1001) ben       (1001)      153 2023-06-09 09:30:50.000000 brainways-0.1.5/src/brainways/project/_tests/test_projects/v0.1.4/project.bwp
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.290109 brainways-0.1.5/src/brainways/project/_tests/test_projects/v0.1.4/subject1/
--rw-rw-r--   0 ben       (1001) ben       (1001)     1902 2023-06-09 09:25:14.000000 brainways-0.1.5/src/brainways/project/_tests/test_projects/v0.1.4/subject1/brainways.bin
--rw-rw-r--   0 ben       (1001) ben       (1001)      697 2023-06-09 08:13:53.000000 brainways-0.1.5/src/brainways/project/_tests/test_utils.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2428 2023-06-09 09:30:50.000000 brainways-0.1.5/src/brainways/project/_utils.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     8792 2023-06-07 15:29:27.000000 brainways-0.1.5/src/brainways/project/brainways_project.py
--rw-rw-r--   0 ben       (1001) ben       (1001)    18570 2023-06-09 09:06:00.000000 brainways-0.1.5/src/brainways/project/brainways_subject.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1388 2023-06-07 15:59:32.000000 brainways-0.1.5/src/brainways/project/info_classes.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.290109 brainways-0.1.5/src/brainways/scripts/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.5/src/brainways/scripts/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.290109 brainways-0.1.5/src/brainways/scripts/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)      920 2023-05-26 08:21:13.000000 brainways-0.1.5/src/brainways/scripts/_tests/test_cli.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3031 2022-09-08 14:06:58.000000 brainways-0.1.5/src/brainways/scripts/batch_create_thumbnails.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3053 2023-05-07 14:18:30.000000 brainways-0.1.5/src/brainways/scripts/cell_detection.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1142 2023-05-04 08:18:52.000000 brainways-0.1.5/src/brainways/scripts/cli.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1588 2023-05-07 14:18:29.000000 brainways-0.1.5/src/brainways/scripts/create_excel.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4944 2022-11-30 14:10:59.000000 brainways-0.1.5/src/brainways/scripts/create_excel_colabelling.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4023 2022-11-23 12:26:10.000000 brainways-0.1.5/src/brainways/scripts/create_reg_model_data.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     5253 2022-11-23 12:35:34.000000 brainways-0.1.5/src/brainways/scripts/display_area.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1618 2022-12-08 14:20:04.000000 brainways-0.1.5/src/brainways/scripts/import_cell_detections_keren.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1192 2022-11-23 12:26:10.000000 brainways-0.1.5/src/brainways/scripts/import_cells.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      920 2022-12-11 10:14:02.000000 brainways-0.1.5/src/brainways/scripts/move_images.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.290109 brainways-0.1.5/src/brainways/transforms/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.5/src/brainways/transforms/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.294109 brainways-0.1.5/src/brainways/transforms/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.5/src/brainways/transforms/_tests/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2173 2022-07-14 13:48:40.000000 brainways-0.1.5/src/brainways/transforms/_tests/test_affine_transform_2d.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1813 2022-11-23 11:35:37.000000 brainways-0.1.5/src/brainways/transforms/_tests/test_depth_registration.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2034 2022-07-14 13:48:40.000000 brainways-0.1.5/src/brainways/transforms/_tests/test_image_to_atlas_transform.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2667 2022-07-14 13:48:40.000000 brainways-0.1.5/src/brainways/transforms/_tests/test_tps_transform.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4104 2022-11-30 13:34:33.000000 brainways-0.1.5/src/brainways/transforms/affine_transform_2d.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      436 2022-07-14 12:46:19.000000 brainways-0.1.5/src/brainways/transforms/base.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      623 2022-07-14 13:40:58.000000 brainways-0.1.5/src/brainways/transforms/compose.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2594 2022-07-14 13:48:40.000000 brainways-0.1.5/src/brainways/transforms/depth_registration.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2205 2022-09-08 13:13:42.000000 brainways-0.1.5/src/brainways/transforms/image_to_atlas_transform.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2185 2022-11-30 13:46:38.000000 brainways-0.1.5/src/brainways/transforms/tps_transform.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.294109 brainways-0.1.5/src/brainways/utils/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-21 08:14:53.000000 brainways-0.1.5/src/brainways/utils/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1674 2022-07-17 07:51:20.000000 brainways-0.1.5/src/brainways/utils/_imports.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.294109 brainways-0.1.5/src/brainways/utils/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.5/src/brainways/utils/_tests/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     7710 2023-05-26 08:21:13.000000 brainways-0.1.5/src/brainways/utils/_tests/test_cell_count_summary.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2715 2023-05-07 14:18:30.000000 brainways-0.1.5/src/brainways/utils/_tests/test_cells.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2412 2022-07-14 13:48:40.000000 brainways-0.1.5/src/brainways/utils/_tests/test_image.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.294109 brainways-0.1.5/src/brainways/utils/atlas/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-21 11:07:35.000000 brainways-0.1.5/src/brainways/utils/atlas/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.294109 brainways-0.1.5/src/brainways/utils/atlas/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.5/src/brainways/utils/atlas/_tests/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3708 2022-07-14 13:40:59.000000 brainways-0.1.5/src/brainways/utils/atlas/_tests/test_slice_atlas.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4263 2022-12-11 16:13:39.000000 brainways-0.1.5/src/brainways/utils/atlas/brainways_atlas.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2280 2023-05-04 09:01:16.000000 brainways-0.1.5/src/brainways/utils/atlas/slice_atlas.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     5751 2023-05-14 15:00:03.000000 brainways-0.1.5/src/brainways/utils/cell_count_summary.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.294109 brainways-0.1.5/src/brainways/utils/cell_detection_importer/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-10-06 09:31:17.000000 brainways-0.1.5/src/brainways/utils/cell_detection_importer/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.294109 brainways-0.1.5/src/brainways/utils/cell_detection_importer/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)     7465 2022-10-06 10:12:40.000000 brainways-0.1.5/src/brainways/utils/cell_detection_importer/_tests/qupath_sample_file.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)     1240 2022-11-23 12:23:47.000000 brainways-0.1.5/src/brainways/utils/cell_detection_importer/_tests/test_brainways_cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1722 2022-12-08 14:20:04.000000 brainways-0.1.5/src/brainways/utils/cell_detection_importer/_tests/test_qupath_cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1343 2022-11-23 12:26:10.000000 brainways-0.1.5/src/brainways/utils/cell_detection_importer/brainways_cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      507 2022-11-27 15:04:03.000000 brainways-0.1.5/src/brainways/utils/cell_detection_importer/cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2438 2022-12-11 10:33:01.000000 brainways-0.1.5/src/brainways/utils/cell_detection_importer/keren_cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      731 2022-12-08 14:20:04.000000 brainways-0.1.5/src/brainways/utils/cell_detection_importer/utils.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4985 2023-05-02 09:29:03.000000 brainways-0.1.5/src/brainways/utils/cells.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4270 2022-09-11 13:34:36.000000 brainways-0.1.5/src/brainways/utils/config.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.294109 brainways-0.1.5/src/brainways/utils/czi/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-15 08:31:32.000000 brainways-0.1.5/src/brainways/utils/czi/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1112 2022-07-14 13:48:40.000000 brainways-0.1.5/src/brainways/utils/czi/czi_to_jpg.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      793 2022-07-14 12:49:34.000000 brainways-0.1.5/src/brainways/utils/dataclasses.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     9025 2023-05-26 13:51:47.000000 brainways-0.1.5/src/brainways/utils/image.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.298109 brainways-0.1.5/src/brainways/utils/io_utils/
--rw-rw-r--   0 ben       (1001) ben       (1001)       42 2022-07-17 07:44:03.000000 brainways-0.1.5/src/brainways/utils/io_utils/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.298109 brainways-0.1.5/src/brainways/utils/io_utils/file_iterators/
--rw-rw-r--   0 ben       (1001) ben       (1001)      379 2022-09-08 08:38:22.000000 brainways-0.1.5/src/brainways/utils/io_utils/file_iterators/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      230 2022-07-07 09:39:04.000000 brainways-0.1.5/src/brainways/utils/io_utils/file_iterators/image_entry.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      407 2022-07-07 09:39:04.000000 brainways-0.1.5/src/brainways/utils/io_utils/file_iterators/path.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      914 2022-11-23 12:29:43.000000 brainways-0.1.5/src/brainways/utils/io_utils/file_iterators/qupath.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      630 2022-07-07 09:39:09.000000 brainways-0.1.5/src/brainways/utils/io_utils/image_path.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.298109 brainways-0.1.5/src/brainways/utils/io_utils/readers/
--rw-rw-r--   0 ben       (1001) ben       (1001)     1041 2022-09-11 12:16:49.000000 brainways-0.1.5/src/brainways/utils/io_utils/readers/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.298109 brainways-0.1.5/src/brainways/utils/io_utils/readers/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)      218 2022-09-22 07:42:16.000000 brainways-0.1.5/src/brainways/utils/io_utils/readers/_tests/test_qupath_reader.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1419 2022-09-08 08:38:21.000000 brainways-0.1.5/src/brainways/utils/io_utils/readers/aicsimageio_reader.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      649 2022-07-14 12:39:58.000000 brainways-0.1.5/src/brainways/utils/io_utils/readers/base.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1364 2022-09-08 08:38:21.000000 brainways-0.1.5/src/brainways/utils/io_utils/readers/czi_reader.py
--rw-rw-r--   0 ben       (1001) ben       (1001)    15748 2023-05-21 10:26:48.000000 brainways-0.1.5/src/brainways/utils/io_utils/readers/qupath_reader.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      108 2022-09-11 13:34:36.000000 brainways-0.1.5/src/brainways/utils/paths.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1181 2022-07-14 13:48:40.000000 brainways-0.1.5/src/brainways/utils/preprocess.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3183 2022-09-11 10:47:30.000000 brainways-0.1.5/src/brainways/utils/qupath.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1083 2022-07-14 13:48:39.000000 brainways-0.1.5/src/brainways/utils/test_utils.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-09 09:31:57.286109 brainways-0.1.5/src/brainways.egg-info/
--rw-rw-r--   0 ben       (1001) ben       (1001)     2343 2023-06-09 09:31:57.000000 brainways-0.1.5/src/brainways.egg-info/PKG-INFO
--rw-rw-r--   0 ben       (1001) ben       (1001)     5729 2023-06-09 09:31:57.000000 brainways-0.1.5/src/brainways.egg-info/SOURCES.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)        1 2023-06-09 09:31:57.000000 brainways-0.1.5/src/brainways.egg-info/dependency_links.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)       57 2023-06-09 09:31:57.000000 brainways-0.1.5/src/brainways.egg-info/entry_points.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)      413 2023-06-09 09:31:57.000000 brainways-0.1.5/src/brainways.egg-info/requires.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)       10 2023-06-09 09:31:57.000000 brainways-0.1.5/src/brainways.egg-info/top_level.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)      540 2022-07-13 13:47:58.000000 brainways-0.1.5/tox.ini
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.988741 brainways-0.1.6/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      292 2022-07-13 13:47:58.000000 brainways-0.1.6/.editorconfig
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.972741 brainways-0.1.6/.github/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      320 2022-07-13 13:47:58.000000 brainways-0.1.6/.github/ISSUE_TEMPLATE.md
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1248 2022-07-13 14:46:16.000000 brainways-0.1.6/.gitignore
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1194 2022-07-14 13:50:01.000000 brainways-0.1.6/.pre-commit-config.yaml
+-rw-rw-r--   0 ben       (1001) ben       (1001)      681 2022-07-13 13:47:58.000000 brainways-0.1.6/.travis.yml
+-rw-rw-r--   0 ben       (1001) ben       (1001)      160 2022-07-13 13:47:58.000000 brainways-0.1.6/AUTHORS.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3523 2022-07-13 13:47:58.000000 brainways-0.1.6/CONTRIBUTING.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)       89 2022-07-13 13:47:58.000000 brainways-0.1.6/HISTORY.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)    35148 2022-08-24 08:26:24.000000 brainways-0.1.6/LICENSE
+-rw-rw-r--   0 ben       (1001) ben       (1001)      262 2022-07-13 13:47:58.000000 brainways-0.1.6/MANIFEST.in
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2430 2023-05-26 08:21:13.000000 brainways-0.1.6/Makefile
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2343 2023-06-15 09:13:26.988741 brainways-0.1.6/PKG-INFO
+-rw-rw-r--   0 ben       (1001) ben       (1001)      962 2023-05-26 08:25:05.000000 brainways-0.1.6/README.rst
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.972741 brainways-0.1.6/data/
+-rw-rw-r--   0 ben       (1001) ben       (1001)   269441 2022-03-11 09:30:01.000000 brainways-0.1.6/data/test_data.npz
+-rw-rw-r--   0 ben       (1001) ben       (1001)    47973 2022-06-30 11:17:43.000000 brainways-0.1.6/data/test_image.jpg
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.972741 brainways-0.1.6/docs/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      610 2022-07-13 13:47:58.000000 brainways-0.1.6/docs/Makefile
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.968741 brainways-0.1.6/docs/_build/
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.968741 brainways-0.1.6/docs/_build/html/
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.972741 brainways-0.1.6/docs/_build/html/_static/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      286 2022-10-06 11:03:00.000000 brainways-0.1.6/docs/_build/html/_static/file.png
+-rw-rw-r--   0 ben       (1001) ben       (1001)       90 2022-10-06 11:03:00.000000 brainways-0.1.6/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 ben       (1001) ben       (1001)       90 2022-10-06 11:03:00.000000 brainways-0.1.6/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 ben       (1001) ben       (1001)       28 2022-07-13 13:47:58.000000 brainways-0.1.6/docs/authors.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      361 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.elastix.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1317 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.pipeline.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      770 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.project.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      500 2023-05-26 08:26:43.000000 brainways-0.1.6/docs/brainways.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2137 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.scripts.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1387 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.transforms.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      601 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.utils.atlas.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1405 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.utils.cell_detection_importer.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      386 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.utils.czi.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      971 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.utils.io_utils.file_iterators.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1145 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.utils.io_utils.readers.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      553 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.utils.io_utils.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1833 2023-05-26 08:18:55.000000 brainways-0.1.6/docs/brainways.utils.rst
+-rwxrwxr-x   0 ben       (1001) ben       (1001)     4967 2023-05-26 08:17:55.000000 brainways-0.1.6/docs/conf.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)       33 2022-07-13 13:47:58.000000 brainways-0.1.6/docs/contributing.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)       28 2022-07-13 13:47:58.000000 brainways-0.1.6/docs/history.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      306 2022-07-13 13:47:58.000000 brainways-0.1.6/docs/index.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1118 2022-07-13 13:47:58.000000 brainways-0.1.6/docs/installation.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      807 2022-07-13 13:47:58.000000 brainways-0.1.6/docs/make.bat
+-rw-rw-r--   0 ben       (1001) ben       (1001)       64 2023-05-26 08:26:43.000000 brainways-0.1.6/docs/modules.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)       27 2022-07-13 13:47:58.000000 brainways-0.1.6/docs/readme.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)       73 2022-07-13 13:47:58.000000 brainways-0.1.6/docs/usage.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      383 2023-05-26 08:03:19.000000 brainways-0.1.6/pyproject.toml
+-rw-rw-r--   0 ben       (1001) ben       (1001)      165 2022-07-13 14:08:33.000000 brainways-0.1.6/requirements_dev.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1967 2023-06-15 09:13:26.988741 brainways-0.1.6/setup.cfg
+-rw-rw-r--   0 ben       (1001) ben       (1001)       60 2023-05-26 07:59:05.000000 brainways-0.1.6/setup.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.968741 brainways-0.1.6/src/
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.972741 brainways-0.1.6/src/brainways/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-13 14:28:10.000000 brainways-0.1.6/src/brainways/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      160 2023-06-15 09:13:26.000000 brainways-0.1.6/src/brainways/_version.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     7627 2023-06-14 09:09:25.000000 brainways-0.1.6/src/brainways/conftest.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.976741 brainways-0.1.6/src/brainways/elastix/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2596 2022-07-14 13:40:58.000000 brainways-0.1.6/src/brainways/elastix/Par0033bspline.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2316 2022-07-14 13:40:58.000000 brainways-0.1.6/src/brainways/elastix/Par0033similarity.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-12-09 12:20:50.000000 brainways-0.1.6/src/brainways/elastix/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.976741 brainways-0.1.6/src/brainways/elastix/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      592 2022-10-27 09:03:02.000000 brainways-0.1.6/src/brainways/elastix/_tests/test_elastix.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2649 2022-09-08 14:32:33.000000 brainways-0.1.6/src/brainways/elastix/elastix.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.976741 brainways-0.1.6/src/brainways/pipeline/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-07 09:39:04.000000 brainways-0.1.6/src/brainways/pipeline/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.976741 brainways-0.1.6/src/brainways/pipeline/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      430 2022-10-27 09:03:02.000000 brainways-0.1.6/src/brainways/pipeline/_tests/test_atlas_registration.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      552 2022-11-23 11:34:52.000000 brainways-0.1.6/src/brainways/pipeline/_tests/test_brainways_pipeline.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      370 2023-06-09 09:30:50.000000 brainways-0.1.6/src/brainways/pipeline/_tests/test_cell_detector.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1097 2022-11-30 13:23:46.000000 brainways-0.1.6/src/brainways/pipeline/affine_2d.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2339 2023-05-24 12:27:57.000000 brainways-0.1.6/src/brainways/pipeline/atlas_registration.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1165 2023-06-07 14:11:19.000000 brainways-0.1.6/src/brainways/pipeline/brainways_params.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3712 2022-11-30 13:35:53.000000 brainways-0.1.6/src/brainways/pipeline/brainways_pipeline.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     5186 2023-06-09 09:29:12.000000 brainways-0.1.6/src/brainways/pipeline/cell_detector.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1596 2022-11-30 13:25:23.000000 brainways-0.1.6/src/brainways/pipeline/tps.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.976741 brainways-0.1.6/src/brainways/project/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-07 09:39:04.000000 brainways-0.1.6/src/brainways/project/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.976741 brainways-0.1.6/src/brainways/project/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.6/src/brainways/project/_tests/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2145 2023-06-15 09:11:39.000000 brainways-0.1.6/src/brainways/project/_tests/conftest.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3207 2023-06-09 09:25:09.000000 brainways-0.1.6/src/brainways/project/_tests/test_brainways_project.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     8662 2023-06-09 09:09:06.000000 brainways-0.1.6/src/brainways/project/_tests/test_brainways_subject.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.968741 brainways-0.1.6/src/brainways/project/_tests/test_projects/
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.976741 brainways-0.1.6/src/brainways/project/_tests/test_projects/v0.1.1/
+-rw-rw-r--   0 ben       (1001) ben       (1001)       38 2023-06-07 15:59:39.000000 brainways-0.1.6/src/brainways/project/_tests/test_projects/v0.1.1/project.bwp
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.976741 brainways-0.1.6/src/brainways/project/_tests/test_projects/v0.1.1/subject1/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2016 2023-06-15 09:11:42.000000 brainways-0.1.6/src/brainways/project/_tests/test_projects/v0.1.1/subject1/brainways.bin
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.980741 brainways-0.1.6/src/brainways/project/_tests/test_projects/v0.1.4/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      153 2023-06-09 09:30:50.000000 brainways-0.1.6/src/brainways/project/_tests/test_projects/v0.1.4/project.bwp
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.980741 brainways-0.1.6/src/brainways/project/_tests/test_projects/v0.1.4/subject1/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1902 2023-06-15 09:11:42.000000 brainways-0.1.6/src/brainways/project/_tests/test_projects/v0.1.4/subject1/brainways.bin
+-rw-rw-r--   0 ben       (1001) ben       (1001)      697 2023-06-09 08:13:53.000000 brainways-0.1.6/src/brainways/project/_tests/test_utils.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2428 2023-06-09 09:30:50.000000 brainways-0.1.6/src/brainways/project/_utils.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     8792 2023-06-15 08:57:35.000000 brainways-0.1.6/src/brainways/project/brainways_project.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)    18570 2023-06-09 09:06:00.000000 brainways-0.1.6/src/brainways/project/brainways_subject.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1388 2023-06-07 15:59:32.000000 brainways-0.1.6/src/brainways/project/info_classes.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.980741 brainways-0.1.6/src/brainways/scripts/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.6/src/brainways/scripts/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.980741 brainways-0.1.6/src/brainways/scripts/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      920 2023-05-26 08:21:13.000000 brainways-0.1.6/src/brainways/scripts/_tests/test_cli.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3031 2022-09-08 14:06:58.000000 brainways-0.1.6/src/brainways/scripts/batch_create_thumbnails.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3053 2023-05-07 14:18:30.000000 brainways-0.1.6/src/brainways/scripts/cell_detection.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1142 2023-05-04 08:18:52.000000 brainways-0.1.6/src/brainways/scripts/cli.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1588 2023-05-07 14:18:29.000000 brainways-0.1.6/src/brainways/scripts/create_excel.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4944 2022-11-30 14:10:59.000000 brainways-0.1.6/src/brainways/scripts/create_excel_colabelling.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4023 2022-11-23 12:26:10.000000 brainways-0.1.6/src/brainways/scripts/create_reg_model_data.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     5253 2022-11-23 12:35:34.000000 brainways-0.1.6/src/brainways/scripts/display_area.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1618 2022-12-08 14:20:04.000000 brainways-0.1.6/src/brainways/scripts/import_cell_detections_keren.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1192 2022-11-23 12:26:10.000000 brainways-0.1.6/src/brainways/scripts/import_cells.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      920 2022-12-11 10:14:02.000000 brainways-0.1.6/src/brainways/scripts/move_images.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.980741 brainways-0.1.6/src/brainways/transforms/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.6/src/brainways/transforms/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.980741 brainways-0.1.6/src/brainways/transforms/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.6/src/brainways/transforms/_tests/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2173 2022-07-14 13:48:40.000000 brainways-0.1.6/src/brainways/transforms/_tests/test_affine_transform_2d.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1813 2022-11-23 11:35:37.000000 brainways-0.1.6/src/brainways/transforms/_tests/test_depth_registration.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2034 2022-07-14 13:48:40.000000 brainways-0.1.6/src/brainways/transforms/_tests/test_image_to_atlas_transform.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2667 2022-07-14 13:48:40.000000 brainways-0.1.6/src/brainways/transforms/_tests/test_tps_transform.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4104 2022-11-30 13:34:33.000000 brainways-0.1.6/src/brainways/transforms/affine_transform_2d.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      436 2022-07-14 12:46:19.000000 brainways-0.1.6/src/brainways/transforms/base.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      623 2022-07-14 13:40:58.000000 brainways-0.1.6/src/brainways/transforms/compose.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2594 2022-07-14 13:48:40.000000 brainways-0.1.6/src/brainways/transforms/depth_registration.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2205 2022-09-08 13:13:42.000000 brainways-0.1.6/src/brainways/transforms/image_to_atlas_transform.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2185 2022-11-30 13:46:38.000000 brainways-0.1.6/src/brainways/transforms/tps_transform.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.984741 brainways-0.1.6/src/brainways/utils/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-21 08:14:53.000000 brainways-0.1.6/src/brainways/utils/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1674 2022-07-17 07:51:20.000000 brainways-0.1.6/src/brainways/utils/_imports.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.984741 brainways-0.1.6/src/brainways/utils/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.6/src/brainways/utils/_tests/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     7710 2023-05-26 08:21:13.000000 brainways-0.1.6/src/brainways/utils/_tests/test_cell_count_summary.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2715 2023-05-07 14:18:30.000000 brainways-0.1.6/src/brainways/utils/_tests/test_cells.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2412 2022-07-14 13:48:40.000000 brainways-0.1.6/src/brainways/utils/_tests/test_image.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.984741 brainways-0.1.6/src/brainways/utils/atlas/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-21 11:07:35.000000 brainways-0.1.6/src/brainways/utils/atlas/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.984741 brainways-0.1.6/src/brainways/utils/atlas/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.6/src/brainways/utils/atlas/_tests/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      222 2023-06-14 09:20:14.000000 brainways-0.1.6/src/brainways/utils/atlas/_tests/test_brainways_atlas.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3708 2022-07-14 13:40:59.000000 brainways-0.1.6/src/brainways/utils/atlas/_tests/test_slice_atlas.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3790 2023-06-15 08:58:02.000000 brainways-0.1.6/src/brainways/utils/atlas/brainways_atlas.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2280 2023-05-04 09:01:16.000000 brainways-0.1.6/src/brainways/utils/atlas/slice_atlas.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     5751 2023-05-14 15:00:03.000000 brainways-0.1.6/src/brainways/utils/cell_count_summary.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.984741 brainways-0.1.6/src/brainways/utils/cell_detection_importer/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-10-06 09:31:17.000000 brainways-0.1.6/src/brainways/utils/cell_detection_importer/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.984741 brainways-0.1.6/src/brainways/utils/cell_detection_importer/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     7465 2022-10-06 10:12:40.000000 brainways-0.1.6/src/brainways/utils/cell_detection_importer/_tests/qupath_sample_file.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1240 2022-11-23 12:23:47.000000 brainways-0.1.6/src/brainways/utils/cell_detection_importer/_tests/test_brainways_cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1722 2022-12-08 14:20:04.000000 brainways-0.1.6/src/brainways/utils/cell_detection_importer/_tests/test_qupath_cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1343 2022-11-23 12:26:10.000000 brainways-0.1.6/src/brainways/utils/cell_detection_importer/brainways_cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      507 2022-11-27 15:04:03.000000 brainways-0.1.6/src/brainways/utils/cell_detection_importer/cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2438 2022-12-11 10:33:01.000000 brainways-0.1.6/src/brainways/utils/cell_detection_importer/keren_cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      731 2022-12-08 14:20:04.000000 brainways-0.1.6/src/brainways/utils/cell_detection_importer/utils.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4985 2023-05-02 09:29:03.000000 brainways-0.1.6/src/brainways/utils/cells.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4270 2022-09-11 13:34:36.000000 brainways-0.1.6/src/brainways/utils/config.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.984741 brainways-0.1.6/src/brainways/utils/czi/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-15 08:31:32.000000 brainways-0.1.6/src/brainways/utils/czi/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1112 2022-07-14 13:48:40.000000 brainways-0.1.6/src/brainways/utils/czi/czi_to_jpg.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      793 2022-07-14 12:49:34.000000 brainways-0.1.6/src/brainways/utils/dataclasses.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     9025 2023-05-26 13:51:47.000000 brainways-0.1.6/src/brainways/utils/image.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.984741 brainways-0.1.6/src/brainways/utils/io_utils/
+-rw-rw-r--   0 ben       (1001) ben       (1001)       42 2022-07-17 07:44:03.000000 brainways-0.1.6/src/brainways/utils/io_utils/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.984741 brainways-0.1.6/src/brainways/utils/io_utils/file_iterators/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      379 2022-09-08 08:38:22.000000 brainways-0.1.6/src/brainways/utils/io_utils/file_iterators/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      230 2022-07-07 09:39:04.000000 brainways-0.1.6/src/brainways/utils/io_utils/file_iterators/image_entry.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      407 2022-07-07 09:39:04.000000 brainways-0.1.6/src/brainways/utils/io_utils/file_iterators/path.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      914 2022-11-23 12:29:43.000000 brainways-0.1.6/src/brainways/utils/io_utils/file_iterators/qupath.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      630 2022-07-07 09:39:09.000000 brainways-0.1.6/src/brainways/utils/io_utils/image_path.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.984741 brainways-0.1.6/src/brainways/utils/io_utils/readers/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1041 2022-09-11 12:16:49.000000 brainways-0.1.6/src/brainways/utils/io_utils/readers/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.988741 brainways-0.1.6/src/brainways/utils/io_utils/readers/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      218 2022-09-22 07:42:16.000000 brainways-0.1.6/src/brainways/utils/io_utils/readers/_tests/test_qupath_reader.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1419 2022-09-08 08:38:21.000000 brainways-0.1.6/src/brainways/utils/io_utils/readers/aicsimageio_reader.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      649 2022-07-14 12:39:58.000000 brainways-0.1.6/src/brainways/utils/io_utils/readers/base.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1364 2022-09-08 08:38:21.000000 brainways-0.1.6/src/brainways/utils/io_utils/readers/czi_reader.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)    15748 2023-05-21 10:26:48.000000 brainways-0.1.6/src/brainways/utils/io_utils/readers/qupath_reader.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      108 2022-09-11 13:34:36.000000 brainways-0.1.6/src/brainways/utils/paths.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1181 2022-07-14 13:48:40.000000 brainways-0.1.6/src/brainways/utils/preprocess.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3183 2022-09-11 10:47:30.000000 brainways-0.1.6/src/brainways/utils/qupath.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1083 2022-07-14 13:48:39.000000 brainways-0.1.6/src/brainways/utils/test_utils.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-15 09:13:26.976741 brainways-0.1.6/src/brainways.egg-info/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2343 2023-06-15 09:13:26.000000 brainways-0.1.6/src/brainways.egg-info/PKG-INFO
+-rw-rw-r--   0 ben       (1001) ben       (1001)     5786 2023-06-15 09:13:26.000000 brainways-0.1.6/src/brainways.egg-info/SOURCES.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)        1 2023-06-15 09:13:26.000000 brainways-0.1.6/src/brainways.egg-info/dependency_links.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)       57 2023-06-15 09:13:26.000000 brainways-0.1.6/src/brainways.egg-info/entry_points.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)      413 2023-06-15 09:13:26.000000 brainways-0.1.6/src/brainways.egg-info/requires.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)       10 2023-06-15 09:13:26.000000 brainways-0.1.6/src/brainways.egg-info/top_level.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)      540 2022-07-13 13:47:58.000000 brainways-0.1.6/tox.ini
```

### Comparing `brainways-0.1.5/.gitignore` & `brainways-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/.pre-commit-config.yaml` & `brainways-0.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/.travis.yml` & `brainways-0.1.6/.travis.yml`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/CONTRIBUTING.rst` & `brainways-0.1.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/LICENSE` & `brainways-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/Makefile` & `brainways-0.1.6/Makefile`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/PKG-INFO` & `brainways-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainways
-Version: 0.1.5
+Version: 0.1.6
 Summary: Brainways
 Home-page: https://github.com/bkntr/brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/brainways#README.md
```

### Comparing `brainways-0.1.5/README.rst` & `brainways-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/data/test_data.npz` & `brainways-0.1.6/data/test_data.npz`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/data/test_image.jpg` & `brainways-0.1.6/data/test_image.jpg`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/docs/Makefile` & `brainways-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/docs/brainways.pipeline.rst` & `brainways-0.1.6/docs/brainways.pipeline.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/docs/brainways.project.rst` & `brainways-0.1.6/docs/brainways.project.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/docs/brainways.scripts.rst` & `brainways-0.1.6/docs/brainways.scripts.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/docs/brainways.transforms.rst` & `brainways-0.1.6/docs/brainways.transforms.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/docs/brainways.utils.atlas.rst` & `brainways-0.1.6/docs/brainways.utils.atlas.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/docs/brainways.utils.cell_detection_importer.rst` & `brainways-0.1.6/docs/brainways.utils.cell_detection_importer.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/docs/brainways.utils.io_utils.file_iterators.rst` & `brainways-0.1.6/docs/brainways.utils.io_utils.file_iterators.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/docs/brainways.utils.io_utils.readers.rst` & `brainways-0.1.6/docs/brainways.utils.io_utils.readers.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/docs/brainways.utils.io_utils.rst` & `brainways-0.1.6/docs/brainways.utils.io_utils.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/docs/brainways.utils.rst` & `brainways-0.1.6/docs/brainways.utils.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/docs/conf.py` & `brainways-0.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/docs/installation.rst` & `brainways-0.1.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/docs/make.bat` & `brainways-0.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/setup.cfg` & `brainways-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/conftest.py` & `brainways-0.1.6/src/brainways/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,22 +37,15 @@
 
 @fixture
 def mock_atlas(test_data: Tuple[np.ndarray, AtlasSlice]) -> BrainwaysAtlas:
     test_image, test_atlas_slice = test_data
     test_atlas_slice.annotation[test_atlas_slice.annotation > 0] = 10
     ATLAS_SIZE = 32
     ATLAS_DEPTH = 10
-    mock_atlas = create_autospec(BrainwaysAtlas)
-    mock_atlas.bounding_boxes = [(0, 0, ATLAS_SIZE, ATLAS_SIZE)] * ATLAS_DEPTH
-    mock_atlas.shape = (ATLAS_DEPTH, ATLAS_SIZE, ATLAS_SIZE)
-    mock_atlas.reference = torch.rand(ATLAS_DEPTH, ATLAS_SIZE, ATLAS_SIZE)
-    mock_atlas.brainglobe_atlas = Mock()
-    mock_atlas.brainglobe_atlas.structure_from_coords = Mock(return_value=10)
-    mock_atlas.brainglobe_atlas.resolution = (1, 2, 3)
-    mock_atlas.brainglobe_atlas.atlas_name = "MOCK_ATLAS"
+
     structures_list = [
         {
             "name": "root",
             "acronym": "root",
             "id": 1,
             "structure_id_path": [1],
             "rgb_triplet": [0, 0, 0],
@@ -72,15 +65,34 @@
             "id": 11,
             "structure_id_path": [1, 11],
             "rgb_triplet": [255, 255, 255],
             "mesh_filename": Path("/"),
         },
     ]
     structures = StructuresDict(structures_list=structures_list)
-    mock_atlas.brainglobe_atlas.structures = structures
+
+    mock_brainglobe_atlas = Mock()
+    mock_brainglobe_atlas.structure_from_coords = Mock(return_value=10)
+    mock_brainglobe_atlas.resolution = (1, 2, 3)
+    mock_brainglobe_atlas.atlas_name = "MOCK_ATLAS"
+    mock_brainglobe_atlas.reference = np.random.rand(
+        ATLAS_DEPTH, ATLAS_SIZE, ATLAS_SIZE
+    )
+    mock_brainglobe_atlas.annotation = np.random.rand(
+        ATLAS_DEPTH, ATLAS_SIZE, ATLAS_SIZE
+    )
+    mock_brainglobe_atlas.hemispheres = np.random.rand(
+        ATLAS_DEPTH, ATLAS_SIZE, ATLAS_SIZE
+    )
+    mock_brainglobe_atlas.shape = (ATLAS_DEPTH, ATLAS_SIZE, ATLAS_SIZE)
+    mock_brainglobe_atlas.structures = structures
+
+    mock_atlas = BrainwaysAtlas(
+        brainglobe_atlas=mock_brainglobe_atlas, exclude_regions=None
+    )
     mock_atlas.slice = Mock(return_value=test_atlas_slice)
     return mock_atlas
 
 
 @fixture(scope="session")
 def test_data() -> Tuple[np.ndarray, AtlasSlice]:
     npz = np.load(str(Path(__file__).parent.parent.parent / "data/test_data.npz"))
```

### Comparing `brainways-0.1.5/src/brainways/elastix/Par0033bspline.txt` & `brainways-0.1.6/src/brainways/elastix/Par0033bspline.txt`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/elastix/Par0033similarity.txt` & `brainways-0.1.6/src/brainways/elastix/Par0033similarity.txt`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/elastix/_tests/test_elastix.py` & `brainways-0.1.6/src/brainways/elastix/_tests/test_elastix.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/elastix/elastix.py` & `brainways-0.1.6/src/brainways/elastix/elastix.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/pipeline/_tests/test_brainways_pipeline.py` & `brainways-0.1.6/src/brainways/pipeline/_tests/test_brainways_pipeline.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/pipeline/affine_2d.py` & `brainways-0.1.6/src/brainways/pipeline/affine_2d.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/pipeline/atlas_registration.py` & `brainways-0.1.6/src/brainways/pipeline/atlas_registration.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/pipeline/brainways_params.py` & `brainways-0.1.6/src/brainways/pipeline/brainways_params.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/pipeline/brainways_pipeline.py` & `brainways-0.1.6/src/brainways/pipeline/brainways_pipeline.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/pipeline/cell_detector.py` & `brainways-0.1.6/src/brainways/pipeline/cell_detector.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/pipeline/tps.py` & `brainways-0.1.6/src/brainways/pipeline/tps.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/project/_tests/conftest.py` & `brainways-0.1.6/src/brainways/project/_tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,28 +25,28 @@
 
 
 @pytest.fixture
 def brainways_project_path_v0_1_1(mock_image_path: ImagePath, tmpdir) -> Path:
     project_path = (
         Path(os.path.realpath(__file__)).parent / "test_projects/v0.1.1/project.bwp"
     )
-    rewrite_image_path(project_path=project_path, image_path=mock_image_path)
     tmp_project_dir = Path(tmpdir / "v0.1.1")
     shutil.copytree(project_path.parent, tmp_project_dir)
+    rewrite_image_path(project_path=tmp_project_dir, image_path=mock_image_path)
     return tmp_project_dir / "project.bwp"
 
 
 @pytest.fixture
 def brainways_project_path_v0_1_4(mock_image_path: ImagePath, tmpdir) -> Path:
     project_path = (
         Path(os.path.realpath(__file__)).parent / "test_projects/v0.1.4/project.bwp"
     )
-    rewrite_image_path(project_path=project_path, image_path=mock_image_path)
     tmp_project_dir = Path(tmpdir / "v0.1.4")
     shutil.copytree(project_path.parent, tmp_project_dir)
+    rewrite_image_path(project_path=tmp_project_dir, image_path=mock_image_path)
     return tmp_project_dir / "project.bwp"
 
 
 def rewrite_image_path(project_path: Path, image_path: ImagePath):
     brainways_subject_paths = project_path.parent.rglob("brainways.bin")
     for brainways_subject_path in brainways_subject_paths:
         with open(brainways_subject_path, "rb") as f:
```

### Comparing `brainways-0.1.5/src/brainways/project/_tests/test_brainways_project.py` & `brainways-0.1.6/src/brainways/project/_tests/test_brainways_project.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/project/_tests/test_brainways_subject.py` & `brainways-0.1.6/src/brainways/project/_tests/test_brainways_subject.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/project/_tests/test_projects/v0.1.1/subject1/brainways.bin` & `brainways-0.1.6/src/brainways/project/_tests/test_projects/v0.1.1/subject1/brainways.bin`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/project/_tests/test_projects/v0.1.4/subject1/brainways.bin` & `brainways-0.1.6/src/brainways/project/_tests/test_projects/v0.1.4/subject1/brainways.bin`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/project/_tests/test_utils.py` & `brainways-0.1.6/src/brainways/project/_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/project/_utils.py` & `brainways-0.1.6/src/brainways/project/_utils.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/project/brainways_project.py` & `brainways-0.1.6/src/brainways/project/brainways_project.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/project/brainways_subject.py` & `brainways-0.1.6/src/brainways/project/brainways_subject.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/project/info_classes.py` & `brainways-0.1.6/src/brainways/project/info_classes.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/scripts/_tests/test_cli.py` & `brainways-0.1.6/src/brainways/scripts/_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/scripts/batch_create_thumbnails.py` & `brainways-0.1.6/src/brainways/scripts/batch_create_thumbnails.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/scripts/cell_detection.py` & `brainways-0.1.6/src/brainways/scripts/cell_detection.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/scripts/cli.py` & `brainways-0.1.6/src/brainways/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/scripts/create_excel.py` & `brainways-0.1.6/src/brainways/scripts/create_excel.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/scripts/create_excel_colabelling.py` & `brainways-0.1.6/src/brainways/scripts/create_excel_colabelling.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/scripts/create_reg_model_data.py` & `brainways-0.1.6/src/brainways/scripts/create_reg_model_data.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/scripts/display_area.py` & `brainways-0.1.6/src/brainways/scripts/display_area.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/scripts/import_cell_detections_keren.py` & `brainways-0.1.6/src/brainways/scripts/import_cell_detections_keren.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/scripts/import_cells.py` & `brainways-0.1.6/src/brainways/scripts/import_cells.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/scripts/move_images.py` & `brainways-0.1.6/src/brainways/scripts/move_images.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/transforms/_tests/test_affine_transform_2d.py` & `brainways-0.1.6/src/brainways/transforms/_tests/test_affine_transform_2d.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/transforms/_tests/test_depth_registration.py` & `brainways-0.1.6/src/brainways/transforms/_tests/test_depth_registration.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/transforms/_tests/test_image_to_atlas_transform.py` & `brainways-0.1.6/src/brainways/transforms/_tests/test_image_to_atlas_transform.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/transforms/_tests/test_tps_transform.py` & `brainways-0.1.6/src/brainways/transforms/_tests/test_tps_transform.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/transforms/affine_transform_2d.py` & `brainways-0.1.6/src/brainways/transforms/affine_transform_2d.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/transforms/compose.py` & `brainways-0.1.6/src/brainways/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/transforms/depth_registration.py` & `brainways-0.1.6/src/brainways/transforms/depth_registration.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/transforms/image_to_atlas_transform.py` & `brainways-0.1.6/src/brainways/transforms/image_to_atlas_transform.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/transforms/tps_transform.py` & `brainways-0.1.6/src/brainways/transforms/tps_transform.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/_imports.py` & `brainways-0.1.6/src/brainways/utils/_imports.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/_tests/test_cell_count_summary.py` & `brainways-0.1.6/src/brainways/utils/_tests/test_cell_count_summary.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/_tests/test_cells.py` & `brainways-0.1.6/src/brainways/utils/_tests/test_cells.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/_tests/test_image.py` & `brainways-0.1.6/src/brainways/utils/_tests/test_image.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/atlas/_tests/test_slice_atlas.py` & `brainways-0.1.6/src/brainways/utils/atlas/_tests/test_slice_atlas.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/atlas/brainways_atlas.py` & `brainways-0.1.6/src/brainways/utils/atlas/brainways_atlas.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,46 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from functools import cached_property
-from typing import List, Optional, Sequence, Union
+from typing import Optional, Sequence, Union
 
-import kornia
+import cv2
 import numpy as np
 import torch
 from bg_atlasapi import BrainGlobeAtlas
 
 from brainways.utils.atlas.slice_atlas import slice_atlas
-from brainways.utils.image import nonzero_bounding_box_tensor
-
-_BRAINWAYS_ATLAS_CACHE = {}
+from brainways.utils.image import nonzero_bounding_box
 
 
 class BrainwaysAtlas:
     def __init__(
         self,
-        brainglobe_atlas: BrainGlobeAtlas,
+        brainglobe_atlas: Union[str, BrainGlobeAtlas],
         exclude_regions: Optional[Sequence[int]],
     ):
-        self.brainglobe_atlas = brainglobe_atlas
+        if isinstance(brainglobe_atlas, str):
+            self.brainglobe_atlas = BrainGlobeAtlas(
+                brainglobe_atlas, check_latest=False
+            )
+        else:
+            self.brainglobe_atlas = brainglobe_atlas
+
         self.exclude_regions = exclude_regions
-        self.bounding_boxes: List[torch.Tensor] = self._calc_bounding_boxes()
 
     @classmethod
     def load(
         cls,
         brainglobe_atlas: Union[str, BrainGlobeAtlas],
-        exclude_regions: Optional[Sequence[int]] = None,
+        exclude_regions: Optional[Sequence[int]],
     ):
-        if isinstance(brainglobe_atlas, str):
-            brainglobe_atlas = BrainGlobeAtlas(brainglobe_atlas)
-
-        cache_key = (brainglobe_atlas.atlas_name, tuple(exclude_regions))
-
-        if cache_key not in _BRAINWAYS_ATLAS_CACHE:
-            _BRAINWAYS_ATLAS_CACHE.clear()
-            atlas = BrainwaysAtlas(
-                brainglobe_atlas=brainglobe_atlas, exclude_regions=exclude_regions
-            )
-            _BRAINWAYS_ATLAS_CACHE[cache_key] = atlas
-
-        return _BRAINWAYS_ATLAS_CACHE[cache_key]
+        return BrainwaysAtlas(
+            brainglobe_atlas=brainglobe_atlas, exclude_regions=exclude_regions
+        )
 
     def slice(
         self,
         ap: float,
         rot_horizontal: float = 0,
         rot_sagittal: float = 0,
         hemisphere: str = "both",
@@ -90,44 +83,40 @@
             reference *= hemispheres == hemisphere_idx
             annotation *= hemispheres == hemisphere_idx
 
         return AtlasSlice(
             reference=reference, annotation=annotation, hemispheres=hemispheres
         )
 
-    def _calc_bounding_boxes(self):
-        boxes = []
-        kernel = torch.ones(5, 5)
-        ann_open = kornia.morphology.opening(self.annotation[:, None], kernel)[:, 0]
-        for ann_open_slice in ann_open:
-            boxes.append(nonzero_bounding_box_tensor(ann_open_slice))
-        return boxes
+    def bounding_box(self, ap: int) -> tuple[int, int, int, int]:
+        kernel = np.ones((5, 5), np.uint8)
+        annotation_mask = (self.annotation[ap] > 0).byte().numpy()
+        ann_open = cv2.morphologyEx(annotation_mask, cv2.MORPH_OPEN, kernel)
+        return nonzero_bounding_box(ann_open)
 
     @property
     def shape(self):
         return self.brainglobe_atlas.shape
 
     @cached_property
     def reference(self):
-        ref = self.brainglobe_atlas.reference.astype(np.float32)
-        ref[self.annotation == 0] = 0
-        return torch.as_tensor(ref / ref.max(), dtype=torch.float32)
+        ref = torch.as_tensor(self.brainglobe_atlas.reference.astype(np.float32))
+        ref /= ref.max()
+        ref *= self.annotation != 0
+        return ref
 
     @cached_property
     def annotation(self):
-        ann = self.brainglobe_atlas.annotation.astype(np.float32)
-        exclude_mask = (ann[..., None] != self.exclude_regions).all(axis=-1)
-        ann = ann * exclude_mask
-        return torch.as_tensor(ann.astype(float), dtype=torch.float32)
+        ann = self.brainglobe_atlas.annotation
+        ann *= np.isin(ann, self.exclude_regions, invert=True)
+        return torch.as_tensor(ann.astype(np.float32))
 
     @cached_property
     def hemispheres(self):
-        return torch.as_tensor(
-            self.brainglobe_atlas.hemispheres.astype(np.float32), dtype=torch.float32
-        )
+        return torch.as_tensor(self.brainglobe_atlas.hemispheres.astype(np.float32))
 
 
 @dataclass
 class AtlasSlice:
     reference: torch.Tensor
     annotation: torch.Tensor
     hemispheres: torch.Tensor
```

### Comparing `brainways-0.1.5/src/brainways/utils/atlas/slice_atlas.py` & `brainways-0.1.6/src/brainways/utils/atlas/slice_atlas.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/cell_count_summary.py` & `brainways-0.1.6/src/brainways/utils/cell_count_summary.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/cell_detection_importer/_tests/qupath_sample_file.txt` & `brainways-0.1.6/src/brainways/utils/cell_detection_importer/_tests/qupath_sample_file.txt`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/cell_detection_importer/_tests/test_brainways_cell_detection_importer.py` & `brainways-0.1.6/src/brainways/utils/cell_detection_importer/_tests/test_brainways_cell_detection_importer.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/cell_detection_importer/_tests/test_qupath_cell_detection_importer.py` & `brainways-0.1.6/src/brainways/utils/cell_detection_importer/_tests/test_qupath_cell_detection_importer.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/cell_detection_importer/brainways_cell_detection_importer.py` & `brainways-0.1.6/src/brainways/utils/cell_detection_importer/brainways_cell_detection_importer.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/cell_detection_importer/keren_cell_detection_importer.py` & `brainways-0.1.6/src/brainways/utils/cell_detection_importer/keren_cell_detection_importer.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/cell_detection_importer/utils.py` & `brainways-0.1.6/src/brainways/utils/cell_detection_importer/utils.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/cells.py` & `brainways-0.1.6/src/brainways/utils/cells.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/config.py` & `brainways-0.1.6/src/brainways/utils/config.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/czi/czi_to_jpg.py` & `brainways-0.1.6/src/brainways/utils/czi/czi_to_jpg.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/dataclasses.py` & `brainways-0.1.6/src/brainways/utils/dataclasses.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/image.py` & `brainways-0.1.6/src/brainways/utils/image.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/io_utils/file_iterators/qupath.py` & `brainways-0.1.6/src/brainways/utils/io_utils/file_iterators/qupath.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/io_utils/image_path.py` & `brainways-0.1.6/src/brainways/utils/io_utils/image_path.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/io_utils/readers/__init__.py` & `brainways-0.1.6/src/brainways/utils/io_utils/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/io_utils/readers/aicsimageio_reader.py` & `brainways-0.1.6/src/brainways/utils/io_utils/readers/aicsimageio_reader.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/io_utils/readers/base.py` & `brainways-0.1.6/src/brainways/utils/io_utils/readers/base.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/io_utils/readers/czi_reader.py` & `brainways-0.1.6/src/brainways/utils/io_utils/readers/czi_reader.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/io_utils/readers/qupath_reader.py` & `brainways-0.1.6/src/brainways/utils/io_utils/readers/qupath_reader.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/preprocess.py` & `brainways-0.1.6/src/brainways/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/qupath.py` & `brainways-0.1.6/src/brainways/utils/qupath.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways/utils/test_utils.py` & `brainways-0.1.6/src/brainways/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.5/src/brainways.egg-info/PKG-INFO` & `brainways-0.1.6/src/brainways.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainways
-Version: 0.1.5
+Version: 0.1.6
 Summary: Brainways
 Home-page: https://github.com/bkntr/brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/brainways#README.md
```

### Comparing `brainways-0.1.5/src/brainways.egg-info/SOURCES.txt` & `brainways-0.1.6/src/brainways.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,15 @@
 src/brainways/utils/_tests/test_cell_count_summary.py
 src/brainways/utils/_tests/test_cells.py
 src/brainways/utils/_tests/test_image.py
 src/brainways/utils/atlas/__init__.py
 src/brainways/utils/atlas/brainways_atlas.py
 src/brainways/utils/atlas/slice_atlas.py
 src/brainways/utils/atlas/_tests/__init__.py
+src/brainways/utils/atlas/_tests/test_brainways_atlas.py
 src/brainways/utils/atlas/_tests/test_slice_atlas.py
 src/brainways/utils/cell_detection_importer/__init__.py
 src/brainways/utils/cell_detection_importer/brainways_cell_detection_importer.py
 src/brainways/utils/cell_detection_importer/cell_detection_importer.py
 src/brainways/utils/cell_detection_importer/keren_cell_detection_importer.py
 src/brainways/utils/cell_detection_importer/utils.py
 src/brainways/utils/cell_detection_importer/_tests/qupath_sample_file.txt
```

### Comparing `brainways-0.1.5/tox.ini` & `brainways-0.1.6/tox.ini`

 * *Files identical despite different names*

