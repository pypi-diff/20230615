# Comparing `tmp/rapid_orientation-0.0.6-py3-none-any.whl.zip` & `tmp/rapid_orientation-3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6289942 bytes, number of entries: 10
--rw-r--r--  2.0 unx      122 b- defN 23-Jun-14 14:37 rapid_orientation/__init__.py
--rw-r--r--  2.0 unx      350 b- defN 23-Jun-14 14:37 rapid_orientation/config.yaml
--rw-r--r--  2.0 unx     2804 b- defN 23-Jun-14 14:37 rapid_orientation/rapid_orientation.py
--rw-r--r--  2.0 unx     7735 b- defN 23-Jun-14 14:37 rapid_orientation/utils.py
+Zip file size: 6289921 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      122 b- defN 23-Jun-15 14:14 rapid_orientation/__init__.py
+-rw-r--r--  2.0 unx      350 b- defN 23-Jun-15 14:14 rapid_orientation/config.yaml
+-rw-r--r--  2.0 unx     2804 b- defN 23-Jun-15 14:14 rapid_orientation/rapid_orientation.py
+-rw-r--r--  2.0 unx     7735 b- defN 23-Jun-15 14:14 rapid_orientation/utils.py
 -rw-rw-r--  2.0 unx  6792721 b- defN 23-Jan-20 13:53 rapid_orientation/models/rapid_orientation.onnx
--rw-r--r--  2.0 unx     2759 b- defN 23-Jun-14 14:38 rapid_orientation-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 14:38 rapid_orientation-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-14 14:38 rapid_orientation-0.0.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 23-Jun-14 14:38 rapid_orientation-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      898 b- defN 23-Jun-14 14:38 rapid_orientation-0.0.6.dist-info/RECORD
-10 files, 6807578 bytes uncompressed, 6288386 bytes compressed:  7.6%
+-rw-r--r--  2.0 unx     2808 b- defN 23-Jun-15 14:15 rapid_orientation-3.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 14:15 rapid_orientation-3.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-15 14:15 rapid_orientation-3.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-15 14:15 rapid_orientation-3.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      888 b- defN 23-Jun-15 14:15 rapid_orientation-3.6.dist-info/RECORD
+10 files, 6807617 bytes uncompressed, 6288385 bytes compressed:  7.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: rapid_orientation/utils.py
 Comment: 
 
 Filename: rapid_orientation/models/rapid_orientation.onnx
 Comment: 
 
-Filename: rapid_orientation-0.0.6.dist-info/METADATA
+Filename: rapid_orientation-3.6.dist-info/METADATA
 Comment: 
 
-Filename: rapid_orientation-0.0.6.dist-info/WHEEL
+Filename: rapid_orientation-3.6.dist-info/WHEEL
 Comment: 
 
-Filename: rapid_orientation-0.0.6.dist-info/entry_points.txt
+Filename: rapid_orientation-3.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapid_orientation-0.0.6.dist-info/top_level.txt
+Filename: rapid_orientation-3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: rapid_orientation-0.0.6.dist-info/RECORD
+Filename: rapid_orientation-3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rapid_orientation-0.0.6.dist-info/METADATA` & `rapid_orientation-3.6.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: rapid-orientation
-Version: 0.0.6
+Version: 3.6
 Summary: Tools for classifying the direction of images containing text based ONNXRuntime.
 Home-page: https://github.com/RapidAI/RapidStructure
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: ppstructure,layout,rapidocr,rapid_orientation
 Platform: Any
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6,<=3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6,<=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: onnxruntime (>=1.7.0)
 Requires-Dist: PyYAML (>=6.0)
 Requires-Dist: opencv-python (>=4.5.1.48)
 Requires-Dist: numpy (>=1.21.6)
 Requires-Dist: Pillow
 
 ## rapid-orientation
 <p align="left">
-    <a href=""><img src="https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg"></a>
+    <a href=""><img src="https://img.shields.io/badge/Python->=3.6,<=3.11-aff.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg"></a>
     <a href="https://pypi.org/project/rapid-orientation/"><img alt="PyPI" src="https://img.shields.io/pypi/v/rapid-orientation"></a>
     <a href="https://pepy.tech/project/rapid-orientation"><img src="https://static.pepy.tech/personalized-badge/rapid-orientation?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads"></a>
 </p>
 
 ### 1. Install package by pypi.
 ```bash
```

### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: rapid-orientation Version: 0.0.6 Summary: Tools for
+Metadata-Version: 2.1 Name: rapid-orientation Version: 3.6 Summary: Tools for
 classifying the direction of images containing text based ONNXRuntime. Home-
 page: https://github.com/RapidAI/RapidStructure Author: SWHL Author-email:
 liekkaskono@163.com License: Apache-2.0 Keywords:
 ppstructure,layout,rapidocr,rapid_orientation Platform: Any Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Requires-Python: >=3.6,<=3.10 Description-Content-Type: text/
-markdown Requires-Dist: onnxruntime (>=1.7.0) Requires-Dist: PyYAML (>=6.0)
-Requires-Dist: opencv-python (>=4.5.1.48) Requires-Dist: numpy (>=1.21.6)
-Requires-Dist: Pillow ## rapid-orientation
-[https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.6,<=3.11 Description-Content-Type: text/markdown Requires-Dist:
+onnxruntime (>=1.7.0) Requires-Dist: PyYAML (>=6.0) Requires-Dist: opencv-
+python (>=4.5.1.48) Requires-Dist: numpy (>=1.21.6) Requires-Dist: Pillow ##
+rapid-orientation
+[https://img.shields.io/badge/Python->=3.6,<=3.11-aff.svg] [https://
 img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg] [PyPI] [https://
 static.pepy.tech/personalized-badge/rapid-
 orientation?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads]
 ### 1. Install package by pypi. ```bash $ pip install rapid-orientation ``` ###
 2. Run by script. - RapidOrientation has the default `model_path` value, you
 can set the different value of `model_path` to use different models, e.g.
 `orientation_engine = RapidOrientation(model_path='rapid_orientation.onnx')` -
```

## Comparing `rapid_orientation-0.0.6.dist-info/RECORD` & `rapid_orientation-3.6.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 rapid_orientation/__init__.py,sha256=WYYdZeKq1BvJkoBpnM-9QZs1Nbx6RV9uagmVFrwGvxU,122
 rapid_orientation/config.yaml,sha256=6FyPLomim5pAjMZtKUO75NLV9XKGgyKihXItxFX-Wb4,350
 rapid_orientation/rapid_orientation.py,sha256=HSuXtvqnooy2Gm0--n2md6nLNDdrODuyJ1ysAC6aJ60,2804
 rapid_orientation/utils.py,sha256=hSoDYMQL_CPmgHioRTLkJt1Wk5ZLeqPYxvcKqT2byWc,7735
 rapid_orientation/models/rapid_orientation.onnx,sha256=nIShBBuY_HQTLRHtraf1r8jJEfrjVc3n0ExijTSvHYo,6792721
-rapid_orientation-0.0.6.dist-info/METADATA,sha256=7RhL24DyXX79VbVbDq8oC916Ss5hYu_dcc87ADB-DfQ,2759
-rapid_orientation-0.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rapid_orientation-0.0.6.dist-info/entry_points.txt,sha256=Yncu1HqYh7MxLxZvupD5ut3hJbU1DWxYCrtANCxbbBg,79
-rapid_orientation-0.0.6.dist-info/top_level.txt,sha256=6Xiql6N2aF4rctCG2D0W55YnVe7aS-9dSZJ6lEYejLc,18
-rapid_orientation-0.0.6.dist-info/RECORD,,
+rapid_orientation-3.6.dist-info/METADATA,sha256=xnZ8CTZs8sSZF4qiZgThX1e-2cbIONuRX4meINpvrTc,2808
+rapid_orientation-3.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rapid_orientation-3.6.dist-info/entry_points.txt,sha256=Yncu1HqYh7MxLxZvupD5ut3hJbU1DWxYCrtANCxbbBg,79
+rapid_orientation-3.6.dist-info/top_level.txt,sha256=6Xiql6N2aF4rctCG2D0W55YnVe7aS-9dSZJ6lEYejLc,18
+rapid_orientation-3.6.dist-info/RECORD,,
```

