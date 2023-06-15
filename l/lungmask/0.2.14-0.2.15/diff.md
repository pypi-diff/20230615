# Comparing `tmp/lungmask-0.2.14.tar.gz` & `tmp/lungmask-0.2.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lungmask-0.2.14.tar", last modified: Tue Apr 18 14:03:51 2023, max compression
+gzip compressed data, was "lungmask-0.2.15.tar", last modified: Thu Jun 15 06:09:22 2023, max compression
```

## Comparing `lungmask-0.2.14.tar` & `lungmask-0.2.15.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:03:51.331893 lungmask-0.2.14/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 14:03:36.000000 lungmask-0.2.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-04-18 14:03:51.331893 lungmask-0.2.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-04-18 14:03:36.000000 lungmask-0.2.14/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:03:51.331893 lungmask-0.2.14/lungmask/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-18 14:03:37.000000 lungmask-0.2.14/lungmask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-18 14:03:37.000000 lungmask-0.2.14/lungmask/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-04-18 14:03:37.000000 lungmask-0.2.14/lungmask/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-04-18 14:03:37.000000 lungmask-0.2.14/lungmask/resunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-04-18 14:03:37.000000 lungmask-0.2.14/lungmask/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:03:51.331893 lungmask-0.2.14/lungmask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-04-18 14:03:51.000000 lungmask-0.2.14/lungmask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-18 14:03:51.000000 lungmask-0.2.14/lungmask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:03:51.000000 lungmask-0.2.14/lungmask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 14:03:51.000000 lungmask-0.2.14/lungmask.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-18 14:03:51.000000 lungmask-0.2.14/lungmask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 14:03:51.000000 lungmask-0.2.14/lungmask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-18 14:03:37.000000 lungmask-0.2.14/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 14:03:51.331893 lungmask-0.2.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-18 14:03:37.000000 lungmask-0.2.14/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:03:51.331893 lungmask-0.2.14/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-18 14:03:37.000000 lungmask-0.2.14/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-18 14:03:37.000000 lungmask-0.2.14/tests/test_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-18 14:03:37.000000 lungmask-0.2.14/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:09:22.337246 lungmask-0.2.15/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 06:09:11.000000 lungmask-0.2.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-15 06:09:22.337246 lungmask-0.2.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-06-15 06:09:11.000000 lungmask-0.2.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:09:22.333246 lungmask-0.2.15/lungmask/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 06:09:11.000000 lungmask-0.2.15/lungmask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-15 06:09:11.000000 lungmask-0.2.15/lungmask/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-06-15 06:09:11.000000 lungmask-0.2.15/lungmask/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-06-15 06:09:11.000000 lungmask-0.2.15/lungmask/resunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-06-15 06:09:11.000000 lungmask-0.2.15/lungmask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:09:22.337246 lungmask-0.2.15/lungmask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-15 06:09:22.000000 lungmask-0.2.15/lungmask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-15 06:09:22.000000 lungmask-0.2.15/lungmask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:09:22.000000 lungmask-0.2.15/lungmask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 06:09:22.000000 lungmask-0.2.15/lungmask.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 06:09:22.000000 lungmask-0.2.15/lungmask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 06:09:22.000000 lungmask-0.2.15/lungmask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-15 06:09:11.000000 lungmask-0.2.15/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 06:09:22.337246 lungmask-0.2.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-15 06:09:11.000000 lungmask-0.2.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:09:22.337246 lungmask-0.2.15/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-15 06:09:11.000000 lungmask-0.2.15/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-15 06:09:11.000000 lungmask-0.2.15/tests/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-06-15 06:09:11.000000 lungmask-0.2.15/tests/test_utils.py
```

### Comparing `lungmask-0.2.14/LICENSE` & `lungmask-0.2.15/LICENSE`

 * *Files identical despite different names*

### Comparing `lungmask-0.2.14/PKG-INFO` & `lungmask-0.2.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lungmask
-Version: 0.2.14
+Version: 0.2.15
 Summary: Package for automated lung segmentation in CT
 Home-page: https://github.com/JoHof/lungmask
 Author: Johannes Hofmanninger
 Author-email: johannes.hofmanninger@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `lungmask-0.2.14/README.md` & `lungmask-0.2.15/README.md`

 * *Files identical despite different names*

### Comparing `lungmask-0.2.14/lungmask/__main__.py` & `lungmask-0.2.15/lungmask/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import sys
 
 import numpy as np
 import pkg_resources  # type: ignore
 import SimpleITK as sitk
 
-from lungmask import mask, utils
+from lungmask import LMInferer, utils
 
 
 def path(string):
     if os.path.exists(string):
         return string
     else:
         sys.exit(f"File not found: {string}")
@@ -44,15 +44,14 @@
     )
     parser.add_argument(
         "--modelpath", help="spcifies the path to the trained model", default=None
     )
     parser.add_argument(
         "--classes",
         help="spcifies the number of output classes of the model",
-        default=3,
     )
     parser.add_argument(
         "--cpu",
         help="Force using the CPU even when a GPU is available, will override batchsize to 1",
         action="store_true",
     )
     parser.add_argument(
@@ -82,49 +81,55 @@
         action="version",
         version=version,
     )
 
     argsin = sys.argv[1:]
     args = parser.parse_args(argsin)
 
+    if args.classes is not None:
+        logging.warn(
+            "!!! Warning: The `classes` parameter is deprecated and will be removed in the next version !!!"
+        )
+
     batchsize = args.batchsize
     if args.cpu:
         batchsize = 1
 
     logging.info("Load model")
 
     input_image = utils.load_input_image(args.input, disable_tqdm=args.noprogress)
     logging.info("Infer lungmask")
     if args.modelname == "LTRCLobes_R231":
         assert (
             args.modelpath is None
         ), "Modelpath can not be specified for LTRCLobes_R231 mode"
-        result = mask.apply_fused(
-            input_image,
+        inferer = LMInferer(
+            modelname="LTRCLobes",
             force_cpu=args.cpu,
+            fillmodel="R231",
             batch_size=batchsize,
             volume_postprocessing=not (args.nopostprocess),
             noHU=args.noHU,
             tqdm_disable=args.noprogress,
         )
+        result = inferer.apply(input_image)
     else:
-        model = mask.get_model(args.modelname, args.modelpath, args.classes)
-        result = mask.apply(
-            input_image,
-            model,
+        inferer = LMInferer(
+            modelname=args.modelname,
+            modelpath=args.modelpath,
             force_cpu=args.cpu,
             batch_size=batchsize,
             volume_postprocessing=not (args.nopostprocess),
             noHU=args.noHU,
             tqdm_disable=args.noprogress,
         )
+        result = inferer.apply(input_image)
 
     if args.noHU:
         file_ending = args.output.split(".")[-1]
-        print(file_ending)
         if file_ending in ["jpg", "jpeg", "png"]:
             result = (result / (result.max()) * 255).astype(np.uint8)
         result = result[0]
 
     result_out = sitk.GetImageFromArray(result)
     result_out.CopyInformation(input_image)
     logging.info(f"Save result to: {args.output}")
```

### Comparing `lungmask-0.2.14/lungmask/mask.py` & `lungmask-0.2.15/lungmask/mask.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import os
 import sys
 import warnings
 from typing import Optional, Union
 
 import numpy as np
 import SimpleITK as sitk
 import skimage
@@ -37,35 +38,34 @@
     "R231CovidWeb": (
         "https://github.com/JoHof/lungmask/releases/download/v0.0/unet_r231covid-0de78a7e.pth",
         3,
     ),
 }
 
 
-def get_model(
-    modelname: str, modelpath: Optional[str] = None, n_classes: int = 3
-) -> torch.nn.Module:
+def get_model(modelname: str, modelpath: Optional[str] = None) -> torch.nn.Module:
     """Loads specific model and state
 
     Args:
         modelname (str): Modelname (e.g. R231, LTRCLobes or R231CovidWeb)
         modelpath (Optional[str], optional): Path to statedict, if not provided will be downloaded automatically. Modelname will be ignored if provided. Defaults to None.
-        n_classes (int, optional): Number of classes. Will be automatically set if modelname is provided. Defaults to 3.
 
     Returns:
         torch.nn.Module: Loaded model in eval state
     """
     if modelpath is None:
         model_url, n_classes = MODEL_URLS[modelname]
         state_dict = torch.hub.load_state_dict_from_url(
             model_url, progress=True, map_location=torch.device("cpu")
         )
     else:
         state_dict = torch.load(modelpath, map_location=torch.device("cpu"))
 
+    n_classes = len(list(state_dict.values())[-1])
+
     model = UNet(
         n_classes=n_classes,
         padding=True,
         depth=5,
         up_mode="upsample",
         batch_norm=True,
         residual=False,
@@ -74,61 +74,72 @@
     model.eval()
     return model
 
 
 class LMInferer:
     def __init__(
         self,
-        modelname="R231",
+        modelname: str = "R231",
+        modelpath: Optional[str] = None,
         fillmodel: Optional[str] = None,
-        force_cpu=False,
-        batch_size=20,
-        volume_postprocessing=True,
-        noHU=False,
-        tqdm_disable=False,
+        fillmodel_path: Optional[str] = None,
+        force_cpu: bool = False,
+        batch_size: int = 20,
+        volume_postprocessing: bool = True,
+        noHU: bool = False,
+        tqdm_disable: bool = False,
     ):
         """LungMaskInference
 
         Args:
             modelname (str, optional): Model to be applied. Defaults to 'R231'.
+            modelpath (str, optional): Path to modeleights. `modelname` parameter will be ignored if provided. Defaults to None.
             fillmodel (Optional[str], optional): Fillmodel to be applied. Defaults to None.
+            fillmodel_path (Optional[str], optional): Path to weights for fillmodel. `fillmodel` parameter will be ignored if provided. Defaults to None.
             force_cpu (bool, optional): Will not use GPU is `True`. Defaults to False.
             batch_size (int, optional): Batch size. Defaults to 20.
             volume_postprocessing (bool, optional): If `Fales` will not perform postprocessing (connected component analysis). Defaults to True.
             noHU (bool, optional): If `True` no HU intensities are expected. Not recommended. Defaults to False.
             tqdm_disable (bool, optional): If `True`, will disable progress bar. Defaults to False.
         """
         assert (
             modelname in MODEL_URLS
         ), "Modelname not found. Please choose from: {}".format(MODEL_URLS.keys())
         if fillmodel is not None:
             assert (
                 fillmodel in MODEL_URLS
             ), "Modelname not found. Please choose from: {}".format(MODEL_URLS.keys())
+
+        # if paths provided, overwrite name
+        if modelpath is not None:
+            modelname = os.path.basename(modelpath)
+        if fillmodel_path is not None:
+            fillmodel = os.path.basename(fillmodel_path)
+
         self.fillmodel = fillmodel
         self.modelname = modelname
         self.force_cpu = force_cpu
         self.batch_size = batch_size
         self.volume_postprocessing = volume_postprocessing
         self.noHU = noHU
         self.tqdm_disable = tqdm_disable
 
-        self.model = get_model(self.modelname)
+        self.model = get_model(self.modelname, modelpath)
 
         self.device = torch.device("cpu")
         if not self.force_cpu:
             if torch.cuda.is_available():
                 self.device = torch.device("cuda")
             else:
                 logging.info("No GPU found, using CPU instead")
         self.model.to(self.device)
 
         self.fillmodelm = None
         if self.fillmodel is not None:
-            self.fillmodelm = get_model(self.fillmodel)
+            self.fillmodelm = get_model(self.fillmodel, fillmodel_path)
             self.fillmodelm.to(self.device)
 
     def _inference(
         self, image: Union[sitk.Image, np.ndarray], model: torch.nn.Module
     ) -> np.ndarray:
         """Performs model inference
 
@@ -246,14 +257,18 @@
     model=None,
     force_cpu=False,
     batch_size=20,
     volume_postprocessing=True,
     noHU=False,
     tqdm_disable=False,
 ):
+    warnings.warn(
+        "The function `apply` will be removed in a future version. Please use the LMInferer class!",
+        DeprecationWarning,
+    )
     inferer = LMInferer(
         force_cpu=force_cpu,
         batch_size=batch_size,
         volume_postprocessing=volume_postprocessing,
         noHU=noHU,
         tqdm_disable=tqdm_disable,
     )
@@ -268,14 +283,18 @@
     fillmodel="R231",
     force_cpu=False,
     batch_size=20,
     volume_postprocessing=True,
     noHU=False,
     tqdm_disable=False,
 ):
+    warnings.warn(
+        "The function `apply_fused` will be removed in a future version. Please use the LMInferer class!",
+        DeprecationWarning,
+    )
     inferer = LMInferer(
         modelname=basemodel,
         force_cpu=force_cpu,
         fillmodel=fillmodel,
         batch_size=batch_size,
         volume_postprocessing=volume_postprocessing,
         noHU=noHU,
```

### Comparing `lungmask-0.2.14/lungmask/resunet.py` & `lungmask-0.2.15/lungmask/resunet.py`

 * *Files identical despite different names*

### Comparing `lungmask-0.2.14/lungmask/utils.py` & `lungmask-0.2.15/lungmask/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,14 +248,15 @@
         spare (list, optional): Labels that are used for mapping to neighbors but not considered for final labelling. This is used for label fusion with a filling model. Defaults to [].
         disable_tqdm (bool, optional): If true, tqdm will be diabled. Defaults to False.
         skip_below (int, optional): If a CC is smaller than this value. It will not be merged but removed. This is for performance optimization.
 
     Returns:
         np.ndarray: Postprocessed volume
     """
+    logging.info("Postprocessing")
 
     # CC analysis
     regionmask = skimage.measure.label(label_image)
     origlabels = np.unique(label_image)
     origlabels_maxsub = np.zeros(
         (max(origlabels) + 1,), dtype=np.uint32
     )  # will hold the largest component for a label
```

### Comparing `lungmask-0.2.14/lungmask.egg-info/PKG-INFO` & `lungmask-0.2.15/lungmask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lungmask
-Version: 0.2.14
+Version: 0.2.15
 Summary: Package for automated lung segmentation in CT
 Home-page: https://github.com/JoHof/lungmask
 Author: Johannes Hofmanninger
 Author-email: johannes.hofmanninger@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `lungmask-0.2.14/setup.py` & `lungmask-0.2.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lungmask",
-    version="0.2.14",
+    version="0.2.15",
     author="Johannes Hofmanninger",
     author_email="johannes.hofmanninger@gmail.com",
     description="Package for automated lung segmentation in CT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JoHof/lungmask",
     packages=setuptools.find_packages(),
```

### Comparing `lungmask-0.2.14/tests/test_cli.py` & `lungmask-0.2.15/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `lungmask-0.2.14/tests/test_utils.py` & `lungmask-0.2.15/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import os
 
 import numpy as np
-import pydicom as pd
-import pydicom as pyd
 import SimpleITK as sitk
-from pydicom.dataset import FileMetaDataset
 
 from lungmask.utils import (
     bbox_3D,
     crop_and_resize,
     load_input_image,
     postprocessing,
     preprocess,
     read_dicoms,
     reshape_mask,
     simple_bodymask,
 )
 
 # creating test dicom data for reference
+# import pydicom as pd
+# import pydicom as pyd
+# from pydicom.dataset import FileMetaDataset
 #
 # studyuid = pyd.uid.generate_uid()
 # seriesuid = pyd.uid.generate_uid()
 # for i in range(2):
 #     testd = pyd.Dataset()
 #     testd.PixelSpacing = [.625, .625]
 #     testd.SliceThickness = 1
```

