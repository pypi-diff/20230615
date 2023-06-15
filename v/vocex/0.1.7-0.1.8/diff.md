# Comparing `tmp/vocex-0.1.7.tar.gz` & `tmp/vocex-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocex-0.1.7.tar", last modified: Wed Jun 14 00:41:03 2023, max compression
+gzip compressed data, was "vocex-0.1.8.tar", last modified: Thu Jun 15 10:02:14 2023, max compression
```

## Comparing `vocex-0.1.7.tar` & `vocex-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 cdminix   (1000) cdminix   (1000)        0 2023-06-14 00:41:03.886232 vocex-0.1.7/
--rw-rw-r--   0 cdminix   (1000) cdminix   (1000)      227 2023-06-14 00:41:03.886232 vocex-0.1.7/PKG-INFO
--rw-rw-r--   0 cdminix   (1000) cdminix   (1000)        9 2023-06-11 08:34:35.000000 vocex-0.1.7/README.md
--rw-rw-r--   0 cdminix   (1000) cdminix   (1000)       38 2023-06-14 00:41:03.886232 vocex-0.1.7/setup.cfg
--rw-rw-r--   0 cdminix   (1000) cdminix   (1000)      470 2023-06-13 23:51:22.000000 vocex-0.1.7/setup.py
-drwxrwxr-x   0 cdminix   (1000) cdminix   (1000)        0 2023-06-14 00:41:03.886232 vocex-0.1.7/test/
--rw-rw-r--   0 cdminix   (1000) cdminix   (1000)       30 2023-06-11 08:34:35.000000 vocex-0.1.7/test/__init__.py
--rw-rw-r--   0 cdminix   (1000) cdminix   (1000)    10149 2023-06-11 08:34:35.000000 vocex-0.1.7/test/test.py
--rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     3033 2023-06-11 08:34:35.000000 vocex-0.1.7/test/wada_snr.py
-drwxrwxr-x   0 cdminix   (1000) cdminix   (1000)        0 2023-06-14 00:41:03.886232 vocex-0.1.7/vocex/
--rw-rw-r--   0 cdminix   (1000) cdminix   (1000)    18362 2023-06-13 23:52:59.000000 vocex-0.1.7/vocex/__init__.py
--rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     3250 2023-06-13 13:05:43.000000 vocex-0.1.7/vocex/conformer_layer.py
--rw-rw-r--   0 cdminix   (1000) cdminix   (1000)    10614 2023-06-13 13:05:43.000000 vocex-0.1.7/vocex/conformer_model.py
--rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     1067 2023-06-13 13:05:43.000000 vocex-0.1.7/vocex/image_helpers.py
--rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     3559 2023-06-13 13:06:09.000000 vocex-0.1.7/vocex/onnx_stft.py
--rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     4203 2023-06-13 13:05:43.000000 vocex-0.1.7/vocex/scaler.py
--rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     3830 2023-06-13 13:05:43.000000 vocex-0.1.7/vocex/softdtw.py
--rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     3377 2023-06-13 13:05:43.000000 vocex-0.1.7/vocex/transformer.py
--rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     1756 2023-06-13 13:05:43.000000 vocex-0.1.7/vocex/utils.py
-drwxrwxr-x   0 cdminix   (1000) cdminix   (1000)        0 2023-06-14 00:41:03.886232 vocex-0.1.7/vocex.egg-info/
--rw-rw-r--   0 cdminix   (1000) cdminix   (1000)      227 2023-06-14 00:41:03.000000 vocex-0.1.7/vocex.egg-info/PKG-INFO
--rw-rw-r--   0 cdminix   (1000) cdminix   (1000)      388 2023-06-14 00:41:03.000000 vocex-0.1.7/vocex.egg-info/SOURCES.txt
--rw-rw-r--   0 cdminix   (1000) cdminix   (1000)        1 2023-06-14 00:41:03.000000 vocex-0.1.7/vocex.egg-info/dependency_links.txt
--rw-rw-r--   0 cdminix   (1000) cdminix   (1000)       60 2023-06-14 00:41:03.000000 vocex-0.1.7/vocex.egg-info/requires.txt
--rw-rw-r--   0 cdminix   (1000) cdminix   (1000)       11 2023-06-14 00:41:03.000000 vocex-0.1.7/vocex.egg-info/top_level.txt
+drwxrwxr-x   0 cdminix   (1000) cdminix   (1000)        0 2023-06-15 10:02:14.581992 vocex-0.1.8/
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)      227 2023-06-15 10:02:14.581992 vocex-0.1.8/PKG-INFO
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     1621 2023-06-15 10:01:24.000000 vocex-0.1.8/README.md
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)       38 2023-06-15 10:02:14.581992 vocex-0.1.8/setup.cfg
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)      501 2023-06-15 09:44:12.000000 vocex-0.1.8/setup.py
+drwxrwxr-x   0 cdminix   (1000) cdminix   (1000)        0 2023-06-15 10:02:14.577992 vocex-0.1.8/test/
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)       30 2023-06-11 08:34:35.000000 vocex-0.1.8/test/__init__.py
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)    10149 2023-06-11 08:34:35.000000 vocex-0.1.8/test/test.py
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     3033 2023-06-11 08:34:35.000000 vocex-0.1.8/test/wada_snr.py
+drwxrwxr-x   0 cdminix   (1000) cdminix   (1000)        0 2023-06-15 10:02:14.581992 vocex-0.1.8/vocex/
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)    19776 2023-06-15 09:46:03.000000 vocex-0.1.8/vocex/__init__.py
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     3250 2023-06-13 13:05:43.000000 vocex-0.1.8/vocex/conformer_layer.py
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)    10614 2023-06-13 13:05:43.000000 vocex-0.1.8/vocex/conformer_model.py
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     1067 2023-06-13 13:05:43.000000 vocex-0.1.8/vocex/image_helpers.py
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     3559 2023-06-13 13:06:09.000000 vocex-0.1.8/vocex/onnx_stft.py
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     4203 2023-06-13 13:05:43.000000 vocex-0.1.8/vocex/scaler.py
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     3830 2023-06-13 13:05:43.000000 vocex-0.1.8/vocex/softdtw.py
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     3377 2023-06-13 13:05:43.000000 vocex-0.1.8/vocex/transformer.py
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     1756 2023-06-13 13:05:43.000000 vocex-0.1.8/vocex/utils.py
+drwxrwxr-x   0 cdminix   (1000) cdminix   (1000)        0 2023-06-15 10:02:14.581992 vocex-0.1.8/vocex.egg-info/
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)      227 2023-06-15 10:02:14.000000 vocex-0.1.8/vocex.egg-info/PKG-INFO
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)      388 2023-06-15 10:02:14.000000 vocex-0.1.8/vocex.egg-info/SOURCES.txt
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)        1 2023-06-15 10:02:14.000000 vocex-0.1.8/vocex.egg-info/dependency_links.txt
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)       80 2023-06-15 10:02:14.000000 vocex-0.1.8/vocex.egg-info/requires.txt
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)       11 2023-06-15 10:02:14.000000 vocex-0.1.8/vocex.egg-info/top_level.txt
```

### Comparing `vocex-0.1.7/test/test.py` & `vocex-0.1.8/test/test.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.7/test/wada_snr.py` & `vocex-0.1.8/test/wada_snr.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.7/vocex/__init__.py` & `vocex-0.1.8/vocex/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import gzip
 
 import torch
 import torchaudio.transforms as T
 from librosa.filters import mel as librosa_mel
 import numpy as np
 from torch import nn
+from transformers.utils.hub import cached_file
+from pathlib import Path
+import requests
+import warnings
 
 from .conformer_model import VocexModel
 from .image_helpers import QuantizeToGivenPalette, transformYIQ2RGB
 from .onnx_stft import TacotronSTFT
 
 class Vocex():
     """ 
@@ -17,19 +21,42 @@
     """
 
     @staticmethod
     def _drc(x, C=1, clip_val=1e-7):
         return torch.log(torch.clamp(x, min=clip_val) * C)
 
     @staticmethod
-    def from_pretrained(model_file, compressed=True, for_onnx=False, **postprocess_kwargs):
+    def from_pretrained(model, compressed=True, for_onnx=False, fp16=True, **postprocess_kwargs):
         """ 
         Load a pretrained model from a given .pt file.
         Also accepts huggingface model names.
         """
+        if isinstance(model, str):
+            if Path(model).is_file():
+                model_file = model
+            elif Path(model).is_dir():
+                if fp16:
+                    model_file = Path(model) / "checkpoint_half.ckpt"
+                else:
+                    model_file = Path(model) / "checkpoint_full.ckpt"
+            elif model.startswith("https://") or model.startswith("http://"):
+                # download from given url (github release, but not huggingface model hub)
+                # use requests to download and save to temporary file
+                # we are not using cached_file here, because it does not work with github releases
+                r = requests.get(model)
+                model_file = Path("/tmp") / Path(model).name
+                with open(model_file, "wb") as f:
+                    f.write(r.content)
+            else:
+                # download from huggingface model hub
+                if fp16:
+                    model_file = cached_file(model, "checkpoint_half.ckpt")
+                else:
+                    model_file = cached_file(model, "checkpoint_full.ckpt")
+
         if compressed:
             # decompress
             with gzip.open(model_file, "rb") as f:
                 checkpoint = torch.load(f)
         else:
             checkpoint = torch.load(model_file)
         model_args = checkpoint["model_args"]
@@ -221,15 +248,18 @@
                 print("WARNING: measure is too short, padding with zeros")
             else:
                 measure = torch.nn.functional.pad(measure, (convolution_window_size // 2, convolution_window_size // 2), mode="reflect")
             if measure.ndim == 1:
                 # add batch dimension if necessary
                 measure = measure.unsqueeze(0)
             if measure.shape[0] == 1:
-                measure = torch.nn.functional.conv1d(measure, window, padding="same")
+                with warnings.catch_warnings():
+                    # ignore warning about conv1d being deprecated
+                    warnings.simplefilter("ignore")
+                    measure = torch.nn.functional.conv1d(measure, window, padding="same")
             else:
                 measure = torch.stack([torch.nn.functional.conv1d(m.unsqueeze(0), window, padding="same") for m in measure]).squeeze(1)
             # remove padding
             measure = measure[:, convolution_window_size // 2:-convolution_window_size // 2]
         if normalize:
             # normalize
             measure = measure / measure.abs().max(dim=-1, keepdim=True)[0]
```

### Comparing `vocex-0.1.7/vocex/conformer_layer.py` & `vocex-0.1.8/vocex/conformer_layer.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.7/vocex/conformer_model.py` & `vocex-0.1.8/vocex/conformer_model.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.7/vocex/image_helpers.py` & `vocex-0.1.8/vocex/image_helpers.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.7/vocex/onnx_stft.py` & `vocex-0.1.8/vocex/onnx_stft.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.7/vocex/scaler.py` & `vocex-0.1.8/vocex/scaler.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.7/vocex/softdtw.py` & `vocex-0.1.8/vocex/softdtw.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.7/vocex/transformer.py` & `vocex-0.1.8/vocex/transformer.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.7/vocex/utils.py` & `vocex-0.1.8/vocex/utils.py`

 * *Files identical despite different names*

