# Comparing `tmp/pynir-0.7.7.tar.gz` & `tmp/pynir-0.7.8.tar.gz`

## Comparing `pynir-0.7.7.tar` & `pynir-0.7.8.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pynir-0.7.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/Makefile
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/conf.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/make.bat
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/modules.rst
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/pynir.rst
--rw-r--r--   0        0        0   530403 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/doctrees/environment.pickle
--rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/doctrees/index.doctree
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/doctrees/modules.doctree
--rw-r--r--   0        0        0   279145 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/doctrees/pynir.doctree
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/.buildinfo
--rw-r--r--   0        0        0    21444 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/genindex.html
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/index.html
--rw-r--r--   0        0        0    26832 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/modules.html
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/objects.inv
--rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/py-modindex.html
--rw-r--r--   0        0        0   118287 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/pynir.html
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/search.html
--rw-r--r--   0        0        0    13003 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/searchindex.js
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_modules/index.html
--rw-r--r--   0        0        0   102728 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_modules/pynir/Calibration.html
--rw-r--r--   0        0        0    73899 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_modules/pynir/CalibrationTransfer.html
--rw-r--r--   0        0        0    53422 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_modules/pynir/FeatureSelection.html
--rw-r--r--   0        0        0    15283 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_modules/pynir/OutlierDection.html
--rw-r--r--   0        0        0    24364 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_modules/pynir/Preprocessing.html
--rw-r--r--   0        0        0    25985 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_modules/pynir/utils.html
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_sources/pynir.rst.txt
--rw-r--r--   0        0        0    11185 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/alabaster.css
--rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/basic.css
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/doctools.js
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/file.png
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/plus.png
--rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0  1215471 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Data_Corn.mat
--rw-r--r--   0        0        0  5505213 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Data_Tablet.mat
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo10_calibrationTransfer_PFCE_simulateNIR.py
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo11_calibrationTransfer_PFCE_Tablet.py
--rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo12_calibrationTransfer_PFCE_Corn.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo1_SimulateNIR.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo2_Regression.py
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo3_Binary_Classification.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo4_Multiclass_Classification.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo5_dataPreprocessing.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo6_outierDection.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo7_FeatureSelection_oneStep.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo8_FeatureSelection_multiSteps.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo9_calibrationTransfer.py
--rw-r--r--   0        0        0    20004 2020-02-02 00:00:00.000000 pynir-0.7.7/src/pynir/Calibration.py
--rw-r--r--   0        0        0    11020 2020-02-02 00:00:00.000000 pynir-0.7.7/src/pynir/CalibrationTransfer.py
--rw-r--r--   0        0        0     8536 2020-02-02 00:00:00.000000 pynir-0.7.7/src/pynir/FeatureSelection.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 pynir-0.7.7/src/pynir/OutlierDection.py
--rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 pynir-0.7.7/src/pynir/Preprocessing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pynir-0.7.7/src/pynir/__init__.py
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 pynir-0.7.7/src/pynir/utils.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pynir-0.7.7/LICENSE.txt
--rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 pynir-0.7.7/README.md
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pynir-0.7.7/pyproject.toml
--rw-r--r--   0        0        0     9025 2020-02-02 00:00:00.000000 pynir-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pynir-0.7.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/Makefile
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/conf.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/make.bat
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/modules.rst
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/pynir.rst
+-rw-r--r--   0        0        0   530403 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/doctrees/index.doctree
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/doctrees/modules.doctree
+-rw-r--r--   0        0        0   279145 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/doctrees/pynir.doctree
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/.buildinfo
+-rw-r--r--   0        0        0    21444 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/genindex.html
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/index.html
+-rw-r--r--   0        0        0    26832 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/modules.html
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/objects.inv
+-rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/py-modindex.html
+-rw-r--r--   0        0        0   118287 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/pynir.html
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/search.html
+-rw-r--r--   0        0        0    13003 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/searchindex.js
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_modules/index.html
+-rw-r--r--   0        0        0   102728 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_modules/pynir/Calibration.html
+-rw-r--r--   0        0        0    73899 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_modules/pynir/CalibrationTransfer.html
+-rw-r--r--   0        0        0    53422 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_modules/pynir/FeatureSelection.html
+-rw-r--r--   0        0        0    15283 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_modules/pynir/OutlierDection.html
+-rw-r--r--   0        0        0    24364 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_modules/pynir/Preprocessing.html
+-rw-r--r--   0        0        0    25985 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_modules/pynir/utils.html
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_sources/pynir.rst.txt
+-rw-r--r--   0        0        0    11185 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_static/doctools.js
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_static/file.png
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_static/plus.png
+-rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 pynir-0.7.8/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0  1215471 2020-02-02 00:00:00.000000 pynir-0.7.8/examples/Data_Corn.mat
+-rw-r--r--   0        0        0  5505213 2020-02-02 00:00:00.000000 pynir-0.7.8/examples/Data_Tablet.mat
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 pynir-0.7.8/examples/Demo10_calibrationTransfer_PFCE_simulateNIR.py
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 pynir-0.7.8/examples/Demo11_calibrationTransfer_PFCE_Tablet.py
+-rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 pynir-0.7.8/examples/Demo12_calibrationTransfer_PFCE_Corn.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pynir-0.7.8/examples/Demo1_SimulateNIR.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 pynir-0.7.8/examples/Demo2_Regression.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 pynir-0.7.8/examples/Demo3_Binary_Classification.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 pynir-0.7.8/examples/Demo4_Multiclass_Classification.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pynir-0.7.8/examples/Demo5_dataPreprocessing.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 pynir-0.7.8/examples/Demo6_outierDection.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 pynir-0.7.8/examples/Demo7_FeatureSelection_oneStep.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 pynir-0.7.8/examples/Demo8_FeatureSelection_multiSteps.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 pynir-0.7.8/examples/Demo9_calibrationTransfer.py
+-rw-r--r--   0        0        0    20004 2020-02-02 00:00:00.000000 pynir-0.7.8/src/pynir/Calibration.py
+-rw-r--r--   0        0        0    11020 2020-02-02 00:00:00.000000 pynir-0.7.8/src/pynir/CalibrationTransfer.py
+-rw-r--r--   0        0        0     8536 2020-02-02 00:00:00.000000 pynir-0.7.8/src/pynir/FeatureSelection.py
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 pynir-0.7.8/src/pynir/OutlierDetection.py
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 pynir-0.7.8/src/pynir/Preprocessing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pynir-0.7.8/src/pynir/__init__.py
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 pynir-0.7.8/src/pynir/utils.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pynir-0.7.8/LICENSE.txt
+-rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 pynir-0.7.8/README.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pynir-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0     9025 2020-02-02 00:00:00.000000 pynir-0.7.8/PKG-INFO
```

### Comparing `pynir-0.7.7/.github/workflows/python-publish.yml` & `pynir-0.7.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/Makefile` & `pynir-0.7.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/conf.py` & `pynir-0.7.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/make.bat` & `pynir-0.7.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/pynir.rst` & `pynir-0.7.8/docs/pynir.rst`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/doctrees/environment.pickle` & `pynir-0.7.8/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/doctrees/index.doctree` & `pynir-0.7.8/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/doctrees/modules.doctree` & `pynir-0.7.8/docs/_build/doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/doctrees/pynir.doctree` & `pynir-0.7.8/docs/_build/doctrees/pynir.doctree`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/genindex.html` & `pynir-0.7.8/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/index.html` & `pynir-0.7.8/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/modules.html` & `pynir-0.7.8/docs/_build/html/modules.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/objects.inv` & `pynir-0.7.8/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/py-modindex.html` & `pynir-0.7.8/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/pynir.html` & `pynir-0.7.8/docs/_build/html/pynir.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/search.html` & `pynir-0.7.8/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/searchindex.js` & `pynir-0.7.8/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/_modules/index.html` & `pynir-0.7.8/docs/_build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/_modules/pynir/Calibration.html` & `pynir-0.7.8/docs/_build/html/_modules/pynir/Calibration.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/_modules/pynir/CalibrationTransfer.html` & `pynir-0.7.8/docs/_build/html/_modules/pynir/CalibrationTransfer.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/_modules/pynir/FeatureSelection.html` & `pynir-0.7.8/docs/_build/html/_modules/pynir/FeatureSelection.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/_modules/pynir/OutlierDection.html` & `pynir-0.7.8/docs/_build/html/_modules/pynir/OutlierDection.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/_modules/pynir/Preprocessing.html` & `pynir-0.7.8/docs/_build/html/_modules/pynir/Preprocessing.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/_modules/pynir/utils.html` & `pynir-0.7.8/docs/_build/html/_modules/pynir/utils.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/_sources/pynir.rst.txt` & `pynir-0.7.8/docs/_build/html/_sources/pynir.rst.txt`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/_static/alabaster.css` & `pynir-0.7.8/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/_static/basic.css` & `pynir-0.7.8/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/_static/doctools.js` & `pynir-0.7.8/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/_static/language_data.js` & `pynir-0.7.8/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/_static/pygments.css` & `pynir-0.7.8/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/_static/searchtools.js` & `pynir-0.7.8/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/docs/_build/html/_static/sphinx_highlight.js` & `pynir-0.7.8/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/examples/Data_Corn.mat` & `pynir-0.7.8/examples/Data_Corn.mat`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/examples/Data_Tablet.mat` & `pynir-0.7.8/examples/Data_Tablet.mat`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/examples/Demo10_calibrationTransfer_PFCE_simulateNIR.py` & `pynir-0.7.8/examples/Demo10_calibrationTransfer_PFCE_simulateNIR.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/examples/Demo11_calibrationTransfer_PFCE_Tablet.py` & `pynir-0.7.8/examples/Demo11_calibrationTransfer_PFCE_Tablet.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/examples/Demo12_calibrationTransfer_PFCE_Corn.py` & `pynir-0.7.8/examples/Demo12_calibrationTransfer_PFCE_Corn.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/examples/Demo1_SimulateNIR.py` & `pynir-0.7.8/examples/Demo1_SimulateNIR.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/examples/Demo2_Regression.py` & `pynir-0.7.8/examples/Demo2_Regression.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/examples/Demo3_Binary_Classification.py` & `pynir-0.7.8/examples/Demo3_Binary_Classification.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/examples/Demo4_Multiclass_Classification.py` & `pynir-0.7.8/examples/Demo4_Multiclass_Classification.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/examples/Demo5_dataPreprocessing.py` & `pynir-0.7.8/examples/Demo5_dataPreprocessing.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/examples/Demo6_outierDection.py` & `pynir-0.7.8/examples/Demo6_outierDection.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     sys.path.insert(0, pynir_dir)
     
 import numpy as np
 import matplotlib.pyplot as plt
 
 from pynir.utils import simulateNIR
 
-from pynir.OutlierDection import outlierDection_PLS
+from pynir.OutlierDection import outlierDetection_PLS
 
 # simulate NIR data
 X,y,wv = simulateNIR(nSample=200,n_components=10,noise=1e-5)
 
-ODModel = outlierDection_PLS(ncomp=3)
+ODModel = outlierDetection_PLS(ncomp=3)
 Q, Tsq, Q_conf, Tsq_conf, idxOutlier = ODModel.fit(X, y).detect(X,y)
 ODModel.plot_HotellingT2_Q(Q, Tsq, Q_conf, Tsq_conf)
```

### Comparing `pynir-0.7.7/examples/Demo7_FeatureSelection_oneStep.py` & `pynir-0.7.8/examples/Demo7_FeatureSelection_oneStep.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/examples/Demo8_FeatureSelection_multiSteps.py` & `pynir-0.7.8/examples/Demo8_FeatureSelection_multiSteps.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/examples/Demo9_calibrationTransfer.py` & `pynir-0.7.8/examples/Demo9_calibrationTransfer.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/src/pynir/Calibration.py` & `pynir-0.7.8/src/pynir/Calibration.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/src/pynir/CalibrationTransfer.py` & `pynir-0.7.8/src/pynir/CalibrationTransfer.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/src/pynir/FeatureSelection.py` & `pynir-0.7.8/src/pynir/FeatureSelection.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/src/pynir/Preprocessing.py` & `pynir-0.7.8/src/pynir/Preprocessing.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/src/pynir/utils.py` & `pynir-0.7.8/src/pynir/utils.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/LICENSE.txt` & `pynir-0.7.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/README.md` & `pynir-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `pynir-0.7.7/pyproject.toml` & `pynir-0.7.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pynir"
-version = "0.7.7"
+version = "0.7.8"
 authors = [{ name = "Jin Zhang", email = "jinzhang@nankai.edu.cn" }]
 description = "NIR calibration toolbox in python"
 readme = "README.md"
 requires-python = ">=3.7"
 
 dependencies = [
   "numpy",
```

### Comparing `pynir-0.7.7/PKG-INFO` & `pynir-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynir
-Version: 0.7.7
+Version: 0.7.8
 Summary: NIR calibration toolbox in python
 Project-URL: Homepage, https://github.com/JinZhangLab/pynir
 Project-URL: Bug Tracker, https://github.com/JinZhangLab/pynir/issues
 Project-URL: Documentation, https://pynir.readthedocs.io/en/latest/
 Author-email: Jin Zhang <jinzhang@nankai.edu.cn>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
```

