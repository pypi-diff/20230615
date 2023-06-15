# Comparing `tmp/mixprop-0.0.5.tar.gz` & `tmp/mixprop-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixprop-0.0.5.tar", last modified: Thu Jun 15 15:56:10 2023, max compression
+gzip compressed data, was "dist/mixprop-0.0.6.tar", last modified: Thu Jun 15 18:08:13 2023, max compression
```

## Comparing `mixprop-0.0.5.tar` & `mixprop-0.0.6.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 15:56:10.280902 mixprop-0.0.5/
--rw-r--r--   0 cur5wz     (502) staff       (20)     1075 2023-06-14 17:36:40.000000 mixprop-0.0.5/LICENSE
--rw-r--r--   0 cur5wz     (502) staff       (20)      122 2023-06-14 17:36:40.000000 mixprop-0.0.5/MANIFEST.in
--rw-r--r--   0 cur5wz     (502) staff       (20)     1129 2023-06-15 15:56:10.281063 mixprop-0.0.5/PKG-INFO
--rw-r--r--   0 cur5wz     (502) staff       (20)      385 2023-06-14 17:36:40.000000 mixprop-0.0.5/README.md
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 15:56:10.124733 mixprop-0.0.5/mixprop/
--rw-r--r--   0 cur5wz     (502) staff       (20)      428 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/__init__.py
--rw-r--r--   0 cur5wz     (502) staff       (20)      196 2023-06-15 15:55:59.000000 mixprop-0.0.5/mixprop/_version.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    43236 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/args.py
--rw-r--r--   0 cur5wz     (502) staff       (20)      233 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/constants.py
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 15:56:10.188405 mixprop-0.0.5/mixprop/curation_pipeline/
--rw-r--r--   0 cur5wz     (502) staff       (20)     3006 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/T_logV_correlation.py
--rw-r--r--   0 cur5wz     (502) staff       (20)        1 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/__init__.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     1884 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/load_data.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     5105 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/pchip_interpolation.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     4369 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/pipeline.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     4326 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/remove_inconsistent.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     1334 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/remove_not_liquid.py
--rw-r--r--   0 cur5wz     (502) staff       (20)      472 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/remove_salts.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     2197 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/split_data.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     3635 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/utils.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     1480 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/curation_pipeline/write_data.py
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 15:56:10.208365 mixprop-0.0.5/mixprop/data/
--rw-r--r--   0 cur5wz     (502) staff       (20)     1276 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/data/__init__.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    32394 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/data/data.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     7839 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/data/scaffold.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     2791 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/data/scaler.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    32574 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/data/utils.py
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 15:56:10.227087 mixprop-0.0.5/mixprop/features/
--rw-r--r--   0 cur5wz     (502) staff       (20)     1393 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/features/__init__.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     6219 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/features/features_generators.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    31849 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/features/featurization.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     4085 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/features/utils.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     7860 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/hyperopt_utils.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     6909 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/hyperparameter_optimization.py
--rwxr-xr-x   0 cur5wz     (502) staff       (20)    13820 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/interpret.py
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 15:56:10.240411 mixprop-0.0.5/mixprop/models/
--rw-r--r--   0 cur5wz     (502) staff       (20)      130 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/models/__init__.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    14231 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/models/model.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    15153 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/models/mpn.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     7788 2023-06-14 17:36:40.000000 mixprop-0.0.5/mixprop/nn_utils.py
--rw-r--r--   0 cur5wz     (502) staff       (20)      636 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/rdkit.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     3025 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/sklearn_predict.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    14923 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/sklearn_train.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     5245 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/spectra_utils.py
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 15:56:10.275492 mixprop-0.0.5/mixprop/train/
--rw-r--r--   0 cur5wz     (502) staff       (20)     1285 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/train/__init__.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     8013 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/train/cross_validate.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     5868 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/train/evaluate.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     9575 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/train/loss_functions.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    15630 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/train/make_predictions.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    13018 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/train/metrics.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     9771 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/train/molecule_fingerprint.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     1795 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/train/predict.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    16099 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/train/run_training.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     6150 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/train/train.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    30646 2023-06-14 17:36:41.000000 mixprop-0.0.5/mixprop/utils.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     6076 2023-06-15 15:52:46.000000 mixprop-0.0.5/mixprop/visc_pred_wrapper.py
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 15:56:10.141760 mixprop-0.0.5/mixprop.egg-info/
--rw-r--r--   0 cur5wz     (502) staff       (20)     1129 2023-06-15 15:56:09.000000 mixprop-0.0.5/mixprop.egg-info/PKG-INFO
--rw-r--r--   0 cur5wz     (502) staff       (20)     1668 2023-06-15 15:56:10.000000 mixprop-0.0.5/mixprop.egg-info/SOURCES.txt
--rw-r--r--   0 cur5wz     (502) staff       (20)      133 2023-06-15 15:56:10.000000 mixprop-0.0.5/mixprop.egg-info/dependency_links.txt
--rw-r--r--   0 cur5wz     (502) staff       (20)        1 2023-06-14 15:18:23.000000 mixprop-0.0.5/mixprop.egg-info/not-zip-safe
--rw-r--r--   0 cur5wz     (502) staff       (20)      133 2023-06-15 15:56:10.000000 mixprop-0.0.5/mixprop.egg-info/requires.txt
--rw-r--r--   0 cur5wz     (502) staff       (20)        8 2023-06-15 15:56:10.000000 mixprop-0.0.5/mixprop.egg-info/top_level.txt
--rw-r--r--   0 cur5wz     (502) staff       (20)      132 2023-06-15 14:28:35.000000 mixprop-0.0.5/requirements.txt
--rw-r--r--   0 cur5wz     (502) staff       (20)      390 2023-06-15 15:56:10.281675 mixprop-0.0.5/setup.cfg
--rw-r--r--   0 cur5wz     (502) staff       (20)     1723 2023-06-15 15:55:34.000000 mixprop-0.0.5/setup.py
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 15:56:10.280387 mixprop-0.0.5/tests/
--rw-r--r--   0 cur5wz     (502) staff       (20)      387 2023-06-14 17:36:41.000000 mixprop-0.0.5/tests/test_mixprop.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 18:08:13.000000 mixprop-0.0.6/
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1075 2023-06-14 17:36:40.000000 mixprop-0.0.6/LICENSE
+-rw-r--r--   0 cur5wz     (502) staff       (20)      122 2023-06-14 17:36:40.000000 mixprop-0.0.6/MANIFEST.in
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1129 2023-06-15 18:08:13.000000 mixprop-0.0.6/PKG-INFO
+-rw-r--r--   0 cur5wz     (502) staff       (20)      385 2023-06-14 17:36:40.000000 mixprop-0.0.6/README.md
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 18:08:13.000000 mixprop-0.0.6/mixprop/
+-rw-r--r--   0 cur5wz     (502) staff       (20)      428 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/__init__.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)      196 2023-06-15 18:06:13.000000 mixprop-0.0.6/mixprop/_version.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    43236 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/args.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)      233 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/constants.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 18:08:13.000000 mixprop-0.0.6/mixprop/curation_pipeline/
+-rw-r--r--   0 cur5wz     (502) staff       (20)     3006 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/curation_pipeline/T_logV_correlation.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)        1 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/curation_pipeline/__init__.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1884 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/curation_pipeline/load_data.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     5105 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/curation_pipeline/pchip_interpolation.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     4412 2023-06-15 17:40:14.000000 mixprop-0.0.6/mixprop/curation_pipeline/pipeline.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     4326 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/curation_pipeline/remove_inconsistent.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1334 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/curation_pipeline/remove_not_liquid.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)      472 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/curation_pipeline/remove_salts.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     2197 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/curation_pipeline/split_data.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     3713 2023-06-15 17:49:48.000000 mixprop-0.0.6/mixprop/curation_pipeline/utils.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1480 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/curation_pipeline/write_data.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 18:08:13.000000 mixprop-0.0.6/mixprop/data/
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1276 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/data/__init__.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    32394 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/data/data.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     7839 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/data/scaffold.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     2791 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/data/scaler.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    32574 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/data/utils.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 18:08:13.000000 mixprop-0.0.6/mixprop/features/
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1393 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/features/__init__.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     6219 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/features/features_generators.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    31849 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/features/featurization.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     4085 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/features/utils.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     7860 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/hyperopt_utils.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     6909 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/hyperparameter_optimization.py
+-rwxr-xr-x   0 cur5wz     (502) staff       (20)    13820 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/interpret.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 18:08:13.000000 mixprop-0.0.6/mixprop/models/
+-rw-r--r--   0 cur5wz     (502) staff       (20)      130 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/models/__init__.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    14231 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/models/model.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    15153 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/models/mpn.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     7788 2023-06-14 17:36:40.000000 mixprop-0.0.6/mixprop/nn_utils.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)      636 2023-06-14 17:36:41.000000 mixprop-0.0.6/mixprop/rdkit.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     3025 2023-06-14 17:36:41.000000 mixprop-0.0.6/mixprop/sklearn_predict.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    14923 2023-06-14 17:36:41.000000 mixprop-0.0.6/mixprop/sklearn_train.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     5245 2023-06-14 17:36:41.000000 mixprop-0.0.6/mixprop/spectra_utils.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 18:08:13.000000 mixprop-0.0.6/mixprop/train/
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1285 2023-06-14 17:36:41.000000 mixprop-0.0.6/mixprop/train/__init__.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     8013 2023-06-14 17:36:41.000000 mixprop-0.0.6/mixprop/train/cross_validate.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     5868 2023-06-14 17:36:41.000000 mixprop-0.0.6/mixprop/train/evaluate.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     9575 2023-06-14 17:36:41.000000 mixprop-0.0.6/mixprop/train/loss_functions.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    15630 2023-06-14 17:36:41.000000 mixprop-0.0.6/mixprop/train/make_predictions.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    13018 2023-06-14 17:36:41.000000 mixprop-0.0.6/mixprop/train/metrics.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     9771 2023-06-14 17:36:41.000000 mixprop-0.0.6/mixprop/train/molecule_fingerprint.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1795 2023-06-14 17:36:41.000000 mixprop-0.0.6/mixprop/train/predict.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    16099 2023-06-14 17:36:41.000000 mixprop-0.0.6/mixprop/train/run_training.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     6150 2023-06-14 17:36:41.000000 mixprop-0.0.6/mixprop/train/train.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    30646 2023-06-14 17:36:41.000000 mixprop-0.0.6/mixprop/utils.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     6070 2023-06-15 17:29:28.000000 mixprop-0.0.6/mixprop/visc_pred_wrapper.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 18:08:13.000000 mixprop-0.0.6/mixprop.egg-info/
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1129 2023-06-15 18:08:12.000000 mixprop-0.0.6/mixprop.egg-info/PKG-INFO
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1668 2023-06-15 18:08:12.000000 mixprop-0.0.6/mixprop.egg-info/SOURCES.txt
+-rw-r--r--   0 cur5wz     (502) staff       (20)      133 2023-06-15 18:08:12.000000 mixprop-0.0.6/mixprop.egg-info/dependency_links.txt
+-rw-r--r--   0 cur5wz     (502) staff       (20)        1 2023-06-14 15:18:23.000000 mixprop-0.0.6/mixprop.egg-info/not-zip-safe
+-rw-r--r--   0 cur5wz     (502) staff       (20)      133 2023-06-15 18:08:12.000000 mixprop-0.0.6/mixprop.egg-info/requires.txt
+-rw-r--r--   0 cur5wz     (502) staff       (20)        8 2023-06-15 18:08:12.000000 mixprop-0.0.6/mixprop.egg-info/top_level.txt
+-rw-r--r--   0 cur5wz     (502) staff       (20)      132 2023-06-15 14:28:35.000000 mixprop-0.0.6/requirements.txt
+-rw-r--r--   0 cur5wz     (502) staff       (20)      390 2023-06-15 18:08:13.000000 mixprop-0.0.6/setup.cfg
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1723 2023-06-15 18:05:52.000000 mixprop-0.0.6/setup.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 18:08:13.000000 mixprop-0.0.6/tests/
+-rw-r--r--   0 cur5wz     (502) staff       (20)      387 2023-06-14 17:36:41.000000 mixprop-0.0.6/tests/test_mixprop.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `mixprop-0.0.5/LICENSE` & `mixprop-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/PKG-INFO` & `mixprop-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixprop
-Version: 0.0.5
+Version: 0.0.6
 Summary: Viscosity prediction for binary liquid mixtures
 Home-page: https://github.com/cbilodeau2/mixprop_viscosity
 Author: Camille Bilodeau
 Author-email: camille79bilodeau@gmail.com
 License: MIT license
 Keywords: mixprop
 Classifier: Intended Audience :: Developers
```

### Comparing `mixprop-0.0.5/mixprop/args.py` & `mixprop-0.0.6/mixprop/args.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/curation_pipeline/T_logV_correlation.py` & `mixprop-0.0.6/mixprop/curation_pipeline/T_logV_correlation.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/curation_pipeline/load_data.py` & `mixprop-0.0.6/mixprop/curation_pipeline/load_data.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/curation_pipeline/pchip_interpolation.py` & `mixprop-0.0.6/mixprop/curation_pipeline/pchip_interpolation.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/curation_pipeline/pipeline.py` & `mixprop-0.0.6/mixprop/curation_pipeline/pipeline.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,38 +54,39 @@
     print("Total Time Elapsed: {}".format(time.time() - start))
 
     print("Writing Dataset to {}: ---".format(input_args["out_path"]))
     write_data(nist_knovel_all, test_mols, input_args)
 
     print("Total Time Elapsed: {:.2f}".format(time.time() - start))
 
-def load_model(args):
-    if 'checkpoint_dir' in args.keys():
-        return mixprop_model(args['checkpoint_dir'])
-    else:
-        path = str(Path(__file__).absolute())
-        path = '/'.join(path.split('/')[:-1])
-        checkpoint_dir = os.path.join(path,'pretrained_models/nist_dippr_model/nist_dippr_model')
+# def load_model(args):
+#     if 'checkpoint_dir' in args.keys():
+#         return mixprop_model(args['checkpoint_dir'])
+#     else:
+#         path = str(Path(__file__).absolute())
+#         path = '/'.join(path.split('/')[:-1])
+#         checkpoint_dir = os.path.join(path,'pretrained_models/nist_dippr_model/nist_dippr_model')
         
-        print('Loading models from {}'.format(checkpoint_dir))
+#         print('Loading models from {}'.format(checkpoint_dir))
         
-        return mixprop_model(checkpoint_dir)
+#         return mixprop_model(checkpoint_dir)
+
+# curation_args = {
+#     "NIST": "pretrained_models/nist_dippr_source/NIST_Visc_Data.csv",  # Path to NIST data
+#     "DIPPR": "pretrained_models/nist_dippr_source/logV_bp_mp.csv",  # Path to DIPPR data
+#     "bp_pred_path": "pretrained_models/bp_data/bp_pred.csv",  # Path to boiling point data (already predicted)
+#     "mp_pred_path": "pretrained_models/mp_data/mp_pred.csv",  # Path to melting point data (already predicted)
+#     "dummy_mol": "CCO",  # Dummy compound for mixing in DIPPR pure component data
+#     "dippr_ref_T": 298,  # DIPPR temperature
+#     "test_split": 0.2,  # Fraction to hold out for testing
+#     "thresh_pure": 0.025,  # Settings for inconsistent pure data screening
+#     "thresh_logV": 0.5,  # Settings for inconsistent pure data screening
+#     "out_path":"." # Location for files to be written to
+# }
 
-curation_args = {
-    "NIST": "pretrained_models/nist_dippr_source/NIST_Visc_Data.csv",  # Path to NIST data
-    "DIPPR": "pretrained_models/nist_dippr_source/logV_bp_mp.csv",  # Path to DIPPR data
-    "bp_pred_path": "pretrained_models/bp_data/bp_pred.csv",  # Path to boiling point data (already predicted)
-    "mp_pred_path": "pretrained_models/mp_data/mp_pred.csv",  # Path to melting point data (already predicted)
-    "dummy_mol": "CCO",  # Dummy compound for mixing in DIPPR pure component data
-    "dippr_ref_T": 298,  # DIPPR temperature
-    "test_split": 0.2,  # Fraction to hold out for testing
-    "thresh_pure": 0.025,  # Settings for inconsistent pure data screening
-    "thresh_logV": 0.5,  # Settings for inconsistent pure data screening
-    "out_path":"." # Location for files to be written to
-}
 def add_paths_to_args(args):
     path = str(Path(__file__).absolute())
     path = '/'.join(path.split('/')[:-2])
     source_path = os.path.join(path,'pretrained_models')
 
     if 'NIST' not in args.keys():
         nist_path = os.path.join(source_path,'nist_dippr_source/NIST_Visc_Data.csv')
```

### Comparing `mixprop-0.0.5/mixprop/curation_pipeline/remove_inconsistent.py` & `mixprop-0.0.6/mixprop/curation_pipeline/remove_inconsistent.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/curation_pipeline/remove_not_liquid.py` & `mixprop-0.0.6/mixprop/curation_pipeline/remove_not_liquid.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/curation_pipeline/split_data.py` & `mixprop-0.0.6/mixprop/curation_pipeline/split_data.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/curation_pipeline/utils.py` & `mixprop-0.0.6/mixprop/curation_pipeline/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,16 @@
     """
     Prints the number of molecules/datapoints in the test and training sets.
     
     nist_knovel_all: pandas dataframe containing the dataset
     test_mols: list containing compounds to held out of the training set and assigned to the test set    
     """
 
+    nist_knovel_all = nist_knovel_all.drop(columns=["ID_1","ID_2","Ref_ID"])
+
     # Average over all data that looks like duplicates before checkpointing
     nist_knovel_all_nodup = nist_knovel_all.groupby(
         ["MOL_1", "MOL_2", "MolFrac_1"]
     ).mean()
     nist_knovel_all_nodup.reset_index(inplace=True)
 
     nist_knovel_all_nodup["test_1"] = nist_knovel_all_nodup["MOL_1"].apply(
```

### Comparing `mixprop-0.0.5/mixprop/curation_pipeline/write_data.py` & `mixprop-0.0.6/mixprop/curation_pipeline/write_data.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/data/__init__.py` & `mixprop-0.0.6/mixprop/data/__init__.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/data/data.py` & `mixprop-0.0.6/mixprop/data/data.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/data/scaffold.py` & `mixprop-0.0.6/mixprop/data/scaffold.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/data/scaler.py` & `mixprop-0.0.6/mixprop/data/scaler.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/data/utils.py` & `mixprop-0.0.6/mixprop/data/utils.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/features/__init__.py` & `mixprop-0.0.6/mixprop/features/__init__.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/features/features_generators.py` & `mixprop-0.0.6/mixprop/features/features_generators.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/features/featurization.py` & `mixprop-0.0.6/mixprop/features/featurization.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/features/utils.py` & `mixprop-0.0.6/mixprop/features/utils.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/hyperopt_utils.py` & `mixprop-0.0.6/mixprop/hyperopt_utils.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/hyperparameter_optimization.py` & `mixprop-0.0.6/mixprop/hyperparameter_optimization.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/interpret.py` & `mixprop-0.0.6/mixprop/interpret.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/models/model.py` & `mixprop-0.0.6/mixprop/models/model.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/models/mpn.py` & `mixprop-0.0.6/mixprop/models/mpn.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/nn_utils.py` & `mixprop-0.0.6/mixprop/nn_utils.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/rdkit.py` & `mixprop-0.0.6/mixprop/rdkit.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/sklearn_predict.py` & `mixprop-0.0.6/mixprop/sklearn_predict.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/sklearn_train.py` & `mixprop-0.0.6/mixprop/sklearn_train.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/spectra_utils.py` & `mixprop-0.0.6/mixprop/spectra_utils.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/train/__init__.py` & `mixprop-0.0.6/mixprop/train/__init__.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/train/cross_validate.py` & `mixprop-0.0.6/mixprop/train/cross_validate.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/train/evaluate.py` & `mixprop-0.0.6/mixprop/train/evaluate.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/train/loss_functions.py` & `mixprop-0.0.6/mixprop/train/loss_functions.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/train/make_predictions.py` & `mixprop-0.0.6/mixprop/train/make_predictions.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/train/metrics.py` & `mixprop-0.0.6/mixprop/train/metrics.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/train/molecule_fingerprint.py` & `mixprop-0.0.6/mixprop/train/molecule_fingerprint.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/train/predict.py` & `mixprop-0.0.6/mixprop/train/predict.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/train/run_training.py` & `mixprop-0.0.6/mixprop/train/run_training.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/train/train.py` & `mixprop-0.0.6/mixprop/train/train.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/utils.py` & `mixprop-0.0.6/mixprop/utils.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/mixprop/visc_pred_wrapper.py` & `mixprop-0.0.6/mixprop/visc_pred_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,16 +74,16 @@
 
 
 def onepoint_assertions(args):
     
     # Requirements:
     assert type(args['smi1'])==str, 'Molecules need to be input as SMILES strings.'
     assert type(args['smi2'])==str, 'Molecules need to be input as SMILES strings.'
-    assert (type(args['T'])==float)|(type(args['T'])==int)|(type(args['T'])==np.int64)|(type(args['T'])==np.float), 'Temperature needs to be input as a number.'
-    assert (type(args['molfrac1'])==float)|(type(args['molfrac1'])==int)|(type(args['T'])==np.int64)|(type(args['T'])==np.float), 'Mole fraction needs to be input as a number.'
+    assert (type(args['T'])==float)|(type(args['T'])==int)|(type(args['T'])==np.int64)|(type(args['T'])==float), 'Temperature needs to be input as a number.'
+    assert (type(args['molfrac1'])==float)|(type(args['molfrac1'])==int)|(type(args['T'])==np.int64)|(type(args['T'])==float), 'Mole fraction needs to be input as a number.'
     
     assert (args['molfrac1']>=0.0)&(args['molfrac1']<=1.0), 'Mole fraction needs to be between 0 and 1.'
     
     mol1 = Chem.MolFromSmiles(args['smi1'])
     mol2 = Chem.MolFromSmiles(args['smi2'])
     assert type(mol1)==Chem.rdchem.Mol, 'Invalid SMILES entry, please check that your SMILES are valid.'
     assert type(mol2)==Chem.rdchem.Mol, 'Invalid SMILES entry, please check that your SMILES are valid.'
```

### Comparing `mixprop-0.0.5/mixprop.egg-info/PKG-INFO` & `mixprop-0.0.6/mixprop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixprop
-Version: 0.0.5
+Version: 0.0.6
 Summary: Viscosity prediction for binary liquid mixtures
 Home-page: https://github.com/cbilodeau2/mixprop_viscosity
 Author: Camille Bilodeau
 Author-email: camille79bilodeau@gmail.com
 License: MIT license
 Keywords: mixprop
 Classifier: Intended Audience :: Developers
```

### Comparing `mixprop-0.0.5/mixprop.egg-info/SOURCES.txt` & `mixprop-0.0.6/mixprop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.5/setup.py` & `mixprop-0.0.6/setup.py`

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
-    version='0.0.5',
+    version='0.0.6',
     zip_safe=False,
 )
```

