# Comparing `tmp/code_loader-0.2.82.tar.gz` & `tmp/code-loader-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_loader-0.2.82.tar", max compression
+gzip compressed data, was "code-loader-0.2.9.tar", max compression
```

## Comparing `code_loader-0.2.82.tar` & `code-loader-0.2.9.tar`

### file list

```diff
@@ -1,32 +1,17 @@
--rw-r--r--   0        0        0     1067 2022-06-21 07:47:34.603402 code_loader-0.2.82/LICENSE
--rw-r--r--   0        0        0       63 2022-06-21 07:47:34.603402 code_loader-0.2.82/README.md
--rw-r--r--   0        0        0      116 2022-06-21 07:47:34.603402 code_loader-0.2.82/code_loader/__init__.py
--rw-r--r--   0        0        0        0 2022-06-21 07:47:34.603402 code_loader-0.2.82/code_loader/contract/__init__.py
--rw-r--r--   0        0        0     4268 2023-03-27 11:58:16.516358 code_loader-0.2.82/code_loader/contract/datasetclasses.py
--rw-r--r--   0        0        0     1481 2023-02-14 09:49:13.765854 code_loader-0.2.82/code_loader/contract/enums.py
--rw-r--r--   0        0        0       51 2023-01-31 13:19:30.815862 code_loader-0.2.82/code_loader/contract/exceptions.py
--rw-r--r--   0        0        0     2577 2023-04-10 12:21:18.280435 code_loader-0.2.82/code_loader/contract/responsedataclasses.py
--rw-r--r--   0        0        0     4761 2023-01-31 13:19:30.815862 code_loader-0.2.82/code_loader/contract/visualizer_classes.py
--rw-r--r--   0        0        0        0 2023-02-05 16:41:56.043877 code_loader-0.2.82/code_loader/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-02-05 16:41:56.043877 code_loader-0.2.82/code_loader/helpers/detection/__init__.py
--rw-r--r--   0        0        0     7527 2023-02-05 16:41:56.043877 code_loader-0.2.82/code_loader/helpers/detection/utils.py
--rw-r--r--   0        0        0        0 2023-02-05 16:41:56.043877 code_loader-0.2.82/code_loader/helpers/detection/yolo/__init__.py
--rw-r--r--   0        0        0     7902 2023-06-15 12:11:54.544590 code_loader-0.2.82/code_loader/helpers/detection/yolo/decoder.py
--rw-r--r--   0        0        0       81 2023-06-15 12:02:20.671928 code_loader-0.2.82/code_loader/helpers/detection/yolo/enums.py
--rw-r--r--   0        0        0     3132 2023-02-05 16:41:56.043877 code_loader-0.2.82/code_loader/helpers/detection/yolo/grid.py
--rw-r--r--   0        0        0    18643 2023-06-13 12:50:07.863065 code_loader-0.2.82/code_loader/helpers/detection/yolo/loss.py
--rw-r--r--   0        0        0    11349 2023-06-13 12:50:07.863065 code_loader-0.2.82/code_loader/helpers/detection/yolo/pytorch_utils.py
--rw-r--r--   0        0        0     8037 2023-06-15 12:11:54.544590 code_loader-0.2.82/code_loader/helpers/detection/yolo/utils.py
--rw-r--r--   0        0        0        0 2023-06-05 08:36:32.233647 code_loader-0.2.82/code_loader/helpers/instancesegmentation/__init__.py
--rw-r--r--   0        0        0      930 2023-06-05 08:36:32.233647 code_loader-0.2.82/code_loader/helpers/instancesegmentation/utils.py
--rw-r--r--   0        0        0       93 2022-06-21 07:47:34.607402 code_loader-0.2.82/code_loader/leap_binder/__init__.py
--rw-r--r--   0        0        0     6692 2023-03-27 11:58:16.516358 code_loader-0.2.82/code_loader/leap_binder/leapbinder.py
--rw-r--r--   0        0        0    15370 2023-06-15 12:02:20.671928 code_loader-0.2.82/code_loader/leaploader.py
--rw-r--r--   0        0        0        0 2023-02-14 09:49:13.765854 code_loader-0.2.82/code_loader/metrics/__init__.py
--rw-r--r--   0        0        0     6727 2023-03-27 11:58:16.520359 code_loader-0.2.82/code_loader/metrics/default_metrics.py
--rw-r--r--   0        0        0     5594 2023-05-22 15:43:07.692875 code_loader-0.2.82/code_loader/samples_generator_parallelized.py
--rw-r--r--   0        0        0     1736 2022-06-21 07:47:34.607402 code_loader-0.2.82/code_loader/utils.py
--rw-r--r--   0        0        0        0 2022-06-21 07:47:34.607402 code_loader-0.2.82/code_loader/visualizers/__init__.py
--rw-r--r--   0        0        0     2226 2023-01-31 13:19:30.815862 code_loader-0.2.82/code_loader/visualizers/default_visualizers.py
--rw-r--r--   0        0        0      900 2023-06-15 12:12:10.292686 code_loader-0.2.82/pyproject.toml
--rw-r--r--   0        0        0      947 1970-01-01 00:00:00.000000 code_loader-0.2.82/PKG-INFO
+-rw-r--r--   0        0        0     1067 2021-12-01 12:49:40.221608 code-loader-0.2.9/LICENSE
+-rw-r--r--   0        0        0       63 2021-12-01 12:49:40.221888 code-loader-0.2.9/README.md
+-rw-r--r--   0        0        0      131 2021-12-02 13:04:01.154724 code-loader-0.2.9/code_loader/__init__.py
+-rw-r--r--   0        0        0        0 2021-12-01 12:49:40.222215 code-loader-0.2.9/code_loader/contract/__init__.py
+-rw-r--r--   0        0        0     2357 2022-03-28 13:14:06.363969 code-loader-0.2.9/code_loader/contract/datasetclasses.py
+-rw-r--r--   0        0        0     1073 2022-01-30 17:03:35.077863 code-loader-0.2.9/code_loader/contract/decoder_classes.py
+-rw-r--r--   0        0        0      752 2022-01-30 17:03:35.078224 code-loader-0.2.9/code_loader/contract/enums.py
+-rw-r--r--   0        0        0     1409 2022-03-28 13:14:06.364283 code-loader-0.2.9/code_loader/contract/responsedataclasses.py
+-rw-r--r--   0        0        0      108 2021-12-02 13:04:01.155417 code-loader-0.2.9/code_loader/dataset_binder/__init__.py
+-rw-r--r--   0        0        0     3410 2022-03-28 13:14:06.364597 code-loader-0.2.9/code_loader/dataset_binder/datasetbinder.py
+-rw-r--r--   0        0        0     9242 2022-03-28 13:14:06.364931 code-loader-0.2.9/code_loader/datasetloader.py
+-rw-r--r--   0        0        0        0 2022-01-02 09:30:24.026399 code-loader-0.2.9/code_loader/decoders/__init__.py
+-rw-r--r--   0        0        0     2320 2022-01-11 15:15:30.813571 code-loader-0.2.9/code_loader/decoders/default_decoders.py
+-rw-r--r--   0        0        0     1548 2022-01-02 09:30:24.027864 code-loader-0.2.9/code_loader/utils.py
+-rw-r--r--   0        0        0      702 2022-03-28 13:14:39.404244 code-loader-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      797 2022-03-29 08:59:48.662325 code-loader-0.2.9/setup.py
+-rw-r--r--   0        0        0      562 2022-03-29 08:59:48.662571 code-loader-0.2.9/PKG-INFO
```

### Comparing `code_loader-0.2.82/LICENSE` & `code-loader-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `code_loader-0.2.82/code_loader/contract/enums.py` & `code-loader-0.2.9/code_loader/contract/enums.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,15 @@
 from enum import Enum, IntEnum
 
 
-class MetricEnum(Enum):
-    MeanSquaredError = 'MeanSquaredError'
-    MeanSquaredLogarithmicError = 'MeanSquaredLogarithmicError'
-    MeanAbsoluteError = 'MeanAbsoluteError'
-    MeanAbsolutePercentageError = 'MeanAbsolutePercentageError'
-    Accuracy = 'Accuracy'
-    BinaryAccuracy = 'BinaryAccuracy'
-    MeanIOU = 'MeanIOU'
-    ConfusionMatrixClassification = 'ConfusionMatrixClassification'
-    ConfusionMatrixBinaryClassification = 'ConfusionMatrixBinaryClassification'
-
-
-# backwards compatability: keeping it to not break old imports of Metric enum
-# should not be copied to engine contracts
-Metric = MetricEnum
-
-
 class LeapDataType(Enum):
     Image = 'Image'
     Text = 'Text'
     Graph = 'Graph'
+    Numeric = 'Numeric'
     HorizontalBar = 'HorizontalBar'
     ImageMask = 'ImageMask'
     TextMask = 'TextMask'
     ImageWithBBox = 'ImageWithBBox'
 
 
 class DatasetMetadataType(Enum):
@@ -35,26 +19,19 @@
     boolean = "boolean"
 
 
 class DataStateType(Enum):
     training = "training"
     validation = "validation"
     test = "test"
-    unlabeled = "unlabeled"
 
 
 class DataStateEnum(IntEnum):
     training = 0
     validation = 1
     test = 2
-    unlabeled = 3
-
-
-class ConfusionMatrixValue(Enum):
-    Positive = "Positive"
-    Negative = "Negative"
 
 
 # todo: handle test not run due to error in pre process and Add to TestingSectionEnum Enum didn't run
 class TestingSectionEnum(Enum):
     Warnings = "Warnings"
     Errors = "Errors"
```

### Comparing `code_loader-0.2.82/code_loader/contract/responsedataclasses.py` & `code-loader-0.2.9/code_loader/contract/responsedataclasses.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import List, Optional, Dict
 
 from dataclasses import dataclass, field
+
 from code_loader.contract.enums import DatasetMetadataType, LeapDataType
 
 
 @dataclass
 class DatasetPreprocess:
     training_length: int
     validation_length: int
     test_length: Optional[int] = None
-    unlabeled_length: Optional[int] = None
 
 
 @dataclass
 class DatasetBaseSectionInstance:
     name: str
 
 
@@ -29,84 +29,42 @@
 
 @dataclass
 class DatasetOutputInstance(DatasetBaseSectionInstance):
     shape: List[int]
 
 
 @dataclass
-class VisualizerInstance:
+class DecoderInstance:
     name: str
     type: LeapDataType
-    arg_names: List[str]
-
-
-@dataclass
-class MetricInstance:
-    name: str
-    arg_names: List[str]
 
 
 @dataclass
-class CustomLossInstance:
-    name: str
-    arg_names: List[str]
-
-
-@dataclass
-class CustomLayerInstance:
-    name: str
-    init_arg_names: List[str]
-    call_arg_names: List[str]
-
-
-@dataclass
-class PredictionTypeInstance:
+class HeatmapBlockInstance:
     name: str
     labels: List[str]
 
 
 @dataclass
 class DatasetSetup:
     preprocess: DatasetPreprocess
     inputs: List[DatasetInputInstance]
     metadata: List[DatasetMetadataInstance]
     outputs: List[DatasetOutputInstance]
-    visualizers: List[VisualizerInstance]
-    prediction_types: List[PredictionTypeInstance]
-    custom_losses: List[CustomLossInstance]
-    metrics: List[MetricInstance] = field(default_factory=list)
-
-
-@dataclass
-class ModelSetup:
-    custom_layers: List[CustomLayerInstance]
+    decoders: List[DecoderInstance]
+    heatmap_blocks: List[HeatmapBlockInstance]
 
 
 @dataclass
 class DatasetTestResultPayload:
     name: str
     display: Dict[str, str] = field(default_factory=dict)
     is_passed: bool = True
     shape: Optional[List[int]] = None
 
 
 @dataclass
-class BoundingBox:
-    # (x, y) is the center of the bounding box
-    x: float  # value between [0, 1], represent the percentage according to the image size.
-    y: float  # value between [0, 1], represent the percentage according to the image size.
-
-    width: float  # value between [0, 1], represent the percentage according to the image size.
-    height: float  # value between [0, 1], represent the percentage according to the image size.
-    confidence: float
-    label: str
-
-
-@dataclass
 class DatasetIntegParseResult:
     payloads: List[DatasetTestResultPayload]
     is_valid: bool
-    is_valid_for_model: Optional[bool] = False
-    setup: Optional[DatasetSetup] = None
-    model_setup: Optional[ModelSetup] = None
-    general_error: Optional[str] = None
-    print_log: Optional[str] = None
+    setup: Optional[DatasetSetup]
+    general_error: Optional[str]
```

### Comparing `code_loader-0.2.82/code_loader/utils.py` & `code-loader-0.2.9/code_loader/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import sys
+from typing import List
 from types import TracebackType
-from typing import List, Union
-
-import numpy as np
-import numpy.typing as npt
+import numpy as np  # type: ignore
 
 from code_loader.contract.datasetclasses import SectionCallableInterface, PreprocessResponse
 
 
 def to_numpy_return_wrapper(encoder_function: SectionCallableInterface) -> SectionCallableInterface:
-    def numpy_encoder_function(idx: int, samples: PreprocessResponse) -> npt.NDArray[np.float32]:
+    def numpy_encoder_function(idx: int, samples: PreprocessResponse) -> np.ndarray:
         result = encoder_function(idx, samples)
-        numpy_result: npt.NDArray[np.float32] = np.array(result)
+        numpy_result = np.array(result)
         return numpy_result
 
     return numpy_encoder_function
 
 
 def get_root_traceback(exc_tb: TracebackType) -> TracebackType:
     return_traceback = exc_tb
@@ -29,26 +27,24 @@
     root_exception_line_number = -1
     if exc_tb is not None:
         root_traceback = get_root_traceback(exc_tb)
         root_exception_line_number = root_traceback.tb_lineno
     return root_exception_line_number
 
 
-def get_shape(result: Union[npt.NDArray[np.float32], str, float, int, bool]) -> List[int]:
-    if not isinstance(result, np.ndarray):
-        return [1]
+def get_shape(result: np.ndarray) -> List[int]:
     np_shape = result.shape
     # fix single result shape viewing
-    if np_shape == ():
+    if np_shape is ():
         np_shape = (1,)
     shape = list(np_shape)
     return shape
 
 
-def rescale_min_max(image: npt.NDArray[np.float32]) -> npt.NDArray[np.float32]:
+def rescale_min_max(image: np.ndarray) -> np.ndarray:
     image = image.astype('float32')
     image -= image.min()
     image /= (image.max() - image.min() + 1e-5)
 
     # rescale the values to range between 0 and 255
     image *= 255
     image = image.astype('uint8')
```

### Comparing `code_loader-0.2.82/pyproject.toml` & `code-loader-0.2.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 [tool.poetry]
 name = "code-loader"
-version = "0.2.82"
+version = "0.2.9"
 description = ""
 authors = ["dorhar <doron.harnoy@tensorleap.ai>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/tensorleap/code-loader"
 homepage = "https://github.com/tensorleap/code-loader"
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
-numpy = "^1.22.3"
-tensorflow = {version = "^2.11.0", markers = "platform_machine  == 'x86_64'"}
-tensorflow-macos = {version = "^2.11.0", markers = "platform_machine  == 'arm64'"}
-typeguard = "^2.13.3"
-psutil = "^5.9.5"
-torch = "1.12.1"
+python = ">=3.6.1,<3.7"
+numpy = "^1.19.2"
+dataclasses = "0.8"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.1"
+pytest = "^6.2.5"
 grappa = "^1.0.1"
 pytest-cov = "^3.0.0"
 pytest-watch = "^4.2.0"
-mypy = "1.3.0"
+mypy = "^0.910"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
-filterwarnings = ["ignore:.*the imp module.*:DeprecationWarning"]
+filterwarnings = ["ignore:.*the imp module.*:DeprecationWarning"]
```

