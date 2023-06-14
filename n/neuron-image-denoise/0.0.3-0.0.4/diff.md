# Comparing `tmp/neuron-image-denoise-0.0.3.tar.gz` & `tmp/neuron-image-denoise-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuron-image-denoise-0.0.3.tar", last modified: Tue Jun  6 11:45:17 2023, max compression
+gzip compressed data, was "neuron-image-denoise-0.0.4.tar", last modified: Wed Jun 14 22:37:33 2023, max compression
```

## Comparing `neuron-image-denoise-0.0.3.tar` & `neuron-image-denoise-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 11:45:17.196068 neuron-image-denoise-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-06-06 11:45:17.178118 neuron-image-denoise-0.0.3/.github/
--rw-rw-rw-   0        0        0        6 2023-06-04 10:12:59.000000 neuron-image-denoise-0.0.3/.github/python-version.txt
-drwxrwxrwx   0        0        0        0 2023-06-06 11:45:17.179113 neuron-image-denoise-0.0.3/.github/workflows/
--rw-rw-rw-   0        0        0     1451 2023-06-04 10:12:59.000000 neuron-image-denoise-0.0.3/.github/workflows/static.yml
--rw-rw-rw-   0        0        0     3258 2023-06-06 05:03:03.000000 neuron-image-denoise-0.0.3/.gitignore
--rw-rw-rw-   0        0        0     1096 2023-06-03 10:23:41.000000 neuron-image-denoise-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       22 2023-06-04 10:06:59.000000 neuron-image-denoise-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2612 2023-06-06 11:45:17.196068 neuron-image-denoise-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1929 2023-06-06 10:08:32.000000 neuron-image-denoise-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 11:45:17.184101 neuron-image-denoise-0.0.3/neuron_image_denoise/
--rw-rw-rw-   0        0        0      219 2023-06-05 16:25:08.000000 neuron-image-denoise-0.0.3/neuron_image_denoise/__init__.py
--rw-rw-rw-   0        0        0     3272 2023-06-06 10:06:27.000000 neuron-image-denoise-0.0.3/neuron_image_denoise/_filter.pyx
--rw-rw-rw-   0        0        0     3195 2023-06-06 11:33:17.000000 neuron-image-denoise-0.0.3/neuron_image_denoise/filter.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:45:17.192079 neuron-image-denoise-0.0.3/neuron_image_denoise.egg-info/
--rw-rw-rw-   0        0        0     2612 2023-06-06 11:45:16.000000 neuron-image-denoise-0.0.3/neuron_image_denoise.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-06-06 11:45:17.000000 neuron-image-denoise-0.0.3/neuron_image_denoise.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 11:45:16.000000 neuron-image-denoise-0.0.3/neuron_image_denoise.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-06 11:45:16.000000 neuron-image-denoise-0.0.3/neuron_image_denoise.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-06 11:45:16.000000 neuron-image-denoise-0.0.3/neuron_image_denoise.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      947 2023-06-06 08:02:29.000000 neuron-image-denoise-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 11:45:17.197066 neuron-image-denoise-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      437 2023-06-04 10:22:19.000000 neuron-image-denoise-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:45:17.194098 neuron-image-denoise-0.0.3/test/
--rw-rw-rw-   0        0        0      317 2023-06-06 11:35:31.000000 neuron-image-denoise-0.0.3/test/case1.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:37:33.922193 neuron-image-denoise-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-06-14 22:37:33.905393 neuron-image-denoise-0.0.4/.github/
+-rw-rw-rw-   0        0        0        6 2023-06-04 10:12:59.000000 neuron-image-denoise-0.0.4/.github/python-version.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 22:37:33.906390 neuron-image-denoise-0.0.4/.github/workflows/
+-rw-rw-rw-   0        0        0     1451 2023-06-04 10:12:59.000000 neuron-image-denoise-0.0.4/.github/workflows/static.yml
+-rw-rw-rw-   0        0        0     3258 2023-06-06 05:03:03.000000 neuron-image-denoise-0.0.4/.gitignore
+-rw-rw-rw-   0        0        0     1096 2023-06-03 10:23:41.000000 neuron-image-denoise-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       22 2023-06-04 10:06:59.000000 neuron-image-denoise-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2664 2023-06-14 22:37:33.921216 neuron-image-denoise-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1981 2023-06-12 18:50:28.000000 neuron-image-denoise-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 22:37:33.910917 neuron-image-denoise-0.0.4/neuron_image_denoise/
+-rw-rw-rw-   0        0        0      219 2023-06-05 16:25:08.000000 neuron-image-denoise-0.0.4/neuron_image_denoise/__init__.py
+-rw-rw-rw-   0        0        0     3272 2023-06-06 10:06:27.000000 neuron-image-denoise-0.0.4/neuron_image_denoise/_filter.pyx
+-rw-rw-rw-   0        0        0     4394 2023-06-14 08:52:26.000000 neuron-image-denoise-0.0.4/neuron_image_denoise/filter.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:37:33.918238 neuron-image-denoise-0.0.4/neuron_image_denoise.egg-info/
+-rw-rw-rw-   0        0        0     2664 2023-06-14 22:37:33.000000 neuron-image-denoise-0.0.4/neuron_image_denoise.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-14 22:37:33.000000 neuron-image-denoise-0.0.4/neuron_image_denoise.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 22:37:33.000000 neuron-image-denoise-0.0.4/neuron_image_denoise.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-14 22:37:33.000000 neuron-image-denoise-0.0.4/neuron_image_denoise.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-14 22:37:33.000000 neuron-image-denoise-0.0.4/neuron_image_denoise.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      947 2023-06-06 08:02:29.000000 neuron-image-denoise-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 22:37:33.922193 neuron-image-denoise-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      437 2023-06-04 10:22:19.000000 neuron-image-denoise-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:37:33.919230 neuron-image-denoise-0.0.4/test/
+-rw-rw-rw-   0        0        0      317 2023-06-14 22:37:10.000000 neuron-image-denoise-0.0.4/test/case1.py
```

### Comparing `neuron-image-denoise-0.0.3/.github/workflows/static.yml` & `neuron-image-denoise-0.0.4/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `neuron-image-denoise-0.0.3/.gitignore` & `neuron-image-denoise-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `neuron-image-denoise-0.0.3/LICENSE` & `neuron-image-denoise-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `neuron-image-denoise-0.0.3/PKG-INFO` & `neuron-image-denoise-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuron-image-denoise
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fluorescent neuron image denoising tools
 Author-email: Zuohan Zhao <zzhmark@126.com>
 License: MIT License
 Project-URL: GitHub Project, https://github.com/SEU-ALLEN-codebase/neuron-image-denoise-py
 Project-URL: Documentation, https://SEU-ALLEN-codebase.github.io/neuron-image-denoise-py
 Keywords: vaa3d,neuron-morphology,image-processing
 Classifier: Programming Language :: Python :: 3
@@ -24,32 +24,32 @@
 ```
 
 # User Guide
 
 ```python
 from neuron_image_denoise.filter import *
 
-img: numpy.ndarray # 3D numpy array, 16bit
+img: numpy.ndarray  # 3D numpy array, 16bit
 
 params = {
-    'ada_interval': (2, 3, 3), 
+    'ada_interval': (2, 3, 3),
     'flare_interval': (2, 8, 8),
-    'ada_sampling': 3, 
-    'flare_sampling': 8, 
+    'ada_sampling': 3,
+    'flare_sampling': 8,
     'flare_weight': .02,
-    'atten_depth': 4, 
-    'flare_x':True, 
+    'atten_depth': 4,
+    'flare_x': True,
     'flare_y': True
 }
 
 out = adaptive_denoise(img, **params)
 
-out = adaptive_denoise_16to8(img, **params)   # 16bit to 8bit
+out = adaptive_denoise_16to8(img, **params)  # 16bit to 8bit
 
-out = gauss_attenuation_filter(img, 32, .1)
+out = adaptive_sectional_feedforward_filter(img, sigma=12., truncate=2., scaling=1, suppression=.8)
 ```
 
 ## Algorithm Explanation
 
 Neurons are illuminated by the fluorescent proteins, which can be seen as dots in the space. Measuring the signal is to 
 locate where the dots are, but the problem is, these dots can diffuse to outside of neurons and their light can be
 spreaded far away due to refraction and microcopy aberration.
```

### Comparing `neuron-image-denoise-0.0.3/README.md` & `neuron-image-denoise-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 ```
 
 # User Guide
 
 ```python
 from neuron_image_denoise.filter import *
 
-img: numpy.ndarray # 3D numpy array, 16bit
+img: numpy.ndarray  # 3D numpy array, 16bit
 
 params = {
-    'ada_interval': (2, 3, 3), 
+    'ada_interval': (2, 3, 3),
     'flare_interval': (2, 8, 8),
-    'ada_sampling': 3, 
-    'flare_sampling': 8, 
+    'ada_sampling': 3,
+    'flare_sampling': 8,
     'flare_weight': .02,
-    'atten_depth': 4, 
-    'flare_x':True, 
+    'atten_depth': 4,
+    'flare_x': True,
     'flare_y': True
 }
 
 out = adaptive_denoise(img, **params)
 
-out = adaptive_denoise_16to8(img, **params)   # 16bit to 8bit
+out = adaptive_denoise_16to8(img, **params)  # 16bit to 8bit
 
-out = gauss_attenuation_filter(img, 32, .1)
+out = adaptive_sectional_feedforward_filter(img, sigma=12., truncate=2., scaling=1, suppression=.8)
 ```
 
 ## Algorithm Explanation
 
 Neurons are illuminated by the fluorescent proteins, which can be seen as dots in the space. Measuring the signal is to 
 locate where the dots are, but the problem is, these dots can diffuse to outside of neurons and their light can be
 spreaded far away due to refraction and microcopy aberration.
```

### Comparing `neuron-image-denoise-0.0.3/neuron_image_denoise/_filter.pyx` & `neuron-image-denoise-0.0.4/neuron_image_denoise/_filter.pyx`

 * *Files identical despite different names*

### Comparing `neuron-image-denoise-0.0.3/neuron_image_denoise.egg-info/PKG-INFO` & `neuron-image-denoise-0.0.4/neuron_image_denoise.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuron-image-denoise
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fluorescent neuron image denoising tools
 Author-email: Zuohan Zhao <zzhmark@126.com>
 License: MIT License
 Project-URL: GitHub Project, https://github.com/SEU-ALLEN-codebase/neuron-image-denoise-py
 Project-URL: Documentation, https://SEU-ALLEN-codebase.github.io/neuron-image-denoise-py
 Keywords: vaa3d,neuron-morphology,image-processing
 Classifier: Programming Language :: Python :: 3
@@ -24,32 +24,32 @@
 ```
 
 # User Guide
 
 ```python
 from neuron_image_denoise.filter import *
 
-img: numpy.ndarray # 3D numpy array, 16bit
+img: numpy.ndarray  # 3D numpy array, 16bit
 
 params = {
-    'ada_interval': (2, 3, 3), 
+    'ada_interval': (2, 3, 3),
     'flare_interval': (2, 8, 8),
-    'ada_sampling': 3, 
-    'flare_sampling': 8, 
+    'ada_sampling': 3,
+    'flare_sampling': 8,
     'flare_weight': .02,
-    'atten_depth': 4, 
-    'flare_x':True, 
+    'atten_depth': 4,
+    'flare_x': True,
     'flare_y': True
 }
 
 out = adaptive_denoise(img, **params)
 
-out = adaptive_denoise_16to8(img, **params)   # 16bit to 8bit
+out = adaptive_denoise_16to8(img, **params)  # 16bit to 8bit
 
-out = gauss_attenuation_filter(img, 32, .1)
+out = adaptive_sectional_feedforward_filter(img, sigma=12., truncate=2., scaling=1, suppression=.8)
 ```
 
 ## Algorithm Explanation
 
 Neurons are illuminated by the fluorescent proteins, which can be seen as dots in the space. Measuring the signal is to 
 locate where the dots are, but the problem is, these dots can diffuse to outside of neurons and their light can be
 spreaded far away due to refraction and microcopy aberration.
```

### Comparing `neuron-image-denoise-0.0.3/pyproject.toml` & `neuron-image-denoise-0.0.4/pyproject.toml`

 * *Files identical despite different names*

