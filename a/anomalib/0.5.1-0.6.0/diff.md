# Comparing `tmp/anomalib-0.5.1.tar.gz` & `tmp/anomalib-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anomalib-0.5.1.tar", last modified: Wed May 24 14:43:06 2023, max compression
+gzip compressed data, was "anomalib-0.6.0.tar", last modified: Thu Jun 15 14:32:21 2023, max compression
```

## Comparing `anomalib-0.5.1.tar` & `anomalib-0.6.0.tar`

### file list

```diff
@@ -1,280 +1,285 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.741655 anomalib-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-24 14:42:52.000000 anomalib-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       98 2023-05-24 14:42:52.000000 anomalib-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    24127 2023-05-24 14:43:06.741655 anomalib-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    23625 2023-05-24 14:42:52.000000 anomalib-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     2968 2023-05-24 14:42:53.000000 anomalib-0.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.705659 anomalib-0.5.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-05-24 14:42:53.000000 anomalib-0.5.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-05-24 14:42:53.000000 anomalib-0.5.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-24 14:42:53.000000 anomalib-0.5.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-24 14:42:53.000000 anomalib-0.5.1/requirements/loggers.txt
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-24 14:42:53.000000 anomalib-0.5.1/requirements/notebooks.txt
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-24 14:42:53.000000 anomalib-0.5.1/requirements/openvino.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-24 14:43:06.741655 anomalib-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-05-24 14:42:53.000000 anomalib-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.701659 anomalib-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.705659 anomalib-0.5.1/src/anomalib/
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.709658 anomalib-0.5.1/src/anomalib/config/
--rw-r--r--   0 runner    (1001) docker     (122)      332 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13768 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.709658 anomalib-0.5.1/src/anomalib/data/
--rw-r--r--   0 runner    (1001) docker     (122)    11412 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12710 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/avenue.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.713658 anomalib-0.5.1/src/anomalib/data/base/
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8134 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/base/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (122)     7327 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/base/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2540 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/base/depth.py
--rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/base/video.py
--rw-r--r--   0 runner    (1001) docker     (122)    12043 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/btech.py
--rw-r--r--   0 runner    (1001) docker     (122)    12955 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/folder.py
--rw-r--r--   0 runner    (1001) docker     (122)    17503 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/folder_3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/inference.py
--rw-r--r--   0 runner    (1001) docker     (122)    11448 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/kolektor.py
--rw-r--r--   0 runner    (1001) docker     (122)    11831 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/mvtec.py
--rw-r--r--   0 runner    (1001) docker     (122)    12984 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/mvtec_3d.py
--rw-r--r--   0 runner    (1001) docker     (122)    14449 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/shanghaitech.py
--rw-r--r--   0 runner    (1001) docker     (122)     6941 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/task_type.py
--rw-r--r--   0 runner    (1001) docker     (122)    11770 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/ucsd_ped.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.713658 anomalib-0.5.1/src/anomalib/data/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6761 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/augmenter.py
--rw-r--r--   0 runner    (1001) docker     (122)     5077 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/boxes.py
--rw-r--r--   0 runner    (1001) docker     (122)    14453 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/download.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.713658 anomalib-0.5.1/src/anomalib/data/utils/generators/
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6027 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/generators/perlin.py
--rw-r--r--   0 runner    (1001) docker     (122)     8113 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/label.py
--rw-r--r--   0 runner    (1001) docker     (122)     2804 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (122)     4870 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/split.py
--rw-r--r--   0 runner    (1001) docker     (122)     5861 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/transform.py
--rw-r--r--   0 runner    (1001) docker     (122)     3651 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/utils/video.py
--rw-r--r--   0 runner    (1001) docker     (122)     9615 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/data/visa.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.713658 anomalib-0.5.1/src/anomalib/deploy/
--rw-r--r--   0 runner    (1001) docker     (122)      437 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5674 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/deploy/export.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.713658 anomalib-0.5.1/src/anomalib/deploy/inferencers/
--rw-r--r--   0 runner    (1001) docker     (122)      326 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/deploy/inferencers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7184 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/deploy/inferencers/base_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (122)     7903 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/deploy/inferencers/openvino_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/deploy/inferencers/torch_inferencer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.713658 anomalib-0.5.1/src/anomalib/models/
--rw-r--r--   0 runner    (1001) docker     (122)     2911 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.717657 anomalib-0.5.1/src/anomalib/models/ai_vad/
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.717657 anomalib-0.5.1/src/anomalib/models/ai_vad/clip/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/clip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7865 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/clip/clip.py
--rw-r--r--   0 runner    (1001) docker     (122)    17868 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/clip/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2922 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    11997 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/density.py
--rw-r--r--   0 runner    (1001) docker     (122)     9489 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/features.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/flow.py
--rw-r--r--   0 runner    (1001) docker     (122)     4699 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1168 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/regions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4331 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ai_vad/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.717657 anomalib-0.5.1/src/anomalib/models/cfa/
--rw-r--r--   0 runner    (1001) docker     (122)      335 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2762 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cfa/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     3059 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cfa/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     5766 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cfa/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1599 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cfa/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)    13213 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cfa/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.717657 anomalib-0.5.1/src/anomalib/models/cflow/
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cflow/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     3154 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cflow/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     8299 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cflow/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     5230 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cflow/torch_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     4179 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/cflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.717657 anomalib-0.5.1/src/anomalib/models/components/
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.717657 anomalib-0.5.1/src/anomalib/models/components/base/
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10187 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/base/anomaly_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/base/dynamic_module.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.717657 anomalib-0.5.1/src/anomalib/models/components/classification/
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5904 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/classification/kde_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.721657 anomalib-0.5.1/src/anomalib/models/components/dimensionality_reduction/
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/dimensionality_reduction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3307 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/dimensionality_reduction/pca.py
--rw-r--r--   0 runner    (1001) docker     (122)     5337 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/dimensionality_reduction/random_projection.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.721657 anomalib-0.5.1/src/anomalib/models/components/feature_extractors/
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/feature_extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4104 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/feature_extractors/timm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9158 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/feature_extractors/torchfx.py
--rw-r--r--   0 runner    (1001) docker     (122)      960 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/feature_extractors/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.721657 anomalib-0.5.1/src/anomalib/models/components/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3553 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/filters/blur.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.721657 anomalib-0.5.1/src/anomalib/models/components/flow/
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12649 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/flow/all_in_one_block.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.721657 anomalib-0.5.1/src/anomalib/models/components/layers/
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3143 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/layers/sspcab.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.721657 anomalib-0.5.1/src/anomalib/models/components/sampling/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/sampling/k_center_greedy.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.721657 anomalib-0.5.1/src/anomalib/models/components/stats/
--rw-r--r--   0 runner    (1001) docker     (122)      245 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2776 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/stats/kde.py
--rw-r--r--   0 runner    (1001) docker     (122)     5603 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/components/stats/multi_variate_gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.721657 anomalib-0.5.1/src/anomalib/models/csflow/
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/csflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/csflow/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/csflow/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4772 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/csflow/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/csflow/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)    21233 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/csflow/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.721657 anomalib-0.5.1/src/anomalib/models/dfkde/
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/dfkde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/dfkde/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4824 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/dfkde/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3052 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/dfkde/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.725657 anomalib-0.5.1/src/anomalib/models/dfm/
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/dfm/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3024 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/dfm/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4998 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/dfm/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     6872 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/dfm/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.725657 anomalib-0.5.1/src/anomalib/models/draem/
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/draem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3149 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/draem/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     5472 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/draem/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/draem/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)    19097 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/draem/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.725657 anomalib-0.5.1/src/anomalib/models/fastflow/
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/fastflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1624 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/fastflow/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/fastflow/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4769 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/fastflow/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/fastflow/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     9915 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/fastflow/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.725657 anomalib-0.5.1/src/anomalib/models/ganomaly/
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ganomaly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3070 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ganomaly/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     9292 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ganomaly/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ganomaly/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)    12986 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/ganomaly/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.729656 anomalib-0.5.1/src/anomalib/models/padim/
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/padim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4731 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/padim/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     3049 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/padim/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4851 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/padim/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     5900 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/padim/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.729656 anomalib-0.5.1/src/anomalib/models/patchcore/
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/patchcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/patchcore/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     3087 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/patchcore/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4699 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/patchcore/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     7789 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/patchcore/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.729656 anomalib-0.5.1/src/anomalib/models/reverse_distillation/
--rw-r--r--   0 runner    (1001) docker     (122)      259 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/reverse_distillation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3374 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/reverse_distillation/anomaly_map.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.729656 anomalib-0.5.1/src/anomalib/models/reverse_distillation/components/
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/reverse_distillation/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5832 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/reverse_distillation/components/bottleneck.py
--rw-r--r--   0 runner    (1001) docker     (122)    11795 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/reverse_distillation/components/de_resnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     3238 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/reverse_distillation/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     5411 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/reverse_distillation/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1005 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/reverse_distillation/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     2925 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/reverse_distillation/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.729656 anomalib-0.5.1/src/anomalib/models/rkde/
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/rkde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3233 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/rkde/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/rkde/feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/rkde/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     5610 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/rkde/region_extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)     3884 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/rkde/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.733656 anomalib-0.5.1/src/anomalib/models/stfpm/
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/stfpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3292 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/stfpm/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     3177 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/stfpm/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4438 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/stfpm/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2691 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/stfpm/loss.py
--rw-r--r--   0 runner    (1001) docker     (122)     2762 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/models/stfpm/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.733656 anomalib-0.5.1/src/anomalib/post_processing/
--rw-r--r--   0 runner    (1001) docker     (122)      683 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/post_processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.733656 anomalib-0.5.1/src/anomalib/post_processing/normalization/
--rw-r--r--   0 runner    (1001) docker     (122)      295 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/post_processing/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1962 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/post_processing/normalization/cdf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/post_processing/normalization/min_max.py
--rw-r--r--   0 runner    (1001) docker     (122)     5797 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/post_processing/post_process.py
--rw-r--r--   0 runner    (1001) docker     (122)    13077 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/post_processing/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.733656 anomalib-0.5.1/src/anomalib/pre_processing/
--rw-r--r--   0 runner    (1001) docker     (122)      291 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/pre_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8889 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/pre_processing/pre_process.py
--rw-r--r--   0 runner    (1001) docker     (122)    15168 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/pre_processing/tiler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.733656 anomalib-0.5.1/src/anomalib/pre_processing/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)      190 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/pre_processing/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/pre_processing/transforms/custom.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.733656 anomalib-0.5.1/src/anomalib/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.737655 anomalib-0.5.1/src/anomalib/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)     8412 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6536 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/cdf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (122)     1760 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/export.py
--rw-r--r--   0 runner    (1001) docker     (122)     1723 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/metrics_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     4143 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/min_max_normalization.py
--rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/model_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.737655 anomalib-0.5.1/src/anomalib/utils/callbacks/nncf/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/nncf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/nncf/callback.py
--rw-r--r--   0 runner    (1001) docker     (122)     7363 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/nncf/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/post_processing_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     2891 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/tiler_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.737655 anomalib-0.5.1/src/anomalib/utils/callbacks/visualizer/
--rw-r--r--   0 runner    (1001) docker     (122)      394 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/visualizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4066 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/visualizer/visualizer_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4159 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/visualizer/visualizer_image.py
--rw-r--r--   0 runner    (1001) docker     (122)     2298 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/callbacks/visualizer/visualizer_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.737655 anomalib-0.5.1/src/anomalib/utils/cli/
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.737655 anomalib-0.5.1/src/anomalib/utils/cv/
--rw-r--r--   0 runner    (1001) docker     (122)      274 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/cv/connected_components.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.737655 anomalib-0.5.1/src/anomalib/utils/hpo/
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1647 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/hpo/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     5035 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/hpo/runners.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.737655 anomalib-0.5.1/src/anomalib/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (122)     4881 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      617 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4849 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/loggers/comet.py
--rw-r--r--   0 runner    (1001) docker     (122)     3792 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (122)     4201 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/loggers/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.741655 anomalib-0.5.1/src/anomalib/utils/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)     6914 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/anomaly_score_distribution.py
--rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/anomaly_score_threshold.py
--rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/aupr.py
--rw-r--r--   0 runner    (1001) docker     (122)     9080 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/aupro.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/auroc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/min_max.py
--rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/optimal_f1.py
--rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/plotting_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2400 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/metrics/pro.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.741655 anomalib-0.5.1/src/anomalib/utils/sweep/
--rw-r--r--   0 runner    (1001) docker     (122)      465 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/sweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6456 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/sweep/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.741655 anomalib-0.5.1/src/anomalib/utils/sweep/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/sweep/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2638 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/sweep/helpers/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)     2320 2023-05-24 14:42:53.000000 anomalib-0.5.1/src/anomalib/utils/sweep/helpers/inference.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 14:43:06.709658 anomalib-0.5.1/src/anomalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    24127 2023-05-24 14:43:06.000000 anomalib-0.5.1/src/anomalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9212 2023-05-24 14:43:06.000000 anomalib-0.5.1/src/anomalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 14:43:06.000000 anomalib-0.5.1/src/anomalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-24 14:43:06.000000 anomalib-0.5.1/src/anomalib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      726 2023-05-24 14:43:06.000000 anomalib-0.5.1/src/anomalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-24 14:43:06.000000 anomalib-0.5.1/src/anomalib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.162515 anomalib-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-06-15 14:32:06.000000 anomalib-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-06-15 14:32:06.000000 anomalib-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    24127 2023-06-15 14:32:21.162515 anomalib-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    23625 2023-06-15 14:32:06.000000 anomalib-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2968 2023-06-15 14:32:06.000000 anomalib-0.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.122515 anomalib-0.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-06-15 14:32:06.000000 anomalib-0.6.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-06-15 14:32:06.000000 anomalib-0.6.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-06-15 14:32:06.000000 anomalib-0.6.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-15 14:32:06.000000 anomalib-0.6.0/requirements/loggers.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-06-15 14:32:06.000000 anomalib-0.6.0/requirements/notebooks.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-15 14:32:06.000000 anomalib-0.6.0/requirements/openvino.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-15 14:32:21.162515 anomalib-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-06-15 14:32:06.000000 anomalib-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.118515 anomalib-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.122515 anomalib-0.6.0/src/anomalib/
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.126515 anomalib-0.6.0/src/anomalib/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13768 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.126515 anomalib-0.6.0/src/anomalib/data/
+-rw-r--r--   0 runner    (1001) docker     (122)    11412 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12710 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/avenue.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.126515 anomalib-0.6.0/src/anomalib/data/base/
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8134 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/base/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7327 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/base/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2540 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/base/depth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/base/video.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12067 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/btech.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12955 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/folder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17503 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/folder_3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/inference.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11448 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/kolektor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12064 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/mvtec.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13095 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/mvtec_3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14449 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/shanghaitech.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6941 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/task_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11841 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/ucsd_ped.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.130515 anomalib-0.6.0/src/anomalib/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6761 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/utils/augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5178 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/utils/boxes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14662 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/utils/download.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.130515 anomalib-0.6.0/src/anomalib/data/utils/generators/
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/utils/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6027 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/utils/generators/perlin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8113 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/utils/label.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2804 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4870 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/utils/split.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5861 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/utils/transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3651 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/utils/video.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9808 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/data/visa.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.130515 anomalib-0.6.0/src/anomalib/deploy/
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5674 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/deploy/export.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.130515 anomalib-0.6.0/src/anomalib/deploy/inferencers/
+-rw-r--r--   0 runner    (1001) docker     (122)      326 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/deploy/inferencers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7198 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/deploy/inferencers/base_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8084 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/deploy/inferencers/openvino_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6406 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/deploy/inferencers/torch_inferencer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.130515 anomalib-0.6.0/src/anomalib/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     3005 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.134515 anomalib-0.6.0/src/anomalib/models/ai_vad/
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/ai_vad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.134515 anomalib-0.6.0/src/anomalib/models/ai_vad/clip/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/ai_vad/clip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7865 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/ai_vad/clip/clip.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17868 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/ai_vad/clip/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3190 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/ai_vad/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    11997 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/ai_vad/density.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9489 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/ai_vad/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/ai_vad/flow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6617 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/ai_vad/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11076 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/ai_vad/regions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5604 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/ai_vad/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.134515 anomalib-0.6.0/src/anomalib/models/cfa/
+-rw-r--r--   0 runner    (1001) docker     (122)      335 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/cfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2762 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/cfa/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3059 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/cfa/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     5766 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/cfa/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1599 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/cfa/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13213 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/cfa/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.134515 anomalib-0.6.0/src/anomalib/models/cflow/
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/cflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/cflow/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3154 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/cflow/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     8299 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/cflow/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5230 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/cflow/torch_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4179 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/cflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.134515 anomalib-0.6.0/src/anomalib/models/components/
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.134515 anomalib-0.6.0/src/anomalib/models/components/base/
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10187 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/base/anomaly_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/base/dynamic_module.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.134515 anomalib-0.6.0/src/anomalib/models/components/classification/
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5904 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/classification/kde_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.134515 anomalib-0.6.0/src/anomalib/models/components/dimensionality_reduction/
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/dimensionality_reduction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3307 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/dimensionality_reduction/pca.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5337 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/dimensionality_reduction/random_projection.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.138515 anomalib-0.6.0/src/anomalib/models/components/feature_extractors/
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/feature_extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4104 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/feature_extractors/timm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9158 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/feature_extractors/torchfx.py
+-rw-r--r--   0 runner    (1001) docker     (122)      960 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/feature_extractors/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.138515 anomalib-0.6.0/src/anomalib/models/components/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3553 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/filters/blur.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.138515 anomalib-0.6.0/src/anomalib/models/components/flow/
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12649 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/flow/all_in_one_block.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.138515 anomalib-0.6.0/src/anomalib/models/components/layers/
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3143 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/layers/sspcab.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.138515 anomalib-0.6.0/src/anomalib/models/components/sampling/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/sampling/k_center_greedy.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.138515 anomalib-0.6.0/src/anomalib/models/components/stats/
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2776 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/stats/kde.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5603 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/components/stats/multi_variate_gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.142515 anomalib-0.6.0/src/anomalib/models/csflow/
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/csflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/csflow/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/csflow/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4772 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/csflow/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/csflow/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21233 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/csflow/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.142515 anomalib-0.6.0/src/anomalib/models/dfkde/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/dfkde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/dfkde/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4824 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/dfkde/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3052 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/dfkde/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.142515 anomalib-0.6.0/src/anomalib/models/dfm/
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/dfm/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3024 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/dfm/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4998 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/dfm/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6872 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/dfm/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.142515 anomalib-0.6.0/src/anomalib/models/draem/
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/draem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3149 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/draem/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     5472 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/draem/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/draem/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19097 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/draem/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.142515 anomalib-0.6.0/src/anomalib/models/efficientad/
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/efficientad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2874 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/efficientad/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    11133 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/efficientad/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12514 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/efficientad/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.142515 anomalib-0.6.0/src/anomalib/models/fastflow/
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/fastflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1624 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/fastflow/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/fastflow/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4769 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/fastflow/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/fastflow/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10219 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/fastflow/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.146515 anomalib-0.6.0/src/anomalib/models/ganomaly/
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/ganomaly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3070 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/ganomaly/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     9292 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/ganomaly/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/ganomaly/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12986 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/ganomaly/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.146515 anomalib-0.6.0/src/anomalib/models/padim/
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/padim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4731 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/padim/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3049 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/padim/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4851 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/padim/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5900 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/padim/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.146515 anomalib-0.6.0/src/anomalib/models/patchcore/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/patchcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/patchcore/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3087 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/patchcore/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4699 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/patchcore/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7789 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/patchcore/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.150515 anomalib-0.6.0/src/anomalib/models/reverse_distillation/
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/reverse_distillation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3374 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/reverse_distillation/anomaly_map.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.150515 anomalib-0.6.0/src/anomalib/models/reverse_distillation/components/
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/reverse_distillation/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5832 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/reverse_distillation/components/bottleneck.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11795 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/reverse_distillation/components/de_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3238 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/reverse_distillation/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     5411 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/reverse_distillation/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1005 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/reverse_distillation/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2925 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/reverse_distillation/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.150515 anomalib-0.6.0/src/anomalib/models/rkde/
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/rkde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3233 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/rkde/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/rkde/feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/rkde/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5610 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/rkde/region_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3884 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/rkde/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.150515 anomalib-0.6.0/src/anomalib/models/stfpm/
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/stfpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3292 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/stfpm/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3177 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/stfpm/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     4438 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/stfpm/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2691 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/stfpm/loss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2762 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/models/stfpm/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.150515 anomalib-0.6.0/src/anomalib/post_processing/
+-rw-r--r--   0 runner    (1001) docker     (122)      683 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/post_processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.150515 anomalib-0.6.0/src/anomalib/post_processing/normalization/
+-rw-r--r--   0 runner    (1001) docker     (122)      295 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/post_processing/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1962 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/post_processing/normalization/cdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/post_processing/normalization/min_max.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5797 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/post_processing/post_process.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13077 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/post_processing/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.154515 anomalib-0.6.0/src/anomalib/pre_processing/
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/pre_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8889 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/pre_processing/pre_process.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15172 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/pre_processing/tiler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.154515 anomalib-0.6.0/src/anomalib/pre_processing/transforms/
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/pre_processing/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/pre_processing/transforms/custom.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.154515 anomalib-0.6.0/src/anomalib/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.154515 anomalib-0.6.0/src/anomalib/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)     8412 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6536 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/callbacks/cdf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1760 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/callbacks/export.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1723 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/callbacks/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/callbacks/metrics_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4143 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/callbacks/min_max_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/callbacks/model_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.154515 anomalib-0.6.0/src/anomalib/utils/callbacks/nncf/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/callbacks/nncf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/callbacks/nncf/callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7363 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/callbacks/nncf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/callbacks/post_processing_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2891 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/callbacks/tiler_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/callbacks/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.158515 anomalib-0.6.0/src/anomalib/utils/callbacks/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (122)      394 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/callbacks/visualizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4066 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/callbacks/visualizer/visualizer_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4159 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/callbacks/visualizer/visualizer_image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2298 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/callbacks/visualizer/visualizer_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.158515 anomalib-0.6.0/src/anomalib/utils/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.158515 anomalib-0.6.0/src/anomalib/utils/cv/
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/cv/connected_components.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.158515 anomalib-0.6.0/src/anomalib/utils/hpo/
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1647 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/hpo/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5035 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/hpo/runners.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.158515 anomalib-0.6.0/src/anomalib/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (122)     4881 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      617 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4849 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/loggers/comet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3792 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4201 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/loggers/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.162515 anomalib-0.6.0/src/anomalib/utils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)     6914 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/metrics/anomaly_score_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/metrics/anomaly_score_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/metrics/aupr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9080 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/metrics/aupro.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/metrics/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/metrics/collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/metrics/min_max.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/metrics/optimal_f1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/metrics/plotting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2400 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/metrics/pro.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.162515 anomalib-0.6.0/src/anomalib/utils/sweep/
+-rw-r--r--   0 runner    (1001) docker     (122)      465 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/sweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6456 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/sweep/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.162515 anomalib-0.6.0/src/anomalib/utils/sweep/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/sweep/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2638 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/sweep/helpers/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2320 2023-06-15 14:32:06.000000 anomalib-0.6.0/src/anomalib/utils/sweep/helpers/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 14:32:21.126515 anomalib-0.6.0/src/anomalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    24127 2023-06-15 14:32:21.000000 anomalib-0.6.0/src/anomalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9398 2023-06-15 14:32:21.000000 anomalib-0.6.0/src/anomalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 14:32:21.000000 anomalib-0.6.0/src/anomalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-15 14:32:21.000000 anomalib-0.6.0/src/anomalib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      726 2023-06-15 14:32:21.000000 anomalib-0.6.0/src/anomalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-15 14:32:21.000000 anomalib-0.6.0/src/anomalib.egg-info/top_level.txt
```

### Comparing `anomalib-0.5.1/LICENSE` & `anomalib-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/PKG-INFO` & `anomalib-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anomalib
-Version: 0.5.1
+Version: 0.6.0
 Summary: anomalib - Anomaly Detection Library
 Home-page: 
 Author: Intel OpenVINO
 Author-email: help@openvino.intel.com
 License: Copyright (c) Intel - All Rights Reserved. Licensed under the Apache License, Version 2.0 (the "License")See LICENSE file for more details.
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `anomalib-0.5.1/README.md` & `anomalib-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/pyproject.toml` & `anomalib-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/setup.py` & `anomalib-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/config/config.py` & `anomalib-0.6.0/src/anomalib/config/config.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/data/__init__.py` & `anomalib-0.6.0/src/anomalib/data/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/data/avenue.py` & `anomalib-0.6.0/src/anomalib/data/avenue.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/data/base/datamodule.py` & `anomalib-0.6.0/src/anomalib/data/base/datamodule.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/data/base/dataset.py` & `anomalib-0.6.0/src/anomalib/data/base/dataset.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/data/base/depth.py` & `anomalib-0.6.0/src/anomalib/data/base/depth.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/data/base/video.py` & `anomalib-0.6.0/src/anomalib/data/base/video.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/data/btech.py` & `anomalib-0.6.0/src/anomalib/data/btech.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 
 logger = logging.getLogger(__name__)
 
 DOWNLOAD_INFO = DownloadInfo(
     name="btech", url="https://avires.dimi.uniud.it/papers/btad/btad.zip", hash="c1fa4d56ac50dd50908ce04e81037a8e"
 )
 
+CATEGORIES = ("01", "02", "03")
+
 
 def make_btech_dataset(path: Path, split: str | Split | None = None) -> DataFrame:
     """Create BTech samples by parsing the BTech data file structure.
 
     The files are expected to follow the structure:
         path/to/dataset/split/category/image_filename.png
         path/to/dataset/ground_truth/category/mask_filename.png
@@ -130,15 +132,15 @@
 
     Examples:
         >>> from anomalib.data.btech import BTechDataset
         >>> from anomalib.pre_processing import get_transforms
         >>> transform = get_transforms(image_size=256)
         >>> dataset = BTechDataset(
         ...     root='./datasets/BTech',
-        ...     category='leather',
+        ...     category='01',
         ...     transform=transform,
         ...     task="classification",
         ...     is_train=True,
         ... )
         >>> dataset[0].keys()
         dict_keys(['image'])
 
@@ -211,21 +213,21 @@
             Defaults to 0.5.
         seed (int | None, optional): Seed which may be set to a fixed value for reproducibility. Defaults to None.
 
     Examples:
         >>> from anomalib.data import BTech
         >>> datamodule = BTech(
         ...     root="./datasets/BTech",
-        ...     category="leather",
+        ...     category="01",
         ...     image_size=256,
         ...     train_batch_size=32,
-        ...     test_batch_size=32,
+        ...     eval_batch_size=32,
         ...     num_workers=8,
         ...     transform_config_train=None,
-        ...     transform_config_val=None,
+        ...     transform_config_eval=None,
         ... )
         >>> datamodule.setup()
 
         >>> i, data = next(enumerate(datamodule.train_dataloader()))
         >>> data.keys()
         dict_keys(['image'])
         >>> data["image"].shape
```

### Comparing `anomalib-0.5.1/src/anomalib/data/folder.py` & `anomalib-0.6.0/src/anomalib/data/folder.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/data/folder_3d.py` & `anomalib-0.6.0/src/anomalib/data/folder_3d.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/data/inference.py` & `anomalib-0.6.0/src/anomalib/data/inference.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/data/kolektor.py` & `anomalib-0.6.0/src/anomalib/data/kolektor.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/data/mvtec.py` & `anomalib-0.6.0/src/anomalib/data/mvtec.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,23 +44,41 @@
     download_and_extract,
     get_transforms,
 )
 
 logger = logging.getLogger(__name__)
 
 
-IMG_EXTENSIONS = [".png", ".PNG"]
+IMG_EXTENSIONS = (".png", ".PNG")
 
 DOWNLOAD_INFO = DownloadInfo(
     name="mvtec",
     url="https://www.mydrive.ch/shares/38536/3830184030e49fe74747669442f0f282/download/420938113-1629952094"
     "/mvtec_anomaly_detection.tar.xz",
     hash="eefca59f2cede9c3fc5b6befbfec275e",
 )
 
+CATEGORIES = (
+    "bottle",
+    "cable",
+    "capsule",
+    "carpet",
+    "grid",
+    "hazelnut",
+    "leather",
+    "metal_nut",
+    "pill",
+    "screw",
+    "tile",
+    "toothbrush",
+    "transistor",
+    "wood",
+    "zipper",
+)
+
 
 def make_mvtec_dataset(
     root: str | Path, split: str | Split | None = None, extensions: Sequence[str] | None = None
 ) -> DataFrame:
     """Create MVTec AD samples by parsing the MVTec AD data file structure.
 
     The files are expected to follow the structure:
```

### Comparing `anomalib-0.5.1/src/anomalib/data/mvtec_3d.py` & `anomalib-0.6.0/src/anomalib/data/mvtec_3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 DOWNLOAD_INFO = DownloadInfo(
     name="mvtec_3d",
     url="https://www.mydrive.ch/shares/45920/dd1eb345346df066c63b5c95676b961b/download/428824485-1643285832"
     "/mvtec_3d_anomaly_detection.tar.xz",
     hash="d8bb2800fbf3ac88e798da6ae10dc819",
 )
 
+CATEGORIES = ("bagel", "cable_gland", "carrot", "cookie", "dowel", "foam", "peach", "potato", "rope", "tire")
+
 
 def make_mvtec_3d_dataset(
     root: str | Path, split: str | Split | None = None, extensions: Sequence[str] | None = None
 ) -> DataFrame:
     """Create MVTec 3D-AD samples by parsing the MVTec AD data file structure.
 
     The files are expected to follow the structure:
```

### Comparing `anomalib-0.5.1/src/anomalib/data/shanghaitech.py` & `anomalib-0.6.0/src/anomalib/data/shanghaitech.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/data/synthetic.py` & `anomalib-0.6.0/src/anomalib/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/data/ucsd_ped.py` & `anomalib-0.6.0/src/anomalib/data/ucsd_ped.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 
 DOWNLOAD_INFO = DownloadInfo(
     name="UCSD Pedestrian",
     url="http://www.svcl.ucsd.edu/projects/anomaly/UCSD_Anomaly_Dataset.tar.gz",
     hash="5006421b89885f45a6f93b041145f2eb",
 )
 
+CATEGORIES = ("UCSDped1", "UCSDped2")
+
 
 def make_ucsd_dataset(path: Path, split: str | Split | None = None) -> DataFrame:
     """Create UCSD Pedestrian dataset by parsing the file structure.
 
     The files are expected to follow the structure:
         path/to/dataset/category/split/video_id/image_filename.tif
         path/to/dataset/category/split/video_id_gt/mask_filename.bmp
@@ -147,15 +149,15 @@
 
 class UCSDpedDataset(AnomalibVideoDataset):
     """UCSDped Dataset class.
 
     Args:
         task (TaskType): Task type, 'classification', 'detection' or 'segmentation'
         root (Path | str): Path to the root of the dataset
-        category (str): Sub-category of the dataset, e.g. 'bottle'
+        category (str): Sub-category of the dataset, e.g. "UCSDped1" or "UCSDped2"
         transform (A.Compose): Albumentations Compose object describing the transforms that are applied to the inputs.
         split (str | Split | None): Split of the dataset, usually Split.TRAIN or Split.TEST
         clip_length_in_frames (int, optional): Number of video frames in each clip.
         frames_between_clips (int, optional): Number of frames between each consecutive video clip.
         target_frame (VideoTargetFrame): Specifies the target frame in the video clip, used for ground truth retrieval
     """
 
@@ -182,15 +184,15 @@
 
 
 class UCSDped(AnomalibVideoDataModule):
     """UCSDped DataModule class.
 
     Args:
         root (Path | str): Path to the root of the dataset
-        category (str): Sub-category of the dataset, e.g. 'bottle'
+        category (str): Sub-category of the dataset, e.g. "UCSDped1" or "UCSDped2"
         clip_length_in_frames (int, optional): Number of video frames in each clip.
         frames_between_clips (int, optional): Number of frames between each consecutive video clip.
         target_frame (VideoTargetFrame): Specifies the target frame in the video clip, used for ground truth retrieval
         task (TaskType): Task type, 'classification', 'detection' or 'segmentation'
         image_size (int | tuple[int, int] | None, optional): Size of the input image.
             Defaults to None.
         center_crop (int | tuple[int, int] | None, optional): When provided, the images will be center-cropped
```

### Comparing `anomalib-0.5.1/src/anomalib/data/utils/__init__.py` & `anomalib-0.6.0/src/anomalib/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/data/utils/augmenter.py` & `anomalib-0.6.0/src/anomalib/data/utils/augmenter.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/data/utils/boxes.py` & `anomalib-0.6.0/src/anomalib/data/utils/boxes.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,19 +40,20 @@
     for im_idx, im_comps in enumerate(batch_comps):
         labels = torch.unique(im_comps)
         im_boxes = []
         im_scores = []
         for label in labels[labels != 0]:
             y_loc, x_loc = torch.where(im_comps == label)
             # add box
-            im_boxes.append(Tensor([torch.min(x_loc), torch.min(y_loc), torch.max(x_loc), torch.max(y_loc)]))
+            box = Tensor([torch.min(x_loc), torch.min(y_loc), torch.max(x_loc), torch.max(y_loc)]).to(masks.device)
+            im_boxes.append(box)
             if anomaly_maps is not None:
                 im_scores.append(torch.max(anomaly_maps[im_idx, y_loc, x_loc]))
-        batch_boxes.append(torch.stack(im_boxes) if im_boxes else torch.empty((0, 4)))
-        batch_scores.append(torch.stack(im_scores) if im_scores else torch.empty(0))
+        batch_boxes.append(torch.stack(im_boxes) if im_boxes else torch.empty((0, 4), device=masks.device))
+        batch_scores.append(torch.stack(im_scores) if im_scores else torch.empty(0, device=masks.device))
 
     return batch_boxes, batch_scores
 
 
 def boxes_to_masks(boxes: list[Tensor], image_size: tuple[int, int]) -> Tensor:
     """Convert bounding boxes to segmentations masks.
 
@@ -61,15 +62,15 @@
             box coordinates of the regions of interest in xyxy format.
         image_size (tuple[int, int]): Image size of the output masks in (H, W) format.
 
     Returns:
         Tensor: Tensor of shape (B, H, W) in which each slice is a binary mask showing the pixels contained by a
             bounding box.
     """
-    masks = torch.zeros((len(boxes),) + image_size)
+    masks = torch.zeros((len(boxes),) + image_size).to(boxes[0].device)
     for im_idx, im_boxes in enumerate(boxes):
         for box in im_boxes:
             x_1, y_1, x_2, y_2 = box.int()
             masks[im_idx, y_1 : y_2 + 1, x_1 : x_2 + 1] = 1
     return masks
```

### Comparing `anomalib-0.5.1/src/anomalib/data/utils/download.py` & `anomalib-0.6.0/src/anomalib/data/utils/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,36 @@
     """
     with file_path.open("rb") as hash_file:
         assert (
             hashlib.md5(hash_file.read()).hexdigest() == expected_hash
         ), f"Downloaded file {file_path} does not match the required hash."
 
 
+def extract(file_name: Path, root: Path) -> None:
+    """Extract a dataset
+
+    Args:
+        file_name (Path): Path of the file to be extracted.
+        root (Path): Root directory where the dataset will be stored.
+
+    """
+    logger.info("Extracting dataset into root folder.")
+    if file_name.suffix == ".zip":
+        with ZipFile(file_name, "r") as zip_file:
+            zip_file.extractall(root)
+    elif file_name.suffix in (".tar", ".gz", ".xz", ".tgz"):
+        with tarfile.open(file_name) as tar_file:
+            safe_extract(tar_file, root)
+    else:
+        raise ValueError(f"Unrecognized file format: {file_name}")
+
+    logger.info("Cleaning up files.")
+    (file_name).unlink()
+
+
 def download_and_extract(root: Path, info: DownloadInfo) -> None:
     """Download and extract a dataset.
 
     Args:
         root (Path): Root directory where the dataset will be stored.
         info (DownloadInfo): Info needed to download the dataset.
     """
@@ -242,26 +264,15 @@
                 url=f"{info.url}",
                 filename=downloaded_file_path,
                 reporthook=progress_bar.update_to,
             )
         logger.info("Checking the hash of the downloaded file.")
         hash_check(downloaded_file_path, info.hash)
 
-    logger.info("Extracting dataset into root folder.")
-    if downloaded_file_path.suffix == ".zip":
-        with ZipFile(downloaded_file_path, "r") as zip_file:
-            zip_file.extractall(root)
-    elif downloaded_file_path.suffix in (".tar", ".gz", ".xz"):
-        with tarfile.open(downloaded_file_path) as tar_file:
-            safe_extract(tar_file, root)
-    else:
-        raise ValueError(f"Unrecognized file format: {downloaded_file_path}")
-
-    logger.info("Cleaning up files.")
-    (downloaded_file_path).unlink()
+    extract(downloaded_file_path, root)
 
 
 def is_within_directory(directory: Path, target: Path):
     """Checks if a target path is located within a given directory.
 
     Args:
         directory (Path): path of the parent directory
```

### Comparing `anomalib-0.5.1/src/anomalib/data/utils/generators/perlin.py` & `anomalib-0.6.0/src/anomalib/data/utils/generators/perlin.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/data/utils/image.py` & `anomalib-0.6.0/src/anomalib/data/utils/image.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/data/utils/path.py` & `anomalib-0.6.0/src/anomalib/data/utils/path.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/data/utils/split.py` & `anomalib-0.6.0/src/anomalib/data/utils/split.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/data/utils/transform.py` & `anomalib-0.6.0/src/anomalib/data/utils/transform.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/data/utils/video.py` & `anomalib-0.6.0/src/anomalib/data/utils/video.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/data/visa.py` & `anomalib-0.6.0/src/anomalib/data/visa.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,29 @@
 
 DOWNLOAD_INFO = DownloadInfo(
     name="VisA",
     url="https://amazon-visual-anomaly.s3.us-west-2.amazonaws.com/VisA_20220922.tar",
     hash="ef908989b6dc701fc218f643c127a4de",
 )
 
+CATEGORIES = (
+    "candle",
+    "capsules",
+    "cashew",
+    "chewinggum",
+    "fryum",
+    "macaroni1",
+    "macaroni2",
+    "pcb1",
+    "pcb2",
+    "pcb3",
+    "pcb4",
+    "pipe_fryum",
+)
+
 
 class VisaDataset(AnomalibDataset):
     """VisA dataset class.
 
     Args:
         task (TaskType): Task type, ``classification``, ``detection`` or ``segmentation``
         transform (A.Compose): Albumentations Compose object describing the transforms that are applied to the inputs.
```

### Comparing `anomalib-0.5.1/src/anomalib/deploy/export.py` & `anomalib-0.6.0/src/anomalib/deploy/export.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/deploy/inferencers/base_inferencer.py` & `anomalib-0.6.0/src/anomalib/deploy/inferencers/base_inferencer.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,19 +170,19 @@
         # standardize image scores
         if "image_mean" in metadata.keys() and "image_std" in metadata.keys():
             pred_scores = standardize(pred_scores, metadata["image_mean"], metadata["image_std"])
             pred_scores = normalize_cdf(pred_scores, metadata["image_threshold"])
 
         return anomaly_maps, float(pred_scores)
 
-    def _load_metadata(self, path: str | Path | None = None) -> dict | DictConfig:
+    def _load_metadata(self, path: str | Path | dict | None = None) -> dict | DictConfig:
         """Loads the meta data from the given path.
 
         Args:
-            path (str | Path | None, optional): Path to JSON file containing the metadata.
+            path (str | Path | dict | None, optional): Path to JSON file containing the metadata.
                 If no path is provided, it returns an empty dict. Defaults to None.
 
         Returns:
             dict | DictConfig: Dictionary containing the metadata.
         """
         metadata: dict[str, float | np.ndarray | Tensor] | DictConfig = {}
         if path is not None:
```

### Comparing `anomalib-0.5.1/src/anomalib/deploy/inferencers/openvino_inferencer.py` & `anomalib-0.6.0/src/anomalib/deploy/inferencers/openvino_inferencer.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 from omegaconf import DictConfig
 
 from anomalib.data import TaskType
 
 from .base_inferencer import Inferencer
 
 if find_spec("openvino") is not None:
-    from openvino.inference_engine import IECore  # type: ignore  # pylint: disable=no-name-in-module
+    from openvino.runtime import Core
+else:
+    raise ImportError("OpenVINO is not installed. Please install OpenVINO to use OpenVINOInferencer.")
 
 
 class OpenVINOInferencer(Inferencer):
     """OpenVINO implementation for the inference.
 
     Args:
         path (str | Path): Path to the openvino onnx, xml or bin file.
@@ -35,54 +37,63 @@
 
     def __init__(
         self,
         path: str | Path | tuple[bytes, bytes],
         metadata: str | Path | dict | None = None,
         device: str | None = "CPU",
         task: str | None = None,
+        config: dict | None = None,
     ) -> None:
         self.device = device
-        self.input_blob, self.output_blob, self.network = self.load_model(path)
-        self.metadata = metadata if isinstance(metadata, dict) else super()._load_metadata(metadata)
+
+        self.config = config
+        self.input_blob, self.output_blob, self.model = self.load_model(path)
+        self.metadata = super()._load_metadata(metadata)
+
         self.task = TaskType(task) if task else TaskType(self.metadata["task"])
 
     def load_model(self, path: str | Path | tuple[bytes, bytes]):
         """Load the OpenVINO model.
 
         Args:
             path (str | Path | tuple[bytes, bytes]): Path to the onnx or xml and bin files
                                                         or tuple of .xml and .bin data as bytes.
 
         Returns:
             [tuple[str, str, ExecutableNetwork]]: Input and Output blob names
                 together with the Executable network.
         """
-        ie_core = IECore()
+        ie_core = Core()
         # If tuple of bytes is passed
 
         if isinstance(path, tuple):
-            network = ie_core.read_network(model=path[0], weights=path[1], init_from_buffer=True)
+            model = ie_core.read_model(model=path[0], weights=path[1], init_from_buffer=True)
         else:
             path = path if isinstance(path, Path) else Path(path)
             if path.suffix in (".bin", ".xml"):
                 if path.suffix == ".bin":
                     bin_path, xml_path = path, path.with_suffix(".xml")
                 elif path.suffix == ".xml":
                     xml_path, bin_path = path, path.with_suffix(".bin")
-                network = ie_core.read_network(xml_path, bin_path)
+                model = ie_core.read_model(xml_path, bin_path)
             elif path.suffix == ".onnx":
-                network = ie_core.read_network(path)
+                model = ie_core.read_model(path)
             else:
                 raise ValueError(f"Path must be .onnx, .bin or .xml file. Got {path.suffix}")
+        # Create cache folder
+        cache_folder = Path("cache")
+        cache_folder.mkdir(exist_ok=True)
+        ie_core.set_property({"CACHE_DIR": cache_folder})
+
+        compile_model = ie_core.compile_model(model=model, device_name=self.device, config=self.config)
 
-        input_blob = next(iter(network.input_info))
-        output_blob = next(iter(network.outputs))
-        executable_network = ie_core.load_network(network=network, device_name=self.device)
+        input_blob = compile_model.input(0)
+        output_blob = compile_model.output(0)
 
-        return input_blob, output_blob, executable_network
+        return input_blob, output_blob, compile_model
 
     def pre_process(self, image: np.ndarray) -> np.ndarray:
         """Pre process the input image by applying transformations.
 
         Args:
             image (np.ndarray): Input image.
 
@@ -105,15 +116,15 @@
 
         Args:
             image (np.ndarray): Input tensor.
 
         Returns:
             np.ndarray: Output predictions.
         """
-        return self.network.infer(inputs={self.input_blob: image})
+        return self.model(image)
 
     def post_process(self, predictions: np.ndarray, metadata: dict | DictConfig | None = None) -> dict[str, Any]:
         """Post process the output predictions.
 
         Args:
             predictions (np.ndarray): Raw output predicted by the model.
             metadata (Dict, optional): Meta data. Post-processing step sometimes requires
```

### Comparing `anomalib-0.5.1/src/anomalib/deploy/inferencers/torch_inferencer.py` & `anomalib-0.6.0/src/anomalib/deploy/inferencers/torch_inferencer.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,19 +56,19 @@
 
         if device == "auto":
             device = "cuda" if torch.cuda.is_available() else "cpu"
         elif device == "gpu":
             device = "cuda"
         return torch.device(device)
 
-    def _load_metadata(self, path: str | Path | None = None) -> dict | DictConfig:
+    def _load_metadata(self, path: str | Path | dict | None = None) -> dict | DictConfig:
         """Load metadata from file.
 
         Args:
-            path (str | Path): Path to the model pt file.
+            path (str | Path | dict): Path to the model pt file.
 
         Returns:
             dict: Dictionary containing the metadata.
         """
         metadata = torch.load(path, map_location=self.device)["metadata"] if path else {}
         return metadata
```

### Comparing `anomalib-0.5.1/src/anomalib/models/__init__.py` & `anomalib-0.6.0/src/anomalib/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from anomalib.models.cfa import Cfa
 from anomalib.models.cflow import Cflow
 from anomalib.models.components import AnomalyModule
 from anomalib.models.csflow import Csflow
 from anomalib.models.dfkde import Dfkde
 from anomalib.models.dfm import Dfm
 from anomalib.models.draem import Draem
+from anomalib.models.efficientad import EfficientAD
 from anomalib.models.fastflow import Fastflow
 from anomalib.models.ganomaly import Ganomaly
 from anomalib.models.padim import Padim
 from anomalib.models.patchcore import Patchcore
 from anomalib.models.reverse_distillation import ReverseDistillation
 from anomalib.models.rkde import Rkde
 from anomalib.models.stfpm import Stfpm
@@ -39,14 +40,15 @@
     "Ganomaly",
     "Padim",
     "Patchcore",
     "ReverseDistillation",
     "Rkde",
     "Stfpm",
     "AiVad",
+    "EfficientAD",
 ]
 
 logger = logging.getLogger(__name__)
 
 
 def _snake_to_pascal_case(model_name: str) -> str:
     """Convert model name from snake case to Pascal case.
@@ -91,14 +93,15 @@
         "ganomaly",
         "padim",
         "patchcore",
         "reverse_distillation",
         "rkde",
         "stfpm",
         "ai_vad",
+        "efficientad",
     ]
     model: AnomalyModule
 
     if config.model.name in model_list:
         module = import_module(f"anomalib.models.{config.model.name}")
         model = getattr(module, f"{_snake_to_pascal_case(config.model.name)}Lightning")(config)
```

### Comparing `anomalib-0.5.1/src/anomalib/models/ai_vad/clip/clip.py` & `anomalib-0.6.0/src/anomalib/models/ai_vad/clip/clip.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/ai_vad/clip/model.py` & `anomalib-0.6.0/src/anomalib/models/ai_vad/clip/model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/ai_vad/config.yaml` & `anomalib-0.6.0/src/anomalib/models/ai_vad/config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -25,19 +25,28 @@
     stride: null
     remove_border_count: 0
     use_random_tiling: False
     random_tile_count: 16
 
 model:
   name: ai_vad
+  # region extraction parameters
   box_score_thresh: 0.7
+  persons_only: false
+  min_bbox_area: 100
+  max_bbox_overlap: 0.65
+  enable_foreground_detections: true
+  foreground_kernel_size: 3
+  foreground_binary_threshold: 18
+  # feature extraction parameters
   n_velocity_bins: 1
   use_velocity_features: True
   use_pose_features: True
   use_deep_features: True
+  # density estimation parameters
   n_components_velocity: 2
   n_neighbors_pose: 1
   n_neighbors_deep: 1
   # generic params
   normalization_method: min_max # options: [null, min_max, cdf]
 
 metrics:
```

### Comparing `anomalib-0.5.1/src/anomalib/models/ai_vad/density.py` & `anomalib-0.6.0/src/anomalib/models/ai_vad/density.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/ai_vad/features.py` & `anomalib-0.6.0/src/anomalib/models/ai_vad/features.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/ai_vad/flow.py` & `anomalib-0.6.0/src/anomalib/models/ai_vad/flow.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/ai_vad/lightning_model.py` & `anomalib-0.6.0/src/anomalib/models/ai_vad/lightning_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -19,52 +19,74 @@
 
 logger = logging.getLogger(__name__)
 
 __all__ = ["AiVad", "AiVadLightning"]
 
 
 class AiVad(AnomalyModule):
-    """PaDiM: a Patch Distribution Modeling Framework for Anomaly Detection and Localization.
+    """AI-VAD: Attribute-based Representations for Accurate and Interpretable Video Anomaly Detection.
 
     Args:
-        layers (list[str]): Layers to extract features from the backbone CNN
-        input_size (tuple[int, int]): Size of the model input.
-        backbone (str): Backbone CNN network
-        pre_trained (bool, optional): Boolean to check whether to use a pre_trained backbone.
-        n_features (int, optional): Number of features to retain in the dimension reduction step.
-                                Default values from the paper are available for: resnet18 (100), wide_resnet50_2 (550).
+        box_score_thresh (float): Confidence threshold for bounding box predictions.
+        persons_only (bool): When enabled, only regions labeled as person are included.
+        min_bbox_area (int): Minimum bounding box area. Regions with a surface area lower than this value are excluded.
+        max_bbox_overlap (float): Maximum allowed overlap between bounding boxes.
+        enable_foreground_detections (bool): Add additional foreground detections based on pixel difference between
+            consecutive frames.
+        foreground_kernel_size (int): Gaussian kernel size used in foreground detection.
+        foreground_binary_threshold (int): Value between 0 and 255 which acts as binary threshold in foreground
+            detection.
+        n_velocity_bins (int): Number of discrete bins used for velocity histogram features.
+        use_velocity_features (bool): Flag indicating if velocity features should be used.
+        use_pose_features (bool): Flag indicating if pose features should be used.
+        use_deep_features (bool): Flag indicating if deep features should be used.
+        n_components_velocity (int): Number of components used by GMM density estimation for velocity features.
+        n_neighbors_pose (int): Number of neighbors used in KNN density estimation for pose features.
+        n_neighbors_deep (int): Number of neighbors used in KNN density estimation for deep features.
     """
 
     def __init__(
         self,
         box_score_thresh: float = 0.8,
+        persons_only: bool = False,
+        min_bbox_area: int = 100,
+        max_bbox_overlap: float = 0.65,
+        enable_foreground_detections: bool = True,
+        foreground_kernel_size: int = 3,
+        foreground_binary_threshold: int = 18,
         n_velocity_bins: int = 8,
         use_velocity_features: bool = True,
         use_pose_features: bool = True,
         use_deep_features: bool = True,
         n_components_velocity: int = 5,
         n_neighbors_pose: int = 1,
         n_neighbors_deep: int = 1,
     ) -> None:
         super().__init__()
 
         self.model = AiVadModel(
             box_score_thresh=box_score_thresh,
+            persons_only=persons_only,
+            min_bbox_area=min_bbox_area,
+            max_bbox_overlap=max_bbox_overlap,
+            enable_foreground_detections=enable_foreground_detections,
+            foreground_kernel_size=foreground_kernel_size,
+            foreground_binary_threshold=foreground_binary_threshold,
             n_velocity_bins=n_velocity_bins,
             use_velocity_features=use_velocity_features,
             use_pose_features=use_pose_features,
             use_deep_features=use_deep_features,
             n_components_velocity=n_components_velocity,
             n_neighbors_pose=n_neighbors_pose,
             n_neighbors_deep=n_neighbors_deep,
         )
 
     @staticmethod
     def configure_optimizers() -> None:
-        """TAI-VAD training does not involve fine-tuning of NN weights, no optimizers needed."""
+        """AI-VAD training does not involve fine-tuning of NN weights, no optimizers needed."""
         return None
 
     def training_step(self, batch: dict[str, str | Tensor]) -> None:
         """Training Step of AI-VAD.
 
         Extract features from the batch of clips and update the density estimators.
 
@@ -99,23 +121,29 @@
         batch["box_scores"] = [score.to(self.device) for score in anomaly_scores]
         batch["pred_scores"] = Tensor(image_scores).to(self.device)
 
         return batch
 
 
 class AiVadLightning(AiVad):
-    """PaDiM: a Patch Distribution Modeling Framework for Anomaly Detection and Localization.
+    """AI-VAD: Attribute-based Representations for Accurate and Interpretable Video Anomaly Detection.
 
     Args:
         hparams (DictConfig | ListConfig): Model params
     """
 
     def __init__(self, hparams: DictConfig | ListConfig) -> None:
         super().__init__(
             box_score_thresh=hparams.model.box_score_thresh,
+            persons_only=hparams.model.persons_only,
+            min_bbox_area=hparams.model.min_bbox_area,
+            max_bbox_overlap=hparams.model.max_bbox_overlap,
+            enable_foreground_detections=hparams.model.enable_foreground_detections,
+            foreground_kernel_size=hparams.model.foreground_kernel_size,
+            foreground_binary_threshold=hparams.model.foreground_binary_threshold,
             n_velocity_bins=hparams.model.n_velocity_bins,
             use_velocity_features=hparams.model.use_velocity_features,
             use_pose_features=hparams.model.use_pose_features,
             use_deep_features=hparams.model.use_deep_features,
             n_components_velocity=hparams.model.n_components_velocity,
             n_neighbors_pose=hparams.model.n_neighbors_pose,
             n_neighbors_deep=hparams.model.n_neighbors_deep,
```

### Comparing `anomalib-0.5.1/src/anomalib/models/ai_vad/torch_model.py` & `anomalib-0.6.0/src/anomalib/models/ai_vad/torch_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,27 +18,41 @@
 
 
 class AiVadModel(nn.Module):
     """AI-VAD model.
 
     Args:
         box_score_thresh (float): Confidence threshold for region extraction stage.
+        persons_only (bool): When enabled, only regions labeled as person are included.
+        min_bbox_area (int): Minimum bounding box area. Regions with a surface area lower than this value are excluded.
+        max_bbox_overlap (float): Maximum allowed overlap between bounding boxes.
+        enable_foreground_detections (bool): Add additional foreground detections based on pixel difference between
+            consecutive frames.
+        foreground_kernel_size (int): Gaussian kernel size used in foreground detection.
+        foreground_binary_threshold (int): Value between 0 and 255 which acts as binary threshold in foreground
+            detection.
         n_velocity_bins (int): Number of discrete bins used for velocity histogram features.
         use_velocity_features (bool): Flag indicating if velocity features should be used.
         use_pose_features (bool): Flag indicating if pose features should be used.
         use_deep_features (bool): Flag indicating if deep features should be used.
         n_components_velocity (int): Number of components used by GMM density estimation for velocity features.
         n_neighbors_pose (int): Number of neighbors used in KNN density estimation for pose features.
         n_neighbors_deep (int): Number of neighbors used in KNN density estimation for deep features.
     """
 
     def __init__(
         self,
         # region-extraction params
         box_score_thresh: float = 0.8,
+        persons_only: bool = False,
+        min_bbox_area: int = 100,
+        max_bbox_overlap: float = 0.65,
+        enable_foreground_detections: bool = True,
+        foreground_kernel_size: int = 3,
+        foreground_binary_threshold: int = 18,
         # feature-extraction params
         n_velocity_bins: int = 8,
         use_velocity_features: bool = True,
         use_pose_features: bool = True,
         use_deep_features: bool = True,
         # density-estimation params
         n_components_velocity: int = 5,
@@ -48,15 +62,23 @@
         super().__init__()
         if not any((use_velocity_features, use_pose_features, use_deep_features)):
             raise ValueError("Select at least one feature type.")
 
         # initialize flow extractor
         self.flow_extractor = FlowExtractor()
         # initialize region extractor
-        self.region_extractor = RegionExtractor(box_score_thresh=box_score_thresh)
+        self.region_extractor = RegionExtractor(
+            box_score_thresh=box_score_thresh,
+            persons_only=persons_only,
+            min_bbox_area=min_bbox_area,
+            max_bbox_overlap=max_bbox_overlap,
+            enable_foreground_detections=enable_foreground_detections,
+            foreground_kernel_size=foreground_kernel_size,
+            foreground_binary_threshold=foreground_binary_threshold,
+        )
         # initialize feature extractor
         self.feature_extractor = FeatureExtractor(
             n_velocity_bins=n_velocity_bins,
             use_velocity_features=use_velocity_features,
             use_pose_features=use_pose_features,
             use_deep_features=use_deep_features,
         )
@@ -87,15 +109,15 @@
         # 1. get first and last frame from clip
         first_frame = batch[:, 0, ...]
         last_frame = batch[:, -1, ...]
 
         # 2. extract flows and regions
         with torch.no_grad():
             flows = self.flow_extractor(first_frame, last_frame)
-            regions = self.region_extractor(last_frame)
+            regions = self.region_extractor(first_frame, last_frame)
 
         # 3. extract pose, appearance and velocity features
         features_per_batch = self.feature_extractor(first_frame, flows, regions)
 
         if self.training:
             return features_per_batch
```

### Comparing `anomalib-0.5.1/src/anomalib/models/cfa/anomaly_map.py` & `anomalib-0.6.0/src/anomalib/models/cfa/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/cfa/config.yaml` & `anomalib-0.6.0/src/anomalib/models/cfa/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/cfa/lightning_model.py` & `anomalib-0.6.0/src/anomalib/models/cfa/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/cfa/loss.py` & `anomalib-0.6.0/src/anomalib/models/cfa/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/cfa/torch_model.py` & `anomalib-0.6.0/src/anomalib/models/cfa/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/cflow/anomaly_map.py` & `anomalib-0.6.0/src/anomalib/models/cflow/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/cflow/config.yaml` & `anomalib-0.6.0/src/anomalib/models/cflow/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/cflow/lightning_model.py` & `anomalib-0.6.0/src/anomalib/models/cflow/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/cflow/torch_model.py` & `anomalib-0.6.0/src/anomalib/models/cflow/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/cflow/utils.py` & `anomalib-0.6.0/src/anomalib/models/cflow/utils.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/components/__init__.py` & `anomalib-0.6.0/src/anomalib/models/components/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/components/base/anomaly_module.py` & `anomalib-0.6.0/src/anomalib/models/components/base/anomaly_module.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/components/base/dynamic_module.py` & `anomalib-0.6.0/src/anomalib/models/components/base/dynamic_module.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/components/classification/kde_classifier.py` & `anomalib-0.6.0/src/anomalib/models/components/classification/kde_classifier.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/components/dimensionality_reduction/pca.py` & `anomalib-0.6.0/src/anomalib/models/components/dimensionality_reduction/pca.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/components/dimensionality_reduction/random_projection.py` & `anomalib-0.6.0/src/anomalib/models/components/dimensionality_reduction/random_projection.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/components/feature_extractors/timm.py` & `anomalib-0.6.0/src/anomalib/models/components/feature_extractors/timm.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/components/feature_extractors/torchfx.py` & `anomalib-0.6.0/src/anomalib/models/components/feature_extractors/torchfx.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/components/feature_extractors/utils.py` & `anomalib-0.6.0/src/anomalib/models/components/feature_extractors/utils.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/components/filters/blur.py` & `anomalib-0.6.0/src/anomalib/models/components/filters/blur.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/components/flow/all_in_one_block.py` & `anomalib-0.6.0/src/anomalib/models/components/flow/all_in_one_block.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/components/layers/sspcab.py` & `anomalib-0.6.0/src/anomalib/models/components/layers/sspcab.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/components/sampling/k_center_greedy.py` & `anomalib-0.6.0/src/anomalib/models/components/sampling/k_center_greedy.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/components/stats/kde.py` & `anomalib-0.6.0/src/anomalib/models/components/stats/kde.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/components/stats/multi_variate_gaussian.py` & `anomalib-0.6.0/src/anomalib/models/components/stats/multi_variate_gaussian.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/csflow/anomaly_map.py` & `anomalib-0.6.0/src/anomalib/models/csflow/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/csflow/config.yaml` & `anomalib-0.6.0/src/anomalib/models/csflow/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/csflow/lightning_model.py` & `anomalib-0.6.0/src/anomalib/models/csflow/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/csflow/loss.py` & `anomalib-0.6.0/src/anomalib/models/csflow/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/csflow/torch_model.py` & `anomalib-0.6.0/src/anomalib/models/csflow/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/dfkde/config.yaml` & `anomalib-0.6.0/src/anomalib/models/dfkde/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/dfkde/lightning_model.py` & `anomalib-0.6.0/src/anomalib/models/dfkde/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/dfkde/torch_model.py` & `anomalib-0.6.0/src/anomalib/models/dfkde/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/dfm/config.yaml` & `anomalib-0.6.0/src/anomalib/models/dfm/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/dfm/lightning_model.py` & `anomalib-0.6.0/src/anomalib/models/dfm/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/dfm/torch_model.py` & `anomalib-0.6.0/src/anomalib/models/dfm/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/draem/config.yaml` & `anomalib-0.6.0/src/anomalib/models/draem/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/draem/lightning_model.py` & `anomalib-0.6.0/src/anomalib/models/draem/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/draem/loss.py` & `anomalib-0.6.0/src/anomalib/models/draem/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/draem/torch_model.py` & `anomalib-0.6.0/src/anomalib/models/draem/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/fastflow/anomaly_map.py` & `anomalib-0.6.0/src/anomalib/models/fastflow/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/fastflow/config.yaml` & `anomalib-0.6.0/src/anomalib/models/fastflow/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/fastflow/lightning_model.py` & `anomalib-0.6.0/src/anomalib/models/fastflow/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/fastflow/loss.py` & `anomalib-0.6.0/src/anomalib/models/fastflow/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/fastflow/torch_model.py` & `anomalib-0.6.0/src/anomalib/models/fastflow/torch_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,18 +37,23 @@
 
     Returns:
         Callable: Sequential for the subnet constructor.
     """
 
     def subnet_conv(in_channels: int, out_channels: int) -> nn.Sequential:
         hidden_channels = int(in_channels * hidden_ratio)
+        # NOTE: setting padding="same" in nn.Conv2d breaks the onnx export so manual padding required.
+        # TODO: Use padding="same" in nn.Conv2d once PyTorch v2.1 is released
+        padding = 2 * (kernel_size // 2 - ((1 + kernel_size) % 2), kernel_size // 2)
         return nn.Sequential(
-            nn.Conv2d(in_channels, hidden_channels, kernel_size, padding="same"),
+            nn.ZeroPad2d(padding),
+            nn.Conv2d(in_channels, hidden_channels, kernel_size),
             nn.ReLU(),
-            nn.Conv2d(hidden_channels, out_channels, kernel_size, padding="same"),
+            nn.ZeroPad2d(padding),
+            nn.Conv2d(hidden_channels, out_channels, kernel_size),
         )
 
     return subnet_conv
 
 
 def create_fast_flow_block(
     input_dimensions: list[int],
```

### Comparing `anomalib-0.5.1/src/anomalib/models/ganomaly/config.yaml` & `anomalib-0.6.0/src/anomalib/models/ganomaly/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/ganomaly/lightning_model.py` & `anomalib-0.6.0/src/anomalib/models/ganomaly/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/ganomaly/loss.py` & `anomalib-0.6.0/src/anomalib/models/ganomaly/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/ganomaly/torch_model.py` & `anomalib-0.6.0/src/anomalib/models/ganomaly/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/padim/anomaly_map.py` & `anomalib-0.6.0/src/anomalib/models/padim/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/padim/config.yaml` & `anomalib-0.6.0/src/anomalib/models/padim/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/padim/lightning_model.py` & `anomalib-0.6.0/src/anomalib/models/padim/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/padim/torch_model.py` & `anomalib-0.6.0/src/anomalib/models/padim/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/patchcore/anomaly_map.py` & `anomalib-0.6.0/src/anomalib/models/patchcore/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/patchcore/config.yaml` & `anomalib-0.6.0/src/anomalib/models/patchcore/config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 dataset:
   name: mvtec
   format: mvtec
   path: ./datasets/MVTec
   task: segmentation
   category: bottle
   train_batch_size: 32
-  test_batch_size: 32
+  eval_batch_size: 32
   num_workers: 8
   image_size: 256 # dimensions to which images are resized (mandatory)
   center_crop: 224 # dimensions to which images are center-cropped after resizing (optional)
   normalization: imagenet # data distribution to which the images will be normalized: [none, imagenet]
   transform_config:
     train: null
     eval: null
```

### Comparing `anomalib-0.5.1/src/anomalib/models/patchcore/lightning_model.py` & `anomalib-0.6.0/src/anomalib/models/patchcore/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/patchcore/torch_model.py` & `anomalib-0.6.0/src/anomalib/models/patchcore/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/reverse_distillation/anomaly_map.py` & `anomalib-0.6.0/src/anomalib/models/reverse_distillation/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/reverse_distillation/components/__init__.py` & `anomalib-0.6.0/src/anomalib/models/reverse_distillation/components/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/reverse_distillation/components/bottleneck.py` & `anomalib-0.6.0/src/anomalib/models/reverse_distillation/components/bottleneck.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/reverse_distillation/components/de_resnet.py` & `anomalib-0.6.0/src/anomalib/models/reverse_distillation/components/de_resnet.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/reverse_distillation/config.yaml` & `anomalib-0.6.0/src/anomalib/models/reverse_distillation/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/reverse_distillation/lightning_model.py` & `anomalib-0.6.0/src/anomalib/models/reverse_distillation/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/reverse_distillation/loss.py` & `anomalib-0.6.0/src/anomalib/models/reverse_distillation/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/reverse_distillation/torch_model.py` & `anomalib-0.6.0/src/anomalib/models/reverse_distillation/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/rkde/config.yaml` & `anomalib-0.6.0/src/anomalib/models/rkde/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/rkde/feature_extractor.py` & `anomalib-0.6.0/src/anomalib/models/rkde/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/rkde/lightning_model.py` & `anomalib-0.6.0/src/anomalib/models/rkde/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/rkde/region_extractor.py` & `anomalib-0.6.0/src/anomalib/models/rkde/region_extractor.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/rkde/torch_model.py` & `anomalib-0.6.0/src/anomalib/models/rkde/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/stfpm/anomaly_map.py` & `anomalib-0.6.0/src/anomalib/models/stfpm/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/stfpm/config.yaml` & `anomalib-0.6.0/src/anomalib/models/stfpm/config.yaml`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/stfpm/lightning_model.py` & `anomalib-0.6.0/src/anomalib/models/stfpm/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/stfpm/loss.py` & `anomalib-0.6.0/src/anomalib/models/stfpm/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/models/stfpm/torch_model.py` & `anomalib-0.6.0/src/anomalib/models/stfpm/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/post_processing/__init__.py` & `anomalib-0.6.0/src/anomalib/post_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/post_processing/normalization/cdf.py` & `anomalib-0.6.0/src/anomalib/post_processing/normalization/cdf.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/post_processing/normalization/min_max.py` & `anomalib-0.6.0/src/anomalib/post_processing/normalization/min_max.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/post_processing/post_process.py` & `anomalib-0.6.0/src/anomalib/post_processing/post_process.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/post_processing/visualizer.py` & `anomalib-0.6.0/src/anomalib/post_processing/visualizer.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/pre_processing/pre_process.py` & `anomalib-0.6.0/src/anomalib/pre_processing/pre_process.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/pre_processing/tiler.py` & `anomalib-0.6.0/src/anomalib/pre_processing/tiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,15 +342,15 @@
     def tile(self, image: Tensor, use_random_tiling: bool | None = False) -> Tensor:
         """Tiles an input image to either overlapping, non-overlapping or random patches.
 
         Args:
             image: Input image to tile.
 
         Examples:
-            >>> from anomalib.data.tiler import Tiler
+            >>> from anomalib.pre_processing import Tiler
             >>> tiler = Tiler(tile_size=512,stride=256)
             >>> image = torch.rand(size=(2, 3, 1024, 1024))
             >>> image.shape
             torch.Size([2, 3, 1024, 1024])
             >>> tiles = tiler.tile(image)
             >>> tiles.shape
             torch.Size([18, 3, 512, 512])
@@ -389,15 +389,15 @@
         If patches, are overlapping patches, the function averages the overlapping pixels,
         and return the reconstructed image.
 
         Args:
             tiles: Tiles from the input image, generated via tile()..
 
         Examples:
-            >>> from anomalib.datasets.tiler import Tiler
+            >>> from anomalib.pre_processing import Tiler
             >>> tiler = Tiler(tile_size=512,stride=256)
             >>> image = torch.rand(size=(2, 3, 1024, 1024))
             >>> image.shape
             torch.Size([2, 3, 1024, 1024])
             >>> tiles = tiler.tile(image)
             >>> tiles.shape
             torch.Size([18, 3, 512, 512])
```

### Comparing `anomalib-0.5.1/src/anomalib/pre_processing/transforms/custom.py` & `anomalib-0.6.0/src/anomalib/pre_processing/transforms/custom.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/callbacks/__init__.py` & `anomalib-0.6.0/src/anomalib/utils/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/callbacks/cdf_normalization.py` & `anomalib-0.6.0/src/anomalib/utils/callbacks/cdf_normalization.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/callbacks/export.py` & `anomalib-0.6.0/src/anomalib/utils/callbacks/export.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/callbacks/graph.py` & `anomalib-0.6.0/src/anomalib/utils/callbacks/graph.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/callbacks/metrics_configuration.py` & `anomalib-0.6.0/src/anomalib/utils/callbacks/metrics_configuration.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/callbacks/min_max_normalization.py` & `anomalib-0.6.0/src/anomalib/utils/callbacks/min_max_normalization.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/callbacks/model_loader.py` & `anomalib-0.6.0/src/anomalib/utils/callbacks/model_loader.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/callbacks/nncf/callback.py` & `anomalib-0.6.0/src/anomalib/utils/callbacks/nncf/callback.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/callbacks/nncf/utils.py` & `anomalib-0.6.0/src/anomalib/utils/callbacks/nncf/utils.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/callbacks/post_processing_configuration.py` & `anomalib-0.6.0/src/anomalib/utils/callbacks/post_processing_configuration.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/callbacks/tiler_configuration.py` & `anomalib-0.6.0/src/anomalib/utils/callbacks/tiler_configuration.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/callbacks/timer.py` & `anomalib-0.6.0/src/anomalib/utils/callbacks/timer.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/callbacks/visualizer/visualizer_base.py` & `anomalib-0.6.0/src/anomalib/utils/callbacks/visualizer/visualizer_base.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/callbacks/visualizer/visualizer_image.py` & `anomalib-0.6.0/src/anomalib/utils/callbacks/visualizer/visualizer_image.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/callbacks/visualizer/visualizer_metric.py` & `anomalib-0.6.0/src/anomalib/utils/callbacks/visualizer/visualizer_metric.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/cli/cli.py` & `anomalib-0.6.0/src/anomalib/utils/cli/cli.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/cv/connected_components.py` & `anomalib-0.6.0/src/anomalib/utils/cv/connected_components.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/hpo/config.py` & `anomalib-0.6.0/src/anomalib/utils/hpo/config.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/hpo/runners.py` & `anomalib-0.6.0/src/anomalib/utils/hpo/runners.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/loggers/__init__.py` & `anomalib-0.6.0/src/anomalib/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/loggers/base.py` & `anomalib-0.6.0/src/anomalib/utils/loggers/base.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/loggers/comet.py` & `anomalib-0.6.0/src/anomalib/utils/loggers/comet.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/loggers/tensorboard.py` & `anomalib-0.6.0/src/anomalib/utils/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/loggers/wandb.py` & `anomalib-0.6.0/src/anomalib/utils/loggers/wandb.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/metrics/__init__.py` & `anomalib-0.6.0/src/anomalib/utils/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/metrics/anomaly_score_distribution.py` & `anomalib-0.6.0/src/anomalib/utils/metrics/anomaly_score_distribution.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/metrics/anomaly_score_threshold.py` & `anomalib-0.6.0/src/anomalib/utils/metrics/anomaly_score_threshold.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/metrics/aupr.py` & `anomalib-0.6.0/src/anomalib/utils/metrics/aupr.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/metrics/aupro.py` & `anomalib-0.6.0/src/anomalib/utils/metrics/aupro.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/metrics/auroc.py` & `anomalib-0.6.0/src/anomalib/utils/metrics/auroc.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/metrics/collection.py` & `anomalib-0.6.0/src/anomalib/utils/metrics/collection.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/metrics/min_max.py` & `anomalib-0.6.0/src/anomalib/utils/metrics/min_max.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/metrics/optimal_f1.py` & `anomalib-0.6.0/src/anomalib/utils/metrics/optimal_f1.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/metrics/plotting_utils.py` & `anomalib-0.6.0/src/anomalib/utils/metrics/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/metrics/pro.py` & `anomalib-0.6.0/src/anomalib/utils/metrics/pro.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/sweep/config.py` & `anomalib-0.6.0/src/anomalib/utils/sweep/config.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/sweep/helpers/callbacks.py` & `anomalib-0.6.0/src/anomalib/utils/sweep/helpers/callbacks.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib/utils/sweep/helpers/inference.py` & `anomalib-0.6.0/src/anomalib/utils/sweep/helpers/inference.py`

 * *Files identical despite different names*

### Comparing `anomalib-0.5.1/src/anomalib.egg-info/PKG-INFO` & `anomalib-0.6.0/src/anomalib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anomalib
-Version: 0.5.1
+Version: 0.6.0
 Summary: anomalib - Anomaly Detection Library
 Home-page: 
 Author: Intel OpenVINO
 Author-email: help@openvino.intel.com
 License: Copyright (c) Intel - All Rights Reserved. Licensed under the Apache License, Version 2.0 (the "License")See LICENSE file for more details.
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `anomalib-0.5.1/src/anomalib.egg-info/SOURCES.txt` & `anomalib-0.6.0/src/anomalib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,18 @@
 src/anomalib/models/dfm/lightning_model.py
 src/anomalib/models/dfm/torch_model.py
 src/anomalib/models/draem/__init__.py
 src/anomalib/models/draem/config.yaml
 src/anomalib/models/draem/lightning_model.py
 src/anomalib/models/draem/loss.py
 src/anomalib/models/draem/torch_model.py
+src/anomalib/models/efficientad/__init__.py
+src/anomalib/models/efficientad/config.yaml
+src/anomalib/models/efficientad/lightning_model.py
+src/anomalib/models/efficientad/torch_model.py
 src/anomalib/models/fastflow/__init__.py
 src/anomalib/models/fastflow/anomaly_map.py
 src/anomalib/models/fastflow/config.yaml
 src/anomalib/models/fastflow/lightning_model.py
 src/anomalib/models/fastflow/loss.py
 src/anomalib/models/fastflow/torch_model.py
 src/anomalib/models/ganomaly/__init__.py
```

### Comparing `anomalib-0.5.1/src/anomalib.egg-info/requires.txt` & `anomalib-0.6.0/src/anomalib.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 tensorboard
 wandb==0.12.17
 GitPython
 ipykernel
 ipywidgets
 notebook
 defusedxml==0.7.1
-requests==2.26.0
+requests>=2.26.0
 networkx~=2.5
 nncf>=2.1.0
 onnx>=1.10.1
 openvino-dev>=2022.3.0
 
 [loggers]
 comet-ml>=3.31.7
@@ -41,12 +41,12 @@
 gitpython
 ipykernel
 ipywidgets
 notebook
 
 [openvino]
 defusedxml==0.7.1
-requests==2.26.0
+requests>=2.26.0
 networkx~=2.5
 nncf>=2.1.0
 onnx>=1.10.1
 openvino-dev>=2022.3.0
```

