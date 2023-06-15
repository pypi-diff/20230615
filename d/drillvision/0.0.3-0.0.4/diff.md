# Comparing `tmp/drillvision-0.0.3.tar.gz` & `tmp/drillvision-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drillvision-0.0.3.tar", last modified: Thu Jun  1 21:28:04 2023, max compression
+gzip compressed data, was "dist/drillvision-0.0.4.tar", last modified: Thu Jun 15 05:41:08 2023, max compression
```

## Comparing `drillvision-0.0.3.tar` & `drillvision-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-06-01 21:28:04.109699 drillvision-0.0.3/
--rw-r--r--   0 amin       (501) staff       (20)      305 2023-05-21 20:38:44.000000 drillvision-0.0.3/MANIFEST.in
--rw-r--r--   0 amin       (501) staff       (20)     8260 2023-06-01 21:28:04.109397 drillvision-0.0.3/PKG-INFO
--rw-r--r--   0 amin       (501) staff       (20)     7638 2023-06-01 21:22:00.000000 drillvision-0.0.3/README.md
-drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-06-01 21:28:04.107316 drillvision-0.0.3/drillvision.egg-info/
--rw-r--r--   0 amin       (501) staff       (20)     8260 2023-06-01 21:28:03.000000 drillvision-0.0.3/drillvision.egg-info/PKG-INFO
--rw-r--r--   0 amin       (501) staff       (20)      747 2023-06-01 21:28:03.000000 drillvision-0.0.3/drillvision.egg-info/SOURCES.txt
--rw-r--r--   0 amin       (501) staff       (20)        1 2023-06-01 21:28:03.000000 drillvision-0.0.3/drillvision.egg-info/dependency_links.txt
--rw-r--r--   0 amin       (501) staff       (20)      248 2023-06-01 21:28:03.000000 drillvision-0.0.3/drillvision.egg-info/requires.txt
--rw-r--r--   0 amin       (501) staff       (20)       21 2023-06-01 21:28:03.000000 drillvision-0.0.3/drillvision.egg-info/top_level.txt
-drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-06-01 21:28:04.105081 drillvision-0.0.3/neural_network_model/
--rw-r--r--   0 amin       (501) staff       (20)        5 2023-06-01 21:24:02.000000 drillvision-0.0.3/neural_network_model/VERSION
--rw-r--r--   0 amin       (501) staff       (20)        0 2023-05-16 02:02:49.000000 drillvision-0.0.3/neural_network_model/__init__.py
--rw-r--r--   0 amin       (501) staff       (20)    22291 2023-06-01 20:54:29.000000 drillvision-0.0.3/neural_network_model/bit_vision.py
--rw-r--r--   0 amin       (501) staff       (20)     5962 2023-05-29 03:59:31.000000 drillvision-0.0.3/neural_network_model/model.py
--rw-r--r--   0 amin       (501) staff       (20)    14713 2023-05-25 23:15:08.000000 drillvision-0.0.3/neural_network_model/process_data.py
--rw-r--r--   0 amin       (501) staff       (20)     2843 2023-05-20 18:27:45.000000 drillvision-0.0.3/neural_network_model/s3.py
--rw-r--r--   0 amin       (501) staff       (20)     1913 2023-05-21 20:09:15.000000 drillvision-0.0.3/pyproject.toml
--rw-r--r--   0 amin       (501) staff       (20)       97 2023-05-13 20:20:47.000000 drillvision-0.0.3/requirements-test.txt
--rw-r--r--   0 amin       (501) staff       (20)      248 2023-05-31 01:33:26.000000 drillvision-0.0.3/requirements.txt
--rw-r--r--   0 amin       (501) staff       (20)       38 2023-06-01 21:28:04.109812 drillvision-0.0.3/setup.cfg
--rw-r--r--   0 amin       (501) staff       (20)     2128 2023-05-29 03:58:58.000000 drillvision-0.0.3/setup.py
-drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-06-01 21:28:04.108722 drillvision-0.0.3/tests/
--rw-r--r--   0 amin       (501) staff       (20)      346 2023-05-20 18:27:45.000000 drillvision-0.0.3/tests/test_bitvision.py
--rw-r--r--   0 amin       (501) staff       (20)     3023 2023-05-20 18:27:45.000000 drillvision-0.0.3/tests/test_preprocessing.py
+drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-06-15 05:41:08.700652 drillvision-0.0.4/
+-rw-r--r--   0 amin       (501) staff       (20)      305 2023-05-21 20:38:44.000000 drillvision-0.0.4/MANIFEST.in
+-rw-r--r--   0 amin       (501) staff       (20)     8511 2023-06-15 05:41:08.700195 drillvision-0.0.4/PKG-INFO
+-rw-r--r--   0 amin       (501) staff       (20)     8080 2023-06-13 00:15:55.000000 drillvision-0.0.4/README.md
+drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-06-15 05:41:08.696889 drillvision-0.0.4/drillvision.egg-info/
+-rw-r--r--   0 amin       (501) staff       (20)     8511 2023-06-15 05:41:08.000000 drillvision-0.0.4/drillvision.egg-info/PKG-INFO
+-rw-r--r--   0 amin       (501) staff       (20)      747 2023-06-15 05:41:08.000000 drillvision-0.0.4/drillvision.egg-info/SOURCES.txt
+-rw-r--r--   0 amin       (501) staff       (20)        1 2023-06-15 05:41:08.000000 drillvision-0.0.4/drillvision.egg-info/dependency_links.txt
+-rw-r--r--   0 amin       (501) staff       (20)      248 2023-06-15 05:41:08.000000 drillvision-0.0.4/drillvision.egg-info/requires.txt
+-rw-r--r--   0 amin       (501) staff       (20)       21 2023-06-15 05:41:08.000000 drillvision-0.0.4/drillvision.egg-info/top_level.txt
+drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-06-15 05:41:08.693288 drillvision-0.0.4/neural_network_model/
+-rw-r--r--   0 amin       (501) staff       (20)        5 2023-06-15 05:40:18.000000 drillvision-0.0.4/neural_network_model/VERSION
+-rw-r--r--   0 amin       (501) staff       (20)        0 2023-05-16 02:02:49.000000 drillvision-0.0.4/neural_network_model/__init__.py
+-rw-r--r--   0 amin       (501) staff       (20)    25121 2023-06-15 04:38:31.000000 drillvision-0.0.4/neural_network_model/bit_vision.py
+-rw-r--r--   0 amin       (501) staff       (20)     5926 2023-06-11 16:44:26.000000 drillvision-0.0.4/neural_network_model/model.py
+-rw-r--r--   0 amin       (501) staff       (20)    14882 2023-06-15 04:53:05.000000 drillvision-0.0.4/neural_network_model/process_data.py
+-rw-r--r--   0 amin       (501) staff       (20)     2843 2023-05-20 18:27:45.000000 drillvision-0.0.4/neural_network_model/s3.py
+-rw-r--r--   0 amin       (501) staff       (20)     1913 2023-05-21 20:09:15.000000 drillvision-0.0.4/pyproject.toml
+-rw-r--r--   0 amin       (501) staff       (20)      108 2023-06-12 16:36:38.000000 drillvision-0.0.4/requirements-test.txt
+-rw-r--r--   0 amin       (501) staff       (20)      248 2023-05-31 01:33:26.000000 drillvision-0.0.4/requirements.txt
+-rw-r--r--   0 amin       (501) staff       (20)       38 2023-06-15 05:41:08.700798 drillvision-0.0.4/setup.cfg
+-rw-r--r--   0 amin       (501) staff       (20)     2134 2023-06-15 05:14:07.000000 drillvision-0.0.4/setup.py
+drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-06-15 05:41:08.698942 drillvision-0.0.4/tests/
+-rw-r--r--   0 amin       (501) staff       (20)      399 2023-06-15 04:02:43.000000 drillvision-0.0.4/tests/test_bitvision.py
+-rw-r--r--   0 amin       (501) staff       (20)     5873 2023-06-15 04:05:57.000000 drillvision-0.0.4/tests/test_preprocessing.py
```

### Comparing `drillvision-0.0.3/PKG-INFO` & `drillvision-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: drillvision
-Version: 0.0.3
+Version: 0.0.4
 Summary: # Drill Bit Classifier
 Home-page: https://github.com/Atashnezhad/DrillBitVision
 Author: Amin Atashnezhad
 Author-email: atashnezhad2@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 # Drill Bit Classifier
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-360/)
 [![PyPI version](https://badge.fury.io/py/drillvision.svg)](https://badge.fury.io/py/drillvision)
+[![Github All Releases](https://img.shields.io/github/downloads/Atashnezhad/DrillBitVision/total.svg)]()
+[![CircleCI](https://circleci.com/gh/Atashnezhad/DrillBitVision.svg?style=svg)](https://github.com/Atashnezhad/DrillBitVision)
+
+
 
 The Drill Bit Classifier is an app that uses a Convolutional Neural Network (CNN) to 
 classify images of drill bits. The app can be used by machinists and engineers to 
 quickly and accurately identify the type of drill bit required for a particular job.
 
 ## Description:
 ### Preprocessing Module
@@ -98,45 +99,53 @@
 ```
 ## Usage
 ```python
 from pathlib import Path
 from neural_network_model.process_data import Preprocessing
 from neural_network_model.bit_vision import BitVision
 
+
 if __name__ == "__main__":
     # download the images
     obj = Preprocessing(dataset_address=Path(__file__).parent / "dataset")
-    obj.download_images()
+    obj.download_images(limit=25)
     print(obj.image_dict)
     obj.augment_data(
-        number_of_images_tobe_gen=10,
+        number_of_images_tobe_gen=100,
         augment_data_address=Path(__file__).parent / "augmented_dataset"
     )
     obj.train_test_split(
         augmented_data_address=Path(__file__).parent / "augmented_dataset",
         train_test_val_split_dir_address=Path(__file__).parent / "dataset_train_test_val"
     )
 
     obj = BitVision(train_test_val_dir=Path(__file__).parent / "dataset_train_test_val")
     print(obj.categories)
     print(obj.data_details)
     obj.plot_image_category()
     obj.compile_model()
-    model_name = "model_test_1.h5"
-    obj.train_model(model_save_address=Path(__file__).parent / "deep_model" / model_name)
+
+    model_name = "model_epoch_{epoch:02d}_loss_{loss:.2f}_acc_{accuracy:.2f}_val_acc_{val_accuracy:.2f}_.h5"
+    obj.train_model(
+        model_save_address=Path(__file__).parent / "deep_model",
+        model_name=model_name,
+        epochs=40,
+    )
     obj.plot_history(fig_folder_address=Path(__file__).parent / "figures")
 
     obj.predict(
         fig_save_address=Path(__file__).parent / "figures",
         model_path=Path(__file__).parent / "deep_model" / model_name,
         test_folder_address=Path(__file__).parent / "dataset_train_test_val" / "test"
     )
 
     # find list of images in the Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit"
     directory_path = Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit"
     list_of_images = [str(x) for x in directory_path.glob("*.jpeg")]
     obj.grad_cam_viz(
+        model_path=Path(__file__).parent / "deep_model" / model_name,
         fig_to_save_address=Path(__file__).parent / "figures",
         img_to_be_applied_path=Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit" / list_of_images[0],
         output_gradcam_fig_name="gradcam.png"
     )
 
+
```

### Comparing `drillvision-0.0.3/README.md` & `drillvision-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Drill Bit Classifier
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-360/)
 [![PyPI version](https://badge.fury.io/py/drillvision.svg)](https://badge.fury.io/py/drillvision)
+[![Github All Releases](https://img.shields.io/github/downloads/Atashnezhad/DrillBitVision/total.svg)]()
+[![CircleCI](https://circleci.com/gh/Atashnezhad/DrillBitVision.svg?style=svg)](https://github.com/Atashnezhad/DrillBitVision)
+
+
 
 The Drill Bit Classifier is an app that uses a Convolutional Neural Network (CNN) to 
 classify images of drill bits. The app can be used by machinists and engineers to 
 quickly and accurately identify the type of drill bit required for a particular job.
 
 ## Description:
 ### Preprocessing Module
@@ -81,45 +85,53 @@
 ```
 ## Usage
 ```python
 from pathlib import Path
 from neural_network_model.process_data import Preprocessing
 from neural_network_model.bit_vision import BitVision
 
+
 if __name__ == "__main__":
     # download the images
     obj = Preprocessing(dataset_address=Path(__file__).parent / "dataset")
-    obj.download_images()
+    obj.download_images(limit=25)
     print(obj.image_dict)
     obj.augment_data(
-        number_of_images_tobe_gen=10,
+        number_of_images_tobe_gen=100,
         augment_data_address=Path(__file__).parent / "augmented_dataset"
     )
     obj.train_test_split(
         augmented_data_address=Path(__file__).parent / "augmented_dataset",
         train_test_val_split_dir_address=Path(__file__).parent / "dataset_train_test_val"
     )
 
     obj = BitVision(train_test_val_dir=Path(__file__).parent / "dataset_train_test_val")
     print(obj.categories)
     print(obj.data_details)
     obj.plot_image_category()
     obj.compile_model()
-    model_name = "model_test_1.h5"
-    obj.train_model(model_save_address=Path(__file__).parent / "deep_model" / model_name)
+
+    model_name = "model_epoch_{epoch:02d}_loss_{loss:.2f}_acc_{accuracy:.2f}_val_acc_{val_accuracy:.2f}_.h5"
+    obj.train_model(
+        model_save_address=Path(__file__).parent / "deep_model",
+        model_name=model_name,
+        epochs=40,
+    )
     obj.plot_history(fig_folder_address=Path(__file__).parent / "figures")
 
     obj.predict(
         fig_save_address=Path(__file__).parent / "figures",
         model_path=Path(__file__).parent / "deep_model" / model_name,
         test_folder_address=Path(__file__).parent / "dataset_train_test_val" / "test"
     )
 
     # find list of images in the Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit"
     directory_path = Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit"
     list_of_images = [str(x) for x in directory_path.glob("*.jpeg")]
     obj.grad_cam_viz(
+        model_path=Path(__file__).parent / "deep_model" / model_name,
         fig_to_save_address=Path(__file__).parent / "figures",
         img_to_be_applied_path=Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit" / list_of_images[0],
         output_gradcam_fig_name="gradcam.png"
     )
 
+
```

### Comparing `drillvision-0.0.3/drillvision.egg-info/PKG-INFO` & `drillvision-0.0.4/drillvision.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: drillvision
-Version: 0.0.3
+Version: 0.0.4
 Summary: # Drill Bit Classifier
 Home-page: https://github.com/Atashnezhad/DrillBitVision
 Author: Amin Atashnezhad
 Author-email: atashnezhad2@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 # Drill Bit Classifier
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-360/)
 [![PyPI version](https://badge.fury.io/py/drillvision.svg)](https://badge.fury.io/py/drillvision)
+[![Github All Releases](https://img.shields.io/github/downloads/Atashnezhad/DrillBitVision/total.svg)]()
+[![CircleCI](https://circleci.com/gh/Atashnezhad/DrillBitVision.svg?style=svg)](https://github.com/Atashnezhad/DrillBitVision)
+
+
 
 The Drill Bit Classifier is an app that uses a Convolutional Neural Network (CNN) to 
 classify images of drill bits. The app can be used by machinists and engineers to 
 quickly and accurately identify the type of drill bit required for a particular job.
 
 ## Description:
 ### Preprocessing Module
@@ -98,45 +99,53 @@
 ```
 ## Usage
 ```python
 from pathlib import Path
 from neural_network_model.process_data import Preprocessing
 from neural_network_model.bit_vision import BitVision
 
+
 if __name__ == "__main__":
     # download the images
     obj = Preprocessing(dataset_address=Path(__file__).parent / "dataset")
-    obj.download_images()
+    obj.download_images(limit=25)
     print(obj.image_dict)
     obj.augment_data(
-        number_of_images_tobe_gen=10,
+        number_of_images_tobe_gen=100,
         augment_data_address=Path(__file__).parent / "augmented_dataset"
     )
     obj.train_test_split(
         augmented_data_address=Path(__file__).parent / "augmented_dataset",
         train_test_val_split_dir_address=Path(__file__).parent / "dataset_train_test_val"
     )
 
     obj = BitVision(train_test_val_dir=Path(__file__).parent / "dataset_train_test_val")
     print(obj.categories)
     print(obj.data_details)
     obj.plot_image_category()
     obj.compile_model()
-    model_name = "model_test_1.h5"
-    obj.train_model(model_save_address=Path(__file__).parent / "deep_model" / model_name)
+
+    model_name = "model_epoch_{epoch:02d}_loss_{loss:.2f}_acc_{accuracy:.2f}_val_acc_{val_accuracy:.2f}_.h5"
+    obj.train_model(
+        model_save_address=Path(__file__).parent / "deep_model",
+        model_name=model_name,
+        epochs=40,
+    )
     obj.plot_history(fig_folder_address=Path(__file__).parent / "figures")
 
     obj.predict(
         fig_save_address=Path(__file__).parent / "figures",
         model_path=Path(__file__).parent / "deep_model" / model_name,
         test_folder_address=Path(__file__).parent / "dataset_train_test_val" / "test"
     )
 
     # find list of images in the Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit"
     directory_path = Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit"
     list_of_images = [str(x) for x in directory_path.glob("*.jpeg")]
     obj.grad_cam_viz(
+        model_path=Path(__file__).parent / "deep_model" / model_name,
         fig_to_save_address=Path(__file__).parent / "figures",
         img_to_be_applied_path=Path(__file__).parent / "dataset_train_test_val" / "test" / "pdc_bit" / list_of_images[0],
         output_gradcam_fig_name="gradcam.png"
     )
 
+
```

### Comparing `drillvision-0.0.3/drillvision.egg-info/SOURCES.txt` & `drillvision-0.0.4/drillvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.3/neural_network_model/bit_vision.py` & `drillvision-0.0.4/neural_network_model/bit_vision.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,51 @@
 import logging
-import random
-
-from keras import Sequential
-from keras.layers import (
-    BatchNormalization,
-    Conv2D,
-    Dense,
-    Dropout,
-    Flatten,
-    MaxPooling2D,
-)
-
-from neural_network_model.model import SETTING
-
-# set seed to get the same random numbers each time
-random.seed(1)
-
+import math
 import os
+import random
 import warnings
 from pathlib import Path
 from typing import Dict, List
 
-# from tensorflow.keras.callbacks import ModelCheckpoint
-from keras.callbacks import ModelCheckpoint
-from tensorflow.keras.applications.resnet50 import decode_predictions, preprocess_input
-
-warnings.filterwarnings("ignore")
-
 import numpy as np
 import tensorflow
-from tensorflow import keras
-
-warnings.filterwarnings("ignore")
-
 import matplotlib.cm as cm
 import matplotlib.pyplot as plt
 import tensorflow as tf
-
-# Display
 from tensorflow import keras
+from tensorflow.keras.applications.resnet50 import decode_predictions, preprocess_input
 from tensorflow.keras.preprocessing import image
-from tensorflow.keras.preprocessing.image import (
-    ImageDataGenerator,
-    img_to_array,
-    load_img,
-)
+from tensorflow.keras.preprocessing.image import ImageDataGenerator, img_to_array, load_img
+from keras import Sequential
+from keras.callbacks import ModelCheckpoint
+from keras.layers import BatchNormalization, Conv2D, Dense, Dropout, Flatten, MaxPooling2D
+
+from neural_network_model.model import SETTING
+
+# Set seed to get the same random numbers each time
+random.seed(1)
 
 # Initialize the logger
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
+
 # Create console handler
 ch = logging.StreamHandler()
 ch.setLevel(logging.INFO)
 
 # Create formatter and add it to the handler
 formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
 ch.setFormatter(formatter)
 
 # Add the handler to the logger
 logger.addHandler(ch)
 
+# Ignore all warnings
+warnings.filterwarnings("ignore")
+
 
 class BitVision:
     """
     This class is used to train a neural network model for bit vision.
     """
 
     def __init__(self, *args, **kwargs):
@@ -186,15 +168,15 @@
             category_path = self.train_test_val_dir / subdir / category
             image_path = category_path / os.listdir(category_path)[1]
             img = load_img(image_path)
             axs[self.categories.index(category)].imshow(img)
             axs[self.categories.index(category)].set_title(category)
         plt.show()
 
-    def _rescaling(self):
+    def _rescaling(self) -> None:
         """
         This function is used to rescale the images.
         The images were augmented before in the preprocessing step.
         Here we just rescale them.
         """
         my_list = ["train", "val"]
         for subdir in my_list:
@@ -221,58 +203,97 @@
             self.train_val_gens[subdir] = generator
             self.model_class_indices = dict(
                 zip(generator.class_indices.values(), generator.class_indices.keys())
             )
 
             logger.info(f"Rescaling {subdir} data, {generator.class_indices}:")
 
-    def _check_points(self) -> ModelCheckpoint:
+    def _check_points(
+        self, model_save_address: str, model_name: str
+    ) -> ModelCheckpoint:
         check_point = ModelCheckpoint(
-            SETTING.MODEL_SETTING.MODEL_PATH,
+            model_save_address / model_name,
             monitor=SETTING.MODEL_SETTING.MONITOR,
             verbose=SETTING.MODEL_SETTING.CHECK_POINT_VERBOSE,
             save_best_only=SETTING.MODEL_SETTING.SAVE_BEST_ONLY,
             mode=SETTING.MODEL_SETTING.MODE,
-            # period=SETTING.MODEL_SETTING.PERIOD,
+            period=SETTING.MODEL_SETTING.PERIOD,
         )
         return check_point
 
-    def train_model(self, model_save_address: str = None):
+    def _calculate_number_from_dict(self, my_dict: dict) -> int:
+        total = sum(my_dict.values())
+        return total
+
+    def train_model(
+        self, model_save_address: str = SETTING.MODEL_SETTING.MODEL_PATH, **kwargs
+    ) -> None:
+        """
+        This function is used to train the model.
+        :param model_save_address:
+        :param kwargs: model_name, epochs, verbose, class_weight, workers, use_multiprocessing, shuffle
+        :return:
+        """
+
+        model_name = kwargs.get("model_name", SETTING.MODEL_SETTING.MODEL_NAME)
+        epochs = kwargs.get("epochs", SETTING.MODEL_SETTING.EPOCHS)
+        verbose = kwargs.get("verbose", SETTING.MODEL_SETTING.FIT_GEN_VERBOSE)
+        class_weight = kwargs.get("class_weight", SETTING.MODEL_SETTING.CLASS_WEIGHT)
+        workers = kwargs.get("workers", SETTING.MODEL_SETTING.WORKERS)
+        use_multiprocessing = kwargs.get(
+            "use_multiprocessing", SETTING.MODEL_SETTING.USE_MULTIPROCESSING
+        )
+        shuffle = kwargs.get("shuffle", SETTING.MODEL_SETTING.SHUFFLE)
+
+        # calculate validation_steps
+        BATCH_SIZE = SETTING.FLOW_FROM_DIRECTORY_SETTING.BATCH_SIZE
+        TRAINING_SIZE = self._calculate_number_from_dict(self.data_details["train"])
+        VALIDATION_SIZE = self._calculate_number_from_dict(self.data_details["val"])
+        # We take the ceiling because we do not drop the remainder of the batch
+        compute_steps_per_epoch = lambda x: int(math.ceil(1.0 * x / BATCH_SIZE))
+        steps_per_epoch = compute_steps_per_epoch(TRAINING_SIZE)
+        val_steps = compute_steps_per_epoch(VALIDATION_SIZE)
+
         self._rescaling()
-        model_history = self.model.fit_generator(
+        self.model_history = self.model.fit_generator(
+            steps_per_epoch=steps_per_epoch,
             generator=self.train_val_gens["train"],
-            epochs=SETTING.MODEL_SETTING.EPOCHS,
-            verbose=SETTING.MODEL_SETTING.FIT_GEN_VERBOSE,
+            epochs=epochs or SETTING.MODEL_SETTING.EPOCHS,
+            verbose=verbose or SETTING.MODEL_SETTING.FIT_GEN_VERBOSE,
             validation_data=self.train_val_gens["val"],
-            validation_steps=SETTING.MODEL_SETTING.VALIDATION_STEPS,
-            class_weight=SETTING.MODEL_SETTING.CLASS_WEIGHT,
+            validation_steps=val_steps or SETTING.MODEL_SETTING.VALIDATION_STEPS,
+            class_weight=class_weight or SETTING.MODEL_SETTING.CLASS_WEIGHT,
             max_queue_size=SETTING.MODEL_SETTING.MAX_QUEUE_SIZE,
-            workers=SETTING.MODEL_SETTING.WORKERS,
-            use_multiprocessing=SETTING.MODEL_SETTING.USE_MULTIPROCESSING,
-            shuffle=SETTING.MODEL_SETTING.SHUFFLE,
+            workers=workers or SETTING.MODEL_SETTING.WORKERS,
+            use_multiprocessing=use_multiprocessing
+            or SETTING.MODEL_SETTING.USE_MULTIPROCESSING,
+            shuffle=shuffle or SETTING.MODEL_SETTING.SHUFFLE,
             initial_epoch=SETTING.MODEL_SETTING.INITIAL_EPOCH,
-            callbacks=[self._check_points()],
+            callbacks=[self._check_points(model_save_address, model_name)],
         )
 
-        self.model.save(model_save_address or SETTING.MODEL_SETTING.MODEL_PATH)
+        self.model.save(
+            model_save_address / model_name
+            or SETTING.MODEL_SETTING.MODEL_PATH / SETTING.MODEL_SETTING.MODEL_NAME
+        )
         logger.info(f"Model saved to {SETTING.MODEL_SETTING.MODEL_PATH}")
-        self.model_history = model_history
 
     def plot_history(self, *args, **kwargs):
         """
         This function is used to plot the history of the model.
         :param fig_folder_address: the address of the folder to save the figure
         :return:
         """
         fig_folder_address = kwargs.get(
             "fig_folder_address", SETTING.FIGURE_SETTING.FIG_PRED_OUT_DIR_ADDRESS
         )
         # if the folder does not exist, create it
-        if not os.path.exists(fig_folder_address):
-            os.makedirs(fig_folder_address)
+        if not os.path.exists(fig_folder_address.resolve()):
+            os.makedirs(fig_folder_address.resolve())
+
         logger.info(self.model_history.history.keys())
         keys_plot = ["loss", "accuracy"]
         # make two plots side by side and have train and val for loss and accuracy
         fig, axs = plt.subplots(
             SETTING.FIGURE_SETTING.NUM_ROWS_IN_PLOT_HIST,
             SETTING.FIGURE_SETTING.NUM_COLS_IN_PLOT_HIST,
             figsize=SETTING.FIGURE_SETTING.FIGURE_SIZE_IN_PLOT_HIST,
@@ -306,21 +327,26 @@
         model_path: the path of the model to be used for prediction
         :return:
         """
         fig_save_address = kwargs.get(
             "fig_save_address", SETTING.FIGURE_SETTING.FIG_PRED_OUT_DIR_ADDRESS
         )
         # if the folder does not exist, create it
-        if not os.path.exists(fig_save_address):
-            os.makedirs(fig_save_address)
-        model_path = kwargs.get("model_path", SETTING.MODEL_SETTING.MODEL_PATH)
+        if not os.path.exists(fig_save_address.resolve()):
+            os.makedirs(fig_save_address.resolve())
+        model_path = kwargs.get(
+            "model_path",
+            SETTING.MODEL_SETTING.MODEL_PATH / SETTING.MODEL_SETTING.MODEL_NAME,
+        )
         if model_path is None:
-            raise ValueError("model_path is None")
+            logger.info(f"model_path from SETTING is was used - {model_path}")
 
-        test_folder_address = kwargs.get("test_folder_address", SETTING.DATA_ADDRESS_SETTING.TEST_DIR_ADDRESS)
+        test_folder_address = kwargs.get(
+            "test_folder_address", SETTING.DATA_ADDRESS_SETTING.TEST_DIR_ADDRESS
+        )
         if test_folder_address is None:
             raise ValueError("test_folder_address is None")
 
         model = keras.models.load_model(model_path)
         logger.info(f"Model loaded from {model_path}")
 
         for category in self.categories:
@@ -404,23 +430,28 @@
             interpolation="nearest",
         )
 
         model.evaluate(DoubleCheck_generator)
 
     # TODO: check the addresses and add as kwargs if needed
     def grad_cam_viz(self, *args, **kwargs):
-        model_path = kwargs.get("model_path", SETTING.MODEL_SETTING.MODEL_PATH)
+        model_path = kwargs.get(
+            "model_path",
+            SETTING.MODEL_SETTING.MODEL_PATH / SETTING.MODEL_SETTING.MODEL_NAME,
+        )
         fig_to_save_address = kwargs.get(
             "fig_to_save_address", SETTING.GRAD_CAM_SETTING.IMAGE_NEW_NAME
         )
         gradcam_fig_name = kwargs.get(
             "output_gradcam_fig_name", SETTING.GRAD_CAM_SETTING.GRAD_CAM_FIG_NAME
         )
 
-        img_to_be_applied_path = kwargs.get("img_to_be_applied_path", SETTING.GRAD_CAM_SETTING.IMG_PATH)
+        img_to_be_applied_path = kwargs.get(
+            "img_to_be_applied_path", SETTING.GRAD_CAM_SETTING.IMG_PATH
+        )
 
         fig_address = fig_to_save_address / gradcam_fig_name
         if model_path is None:
             raise ValueError("model_path is None")
 
         model = keras.models.load_model(model_path)
         logger.info(f"Model loaded from {model_path}")
@@ -525,15 +556,15 @@
         img = keras.preprocessing.image.load_img(img_path)
         img = keras.preprocessing.image.img_to_array(img)
 
         # Rescale heatmap to a range 0-255
         heatmap = np.uint8((1 / SETTING.DATA_GEN_SETTING.RESCALE) * heatmap)
 
         # Use jet colormap to colorize heatmap
-        jet = cm.get_cmap("jet")
+        jet = cm.get_cmap("plasma")
 
         # Use RGB values of the colormap
         jet_colors = jet(np.arange(256))[:, :3]
         jet_heatmap = jet_colors[heatmap]
 
         # Create an image with RGB colorized heatmap
         jet_heatmap = keras.preprocessing.image.array_to_img(jet_heatmap)
@@ -543,14 +574,43 @@
         # Superimpose the heatmap on original image
         superimposed_img = jet_heatmap * alpha + img
         superimposed_img = keras.preprocessing.image.array_to_img(superimposed_img)
 
         # Save the superimposed image
         superimposed_img.save(cam_path)
 
+    @staticmethod
+    def return_best_model_name(
+        directory: str = SETTING.MODEL_SETTING.MODEL_PATH,
+    ) -> str:
+        """
+        Return the best model name
+        :param directory:
+        :return:
+        """
+
+        best_model = None
+        best_val_acc = 0.0
+
+        for filename in os.listdir(directory):
+            if (
+                filename.endswith(".h5")
+                and "val_acc" in filename
+                and not "val_accuracy" in filename
+            ):
+                # Extract the validation accuracy from the filename
+                print(filename.split("_val_acc_")[1].split("_.h5")[0])
+                val_acc = float(filename.split("_val_acc_")[1].split("_.h5")[0])
+
+                if val_acc > best_val_acc:
+                    best_val_acc = val_acc
+                    best_model = filename
+
+        return best_model
+
 
 if __name__ == "__main__":
     obj = BitVision(
         train_test_val_dir=Path(__file__).parent / ".." / "dataset_train_test_val"
     )
     print(obj.categories)
     print(obj.data_details)
```

### Comparing `drillvision-0.0.3/neural_network_model/model.py` & `drillvision-0.0.4/neural_network_model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,29 +61,26 @@
     TRAIN_TEST_SPLIT_DIR_NAMES: list = ["train", "test", "val"]
     TRAIN_FRACTION: float = 0.7
     TEST_FRACTION: float = 0.2
     VAL_FRACTION: float = 0.1
 
 
 class ModelSetting(BaseModel):
-    MODEL_PATH: str = (
-        Path(__file__).parent
-        / ".."
-        / "deep_model"
-        / "model_epoch_27_loss_0.52_acc_0.64_val_acc_0.62_.h5"
-    )
+    MODEL_PATH: str = (Path(__file__).parent / ".." / "deep_model").resolve()
+
+    MODEL_NAME: str = "model_.h5"
 
     # compile
     LOSS: str = "categorical_crossentropy"
     METRICS: List = ["accuracy"]
 
     # fit generator
-    EPOCHS: int = 5
+    EPOCHS: int = 3
     FIT_GEN_VERBOSE: int = 1
-    VALIDATION_STEPS: int = 2
+    VALIDATION_STEPS: int = 4
     CLASS_WEIGHT: dict = None
     MAX_QUEUE_SIZE: int = 10
     WORKERS: int = 1
     SHUFFLE: bool = True
     INITIAL_EPOCH: int = 1
     USE_MULTIPROCESSING: bool = False
 
@@ -98,15 +95,15 @@
 
 
 class FigureSetting(BaseModel):
     # in the predict method of BitVision class
     FIGURE_SIZE_IN_PRED_MODEL: tuple = (20, 15)
     NUM_ROWS_IN_PRED_MODEL: int = 5
     NUM_COLS_IN_PRED_MODEL: int = 7
-    FIG_PRED_OUT_DIR_ADDRESS: str = Path(__file__) / ".." / ".." / "figures"
+    FIG_PRED_OUT_DIR_ADDRESS: str = (Path(__file__) / ".." / ".." / "figures").resolve()
 
     # in the plot_history method of BitVision class
     FIGURE_SIZE_IN_PLOT_HIST: tuple = (17, 10)
     NUM_ROWS_IN_PLOT_HIST: int = 1
     NUM_COLS_IN_PLOT_HIST: int = 2
```

### Comparing `drillvision-0.0.3/neural_network_model/process_data.py` & `drillvision-0.0.4/neural_network_model/process_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,51 +1,45 @@
 import logging
 import os
 import random
 import shutil
+from pathlib import Path
+from typing import Any, Dict, List
+import warnings
 
 from bing_image_downloader import downloader
 from tensorflow.keras.preprocessing import image
-from tensorflow.keras.preprocessing.image import (
-    ImageDataGenerator,
-    img_to_array,
-    load_img,
-)
+from tensorflow.keras.preprocessing.image import ImageDataGenerator, img_to_array, load_img
+from tqdm import tqdm
 
 from neural_network_model.model import SETTING
 from neural_network_model.s3 import MyS3
 
-# set seed to get the same random numbers each time
+# Set seed to get the same random numbers each time
 random.seed(SETTING.RANDOM_SEED_SETTING.SEED)
-import random
-
-# import sys
-import warnings
-from pathlib import Path
-from typing import Any, Dict, List
-
-# import shutil
-from tqdm import tqdm
 
 warnings.filterwarnings("ignore")
 
 # Initialize the logger
 logger = logging.getLogger()
 logger.setLevel(logging.FATAL)
+
 # Create console handler
 ch = logging.StreamHandler()
 ch.setLevel(logging.FATAL)
 
 # Create formatter and add it to the handler
 formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
 ch.setFormatter(formatter)
 
 # Add the handler to the logger
 logger.addHandler(ch)
 
+logging.basicConfig(level=logging.FATAL)
+
 
 class Preprocessing:
     """
     This class is used to train the neural network model.
     for the bit type detection.
     """
 
@@ -53,29 +47,30 @@
         """
         This function is used to initialize the class.
         :param args:
         :param kwargs:
         """
         self.dataset_address = kwargs.get("dataset_address", None)
         self.categories_name_folders = None
+        self.sub_catego_data_address = None
 
     def download_images(self, category_list=None, from_s3=False, limit=None) -> None:
         """
         This function is used to download the images from the internet.
         :param category_list:
         :param from_s3: bool
         :param limit: int
         :param download_location_address:
         :return:
         """
         if from_s3:
             # download the images from the S3 bucket
             s3 = MyS3()
 
-            # Specify your bucket name and subfolders
+            # Specify your bucket name and folders
             bucket_name = SETTING.S3_BUCKET_SETTING.BUCKET_NAME
             subfolders = SETTING.S3_BUCKET_SETTING.SUBFOLDER_NAME
             download_location_address = (
                 self.dataset_address or SETTING.S3_BUCKET_SETTING.DOWNLOAD_LOCATION
             )
 
             s3.download_files_from_subfolders(
@@ -138,19 +133,26 @@
         image_dicts = {}
         for category_folder in self.categorie_name:
             # read the files in the dataset folder
             main_dataset_folder = (
                 self.dataset_address
                 or SETTING.DATA_ADDRESS_SETTING.MAIN_DATA_DIR_ADDRESS
             )
-            data_address = main_dataset_folder / category_folder
+            # check if the main_datast_folder is not None if yes then raise error
+            if main_dataset_folder is None:
+                logging.error("main_dataset_folder is None")
+                raise ValueError("main_dataset_folder is None")
+
+            self.sub_catego_data_address = main_dataset_folder / category_folder
             image_dicts[category_folder] = {}
-            image_dicts[category_folder]["image_list"] = list(data_address.iterdir())
+            image_dicts[category_folder]["image_list"] = list(
+                self.sub_catego_data_address.iterdir()
+            )
             image_dicts[category_folder]["number_of_images"] = len(
-                list(data_address.iterdir())
+                list(self.sub_catego_data_address.iterdir())
             )
 
         return image_dicts
 
     def augment_data(
         self,
         number_of_images_tobe_gen: int = SETTING.AUGMENTATION_SETTING.NUMBER_OF_IMAGES_TOBE_GENERATED,
@@ -265,18 +267,14 @@
         self._populated_augmented_images_into_train_test_val_dirs(
             augmented_data_address, train_test_val_split_dir_address
         )
 
     def _populated_augmented_images_into_train_test_val_dirs(self, *arges, **kwargs):
         dataset_augmented_dir_address = arges[0]
         train_test_val_split_dir_address = arges[1]
-        # dataset_augmented_dir_address = (
-        #         kwargs.get("dataset_augmented")
-        #         or SETTING.AUGMENTATION_SETTING.AUGMENTED_IMAGES_DIR_ADDRESS
-        # )
 
         for category in self.categories_name_folders:
             # get the list of images in the dataset_augmented category (i.e. pdc_bit) folder
             original_list = os.listdir(dataset_augmented_dir_address / category)
 
             # Number of items to select for each new list
             num_train = int(
@@ -352,15 +350,15 @@
         logger.info(
             f"copied {len(images)} images for category {categ} to {dest_folder}"
         )
 
 
 if __name__ == "__main__":
     obj = Preprocessing(dataset_address=Path(__file__).parent / ".." / "dataset")
-    obj.download_images()
+    # obj.download_images()
 
     # or download the data from s3. this is after you have downloaded the data
     # using Process.download_images() and uploaded it to s3
     # this way the data would be consistent across all the users
     # obj = Preprocessing(dataset_address=Path(__file__).parent / ".." / "s3_dataset")
     # obj.download_images(from_s3=True)
```

### Comparing `drillvision-0.0.3/neural_network_model/s3.py` & `drillvision-0.0.4/neural_network_model/s3.py`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.3/pyproject.toml` & `drillvision-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.3/setup.py` & `drillvision-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,16 +57,16 @@
     include_package_data=True,
     license="BSD-3",
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.8",
+        # "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: Implementation :: CPython",
-        "Programming Language :: Python :: Implementation :: PyPy",
+        # "Programming Language :: Python :: Implementation :: CPython",
+        # "Programming Language :: Python :: Implementation :: PyPy",
     ],
 )
 
 if __name__ == "__main__":
     list_reqs()
```

