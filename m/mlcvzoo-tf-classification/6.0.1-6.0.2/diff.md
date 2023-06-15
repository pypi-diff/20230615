# Comparing `tmp/mlcvzoo_tf_classification-6.0.1.tar.gz` & `tmp/mlcvzoo_tf_classification-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcvzoo_tf_classification-6.0.1.tar", max compression
+gzip compressed data, was "mlcvzoo_tf_classification-6.0.2.tar", max compression
```

## Comparing `mlcvzoo_tf_classification-6.0.1.tar` & `mlcvzoo_tf_classification-6.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      434 2023-05-02 10:18:08.297754 mlcvzoo_tf_classification-6.0.1/README.md
--rw-r--r--   0        0        0      177 2023-05-05 09:21:26.582902 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/__init__.py
--rw-r--r--   0        0        0     1890 2023-05-02 10:18:08.297754 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/annotation_utils.py
--rw-r--r--   0        0        0    12346 2023-05-02 10:18:08.297754 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/base_model.py
--rw-r--r--   0        0        0     9170 2023-05-02 10:18:08.297754 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/configuration.py
--rw-r--r--   0        0        0     3040 2023-05-02 10:18:08.297754 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/const.py
--rw-r--r--   0        0        0      263 2023-05-02 10:18:08.297754 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/custom_block/__init__.py
--rw-r--r--   0        0        0     1073 2023-05-02 10:18:08.297754 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/custom_block/configuration.py
--rw-r--r--   0        0        0     4484 2023-05-02 10:18:08.297754 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/custom_block/model.py
--rw-r--r--   0        0        0    11815 2023-05-02 10:18:08.297754 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/image_generator.py
--rw-r--r--   0        0        0      154 2023-05-02 10:18:08.297754 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/py.typed
--rw-r--r--   0        0        0      279 2023-05-02 10:18:08.301755 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/xception/__init__.py
--rw-r--r--   0        0        0     1111 2023-05-02 10:18:08.301755 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/xception/configuration.py
--rw-r--r--   0        0        0     3804 2023-05-02 10:18:08.301755 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/xception/model.py
--rw-r--r--   0        0        0     3870 2023-05-05 09:21:26.582902 mlcvzoo_tf_classification-6.0.1/pyproject.toml
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 mlcvzoo_tf_classification-6.0.1/setup.py
--rw-r--r--   0        0        0     1982 1970-01-01 00:00:00.000000 mlcvzoo_tf_classification-6.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11412 2023-06-13 11:44:42.497695 mlcvzoo_tf_classification-6.0.2/LICENSE
+-rw-r--r--   0        0        0      434 2023-06-13 11:44:42.497695 mlcvzoo_tf_classification-6.0.2/README.md
+-rw-r--r--   0        0        0      244 2023-06-15 07:08:06.195871 mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/__init__.py
+-rw-r--r--   0        0        0     1932 2023-06-13 11:44:42.497695 mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/annotation_utils.py
+-rw-r--r--   0        0        0    12388 2023-06-13 11:44:42.497695 mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/base_model.py
+-rw-r--r--   0        0        0     9212 2023-06-13 11:44:42.497695 mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/configuration.py
+-rw-r--r--   0        0        0     3082 2023-06-13 11:44:42.497695 mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/const.py
+-rw-r--r--   0        0        0      305 2023-06-13 11:44:42.497695 mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/custom_block/__init__.py
+-rw-r--r--   0        0        0     1115 2023-06-13 11:44:42.497695 mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/custom_block/configuration.py
+-rw-r--r--   0        0        0     4526 2023-06-13 11:44:42.497695 mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/custom_block/model.py
+-rw-r--r--   0        0        0    11857 2023-06-13 11:44:42.497695 mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/image_generator.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:44:42.497695 mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/py.typed
+-rw-r--r--   0        0        0      321 2023-06-13 11:44:42.501695 mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/xception/__init__.py
+-rw-r--r--   0        0        0     1153 2023-06-13 11:44:42.501695 mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/xception/configuration.py
+-rw-r--r--   0        0        0     3846 2023-06-13 11:44:42.501695 mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/xception/model.py
+-rw-r--r--   0        0        0     3971 2023-06-15 07:08:06.195871 mlcvzoo_tf_classification-6.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1557 1970-01-01 00:00:00.000000 mlcvzoo_tf_classification-6.0.2/setup.py
+-rw-r--r--   0        0        0     1986 1970-01-01 00:00:00.000000 mlcvzoo_tf_classification-6.0.2/PKG-INFO
```

### Comparing `mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/annotation_utils.py` & `mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/annotation_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for handling annotation utility methods that are used across the
 mlcvzoo_tf_classification package.
 """
 
 from typing import Any, Dict, List
```

### Comparing `mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/base_model.py` & `mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for handling the implementation of a generic base model that wraps tensorflow
 classification models.
 """
 
 import logging
```

### Comparing `mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/configuration.py` & `mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Definition of the Config that is used to configure the models of the
 mlcvzoo_tf_classification package.
 """
 import logging
 from typing import List, Optional, Union
```

### Comparing `mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/const.py` & `mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for enumerating options for different configurations for different parameters.
 The constant classes listed here are e.g. used in data generators to
 limit the options in configuration.
 """
```

### Comparing `mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/custom_block/configuration.py` & `mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/custom_block/configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 This configuration class is for building python objects from the configuration file.
 The respective config fields are parsed via the related component from config_builder module.
 """
 
 import related
```

### Comparing `mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/custom_block/model.py` & `mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/custom_block/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 The CustomBlockModel configures the model for training and inference.
 The respective model is compiled from the provided configuration file and net class.
 Input data classes are parsed via the AnnotationClassMapper.
 Data flow is regulated via Generators.
 """
```

### Comparing `mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/image_generator.py` & `mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/image_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for handling the generation of images for the training of
 tensorflow classification models.
 """
 
 import logging
```

### Comparing `mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/xception/configuration.py` & `mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/xception/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 This configuration class is for building python objects from the configuration file.
 The respective config fields are parsed via the related component from config_builder module.
 """
 import related
 from attr import define
```

### Comparing `mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/xception/model.py` & `mlcvzoo_tf_classification-6.0.2/mlcvzoo_tf_classification/xception/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 The TrainableNetBasedModel class configures the model for training and inference.
 The respective model is compiled from the provided configuration file and net class.
 Input parameters are parsed via the AnnotationMapper.
 Data flow is regulated via Generators.
 """
```

### Comparing `mlcvzoo_tf_classification-6.0.1/pyproject.toml` & `mlcvzoo_tf_classification-6.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "mlcvzoo_tf_classification"
-version = "6.0.1"
-license = "Open Logistics License Version 1.0"
 description = "MLCVZoo TF Classifcation Package"
+version = "6.0.2"
+license = "Open Logistics Foundation License v1.3"
 readme = "README.md"
 homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -26,40 +26,43 @@
 exclude = ["mlcvzoo_tf_classification/tests/**/*"]
 
 packages = [
     { include = "mlcvzoo_tf_classification" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8, <3.11"
+# The limit to python 3.11 is necessary for tensorflow-io-gcs-filesystem
+python = ">=3.8, <3.12"
 
 yaml-config-builder = { version = "^8" }
-related-mltoolbox = { version = "^1.0" }
-mlcvzoo_base = { version = "^5.0" }
-
+related-mltoolbox = { version = "^1" }
+mlcvzoo_base = { version = "^5" }
 attrs = { version = ">=20" }
-opencv-python = { version = "^4.5,!=4.5.5.64,!=4.6.0.66" }
-opencv-contrib-python = { version = "^4.5,!=4.5.5.64,!=4.6.0.66,!=4.7.0.68" }
+
 # 1.19.2 is oldest available on aarch64 but 1.19.5 leads to unbuildable pytorch there, all is well on amd64
 numpy = { version = ">=1.19.2,!=1.19.5" }
 nptyping = { version = ">=2.0" }
+opencv-python = { version = ">=4.5,!=4.5.5.64"}
+opencv-contrib-python = { version = ">=4.5,!=4.5.5.64" }
+
 tensorflow-cpu = { version=">=2.6" }
 keras = { version=">=2.6" }
 keras-preprocessing = { version=">=1" }
 pandas = { version=">=1.3.3" }
 
 [tool.poetry.dev-dependencies]
 mock = { version = ">=4.0" }
 pytest = { version = ">=7.0" }
 pytest-cov = { version = ">=3.0.0" }
 black = { version = ">=22" }
 mypy = { version = ">=0.961" }
 pylint = { version = ">=2.9.6" }
-isort = { version = ">=5.9" }
-pytest-mock = ">=3.7"
+# Isort guarantees formatting results for 5.X
+isort = { version = "^5.0" }
+pytest-mock = { version = ">=3.7" }
 
 [build-system]
 # NOTE: Don't remove setuptools, therefore require it from the build system
 requires = ["setuptools", "poetry_core>=1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
```

### Comparing `mlcvzoo_tf_classification-6.0.1/setup.py` & `mlcvzoo_tf_classification-6.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,35 +9,35 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['attrs>=20',
  'keras-preprocessing>=1',
  'keras>=2.6',
- 'mlcvzoo_base>=5.0,<6.0',
+ 'mlcvzoo_base>=5,<6',
  'nptyping>=2.0',
  'numpy>=1.19.2,!=1.19.5',
- 'opencv-contrib-python>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66,!=4.7.0.68',
- 'opencv-python>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66',
+ 'opencv-contrib-python>=4.5,!=4.5.5.64',
+ 'opencv-python>=4.5,!=4.5.5.64',
  'pandas>=1.3.3',
- 'related-mltoolbox>=1.0,<2.0',
+ 'related-mltoolbox>=1,<2',
  'tensorflow-cpu>=2.6',
  'yaml-config-builder>=8,<9']
 
 setup_kwargs = {
     'name': 'mlcvzoo-tf-classification',
-    'version': '6.0.1',
+    'version': '6.0.2',
     'description': 'MLCVZoo TF Classifcation Package',
     'long_description': '# MLCVZoo TF Classification\n\nThe MLCVZoo is an SDK for simplifying the usage of various (machine learning driven)\ncomputer vision algorithms. The package **mlcvzoo_tf_classification** is the wrapper module\nfor classification algorithms that are implemented using tensorflow.\n\nFurther information about the MLCVZoo can be found [here](../README.md).\n\n## Install\n`\npip install mlcvzoo-tf-classification\n`\n\n## Technology stack\n\n- Python\n',
     'author': 'Maximilian Otten',
     'author_email': 'maximilian.otten@iml.fraunhofer.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
+    'python_requires': '>=3.8,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `mlcvzoo_tf_classification-6.0.1/PKG-INFO` & `mlcvzoo_tf_classification-6.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: mlcvzoo-tf-classification
-Version: 6.0.1
+Version: 6.0.2
 Summary: MLCVZoo TF Classifcation Package
 Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
-License: Open Logistics License Version 1.0
+License: Open Logistics Foundation License v1.3
 Author: Maximilian Otten
 Author-email: maximilian.otten@iml.fraunhofer.de
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=20)
 Requires-Dist: keras (>=2.6)
 Requires-Dist: keras-preprocessing (>=1)
-Requires-Dist: mlcvzoo_base (>=5.0,<6.0)
+Requires-Dist: mlcvzoo_base (>=5,<6)
 Requires-Dist: nptyping (>=2.0)
 Requires-Dist: numpy (>=1.19.2,!=1.19.5)
-Requires-Dist: opencv-contrib-python (>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66,!=4.7.0.68)
-Requires-Dist: opencv-python (>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66)
+Requires-Dist: opencv-contrib-python (>=4.5,!=4.5.5.64)
+Requires-Dist: opencv-python (>=4.5,!=4.5.5.64)
 Requires-Dist: pandas (>=1.3.3)
-Requires-Dist: related-mltoolbox (>=1.0,<2.0)
+Requires-Dist: related-mltoolbox (>=1,<2)
 Requires-Dist: tensorflow-cpu (>=2.6)
 Requires-Dist: yaml-config-builder (>=8,<9)
 Project-URL: Documentation, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc
 Project-URL: Repository, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
 Description-Content-Type: text/markdown
 
 # MLCVZoo TF Classification
```

