# Comparing `tmp/cryoCARE-0.2.2.tar.gz` & `tmp/cryoCARE-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryoCARE-0.2.2.tar", last modified: Wed Mar  1 12:07:54 2023, max compression
+gzip compressed data, was "cryoCARE-0.3.0.tar", last modified: Thu Jun 15 13:34:42 2023, max compression
```

## Comparing `cryoCARE-0.2.2.tar` & `cryoCARE-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-01 12:07:54.563096 cryoCARE-0.2.2/
--rw-r--r--   0 twagner  (22293) domain users (32000)     1514 2022-10-05 15:29:22.000000 cryoCARE-0.2.2/LICENSE
--rw-r--r--   0 twagner  (22293) domain users (32000)     8551 2023-03-01 12:07:54.563096 cryoCARE-0.2.2/PKG-INFO
--rw-r--r--   0 twagner  (22293) domain users (32000)     6539 2022-11-11 14:28:06.000000 cryoCARE-0.2.2/README.md
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-01 12:07:54.563096 cryoCARE-0.2.2/cryoCARE.egg-info/
--rw-r--r--   0 twagner  (22293) domain users (32000)     8551 2023-03-01 12:07:54.000000 cryoCARE-0.2.2/cryoCARE.egg-info/PKG-INFO
--rw-r--r--   0 twagner  (22293) domain users (32000)      458 2023-03-01 12:07:54.000000 cryoCARE-0.2.2/cryoCARE.egg-info/SOURCES.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)        1 2023-03-01 12:07:54.000000 cryoCARE-0.2.2/cryoCARE.egg-info/dependency_links.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)       43 2023-03-01 12:07:54.000000 cryoCARE-0.2.2/cryoCARE.egg-info/requires.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)        9 2023-03-01 12:07:54.000000 cryoCARE-0.2.2/cryoCARE.egg-info/top_level.txt
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-01 12:07:54.563096 cryoCARE-0.2.2/cryocare/
--rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-10-05 15:29:22.000000 cryoCARE-0.2.2/cryocare/__init__.py
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-01 12:07:54.563096 cryoCARE-0.2.2/cryocare/internals/
--rw-r--r--   0 twagner  (22293) domain users (32000)    16339 2023-03-01 10:42:16.000000 cryoCARE-0.2.2/cryocare/internals/CryoCARE.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    12137 2023-03-01 10:42:16.000000 cryoCARE-0.2.2/cryocare/internals/CryoCAREDataModule.py
--rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-10-05 15:29:22.000000 cryoCARE-0.2.2/cryocare/internals/__init__.py
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-03-01 12:07:54.563096 cryoCARE-0.2.2/cryocare/scripts/
--rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-10-05 15:29:22.000000 cryoCARE-0.2.2/cryocare/scripts/__init__.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1383 2022-10-05 15:29:22.000000 cryoCARE-0.2.2/cryocare/scripts/cryoCARE_extract_train_data.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     6184 2023-03-01 10:42:16.000000 cryoCARE-0.2.2/cryocare/scripts/cryoCARE_predict.py
--rw-r--r--   0 twagner  (22293) domain users (32000)     1893 2022-10-05 15:29:22.000000 cryoCARE-0.2.2/cryocare/scripts/cryoCARE_train.py
--rw-r--r--   0 twagner  (22293) domain users (32000)       38 2023-03-01 12:07:54.563096 cryoCARE-0.2.2/setup.cfg
--rw-r--r--   0 twagner  (22293) domain users (32000)     1147 2023-03-01 12:07:22.000000 cryoCARE-0.2.2/setup.py
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-06-15 13:34:42.247230 cryoCARE-0.3.0/
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1807 2022-10-05 15:29:22.000000 cryoCARE-0.3.0/.gitignore
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1514 2022-10-05 15:29:22.000000 cryoCARE-0.3.0/LICENSE
+-rw-r--r--   0 twagner  (22293) domain users (32000)     8756 2023-06-15 13:34:42.247230 cryoCARE-0.3.0/PKG-INFO
+-rw-r--r--   0 twagner  (22293) domain users (32000)     8130 2023-06-15 13:33:09.000000 cryoCARE-0.3.0/README.md
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-06-15 13:34:42.247230 cryoCARE-0.3.0/cryoCARE.egg-info/
+-rw-r--r--   0 twagner  (22293) domain users (32000)     8756 2023-06-15 13:34:42.000000 cryoCARE-0.3.0/cryoCARE.egg-info/PKG-INFO
+-rw-r--r--   0 twagner  (22293) domain users (32000)      530 2023-06-15 13:34:42.000000 cryoCARE-0.3.0/cryoCARE.egg-info/SOURCES.txt
+-rw-r--r--   0 twagner  (22293) domain users (32000)        1 2023-06-15 13:34:42.000000 cryoCARE-0.3.0/cryoCARE.egg-info/dependency_links.txt
+-rw-r--r--   0 twagner  (22293) domain users (32000)       51 2023-06-15 13:34:42.000000 cryoCARE-0.3.0/cryoCARE.egg-info/requires.txt
+-rw-r--r--   0 twagner  (22293) domain users (32000)        9 2023-06-15 13:34:42.000000 cryoCARE-0.3.0/cryoCARE.egg-info/top_level.txt
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-06-15 13:34:42.247230 cryoCARE-0.3.0/cryocare/
+-rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-10-05 15:29:22.000000 cryoCARE-0.3.0/cryocare/__init__.py
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-06-15 13:34:42.247230 cryoCARE-0.3.0/cryocare/internals/
+-rw-r--r--   0 twagner  (22293) domain users (32000)    16339 2023-03-01 10:42:16.000000 cryoCARE-0.3.0/cryocare/internals/CryoCARE.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    12137 2023-03-01 10:42:16.000000 cryoCARE-0.3.0/cryocare/internals/CryoCAREDataModule.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-10-05 15:29:22.000000 cryoCARE-0.3.0/cryocare/internals/__init__.py
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-06-15 13:34:42.247230 cryoCARE-0.3.0/cryocare/scripts/
+-rw-r--r--   0 twagner  (22293) domain users (32000)        0 2022-10-05 15:29:22.000000 cryoCARE-0.3.0/cryocare/scripts/__init__.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1383 2022-10-05 15:29:22.000000 cryoCARE-0.3.0/cryocare/scripts/cryoCARE_extract_train_data.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     6184 2023-03-01 10:42:16.000000 cryoCARE-0.3.0/cryocare/scripts/cryoCARE_predict.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)     2033 2023-06-15 13:33:09.000000 cryoCARE-0.3.0/cryocare/scripts/cryoCARE_train.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      202 2023-03-01 10:42:16.000000 cryoCARE-0.3.0/predict_config.json
+-rw-r--r--   0 twagner  (22293) domain users (32000)       38 2023-06-15 13:34:42.247230 cryoCARE-0.3.0/setup.cfg
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1155 2023-06-15 13:33:40.000000 cryoCARE-0.3.0/setup.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)      242 2022-11-11 14:28:06.000000 cryoCARE-0.3.0/train_config.json
+-rw-r--r--   0 twagner  (22293) domain users (32000)      237 2022-10-05 15:29:22.000000 cryoCARE-0.3.0/train_data_config.json
```

### Comparing `cryoCARE-0.2.2/LICENSE` & `cryoCARE-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cryoCARE-0.2.2/PKG-INFO` & `cryoCARE-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,187 +1,215 @@
 Metadata-Version: 2.1
 Name: cryoCARE
-Version: 0.2.2
+Version: 0.3.0
 Summary: cryoCARE is a deep learning approach for cryo-TEM tomogram denoising.
 Home-page: https://github.com/juglab/cryoCARE_pip
 Author: Tim-Oliver Buchholz, Thorsten Wagner
 Author-email: tim-oliver.buchholz@fmi.ch, thorsten.wagner@mpi-dortmund.mpg.de
-License: UNKNOWN
-Description: # cryoCARE
-        
-        This package is a memory efficient implementation of [cryoCARE](https://github.com/juglab/cryoCARE_T2T). 
-        
-        This setup trains a denoising U-Net for tomographic reconstruction according to the [Noise2Noise](https://arxiv.org/pdf/1803.04189.pdf) training paradigm. 
-        Therefore the user has to provide two tomograms of the same sample. 
-        The simplest way to achieve this is with direct-detector movie-frames.
-        
-        You can use Warp to generate two reconstructed tomograms based on the even/odd frames. Alternatively, the movie-frames can be split in two halves (e.g. with MotionCor2 `-SplitSum 1` or with IMOD `alignframes -debug 10000`) from which two identical, up to random noise, tomograms can be reconstructed. 
-        
-        These two (even and odd) tomograms can be used as input to this cryoCARE implementation.
-        
-        ## Changelog
-        
-        ### Version 0.2
-        
-        * `cyroCARE_train` produces a compressed and more portable model. This model can be copied and shared with others without relying on a certain folder structure.
-        * `cryoCARE_predict` supports to predict multiple tomograms in one run. Streamlined configuration with respect to the changes of `cryoCARE_train`.
-        * Streamlined installation instructions
-        * CUDA 11 support
-        * Minor changes/ fixed couple of bugs:
-            * Proper padding of tomograms to avoid black frames in the denoised tomograms
-            * Fix computation of validation cut off for small tomograms
-            * Fix `cryoCARE_predict` if no tiling happens
-        
-        ## Installation
-        
-        __Note:__ We assume that you have  [miniconda](https://docs.conda.io/en/latest/miniconda.html) installed.
-        
-        First you need to create a conda environment.
-        
-        ### For CUDA 11:
-        ```
-        conda create -n cryocare_11 python=3.8 cudatoolkit=11.0 cudnn=8.0 -c conda-forge
-        conda activate cryocare_11
-        pip install tensorflow==2.4
-        pip install cryoCARE
-        ```
-        
-        ### For CUDA 10:
-        ```
-        conda create -n cryocare -c conda-forge -c anaconda python=3 keras-gpu=2.3.1
-        conda activate cryocare
-        pip install cryoCARE
-        ```
-        
-        ## Manual
-        cryoCARE uses `.json` configuration files and is run in three steps:
-        
-        ### 1. Prepare Training Data
-        To prepare the training data we have to provide all tomograms on which we want to train. 
-        Create an empty file called `train_data_config.json`, copy-paste the following template and fill it in.
-        ```
-        {
-          "even": [
-            "/path/to/even.rec"
-          ],
-          "odd": [
-            "/path/to/odd.rec"
-          ],
-          "patch_shape": [
-            72,
-            72,
-            72
-          ],
-          "num_slices": 1200,
-          "split": 0.9,
-          "tilt_axis": "Y",
-          "n_normalization_samples": 500,
-          "path": "./"
-        }
-        ```
-        #### Parameters:
-        * `"even"`: List of all even tomograms.
-        * `"odd"`: List of all odd tomograms. Note the order has to be the same as in `"even"`.
-        * `"patch_shape"`: Size of the sub-volumes used for training. Should not be smaller than `64, 64, 64`.
-        * `"num_slices"`: Number of sub-volumes extracted per tomograms. 
-        * `"tilt_axis"`: Tilt-axis of the tomograms. We split the tomogram along this axis to extract train- and validation data separately.
-        * `"n_normalization_samples"`: Number of sub-volumes extracted per tomograms, which are used to compute `mean` and `standard deviation` for normalization.
-        * `"path"`: The training and validation data are saved here.
-        
-        #### Run Training Data Preparation:
-        After installation of the package we have access to built in Python-scripts which we can call. 
-        To run the training data preparation we run the following command:
-        `cryoCARE_extract_train_data.py --conf train_data_config.json`
-        
-        ### 2. Training
-        Create an empty file called `train_config.json`, copy-paste the following template and fill it in.
-        ```
-        {
-          "train_data": "./",
-          "epochs": 100,
-          "steps_per_epoch": 200,
-          "batch_size": 16,
-          "unet_kern_size": 3,
-          "unet_n_depth": 3,
-          "unet_n_first": 16,
-          "learning_rate": 0.0004,
-          "model_name": "model_name",
-          "path": "./",
-          "gpu_id": 0
-        }
-        ```
-        
-        #### Parameters:
-        * `"train_data"`: Path to the directory containing the train- and validation data. This should be the same as the `"path"` from above.
-        * `"epochs"`: Number of epochs used to train the network.
-        * `"steps_per_epoch"`: Number of gradient steps performed per epoch.
-        * `"batch_size"`: Used training batch size.
-        * `"unet_kern_size"`: Convolution kernel size of the U-Net. Has to be an odd number.
-        * `"unet_n_depth"`: Depth of the U-Net.
-        * `"unet_n_first"`: Number of initial feature channels.
-        * `"learning_rate"`: Learning rate of the model training.
-        * `"model_name"`: Name of the model.
-        * `"path"`: Output path for the model.
-        * `"gpu_id"`: This is optional. Provide the GPU ID(s) of the GPUs you wish to use.
-        
-        #### Run Training:
-        To run the training we run the following command:
-        `cryoCARE_train.py --conf train_config.json`
-        
-        You will find a `.tar.gz` file in the directory you specified as `path`. This your model an will be used in the next step.
-        
-        ### 3. Prediction
-        Create an empty file called `predict_config.json`, copy-paste the following template and fill it in.
-        ```
-        {
-          "path": "path/to/your/model/model_name.tar.gz",
-          "even": "/path/to/even.rec",
-          "odd": "/path/to/odd.rec",
-          "n_tiles": [1,1,1],
-          "output": "denoised.rec",
-          "overwrite": False,
-          "gpu_id": 0
-        }
-        ```
-        
-        #### Parameters:
-        * `"path"`: Path to your model file.
-        * `"even"`: Path to directory with even tomograms or a specific even tomogram or a list of specific even tomograms.
-        * `"odd"`: Path to directory with odd tomograms or a specific odd tomogram or a list of specific odd tomograms in the same order as the even tomograms.
-        * `"n_tiles"`: Initial tiles per dimension. Gets increased if the tiles do not fit on the GPU.
-        * `"output"`: Path where the denoised tomograms will be written.
-        * `"overwrite"`: Allow previous files to be overwritten.
-        * `"gpu_id"`: This is optional. Provide the GPU ID(s) of the GPUs you wish to use.
-        
-        #### Run Prediction:
-        To run the training we run the following command:
-        `cryoCARE_predict.py --conf predict_config.json`
-        
-        ## How to Cite
-        ```
-        @inproceedings{buchholz2019cryo,
-          title={Cryo-CARE: content-aware image restoration for cryo-transmission electron microscopy data},
-          author={Buchholz, Tim-Oliver and Jordan, Mareike and Pigino, Gaia and Jug, Florian},
-          booktitle={2019 IEEE 16th International Symposium on Biomedical Imaging (ISBI 2019)},
-          pages={502--506},
-          year={2019},
-          organization={IEEE}
-        }
-        
-        @article{buchholz2019content,
-          title={Content-aware image restoration for electron microscopy.},
-          author={Buchholz, Tim-Oliver and Krull, Alexander and Shahidi, R{\'e}za and Pigino, Gaia and J{\'e}kely, G{\'a}sp{\'a}r and Jug, Florian},
-          journal={Methods in cell biology},
-          volume={152},
-          pages={277--289},
-          year={2019}
-        }
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# cryoCARE
+
+This package is a memory efficient implementation of [cryoCARE](https://github.com/juglab/cryoCARE_T2T). 
+
+This setup trains a denoising U-Net for tomographic reconstruction according to the [Noise2Noise](https://arxiv.org/pdf/1803.04189.pdf) training paradigm. 
+Therefore the user has to provide two tomograms of the same sample. 
+The simplest way to achieve this is with direct-detector movie-frames.
+
+You can use Warp to generate two reconstructed tomograms based on the even/odd frames. Alternatively, the movie-frames can be split in two halves (e.g. with MotionCor2 `-SplitSum 1` or with IMOD `alignframes -debug 10000`) from which two identical, up to random noise, tomograms can be reconstructed. 
+
+These two (even and odd) tomograms can be used as input to this cryoCARE implementation.
+
+## Changelog
+
+
+### Version 0.3
+
+* `cyroCARE_train` now supports parallelization over multiple GPUs.
+
+### Version 0.2
+
+* `cyroCARE_train` produces a compressed and more portable model. This model can be copied and shared with others without relying on a certain folder structure.
+* `cryoCARE_predict` supports to predict multiple tomograms in one run. Streamlined configuration with respect to the changes of `cryoCARE_train`.
+* Streamlined installation instructions
+* CUDA 11 support
+* Minor changes/ fixed couple of bugs:
+    * Proper padding of tomograms to avoid black frames in the denoised tomograms
+    * Fix computation of validation cut off for small tomograms
+    * Fix `cryoCARE_predict` if no tiling happens
+
+## Installation
+
+__Note:__ We assume that you have  [miniconda](https://docs.conda.io/en/latest/miniconda.html) installed.
+
+First you need to create a conda environment.
+
+### For CUDA 11:
+```
+conda create -n cryocare_11 python=3.8 cudatoolkit=11.0 cudnn=8.0 -c conda-forge
+conda activate cryocare_11
+pip install tensorflow==2.4
+pip install cryoCARE
+```
+
+### For CUDA 10:
+```
+conda create -n cryocare -c conda-forge -c anaconda python=3 keras-gpu=2.3.1
+conda activate cryocare
+pip install cryoCARE
+```
+
+## Manual
+cryoCARE uses `.json` configuration files and is run in three steps:
+
+### 1. Prepare Training Data
+To prepare the training data we have to provide all tomograms on which we want to train. 
+Create an empty file called `train_data_config.json`, copy-paste the following template and fill it in.
+```
+{
+  "even": [
+    "/path/to/even.rec"
+  ],
+  "odd": [
+    "/path/to/odd.rec"
+  ],
+  "patch_shape": [
+    72,
+    72,
+    72
+  ],
+  "num_slices": 1200,
+  "split": 0.9,
+  "tilt_axis": "Y",
+  "n_normalization_samples": 500,
+  "path": "./"
+}
+```
+#### Parameters:
+* `"even"`: List of all even tomograms.
+* `"odd"`: List of all odd tomograms. Note the order has to be the same as in `"even"`.
+* `"patch_shape"`: Size of the sub-volumes used for training. Should not be smaller than `64, 64, 64`.
+* `"num_slices"`: Number of sub-volumes extracted per tomograms. 
+* `"tilt_axis"`: Tilt-axis of the tomograms. We split the tomogram along this axis to extract train- and validation data separately.
+* `"n_normalization_samples"`: Number of sub-volumes extracted per tomograms, which are used to compute `mean` and `standard deviation` for normalization.
+* `"path"`: The training and validation data are saved here.
+
+#### Run Training Data Preparation:
+After installation of the package we have access to built in Python-scripts which we can call. 
+To run the training data preparation we run the following command:
+`cryoCARE_extract_train_data.py --conf train_data_config.json`
+
+### 2. Training
+Create an empty file called `train_config.json`, copy-paste the following template and fill it in.
+```
+{
+  "train_data": "./",
+  "epochs": 100,
+  "steps_per_epoch": 200,
+  "batch_size": 16,
+  "unet_kern_size": 3,
+  "unet_n_depth": 3,
+  "unet_n_first": 16,
+  "learning_rate": 0.0004,
+  "model_name": "model_name",
+  "path": "./",
+  "gpu_id": 0
+}
+```
+
+#### Parameters:
+* `"train_data"`: Path to the directory containing the train- and validation data. This should be the same as the `"path"` from above.
+* `"epochs"`: Number of epochs used to train the network.
+* `"steps_per_epoch"`: Number of gradient steps performed per epoch.
+* `"batch_size"`: Used training batch size.
+* `"unet_kern_size"`: Convolution kernel size of the U-Net. Has to be an odd number.
+* `"unet_n_depth"`: Depth of the U-Net.
+* `"unet_n_first"`: Number of initial feature channels.
+* `"learning_rate"`: Learning rate of the model training.
+* `"model_name"`: Name of the model.
+* `"path"`: Output path for the model.
+* `"gpu_id"`: This is optional. Provide the ID(s) of the GPUs you wish to use. Alternatively, you can specify the GPU ID(s) using the `CUDA_VISIBLE_DEVICES` environment variable. Training supports multiple GPUs (see below).
+
+#### Run Training:
+To run the training we run the following command:
+`cryoCARE_train.py --conf train_config.json`
+
+You will find a `.tar.gz` file in the directory you specified as `path`. This your model an will be used in the next step.
+
+##### Train using multiple GPUs:
+Training can be faster by running on multiple GPUs (which must be available in the same machine). Please note that the performance does not improve linearly with the number of devices used for training. The actual speedup will depend on your training settings and hardware.
+
+There are two methods for specifying multiple GPU ID(s):
+
+###### Method 1: Using `gpu_id`
+
+You can specify multiple GPU ID(s) in the `train_config.json` file as follows (with 4 GPUs in this example):
+
+`"gpu_id": [0,1,2,3]`
+
+**Note:** This method takes precedence over the `CUDA_VISIBLE_DEVICES` method below. If you want to use that method, you should **omit** the `"gpu_id"` entry from your `train_config.json` file.
+
+###### Method 2: Using the `CUDA_VISIBLE_DEVICES` environment variable
+
+For example, with 4 GPUs:
+
+````
+export CUDA_VISIBLE_DEVICES=0,1,2,3
+cryoCARE_train.py --conf train_config.json
+````
+
+**Note:** If running cryoCARE under a cluster resource manager such as SLURM, the `CUDA_VISIBLE_DEVICES` environment variable might be automatically set when you request a certain number of GPUs, so you don't need to set it explicitly. Check your cluster documentation or support team for details.
+
+### 3. Prediction
+Create an empty file called `predict_config.json`, copy-paste the following template and fill it in.
+```
+{
+  "path": "path/to/your/model/model_name.tar.gz",
+  "even": "/path/to/even.rec",
+  "odd": "/path/to/odd.rec",
+  "n_tiles": [1,1,1],
+  "output": "denoised.rec",
+  "overwrite": False,
+  "gpu_id": 0
+}
+```
+
+#### Parameters:
+* `"path"`: Path to your model file.
+* `"even"`: Path to directory with even tomograms or a specific even tomogram or a list of specific even tomograms.
+* `"odd"`: Path to directory with odd tomograms or a specific odd tomogram or a list of specific odd tomograms in the same order as the even tomograms.
+* `"n_tiles"`: Initial tiles per dimension. Gets increased if the tiles do not fit on the GPU.
+* `"output"`: Path where the denoised tomograms will be written.
+* `"overwrite"`: Allow previous files to be overwritten.
+* `"gpu_id"`: This is optional. Provide the ID of the GPU you wish to use. Alternatively, you can specify the GPU ID using the `CUDA_VISIBLE_DEVICES` environment variable. Note that prediction only supports a single GPU currently.
+
+#### Run Prediction:
+To run the training we run the following command:
+`cryoCARE_predict.py --conf predict_config.json`
+
+## How to Cite
+```
+@inproceedings{buchholz2019cryo,
+  title={Cryo-CARE: content-aware image restoration for cryo-transmission electron microscopy data},
+  author={Buchholz, Tim-Oliver and Jordan, Mareike and Pigino, Gaia and Jug, Florian},
+  booktitle={2019 IEEE 16th International Symposium on Biomedical Imaging (ISBI 2019)},
+  pages={502--506},
+  year={2019},
+  organization={IEEE}
+}
+
+@article{buchholz2019content,
+  title={Content-aware image restoration for electron microscopy.},
+  author={Buchholz, Tim-Oliver and Krull, Alexander and Shahidi, R{\'e}za and Pigino, Gaia and J{\'e}kely, G{\'a}sp{\'a}r and Jug, Florian},
+  journal={Methods in cell biology},
+  volume={152},
+  pages={277--289},
+  year={2019}
+}
+```
```

### Comparing `cryoCARE-0.2.2/README.md` & `cryoCARE-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 
 You can use Warp to generate two reconstructed tomograms based on the even/odd frames. Alternatively, the movie-frames can be split in two halves (e.g. with MotionCor2 `-SplitSum 1` or with IMOD `alignframes -debug 10000`) from which two identical, up to random noise, tomograms can be reconstructed. 
 
 These two (even and odd) tomograms can be used as input to this cryoCARE implementation.
 
 ## Changelog
 
+
+### Version 0.3
+
+* `cyroCARE_train` now supports parallelization over multiple GPUs.
+
 ### Version 0.2
 
 * `cyroCARE_train` produces a compressed and more portable model. This model can be copied and shared with others without relying on a certain folder structure.
 * `cryoCARE_predict` supports to predict multiple tomograms in one run. Streamlined configuration with respect to the changes of `cryoCARE_train`.
 * Streamlined installation instructions
 * CUDA 11 support
 * Minor changes/ fixed couple of bugs:
@@ -109,22 +114,46 @@
 * `"batch_size"`: Used training batch size.
 * `"unet_kern_size"`: Convolution kernel size of the U-Net. Has to be an odd number.
 * `"unet_n_depth"`: Depth of the U-Net.
 * `"unet_n_first"`: Number of initial feature channels.
 * `"learning_rate"`: Learning rate of the model training.
 * `"model_name"`: Name of the model.
 * `"path"`: Output path for the model.
-* `"gpu_id"`: This is optional. Provide the GPU ID(s) of the GPUs you wish to use.
+* `"gpu_id"`: This is optional. Provide the ID(s) of the GPUs you wish to use. Alternatively, you can specify the GPU ID(s) using the `CUDA_VISIBLE_DEVICES` environment variable. Training supports multiple GPUs (see below).
 
 #### Run Training:
 To run the training we run the following command:
 `cryoCARE_train.py --conf train_config.json`
 
 You will find a `.tar.gz` file in the directory you specified as `path`. This your model an will be used in the next step.
 
+##### Train using multiple GPUs:
+Training can be faster by running on multiple GPUs (which must be available in the same machine). Please note that the performance does not improve linearly with the number of devices used for training. The actual speedup will depend on your training settings and hardware.
+
+There are two methods for specifying multiple GPU ID(s):
+
+###### Method 1: Using `gpu_id`
+
+You can specify multiple GPU ID(s) in the `train_config.json` file as follows (with 4 GPUs in this example):
+
+`"gpu_id": [0,1,2,3]`
+
+**Note:** This method takes precedence over the `CUDA_VISIBLE_DEVICES` method below. If you want to use that method, you should **omit** the `"gpu_id"` entry from your `train_config.json` file.
+
+###### Method 2: Using the `CUDA_VISIBLE_DEVICES` environment variable
+
+For example, with 4 GPUs:
+
+````
+export CUDA_VISIBLE_DEVICES=0,1,2,3
+cryoCARE_train.py --conf train_config.json
+````
+
+**Note:** If running cryoCARE under a cluster resource manager such as SLURM, the `CUDA_VISIBLE_DEVICES` environment variable might be automatically set when you request a certain number of GPUs, so you don't need to set it explicitly. Check your cluster documentation or support team for details.
+
 ### 3. Prediction
 Create an empty file called `predict_config.json`, copy-paste the following template and fill it in.
 ```
 {
   "path": "path/to/your/model/model_name.tar.gz",
   "even": "/path/to/even.rec",
   "odd": "/path/to/odd.rec",
@@ -138,15 +167,15 @@
 #### Parameters:
 * `"path"`: Path to your model file.
 * `"even"`: Path to directory with even tomograms or a specific even tomogram or a list of specific even tomograms.
 * `"odd"`: Path to directory with odd tomograms or a specific odd tomogram or a list of specific odd tomograms in the same order as the even tomograms.
 * `"n_tiles"`: Initial tiles per dimension. Gets increased if the tiles do not fit on the GPU.
 * `"output"`: Path where the denoised tomograms will be written.
 * `"overwrite"`: Allow previous files to be overwritten.
-* `"gpu_id"`: This is optional. Provide the GPU ID(s) of the GPUs you wish to use.
+* `"gpu_id"`: This is optional. Provide the ID of the GPU you wish to use. Alternatively, you can specify the GPU ID using the `CUDA_VISIBLE_DEVICES` environment variable. Note that prediction only supports a single GPU currently.
 
 #### Run Prediction:
 To run the training we run the following command:
 `cryoCARE_predict.py --conf predict_config.json`
 
 ## How to Cite
 ```
```

### Comparing `cryoCARE-0.2.2/cryoCARE.egg-info/PKG-INFO` & `cryoCARE-0.3.0/cryoCARE.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,187 +1,215 @@
 Metadata-Version: 2.1
 Name: cryoCARE
-Version: 0.2.2
+Version: 0.3.0
 Summary: cryoCARE is a deep learning approach for cryo-TEM tomogram denoising.
 Home-page: https://github.com/juglab/cryoCARE_pip
 Author: Tim-Oliver Buchholz, Thorsten Wagner
 Author-email: tim-oliver.buchholz@fmi.ch, thorsten.wagner@mpi-dortmund.mpg.de
-License: UNKNOWN
-Description: # cryoCARE
-        
-        This package is a memory efficient implementation of [cryoCARE](https://github.com/juglab/cryoCARE_T2T). 
-        
-        This setup trains a denoising U-Net for tomographic reconstruction according to the [Noise2Noise](https://arxiv.org/pdf/1803.04189.pdf) training paradigm. 
-        Therefore the user has to provide two tomograms of the same sample. 
-        The simplest way to achieve this is with direct-detector movie-frames.
-        
-        You can use Warp to generate two reconstructed tomograms based on the even/odd frames. Alternatively, the movie-frames can be split in two halves (e.g. with MotionCor2 `-SplitSum 1` or with IMOD `alignframes -debug 10000`) from which two identical, up to random noise, tomograms can be reconstructed. 
-        
-        These two (even and odd) tomograms can be used as input to this cryoCARE implementation.
-        
-        ## Changelog
-        
-        ### Version 0.2
-        
-        * `cyroCARE_train` produces a compressed and more portable model. This model can be copied and shared with others without relying on a certain folder structure.
-        * `cryoCARE_predict` supports to predict multiple tomograms in one run. Streamlined configuration with respect to the changes of `cryoCARE_train`.
-        * Streamlined installation instructions
-        * CUDA 11 support
-        * Minor changes/ fixed couple of bugs:
-            * Proper padding of tomograms to avoid black frames in the denoised tomograms
-            * Fix computation of validation cut off for small tomograms
-            * Fix `cryoCARE_predict` if no tiling happens
-        
-        ## Installation
-        
-        __Note:__ We assume that you have  [miniconda](https://docs.conda.io/en/latest/miniconda.html) installed.
-        
-        First you need to create a conda environment.
-        
-        ### For CUDA 11:
-        ```
-        conda create -n cryocare_11 python=3.8 cudatoolkit=11.0 cudnn=8.0 -c conda-forge
-        conda activate cryocare_11
-        pip install tensorflow==2.4
-        pip install cryoCARE
-        ```
-        
-        ### For CUDA 10:
-        ```
-        conda create -n cryocare -c conda-forge -c anaconda python=3 keras-gpu=2.3.1
-        conda activate cryocare
-        pip install cryoCARE
-        ```
-        
-        ## Manual
-        cryoCARE uses `.json` configuration files and is run in three steps:
-        
-        ### 1. Prepare Training Data
-        To prepare the training data we have to provide all tomograms on which we want to train. 
-        Create an empty file called `train_data_config.json`, copy-paste the following template and fill it in.
-        ```
-        {
-          "even": [
-            "/path/to/even.rec"
-          ],
-          "odd": [
-            "/path/to/odd.rec"
-          ],
-          "patch_shape": [
-            72,
-            72,
-            72
-          ],
-          "num_slices": 1200,
-          "split": 0.9,
-          "tilt_axis": "Y",
-          "n_normalization_samples": 500,
-          "path": "./"
-        }
-        ```
-        #### Parameters:
-        * `"even"`: List of all even tomograms.
-        * `"odd"`: List of all odd tomograms. Note the order has to be the same as in `"even"`.
-        * `"patch_shape"`: Size of the sub-volumes used for training. Should not be smaller than `64, 64, 64`.
-        * `"num_slices"`: Number of sub-volumes extracted per tomograms. 
-        * `"tilt_axis"`: Tilt-axis of the tomograms. We split the tomogram along this axis to extract train- and validation data separately.
-        * `"n_normalization_samples"`: Number of sub-volumes extracted per tomograms, which are used to compute `mean` and `standard deviation` for normalization.
-        * `"path"`: The training and validation data are saved here.
-        
-        #### Run Training Data Preparation:
-        After installation of the package we have access to built in Python-scripts which we can call. 
-        To run the training data preparation we run the following command:
-        `cryoCARE_extract_train_data.py --conf train_data_config.json`
-        
-        ### 2. Training
-        Create an empty file called `train_config.json`, copy-paste the following template and fill it in.
-        ```
-        {
-          "train_data": "./",
-          "epochs": 100,
-          "steps_per_epoch": 200,
-          "batch_size": 16,
-          "unet_kern_size": 3,
-          "unet_n_depth": 3,
-          "unet_n_first": 16,
-          "learning_rate": 0.0004,
-          "model_name": "model_name",
-          "path": "./",
-          "gpu_id": 0
-        }
-        ```
-        
-        #### Parameters:
-        * `"train_data"`: Path to the directory containing the train- and validation data. This should be the same as the `"path"` from above.
-        * `"epochs"`: Number of epochs used to train the network.
-        * `"steps_per_epoch"`: Number of gradient steps performed per epoch.
-        * `"batch_size"`: Used training batch size.
-        * `"unet_kern_size"`: Convolution kernel size of the U-Net. Has to be an odd number.
-        * `"unet_n_depth"`: Depth of the U-Net.
-        * `"unet_n_first"`: Number of initial feature channels.
-        * `"learning_rate"`: Learning rate of the model training.
-        * `"model_name"`: Name of the model.
-        * `"path"`: Output path for the model.
-        * `"gpu_id"`: This is optional. Provide the GPU ID(s) of the GPUs you wish to use.
-        
-        #### Run Training:
-        To run the training we run the following command:
-        `cryoCARE_train.py --conf train_config.json`
-        
-        You will find a `.tar.gz` file in the directory you specified as `path`. This your model an will be used in the next step.
-        
-        ### 3. Prediction
-        Create an empty file called `predict_config.json`, copy-paste the following template and fill it in.
-        ```
-        {
-          "path": "path/to/your/model/model_name.tar.gz",
-          "even": "/path/to/even.rec",
-          "odd": "/path/to/odd.rec",
-          "n_tiles": [1,1,1],
-          "output": "denoised.rec",
-          "overwrite": False,
-          "gpu_id": 0
-        }
-        ```
-        
-        #### Parameters:
-        * `"path"`: Path to your model file.
-        * `"even"`: Path to directory with even tomograms or a specific even tomogram or a list of specific even tomograms.
-        * `"odd"`: Path to directory with odd tomograms or a specific odd tomogram or a list of specific odd tomograms in the same order as the even tomograms.
-        * `"n_tiles"`: Initial tiles per dimension. Gets increased if the tiles do not fit on the GPU.
-        * `"output"`: Path where the denoised tomograms will be written.
-        * `"overwrite"`: Allow previous files to be overwritten.
-        * `"gpu_id"`: This is optional. Provide the GPU ID(s) of the GPUs you wish to use.
-        
-        #### Run Prediction:
-        To run the training we run the following command:
-        `cryoCARE_predict.py --conf predict_config.json`
-        
-        ## How to Cite
-        ```
-        @inproceedings{buchholz2019cryo,
-          title={Cryo-CARE: content-aware image restoration for cryo-transmission electron microscopy data},
-          author={Buchholz, Tim-Oliver and Jordan, Mareike and Pigino, Gaia and Jug, Florian},
-          booktitle={2019 IEEE 16th International Symposium on Biomedical Imaging (ISBI 2019)},
-          pages={502--506},
-          year={2019},
-          organization={IEEE}
-        }
-        
-        @article{buchholz2019content,
-          title={Content-aware image restoration for electron microscopy.},
-          author={Buchholz, Tim-Oliver and Krull, Alexander and Shahidi, R{\'e}za and Pigino, Gaia and J{\'e}kely, G{\'a}sp{\'a}r and Jug, Florian},
-          journal={Methods in cell biology},
-          volume={152},
-          pages={277--289},
-          year={2019}
-        }
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# cryoCARE
+
+This package is a memory efficient implementation of [cryoCARE](https://github.com/juglab/cryoCARE_T2T). 
+
+This setup trains a denoising U-Net for tomographic reconstruction according to the [Noise2Noise](https://arxiv.org/pdf/1803.04189.pdf) training paradigm. 
+Therefore the user has to provide two tomograms of the same sample. 
+The simplest way to achieve this is with direct-detector movie-frames.
+
+You can use Warp to generate two reconstructed tomograms based on the even/odd frames. Alternatively, the movie-frames can be split in two halves (e.g. with MotionCor2 `-SplitSum 1` or with IMOD `alignframes -debug 10000`) from which two identical, up to random noise, tomograms can be reconstructed. 
+
+These two (even and odd) tomograms can be used as input to this cryoCARE implementation.
+
+## Changelog
+
+
+### Version 0.3
+
+* `cyroCARE_train` now supports parallelization over multiple GPUs.
+
+### Version 0.2
+
+* `cyroCARE_train` produces a compressed and more portable model. This model can be copied and shared with others without relying on a certain folder structure.
+* `cryoCARE_predict` supports to predict multiple tomograms in one run. Streamlined configuration with respect to the changes of `cryoCARE_train`.
+* Streamlined installation instructions
+* CUDA 11 support
+* Minor changes/ fixed couple of bugs:
+    * Proper padding of tomograms to avoid black frames in the denoised tomograms
+    * Fix computation of validation cut off for small tomograms
+    * Fix `cryoCARE_predict` if no tiling happens
+
+## Installation
+
+__Note:__ We assume that you have  [miniconda](https://docs.conda.io/en/latest/miniconda.html) installed.
+
+First you need to create a conda environment.
+
+### For CUDA 11:
+```
+conda create -n cryocare_11 python=3.8 cudatoolkit=11.0 cudnn=8.0 -c conda-forge
+conda activate cryocare_11
+pip install tensorflow==2.4
+pip install cryoCARE
+```
+
+### For CUDA 10:
+```
+conda create -n cryocare -c conda-forge -c anaconda python=3 keras-gpu=2.3.1
+conda activate cryocare
+pip install cryoCARE
+```
+
+## Manual
+cryoCARE uses `.json` configuration files and is run in three steps:
+
+### 1. Prepare Training Data
+To prepare the training data we have to provide all tomograms on which we want to train. 
+Create an empty file called `train_data_config.json`, copy-paste the following template and fill it in.
+```
+{
+  "even": [
+    "/path/to/even.rec"
+  ],
+  "odd": [
+    "/path/to/odd.rec"
+  ],
+  "patch_shape": [
+    72,
+    72,
+    72
+  ],
+  "num_slices": 1200,
+  "split": 0.9,
+  "tilt_axis": "Y",
+  "n_normalization_samples": 500,
+  "path": "./"
+}
+```
+#### Parameters:
+* `"even"`: List of all even tomograms.
+* `"odd"`: List of all odd tomograms. Note the order has to be the same as in `"even"`.
+* `"patch_shape"`: Size of the sub-volumes used for training. Should not be smaller than `64, 64, 64`.
+* `"num_slices"`: Number of sub-volumes extracted per tomograms. 
+* `"tilt_axis"`: Tilt-axis of the tomograms. We split the tomogram along this axis to extract train- and validation data separately.
+* `"n_normalization_samples"`: Number of sub-volumes extracted per tomograms, which are used to compute `mean` and `standard deviation` for normalization.
+* `"path"`: The training and validation data are saved here.
+
+#### Run Training Data Preparation:
+After installation of the package we have access to built in Python-scripts which we can call. 
+To run the training data preparation we run the following command:
+`cryoCARE_extract_train_data.py --conf train_data_config.json`
+
+### 2. Training
+Create an empty file called `train_config.json`, copy-paste the following template and fill it in.
+```
+{
+  "train_data": "./",
+  "epochs": 100,
+  "steps_per_epoch": 200,
+  "batch_size": 16,
+  "unet_kern_size": 3,
+  "unet_n_depth": 3,
+  "unet_n_first": 16,
+  "learning_rate": 0.0004,
+  "model_name": "model_name",
+  "path": "./",
+  "gpu_id": 0
+}
+```
+
+#### Parameters:
+* `"train_data"`: Path to the directory containing the train- and validation data. This should be the same as the `"path"` from above.
+* `"epochs"`: Number of epochs used to train the network.
+* `"steps_per_epoch"`: Number of gradient steps performed per epoch.
+* `"batch_size"`: Used training batch size.
+* `"unet_kern_size"`: Convolution kernel size of the U-Net. Has to be an odd number.
+* `"unet_n_depth"`: Depth of the U-Net.
+* `"unet_n_first"`: Number of initial feature channels.
+* `"learning_rate"`: Learning rate of the model training.
+* `"model_name"`: Name of the model.
+* `"path"`: Output path for the model.
+* `"gpu_id"`: This is optional. Provide the ID(s) of the GPUs you wish to use. Alternatively, you can specify the GPU ID(s) using the `CUDA_VISIBLE_DEVICES` environment variable. Training supports multiple GPUs (see below).
+
+#### Run Training:
+To run the training we run the following command:
+`cryoCARE_train.py --conf train_config.json`
+
+You will find a `.tar.gz` file in the directory you specified as `path`. This your model an will be used in the next step.
+
+##### Train using multiple GPUs:
+Training can be faster by running on multiple GPUs (which must be available in the same machine). Please note that the performance does not improve linearly with the number of devices used for training. The actual speedup will depend on your training settings and hardware.
+
+There are two methods for specifying multiple GPU ID(s):
+
+###### Method 1: Using `gpu_id`
+
+You can specify multiple GPU ID(s) in the `train_config.json` file as follows (with 4 GPUs in this example):
+
+`"gpu_id": [0,1,2,3]`
+
+**Note:** This method takes precedence over the `CUDA_VISIBLE_DEVICES` method below. If you want to use that method, you should **omit** the `"gpu_id"` entry from your `train_config.json` file.
+
+###### Method 2: Using the `CUDA_VISIBLE_DEVICES` environment variable
+
+For example, with 4 GPUs:
+
+````
+export CUDA_VISIBLE_DEVICES=0,1,2,3
+cryoCARE_train.py --conf train_config.json
+````
+
+**Note:** If running cryoCARE under a cluster resource manager such as SLURM, the `CUDA_VISIBLE_DEVICES` environment variable might be automatically set when you request a certain number of GPUs, so you don't need to set it explicitly. Check your cluster documentation or support team for details.
+
+### 3. Prediction
+Create an empty file called `predict_config.json`, copy-paste the following template and fill it in.
+```
+{
+  "path": "path/to/your/model/model_name.tar.gz",
+  "even": "/path/to/even.rec",
+  "odd": "/path/to/odd.rec",
+  "n_tiles": [1,1,1],
+  "output": "denoised.rec",
+  "overwrite": False,
+  "gpu_id": 0
+}
+```
+
+#### Parameters:
+* `"path"`: Path to your model file.
+* `"even"`: Path to directory with even tomograms or a specific even tomogram or a list of specific even tomograms.
+* `"odd"`: Path to directory with odd tomograms or a specific odd tomogram or a list of specific odd tomograms in the same order as the even tomograms.
+* `"n_tiles"`: Initial tiles per dimension. Gets increased if the tiles do not fit on the GPU.
+* `"output"`: Path where the denoised tomograms will be written.
+* `"overwrite"`: Allow previous files to be overwritten.
+* `"gpu_id"`: This is optional. Provide the ID of the GPU you wish to use. Alternatively, you can specify the GPU ID using the `CUDA_VISIBLE_DEVICES` environment variable. Note that prediction only supports a single GPU currently.
+
+#### Run Prediction:
+To run the training we run the following command:
+`cryoCARE_predict.py --conf predict_config.json`
+
+## How to Cite
+```
+@inproceedings{buchholz2019cryo,
+  title={Cryo-CARE: content-aware image restoration for cryo-transmission electron microscopy data},
+  author={Buchholz, Tim-Oliver and Jordan, Mareike and Pigino, Gaia and Jug, Florian},
+  booktitle={2019 IEEE 16th International Symposium on Biomedical Imaging (ISBI 2019)},
+  pages={502--506},
+  year={2019},
+  organization={IEEE}
+}
+
+@article{buchholz2019content,
+  title={Content-aware image restoration for electron microscopy.},
+  author={Buchholz, Tim-Oliver and Krull, Alexander and Shahidi, R{\'e}za and Pigino, Gaia and J{\'e}kely, G{\'a}sp{\'a}r and Jug, Florian},
+  journal={Methods in cell biology},
+  volume={152},
+  pages={277--289},
+  year={2019}
+}
+```
```

### Comparing `cryoCARE-0.2.2/cryocare/internals/CryoCARE.py` & `cryoCARE-0.3.0/cryocare/internals/CryoCARE.py`

 * *Files identical despite different names*

### Comparing `cryoCARE-0.2.2/cryocare/internals/CryoCAREDataModule.py` & `cryoCARE-0.3.0/cryocare/internals/CryoCAREDataModule.py`

 * *Files identical despite different names*

### Comparing `cryoCARE-0.2.2/cryocare/scripts/cryoCARE_extract_train_data.py` & `cryoCARE-0.3.0/cryocare/scripts/cryoCARE_extract_train_data.py`

 * *Files identical despite different names*

### Comparing `cryoCARE-0.2.2/cryocare/scripts/cryoCARE_predict.py` & `cryoCARE-0.3.0/cryocare/scripts/cryoCARE_predict.py`

 * *Files identical despite different names*

### Comparing `cryoCARE-0.2.2/cryocare/scripts/cryoCARE_train.py` & `cryoCARE-0.3.0/cryocare/scripts/cryoCARE_train.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json
 from cryocare.internals.CryoCARE import CryoCARE
 from csbdeep.models import Config
 import pickle
 from os.path import join
 from cryocare.internals.CryoCAREDataModule import CryoCARE_DataModule
 from cryocare.scripts.cryoCARE_predict import set_gpu_id
+import tensorflow as tf
 
 def main():
     parser = argparse.ArgumentParser(description='Load training config.')
     parser.add_argument('--conf')
 
     args = parser.parse_args()
     with open(args.conf, 'r') as f:
@@ -29,18 +30,23 @@
         train_batch_size=config['batch_size'],
         unet_kern_size=config['unet_kern_size'],
         unet_n_depth=config['unet_n_depth'],
         unet_n_first=config['unet_n_first'],
         train_tensorboard=False,
         train_learning_rate=config['learning_rate']
     )
+    
+    mirrored_strategy = tf.distribute.MirroredStrategy()
+
+    with mirrored_strategy.scope():
 
-    model = CryoCARE(net_conf, config['model_name'], basedir=config['path'])
+        model = CryoCARE(net_conf, config['model_name'], basedir=config['path'])
 
-    history = model.train(dm.get_train_dataset(), dm.get_val_dataset())
+        history = model.train(dm.get_train_dataset(), dm.get_val_dataset())
+        
     mean, std = dm.train_dataset.mean, dm.train_dataset.std
 
     with open(join(config['path'], config['model_name'], 'history.dat'), 'wb+') as f:
         pickle.dump(history.history, f)
 
 
     # Write norm to disk
```

### Comparing `cryoCARE-0.2.2/setup.py` & `cryoCARE-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cryoCARE",
-    version="0.2.2",
+    version="0.3.0",
     author="Tim-Oliver Buchholz, Thorsten Wagner",
     author_email="tim-oliver.buchholz@fmi.ch, "
                  "thorsten.wagner@mpi-dortmund.mpg.de",
     description="cryoCARE is a deep learning approach for cryo-TEM tomogram denoising.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/juglab/cryoCARE_pip",
@@ -19,15 +19,15 @@
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering",
         "License :: OSI Approved :: BSD License"
     ],
     python_requires='>=3.8',
     install_requires=[
-        "numpy",
+        "numpy~=1.19.2",
         "mrcfile",
         "csbdeep>=0.7.0,<0.8.0",
         "psutil"
     ],
     scripts=[
         'cryocare/scripts/cryoCARE_extract_train_data.py',
         'cryocare/scripts/cryoCARE_train.py',
```

