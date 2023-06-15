# Comparing `tmp/mixprop-0.0.2.tar.gz` & `tmp/mixprop-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixprop-0.0.2.tar", last modified: Wed Jun 14 15:33:03 2023, max compression
+gzip compressed data, was "mixprop-0.0.3.tar", last modified: Thu Jun 15 14:10:13 2023, max compression
```

## Comparing `mixprop-0.0.2.tar` & `mixprop-0.0.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-14 15:33:03.070280 mixprop-0.0.2/
--rw-r--r--   0 cur5wz     (502) staff       (20)     1075 2023-06-13 20:42:10.000000 mixprop-0.0.2/LICENSE
--rw-r--r--   0 cur5wz     (502) staff       (20)      122 2023-06-13 20:42:10.000000 mixprop-0.0.2/MANIFEST.in
--rw-r--r--   0 cur5wz     (502) staff       (20)     1119 2023-06-14 15:33:03.070423 mixprop-0.0.2/PKG-INFO
--rw-r--r--   0 cur5wz     (502) staff       (20)      385 2023-06-13 20:42:10.000000 mixprop-0.0.2/README.md
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-14 15:33:03.027626 mixprop-0.0.2/mixprop/
--rw-r--r--   0 cur5wz     (502) staff       (20)      428 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/__init__.py
--rw-r--r--   0 cur5wz     (502) staff       (20)      196 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/_version.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    43236 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/args.py
--rw-r--r--   0 cur5wz     (502) staff       (20)      233 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/constants.py
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-14 15:33:03.043800 mixprop-0.0.2/mixprop/curation_pipeline/
--rw-r--r--   0 cur5wz     (502) staff       (20)     3006 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/curation_pipeline/T_logV_correlation.py
--rw-r--r--   0 cur5wz     (502) staff       (20)        1 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/curation_pipeline/__init__.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     1884 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/curation_pipeline/load_data.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     5105 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/curation_pipeline/pchip_interpolation.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     4369 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/curation_pipeline/pipeline.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     4326 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/curation_pipeline/remove_inconsistent.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     1334 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/curation_pipeline/remove_not_liquid.py
--rw-r--r--   0 cur5wz     (502) staff       (20)      472 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/curation_pipeline/remove_salts.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     2197 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/curation_pipeline/split_data.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     3635 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/curation_pipeline/utils.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     1480 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/curation_pipeline/write_data.py
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-14 15:33:03.048032 mixprop-0.0.2/mixprop/data/
--rw-r--r--   0 cur5wz     (502) staff       (20)     1276 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/data/__init__.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    32394 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/data/data.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     7839 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/data/scaffold.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     2791 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/data/scaler.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    32574 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/data/utils.py
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-14 15:33:03.051190 mixprop-0.0.2/mixprop/features/
--rw-r--r--   0 cur5wz     (502) staff       (20)     1393 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/features/__init__.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     6219 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/features/features_generators.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    31849 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/features/featurization.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     4085 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/features/utils.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     7860 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/hyperopt_utils.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     6909 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/hyperparameter_optimization.py
--rwxr-xr-x   0 cur5wz     (502) staff       (20)    13820 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/interpret.py
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-14 15:33:03.053464 mixprop-0.0.2/mixprop/models/
--rw-r--r--   0 cur5wz     (502) staff       (20)      130 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/models/__init__.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    14231 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/models/model.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    15153 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/models/mpn.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     7788 2023-06-14 14:29:57.000000 mixprop-0.0.2/mixprop/nn_utils.py
--rw-r--r--   0 cur5wz     (502) staff       (20)      636 2023-06-14 14:29:59.000000 mixprop-0.0.2/mixprop/rdkit.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     3025 2023-06-14 14:29:59.000000 mixprop-0.0.2/mixprop/sklearn_predict.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    14923 2023-06-14 14:29:59.000000 mixprop-0.0.2/mixprop/sklearn_train.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     5245 2023-06-14 14:29:59.000000 mixprop-0.0.2/mixprop/spectra_utils.py
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-14 15:33:03.068719 mixprop-0.0.2/mixprop/train/
--rw-r--r--   0 cur5wz     (502) staff       (20)     1285 2023-06-14 14:29:59.000000 mixprop-0.0.2/mixprop/train/__init__.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     8013 2023-06-14 14:29:59.000000 mixprop-0.0.2/mixprop/train/cross_validate.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     5868 2023-06-14 14:29:59.000000 mixprop-0.0.2/mixprop/train/evaluate.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     9575 2023-06-14 14:29:59.000000 mixprop-0.0.2/mixprop/train/loss_functions.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    15630 2023-06-14 14:29:59.000000 mixprop-0.0.2/mixprop/train/make_predictions.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    13018 2023-06-14 14:29:59.000000 mixprop-0.0.2/mixprop/train/metrics.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     9771 2023-06-14 14:29:59.000000 mixprop-0.0.2/mixprop/train/molecule_fingerprint.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     1795 2023-06-14 14:29:59.000000 mixprop-0.0.2/mixprop/train/predict.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    16099 2023-06-14 14:29:59.000000 mixprop-0.0.2/mixprop/train/run_training.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     6150 2023-06-14 14:29:59.000000 mixprop-0.0.2/mixprop/train/train.py
--rw-r--r--   0 cur5wz     (502) staff       (20)    30646 2023-06-14 14:29:59.000000 mixprop-0.0.2/mixprop/utils.py
--rw-r--r--   0 cur5wz     (502) staff       (20)     5859 2023-06-14 14:29:59.000000 mixprop-0.0.2/mixprop/visc_pred_wrapper.py
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-14 15:33:03.033307 mixprop-0.0.2/mixprop.egg-info/
--rw-r--r--   0 cur5wz     (502) staff       (20)     1119 2023-06-14 15:33:02.000000 mixprop-0.0.2/mixprop.egg-info/PKG-INFO
--rw-r--r--   0 cur5wz     (502) staff       (20)     1668 2023-06-14 15:33:02.000000 mixprop-0.0.2/mixprop.egg-info/SOURCES.txt
--rw-r--r--   0 cur5wz     (502) staff       (20)      122 2023-06-14 15:33:02.000000 mixprop-0.0.2/mixprop.egg-info/dependency_links.txt
--rw-r--r--   0 cur5wz     (502) staff       (20)        1 2023-06-14 15:18:23.000000 mixprop-0.0.2/mixprop.egg-info/not-zip-safe
--rw-r--r--   0 cur5wz     (502) staff       (20)      122 2023-06-14 15:33:02.000000 mixprop-0.0.2/mixprop.egg-info/requires.txt
--rw-r--r--   0 cur5wz     (502) staff       (20)        8 2023-06-14 15:33:02.000000 mixprop-0.0.2/mixprop.egg-info/top_level.txt
--rw-r--r--   0 cur5wz     (502) staff       (20)      121 2023-06-14 15:28:32.000000 mixprop-0.0.2/requirements.txt
--rw-r--r--   0 cur5wz     (502) staff       (20)      390 2023-06-14 15:33:03.071201 mixprop-0.0.2/setup.cfg
--rw-r--r--   0 cur5wz     (502) staff       (20)     1713 2023-06-14 15:32:52.000000 mixprop-0.0.2/setup.py
-drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-14 15:33:03.069784 mixprop-0.0.2/tests/
--rw-r--r--   0 cur5wz     (502) staff       (20)      387 2023-06-13 20:42:10.000000 mixprop-0.0.2/tests/test_mixprop.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 14:10:13.780224 mixprop-0.0.3/
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1075 2023-06-14 17:36:40.000000 mixprop-0.0.3/LICENSE
+-rw-r--r--   0 cur5wz     (502) staff       (20)      122 2023-06-14 17:36:40.000000 mixprop-0.0.3/MANIFEST.in
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1129 2023-06-15 14:10:13.780534 mixprop-0.0.3/PKG-INFO
+-rw-r--r--   0 cur5wz     (502) staff       (20)      385 2023-06-14 17:36:40.000000 mixprop-0.0.3/README.md
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 14:10:13.631702 mixprop-0.0.3/mixprop/
+-rw-r--r--   0 cur5wz     (502) staff       (20)      428 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/__init__.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)      196 2023-06-15 14:08:53.000000 mixprop-0.0.3/mixprop/_version.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    43236 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/args.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)      233 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/constants.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 14:10:13.678251 mixprop-0.0.3/mixprop/curation_pipeline/
+-rw-r--r--   0 cur5wz     (502) staff       (20)     3006 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/curation_pipeline/T_logV_correlation.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)        1 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/curation_pipeline/__init__.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1884 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/curation_pipeline/load_data.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     5105 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/curation_pipeline/pchip_interpolation.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     4369 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/curation_pipeline/pipeline.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     4326 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/curation_pipeline/remove_inconsistent.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1334 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/curation_pipeline/remove_not_liquid.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)      472 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/curation_pipeline/remove_salts.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     2197 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/curation_pipeline/split_data.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     3635 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/curation_pipeline/utils.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1480 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/curation_pipeline/write_data.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 14:10:13.700016 mixprop-0.0.3/mixprop/data/
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1276 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/data/__init__.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    32394 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/data/data.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     7839 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/data/scaffold.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     2791 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/data/scaler.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    32574 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/data/utils.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 14:10:13.720604 mixprop-0.0.3/mixprop/features/
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1393 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/features/__init__.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     6219 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/features/features_generators.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    31849 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/features/featurization.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     4085 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/features/utils.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     7860 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/hyperopt_utils.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     6909 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/hyperparameter_optimization.py
+-rwxr-xr-x   0 cur5wz     (502) staff       (20)    13820 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/interpret.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 14:10:13.734435 mixprop-0.0.3/mixprop/models/
+-rw-r--r--   0 cur5wz     (502) staff       (20)      130 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/models/__init__.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    14231 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/models/model.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    15153 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/models/mpn.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     7788 2023-06-14 17:36:40.000000 mixprop-0.0.3/mixprop/nn_utils.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)      636 2023-06-14 17:36:41.000000 mixprop-0.0.3/mixprop/rdkit.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     3025 2023-06-14 17:36:41.000000 mixprop-0.0.3/mixprop/sklearn_predict.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    14923 2023-06-14 17:36:41.000000 mixprop-0.0.3/mixprop/sklearn_train.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     5245 2023-06-14 17:36:41.000000 mixprop-0.0.3/mixprop/spectra_utils.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 14:10:13.776015 mixprop-0.0.3/mixprop/train/
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1285 2023-06-14 17:36:41.000000 mixprop-0.0.3/mixprop/train/__init__.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     8013 2023-06-14 17:36:41.000000 mixprop-0.0.3/mixprop/train/cross_validate.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     5868 2023-06-14 17:36:41.000000 mixprop-0.0.3/mixprop/train/evaluate.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     9575 2023-06-14 17:36:41.000000 mixprop-0.0.3/mixprop/train/loss_functions.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    15630 2023-06-14 17:36:41.000000 mixprop-0.0.3/mixprop/train/make_predictions.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    13018 2023-06-14 17:36:41.000000 mixprop-0.0.3/mixprop/train/metrics.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     9771 2023-06-14 17:36:41.000000 mixprop-0.0.3/mixprop/train/molecule_fingerprint.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1795 2023-06-14 17:36:41.000000 mixprop-0.0.3/mixprop/train/predict.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    16099 2023-06-14 17:36:41.000000 mixprop-0.0.3/mixprop/train/run_training.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     6150 2023-06-14 17:36:41.000000 mixprop-0.0.3/mixprop/train/train.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)    30646 2023-06-14 17:36:41.000000 mixprop-0.0.3/mixprop/utils.py
+-rw-r--r--   0 cur5wz     (502) staff       (20)     5859 2023-06-14 17:36:41.000000 mixprop-0.0.3/mixprop/visc_pred_wrapper.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 14:10:13.638613 mixprop-0.0.3/mixprop.egg-info/
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1129 2023-06-15 14:10:12.000000 mixprop-0.0.3/mixprop.egg-info/PKG-INFO
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1668 2023-06-15 14:10:13.000000 mixprop-0.0.3/mixprop.egg-info/SOURCES.txt
+-rw-r--r--   0 cur5wz     (502) staff       (20)      133 2023-06-15 14:10:12.000000 mixprop-0.0.3/mixprop.egg-info/dependency_links.txt
+-rw-r--r--   0 cur5wz     (502) staff       (20)        1 2023-06-14 15:18:23.000000 mixprop-0.0.3/mixprop.egg-info/not-zip-safe
+-rw-r--r--   0 cur5wz     (502) staff       (20)      133 2023-06-15 14:10:12.000000 mixprop-0.0.3/mixprop.egg-info/requires.txt
+-rw-r--r--   0 cur5wz     (502) staff       (20)        8 2023-06-15 14:10:12.000000 mixprop-0.0.3/mixprop.egg-info/top_level.txt
+-rw-r--r--   0 cur5wz     (502) staff       (20)      132 2023-06-15 14:05:33.000000 mixprop-0.0.3/requirements.txt
+-rw-r--r--   0 cur5wz     (502) staff       (20)      390 2023-06-15 14:10:13.784623 mixprop-0.0.3/setup.cfg
+-rw-r--r--   0 cur5wz     (502) staff       (20)     1723 2023-06-15 12:48:33.000000 mixprop-0.0.3/setup.py
+drwxr-xr-x   0 cur5wz     (502) staff       (20)        0 2023-06-15 14:10:13.779130 mixprop-0.0.3/tests/
+-rw-r--r--   0 cur5wz     (502) staff       (20)      387 2023-06-14 17:36:41.000000 mixprop-0.0.3/tests/test_mixprop.py
```

### Comparing `mixprop-0.0.2/LICENSE` & `mixprop-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/PKG-INFO` & `mixprop-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mixprop
-Version: 0.0.2
+Version: 0.0.3
 Summary: Viscosity prediction for binary liquid mixtures
-Home-page: https://github.com/cbilodeau2/mixprop
+Home-page: https://github.com/cbilodeau2/mixprop_viscosity
 Author: Camille Bilodeau
 Author-email: camille79bilodeau@gmail.com
 License: MIT license
 Keywords: mixprop
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `mixprop-0.0.2/mixprop/args.py` & `mixprop-0.0.3/mixprop/args.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/curation_pipeline/T_logV_correlation.py` & `mixprop-0.0.3/mixprop/curation_pipeline/T_logV_correlation.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/curation_pipeline/load_data.py` & `mixprop-0.0.3/mixprop/curation_pipeline/load_data.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/curation_pipeline/pchip_interpolation.py` & `mixprop-0.0.3/mixprop/curation_pipeline/pchip_interpolation.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/curation_pipeline/pipeline.py` & `mixprop-0.0.3/mixprop/curation_pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/curation_pipeline/remove_inconsistent.py` & `mixprop-0.0.3/mixprop/curation_pipeline/remove_inconsistent.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/curation_pipeline/remove_not_liquid.py` & `mixprop-0.0.3/mixprop/curation_pipeline/remove_not_liquid.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/curation_pipeline/split_data.py` & `mixprop-0.0.3/mixprop/curation_pipeline/split_data.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/curation_pipeline/utils.py` & `mixprop-0.0.3/mixprop/curation_pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/curation_pipeline/write_data.py` & `mixprop-0.0.3/mixprop/curation_pipeline/write_data.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/data/__init__.py` & `mixprop-0.0.3/mixprop/data/__init__.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/data/data.py` & `mixprop-0.0.3/mixprop/data/data.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/data/scaffold.py` & `mixprop-0.0.3/mixprop/data/scaffold.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/data/scaler.py` & `mixprop-0.0.3/mixprop/data/scaler.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/data/utils.py` & `mixprop-0.0.3/mixprop/data/utils.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/features/__init__.py` & `mixprop-0.0.3/mixprop/features/__init__.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/features/features_generators.py` & `mixprop-0.0.3/mixprop/features/features_generators.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/features/featurization.py` & `mixprop-0.0.3/mixprop/features/featurization.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/features/utils.py` & `mixprop-0.0.3/mixprop/features/utils.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/hyperopt_utils.py` & `mixprop-0.0.3/mixprop/hyperopt_utils.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/hyperparameter_optimization.py` & `mixprop-0.0.3/mixprop/hyperparameter_optimization.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/interpret.py` & `mixprop-0.0.3/mixprop/interpret.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/models/model.py` & `mixprop-0.0.3/mixprop/models/model.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/models/mpn.py` & `mixprop-0.0.3/mixprop/models/mpn.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/nn_utils.py` & `mixprop-0.0.3/mixprop/nn_utils.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/rdkit.py` & `mixprop-0.0.3/mixprop/rdkit.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/sklearn_predict.py` & `mixprop-0.0.3/mixprop/sklearn_predict.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/sklearn_train.py` & `mixprop-0.0.3/mixprop/sklearn_train.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/spectra_utils.py` & `mixprop-0.0.3/mixprop/spectra_utils.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/train/__init__.py` & `mixprop-0.0.3/mixprop/train/__init__.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/train/cross_validate.py` & `mixprop-0.0.3/mixprop/train/cross_validate.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/train/evaluate.py` & `mixprop-0.0.3/mixprop/train/evaluate.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/train/loss_functions.py` & `mixprop-0.0.3/mixprop/train/loss_functions.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/train/make_predictions.py` & `mixprop-0.0.3/mixprop/train/make_predictions.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/train/metrics.py` & `mixprop-0.0.3/mixprop/train/metrics.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/train/molecule_fingerprint.py` & `mixprop-0.0.3/mixprop/train/molecule_fingerprint.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/train/predict.py` & `mixprop-0.0.3/mixprop/train/predict.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/train/run_training.py` & `mixprop-0.0.3/mixprop/train/run_training.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/train/train.py` & `mixprop-0.0.3/mixprop/train/train.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/utils.py` & `mixprop-0.0.3/mixprop/utils.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop/visc_pred_wrapper.py` & `mixprop-0.0.3/mixprop/visc_pred_wrapper.py`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/mixprop.egg-info/PKG-INFO` & `mixprop-0.0.3/mixprop.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mixprop
-Version: 0.0.2
+Version: 0.0.3
 Summary: Viscosity prediction for binary liquid mixtures
-Home-page: https://github.com/cbilodeau2/mixprop
+Home-page: https://github.com/cbilodeau2/mixprop_viscosity
 Author: Camille Bilodeau
 Author-email: camille79bilodeau@gmail.com
 License: MIT license
 Keywords: mixprop
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `mixprop-0.0.2/mixprop.egg-info/SOURCES.txt` & `mixprop-0.0.3/mixprop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mixprop-0.0.2/setup.py` & `mixprop-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,11 +47,11 @@
     include_package_data=True,
     keywords='mixprop',
     name='mixprop',
     packages=find_packages(include=['mixprop', 'mixprop.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
-    url='https://github.com/cbilodeau2/mixprop',
-    version='0.0.2',
+    url='https://github.com/cbilodeau2/mixprop_viscosity',
+    version='0.0.3',
     zip_safe=False,
 )
```

