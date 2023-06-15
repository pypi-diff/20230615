# Comparing `tmp/grad-cam-1.4.5.tar.gz` & `tmp/grad-cam-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\grad-cam-1.4.5.tar", last modified: Thu Aug 25 06:44:53 2022, max compression
+gzip compressed data, was "dist\grad-cam-1.4.6.tar", last modified: Tue Oct 18 07:54:06 2022, max compression
```

## Comparing `grad-cam-1.4.5.tar` & `grad-cam-1.4.6.tar`

### file list

```diff
@@ -1,116 +1,118 @@
-drwxrwxrwx   0        0        0        0 2022-08-25 06:44:53.000000 grad-cam-1.4.5/
--rw-rw-rw-   0        0        0       45 2021-12-30 18:15:48.000000 grad-cam-1.4.5/.gitattributes
-drwxrwxrwx   0        0        0        0 2022-08-25 06:44:53.000000 grad-cam-1.4.5/.github/
-drwxrwxrwx   0        0        0        0 2022-08-25 06:44:53.000000 grad-cam-1.4.5/.github/workflows/
--rw-rw-rw-   0        0        0     1181 2022-08-01 03:43:36.000000 grad-cam-1.4.5/.github/workflows/python-app.yml
--rw-rw-rw-   0        0        0       33 2021-04-03 13:55:26.000000 grad-cam-1.4.5/.gitignore
--rw-rw-rw-   0        0        0     1094 2021-09-13 05:28:59.000000 grad-cam-1.4.5/LICENSE
--rw-rw-rw-   0        0        0       15 2022-08-01 09:16:16.000000 grad-cam-1.4.5/MANIFEST.in
--rw-rw-rw-   0        0        0    16632 2022-08-25 06:44:53.000000 grad-cam-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0    16005 2022-08-12 14:58:00.000000 grad-cam-1.4.5/README.md
--rw-rw-rw-   0        0        0     5485 2022-08-25 06:44:25.000000 grad-cam-1.4.5/cam.py
-drwxrwxrwx   0        0        0        0 2022-08-25 06:44:53.000000 grad-cam-1.4.5/examples/
--rw-rw-rw-   0        0        0    18447 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/augsmooth.jpg
--rw-rw-rw-   0        0        0    90226 2021-04-02 11:03:17.000000 grad-cam-1.4.5/examples/both.png
--rw-rw-rw-   0        0        0    74805 2021-12-30 15:52:29.000000 grad-cam-1.4.5/examples/both_detection.png
--rw-rw-rw-   0        0        0    10719 2021-04-02 11:03:17.000000 grad-cam-1.4.5/examples/cam_gb_dog.jpg
--rw-rw-rw-   0        0        0   286808 2021-12-30 15:52:29.000000 grad-cam-1.4.5/examples/cars_segmentation.png
--rw-rw-rw-   0        0        0    19413 2021-04-02 11:03:17.000000 grad-cam-1.4.5/examples/cat.jpg
--rw-rw-rw-   0        0        0   626320 2022-08-01 10:18:31.000000 grad-cam-1.4.5/examples/dff1.png
--rw-rw-rw-   0        0        0   596116 2022-08-01 10:18:51.000000 grad-cam-1.4.5/examples/dff2.png
--rw-rw-rw-   0        0        0    18669 2021-04-02 11:03:17.000000 grad-cam-1.4.5/examples/dog.jpg
--rw-rw-rw-   0        0        0     8608 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/dog_cat.jfif
--rw-rw-rw-   0        0        0   272570 2021-04-03 13:55:26.000000 grad-cam-1.4.5/examples/dogs.png
--rw-rw-rw-   0        0        0    29005 2021-04-03 13:55:26.000000 grad-cam-1.4.5/examples/dogs_gradcam++_resnet50.jpg
--rw-rw-rw-   0        0        0    29106 2021-04-03 13:55:26.000000 grad-cam-1.4.5/examples/dogs_gradcam++_vgg16.jpg
--rw-rw-rw-   0        0        0    28798 2021-04-03 13:55:26.000000 grad-cam-1.4.5/examples/dogs_gradcam_resnet50.jpg
--rw-rw-rw-   0        0        0    29319 2021-04-03 13:55:26.000000 grad-cam-1.4.5/examples/dogs_gradcam_vgg16.jpg
--rw-rw-rw-   0        0        0    28993 2021-04-03 13:55:26.000000 grad-cam-1.4.5/examples/dogs_scorecam_resnet50.jpg
--rw-rw-rw-   0        0        0    28384 2021-04-03 13:55:26.000000 grad-cam-1.4.5/examples/dogs_scorecam_vgg16.jpg
--rw-rw-rw-   0        0        0    18219 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/eigenaug.jpg
--rw-rw-rw-   0        0        0    18207 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/eigensmooth.jpg
--rw-rw-rw-   0        0        0  2201243 2022-07-09 09:36:24.000000 grad-cam-1.4.5/examples/embeddings.png
--rw-rw-rw-   0        0        0    50158 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/horses.jpg
--rw-rw-rw-   0        0        0   352428 2022-07-09 13:05:02.000000 grad-cam-1.4.5/examples/metrics.png
--rw-rw-rw-   0        0        0    18414 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/nosmooth.jpg
--rw-rw-rw-   0        0        0    17530 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/resnet50_cat_ablationcam_cam.jpg
--rw-rw-rw-   0        0        0    17490 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/resnet50_cat_gradcam_cam.jpg
--rw-rw-rw-   0        0        0    17436 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/resnet50_cat_scorecam_cam.jpg
--rw-rw-rw-   0        0        0    17810 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/resnet50_dog_ablationcam_cam.jpg
--rw-rw-rw-   0        0        0    17780 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/resnet50_dog_gradcam_cam.jpg
--rw-rw-rw-   0        0        0    17754 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/resnet50_dog_scorecam_cam.jpg
--rw-rw-rw-   0        0        0    71715 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/resnet_horses_ablationcam_cam.jpg
--rw-rw-rw-   0        0        0    71843 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/resnet_horses_gradcam++_cam.jpg
--rw-rw-rw-   0        0        0    71766 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/resnet_horses_gradcam_cam.jpg
--rw-rw-rw-   0        0        0    71262 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/resnet_horses_horses_eigencam_cam.jpg
--rw-rw-rw-   0        0        0    71917 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/resnet_horses_scorecam_cam.jpg
--rw-rw-rw-   0        0        0    80319 2022-07-09 09:55:24.000000 grad-cam-1.4.5/examples/road.png
--rw-rw-rw-   0        0        0    17331 2021-05-14 10:33:52.000000 grad-cam-1.4.5/examples/swinT_cat_ablationcam_cam.jpg
--rw-rw-rw-   0        0        0    17400 2021-05-14 10:33:52.000000 grad-cam-1.4.5/examples/swinT_cat_gradcam_cam.jpg
--rw-rw-rw-   0        0        0    17627 2021-05-14 10:33:52.000000 grad-cam-1.4.5/examples/swinT_cat_scorecam_cam.jpg
--rw-rw-rw-   0        0        0    18105 2021-05-14 10:33:52.000000 grad-cam-1.4.5/examples/swinT_dog_ablationcam_cam.jpg
--rw-rw-rw-   0        0        0    17649 2021-05-14 10:33:52.000000 grad-cam-1.4.5/examples/swinT_dog_gradcam_cam.jpg
--rw-rw-rw-   0        0        0    17720 2021-05-14 10:33:52.000000 grad-cam-1.4.5/examples/swinT_dog_scorecam_cam.jpg
--rw-rw-rw-   0        0        0    71353 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/vgg_horses_ablationcam_cam.jpg
--rw-rw-rw-   0        0        0    71040 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/vgg_horses_eigencam_cam.jpg
--rw-rw-rw-   0        0        0    71326 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/vgg_horses_gradcam++_cam.jpg
--rw-rw-rw-   0        0        0    71409 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/vgg_horses_gradcam_cam.jpg
--rw-rw-rw-   0        0        0    71522 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/vgg_horses_scorecam_cam.jpg
--rw-rw-rw-   0        0        0    18096 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/vit_cat_ablationcam_cam.jpg
--rw-rw-rw-   0        0        0    17951 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/vit_cat_gradcam_cam.jpg
--rw-rw-rw-   0        0        0    18218 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/vit_cat_scorecam_cam.jpg
--rw-rw-rw-   0        0        0    19807 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/vit_dog_ablationcam_cam.jpg
--rw-rw-rw-   0        0        0    19396 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/vit_dog_gradcam_cam.jpg
--rw-rw-rw-   0        0        0    18240 2021-05-01 13:07:59.000000 grad-cam-1.4.5/examples/vit_dog_scorecam_cam.jpg
--rw-rw-rw-   0        0        0  1788713 2022-08-01 05:50:56.000000 grad-cam-1.4.5/examples/yolo_eigencam.png
-drwxrwxrwx   0        0        0        0 2022-08-25 06:44:53.000000 grad-cam-1.4.5/grad_cam.egg-info/
--rw-rw-rw-   0        0        0    16632 2022-08-25 06:44:53.000000 grad-cam-1.4.5/grad_cam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3268 2022-08-25 06:44:53.000000 grad-cam-1.4.5/grad_cam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-25 06:44:53.000000 grad-cam-1.4.5/grad_cam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2022-08-25 06:44:53.000000 grad-cam-1.4.5/grad_cam.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2022-08-25 06:44:53.000000 grad-cam-1.4.5/grad_cam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-04-03 13:55:26.000000 grad-cam-1.4.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2022-08-25 06:44:53.000000 grad-cam-1.4.5/pytorch_grad_cam/
--rw-rw-rw-   0        0        0     1176 2022-08-24 14:58:18.000000 grad-cam-1.4.5/pytorch_grad_cam/__init__.py
--rw-rw-rw-   0        0        0     6939 2022-08-01 05:50:56.000000 grad-cam-1.4.5/pytorch_grad_cam/ablation_cam.py
--rw-rw-rw-   0        0        0     5195 2021-12-30 15:52:29.000000 grad-cam-1.4.5/pytorch_grad_cam/ablation_cam_multilayer.py
--rw-rw-rw-   0        0        0     6325 2022-08-01 05:50:56.000000 grad-cam-1.4.5/pytorch_grad_cam/ablation_layer.py
--rw-rw-rw-   0        0        0     1771 2022-08-23 19:20:12.000000 grad-cam-1.4.5/pytorch_grad_cam/activations_and_gradients.py
--rw-rw-rw-   0        0        0     8452 2022-08-24 14:55:17.000000 grad-cam-1.4.5/pytorch_grad_cam/base_cam.py
--rw-rw-rw-   0        0        0      862 2022-04-01 12:43:32.000000 grad-cam-1.4.5/pytorch_grad_cam/eigen_cam.py
--rw-rw-rw-   0        0        0      800 2021-09-12 17:27:25.000000 grad-cam-1.4.5/pytorch_grad_cam/eigen_grad_cam.py
-drwxrwxrwx   0        0        0        0 2022-08-25 06:44:53.000000 grad-cam-1.4.5/pytorch_grad_cam/feature_factorization/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:14:13.000000 grad-cam-1.4.5/pytorch_grad_cam/feature_factorization/__init__.py
--rw-rw-rw-   0        0        0     3873 2022-08-13 13:53:59.000000 grad-cam-1.4.5/pytorch_grad_cam/feature_factorization/deep_feature_factorization.py
--rw-rw-rw-   0        0        0     4190 2021-12-30 15:52:29.000000 grad-cam-1.4.5/pytorch_grad_cam/fullgrad_cam.py
--rw-rw-rw-   0        0        0      639 2022-08-23 19:17:00.000000 grad-cam-1.4.5/pytorch_grad_cam/grad_cam.py
--rw-rw-rw-   0        0        0      965 2022-08-01 05:50:56.000000 grad-cam-1.4.5/pytorch_grad_cam/grad_cam_elementwise.py
--rw-rw-rw-   0        0        0     1262 2021-09-12 17:27:41.000000 grad-cam-1.4.5/pytorch_grad_cam/grad_cam_plusplus.py
--rw-rw-rw-   0        0        0     3371 2021-09-13 07:15:27.000000 grad-cam-1.4.5/pytorch_grad_cam/guided_backprop.py
--rw-rw-rw-   0        0        0     1050 2022-08-01 05:50:56.000000 grad-cam-1.4.5/pytorch_grad_cam/hirescam.py
--rw-rw-rw-   0        0        0     1058 2022-07-08 09:17:05.000000 grad-cam-1.4.5/pytorch_grad_cam/layer_cam.py
-drwxrwxrwx   0        0        0        0 2022-08-25 06:44:53.000000 grad-cam-1.4.5/pytorch_grad_cam/metrics/
--rw-rw-rw-   0        0        0        0 2022-08-25 06:44:39.000000 grad-cam-1.4.5/pytorch_grad_cam/metrics/__init__.py
--rw-rw-rw-   0        0        0     1222 2022-08-01 05:50:56.000000 grad-cam-1.4.5/pytorch_grad_cam/metrics/cam_mult_image.py
--rw-rw-rw-   0        0        0     3621 2022-08-01 05:50:56.000000 grad-cam-1.4.5/pytorch_grad_cam/metrics/perturbation_confidence.py
--rw-rw-rw-   0        0        0     7897 2022-08-01 05:50:56.000000 grad-cam-1.4.5/pytorch_grad_cam/metrics/road.py
--rw-rw-rw-   0        0        0      679 2022-07-09 07:46:06.000000 grad-cam-1.4.5/pytorch_grad_cam/random_cam.py
--rw-rw-rw-   0        0        0     2367 2022-08-06 09:33:52.000000 grad-cam-1.4.5/pytorch_grad_cam/score_cam.py
--rw-rw-rw-   0        0        0      375 2022-08-01 05:50:56.000000 grad-cam-1.4.5/pytorch_grad_cam/sobel_cam.py
-drwxrwxrwx   0        0        0        0 2022-08-25 06:44:53.000000 grad-cam-1.4.5/pytorch_grad_cam/utils/
--rw-rw-rw-   0        0        0      236 2022-08-25 06:44:06.000000 grad-cam-1.4.5/pytorch_grad_cam/utils/__init__.py
--rw-rw-rw-   0        0        0     1083 2022-08-01 05:50:56.000000 grad-cam-1.4.5/pytorch_grad_cam/utils/find_layers.py
--rw-rw-rw-   0        0        0     6452 2022-08-12 15:08:32.000000 grad-cam-1.4.5/pytorch_grad_cam/utils/image.py
--rw-rw-rw-   0        0        0     3134 2022-08-01 05:50:56.000000 grad-cam-1.4.5/pytorch_grad_cam/utils/model_targets.py
--rw-rw-rw-   0        0        0     1044 2022-08-01 05:50:56.000000 grad-cam-1.4.5/pytorch_grad_cam/utils/reshape_transforms.py
--rw-rw-rw-   0        0        0      829 2022-07-30 18:19:49.000000 grad-cam-1.4.5/pytorch_grad_cam/utils/svd_on_activations.py
--rw-rw-rw-   0        0        0      891 2021-09-12 16:58:05.000000 grad-cam-1.4.5/pytorch_grad_cam/xgrad_cam.py
--rw-rw-rw-   0        0        0      101 2022-08-01 05:50:56.000000 grad-cam-1.4.5/requirements.txt
--rw-rw-rw-   0        0        0      711 2022-08-25 06:44:53.000000 grad-cam-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1036 2022-08-25 06:44:48.000000 grad-cam-1.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-25 06:44:53.000000 grad-cam-1.4.5/tests/
--rw-rw-rw-   0        0        0     2171 2022-01-15 17:07:07.000000 grad-cam-1.4.5/tests/test_context_release.py
--rw-rw-rw-   0        0        0     2553 2021-12-30 15:52:29.000000 grad-cam-1.4.5/tests/test_run_all_models.py
-drwxrwxrwx   0        0        0        0 2022-08-25 06:44:53.000000 grad-cam-1.4.5/usage_examples/
--rw-rw-rw-   0        0        0     4245 2022-03-11 09:57:13.000000 grad-cam-1.4.5/usage_examples/swinT_example.py
--rw-rw-rw-   0        0        0     4472 2022-05-16 16:45:24.000000 grad-cam-1.4.5/usage_examples/vit_example.py
+drwxrwxrwx   0        0        0        0 2022-10-18 07:54:06.000000 grad-cam-1.4.6/
+-rw-rw-rw-   0        0        0       45 2021-12-30 18:15:48.000000 grad-cam-1.4.6/.gitattributes
+drwxrwxrwx   0        0        0        0 2022-10-18 07:54:06.000000 grad-cam-1.4.6/.github/
+drwxrwxrwx   0        0        0        0 2022-10-18 07:54:06.000000 grad-cam-1.4.6/.github/workflows/
+-rw-rw-rw-   0        0        0     1181 2022-08-01 03:43:36.000000 grad-cam-1.4.6/.github/workflows/python-app.yml
+-rw-rw-rw-   0        0        0       33 2021-04-03 13:55:26.000000 grad-cam-1.4.6/.gitignore
+-rw-rw-rw-   0        0        0     1094 2021-09-13 05:28:59.000000 grad-cam-1.4.6/LICENSE
+-rw-rw-rw-   0        0        0       15 2022-08-01 09:16:16.000000 grad-cam-1.4.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    16792 2022-10-18 07:54:06.000000 grad-cam-1.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0    16165 2022-10-18 07:47:18.000000 grad-cam-1.4.6/README.md
+-rw-rw-rw-   0        0        0     5480 2022-10-18 07:37:42.000000 grad-cam-1.4.6/cam.py
+drwxrwxrwx   0        0        0        0 2022-10-18 07:54:06.000000 grad-cam-1.4.6/examples/
+-rw-rw-rw-   0        0        0    18447 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/augsmooth.jpg
+-rw-rw-rw-   0        0        0    90226 2021-04-02 11:03:17.000000 grad-cam-1.4.6/examples/both.png
+-rw-rw-rw-   0        0        0    74805 2021-12-30 15:52:29.000000 grad-cam-1.4.6/examples/both_detection.png
+-rw-rw-rw-   0        0        0    10719 2021-04-02 11:03:17.000000 grad-cam-1.4.6/examples/cam_gb_dog.jpg
+-rw-rw-rw-   0        0        0   286808 2021-12-30 15:52:29.000000 grad-cam-1.4.6/examples/cars_segmentation.png
+-rw-rw-rw-   0        0        0    19413 2021-04-02 11:03:17.000000 grad-cam-1.4.6/examples/cat.jpg
+-rw-rw-rw-   0        0        0   626320 2022-08-01 10:18:31.000000 grad-cam-1.4.6/examples/dff1.png
+-rw-rw-rw-   0        0        0   596116 2022-08-01 10:18:51.000000 grad-cam-1.4.6/examples/dff2.png
+-rw-rw-rw-   0        0        0    18669 2021-04-02 11:03:17.000000 grad-cam-1.4.6/examples/dog.jpg
+-rw-rw-rw-   0        0        0     8608 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/dog_cat.jfif
+-rw-rw-rw-   0        0        0   272570 2021-04-03 13:55:26.000000 grad-cam-1.4.6/examples/dogs.png
+-rw-rw-rw-   0        0        0    29005 2021-04-03 13:55:26.000000 grad-cam-1.4.6/examples/dogs_gradcam++_resnet50.jpg
+-rw-rw-rw-   0        0        0    29106 2021-04-03 13:55:26.000000 grad-cam-1.4.6/examples/dogs_gradcam++_vgg16.jpg
+-rw-rw-rw-   0        0        0    28798 2021-04-03 13:55:26.000000 grad-cam-1.4.6/examples/dogs_gradcam_resnet50.jpg
+-rw-rw-rw-   0        0        0    29319 2021-04-03 13:55:26.000000 grad-cam-1.4.6/examples/dogs_gradcam_vgg16.jpg
+-rw-rw-rw-   0        0        0    28993 2021-04-03 13:55:26.000000 grad-cam-1.4.6/examples/dogs_scorecam_resnet50.jpg
+-rw-rw-rw-   0        0        0    28384 2021-04-03 13:55:26.000000 grad-cam-1.4.6/examples/dogs_scorecam_vgg16.jpg
+-rw-rw-rw-   0        0        0    18219 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/eigenaug.jpg
+-rw-rw-rw-   0        0        0    18207 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/eigensmooth.jpg
+-rw-rw-rw-   0        0        0  2201243 2022-07-09 09:36:24.000000 grad-cam-1.4.6/examples/embeddings.png
+-rw-rw-rw-   0        0        0    50158 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/horses.jpg
+-rw-rw-rw-   0        0        0   352428 2022-07-09 13:05:02.000000 grad-cam-1.4.6/examples/metrics.png
+-rw-rw-rw-   0        0        0    18414 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/nosmooth.jpg
+-rw-rw-rw-   0        0        0    17530 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/resnet50_cat_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    17490 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/resnet50_cat_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    17436 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/resnet50_cat_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0    17810 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/resnet50_dog_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    17780 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/resnet50_dog_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    17754 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/resnet50_dog_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0    71715 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/resnet_horses_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    71843 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/resnet_horses_gradcam++_cam.jpg
+-rw-rw-rw-   0        0        0    71766 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/resnet_horses_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    71262 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/resnet_horses_horses_eigencam_cam.jpg
+-rw-rw-rw-   0        0        0    71917 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/resnet_horses_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0    80319 2022-07-09 09:55:24.000000 grad-cam-1.4.6/examples/road.png
+-rw-rw-rw-   0        0        0    17331 2021-05-14 10:33:52.000000 grad-cam-1.4.6/examples/swinT_cat_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    17400 2021-05-14 10:33:52.000000 grad-cam-1.4.6/examples/swinT_cat_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    17627 2021-05-14 10:33:52.000000 grad-cam-1.4.6/examples/swinT_cat_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0    18105 2021-05-14 10:33:52.000000 grad-cam-1.4.6/examples/swinT_dog_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    17649 2021-05-14 10:33:52.000000 grad-cam-1.4.6/examples/swinT_dog_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    17720 2021-05-14 10:33:52.000000 grad-cam-1.4.6/examples/swinT_dog_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0    71353 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/vgg_horses_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    71040 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/vgg_horses_eigencam_cam.jpg
+-rw-rw-rw-   0        0        0    71326 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/vgg_horses_gradcam++_cam.jpg
+-rw-rw-rw-   0        0        0    71409 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/vgg_horses_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    71522 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/vgg_horses_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0    18096 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/vit_cat_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    17951 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/vit_cat_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    18218 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/vit_cat_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0    19807 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/vit_dog_ablationcam_cam.jpg
+-rw-rw-rw-   0        0        0    19396 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/vit_dog_gradcam_cam.jpg
+-rw-rw-rw-   0        0        0    18240 2021-05-01 13:07:59.000000 grad-cam-1.4.6/examples/vit_dog_scorecam_cam.jpg
+-rw-rw-rw-   0        0        0  1788713 2022-08-01 05:50:56.000000 grad-cam-1.4.6/examples/yolo_eigencam.png
+drwxrwxrwx   0        0        0        0 2022-10-18 07:54:06.000000 grad-cam-1.4.6/grad_cam.egg-info/
+-rw-rw-rw-   0        0        0    16792 2022-10-18 07:54:05.000000 grad-cam-1.4.6/grad_cam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3342 2022-10-18 07:54:06.000000 grad-cam-1.4.6/grad_cam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-18 07:54:05.000000 grad-cam-1.4.6/grad_cam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2022-10-18 07:54:05.000000 grad-cam-1.4.6/grad_cam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2022-10-18 07:54:05.000000 grad-cam-1.4.6/grad_cam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-04-03 13:55:26.000000 grad-cam-1.4.6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2022-10-18 07:54:06.000000 grad-cam-1.4.6/pytorch_grad_cam/
+-rw-rw-rw-   0        0        0     1196 2022-10-18 07:37:44.000000 grad-cam-1.4.6/pytorch_grad_cam/__init__.py
+-rw-rw-rw-   0        0        0     6939 2022-08-01 05:50:56.000000 grad-cam-1.4.6/pytorch_grad_cam/ablation_cam.py
+-rw-rw-rw-   0        0        0     5195 2021-12-30 15:52:29.000000 grad-cam-1.4.6/pytorch_grad_cam/ablation_cam_multilayer.py
+-rw-rw-rw-   0        0        0     6325 2022-08-01 05:50:56.000000 grad-cam-1.4.6/pytorch_grad_cam/ablation_layer.py
+-rw-rw-rw-   0        0        0     1771 2022-10-17 11:35:47.000000 grad-cam-1.4.6/pytorch_grad_cam/activations_and_gradients.py
+-rw-rw-rw-   0        0        0     8452 2022-10-18 07:46:13.000000 grad-cam-1.4.6/pytorch_grad_cam/base_cam.py
+-rw-rw-rw-   0        0        0      862 2022-04-01 12:43:32.000000 grad-cam-1.4.6/pytorch_grad_cam/eigen_cam.py
+-rw-rw-rw-   0        0        0      800 2021-09-12 17:27:25.000000 grad-cam-1.4.6/pytorch_grad_cam/eigen_grad_cam.py
+drwxrwxrwx   0        0        0        0 2022-10-18 07:54:06.000000 grad-cam-1.4.6/pytorch_grad_cam/feature_factorization/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:14:13.000000 grad-cam-1.4.6/pytorch_grad_cam/feature_factorization/__init__.py
+-rw-rw-rw-   0        0        0     5541 2022-10-18 07:37:44.000000 grad-cam-1.4.6/pytorch_grad_cam/feature_factorization/deep_feature_factorization.py
+-rw-rw-rw-   0        0        0      771 2022-10-18 07:37:44.000000 grad-cam-1.4.6/pytorch_grad_cam/feature_factorization/utils.py
+-rw-rw-rw-   0        0        0     4190 2021-12-30 15:52:29.000000 grad-cam-1.4.6/pytorch_grad_cam/fullgrad_cam.py
+-rw-rw-rw-   0        0        0      639 2022-10-17 16:38:03.000000 grad-cam-1.4.6/pytorch_grad_cam/grad_cam.py
+-rw-rw-rw-   0        0        0      965 2022-08-01 05:50:56.000000 grad-cam-1.4.6/pytorch_grad_cam/grad_cam_elementwise.py
+-rw-rw-rw-   0        0        0     1262 2021-09-12 17:27:41.000000 grad-cam-1.4.6/pytorch_grad_cam/grad_cam_plusplus.py
+-rw-rw-rw-   0        0        0     3371 2021-09-13 07:15:27.000000 grad-cam-1.4.6/pytorch_grad_cam/guided_backprop.py
+-rw-rw-rw-   0        0        0     1050 2022-08-01 05:50:56.000000 grad-cam-1.4.6/pytorch_grad_cam/hirescam.py
+-rw-rw-rw-   0        0        0     1058 2022-07-08 09:17:05.000000 grad-cam-1.4.6/pytorch_grad_cam/layer_cam.py
+drwxrwxrwx   0        0        0        0 2022-10-18 07:54:06.000000 grad-cam-1.4.6/pytorch_grad_cam/metrics/
+-rw-rw-rw-   0        0        0        0 2022-08-25 06:44:39.000000 grad-cam-1.4.6/pytorch_grad_cam/metrics/__init__.py
+-rw-rw-rw-   0        0        0     1222 2022-08-01 05:50:56.000000 grad-cam-1.4.6/pytorch_grad_cam/metrics/cam_mult_image.py
+-rw-rw-rw-   0        0        0     3621 2022-08-01 05:50:56.000000 grad-cam-1.4.6/pytorch_grad_cam/metrics/perturbation_confidence.py
+-rw-rw-rw-   0        0        0     7897 2022-08-01 05:50:56.000000 grad-cam-1.4.6/pytorch_grad_cam/metrics/road.py
+-rw-rw-rw-   0        0        0      679 2022-07-09 07:46:06.000000 grad-cam-1.4.6/pytorch_grad_cam/random_cam.py
+-rw-rw-rw-   0        0        0     2367 2022-08-06 09:33:52.000000 grad-cam-1.4.6/pytorch_grad_cam/score_cam.py
+-rw-rw-rw-   0        0        0      375 2022-08-01 05:50:56.000000 grad-cam-1.4.6/pytorch_grad_cam/sobel_cam.py
+drwxrwxrwx   0        0        0        0 2022-10-18 07:54:06.000000 grad-cam-1.4.6/pytorch_grad_cam/utils/
+-rw-rw-rw-   0        0        0      236 2022-08-25 06:44:06.000000 grad-cam-1.4.6/pytorch_grad_cam/utils/__init__.py
+-rw-rw-rw-   0        0        0     1083 2022-08-01 05:50:56.000000 grad-cam-1.4.6/pytorch_grad_cam/utils/find_layers.py
+-rw-rw-rw-   0        0        0     7237 2022-10-18 07:37:45.000000 grad-cam-1.4.6/pytorch_grad_cam/utils/image.py
+-rw-rw-rw-   0        0        0     3134 2022-08-01 05:50:56.000000 grad-cam-1.4.6/pytorch_grad_cam/utils/model_targets.py
+-rw-rw-rw-   0        0        0     1044 2022-10-16 13:31:03.000000 grad-cam-1.4.6/pytorch_grad_cam/utils/reshape_transforms.py
+-rw-rw-rw-   0        0        0      829 2022-07-30 18:19:49.000000 grad-cam-1.4.6/pytorch_grad_cam/utils/svd_on_activations.py
+-rw-rw-rw-   0        0        0      891 2021-09-12 16:58:05.000000 grad-cam-1.4.6/pytorch_grad_cam/xgrad_cam.py
+-rw-rw-rw-   0        0        0      101 2022-08-01 05:50:56.000000 grad-cam-1.4.6/requirements.txt
+-rw-rw-rw-   0        0        0      711 2022-10-18 07:54:06.000000 grad-cam-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1044 2022-10-18 07:47:29.000000 grad-cam-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-18 07:54:06.000000 grad-cam-1.4.6/tests/
+-rw-rw-rw-   0        0        0     2187 2022-10-18 07:37:45.000000 grad-cam-1.4.6/tests/test_context_release.py
+-rw-rw-rw-   0        0        0     1451 2022-10-18 07:37:45.000000 grad-cam-1.4.6/tests/test_one_channel.py
+-rw-rw-rw-   0        0        0     2577 2022-10-18 07:37:45.000000 grad-cam-1.4.6/tests/test_run_all_models.py
+drwxrwxrwx   0        0        0        0 2022-10-18 07:54:06.000000 grad-cam-1.4.6/usage_examples/
+-rw-rw-rw-   0        0        0     4245 2022-10-18 07:37:46.000000 grad-cam-1.4.6/usage_examples/swinT_example.py
+-rw-rw-rw-   0        0        0     4471 2022-10-18 07:37:46.000000 grad-cam-1.4.6/usage_examples/vit_example.py
```

### Comparing `grad-cam-1.4.5/.github/workflows/python-app.yml` & `grad-cam-1.4.6/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/LICENSE` & `grad-cam-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/PKG-INFO` & `grad-cam-1.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grad-cam
-Version: 1.4.5
+Version: 1.4.6
 Summary: Many Class Activation Map methods implemented in Pytorch for classification, segmentation, object detection and more
 Home-page: https://github.com/jacobgil/pytorch-grad-cam
 Author: Jacob Gildenblat
 Author-email: jacob.gildenblat@gmail.com
 Project-URL: Bug Tracker, https://github.com/jacobgil/pytorch-grad-cam/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -200,14 +200,16 @@
 2. Model Targets, that define what target do you want to compute the visualizations for, for example a specific category, or a list of bounding boxes.
 
 Here you can find detailed examples of how to use this for various custom use cases like object detection:
 
 These point to the new documentation jupter-book for fast rendering.
 The jupyter notebooks themselves can be found under the tutorials folder in the git repository.
 
+- [Notebook tutorial: XAI Recepies for the HuggingFace 🤗 Image Classification Models](<https://jacobgil.github.io/pytorch-gradcam-book/huggingface.html>)
+
 - [Notebook tutorial: Deep Feature Factorizations for better model explainability](<https://jacobgil.github.io/pytorch-gradcam-book/Deep%20Feature%20Factorizations.html>)
 
 - [Notebook tutorial: Class Activation Maps for Object Detection with Faster-RCNN](<https://jacobgil.github.io/pytorch-gradcam-book/Class%20Activation%20Maps%20for%20Object%20Detection%20With%20Faster%20RCNN.html>)
 
 - [Notebook tutorial: Class Activation Maps for YOLO5](<https://jacobgil.github.io/pytorch-gradcam-book/EigenCAM%20for%20YOLO5.html>)
 
 - [Notebook tutorial: Class Activation Maps for Semantic Segmentation](<https://jacobgil.github.io/pytorch-gradcam-book/Class%20Activation%20Maps%20for%20Semantic%20Segmentation.html>)
```

### Comparing `grad-cam-1.4.5/README.md` & `grad-cam-1.4.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -185,14 +185,16 @@
 2. Model Targets, that define what target do you want to compute the visualizations for, for example a specific category, or a list of bounding boxes.
 
 Here you can find detailed examples of how to use this for various custom use cases like object detection:
 
 These point to the new documentation jupter-book for fast rendering.
 The jupyter notebooks themselves can be found under the tutorials folder in the git repository.
 
+- [Notebook tutorial: XAI Recepies for the HuggingFace 🤗 Image Classification Models](<https://jacobgil.github.io/pytorch-gradcam-book/huggingface.html>)
+
 - [Notebook tutorial: Deep Feature Factorizations for better model explainability](<https://jacobgil.github.io/pytorch-gradcam-book/Deep%20Feature%20Factorizations.html>)
 
 - [Notebook tutorial: Class Activation Maps for Object Detection with Faster-RCNN](<https://jacobgil.github.io/pytorch-gradcam-book/Class%20Activation%20Maps%20for%20Object%20Detection%20With%20Faster%20RCNN.html>)
 
 - [Notebook tutorial: Class Activation Maps for YOLO5](<https://jacobgil.github.io/pytorch-gradcam-book/EigenCAM%20for%20YOLO5.html>)
 
 - [Notebook tutorial: Class Activation Maps for Semantic Segmentation](<https://jacobgil.github.io/pytorch-gradcam-book/Class%20Activation%20Maps%20for%20Semantic%20Segmentation.html>)
```

### Comparing `grad-cam-1.4.5/cam.py` & `grad-cam-1.4.6/cam.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     AblationCAM, \
     XGradCAM, \
     EigenCAM, \
     EigenGradCAM, \
     LayerCAM, \
     FullGrad, \
     GradCAMElementWise
-    
+
 
 from pytorch_grad_cam import GuidedBackpropReLUModel
 from pytorch_grad_cam.utils.image import show_cam_on_image, \
     deprocess_image, \
     preprocess_image
 from pytorch_grad_cam.utils.model_targets import ClassifierOutputTarget
 
@@ -64,15 +64,15 @@
         2. Guided Back Propagation
         3. Combining both
     """
 
     args = get_args()
     methods = \
         {"gradcam": GradCAM,
-         "hirescam":HiResCAM,
+         "hirescam": HiResCAM,
          "scorecam": ScoreCAM,
          "gradcam++": GradCAMPlusPlus,
          "ablationcam": AblationCAM,
          "xgradcam": XGradCAM,
          "eigencam": EigenCAM,
          "eigengradcam": EigenGradCAM,
          "layercam": LayerCAM,
@@ -97,15 +97,14 @@
 
     rgb_img = cv2.imread(args.image_path, 1)[:, :, ::-1]
     rgb_img = np.float32(rgb_img) / 255
     input_tensor = preprocess_image(rgb_img,
                                     mean=[0.485, 0.456, 0.406],
                                     std=[0.229, 0.224, 0.225])
 
-
     # We have to specify the target we want to generate
     # the Class Activation Maps for.
     # If targets is None, the highest scoring category (for every member in the batch) will be used.
     # You can target specific categories by
     # targets = [e.g ClassifierOutputTarget(281)]
     targets = None
```

### Comparing `grad-cam-1.4.5/examples/augsmooth.jpg` & `grad-cam-1.4.6/examples/augsmooth.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/both.png` & `grad-cam-1.4.6/examples/both.png`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/both_detection.png` & `grad-cam-1.4.6/examples/both_detection.png`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/cam_gb_dog.jpg` & `grad-cam-1.4.6/examples/cam_gb_dog.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/cars_segmentation.png` & `grad-cam-1.4.6/examples/cars_segmentation.png`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/cat.jpg` & `grad-cam-1.4.6/examples/cat.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/dff1.png` & `grad-cam-1.4.6/examples/dff1.png`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/dff2.png` & `grad-cam-1.4.6/examples/dff2.png`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/dog.jpg` & `grad-cam-1.4.6/examples/dog.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/dog_cat.jfif` & `grad-cam-1.4.6/examples/dog_cat.jfif`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/dogs.png` & `grad-cam-1.4.6/examples/dogs.png`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/dogs_gradcam++_resnet50.jpg` & `grad-cam-1.4.6/examples/dogs_gradcam++_resnet50.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/dogs_gradcam++_vgg16.jpg` & `grad-cam-1.4.6/examples/dogs_gradcam++_vgg16.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/dogs_gradcam_resnet50.jpg` & `grad-cam-1.4.6/examples/dogs_gradcam_resnet50.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/dogs_gradcam_vgg16.jpg` & `grad-cam-1.4.6/examples/dogs_gradcam_vgg16.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/dogs_scorecam_resnet50.jpg` & `grad-cam-1.4.6/examples/dogs_scorecam_resnet50.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/dogs_scorecam_vgg16.jpg` & `grad-cam-1.4.6/examples/dogs_scorecam_vgg16.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/eigenaug.jpg` & `grad-cam-1.4.6/examples/eigenaug.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/eigensmooth.jpg` & `grad-cam-1.4.6/examples/eigensmooth.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/embeddings.png` & `grad-cam-1.4.6/examples/embeddings.png`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/horses.jpg` & `grad-cam-1.4.6/examples/horses.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/metrics.png` & `grad-cam-1.4.6/examples/metrics.png`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/nosmooth.jpg` & `grad-cam-1.4.6/examples/nosmooth.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/resnet50_cat_ablationcam_cam.jpg` & `grad-cam-1.4.6/examples/resnet50_cat_ablationcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/resnet50_cat_gradcam_cam.jpg` & `grad-cam-1.4.6/examples/resnet50_cat_gradcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/resnet50_cat_scorecam_cam.jpg` & `grad-cam-1.4.6/examples/resnet50_cat_scorecam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/resnet50_dog_ablationcam_cam.jpg` & `grad-cam-1.4.6/examples/resnet50_dog_ablationcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/resnet50_dog_gradcam_cam.jpg` & `grad-cam-1.4.6/examples/resnet50_dog_gradcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/resnet50_dog_scorecam_cam.jpg` & `grad-cam-1.4.6/examples/resnet50_dog_scorecam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/resnet_horses_ablationcam_cam.jpg` & `grad-cam-1.4.6/examples/resnet_horses_ablationcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/resnet_horses_gradcam++_cam.jpg` & `grad-cam-1.4.6/examples/resnet_horses_gradcam++_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/resnet_horses_gradcam_cam.jpg` & `grad-cam-1.4.6/examples/resnet_horses_gradcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/resnet_horses_horses_eigencam_cam.jpg` & `grad-cam-1.4.6/examples/resnet_horses_horses_eigencam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/resnet_horses_scorecam_cam.jpg` & `grad-cam-1.4.6/examples/resnet_horses_scorecam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/road.png` & `grad-cam-1.4.6/examples/road.png`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/swinT_cat_ablationcam_cam.jpg` & `grad-cam-1.4.6/examples/swinT_cat_ablationcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/swinT_cat_gradcam_cam.jpg` & `grad-cam-1.4.6/examples/swinT_cat_gradcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/swinT_cat_scorecam_cam.jpg` & `grad-cam-1.4.6/examples/swinT_cat_scorecam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/swinT_dog_ablationcam_cam.jpg` & `grad-cam-1.4.6/examples/swinT_dog_ablationcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/swinT_dog_gradcam_cam.jpg` & `grad-cam-1.4.6/examples/swinT_dog_gradcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/swinT_dog_scorecam_cam.jpg` & `grad-cam-1.4.6/examples/swinT_dog_scorecam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/vgg_horses_ablationcam_cam.jpg` & `grad-cam-1.4.6/examples/vgg_horses_ablationcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/vgg_horses_eigencam_cam.jpg` & `grad-cam-1.4.6/examples/vgg_horses_eigencam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/vgg_horses_gradcam++_cam.jpg` & `grad-cam-1.4.6/examples/vgg_horses_gradcam++_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/vgg_horses_gradcam_cam.jpg` & `grad-cam-1.4.6/examples/vgg_horses_gradcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/vgg_horses_scorecam_cam.jpg` & `grad-cam-1.4.6/examples/vgg_horses_scorecam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/vit_cat_ablationcam_cam.jpg` & `grad-cam-1.4.6/examples/vit_cat_ablationcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/vit_cat_gradcam_cam.jpg` & `grad-cam-1.4.6/examples/vit_cat_gradcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/vit_cat_scorecam_cam.jpg` & `grad-cam-1.4.6/examples/vit_cat_scorecam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/vit_dog_ablationcam_cam.jpg` & `grad-cam-1.4.6/examples/vit_dog_ablationcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/vit_dog_gradcam_cam.jpg` & `grad-cam-1.4.6/examples/vit_dog_gradcam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/vit_dog_scorecam_cam.jpg` & `grad-cam-1.4.6/examples/vit_dog_scorecam_cam.jpg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/examples/yolo_eigencam.png` & `grad-cam-1.4.6/examples/yolo_eigencam.png`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/grad_cam.egg-info/PKG-INFO` & `grad-cam-1.4.6/grad_cam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grad-cam
-Version: 1.4.5
+Version: 1.4.6
 Summary: Many Class Activation Map methods implemented in Pytorch for classification, segmentation, object detection and more
 Home-page: https://github.com/jacobgil/pytorch-grad-cam
 Author: Jacob Gildenblat
 Author-email: jacob.gildenblat@gmail.com
 Project-URL: Bug Tracker, https://github.com/jacobgil/pytorch-grad-cam/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -200,14 +200,16 @@
 2. Model Targets, that define what target do you want to compute the visualizations for, for example a specific category, or a list of bounding boxes.
 
 Here you can find detailed examples of how to use this for various custom use cases like object detection:
 
 These point to the new documentation jupter-book for fast rendering.
 The jupyter notebooks themselves can be found under the tutorials folder in the git repository.
 
+- [Notebook tutorial: XAI Recepies for the HuggingFace 🤗 Image Classification Models](<https://jacobgil.github.io/pytorch-gradcam-book/huggingface.html>)
+
 - [Notebook tutorial: Deep Feature Factorizations for better model explainability](<https://jacobgil.github.io/pytorch-gradcam-book/Deep%20Feature%20Factorizations.html>)
 
 - [Notebook tutorial: Class Activation Maps for Object Detection with Faster-RCNN](<https://jacobgil.github.io/pytorch-gradcam-book/Class%20Activation%20Maps%20for%20Object%20Detection%20With%20Faster%20RCNN.html>)
 
 - [Notebook tutorial: Class Activation Maps for YOLO5](<https://jacobgil.github.io/pytorch-gradcam-book/EigenCAM%20for%20YOLO5.html>)
 
 - [Notebook tutorial: Class Activation Maps for Semantic Segmentation](<https://jacobgil.github.io/pytorch-gradcam-book/Class%20Activation%20Maps%20for%20Semantic%20Segmentation.html>)
```

### Comparing `grad-cam-1.4.5/grad_cam.egg-info/SOURCES.txt` & `grad-cam-1.4.6/grad_cam.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -84,21 +84,23 @@
 pytorch_grad_cam/layer_cam.py
 pytorch_grad_cam/random_cam.py
 pytorch_grad_cam/score_cam.py
 pytorch_grad_cam/sobel_cam.py
 pytorch_grad_cam/xgrad_cam.py
 pytorch_grad_cam/feature_factorization/__init__.py
 pytorch_grad_cam/feature_factorization/deep_feature_factorization.py
+pytorch_grad_cam/feature_factorization/utils.py
 pytorch_grad_cam/metrics/__init__.py
 pytorch_grad_cam/metrics/cam_mult_image.py
 pytorch_grad_cam/metrics/perturbation_confidence.py
 pytorch_grad_cam/metrics/road.py
 pytorch_grad_cam/utils/__init__.py
 pytorch_grad_cam/utils/find_layers.py
 pytorch_grad_cam/utils/image.py
 pytorch_grad_cam/utils/model_targets.py
 pytorch_grad_cam/utils/reshape_transforms.py
 pytorch_grad_cam/utils/svd_on_activations.py
 tests/test_context_release.py
+tests/test_one_channel.py
 tests/test_run_all_models.py
 usage_examples/swinT_example.py
 usage_examples/vit_example.py
```

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/__init__.py` & `grad-cam-1.4.6/pytorch_grad_cam/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 from pytorch_grad_cam.layer_cam import LayerCAM
 from pytorch_grad_cam.eigen_cam import EigenCAM
 from pytorch_grad_cam.eigen_grad_cam import EigenGradCAM
 from pytorch_grad_cam.random_cam import RandomCAM
 from pytorch_grad_cam.fullgrad_cam import FullGrad
 from pytorch_grad_cam.guided_backprop import GuidedBackpropReLUModel
 from pytorch_grad_cam.activations_and_gradients import ActivationsAndGradients
-from pytorch_grad_cam.feature_factorization.deep_feature_factorization import DeepFeatureFactorization
+from pytorch_grad_cam.feature_factorization.deep_feature_factorization import DeepFeatureFactorization, run_dff_on_image
 import pytorch_grad_cam.utils.model_targets
 import pytorch_grad_cam.utils.reshape_transforms
 import pytorch_grad_cam.metrics.cam_mult_image
-import pytorch_grad_cam.metrics.road
+import pytorch_grad_cam.metrics.road
```

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/ablation_cam.py` & `grad-cam-1.4.6/pytorch_grad_cam/ablation_cam.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/ablation_cam_multilayer.py` & `grad-cam-1.4.6/pytorch_grad_cam/ablation_cam_multilayer.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/ablation_layer.py` & `grad-cam-1.4.6/pytorch_grad_cam/ablation_layer.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/activations_and_gradients.py` & `grad-cam-1.4.6/pytorch_grad_cam/activations_and_gradients.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/base_cam.py` & `grad-cam-1.4.6/pytorch_grad_cam/base_cam.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/eigen_cam.py` & `grad-cam-1.4.6/pytorch_grad_cam/eigen_cam.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/eigen_grad_cam.py` & `grad-cam-1.4.6/pytorch_grad_cam/eigen_grad_cam.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/feature_factorization/deep_feature_factorization.py` & `grad-cam-1.4.6/pytorch_grad_cam/feature_factorization/deep_feature_factorization.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
+from PIL import Image
 import torch
-from typing import Callable, List, Tuple
+from typing import Callable, List, Tuple, Optional
 from sklearn.decomposition import NMF
 from pytorch_grad_cam.activations_and_gradients import ActivationsAndGradients
-from pytorch_grad_cam.utils.image import scale_cam_image
+from pytorch_grad_cam.utils.image import scale_cam_image, create_labels_legend, show_factorization_on_image
 
 
 def dff(activations: np.ndarray, n_components: int = 5):
     """ Compute Deep Feature Factorization on a 2d Activations tensor.
 
     :param activations: A numpy array of shape batch x channels x height x width
     :param n_components: The number of components for the non negative matrix factorization
@@ -18,15 +19,15 @@
     batch_size, channels, h, w = activations.shape
     reshaped_activations = activations.transpose((1, 0, 2, 3))
     reshaped_activations[np.isnan(reshaped_activations)] = 0
     reshaped_activations = reshaped_activations.reshape(
         reshaped_activations.shape[0], -1)
     offset = reshaped_activations.min(axis=-1)
     reshaped_activations = reshaped_activations - offset[:, None]
-        
+
     model = NMF(n_components=n_components, init='random', random_state=0)
     W = model.fit_transform(reshaped_activations)
     H = model.components_
     concepts = W + offset[:, None]
     explanations = H.reshape(n_components, batch_size, h, w)
     explanations = explanations.transpose((1, 0, 2, 3))
     return concepts, explanations
@@ -56,19 +57,23 @@
             self.model, [target_layer], reshape_transform)
 
     def __call__(self,
                  input_tensor: torch.Tensor,
                  n_components: int = 16):
         batch_size, channels, h, w = input_tensor.size()
         _ = self.activations_and_grads(input_tensor)
-        activations = self.activations_and_grads.activations[0].cpu().numpy()
+
+        with torch.no_grad():
+            activations = self.activations_and_grads.activations[0].cpu(
+            ).numpy()
+
         concepts, explanations = dff(activations, n_components=n_components)
 
         processed_explanations = []
-        
+
         for batch in explanations:
             processed_explanations.append(scale_cam_image(batch, (w, h)))
 
         if self.computation_on_concepts:
             with torch.no_grad():
                 concept_tensors = torch.from_numpy(
                     np.float32(concepts).transpose((1, 0)))
@@ -84,7 +89,43 @@
     def __exit__(self, exc_type, exc_value, exc_tb):
         self.activations_and_grads.release()
         if isinstance(exc_value, IndexError):
             # Handle IndexError here...
             print(
                 f"An exception occurred in ActivationSummary with block: {exc_type}. Message: {exc_value}")
             return True
+
+
+def run_dff_on_image(model: torch.nn.Module,
+                     target_layer: torch.nn.Module,
+                     classifier: torch.nn.Module,
+                     img_pil: Image,
+                     img_tensor: torch.Tensor,
+                     reshape_transform=Optional[Callable],
+                     n_components: int = 5,
+                     top_k: int = 2) -> np.ndarray:
+    """ Helper function to create a Deep Feature Factorization visualization for a single image.
+        TBD: Run this on a batch with several images.
+    """
+    rgb_img_float = np.array(img_pil) / 255
+    dff = DeepFeatureFactorization(model=model,
+                                   reshape_transform=reshape_transform,
+                                   target_layer=target_layer,
+                                   computation_on_concepts=classifier)
+
+    concepts, batch_explanations, concept_outputs = dff(
+        img_tensor[None, :], n_components)
+
+    concept_outputs = torch.softmax(
+        torch.from_numpy(concept_outputs),
+        axis=-1).numpy()
+    concept_label_strings = create_labels_legend(concept_outputs,
+                                                 labels=model.config.id2label,
+                                                 top_k=top_k)
+    visualization = show_factorization_on_image(
+        rgb_img_float,
+        batch_explanations[0],
+        image_weight=0.3,
+        concept_labels=concept_label_strings)
+
+    result = np.hstack((np.array(img_pil), visualization))
+    return result
```

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/fullgrad_cam.py` & `grad-cam-1.4.6/pytorch_grad_cam/fullgrad_cam.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/grad_cam.py` & `grad-cam-1.4.6/pytorch_grad_cam/grad_cam.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/grad_cam_elementwise.py` & `grad-cam-1.4.6/pytorch_grad_cam/grad_cam_elementwise.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/grad_cam_plusplus.py` & `grad-cam-1.4.6/pytorch_grad_cam/grad_cam_plusplus.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/guided_backprop.py` & `grad-cam-1.4.6/pytorch_grad_cam/guided_backprop.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/hirescam.py` & `grad-cam-1.4.6/pytorch_grad_cam/hirescam.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/layer_cam.py` & `grad-cam-1.4.6/pytorch_grad_cam/layer_cam.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/metrics/cam_mult_image.py` & `grad-cam-1.4.6/pytorch_grad_cam/metrics/cam_mult_image.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/metrics/perturbation_confidence.py` & `grad-cam-1.4.6/pytorch_grad_cam/metrics/perturbation_confidence.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/metrics/road.py` & `grad-cam-1.4.6/pytorch_grad_cam/metrics/road.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/random_cam.py` & `grad-cam-1.4.6/pytorch_grad_cam/random_cam.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/score_cam.py` & `grad-cam-1.4.6/pytorch_grad_cam/score_cam.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/utils/find_layers.py` & `grad-cam-1.4.6/pytorch_grad_cam/utils/find_layers.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/utils/image.py` & `grad-cam-1.4.6/pytorch_grad_cam/utils/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import matplotlib
 from matplotlib import pyplot as plt
 from matplotlib.lines import Line2D
 import cv2
 import numpy as np
 import torch
 from torchvision.transforms import Compose, Normalize, ToTensor
-from typing import List
+from typing import List, Dict
+import math
 
 
 def preprocess_image(
     img: np.ndarray, mean=[
         0.5, 0.5, 0.5], std=[
             0.5, 0.5, 0.5]) -> torch.Tensor:
     preprocessing = Compose([
@@ -59,14 +60,30 @@
                 Got: {image_weight}")
 
     cam = (1 - image_weight) * heatmap + image_weight * img
     cam = cam / np.max(cam)
     return np.uint8(255 * cam)
 
 
+def create_labels_legend(concept_scores: np.ndarray,
+                         labels: Dict[int, str],
+                         top_k=2):
+    concept_categories = np.argsort(concept_scores, axis=1)[:, ::-1][:, :top_k]
+    concept_labels_topk = []
+    for concept_index in range(concept_categories.shape[0]):
+        categories = concept_categories[concept_index, :]
+        concept_labels = []
+        for category in categories:
+            score = concept_scores[concept_index, category]
+            label = f"{','.join(labels[category].split(',')[:3])}:{score:.2f}"
+            concept_labels.append(label)
+        concept_labels_topk.append("\n".join(concept_labels))
+    return concept_labels_topk
+
+
 def show_factorization_on_image(img: np.ndarray,
                                 explanations: np.ndarray,
                                 colors: List[np.ndarray] = None,
                                 image_weight: float = 0.5,
                                 concept_labels: List = None) -> np.ndarray:
     """ Color code the different component heatmaps on top of the image.
         Every component color code will be magnified according to the heatmap itensity
@@ -114,15 +131,16 @@
     mask = np.sum(np.float32(masks), axis=0)
     result = img * image_weight + mask * (1 - image_weight)
     result = np.uint8(result * 255)
 
     if concept_labels is not None:
         px = 1 / plt.rcParams['figure.dpi']  # pixel in inches
         fig = plt.figure(figsize=(result.shape[1] * px, result.shape[0] * px))
-        plt.rcParams['legend.fontsize'] = 15 * result.shape[0] / 256
+        plt.rcParams['legend.fontsize'] = int(
+            14 * result.shape[0] / 256 / max(1, n_components / 6))
         lw = 5 * result.shape[0] / 256
         lines = [Line2D([0], [0], color=colors[i], lw=lw)
                  for i in range(n_components)]
         plt.legend(lines,
                    concept_labels,
                    mode="expand",
                    fancybox=True,
```

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/utils/model_targets.py` & `grad-cam-1.4.6/pytorch_grad_cam/utils/model_targets.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/utils/reshape_transforms.py` & `grad-cam-1.4.6/pytorch_grad_cam/utils/reshape_transforms.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/utils/svd_on_activations.py` & `grad-cam-1.4.6/pytorch_grad_cam/utils/svd_on_activations.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/pytorch_grad_cam/xgrad_cam.py` & `grad-cam-1.4.6/pytorch_grad_cam/xgrad_cam.py`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/setup.cfg` & `grad-cam-1.4.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `grad-cam-1.4.5/setup.py` & `grad-cam-1.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.readlines()
 
 setuptools.setup(
     name='grad-cam',
-    version='1.4.5',
+    version='1.4.6',
     author='Jacob Gildenblat',
     author_email='jacob.gildenblat@gmail.com',
     description='Many Class Activation Map methods implemented in Pytorch for classification, segmentation, object detection and more',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/jacobgil/pytorch-grad-cam',
     project_urls={
         'Bug Tracker': 'https://github.com/jacobgil/pytorch-grad-cam/issues',
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    packages=setuptools.find_packages(exclude=["*tutorials*"]),
+    packages=setuptools.find_packages(
+        exclude=["*tutorials*"]),
     python_requires='>=3.6',
-    install_requires=requirements
-)
+    install_requires=requirements)
```

### Comparing `grad-cam-1.4.5/tests/test_context_release.py` & `grad-cam-1.4.6/tests/test_context_release.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,16 @@
     img = cv2.resize(numpy_image, (width, height))
     input_tensor = preprocess_image(img)
     input_tensor = input_tensor.repeat(batch_size, 1, 1, 1)
     model = cnn_model(pretrained=True)
     target_layers = []
     for layer in target_layer_names:
         target_layers.append(eval(f"model.{layer}"))
-    targets = [ClassifierOutputTarget(target_category) for _ in range(batch_size)]
+    targets = [ClassifierOutputTarget(target_category)
+               for _ in range(batch_size)]
     initial_memory = 0
     for i in range(100):
         with cam_method(model=model,
                         target_layers=target_layers,
                         use_cuda=False) as cam:
             grayscale_cam = cam(input_tensor=input_tensor,
                                 targets=targets,
```

### Comparing `grad-cam-1.4.5/tests/test_run_all_models.py` & `grad-cam-1.4.6/tests/test_run_all_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,17 +64,18 @@
         target_layers.append(eval(f"model.{layer}"))
 
     cam = cam_method(model=model,
                      target_layers=target_layers,
                      use_cuda=False)
     cam.batch_size = 4
     if target_category is None:
-      targets = None
+        targets = None
     else:
-      targets = [ClassifierOutputTarget(target_category) for _ in range(batch_size)]
+        targets = [ClassifierOutputTarget(target_category)
+                   for _ in range(batch_size)]
 
     grayscale_cam = cam(input_tensor=input_tensor,
                         targets=targets,
                         aug_smooth=aug_smooth,
                         eigen_smooth=eigen_smooth)
     assert(grayscale_cam.shape[0] == input_tensor.shape[0])
     assert(grayscale_cam.shape[1:] == input_tensor.shape[2:])
```

### Comparing `grad-cam-1.4.5/usage_examples/swinT_example.py` & `grad-cam-1.4.6/usage_examples/swinT_example.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     LayerCAM, \
     FullGrad
 
 from pytorch_grad_cam.utils.image import show_cam_on_image, \
     preprocess_image
 from pytorch_grad_cam.ablation_layer import AblationLayerVit
 
+
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument('--use-cuda', action='store_true', default=False,
                         help='Use NVIDIA GPU acceleration')
     parser.add_argument(
         '--image-path',
         type=str,
@@ -107,15 +108,14 @@
 
     rgb_img = cv2.imread(args.image_path, 1)[:, :, ::-1]
     rgb_img = cv2.resize(rgb_img, (224, 224))
     rgb_img = np.float32(rgb_img) / 255
     input_tensor = preprocess_image(rgb_img, mean=[0.5, 0.5, 0.5],
                                     std=[0.5, 0.5, 0.5])
 
-
     # AblationCAM and ScoreCAM have batched implementations.
     # You can override the internal batch size for faster computation.
     cam.batch_size = 32
 
     grayscale_cam = cam(input_tensor=input_tensor,
                         targets=None,
                         eigen_smooth=args.eigen_smooth,
```

### Comparing `grad-cam-1.4.5/usage_examples/vit_example.py` & `grad-cam-1.4.6/usage_examples/vit_example.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     FullGrad
 
 from pytorch_grad_cam import GuidedBackpropReLUModel
 from pytorch_grad_cam.utils.image import show_cam_on_image, \
     preprocess_image
 from pytorch_grad_cam.ablation_layer import AblationLayerVit
 
+
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument('--use-cuda', action='store_true', default=False,
                         help='Use NVIDIA GPU acceleration')
     parser.add_argument(
         '--image-path',
         type=str,
@@ -102,15 +103,14 @@
                                    ablation_layer=AblationLayerVit())
     else:
         cam = methods[args.method](model=model,
                                    target_layers=target_layers,
                                    use_cuda=args.use_cuda,
                                    reshape_transform=reshape_transform)
 
-
     rgb_img = cv2.imread(args.image_path, 1)[:, :, ::-1]
     rgb_img = cv2.resize(rgb_img, (224, 224))
     rgb_img = np.float32(rgb_img) / 255
     input_tensor = preprocess_image(rgb_img, mean=[0.5, 0.5, 0.5],
                                     std=[0.5, 0.5, 0.5])
 
     # If None, returns the map for the highest scoring category.
@@ -118,15 +118,15 @@
     targets = None
 
     # AblationCAM and ScoreCAM have batched implementations.
     # You can override the internal batch size for faster computation.
     cam.batch_size = 32
 
     grayscale_cam = cam(input_tensor=input_tensor,
-                        targets=targets ,
+                        targets=targets,
                         eigen_smooth=args.eigen_smooth,
                         aug_smooth=args.aug_smooth)
 
     # Here grayscale_cam has only one image in the batch
     grayscale_cam = grayscale_cam[0, :]
 
     cam_image = show_cam_on_image(rgb_img, grayscale_cam)
```

