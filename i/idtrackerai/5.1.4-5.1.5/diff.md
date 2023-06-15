# Comparing `tmp/idtrackerai-5.1.4.tar.gz` & `tmp/idtrackerai-5.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idtrackerai-5.1.4.tar", last modified: Mon May 29 18:55:03 2023, max compression
+gzip compressed data, was "idtrackerai-5.1.5.tar", last modified: Thu Jun 15 10:24:12 2023, max compression
```

## Comparing `idtrackerai-5.1.4.tar` & `idtrackerai-5.1.5.tar`

### file list

```diff
@@ -1,151 +1,135 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.786815 idtrackerai-5.1.4/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    35987 2023-02-10 16:03:19.000000 idtrackerai-5.1.4/LICENSE
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2828 2023-05-29 18:55:03.786815 idtrackerai-5.1.4/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1601 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/README.md
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3050 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/pyproject.toml
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-05-29 18:55:03.786815 idtrackerai-5.1.4/setup.cfg
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.762814 idtrackerai-5.1.4/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.762814 idtrackerai-5.1.4/src/idmatcherai/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idmatcherai/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     9102 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idmatcherai/main.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3643 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idmatcherai/matcher.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.762814 idtrackerai-5.1.4/src/idtrackerai/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      587 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/__init__.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.762814 idtrackerai-5.1.4/src/idtrackerai/animals_detection/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/animals_detection/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6157 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai/animals_detection/animals_detection.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    15527 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/animals_detection/segmentation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    31625 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/blob.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3215 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai/constants.toml
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.762814 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       96 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     7497 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/crossing_detector.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3115 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/crossings_detection.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.762814 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/dataset/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/dataset/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3947 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/dataset/crossings_dataloader.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     7161 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/dataset/crossings_dataset.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4938 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/model_area.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.762814 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/network/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/network/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      828 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/network/predictor_crossing_detector.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5107 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/network/stop_training_criteria_crossings.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3101 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/network/trainer_crossing_detector.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.770815 idtrackerai-5.1.4/src/idtrackerai/data/
--rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5933626 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/data/test_A.avi
--rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5976882 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/data/test_B.avi
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    26172 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/fragment.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.778815 idtrackerai-5.1.4/src/idtrackerai/fragmentation/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       78 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/fragmentation/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4529 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/fragmentation/fragmentation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8468 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/globalfragment.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.778815 idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    22092 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    20302 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3924 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5589 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/generate_groundtruth.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3989 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    15642 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/list_of_blobs.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    27145 2023-05-29 18:33:25.000000 idtrackerai-5.1.4/src/idtrackerai/list_of_fragments.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    12556 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/list_of_global_fragments.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.778815 idtrackerai-5.1.4/src/idtrackerai/network/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      459 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/network/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2556 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/network/evaluate.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3172 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/network/learners.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6563 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai/network/models.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2046 2023-05-29 18:41:52.000000 idtrackerai-5.1.4/src/idtrackerai/network/network_params.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2818 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/network/train.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2419 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/network/utils.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.778815 idtrackerai-5.1.4/src/idtrackerai/postprocess/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      292 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/postprocess/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    27711 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/postprocess/assign_them_all.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2725 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/postprocess/compute_velocity_model.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    21299 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3602 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/postprocess/erosion.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8671 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/postprocess/get_trajectories.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2592 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5168 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/postprocess/trajectories_creation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4209 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai/postprocess/trajectories_to_csv.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.778815 idtrackerai-5.1.4/src/idtrackerai/tracker/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    37146 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/accumulation_manager.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3151 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/accumulation_manager_utils.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8802 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/accumulator.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5742 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/assigner.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.778815 idtrackerai-5.1.4/src/idtrackerai/tracker/dataset/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/dataset/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3593 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/dataset/identification_dataloader.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6107 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/dataset/identification_dataset.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5561 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/identity_transfer.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.782815 idtrackerai-5.1.4/src/idtrackerai/tracker/network/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/network/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1536 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/network/get_predictions.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     7058 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/network/stop_training_criteria.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3175 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/network/trainer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6820 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/pre_trainer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    31972 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/tracker.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.782815 idtrackerai-5.1.4/src/idtrackerai/utils/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1180 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/utils/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2151 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/utils/check_PyPI_version.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1143 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/utils/confparams.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2954 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/utils/init_logger.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    13532 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/utils/py_utils.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    32730 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/video.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.762814 idtrackerai-5.1.4/src/idtrackerai.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2828 2023-05-29 18:55:03.000000 idtrackerai-5.1.4/src/idtrackerai.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5795 2023-05-29 18:55:03.000000 idtrackerai-5.1.4/src/idtrackerai.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-05-29 18:55:03.000000 idtrackerai-5.1.4/src/idtrackerai.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      341 2023-05-29 18:55:03.000000 idtrackerai-5.1.4/src/idtrackerai.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      351 2023-05-29 18:55:03.000000 idtrackerai-5.1.4/src/idtrackerai.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      108 2023-05-29 18:55:03.000000 idtrackerai-5.1.4/src/idtrackerai.egg-info/top_level.txt
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.782815 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6454 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/GUI_main_base.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      794 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2448 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    66516 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/logo_256.png
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    10027 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/themes.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      619 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/tooltips.toml
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.782815 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5484 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/canvas.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6069 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8204 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2870 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    13532 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/video_player.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.782815 idtrackerai-5.1.4/src/idtrackerai_start_app/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4959 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/__main__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1515 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/all_valid_parameters.dat
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6826 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/arg_parser.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5403 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/run_idtrackerai.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    16111 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_GUI.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.782815 idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8406 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      482 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5790 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5715 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3534 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2368 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6800 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5007 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2713 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/tooltips.toml
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.782815 idtrackerai-5.1.4/src/idtrackerai_validator/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai_validator/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      672 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_validator/__main__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      715 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai_validator/tooltips.toml
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    33550 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_validator/validation_GUI.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.786815 idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      547 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1904 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/additional_info.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8104 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/errors_explorer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6073 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/id_groups.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1505 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/id_labels.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    12933 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/interpolator.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4494 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/mark_properties.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6695 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/paint_blobs.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4835 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/setup_points.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.786815 idtrackerai-5.1.4/src/idtrackerai_video/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai_video/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5289 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_video/general_video.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4085 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_video/individual_videos.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2961 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_video/main.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.037140 idtrackerai-5.1.5/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    35987 2023-02-10 16:03:19.000000 idtrackerai-5.1.5/LICENSE
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2828 2023-06-15 10:24:12.037140 idtrackerai-5.1.5/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1601 2023-05-29 19:16:39.000000 idtrackerai-5.1.5/README.md
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3095 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/pyproject.toml
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-06-15 10:24:12.037140 idtrackerai-5.1.5/setup.cfg
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.013139 idtrackerai-5.1.5/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.013139 idtrackerai-5.1.5/src/idmatcherai/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idmatcherai/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     9102 2023-05-29 19:16:39.000000 idtrackerai-5.1.5/src/idmatcherai/main.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3614 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idmatcherai/matcher.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.013139 idtrackerai-5.1.5/src/idtrackerai/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      587 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/__init__.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.017139 idtrackerai-5.1.5/src/idtrackerai/animals_detection/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/animals_detection/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6157 2023-05-29 18:19:35.000000 idtrackerai-5.1.5/src/idtrackerai/animals_detection/animals_detection.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    14496 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/animals_detection/segmentation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    31620 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/blob.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3215 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai/constants.toml
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.017139 idtrackerai-5.1.5/src/idtrackerai/crossings_detection/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1658 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/crossings_detection/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5128 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/crossings_detection/crossing_detector.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     7941 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/crossings_detection/crossings_dataset.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5788 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/crossings_detection/crossings_network.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4938 2023-05-29 19:16:39.000000 idtrackerai-5.1.5/src/idtrackerai/crossings_detection/model_area.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.021139 idtrackerai-5.1.5/src/idtrackerai/data/
+-rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5933626 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/data/test_A.avi
+-rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5976882 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/data/test_B.avi
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    26290 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/fragment.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.029139 idtrackerai-5.1.5/src/idtrackerai/fragmentation/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       78 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/fragmentation/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4529 2023-06-12 11:03:30.000000 idtrackerai-5.1.5/src/idtrackerai/fragmentation/fragmentation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     7903 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/globalfragment.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.029139 idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    22015 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    20302 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3924 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5589 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/generate_groundtruth.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3989 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    15622 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/list_of_blobs.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    27122 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/list_of_fragments.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    10046 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/list_of_global_fragments.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.029139 idtrackerai-5.1.5/src/idtrackerai/network/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      489 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/network/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2541 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/network/evaluate.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3097 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/network/learners.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6563 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai/network/models.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2049 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/network/network_params.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2190 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/network/train.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3109 2023-06-15 10:19:56.000000 idtrackerai-5.1.5/src/idtrackerai/network/utils.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.029139 idtrackerai-5.1.5/src/idtrackerai/postprocess/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      292 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/postprocess/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    27711 2023-05-29 19:16:39.000000 idtrackerai-5.1.5/src/idtrackerai/postprocess/assign_them_all.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2731 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/postprocess/compute_velocity_model.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    21299 2023-05-29 19:16:39.000000 idtrackerai-5.1.5/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3602 2023-05-29 19:16:39.000000 idtrackerai-5.1.5/src/idtrackerai/postprocess/erosion.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8671 2023-05-29 19:16:39.000000 idtrackerai-5.1.5/src/idtrackerai/postprocess/get_trajectories.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2592 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5168 2023-05-29 19:16:39.000000 idtrackerai-5.1.5/src/idtrackerai/postprocess/trajectories_creation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4576 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/postprocess/trajectories_to_csv.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.033139 idtrackerai-5.1.5/src/idtrackerai/tracker/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/tracker/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    34690 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/tracker/accumulation_manager.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8555 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/tracker/accumulator.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5735 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/tracker/assigner.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6611 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/tracker/identity_dataset.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     7871 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/tracker/identity_network.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5548 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/tracker/identity_transfer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6595 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/tracker/pre_trainer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    26449 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/tracker/tracker.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.033139 idtrackerai-5.1.5/src/idtrackerai/utils/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1216 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/utils/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2170 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/utils/check_PyPI_version.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1143 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai/utils/confparams.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2890 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/utils/init_logger.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    13544 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/utils/py_utils.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    32674 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai/video.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.017139 idtrackerai-5.1.5/src/idtrackerai.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2828 2023-06-15 10:24:11.000000 idtrackerai-5.1.5/src/idtrackerai.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5052 2023-06-15 10:24:12.000000 idtrackerai-5.1.5/src/idtrackerai.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-06-15 10:24:12.000000 idtrackerai-5.1.5/src/idtrackerai.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      341 2023-06-15 10:24:12.000000 idtrackerai-5.1.5/src/idtrackerai.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      364 2023-06-15 10:24:12.000000 idtrackerai-5.1.5/src/idtrackerai.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      108 2023-06-15 10:24:12.000000 idtrackerai-5.1.5/src/idtrackerai.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.033139 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6443 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/GUI_main_base.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1016 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2448 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    66516 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/logo_256.png
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     9146 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/themes.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      619 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/tooltips.toml
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.033139 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5528 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/canvas.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6046 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8201 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2870 2023-05-29 18:19:35.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    13651 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/video_player.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.033139 idtrackerai-5.1.5/src/idtrackerai_start_app/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5657 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/__main__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1515 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/all_valid_parameters.dat
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6826 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/arg_parser.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5904 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/run_idtrackerai.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    16108 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_GUI.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.033139 idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8407 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      482 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5782 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5804 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3527 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2358 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6777 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4997 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2713 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai_start_app/tooltips.toml
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.037140 idtrackerai-5.1.5/src/idtrackerai_validator/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai_validator/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      671 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_validator/__main__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      715 2023-05-16 10:39:16.000000 idtrackerai-5.1.5/src/idtrackerai_validator/tooltips.toml
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    35131 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_validator/validation_GUI.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.037140 idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      547 2023-05-29 19:16:39.000000 idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1986 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/additional_info.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8093 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/errors_explorer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6047 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/id_groups.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1495 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/id_labels.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    12980 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/interpolator.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4484 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/mark_properties.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6771 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/paint_blobs.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4926 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/setup_points.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-15 10:24:12.037140 idtrackerai-5.1.5/src/idtrackerai_video/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:15:16.000000 idtrackerai-5.1.5/src/idtrackerai_video/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5157 2023-06-15 10:18:22.000000 idtrackerai-5.1.5/src/idtrackerai_video/general_video.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4085 2023-05-29 19:16:39.000000 idtrackerai-5.1.5/src/idtrackerai_video/individual_videos.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2961 2023-05-29 18:19:35.000000 idtrackerai-5.1.5/src/idtrackerai_video/main.py
```

### Comparing `idtrackerai-5.1.4/LICENSE` & `idtrackerai-5.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/PKG-INFO` & `idtrackerai-5.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idtrackerai
-Version: 5.1.4
+Version: 5.1.5
 Summary: Idtracker.ai tracks up to 100 unmarked animals from videos recorded in laboratory conditions using artificial intelligence. Free and open source.
 Author: Francisco Romero Ferrero, Mattia G. Bergomi, Francisco J.H. Heras, Ricardo Ribeiro
 Author-email: Jordi Torrents <jordi.torrentsm@gmail.com>
 Project-URL: Homepage, https://idtracker.ai/
 Project-URL: Repository, https://gitlab.com/polavieja_lab/idtrackerai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `idtrackerai-5.1.4/README.md` & `idtrackerai-5.1.5/README.md`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/pyproject.toml` & `idtrackerai-5.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "idtrackerai"
-version = "5.1.4"
+version = "5.1.5"
 authors = [
     { name = "Jordi Torrents", email = "jordi.torrentsm@gmail.com" },
     { name = "Francisco Romero Ferrero" },
     { name = "Mattia G. Bergomi" },
     { name = "Francisco J.H. Heras" },
     { name = "Ricardo Ribeiro" },
 ]
@@ -32,15 +32,16 @@
 ]
 dependencies = [
     "numpy >= 1.24.2",
     "rich >= 13.3.1",
     "h5py >= 3.8.0",
     "scipy >= 1.10.0",
     "opencv-python-headless >= 4.7.0",
-    "pyqt6 >= 6.4.2",
+    "pyqt5 >= 5.15.9",
+    "qtpy >= 2.3.1",
     'superqt >= 0.4.1',
     'toml >= 0.10.2',
     "matplotlib >= 3.7.0",
 ]
 
 [project.optional-dependencies]
 dev = [
@@ -97,16 +98,17 @@
 skip-magic-trailing-comma = true
 preview = true
 
 [tool.isort]
 profile = "black"
 
 [tool.pylint]
-extension-pkg-whitelist = 'PyQt6'
+extension-pkg-whitelist = 'qtpy'
 generated-members = 'cv2.*, torch.*'
+ignore_modules = 'qtpy'
 disable = [
     "missing-docstring",
     "fixme",
     "logging-fstring-interpolation",
     "wrong-import-order",
     "invalid-name",
 ]
```

### Comparing `idtrackerai-5.1.4/src/idmatcherai/main.py` & `idtrackerai-5.1.5/src/idmatcherai/main.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idmatcherai/matcher.py` & `idtrackerai-5.1.5/src/idmatcherai/matcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from typing import Iterable
 
 import h5py
 import numpy as np
 
 from idtrackerai.network import LearnerClassification, NetworkParams
-from idtrackerai.tracker.network.get_predictions import get_predictions_identities
+from idtrackerai.tracker.identity_network import get_predictions_identities
 
 
 def match(id_images_path: Path, model_path: Path):
     logging.info(
         "Matching images from %s with model from %s", id_images_path, model_path
     )
 
@@ -98,14 +98,13 @@
     identification_network_params = NetworkParams(
         schedule=params["schedule"],
         number_of_classes=params["number_of_classes"],
         architecture="idCNN",
         restore_folder=model_folder,
         model_name=params["model_name"],
         image_size=params["image_size"],
-        use_gpu=True,
     )
 
     identification_model = LearnerClassification.load_model(
         identification_network_params
     )
     return identification_model, identification_network_params
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/__init__.py` & `idtrackerai-5.1.5/src/idtrackerai/__init__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai/animals_detection/animals_detection.py` & `idtrackerai-5.1.5/src/idtrackerai/animals_detection/animals_detection.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai/animals_detection/segmentation.py` & `idtrackerai-5.1.5/src/idtrackerai/animals_detection/segmentation.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     blobs_in_episode = []
     for frame_number_in_video_path, global_frame_number in zip(
         range(episode.local_start, episode.local_end),
         range(episode.global_start, episode.global_end),
     ):
         ret, frame = cap.read()
         if ret:
-            blobs_in_frame = _get_blobs_in_frame(
+            blobs_in_frame = get_blobs_in_frame(
                 frame, segmentation_parameters, global_frame_number, bbox_images_path
             )
         else:
             logging.error(
                 "OpenCV could not read frame "
                 f"{frame_number_in_video_path} of {video_path}"
             )
@@ -108,62 +108,45 @@
         # store all the blobs encountered in the episode
         blobs_in_episode.append(blobs_in_frame)
 
     cap.release()
     return blobs_in_episode, episode
 
 
-def _get_blobs_in_frame(
+def get_blobs_in_frame(
     frame, segmentation_parameters, global_frame_number, bbox_images_path
 ) -> list[Blob]:
     """Segments a frame read from `cap` according to the preprocessing parameters
     in `video`. Returns a list `blobs_in_frame` with the Blob objects in the frame
     and the `max_number_of_blobs` found in the video so far. Frames are segmented
     in gray scale.
 
     Parameters
     ----------
-    cap : <VideoCapture object>
-        OpenCV object used to read the frames of the video
-    video : <Video object>
-        Object collecting all the parameters of the video and paths for saving and loading
     segmentation_thresholds : dict
         Dictionary with the thresholds used for the segmentation: `min_threshold`,
         `max_threshold`, `min_area`, `max_area`
-    max_number_of_blobs : int
-        Maximum number of blobs found in the whole video so far in the segmentation process
-    frame_number : int
-        Number of the frame being segmented. It is used to print in the terminal the frames
-        where the segmentation fails. This frame is the frame of the episode if the video
-        is chuncked.
     global_frame_number : int
         This is the frame number in the whole video. It will be different to the frame_number
         if the video is chuncked.
 
 
     Returns
     -------
     blobs_in_frame : list
         List of <Blob object> segmented in the current frame
-
-    See Also
-    --------
-    Video
-    Blob
-    segment_frame
-    blob_extractor
     """
-
     _, contours, frame = process_frame(frame, **segmentation_parameters)
 
-    bbox_images = [get_bbox_image(frame, cnt) for cnt in contours]
-
-    blobs_in_frame = create_blobs_objects(
-        bbox_images, contours, bbox_images_path, global_frame_number
-    )
+    blobs_in_frame: list[Blob] = []
+    with h5py.File(bbox_images_path, "a") as file:
+        for i, contour in enumerate(contours):
+            dataset_name = f"{global_frame_number}-{i}"
+            file.create_dataset(dataset_name, data=get_bbox_image(frame, contour))
+            blobs_in_frame.append(Blob(contour, global_frame_number, dataset_name))
 
     return blobs_in_frame
 
 
 def process_frame(
     frame,
     intensity_ths,
@@ -211,33 +194,14 @@
         area = cv2.contourArea(contour)
         if area_ths[0] <= area <= area_ths[1]:
             good_contours.append(np.squeeze(contour))
             areas.append(area)
     return areas, good_contours, frame
 
 
-def create_blobs_objects(
-    miniframes, contours, bbox_images_path, global_frame_number
-) -> list[Blob]:
-    with h5py.File(bbox_images_path, "a") as f1:
-        for i, miniframe in enumerate(miniframes):
-            f1.create_dataset(f"{global_frame_number}-{i}", data=miniframe)
-
-    blobs_in_frame = [
-        Blob(
-            contour=contour,
-            frame_number=global_frame_number,
-            bbox_img_id=f"{global_frame_number}-{i}",
-        )
-        for i, contour in enumerate(contours)
-    ]
-
-    return blobs_in_frame
-
-
 def segment(
     segmentation_parameters: dict,
     episodes: list[Episode],
     bbox_images_path: Path,
     video_paths: list[Path],
     number_of_frames: int,
 ) -> list[list[Blob]]:
@@ -271,15 +235,15 @@
 
     inputs = [
         (episode, video_paths, segmentation_parameters, bbox_images_path.parent)
         for episode in episodes
     ]
 
     blobs_in_video: list[list[Blob]] = [[]] * number_of_frames
-    with Pool(min(num_jobs, len(inputs))) as p:
+    with Pool(num_jobs) as p:
         for blobs_in_episode, episode in track(
             p.imap_unordered(segment_episode, inputs), "Segmenting video", len(inputs)
         ):
             blobs_in_video[episode.global_start : episode.global_end] = blobs_in_episode
 
     return blobs_in_video
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/blob.py` & `idtrackerai-5.1.5/src/idtrackerai/blob.py`

 * *Files 0% similar despite different names*

```diff
@@ -628,15 +628,15 @@
         #     flags=cv2.INTER_CUBIC,
         # )
 
         # # we build the offset like this to have the minimal ones on the
         # # beginning of the array and be preferably selected by max()
         # origins = [0]
         # for offset in range(img_size2 // 2):
-        #     origins.extend((diag - img_size2 + offset, diag - img_size2 - offset))
+        #     origins += (diag - img_size2 + offset, diag - img_size2 - offset)
 
         # origin = max(
         #     origins,
         #     key=lambda origin: np.count_nonzero(
         #         id_img[origin : origin + img_size, origin : origin + img_size]
         #     ),
         # )
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/constants.toml` & `idtrackerai-5.1.5/src/idtrackerai/constants.toml`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai/crossings_detection/model_area.py` & `idtrackerai-5.1.5/src/idtrackerai/crossings_detection/model_area.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai/crossings_detection/network/stop_training_criteria_crossings.py` & `idtrackerai-5.1.5/src/idtrackerai/crossings_detection/crossings_network.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,29 @@
-# This file is part of idtracker.ai a multiple animals tracking system
-# described in [1].
-# Copyright (C) 2017- Francisco Romero Ferrero, Mattia G. Bergomi,
-# Francisco J.H. Heras, Robert Hinz, Gonzalo G. de Polavieja and the
-# Champalimaud Foundation.
-#
-# idtracker.ai is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details. In addition, we require
-# derivatives or applications to acknowledge the authors by citing [1].
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
-#
-# For more information please send an email (idtrackerai@gmail.com) or
-# use the tools available at https://gitlab.com/polavieja_lab/idtrackerai.git.
-#
-# [1] Romero-Ferrero, F., Bergomi, M.G., Hinz, R.C., Heras, F.J.H.,
-# de Polavieja, G.G., Nature Methods, 2019.
-# idtracker.ai: tracking all individuals in small or large collectives of
-# unmarked animals.
-# (F.R.-F. and M.G.B. contributed equally to this work.
-# Correspondence should be addressed to G.G.d.P:
-# gonzalo.polavieja@neuro.fchampalimaud.org)
-
 import logging
 import sys
+from contextlib import suppress
+from pathlib import Path
 
 import numpy as np
+import torch
+from rich.console import Console
 from rich.status import Status
+from torch.utils.data import DataLoader
+
+from idtrackerai import Blob
+from idtrackerai.network import (
+    LearnerClassification,
+    NetworkParams,
+    evaluate,
+    get_device,
+    train,
+)
+from idtrackerai.utils import conf, track
 
-from idtrackerai.utils import conf
+from .crossings_dataset import get_test_data_loader
 
 
 class StopTraining:
     """CROSSING Stops the training of the network according to the conditions specified
     in __call__
     """
 
@@ -121,7 +105,66 @@
             # if the validation loss is 0.
             if previous_loss == 0.0 or current_loss == 0.0:
                 status.stop()
                 logging.info("The validation loss is 0.0, we stop the training")
                 return True
 
         return False
+
+
+def train_deep_crossing(
+    learner: LearnerClassification,
+    train_loader: DataLoader,
+    val_loader: DataLoader,
+    network_params: NetworkParams,
+    stop_training: StopTraining,
+) -> tuple[bool, Path]:
+    logging.info("Training Deep Crossing Detector")
+
+    # Initialize metric storage
+    train_loss = 0.0
+    val_losses = []
+    val_acc = 0.0
+
+    logging.debug("Entering the epochs loop...")
+    with Console().status("[red]Epochs loop...") as status:
+        while not stop_training(train_loss, val_losses, val_acc, status):
+            epoch = stop_training.epochs_completed
+
+            train_loss = train(epoch, train_loader, learner)
+            val_loss, val_acc = evaluate(val_loader, network_params, learner)
+
+            val_losses.append(val_loss)
+
+            with suppress(IndexError):
+                status.update(
+                    f"[red]Epoch {epoch}: training loss ="
+                    f" {train_loss:.6f}, validation loss ="
+                    f" {val_loss:.6f} and accuracy = {val_acc:.4%}"
+                )
+
+        logging.info("Last epoch loop: %s", status.status, extra={"markup": True})
+
+    learner.save_model(network_params.model_path)
+    return np.isnan(train_loss) or np.isnan(val_loss), network_params.model_path
+
+
+def get_predictions_crossigns(
+    id_images_file_paths: list[Path], model: torch.nn.Module, blobs: list[Blob]
+):
+    loader = get_test_data_loader(id_images_file_paths, blobs)
+    predictions = []
+
+    model.eval()
+    for input, _target in track(loader, "Predicting crossings"):
+        # Prepare the inputs
+
+        with torch.no_grad():
+            input = input.to(get_device())
+
+        # Inference
+        output = model(input)
+        pred = output.argmax(1)  # find the predicted class
+
+        predictions += pred.tolist()
+
+    return predictions
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/data/test_A.avi` & `idtrackerai-5.1.5/src/idtrackerai/data/test_A.avi`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai/data/test_B.avi` & `idtrackerai-5.1.5/src/idtrackerai/data/test_B.avi`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai/fragment.py` & `idtrackerai-5.1.5/src/idtrackerai/fragment.py`

 * *Files 1% similar despite different names*

```diff
@@ -635,15 +635,14 @@
         if accumulation_strategy == "global":
             self.accumulated_globally = True
         elif accumulation_strategy == "partial":
             self.accumulated_partially = True
 
     @property
     def properties(self) -> Sequence[str]:
-        max_p1 = np.argmax(self.P1_vector)
         return (
             f"Fragment {self.identifier}",
             (
                 f"Frames from {self.start_frame} to {self.end_frame} (length"
                 f" {self.end_frame-self.start_frame})"
             ),
             ("Individual" if self.is_an_individual else "Crossing")
@@ -659,11 +658,16 @@
             f"Fixed identity: {self.identity_is_fixed}",
             f"Globally accumulated: {self.accumulated_globally}",
             f"Partially accumulated: {self.accumulated_partially}",
             f"Accumulable: {self.accumulable}",
             f"Accumulated at step {self.accumulation_step}",
             f"Is certain: {self.is_certain}",
             "Non consistent" if self.non_consistent else "Consistent",
-            f"Max P1 {max_p1+1} with value {self.P1_vector[max_p1]}",
+            (
+                f"Max P1 {np.argmax(self.P1_vector)+1} with value"
+                f" {self.P1_vector.max()}"
+                if hasattr(self, "P1_vector")
+                else "Doesn't have P1 vector"
+            ),
             f"Certainty: {self.certainty}",
             f"P1 below random: {self.P1_below_random}",
         )
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/fragmentation/fragmentation.py` & `idtrackerai-5.1.5/src/idtrackerai/fragmentation/fragmentation.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai/globalfragment.py` & `idtrackerai-5.1.5/src/idtrackerai/globalfragment.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,28 +55,28 @@
 
     accumulation_step: int | None = None
     """Integer indicating the accumulation step at which the fragment was
     accumulated. See also the accumulation_manager.py module."""
 
     duplicated_identities: set
     first_frame_of_the_core: int
-    individual_fragments_identifiers: list[int]
+    individual_fragments_identifiers: tuple[int]
     individual_fragments: list[Fragment]
     minimum_distance_travelled: float
 
     def __init__(
         self,
         blobs_in_video: list[list[Blob]],
         fragments: list[Fragment],
         first_frame_of_the_core: int,
     ):
         self.first_frame_of_the_core = first_frame_of_the_core
-        self.individual_fragments_identifiers = [
+        self.individual_fragments_identifiers = tuple(
             blob.fragment_identifier for blob in blobs_in_video[first_frame_of_the_core]
-        ]
+        )
         self.set_individual_fragments(fragments)
 
         distance_travelled_per_individual_fragment: list[float] = []
 
         for fragment in self.individual_fragments:
             fragment.is_in_a_global_fragment = True
             distance_travelled_per_individual_fragment.append(
@@ -155,37 +155,17 @@
         """
         self.individual_fragments = [
             fragments[identifier]
             for identifier in self.individual_fragments_identifiers
         ]
 
     def acceptable_for_training(self, accumulation_strategy: str) -> bool:
-        """Returns True if the global fragment is acceptable for training.
-
+        """Returns True if the global fragment is acceptable for training"""
 
-        See :attr:`fragment.Fragment.acceptable_for_training` for every
-        individual fragment in the global fragment.
-
-        Parameters
-        ----------
-        accumulation_strategy : str
-            Can be either "global" or "partial"
-
-        Returns
-        -------
-        bool
-            True if the global fragment is acceptable for training the
-            identification neural network.
-        """
-        if accumulation_strategy == "global":
-            return all(
-                fragment.acceptable_for_training
-                for fragment in self.individual_fragments
-            )
-        return any(
+        return (all if accumulation_strategy == "global" else any)(
             fragment.acceptable_for_training for fragment in self.individual_fragments
         )
 
     @property
     def total_number_of_images(self) -> int:
         """Gets the total number of images in the global fragment"""
         return sum(fragment.number_of_images for fragment in self.individual_fragments)
@@ -214,11 +194,11 @@
         Tuple
             Tuple with two Numpy arrays with the images and their labels.
         """
         images = []
         labels = []
 
         for temporary_id, fragment in enumerate(self.individual_fragments):
-            images.extend(fragment.image_locations)
-            labels.extend([temporary_id] * fragment.number_of_images)
+            images += fragment.image_locations
+            labels += [temporary_id] * fragment.number_of_images
 
         return load_id_images(id_images_file_paths, images), np.asarray(labels)
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py` & `idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,17 +72,15 @@
             if isinstance(gt_identity, int) and gt_identity != 0:
                 results["number_of_blobs_per_identity"][gt_identity] += 1
             elif isinstance(gt_identity, list):
                 for identity in gt_identity:
                     if identity != 0:
                         results["number_of_blobs_per_identity"][identity] += 1
             elif gt_identity is None:
-                logging.debug(
-                    "***************************************unidentified blobs"
-                )
+                logging.debug("unidentified blobs")
 
             if (
                 blob_gt.is_an_individual
                 and not blob_gt.was_a_crossing
                 and gt_identity != blob.assigned_identities
             ):
                 results["number_of_individuals_badly_assigned"][gt_identity] += 1
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py` & `idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py` & `idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/generate_groundtruth.py` & `idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/generate_groundtruth.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py` & `idtrackerai-5.1.5/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai/list_of_blobs.py` & `idtrackerai-5.1.5/src/idtrackerai/list_of_blobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,15 @@
                 file,
                 episode,
                 self.blobs_in_video[episode.global_start : episode.global_end],
             )
             for file, episode in zip(id_images_file_paths, episodes)
         ]
 
-        with Pool(min(conf.number_of_parallel_workers, len(episodes))) as p:
+        with Pool(conf.number_of_parallel_workers) as p:
             for blobs_in_episode, episode in track(
                 p.imap_unordered(self.set_id_images_per_episode, inputs),
                 "Setting images for identification",
                 len(inputs),
             ):
                 self.blobs_in_video[episode.global_start : episode.global_end] = (
                     blobs_in_episode
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/list_of_fragments.py` & `idtrackerai-5.1.5/src/idtrackerai/list_of_fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         -------
         ndarray
             [number_of_images, height, width, number_of_channels]
         """
         images: list[tuple[int, int]] = []
         for fragment in self.individual_fragments:
             if not fragment.used_for_training:
-                images.extend(fragment.image_locations)
+                images += fragment.image_locations
 
         logging.info(
             f"Number of images to identify non-accumulated fragments: {len(images)}"
         )
         return load_id_images(self.id_images_file_paths, images)
 
     # TODO: The following methods could be properties.
@@ -287,16 +287,15 @@
                 fragments_to_the_past, key=lambda x: x.end_frame, reverse=True
             )
         elif scope == "to_the_future":
             fragments_to_the_future = filter(
                 lambda frag: frag.start_frame >= specific_frame, self.fragments
             )
             return sorted(fragments_to_the_future, key=lambda x: x.start_frame)
-        else:
-            raise ValueError(scope)
+        raise ValueError(scope)
 
     def save(self, path: Path | str):
         """Save an instance of the object in disk,
 
         Parameters
         ----------
         fragments_path : str
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/list_of_global_fragments.py` & `idtrackerai-5.1.5/src/idtrackerai/list_of_global_fragments.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 import json
 import logging
 import pickle
 from pathlib import Path
+from typing import Iterable
 
 import numpy as np
 
 from . import Blob, Fragment, GlobalFragment
 from .utils import conf, resolve_path
 
 
@@ -56,29 +57,35 @@
 
     non_accumulable_global_fragments: list[GlobalFragment]
     """List of global fragments which are NOT candidate for accumulation"""
 
     global_fragments: list[GlobalFragment]
     """List of global fragments which are candidate for accumulation"""
 
-    first_global_fragment_for_accumulation: GlobalFragment
-
-    def __init__(self, global_fragments: list[GlobalFragment]):
+    def __init__(self, global_fragments: Iterable[GlobalFragment]):
         self.global_fragments = []
         self.non_accumulable_global_fragments = []
 
         for global_fragment in global_fragments:
             if (
                 global_fragment.min_n_images_per_fragment
                 > conf.MINIMUM_NUMBER_OF_FRAMES_TO_BE_A_CANDIDATE_FOR_ACCUMULATION
             ):
                 self.global_fragments.append(global_fragment)
             else:
                 self.non_accumulable_global_fragments.append(global_fragment)
 
+        logging.info(
+            "Total number of global_fragments: %d",
+            len(self.non_accumulable_global_fragments) + len(self.global_fragments),
+        )
+        logging.info(
+            "Of which %d are long enough to be accumulated", len(self.global_fragments)
+        )
+
     @classmethod
     def from_fragments(
         cls,
         blobs_in_video: list[list[Blob]],
         fragments: list[Fragment],
         num_animals: int,
     ):
@@ -106,103 +113,46 @@
             for i, blobs_in_frame in enumerate(blobs_in_video)
         ]
 
         indices_beginning_of_fragment = detect_global_fragments_core_first_frame(
             global_fragments_boolean_array
         )
 
-        global_fragments = [
+        return cls(
             GlobalFragment(blobs_in_video, fragments, i)
             for i in indices_beginning_of_fragment
-        ]
-        logging.info(f"Total number of global_fragments: {len(global_fragments)}")
-        return cls(global_fragments)
+        )
 
     @property
-    def number_of_global_fragments(self) -> int:
-        return len(self.global_fragments)
+    def single_global_fragment(self) -> bool:
+        return len(self.global_fragments) == 1
 
     @property
-    def single_global_fragment(self) -> bool:
-        return self.number_of_global_fragments == 1
+    def no_global_fragment(self) -> bool:
+        return len(self.global_fragments) == 0
 
-    def order_by_distance_travelled(self):
-        """Sorts the global fragments by the minimum distance travelled.
-        See :attr:`global_fragment.GlobalFragment.minimum_distance_travelled`
-        """
+    def sort_by_distance_travelled(self):
         self.global_fragments.sort(
             key=lambda x: x.minimum_distance_travelled, reverse=True
         )
 
-    def set_first_global_fragment_for_accumulation(
-        self, accumulation_trial: int
-    ) -> GlobalFragment | None:
-        """Sets the first global fragment that will be used during the
-        accumulation in the cascade of training and identification protocols.
-
-        If the user asked to perform identity transfer, then the identities
-        of the first global fragment will be tried to be assigned using the
-        neural network provided by the knowledge_transfer_folder parameter.
-
-        Parameters
-        ----------
-        video : :class:`video.Video`
-            Video object containing information about the video and the
-            tracking process.
-        accumulation_trial : int, optional
-            Accumulation trials during the cascade of training and
-            identification protocols, by default 0.
-        identification_model : str, optional
-            Path to the directory where the identification neural network
-            model that should be used for identity transfer is stored,
-            by default None.
-        network_params : <NetworkParams object>, optional
-            Object with the parameters of the network and how to train it,
-             by default None.
-        knowledge_transfer_info_dict : dic, optional
-            Dictionary with information about the knowledge transfer,
-            by default None.
-
-        Returns
-        -------
-        int
-            A unique identifier of the global fragment that will be used as the
-            first global fragment for training.
-        """
-        logging.info("Setting #%d global fragment for accumulation", accumulation_trial)
-        self.order_by_distance_travelled()
-
-        try:
-            self.first_global_fragment_for_accumulation = self.global_fragments[
-                accumulation_trial
-            ]
-        except IndexError:  # TODO what happens with this exception
-            return None
-
-        return self.first_global_fragment_for_accumulation
-
-    def order_by_distance_to_the_first_global_fragment_for_accumulation(
-        self, first_frame_first_global_fragment: list, accumulation_trial: int
-    ):
+    def order_by_distance_to_the_frame(self, frame_number: int):
         """Sorts the global fragments with respect to their distance from the
         first global fragment chose for accumulation.
 
         Parameters
         ----------
         video : :class:`video.Video`
             Instance of the class :class:`video.Video`.
         accumulation_trial : int
             accumulation number (protocol 2 performs a single accumulation
             attempt, and if used, protocol 3 will perform 3 other attempts)
         """
         self.global_fragments.sort(
-            key=lambda x: abs(
-                x.first_frame_of_the_core
-                - first_frame_first_global_fragment[accumulation_trial]
-            )
+            key=lambda x: abs(x.first_frame_of_the_core - frame_number)
         )
 
     def save(self, path: Path | str):
         """Saves an instance of the class.
 
         Before saving the instances of fragments associated to every global
         fragment are removed and reset them after saving. This
@@ -253,20 +203,14 @@
         ]
 
         list_of_global_fragments.non_accumulable_global_fragments = [
             GlobalFragment.from_json(g_frag_data, fragments)
             for g_frag_data in json_data["non_accumulable_global_fragments"]
         ]
 
-        if "first_global_fragment_for_accumulation" in json_data:
-            list_of_global_fragments.first_global_fragment_for_accumulation = (
-                GlobalFragment.from_json(
-                    json_data["first_global_fragment_for_accumulation"], fragments
-                )
-            )
         return list_of_global_fragments
 
 
 def detect_global_fragments_core_first_frame(boolean_array: list[bool]) -> list[int]:
     """Detects the frame where the core of a global fragment starts.
 
     A core of a global fragment is the part of the global fragment where all
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/network/evaluate.py` & `idtrackerai-5.1.5/src/idtrackerai/network/evaluate.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 from statistics import fmean
 
 import torch
 from torch.utils.data import DataLoader
 
-from . import LearnerClassification, NetworkParams
+from . import LearnerClassification, NetworkParams, get_device
 from .utils import Confusion
 
 
 def evaluate(
     eval_loader: DataLoader,
     network_params: NetworkParams,
     learner: LearnerClassification,
@@ -47,18 +47,17 @@
         losses = []
         confusion = Confusion(network_params.number_of_classes)
 
     learner.eval()
 
     for input_, target in eval_loader:
         # Prepare the inputs
-        if network_params.use_gpu:
-            with torch.no_grad():
-                input_ = input_.cuda()
-                target = target.cuda()
+        with torch.no_grad():
+            input_ = input_.to(get_device())
+            target = target.to(get_device())
         train_target, eval_target = (target, target)
 
         with torch.no_grad():
             # Optimization
             loss, output = learner.forward_with_criterion(input_, train_target)
 
             losses += [loss] * input_.size(0)
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/network/learners.py` & `idtrackerai-5.1.5/src/idtrackerai/network/learners.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,20 +72,19 @@
 
     def forward_with_criterion(self, inputs, targets):
         out = self.forward(inputs)
         targets = targets.long()
         return self.criterion(out, targets), out
 
     def learn(self, inputs, targets):
-        with torch.autograd.set_detect_anomaly(True):
-            loss, out = self.forward_with_criterion(inputs, targets)
-            self.optimizer.zero_grad()
-            loss.backward()
-            self.optimizer.step()
-        return loss, out
+        loss, out = self.forward_with_criterion(inputs, targets)
+        self.optimizer.zero_grad()
+        loss.backward()
+        self.optimizer.step()
+        return loss
 
     def step_schedule(self, epoch):
         self.epoch = epoch
         self.scheduler.step()
 
     def save_model(self, savename: Path, **extra_data):
         logging.info("Saving model at %s", savename)
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/network/models.py` & `idtrackerai-5.1.5/src/idtrackerai/network/models.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai/network/network_params.py` & `idtrackerai-5.1.5/src/idtrackerai/network/network_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import json
 import logging
 from dataclasses import asdict, dataclass, field
 from pathlib import Path
-from typing import Optional
+from typing import Literal, Optional
 
 from idtrackerai.utils import create_dir, json_default
 
 
 @dataclass(slots=True)
 class NetworkParams:
     number_of_classes: int
     schedule: list[int]
     architecture: str
     model_name: str
     image_size: list[int]
     optim_args: dict = field(default_factory=dict)
     epochs: int = 0
-    optimizer: str = "SGD"
+    optimizer: Literal["Adam", "SGD"] = "SGD"
     loss: str = "CE"
-    use_gpu: bool = True
     save_folder: Path = Path("")
     scopes_layers_to_optimize: Optional[list[str]] = field(default_factory=list)
     knowledge_transfer_folder: Path | None = None
     use_adam_optimiser: bool = False
     return_store_objects: bool = False
     restore_folder: Path = Path()
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/network/utils.py` & `idtrackerai-5.1.5/src/idtrackerai/network/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,31 @@
+import logging
+from functools import cache
+
 import torch
+from torch.backends import mps
+
+
+@cache
+def get_device() -> torch.device:
+    """Returns the current available device for PyTorch"""
+    if torch.cuda.is_available():
+        logging.info('Using Cuda backend with "%s"', torch.cuda.get_device_name(0))
+        return torch.device(0)
+    if mps.is_available():
+        logging.info("Using MacOS Metal backend")
+        return torch.device("mps")
+    logging.warning(
+        (
+            "[bold red]No graphics device was found available[/], running neural"
+            " networks on CPU. This may slow down the training steps."
+        ),
+        extra={"markup": True},
+    )
+    return torch.device("cpu")
 
 
 def weights_xavier_init(m):
     if isinstance(m, (torch.nn.Linear, torch.nn.Conv2d)):
         torch.nn.init.xavier_uniform_(m.weight.data)
 
 
@@ -54,14 +77,14 @@
             _, pred = output.max(1)  # find the predicted class
         else:  # it is already the predicted class
             pred = output
         indices = (
             target * self.conf.stride(0) + pred.squeeze_().type_as(target)
         ).type_as(self.conf)
         ones = torch.ones(1).type_as(self.conf).expand(indices.size(0))
-        self._conf_flat = self.conf.view(-1)
-        self._conf_flat.index_add_(0, indices, ones)
+        conf_flat = self.conf.view(-1)
+        conf_flat.index_add_(0, indices, ones)
 
     def acc(self):
         TP = self.conf.diag().sum().item()
         total = self.conf.sum().item()
         return 0.0 if total == 0 else TP / total
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/postprocess/assign_them_all.py` & `idtrackerai-5.1.5/src/idtrackerai/postprocess/assign_them_all.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai/postprocess/compute_velocity_model.py` & `idtrackerai-5.1.5/src/idtrackerai/postprocess/compute_velocity_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,16 @@
     if percentile is None:
         percentile = conf.VEL_PERCENTILE
     distance_travelled_in_individual_fragments: list[float] = []
 
     for fragment in track(
         list_of_fragments.individual_fragments, "Computing velocity model"
     ):
-        distance_travelled_in_individual_fragments.extend(
-            fragment.frame_by_frame_velocity
+        distance_travelled_in_individual_fragments += (
+            fragment.frame_by_frame_velocity.tolist()
         )
     return (
         2 * np.max(distance_travelled_in_individual_fragments)
         if percentile is None
         else 2.0
         * float(np.percentile(distance_travelled_in_individual_fragments, percentile))
     )
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py` & `idtrackerai-5.1.5/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai/postprocess/erosion.py` & `idtrackerai-5.1.5/src/idtrackerai/postprocess/erosion.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai/postprocess/get_trajectories.py` & `idtrackerai-5.1.5/src/idtrackerai/postprocess/get_trajectories.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py` & `idtrackerai-5.1.5/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai/postprocess/trajectories_creation.py` & `idtrackerai-5.1.5/src/idtrackerai/postprocess/trajectories_creation.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai/postprocess/trajectories_to_csv.py` & `idtrackerai-5.1.5/src/idtrackerai/postprocess/trajectories_to_csv.py`

 * *Files 10% similar despite different names*

```diff
@@ -95,22 +95,32 @@
 @wrap_exceptions
 def main():
     logging.basicConfig(level=logging.DEBUG, format="%(message)s", datefmt="%H:%M:%S")
 
     parser = ArgumentParser()
 
     parser.add_argument(
-        "session", help="Session path to convert trajectories to CSV and JSON", type=str
+        "paths",
+        help=(
+            "Paths to convert trajectories to CSV and JSON. Can be session folders (to"
+            " convert all .npy files inside trajectory subfolder), arbitrary folder (to"
+            " convert all .npy files in it) and specific .npy files."
+        ),
+        type=Path,
+        nargs="+",
     )
 
     args = parser.parse_args()
-    path = Path(args.session)
 
-    if path.name.startswith("session_"):
-        path /= "trajectories"
+    for path in args.paths:
+        if path.is_file() and path.suffix == ".npy":
+            convert_trajectories_file_to_csv_and_json(path)
 
-    for file in path.glob("*.npy"):
-        convert_trajectories_file_to_csv_and_json(file)
+        if path.name.startswith("session_"):
+            path /= "trajectories"
+
+        for file in path.glob("*.npy"):
+            convert_trajectories_file_to_csv_and_json(file)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/tracker/accumulation_manager.py` & `idtrackerai-5.1.5/src/idtrackerai/tracker/accumulation_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,40 @@
-# This file is part of idtracker.ai a multiple animals tracking system
-# described in [1].
-# Copyright (C) 2017- Francisco Romero Ferrero, Mattia G. Bergomi,
-# Francisco J.H. Heras, Robert Hinz, Gonzalo G. de Polavieja and the
-# Champalimaud Foundation.
-#
-# idtracker.ai is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details. In addition, we require
-# derivatives or applications to acknowledge the authors by citing [1].
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
-#
-# For more information please send an email (idtrackerai@gmail.com) or
-# use the tools available at https://gitlab.com/polavieja_lab/idtrackerai.git.
-#
-# [1] Romero-Ferrero, F., Bergomi, M.G., Hinz, R.C., Heras, F.J.H.,
-# de Polavieja, G.G., Nature Methods, 2019.
-# idtracker.ai: tracking all individuals in small or large collectives of
-# unmarked animals.
-# (F.R.-F. and M.G.B. contributed equally to this work.
-# Correspondence should be addressed to G.G.d.P:
-# gonzalo.polavieja@neuro.fchampalimaud.org)
 import logging
 import random
 from pathlib import Path
+from typing import Literal
 
 import numpy as np
 from torch.nn import Module
 
 from idtrackerai import Fragment, GlobalFragment, ListOfFragments, ListOfGlobalFragments
+from idtrackerai.network import NetworkParams
 from idtrackerai.utils import conf, load_id_images
 
-from .accumulation_manager_utils import (
-    get_P1_array_and_argsort,
-    p1_below_random,
-    set_fragment_temporary_id,
-)
-from .network.get_predictions import get_predictions_identities
+from .identity_network import get_predictions_identities
 
 
 class AccumulationManager:
     """Manages the process of accumulating images for training the network.
 
     Attributes
     ----------
 
-    video : <Video object>
-        Object containing all the parameters of the video.
-    number_of_animals : int
-        Number of animals to be tracked
-    list_of_fragments : ListOfFragments
-        Collection of individual and crossing fragments with associated methods
     list_of_global_fragments: ListOfGlobalFragments
         Collection of global fragments
     counter : int
         Number of iterations for an instantiation
     certainty_threshold: float
         Value in [0,1] to establish if the identitification of a fragment
         is certain.
     threshold_acceptable_accumulation: float
         Value in [0,1] to establish if an accumulation is acceptable
     accumulation_strategy: string
         Accepts "global" and "partial" in order to perform either partial or
         global accumulation.
-    individual_fragments_used: list
-        list with the individual_fragments_identifiers of the individual
-        fragments used for training
     used_images : nd.array
         images used for training the network
     used_labels : nd.array
         labels for the images used for training
     new_images : nd.array
         set of images that will be added to the new training
     new_labels : nd.array
@@ -102,16 +60,20 @@
         self.id_images_file_paths = id_images_file_paths
         self.number_of_animals = number_of_animals
         self.list_of_fragments = list_of_fragments
         self.list_of_global_fragments = list_of_global_fragments
         self.current_step: int = 0
         self.certainty_threshold = certainty_threshold
         self.threshold_acceptable_accumulation = threshold_acceptable_accumulation
-        self.accumulation_strategy = "global"
-        self.individual_fragments_used: list[int] = []
+        self.accumulation_strategy: Literal["global", "partial"] = "global"
+        self.individual_fragments_used: set[int] = set()
+        """set with the individual_fragments_identifiers of the individual
+        fragments used for training"""
+        self.temporary_individual_fragments_used: set[int] = set()
+
         self.used_images = None
         self.used_labels = None
         self.new_images = None
         self.new_labels = None
         self.ratio_accumulated_images: float
         # When we init the Accumulation manager we are starting Protocol 1
         # or the accumulation parachute (
@@ -119,43 +81,44 @@
             conf.THRESHOLD_EARLY_STOP_ACCUMULATION
         )
 
     @property
     def new_global_fragments_for_training(self) -> bool:
         """We stop the accumulation when there are not more global fragments
         that are acceptable for training."""
-        if any(
+        there_are = any(
             (
                 global_fragment.acceptable_for_training(self.accumulation_strategy)
                 and not global_fragment.used_for_training
             )
             for global_fragment in self.list_of_global_fragments.global_fragments
-        ):
-            logging.info(
-                "[bold]There are global fragments acceptable for training",
-                extra={"markup": True},
-            )
-            return True
+        )
+
         logging.info(
-            "[bold]There are no more global fragments acceptable for training",
+            (
+                "[bold]There are global fragments acceptable for training"
+                if there_are
+                else "[bold]There are no more global fragments acceptable for training"
+            ),
             extra={"markup": True},
         )
-        return False
+
+        return there_are
 
     def get_new_images_and_labels(self):
         """Get the images and labels of the new global fragments that are going
         to be used for training. This function checks whether the images of a individual
         fragment have been added before"""
 
         images = []
         labels = []
         for fragment in self.list_of_fragments.individual_fragments:
             if fragment.acceptable_for_training and not fragment.used_for_training:
-                images.extend(fragment.image_locations)
-                labels.extend([fragment.temporary_id] * fragment.number_of_images)
+                images += fragment.image_locations
+                labels += [fragment.temporary_id] * fragment.number_of_images
 
         if images:
             self.new_images, self.new_labels = np.asarray(images), np.asarray(labels)
         else:
             self.new_images, self.new_labels = None, None
 
         n_used_images = len(self.used_images) if self.used_images is not None else 0
@@ -227,43 +190,37 @@
                     # the number of used images to reac the conf.MAXIMAL_IMAGES_PER_ANIMAL
                     number_samples_new = number_of_new_images
                     number_samples_used = (
                         conf.MAXIMAL_IMAGES_PER_ANIMAL - number_samples_new
                     )
                 # we put together a random sample of the new images and the used images
                 if self.new_images is not None:
-                    images.extend(
-                        random.sample(
-                            list(self.new_images[new_images_indices]),
-                            number_samples_new,
-                        )
+                    images += random.sample(
+                        list(self.new_images[new_images_indices]), number_samples_new
                     )
-                    labels.extend([i] * number_samples_new)
+                    labels += [i] * number_samples_new
                 if self.used_images is not None:
                     # this condition is set because the first time we accumulate
                     # the variable used_images is None
-                    images.extend(
-                        random.sample(
-                            list(self.used_images[used_images_indices]),
-                            number_samples_used,
-                        )
+                    images += random.sample(
+                        list(self.used_images[used_images_indices]), number_samples_used
                     )
-                    labels.extend([i] * number_samples_used)
+                    labels += [i] * number_samples_used
             else:
                 # if the total number of images for this label does not exceed
                 # the conf.MAXIMAL_IMAGES_PER_ANIMAL
                 # we take all the new images and all the used images
                 if self.new_images is not None:
-                    images.extend(list(self.new_images[new_images_indices]))
-                    labels.extend([i] * number_of_new_images)
+                    images += list(self.new_images[new_images_indices])
+                    labels += [i] * number_of_new_images
                 if self.used_images is not None:
                     # this condition is set because the first time we accumulate
                     # the variable used_images is None
-                    images.extend(list(self.used_images[used_images_indices]))
-                    labels.extend([i] * number_of_used_images)
+                    images += list(self.used_images[used_images_indices])
+                    labels += [i] * number_of_used_images
         return load_id_images(self.id_images_file_paths, images), np.asarray(labels)
 
     def update_used_images_and_labels(self):
         """Sets as used the images already used for training"""
         logging.info("Update images and labels used for training")
         if self.current_step == 0:
             self.used_images = self.new_images
@@ -299,42 +256,25 @@
         logging.info("Assigning identities to accumulated global fragments")
         for fragment in self.list_of_fragments.fragments:
             if fragment.used_for_training:
                 assert fragment.temporary_id is not None
                 fragment.identity = fragment.temporary_id + 1
                 fragment.set_P1_vector_accumulated()
 
-    def update_individual_fragments_used_for_training(self) -> list[int]:
-        """Returns the individual fragments used for training.
-
-        Returns
-        -------
-        individual_fragments_used_for_training : list
-            List of Fragment objects.
-
-        """
-        return list(
-            {
-                fragment.identifier
-                for fragment in self.list_of_fragments.fragments
-                if fragment.used_for_training
-                and fragment.identifier not in self.individual_fragments_used
-            }
-        )
-
-    def update_list_of_individual_fragments_used(self):
+    def update_set_of_individual_fragments_used(self):
         """Updates the list of individual fragments used for training and
         their identities.
         If an individual fragment was added before is not added again.
         """
         logging.info("Updating list of individual fragments used for training")
-        new_individual_fragments_identifiers = (
-            self.update_individual_fragments_used_for_training()
-        )
-        self.individual_fragments_used.extend(new_individual_fragments_identifiers)
+        self.individual_fragments_used = {
+            fragment.identifier
+            for fragment in self.list_of_fragments.fragments
+            if fragment.used_for_training
+        }
 
     def split_predictions_after_network_assignment(
         self,
         predictions,
         softmax_probs,
         indices_to_split,
         candidate_individual_fragments_identifiers: list[int],
@@ -363,15 +303,15 @@
                 self.list_of_fragments.number_of_animals,
             )
 
     def reset_accumulation_variables(self):
         """After an accumulation is finished reinitialise the variables involved
         in the process.
         """
-        self.temporary_individual_fragments_used: list[int] = []
+        self.temporary_individual_fragments_used.clear()
         if self.accumulation_strategy == "global":
             self.number_of_noncertain_global_fragments = 0
             self.number_of_random_assigned_global_fragments = 0
             self.number_of_nonconsistent_global_fragments = 0
             self.number_of_nonunique_global_fragments = 0
         self.number_of_sparse_fragments = 0
         self.number_of_noncertain_fragments = 0
@@ -426,15 +366,16 @@
         self.candidate_individual_fragments_identifiers = (
             candidate_individual_fragments_identifiers
         )
         self.reset_accumulation_variables()
         logging.debug("Accumulating by global strategy")
         for global_fragment in self.list_of_global_fragments.global_fragments:
             if not global_fragment.used_for_training:
-                self.check_if_is_acceptable_for_training(global_fragment)
+                self.check_if_is_globally_acceptable_for_training(global_fragment)
+
         self.number_of_acceptable_global_fragments = sum(
             global_fragment.acceptable_for_training(self.accumulation_strategy)
             and not global_fragment.used_for_training
             for global_fragment in self.list_of_global_fragments.global_fragments
         )
         if accumulation_trial == 0:
             min_number_of_imgs_accumulated_to_start_partial_accumulation = (
@@ -449,15 +390,15 @@
             and self.ratio_accumulated_images < self.threshold_early_stop_accumulation
         ):
             logging.debug("Accumulating by partial strategy")
             self.accumulation_strategy = "partial"
             self.reset_accumulation_variables()
             for global_fragment in self.list_of_global_fragments.global_fragments:
                 if not global_fragment.used_for_training:
-                    self.check_if_is_acceptable_for_training(global_fragment)
+                    self.check_if_is_partially_acceptable_for_training(global_fragment)
         elif (
             self.ratio_accumulated_images
             < min_number_of_imgs_accumulated_to_start_partial_accumulation
         ):
             logging.info(
                 "The ratio of accumulated images is too small and a partial"
                 " accumulation might fail."
@@ -485,277 +426,224 @@
         ----------
         global_fragment : GlobalFragment object
             Collection of images relative to a part of the video in which all the animals are visible.
         """
         for fragment in global_fragment.individual_fragments:
             self.reset_non_acceptable_fragment(fragment)
 
-    @staticmethod
-    def is_not_certain(fragment: Fragment, certainty_threshold):
-        """State if a fragment has been assigned with sufficient certainty
+    def check_if_is_globally_acceptable_for_training(
+        self, global_fragment: GlobalFragment
+    ):
+        assert self.accumulation_strategy == "global"
 
-        Parameters
-        ----------
-        fragment : Fragment object
-            Collection of images related to the same individual
-        certainty_threshold : float
-            Lower boundary in [0,1] for the certainty of a fragment
+        for fragment in global_fragment.individual_fragments:
+            fragment.acceptable_for_training = True
 
-        Returns
-        -------
-        is_not_certain_flag : bool
-            True if the fragment is assigned with high enough certainty
+        for fragment in global_fragment.individual_fragments:
+            if fragment.identifier in self.candidate_individual_fragments_identifiers:
+                if fragment.certainty < self.certainty_threshold:
+                    # if the certainty of the individual fragment is not high enough
+                    # we set the global fragment to be non-acceptable for training
+                    self.reset_non_acceptable_global_fragment(global_fragment)
+                    self.number_of_noncertain_global_fragments += 1
+                    fragment.is_certain = False
+                    break
+                # if the certainty of the individual fragment is high enough
+                fragment.is_certain = True
+            elif fragment.identifier in self.individual_fragments_used:
+                # if the individual fragment is not in the list of
+                # candidates is because it has been assigned
+                # and it is in the list of individual_fragments_used.
+                # We set the certainty to 1. And we
+                fragment.is_certain = True
+            else:
+                logging.warning(
+                    "Individual fragment not in candidates or in used, this should"
+                    " not happen"
+                )
+        # Compute identities if the global_fragment is certain
+        if not global_fragment.acceptable_for_training("global"):
+            return
 
-        """
-        return fragment.certainty < certainty_threshold
+        P1_array, index_individual_fragments_sorted_by_P1_max_to_min = (
+            get_P1_array_and_argsort(global_fragment)
+        )
+        # set to zero the P1 of the the identities of the individual
+        # fragments that have been already used
+        for index_individual_fragment, fragment in enumerate(
+            global_fragment.individual_fragments
+        ):
+            if (
+                fragment.identifier in self.individual_fragments_used
+                or fragment.identifier in self.temporary_individual_fragments_used
+            ):
+                P1_array[index_individual_fragment, :] = 0.0
+                P1_array[:, fragment.temporary_id] = 0.0
+        # assign temporal identity to individual fragments by hierarchical P1
+        for (
+            index_individual_fragment
+        ) in index_individual_fragments_sorted_by_P1_max_to_min:
+            fragment = global_fragment.individual_fragments[index_individual_fragment]
+            assert isinstance(fragment, Fragment)
+            if fragment.temporary_id is None:
+                if p1_below_random(P1_array, index_individual_fragment, fragment):
+                    fragment.P1_below_random = True
+                    self.number_of_random_assigned_global_fragments += 1
+                    self.reset_non_acceptable_global_fragment(global_fragment)
+                    break
+
+                temporary_id = np.argmax(P1_array[index_individual_fragment, :])
+                if not fragment.check_consistency_with_coexistent_individual_fragments(
+                    temporary_id
+                ):
+                    self.reset_non_acceptable_global_fragment(global_fragment)
+                    fragment.non_consistent = True
+                    self.number_of_nonconsistent_global_fragments += 1
+                    break
 
-    def check_if_is_acceptable_for_training(self, global_fragment: GlobalFragment):
-        """Check if global_fragment is acceptable for training
+                P1_array = set_fragment_temporary_id(
+                    fragment, int(temporary_id), P1_array, index_individual_fragment
+                )
 
-        Parameters
-        ----------
-        global_fragment : GlobalFragment
-            Object collecting the individual fragments relative to a part of the
-            video in which all the animals are visible
-        """
-        if self.accumulation_strategy == "global":
-            # Check certainties of the individual fragments in the global fragment
-            # for individual_fragment_identifier in
-            # global_fragment.individual_fragments_identifiers:
+        # Check if the global fragment is unique after assigning the identities
+        if global_fragment.acceptable_for_training("global"):
+            if not global_fragment.is_unique(self.number_of_animals):
+                # set acceptable_for_training to False and temporary_id to
+                # None for all the individual_fragments
+                # that had not been accumulated before (i.e. not in
+                # temporary_individual_fragments_used or individual_fragments_used)
+                self.reset_non_acceptable_global_fragment(global_fragment)
+                self.number_of_nonunique_global_fragments += 1
+            else:
+                global_fragment.accumulation_step = self.current_step
+                self.temporary_individual_fragments_used.update(
+                    fragment.identifier
+                    for fragment in global_fragment.individual_fragments
+                    if fragment.identifier not in self.individual_fragments_used
+                )
 
-            for fragment in global_fragment.individual_fragments:
-                fragment.acceptable_for_training = True
+    def check_if_is_partially_acceptable_for_training(
+        self, global_fragment: GlobalFragment
+    ):
+        assert self.accumulation_strategy == "partial"
+        for fragment in global_fragment.individual_fragments:
+            fragment.acceptable_for_training = False
 
-            for fragment in global_fragment.individual_fragments:
-                if (
-                    fragment.identifier
-                    in self.candidate_individual_fragments_identifiers
-                ):
-                    if self.is_not_certain(fragment, self.certainty_threshold):
+        for fragment in global_fragment.individual_fragments:
+            # Check certainties of the individual fragme
+            if fragment.identifier in self.candidate_individual_fragments_identifiers:
+                if fragment.has_enough_accumulated_coexisting_fragments:
+                    # Check if the more than half of the individual fragments
+                    # that coexist with this one have being accumulated
+                    if fragment.certainty < self.certainty_threshold:
                         # if the certainty of the individual fragment is not high enough
-                        # we set the global fragment to be non-acceptable for training
-                        self.reset_non_acceptable_global_fragment(global_fragment)
-                        self.number_of_noncertain_global_fragments += 1
+                        # we set the global fragment not to be acceptable for training
+                        self.reset_non_acceptable_fragment(fragment)
+                        self.number_of_noncertain_fragments += 1
                         fragment.is_certain = False
-                        break
-                    # if the certainty of the individual fragment is high enough
-                    fragment.is_certain = True
-                elif fragment.identifier in self.individual_fragments_used:
-                    # if the individual fragment is not in the list of
-                    # candidates is because it has been assigned
-                    # and it is in the list of individual_fragments_used.
-                    # We set the certainty to 1. And we
-                    fragment.is_certain = True
-                else:
-                    logging.warning(
-                        "Individual fragment not in candidates or in used, this should"
-                        " not happen"
-                    )
-            # Compute identities if the global_fragment is certain
-            if global_fragment.acceptable_for_training(self.accumulation_strategy):
-                P1_array, index_individual_fragments_sorted_by_P1_max_to_min = (
-                    get_P1_array_and_argsort(global_fragment)
-                )
-                # set to zero the P1 of the the identities of the individual
-                # fragments that have been already used
-                for index_individual_fragment, fragment in enumerate(
-                    global_fragment.individual_fragments
-                ):
-                    if (
-                        fragment.identifier in self.individual_fragments_used
-                        or fragment.identifier
-                        in self.temporary_individual_fragments_used
-                    ):
-                        P1_array[index_individual_fragment, :] = 0.0
-                        P1_array[:, fragment.temporary_id] = 0.0
-                # assign temporal identity to individual fragments by hierarchical P1
-                for (
-                    index_individual_fragment
-                ) in index_individual_fragments_sorted_by_P1_max_to_min:
-                    fragment = global_fragment.individual_fragments[
-                        index_individual_fragment
-                    ]
-                    assert isinstance(fragment, Fragment)
-                    if fragment.temporary_id is None:
-                        if p1_below_random(
-                            P1_array, index_individual_fragment, fragment
-                        ):
-                            fragment.P1_below_random = True
-                            self.number_of_random_assigned_global_fragments += 1
-                            self.reset_non_acceptable_global_fragment(global_fragment)
-                            break
-
-                        temporary_id = np.argmax(P1_array[index_individual_fragment, :])
-                        if not fragment.check_consistency_with_coexistent_individual_fragments(
-                            temporary_id
-                        ):
-                            self.reset_non_acceptable_global_fragment(global_fragment)
-                            fragment.non_consistent = True
-                            self.number_of_nonconsistent_global_fragments += 1
-                            break
-
-                        P1_array = set_fragment_temporary_id(
-                            fragment,
-                            int(temporary_id),
-                            P1_array,
-                            index_individual_fragment,
-                        )
-
-                # Check if the global fragment is unique after assigning the identities
-                if global_fragment.acceptable_for_training(self.accumulation_strategy):
-                    if not global_fragment.is_unique(self.number_of_animals):
-                        # set acceptable_for_training to False and temporary_id to
-                        # None for all the individual_fragments
-                        # that had not been accumulated before (i.e. not in
-                        # temporary_individual_fragments_used or individual_fragments_used)
-                        self.reset_non_acceptable_global_fragment(global_fragment)
-                        self.number_of_nonunique_global_fragments += 1
-                    else:
-                        global_fragment.accumulation_step = self.current_step
-                        self.temporary_individual_fragments_used.extend(
-                            fragment.identifier
-                            for fragment in global_fragment.individual_fragments
-                            if fragment.identifier
-                            not in self.temporary_individual_fragments_used
-                            and fragment.identifier
-                            not in self.individual_fragments_used
-                        )
-        elif self.accumulation_strategy == "partial":
-            for fragment in global_fragment.individual_fragments:
-                fragment.acceptable_for_training = False
-
-            for fragment in global_fragment.individual_fragments:
-                # Check certainties of the individual fragme
-                if (
-                    fragment.identifier
-                    in self.candidate_individual_fragments_identifiers
-                ):
-                    if fragment.has_enough_accumulated_coexisting_fragments:
-                        # Check if the more than half of the individual fragments
-                        # that coexist with this one have being accumulated
-                        if fragment.certainty < self.certainty_threshold:
-                            # if the certainty of the individual fragment is not high enough
-                            # we set the global fragment not to be acceptable for training
-                            self.reset_non_acceptable_fragment(fragment)
-                            self.number_of_noncertain_fragments += 1
-                            fragment.is_certain = False
-                        else:
-                            # if the certainty of the individual fragment is high enough
-                            fragment.is_certain = True
-                            fragment.acceptable_for_training = True
                     else:
-                        self.reset_non_acceptable_fragment(fragment)
-                        self.number_of_sparse_fragments += 1
-                elif fragment.identifier in self.individual_fragments_used:
-                    # if the individual fragment is not in the list of candidates
-                    # is because it has been assigned
-                    # and it is in the list of individual_fragments_used.
-                    # We set the certainty to 1. And we
-                    fragment.is_certain = True
+                        # if the certainty of the individual fragment is high enough
+                        fragment.is_certain = True
+                        fragment.acceptable_for_training = True
                 else:
-                    logging.warning(
-                        "Individual fragment not in candidates or in used, this should"
-                        " not happen"
-                    )
+                    self.reset_non_acceptable_fragment(fragment)
+                    self.number_of_sparse_fragments += 1
+            elif fragment.identifier in self.individual_fragments_used:
+                # if the individual fragment is not in the list of candidates
+                # is because it has been assigned
+                # and it is in the list of individual_fragments_used.
+                # We set the certainty to 1. And we
+                fragment.is_certain = True
+            else:
+                logging.warning(
+                    "Individual fragment not in candidates or in used, this should"
+                    " not happen"
+                )
 
-            # Compute identities if the global_fragment is certain
-            # get array of P1 values for the global fragment
-            P1_array = np.asarray(
-                [
-                    fragment.P1_vector
-                    for fragment in global_fragment.individual_fragments
-                ]
-            )
-            # get the maximum P1 of each individual fragment
-            P1_max = np.max(P1_array, axis=1)
-            # logging.debug("P1 max: %s" %str(P1_max))
-            # get the index position of the individual fragments ordered by
-            # P1_max from max to min
-            index_individual_fragments_sorted_by_P1_max_to_min = np.argsort(P1_max)[
-                ::-1
-            ]
-            # set to zero the P1 of the the identities of the individual
-            # fragments that have been already used
-            for index_individual_fragment, fragment in enumerate(
-                global_fragment.individual_fragments
+        # Compute identities if the global_fragment is certain
+        # get array of P1 values for the global fragment
+        P1_array = np.asarray(
+            [fragment.P1_vector for fragment in global_fragment.individual_fragments]
+        )
+        # get the maximum P1 of each individual fragment
+        P1_max = np.max(P1_array, axis=1)
+        # logging.debug("P1 max: %s" %str(P1_max))
+        # get the index position of the individual fragments ordered by
+        # P1_max from max to min
+        index_individual_fragments_sorted_by_P1_max_to_min = np.argsort(P1_max)[::-1]
+        # set to zero the P1 of the the identities of the individual
+        # fragments that have been already used
+        for index_individual_fragment, fragment in enumerate(
+            global_fragment.individual_fragments
+        ):
+            if (
+                fragment.identifier in self.individual_fragments_used
+                or fragment.identifier in self.temporary_individual_fragments_used
             ):
+                P1_array[index_individual_fragment, :] = 0.0
+                P1_array[:, fragment.temporary_id] = 0.0
+
+        # assign temporary identity to individual fragments by hierarchical P1
+        for (
+            index_individual_fragment
+        ) in index_individual_fragments_sorted_by_P1_max_to_min:
+            fragment = global_fragment.individual_fragments[index_individual_fragment]
+            assert isinstance(fragment, Fragment)  # for PyLance
+
+            if fragment.temporary_id is None and fragment.acceptable_for_training:
                 if (
-                    fragment.identifier in self.individual_fragments_used
-                    or fragment.identifier in self.temporary_individual_fragments_used
+                    np.max(P1_array[index_individual_fragment, :])
+                    < 1.0 / fragment.number_of_images
                 ):
-                    P1_array[index_individual_fragment, :] = 0.0
-                    P1_array[:, fragment.temporary_id] = 0.0
-
-            # assign temporary identity to individual fragments by hierarchical P1
-            for (
-                index_individual_fragment
-            ) in index_individual_fragments_sorted_by_P1_max_to_min:
-                fragment = global_fragment.individual_fragments[
-                    index_individual_fragment
-                ]
-                assert isinstance(fragment, Fragment)  # for PyLance
-
-                if fragment.temporary_id is None and fragment.acceptable_for_training:
-                    if (
-                        np.max(P1_array[index_individual_fragment, :])
-                        < 1.0 / fragment.number_of_images
+                    fragment.P1_below_random = True
+                    self.number_of_random_assigned_fragments += 1
+                    self.reset_non_acceptable_fragment(fragment)
+                else:
+                    temporary_id = np.argmax(P1_array[index_individual_fragment, :])
+                    if not fragment.check_consistency_with_coexistent_individual_fragments(
+                        temporary_id
                     ):
-                        fragment.P1_below_random = True
-                        self.number_of_random_assigned_fragments += 1
                         self.reset_non_acceptable_fragment(fragment)
+                        fragment.non_consistent = True
+                        self.number_of_nonconsistent_fragments += 1
                     else:
-                        temporary_id = np.argmax(P1_array[index_individual_fragment, :])
-                        if not fragment.check_consistency_with_coexistent_individual_fragments(
-                            temporary_id
-                        ):
-                            self.reset_non_acceptable_fragment(fragment)
-                            fragment.non_consistent = True
-                            self.number_of_nonconsistent_fragments += 1
-                        else:
-                            fragment.acceptable_for_training = True
-                            fragment.temporary_id = int(temporary_id)
-                            P1_array[index_individual_fragment, :] = 0.0
-                            P1_array[:, temporary_id] = 0.0
-
-            # Check if the global fragment is unique after assigning the identities
-            if not global_fragment.is_partially_unique:
-                number_of_duplicated_fragments = len(
-                    [
-                        self.reset_non_acceptable_fragment(fragment)
-                        for fragment in global_fragment.individual_fragments
-                        if fragment.temporary_id
-                        in global_fragment.duplicated_identities
-                    ]
-                )
-                self.number_of_nonunique_fragments += number_of_duplicated_fragments
+                        fragment.acceptable_for_training = True
+                        fragment.temporary_id = int(temporary_id)
+                        P1_array[index_individual_fragment, :] = 0.0
+                        P1_array[:, temporary_id] = 0.0
 
-            [
-                self.temporary_individual_fragments_used.append(fragment.identifier)
-                for fragment in global_fragment.individual_fragments
-                if fragment.identifier not in self.temporary_individual_fragments_used
-                and fragment.identifier not in self.individual_fragments_used
-                and fragment.acceptable_for_training
-            ]
-            self.number_of_acceptable_fragments += sum(
-                bool(fragment.acceptable_for_training)
-                and not fragment.used_for_training
-                for fragment in global_fragment.individual_fragments
-            )
-            global_fragment.accumulation_step = self.current_step
+        # Check if the global fragment is unique after assigning the identities
+        if not global_fragment.is_partially_unique:
+            for fragment in global_fragment.individual_fragments:
+                if fragment.temporary_id in global_fragment.duplicated_identities:
+                    self.reset_non_acceptable_fragment(fragment)
+                    self.number_of_nonunique_fragments += 1
+
+        self.temporary_individual_fragments_used.update(
+            fragment.identifier
+            for fragment in global_fragment.individual_fragments
+            if fragment.acceptable_for_training
+            and fragment.identifier not in self.individual_fragments_used
+        )
+        self.number_of_acceptable_fragments += sum(
+            bool(fragment.acceptable_for_training) and not fragment.used_for_training
+            for fragment in global_fragment.individual_fragments
+        )
+        global_fragment.accumulation_step = self.current_step
         assert all(
             fragment.temporary_id is not None
             for fragment in global_fragment.individual_fragments
             if fragment.acceptable_for_training and fragment.is_an_individual
         )
 
 
 def get_predictions_of_candidates_fragments(
     identification_model: Module,
     id_images_file_paths: list[Path],
-    network_params,
+    network_params: NetworkParams,
     list_of_fragments: ListOfFragments,
 ):
     """Get predictions of individual fragments that have been used to train the
     idCNN in an accumulation's iteration
 
     Parameters
     ----------
@@ -781,15 +669,15 @@
     """
     images = []
     lengths = []
     candidate_individual_fragments_identifiers: list[int] = []
 
     for fragment in list_of_fragments.individual_fragments:
         if not fragment.used_for_training:
-            images.extend(fragment.image_locations)
+            images += fragment.image_locations
             lengths.append(fragment.number_of_images)
             candidate_individual_fragments_identifiers.append(fragment.identifier)
 
     assert images
     images = load_id_images(id_images_file_paths, images)
 
     predictions, softmax_probs = get_predictions_identities(
@@ -799,7 +687,96 @@
     assert sum(lengths) == len(predictions)
     return (
         predictions,
         softmax_probs,
         np.cumsum(lengths)[:-1],
         candidate_individual_fragments_identifiers,
     )
+
+
+def get_P1_array_and_argsort(global_fragment: GlobalFragment):
+    """Given a global fragment computes P1 for each of its individual
+    fragments and returns a
+    matrix of sorted indices according to P1
+
+    Parameters
+    ----------
+    global_fragment : GlobalFragment object
+        Collection of images relative to a part of the video in which all
+        the animals are visible.
+
+    Returns
+    -------
+    P1_array : nd.array
+        P1 computed for every individual fragment in the global fragment
+    index_individual_fragments_sorted_by_P1_max_to_min : nd.array
+        Argsort of P1 array of each individual fragment
+    """
+    # get array of P1 values for the global fragment
+    P1_array = np.asarray(
+        [fragment.P1_vector for fragment in global_fragment.individual_fragments]
+    )
+    # get the maximum P1 of each individual fragment
+    P1_max = np.max(P1_array, axis=1)
+    # logging.debug("P1 max: %s" %str(P1_max))
+    # get the index position of the individual fragments ordered by P1_max
+    # from max to min
+    index_individual_fragments_sorted_by_P1_max_to_min = np.argsort(P1_max)[::-1]
+    return P1_array, index_individual_fragments_sorted_by_P1_max_to_min
+
+
+def p1_below_random(
+    P1_array: np.ndarray, index_individual_fragment: np.ndarray, fragment: Fragment
+):
+    """Evaluate if a fragment has been assigned with a certainty lower than
+    random (wrt the number of possible identities)
+
+    Parameters
+    ----------
+    P1_array  : nd.array
+        P1 vector of a fragment object
+    index_individual_fragment  : nd.array
+        Argsort of the P1 array of fragment
+    fragment : Fragment
+        Fragment object containing images associated with a single individual
+
+    Returns
+    -------
+    p1_below_random_flag : bool
+        True if a fragment has been identified with a certainty below random
+    """
+    return (
+        np.max(P1_array[index_individual_fragment, :]) < 1.0 / fragment.number_of_images
+    )
+
+
+def set_fragment_temporary_id(
+    fragment: Fragment,
+    temporary_id: int,
+    P1_array: np.ndarray,
+    index_individual_fragment: int,
+):
+    """Given a P1 array relative to a global fragment sets to 0 the row
+    relative to fragment
+    which is temporarily identified with identity temporary_id
+
+    Parameters
+    ----------
+    fragment : Fragment
+        Fragment object containing images associated with a single individual
+    temporary_id : int
+        temporary identifier associated to fragment
+    P1_array  : nd.array
+        P1 vector of fragment
+    index_individual_fragment : int
+        Index of fragment with respect to a global fragment in which it is
+        contained
+
+    Returns
+    -------
+    P1_array  : nd.array
+        updated P1 array
+    """
+    fragment.temporary_id = int(temporary_id)
+    P1_array[index_individual_fragment, :] = 0.0
+    P1_array[:, temporary_id] = 0.0
+    return P1_array
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/tracker/accumulator.py` & `idtrackerai-5.1.5/src/idtrackerai/tracker/accumulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,25 +33,23 @@
 
 import torch
 from torch.backends import cudnn
 from torch.nn import CrossEntropyLoss, Module
 from torch.optim.lr_scheduler import MultiStepLR
 
 from idtrackerai import Video
-from idtrackerai.network import LearnerClassification, NetworkParams
+from idtrackerai.network import LearnerClassification, NetworkParams, get_device
 from idtrackerai.utils import conf
 
 from .accumulation_manager import (
     AccumulationManager,
     get_predictions_of_candidates_fragments,
 )
-from .dataset.identification_dataloader import get_training_data_loaders
-from .dataset.identification_dataset import split_data_train_and_validation
-from .network.stop_training_criteria import StopTraining
-from .network.trainer import TrainIdentification
+from .identity_dataset import get_training_data_loaders, split_data_train_and_validation
+from .identity_network import StopTraining, TrainIdentification
 
 
 def perform_one_accumulation_step(
     accumulation_manager: AccumulationManager,
     video: Video,
     identification_model: Module,
     network_params: NetworkParams,
@@ -81,23 +79,18 @@
         video.number_of_animals, train_data, val_data
     )
 
     # Set criterion
     logging.info("Setting training criterion")
     criterion = CrossEntropyLoss(weight=torch.tensor(train_data["weights"]))
 
-    # Send model and criterion to GPU
-    if network_params.use_gpu:
-        torch.cuda.set_device(0)
-        logging.info(
-            'Sending model and criterion to GPU: "%s"', torch.cuda.get_device_name()
-        )
-        cudnn.benchmark = True  # make it train faster
-        identification_model = identification_model.cuda()
-        criterion = criterion.cuda()
+    logging.info("Sending model and criterion to GPU")
+    cudnn.benchmark = True  # make it train faster
+    identification_model = identification_model.to(get_device())
+    criterion = criterion.to(get_device())
 
     logging.info(f"Setting {network_params.optimizer} optimizer")
     if network_params.optimizer == "Adam":
         optimizer = torch.optim.Adam(
             identification_model.parameters(), **network_params.optim_args
         )
     elif network_params.optimizer == "SGD":
@@ -128,15 +121,15 @@
     TrainIdentification(
         learner, train_loader, val_loader, network_params, stop_training
     )
 
     accumulation_manager.update_fragments_used_for_training()
     accumulation_manager.update_used_images_and_labels()
     accumulation_manager.assign_identities_to_fragments_used_for_training()
-    accumulation_manager.update_list_of_individual_fragments_used()
+    accumulation_manager.update_set_of_individual_fragments_used()
 
     # compute ratio of accumulated images and stop if it is above random
     accumulation_manager.ratio_accumulated_images = (
         accumulation_manager.list_of_fragments.compute_ratio_of_images_used_for_training()
     )
 
     if (
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/tracker/assigner.py` & `idtrackerai-5.1.5/src/idtrackerai/tracker/assigner.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy as np
 from torch import load, nn
 
 from idtrackerai import Fragment, ListOfFragments
 from idtrackerai.network import NetworkParams
 from idtrackerai.utils import Timer
 
-from .network.get_predictions import get_predictions_identities
+from .identity_network import get_predictions_identities
 
 
 def compute_identification_statistics_for_non_accumulated_fragments(
     fragments: list[Fragment],
     all_predictions: np.ndarray,
     all_softmax_probs: np.ndarray,
     number_of_animals: int,
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/tracker/dataset/identification_dataset.py` & `idtrackerai-5.1.5/src/idtrackerai/tracker/identity_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,20 @@
-# This file is part of idtracker.ai a multiple animals tracking system
-# described in [1].
-# Copyright (C) 2017- Francisco Romero Ferrero, Mattia G. Bergomi,
-# Francisco J.H. Heras, Robert Hinz, Gonzalo G. de Polavieja and the
-# Champalimaud Foundation.
-#
-# idtracker.ai is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details. In addition, we require
-# derivatives or applications to acknowledge the authors by citing [1].
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
-#
-# For more information please send an email (idtrackerai@gmail.com) or
-# use the tools available at https://gitlab.com/polavieja_lab/idtrackerai.git.
-#
-# [1] Romero-Ferrero, F., Bergomi, M.G., Hinz, R.C., Heras, F.J.H.,
-# de Polavieja, G.G., Nature Methods, 2019.
-# idtracker.ai: tracking all individuals in small or large collectives of
-# unmarked animals.
-# (F.R.-F. and M.G.B. contributed equally to this work.
-# Correspondence should be addressed to G.G.d.P:
-# gonzalo.polavieja@neuro.fchampalimaud.org)
+import logging
+
 import numpy as np
+from torch.utils.data import DataLoader
+from torchvision import transforms
 from torchvision.datasets.folder import VisionDataset
 
+from idtrackerai.network import normalize
 from idtrackerai.utils import conf
 
+num_workers_train = 1
+num_workers_val = 1
+
 
 class IdentificationDataset(VisionDataset):
     def __init__(self, data_dict, scope, transform=None):
         super().__init__("", transform=transform)
         self.scope = scope
         self.images = data_dict["images"]
         if self.scope in ("training", "validation", "test"):
@@ -154,7 +132,61 @@
         Array of shape [2*number of images, 1] containing the labels corresponding
         to the original images and the images rotated
     """
     augmented_images = np.rot90(training_images, 2, axes=(1, 2))
     training_images = np.concatenate([training_images, augmented_images], axis=0)
     training_labels = np.concatenate([training_labels, training_labels], axis=0)
     return training_images, training_labels
+
+
+def get_training_data_loaders(
+    number_of_animals: int, train_data, val_data
+) -> tuple[DataLoader, DataLoader]:
+    logging.info("Creating training IdentificationDataset")
+    training_set = IdentificationDataset(
+        train_data,
+        scope="training",
+        transform=transforms.Compose([transforms.ToTensor(), normalize]),
+    )
+    train_loader = DataLoader(
+        training_set,
+        batch_size=conf.BATCH_SIZE_IDCNN,
+        shuffle=True,
+        num_workers=num_workers_train,
+        persistent_workers=num_workers_train > 0,
+    )
+    train_loader.num_classes = number_of_animals
+    train_loader.image_shape = training_set[0][0].shape
+
+    logging.info("Creating validation IdentificationDataset")
+    validation_set = IdentificationDataset(
+        val_data,
+        scope="validation",
+        transform=transforms.Compose([transforms.ToTensor(), normalize]),
+    )
+    val_loader = DataLoader(
+        validation_set,
+        batch_size=conf.BATCH_SIZE_PREDICTIONS_IDCNN,
+        num_workers=num_workers_val,
+        persistent_workers=num_workers_val > 0,
+    )
+    val_loader.num_classes = number_of_animals
+    val_loader.image_shape = validation_set[0][0].shape
+    return train_loader, val_loader
+
+
+def get_test_data_loader(test_data, number_of_classes):
+    logging.debug("Creating test IdentificationDataset")
+    test_set = IdentificationDataset(
+        test_data,
+        scope="predict",
+        transform=transforms.Compose([transforms.ToTensor(), normalize]),
+    )
+    test_loader = DataLoader(
+        test_set,
+        batch_size=conf.BATCH_SIZE_PREDICTIONS_IDCNN,
+        num_workers=num_workers_val,
+        persistent_workers=num_workers_val > 0,
+    )
+    test_loader.num_classes = number_of_classes
+    test_loader.image_shape = test_set[0][0].shape
+    return test_loader
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/tracker/identity_transfer.py` & `idtrackerai-5.1.5/src/idtrackerai/tracker/identity_transfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import numpy as np
 from torch.nn import Module
 
 from idtrackerai import GlobalFragment, Video
 from idtrackerai.network import NetworkParams, fc_weights_reinit
 from idtrackerai.utils import conf
 
-from .accumulation_manager_utils import (
+from .accumulation_manager import (
     get_P1_array_and_argsort,
     p1_below_random,
     set_fragment_temporary_id,
 )
 from .assigner import compute_identification_statistics_for_non_accumulated_fragments
-from .network.get_predictions import get_predictions_identities
+from .identity_network import get_predictions_identities
 
 
 def identify_first_global_fragment_for_accumulation(
     first_global_fragment_for_accumulation: GlobalFragment,
     video: Video,
     identification_model: Module | None,
     network_params: NetworkParams,
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/tracker/network/stop_training_criteria.py` & `idtrackerai-5.1.5/src/idtrackerai/tracker/identity_network.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,28 @@
-# This file is part of idtracker.ai a multiple animals tracking system
-# described in [1].
-# Copyright (C) 2017- Francisco Romero Ferrero, Mattia G. Bergomi,
-# Francisco J.H. Heras, Robert Hinz, Gonzalo G. de Polavieja and the
-# Champalimaud Foundation.
-#
-# idtracker.ai is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details. In addition, we require
-# derivatives or applications to acknowledge the authors by citing [1].
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
-#
-# For more information please send an email (idtrackerai@gmail.com) or
-# use the tools available at https://gitlab.com/polavieja_lab/idtrackerai.git.
-#
-# [1] Romero-Ferrero, F., Bergomi, M.G., Hinz, R.C., Heras, F.J.H.,
-# de Polavieja, G.G., Nature Methods, 2019.
-# idtracker.ai: tracking all individuals in small or large collectives of
-# unmarked animals.
-# (F.R.-F. and M.G.B. contributed equally to this work.
-# Correspondence should be addressed to G.G.d.P:
-# gonzalo.polavieja@neuro.fchampalimaud.org)
 import logging
 import sys
+from contextlib import suppress
 
 import numpy as np
+import torch
+from rich.console import Console
 from rich.status import Status
+from torch.backends import cudnn
+from torch.utils.data import DataLoader
 
-from idtrackerai.utils import conf
+from idtrackerai.network import (
+    LearnerClassification,
+    NetworkParams,
+    evaluate,
+    get_device,
+    train,
+)
+from idtrackerai.utils import CustomError, conf, track
+
+from .identity_dataset import get_test_data_loader
 
 
 class StopTraining:
     """Stops the training of the network according to the conditions specified
     in :meth:`__call__`
 
     Attributes
@@ -72,29 +56,15 @@
         self,
         loss_training: float,
         loss_validation: list,
         accuracy_validation: float,
         status: Status,
     ):
         """Returns True when one of the conditions to stop the training is
-        satisfied, otherwise it returns False
-
-        Parameters
-        ----------
-        loss_accuracy_training : list
-            List with the values of the loss in the training set for the
-            previous epochs
-        loss_accuracy_validation : list
-            List with the values of the loss in the validation set for the
-            previous epochs
-        epochs_completed : int
-            Number of epochs completed before checking the conditions
-
-        """
-        # check that the model did not diverged (nan loss).
+        satisfied, otherwise it returns False"""
         self.epochs_completed += 1
 
         if self.epochs_completed > 0 and (
             np.isnan(loss_training) or np.isnan(loss_validation[-1])
         ):
             status.stop()
             logging.error(
@@ -181,7 +151,79 @@
         # if the validation loss is 0.
         if previous_loss == 0.0 or current_loss == 0.0:
             status.stop()
             logging.info("The validation loss is 0.0, we stop the training")
             return True
 
         return False
+
+
+def TrainIdentification(
+    learner: LearnerClassification,
+    train_loader: DataLoader,
+    val_loader: DataLoader,
+    network_params: NetworkParams,
+    stop_training: StopTraining,
+):
+    logging.info("Training Identification Network")
+
+    # Initialize metric storage
+    train_loss = 0.0
+    val_losses = []
+    val_acc = 0.0
+
+    logging.debug("Entering the epochs loop...")
+    with Console().status("[red]Epochs loop...") as status:
+        while not stop_training(train_loss, val_losses, val_acc, status):
+            epoch = stop_training.epochs_completed
+
+            train_loss = train(epoch, train_loader, learner)
+            val_loss, val_acc = evaluate(val_loader, network_params, learner)
+
+            val_losses.append(val_loss)
+
+            with suppress(IndexError):
+                status.update(
+                    f"[red]Epoch {epoch}: training loss = {train_loss:.6f},"
+                    f" validation loss = {val_loss:.6f} and accuracy ="
+                    f" {val_acc:.4%}"
+                )
+
+        logging.info("Last epoch loop: %s", status.status, extra={"markup": True})
+
+    learner.save_model(network_params.model_path, val_acc=val_acc)
+
+    if np.isnan(train_loss) or np.isnan(val_loss):
+        raise CustomError("The model diverged")
+
+    logging.info("Identification network trained")
+
+
+def get_predictions_identities(
+    model: torch.nn.Module, images: np.ndarray, network_params: NetworkParams
+):
+    logging.debug("Generating prediction data set with %d images", len(images))
+    loader = get_test_data_loader({"images": images}, network_params.number_of_classes)
+    predictions = []
+    softmax_probs = []
+
+    logging.debug("Using trained network to predict images identities")
+    if not next(model.parameters()).is_cuda:
+        logging.info("Sending model and criterion to GPU")
+        cudnn.benchmark = True  # make it train faster
+        model = model.to(get_device())
+
+    model.eval()
+    for input_, _target in track(loader, "Predicting identities"):
+        # Prepare the inputs
+        with torch.no_grad():
+            input_ = input_.to(get_device())
+
+        # Inference
+        with torch.no_grad():
+            softmax = model.softmax_probs(input_)  # type: ignore
+            pred = softmax.argmax(1)  # find the predicted class
+
+            predictions += pred.tolist()
+            softmax_probs += softmax.tolist()
+
+    return np.asarray(predictions) + 1, np.asarray(softmax_probs)
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/tracker/pre_trainer.py` & `idtrackerai-5.1.5/src/idtrackerai/tracker/pre_trainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,21 +32,24 @@
 
 import torch
 from torch.backends import cudnn
 from torch.nn import CrossEntropyLoss, Module
 from torch.optim.lr_scheduler import MultiStepLR
 
 from idtrackerai import GlobalFragment, ListOfFragments
-from idtrackerai.network import LearnerClassification, NetworkParams, fc_weights_reinit
+from idtrackerai.network import (
+    LearnerClassification,
+    NetworkParams,
+    fc_weights_reinit,
+    get_device,
+)
 from idtrackerai.utils import conf
 
-from .dataset.identification_dataloader import get_training_data_loaders
-from .dataset.identification_dataset import split_data_train_and_validation
-from .network.stop_training_criteria import StopTraining
-from .network.trainer import TrainIdentification
+from .identity_dataset import get_training_data_loaders, split_data_train_and_validation
+from .identity_network import StopTraining, TrainIdentification
 
 
 def pre_train_global_fragment(
     number_of_animals: int,
     accumulation_step: int,
     identification_model: Module,
     network_params: NetworkParams,
@@ -113,23 +116,18 @@
     # Set criterion
     logging.info("Setting training criterion")
     criterion = CrossEntropyLoss(weight=torch.tensor(train_data["weights"]))
 
     # Re-initialize fully-connected layers
     identification_model.apply(fc_weights_reinit)
 
-    # Send model and criterion to GPU
-    if network_params.use_gpu:
-        torch.cuda.set_device(0)
-        logging.info(
-            'Sending model and criterion to GPU: "%s"', torch.cuda.get_device_name()
-        )
-        cudnn.benchmark = True  # make it train faster
-        identification_model = identification_model.cuda()
-        criterion = criterion.cuda()
+    logging.info("Sending model and criterion to GPU")
+    cudnn.benchmark = True  # make it train faster
+    identification_model = identification_model.to(get_device())
+    criterion = criterion.to(get_device())
 
     logging.info(f"Setting {network_params.optimizer} optimizer")
     if network_params.optimizer == "Adam":
         optimizer = torch.optim.Adam(
             identification_model.parameters(), **network_params.optim_args
         )
     elif network_params.optimizer == "SGD":
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/tracker/tracker.py` & `idtrackerai-5.1.5/src/idtrackerai/tracker/tracker.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from torch.backends import cudnn
 
 from idtrackerai import ListOfBlobs, ListOfFragments, ListOfGlobalFragments, Video
 from idtrackerai.network import (
     LearnerClassification,
     NetworkParams,
     fc_weights_reinit,
+    get_device,
     weights_xavier_init,
 )
 from idtrackerai.utils import CustomError, conf, create_dir, json_object_hook
 
 from .accumulation_manager import AccumulationManager
 from .accumulator import perform_one_accumulation_step
 from .assigner import assign_remaining_fragments
@@ -79,18 +80,18 @@
                 self.knowledge_transfer_info_dict: dict = np.load(
                     kt_info_dict_path.with_suffix(".npy"), allow_pickle=True
                 ).item()
         else:
             self.knowledge_transfer_info_dict = {}
 
         # Old requirements for restoring
-        self.processes_to_restore = {}
+        # self.processes_to_restore = {}
 
         self.accumulation_network_params: NetworkParams
-        self.restoring_first_accumulation = False  # Flag restores first accumulation
+        # self.restoring_first_accumulation = False  # Flag restores first accumulation
 
     def track_single_animal(self):
         logging.debug("Assigning identity 1 to all blobs")
         for blob in self.list_of_blobs.all_blobs:
             blob.identity = 1
 
     def track_single_global_fragment_video(self):
@@ -110,154 +111,37 @@
         self.video.first_frame_first_global_fragment = [0]  # in case
 
     def track_with_identities(self) -> ListOfFragments:
         """In protocol 3, list_of_fragments is loaded from accumulation
         folders so the reference from outside tracker_API is lost.
         That's why list_of_fragments has to be returned"""
         self.video.tracking_timer.start()
-        self._track_with_protocols_cascade()
+        self.track_with_protocols_cascade()
         self.video.tracking_timer.finish()
         return self.list_of_fragments
-        # track_with_cascade = True
-        # if track_with_cascade:
-        #     # This runs the protocol cascade and also the residual
-        #     # identification, the impossible_jumps, the creation of
-        #     # trajectories, the crossings interpolation, and the
-        #     # creation of trajectories_wo_gaps
-        #     # TODO: Factorize track_with_protocols_cascade so it only runs
-        #     # up to residual identification
-        #     self._track_with_protocols_cascade()
-        # else:
-        #     # TODO: Here is where new tracking methods should come
-        #     # Call to tracking method
-
-        #     # Call to postprocessing
-        #     # TODO: Factorize postprocess_impossible_jumps
-        #     # postprocess_impossible_jumps
-        #     # create_trajectories
-        #     # crossings_interpolation
-        #     # create_trajectories_wo_gaps
-        #     self.postprocess_impossible_jumps()
-        #     raise NotImplementedError("New tracking methods are not allwoed")
-
-    def _track_with_protocols_cascade(self):
-        logging.info("******* Start tracking with protocol cascade ********")
-        # Restoring
-
-        delete = not self.processes_to_restore.get("protocols1_and_2")
-        # Create accumulation folder
-        self.video.create_accumulation_folder(iteration_number=0, delete=delete)
-
-        self.init_accumulation_idCNN_params()
-
-        # Restoring
-        self.restoring_first_accumulation = False
-        if self.processes_to_restore.get("post_processing"):
-            raise NotImplementedError
-            # self.restore_trajectories()
-            # self.restore_crossings_solved()
-            # self.restore_trajectories_wo_gaps()
-
-        if self.processes_to_restore.get("residual_identification"):
-            raise NotImplementedError
-            # if self.video.track_wo_identities:
-            # TODO: bring restoring back to life
-            # raise
-            # self.restore_trajectories()
-
-            # else:
-            # TODO: bring restoring back to life
-            # raise
-            # logging.info("Restoring residual identification")
-            # self.restore_identification()
-            # self.create_trajectories()
-
-        if self.processes_to_restore.get("protocol3_accumulation"):
-            raise NotImplementedError
-            # logging.info("Restoring second accumulation")
-            # # self.restore_second_accumulation()
-            # self.video._first_frame_first_global_fragment = (
-            #     self.video._first_frame_first_global_fragment
-            # )
-            # logging.warning(
-            #     "first_frame_first_global_fragment "
-            #     + str(
-            #         self.video.first_frame_first_global_fragment
-            #     )
-            # )
-            # logging.info("Starting identification")
-            #
-            # self.create_trajectories()
-
-        if self.processes_to_restore.get("protocol3_pretraining"):
-            # TODO: bring restoring back to life
-            raise NotImplementedError
-            # logging.info("Restoring pretraining")
-            # logging.info("Initializing pretraining network")
-            # self.init_pretraining_net()
-            # logging.info("Restoring pretraining")
-            # self.accumulation_step_finished = True
-            # self.restore_first_accumulation()
-            # self.restore_pretraining()
-            # self.accumulation_manager.ratio_accumulated_images =
-            # self.video.percentage_of_accumulated_images[0]
-            # self.video._first_frame_first_global_fragment = [
-            #     self.video._first_frame_first_global_fragment[
-            #         0
-            #     ]
-            # ]
-            # self.video._percentage_of_accumulated_images = [
-            #     self.video.percentage_of_accumulated_images[0]
-            # ]
-            # logging.info("Start accumulation parachute")
-            #
-            # self.accumulate()
-
-        if self.processes_to_restore.get("protocols1_and_2"):
-            # TODO: bring restoring back to life
-            raise NotImplementedError
-            # logging.info("Restoring protocol 1 and 2")
-            # self.restoring_first_accumulation = True
-            # # self.restore_first_accumulation()
-            # self.accumulation_manager.ratio_accumulated_images =
-            # self.video.percentage_of_accumulated_images[0]
-            # self.video._first_frame_first_global_fragment = [
-            #     self.video._first_frame_first_global_fragment[
-            #         0
-            #     ]
-            # ]
-            # self.video._percentage_of_accumulated_images = [
-            #     self.video.percentage_of_accumulated_images[0]
-            # ]
-            # self.accumulation_step_finished = True
-            #
-            # self.accumulate()
-
-        if not self.processes_to_restore.get("protocols1_and_2"):
-            logging.info("Starting protocol cascade")
-            self.protocol1()
 
-    def init_accumulation_idCNN_params(self):
+    def track_with_protocols_cascade(self):
+        logging.info("Starting protocol cascade")
+        self.video.create_accumulation_folder(iteration_number=0, delete=True)
         self.accumulation_network_params = NetworkParams(
             number_of_classes=self.video.number_of_animals,
             architecture=conf.IDCNN_NETWORK_NAME,
             save_folder=self.video.accumulation_folder,
             knowledge_transfer_folder=self.video.knowledge_transfer_folder,
             model_name="identification_network",
             image_size=self.video.id_image_size,
             scopes_layers_to_optimize=conf.LAYERS_TO_OPTIMISE_PRETRAINING,
-            use_gpu=True,
             optimizer="SGD",
             schedule=[30, 60],
             optim_args={"lr": conf.LEARNING_RATE_IDCNN_ACCUMULATION, "momentum": 0.9},
             epochs=conf.MAXIMUM_NUMBER_OF_EPOCHS_IDCNN,
             return_store_objects=False,
         )
-        # Save network params
         self.accumulation_network_params.save()
+        self.protocol1()
 
     def protocol1(self):
         self.video.protocol1_timer.start()
 
         # reset list of fragments and global fragments to fragmentation
         self.list_of_fragments.reset(roll_back_to="fragmentation")
 
@@ -288,40 +172,35 @@
                 self.identification_model.apply(weights_xavier_init)
         else:
             self.identification_model = LearnerClassification.create_model(
                 self.accumulation_network_params
             )
             self.identification_model.apply(weights_xavier_init)
 
-        # Set first global fragment to start accumulation.
-        # The network is passed in case of identity transfer.
-        logging.info("Setting first global fragment for accumulation")
-        first_global_fragment = (
-            self.list_of_global_fragments.set_first_global_fragment_for_accumulation(
-                accumulation_trial=0
-            )
+        logging.info("Setting the first global fragment for accumulation")
+        first_global_fragment = max(
+            self.list_of_global_fragments.global_fragments,
+            key=lambda gf: gf.minimum_distance_travelled,
         )
 
         self.video.first_frame_first_global_fragment.append(
             first_global_fragment.first_frame_of_the_core
-            if first_global_fragment is not None
-            else None
         )
-        if first_global_fragment is not None:
-            identify_first_global_fragment_for_accumulation(
-                first_global_fragment,
-                self.video,
-                network_params=self.accumulation_network_params,
-                identification_model=self.identification_model,
-                knowledge_transfer_info_dict=self.knowledge_transfer_info_dict,
-            )
+
+        identify_first_global_fragment_for_accumulation(
+            first_global_fragment,
+            self.video,
+            network_params=self.accumulation_network_params,
+            identification_model=self.identification_model,
+            knowledge_transfer_info_dict=self.knowledge_transfer_info_dict,
+        )
 
         # Order global fragments by distance to the first global fragment for the accumulation
-        self.list_of_global_fragments.order_by_distance_to_the_first_global_fragment_for_accumulation(
-            self.video.first_frame_first_global_fragment, accumulation_trial=0
+        self.list_of_global_fragments.order_by_distance_to_the_frame(
+            first_global_fragment.first_frame_of_the_core
         )
 
         # Instantiate accumulation manager
         self.accumulation_manager = AccumulationManager(
             self.video.id_images_file_paths,
             self.video.number_of_animals,
             self.list_of_fragments,
@@ -384,18 +263,15 @@
                 assign_remaining_fragments(
                     self.list_of_fragments,
                     self.identification_model,
                     self.accumulation_network_params,
                     self.video.identify_timer,
                 )
 
-            elif (
-                self.accumulation_manager.ratio_accumulated_images
-                < conf.THRESHOLD_ACCEPTABLE_ACCUMULATION
-            ):
+            else:
                 self.video.protocol1_timer.finish()
                 self.video.protocol2_timer.finish(raise_if_not_started=False)
                 logging.warning(
                     "[red]Protocol 2 failed, protocol 3 is going to start",
                     extra={"markup": True},
                 )
                 ask_about_protocol3(
@@ -446,24 +322,24 @@
         if self.accumulation_manager.new_global_fragments_for_training:
             self.accumulate()
 
     def save_after_first_accumulation(self):
         """Set flags and save data"""
         logging.info("Saving first accumulation parameters")
 
-        if not self.restoring_first_accumulation:
-            self.video.ratio_accumulated_images = (
-                self.accumulation_manager.ratio_accumulated_images
-            )
-            self.video.percentage_of_accumulated_images = [
-                self.video.ratio_accumulated_images
-            ]
-            self.video.save()
-            self.list_of_fragments.save(self.video.fragments_path)
-            self.list_of_global_fragments.save(self.video.global_fragments_path)
+        # if not self.restoring_first_accumulation:
+        self.video.ratio_accumulated_images = (
+            self.accumulation_manager.ratio_accumulated_images
+        )
+        self.video.percentage_of_accumulated_images = [
+            self.video.ratio_accumulated_images
+        ]
+        self.video.save()
+        self.list_of_fragments.save(self.video.fragments_path)
+        self.list_of_global_fragments.save(self.video.global_fragments_path)
 
     """ pretraining """
 
     def protocol3(self):
         self.init_pretraining_variables()
 
         logging.info(
@@ -497,35 +373,33 @@
         else:
             self.identification_model = LearnerClassification.create_model(
                 self.pretrain_network_params
             )
             self.identification_model.apply(weights_xavier_init)
 
     def init_pretraining_net(self):
-        delete = not self.processes_to_restore.get("protocol3_pretraining")
-        create_dir(self.video.pretraining_folder, remove_existing=delete)
+        create_dir(self.video.pretraining_folder, remove_existing=True)
 
         self.pretrain_network_params = NetworkParams(
             number_of_classes=self.video.number_of_animals,
             architecture=conf.IDCNN_NETWORK_NAME,
             save_folder=self.video.pretraining_folder,
             model_name="identification_network",
             image_size=self.video.id_image_size,
             scopes_layers_to_optimize=conf.LAYERS_TO_OPTIMISE_PRETRAINING,
-            use_gpu=True,
             optimizer="SGD",
             schedule=[30, 60],
             optim_args={"lr": conf.LEARNING_RATE_IDCNN_ACCUMULATION, "momentum": 0.9},
             epochs=conf.MAXIMUM_NUMBER_OF_EPOCHS_IDCNN,
             return_store_objects=False,
         )
 
     def pretraining_loop(self):
         self.list_of_fragments.reset(roll_back_to="fragmentation")
-        self.list_of_global_fragments.order_by_distance_travelled()
+        self.list_of_global_fragments.sort_by_distance_travelled()
         self.one_shot_pretraining()
         self.continue_pretraining()
 
     def one_shot_pretraining(self):
         self.pretraining_step_finished = False
         self.pretraining_global_fragment = (
             self.list_of_global_fragments.global_fragments[self.pretraining_counter]
@@ -559,32 +433,38 @@
         elif self.ratio_of_pretrained_images > conf.MAX_RATIO_OF_PRETRAINED_IMAGES:
             logging.warning("Calling accumulate from continue_pretraining")
             self.video.protocol3_pretraining_timer.finish()
             self.accumulate()
 
     """ parachute """
 
-    def accumulation_parachute_init(self, iteration_number):
+    def accumulation_parachute_init(self, iteration_number: int):
         logging.debug("Accumulation_parachute_init")
         logging.info("Starting accumulation %i" % iteration_number)
 
-        delete = not self.processes_to_restore.get("protocol3_accumulation")
+        # delete = not self.processes_to_restore.get("protocol3_accumulation")
 
         self.video.create_accumulation_folder(
-            iteration_number=iteration_number, delete=delete
+            iteration_number=iteration_number, delete=True
         )
         self.video.accumulation_trial = iteration_number
         self.list_of_fragments.reset(roll_back_to="fragmentation")
 
-        first_global_fragment = (
-            self.list_of_global_fragments.set_first_global_fragment_for_accumulation(
-                accumulation_trial=iteration_number - 1
-            )
+        logging.info(
+            "Setting #%d global fragment for accumulation", iteration_number - 1
         )
 
+        self.list_of_global_fragments.sort_by_distance_travelled()
+        try:
+            first_global_fragment = self.list_of_global_fragments.global_fragments[
+                iteration_number - 1
+            ]
+        except IndexError:
+            first_global_fragment = None  # TODO what if this happens
+
         self.video.first_frame_first_global_fragment.append(
             first_global_fragment.first_frame_of_the_core
             if first_global_fragment is not None
             else None
         )
 
         if first_global_fragment is not None:
@@ -597,17 +477,16 @@
                     else None
                 ),
                 self.accumulation_network_params,
                 self.knowledge_transfer_info_dict,
             )
 
         # Sort global fragments by distance
-        self.list_of_global_fragments.order_by_distance_to_the_first_global_fragment_for_accumulation(
-            self.video.first_frame_first_global_fragment,
-            accumulation_trial=iteration_number - 1,
+        self.list_of_global_fragments.order_by_distance_to_the_frame(
+            self.video.first_frame_first_global_fragment[iteration_number - 1]
         )
         logging.warning(
             "first_frame_first_global_fragment "
             + str(self.video.first_frame_first_global_fragment)
         )
         logging.info(
             "We will restore the network from a previous pretraining: %s"
@@ -700,22 +579,17 @@
         self.identification_model = LearnerClassification.load_model(
             self.accumulation_network_params
         )
 
         # # Re-initialize fully-connected layers
         # self.identification_model.apply(fc_weights_reinit)
 
-        # Send model and criterion to GPU
-        if self.accumulation_network_params.use_gpu:
-            torch.cuda.set_device(0)
-            logging.info(
-                'Sending model and criterion to GPU: "%s"', torch.cuda.get_device_name()
-            )
-            cudnn.benchmark = True  # make it train faster
-            self.identification_model = self.identification_model.cuda()
+        logging.info("Sending model and criterion to GPU")
+        cudnn.benchmark = True  # make it train faster
+        self.identification_model = self.identification_model.to(get_device())
 
         self.video.save()
 
 
 def ask_about_protocol3(protocol3_action: str, n_error_frames: int) -> None:
     """Raises a CustomError if protocol3_action is abort or aks and user answers abortion"""
     logging.info("Protocol 3 action: %s", protocol3_action)
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/utils/__init__.py` & `idtrackerai-5.1.5/src/idtrackerai/utils/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .check_PyPI_version import (
     check_version,
     check_version_on_console,
     check_version_on_console_thread,
 )
 from .confparams import conf
-from .init_logger import CustomError, initLogger, wrap_exceptions
+from .init_logger import LOG_FILE_PATH, CustomError, initLogger, wrap_exceptions
 from .py_utils import (
     Episode,
     Timer,
     assert_all_files_exist,
     build_ROI_mask_from_list,
     check_if_identity_transfer_is_possible,
     clean_attrs,
@@ -22,14 +22,15 @@
     remove_dir,
     remove_file,
     resolve_path,
     track,
 )
 
 __all__ = [
+    "LOG_FILE_PATH",
     "clean_attrs",
     "wrap_exceptions",
     "check_version",
     "check_version_on_console",
     "initLogger",
     "conf",
     "CustomError",
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/utils/check_PyPI_version.py` & `idtrackerai-5.1.5/src/idtrackerai/utils/check_PyPI_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 import re
+from importlib import metadata
 from threading import Thread
 from urllib.request import urlopen
 
-import idtrackerai
-
 
 def check_version_on_console_thread():
     Thread(target=check_version_on_console).start()
 
 
 def available_is_greater(available: str, current: str):
     for available_part, current_part in zip(available.split("."), current.split(".")):
@@ -45,15 +44,15 @@
     no_yanked_versions = "\n".join(
         (line for line in out_text.splitlines() if "yanked" not in line)
     )
     versions: list[tuple[str, str]] = re.findall(
         ">idtrackerai-(.+?)(.tar.gz|-py3-none-any.whl)<", no_yanked_versions
     )
 
-    current_version = idtrackerai.__version__
+    current_version = metadata.version("idtrackerai")
     for version, _file_extension in versions:
         if not version.replace(".", "").isdigit():
             continue  # not a stable version
 
         if available_is_greater(version, current_version):
             return (
                 True,
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/utils/confparams.py` & `idtrackerai-5.1.5/src/idtrackerai/utils/confparams.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai/utils/init_logger.py` & `idtrackerai-5.1.5/src/idtrackerai/utils/init_logger.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,85 +7,85 @@
 from platform import platform
 
 from rich.console import Console
 from rich.logging import RichHandler
 
 from .check_PyPI_version import check_version_on_console_thread
 
+LOG_FILE_PATH = Path("idtrackerai.log").resolve()
+
 
 class CustomError(Exception):
     pass
 
 
 def initLogger(testing=False, check_version=True, level: int = logging.DEBUG):
-    logger_width_when_no_terminal = 150
+    logger_width_when_no_terminal = 130
     try:
         os.get_terminal_size()
     except OSError:
         # stdout is sent to file. We define logger width to a constant
         size = logger_width_when_no_terminal
     else:
         # stdout is sent to terminal
         # We define logger width to adapt to the terminal width
         size = None
 
-    if os.path.exists("idtrackerai.log"):
-        os.remove("idtrackerai.log")  # avoid conflicts and merged files
+    LOG_FILE_PATH.unlink(True)  # avoid conflicts and merged files
 
     # The first handler is the terminal, the second one the .log file,
     # both rendered with Rich and full logging (level=0)
     logging.basicConfig(
         level=level,
         format="%(message)s",
         datefmt="%H:%M:%S",
         force=not testing,
         handlers=[
             RichHandler(console=Console(width=size)),
             RichHandler(
                 console=Console(
-                    file=open("idtrackerai.log", "w", encoding="utf_8"),  # noqa SIM115
+                    file=LOG_FILE_PATH.open("w", encoding="utf_8"),  # noqa SIM115
                     width=logger_width_when_no_terminal,
                 )
             ),
         ],
     )
 
-    logging.getLogger("PyQt6").setLevel(logging.INFO)
     logging.info("Welcome to idtracker.ai")
     logging.debug(
         f"Running idtracker.ai '{metadata.version('idtrackerai')}'"
         f" on Python '{sys.version.split(' ')[0]}'\nPlatform: '{platform(True)}'"
         "\nDate: "
         + str(datetime.now()).split(".")[0]
     )
+    logging.info("Writing log in %s", LOG_FILE_PATH)
 
     if check_version:
         check_version_on_console_thread()
 
 
 def wrap_exceptions(main_function):
     def applicator(*args, **kwargs):
         try:
             return main_function(*args, **kwargs)
         except CustomError as error:
             logging.critical(error, exc_info=False)
             return False
         except Exception as error:
             logging.critical(error, exc_info=True)
-            log_file_path = Path("idtrackerai.log").resolve()
             logging.warning(
                 (
                     "\n\nIf this error persists please let us know by "
-                    "following any of the following options\n"
+                    "following any of the following options:\n"
                     "  - posting on "
                     "https://groups.google.com/g/idtrackerai_users\n"
                     "  - opening an issue at "
                     "https://gitlab.com/polavieja_lab/idtrackerai\n"
                     "  - sending an email to idtrackerai@gmail.com\n"
                     "Share the log file (%s) when "
                     "doing any of the options above"
                 ),
-                log_file_path,
+                LOG_FILE_PATH,
             )
             return False
 
     return applicator
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/utils/py_utils.py` & `idtrackerai-5.1.5/src/idtrackerai/utils/py_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         elif line[0] == "-":
             cv2.fillPoly(ROI_mask, (vertices,), color=0)
         else:
             raise TypeError
     return ROI_mask.astype(bool)
 
 
-@dataclass
+@dataclass(slots=True)
 class Episode:
     index: int
     local_start: int
     local_end: int
     video_path_index: int
     global_start: int
     global_end: int
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai/video.py` & `idtrackerai-5.1.5/src/idtrackerai/video.py`

 * *Files 0% similar despite different names*

```diff
@@ -864,15 +864,13 @@
         ):
             if not path.is_file():
                 continue
             with (
                 h5py.File(path, "r") as original_file,
                 h5py.File(tmp_path, "w") as compressed_file,
             ):
-                for key in original_file.keys():
+                for key, data in original_file.items():
                     compressed_file.create_dataset(
-                        key,
-                        data=original_file[key],
-                        compression="gzip" if "image" in key else None,
+                        key, data=data, compression="gzip" if "image" in key else None
                     )
             path.unlink()  # Windows needs this call before rename()
             tmp_path.rename(path)
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai.egg-info/PKG-INFO` & `idtrackerai-5.1.5/src/idtrackerai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idtrackerai
-Version: 5.1.4
+Version: 5.1.5
 Summary: Idtracker.ai tracks up to 100 unmarked animals from videos recorded in laboratory conditions using artificial intelligence. Free and open source.
 Author: Francisco Romero Ferrero, Mattia G. Bergomi, Francisco J.H. Heras, Ricardo Ribeiro
 Author-email: Jordi Torrents <jordi.torrentsm@gmail.com>
 Project-URL: Homepage, https://idtracker.ai/
 Project-URL: Repository, https://gitlab.com/polavieja_lab/idtrackerai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai.egg-info/SOURCES.txt` & `idtrackerai-5.1.5/src/idtrackerai.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -20,23 +20,17 @@
 src/idtrackerai.egg-info/requires.txt
 src/idtrackerai.egg-info/top_level.txt
 src/idtrackerai/animals_detection/__init__.py
 src/idtrackerai/animals_detection/animals_detection.py
 src/idtrackerai/animals_detection/segmentation.py
 src/idtrackerai/crossings_detection/__init__.py
 src/idtrackerai/crossings_detection/crossing_detector.py
-src/idtrackerai/crossings_detection/crossings_detection.py
+src/idtrackerai/crossings_detection/crossings_dataset.py
+src/idtrackerai/crossings_detection/crossings_network.py
 src/idtrackerai/crossings_detection/model_area.py
-src/idtrackerai/crossings_detection/dataset/__init__.py
-src/idtrackerai/crossings_detection/dataset/crossings_dataloader.py
-src/idtrackerai/crossings_detection/dataset/crossings_dataset.py
-src/idtrackerai/crossings_detection/network/__init__.py
-src/idtrackerai/crossings_detection/network/predictor_crossing_detector.py
-src/idtrackerai/crossings_detection/network/stop_training_criteria_crossings.py
-src/idtrackerai/crossings_detection/network/trainer_crossing_detector.py
 src/idtrackerai/data/test_A.avi
 src/idtrackerai/data/test_B.avi
 src/idtrackerai/fragmentation/__init__.py
 src/idtrackerai/fragmentation/fragmentation.py
 src/idtrackerai/groundtruth_utils/__init__.py
 src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py
 src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py
@@ -57,27 +51,21 @@
 src/idtrackerai/postprocess/erosion.py
 src/idtrackerai/postprocess/get_trajectories.py
 src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py
 src/idtrackerai/postprocess/trajectories_creation.py
 src/idtrackerai/postprocess/trajectories_to_csv.py
 src/idtrackerai/tracker/__init__.py
 src/idtrackerai/tracker/accumulation_manager.py
-src/idtrackerai/tracker/accumulation_manager_utils.py
 src/idtrackerai/tracker/accumulator.py
 src/idtrackerai/tracker/assigner.py
+src/idtrackerai/tracker/identity_dataset.py
+src/idtrackerai/tracker/identity_network.py
 src/idtrackerai/tracker/identity_transfer.py
 src/idtrackerai/tracker/pre_trainer.py
 src/idtrackerai/tracker/tracker.py
-src/idtrackerai/tracker/dataset/__init__.py
-src/idtrackerai/tracker/dataset/identification_dataloader.py
-src/idtrackerai/tracker/dataset/identification_dataset.py
-src/idtrackerai/tracker/network/__init__.py
-src/idtrackerai/tracker/network/get_predictions.py
-src/idtrackerai/tracker/network/stop_training_criteria.py
-src/idtrackerai/tracker/network/trainer.py
 src/idtrackerai/utils/__init__.py
 src/idtrackerai/utils/check_PyPI_version.py
 src/idtrackerai/utils/confparams.py
 src/idtrackerai/utils/init_logger.py
 src/idtrackerai/utils/py_utils.py
 src/idtrackerai_GUI_tools/GUI_main_base.py
 src/idtrackerai_GUI_tools/__init__.py
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_GUI_tools/GUI_main_base.py` & `idtrackerai-5.1.5/src/idtrackerai_GUI_tools/GUI_main_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 from pathlib import Path
 
-from PyQt6.QtCore import Qt, QThread, QTimer, QUrl, pyqtSignal
-from PyQt6.QtGui import QAction, QCloseEvent, QDesktopServices, QGuiApplication, QIcon
-from PyQt6.QtWidgets import (
+from qtpy.QtCore import Qt, QThread, QTimer, QUrl, Signal
+from qtpy.QtGui import QAction, QCloseEvent, QDesktopServices, QGuiApplication, QIcon
+from qtpy.QtWidgets import (
     QApplication,
     QDialog,
     QHBoxLayout,
     QLayout,
     QMainWindow,
     QMessageBox,
     QSizePolicy,
@@ -181,13 +181,13 @@
         QApplication.setFont(font)
 
         # This has to be here so that the font size change takes place
         self.parent_widget.setStyleSheet("QToolTip { color: black;}")
 
 
 class AutoCheckUpdatesThread(QThread):
-    out_of_date = pyqtSignal(str)
+    out_of_date = Signal(str)
 
     def run(self):
         is_out_of_date, message = check_version()
         if is_out_of_date:
             self.out_of_date.emit(message)
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat` & `idtrackerai-5.1.5/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai_GUI_tools/logo_256.png` & `idtrackerai-5.1.5/src/idtrackerai_GUI_tools/logo_256.png`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai_GUI_tools/tooltips.toml` & `idtrackerai-5.1.5/src/idtrackerai_GUI_tools/tooltips.toml`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/canvas.py` & `idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/canvas.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import logging
 from dataclasses import dataclass
 from math import sqrt
 
-from PyQt6.QtCore import QPoint, QPointF, Qt, pyqtSignal
-from PyQt6.QtGui import (
+from qtpy.QtCore import QPoint, QPointF, Qt, Signal
+from qtpy.QtGui import (
     QColor,
+    QColorConstants,
     QMouseEvent,
     QPainter,
     QPaintEvent,
     QPolygon,
     QWheelEvent,
 )
-from PyQt6.QtWidgets import QWidget
+from qtpy.QtWidgets import QWidget
 
 
-@dataclass
+@dataclass(slots=True)
 class CanvasMouseEvent:
     button: Qt.MouseButton
     """Clicked button"""
     zoom: float
     """Current zoom of the canvas when event was created"""
     xy_data: tuple[float, float]
     """Position of the click in content data units"""
@@ -38,32 +39,32 @@
     def drawPolygonFromVertices(self, vertices, scale: float):
         poly = QPolygon()
         poly.setPoints(
             *[int(coord * scale + 0.5) for point in vertices for coord in point]
         )
         super().drawPolygon(poly)
 
-    def setPenColor(self, color: QColor | int):
+    def setPenColor(self, color: QColor | int | Qt.GlobalColor):
         super().setPen(color)
         pen = self.pen()
         pen.setWidthF(1.3 * self.applied_zoom)
         super().setPen(pen)
 
     def drawBigPoint(self, x: float, y: float, size=7):
         radi = (size * self.applied_zoom) / 2
         super().drawEllipse(QPointF(x, y), radi, radi)
 
 
 class Canvas(QWidget):
     # TODO check better implementations with
     # QGraphicsItem, QGraphicsScene, QtQuick, Canvas
 
-    click_event = pyqtSignal(CanvasMouseEvent)
-    double_click_event = pyqtSignal(CanvasMouseEvent)
-    painting_time = pyqtSignal(CanvasPainter)
+    click_event = Signal(CanvasMouseEvent)
+    double_click_event = Signal(CanvasMouseEvent)
+    painting_time = Signal(CanvasPainter)
 
     def __init__(self, parent=None):
         super().__init__(parent)
         self.setFocusPolicy(Qt.FocusPolicy.StrongFocus)
         self.zoom = 3.0
         self.centerX: float = 0.0
         self.centerY: float = 0.0
@@ -77,15 +78,15 @@
         self.setCursor(Qt.CursorShape.PointingHandCursor)
 
     def paintEvent(self, event: QPaintEvent):
         painter = CanvasPainter(self, self.zoom)
         try:
             painter_rect = event.rect()
             painter.setRenderHint(QPainter.RenderHint.Antialiasing, True)
-            painter.fillRect(painter_rect, 0x000000)
+            painter.fillRect(painter_rect, QColorConstants.Black)
             axis_w = painter_rect.width() * self.zoom
             axis_h = painter_rect.height() * self.zoom
 
             # save inaccuracies in rounding to use in self.to_physical_units
             self.real_w_zoom = int(axis_w) / painter_rect.width()
             self.real_h_zoom = int(axis_h) / painter_rect.height()
             self.real_x0 = int(self.centerX - axis_w / 2)
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py` & `idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from PyQt6.QtCore import QEvent, QSize, Qt, QTimer, pyqtSignal
-from PyQt6.QtGui import QColor, QFocusEvent, QPainter, QPixmap
-from PyQt6.QtWidgets import (
+from qtpy.QtCore import QEvent, QSize, Qt, QTimer, Signal
+from qtpy.QtGui import QColor, QFocusEvent, QPainter, QPixmap
+from qtpy.QtWidgets import (
     QHBoxLayout,
     QLabel,
     QListWidget,
     QListWidgetItem,
     QToolButton,
     QWidget,
 )
 
 
 class CustomList(QListWidget):
-    lost_focus = pyqtSignal()
-    ListChanged = pyqtSignal()
-    newItemSelected = pyqtSignal(object)
-    removedItem = pyqtSignal(str)
+    lost_focus = Signal()
+    ListChanged = Signal()
+    newItemSelected = Signal(object)
+    removedItem = Signal(str)
 
     def __init__(self, max_n_row: int = 5):
         super().__init__()
         self.max_n_row = max_n_row
 
         self.setAlternatingRowColors(True)
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py` & `idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional
 
 import numpy as np
-from PyQt6.QtCore import QEvent, QPoint, QPointF, Qt
-from PyQt6.QtGui import QKeyEvent, QPainterPath, QPalette, QResizeEvent
-from PyQt6.QtWidgets import QFrame, QLabel, QSizePolicy, QWidget
+from qtpy.QtCore import QEvent, QPoint, QPointF, Qt
+from qtpy.QtGui import QKeyEvent, QPainterPath, QPalette, QResizeEvent
+from qtpy.QtWidgets import QFrame, QLabel, QSizePolicy, QWidget
 from superqt import QLabeledRangeSlider, QLabeledSlider
 from superqt.sliders._labeled import LabelPosition
 
 from idtrackerai.utils import get_vertices_from_label
 
 
 class QHLine(QFrame):
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py` & `idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/video_player.py` & `idtrackerai-5.1.5/src/idtrackerai_GUI_tools/widgets_utils/video_player.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,77 +1,78 @@
 import json
 from contextlib import suppress
 from pathlib import Path
 from time import perf_counter
 
 import numpy as np
 import toml
-from PyQt6.QtCore import QEvent, QRectF, QSize, Qt, QTimer, pyqtSignal
-from PyQt6.QtGui import (
+from qtpy.QtCore import QEvent, QRectF, QSize, Qt, QTimer, Signal
+from qtpy.QtGui import (
     QAction,
     QCloseEvent,
+    QColor,
+    QColorConstants,
     QIcon,
     QImage,
     QKeyEvent,
     QPainter,
     QPixmap,
     QPolygon,
 )
-from PyQt6.QtWidgets import (
+from qtpy.QtWidgets import (
     QDialog,
     QHBoxLayout,
     QLabel,
     QMainWindow,
     QSlider,
     QSpinBox,
     QToolButton,
     QVBoxLayout,
     QWidget,
 )
 
-from idtrackerai_GUI_tools import Canvas
-
+from .canvas import Canvas
 from .video_paths_holder import VideoPathHolder
 
 
 def play_pixmap(size: int):
     canvas = QPixmap(size, size)
     canvas.fill(Qt.GlobalColor.transparent)
     painter = QPainter(canvas)
     pen = painter.pen()
-    pen.setColor(0x306F00)
+    pen.setColor(QColor(0x306F00))
     pen.setWidth(2)
-    painter.setBrush(0xC0DF50)
+    painter.setBrush(QColor(0xC0DF50))
     painter.setPen(pen)
     poly = QPolygon()
     poly.setPoints(0, 0, 0, size, size, size // 2)
     painter.drawPolygon(poly)
     return canvas
 
 
 def pause_pixmap(size: int):
     canvas = QPixmap(size, size)
     canvas.fill(Qt.GlobalColor.transparent)
     painter = QPainter(canvas)
     a = size // 3
     poly = QPolygon()
     pen = painter.pen()
-    pen.setColor(0x404F40)
+    pen.setColor(QColor(0x404F40))
     pen.setWidth(2)
-    painter.setBrush(0x809F70)
+    painter.setBrush(QColor(0x809F70))
     painter.setPen(pen)
     poly.setPoints(0, 0, a, 0, a, size, 0, size)
     painter.drawPolygon(poly)
     poly.setPoints(size - a, 0, size, 0, size, size, size - a, size)
     painter.drawPolygon(poly)
     return canvas
 
 
 class VideoPlayer(QWidget):
-    painting_time = pyqtSignal(QPainter, int, np.ndarray)
+    painting_time = Signal(QPainter, int, np.ndarray)
     control_bar_h = 30
 
     def __init__(self, parent: QMainWindow):
         super().__init__(parent)
         self.canvas = Canvas(self)
         self.video_path_holder = VideoPathHolder()
 
@@ -238,26 +239,27 @@
 
         painter.drawImage(
             self.rect_to_draw_image,
             QImage(
                 frame.data,
                 frame.shape[1],
                 frame.shape[0],
+                (frame.shape[1] * 3 if color else frame.shape[1]),
                 (
                     QImage.Format.Format_BGR888
                     if color
                     else QImage.Format.Format_Grayscale8
                 ),
             ),
         )
         self.painting_time.emit(painter, current_frame, frame)
 
         painter.resetTransform()
         painter.setFont(self.font())
-        painter.setPen(0xFFFFFF)
+        painter.setPen(QColorConstants.White)
         if self.speed_label:
             painter.drawText(
                 self.canvas.rect(), Qt.AlignmentFlag.AlignBottom, self.speed_label
             )
 
         self.drawn_frame = current_frame
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_start_app/__main__.py` & `idtrackerai-5.1.5/src/idtrackerai_start_app/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 import logging
 import shutil
 import sys
 from importlib.metadata import version
 from importlib.resources import files
 from pathlib import Path
 
+try:
+    # PyQt has to be imported before CV2 (importing idtrackerai stuff implies CV2)
+    # If not, the QFileDialog.getFileNames() does not load the icons, very weird
+    from qtpy.QtWidgets import QApplication
+except ImportError:
+    logging.error(
+        "\n\tRUNNING AN IDTRACKER.AI INSTALLATION WITHOUT ANY QT BINDING.\n\tGUIs are"
+        " not available, only tracking directly from the terminal with the `--track`"
+        " flag.\n\tRun `pip install pyqt5` or `pip install pyqt6` to build a Qt"
+        " binding."
+    )
+
 import toml
-from PyQt6.QtWidgets import QApplication
 
 from idtrackerai.utils import (
     CustomError,
     check_version_on_console_thread,
     conf,
     initLogger,
     pprint_dict,
     wrap_exceptions,
 )
 
 from .arg_parser import parse_args
 
-# PyQt has to be imported before CV2 (importing idtrackerai stuff implies CV2)
-# If not, the QFileDialog.getFileNames() does not load the icons, very weird
-
 all_valid_parameters = (
     (Path(__file__).parent / "all_valid_parameters.dat").read_text().splitlines()
 )
 
 
 def load_toml(path: Path, name: str = "") -> dict:
     if not path.is_file():
@@ -110,16 +118,23 @@
         from .run_idtrackerai import RunIdTrackerAi
 
         return RunIdTrackerAi(parameters).track_video()
     return False
 
 
 def run_segmentation_GUI(params: dict):
-    from idtrackerai_start_app.segmentation_GUI import SegmentationGUI
-
+    try:
+        from idtrackerai_start_app.segmentation_GUI import SegmentationGUI
+    except ImportError:
+        raise CustomError(
+            "\n\tRUNNING AN IDTRACKER.AI INSTALLATION WITHOUT ANY QT BINDING.\n\tGUIs"
+            " are not available, only tracking directly from the terminal with the"
+            " `--track` flag.\n\tRun `pip install pyqt5` or `pip install pyqt6` to"
+            " build a Qt binding."
+        )
     app = QApplication(sys.argv)
     window = SegmentationGUI(params)
     window.show()
     app.exec()
 
 
 @wrap_exceptions
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_start_app/all_valid_parameters.dat` & `idtrackerai-5.1.5/src/idtrackerai_start_app/all_valid_parameters.dat`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai_start_app/arg_parser.py` & `idtrackerai-5.1.5/src/idtrackerai_start_app/arg_parser.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai_start_app/run_idtrackerai.py` & `idtrackerai-5.1.5/src/idtrackerai_start_app/run_idtrackerai.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import logging
 from os import cpu_count
-from pathlib import Path
 from shutil import copy
 
 from idtrackerai import ListOfBlobs, ListOfFragments, ListOfGlobalFragments, Video
 from idtrackerai.animals_detection import animals_detection_API
 from idtrackerai.crossings_detection import crossings_detection_API
 from idtrackerai.fragmentation import fragmentation_API
 from idtrackerai.postprocess import trajectories_API
 from idtrackerai.tracker.tracker import TrackerAPI
-from idtrackerai.utils import CustomError, conf
+from idtrackerai.utils import LOG_FILE_PATH, CustomError, conf
 
 
 class RunIdTrackerAi:
     def __init__(self, user_parameters: dict):
         # Set the number of jobs accordingly to the computer number of CPUs
         n_jobs = user_parameters["number_of_parallel_workers"]
         computer_CPUs = cpu_count()
@@ -103,14 +102,21 @@
                 self.list_of_global_fragments,
             )
 
             if not self.video.track_wo_identities:
                 if self.video.single_animal:
                     tracker.track_single_animal()
                 else:
+                    if self.list_of_global_fragments.no_global_fragment:
+                        raise CustomError(
+                            "There are no Global Fragments long enough to be candidates"
+                            " for accumulation, thus it is not possible to train the"
+                            " identification networks. The video has to contain longer"
+                            " slices where all animals are visible without crossings."
+                        )
                     if self.list_of_global_fragments.single_global_fragment:
                         tracker.track_single_global_fragment_video()
                     else:
                         self.list_of_fragments = tracker.track_with_identities()
                         self.list_of_fragments.update_id_images_dataset()
 
             self.save()
@@ -139,16 +145,16 @@
             logging.error(
                 "An error occurred, saving data before "
                 "printing traceback and exiting the program"
             )
             self.save()
             raise error
 
-        if hasattr(self, "video"):
-            copy(Path("idtrackerai.log"), self.video.session_folder / "idtrackerai.log")
+        if hasattr(self, "video") and LOG_FILE_PATH.is_file():
+            copy(LOG_FILE_PATH, self.video.session_folder / LOG_FILE_PATH.name)
         return success
 
     def save(self):
         if hasattr(self, "video"):
             self.video.save()
         if hasattr(self, "list_of_blobs"):
             self.list_of_blobs.save(self.video.blobs_path)
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_GUI.py` & `idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_GUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from pathlib import Path
 
 import toml
-from PyQt6.QtCore import Qt, QTimer
-from PyQt6.QtGui import QKeyEvent
-from PyQt6.QtWidgets import (
+from qtpy.QtCore import Qt, QTimer
+from qtpy.QtGui import QKeyEvent
+from qtpy.QtWidgets import (
     QCheckBox,
     QFileDialog,
     QHBoxLayout,
     QLabel,
     QLineEdit,
     QMessageBox,
     QPushButton,
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py` & `idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from cv2 import fitEllipse
-from PyQt6.QtCore import Qt, pyqtSignal
-from PyQt6.QtGui import QColor, QPainterPath
-from PyQt6.QtWidgets import (
+from qtpy.QtCore import Qt, Signal
+from qtpy.QtGui import QColor, QPainterPath
+from qtpy.QtWidgets import (
     QCheckBox,
     QDialog,
     QGridLayout,
     QHBoxLayout,
     QListView,
     QListWidgetItem,
     QMessageBox,
@@ -23,16 +23,16 @@
     CanvasPainter,
     CustomList,
     build_ROI_patches_from_list,
 )
 
 
 class ROIWidget(QWidget):
-    needToDraw = pyqtSignal()
-    valueChanged = pyqtSignal(object)  # np.ndarray | None
+    needToDraw = Signal()
+    valueChanged = Signal(object)  # np.ndarray | None
 
     def __init__(self, parent):
         super().__init__()
 
         self.CheckBox = QCheckBox("Regions of interest")
         self.CheckBox.stateChanged.connect(self.CheckBox_changed)
 
@@ -189,21 +189,21 @@
         if not self.CheckBox.isChecked():
             return
         painter.setPen(Qt.PenStyle.NoPen)
         painter.setBrush(QColor(255, 0, 0, 50))
         painter.drawPath(self.mask_path)
 
         painter.setBrush(Qt.BrushStyle.NoBrush)
-        painter.setPenColor(0x32640A)
+        painter.setPenColor(QColor(0x32640A))
         if self.ListItem_clicked:
             painter.drawPolygonFromVertices(
                 self.clicked_points, self.resolution_reduction
             )
         else:
-            painter.setBrush(0x349650)
+            painter.setBrush(QColor(0x349650))
             for point in self.clicked_points:
                 painter.drawBigPoint(*point)
 
 
 class ROI_PopUp(QDialog):
     def __init__(self, parent=None):
         super().__init__(parent=parent)
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py` & `idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
-from PyQt6.QtCore import Qt, QThread, QTimer, pyqtSignal
-from PyQt6.QtGui import QImage, QPainter, QPixmap
-from PyQt6.QtWidgets import (
+from qtpy.QtCore import Qt, QThread, QTimer, Signal
+from qtpy.QtGui import QImage, QPainter, QPixmap
+from qtpy.QtWidgets import (
     QCheckBox,
     QDialog,
     QHBoxLayout,
     QMessageBox,
     QProgressDialog,
     QToolButton,
     QWidget,
@@ -16,15 +16,15 @@
     generate_frame_stack,
 )
 from idtrackerai.utils import conf
 from idtrackerai_GUI_tools import Canvas
 
 
 class BkgComputationThread(QThread):
-    progress_changed = pyqtSignal(int)
+    progress_changed = Signal(int)
 
     def __init__(self):
         super().__init__()
         self.frame_stack = None
         self.bkg = None
         self.abort = False
         self.finished.connect(
@@ -76,15 +76,15 @@
 
     def paint_image(self, painter: QPainter):
         painter.drawPixmap(0, 0, self.pixmap)
 
     def show(self, frame: np.ndarray):
         height, width = frame.shape
         self.pixmap = QPixmap.fromImage(
-            QImage(frame.data, width, height, QImage.Format.Format_Grayscale8)
+            QImage(frame.data, width, height, width, QImage.Format.Format_Grayscale8)
         )
 
         self.canvas.centerX = int(width / 2)
         self.canvas.centerY = int(height / 2)
 
         ratio = width / height
 
@@ -97,15 +97,15 @@
             window_height = QDialog_size
         self.setGeometry(0, 0, window_width, window_height)
         QTimer.singleShot(0, lambda: self.canvas.adjust_zoom_to(width, height))
         super().exec()
 
 
 class BkgWidget(QWidget):
-    new_bkg_data = pyqtSignal(object)
+    new_bkg_data = Signal(object)
 
     def __init__(self, parent: QWidget):
         super().__init__()
         self.checkBox = QCheckBox("Background subtraction")
         self.checkBox.stateChanged.connect(self.CheckBox_changed)
         self.view_bkg = QToolButton()
         self.view_bkg.setText("View background")
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py` & `idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from PyQt6.QtCore import QRectF, Qt
-from PyQt6.QtGui import QPainter, QPaintEvent
-from PyQt6.QtWidgets import QWidget
+from qtpy.QtCore import QRectF, Qt
+from qtpy.QtGui import QColor, QColorConstants, QPainter, QPaintEvent
+from qtpy.QtWidgets import QWidget
 
 
 class BlobInfoWidget(QWidget):
     bar_width = 0.65
 
     def __init__(self):
         super().__init__()
@@ -90,24 +90,24 @@
             min_area_line = None
         elif number_of_blobs == 0:
             title = "No blobs detected"
             min_area_line = None
         else:
             if self.n_animals == 0:
                 title_prefix = "# animals = 0! "
-                painter.setBrush(0xBA2320)
-                painter.setPen(0x5A1010)
+                painter.setBrush(QColor(0xBA2320))
+                painter.setPen(QColor(0x5A1010))
             elif number_of_blobs > self.n_animals:
                 title_prefix = "More blobs than animals! "
-                painter.setBrush(0xBA2320)
-                painter.setPen(0x5A1010)
+                painter.setBrush(QColor(0xBA2320))
+                painter.setPen(QColor(0x5A1010))
             else:
                 title_prefix = ""
-                painter.setBrush(0x44A0D9)
-                painter.setPen(0x286384)
+                painter.setBrush(QColor(0x44A0D9))
+                painter.setPen(QColor(0x286384))
 
             bar_sep = axis_w / number_of_blobs
             bar_width = 0.7 * axis_w / number_of_blobs
             scale = axis_h / (1.1 * max(self.areas))
             rects = [
                 QRectF(
                     left + (i + 0.5) * bar_sep - 0.5 * bar_width,
@@ -128,28 +128,28 @@
                     + f"{number_of_blobs} blobs detected. "
                     f"Minimum area: {min_area_line:.0f} px"
                 )
 
         # Draw min area dashed line
         if min_area_line is not None:
             pen = painter.pen()
-            pen.setColor(0x808080)
+            pen.setColor(QColor(0x808080))
             pen.setStyle(Qt.PenStyle.DotLine)
             pen.setWidth(2)
             painter.setPen(pen)
             painter.drawLine(
                 left,
                 bottom - int(min_area_line * scale),
                 right,
                 bottom - int(min_area_line * scale),
             )
 
         # Draw title
         painter.setPen(
-            0xFF0000 if title == "Number of animals missing!" else base_color
+            QColorConstants.Red if title == "Number of animals missing!" else base_color
         )
         painter.drawText(
             0,
             0,
             w,
             top,
             Qt.AlignmentFlag.AlignHCenter | Qt.AlignmentFlag.AlignVCenter,
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py` & `idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import cv2
 import numpy as np
-from PyQt6.QtCore import pyqtSignal
-from PyQt6.QtGui import QColor, QPolygon
-from PyQt6.QtWidgets import QWidget
+from qtpy.QtCore import Signal
+from qtpy.QtGui import QColor, QPolygon
+from qtpy.QtWidgets import QWidget
 
 from idtrackerai.animals_detection.segmentation import process_frame
 from idtrackerai_GUI_tools import CanvasPainter
 
 
 class FrameAnalyzer(QWidget):
-    new_areas = pyqtSignal(int, list)
-    new_parameters = pyqtSignal()
+    new_areas = Signal(int, list)
+    new_parameters = Signal()
 
     def set_bkg(self, bkg_model):
         self.bkg_model = bkg_model
         self.bkg_model_resreduct = bkg_model
         self.use_bkg = bkg_model is not None
 
         if bkg_model is not None and self.resolution_reduction != 1:
@@ -93,11 +93,11 @@
 
     def paint_on_canvas(self, painter: CanvasPainter, frame_number: int, frame):
         if self.drawn_frame != frame_number or self.need_to_redraw:
             self.process_frame(frame)
             self.new_areas.emit(frame_number, self.areas)
             self.need_to_redraw = False
         painter.setBrush(QColor(60, 160, 255, 150))
-        painter.setPenColor(0x286384)
+        painter.setPenColor(QColor(0x286384))
         for i in range(self.n_blobs):
             painter.drawPolygon(self.blob_polygons[i])
         self.drawn_frame = frame_number
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py` & `idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from PyQt6.QtCore import Qt, pyqtSignal
-from PyQt6.QtWidgets import QHBoxLayout, QLabel, QWidget
+from qtpy.QtCore import Qt, Signal
+from qtpy.QtWidgets import QHBoxLayout, QLabel, QWidget
 
 from idtrackerai_GUI_tools import LabeledSlider, LabelRangeSlider
 
 
 class IntensityThresholds(QWidget):
-    newValue = pyqtSignal(object)
+    newValue = Signal(object)
 
     def __init__(self, parent, min, max):
         super().__init__()
         self.parent_widget = parent
         self.label_nobkg = QLabel("Blob intensity\nthresholds")
         self.label_nobkg.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.label_yesbkg = QLabel("Background\ndifference threshold")
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py` & `idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from typing import Sequence
 
-from PyQt6.QtCore import Qt, pyqtSignal
-from PyQt6.QtGui import QFocusEvent
-from PyQt6.QtWidgets import (
+from qtpy.QtCore import Qt, Signal
+from qtpy.QtGui import QFocusEvent
+from qtpy.QtWidgets import (
     QFileDialog,
     QHBoxLayout,
     QListView,
     QListWidget,
     QMessageBox,
     QPushButton,
     QSizePolicy,
@@ -54,18 +54,18 @@
     def focusOutEvent(self, event: QFocusEvent):
         super().focusOutEvent(event)
         if event.reason() is not Qt.FocusReason.ActiveWindowFocusReason:
             self.clearSelection()  # this IF fixes drag and drop errors on Wayland
 
 
 class OpenVideoWidget(QWidget):
-    new_video_paths = pyqtSignal(list, tuple, int, int, list)
-    path_clicked = pyqtSignal(int)
-    video_paths_reordered = pyqtSignal(list)
-    new_episodes = pyqtSignal(list, object)
+    new_video_paths = Signal(list, tuple, int, int, list)
+    path_clicked = Signal(int)
+    video_paths_reordered = Signal(list)
+    new_episodes = Signal(list, object)
 
     def __init__(self, parent=None):
         super().__init__()
         self.setLayout(QHBoxLayout())
         self.parent_widget = parent
         self.avaliable_extensions = conf.AVAILABLE_VIDEO_EXTENSION
         self.extension_filter = (
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py` & `idtrackerai-5.1.5/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import ast
 
-from PyQt6.QtCore import pyqtSignal
-from PyQt6.QtWidgets import QCheckBox, QHBoxLayout, QLineEdit, QMessageBox, QWidget
+from qtpy.QtCore import Signal
+from qtpy.QtWidgets import QCheckBox, QHBoxLayout, QLineEdit, QMessageBox, QWidget
 
 from idtrackerai_GUI_tools import LabelRangeSlider
 
 
 class TrackingIntervalsWidget(QWidget):
-    newValue = pyqtSignal(object)
+    newValue = Signal(object)
 
     def __init__(self, parent):
         super().__init__()
         self.checkbox = QCheckBox("Tracking interval")
         self.checkbox.clicked.connect(self.checkbox_clicked)
         self.range_slider = LabelRangeSlider(parent=parent, min=0, max=1)
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_start_app/tooltips.toml` & `idtrackerai-5.1.5/src/idtrackerai_start_app/tooltips.toml`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai_validator/__main__.py` & `idtrackerai-5.1.5/src/idtrackerai_validator/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 from argparse import ArgumentParser
 from pathlib import Path
 
-from PyQt6.QtWidgets import QApplication
+from qtpy.QtWidgets import QApplication
 
 from idtrackerai.utils import initLogger, wrap_exceptions
 from idtrackerai_validator.validation_GUI import ValidationGUI
 
 
 def input_args():
     parser = ArgumentParser()
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_validator/tooltips.toml` & `idtrackerai-5.1.5/src/idtrackerai_validator/tooltips.toml`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai_validator/validation_GUI.py` & `idtrackerai-5.1.5/src/idtrackerai_validator/validation_GUI.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import logging
 import sys
 from enum import Enum
 from pathlib import Path
 
 import numpy as np
 import toml
-from PyQt6.QtCore import Qt, QThread, QTimer, pyqtSignal
-from PyQt6.QtGui import QAction, QCloseEvent, QColor, QKeyEvent
-from PyQt6.QtWidgets import (
+from qtpy.QtCore import Qt, QThread, QTimer, Signal
+from qtpy.QtGui import QAction, QCloseEvent, QColor, QKeyEvent
+from qtpy.QtWidgets import (
     QApplication,
     QCheckBox,
     QDialog,
     QFileDialog,
     QHBoxLayout,
+    QInputDialog,
     QLabel,
     QMessageBox,
     QProgressDialog,
     QPushButton,
     QSpinBox,
     QSplitter,
     QTabWidget,
@@ -33,36 +34,31 @@
 from idtrackerai_GUI_tools import (
     CanvasMouseEvent,
     CanvasPainter,
     GUIBase,
     LabelRangeSlider,
     QHLine,
     VideoPlayer,
+    build_ROI_patches_from_list,
+    get_cmap,
 )
-from idtrackerai_GUI_tools import __file__ as idtrackerai_GUI_tools_file
-from idtrackerai_GUI_tools import build_ROI_patches_from_list
 
 from .validator_widgets import (
     AdditionalInfo,
     ErrorsExplorer,
     IdGroups,
     IdLabels,
     Interpolator,
     MarkBlobs,
     SetupPoints,
     find_selected_blob,
     paintBlobs,
     paintTrails,
 )
 
-parent_dir = Path(idtrackerai_GUI_tools_file).parent
-for file in parent_dir.glob("cmap_*"):
-    general_cmap = np.loadtxt(parent_dir / file, dtype=np.uint8)
-assert general_cmap is not None
-
 SELECT_POINT_DIST = 300
 
 
 class WarningRedirector(logging.Handler):
     def __init__(self, parent: GUIBase):
         super().__init__()
         self.parent = parent
@@ -344,14 +340,20 @@
             )
         )
 
         for action in drawing_flags.actions():
             action.setCheckable(True)
             action.toggled.connect(self.video_player.update)
 
+        find_identity_action = QAction("Find identity", self)
+        find_identity_action.setShortcut("Ctrl+F")
+        drawing_flags.addSeparator()
+        drawing_flags.addAction(find_identity_action)
+        find_identity_action.triggered.connect(self.find_identity)
+
         # Defaults
         self.view_labels.setChecked(True)
         self.view_contours.setChecked(True)
         self.view_centroids.setChecked(True)
         self.view_bboxes.setChecked(False)
         self.view_trails.setChecked(True)
         self.view_ROIs.setChecked(False)
@@ -376,14 +378,56 @@
                 tooltips["input_size"]
             )
 
         if session_path is not None:
             QTimer.singleShot(0, lambda: self.open_session(session_path))
         self.unsaved_changes = False
 
+    def find_identity(self):
+        """Displays a QInputDialog to select an identity to, then, find
+        its blob, select it and center the video canvas to its centroid"""
+        to_find, success = QInputDialog.getText(
+            self,
+            "",
+            "Identity to find:",
+            text=str(self.selected_id) if self.selected_id not in (None, -1) else "",
+            flags=Qt.WindowType.SplashScreen,
+        )
+        to_find = to_find.strip()
+
+        if not success or not to_find:
+            return
+
+        if to_find.isdigit():
+            identity_to_find = int(to_find)
+        else:
+            try:
+                identity_to_find = self.id_labels.labels.index(to_find)
+            except ValueError:
+                QMessageBox.warning(
+                    self, "Find error", f'Identity not recognized: "{to_find}"'
+                )
+                return
+
+        for blob in self.blobs.blobs_in_video[self.current_frame_number]:
+            for identity, centroid in blob.final_ids_and_centroids:
+                if identity == identity_to_find:
+                    self.selected_blob = blob
+                    self.selected_id = identity
+                    self.selection_last_location = centroid
+                    self.current_frame_number = -1  # this makes info_widget to update
+                    self.video_player.center_canvas_at(
+                        *centroid, 50 * self.median_speed
+                    )
+                    return
+
+        QMessageBox.warning(
+            self, "Find error", f"Identity {identity_to_find} not found in this frame"
+        )
+
     def keyPressEvent(self, event: QKeyEvent):
         if event.key() in (Qt.Key.Key_Return, Qt.Key.Key_Enter):
             self.id_groups.uncheck_edit_buttons()
             self.setup_points.add.setChecked(False)
 
     def go_to_error(
         self,
@@ -536,19 +580,19 @@
         self.generate_trajectories(self.blobs.blobs_in_video)
         self.median_speed = np.nanmedian(
             np.sqrt(np.sum(np.diff(self.trajectories, axis=0) ** 2, axis=-1))
         )
         self.centralWidget().setEnabled(True)
         self.dbl_click_dialog = DblClickDialog(self, video.number_of_animals)
 
-        cmap = [(255, 255, 255)] + list(
-            general_cmap[np.linspace(0, 255, video.number_of_animals, dtype=int)]
+        cmap = [(255, 255, 255)] + (
+            get_cmap()[np.linspace(0, 255, video.number_of_animals, dtype=int)].tolist()
         )
-        self.cmap = [QColor(*color) for color in cmap]
-        self.cmap_alpha = [QColor(*color, alpha=77) for color in cmap]
+        self.cmap = tuple(QColor(*color) for color in cmap)
+        self.cmap_alpha = tuple(QColor(*color, alpha=77) for color in cmap)
 
         self.id_groups.load_groups(video.identities_groups)
         self.id_labels.load_labels(
             video.identities_labels
             or [str(i + 1) for i in range(video.number_of_animals)]
         )
 
@@ -585,16 +629,15 @@
 
         self.reset_session_dialog = ResetSessionDialog(self, video.number_of_frames)
 
     def click_on_canvas(self, event: CanvasMouseEvent):
         self.selected_blob, self.selected_id, self.selection_last_location = clicked_id(
             self.blobs.blobs_in_video[self.current_frame_number], event
         )
-        if self.selected_id not in (-1, None):
-            self.id_groups.selected_id(self.selected_id)
+        self.id_groups.selected_id(self.selected_id)
         self.current_frame_number = -1  # this makes info_widget to update
         self.video_player.update()
 
     def double_click_on_canvas(self, event: CanvasMouseEvent):
         if (
             self.selected_blob is None
             or self.id_groups.is_active()
@@ -794,15 +837,15 @@
     if distances_to_centroids:
         return min(distances_to_centroids, key=lambda x: x[-1])[:-1]
 
     return None, -1, None
 
 
 class SaveTrajectoriesThread(QThread):
-    progress_changed = pyqtSignal(int)
+    progress_changed = Signal(int)
 
     def __init__(
         self,
         blobs_in_video: list[list[Blob]],
         video: Video,
         list_of_fragments: list[Fragment] | None,
     ):
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/__init__.py` & `idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/additional_info.py` & `idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/additional_info.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from PyQt6.QtGui import QKeyEvent
-from PyQt6.QtWidgets import QLabel, QListWidget, QVBoxLayout, QWidget
+from contextlib import suppress
+
+from qtpy.QtGui import QKeyEvent
+from qtpy.QtWidgets import QLabel, QListWidget, QVBoxLayout, QWidget
 
 from idtrackerai import Blob, Fragment
 from idtrackerai_GUI_tools import key_event_modifier
 
 
 class CustomListWidget(QListWidget):
     def __init__(self):
@@ -48,10 +50,11 @@
             return
 
         self.blob_properties.addItems(blob.properties)
 
         if self.fragments is None:
             return
 
-        self.fragment_properties.addItems(
-            self.fragments[blob.fragment_identifier].properties
-        )
+        with suppress(AttributeError):
+            self.fragment_properties.addItems(
+                self.fragments[blob.fragment_identifier].properties
+            )
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/errors_explorer.py` & `idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/errors_explorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import warnings
 
 import numpy as np
-from PyQt6.QtCore import Qt, pyqtSignal
-from PyQt6.QtGui import QKeyEvent
-from PyQt6.QtWidgets import (
+from qtpy.QtCore import Qt, Signal
+from qtpy.QtGui import QKeyEvent
+from qtpy.QtWidgets import (
     QAbstractItemView,
     QHBoxLayout,
     QHeaderView,
     QLabel,
     QTableWidget,
     QTableWidgetItem,
     QToolButton,
@@ -39,15 +39,15 @@
     def __lt__(self, other: QTableWidgetItem) -> bool:
         return self.data(Qt.ItemDataRole.UserRole) < other.data(
             Qt.ItemDataRole.UserRole
         )
 
 
 class ErrorsExplorer(QWidget):
-    go_to_error = pyqtSignal(str, int, int, object, int)
+    go_to_error = Signal(str, int, int, object, int)
     # kind, start, end, where, id
 
     def __init__(self):
         super().__init__()
         self.table = CustomTableWidget(1, 4)
         horizontalHeader = self.table.horizontalHeader()
         horizontalHeader.setSectionResizeMode(QHeaderView.ResizeMode.Stretch)
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/id_groups.py` & `idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/id_groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from PyQt6.QtCore import Qt, pyqtSignal
-from PyQt6.QtGui import QColor
-from PyQt6.QtWidgets import (
+from qtpy.QtCore import Qt, Signal
+from qtpy.QtGui import QColor
+from qtpy.QtWidgets import (
     QHBoxLayout,
     QInputDialog,
     QLabel,
     QToolButton,
     QVBoxLayout,
     QWidget,
 )
@@ -14,16 +14,16 @@
 Selected_Color = QColor(255, 0, 0)
 Unselected_Color = QColor(255, 255, 255)
 Selected_Color_alpha = QColor(255, 0, 0, 75)
 Unselected_Color_alpha = QColor(255, 255, 255, 75)
 
 
 class IdGroups(QWidget):
-    needToDraw = pyqtSignal()
-    unsaved_changes = pyqtSignal()
+    needToDraw = Signal()
+    unsaved_changes = Signal()
 
     def __init__(self, parent: QWidget):
         super().__init__(parent)
         self.main_layout = QVBoxLayout()
         self.setLayout(self.main_layout)
         first_row = QHBoxLayout()
         first_row.addWidget(QLabel("Identity groups"))
@@ -109,24 +109,26 @@
 
         self.id_groups = {
             key: (self.generate_row(key, set(value)), set(value))
             for key, value in identities_groups.items()
         }
 
     def selected_id(self, identity: int | None):
-        if self.editing_name and identity is not None:
-            row, group = self.id_groups[self.editing_name]
-            if identity in group:
-                group.remove(identity)
-            else:
-                group.add(identity)
-            label = row.findChild(WrappedLabel, "label")
-            assert isinstance(label, WrappedLabel)
-            label.setText(f"{self.editing_name}: {', '.join(map(str,group))}")
-            self.unsaved_changes.emit()
+        if not self.editing_name or identity in (-1, None):
+            return
+
+        row, group = self.id_groups[self.editing_name]
+        if identity in group:
+            group.remove(identity)
+        else:
+            group.add(identity)
+        label = row.findChild(WrappedLabel, "label")
+        assert isinstance(label, WrappedLabel)
+        label.setText(f"{self.editing_name}: {', '.join(map(str,group))}")
+        self.unsaved_changes.emit()
 
     def add_clicked(self):
         name, ok = QInputDialog.getText(
             self, "idtracker.ai", "Enter identity group name:"
         )
         name = name.strip()
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/id_labels.py` & `idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/id_labels.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from PyQt6.QtCore import Qt, pyqtSignal
-from PyQt6.QtWidgets import QFormLayout, QLineEdit, QScrollArea, QWidget
+from qtpy.QtCore import Qt, Signal
+from qtpy.QtWidgets import QFormLayout, QLineEdit, QScrollArea, QWidget
 
 
 class IdLabels(QScrollArea):
-    needToDraw = pyqtSignal()
+    needToDraw = Signal()
     labels: list[str]
 
     def __init__(self):
         super().__init__()
         self.form_layout = QFormLayout()
         self.setWidgetResizable(True)
         wid = QWidget()
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/interpolator.py` & `idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/interpolator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
-from PyQt6.QtCore import QEvent, QPointF, Qt, pyqtSignal
-from PyQt6.QtGui import QKeyEvent
-from PyQt6.QtWidgets import (
+from qtpy.QtCore import QEvent, QPointF, Qt, Signal
+from qtpy.QtGui import QColorConstants, QKeyEvent
+from qtpy.QtWidgets import (
     QComboBox,
     QGroupBox,
     QHBoxLayout,
     QLabel,
     QMessageBox,
     QPushButton,
     QRadioButton,
@@ -33,20 +33,20 @@
         event = key_event_modifier(e)
         if event is not None:
             super().keyReleaseEvent(event)
 
 
 class Interpolator(QGroupBox):
     interpolation_kinds = {"linear": 1, "quadratic": 2, "cubic": 3, "5th order": 5}
-    neew_to_draw = pyqtSignal()
-    update_trajectories = pyqtSignal(int, int)
-    go_to_frame = pyqtSignal(int)
-    preload_frames = pyqtSignal(int, int)
-    interpolation_accepted = pyqtSignal()
-    enabled_changed = pyqtSignal(bool)
+    neew_to_draw = Signal()
+    update_trajectories = Signal(int, int)
+    go_to_frame = Signal(int)
+    preload_frames = Signal(int, int)
+    interpolation_accepted = Signal()
+    enabled_changed = Signal(bool)
 
     def __init__(self) -> None:
         super().__init__()
         layout = QVBoxLayout()
         self.setLayout(layout)
 
         self.warning = WrappedLabel()
@@ -330,35 +330,35 @@
 
     def paint_on_canvas(self, painter: CanvasPainter, frame: int):
         self.current_frame = frame
         x_input = self.interp1d.x
         y_input = self.interp1d.y.T
 
         # interpolated points
-        painter.setPenColor(0xFFFFFF)
-        painter.setBrush(0xFFFFFF)
+        painter.setPenColor(QColorConstants.White)
+        painter.setBrush(QColorConstants.White)
         for point in self.interp1d(self.interpolation_range).T:
             painter.drawBigPoint(*point)
 
         # continuum interpolated range
         painter.drawPolyline(
             [
                 QPointF(*xy)
                 for xy in self.interp1d(self.continuous_interpolation_range).T
             ]  # type: ignore
         )
 
         # interpolator input data
-        painter.setPenColor(0xFF0000)
-        painter.setBrush(0xFF0000)
+        painter.setPenColor(QColorConstants.Red)
+        painter.setBrush(QColorConstants.Red)
         painter.drawPolyline([QPointF(*xy) for xy in y_input[x_input < self.start]])  # type: ignore
         painter.drawPolyline([QPointF(*xy) for xy in y_input[x_input >= self.end]])  # type: ignore
         for point in y_input:
             painter.drawBigPoint(*point)
 
         # actual point
         if (
             self.current_frame in self.interp1d.x
             or self.current_frame in self.interpolation_range
         ):
-            painter.setPenColor(0xFFFFFF)
+            painter.setPenColor(QColorConstants.White)
             painter.drawBigPoint(*self.interp1d(frame))
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/mark_properties.py` & `idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/mark_properties.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from collections.abc import Iterable
 
-from PyQt6.QtCore import Qt, pyqtSignal
-from PyQt6.QtWidgets import (
+from qtpy.QtCore import Qt, Signal
+from qtpy.QtWidgets import (
     QHBoxLayout,
     QRadioButton,
     QScrollArea,
     QSpinBox,
     QVBoxLayout,
     QWidget,
 )
 
 from idtrackerai import Blob, Fragment
 
 
 class MarkBlobs(QScrollArea):
-    needToDraw = pyqtSignal()
+    needToDraw = Signal()
 
     def __init__(self, parent: QWidget):
         main_layout = QVBoxLayout()
         super().__init__(parent)
         self.setWidgetResizable(True)
         wid = QWidget()
         wid.setLayout(main_layout)
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/paint_blobs.py` & `idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/paint_blobs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from typing import Iterable
+from typing import Iterable, Sequence
 
 import numpy as np
-from PyQt6.QtCore import QPointF, QRectF, Qt
-from PyQt6.QtGui import QColor, QImage, QPainter, QPolygon
+from qtpy.QtCore import QPointF, QRectF, Qt
+from qtpy.QtGui import QColor, QColorConstants, QImage, QPainter, QPolygon
 
 from idtrackerai import Blob
 from idtrackerai_GUI_tools import CanvasPainter
 
 
 def find_selected_blob(
     blobs_in_frame: list[Blob],
@@ -36,16 +36,16 @@
 def paintBlobs(
     draw_contours: bool,
     draw_centroids: bool,
     draw_bboxes: bool,
     draw_labels: bool,
     painter: CanvasPainter,
     blobs_in_frame: list[Blob],
-    cmap: list[QColor],
-    cmap_alpha: list[QColor],
+    cmap: Sequence[QColor],
+    cmap_alpha: Sequence[QColor],
     selected_blob: Blob | None,
     selected_centroid: tuple[float, float] | None,
     labels: list[str],
     marked_blobs: Iterable[Blob],
 ):
     labels_to_draw: list[tuple[QColor, str, tuple]] = []
     polygon = QPolygon()
@@ -56,15 +56,15 @@
             selected_blob_final_identities[0]
             if len(selected_blob_final_identities) == 1
             and selected_blob_final_identities[0] is not None
             else 0
         )
         color_alpha = cmap_alpha[color_indx]
 
-        painter.setPenColor(0xFFFFFF)
+        painter.setPenColor(QColorConstants.White)
         polygon.setPoints(*selected_blob.contour.ravel())
         painter.setBrush(color_alpha)
         painter.drawPolygon(polygon)
         painter.setBrush(Qt.BrushStyle.NoBrush)
 
     painter.setPen(Qt.PenStyle.NoPen)
     painter.setBrush(QColor(255, 0, 0, 128))
@@ -115,15 +115,15 @@
 
             color = cmap[0 if identity is None else identity]
             labels_to_draw.append((color, idstr, centroid))
 
     if selected_blob is not None and selected_centroid is not None:
         radius = 15 * painter.applied_zoom
         x, y = selected_centroid
-        painter.setPenColor(0x000000)
+        painter.setPenColor(QColorConstants.Black)
         painter.setBrush(Qt.BrushStyle.NoBrush)
         painter.drawEllipse(QRectF(x - radius / 2, y - radius / 2, radius, radius))
 
     # colored centroids
     if draw_centroids:
         painter.setPen(Qt.PenStyle.NoPen)
         for color, _idstr, (x, y) in labels_to_draw:
@@ -140,15 +140,15 @@
                 color.setAlpha(90)
                 painter.setPenColor(color)
                 painter.drawLine(pointA, pointB)
 
     # black centroid contour
     if draw_centroids:
         painter.setBrush(Qt.BrushStyle.NoBrush)
-        painter.setPenColor(0x000000)
+        painter.setPenColor(QColorConstants.Black)
         for _color, _idstr, (x, y) in labels_to_draw:
             painter.drawBigPoint(x, y)
 
     # label text
     if draw_labels:
         zoom = painter.applied_zoom
         for color, idstr, (x, y) in labels_to_draw:
@@ -159,15 +159,15 @@
                 painter.drawText(pointA, idstr)
 
 
 def paintTrails(
     frame_number: int,
     painter: CanvasPainter,
     trajectories: np.ndarray,
-    cmap: list[QColor],
+    cmap: Sequence[QColor],
 ):
     trail_length = 30
     trail_origin = None if frame_number < trail_length else frame_number - trail_length
     canvas = QImage(
         painter.viewport().size(), QImage.Format.Format_ARGB32_Premultiplied
     )
     canvas.fill(Qt.GlobalColor.transparent)
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/setup_points.py` & `idtrackerai-5.1.5/src/idtrackerai_validator/validator_widgets/setup_points.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 from re import compile
 
-from PyQt6.QtCore import Qt, pyqtSignal
-from PyQt6.QtWidgets import QInputDialog, QToolButton, QVBoxLayout, QWidget
+from qtpy.QtCore import Qt, Signal
+from qtpy.QtGui import QColor, QColorConstants
+from qtpy.QtWidgets import QInputDialog, QToolButton, QVBoxLayout, QWidget
 
 from idtrackerai_GUI_tools import CanvasMouseEvent, CanvasPainter, CustomList
 
 
 def has_invalid_chars(string):
     if len(string) == 0:
         return True
     regex = compile(r"[@!$%^&*?/\~:|]")
     return regex.search(string) is not None
 
 
 QColors = [
-    0x9467BD,
-    0x2CA02C,
-    0xBCBD22,
-    0xFF7F0E,
-    0x8C564B,
-    0xE377C2,
-    0x7F7F7F,
-    0x17BECF,
+    QColor(0x9467BD),
+    QColor(0x2CA02C),
+    QColor(0xBCBD22),
+    QColor(0xFF7F0E),
+    QColor(0x8C564B),
+    QColor(0xE377C2),
+    QColor(0x7F7F7F),
+    QColor(0x17BECF),
 ]
 n_colors = len(QColors)
 
 
 class SetupPoints(QWidget):
-    needToDraw = pyqtSignal()
+    needToDraw = Signal()
 
     def __init__(self):
         super().__init__()
 
         self.add = QToolButton()
         self.add.setText("Add")
         self.add.setCheckable(True)
@@ -41,15 +42,15 @@
         layout = QVBoxLayout()
         layout.setSpacing(2)
         self.setLayout(layout)
         layout.addWidget(self.add)
         layout.addWidget(self.list)
 
         self.add.toggled.connect(self.add_clicked)
-        self.setup_points_dict: dict[str, tuple[int, list[tuple[float, float]]]] = {}
+        self.setup_points_dict: dict[str, tuple[QColor, list[tuple[float, float]]]] = {}
         self.list.ListChanged.connect(self.needToDraw.emit)
         self.list.removedItem.connect(self.remove_item)
         self.color_count = -1
         self.setup_name = None
 
     def click_event(self, event: CanvasMouseEvent):
         if self.isVisible() and self.isEnabled() and self.setup_name is not None:
@@ -130,12 +131,12 @@
                 color=QColors[self.color_count],
             )
 
     def get_points(self) -> dict[str, list[tuple[float, float]]]:
         return {key: value[1] for key, value in self.setup_points_dict.items()}
 
     def paint_on_canvas(self, painter: CanvasPainter):
-        painter.setPenColor(0x000000)  # set pen to color black
+        painter.setPenColor(QColorConstants.Black)
         for color, points in self.setup_points_dict.values():
             painter.setBrush(color)
             for point in points:
                 painter.drawBigPoint(*point)
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_video/general_video.py` & `idtrackerai-5.1.5/src/idtrackerai_video/general_video.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 import logging
-from pathlib import Path
 
 import cv2
 import numpy as np
-from PyQt6.QtCore import Qt
-from PyQt6.QtGui import QColor, QImage, QPainter
+from qtpy.QtCore import Qt
+from qtpy.QtGui import QColor, QImage, QPainter
 
-import idtrackerai_GUI_tools
 from idtrackerai import Video
 from idtrackerai.utils import track
+from idtrackerai_GUI_tools import VideoPathHolder, get_cmap
 
 
 def QImageToArray(qimg: QImage) -> np.ndarray:
     width = qimg.width()
     height = qimg.height()
     byte_str = qimg.bits()
     return np.frombuffer(byte_str.asarray(height * width * 4), np.uint8).reshape(
         (height, width, 4)
     )[:, :, :-1]
 
 
-def setColormap(n_animals):
-    parent_dir = Path(idtrackerai_GUI_tools.__file__).parent
-    for file in parent_dir.glob("cmap_*"):
-        general_cmap = np.loadtxt(parent_dir / file, dtype=np.int32)
-    return [general_cmap[int(i * 255 / n_animals)] for i in range(n_animals)]
+def setColormap(n_animals: int):
+    return get_cmap()[[int(i * 255 / n_animals) for i in range(n_animals)]]
 
 
 def draw_general_frame(
     np_frame: np.ndarray,
     frame_number: int,
     trajectories: np.ndarray,
     centroid_trace_length: int,
     colors: list[tuple[int, int, int]],
     labels: list[str],
 ) -> np.ndarray:
     ordered_centroid = trajectories[frame_number]
     frame = QImage(
-        np_frame.data, np_frame.shape[1], np_frame.shape[0], QImage.Format.Format_BGR888
+        np_frame.data,
+        np_frame.shape[1],
+        np_frame.shape[0],
+        np_frame.shape[1] * 3,
+        QImage.Format.Format_BGR888,
     )
     canvas = QImage(frame.size(), QImage.Format.Format_ARGB32_Premultiplied)
     canvas.fill(Qt.GlobalColor.transparent)
     painter = QPainter(canvas)
     painter.setRenderHint(QPainter.RenderHint.Antialiasing, True)
     painter.setCompositionMode(QPainter.CompositionMode.CompositionMode_Source)
     pen = painter.pen()
@@ -133,15 +133,15 @@
     video_writer = cv2.VideoWriter(
         str(path_to_save_video),
         cv2.VideoWriter_fourcc(*"XVID"),
         video.frames_per_second,
         (out_video_width, out_video_height),
     )
 
-    videoPathHolder = idtrackerai_GUI_tools.VideoPathHolder(video.video_paths)
+    videoPathHolder = VideoPathHolder(video.video_paths)
 
     ending_frame = len(trajectories) - 1 if ending_frame is None else ending_frame
     logging.info(f"Drawing from frame {starting_frame} to {ending_frame}")
 
     for frame in track(range(starting_frame, ending_frame), "Generating video"):
         img = videoPathHolder.read_frame(frame, True)
```

### Comparing `idtrackerai-5.1.4/src/idtrackerai_video/individual_videos.py` & `idtrackerai-5.1.5/src/idtrackerai_video/individual_videos.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.4/src/idtrackerai_video/main.py` & `idtrackerai-5.1.5/src/idtrackerai_video/main.py`

 * *Files identical despite different names*

