# Comparing `tmp/mixprop-0.0.4.tar.gz` & `tmp/mixprop-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixprop-0.0.4.tar", last modified: Thu Jun 15 14:48:21 2023, max compression
+gzip compressed data, was "mixprop-0.0.5.tar", last modified: Thu Jun 15 15:56:10 2023, max compression
```

## Comparing `mixprop-0.0.4.tar` & `mixprop-0.0.5.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 14:48:21.232218 mixprop-0.0.4/
--rw-r--r--   0 cur5wz     (502) staff       (20)     1075 2023-06-14 17:36:40.000000 mixprop-0.0.4/LICENSE
--rw-r--r--   0 cur5wz     (502) staff       (20)      122 2023-06-14 17:36:40.000000 mixprop-0.0.4/MANIFEST.in
--rw-r--r--   0 cur5wz     (502) staff       (20)     1129 2023-06-15 14:48:21.232564 mixprop-0.0.4/PKG-INFO
--rw-r--r--   0 cur5wz     (502) staff       (20)      385 2023-06-14 17:36:40.000000 mixprop-0.0.4/README.md
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 14:48:21.074835 mixprop-0.0.4/mixprop/
--rw-r--r--   0 cur5wz     (502) staff       (20)      428 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/__init__.py
--rw-r--r--   0 cur5wz     (502) staff       (20)      196 2023-06-15 14:47:30.000000 mixprop-0.0.4/mixprop/_version.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    43236 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/args.py
--rw-r--r--   0 cur5wz     (502) staff       (20)      233 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/constants.py
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 14:48:21.123871 mixprop-0.0.4/mixprop/curation_pipeline/
--rw-r--r--   0 cur5wz     (502) staff       (20)     3006 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/curation_pipeline/T_logV_correlation.py
--rw-r--r--   0 cur5wz     (502) staff       (20)        1 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/curation_pipeline/__init__.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     1884 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/curation_pipeline/load_data.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     5105 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/curation_pipeline/pchip_interpolation.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     4369 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/curation_pipeline/pipeline.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     4326 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/curation_pipeline/remove_inconsistent.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     1334 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/curation_pipeline/remove_not_liquid.py
--rw-r--r--   0 cur5wz     (502) staff       (20)      472 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/curation_pipeline/remove_salts.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     2197 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/curation_pipeline/split_data.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     3635 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/curation_pipeline/utils.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     1480 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/curation_pipeline/write_data.py
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 14:48:21.144793 mixprop-0.0.4/mixprop/data/
--rw-r--r--   0 cur5wz     (502) staff       (20)     1276 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/data/__init__.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    32394 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/data/data.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     7839 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/data/scaffold.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     2791 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/data/scaler.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    32574 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/data/utils.py
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 14:48:21.177116 mixprop-0.0.4/mixprop/features/
--rw-r--r--   0 cur5wz     (502) staff       (20)     1393 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/features/__init__.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     6219 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/features/features_generators.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    31849 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/features/featurization.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     4085 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/features/utils.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     7860 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/hyperopt_utils.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     6909 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/hyperparameter_optimization.py
--rwxr-xr-x   0 cur5wz     (502) staff       (20)    13820 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/interpret.py
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 14:48:21.187102 mixprop-0.0.4/mixprop/models/
--rw-r--r--   0 cur5wz     (502) staff       (20)      130 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/models/__init__.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    14231 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/models/model.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    15153 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/models/mpn.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     7788 2023-06-14 17:36:40.000000 mixprop-0.0.4/mixprop/nn_utils.py
--rw-r--r--   0 cur5wz     (502) staff       (20)      636 2023-06-14 17:36:41.000000 mixprop-0.0.4/mixprop/rdkit.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     3025 2023-06-14 17:36:41.000000 mixprop-0.0.4/mixprop/sklearn_predict.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    14923 2023-06-14 17:36:41.000000 mixprop-0.0.4/mixprop/sklearn_train.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     5245 2023-06-14 17:36:41.000000 mixprop-0.0.4/mixprop/spectra_utils.py
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 14:48:21.227790 mixprop-0.0.4/mixprop/train/
--rw-r--r--   0 cur5wz     (502) staff       (20)     1285 2023-06-14 17:36:41.000000 mixprop-0.0.4/mixprop/train/__init__.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     8013 2023-06-14 17:36:41.000000 mixprop-0.0.4/mixprop/train/cross_validate.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     5868 2023-06-14 17:36:41.000000 mixprop-0.0.4/mixprop/train/evaluate.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     9575 2023-06-14 17:36:41.000000 mixprop-0.0.4/mixprop/train/loss_functions.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    15630 2023-06-14 17:36:41.000000 mixprop-0.0.4/mixprop/train/make_predictions.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    13018 2023-06-14 17:36:41.000000 mixprop-0.0.4/mixprop/train/metrics.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     9771 2023-06-14 17:36:41.000000 mixprop-0.0.4/mixprop/train/molecule_fingerprint.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     1795 2023-06-14 17:36:41.000000 mixprop-0.0.4/mixprop/train/predict.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    16099 2023-06-14 17:36:41.000000 mixprop-0.0.4/mixprop/train/run_training.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     6150 2023-06-14 17:36:41.000000 mixprop-0.0.4/mixprop/train/train.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    30646 2023-06-14 17:36:41.000000 mixprop-0.0.4/mixprop/utils.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     6076 2023-06-15 14:45:29.000000 mixprop-0.0.4/mixprop/visc_pred_wrapper.py
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 14:48:21.080511 mixprop-0.0.4/mixprop.egg-info/
--rw-r--r--   0 cur5wz     (502) staff       (20)     1129 2023-06-15 14:48:20.000000 mixprop-0.0.4/mixprop.egg-info/PKG-INFO
--rw-r--r--   0 cur5wz     (502) staff       (20)     1668 2023-06-15 14:48:20.000000 mixprop-0.0.4/mixprop.egg-info/SOURCES.txt
--rw-r--r--   0 cur5wz     (502) staff       (20)      133 2023-06-15 14:48:20.000000 mixprop-0.0.4/mixprop.egg-info/dependency_links.txt
--rw-r--r--   0 cur5wz     (502) staff       (20)        1 2023-06-14 15:18:23.000000 mixprop-0.0.4/mixprop.egg-info/not-zip-safe
--rw-r--r--   0 cur5wz     (502) staff       (20)      133 2023-06-15 14:48:20.000000 mixprop-0.0.4/mixprop.egg-info/requires.txt
--rw-r--r--   0 cur5wz     (502) staff       (20)        8 2023-06-15 14:48:20.000000 mixprop-0.0.4/mixprop.egg-info/top_level.txt
--rw-r--r--   0 cur5wz     (502) staff       (20)      132 2023-06-15 14:28:35.000000 mixprop-0.0.4/requirements.txt
--rw-r--r--   0 cur5wz     (502) staff       (20)      390 2023-06-15 14:48:21.234981 mixprop-0.0.4/setup.cfg
--rw-r--r--   0 cur5wz     (502) staff       (20)     1723 2023-06-15 14:47:16.000000 mixprop-0.0.4/setup.py
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 14:48:21.231204 mixprop-0.0.4/tests/
--rw-r--r--   0 cur5wz     (502) staff       (20)      387 2023-06-14 17:36:41.000000 mixprop-0.0.4/tests/test_mixprop.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 15:56:10.280902 mixprop-0.0.5/
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1075 2023-06-14 17:36:40.000000 mixprop-0.0.5/LICENSE
+-rw-r--r--   0 cur5wz     (502) staff       (20)      122 2023-06-14 17:36:40.000000 mixprop-0.0.5/MANIFEST.in
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1129 2023-06-15 15:56:10.281063 mixprop-0.0.5/PKG-INFO
+-rw-r--r--   0 cur5wz     (502) staff       (20)      385 2023-06-14 17:36:40.000000 mixprop-0.0.5/README.md
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 15:56:10.124733 mixprop-0.0.5/mixprop/
+-rw-r--r--   0 cur5wz     (502) staff       (20)      428 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/__init__.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)      196 2023-06-15 15:55:59.000000 mixprop-0.0.5/mixprop/_version.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    43236 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/args.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)      233 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/constants.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 15:56:10.188405 mixprop-0.0.5/mixprop/curation_pipeline/
+-rw-r--r--   0 cur5wz     (502) staff       (20)     3006 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/T_logV_correlation.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)        1 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/__init__.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1884 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/load_data.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     5105 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/pchip_interpolation.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     4369 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/pipeline.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     4326 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/remove_inconsistent.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1334 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/remove_not_liquid.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)      472 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/remove_salts.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     2197 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/split_data.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     3635 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/utils.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1480 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/write_data.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 15:56:10.208365 mixprop-0.0.5/mixprop/data/
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1276 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/data/__init__.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    32394 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/data/data.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     7839 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/data/scaffold.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     2791 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/data/scaler.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    32574 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/data/utils.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 15:56:10.227087 mixprop-0.0.5/mixprop/features/
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1393 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/features/__init__.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     6219 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/features/features_generators.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    31849 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/features/featurization.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     4085 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/features/utils.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     7860 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/hyperopt_utils.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     6909 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/hyperparameter_optimization.py
+-rwxr-xr-x   0 cur5wz     (502) staff       (20)    13820 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/interpret.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 15:56:10.240411 mixprop-0.0.5/mixprop/models/
+-rw-r--r--   0 cur5wz     (502) staff       (20)      130 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/models/__init__.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    14231 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/models/model.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    15153 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/models/mpn.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     7788 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/nn_utils.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)      636 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/rdkit.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     3025 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/sklearn_predict.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    14923 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/sklearn_train.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     5245 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/spectra_utils.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 15:56:10.275492 mixprop-0.0.5/mixprop/train/
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1285 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/train/__init__.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     8013 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/train/cross_validate.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     5868 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/train/evaluate.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     9575 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/train/loss_functions.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    15630 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/train/make_predictions.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    13018 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/train/metrics.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     9771 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/train/molecule_fingerprint.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1795 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/train/predict.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    16099 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/train/run_training.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     6150 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/train/train.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    30646 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/utils.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     6076 2023-06-15 15:52:46.000000 mixprop-0.0.5/mixprop/visc_pred_wrapper.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 15:56:10.141760 mixprop-0.0.5/mixprop.egg-info/
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1129 2023-06-15 15:56:09.000000 mixprop-0.0.5/mixprop.egg-info/PKG-INFO
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1668 2023-06-15 15:56:10.000000 mixprop-0.0.5/mixprop.egg-info/SOURCES.txt
+-rw-r--r--   0 cur5wz     (502) staff       (20)      133 2023-06-15 15:56:10.000000 mixprop-0.0.5/mixprop.egg-info/dependency_links.txt
+-rw-r--r--   0 cur5wz     (502) staff       (20)        1 2023-06-14 15:18:23.000000 mixprop-0.0.5/mixprop.egg-info/not-zip-safe
+-rw-r--r--   0 cur5wz     (502) staff       (20)      133 2023-06-15 15:56:10.000000 mixprop-0.0.5/mixprop.egg-info/requires.txt
+-rw-r--r--   0 cur5wz     (502) staff       (20)        8 2023-06-15 15:56:10.000000 mixprop-0.0.5/mixprop.egg-info/top_level.txt
+-rw-r--r--   0 cur5wz     (502) staff       (20)      132 2023-06-15 14:28:35.000000 mixprop-0.0.5/requirements.txt
+-rw-r--r--   0 cur5wz     (502) staff       (20)      390 2023-06-15 15:56:10.281675 mixprop-0.0.5/setup.cfg
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1723 2023-06-15 15:55:34.000000 mixprop-0.0.5/setup.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 15:56:10.280387 mixprop-0.0.5/tests/
+-rw-r--r--   0 cur5wz     (502) staff       (20)      387 2023-06-14 17:36:41.000000 mixprop-0.0.5/tests/test_mixprop.py
```

### Comparing `mixprop-0.0.4/LICENSE` & `mixprop-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/PKG-INFO` & `mixprop-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixprop
-Version: 0.0.4
+Version: 0.0.5
 Summary: Viscosity prediction for binary liquid mixtures
 Home-page: https://github.com/cbilodeau2/mixprop_viscosity
 Author: Camille Bilodeau
 Author-email: camille79bilodeau@gmail.com
 License: MIT license
 Keywords: mixprop
 Classifier: Intended Audience :: Developers
```

### Comparing `mixprop-0.0.4/mixprop/args.py` & `mixprop-0.0.5/mixprop/args.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/curation_pipeline/T_logV_correlation.py` & `mixprop-0.0.5/mixprop/curation_pipeline/T_logV_correlation.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/curation_pipeline/load_data.py` & `mixprop-0.0.5/mixprop/curation_pipeline/load_data.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/curation_pipeline/pchip_interpolation.py` & `mixprop-0.0.5/mixprop/curation_pipeline/pchip_interpolation.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/curation_pipeline/pipeline.py` & `mixprop-0.0.5/mixprop/curation_pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/curation_pipeline/remove_inconsistent.py` & `mixprop-0.0.5/mixprop/curation_pipeline/remove_inconsistent.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/curation_pipeline/remove_not_liquid.py` & `mixprop-0.0.5/mixprop/curation_pipeline/remove_not_liquid.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/curation_pipeline/split_data.py` & `mixprop-0.0.5/mixprop/curation_pipeline/split_data.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/curation_pipeline/utils.py` & `mixprop-0.0.5/mixprop/curation_pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/curation_pipeline/write_data.py` & `mixprop-0.0.5/mixprop/curation_pipeline/write_data.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/data/__init__.py` & `mixprop-0.0.5/mixprop/data/__init__.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/data/data.py` & `mixprop-0.0.5/mixprop/data/data.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/data/scaffold.py` & `mixprop-0.0.5/mixprop/data/scaffold.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/data/scaler.py` & `mixprop-0.0.5/mixprop/data/scaler.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/data/utils.py` & `mixprop-0.0.5/mixprop/data/utils.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/features/__init__.py` & `mixprop-0.0.5/mixprop/features/__init__.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/features/features_generators.py` & `mixprop-0.0.5/mixprop/features/features_generators.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/features/featurization.py` & `mixprop-0.0.5/mixprop/features/featurization.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/features/utils.py` & `mixprop-0.0.5/mixprop/features/utils.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/hyperopt_utils.py` & `mixprop-0.0.5/mixprop/hyperopt_utils.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/hyperparameter_optimization.py` & `mixprop-0.0.5/mixprop/hyperparameter_optimization.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/interpret.py` & `mixprop-0.0.5/mixprop/interpret.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/models/model.py` & `mixprop-0.0.5/mixprop/models/model.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/models/mpn.py` & `mixprop-0.0.5/mixprop/models/mpn.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/nn_utils.py` & `mixprop-0.0.5/mixprop/nn_utils.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/rdkit.py` & `mixprop-0.0.5/mixprop/rdkit.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/sklearn_predict.py` & `mixprop-0.0.5/mixprop/sklearn_predict.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/sklearn_train.py` & `mixprop-0.0.5/mixprop/sklearn_train.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/spectra_utils.py` & `mixprop-0.0.5/mixprop/spectra_utils.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/train/__init__.py` & `mixprop-0.0.5/mixprop/train/__init__.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/train/cross_validate.py` & `mixprop-0.0.5/mixprop/train/cross_validate.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/train/evaluate.py` & `mixprop-0.0.5/mixprop/train/evaluate.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/train/loss_functions.py` & `mixprop-0.0.5/mixprop/train/loss_functions.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/train/make_predictions.py` & `mixprop-0.0.5/mixprop/train/make_predictions.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/train/metrics.py` & `mixprop-0.0.5/mixprop/train/metrics.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/train/molecule_fingerprint.py` & `mixprop-0.0.5/mixprop/train/molecule_fingerprint.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/train/predict.py` & `mixprop-0.0.5/mixprop/train/predict.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/train/run_training.py` & `mixprop-0.0.5/mixprop/train/run_training.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/train/train.py` & `mixprop-0.0.5/mixprop/train/train.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/utils.py` & `mixprop-0.0.5/mixprop/utils.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop/visc_pred_wrapper.py` & `mixprop-0.0.5/mixprop/visc_pred_wrapper.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/mixprop.egg-info/PKG-INFO` & `mixprop-0.0.5/mixprop.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixprop
-Version: 0.0.4
+Version: 0.0.5
 Summary: Viscosity prediction for binary liquid mixtures
 Home-page: https://github.com/cbilodeau2/mixprop_viscosity
 Author: Camille Bilodeau
 Author-email: camille79bilodeau@gmail.com
 License: MIT license
 Keywords: mixprop
 Classifier: Intended Audience :: Developers
```

### Comparing `mixprop-0.0.4/mixprop.egg-info/SOURCES.txt` & `mixprop-0.0.5/mixprop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.4/setup.py` & `mixprop-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='mixprop',
     name='mixprop',
     packages=find_packages(include=['mixprop', 'mixprop.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/cbilodeau2/mixprop_viscosity',
-    version='0.0.4',
+    version='0.0.5',
     zip_safe=False,
 )
```

