# Comparing `tmp/spanda-0.0.8.tar.gz` & `tmp/spanda-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spanda-0.0.8.tar", last modified: Wed Mar 29 19:52:04 2023, max compression
+gzip compressed data, was "spanda-0.0.9.tar", last modified: Thu May  4 17:02:50 2023, max compression
```

## Comparing `spanda-0.0.8.tar` & `spanda-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 franckalbinet   (501) staff       (20)        0 2023-03-29 19:52:04.562995 spanda-0.0.8/
--rw-rw-r--   0 franckalbinet   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 spanda-0.0.8/LICENSE
--rw-rw-r--   0 franckalbinet   (501) staff       (20)      111 2022-09-05 16:31:43.000000 spanda-0.0.8/MANIFEST.in
--rw-r--r--   0 franckalbinet   (501) staff       (20)     1132 2023-03-29 19:52:04.562814 spanda-0.0.8/PKG-INFO
--rw-r--r--   0 franckalbinet   (501) staff       (20)      297 2022-10-12 14:12:40.000000 spanda-0.0.8/README.md
--rw-r--r--   0 franckalbinet   (501) staff       (20)      949 2023-03-29 19:44:59.000000 spanda-0.0.8/settings.ini
--rw-r--r--   0 franckalbinet   (501) staff       (20)       38 2023-03-29 19:52:04.563049 spanda-0.0.8/setup.cfg
--rw-rw-r--   0 franckalbinet   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 spanda-0.0.8/setup.py
-drwxr-xr-x   0 franckalbinet   (501) staff       (20)        0 2023-03-29 19:52:04.560524 spanda-0.0.8/spanda/
--rw-r--r--   0 franckalbinet   (501) staff       (20)       22 2023-03-29 19:45:00.000000 spanda-0.0.8/spanda/__init__.py
--rw-r--r--   0 franckalbinet   (501) staff       (20)     9024 2023-03-29 19:45:00.000000 spanda-0.0.8/spanda/_modidx.py
--rw-r--r--   0 franckalbinet   (501) staff       (20)     2206 2023-03-19 18:03:36.000000 spanda-0.0.8/spanda/_nbdev.py
-drwxr-xr-x   0 franckalbinet   (501) staff       (20)        0 2023-03-29 19:52:04.561746 spanda-0.0.8/spanda/data/
--rw-r--r--   0 franckalbinet   (501) staff       (20)        0 2023-03-29 19:45:00.000000 spanda-0.0.8/spanda/data/__init__.py
-drwxr-xr-x   0 franckalbinet   (501) staff       (20)        0 2023-03-29 19:52:04.562545 spanda-0.0.8/spanda/data/external/
--rw-r--r--   0 franckalbinet   (501) staff       (20)        0 2023-03-29 19:45:00.000000 spanda-0.0.8/spanda/data/external/__init__.py
--rw-r--r--   0 franckalbinet   (501) staff       (20)     3049 2023-03-29 19:44:59.000000 spanda-0.0.8/spanda/data/external/kssl.py
--rw-r--r--   0 franckalbinet   (501) staff       (20)      365 2023-03-29 19:44:59.000000 spanda-0.0.8/spanda/data/external/lucas.py
--rw-r--r--   0 franckalbinet   (501) staff       (20)     4175 2023-03-29 19:44:59.000000 spanda-0.0.8/spanda/data/external/wcrc.py
--rw-r--r--   0 franckalbinet   (501) staff       (20)     5427 2023-03-29 19:44:59.000000 spanda-0.0.8/spanda/data/transforms.py
--rw-r--r--   0 franckalbinet   (501) staff       (20)     2060 2023-03-29 19:44:59.000000 spanda-0.0.8/spanda/readers.py
--rw-r--r--   0 franckalbinet   (501) staff       (20)      929 2023-03-29 19:44:59.000000 spanda-0.0.8/spanda/sig.py
--rw-r--r--   0 franckalbinet   (501) staff       (20)      630 2023-03-29 19:44:59.000000 spanda-0.0.8/spanda/utils.py
-drwxr-xr-x   0 franckalbinet   (501) staff       (20)        0 2023-03-29 19:52:04.561571 spanda-0.0.8/spanda.egg-info/
--rw-r--r--   0 franckalbinet   (501) staff       (20)     1132 2023-03-29 19:52:04.000000 spanda-0.0.8/spanda.egg-info/PKG-INFO
--rw-r--r--   0 franckalbinet   (501) staff       (20)      535 2023-03-29 19:52:04.000000 spanda-0.0.8/spanda.egg-info/SOURCES.txt
--rw-r--r--   0 franckalbinet   (501) staff       (20)        1 2023-03-29 19:52:04.000000 spanda-0.0.8/spanda.egg-info/dependency_links.txt
--rw-r--r--   0 franckalbinet   (501) staff       (20)       34 2023-03-29 19:52:04.000000 spanda-0.0.8/spanda.egg-info/entry_points.txt
--rw-r--r--   0 franckalbinet   (501) staff       (20)        1 2022-10-13 08:35:42.000000 spanda-0.0.8/spanda.egg-info/not-zip-safe
--rw-r--r--   0 franckalbinet   (501) staff       (20)       72 2023-03-29 19:52:04.000000 spanda-0.0.8/spanda.egg-info/requires.txt
--rw-r--r--   0 franckalbinet   (501) staff       (20)        7 2023-03-29 19:52:04.000000 spanda-0.0.8/spanda.egg-info/top_level.txt
+drwxr-xr-x   0 franckalbinet   (501) staff       (20)        0 2023-05-04 17:02:50.361291 spanda-0.0.9/
+-rw-rw-r--   0 franckalbinet   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 spanda-0.0.9/LICENSE
+-rw-rw-r--   0 franckalbinet   (501) staff       (20)      111 2022-09-05 16:31:43.000000 spanda-0.0.9/MANIFEST.in
+-rw-r--r--   0 franckalbinet   (501) staff       (20)     1132 2023-05-04 17:02:50.361150 spanda-0.0.9/PKG-INFO
+-rw-r--r--   0 franckalbinet   (501) staff       (20)      297 2022-10-12 14:12:40.000000 spanda-0.0.9/README.md
+-rw-r--r--   0 franckalbinet   (501) staff       (20)      954 2023-05-04 17:02:45.000000 spanda-0.0.9/settings.ini
+-rw-r--r--   0 franckalbinet   (501) staff       (20)       38 2023-05-04 17:02:50.361342 spanda-0.0.9/setup.cfg
+-rw-rw-r--   0 franckalbinet   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 spanda-0.0.9/setup.py
+drwxr-xr-x   0 franckalbinet   (501) staff       (20)        0 2023-05-04 17:02:50.359416 spanda-0.0.9/spanda/
+-rw-r--r--   0 franckalbinet   (501) staff       (20)       22 2023-05-04 17:02:45.000000 spanda-0.0.9/spanda/__init__.py
+-rw-r--r--   0 franckalbinet   (501) staff       (20)    10510 2023-05-04 17:02:45.000000 spanda-0.0.9/spanda/_modidx.py
+-rw-r--r--   0 franckalbinet   (501) staff       (20)     2206 2023-03-19 18:03:36.000000 spanda-0.0.9/spanda/_nbdev.py
+drwxr-xr-x   0 franckalbinet   (501) staff       (20)        0 2023-05-04 17:02:50.360617 spanda-0.0.9/spanda/data/
+-rw-r--r--   0 franckalbinet   (501) staff       (20)        0 2023-05-04 17:02:45.000000 spanda-0.0.9/spanda/data/__init__.py
+drwxr-xr-x   0 franckalbinet   (501) staff       (20)        0 2023-05-04 17:02:50.360992 spanda-0.0.9/spanda/data/external/
+-rw-r--r--   0 franckalbinet   (501) staff       (20)        0 2023-05-04 17:02:45.000000 spanda-0.0.9/spanda/data/external/__init__.py
+-rw-r--r--   0 franckalbinet   (501) staff       (20)     3049 2023-05-04 17:02:45.000000 spanda-0.0.9/spanda/data/external/kssl.py
+-rw-r--r--   0 franckalbinet   (501) staff       (20)      365 2023-05-04 17:02:45.000000 spanda-0.0.9/spanda/data/external/lucas.py
+-rw-r--r--   0 franckalbinet   (501) staff       (20)     4175 2023-05-04 17:02:45.000000 spanda-0.0.9/spanda/data/external/wcrc.py
+-rw-r--r--   0 franckalbinet   (501) staff       (20)     6224 2023-05-04 17:02:45.000000 spanda-0.0.9/spanda/data/transforms.py
+-rw-r--r--   0 franckalbinet   (501) staff       (20)     2060 2023-05-04 17:02:45.000000 spanda-0.0.9/spanda/readers.py
+-rw-r--r--   0 franckalbinet   (501) staff       (20)      929 2023-05-04 17:02:45.000000 spanda-0.0.9/spanda/sig.py
+-rw-r--r--   0 franckalbinet   (501) staff       (20)      630 2023-05-04 17:02:45.000000 spanda-0.0.9/spanda/utils.py
+drwxr-xr-x   0 franckalbinet   (501) staff       (20)        0 2023-05-04 17:02:50.360438 spanda-0.0.9/spanda.egg-info/
+-rw-r--r--   0 franckalbinet   (501) staff       (20)     1132 2023-05-04 17:02:50.000000 spanda-0.0.9/spanda.egg-info/PKG-INFO
+-rw-r--r--   0 franckalbinet   (501) staff       (20)      535 2023-05-04 17:02:50.000000 spanda-0.0.9/spanda.egg-info/SOURCES.txt
+-rw-r--r--   0 franckalbinet   (501) staff       (20)        1 2023-05-04 17:02:50.000000 spanda-0.0.9/spanda.egg-info/dependency_links.txt
+-rw-r--r--   0 franckalbinet   (501) staff       (20)       34 2023-05-04 17:02:50.000000 spanda-0.0.9/spanda.egg-info/entry_points.txt
+-rw-r--r--   0 franckalbinet   (501) staff       (20)        1 2022-10-13 08:35:42.000000 spanda-0.0.9/spanda.egg-info/not-zip-safe
+-rw-r--r--   0 franckalbinet   (501) staff       (20)       77 2023-05-04 17:02:50.000000 spanda-0.0.9/spanda.egg-info/requires.txt
+-rw-r--r--   0 franckalbinet   (501) staff       (20)        7 2023-05-04 17:02:50.000000 spanda-0.0.9/spanda.egg-info/top_level.txt
```

### Comparing `spanda-0.0.8/LICENSE` & `spanda-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spanda-0.0.8/PKG-INFO` & `spanda-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spanda
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utilities to do research in soil spectroscopy harnessing the fastai framework and mindset
 Home-page: https://github.com/franckalbinet/spanda
 Author: Franck Albinet
 Author-email: franckalbinet@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `spanda-0.0.8/settings.ini` & `spanda-0.0.9/settings.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = spanda
 lib_name = spanda
-version = 0.0.8
+version = 0.0.9
 min_python = 3.7
 license = apache2
 doc_path = _docs
 lib_path = spanda
 nbs_path = nbs
 recursive = True
 tst_flags = notest
@@ -21,15 +21,15 @@
 author_email = franckalbinet@gmail.com
 copyright = 2022 onwards, Franck Albinet
 description = Utilities to do research in soil spectroscopy harnessing the fastai framework and mindset
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = franckalbinet
-requirements = fastai pandas matplotlib brukeropusreader openpyxl kennard-stone
+requirements = fastai pandas matplotlib brukeropusreader openpyxl kennard-stone timm
 host = github
 black_formatting = False
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
```

### Comparing `spanda-0.0.8/setup.py` & `spanda-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `spanda-0.0.8/spanda/_modidx.py` & `spanda-0.0.9/spanda/_modidx.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,21 @@
                                         'spanda.data.transforms.AvgTfm.encodes': ( 'data.transforms.html#avgtfm.encodes',
                                                                                    'spanda/data/transforms.py'),
                                         'spanda.data.transforms.DerivTfm': ('data.transforms.html#derivtfm', 'spanda/data/transforms.py'),
                                         'spanda.data.transforms.DerivTfm.__init__': ( 'data.transforms.html#derivtfm.__init__',
                                                                                       'spanda/data/transforms.py'),
                                         'spanda.data.transforms.DerivTfm.encodes': ( 'data.transforms.html#derivtfm.encodes',
                                                                                      'spanda/data/transforms.py'),
+                                        'spanda.data.transforms.GADFTfm': ('data.transforms.html#gadftfm', 'spanda/data/transforms.py'),
+                                        'spanda.data.transforms.GADFTfm.__init__': ( 'data.transforms.html#gadftfm.__init__',
+                                                                                     'spanda/data/transforms.py'),
+                                        'spanda.data.transforms.GADFTfm.encodes': ( 'data.transforms.html#gadftfm.encodes',
+                                                                                    'spanda/data/transforms.py'),
+                                        'spanda.data.transforms.GADFTfm.rescale': ( 'data.transforms.html#gadftfm.rescale',
+                                                                                    'spanda/data/transforms.py'),
                                         'spanda.data.transforms.LogTfm': ('data.transforms.html#logtfm', 'spanda/data/transforms.py'),
                                         'spanda.data.transforms.LogTfm.encodes': ( 'data.transforms.html#logtfm.encodes',
                                                                                    'spanda/data/transforms.py'),
                                         'spanda.data.transforms.NormalizeTfm': ( 'data.transforms.html#normalizetfm',
                                                                                  'spanda/data/transforms.py'),
                                         'spanda.data.transforms.NormalizeTfm.__init__': ( 'data.transforms.html#normalizetfm.__init__',
                                                                                           'spanda/data/transforms.py'),
@@ -46,14 +53,19 @@
                                                                                          'spanda/data/transforms.py'),
                                         'spanda.data.transforms.RandWAvgTfm': ( 'data.transforms.html#randwavgtfm',
                                                                                 'spanda/data/transforms.py'),
                                         'spanda.data.transforms.RandWAvgTfm._weights': ( 'data.transforms.html#randwavgtfm._weights',
                                                                                          'spanda/data/transforms.py'),
                                         'spanda.data.transforms.RandWAvgTfm.encodes': ( 'data.transforms.html#randwavgtfm.encodes',
                                                                                         'spanda/data/transforms.py'),
+                                        'spanda.data.transforms.ResizeTfm': ('data.transforms.html#resizetfm', 'spanda/data/transforms.py'),
+                                        'spanda.data.transforms.ResizeTfm.__init__': ( 'data.transforms.html#resizetfm.__init__',
+                                                                                       'spanda/data/transforms.py'),
+                                        'spanda.data.transforms.ResizeTfm.encodes': ( 'data.transforms.html#resizetfm.encodes',
+                                                                                      'spanda/data/transforms.py'),
                                         'spanda.data.transforms.SNVTfm': ('data.transforms.html#snvtfm', 'spanda/data/transforms.py'),
                                         'spanda.data.transforms.SNVTfm.encodes': ( 'data.transforms.html#snvtfm.encodes',
                                                                                    'spanda/data/transforms.py'),
                                         'spanda.data.transforms.Spectra': ('data.transforms.html#spectra', 'spanda/data/transforms.py'),
                                         'spanda.data.transforms.Spectra.reset': ( 'data.transforms.html#spectra.reset',
                                                                                   'spanda/data/transforms.py'),
                                         'spanda.data.transforms.Spectra.show': ( 'data.transforms.html#spectra.show',
```

### Comparing `spanda-0.0.8/spanda/_nbdev.py` & `spanda-0.0.9/spanda/_nbdev.py`

 * *Files identical despite different names*

### Comparing `spanda-0.0.8/spanda/data/external/kssl.py` & `spanda-0.0.9/spanda/data/external/kssl.py`

 * *Files identical despite different names*

### Comparing `spanda-0.0.8/spanda/data/external/wcrc.py` & `spanda-0.0.9/spanda/data/external/wcrc.py`

 * *Files identical despite different names*

### Comparing `spanda-0.0.8/spanda/data/transforms.py` & `spanda-0.0.9/spanda/data/transforms.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 # %% ../../nbs/04_data.transforms.ipynb 3
 from __future__ import annotations
 from fastai.vision.all import *
 from fastai.data.all import *
 from fastcore.basics import patch
 from pathlib import Path
 import pandas as pd
+import torchvision.transforms as T
+
 from scipy.signal import savgol_filter
 from tqdm import tqdm
 
 # %% auto 0
 __all__ = ['Spectra', 'SpectraTfm', 'ToAbsorbanceTfm', 'SpectraBlock', 'RandWAvgTfm', 'AvgTfm', 'SNVTfm', 'NormalizeTfm',
-           'TrimTfm', 'DerivTfm', 'Analytes', 'AnalytesTfm', 'AnalytesBlock', 'LogTfm']
+           'TrimTfm', 'DerivTfm', 'GADFTfm', 'ResizeTfm', 'Analytes', 'AnalytesTfm', 'AnalytesBlock', 'LogTfm']
 
 # %% ../../nbs/04_data.transforms.ipynb 7
 class Spectra(Tensor):
     "A 'showable' spectra class subclassing torch.Tensor"
     domain = domain_name = light = None
         
     def show(self, ctx=None, wn=np.arange(4000, 600, -2), figsize=(8,2), **kwargs):
@@ -121,36 +123,62 @@
     def encodes(self, 
                 x:Spectra
                ):
         x = savgol_filter(x.detach().numpy(), 
                           self.window_length, self.polyorder, self.deriv)
         return Spectra(torch.Tensor(x))
 
-# %% ../../nbs/04_data.transforms.ipynb 20
+# %% ../../nbs/04_data.transforms.ipynb 18
+class GADFTfm(Transform):
+    def __init__(self, neg=True):
+        self.neg = neg
+        
+    def rescale(self, x):
+        m, M = x.min(), x.max()
+        return ((x - M) + (x - m)) / (M - m) if self.neg else (x - m) / (M - m)
+
+    def encodes(self, 
+                x:Spectra
+               ):
+        X, I = self.rescale(x), torch.ones((1, x.shape[1]))
+        K = torch.sqrt(I - torch.square(X))
+        return K.t()@X - X.t()@K
+
+# %% ../../nbs/04_data.transforms.ipynb 19
+class ResizeTfm(Transform):
+    def __init__(self, size=256):
+        self.size = size
+        
+    def encodes(self, 
+                x:Spectra
+               ):
+        return T.Resize(self.size)(x.unsqueeze(0))
+
+# %% ../../nbs/04_data.transforms.ipynb 24
 class Analytes(Tensor, ShowTitle):
     def __init__(self, ys):
         self.ys = ys
         # Ideally, w'd like to show (idx: 1234 | 725: 0.123 | 433: 0.7) decoded
 
-# %% ../../nbs/04_data.transforms.ipynb 21
+# %% ../../nbs/04_data.transforms.ipynb 25
 class AnalytesTfm(Transform):
     "Transform a folder path into a tensor of soil analyte(s) measurement"
     def __init__(self, 
                  analytes:list|None=None):
         self.analytes = analytes
         
     def encodes(self,
                 o:Path # Path to directory containing both spectra and analyte(s) measurement
                ):
         df = pd.read_csv(o)
         if self.analytes:
             df = df[df.analyte.isin(self.analytes)]
         return Analytes(df['value'].values)
 
-# %% ../../nbs/04_data.transforms.ipynb 23
+# %% ../../nbs/04_data.transforms.ipynb 27
 def AnalytesBlock(analytes):
     return TransformBlock(type_tfms=AnalytesTfm(analytes))
 
-# %% ../../nbs/04_data.transforms.ipynb 24
+# %% ../../nbs/04_data.transforms.ipynb 28
 class LogTfm(Transform):
     def encodes(self, ys:Analytes):
         return torch.log10(ys)
```

### Comparing `spanda-0.0.8/spanda/readers.py` & `spanda-0.0.9/spanda/readers.py`

 * *Files identical despite different names*

### Comparing `spanda-0.0.8/spanda/sig.py` & `spanda-0.0.9/spanda/sig.py`

 * *Files identical despite different names*

### Comparing `spanda-0.0.8/spanda/utils.py` & `spanda-0.0.9/spanda/utils.py`

 * *Files identical despite different names*

### Comparing `spanda-0.0.8/spanda.egg-info/PKG-INFO` & `spanda-0.0.9/spanda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spanda
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utilities to do research in soil spectroscopy harnessing the fastai framework and mindset
 Home-page: https://github.com/franckalbinet/spanda
 Author: Franck Albinet
 Author-email: franckalbinet@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `spanda-0.0.8/spanda.egg-info/SOURCES.txt` & `spanda-0.0.9/spanda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

