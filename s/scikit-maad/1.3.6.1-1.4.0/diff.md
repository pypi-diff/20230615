# Comparing `tmp/scikit-maad-1.3.6.1.tar.gz` & `tmp/scikit_maad-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-maad-1.3.6.1.tar", last modified: Thu Oct 20 20:03:28 2022, max compression
+gzip compressed data, was "scikit_maad-1.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `scikit-maad-1.3.6.1.tar` & `scikit_maad-1.4.0.tar`

### file list

```diff
@@ -1,47 +1,41 @@
-drwxrwxr-x   0 haupert   (1000) users      (100)        0 2022-10-20 20:03:28.453853 scikit-maad-1.3.6.1/
--rwxrwxr-x   0 haupert   (1000) users      (100)     1505 2021-03-01 09:09:10.000000 scikit-maad-1.3.6.1/LICENSE
--rwxrwxr-x   0 haupert   (1000) users      (100)       15 2020-05-26 10:28:24.000000 scikit-maad-1.3.6.1/MANIFEST.in
--rwxrwxr-x   0 haupert   (1000) users      (100)     5549 2022-10-20 20:03:28.453594 scikit-maad-1.3.6.1/PKG-INFO
--rwxrwxr-x   0 haupert   (1000) users      (100)     4488 2021-11-24 15:13:48.000000 scikit-maad-1.3.6.1/README.md
-drwxrwxr-x   0 haupert   (1000) users      (100)        0 2022-10-20 20:03:28.431721 scikit-maad-1.3.6.1/maad/
--rwxrwxr-x   0 haupert   (1000) users      (100)     1167 2021-02-26 08:08:18.000000 scikit-maad-1.3.6.1/maad/__init__.py
-drwxrwxr-x   0 haupert   (1000) users      (100)        0 2022-10-20 20:03:28.436666 scikit-maad-1.3.6.1/maad/features/
--rwxrwxr-x   0 haupert   (1000) users      (100)     4626 2021-01-31 22:36:49.000000 scikit-maad-1.3.6.1/maad/features/__init__.py
--rwxrwxr-x   0 haupert   (1000) users      (100)   126259 2022-07-04 20:37:25.000000 scikit-maad-1.3.6.1/maad/features/alpha_indices.py
--rwxrwxr-x   0 haupert   (1000) users      (100)    40562 2021-07-01 10:14:39.000000 scikit-maad-1.3.6.1/maad/features/shape.py
--rwxrwxr-x   0 haupert   (1000) users      (100)     2226 2021-04-20 08:15:56.000000 scikit-maad-1.3.6.1/maad/features/spectral.py
--rwxrwxr-x   0 haupert   (1000) users      (100)     2648 2021-05-11 22:06:58.000000 scikit-maad-1.3.6.1/maad/features/temporal.py
-drwxrwxr-x   0 haupert   (1000) users      (100)        0 2022-10-20 20:03:28.438537 scikit-maad-1.3.6.1/maad/rois/
--rwxrwxr-x   0 haupert   (1000) users      (100)      748 2021-01-25 08:28:02.000000 scikit-maad-1.3.6.1/maad/rois/__init__.py
--rwxrwxr-x   0 haupert   (1000) users      (100)     7913 2022-02-17 17:11:23.000000 scikit-maad-1.3.6.1/maad/rois/rois_1d.py
--rwxrwxr-x   0 haupert   (1000) users      (100)    29981 2022-04-28 12:31:17.000000 scikit-maad-1.3.6.1/maad/rois/rois_2d.py
-drwxrwxr-x   0 haupert   (1000) users      (100)        0 2022-10-20 20:03:28.444150 scikit-maad-1.3.6.1/maad/sound/
--rwxrwxr-x   0 haupert   (1000) users      (100)     2946 2022-03-18 13:13:44.000000 scikit-maad-1.3.6.1/maad/sound/__init__.py
--rwxrwxr-x   0 haupert   (1000) users      (100)    15666 2021-03-30 20:25:09.000000 scikit-maad-1.3.6.1/maad/sound/filter.py
--rwxrwxr-x   0 haupert   (1000) users      (100)    17032 2021-11-24 15:13:48.000000 scikit-maad-1.3.6.1/maad/sound/input_output.py
--rwxrwxr-x   0 haupert   (1000) users      (100)     6185 2022-05-10 15:38:02.000000 scikit-maad-1.3.6.1/maad/sound/metrics.py
--rwxrwxr-x   0 haupert   (1000) users      (100)    40007 2021-07-01 09:55:22.000000 scikit-maad-1.3.6.1/maad/sound/spectral_subtraction.py
--rwxrwxr-x   0 haupert   (1000) users      (100)    18299 2022-07-04 19:23:45.000000 scikit-maad-1.3.6.1/maad/sound/spectro_func.py
--rwxrwxr-x   0 haupert   (1000) users      (100)    17776 2022-03-18 13:13:44.000000 scikit-maad-1.3.6.1/maad/sound/transform.py
--rwxrwxr-x   0 haupert   (1000) users      (100)     2665 2021-05-11 22:06:58.000000 scikit-maad-1.3.6.1/maad/sound/trim_func.py
-drwxrwxr-x   0 haupert   (1000) users      (100)        0 2022-10-20 20:03:28.446000 scikit-maad-1.3.6.1/maad/spl/
--rwxrwxr-x   0 haupert   (1000) users      (100)     2017 2022-02-18 09:27:03.000000 scikit-maad-1.3.6.1/maad/spl/__init__.py
--rwxrwxr-x   0 haupert   (1000) users      (100)    33132 2022-02-17 17:11:23.000000 scikit-maad-1.3.6.1/maad/spl/active_space.py
--rwxrwxr-x   0 haupert   (1000) users      (100)    22378 2022-01-10 22:27:40.000000 scikit-maad-1.3.6.1/maad/spl/conversion_SPL.py
-drwxrwxr-x   0 haupert   (1000) users      (100)        0 2022-10-20 20:03:28.450554 scikit-maad-1.3.6.1/maad/util/
--rwxrwxr-x   0 haupert   (1000) users      (100)     5364 2022-04-28 10:29:49.000000 scikit-maad-1.3.6.1/maad/util/__init__.py
--rwxrwxr-x   0 haupert   (1000) users      (100)     9743 2022-04-28 14:34:22.000000 scikit-maad-1.3.6.1/maad/util/audio_metadata_utilities.py
--rwxrwxr-x   0 haupert   (1000) users      (100)    15111 2022-07-04 12:29:01.000000 scikit-maad-1.3.6.1/maad/util/math_func.py
--rwxrwxr-x   0 haupert   (1000) users      (100)    35297 2022-05-11 00:16:53.000000 scikit-maad-1.3.6.1/maad/util/miscellaneous.py
--rwxrwxr-x   0 haupert   (1000) users      (100)    15773 2022-10-14 12:24:38.000000 scikit-maad-1.3.6.1/maad/util/parser.py
--rwxrwxr-x   0 haupert   (1000) users      (100)    68143 2022-06-28 08:16:10.000000 scikit-maad-1.3.6.1/maad/util/visualization.py
--rwxrwxr-x   0 haupert   (1000) users      (100)    17215 2022-10-14 14:59:30.000000 scikit-maad-1.3.6.1/maad/util/xeno_canto.py
--rwxrwxr-x   0 haupert   (1000) users      (100)       89 2022-10-20 20:03:17.000000 scikit-maad-1.3.6.1/maad/version.py
-drwxrwxr-x   0 haupert   (1000) users      (100)        0 2022-10-20 20:03:28.453016 scikit-maad-1.3.6.1/scikit_maad.egg-info/
--rwxrwxr-x   0 haupert   (1000) users      (100)     5549 2022-10-20 20:03:28.000000 scikit-maad-1.3.6.1/scikit_maad.egg-info/PKG-INFO
--rwxrwxr-x   0 haupert   (1000) users      (100)      898 2022-10-20 20:03:28.000000 scikit-maad-1.3.6.1/scikit_maad.egg-info/SOURCES.txt
--rwxrwxr-x   0 haupert   (1000) users      (100)        1 2022-10-20 20:03:28.000000 scikit-maad-1.3.6.1/scikit_maad.egg-info/dependency_links.txt
--rwxrwxr-x   0 haupert   (1000) users      (100)       83 2022-10-20 20:03:28.000000 scikit-maad-1.3.6.1/scikit_maad.egg-info/requires.txt
--rwxrwxr-x   0 haupert   (1000) users      (100)        5 2022-10-20 20:03:28.000000 scikit-maad-1.3.6.1/scikit_maad.egg-info/top_level.txt
--rwxrwxr-x   0 haupert   (1000) users      (100)       38 2022-10-20 20:03:28.453946 scikit-maad-1.3.6.1/setup.cfg
--rwxrwxr-x   0 haupert   (1000) users      (100)     2644 2022-10-20 20:00:43.000000 scikit-maad-1.3.6.1/setup.py
+-rw-r--r--   0        0        0     1258 2023-02-25 03:24:32.000000 scikit_maad-1.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      609 2023-02-25 03:24:32.000000 scikit_maad-1.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1462 2023-05-18 13:51:01.000000 scikit_maad-1.4.0/.github/workflows/ci-cd.yml
+-rw-r--r--   0        0        0     1494 2023-02-25 03:24:47.000000 scikit_maad-1.4.0/.github/workflows/python-compatibility.yml
+-rw-r--r--   0        0        0     1734 2023-06-15 15:11:33.000000 scikit_maad-1.4.0/.gitignore
+-rw-r--r--   0        0        0      591 2023-02-25 03:24:32.000000 scikit_maad-1.4.0/CITATION.bib
+-rw-r--r--   0        0        0     5223 2023-02-25 03:24:32.000000 scikit_maad-1.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3674 2023-03-09 19:24:07.000000 scikit_maad-1.4.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1505 2021-02-27 02:48:38.000000 scikit_maad-1.4.0/LICENSE
+-rw-r--r--   0        0        0     7158 2023-06-15 15:07:40.000000 scikit_maad-1.4.0/README.md
+-rw-r--r--   0        0        0     1177 2023-03-09 19:24:07.000000 scikit_maad-1.4.0/maad/__init__.py
+-rw-r--r--   0        0        0     5337 2023-03-15 19:23:57.000000 scikit_maad-1.4.0/maad/features/__init__.py
+-rw-r--r--   0        0        0   129626 2023-06-15 15:07:40.000000 scikit_maad-1.4.0/maad/features/alpha_indices.py
+-rw-r--r--   0        0        0    41647 2023-06-15 15:07:40.000000 scikit_maad-1.4.0/maad/features/shape.py
+-rwxr-xr-x   0        0        0    13928 2023-06-15 15:07:40.000000 scikit_maad-1.4.0/maad/features/spectral.py
+-rw-r--r--   0        0        0    13577 2023-06-15 15:07:40.000000 scikit_maad-1.4.0/maad/features/temporal.py
+-rw-r--r--   0        0        0      895 2023-02-25 03:24:33.000000 scikit_maad-1.4.0/maad/rois/__init__.py
+-rw-r--r--   0        0        0     8114 2023-06-15 15:10:50.000000 scikit_maad-1.4.0/maad/rois/rois_1d.py
+-rw-r--r--   0        0        0    30833 2023-06-15 15:07:40.000000 scikit_maad-1.4.0/maad/rois/rois_2d.py
+-rw-r--r--   0        0        0     6304 2023-02-25 03:24:33.000000 scikit_maad-1.4.0/maad/rois/template_matching_func.py
+-rw-r--r--   0        0        0     2946 2022-03-04 19:33:45.000000 scikit_maad-1.4.0/maad/sound/__init__.py
+-rw-r--r--   0        0        0    16791 2023-06-15 15:07:40.000000 scikit_maad-1.4.0/maad/sound/filter.py
+-rw-r--r--   0        0        0    18024 2023-06-15 15:07:40.000000 scikit_maad-1.4.0/maad/sound/input_output.py
+-rw-r--r--   0        0        0     6185 2021-07-01 20:35:03.000000 scikit_maad-1.4.0/maad/sound/metrics.py
+-rw-r--r--   0        0        0    39987 2023-03-18 03:04:59.000000 scikit_maad-1.4.0/maad/sound/spectral_subtraction.py
+-rw-r--r--   0        0        0    18299 2022-07-27 22:52:22.000000 scikit_maad-1.4.0/maad/sound/spectro_func.py
+-rw-r--r--   0        0        0    18910 2023-05-18 21:10:58.000000 scikit_maad-1.4.0/maad/sound/transform.py
+-rw-r--r--   0        0        0     2665 2021-04-21 21:07:37.000000 scikit_maad-1.4.0/maad/sound/trim_func.py
+-rw-r--r--   0        0        0     1857 2023-03-09 19:24:07.000000 scikit_maad-1.4.0/maad/spl/__init__.py
+-rw-r--r--   0        0        0    33132 2022-02-17 20:04:47.000000 scikit_maad-1.4.0/maad/spl/active_space.py
+-rw-r--r--   0        0        0    22378 2022-01-17 13:55:42.000000 scikit_maad-1.4.0/maad/spl/conversion_SPL.py
+-rw-r--r--   0        0        0     5596 2022-11-03 17:45:28.000000 scikit_maad-1.4.0/maad/util/__init__.py
+-rw-r--r--   0        0        0     9743 2022-04-28 14:26:06.000000 scikit_maad-1.4.0/maad/util/audio_metadata_utilities.py
+-rw-r--r--   0        0        0    14953 2023-03-18 02:50:31.000000 scikit_maad-1.4.0/maad/util/math_func.py
+-rw-r--r--   0        0        0    35231 2023-04-12 13:55:24.000000 scikit_maad-1.4.0/maad/util/miscellaneous.py
+-rw-r--r--   0        0        0    15767 2022-12-26 14:21:51.000000 scikit_maad-1.4.0/maad/util/parser.py
+-rw-r--r--   0        0        0    68301 2023-06-15 15:07:40.000000 scikit_maad-1.4.0/maad/util/visualization.py
+-rw-r--r--   0        0        0    24595 2023-06-08 14:31:20.000000 scikit_maad-1.4.0/maad/util/xeno_canto.py
+-rw-r--r--   0        0        0       88 2023-06-15 15:52:53.000000 scikit_maad-1.4.0/maad/version.py
+-rw-r--r--   0        0        0     1726 2023-03-09 19:24:07.000000 scikit_maad-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8788 1970-01-01 00:00:00.000000 scikit_maad-1.4.0/PKG-INFO
```

### Comparing `scikit-maad-1.3.6.1/LICENSE` & `scikit_maad-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-maad-1.3.6.1/maad/__init__.py` & `scikit_maad-1.4.0/maad/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,12 +24,12 @@
     Load, preprocess and transform (e.g. stft) audio signals - :ref:`maad.sound`
     
 util
     Miscelaneous and useful set of tools used in the audio analysis framework - :ref:`maad.util`    
 """
 from .version import __version__
 
-from . import spl
-from . import features
-from . import rois
-from . import sound
-from . import util
+# from . import spl
+# from . import features
+# from . import rois
+# from . import sound
+# from . import util
```

### Comparing `scikit-maad-1.3.6.1/maad/features/__init__.py` & `scikit_maad-1.4.0/maad/features/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -55,36 +55,50 @@
 Temporal features
 -----------------
 .. autosummary::
     :toctree: generated/
     
     temporal_moments
     zero_crossing_rate
+    temporal_duration
+    temporal_quantile
+    all_temporal_features
     
 Spectral features
 -----------------
 .. autosummary::
     :toctree: generated/
         
     spectral_moments
+    peak_frequency
+    spectral_quantile
+    spectral_bandwidth
+    all_spectral_features
 
 """
 
 from .shape import (filter_multires,
                           filter_bank_2d_nodc,
                           opt_shape_presets,
                           shape_features,
                           shape_features_raw,
                           centroid_features,
                           all_shape_features)
 
-from .spectral import (spectral_moments)
+from .spectral import (spectral_moments,
+                       peak_frequency,
+                       spectral_quantile,
+                       spectral_bandwidth,
+                       all_spectral_features)
 
 from .temporal import (temporal_moments,
-                       zero_crossing_rate)
+                       zero_crossing_rate,
+                       temporal_duration,
+                       temporal_quantile,
+                       all_temporal_features)
 
 from .alpha_indices import (temporal_median,
                             temporal_entropy,
                             acoustic_richness_index,
                             temporal_activity,
                             temporal_events,
                             acoustic_complexity_index,
@@ -117,17 +131,24 @@
            'opt_shape_presets',
            'shape_features',
            'shape_features_raw',
            'centroid_features',
            'all_shape_features',
            # spectral
            'spectral_moments',
+           'peak_frequency',
+           'spectral_quantile',
+           'temporal_quantile',
+           'spectral_bandwidth',
+           'all_spectral_features',
            # temporal
            'temporal_moments',
            'zero_crossing_rate',
+           'temporal_duration',
+           'all_temporal_features',
            # alpha_indices
            'temporal_moments',
            'temporal_median',
            'temporal_entropy',
            'acoustic_richness_index',
            "temporal_activity",
            "temporal_events",
```

### Comparing `scikit-maad-1.3.6.1/maad/features/alpha_indices.py` & `scikit_maad-1.4.0/maad/features/alpha_indices.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,30 +15,30 @@
 # -------------------       Load modules         ---------------------------
 #***************************************************************************
 # Import external modules
 import numbers
 import numpy as np 
 from numpy import sum, log, min, max, abs, mean, median, sqrt, diff, var
 from skimage.morphology import opening
-from scipy.ndimage.morphology import binary_erosion, binary_dilation
+from scipy.ndimage import binary_erosion, binary_dilation
 from scipy.stats import rankdata
 from scipy.signal import find_peaks
 import matplotlib.pyplot as plt
 import pandas as pd # for csv
 # min value
 import sys
 _MIN_ = sys.float_info.min
 
 # Import internal modules
 from maad.util import (rle, index_bw, amplitude2dB, power2dB, dB2power, mean_dB,
-                       skewness, kurtosis, format_features, into_bins, entropy, 
-                       linear_scale, plot1d, plot2d, overlay_rois)
+                        skewness, kurtosis, format_features, into_bins, entropy, 
+                        linear_scale, plot1d, plot2d, overlay_rois)
 from maad.spl import wav2leq, psd2leq, power2dBSPL
 from maad.features import (centroid_features, zero_crossing_rate, temporal_moments, 
-                           spectral_moments)
+                        spectral_moments)
 from maad.sound import (envelope, smooth, temporal_snr, linear_to_octave, 
                         avg_amplitude_spectro, avg_power_spectro, spectral_snr, 
                         median_equalizer)
 from maad.rois import select_rois, create_mask
 
 #%%
 # =============================================================================
@@ -80,15 +80,15 @@
 
     ACTsp [Towsey] : ACTfract (proportion (fraction) of point value above the theshold)
     EVNsp [Towsey] : ACTcount (number of point value above the theshold)
     """ 
     
     ### For x to be a ndarray
     xdB = np.asarray(xdB)
-   
+
     ### compute _score
     ACTfract, ACTcount = _score(xdB, dB_threshold, axis=axis)
     ACTfract= ACTfract.tolist()
     ACTcount = ACTcount.tolist()
     ACTmean = mean_dB(xdB[xdB>dB_threshold])
     return ACTfract, ACTcount, ACTmean 
 
@@ -264,15 +264,15 @@
         Gini value
         
     References
     ----------
     Ported from ineq library in R
     """
     if sum(x) == 0:
-       G = 0 # null gini
+        G = 0 # null gini
     else:
         n = len(x)
         x.sort()
         G = sum(x * np.arange(1,n+1,1))
         G = 2 * G/sum(x) - (n + 1)
         if corr : G = G/(n - 1)
         else : G= G/n
@@ -465,21 +465,22 @@
         - "Hilbert" : estimation of the envelope from the Hilbert transform. The method is slow
     Nt : integer, optional, default is 512
         Size of each frame. The largest, the highest is the approximation.
     
     Returns
     -------
     MED: float
-       Median of the envelope 
+        Median of the envelope 
 
     Examples
     --------
+    >>> import maad
     >>> s, fs = maad.sound.load('../data/spinetail.wav')
     >>> med = maad.features.temporal_median(s)
-    >>> print(med)
+    >>> print(med) # doctest: +NORMALIZE_WHITESPACE
     0.007934564717486147
     
     """
     # Envelope
     env = envelope(s, mode=mode, Nt=Nt)
     # median
     MED = np.median(env)
@@ -503,37 +504,38 @@
     mode : str, optional, default is "fast"
         Select the mode to compute the envelope of the audio waveform.
         
         - "fast" : The sound is first divided into frames (2d) using the function _wave2timeframes(s), then the max of each frame gives a good approximation of the envelope.
         - "Hilbert" : estimation of the envelope from the Hilbert transform. The method is slow.
     Nt : integer, optional, default is 512
         Size of each frame. The largest, the highest is the approximation.
-   
+
     Returns
     -------
     Ht: float
-       Temporal entropy of the audio 
-       
+        Temporal entropy of the audio 
+    
     References
     ----------
     .. [1] Seewave : http://rug.mnhn.fr/seewave. Sueur, J., Aubin, T., & Simonis, C. (2008). Seewave, a free modular tool for sound analysis and synthesis. Bioacoustics, 18(2), 213-226. `DOI: 10.1080/09524622.2008.9753600 <https://doi.org/10.1080/09524622.2008.9753600>`_ 
     .. [2] QUT : https://github.com/QutEcoacoustics/audio-analysis. Michael Towsey, Anthony Truskinger, Mark Cottman-Fields, & Paul Roe. (2018, March 5). Ecoacoustics Audio Analysis Software v18.03.0.41 (Version v18.03.0.41). Zenodo. http://doi.org/10.5281/zenodo.1188744
     
     Notes
     -----
     The entropy of an audio signal is a measure of energy dispersion. In the temporal domain, 
     values below 0.7 indicate a brief concentration of energy (few miliseconds), while 
     values close 1 indicate low concentration of energy, no peaks, smooth and constant 
     background noise.
 
     Examples
     --------
+    >>> import maad
     >>> s, fs = maad.sound.load('../data/spinetail.wav')
     >>> Ht = maad.features.temporal_entropy (s)
-    >>> print(Ht)
+    >>> print(Ht) # doctest: +NORMALIZE_WHITESPACE
     0.7518917279549968
 
     """
     # Envelope
     env = envelope(s, mode=mode, Nt=Nt)
     # Entropy
     if compatibility == 'QUT':
@@ -568,29 +570,31 @@
     References
     ----------
     .. [1] Depraetere, M., Pavoine, S., Jiguet, F., Gasc, A., Duvail, S., & Sueur, J. (2012). Monitoring animal diversity using acoustic indices: Implementation in a temperate woodland. Ecological Indicators, 13, 46–54. `DOI: 10.1016/j.ecolind.2011.05.006 <https://doi.org/10.1016/j.ecolind.2011.05.006>`_ 
     .. [2] Seewave : http://rug.mnhn.fr/seewave. Sueur, J., Aubin, T., & Simonis, C. (2008). Seewave, a free modular tool for sound analysis and synthesis. Bioacoustics, 18(2), 213-226. `DOI: 10.1080/09524622.2008.9753600 <https://doi.org/10.1080/09524622.2008.9753600>`_ 
 
     Examples
     --------
+    >>> import maad
+
     >>> s, fs = maad.sound.load('../data/indices/S4A03895_20190522_060000.wav')
     >>> Ht_6h00 = maad.features.temporal_entropy(s)
     >>> M_6h00 = maad.features.temporal_median(s)
     
     >>> s, fs = maad.sound.load('../data/indices/S4A03895_20190522_080000.wav')
     >>> Ht_8h00= maad.features.temporal_entropy(s)
     >>> M_8h00 = maad.features.temporal_median(s)
     
     >>> s, fs = maad.sound.load('../data/indices/S4A03895_20190522_100000.wav')
     >>> Ht_10h00 = maad.features.temporal_entropy(s)
     >>> M_10h00 = maad.features.temporal_median(s)
     
-    >>> maad.features.acoustic_richness_index([Ht_6h00,Ht_8h00,Ht_10h00],
-                                              [M_6h00,M_8h00,M_10h00])
-    array([0.11111111, 0.44444444, 1.        ])
+    >>> result = maad.features.acoustic_richness_index([Ht_6h00,Ht_8h00,Ht_10h00],[M_6h00,M_8h00,M_10h00]) 
+    >>> print(result) # doctest: +NORMALIZE_WHITESPACE
+    [0.11111111 0.44444444 1.        ]
     
     """    
     if len(Ht_array) != len(M_array) : 
         print ("warning : Ht_array and M_array must have the same length")
     
     AR = rankdata(Ht_array) * rankdata(M_array) / len(Ht_array)**2
     
@@ -615,15 +619,15 @@
     ----------
     s : 1D array of floats
         audio to process (wav)
     dB_threshold : scalar, optional, default is 3dB
         data >Threshold is considered to be an activity 
     mode : str, optional, default is "fast"
         Select the mode to compute the envelope of the audio waveform
-       
+    
         - "fast" : The sound is first divided into frames (2d) using the 
             function _wave2timeframes(s), then the max of each frame gives a 
             good approximation of the envelope.
         - "Hilbert" : estimation of the envelope from the Hilbert transform. 
             The method is slow
     Nt : integer, optional, default is 512
         Size of each frame. The largest, the highest is the approximation.    
@@ -640,17 +644,18 @@
     References 
     ----------
     .. [1] Towsey, Michael (2013), Noise Removal from Waveforms and Spectrograms Derived from Natural Recordings of the Environment. Queensland University of Technology, Brisbane. https://eprints.qut.edu.au/61399/4/61399.pdf
     .. [2] QUT : https://github.com/QutEcoacoustics/audio-analysis. Michael Towsey, Anthony Truskinger, Mark Cottman-Fields, & Paul Roe. (2018, March 5). Ecoacoustics Audio Analysis Software v18.03.0.41 (Version v18.03.0.41). Zenodo. http://doi.org/10.5281/zenodo.1188744
 
     Examples
     --------
+    >>> import maad
     >>> s, fs = maad.sound.load('../data/spinetail.wav')
     >>> ACTfract, ACTcount, ACTmean = maad.features.temporal_activity (s, 6)
-    >>> print('ACTfract: %2.2f / ACTcount: %2.0f / ACTmean: %2.2f' % (ACTfract, ACTcount, ACTmean))
+    >>> print('ACTfract: %2.2f / ACTcount: %2.0f / ACTmean: %2.2f' % (ACTfract, ACTcount, ACTmean)) # doctest: +NORMALIZE_WHITESPACE
     ACTfract: 0.37 / ACTcount: 620 / ACTmean: 24.41
     
     """ 
 
     ### For wave to be a ndarray
     s = np.asarray(s) 
     
@@ -714,15 +719,15 @@
         - "Hilbert" : 
             Estimation of the envelope from the Hilbert transform. 
             The method is slow
     Nt : integer, optional, default is 512
         Size of each frame. The largest, the highest is the approximation.
     display : boolean, optional, default is False
         Display the selected events on the audio waveform
-    \*\*kwargs, optional. 
+    kwargs, optional. 
         This parameter is used by plt.plot
 
     Returns
     -------    
     EVNtFraction :scalar
         Fraction: events duration over total duration
     EVNmean: scalar
@@ -737,17 +742,18 @@
     References 
     ----------
     .. [1] Towsey, Michael (2013), Noise Removal from Waveforms and Spectrograms Derived from Natural Recordings of the Environment. Queensland University of Technology, Brisbane. https://eprints.qut.edu.au/61399/4/61399.pdf
     .. [2] QUT : https://github.com/QutEcoacoustics/audio-analysis. Michael Towsey, Anthony Truskinger, Mark Cottman-Fields, & Paul Roe. (2018, March 5). Ecoacoustics Audio Analysis Software v18.03.0.41 (Version v18.03.0.41). Zenodo. http://doi.org/10.5281/zenodo.1188744
 
     Examples
     --------
+    >>> import maad
     >>> s, fs = maad.sound.load('../data/spinetail.wav')
     >>> EVNtFract, EVNmean, EVNcount, _ = maad.features.temporal_events (s, fs, 6)
-    >>> print('EVNtFract: %2.2f / EVNmean: %2.2f / EVNcount: %2.0f' % (EVNtFract, EVNmean, EVNcount))
+    >>> print('EVNtFract: %2.2f / EVNmean: %2.2f / EVNcount: %2.0f' % (EVNtFract, EVNmean, EVNcount)) # doctest: +NORMALIZE_WHITESPACE
     EVNtFract: 0.37 / EVNmean: 0.08 / EVNcount:  5
     
     """  
     ### For wave to be a ndarray
     s = np.asarray(s) 
     
     ### envelope
@@ -799,50 +805,54 @@
     ----------
     X : 1D or 2D array
         Power Spectral/Spectrogram Density (PSD) of an audio
         Better to work with PSD (amplitude¹) than with amplitude for energy 
         conservation
     compatibility : string {'QUT', 'seewave'}, default is 'QUT'
         Select the way to compute the spectral entropy.
-           
+        
         - QUT [2]_ : entropy of P
         - seewave [1]_ : entropy of sqrt(P)   
     
     Returns
     -------
     Hf: float
-       spectral entropy of the audio 
+        spectral entropy of the audio 
     Ht_per_bin : array of floats
         temporal entropy along time axis for each frequency when P is a 
         spectrogram (2d) otherwise Ht_per_bin is empty   
-       
+    
     References
     ----------
     .. [1] Seewave : http://rug.mnhn.fr/seewave. Sueur, J., Aubin, T., & Simonis, C. (2008). Seewave, a free modular tool for sound analysis and synthesis. Bioacoustics, 18(2), 213-226. `DOI: 10.1080/09524622.2008.9753600 <https://doi.org/10.1080/09524622.2008.9753600>`_ 
     .. [2] QUT : https://github.com/QutEcoacoustics/audio-analysis. Michael Towsey, Anthony Truskinger, Mark Cottman-Fields, & Paul Roe. (2018, March 5). Ecoacoustics Audio Analysis Software v18.03.0.41 (Version v18.03.0.41). Zenodo. http://doi.org/10.5281/zenodo.1188744
-  
+
     Notes
     -----
     The spectral entropy of a signal measures the energy dispersion along frequencies. Low values 
     indicates a concentration of energy around a narrow frequency band. 
     If the DC value is not removed before processing the large peak at f=0Hz will 
     lower the entropy of the signal.
 
     Examples
     --------
+    >>> import maad
     >>> s, fs = maad.sound.load('../data/spinetail.wav')
     >>> Sxx_power,_,_,_ = maad.sound.spectrogram (s, fs)   
     >>> Hf, Ht_per_bin = maad.features.frequency_entropy(Sxx_power)
-    >>> print(Hf)
-    0.6313982665877063
-    >>> print('Length of Ht_per_bin is : %2.0f' % len(Ht_per_bin))
+    >>> print(Hf) # doctest: +NORMALIZE_WHITESPACE
+    0.631398266587706
+
+    >>> print('Length of Ht_per_bin is : %2.0f' % len(Ht_per_bin)) # doctest: +NORMALIZE_WHITESPACE
     Length of Ht_per_bin is : 512
-    >>> print(Ht_per_bin)
+    
+    print only the first ten values of the vector
+    >>> print(Ht_per_bin [0:9]) # doctest: +NORMALIZE_WHITESPACE
     [0.73458664 0.73476487 0.87981728 0.9161413  0.90153962 0.91684881
-     0.91816039 0.93453925 0.92958317 0.93763948 0.93524745 0.93736222...]
+    0.91816039 0.93453925 0.92958317]
     
     """
     # Force to be an array
     X = np.asarray(X)
     
     # test if P has 2 dimension (i.e a spectrogram Pxx)
     if X.ndim==1 :
@@ -916,17 +926,19 @@
     References
     ----------
     .. [1] Gasc, A. & al (2013). Biodiversity sampling using a global acoustic approach: contrasting sites with microendemics in New Caledonia. PloS one, 8(5), e65311. `DOI: 10.1371/journal.pone.0065311 <https://doi.org/10.1371/journal.pone.0065311>`_ 
     .. [2] Seewave : http://rug.mnhn.fr/seewave. Sueur, J., Aubin, T., & Simonis, C. (2008). Seewave, a free modular tool for sound analysis and synthesis. Bioacoustics, 18(2), 213-226. `DOI: 10.1080/09524622.2008.9753600 <https://doi.org/10.1080/09524622.2008.9753600>`_ 
     
     Examples
     --------
+    >>> import maad
     >>> s, fs = maad.sound.load('../data/cold_forest_daylight.wav')
     >>> Sxx_power, tn, fn, _ = maad.sound.spectrogram (s, fs)  
-    >>> maad.features.number_of_peaks(Sxx_power, fn, slopes=6, min_freq_dist=100, display=True) 
+    >>> maad.features.number_of_peaks(Sxx_power, fn, slopes=6, min_freq_dist=100, display=True) # doctest: +NORMALIZE_WHITESPACE
+    14
 
     """
     # Force to be an array
     X = np.asarray(X)
     
     # mean spectrum
     if X.ndim == 2 :
@@ -939,16 +951,16 @@
         S = amplitude2dB(S)
         if min_peak_val is not None :
             min_peak_val = amplitude2dB(min_peak_val)
 
     # Find peaks
     min_pix_distance = min_freq_dist/(fn[1]-fn[0])
     index, prop = find_peaks(S, height = min_peak_val, 
-                             distance = min_pix_distance, 
-                             prominence=prominence)
+                            distance = min_pix_distance, 
+                            prominence=prominence)
     
     # keep peaks with with slopes higher than the limit
     if slopes is None :
         index_select = index
     elif isinstance(slopes, numbers.Number) :
         left_slope = S[index] - S[prop['left_bases']]
         index_select = index[(left_slope>=slopes)]
@@ -974,18 +986,18 @@
     # display
     if display :
         if mode == 'dB' :
             ylabel ='Amplitude [dB]'
         else:
             ylabel = 'Amplitude [AU]'
         fig_kwargs = {
-                      'figtitle':'Mean Spectrum with detected peaks',
-                      'xlabel': kwargs.pop('xlabel','Frequency [Hz]'),
-                      'ylabel': kwargs.pop('ylabel',ylabel)
-                      }
+                    'figtitle':'Mean Spectrum with detected peaks',
+                    'xlabel': kwargs.pop('xlabel','Frequency [Hz]'),
+                    'ylabel': kwargs.pop('ylabel',ylabel)
+                    }
 
         ax, _ = plot1d(fn,S, **fig_kwargs)
         ax.plot(fn[index_select], S[index_select], '+', mfc=None, mec='r', 
                 mew=2, ms=8)
     return NBPeaks
 
 
@@ -1033,19 +1045,20 @@
     References 
     ----------
     .. [1] TOWSEY, Michael W. The calculation of acoustic indices derived from long-duration recordings of the natural environment. 2017. https://eprints.qut.edu.au/110634/1/QUTePrints110634_TechReport_Towsey2017August_AcousticIndices%20v3.pdf
     .. [2] QUT : https://github.com/QutEcoacoustics/audio-analysis. Michael Towsey, Anthony Truskinger, Mark Cottman-Fields, & Paul Roe. (2018, March 5). Ecoacoustics Audio Analysis Software v18.03.0.41 (Version v18.03.0.41). Zenodo. http://doi.org/10.5281/zenodo.1188744
 
     Examples
     --------
+    >>> import maad
     >>> s, fs = maad.sound.load('../data/cold_forest_daylight.wav')
     >>> Sxx_power, tn, fn, _ = maad.sound.spectrogram (s, fs)  
     >>> EAS, ECU, ECV, EPS, EPS_KURT, EPS_SKEW = maad.features.spectral_entropy(Sxx_power, fn, flim=(2000,10000)) 
-    >>> print('EAS: %2.2f / ECU: %2.2f / ECV: %2.2f / EPS: %2.2f / EPS_KURT: %2.2f / EPS_SKEW: %2.2f' % (EAS, ECU, ECV, EPS, EPS_KURT, EPS_SKEW))
-    EAS: 0.27 / ECU: 0.49 / ECV: 0.24 / EPS: 1.00 / EPS_KURT: 17.58 / EPS_SKEW: 3.55
+    >>> print('EAS: %2.2f / ECU: %2.2f / ECV: %2.2f / EPS: %2.2f / EPS_KURT: %2.2f / EPS_SKEW: %2.2f' % (EAS, ECU, ECV, EPS, EPS_KURT, EPS_SKEW)) # doctest: +NORMALIZE_WHITESPACE
+    EAS: 0.27 / ECU: 0.49 / ECV: 0.24 / EPS: 0.25 / EPS_KURT: 17.58 / EPS_SKEW: 3.55
     
     """
     
     if isinstance(flim, numbers.Number) :
         print ("WARNING: flim must be a tupple (fmin, fmax) or None")
         return
     
@@ -1111,15 +1124,15 @@
         ax.legend()
 
     return EAS, ECU, ECV, EPS, EPS_KURT, EPS_SKEW
 
 #=============================================================================
 
 def spectral_cover (Sxx, fn, dB_threshold=3, flim_LF=(0,1000), flim_MF=(1000,10000), 
-                   flim_HF=(10000,20000)):
+                flim_HF=(10000,20000)):
     """
     Compute the proportion (cover) of the spectrogram above a threshold for 
     three bandwidths : low frequency band (LF), medium frequency band (MF) and 
     high frequency band (HF) [1]_ [2]_.  
     
     Parameters
     ----------
@@ -1153,20 +1166,21 @@
     References 
     ----------
     .. [1] TOWSEY, Michael W. The calculation of acoustic indices derived from long-duration recordings of the natural environment. 2017. https://eprints.qut.edu.au/110634/1/QUTePrints110634_TechReport_Towsey2017August_AcousticIndices%20v3.pdf
     .. [2] QUT : https://github.com/QutEcoacoustics/audio-analysis. Michael Towsey, Anthony Truskinger, Mark Cottman-Fields, & Paul Roe. (2018, March 5). Ecoacoustics Audio Analysis Software v18.03.0.41 (Version v18.03.0.41). Zenodo. http://doi.org/10.5281/zenodo.1188744
 
     Examples
     --------
+    >>> import maad
     >>> s, fs = maad.sound.load('../data/cold_forest_daylight.wav')
     >>> Sxx_power, tn, fn, ext = maad.sound.spectrogram (s, fs)  
     >>> Sxx_noNoise= maad.sound.median_equalizer(Sxx_power, display=True, extent=ext) 
     >>> Sxx_dB_noNoise = maad.util.power2dB(Sxx_noNoise)
     >>> LFC, MFC, HFC = maad.features.spectral_cover(Sxx_dB_noNoise, fn) 
-    >>> print('LFC: %2.2f / MFC: %2.2f / HFC: %2.2f' % (LFC, MFC, HFC))
+    >>> print('LFC: %2.2f / MFC: %2.2f / HFC: %2.2f' % (LFC, MFC, HFC)) # doctest: +NORMALIZE_WHITESPACE
     LFC: 0.15 / MFC: 0.19 / HFC: 0.13
     
     """ 
 
     ### For Sxx to be a ndarray
     Sxx = np.asarray(Sxx) 
     
@@ -1220,21 +1234,22 @@
     References 
     ----------
     .. [1] TOWSEY, Michael W. The calculation of acoustic indices derived from long-duration recordings of the natural environment. 2017. https://eprints.qut.edu.au/110634/1/QUTePrints110634_TechReport_Towsey2017August_AcousticIndices%20v3.pdf
     .. [2] QUT : https://github.com/QutEcoacoustics/audio-analysis. Michael Towsey, Anthony Truskinger, Mark Cottman-Fields, & Paul Roe. (2018, March 5). Ecoacoustics Audio Analysis Software v18.03.0.41 (Version v18.03.0.41). Zenodo. http://doi.org/10.5281/zenodo.1188744
 
     Examples
     --------
+    >>> import maad
     >>> import numpy as np
     >>> s, fs = maad.sound.load('../data/cold_forest_daylight.wav')
     >>> Sxx_power, tn, fn, ext = maad.sound.spectrogram (s, fs)  
     >>> Sxx_noNoise= maad.sound.median_equalizer(Sxx_power, display=True, extent=ext) 
     >>> Sxx_dB_noNoise = maad.util.power2dB(Sxx_noNoise)
     >>> ACTspfract_per_bin, ACTspcount_per_bin, ACTspmean_per_bin = maad.features.spectral_activity(Sxx_dB_noNoise)  
-    >>> print('Mean proportion of spectrogram above threshold : %2.2f%%' %np.mean(ACTspfract_per_bin))
+    >>> print('Mean proportion of spectrogram above threshold : %2.2f%%' %np.mean(ACTspfract_per_bin)) # doctest: +NORMALIZE_WHITESPACE
     Mean proportion of spectrogram above threshold : 0.07%
     
     """ 
 
     ### For Sxx_dB to be a ndarray
     Sxx_dB = np.asarray(Sxx_dB) 
     
@@ -1252,15 +1267,15 @@
     An acoustic event corresponds to the period of the signal above a 
     threshold. An acoustic event could be short (at list one point if 
     rejectDuration is None) or very long (the duration of the entire audio). 
     Two acoustic events are separated by a period with low audio signal (ie
     below the threshold). Acoustic events are calculated frequency by frequency
     along time axis
     This function computes:
-      
+    
         - EVNspFraction : Fraction of events duration over total duration
         - EVNspmean : mean events duration (s)
         - EVNspcount : number of events per s
         - EVNsp : binary vector or matrix with 1 corresponding to event position
     
     Parameters
     ----------
@@ -1275,15 +1290,15 @@
         if the length is > rejectLength
     rejectDuration : scalar, optional, default is None
         event shorter than rejectDuration are discarded
         duration is in s
     display : boolean, optional, default is false
         Display a plot with the number of events per s (EVNspCount) and
         a binary image with the detected events.
-    \*\*kwargs : optional. See matplotlib documentation
+    kwargs : optional. See matplotlib documentation
 
     Returns
     -------    
     EVNspFract :scalar
         Fraction: events duration over total duration
     EVNspMean: scalar
         mean events duration in s
@@ -1297,30 +1312,31 @@
     References 
     ----------
     .. [1] TOWSEY, Michael W. The calculation of acoustic indices derived from long-duration recordings of the natural environment. 2017. https://eprints.qut.edu.au/110634/1/QUTePrints110634_TechReport_Towsey2017August_AcousticIndices%20v3.pdf
     .. [2] QUT : https://github.com/QutEcoacoustics/audio-analysis. Michael Towsey, Anthony Truskinger, Mark Cottman-Fields, & Paul Roe. (2018, March 5). Ecoacoustics Audio Analysis Software v18.03.0.41 (Version v18.03.0.41). Zenodo. http://doi.org/10.5281/zenodo.1188744
 
     Examples
     --------
+    >>> import maad
     >>> import numpy as np
     >>> s, fs = maad.sound.load('../data/cold_forest_daylight.wav')
     >>> Sxx_power, tn, fn, ext = maad.sound.spectrogram (s, fs)  
     >>> Sxx_noNoise= maad.sound.median_equalizer(Sxx_power) 
     >>> Sxx_dB_noNoise = maad.util.power2dB(Sxx_noNoise)
     >>> EVNspFract_per_bin, EVNspMean_per_bin, EVNspCount_per_bin, EVNsp = maad.features.spectral_events(Sxx_dB_noNoise, dt=tn[1]-tn[0], dB_threshold=6, rejectDuration=0.1, display=True, extent=ext)  
-    >>> print('Mean proportion of spectrogram with event s: %2.2f%%' %np.mean(EVNspFract_per_bin))
-    Mean proportion of spectrogram with events : 0.01%
+    >>> print('Mean proportion of spectrogram with events: %2.2f%%' %np.mean(EVNspFract_per_bin)) # doctest: +NORMALIZE_WHITESPACE
+    Mean proportion of spectrogram with events: 0.01%
     
     """  
     ### For wave to be a ndarray
     Sxx_dB = np.asarray(Sxx_dB) 
         
     EVNspSum, EVNspMean, EVNspCount, EVNsp = _acoustic_events (Sxx_dB, dt, 
-                                                               dB_threshold, 
-                                                               rejectDuration=rejectDuration)
+                                                            dB_threshold, 
+                                                            rejectDuration=rejectDuration)
     
     # EVNspFract = EVNspSum  * total_duration
     EVNspFract = EVNspSum / (dt * Sxx_dB.shape[1])
     
     if display :
         # display Number of events/s / frequency
         extent =  kwargs.pop('extent',None)
@@ -1349,16 +1365,16 @@
         title  =kwargs.pop('title','Events detected') 
         cmap   =kwargs.pop('cmap','gray')  
         figsize=kwargs.pop('figsize',(4, 13))  
         vmin=kwargs.pop('vmin',0)  
         vmax=kwargs.pop('vmax',1)
         
         ax, fig = plot2d (EVNsp*1, extent=extent, now=False, figsize=figsize, 
-                          title=title, ylabel=ylabel,xlabel=xlabel,
-                          vmin=vmin,vmax=vmax,  cmap=cmap, **kwargs) 
+                        title=title, ylabel=ylabel,xlabel=xlabel,
+                        vmin=vmin,vmax=vmax,  cmap=cmap, **kwargs) 
     
     return EVNspFract, EVNspMean, EVNspCount, EVNsp
 
 
 #=============================================================================
 def acoustic_complexity_index(Sxx):
     """
@@ -1395,18 +1411,19 @@
         
     References
     ----------
     .. [1] Pieretti N, Farina A, Morri FD (2011) A new methodology to infer the singing activity of an avian community: the Acoustic Complexity Index (ACI). Ecological Indicators, 11, 868-873. `DOI: 10.1016/j.ecolind.2010.11.005 <https://doi.org/10.1016/j.ecolind.2010.11.005>`_ 
     
     Examples
     --------
+    >>> import maad
     >>> s, fs = maad.sound.load('../data/cold_forest_daylight.wav')
     >>> Sxx, tn, fn, ext = maad.sound.spectrogram (s, fs, mode='amplitude')  
     >>> _, _ , ACI  = maad.features.acoustic_complexity_index(Sxx)
-    >>> print('ACI : %2.0f ' %ACI)
+    >>> print('ACI : %2.0f ' %ACI) # doctest: +NORMALIZE_WHITESPACE
     ACI : 306
     """   
     ACI_xx = ((np.abs(diff(Sxx,1)).transpose())/(np.sum(Sxx,1)).transpose()).transpose()       
     ACI_per_bin = np.sum(ACI_xx,axis=1)
     ACI_sum = np.sum(ACI_per_bin)
     
     return ACI_xx, ACI_per_bin, ACI_sum 
@@ -1466,32 +1483,33 @@
     
     References
     ----------
     .. [1] Villanueva-Rivera, L. J., B. C. Pijanowski, J. Doucette, and B. Pekin. 2011. A primer of acoustic analysis for landscape ecologists. Landscape Ecology 26: 1233-1246.`DOI: 10.1007/s10980-011-9636-9 <https://doi.org/10.1007/s10980-011-9636-9>`_ 
     
     Examples
     --------
+    >>> import maad
     
     Load the signal and compute the spectrogram to give the same result as soundecology
     
     >>> s, fs = maad.sound.load('../data/cold_forest_daylight.wav', detrend=False)
     >>> Sxx, tn, fn, ext = maad.sound.spectrogram (s, fs, nperseg=int(fs/10), noverlap=0, mode='amplitude', detrend=False) 
     >>> ADI  = maad.features.acoustic_diversity_index(Sxx,fn,fmax=10000)
-    >>> print('ADI : %2.2f ' %ADI)
+    >>> print('ADI : %2.2f ' %ADI) # doctest: +NORMALIZE_WHITESPACE
     ADI : 2.05
     
     Load the signal and compute the spectrogram as usual (detrend ON) such that
     the dB threshold needs to be adapted to give results that are more or less
     in line with soundecology
     
     >>> s, fs = maad.sound.load('../data/cold_forest_daylight.wav') 
     >>> Sxx, tn, fn, ext = maad.sound.spectrogram (s, fs, mode='amplitude')   
-    >>> ADI  = maad.features.acoustic_diversity_index(Sxx,fn,fmax=10000, dB_threshold = -30)
-    >>> print('ADI : %2.2f ' %ADI)
-    ADI : 1.46
+    >>> ADI  = maad.features.acoustic_diversity_index(Sxx,fn,fmax=10000, dB_threshold = -47)
+    >>> print('ADI : %2.2f ' %ADI) # doctest: +NORMALIZE_WHITESPACE
+    ADI : 2.06
     
     """
         
     # number of frequency intervals to compute the score
     N = np.floor((fmax-fmin)/bin_step)
     
     # convert into dB and normalization by the max
@@ -1519,15 +1537,15 @@
         s = s**2
         ADI = 1/sum(s)   
     
     return ADI
 
 #=============================================================================
 def acoustic_eveness_index (Sxx, fn, fmin=0, fmax=20000, bin_step=500, 
-                          dB_threshold=-50):
+                        dB_threshold=-50):
     
     """
     Compute the Acoustic Eveness Index (AEI) from a spectrogram [1]_.
     
     Parameters
     ----------
     Sxx: ndarray of floats
@@ -1568,31 +1586,32 @@
         
     References 
     ----------
     .. [1] Villanueva-Rivera, L. J., B. C. Pijanowski, J. Doucette, and B. Pekin. 2011. A primer of acoustic analysis for landscape ecologists. Landscape Ecology 26: 1233-1246.`DOI: 10.1007/s10980-011-9636-9 <https://doi.org/10.1007/s10980-011-9636-9>`_ 
     
     Examples
     --------
-    
+    >>> import maad
+
     Load the signal and compute the spectrogram to give the same result as soundecology
     
     >>> s, fs = maad.sound.load('../data/cold_forest_daylight.wav', detrend=False) 
     >>> Sxx, tn, fn, ext = maad.sound.spectrogram (s, fs, nperseg=int(fs/10), noverlap=0, mode='amplitude', detrend=False)   
     >>> AEI  = maad.features.acoustic_eveness_index(Sxx,fn,fmax=10000)
-    >>> print('AEI : %2.2f ' %AEI)
+    >>> print('AEI : %2.2f ' %AEI) # doctest: +NORMALIZE_WHITESPACE
     AEI : 0.39   
     
     Load the signal and compute the spectrogram as usual (detrend ON) such that
     the dB threshold needs to be adapted to give results that are more or less
     in line with soundecology
     
     >>> s, fs = maad.sound.load('../data/cold_forest_daylight.wav') 
     >>> Sxx, tn, fn, ext = maad.sound.spectrogram (s, fs, mode='amplitude')   
-    >>> AEI  = maad.features.acoustic_eveness_index(Sxx,fn,fmax=10000, dB_threshold = -30)
-    >>> print('AEI : %2.2f ' %AEI)
+    >>> AEI  = maad.features.acoustic_eveness_index(Sxx,fn,fmax=10000, dB_threshold = -47)
+    >>> print('AEI : %2.2f ' %AEI) # doctest: +NORMALIZE_WHITESPACE
     AEI : 0.39   
     
     """
 
     # number of frequency intervals to compute the score
     N = np.floor((fmax-fmin)/bin_step)
     
@@ -1614,15 +1633,15 @@
     
     return AEI
 
 #=============================================================================
 ####    Indices based on the energy
 #=============================================================================
 def soundscape_index (Sxx_power,fn,flim_bioPh=(1000,10000),flim_antroPh=(0,1000), 
-                     R_compatible = 'soundecology'):
+                    R_compatible = 'soundecology'):
     """
     Compute the Normalized Difference Soundscape Index from a power spectrogram [1]_.
         
     Parameters
     ----------
     Sxx_power : ndarray of floats
         2d : Power Spectrogram
@@ -1655,37 +1674,38 @@
     ----------
     .. [1] Kasten, Eric P., Stuart H. Gage, Jordan Fox, and Wooyeong Joo. 2012. The Remote Environmental Assessment Laboratory's Acoustic Library: An Archive for Studying Soundscape Ecology. Ecological Informatics 12: 50-67. `DOI: 10.1016/j.ecoinf.2012.08.001 <https://doi.org/10.1016/j.ecoinf.2012.08.001>`_ https://doi.org/10.1016/j.ecoinf.2012.08.001
     
     Ported from Seewave (http://rug.mnhn.fr/seewave) and soundecology R packages (cran.ms.unimelb.edu.au/web/packages/soundecology/soundecology.pdf).
     
     Examples
     --------
+    >>> import maad
     >>> s, fs = maad.sound.load('../data/cold_forest_daylight.wav')
     >>> Sxx_power, tn, fn, ext = maad.sound.spectrogram (s, fs)  
     >>> NDSI, ratioBA, antroPh, bioPh  = maad.features.soundscape_index(Sxx_power,fn)
-    >>> print('NDSI Soundecology : %2.2f ' %NDSI)
+    >>> print('NDSI Soundecology : %2.2f ' %NDSI) # doctest: +NORMALIZE_WHITESPACE
     NDSI Soundecology : 0.10
     >>> NDSI, ratioBA, antroPh, bioPh  = maad.features.soundscape_index(Sxx_power,fn,R_compatible=None)
-    >>> print('NDSI MAAD: %2.2f ' %NDSI)
-    NDSI MAAD : 0.99
+    >>> print('NDSI MAAD: %2.2f ' %NDSI) # doctest: +NORMALIZE_WHITESPACE
+    NDSI MAAD: 0.99
     
     """
     
     if R_compatible == 'soundecology' :
         # Step is determined as the difference between anthro_max and anthro_min
         bin_step = flim_antroPh[1] - flim_antroPh[0]
         #Convert into bins
         Sxx_bins, bins = into_bins(Sxx_power, fn, bin_min=fn[0], bin_max=fn[-1], 
-                                  bin_step=bin_step, axis=0)   
+                                bin_step=bin_step, axis=0)   
     else:
         # Frequency resolution is 1000 Hz
         bin_step = 1000
         #Convert into bins
         Sxx_bins, bins = into_bins(Sxx_power, fn, bin_min=fn[0], bin_max=fn[-1], 
-                                  bin_step=bin_step, axis=0) 
+                                bin_step=bin_step, axis=0) 
         # In Seewave, the first bin (0kHz) is removed
         Sxx_bins = Sxx_bins[bins>=1000,]
         bins = bins[bins>=1000]
         
     # Energy in BIOBAND
     bioPh = sum(Sxx_bins[index_bw(bins, flim_bioPh), ])
     # Energy in ANTHROPOBAND
@@ -1729,21 +1749,22 @@
     Soundecology compatible version:
     * Average of dB value
     * Remove negative value in order to get positive values only
     * Dividing by the frequency resolution df instead of multiplication
     
     Examples
     --------
+    >>> import maad
     >>> s, fs = maad.sound.load('../data/cold_forest_daylight.wav')
     >>> Sxx, tn, fn, ext = maad.sound.spectrogram (s, fs,mode='amplitude')  
     >>> BI = maad.features.bioacoustics_index(Sxx,fn)
-    >>> print('BI Soundecology : %2.2f ' %BI)
+    >>> print('BI Soundecology : %2.2f ' %BI) # doctest: +NORMALIZE_WHITESPACE
     BI Soundecology : 52.84
     >>> BI  = maad.features.bioacoustics_index(Sxx,fn,R_compatible=None)
-    >>> print('BI MAAD: %2.2f ' %BI)
+    >>> print('BI MAAD : %2.2f ' %BI) # doctest: +NORMALIZE_WHITESPACE
     BI MAAD : 17.05
     
     """    
     
     # select the indices corresponding to the frequency bins range
     indf = index_bw(fn,flim)
     
@@ -1809,17 +1830,18 @@
     Returns
     -------
     LEQt: float
         Equivalent Continuous Sound level (Leq) in dB SPL
 
     Examples
     --------
+    >>> import maad
     >>> s, fs = maad.sound.load('../data/spinetail.wav')
     >>> Leq = maad.features.temporal_leq (s, fs, gain=42)
-    >>> print('Leq is %2.1fdB SPL' % Leq)
+    >>> print('Leq is %2.1fdB SPL' % Leq) # doctest: +NORMALIZE_WHITESPACE
     Leq is 63.7dB SPL
     
     """
     # compute the Leq for each dt step
     leq = wav2leq(s, fs, gain, Vadc, dt, sensitivity, dBref)
     # average them
     LEQt = mean_dB(leq, axis=1)
@@ -1852,18 +1874,19 @@
     Returns
     -------
     LEQf: float
         Equivalent Continuous Sound level (Leq) in dB SPL
 
     Examples
     --------
+    >>> import maad
     >>> s, fs = maad.sound.load('../data/spinetail.wav')
     >>> Sxx_power,_,_,_ = maad.sound.spectrogram(s,fs)
     >>> Leqf, Leqf_per_bin = maad.features.spectral_leq(Sxx_power, gain=42)
-    >>> print('Leq (from spectrogram) is %2.1fdB SPL' % Leqf)
+    >>> print('Leq (from spectrogram) is %2.1fdB SPL' % Leqf) # doctest: +NORMALIZE_WHITESPACE
     Leq (from spectrogram) is 63.7dB SPL
     
     """
     # force X to be an ndarray
     X = np.asarray(X)
     
     # test if X has 2d (Spectrogram Pxx)
@@ -1921,29 +1944,30 @@
         
     References
     ----------
     .. [1] Zhao, Yueqin. "Rao's Quadratic Entropy and Some New Applications" (2010). Doctor of Philosophy (PhD), dissertation,Mathematics and Statistics, Old Dominion University. `DOI: 10.25777/qgak-sf09 <https://doi.org/10.25777/qgak-sf09>`_
     
     Examples
     --------
+    >>> import maad
     
     Compute entropy in time domain.
     
     >>> s, fs = maad.sound.load('../data/spinetail.wav')
     >>> env = maad.sound.envelope(s)
     >>> Ht_Havrda, Ht_Renyi, Ht_pairedShannon, Ht_gamma, Ht_GiniSimpson = maad.features.more_entropy(env**2, order=3)
-    >>> print('Ht_Havrda: %2.2f / Ht_Renyi: %2.2f / Ht_pairedShannon: %2.2f / Ht_gamma: %2.0f / Ht_GiniSimpson: %2.2f' % (Ht_Havrda, Ht_Renyi, Ht_pairedShannon, Ht_gamma, Ht_GiniSimpson))
+    >>> print('Ht_Havrda: %2.2f / Ht_Renyi: %2.2f / Ht_pairedShannon: %2.2f / Ht_gamma: %2.0f / Ht_GiniSimpson: %2.2f' % (Ht_Havrda, Ht_Renyi, Ht_pairedShannon, Ht_gamma, Ht_GiniSimpson)) # doctest: +NORMALIZE_WHITESPACE
     Ht_Havrda: 0.33 / Ht_Renyi: 7.20 / Ht_pairedShannon: 9.04 / Ht_gamma: 24223924 / Ht_GiniSimpson: 1.00
     
     Compute entropy in spectral domain.
     
     >>> Sxx_power,_,_,_ = maad.sound.spectrogram(s,fs)
     >>> S_power = maad.sound.avg_power_spectro(Sxx_power)
     >>> Hf_Havrda, Hf_Renyi, Hf_pairedShannon, Hf_gamma, Hf_GiniSimpson = maad.features.more_entropy(S_power, order=3)
-    >>> print('Hf_Havrda: %2.2f / Hf_Renyi: %2.2f / Hf_pairedShannon: %2.2f / Hf_gamma: %2.0f / Hf_GiniSimpson: %2.2f' % (Hf_Havrda, Hf_Renyi, Hf_pairedShannon, Hf_gamma, Hf_GiniSimpson))
+    >>> print('Hf_Havrda: %2.2f / Hf_Renyi: %2.2f / Hf_pairedShannon: %2.2f / Hf_gamma: %2.0f / Hf_GiniSimpson: %2.2f' % (Hf_Havrda, Hf_Renyi, Hf_pairedShannon, Hf_gamma, Hf_GiniSimpson)) # doctest: +NORMALIZE_WHITESPACE
     Hf_Havrda: 0.33 / Hf_Renyi: 3.23 / Hf_pairedShannon: 4.92 / Hf_gamma: 7931 / Hf_GiniSimpson: 0.97
     
     """
     
     if isinstance(x, (np.ndarray)) == True:
         if x.ndim > axis:
             if x.shape[axis] == 1:
@@ -1995,91 +2019,101 @@
         
     References
     ----------
     .. [1] Zhao, Yueqin. "Rao's Quadratic Entropy and Some New Applications" (2010). Doctor of Philosophy (PhD), dissertation,Mathematics and Statistics, Old Dominion University. `DOI: 10.25777/qgak-sf09 <https://doi.org/10.25777/qgak-sf09>`_
     
     Examples
     --------
+    >>> import maad
     >>> s, fs = maad.sound.load('../data/spinetail.wav')
     >>> Sxx_power,tn,fn,_ = maad.sound.spectrogram(s,fs)
     >>> S_power = maad.sound.avg_power_spectro(Sxx_power) 
-    >>> maad.features.frequency_raoq(S_power, fn)
+    >>> maad.features.frequency_raoq(S_power, fn) # doctest: +NORMALIZE_WHITESPACE
     0.10556621228886422
     
     """
     
     # be sure they are ndarray
     X = np.asarray(S_power)    
 
     #Convert into bins
     X_bins, bins = into_bins(X, fn, bin_min=fn[0], bin_max=fn[-1], 
                             bin_step=bin_step, axis=None) 
-              
+    
     # Compute Rao Quadratic Entropy
     RAOQ = _raoQ(X_bins,bins)
     
     return RAOQ
 
 #=============================================================================    
 
-def tfsd (Sxx, fn, tn, flim=(2000,8000), mode='thirdOctave', display=False):
+def tfsd (Sxx, fn, tn, flim=(2000,8000), log=True, mode='thirdOctave', display=False):
     """
     Compute the Time frequency derivation index (tfsd) from a spectrogram. [1]_ [2]_
         
     Parameters
     ----------
     Sxx : ndarray of floats
-        matrix : Spectrogram  
+        matrix : Amplitude spectrogram  
     fn : vector
         frequency vector corresponding to the spectrogram
     tn : vector
         time vector corresponding to the spectrogram 
     flim : tupple (fmin, fmax), optional, default is (2000, 8000)
         Frequency band used to compute tfsd. 
+    log : boolean, optional, default is True
+        If True, the log of Sxx is taken before calculating the TFSD as it was defined in [1]_ [2]_
+        if False, no log is applied, TFSD > 0.3 indicates the presence of birds 
     mode : string {'thirdOctave','Octave'}, default is thirdOctave  
         Select the way to transform the spectrogram with linear bands into 
         octave bands    
     display : boolean, optional, default is False
         Display the 1st and 2nd derivation of the spectrogram
 
     Returns
     -------    
     tfsd : scalar
         Time frequency derivation index
         
     Notes
     -----
-    The higher the TFSD varies between 0 and 1, the greater the temporal 
-    presence of avian or human vocalizations.  
-    With the default configuration, a TFSD > 0.3 indicates a very important 
-    presence time of the vocalizations in the signal. 
-    The TFSD is always greater than 0.
-       
+    The TFSD varies between 0 and 1, where 1 indicates sound events on the full spectrogram. 
+    When flim=(2000,8000), TFSD mostly indicates the presence of birds in the signal
+    When flim=(0,1000), TFSD mostly indicates the presence of human voice in the signal
+    When log=False and flim=(2000,8000), a TFSD > 0.3 indicates the presence of birds in the signal
+
     References 
     ----------
     .. [1] Aumond, P., Can, A., De Coensel, B., Botteldooren, D., Ribeiro, C., & Lavandier, C. (2017). Modeling soundscape pleasantness using perceptual assessments and acoustic measurements along paths in urban context. Acta Acustica united with Acustica. `DOI: 10.3813/AAA.919073 <https://doi.org/10.3813/AAA.919073>`_ 
     .. [2] Gontier, F., Lavandier, C., Aumond, P., Lagrange, M., & Petiot, J. F. (2019). Estimation of the perceived time of presence of sources in urban acoustic environments using deep learning techniques. Acta Acustica united with Acustica.`DOI: 10.3813/AAA.919384 <https://doi.org/10.3813/AAA.919384>`_
     
     Examples
     --------
+    >>> import maad
+
     During the day
     
     >>> s, fs = maad.sound.load('../data/cold_forest_daylight.wav')
     >>> Sxx_power,tn,fn,_ = maad.sound.spectrogram(s,fs)
-    >>> maad.features.tfsd(Sxx_power,fn, tn)  
-    0.5002113200343906
+    >>> maad.features.tfsd(Sxx_power,fn, tn)  # doctest: +NORMALIZE_WHITESPACE 
+    0.4637352908292768
     
     During the night
     
     >>> s, fs = maad.sound.load('../data/cold_forest_night.wav')
     >>> Sxx_power,tn,fn,_ = maad.sound.spectrogram(s,fs)
-    >>> maad.features.tfsd(Sxx_power,fn, tn)  
-    0.012818445992714088
+    >>> maad.features.tfsd(Sxx_power,fn, tn)   # doctest: +NORMALIZE_WHITESPACE
+    0.42435773298811824
     
     """
+    
+    # In order to be complient with the definition of the tfsd, it must be computed on dB scale
+    # But t
+    if log : Sxx = np.log10(Sxx)
+    
     # convert into 1/3 octave
     if mode == 'thirdOctave' : 
         x, fn_bin = linear_to_octave(Sxx, fn, thirdOctave=True)
     elif mode == 'Octave' : 
         x, fn_bin = linear_to_octave(Sxx, fn, thirdOctave=False)   
 
     # Derivation along the time axis, for each frequency bin
@@ -2106,42 +2140,41 @@
             fig.set_facecolor('w')
             fig.set_edgecolor('k')
             fig.set_figheight(4)
             fig.set_figwidth (13)
                     
             # display image
             _im1 = ax1.imshow(power2dB(GRADdt), 
-                              vmax = max(power2dB(GRADdt)), 
-                              vmin = min(power2dB(GRADdt)),
-                              interpolation='none', origin='lower', 
-                              cmap='gray', extent=extent)
+                            vmax = max(power2dB(GRADdt)), 
+                            vmin = min(power2dB(GRADdt)),
+                            interpolation='none', origin='lower', 
+                            cmap='gray', extent=extent)
             plt.colorbar(_im1, ax=ax1)
             
             # set the parameters of the subplot
             ax1.set_title('Derivation along time axis')
             ax1.set_xlabel('Time [sec]')
             ax1.set_ylabel('Frequency [Hz]')   
             ax1.axis('tight') 
             
             # display image
             _im2 = ax2.imshow(power2dB(GRADdf), 
-                              vmax = max(power2dB(GRADdf)), 
-                              vmin = min(power2dB(GRADdf)),
-                              interpolation='none', origin='lower', 
-                              cmap='gray', extent=extent)
+                            vmax = max(power2dB(GRADdf)), 
+                            vmin = min(power2dB(GRADdf)),
+                            interpolation='none', origin='lower', 
+                            cmap='gray', extent=extent)
             plt.colorbar(_im2, ax=ax2)
-       
             # set the parameters of the subplot
             ax2.set_title('Derivation along frequency axis')
             ax2.set_xlabel('Time [sec]')
             ax2.set_ylabel('Frequency [Hz]')
             ax2.axis('tight') 
-         
+        
             fig.tight_layout()
-             
+            
             # Display the figure now
             plt.show()
     
     return tfsd
 
 #=============================================================================
 def acoustic_gradient_index(Sxx, dt, order=1, norm='per_bin', display=False):
@@ -2174,31 +2207,32 @@
     AGI_mean ; scalar
         average AGI value per frequency bin (independant of the number of 
         frequency bin)
         mean(AGI_per_bin)
     
     Examples
     --------
+    >>> import maad
     
     During the day
     
     >>> s, fs = maad.sound.load('../data/cold_forest_daylight.wav')
     >>> Sxx_power,tn,fn,_ = maad.sound.spectrogram(s,fs)
     >>> _, _, AGI_mean, _ = maad.features.acoustic_gradient_index(Sxx_power,tn[1]-tn[0])
-    >>> AGI_mean
-    5.026112548525072
+    >>> AGI_mean # doctest: +NORMALIZE_WHITESPACE
+    5.026112548525073
     
     During the night
     
     >>> s, fs = maad.sound.load('../data/cold_forest_night.wav')
     >>> Sxx_power,tn,fn,_ = maad.sound.spectrogram(s,fs)
     >>> _, _, AGI_mean, _ = maad.features.acoustic_gradient_index(Sxx_power,tn[1]-tn[0])
-    >>> AGI_mean
+    >>> AGI_mean # doctest: +NORMALIZE_WHITESPACE
     1.45631461307782  
-     
+    
     """     
     # derivative (order = 1, 2, 3...)
     AGI_xx = abs(diff(Sxx, order, axis=1)) / (dt**order )
     
     if norm is not None :
         # Normalize the derivative by the median derivative which should 
         # correspond to the background (noise) derivative
@@ -2226,43 +2260,43 @@
         fig4.set_facecolor('w')
         fig4.set_edgecolor('k')
         fig4.set_figheight(4)
         fig4.set_figwidth (13)
                 
         # display image
         _im = ax4.imshow(power2dB(Sxx**2), 
-                         interpolation='none', origin='lower', 
-                         vmin =20, vmax=70, cmap='gray')
+                        interpolation='none', origin='lower', 
+                        vmin =20, vmax=70, cmap='gray')
         plt.colorbar(_im, ax=ax4)
- 
+
         # set the parameters of the subplot
         ax4.set_title('Spectrogram')
         ax4.set_xlabel('Time [sec]')
         ax4.set_ylabel('Frequency [Hz]')
         ax4.axis('tight') 
-     
+    
         fig4.tight_layout()
-         
+        
         # Display the figure now
         plt.show()
         
     return AGI_xx, AGI_per_bin, AGI_mean, AGI_sum
 
 #=============================================================================
 
 def region_of_interest_index(Sxx_dB_noNoise, tn, fn, 
-                             smooth_param1=1, 
-                             mask_mode='relative', 
-                             mask_param1=6, 
-                             mask_param2=0.5, 
-                             min_roi=9, 
-                             max_roi=512*10000, 
-                             max_ratio_xy = None,
-                             remove_rain = False,
-                             display=False, **kwargs):
+                            smooth_param1=1, 
+                            mask_mode='relative', 
+                            mask_param1=6, 
+                            mask_param2=0.5, 
+                            min_roi=9, 
+                            max_roi=512*10000, 
+                            max_ratio_xy = None,
+                            remove_rain = False,
+                            display=False, **kwargs):
     """
     Compute an acoustic activity index based on the regions of interested 
     detected on a spectrogram.
     
     The function first find regions of interest (ROI) and then compute the number
     or ROIs and the cover area of these ROIS
     on the spectrogram.
@@ -2276,34 +2310,37 @@
     fn : 1d ndarray of floats
         Frequency vector (vertical y-axis) 
     smooth_param1 : scalar, default is 1
         Standard deviation of the gaussian kernel used to smooth the image 
         The larger is the number, the smoother will be the image and the longer 
         it takes. Standard values should fall between 0.5 to 3 
     mask_mode : string in {'relative', 'absolute'}, optional, default is 'relative'
-        if 'relative':
+        | if 'relative':
             Binarize an image based on a double relative threshold.  
             The values used for the thresholding depends on the values found 
             in the image. => relative threshold 
-        if 'absolute' :
+        | if 'absolute' :
             Binarize an image based on a double relative threshold.  
             The values used for the thresholding are independent of the values 
-            in the image => absolute threshold 
-        .. warning:: The default ``mask_mode`` parameter is deprecated in 
-        version 1.3 and will be changed to ``absolute`` in 1.4.
+            in the image => absolute threshold
+
+        .. warning:: The default ``mask_mode`` parameter is deprecated in version 1.3 and will be changed to ``absolute`` in version 1.4.
+
     mask_param1 : scalar, default is 6
-        if 'relative' : bin_std 
-        if 'absolute' : bin_h
-        .. warning:: The default ``mask_param1`` parameter is deprecated in 
-        version 1.3 and will be changed to ``10`` in 1.4.
+        | if 'relative' : bin_std 
+        | if 'absolute' : bin_h
+
+        .. warning:: The default ``mask_param1`` parameter is deprecated in version 1.3 and will be changed to ``10`` in version 1.4.
+
     mask_param2 : scalar, default is 0.5
-        if 'relative' : bin_per
-        if 'absolute' : bin_l
-        .. warning:: The default ``mask_param2`` parameter is deprecated in 
-        version 1.3 and will be changed to ``3`` in 1.4.
+        | if 'relative' : bin_per
+        | if 'absolute' : bin_l
+        
+        .. warning:: The default ``mask_param2`` parameter is deprecated in version 1.3 and will be changed to ``3`` in 1.4.
+    
     min_roi, max_roi : scalars, optional, default : 9,  512*10000
         Define the minimum and the maximum area possible for a ROI. If None,  
         the minimum ROI area is 1 pixel and the maximum ROI area is the area of  
         the image 
         .. warning:: The default ``min_roi`` and ``max_roi`` parameter is 
         deprecated in version 1.3 and will be changed to ``None`` in 1.4.
     max_ratio_xy : scalar, optional, default : None
@@ -2320,65 +2357,66 @@
     display : boolean, default is false
         plot graphs and spectrograms
     /*/*kwargs optional. This parameter is used by plt.plot and savefig functions 
 
     Returns
     -------    
     ROItotal : float
-         Total number of ROIs found. The higher is the number of ROI, the higher
-         is the acoustic abondance and/or richness expected
+        Total number of ROIs found. The higher is the number of ROI, the higher
+        is the acoustic abondance and/or richness expected
     ROIcover : float
         Percentage of spectrogram cover. The higher is the cover percentage, 
         the higher is the acoustic richness expected.
         
     Examples
-    -------- 
+    --------
+    >>> import maad 
     >>> s, fs = maad.sound.load('../data/cold_forest_daylight.wav')
     >>> Sxx_power,tn,fn,_ = maad.sound.spectrogram(s,fs)
     >>> Sxx_noNoise= maad.sound.median_equalizer(Sxx_power) 
     >>> Sxx_dB_noNoise = maad.util.power2dB(Sxx_noNoise)
     >>> ROItotal, ROIcover = maad.features.region_of_interest_index(Sxx_dB_noNoise, tn, fn, display=True)
-    >>> print('The total number of ROIs found in the spectrogram is %2.0f' %ROItotal)
+    >>> print('The total number of ROIs found in the spectrogram is %2.0f' %ROItotal) # doctest: +NORMALIZE_WHITESPACE
     The total number of ROIs found in the spectrogram is 265
-    >>> print('The percentage of spectrogram covered by ROIs is %2.0f%%' %ROIcover)
+    >>> print('The percentage of spectrogram covered by ROIs is %2.0f%%' %ROIcover) # doctest: +NORMALIZE_WHITESPACE
     The percentage of spectrogram covered by ROIs is 12%
     
     """ 
     
     # extent
     kwargs.update({'extent':(tn[0], tn[-1], fn[0], fn[-1])})
     
     # if remove rain => remove frequential spikes (rain)
     if remove_rain == True :
         Sxx_dB_noNoise = opening(Sxx_dB_noNoise, selem=np.ones([1,5]))
 
     # Smooth the spectrogram in order to facilitate the creation of masks
     Sxx_dB_noNoise_smooth = smooth(Sxx_dB_noNoise, std=smooth_param1, 
-                                   display=display, savefig=None,**kwargs) 
+                                display=display, savefig=None,**kwargs) 
     # binarization of the spectrogram to select part of the spectrogram with 
     # acoustic activity
     if mask_mode == 'relative' :
         im_mask = create_mask(Sxx_dB_noNoise_smooth,  
-                              mode_bin = 'relative', bin_std=mask_param1, 
-                              bin_per=mask_param2,
-                              display=display, savefig=None, **kwargs) 
+                            mode_bin = 'relative', bin_std=mask_param1, 
+                            bin_per=mask_param2,
+                            display=display, savefig=None, **kwargs) 
     elif  mask_mode == 'absolute' :   
         im_mask = create_mask(Sxx_dB_noNoise_smooth,  
-                              mode_bin = 'absolute', bin_h=mask_param1, 
-                              bin_l=mask_param2,
-                              display=display, savefig=None, **kwargs)    
+                            mode_bin = 'absolute', bin_h=mask_param1, 
+                            bin_l=mask_param2,
+                            display=display, savefig=None, **kwargs)    
     else:
         raise TypeError ('mask_mode should be selected in {relative, absolute}')
             
     # get the mask with rois (im_rois) and the bounding box for each rois (rois_bbox) 
     # and an unique index for each rois => in the pandas dataframe rois
     im_rois, rois  = select_rois(im_mask,
-                                 min_roi=min_roi, 
-                                 max_roi=max_roi,
-                                 display= display, **kwargs)
+                                min_roi=min_roi, 
+                                max_roi=max_roi,
+                                display= display, **kwargs)
     
     ##### Extract centroids features of each roi from the spectrogram in dB without noise 
     X = dB2power(Sxx_dB_noNoise)
     rois = format_features(rois, tn, fn) 
     centroid = centroid_features(X, rois, im_rois)
     
     ###### remove rois with ratio >max_ratio_xy (they are mostly artefact 
@@ -2404,15 +2442,14 @@
     x,y = im_rois.shape
     total_area = x*y
     # Pourcentage of ROI over the total area
     ROIcover = sum(area) / total_area *100
     
     return  ROItotal, ROIcover
 
-
 #=============================================================================
 def all_temporal_alpha_indices(s, fs, verbose=False, display=False, **kwargs):
     """
     Compute 16 temporal domain acoustic indices.
 
     Parameters
     ----------
@@ -2420,15 +2457,15 @@
         Audio to process (wav)
     fs : float
         Sampling frequency of the audio (Hz)
     verbose : boolean, default is False
         print indices on the default terminal
     display : boolean, default is False
         Display graphs
-    \*\*kwargs : arguments for functions:
+    kwargs : arguments for functions:
         
         - temporal_leq(s, fs, gain, Vadc, sensitivity, dBref, dt)
         - temporal_snr(s, mode, Nt) 
         - temporal_median(s, mode, Nt)
         - temporal_entropy(s, compatibility, mode, Nt)
         - temporal_activity (s,dB_threshold, mode, Nt)
         - temporal_events (s, fs, dB_threshold, rejectDuration, mode, Nt,display)
@@ -2469,47 +2506,49 @@
         
         For audio activity and events
         
         dB_threshold : scalar, optional, default is 3dB
             data >Threshold is considered to be an event if the length is > rejectLength
         rejectDuration : scalar, optional, default is None
             event shorter than rejectDuration are discarded duration is in s
-   
+
     Returns
     -------
     df_temporal_indices: Pandas dataframe
-       Dataframe containing of the calculated audio indices : ZCR, MEANt, 
-       VARt, SKEWt, KURTt, LEQt, BGNt, SNRt, MED, Ht, ACTtFraction, 
-       ACTtCount, ACTtMean, EVNtFraction, EVNtMean, EVNtCount
-           
+        Dataframe containing of the calculated audio indices : ZCR, MEANt, 
+        VARt, SKEWt, KURTt, LEQt, BGNt, SNRt, MED, Ht, ACTtFraction, 
+        ACTtCount, ACTtMean, EVNtFraction, EVNtMean, EVNtCount
+    
     See also
     --------
     temporal_moments, temporal_events, temporal_activity, temporal_entropy, 
     temporal_median, temporal_leq, temporal_snr, zero_crossing_rate
 
     Examples
     --------
+    >>> import maad
+
     >>> s, fs = maad.sound.load('../data/cold_forest_night.wav')
-    >>> df_tempora_indices_NIGHT = maad.features.all_temporal_alpha_indices (s,fs)
+    >>> df_temporal_indices_NIGHT = maad.features.all_temporal_alpha_indices (s,fs)
     >>> s, fs = maad.sound.load('../data/cold_forest_daylight.wav')
     >>> df_temporal_indices_DAY = maad.features.all_temporal_alpha_indices (s,fs)
     
     Variation between night and day
     
-    >>> var = abs(df_temporal_indices_DAY - df_temporal_indices_NIGHT)/df_temporal_indices_NIGHT*100
-    >>> print('LEQt var night vs day: %2.2f %%' % var.LEQt)
-    LEQt var : 29.66 %
-    >>> print('Ht var night vs day: %2.2f %%' % var.Ht)
-    Ht var : 2.33 %
-    >>> print('MEANt var night vs day: %2.2f %%' % var.MEANt)
-    MEANt var night vs day: 299.62 %
-    >>> print('VARt var night vs day: %2.2f %%' % var.VARt)
-    VARt var night vs day: 1664.02 %
-    >>> print('EVNtFraction var night vs day: %2.2f %%' % var.EVNtFraction)
-    EVNtFraction var night vs day: 98.48 %
+    >>> variation = abs(df_temporal_indices_DAY - df_temporal_indices_NIGHT)/df_temporal_indices_NIGHT*100
+    >>> print('LEQt variation night vs day: %2.2f %%' % variation['LEQt'][0]) # doctest: +NORMALIZE_WHITESPACE
+    LEQt variation night vs day: 29.66 %
+    >>> print('Ht variation night vs day: %2.2f %%' % variation.Ht.iloc[0]) # doctest: +NORMALIZE_WHITESPACE
+    Ht variation night vs day: 2.33 %
+    >>> print('MEANt variation night vs day: %2.2f %%' % variation['MEANt'][0]) # doctest: +NORMALIZE_WHITESPACE
+    MEANt variation night vs day: 299.62 %
+    >>> print('VARt variation night vs day: %2.2f %%' % variation['VARt'][0]) # doctest: +NORMALIZE_WHITESPACE
+    VARt variation night vs day: 1664.02 %
+    >>> print('EVNtFraction variation night vs day: %2.2f %%' % variation['EVNtFraction'][0]) # doctest: +NORMALIZE_WHITESPACE
+    EVNtFraction variation night vs day: 98.48 %
     
     """
     
     #### get variables
     # Envelope => mode {'fast', 'hilbert"}, if 'fast', set Nt, number of point by frame 
     mode = kwargs.pop('mode','fast')
     Nt = kwargs.pop('Nt',512)
@@ -2578,17 +2617,17 @@
     df_temporal_indices += [ACTtFraction, ACTtCount, ACTtMean]
     if verbose :
         print("ACTtFraction %2.5f" % ACTtFraction)
         print("ACTtCount %2.5f" % ACTtCount)
         print("ACTtMean %2.5f" % ACTtMean)
     
     EVNtFraction, EVNtMean, EVNtCount, _ = temporal_events (s, fs, dB_threshold,
-                                                         rejectDuration,
-                                                         mode, Nt,
-                                                         display=display)
+                                                        rejectDuration,
+                                                        mode, Nt,
+                                                        display=display)
     df_temporal_indices += [EVNtFraction, EVNtMean, EVNtCount]
     if verbose :    
         print("EVNtFraction %2.5f" % EVNtFraction)
         print("EVNtMean %2.5f" % EVNtMean)
         print("EVNtCount %2.5f" % EVNtCount)
     
     df_temporal_indices = pd.DataFrame([df_temporal_indices], 
@@ -2608,18 +2647,18 @@
                                             'EVNtFraction', 
                                             'EVNtMean', 
                                             'EVNtCount'])
     return df_temporal_indices
 
 
 def all_spectral_alpha_indices (Sxx_power, tn, fn,
-                      flim_low=[0,1000], 
-                      flim_mid=[1000,10000], 
-                      flim_hi=[10000,20000], 
-                      verbose=False, display=False, **kwargs):
+                    flim_low=[0,1000], 
+                    flim_mid=[1000,10000], 
+                    flim_hi=[10000,20000], 
+                    verbose=False, display=False, **kwargs):
     """
     Computes the acoustic indices in spectral (spectrum (1d) or spectrogram (2d)) domain.
 
     Parameters
     ----------
     Sxx_power : 2D array of floats
         Power spectrogram to process (taken directly from maad.sound.spectrogram)
@@ -2633,28 +2672,28 @@
         mid frequency band in Hz
     flim_hi : tupple, optional, default is (10000,20000)
         high frequency band in Hz        
     verbose : boolean, default is False
         print indices on the default terminal
     display : boolean, default is False
         Display graphs
-    \*\*kwargs : arguments for functions:
+    kwargs : arguments for functions:
     
         - spectral_leq
         - frequency_entropy
         - soundscape_index
         - bioacoustics_index
         - acoustic_diversity_index
         - acoustic_eveness_index
         - spectral_cover
         - spectral_activity
         - spectral_events
         - tfsd
         - region_of_interest_index
-               
+        
         For soundscape_index, bioacoustics_index, acoustic_diversity_index, acoustic_eveness_index
         
         R_compatible : string, optional, default is "soundecology"
             if 'soundecology', the result is similar to the package SoundEcology in R. Otherwise, the result is specific to maad
                 
         For LEQf calculation
         
@@ -2665,15 +2704,15 @@
         sensitivity : float, optional, default is -35 (dB/V)
             Sensitivity of the microphone
         dBref : integer, optional, default is 94 (dBSPL)
             Pressure sound level used for the calibration of the microphone (usually 94dB, sometimes 114dB)
         pRef : float
             Sound pressure reference in the medium (air : 20e-6, water : 1e-6)
         
-        For spectral activity and events, ADI, AEI
+        For spectral activity and events
         
         dB_threshold : scalar, optional, default is 3dB
             data >Threshold is considered to be an event 
             if the length is > rejectLength
             
         For spectral activity and events
         
@@ -2713,60 +2752,77 @@
         min_roi, max_roi : scalars, optional, default : 9,  512*10000
             Define the minimum and the maximum area possible for an ROI. If None,  
             the minimum ROI area is 1 pixel and the maximum ROI area is the area of  
             the image     
         
         For ADI, AEI, RAOQ
         
-        bin_step : scalar, optional, default is 500
-            Frequency step in Hz        
-  
+        bin_step : scalar, optional, default is 1000
+            Frequency step in Hz   
+
+        For ADI and AEI
+        
+        ADI_dB_threshold : scalar, optional, default is -50   
+            Threshold in dB
+        AEI_dB_threshold : scalar, optional, default is -50   
+            Threshold in dB
+
     Returns
     -------
     df_spectral_indices: Panda dataframe
         Dataframe containing of the calculated spectral indices :
     df_per_bin_indices : Panda dataframe
         Dataframe containing of the calculated spectral indices  per frequency
         bin :
-           
+    
     See Also
     --------
     number_of_peaks, spectral_leq, spectral_snr, frequency_entropy, 
     spectral_entropy, acoustic_complexity_index, soundscape_index, soundscape_index,
     roughness, acoustic_diversity_index, acoustic_eveness_index, spectral_cover, 
     spectral_activity, spectral_events, tfsd, more_entropy, frequency_raoq, 
     acoustic_gradient_index, region_of_interest_index
 
+    Notes
+    -----
+    In order to obtain the same output for AEI and ADI as for soundecology,
+        the signal and the spectrogram need to be processed without detrend on.
+        maad.sound.load("myfile.wav", ..., detrend = False)
+        maad.sound.spectrogram(s, fs, ..., detrend = False)
+        For a complete example, see the examples of the functions acoustic_eveness_index and acoustic_diversity_index
+
     Examples
-    --------    
+    --------
+    >>> import maad
+
     Spectral indices on a daylight recording
     
     >>> s, fs = maad.sound.load('../data/cold_forest_daylight.wav')
     >>> Sxx_power,tn,fn,ext = maad.sound.spectrogram (s, fs)  
     >>> df_spectral_indices_DAY, _ = maad.features.all_spectral_alpha_indices(Sxx_power,tn,fn,display=True, extent=ext)
     
     Spectral indices on a night recording
     
     >>> s, fs = maad.sound.load('../data/cold_forest_night.wav')
     >>> Sxx_power,tn,fn,ext = maad.sound.spectrogram (s, fs)  
     >>> df_spectral_indices_NIGHT, _ = maad.features.all_spectral_alpha_indices(Sxx_power,tn,fn,display=True)
     
     Variation between night and day
     
-    >>> var = abs(df_spectral_indices_DAY - df_spectral_indices_NIGHT)/df_spectral_indices_NIGHT*100
-    >>> print('LEQf var night vs day: %2.2f %%' % var.LEQf)
-    LEQf var night vs day: 34.94 %
-    >>> print('Hf var night vs day: %2.2f %%' % var.Hf)
-    Hf var night vs day: 105.61 %
-    >>> print('ACI var night vs day: %2.2f %%' % var.ACI)
-    ACI var night vs day: 3.39 %
-    >>> print('AGI var night vs day: %2.2f %%' % var.AGI)
-    AGI var night vs day: 20.50 %
-    >>> print('ROItotal var night vs day: %2.2f %%' % var.ROItotal)
-    ROItotal var night vs day: 248.68 %
+    >>> variation = abs(df_spectral_indices_DAY - df_spectral_indices_NIGHT)/df_spectral_indices_NIGHT*100
+    >>> print('LEQf variation night vs day: %2.2f %%' % variation['LEQf'][0]) # doctest: +NORMALIZE_WHITESPACE
+    LEQf variation night vs day: 34.94 %
+    >>> print('Hf variation night vs day: %2.2f %%' % variation['Hf'][0]) # doctest: +NORMALIZE_WHITESPACE
+    Hf variation night vs day: 105.61 %
+    >>> print('ACI variation night vs day: %2.2f %%' % variation['ACI'][0]) # doctest: +NORMALIZE_WHITESPACE
+    ACI variation night vs day: 3.39 %
+    >>> print('AGI variation night vs day: %2.2f %%' % variation['AGI'][0]) # doctest: +NORMALIZE_WHITESPACE
+    AGI variation night vs day: 20.50 %
+    >>> print('ROItotal variation night vs day: %2.2f %%' % variation['ROItotal'][0]) # doctest: +NORMALIZE_WHITESPACE
+    ROItotal variation night vs day: 264.47 %
     
     """
     
     # extent
     kwargs.update({'extent':(tn[0], tn[-1], fn[0], fn[-1])})
     
     #### get variables  
@@ -2791,14 +2847,15 @@
     mask_param1     = kwargs.pop('mask_param1',6)
     mask_param2     = kwargs.pop('mask_param2',0.5)
     remove_rain     = kwargs.pop('remove_rain',False)
     max_ratio_xy    = kwargs.pop('max_ratio_xy',10)
     
     ### for ADI, AEI, RAOQ
     bin_step = kwargs.pop('bin_step',1000) # in Hz
+    ### for ADI, AEI
     ADI_dB_threshold = kwargs.pop('ADI_dB_threshold',-50) # in dB 
     AEI_dB_threshold = kwargs.pop('AEI_dB_threshold',-50) # in dB 
     # => for same result as soundecology, we have to compute AEI and ADI outside
     # of this function as the signal can't be detrended (the dc value is not
     # removed)
     # -30 seems to give reasonable results that are more or less expected
     
@@ -2829,23 +2886,25 @@
     MEANf, VARf, SKEWf, KURTf = spectral_moments(S_amplitude)
     df_spectral_indices += [MEANf, VARf, SKEWf, KURTf]
     if verbose :
         print("MEANf %2.5f" % MEANf)
         print("VARf %2.5f" % VARf)
         print("SKEWf %2.5f" % SKEWf)
         print("KURTf %2.5f" % KURTf)
-     
+    
     """*********************** 4 audio moments per bin ********************""" 
     MEANt_per_bin, VARt_per_bin, SKEWt_per_bin, KURTt_per_bin = spectral_moments(Sxx_amplitude, axis=1) 
     MEANt_per_bin = np.asarray(MEANt_per_bin).tolist()
     VARt_per_bin = np.asarray(VARt_per_bin).tolist()
     SKEWt_per_bin = np.asarray(SKEWt_per_bin).tolist()
     KURTt_per_bin = np.asarray(KURTt_per_bin).tolist()
-    df_per_bin_indices += [MEANt_per_bin,VARt_per_bin,
-                           SKEWt_per_bin,KURTt_per_bin]
+    df_per_bin_indices += [
+                        MEANt_per_bin,VARt_per_bin,
+                        SKEWt_per_bin,KURTt_per_bin
+                        ]
     """**************************** Number of peaks ************************"""
     NBPEAKS = number_of_peaks(S_amplitude,fn,display=display)
     df_spectral_indices += [NBPEAKS]
     if verbose :
         print("NBPEAKS %2.5f" % NBPEAKS)
     
     """********* total sound pressure level in frequency domain ************"""
@@ -2855,17 +2914,19 @@
     if verbose :
         print("LEQf %2.5f" % LEQf)
     
     """************ Signal to noise Ratio and noise energy   *************"""
     """ SNRf [TOWSEY] """
     ENRf, BGNf, SNRf, ENRf_per_bin, BGNf_per_bin, SNRf_per_bin = spectral_snr(Sxx_power)
     df_spectral_indices += [ENRf, BGNf, SNRf]
-    df_per_bin_indices += [np.asarray(ENRf_per_bin).tolist(),
-                           np.asarray(BGNf_per_bin).tolist(),
-                           np.asarray(SNRf_per_bin).tolist()]
+    df_per_bin_indices += [
+                        np.asarray(ENRf_per_bin).tolist(),
+                        np.asarray(BGNf_per_bin).tolist(),
+                        np.asarray(SNRf_per_bin).tolist()
+                        ]
     if verbose :
         print("ENRf %2.5f" % ENRf)
         print("BGNf %2.5f" % BGNf)
         print("SNRf %2.5f" % SNRf)
 
     """*******************  energy concentration : entropy ****************"""
     Hf, Ht_per_bin = frequency_entropy(Sxx_power, compatibility="QUT")
@@ -2881,17 +2942,17 @@
     #### Convert into dB
     Sxx_dB_noNoise = power2dB(Sxx_power_noNoise)
 
     """******** Spectral indices from Spectrum (Amplitude or Energy) *******"""  
     """ EAS, ECU, ECV, EPS, KURT, SKEW [TOWSEY]  """
     #### Does not take into account low frequencies.
     EAS, ECU, ECV, EPS, EPS_KURT, EPS_SKEW = spectral_entropy (Sxx_power_noNoise,
-                                                               fn,
-                                                               flim=(flim_mid[0],flim_hi[1]),
-                                                               display=display)
+                                                            fn,
+                                                            flim=(flim_mid[0],flim_hi[1]),
+                                                            display=display)
     df_spectral_indices += [EAS, ECU, ECV, EPS, EPS_KURT, EPS_SKEW] 
     if verbose :
         print("EAS %2.5f" % EAS)
         print("ECU %2.5f" % ECU)
         print("ECV %2.5f" % ECV)
         print("EPS %2.5f" % EPS)
         print("EPS_KURT %2.5f" % EPS_KURT)
@@ -2913,28 +2974,28 @@
     df_per_bin_indices += [np.asarray(ACI_per_bin).tolist()]
     if verbose :
         print("ACI {seewave} %2.5f" %ACI)
 
     #### energy repartition in the frequency bins
     """ NDSI & rBA """
     NDSI, rBA, AnthroEnergy, BioEnergy = soundscape_index(Sxx_power, fn, 
-                                                         flim_bioPh=flim_mid,
-                                                         flim_antroPh=flim_low,
-                                                         R_compatible=R_compatible) 
+                                                        flim_bioPh=flim_mid,
+                                                        flim_antroPh=flim_low,
+                                                        R_compatible=R_compatible) 
     df_spectral_indices += [NDSI, rBA, AnthroEnergy, BioEnergy]
     if verbose :                                         
         if R_compatible == 'soundecology' :
             print("NDSI {soundecology} %2.5f" %NDSI)
         else :
             print("NDSI {seewave} %2.5f" %NDSI)
-   
+
     ###### Bioacoustics Index : the calculation in R from soundecology is weird...
     """ BI """
     BI = bioacoustics_index(Sxx_amplitude, fn, 
-                           flim=flim_mid, R_compatible=R_compatible) 
+                        flim=flim_mid, R_compatible=R_compatible) 
     df_spectral_indices += [BI]
     if verbose :
         if R_compatible == 'soundecology' :
             print("BI {SoundEcology} %2.5f" %BI)
         else :
             print("BI {MAAD} %2.5f" %BI)
     
@@ -2949,27 +3010,27 @@
     
     """*********** Spectral indices from the decibel spectrogram ***********"""
     #### Score
     """ ADI & AEI """ 
     """ 
         COMMENT :
                 - threshold : -50dB when norm by the max (as soundecology)
-                              6dB if PSDxxdB_SansNoise
+                            6dB if PSDxxdB_SansNoise
     """  
     ADI = acoustic_diversity_index(Sxx_amplitude, fn, fmin=flim_low[0], 
-                                 fmax=flim_mid[1], bin_step=bin_step, 
-                                 dB_threshold=ADI_dB_threshold, index="shannon") 
+                                fmax=flim_mid[1], bin_step=bin_step, 
+                                dB_threshold=ADI_dB_threshold, index="shannon") 
     AEI = acoustic_eveness_index(Sxx_amplitude, fn, fmin=flim_low[0], 
-                               fmax=flim_mid[1], bin_step=bin_step, 
-                               dB_threshold=AEI_dB_threshold) 
+                            fmax=flim_mid[1], bin_step=bin_step, 
+                            dB_threshold=AEI_dB_threshold) 
     df_spectral_indices += [ADI, AEI]
     if verbose :
         print("ADI %2.5f" %ADI)
         print("AEI %2.5f" %AEI)
-               
+    
     """************************** SPECTRAL COVER ***************************"""
     #### frequency cover 
     """ LFC, MFC, HFC [TOWSEY] """
     LFC, MFC, HFC = spectral_cover (Sxx_dB_noNoise, fn,dB_threshold=dB_threshold, 
                                     flim_LF=flim_low,flim_MF=flim_mid,flim_HF=flim_hi)
     df_spectral_indices += [LFC, MFC, HFC]
     if verbose :
@@ -2985,16 +3046,18 @@
         rejectDuration = DELTA_T * 3
     
     X = Sxx_dB_noNoise
     ACTspFract, ACTspCount, ACTspMean = spectral_activity (X, dB_threshold=dB_threshold)
     ACTspFract_avg = np.mean(ACTspFract)
     ACTspCount_avg = np.mean(ACTspCount)
     df_spectral_indices += [ACTspFract_avg, ACTspCount_avg, ACTspMean]
-    df_per_bin_indices += [np.asarray(ACTspFract).tolist(),
-                           np.asarray(ACTspCount).tolist()]
+    df_per_bin_indices += [
+                        np.asarray(ACTspFract).tolist(),
+                        np.asarray(ACTspCount).tolist()
+                        ]
     if verbose :
         print("ACTspFract %2.5f" %ACTspFract_avg)
         print("ACTspCount %2.5f" %ACTspCount_avg)
         print("ACTspMean %2.5f" %ACTspMean)
 
     EVNspFract, EVNspMean, EVNspCount, _ = spectral_events (X, 
                                                             dt=DELTA_T,
@@ -3002,26 +3065,28 @@
                                                             rejectDuration=rejectDuration,
                                                             display=display,
                                                             **kwargs)
     EVNspFract_avg = np.mean(EVNspFract)
     EVNspMean_avg = np.mean(EVNspMean)
     EVNspCount_avg = np.mean(EVNspCount)
     df_spectral_indices += [EVNspFract_avg, EVNspMean_avg, EVNspCount_avg]
-    df_per_bin_indices += [np.asarray(EVNspFract).tolist(),
-                           np.asarray(EVNspMean).tolist(),
-                           np.asarray(EVNspCount).tolist()]
+    df_per_bin_indices += [
+                        np.asarray(EVNspFract).tolist(),
+                        np.asarray(EVNspMean).tolist(),
+                        np.asarray(EVNspCount).tolist()
+                        ]
     if verbose :
         print("EVNspFract %2.5f" %mean(EVNspFract))
         print("EVNspMean %2.5f" %mean(EVNspMean))
         print("EVNspCount %2.5f" %mean(EVNspCount))
-          
+
     """**************************** New indices*****************************""" 
     """ TFSD """
     # compute TFSD with mode = ThirdOctave and flim
-    TFSD= tfsd(Sxx_amplitude,fn,tn,flim=flim_mid,mode='thirdOctave')
+    TFSD= tfsd(Sxx_amplitude,fn,tn,flim=flim_mid,mode='thirdOctave', log=True)
     df_spectral_indices += [TFSD]
     if verbose :
         print("TFSD %2.5f" % TFSD)
     
     """ More entropy"""
     X = S_power
     H_Havrda, H_Renyi, H_pairedShannon, H_gamma, H_GiniSimpson = more_entropy(X, order=3)
@@ -3041,16 +3106,18 @@
         print("RAOQ %2.2f" % RAOQ)
     
     #### Acoustic gradient index => real 1st derivative of the spectrogram
     """ AGI """
     # Time resolution (in s)
     DELTA_T = tn[1]-tn[0]
     X = Sxx_amplitude
-    _, AGI_per_bin, AGI, _ = acoustic_gradient_index(X, dt=DELTA_T, 
-                                                   order=1, norm='per_bin')
+    _, AGI_per_bin, AGI, _ = acoustic_gradient_index(
+                                                X, dt=DELTA_T, 
+                                                order=1, norm='per_bin'
+                                                )
     df_spectral_indices += [AGI]
     df_per_bin_indices += [np.asarray(AGI_per_bin).tolist()]
     if verbose :
         print("AGI %2.3f" % AGI)
     
     """ ROI index """
     # Time resolution (in s)
@@ -3061,74 +3128,74 @@
     MIN_EVENT_DUR = 30e-3
     # Minimum frequency bandwidth (in Hz)
     MIN_FREQ_BW = 100
     # Min Region Of Interest ROI
     if min_roi_area is None :
         min_roi_area = int(MIN_EVENT_DUR/DELTA_T * MIN_FREQ_BW / DELTA_F)
     ROItotal, ROIcover = region_of_interest_index(Sxx_dB_noNoise, 
-                                               tn, fn, 
-                                               smooth_param1, 
-                                               mask_mode,
-                                               mask_param1, 
-                                               mask_param2, 
-                                               min_roi=min_roi_area, 
-                                               max_roi=max_roi_area,
-                                               remove_rain = remove_rain,
-                                               max_ratio_xy = max_ratio_xy,
-                                               display=display)
+                                            tn, fn, 
+                                            smooth_param1, 
+                                            mask_mode,
+                                            mask_param1, 
+                                            mask_param2, 
+                                            min_roi=min_roi_area, 
+                                            max_roi=max_roi_area,
+                                            remove_rain = remove_rain,
+                                            max_ratio_xy = max_ratio_xy,
+                                            display=display)
     df_spectral_indices += [ROItotal, ROIcover]
     if verbose :
         print("ROItotal %2.3f" % ROItotal)
         print("ROIcover %2.3f" % ROIcover)
         
     df_spectral_indices = pd.DataFrame([df_spectral_indices], 
                                     columns=['MEANf', 
-                                             'VARf', 
-                                             'SKEWf', 
-                                             'KURTf', 
-                                             'NBPEAKS', 
-                                             'LEQf', 
-                                             'ENRf', 
-                                             'BGNf', 
-                                             'SNRf',
-                                             'Hf', 
-                                             'EAS',
-                                             'ECU',
-                                             'ECV',
-                                             'EPS',
-                                             'EPS_KURT',
-                                             'EPS_SKEW',
-                                             'ACI',
-                                             'NDSI',
-                                             'rBA',
-                                             'AnthroEnergy',
-                                             'BioEnergy',
-                                             'BI',
-                                             'ROU',
-                                             'ADI',
-                                             'AEI',
-                                             'LFC',
-                                             'MFC',
-                                             'HFC',
-                                             'ACTspFract',
-                                             'ACTspCount',
-                                             'ACTspMean', 
-                                             'EVNspFract',
-                                             'EVNspMean',
-                                             'EVNspCount',
-                                             'TFSD',
-                                             'H_Havrda',
-                                             'H_Renyi',
-                                             'H_pairedShannon', 
-                                             'H_gamma', 
-                                             'H_GiniSimpson',
-                                             'RAOQ',
-                                             'AGI',
-                                             'ROItotal',
-                                             'ROIcover'])
+                                            'VARf', 
+                                            'SKEWf', 
+                                            'KURTf', 
+                                            'NBPEAKS', 
+                                            'LEQf', 
+                                            'ENRf', 
+                                            'BGNf', 
+                                            'SNRf',
+                                            'Hf', 
+                                            'EAS',
+                                            'ECU',
+                                            'ECV',
+                                            'EPS',
+                                            'EPS_KURT',
+                                            'EPS_SKEW',
+                                            'ACI',
+                                            'NDSI',
+                                            'rBA',
+                                            'AnthroEnergy',
+                                            'BioEnergy',
+                                            'BI',
+                                            'ROU',
+                                            'ADI',
+                                            'AEI',
+                                            'LFC',
+                                            'MFC',
+                                            'HFC',
+                                            'ACTspFract',
+                                            'ACTspCount',
+                                            'ACTspMean', 
+                                            'EVNspFract',
+                                            'EVNspMean',
+                                            'EVNspCount',
+                                            'TFSD',
+                                            'H_Havrda',
+                                            'H_Renyi',
+                                            'H_pairedShannon', 
+                                            'H_gamma', 
+                                            'H_GiniSimpson',
+                                            'RAOQ',
+                                            'AGI',
+                                            'ROItotal',
+                                            'ROIcover'])
         
     df_per_bin_indices = pd.DataFrame([df_per_bin_indices], 
                                     columns=['frequencies',
                                             'LTS',
                                             'MEANt_per_bin',
                                             'VARt_per_bin', 
                                             'SKEWt_per_bin',
@@ -3145,7 +3212,11 @@
                                             'EVNspFract_per_bin',
                                             'EVNspMean_per_bin',
                                             'EVNspCount_per_bin',
                                             'AGI_per_bin'])
                                     
     return df_spectral_indices, df_per_bin_indices
 
+
+if __name__ == "__main__":
+    import doctest
+    doctest.testmod()
```

### Comparing `scikit-maad-1.3.6.1/maad/features/shape.py` & `scikit_maad-1.4.0/maad/features/shape.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # -------------------       Load modules         ---------------------------
 #***************************************************************************
 # Import external modules
 
 from __future__ import print_function 
 import numpy as np 
 import pandas as pd 
-from scipy import ndimage as ndi 
+from scipy import ndimage as ndi
 import itertools as it 
 import matplotlib.pyplot as plt 
 from skimage import transform, measure 
 from scipy import ndimage 
 
 # Import internal modules
 from maad.util import format_features, overlay_rois, plot_shape, overlay_centroid
@@ -102,15 +102,15 @@
     y0 = np.ceil(max(np.abs(n_stds * sigma_y * np.cos(theta)), 
                      np.abs(n_stds * sigma_x * np.sin(theta)), 1)) 
     y, x = np.mgrid[-y0:y0 + 1, -x0:x0 + 1] 
     # rotation matrix 
     rotx = x * np.cos(theta) + y * np.sin(theta) 
     roty = -x * np.sin(theta) + y * np.cos(theta) 
     # combine gambor and  
-    g = np.zeros(y.shape, dtype=np.complex) 
+    g = np.zeros(y.shape, dtype=complex) 
     g[:] = np.exp(-0.5 * (rotx ** 2 / sigma_x ** 2 + roty ** 2 / sigma_y ** 2)) 
     g /= 2 * np.pi * sigma_x * sigma_y # gaussian envelope 
     oscil = np.exp(1j * (2 * np.pi * frequency * rotx + offset)) # harmonic / oscilatory function 
     g_dc = g*oscil 
     # remove dc component by subtracting the envelope weighted by K 
     K = np.sum(g_dc)/np.sum(g) 
     g_nodc = g_dc - K*g 
@@ -314,61 +314,61 @@
     Returns 
     ------- 
     Sxx_out: list of 2D arrays 
         List of spectrograms filtered by each 2D kernel 
      
     Examples 
     -------- 
+    >>> import maad
     >>> from maad.sound import load, spectrogram 
     >>> from maad.features import filter_bank_2d_nodc, filter_multires 
     >>> from maad import util
     >>> s, fs = load('../data/spinetail.wav') 
     >>> Sxx, dt, df, ext = spectrogram(s, fs) 
     >>> Sxx_db = util.power2dB(Sxx, db_range=80) + 80
-    >>> util.plot2d(Sxx_db, **{'extension':ext})
+    >>> ax, fig = util.plot2d(Sxx_db, **{'extent':ext})
     >>> params, kernels = filter_bank_2d_nodc(frequency=(0.5, 0.25), ntheta=2,gamma=2) 
     >>> Sxx_out = filter_multires(Sxx, kernels, npyr=2)
     
     Plot one of the resulting spectrograms.
     
-    >>> util.plot2d(Sxx_out[5], **{'extension':ext})
+    >>> ax, fig = util.plot2d(Sxx_out[5], **{'extent':ext})
      
     """     
- 
-    # Downscale image using gaussian pyramid 
-    if npyr<2: 
-        print('Warning: npyr should be int and larger than 2 for multiresolution') 
-        im_pyr = tuple(transform.pyramid_gaussian(Sxx, downscale=2,  
-                                                  max_layer=1, multichannel=False))  
-    else:     
-        im_pyr = tuple(transform.pyramid_gaussian(Sxx, downscale=2,  
-                                                  max_layer=npyr-1, multichannel=False))  
- 
-    # filter 2d array at multiple resolutions using gabor kernels 
-    im_filt=[] 
-    for im in im_pyr:  # for each pyramid 
-        for kernel, param in kernels:  # for each kernel 
-            im_filt.append(_filter_mag(im, kernel))  #  magnitude response of filter 
-     
-    # Rescale image using gaussian pyramid 
-    if rescale: 
-        dims_raw = Sxx.shape 
-        Sxx_out=[] 
-        for im in im_filt: 
-            ratio = np.array(dims_raw)/np.array(im.shape) 
-            if ratio[0] > 1: 
-                im = transform.rescale(im, scale = ratio, mode='reflect', 
-                                       multichannel=False, anti_aliasing=True) 
-            else: 
-                pass 
-            Sxx_out.append(im) 
-    else: 
-        pass 
- 
-    return Sxx_out 
+    # Downscale image using gaussian pyramid  
+    if npyr<2:  
+        print('Warning: npyr should be int and larger than 2 for multiresolution')  
+        im_pyr = tuple(transform.pyramid_gaussian(Sxx, downscale=2,   
+                                                  max_layer=1)) 
+    else:      
+        im_pyr = tuple(transform.pyramid_gaussian(Sxx, downscale=2,   
+                                                  max_layer=npyr-1)) 
+  
+    # filter 2d array at multiple resolutions using gabor kernels  
+    im_filt=[]  
+    for im in im_pyr:  # for each pyramid  
+        for kernel, param in kernels:  # for each kernel  
+            im_filt.append(_filter_mag(im, kernel))  #  magnitude response of filter  
+      
+    # Rescale image using gaussian pyramid  
+    if rescale:  
+        dims_raw = Sxx.shape  
+        Sxx_out=[]  
+        for im in im_filt:  
+            ratio = np.array(dims_raw)/np.array(im.shape)  
+            if ratio[0] > 1:  
+                im = transform.rescale(im, scale = ratio, mode='reflect',  
+                                       anti_aliasing=True) 
+            else:  
+                pass  
+            Sxx_out.append(im)  
+    else:  
+        pass  
+  
+    return Sxx_out  
  
 #%%
 def filter_bank_2d_nodc(frequency, ntheta, bandwidth=1, gamma=2, display=False, **kwargs): 
     r""" 
     Build an ensemble of complex 2D Gabor filters with no DC offset. 
     
     A Gabor kernel is a Gaussian kernel modulated by a complex harmonic function. 
@@ -423,14 +423,16 @@
     
     See also
     --------
     filter_multires, opt_shape_presets, shape_features
     
     Examples 
     -------- 
+    >>> import maad
+
     Build a filter bank using predefined parameters with the function maad.features.opt_shape_presets.
  
     >>> from maad.features import filter_bank_2d_nodc, opt_shape_presets 
     >>> opt = opt_shape_presets(resolution='med') 
     >>> params, kernels = filter_bank_2d_nodc(opt['frequency'], opt['ntheta'], opt['bandwidth'], opt['gamma'], display=True) 
  
     Alternatively, custom parameters can be provided to define the filter bank.
@@ -481,32 +483,34 @@
         
     See also
     --------
     filter_bank_2d_nodc, filter_multires, shape_features
          
     Examples 
     -------- 
+    >>> import maad
+
     Get parameters to analyse at low, med and high shape resolutions.
      
     >>> from maad.features import opt_shape_presets 
-    >>> opt_shape_presets('low') 
+    >>> opt_shape_presets('low')  # doctest: +NORMALIZE_WHITESPACE
     {'ntheta': 2,
      'bandwidth': 0.8,
      'frequency': (0.35, 0.5),
      'gamma': 2,
      'npyr': 4}
     
-    >>> opt_shape_presets('med') 
+    >>> opt_shape_presets('med')  # doctest: +NORMALIZE_WHITESPACE
     {'ntheta': 4,
      'bandwidth': 0.8,
      'frequency': (0.35, 0.5),
      'gamma': 2,
      'npyr': 6}
     
-    >>> opt_shape_presets('high')
+    >>> opt_shape_presets('high') # doctest: +NORMALIZE_WHITESPACE
     {'ntheta': 8,
      'bandwidth': 0.8,
      'frequency': (0.35, 0.5),
      'gamma': 2,
      'npyr': 6}
     
     """ 
@@ -593,42 +597,43 @@
     ----------
     .. [1] Ulloa, J. S., Aubin, T., Llusia, D., Bouveyron, C., & Sueur, J. (2018). Estimating animal acoustic diversity in tropical environments using unsupervised multiresolution analysis. Ecological Indicators, 90, 346–355. `DOI: 10.1016/j.ecolind.2018.03.026 <https://doi.org/10.1016/j.ecolind.2018.03.026>`_
     .. [2] Sifre, L., & Mallat, S. (2013). Rotation, scaling and deformation invariant scattering for texture discrimination. Computer Vision and Pattern Recognition (CVPR), 2013 IEEE Conference On, 1233–1240. `DOI: 10.1109/CVPR.2013.163 <https://doi.org/10.1109/CVPR.2013.163>`_
     .. [3] Mallat, S. (2008). A Wavelet Tour of Signal Processing: The Sparse Way. Academic Press. `DOI: 10.1016/B978-0-12-374370-1.X0001-8 <https://doi.org/10.1016/B978-0-12-374370-1.X0001-8>`_ 
 
     Examples 
     -------- 
- 
+
     Get shape features from the whole power spectrogram 
- 
+
     >>> from maad.sound import load, spectrogram 
     >>> from maad.features import shape_features
     >>> from maad.util import format_features, power2dB, plot_shape 
     >>> s, fs = load('../data/spinetail.wav')
     >>> Sxx, tn, fn, ext = spectrogram(s, fs, db_range=100, display=True) 
     >>> Sxx_db = power2dB(Sxx, db_range=100)
     >>> shape, params = shape_features(Sxx_db, resolution='med') 
     >>> ax = plot_shape(shape.mean(), params) 
-     
+    
     Or get shape features from specific regions of interest 
-     
+    
     >>> from maad.util import read_audacity_annot
     >>> rois = read_audacity_annot('../data/spinetail.txt') 
     >>> rois = format_features(rois, tn, fn) 
     >>> shape, params = shape_features(Sxx_db, resolution='med', rois=rois)
     
     The shape coefficient can be visualized using ``plot_shape``. Note that these
     coefficient allow to disciminate between the two vocalization types found in the
     audio file, the spinetail song and the background calls.
     
     >>> shape_crer, shape_sp = shape.groupby('label')
-    >>> ax1 = plot_shape(shape_crer[1].mean(), params) 
-    >>> ax1.set_title('Spinetail song')
-    >>> ax2 = plot_shape(shape_sp[1].mean(), params) 
-    >>> ax2.set_title('Background call')
+    >>> ax1 = plot_shape(shape_crer[1].filter(regex=r'^shp_').mean(), params) 
+    >>> ax1 = ax1.set_title('Spinetail song')
+    >>> ax2 = plot_shape(shape_sp[1].filter(regex=r'^shp_').mean(), params) 
+    >>> ax2 = ax2.set_title('Background call') # doctest: +NORMALIZE_WHITESPACE
+
     """     
  
     # Check input data and unpack settings 
     if type(Sxx) is not np.ndarray and len(Sxx.shape) != 2: 
         raise TypeError('Sxx must be a numpy 2D array')   
      
     if type(resolution) is str: 
@@ -710,28 +715,29 @@
     See also
     --------
     maad.features.shape_features, maad.features.opt_shape_presets, 
     maad.features.filter_bank_2d_nodc, maad.util.plot_shape
     
     Examples
     --------
-    
+    >>> import maad
+
     Scatter the spectrogram acoustic components using 2D Gabor filters.
 
     >>> from maad.sound import load, spectrogram 
     >>> from maad.features import shape_features_raw
     >>> from maad.util import power2dB, plot2d
     >>> s, fs = load('../data/spinetail.wav')
     >>> Sxx, tn, fn, ext = spectrogram(s, fs, db_range=80, display=True) 
     >>> Sxx_db = power2dB(Sxx, db_range=80)
     >>> shape_raw, params = shape_features_raw(Sxx_db, resolution='low')
-    >>> plot2d(shape_raw[0], **{'extent':ext, 'title': 'High-frequency vertical component'})
-    >>> plot2d(shape_raw[13], **{'extent':ext, 'title': 'Low-frequency vertical components'})
-    >>> plot2d(shape_raw[2], **{'extent':ext, 'title': 'High-frequency horizontal components'})
-    >>> plot2d(shape_raw[15], **{'extent':ext, 'title': 'Low-frequency horizontal components'})
+    >>> fig, ax = plot2d(shape_raw[0], **{'extent':ext, 'title': 'High-frequency vertical component'})
+    >>> fig, ax = plot2d(shape_raw[13], **{'extent':ext, 'title': 'Low-frequency vertical components'})
+    >>> fig, ax = plot2d(shape_raw[2], **{'extent':ext, 'title': 'High-frequency horizontal components'})
+    >>> fig, ax = plot2d(shape_raw[15], **{'extent':ext, 'title': 'Low-frequency horizontal components'}) # doctest: +NORMALIZE_WHITESPACE
     """     
      
     # unpack settings 
     opt_shape = opt_shape_presets(resolution, opt_shape) 
     npyr = opt_shape['npyr'] 
     # build filterbank 
     params, kernels = filter_bank_2d_nodc(ntheta=opt_shape['ntheta'], 
@@ -773,21 +779,21 @@
     See Also
     --------
     maad.features.shape_features, maad.util.overlay_rois, 
     maad.util.format_features
  
     Examples
     --------
+    >>> import maad
  
     Get centroid from the whole power spectrogram 
  
     >>> from maad.sound import load, spectrogram
     >>> from maad.features import centroid_features
-    >>> from maad.util import (power2dB, format_features, overlay_rois, plot2d,
-                               overlay_centroid)
+    >>> from maad.util import (power2dB, format_features, overlay_rois, plot2d, overlay_centroid)
      
     Load audio and compute spectrogram 
      
     >>> s, fs = load('../data/spinetail.wav') 
     >>> Sxx,tn,fn,ext = spectrogram(s, fs, db_range=80) 
     >>> Sxx = power2dB(Sxx, db_range=80)
      
@@ -882,15 +888,15 @@
         Options for the spectrogram with keys, window length 'nperseg', 
         window overlap in percentage 'overlap' and frequency limits 'flims' 
         which is a list of 2 scalars : minimum and maximum boundary frequency  
         values in Hertz 
     display: boolean, optional, default is False 
         Flag. If display is True, plot results 
         
-    \*\*kwargs, optional. This parameter is used by plt.plot and savefig functions 
+    kwargs, optional. This parameter is used by plt.plot and savefig functions 
             
         - savefilename : str, optional, default :'_spectro_overlaycentroid.png' 
             Postfix of the figure filename 
          
         - figsize : tuple of integers, optional, default: (4,10) 
             width, height in inches.   
          
@@ -927,42 +933,68 @@
     Returns 
     ------- 
     feature_rois: pandas Dataframe 
         A dataframe with each column corresponding to a feature 
      
     Examples 
     -------- 
+    >>> import maad
     >>> from maad.util import read_audacity_annot 
     >>> from maad.sound import load 
     >>> from maad.features import all_shape_features 
     >>> s, fs = load('../data/spinetail.wav')
     >>> rois = read_audacity_annot('../data/spinetail.txt')
-    >>> features = all_shape_features(s, fs, rois, resolution='low', display=True)
-    >>> features
-        label      min_t     ...       duration_x  bandwidth_y
-        0     SP   0.101385     ...              0.0          0.0
-        1   CRER   0.506924     ...              0.0          0.0
-        2     SP   1.203945     ...              0.0          0.0
-        3     SP   2.724718     ...              0.0          0.0
-        4   CRER   5.221319     ...              0.0          0.0
-        5     SP   6.260514     ...              0.0          0.0
-        6     SP   7.946037     ...              0.0          0.0
-        7     SP   8.896519     ...              0.0          0.0
-        8     SP   9.973733     ...              0.0          0.0
-        9   CRER  11.329756     ...              0.0          0.0
-        10    SP  11.773314     ...              0.0          0.0
-        ....
-    >>> features.columns
-    Index(['label', 'min_t', 'min_f', 'max_t', 'max_f', 'min_y', 'min_x', 'max_y',
-           'max_x', 'shp_001', 'shp_002', 'shp_003', 'shp_004', 'shp_005',
-           'shp_006', 'shp_007', 'shp_008', 'shp_009', 'shp_010', 'shp_011',
-           'shp_012', 'shp_013', 'shp_014', 'shp_015', 'shp_016', 'centroid_y',
-           'centroid_x', 'duration_x', 'bandwidth_y', 'area_xy', 'centroid_f',
-           'centroid_t', 'duration_t', 'bandwidth_f', 'area_tf'],
-          dtype='object')
+    >>> features = all_shape_features(s, fs, rois, resolution='low', display=True)  # doctest: +NORMALIZE_WHITESPACE
+        number of rois : 18
+    >>> print(features.iloc[0]) # doctest: +NORMALIZE_WHITESPACE
+        label                    SP
+        min_t              0.101385
+        min_f           6441.064453
+        max_t               0.36752
+        max_f          12296.577148
+        min_y                   150
+        min_x                     8
+        max_y                   286
+        max_x                    31
+        shp_001            0.160656
+        shp_002            0.155573
+        shp_003            0.064787
+        shp_004            0.066215
+        shp_005            0.158675
+        shp_006            0.125203
+        shp_007            0.044987
+        shp_008            0.043188
+        shp_009            0.218268
+        shp_010            0.158725
+        shp_011            0.043553
+        shp_012            0.031206
+        shp_013            0.268222
+        shp_014             0.21718
+        shp_015            0.059112
+        shp_016            0.038394
+        centroid_y            220.0
+        centroid_x             19.0
+        duration_x       135.999274
+        bandwidth_y             0.0
+        area_xy               12512
+        centroid_f      9474.609375
+        centroid_t           0.2322
+        duration_t         0.267029
+        bandwidth_f      5857.03125
+        area_tf              1564.0
+        Name: 0, dtype: object
+    >>> features.columns # doctest: +NORMALIZE_WHITESPACE
+        Index(['label', 'min_t', 'min_f', 'max_t', 'max_f', 'min_y', 'min_x', 'max_y',
+            'max_x', 'shp_001', 'shp_002', 'shp_003', 'shp_004', 'shp_005',
+            'shp_006', 'shp_007', 'shp_008', 'shp_009', 'shp_010', 'shp_011',
+            'shp_012', 'shp_013', 'shp_014', 'shp_015', 'shp_016', 'centroid_y',
+            'centroid_x', 'duration_x', 'bandwidth_y', 'area_xy', 'centroid_f',
+            'centroid_t', 'duration_t', 'bandwidth_f', 'area_tf'],
+            dtype='object')
+
     """    
    
     # Spectro computing
     N=1024
     window  = kwargs.pop('window','hann')
     nperseg = kwargs.pop('nperseg',N) 
     overlap = kwargs.pop('overlap',N//2)  
@@ -981,15 +1013,15 @@
     
     # dB scale
     Sxx = 10*np.log10(Sxx)
      
     # format rois to bbox 
     rois = format_features(rois, tn, fn) 
     
-    # if rois becomes empty aveter format_features
+    # if rois becomes empty after format_features
     if rois.empty :
         print ('rois is empty')
         features = rois
         return features
     else:
         print('number of rois : %d' % len(rois))
      
@@ -1009,19 +1041,22 @@
     if display :
         # view bbox
         ax, fig = overlay_rois(Sxx, rois, vmin=vmin, vmax=vmax, **kwargs)
         # view centroids
         overlay_centroid(Sxx, centroid, savefig=None, 
                          fig=fig, ax=ax, **kwargs)
         # plot shape
-        plot_shape(shape.mean(), params)
+        plot_shape(shape.filter(regex=r'^shp_').mean(), params)
     
     # combine into a single df without columns duplication
     features = pd.concat([rois, shape, centroid], axis=1, sort=False)
     features = features.loc[:,~features.columns.duplicated()]
     
     if verbose : 
         print('list of features')
         print(list(features))
      
     return features 
- 
+
+if __name__ == "__main__":
+    import doctest
+    doctest.testmod()
```

### Comparing `scikit-maad-1.3.6.1/maad/rois/rois_1d.py` & `scikit_maad-1.4.0/maad/rois/rois_1d.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,28 +58,28 @@
     if onset[-1] > offset[-1]:      # check end
         offset = np.append(offset,tmax)
     else:
         pass
     return onset, offset
 
 #%%
-def _energy_windowed(s, wl=512, fs=None):
+def _energy_windowed(s, fs: float, wl: int=512):
     """ 
     Computse windowed energy on an audio signal.
     
     Computes the energy of the signals by windows of length wl. Used to amplify sectors where the density of energy is higher
     
     Parameters
     ----------
     s : ndarray
         input signal
-    wl : float
-        length of the window to summarize the rms value
     fs : float
         frequency sampling of the signal, used to keep track of temporal information of the signal
+    wl : int, default is 512
+        length of the window to summarize the rms value
 
     Returns
     -------
     time : ndarray
         temporal index vector
     s_rms : ndarray
         windowed rms signal
@@ -93,15 +93,15 @@
     time = np.arange(0,len(s_rms)) * wl / fs + wl*0.5/fs
     return time, s_rms
 
 #%%
 # =============================================================================
 # Public functions
 # =============================================================================
-def find_rois_cwt(s, fs, flims, tlen, th=0, display=False, save_df=False, 
+def find_rois_cwt(s, fs, flims, tlen, th: float=0, display=False, save_df=False, 
                   savefilename='rois.csv', **kwargs):
     """
     Find region of interest using known estimates of signal length and frequency limits.
     
     The general approach is based on continous wavelet transform following a three step process
     
     1. Filter the signal with a bandpass sinc filter
@@ -110,14 +110,16 @@
     
     3. Binarize the signal applying a linear threshold
         
     Parameters
     ----------
     s : ndarray
         input signal
+    fs : float
+        frequency sampling of the signal, used to keep track of temporal information of the signal
     flims : int
         upper and lower frequencies (in Hz) 
     tlen : int 
         temporal length of signal searched (in s)
     th : float, optional
         threshold to binarize the output
     display: boolean, optional, default is False
@@ -135,33 +137,33 @@
     References
     ----------
     .. [1] Pan Du, Warren A. Kibbe, Simon M. Lin, Improved peak detection in mass spectrum by incorporating continuous wavelet transform-based pattern matching, Bioinformatics, Volume 22, Issue 17, 1 September 2006, Pages 2059–2065, `DOI: 10.1093/bioinformatics/btl355 <https://doi.org/10.1093/bioinformatics/btl355>`_ 
     
     Examples
     --------
     >>> from maad import sound, rois
-    >>> s, fs = sound.load('./data/spinetail.wav')
+    >>> s, fs = sound.load('../data/spinetail.wav')
     >>> rois.find_rois_cwt(s, fs, flims=(4500,8000), tlen=2, th=0, display=True)
         min_f     min_t   max_f     max_t
     0  4500.0   0.74304  8000.0   2.50776
     1  4500.0   5.10839  8000.0   7.33751
     2  4500.0  11.23846  8000.0  13.37469
     3  4500.0  16.16109  8000.0  18.29732
     """
     # filter signal
     s_filt = sinc(s, flims, fs, atten=80, transition_bw=0.8)
     # rms: calculate window of maximum 5% of tlen. improves speed of cwt
     wl = 2**np.floor(np.log2(tlen*fs*0.05)) 
-    t, s_rms = _energy_windowed(s_filt, int(wl), fs)
+    t, s_rms = _energy_windowed(s_filt, fs, int(wl))
     # find peaks
     cwt_width = [round(tlen*fs/wl/2)]
     npad = 5 ## seems to work with 3, but not sure
-    s_rms = np.pad(s_rms, np.int(cwt_width[0]*npad), 'reflect')  ## add pad
+    s_rms = np.pad(s_rms, np.int64(cwt_width[0]*npad), 'reflect')  ## add pad
     s_cwt = signal.cwt(s_rms, signal.ricker, cwt_width)
-    s_cwt = s_cwt[0][np.int(cwt_width[0]*npad):len(s_cwt[0])-np.int(cwt_width[0]*npad)] ## rm pad
+    s_cwt = s_cwt[0][np.int64(cwt_width[0]*npad):len(s_cwt[0])-np.int64(cwt_width[0]*npad)] ## rm pad
     # find onset and offset of sound
     segments_bin = np.array(s_cwt > th)
     onset = t[np.where(np.diff(segments_bin.astype(int)) > 0)]+t[0]  # there is delay because of the diff that needs to  be accounted
     offset = t[np.where(np.diff(segments_bin.astype(int)) < 0)]+t[0]
     # format for output
     if onset.size==0 or offset.size==0:
     # No detection found
@@ -178,15 +180,15 @@
                                 np.repeat(flims[1],repeats=len(onset)),
                                 np.round(offset,5)])
         cols=['min_f', 'min_t','max_f', 'max_t']
         df = pd.DataFrame(data=rois_tf,columns=cols)
         if save_df==True:
             df.to_csv(savefilename, sep=',', header=True, index=False)
 
-    #%% Display
+    # Display
     if display==True: 
         figsize = kwargs.pop('figsize',(12,6))
         cmap = kwargs.pop('cmap','gray')
         nfft = kwargs.pop('nperseg',512)
         noverlap = kwargs.pop('noverlap',512)
         nperseg = kwargs.pop('nperseg',1024)
         db_range = kwargs.pop('db_range',80)
@@ -200,16 +202,21 @@
         ax1.hlines(th, 0, len(s_cwt), linestyles='dashed', colors='r')
         #plot spectrogram
         Sxx, tn, fn, ext = sound.spectrogram(s, fs, nperseg = nperseg, noverlap=noverlap, mode='psd')
         util.plot_spectrogram(Sxx, ext, db_range, ax=ax2, colorbar=False)
         ax2.set_ylabel('Frequency (Hz)')
         ax2.set_xlabel('Time (s)')
         if not(df.empty):
-            for idx, _ in df.iterrows():
-                xy = (df.min_t[idx],df.min_f[idx])
-                width = df.max_t[idx] - df.min_t[idx]
-                height = df.max_f[idx] - df.min_f[idx]
+            for idx, row in df.iterrows():
+                xy = (row.min_t, row.min_f)
+                width = row.max_t- row.min_t
+                height = row.max_f- row.min_f
                 rect = patches.Rectangle(xy, width, height, lw=1, 
-                                         edgecolor='r', facecolor='none')
+                                        edgecolor='yellow', facecolor='none')
                 ax2.add_patch(rect)
         plt.show()
+    
     return df
+
+if __name__ == "__main__":
+    import doctest
+    doctest.testmod()
```

### Comparing `scikit-maad-1.3.6.1/maad/rois/rois_2d.py` & `scikit_maad-1.4.0/maad/rois/rois_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     display : boolean, optional, default is False 
         Display the signal if True 
          
     savefig : string, optional, default is None 
         Root filename (with full path) is required to save the figures. Postfix 
         is added to the root filename. 
          
-    \*\*kwargs, optional. This parameter is used by plt.plot and savefig functions 
+    kwargs, optional. This parameter is used by plt.plot and savefig functions 
              
         - savefilename : str, optional, default :'_spectro_after_noise_subtraction.png' 
             Postfix of the figure filename 
           
         - figsize : tuple of integers, optional, default: (4,10) 
             width, height in inches.   
          
@@ -227,15 +227,15 @@
     display : boolean, optional, default is False 
         Display the signal if True 
          
     savefig : string, optional, default is None 
         Root filename (with full path) is required to save the figures. Postfix 
         is added to the root filename. 
          
-    \*\*kwargs, optional. This parameter is used by plt.plot and savefig functions 
+    kwargs, optional. This parameter is used by plt.plot and savefig functions 
            
         - savefilename : str, optional, default :'_spectro_after_noise_subtraction.png' 
             Postfix of the figure filename 
          
         - figsize : tuple of integers, optional, default: (4,10) 
             width, height in inches.   
          
@@ -361,29 +361,29 @@
     Parameters 
     ---------- 
     im : 2d ndarray of scalars 
         Spectrogram (or image) 
  
     mode_bin : string in {'relative', 'absolute'}, optional, default is 'relative' 
         if 'absolute' [1]_ , a double threshold with absolute value is performed 
-        with two parameters (see \*\*kwargs section)
+        with two parameters (see kwargs section)
         if 'relative' [2]_, a relative double threshold is performed with two 
-        parameters (see \*\*kwargs section)
+        parameters (see kwargs section)
 
     verbose : boolean, optional, default is False
         print messages
          
     display : boolean, optional, default is False 
         Display the signal if True 
          
     savefig : string, optional, default is None 
         Root filename (with full path) is required to save the figures. Postfix 
         is added to the root filename. 
          
-    \*\*kwargs, optional. This parameter is used by the maad functions as well 
+    kwargs, optional. This parameter is used by the maad functions as well 
         as the plt.plot and savefig functions. 
         All the input arguments required or optional in the signature of the 
         functions above can be passed as kwargs : 
         
         if 'absolute' [1]_ 
         - bin_h : scalar, optional, default is 0.7 
         Set the first threshold. Value higher than this value are set to 1,  
@@ -418,14 +418,16 @@
     References
     ----------
     .. [1] J. Canny. A computational approach to edge detection. IEEE Transactions on Pattern Analysis and Machine Intelligence. 1986; vol. 8, pp.679-698. `DOI: 10.1109/TPAMI.1986.4767851 <https://doi.org/10.1109/TPAMI.1986.4767851>`_
     .. [2] from MATLAB: Threshold estimation (Oliveira et al, 2015) 
      
     Examples 
     -------- 
+
+    >>> import maad
     
     Load audio recording and convert it into spectrogram
     
     >>> s, fs = maad.sound.load('../data/cold_forest_daylight.wav')
     >>> Sxx,tn,fn,ext = maad.sound.spectrogram (s, fs, fcrop=(0,10000))   
     
     Convert linear spectrogram into dB
@@ -440,16 +442,16 @@
     
     >>> im_bin = maad.rois.create_mask(Sxx_dB_blurred, bin_std=1.5, bin_per=0.25, mode='relative') 
     
     Plot spectrograms
     
     >>> import matplotlib.pyplot as plt 
     >>> fig, (ax1, ax2) = plt.subplots(2, 1)
-    >>> maad.util.plot2d(Sxx_dB, ax=ax1, extent=ext, title='original', vmin=10, vmax=70)
-    >>> maad.util.plot2d(im_bin, ax=ax2, extent=ext, title='mask')
+    >>> ax1, fig = maad.util.plot2d(Sxx_dB, ax=ax1, extent=ext, title='original', vmin=10, vmax=70)
+    >>> ax2, fig = maad.util.plot2d(im_bin, ax=ax2, extent=ext, title='mask')
     >>> fig.set_size_inches(13,8)
     >>> fig.tight_layout() 
     
     """ 
         
     if mode_bin == 'relative': 
         bin_std=kwargs.pop('bin_std', 6)  
@@ -489,15 +491,15 @@
     display : boolean, optional, default is False 
         Display the signal if True 
          
     savefig : string, optional, default is None 
         Root filename (with full path) is required to save the figures. Postfix 
         is added to the root filename. 
          
-    \*\*kwargs, optional. This parameter is used by plt.plot and savefig functions 
+    kwargs, optional. This parameter is used by plt.plot and savefig functions 
             
         - savefilename : str, optional, default :'_spectro_after_noise_subtraction.png' 
             Postfix of the figure filename 
          
         - figsize : tuple of integers, optional, default: (4,10) 
             width, height in inches.   
          
@@ -546,42 +548,62 @@
         Array have column names: ``labelID``, ``label``, ``min_y``, ``min_x``,
         ``max_y``, ``max_x``,
         Use the function ``maad.util.format_features`` before using 
         centroid_features to format of the ``rois`` DataFrame 
         correctly.
         
     Examples 
-    -------- 
+    --------
+    >>> import maad
     
     Load audio recording compute the spectrogram in dB.
     
     >>> s, fs = maad.sound.load('../data/cold_forest_daylight.wav')
-    >>> Sxx,tn,fn,ext = maad.sound.spectrogram (s, fs, fcrop=(0,20000), display=True)           
+    >>> Sxx,tn,fn,ext = maad.sound.spectrogram (s, fs, flims=(0,20000), display=True)           
     >>> Sxx_dB = maad.util.power2dB(Sxx) +96
     
     Smooth the spectrogram
     
     >>> Sxx_dB_blurred = maad.sound.smooth(Sxx_dB)
     
      Using image binarization, detect isolated region in the time-frequency domain with high density of energy, i.e. regions of interest (ROIs).
     
     >>> im_bin = maad.rois.create_mask(Sxx_dB_blurred, bin_std=1.5, bin_per=0.5, mode='relative')
     
     Select ROIs from the binary mask.
     
     >>> im_rois, df_rois = maad.rois.select_rois(im_bin, display=True)
-    
+    >>> print('Without subtracted the background noise, only {} ROIs have been segmented'.format(len(df_rois)))
+    Without subtracted the background noise, only 13 ROIs have been segmented
+    >>> df_rois.iloc[-1]
+    labelID         13
+    label      unknown
+    min_y          162
+    min_x         1105
+    max_y          193
+    max_x         1127
+    Name: 12, dtype: object
+
     We detected the background noise as a ROI, and that multiple ROIs are mixed in a single region. To have better results, it is adviced to preprocess the spectrogram to remove the background noise before creating the mask.
     
     >>> Sxx_noNoise = maad.sound.median_equalizer(Sxx)
     >>> Sxx_noNoise_dB = maad.util.power2dB(Sxx_noNoise)     
     >>> Sxx_noNoise_dB_blurred = maad.sound.smooth(Sxx_noNoise_dB)        
     >>> im_bin2 = maad.rois.create_mask(Sxx_noNoise_dB_blurred, bin_std=6, bin_per=0.5, mode='relative') 
     >>> im_rois2, df_rois2 = maad.rois.select_rois(im_bin2, display=True)
-    
+    >>> print('{} ROIs have been segmented'.format(len(df_rois2)))
+    274 ROIs have been segmented
+    >>> df_rois2.iloc[-1]
+    labelID        274
+    label      unknown
+    min_y          214
+    min_x         4485
+    max_y          230
+    max_x         4494
+    Name: 273, dtype: object
     """ 
  
     # test if max_roi and min_roi are defined 
     if max_roi is None:  
         # the maximum ROI is set to the aera of the image 
         max_roi=im_bin.shape[0]*im_bin.shape[1] 
          
@@ -645,14 +667,15 @@
             ylabel = 'pseudofrequency [points]'
          
         # randcmap = rand_cmap(len(rois_label)) 
         # cmap   =kwargs.pop('cmap',randcmap)  
         cmap   =kwargs.pop('cmap','tab20') 
          
         _, fig = plot2d (im_rois, 
+                         interpolation = 'none',
                          extent = extent,
                          title  = title,  
                          ylabel = ylabel, 
                          xlabel = xlabel,
                          cmap   = cmap, 
                          **kwargs) 
         # SAVE FIGURE 
@@ -689,15 +712,15 @@
     --------
     >>> from maad import rois, util
     >>> import pandas as pd
     >>> import numpy as np
     >>> im_zeros = np.zeros((100,300))
     >>> df_rois = pd.DataFrame({'min_y': [10, 40], 'min_x': [10, 200], 'max_y': [60, 80], 'max_x': [110, 250]})
     >>> im_blobs = rois.rois_to_imblobs(im_zeros, df_rois)
-    >>> util.plot2d(im_blobs)
+    >>> ax, fig = util.plot2d(im_blobs)
     """ 
     # Check format of the input data 
     if type(rois) is not pd.core.frame.DataFrame : 
         raise TypeError('Rois must be of type pandas DataFrame')   
          
     if not(('min_y' and 'min_x' and 'max_y' and 'max_x')  in rois)  : 
             raise TypeError('Array must be a Pandas DataFrame with column names:((min_y, min_x, max_y, max_x). Check example in documentation.')   
@@ -708,9 +731,10 @@
     for min_y, min_x, max_y, max_x in rois_bbox.values: 
         im_zeros[int(min_y):int(max_y+1), int(min_x):int(max_x+1)] = 1 
      
     im_blobs = im_zeros.astype(int) 
      
     return im_blobs 
 
- 
- 
+if __name__ == "__main__":
+    import doctest
+    doctest.testmod()
```

### Comparing `scikit-maad-1.3.6.1/maad/sound/__init__.py` & `scikit_maad-1.4.0/maad/sound/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-maad-1.3.6.1/maad/sound/filter.py` & `scikit_maad-1.4.0/maad/sound/filter.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 
 # =============================================================================
 # Load the modules
 # =============================================================================
 # Import external modules
 import numpy as np
 import matplotlib.pyplot as plt
-from scipy.signal import (sosfiltfilt, convolve, iirfilter, get_window, 
-                          kaiserord, firwin, lfilter)
+from scipy.signal import (
+    sosfiltfilt, convolve, iirfilter, get_window, 
+    kaiserord, firwin, lfilter
+    )
 from skimage import filters
 
 # Import internal modules 
 from maad.util import plot2d
 
 #%%
 # =============================================================================
 # public functions
 # =============================================================================
 def select_bandwidth (x, fs, fcut, forder, fname ='butter', ftype='bandpass', 
-                     rp=None, rs=None):
+                    rp=None, rs=None):
     """
     Use a lowpass, highpass, bandpass or bandstop filter to process a 1d signal with an iir filter.
         
     Parameters
     ----------
     x : array_like
         1d vector of scalars to be filtered
@@ -67,43 +69,49 @@
     See Also
     --------
     fir_filter1d
         Lowpass, highpass, bandpass or bandstop a 1d signal with an Fir filter
     
     Examples
     --------
+    >>> import maad
+
     Load and display the spectrogram of a sound waveform
     
     >>> w, fs = maad.sound.load('../data/cold_forest_daylight.wav') 
     >>> Sxx_power,tn,fn,_ = maad.sound.spectrogram(w,fs)
-    >>> Sxx_dB = maad.util.power2dB(Sxx_power) # convert into dB 
-    >>> fig_kwargs = {'vmax': Sxx_dB.max(),
-                      'vmin':-90,
-                      'extent':(tn[0], tn[-1], fn[0], fn[-1]),
-                      'figsize':(4,13),
-                      'title':'Power spectrogram density (PSD)',
-                      'xlabel':'Time [sec]',
-                      'ylabel':'Frequency [Hz]',
-                      }
-    >>> fig1, ax1 = maad.util.plot2d(Sxx_dB, **fig_kwargs)
+    >>> Sxx_dB = maad.spl.power2dBSPL(Sxx_power, gain=42) # convert into dB SPL
+    >>> fig_kwargs = {'vmax': Sxx_dB.max(),\
+                    'vmin':0,\
+                    'extent':(tn[0], tn[-1], fn[0], fn[-1]),\
+                    'figsize':(4,13),\
+                    'title':'Power spectrogram density (PSD)',\
+                    'xlabel':'Time [sec]',\
+                    'ylabel':'Frequency [Hz]',\
+                    }
+    >>> ax, fig = maad.util.plot2d(Sxx_dB, **fig_kwargs)
+    >>> print('The energy in the spectrogram is {} dB SPL'.format(maad.util.add_dB(maad.util.add_dB(Sxx_dB))))
+    The energy in the spectrogram is 90.68996875800728 dB SPL
     
     Filter the waveform : keep the bandwidth between 6-10kHz
     
     >>> w_filtered = maad.sound.select_bandwidth(w,fs,fcut=(6000,10000), forder=5, fname ='butter', ftype='bandpass')
     >>> Sxx_power_filtered,tn,fn,_ = maad.sound.spectrogram(w_filtered,fs)
-    >>> Sxx_dB_filtered = maad.util.power2dB(Sxx_power_filtered) # convert into dB 
-    >>> maad.util.plot2d(Sxx_dB_filtered, **fig_kwargs)
-    
+    >>> Sxx_dB_filtered = maad.spl.power2dBSPL(Sxx_power_filtered, gain=42) # convert into dB SPL
+    >>> ax, fig = maad.util.plot2d(Sxx_dB_filtered, **fig_kwargs)
+    >>> print('The energy in the spectrogram is {} dB SPL'.format(maad.util.add_dB(maad.util.add_dB(Sxx_dB_filtered))))
+    The energy in the spectrogram is 72.75045485363799 dB SPL
+
     """
     sos = iirfilter(N=forder, Wn=np.asarray(fcut)/(fs/2), btype=ftype,ftype=fname, rp=rp, 
-                     rs=rs, output='sos')
+                    rs=rs, output='sos')
     # use sosfiltfilt insteasd of sosfilt to keep the phase of y matches x
     y = sosfiltfilt(sos, x)
     return y
- 
+
 #%%
 def fir_filter(x, kernel, axis=0):
     """
     Filter a signal using a 1d finite impulse response filter.
     
     This function uses a digital filter based on convolution of 1d kernel over a vector 
     or along an axis of a matrix.
@@ -144,41 +152,51 @@
     See Also
     --------
     select_bandwidth
         Lowpass, highpass, bandpass or bandstop a 1d signal with an iir filter
     
     Examples
     --------  
+    >>> import maad
     
     Load and display the spectrogram of a sound waveform
     
     >>> w, fs = maad.sound.load('../data/cold_forest_daylight.wav') 
     >>> Sxx_power, tn, fn, ext = maad.sound.spectrogram(w,fs)
     >>> Lxx = maad.spl.power2dBSPL(Sxx_power, gain=42) # convert into dB SPL
-    >>> fig_kwargs = {'vmax': Lxx.max(),
-                      'vmin':0,
-                      'extent': ext,
-                      'figsize': (4,13),
-                      'title': 'Power spectrogram density (PSD)',
-                      'xlabel': 'Time [sec]',
-                      'ylabel': 'Frequency [Hz]',
-                      }
-    >>> fig, ax = maad.util.plot2d(Lxx,**fig_kwargs)
+    >>> fig_kwargs = {'vmax': Lxx.max(),\
+                    'vmin':0,\
+                    'extent': ext,\
+                    'figsize': (4,13),\
+                    'title': 'Power spectrogram density (PSD)',\
+                    'xlabel': 'Time [sec]',\
+                    'ylabel': 'Frequency [Hz]',\
+                    }
+    >>> ax, fig = maad.util.plot2d(Lxx,**fig_kwargs)
+
+    >>> print('The energy in the spectrogram is {} dB SPL'.format(maad.util.add_dB(maad.util.add_dB(Lxx))))
+    The energy in the spectrogram is 90.68996875800728 dB SPL
     
     Smooth the waveform (lowpass)
     
     >>> w_filtered = maad.sound.fir_filter(w, kernel=(('gaussian', 2), 5))
     >>> Sxx_power_filtered,tn,fn,_ = maad.sound.spectrogram(w_filtered,fs)
     >>> Lxx_filtered = maad.spl.power2dBSPL(Sxx_power_filtered, gain=42) # convert into dB SPL
-    >>> fig, ax = maad.util.plot2d(Lxx_filtered,**fig_kwargs)
+    >>> ax, fig = maad.util.plot2d(Lxx_filtered,**fig_kwargs)
+
+    >>> print('The energy in the spectrogram is {} dB SPL'.format(maad.util.add_dB(maad.util.add_dB(Lxx_filtered))))
+    The energy in the spectrogram is 89.51776241848223 dB SPL
     
     Smooth the spectrogram, frequency by frequency (blurr)
     
     >>> Lxx_blurr = maad.sound.fir_filter(Lxx, kernel=(('gaussian', 1), 5), axis=1)
-    >>> fig, ax = maad.util.plot2d(Lxx_blurr,**fig_kwargs)
+    >>> ax, fig = maad.util.plot2d(Lxx_blurr,**fig_kwargs)
+
+    >>> print('The energy in the spectrogram is {} dB SPL'.format(maad.util.add_dB(maad.util.add_dB(Lxx_blurr))))
+    The energy in the spectrogram is 88.83611122906812 dB SPL
     
     """
     if isinstance(kernel,tuple) :
         if len(kernel) ==1 :
             win = get_window(kernel[0])
         if len(kernel) ==2 :
             win = get_window(kernel[0], kernel[1])
@@ -231,111 +249,119 @@
     Returns
     -------
     s_filt : array 
         signal filtered
     
     Examples
     --------
+    >>> import maad
     >>> s, fs = maad.sound.load('../data/spinetail.wav')
     >>> import numpy as np
     >>> tn = np.arange(0,len(s))/fs
     >>> s_filt_7_12kHz = maad.sound.sinc(s, cutoff=[7000,12000], fs=fs, atten=80, transition_bw=0.8)
     >>> s_filt_4_8kHz = maad.sound.sinc(s, cutoff=[4500,8000], fs=fs, atten=80, transition_bw=0.8)
     >>> import matplotlib.pyplot as plt
     >>> fig, (ax0, ax1,ax2) = plt.subplots(3,1, sharex=True, squeeze=True)
-    >>> maad.util.plot1d(tn,s,ax=ax0, figtitle='original')
-    >>> maad.util.plot1d(tn,s_filt_7_12kHz,ax=ax1, figtitle='Kaiser-windowed filter 7-12kHz')
-    >>> maad.util.plot1d(tn,s_filt_4_8kHz,ax=ax2, figtitle='Kaiser-windowed filter 4.5-8kHz')
+    >>> ax0, fig = maad.util.plot1d(tn,s,ax=ax0, figtitle='original')
+    >>> ax1, fig = maad.util.plot1d(tn,s_filt_7_12kHz,ax=ax1, figtitle='Kaiser-windowed filter 7-12kHz')
+    >>> a2 , fig = maad.util.plot1d(tn,s_filt_4_8kHz,ax=ax2, figtitle='Kaiser-windowed filter 4.5-8kHz')
     >>> fig.tight_layout()
     
     """
     width = (cutoff[1] - cutoff[0]) * transition_bw
     numtaps, beta = kaiserord(atten, width/(0.5*fs))
     np.ceil(numtaps-1) // 2 * 2 + 1  # round to nearest odd to have Type I filter
-    taps = firwin(numtaps, cutoff, window=('kaiser', beta), 
-                         scale=False, nyq=0.5*fs, pass_zero=not(bandpass))
+    taps = firwin(
+        numtaps, 
+        cutoff, 
+        window=('kaiser', beta), 
+        scale=False, 
+        nyq=0.5*fs, 
+        pass_zero=not(bandpass)
+        )
     s_filt = lfilter(taps, 1, s)
     return s_filt
 
 #%%
-def smooth (Sxx, std=1, verbose=False, display = False, savefig=None, **kwargs): 
+def smooth (Sxx, std: float=1, verbose=False, display = False, savefig=None, **kwargs): 
     """ 
     Smooth a spectrogram with a gaussian filter.
-     
+    
     Parameters 
     ---------- 
     Sxx : 2d ndarray of scalars 
         Spectrogram (or image) 
-     
+    
     std : scalar, optional, default is 1 
         Standard deviation of the gaussian kernel used to smooth the spectrogram.
         The larger is the number, the smoother will be the image and the longer 
         it takes. Standard values should fall between 0.5 and 3.
     
     verbose : boolean, optional, default is False 
         Print messages
     
     display : boolean, optional, default is False 
         Display the signal if True 
-         
+        
     savefig : string, optional, default is None 
         Root filename (with full path) is required to save the figures. Postfix 
         is added to the root filename. 
-         
-    \*\*kwargs, optional. This parameter is used by plt.plot and savefig functions 
-             
+        
+    kwargs, optional. This parameter is used by plt.plot and savefig functions 
+        
         - savefilename : str, optional, default :'_spectro_after_noise_subtraction.png' 
             Postfix of the figure filename 
-          
+        
         - extent : list of scalars [left, right, bottom, top], optional, default: None
             The location, in data-coordinates, of the lower-left and
             upper-right corners. If `None`, the image is positioned such that
             the pixel centers fall on zero-based (row, column) indices.
-         
+        
         - title : string, optional, default : 'Spectrogram' 
             title of the figure 
-         
+        
         - xlabel : string, optional, default : 'Time [s]' 
             label of the horizontal axis 
-         
+        
         - ylabel : string, optional, default : 'Amplitude [AU]' 
             label of the vertical axis 
-         
+        
         - cmap : string or Colormap object, optional, default is 'gray' 
             See https://matplotlib.org/examples/color/colormaps_reference.html 
             in order to get all the  existing colormaps 
             examples: 'hsv', 'hot', 'bone', 'tab20c', 'jet', 'seismic',  
             'viridis'... 
-         
+        
         - vmin, vmax : scalar, optional, default: None 
             `vmin` and `vmax` are used in conjunction with norm to normalize 
             luminance data.  Note if you pass a `norm` instance, your 
             settings for `vmin` and `vmax` will be ignored. 
-         
+        
         - extent : scalars (left, right, bottom, top), optional, default: None 
             The location, in data-coordinates, of the lower-left and 
             upper-right corners. If `None`, the image is positioned such that 
             the pixel centers fall on zero-based (row, column) indices. 
-         
+        
         - dpi : integer, optional, default is 96 
             Dot per inch.  
             For printed version, choose high dpi (i.e. dpi=300) => slow 
             For screen version, choose low dpi (i.e. dpi=96) => fast 
-         
+        
         - format : string, optional, default is 'png' 
             Format to save the figure 
-             
+            
         ... and more, see matplotlib    
-         
+        
     Returns 
     ------- 
     im_out: smothed or blurred image  
     
     Examples
     --------
+    >>> import maad
     
     Load audio recording and convert it into spectrogram
     
     >>> s, fs = maad.sound.load('../data/cold_forest_daylight.wav')
     >>> Sxx,tn,fn,ext = maad.sound.spectrogram (s, fs, tcrop=(5,10), fcrop=(0,10000))   
     
     Convert linear spectrogram into dB
@@ -348,30 +374,30 @@
     >>> Sxx_dB_std10 = maad.sound.smooth(Sxx_dB, std=1)
     >>> Sxx_dB_std15 = maad.sound.smooth(Sxx_dB, std=1.5)
     
     Plot spectrograms
     
     >>> import matplotlib.pyplot as plt 
     >>> fig, (ax1, ax2, ax3, ax4) = plt.subplots(4, 1)
-    >>> maad.util.plot2d(Sxx_dB, ax=ax1, extent=ext, title='original', vmin=10, vmax=70)
-    >>> maad.util.plot2d(Sxx_dB_std05, ax=ax2, extent=ext, title='smooth (std=0.5)', vmin=10, vmax=70)
-    >>> maad.util.plot2d(Sxx_dB_std10, ax=ax3, extent=ext, title='smooth (std=1)', vmin=10, vmax=70)
-    >>> maad.util.plot2d(Sxx_dB_std15, ax=ax4, extent=ext, title='smooth (std=1.5)', vmin=10, vmax=70)
+    >>> ax1, fig = maad.util.plot2d(Sxx_dB, ax=ax1, extent=ext, title='original', vmin=10, vmax=70)
+    >>> ax2, fig = maad.util.plot2d(Sxx_dB_std05, ax=ax2, extent=ext, title='smooth (std=0.5)', vmin=10, vmax=70)
+    >>> ax3, fig = maad.util.plot2d(Sxx_dB_std10, ax=ax3, extent=ext, title='smooth (std=1)', vmin=10, vmax=70)
+    >>> ax4, fig = maad.util.plot2d(Sxx_dB_std15, ax=ax4, extent=ext, title='smooth (std=1.5)', vmin=10, vmax=70)
     >>> fig.set_size_inches(7,9)
     >>> fig.tight_layout() 
     
     """ 
     
     if verbose:
         print(72 * '_') 
         print('Smooth the image with a gaussian filter (std = %.1f)' %std) 
-     
+    
     # use scikit image (faster than scipy) 
     Sxx_out = filters.gaussian(Sxx,std) 
-     
+    
     # Display 
     if display :  
         ylabel =kwargs.pop('ylabel','Frequency [Hz]') 
         xlabel =kwargs.pop('xlabel','Time [sec]')   
         cmap   =kwargs.pop('cmap','gray')  
         vmin=kwargs.pop('vmin',np.percentile(Sxx_out,0.1)) 
         vmax=kwargs.pop('vmax',np.percentile(Sxx_out,99.9)) 
@@ -401,8 +427,11 @@
             format=kwargs.pop('format','png') 
             filename=kwargs.pop('filename','_spectro_blurr')              
             filename = savefig+filename+'.'+format 
             print('\n''save figure : %s' %filename) 
             fig.savefig(filename, bbox_inches='tight', dpi=dpi, format=format, 
                         **kwargs)    
     return Sxx_out 
- 
+
+if __name__ == "__main__":
+    import doctest
+    doctest.testmod()
```

### Comparing `scikit-maad-1.3.6.1/maad/sound/input_output.py` & `scikit_maad-1.4.0/maad/sound/input_output.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # License: New BSD License
 
 # =============================================================================
 # Load the modules
 # =============================================================================
 # Import external modules
 import numpy as np
-from warnings import warn
+import warnings
 import io
 from urllib.request import urlopen
 from scipy.io import wavfile 
 from skimage.io import imread 
 from scipy.io.wavfile import write as write_wav
 
 # Import internal modules
@@ -46,15 +46,15 @@
     verbose : boolean, optional, default is False
         Print messages into the console or terminal if verbose is True
     display : boolean, optional, default is False
         Display the signal if True
     savefig : string, optional, default is None
         Root filename (with full path) is required to save the figures. Postfix
         is added to the root filename.
-    \*\*kwargs, optional. This parameter is used by plt.plot and savefig functions    
+    kwargs, optional. This parameter is used by plt.plot and savefig functions    
         - savefilename : str, optional, default :'_audiogram.png'
             Postfix of the figure filename
         - figsize : tuple of integers, optional, default: (4,10)
             width, height in inches.  
         - title : string, optional, default : 'Spectrogram'
             title of the figure
         - xlabel : string, optional, default : 'Time [s]'
@@ -76,46 +76,55 @@
             the pixel centers fall on zero-based (row, column) indices.
         - dpi : integer, optional, default is 96
             Dot per inch. 
             For printed version, choose high dpi (i.e. dpi=300) => slow
             For screen version, choose low dpi (i.e. dpi=96) => fast
         - format : string, optional, default is 'png'
             Format to save the figure
-           
+
         ... and more, see matplotlib     
         
     Returns
     -------    
     s_out : 1d ndarray of integer
         Vector containing the audiogram 
     fs : int 
         The sampling frequency in Hz of the audiogram    
         
     Examples
     --------
+    >>> import maad
     >>> s, fs = maad.sound.load("../data/tropical_forest_morning.wav", channel='left')
+    >>> print("The sampling frequency of the audio file is {} Hz".format(fs))
+    The sampling frequency of the audio file is 48000 Hz
     >>> import numpy as np
     >>> tn = np.arange(0,len(s))/fs
     >>> import matplotlib.pyplot as plt
     >>> fig, (ax0, ax1) = plt.subplots(2,1, sharex=True, squeeze=True)
     >>> ax0, _ = maad.util.plot1d(tn,s,ax=ax0, figtitle='ground level')
-    >>> ax0.set_ylim((-0.075,0.0751))
+    >>> ax0.set_ylim((-0.075,0.075))
+    (-0.075, 0.075)
     >>> s, fs = maad.sound.load("../data/tropical_forest_morning.wav", channel='right')
     >>> ax1, _ = maad.util.plot1d(tn,s,ax=ax1, figtitle='canopy level')
     >>> ax1.set_ylim((-0.075,0.075))
+    (-0.075, 0.075)
     >>> fig.tight_layout()
     """
     if verbose :
         print(72 * '_' )
         print("loading %s..." %filename)   
     
-    # read the .wav file and return the sampling frequency fs (Hz) 
+    # Read the .wav file and return the sampling frequency fs (Hz) 
     # and the audiogram s as a 1D array of integer
-    fs, s = wavfile.read(filename)
-    if verbose :print("Sampling frequency: %dHz" % fs)
+    # Execute the function wavfile.read with warnings suppressed in order to avoid the 
+    # common warning "WavFileWarning: Chunk (non-data) not understood, skipping it"
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore")  # Ignore all warnings
+        fs, s = wavfile.read(filename)
+        if verbose :print("Sampling frequency: %dHz" % fs)
     
     # Normalize the signal between -1 to 1 depending on the type (number of bits)
     if s.dtype == np.int32:
         bit = 32
         s = s/2**(bit-1)
     elif s.dtype == np.int16:
         bit = 16
@@ -151,85 +160,85 @@
             bbox_inches=kwargs.pop('bbox_inches', 'tight') 
             format=kwargs.pop('format','png')
             savefilename=kwargs.pop('savefilename', '_audiogram')  
             filename = savefig+savefilename+'.'+format
             if verbose :print('\n''save figure : %s' %filename)
             fig.savefig(fname=filename, dpi=dpi, bbox_inches=bbox_inches,
                         format=format, **kwargs)  
-                           
+            
     return s_out, fs
 
 #%%
 def load_spectrogram(filename, fs, duration, flims = None, flipud = True,
                 verbose=False, display=False, **kwargs): 
     """ 
     Load an image from a file or an URL 
-     
+
     Parameters 
     ----------   
     filename : string 
         Image file name, e.g. ``test.jpg`` or URL. 
-     
+
     fs : scalar 
         Sampling frequency of the audiogram (in Hz) 
-     
+
     duration : scalar 
         Duration of the audiogram (in s) 
         
     flims : list of 2 scalars [min, max], optional, default is None
         flims corresponds to the min and max boundary frequency values
         
     flipud : boolean, optional, default is True 
         Vertical flip of the matrix (image) 
         
     verbose : boolean, optional, default is False
         if True, print message in terminal
-     
+
     display : boolean, optional, default is False 
         if True, display the image 
-         
-    \*\*kwargs, optional. This parameter is used by plt.plot  
+
+    kwargs, optional. This parameter is used by plt.plot  
         - figsize : tuple of integers, optional, default: (4,10) 
             width, height in inches.   
-         
+
         - title : string, optional, default : 'Spectrogram' 
             title of the figure 
-         
+
         - xlabel : string, optional, default : 'Time [s]' 
             label of the horizontal axis 
-         
+
         - ylabel : string, optional, default : 'Amplitude [AU]' 
             label of the vertical axis 
-         
+
         - cmap : string or Colormap object, optional, default is 'gray' 
             See https://matplotlib.org/examples/color/colormaps_reference.html 
             in order to get all the  existing colormaps 
             examples: 'hsv', 'hot', 'bone', 'tab20c', 'jet', 'seismic',  
             'viridis'... 
-         
+
         - vmin, vmax : scalar, optional, default: None 
             `vmin` and `vmax` are used in conjunction with norm to normalize 
             luminance data.  Note if you pass a `norm` instance, your 
             settings for `vmin` and `vmax` will be ignored. 
-         
+
         - extent : scalars (left, right, bottom, top), optional, default: None 
             The location, in data-coordinates, of the lower-left and 
             upper-right corners. If `None`, the image is positioned such that 
             the pixel centers fall on zero-based (row, column) indices. 
-         
+
         - dpi : integer, optional, default is 96 
             Dot per inch.  
             For printed version, choose high dpi (i.e. dpi=300) => slow 
             For screen version, choose low dpi (i.e. dpi=96) => fast 
-         
+
         - format : string, optional, default is 'png' 
             Format to save the figure  
-         
+
         ... and more, see matplotlib  
-         
+
     Returns 
     ------- 
     Sxx : ndarray 
         The different color bands/channels are stored in the 
         third dimension, such that a gray-image is MxN, an 
         RGB-image MxNx3 and an RGBA-image MxNx4.    
     tn : 1d ndarray of floats
@@ -238,73 +247,76 @@
         Frequency vector (vertical y-axis)    
     extent : list of scalars [left, right, bottom, top]
         The location, in data-coordinates, of the lower-left and
         upper-right corners. 
         
     Examples
     --------
+    >>> import maad
     >>> xenocanto_link = 'https://www.xeno-canto.org/sounds/uploaded/DTKJSKMKZD/ffts/XC445081-med.png'
-    >>> Sxx, tn, fn, ext = maad.sound.load_spectrogram(filename= xenocanto_link,
-                                          fs=44100,            
-                                          flims=[0,15000],
-                                          duration = 10
-                                          )
+    >>> Sxx, tn, fn, ext = maad.sound.load_spectrogram(filename=xenocanto_link, \
+                                                        fs=44100,               \
+                                                        flims=[0,15000],        \
+                                                        duration = 10,          \
+                                                        )
+    >>> print("The time resolution of the spectrogram is {} s and the frequency resolution is {} Hz".format(tn[1]-tn[0], fn[1]-fn[0]))
+    The time resolution of the spectrogram is 0.020876826722338204 s and the frequency resolution is 94.33962264150944 Hz
     >>> import matplotlib.pyplot as plt
-    >>> maad.util.plot2d(Sxx,extent=ext)
+    >>> ax, fig = maad.util.plot2d(Sxx,extent=ext)
     
     """ 
     
     if verbose :
         print(72 * '_' ) 
         print("loading %s..." %filename)  
-     
+    
     # Load image 
-    Sxx  = imread(filename, as_gray=True) 
-     
+    Sxx = imread(filename, as_gray=True) 
+    
     # if 3D, convert into 2D 
     if len(Sxx.shape) == 3: 
         Sxx = Sxx[:,:,0] 
-         
+    
     # Rescale the image between 0 to 1 
-    Sxx = linear_scale(Sxx, minval= 0.0, maxval=1.0) 
-             
+    Sxx = linear_scale(Sxx, minval= 0.0, maxval=1.0, axis=None) 
+    
     # Get the resolution 
     if flims is None :
         df = fs/(Sxx.shape[0]-1) 
     else:
         df = (flims[1]-flims[0]) / (Sxx.shape[0]-1)
     dt = duration/(Sxx.shape[1]-1) 
     
     # create the vectors
     if flims is None :
         fn = np.arange(0,fs/2,df) 
     else:
         fn = np.arange(flims[0],flims[1],df)  
     tn = np.arange(0,Sxx.shape[1],1) * dt
-     
+    
     # Extent 
     extent = [tn[0], tn[-1], fn[0], fn[-1]] 
-     
+    
     # flip the image vertically 
     if flipud: Sxx = np.flip(Sxx, 0) 
-     
+    
     # Display 
     if display :  
         ylabel =kwargs.pop('ylabel','Frequency [Hz]') 
         xlabel =kwargs.pop('xlabel','Time [sec]')  
         title  =kwargs.pop('title','loaded spectrogram') 
         cmap   =kwargs.pop('cmap','gray')  
         figsize=kwargs.pop('figsize',(4, 0.33*(extent[1]-extent[0])))  
         vmin=kwargs.pop('vmin',Sxx.min())  
         vmax=kwargs.pop('vmax',Sxx.max())  
-         
+        
         _, fig = plot2d (Sxx, extent=extent, figsize=figsize,title=title,  
-                         ylabel = ylabel, xlabel = xlabel,vmin=vmin, vmax=vmax, 
-                         cmap=cmap, **kwargs) 
-     
+                        ylabel = ylabel, xlabel = xlabel,vmin=vmin, vmax=vmax, 
+                        cmap=cmap, **kwargs) 
+    
     return Sxx, tn, fn, extent 
 #%%
 def write(filename, fs, data, bit_depth=None):
     """
     Write a NumPy array as a WAV file with the Scipy method. [1]_ 
 
     Parameters
@@ -347,35 +359,35 @@
     .. [2] IBM Corporation and Microsoft Corporation, "Multimedia Programming
        Interface and Data Specifications 1.0", section "Data Format of the
        Samples", August 1991
        http://www.tactilemedia.com/info/MCI_Control_Info.html
 
     Examples
     --------
+    >>> from maad import sound
     
     Synthesize a 440Hz sine wave at 44100 Hz and write it to disk.
     
     >>> import numpy as np
     >>> fs = 44100; T = 2.0
     >>> t = np.linspace(0, T, int(T*fs))
     >>> data = np.sin(2. * np.pi * 440. *t)
-    >>> maad.sound.write('example.wav', fs, data)
+    >>> sound.write('example.wav', fs, data, bit_depth=16)
     
     Open an audio file, filter a frequency band and write to disk specifying the bit depth.
-    
-    >>> from maad import sound
+
     >>> s, fs = sound.load('../data/spinetail.wav')
     >>> s_filt = sound.sinc(s, (3000, 10000), fs)
     >>> sound.write('spinetail_filtered.wav', fs, s_filt, bit_depth=16)
     """
 
     if (data.dtype == 'float64') | (data.dtype == 'float32'):
         # Check that the array has values between -1 and 1
         if (data.min() < -1) | (data.max() > 1):
-            warn('Values should be between [-1, 1]. Clipping signal.')
+            warnings.warn('Values should be between [-1, 1]. Clipping signal.')
             data[data<-1] = -1
             data[data>1] = 1
         
         # Convert to desired bit depth
         if bit_depth == 8:
             data = data + 1 # change range to postive [0,2]
             data = (data * 127).astype(np.uint8)
@@ -383,15 +395,15 @@
         elif bit_depth == 16:
             data = (data * 32767).astype(np.int16)
             
         elif bit_depth == 32:
             data = (data * 2147483647).astype(np.int32)
         
         else:
-            warn('Values for bit depth should be 8, 16 or 32. Argument ignored.')
+            warnings.warn('Values for bit depth should be 8, 16 or 32. Argument ignored.')
             pass
         
     if data.ndim > 1:
         data = data.T
     
     write_wav(filename, fs, np.asfortranarray(data))
     
@@ -416,19 +428,22 @@
     Examples
     --------
     
     Load an audio example using its code name.
     
     >>> from maad import sound
     >>> s, fs = sound.load_url('spinetail')
-    
+    >>> print('The samping rate of the audio file is {} Hz'.format(fs))
+    The samping rate of the audio file is 44100 Hz
+
     Load an audio example using the full web address.
     
-    >>> from maad import sound
     >>> s, fs = sound.load_url('https://github.com/scikit-maad/scikit-maad/raw/production/data/spinetail.wav')
+    >>> print('The samping rate of the audio file is {} Hz'.format(fs))
+    The samping rate of the audio file is 44100 Hz
     """
 
     # set dictionary for examples from the audio dataset
     code_name_url = {
         'spinetail': 'https://github.com/scikit-maad/scikit-maad/raw/production/data/spinetail.wav',
         'cold_forest_daylight': 'https://github.com/scikit-maad/scikit-maad/raw/production/data/cold_forest_daylight.wav',
         'cold_forest_night': 'https://github.com/scikit-maad/scikit-maad/raw/production/data/cold_forest_night.wav',
@@ -440,8 +455,13 @@
     if url in code_name_url.keys():
         url_path = code_name_url[url]
     # load as web address
     else:
         url_path = url
     
     s, fs = load(io.BytesIO(urlopen(url_path).read()))
-    return s, fs
+    return s, fs
+
+
+if __name__ == "__main__":
+    import doctest
+    doctest.testmod()
```

### Comparing `scikit-maad-1.3.6.1/maad/sound/metrics.py` & `scikit_maad-1.4.0/maad/sound/metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-maad-1.3.6.1/maad/sound/spectral_subtraction.py` & `scikit_maad-1.4.0/maad/sound/spectral_subtraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     display : boolean, optional, default is False 
         Display the signal if True 
 
     savefig : string, optional, default is None 
         Root filename (with full path) is required to save the figures. Postfix 
         is added to the root filename. 
 
-    \*\*kwargs, optional. This parameter is used by plt.plot and savefig functions 
+    kwargs, optional. This parameter is used by plt.plot and savefig functions 
 
         - savefilename : str, optional, default :'_spectro_after_noise_subtraction.png' 
             Postfix of the figure filename 
 
         - figsize : tuple of integers, optional, default: (4,10) 
             width, height in inches.   
 
@@ -286,15 +286,15 @@
     display : boolean, optional, default is False 
         Display the signal if True 
 
     savefig : string, optional, default is None 
         Root filename (with full path) is required to save the figures. Postfix 
         is added to the root filename. 
 
-    \*\*kwargs, optional. This parameter is used by plt.plot and savefig functions 
+    kwargs, optional. This parameter is used by plt.plot and savefig functions 
 
         - savefilename : str, optional, default :'_spectro_after_noise_subtraction.png' 
             Postfix of the figure filename 
 
         - figsize : tuple of integers, optional, default: (4,10) 
             width, height in inches.   
 
@@ -493,15 +493,15 @@
     display : boolean, optional, default is False 
         Display the signal if True 
 
     savefig : string, optional, default is None 
         Root filename (with full path) is required to save the figures. Postfix 
         is added to the root filename. 
 
-    \*\*kwargs, optional. This parameter is used by plt.plot and savefig functions 
+    kwargs, optional. This parameter is used by plt.plot and savefig functions 
 
         - savefilename : str, optional, default :'_spectro_after_noise_subtraction.png' 
             Postfix of the figure filename 
 
         - figsize : tuple of integers, optional, default: (4,10) 
             width, height in inches.   
 
@@ -666,15 +666,15 @@
     display : boolean, optional, default is False 
         Display the signal if True 
 
     savefig : string, optional, default is None 
         Root filename (with full path) is required to save the figures. Postfix 
         is added to the root filename. 
 
-    \*\*kwargs, optional. This parameter is used by plt.plot and savefig functions 
+    kwargs, optional. This parameter is used by plt.plot and savefig functions 
 
         - savefilename : str, optional, default :'_spectro_after_noise_subtraction.png' 
             Postfix of the figure filename 
 
         - figsize : tuple of integers, optional, default: (4,10) 
             width, height in inches.   
 
@@ -842,15 +842,15 @@
        display : boolean, optional, default is False
            Display the signal if True
 
        savefig : string, optional, default is None
            Root filename (with full path) is required to save the figures. Postfix
            is added to the root filename.
 
-       \*\*kwargs, optional. This parameter is used by plt.plot and savefig functions
+       kwargs, optional. This parameter is used by plt.plot and savefig functions
 
            - savefilename : str, optional, default :'_spectro_after_noise_subtraction.png'
                Postfix of the figure filename
 
            - figsize : tuple of integers, optional, default: (4,10)
                width, height in inches.
```

### Comparing `scikit-maad-1.3.6.1/maad/sound/spectro_func.py` & `scikit_maad-1.4.0/maad/sound/spectro_func.py`

 * *Files identical despite different names*

### Comparing `scikit-maad-1.3.6.1/maad/sound/transform.py` & `scikit_maad-1.4.0/maad/sound/transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from scipy.signal import hilbert
 from scipy.signal import periodogram, welch
 import scipy
 import resampy
+from warnings import warn
 
 # import internal modules
 from maad.sound import wave2frames
 from maad.util import plot_spectrum
 
 #%%
 # =============================================================================
@@ -98,15 +99,15 @@
         env = np.abs(hilbert(s))  
     else:
         raise Exception("Invalid mode. Mode should be 'fast' or 'hilbert' ")
         
     return env
 
 #%%
-def spectrum(s, fs, nperseg=256, noverlap=None, nfft=None, window='hanning', method='welch', 
+def spectrum(s, fs, nperseg=256, noverlap=None, nfft=None, window='hann', method='welch', 
         tlims=None, flims=None, scaling='spectrum', as_pandas_series=False, display=False):
     """ 
     Estimate the power spectral density or power spectrum of 1D signal.
     
     The estimates can be computed using two methods: Welch or periodogram. Welch's method
     divides the signal into segments, computes the power spectral density for each 
     segment and then takes the average between segments. The periodogram method computes
@@ -123,16 +124,17 @@
     
     nperseg: int, optional
         Length of segment for 'welch' method, default is 256
     
     noverlap: int, optional
         Overlap between segments for Welch's method. If None, noverlap = nperseg/2.
     
-    window : string, default is 'hanning
-        Name of the window used for the short fourier transform.
+    window : string, default is 'hann'
+        Name of the window used for the short fourier transform, 'hanning' window is 
+        now deprecated.
     
     nfft: int, optional
         Length of FFT for periodogram method. If None, length of signal will be used.
         Length of FFT for welch method if zero padding is desired. If None, length of nperseg will be used.
     
     method: {'welch', 'periodogram'}
         Method used to estimate the power spectral density of the signal
@@ -177,22 +179,26 @@
     
     Specify temporal and spectral limits to get spectral characteristics of the 
     spinetail's song.
     
     >>> spec, f_idx = sound.spectrum(s, fs, nperseg=2056, tlims=(5.3, 7.9), flims=(2000, 12000), display=True)
     
     """
-    
     if tlims is not None:
     # trim audio signal
         try:
             s = s[int(tlims[0]*fs): int(tlims[1]*fs)]
         except:
             raise Exception('length of tlims tuple should be 2')
     
+    # small fix to keep compatibility with old scipy version
+    if window=='hanning':
+        window='hann'
+        warn("Window type 'hanning' will be deprecated. Changing to 'hann' window.", FutureWarning)
+
     if method=='welch':
         f_idx, pxx = welch(s, fs, window, nperseg, noverlap, nfft, scaling=scaling)
     
     elif method=='periodogram':
         f_idx, pxx = periodogram(s, fs, window, nfft, scaling=scaling)
         
     else:
@@ -225,18 +231,19 @@
     fs : int
         Time series sampling rate. 
 
     target_fs : int
         Target sampling rate.
 
     res_type : str, optional
-        Resample method. By default 'kaiser_best', is a high-quality method.
-        `res_type='kaiser_fast'` is a faster method.
-        `res_type='sinc_window'` is an advanced and custom method of resampling. 
-        `res_type='scipy'` is a Fourier transforms method based.
+        Resample method. By default 'kaiser_best'.
+        'kaiser_best' method that applies a Kaiser windowed sinc interpolation.
+        'kaiser_fast' similar to kaiser_best, but faster.
+        'scipy' is a Fourier transform method implemented in scipy.
+        'scipy_poly' Resample using polyphase filtering and an FIR filter. 
 
     kwargs : additional keyword arguments
         If `res_type='sinc_window'`, additional keyword arguments to pass to
         `resampy.resample`.
 
     Returns
     -------
@@ -259,23 +266,36 @@
     ...       'Number of samples - resampled audio:', s_resamp.shape[0])
     >>> _ = sound.spectrogram(s, fs, display=True)
     >>> _ = sound.spectrogram(s_resamp, fs/2, display=True)
 
     """
     if fs == target_fs:
         return s
-    
-    ratio = float(target_fs) / fs
-    n_samples = int(np.ceil(s.shape[-1] * ratio))
 
     if res_type == 'scipy':
-        res_data = scipy.signal.resample(s, n_samples, axis = -1)
+        # Calculate the resampling ratio and get the number of output samples
+        ratio = float(target_fs) / fs
+        n_samples = int(np.round(s.shape[-1] * ratio))
+        res_data = scipy.signal.resample(s, n_samples, axis=-1, **kwargs)
+    
+    elif res_type == 'scipy_poly':
+        # Calculate the resampling ratio and get the common denominator
+        gcd = np.gcd(int(fs), int(target_fs))
+        num = target_fs // gcd
+        den = fs // gcd
+        # Resample the signal using SciPy's resample_poly function
+        res_data = scipy.signal.resample_poly(s, num, den)
     
-    else:
+    elif res_type in ('kaiser_best', 'kaiser_fast'):
+        warn("Methods 'kaiser_fast' and 'kaiser_best' are deprecated and will be removed from future versions.", DeprecationWarning)
         res_data = resampy.resample(s, fs, target_fs, filter=res_type, axis=-1, **kwargs)
+    
+    else:
+        raise ValueError("Valid resample methods are 'scipy', 'scipy_poly', 'kaiser_best', 'kaiser_fast', not res_type={}".format(res_type))
+                         
     return np.ascontiguousarray(res_data, dtype=s.dtype)
 
 #%%
 def trim(s, fs, min_t, max_t, pad=False, pad_constant=0):
     """
     Slices a time series, from a initial time `min_t` to an ending time `max_t`.  
     If the target duration `duration =` is larger than the original duration and `pad = True`,
```

### Comparing `scikit-maad-1.3.6.1/maad/sound/trim_func.py` & `scikit_maad-1.4.0/maad/sound/trim_func.py`

 * *Files identical despite different names*

### Comparing `scikit-maad-1.3.6.1/maad/spl/__init__.py` & `scikit_maad-1.4.0/maad/spl/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,34 +46,34 @@
                         amplitude2dBSPL,
                         wav2dBSPL,
                         wav2leq,
                         pressure2leq,
                         psd2leq)
 
 from .active_space import (attenuation_dB,
-                           dBSPL_per_bin,
-                           detection_distance,
-                           pressure_at_r0,
-                           dBSPL_at_r0,
-                           apply_attenuation)
+                        dBSPL_per_bin,
+                        detection_distance,
+                        pressure_at_r0,
+                        dBSPL_at_r0,
+                        apply_attenuation)
 
 __all__ = [
-           # conversion_SPL        
-           'wav2volt',
-           'volt2pressure',
-           'wav2pressure',
-           'pressure2dBSPL',
-           'dBSPL2pressure',
-           'power2dBSPL',
-           'amplitude2dBSPL',
-           'wav2dBSPL',
-           'wav2leq',
-           'pressure2leq',
-           'psd2leq'
-           #active_space
-           'attenuation_dB',
-           'dBSPL_per_bin',
-           'detection_distance',
-           'pressure_at_r0',
-           'dBSPL_at_r0',
-           'apply_attenuation'
-           ]
+    # conversion_SPL        
+    'wav2volt',
+    'volt2pressure',
+    'wav2pressure',
+    'pressure2dBSPL',
+    'dBSPL2pressure',
+    'power2dBSPL',
+    'amplitude2dBSPL',
+    'wav2dBSPL',
+    'wav2leq',
+    'pressure2leq',
+    'psd2leq',
+    #active_space
+    'attenuation_dB',
+    'dBSPL_per_bin',
+    'detection_distance',
+    'pressure_at_r0',
+    'dBSPL_at_r0',
+    'apply_attenuation'
+]
```

### Comparing `scikit-maad-1.3.6.1/maad/spl/active_space.py` & `scikit_maad-1.4.0/maad/spl/active_space.py`

 * *Files identical despite different names*

### Comparing `scikit-maad-1.3.6.1/maad/spl/conversion_SPL.py` & `scikit_maad-1.4.0/maad/spl/conversion_SPL.py`

 * *Files identical despite different names*

### Comparing `scikit-maad-1.3.6.1/maad/util/__init__.py` & `scikit_maad-1.4.0/maad/util/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,15 +141,18 @@
                      read_raven_annot,
                      write_raven_annot,
                      date_parser)
 
 from .xeno_canto import (xc_query,
                          xc_multi_query,
                          xc_selection,
-                         xc_download)
+                         xc_download,
+                         # xc_save_csv,
+                         # xc_read_csv
+                         )
 
 from .audio_metadata_utilities import (check_file_format,
                                        audio_header,
                                        filename_info,
                                        get_metadata_file,
                                        get_metadata_dir)
 
@@ -194,20 +197,24 @@
            'rms',
            'kurtosis',
            'skewness',
            'moments',
            # parser
            'read_audacity_annot',
            'write_audacity_annot',
+           'read_raven_annot',
+           'write_raven_annot',
            'date_parser',
            # xeno_canto
            'xc_query',
            'xc_multi_query',
            'xc_selection',
            'xc_download',
+           # 'xc_save_csv',
+           # 'xc_read_csv',
             # audio_metadata_utilities
             'check_file_format',
             'audio_header',
             'filename_info',
             'get_metadata_file',
             'get_metadata_dir'
             ]
```

### Comparing `scikit-maad-1.3.6.1/maad/util/audio_metadata_utilities.py` & `scikit_maad-1.4.0/maad/util/audio_metadata_utilities.py`

 * *Files identical despite different names*

### Comparing `scikit-maad-1.3.6.1/maad/util/math_func.py` & `scikit_maad-1.4.0/maad/util/math_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 #!/usr/bin/env python
 """ 
 Mathematical tools for audio signal processing.
 """
-#
-# Authors:  Juan Sebastian ULLOA <lisofomia@gmail.com>
-#           Sylvain HAUPERT <sylvain.haupert@mnhn.fr>
-#
-# License: New BSD License
-
 # =============================================================================
 # Load the modules
 # =============================================================================
 # Import external modules
 import matplotlib.pyplot as plt
 import numpy as np 
 from numpy import mean, median, var
-from scipy.ndimage.filters import uniform_filter1d # for fast running mean
+from scipy.ndimage import uniform_filter1d # for fast running mean
 from scipy.signal import periodogram, welch
 import pandas as pd
 # min value
 import sys
 _MIN_ = sys.float_info.min
 
 # Import internal modules
@@ -126,15 +120,15 @@
     Examples
     --------
     
     This function is interesting to obtain the background noise (BGN) profile (e.g. frequency bin
     by frequency bin) of a spectrogram
     
     >>> w, fs = maad.sound.load('../data/cold_forest_daylight.wav') 
-    >>> Sxx_power,tn,fn,_ = maad.sound.spectrogram(w,fs,window='hanning',noverlap=512, nFFT=1024)
+    >>> Sxx_power,tn,fn,_ = maad.sound.spectrogram(w,fs,window='hann',noverlap=512, nFFT=1024)
     >>> Sxx_dB = maad.util.power2dB(Sxx_power)
     >>> BGN_med = maad.util.get_unimode (Sxx_dB, mode='median', axis=1)
     >>> import matplotlib.pyplot as plt 
     >>> plt.plot(fn,maad.util.mean_dB(Sxx_dB,axis=1))
     >>> plt.plot(fn,BGN_med)
     
     Extract the background noise from mean
```

### Comparing `scikit-maad-1.3.6.1/maad/util/miscellaneous.py` & `scikit_maad-1.4.0/maad/util/miscellaneous.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     -------
     index : 1d ndarray of scalars
         Vector of booleans corresponding to the selected frequency(-ies)
 
     Examples
     --------
     >>> w, fs = maad.sound.load('../data/cold_forest_daylight.wav') 
-    >>> Sxx_power,tn,fn,_ = maad.sound.spectrogram(w,fs,window='hanning',noverlap=512, nFFT=1024)
+    >>> Sxx_power,tn,fn,_ = maad.sound.spectrogram(w,fs,window='hann',noverlap=512, nFFT=1024)
     >>> Sxx_dB = maad.util.power2dB(Sxx_power) # convert into dB
     >>> bw = (2000,6000) #in Hz
     >>> fig_kwargs = {'vmax': Sxx_dB.max(),
                       'vmin': -90,
                       'extent':(tn[0], tn[-1], fn[0], fn[-1]),
                       'figsize':(10,13),
                       'title':'Power Spectrum Density (PSD)',
@@ -853,132 +853,132 @@
                 warnings.warn(
                     'ROIs boundaries are outside time or frecuency signal limits. Clipping ROIS to valid boundaries.')
                 df.loc[df.min_t < tn.min(), 'min_t'] = tn.min()
                 df.loc[df.max_t > tn.max(), 'max_t'] = tn.max()
                 df.loc[df.min_f < fn.min(), 'min_f'] = fn.min()
                 df.loc[df.max_f > fn.max(), 'max_f'] = fn.max()
 
-            df_bbox = []
+            bbox = []
             for idx in df.index:
                 min_y = nearest_idx(fn, df.loc[idx, 'min_f'])
                 min_x = nearest_idx(tn, df.loc[idx, 'min_t'])
                 max_y = nearest_idx(fn, df.loc[idx, 'max_f'])
                 max_x = nearest_idx(tn, df.loc[idx, 'max_t'])
                 # test if max > min, if not, drop row form df
                 if (min_y <= max_y) and (min_x <= max_x):
-                    df_bbox.append((min_y, min_x, max_y, max_x))
+                    bbox.append((min_y, min_x, max_y, max_x))
                 else:
                     df = df.drop(idx)
             
             # check if new columns
             if not (('min_y' and 'min_x' and 'max_y' and 'max_x') in df):
-                df = df.join(pd.DataFrame(df_bbox,
+                df = df.join(pd.DataFrame(bbox,
                                           columns=['min_y', 'min_x',
                                                    'max_y', 'max_x'],
                                           index=df.index))
             # otherwise update the existing columns with new values
             else:
-                df.update(pd.DataFrame(df_bbox,
+                df.update(pd.DataFrame(bbox,
                                        columns=['min_y', 'min_x',
                                                 'max_y', 'max_x'],
                                        index=df.index))
          
 
         # if ('min_y' and 'min_x' and 'max_y' and 'max_x') in df and not (('min_t' and 'min_f' and 'max_t' and 'max_f') in df):
         if ('min_y' and 'min_x' and 'max_y' and 'max_x') in df:
-            df_bbox = []
+            bbox = []
             for _, row in df.iterrows():
                 min_f = fn[int(round(row.min_y))]
                 min_t = tn[int(round(row.min_x))]
                 max_f = fn[int(round(row.max_y))]
                 max_t = tn[int(round(row.max_x))]
                 # test if max > min, if not, drop row form df
                 if (min_f <= max_f) and (min_t <= max_t):
-                    df_bbox.append((min_f, min_t, max_f, max_t))
+                    bbox.append((min_f, min_t, max_f, max_t))
                 else:
                     df = df.drop(row.name)
 
             # check if new columns
             if not (('min_t' and 'min_f' and 'max_t' and 'max_f') in df):
-                df = df.join(pd.DataFrame(df_bbox,
+                df = df.join(pd.DataFrame(bbox,
                                           columns=['min_f', 'min_t',
                                                    'max_f', 'max_t'],
                                           index=df.index))
             
 
         # if ('centroid_y' and 'centroid_x') in df and not (('centroid_f' and 'centroid_t') in df):
         if ('centroid_y' and 'centroid_x') in df:
-            df_centroid = []
+            centroid = []
             for _, row in df.iterrows():
                 centroid_f = fn[int(round(row.centroid_y))]
                 centroid_t = tn[int(round(row.centroid_x))]
-                df_centroid.append((centroid_f, centroid_t))
+                centroid.append((centroid_f, centroid_t))
                 
             # check if new columns
             if not (('centroid_f' and 'centroid_t') in df) :
-                df = df.join(pd.DataFrame(df_centroid,
+                df = df.join(pd.DataFrame(centroid,
                                           columns=['centroid_f', 'centroid_t'],
                                           index=df.index))
 
         # if ('centroid_f' and 'centroid_t') in df and not (('centroid_y' and 'centroid_x') in df):
         if ('centroid_f' and 'centroid_t') in df:
-            df_centroid = []
+            centroid = []
             for idx in df.index:
                 centroid_y = nearest_idx(fn, df.loc[idx, 'centroid_f'])
                 centroid_x = nearest_idx(tn, df.loc[idx, 'centroid_t'])
-                df_centroid.append((centroid_y, centroid_x))
+                centroid.append((centroid_y, centroid_x))
 
             # check if new columns
             if not (('centroid_y' and 'centroid_x') in df) :
-                df = df.join(pd.DataFrame(df_centroid,
+                df = df.join(pd.DataFrame(centroid,
                                           columns=['centroid_y', 'centroid_x'],
                                           index=df.index))
             # otherwise update the existing columns with new values
             else:
-                df.update(pd.DataFrame(df_centroid,
+                df.update(pd.DataFrame(centroid,
                                        columns=['centroid_y', 'centroid_x'],
                                        index=df.index))
                 
         # =============
         # if ('duration_x' and 'bandwidth_y' and 'area_xy') in df and not (('duration_t' and 'bandwidth_f' and 'area_tf') in df):
         if ('duration_x' and 'bandwidth_y' and 'area_xy') in df:
-            df_area = []
+            area = []
             for _, row in df.iterrows():
                 bandwidth_f = row.bandwidth_y * (fn[1]-fn[0])
                 duration_t = row.duration_x * (tn[1]-tn[0])
                 area_tf = row.area_xy * (fn[1]-fn[0]) * (tn[1]-tn[0])
-                df_area.append((duration_t, bandwidth_f, area_tf))
+                area.append((duration_t, bandwidth_f, area_tf))
                 
             # check if new columns
             if not (('duration_t' and 'bandwidth_f' and 'area_tf') in df) :
-                df = df.join(pd.DataFrame(df_area,
+                df = df.join(pd.DataFrame(area,
                                           columns=['duration_t',
                                                     'bandwidth_f', 'area_tf'],
                                           index=df.index))
  
         # if ('duration_t' and 'bandwidth_f' and 'area_tf') in df and not (('duration_x' and 'bandwidth_y' and 'area_xy') in df):
         if ('duration_t' and 'bandwidth_f' and 'area_tf') in df:
-            df_area = []
+            area = []
             for idx in df.index:
                 bandwidth_y = round(
                     df.loc[idx, 'bandwidth_f']) / ((fn[1]-fn[0]))
                 duration_x = round(df.loc[idx, 'duration_t']) / (tn[1]-tn[0])
                 area_xy = round(df.loc[idx, 'area_xy'] /
                                 ((fn[1]-fn[0]) * (tn[1]-tn[0])))
-                df_area.append((bandwidth_y, duration_x, area_xy))
+                area.append((bandwidth_y, duration_x, area_xy))
 
             # check if new columns
             if not (('duration_x' and 'bandwidth_y' and 'area_xy') in df):
-                df = df.join(pd.DataFrame(df_area,
+                df = df.join(pd.DataFrame(area,
                                           columns=['duration_x',
                                                     'bandwidth_y', 'area_xy'],
                                           index=df.index))
             # otherwise update the existing columns with new values
             else:
-                df.update(pd.DataFrame(df_area,
+                df.update(pd.DataFrame(area,
                                        columns=['duration_x',
                                                 'bandwidth_y', 'area_xy'],
                                        index=df.index))
 
         count += 1
 
     return df
```

### Comparing `scikit-maad-1.3.6.1/maad/util/parser.py` & `scikit_maad-1.4.0/maad/util/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 #%%
 # =============================================================================
 # Public functions
 # =============================================================================
 def read_audacity_annot (audacity_filename):
     """
-    Read audacity annotations file (or labeling file) and return a Pandas Dataframe
+    Read Audacity annotations file (or labeling file) and return a Pandas Dataframe
     with the bounding box and the label of each region of interest (ROI). Allows to
     read annotations with standard Audacity style (temporal selection) and with
     spectral selection style (spectro-temporal selection). If the file exists but has no 
     annotations, the function returns and empty dataframe.
     
     Parameters
     ----------
@@ -238,15 +238,15 @@
             pass
     
     return df_to_save
 
 #%% 
 def read_raven_annot(raven_filename):
     """
-    Read raven annotations file (or labeling file) and return a Pandas Dataframe
+    Read Raven annotations file (or labeling file) and return a Pandas Dataframe
     with the bounding box and the label of each region of interest (ROI). If the file 
     exists but has no annotations, the function returns and empty dataframe.
     
     Parameters
     ----------
     raven_filename : string
         Path to the annotation file
@@ -263,16 +263,16 @@
     """
     df_out = pd.read_csv(raven_filename, sep='\t')
     return df_out
     
 #%%
 def write_raven_annot(fname, df_rois, save_file=True):
     """ 
-    Write audio segmentation to text file in Audacity format, a file that can be imported
-    and modified with Audacity. If the dataframe has no frequency delimiters, annotations
+    Write audio segmentation to text file in Raven format, a file that can be imported
+    and modified with Raven. If the dataframe has no frequency delimiters, annotations
     are saved with standard Audacity format (temporal segmentation). If the dataframe has
     temporal and frequencial delimiters, the annotations are saved as spectral selection 
     style (spectro-temporal selection). If the dataframe is empty, the function saves an 
     empty file.
     
     Parameters
     ----------
```

### Comparing `scikit-maad-1.3.6.1/maad/util/visualization.py` & `scikit_maad-1.4.0/maad/util/visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         Do format_features(rois,tn,fn) before using overlay_centroid to be sure that 
         the format of the DataFrame is correct 
              
     savefig : string, optional, default is None 
         Root filename (with full path) is required to save the figures. Postfix 
         is added to the root filename. 
          
-    \*\*kwargs, optional. This parameter is used by plt.plot and savefig functions 
+    kwargs, optional. This parameter is used by plt.plot and savefig functions 
             
         - savefilename : str, optional, default :'_spectro_overlaycentroid.png' 
             Postfix of the figure filename 
          
         - extent : list of scalars [left, right, bottom, top], optional, default: None
             The location, in data-coordinates, of the lower-left and
             upper-right corners. If `None`, the image is positioned such that
@@ -317,15 +317,15 @@
         The rois_bbox pandas.DataFrame must have a column called 'label' with names
         assigned to each ROI.
  
     savefig : string, optional, default is None 
         Root filename (with full path) is required to save the figures. Postfix 
         is added to the root filename. 
          
-    \*\*kwargs, optional. This parameter is used by plt.plot and savefig functions 
+    kwargs, optional. This parameter is used by plt.plot and savefig functions 
             
         - savefilename : str, optional, default :'_spectro_overlayrois.png' 
             Postfix of the figure filename 
             
         - extent : list of scalars [left, right, bottom, top], optional, default: None
             The location, in data-coordinates, of the lower-left and
             upper-right corners. If `None`, the image is positioned such that
@@ -526,19 +526,20 @@
                     color='white',
                     fontweight='semibold',
                     fontsize='small',
                     fontfamily='sans-serif',
                     fontvariant='small-caps',
                     bbox=textbox
                     )
-
-    fig.canvas.draw()
+            
+    if fig is not None:
+        fig.canvas.draw()
 
     # SAVE FIGURE
-    if savefig is not None:
+    if savefig is not None and fig is not None:
         dpi = kwargs.pop("dpi", 96)
         format = kwargs.pop("format", "png")
         filename = kwargs.pop("filename", "_spectro_overlayrois")
         filename = savefig + filename + "." + format
         fig.savefig(filename, bbox_inches="tight", dpi=dpi, format=format, **kwargs)
 
     return ax, fig
@@ -557,15 +558,15 @@
     y : 1d ndarray of scalar
         Vector containing the ordinate values (vertical axis)  
     
     ax : axis, optional, default is None
         Draw the signal on this specific axis. Allow multiple plots on the same
         axis.
             
-    \*\*kwargs, optional
+    kwargs, optional
         - figsize : tuple of integers, optional, default: (4,10)
             width, height in inches.  
         - facecolor : matplotlib color, optional, default: 'w' (white)
             the background color.  
         - edgecolor : matplotlib color, optional, default: 'k' (black)
             the border color. 
         - color : matplotlib color, optional, default: 'k' (black)
@@ -642,15 +643,15 @@
     edgecolor = kwargs.pop("edgecolor", "k")
     linewidth = kwargs.pop("linewidth", 0.5)
     color = kwargs.pop("color", "k")
     title = kwargs.pop("figtitle", "")
     xlabel = kwargs.pop("xlabel", "Time [s]")
     ylabel = kwargs.pop("ylabel", "Amplitude [AU]")
     legend = kwargs.pop("legend", None)
-    now = kwargs.pop("now", True)
+    now = kwargs.pop("now", False)
 
     # if no ax, create a figure and a subplot associated a figure otherwise
     # find the figure that belongs to ax
     if ax is None:
         fig, ax = plt.subplots()
         # set the paramters of the figure
         fig.set_figheight(figsize[0])
@@ -832,15 +833,15 @@
     im : 2D numpy array 
         Image or Spectrogram
              
     ax : axis, optional, default is None
         Draw the image on this specific axis. Allow multiple plots on the same
         figure.
             
-    \*\*kwargs, optional
+    kwargs, optional
         - figsize : tuple of integers, optional, default: (4,13)
             width, height in inches.  
         - title : string, optional, default : 'Spectrogram'
             title of the figure
         - xlabel : string, optional, default : 'Time [s]'
             label of the horizontal axis
         - ylabel : string, optional, default : 'Frequency [Hz]'
@@ -904,15 +905,15 @@
     xlabel = kwargs.pop("xlabel", "Time [s]")
     xticks = kwargs.pop("xticks", None)
     yticks = kwargs.pop("yticks", None)
     cmap = kwargs.pop("cmap", "gray")
     vmin = kwargs.pop("vmin", None)
     vmax = kwargs.pop("vmax", None)
     extent = kwargs.pop("extent", None)
-    now = kwargs.pop("now", True)
+    now = kwargs.pop("now", False)
 
     if extent is not None:
         figsize = kwargs.pop(
             "figsize",
             (0.20 * (extent[3] - extent[2]) / 1000, 0.33 * (extent[1] - extent[0])),
         )
     else:
@@ -1559,16 +1560,17 @@
     >>> np.random.seed(2021)
     >>> M = np.random.rand(10, 10)
     >>> df = pd.DataFrame(M)
     >>> indices = ['A','B','C','D','E','F','G','H','I','J']
     >>> df.columns = indices
     >>> maad.util.plot_correlation_map(df, R_threshold=0)
     """
-    # Correlation matrix
-    corr_matrix = df.corr(method)
+    # Correlation matrix with only the columns that contain numeric values
+    numeric_columns = df.select_dtypes(include='number')
+    corr_matrix = numeric_columns.corr()
 
     # pop kwargs
     figsize = kwargs.pop("figsize", (10, 8))
     cmap = kwargs.pop("cmap", "RdBu_r")
     label_colorbar = kwargs.pop("label_colorbar", "R")
 
     fig = plt.figure()
@@ -1652,15 +1654,15 @@
     display : boolean, default is False
         Display False Color Spectro
         
     savefig : string, optional, default is None 
         if not None, figures will be safe. Savefig is the prefix of the save
         filename.
     
-    \*\*kwargs, optional
+    kwargs, optional
        - dpi : scalar, optional, default 96
        - format : str, optional, default .png
     
     Returns
     -------
     false_color_image : ndarray of scalars
         Matrix with ndim = 4 if multiple false color spectro or ndim = 3, if
```

