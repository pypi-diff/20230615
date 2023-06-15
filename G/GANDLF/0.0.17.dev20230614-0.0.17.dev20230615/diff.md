# Comparing `tmp/GANDLF-0.0.17.dev20230614.tar.gz` & `tmp/GANDLF-0.0.17.dev20230615.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GANDLF-0.0.17.dev20230614.tar", last modified: Wed Jun 14 03:12:42 2023, max compression
+gzip compressed data, was "GANDLF-0.0.17.dev20230615.tar", last modified: Thu Jun 15 03:12:54 2023, max compression
```

## Comparing `GANDLF-0.0.17.dev20230614.tar` & `GANDLF-0.0.17.dev20230615.tar`

### file list

```diff
@@ -1,172 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:12:42.996036 GANDLF-0.0.17.dev20230614/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/Dockerfile-CPU
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/Dockerfile-CUDA11.6
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/Dockerfile-ROCm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:12:42.952035 GANDLF-0.0.17.dev20230614/GANDLF/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:12:42.956035 GANDLF-0.0.17.dev20230614/GANDLF/anonymize/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/anonymize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/anonymize/convert_to_nifti.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:12:42.960035 GANDLF-0.0.17.dev20230614/GANDLF/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/cli/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/cli/generate_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/cli/main_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/cli/patch_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/cli/post_training_model_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/cli/preprocess_and_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/cli/recover_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:12:42.960035 GANDLF-0.0.17.dev20230614/GANDLF/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/compute/forward_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/compute/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/compute/inference_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/compute/loss_and_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/compute/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/compute/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:12:42.960035 GANDLF-0.0.17.dev20230614/GANDLF/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/ImagesFromDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:12:42.964035 GANDLF-0.0.17.dev20230614/GANDLF/data/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/augmentation/blur_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/augmentation/noise_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/augmentation/rgb_augs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/augmentation/rotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/augmentation/wrap_torchio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/inference_dataloader_histopath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:12:42.964035 GANDLF-0.0.17.dev20230614/GANDLF/data/patch_miner/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/patch_miner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:12:42.964035 GANDLF-0.0.17.dev20230614/GANDLF/data/patch_miner/opm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/patch_miner/opm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/patch_miner/opm/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    21747 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/patch_miner/opm/patch_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/patch_miner/opm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:12:42.968036 GANDLF-0.0.17.dev20230614/GANDLF/data/post_process/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/post_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/post_process/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/post_process/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:12:42.968036 GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/crop_zero_planes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/non_zero_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/normalize_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/resample_minimum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/rgb_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:12:42.972036 GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/template_matching/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/template_matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/template_matching/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/template_matching/histogram_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/template_matching/stain_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/template_matching/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/threshold_and_clip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:12:42.972036 GANDLF-0.0.17.dev20230614/GANDLF/grad_clipping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/grad_clipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/grad_clipping/adaptive_gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/grad_clipping/clip_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/grad_clipping/grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/inference_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:12:42.972036 GANDLF-0.0.17.dev20230614/GANDLF/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/losses/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/losses/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/losses/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:12:42.976036 GANDLF-0.0.17.dev20230614/GANDLF/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/metrics/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/metrics/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:12:42.984036 GANDLF-0.0.17.dev20230614/GANDLF/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/MSDNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/brain_age.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/deep_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/imagenet_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/imagenet_vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/light_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/light_unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/modelBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/sdnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:12:42.988036 GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/DecodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/DownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/EncodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/FCNUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/IncConv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/IncDownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/IncDropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/IncUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/InceptionModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/InitialConv.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/Interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/ResNetModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/UpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/add_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/add_downsample_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/average_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/out_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/transunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/uinc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/models/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:12:42.988036 GANDLF-0.0.17.dev20230614/GANDLF/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/optimizers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    29587 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/parseConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:12:42.992036 GANDLF-0.0.17.dev20230614/GANDLF/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/schedulers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/training_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:12:42.992036 GANDLF-0.0.17.dev20230614/GANDLF/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/utils/handle_collisions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/utils/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/utils/modelbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/utils/modelio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/utils/parameter_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/utils/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/GANDLF/utils/write_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 03:12:36.000000 GANDLF-0.0.17.dev20230614/GANDLF/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:12:42.956035 GANDLF-0.0.17.dev20230614/GANDLF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-06-14 03:12:42.000000 GANDLF-0.0.17.dev20230614/GANDLF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-06-14 03:12:42.000000 GANDLF-0.0.17.dev20230614/GANDLF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 03:12:42.000000 GANDLF-0.0.17.dev20230614/GANDLF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 03:10:31.000000 GANDLF-0.0.17.dev20230614/GANDLF.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-14 03:12:42.000000 GANDLF-0.0.17.dev20230614/GANDLF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 03:12:42.000000 GANDLF-0.0.17.dev20230614/GANDLF.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-06-14 03:12:42.992036 GANDLF-0.0.17.dev20230614/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/gandlf_anonymizer
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/gandlf_collectStats
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/gandlf_configGenerator
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/gandlf_constructCSV
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/gandlf_deploy
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/gandlf_generateMetrics
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/gandlf_optimizeModel
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/gandlf_patchMiner
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/gandlf_preprocess
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/gandlf_recoverConfig
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/gandlf_run
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/gandlf_verifyInstall
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 03:12:42.996036 GANDLF-0.0.17.dev20230614/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-06-14 03:10:13.000000 GANDLF-0.0.17.dev20230614/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.025174 GANDLF-0.0.17.dev20230615/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/Dockerfile-CPU
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/Dockerfile-CUDA11.6
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/Dockerfile-ROCm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:53.993174 GANDLF-0.0.17.dev20230615/GANDLF/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:53.993174 GANDLF-0.0.17.dev20230615/GANDLF/anonymize/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/anonymize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/anonymize/convert_to_nifti.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:53.997174 GANDLF-0.0.17.dev20230615/GANDLF/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/cli/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/cli/generate_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/cli/main_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/cli/patch_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/cli/post_training_model_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/cli/preprocess_and_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/cli/recover_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:53.997174 GANDLF-0.0.17.dev20230615/GANDLF/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/compute/forward_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/compute/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/compute/inference_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/compute/loss_and_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/compute/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/compute/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:53.997174 GANDLF-0.0.17.dev20230615/GANDLF/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/ImagesFromDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.001174 GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/blur_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/noise_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/rgb_augs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/rotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/wrap_torchio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/inference_dataloader_histopath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.001174 GANDLF-0.0.17.dev20230615/GANDLF/data/patch_miner/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/patch_miner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.001174 GANDLF-0.0.17.dev20230615/GANDLF/data/patch_miner/opm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/patch_miner/opm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/patch_miner/opm/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21747 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/patch_miner/opm/patch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/patch_miner/opm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.001174 GANDLF-0.0.17.dev20230615/GANDLF/data/post_process/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/post_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/post_process/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/post_process/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.005174 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/crop_zero_planes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/non_zero_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/normalize_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/resample_minimum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/rgb_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.005174 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/histogram_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/stain_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/threshold_and_clip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.005174 GANDLF-0.0.17.dev20230615/GANDLF/grad_clipping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/grad_clipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/grad_clipping/adaptive_gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/grad_clipping/clip_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/grad_clipping/grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/inference_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.009174 GANDLF-0.0.17.dev20230615/GANDLF/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/losses/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/losses/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/losses/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.009174 GANDLF-0.0.17.dev20230615/GANDLF/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/metrics/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/metrics/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/metrics/synthesis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.017174 GANDLF-0.0.17.dev20230615/GANDLF/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/MSDNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/brain_age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/deep_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/imagenet_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/imagenet_vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/light_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/light_unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/modelBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/sdnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.021174 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/DecodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/DownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/EncodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/FCNUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/IncConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/IncDownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/IncDropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/IncUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/InceptionModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/InitialConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/Interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/ResNetModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/UpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/add_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/add_downsample_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/average_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/out_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/transunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/uinc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/models/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.021174 GANDLF-0.0.17.dev20230615/GANDLF/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/optimizers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29587 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/parseConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.021174 GANDLF-0.0.17.dev20230615/GANDLF/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/schedulers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/training_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:54.025174 GANDLF-0.0.17.dev20230615/GANDLF/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/utils/handle_collisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/utils/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/utils/modelbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/utils/modelio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/utils/parameter_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/utils/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/GANDLF/utils/write_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 03:12:47.000000 GANDLF-0.0.17.dev20230615/GANDLF/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:12:53.993174 GANDLF-0.0.17.dev20230615/GANDLF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-06-15 03:12:53.000000 GANDLF-0.0.17.dev20230615/GANDLF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-06-15 03:12:53.000000 GANDLF-0.0.17.dev20230615/GANDLF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 03:12:53.000000 GANDLF-0.0.17.dev20230615/GANDLF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 03:10:37.000000 GANDLF-0.0.17.dev20230615/GANDLF.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-15 03:12:53.000000 GANDLF-0.0.17.dev20230615/GANDLF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 03:12:53.000000 GANDLF-0.0.17.dev20230615/GANDLF.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-06-15 03:12:54.025174 GANDLF-0.0.17.dev20230615/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_anonymizer
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_collectStats
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_configGenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_constructCSV
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_deploy
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_generateMetrics
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_optimizeModel
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_patchMiner
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_preprocess
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_recoverConfig
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_run
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/gandlf_verifyInstall
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 03:12:54.025174 GANDLF-0.0.17.dev20230615/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-15 03:10:15.000000 GANDLF-0.0.17.dev20230615/setup.py
```

### Comparing `GANDLF-0.0.17.dev20230614/CODE_OF_CONDUCT.md` & `GANDLF-0.0.17.dev20230615/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/CONTRIBUTING.md` & `GANDLF-0.0.17.dev20230615/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/Dockerfile-CPU` & `GANDLF-0.0.17.dev20230615/Dockerfile-CPU`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/Dockerfile-CUDA11.6` & `GANDLF-0.0.17.dev20230615/Dockerfile-CUDA11.6`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/Dockerfile-ROCm` & `GANDLF-0.0.17.dev20230615/Dockerfile-ROCm`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/anonymize/__init__.py` & `GANDLF-0.0.17.dev20230615/GANDLF/anonymize/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/anonymize/convert_to_nifti.py` & `GANDLF-0.0.17.dev20230615/GANDLF/anonymize/convert_to_nifti.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/cli/__init__.py` & `GANDLF-0.0.17.dev20230615/GANDLF/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/cli/config_generator.py` & `GANDLF-0.0.17.dev20230615/GANDLF/cli/config_generator.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/cli/deploy.py` & `GANDLF-0.0.17.dev20230615/GANDLF/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/cli/main_run.py` & `GANDLF-0.0.17.dev20230615/GANDLF/cli/main_run.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/cli/patch_extraction.py` & `GANDLF-0.0.17.dev20230615/GANDLF/cli/patch_extraction.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/cli/post_training_model_optimization.py` & `GANDLF-0.0.17.dev20230615/GANDLF/cli/post_training_model_optimization.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/cli/preprocess_and_save.py` & `GANDLF-0.0.17.dev20230615/GANDLF/cli/preprocess_and_save.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/cli/recover_config.py` & `GANDLF-0.0.17.dev20230615/GANDLF/cli/recover_config.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/compute/forward_pass.py` & `GANDLF-0.0.17.dev20230615/GANDLF/compute/forward_pass.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/compute/generic.py` & `GANDLF-0.0.17.dev20230615/GANDLF/compute/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/compute/inference_loop.py` & `GANDLF-0.0.17.dev20230615/GANDLF/compute/inference_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/compute/loss_and_metric.py` & `GANDLF-0.0.17.dev20230615/GANDLF/compute/loss_and_metric.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/compute/step.py` & `GANDLF-0.0.17.dev20230615/GANDLF/compute/step.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/compute/training_loop.py` & `GANDLF-0.0.17.dev20230615/GANDLF/compute/training_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/ImagesFromDataFrame.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/ImagesFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/__init__.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/augmentation/__init__.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/augmentation/blur_enhanced.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/blur_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/augmentation/noise_enhanced.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/noise_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/augmentation/rgb_augs.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/rgb_augs.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/augmentation/rotations.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/rotations.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/augmentation/wrap_torchio.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/augmentation/wrap_torchio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/inference_dataloader_histopath.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/inference_dataloader_histopath.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/patch_miner/opm/patch.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/patch_miner/opm/patch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/patch_miner/opm/patch_manager.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/patch_miner/opm/patch_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/patch_miner/opm/utils.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/patch_miner/opm/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/post_process/morphology.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/post_process/morphology.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/post_process/tensor.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/post_process/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/__init__.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/crop_zero_planes.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/crop_zero_planes.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/non_zero_normalize.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/non_zero_normalize.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/normalize_rgb.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/normalize_rgb.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/resample_minimum.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/resample_minimum.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/rgb_conversion.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/rgb_conversion.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/template_matching/base.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/base.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/template_matching/histogram_matching.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/histogram_matching.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/template_matching/stain_extractors.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/stain_extractors.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/template_matching/stain_normalizer.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/stain_normalizer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/template_matching/utils.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/template_matching/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/data/preprocessing/threshold_and_clip.py` & `GANDLF-0.0.17.dev20230615/GANDLF/data/preprocessing/threshold_and_clip.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/grad_clipping/adaptive_gradient_clipping.py` & `GANDLF-0.0.17.dev20230615/GANDLF/grad_clipping/adaptive_gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/grad_clipping/clip_gradients.py` & `GANDLF-0.0.17.dev20230615/GANDLF/grad_clipping/clip_gradients.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/grad_clipping/grad_scaler.py` & `GANDLF-0.0.17.dev20230615/GANDLF/grad_clipping/grad_scaler.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/inference_manager.py` & `GANDLF-0.0.17.dev20230615/GANDLF/inference_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/logger.py` & `GANDLF-0.0.17.dev20230615/GANDLF/logger.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/losses/__init__.py` & `GANDLF-0.0.17.dev20230615/GANDLF/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/losses/hybrid.py` & `GANDLF-0.0.17.dev20230615/GANDLF/losses/hybrid.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/losses/regression.py` & `GANDLF-0.0.17.dev20230615/GANDLF/losses/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/losses/segmentation.py` & `GANDLF-0.0.17.dev20230615/GANDLF/losses/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/metrics/__init__.py` & `GANDLF-0.0.17.dev20230615/GANDLF/metrics/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,25 @@
     recall_score,
     precision_score,
     iou_score,
     f1_score,
     accuracy,
     specificity_score,
 )
+from .synthesis import (
+    structural_similarity_index,
+    mean_squared_error,
+    peak_signal_noise_ratio,
+    mean_squared_log_error,
+    mean_absolute_error,
+    ncc_mean,
+    ncc_std,
+    ncc_max,
+    ncc_min,
+)
 import GANDLF.metrics.classification as classification
 import GANDLF.metrics.regression as regression
 
 
 # global defines for the metrics
 global_metrics_dict = {
     "dice": multi_class_dice,
```

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/metrics/classification.py` & `GANDLF-0.0.17.dev20230615/GANDLF/metrics/classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             ),
             "precision": tm.Precision(
                 num_classes=params["model"]["num_classes"], average=average_type_key
             ),
             "recall": tm.Recall(
                 num_classes=params["model"]["num_classes"], average=average_type_key
             ),
-            "f1": tm.F1(
+            "f1": tm.F1Score(
                 num_classes=params["model"]["num_classes"], average=average_type_key
             ),
             "specificity": tm.Specificity(
                 num_classes=params["model"]["num_classes"], average=average_type_key
             ),
             ## weird error for multi-class problem, where pos_label is not getting set
             # "aucroc": tm.AUROC(
```

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/metrics/generic.py` & `GANDLF-0.0.17.dev20230615/GANDLF/metrics/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import torch
-from torchmetrics import F1, Precision, Recall, IoU, Accuracy, Specificity
+from torchmetrics import F1Score, Precision, Recall, JaccardIndex, Accuracy, Specificity
 from GANDLF.utils.tensor import one_hot
 
 
 def generic_function_output_with_check(predicted_classes, label, metric_function):
     if torch.min(predicted_classes) < 0:
         print(
             "WARNING: Negative values detected in prediction, cannot compute torchmetrics calculations."
@@ -45,15 +45,15 @@
 
 
 def precision_score(output, label, params):
     return generic_torchmetrics_score(output, label, Precision, "precision", params)
 
 
 def f1_score(output, label, params):
-    return generic_torchmetrics_score(output, label, F1, "f1", params)
+    return generic_torchmetrics_score(output, label, F1Score, "f1", params)
 
 
 def accuracy(output, label, params):
     return generic_torchmetrics_score(output, label, Accuracy, "accuracy", params)
 
 
 def specificity_score(output, label, params):
@@ -64,15 +64,15 @@
     num_classes = params["model"]["num_classes"]
     predicted_classes = output
     if params["problem_type"] == "classification":
         predicted_classes = torch.argmax(output, 1)
     elif params["problem_type"] == "segmentation":
         label = one_hot(label, params["model"]["class_list"])
 
-    recall = IoU(
+    recall = JaccardIndex(
         reduction=params["metrics"]["iou"]["reduction"],
         num_classes=num_classes,
         threshold=params["metrics"]["iou"]["threshold"],
     )
 
     return generic_function_output_with_check(
         predicted_classes.cpu().int(), label.cpu().int(), recall
```

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/metrics/regression.py` & `GANDLF-0.0.17.dev20230615/GANDLF/metrics/regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,16 +111,16 @@
             output_metrics[
                 f"{metric_name}_{reduction_type}"
             ] = get_output_from_calculator(predictions, ground_truth, calculator)
     # metrics that do not have any "reduction" parameter
     calculators = {
         "mse": tm.MeanSquaredError(),
         "mae": tm.MeanAbsoluteError(),
-        "pearson": tm.PearsonCorrcoef(),
-        "spearman": tm.SpearmanCorrcoef(),
+        "pearson": tm.PearsonCorrCoef(),
+        "spearman": tm.SpearmanCorrCoef(),
     }
     for metric_name, calculator in calculators.items():
         output_metrics[metric_name] = get_output_from_calculator(
             predictions, ground_truth, calculator
         )
 
     return output_metrics
```

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/metrics/segmentation.py` & `GANDLF-0.0.17.dev20230615/GANDLF/metrics/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/MSDNet.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/MSDNet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/__init__.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/brain_age.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/brain_age.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/deep_unet.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/deep_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/densenet.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/densenet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/efficientnet.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/fcn.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/fcn.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/imagenet_unet.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/imagenet_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/imagenet_vgg.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/imagenet_vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/light_unet.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/light_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/light_unet_multilayer.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/light_unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/modelBase.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/modelBase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/resnet.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/resnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/sdnet.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/sdnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/DecodingModule.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/DecodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/DownsamplingModule.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/DownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/EncodingModule.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/EncodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/FCNUpsamplingModule.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/FCNUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/IncConv.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/IncConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/IncDownsamplingModule.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/IncDownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/IncDropout.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/IncDropout.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/IncUpsamplingModule.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/IncUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/InceptionModule.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/InceptionModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/InitialConv.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/InitialConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/Interpolate.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/Interpolate.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/ResNetModule.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/ResNetModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/UpsamplingModule.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/UpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/add_conv_block.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/add_conv_block.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/average_pool.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/average_pool.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/seg_modules/out_conv.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/seg_modules/out_conv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/transunet.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/transunet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/uinc.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/uinc.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/unet.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/unet_multilayer.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/unetr.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/unetr.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/models/vgg.py` & `GANDLF-0.0.17.dev20230615/GANDLF/models/vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/optimizers/__init__.py` & `GANDLF-0.0.17.dev20230615/GANDLF/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/optimizers/wrap_torch.py` & `GANDLF-0.0.17.dev20230615/GANDLF/optimizers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/parseConfig.py` & `GANDLF-0.0.17.dev20230615/GANDLF/parseConfig.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/schedulers/__init__.py` & `GANDLF-0.0.17.dev20230615/GANDLF/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/schedulers/wrap_torch.py` & `GANDLF-0.0.17.dev20230615/GANDLF/schedulers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/training_manager.py` & `GANDLF-0.0.17.dev20230615/GANDLF/training_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/utils/__init__.py` & `GANDLF-0.0.17.dev20230615/GANDLF/utils/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     get_class_imbalance_weights,
     get_class_imbalance_weights_segmentation,
     get_class_imbalance_weights_classification,
     get_linear_interpolation_mode,
     print_model_summary,
     get_ground_truths_and_predictions_tensor,
     get_output_from_calculator,
+    get_tensor_from_image,
+    get_image_from_tensor,
 )
 
 from .write_parse import (
     writeTrainingCSV,
     parseTrainingCSV,
     parseTestingCSV,
     get_dataframe,
```

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/utils/generic.py` & `GANDLF-0.0.17.dev20230615/GANDLF/utils/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/utils/handle_collisions.py` & `GANDLF-0.0.17.dev20230615/GANDLF/utils/handle_collisions.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/utils/imaging.py` & `GANDLF-0.0.17.dev20230615/GANDLF/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/utils/modelbase.py` & `GANDLF-0.0.17.dev20230615/GANDLF/utils/modelbase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/utils/modelio.py` & `GANDLF-0.0.17.dev20230615/GANDLF/utils/modelio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/utils/parameter_processing.py` & `GANDLF-0.0.17.dev20230615/GANDLF/utils/parameter_processing.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/utils/tensor.py` & `GANDLF-0.0.17.dev20230615/GANDLF/utils/tensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os, sys
+from typing import Union
 import numpy as np
+import SimpleITK as sitk
 import torch
 import torch.nn as nn
 from torch.utils.data import DataLoader
 import torchio
 from tqdm import tqdm
 from torchinfo import summary
 from GANDLF.utils.generic import get_array_from_image_or_tensor
@@ -490,7 +492,42 @@
     """
     temp_output = calculator(predictions, ground_truth)
     if temp_output.dim() > 0:
         temp_output = temp_output.cpu().tolist()
     else:
         temp_output = temp_output.cpu().item()
     return temp_output
+
+
+def get_tensor_from_image(input_image: Union[sitk.Image, str]) -> torch.Tensor:
+    """
+    This function converts a sitk image to a torch tensor.
+
+    Args:
+        input_image (sitk.Image): The input image.
+
+    Returns:
+        torch.Tensor: The converted torch tensor.
+    """
+    input_image = (
+        sitk.ReadImage(input_image) if isinstance(input_image, str) else input_image
+    )
+    return torch.from_numpy(sitk.GetArrayFromImage(input_image))
+
+
+def get_image_from_tensor(input_tensor: torch.Tensor) -> sitk.Image:
+    """
+    This function converts a torch tensor to a sitk image.
+
+    Args:
+        input_tensor (torch.Tensor): The input tensor.
+
+    Returns:
+        sitk.Image: The converted sitk image.
+    """
+    arr = input_tensor.cpu().numpy()
+    return_image = sitk.GetImageFromArray(arr)
+    # this is specifically the case for 3D images
+    if (arr.shape[0] == 1) and (arr.shape[1] > 3):
+        return_image = sitk.GetImageFromArray(arr[0])
+
+    return return_image
```

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF/utils/write_parse.py` & `GANDLF-0.0.17.dev20230615/GANDLF/utils/write_parse.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF.egg-info/PKG-INFO` & `GANDLF-0.0.17.dev20230615/GANDLF.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.17.dev20230614
+Version: 0.0.17.dev20230615
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230614 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230615 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.17.dev20230614/GANDLF.egg-info/SOURCES.txt` & `GANDLF-0.0.17.dev20230615/GANDLF.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,15 @@
 GANDLF/losses/regression.py
 GANDLF/losses/segmentation.py
 GANDLF/metrics/__init__.py
 GANDLF/metrics/classification.py
 GANDLF/metrics/generic.py
 GANDLF/metrics/regression.py
 GANDLF/metrics/segmentation.py
+GANDLF/metrics/synthesis.py
 GANDLF/models/MSDNet.py
 GANDLF/models/__init__.py
 GANDLF/models/brain_age.py
 GANDLF/models/deep_unet.py
 GANDLF/models/densenet.py
 GANDLF/models/efficientnet.py
 GANDLF/models/fcn.py
```

### Comparing `GANDLF-0.0.17.dev20230614/HISTORY.md` & `GANDLF-0.0.17.dev20230615/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ## 0.0.17
 - Added a CLI for metrics computation
+- Added metrics specific for image-to-image comparison
 
 ## 0.0.16
 - Added a script "gandlf_deploy", allowing deployment of models into MLCubes (currently requires Docker)
 - ImageNet pre-trained models for UNet with variable encoders is now available
 - ACS/Soft conversion is available for ImageNet-pretrained UNet
 - Updated links, copyright and email to MLCommons
 - Allowing provision for user to generate multiple configurations for experimentation
```

### Comparing `GANDLF-0.0.17.dev20230614/LICENSE` & `GANDLF-0.0.17.dev20230615/LICENSE`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/PKG-INFO` & `GANDLF-0.0.17.dev20230615/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.17.dev20230614
+Version: 0.0.17.dev20230615
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230614 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230615 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.17.dev20230614/README.md` & `GANDLF-0.0.17.dev20230615/README.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/SECURITY.md` & `GANDLF-0.0.17.dev20230615/SECURITY.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/gandlf_anonymizer` & `GANDLF-0.0.17.dev20230615/gandlf_anonymizer`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/gandlf_collectStats` & `GANDLF-0.0.17.dev20230615/gandlf_collectStats`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/gandlf_configGenerator` & `GANDLF-0.0.17.dev20230615/gandlf_configGenerator`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/gandlf_constructCSV` & `GANDLF-0.0.17.dev20230615/gandlf_constructCSV`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/gandlf_deploy` & `GANDLF-0.0.17.dev20230615/gandlf_deploy`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/gandlf_generateMetrics` & `GANDLF-0.0.17.dev20230615/gandlf_generateMetrics`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/gandlf_optimizeModel` & `GANDLF-0.0.17.dev20230615/gandlf_optimizeModel`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/gandlf_patchMiner` & `GANDLF-0.0.17.dev20230615/gandlf_patchMiner`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/gandlf_preprocess` & `GANDLF-0.0.17.dev20230615/gandlf_preprocess`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/gandlf_recoverConfig` & `GANDLF-0.0.17.dev20230615/gandlf_recoverConfig`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/gandlf_run` & `GANDLF-0.0.17.dev20230615/gandlf_run`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/gandlf_verifyInstall` & `GANDLF-0.0.17.dev20230615/gandlf_verifyInstall`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230614/setup.py` & `GANDLF-0.0.17.dev20230615/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     "requests>=2.25.0",
     "pytest",
     "coverage",
     "pytest-cov",
     "psutil",
     "medcam",
     "opencv-python",
-    "torchmetrics==0.5.1",  # newer versions have changed api for f1 invocation
+    "torchmetrics==0.8.1",
     "zarr==2.10.3",
     "pydicom",
     "onnx",
     "torchinfo==1.7.0",
     "segmentation-models-pytorch==0.3.2",
     "ACSConv==0.1.1",
     "docker",
```

