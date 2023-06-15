# Comparing `tmp/rapid_table-0.0.9-py3-none-any.whl.zip` & `tmp/rapid_table-3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 7076416 bytes, number of entries: 14
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-19 02:02 rapid_table/__init__.py
--rw-r--r--  2.0 unx     3142 b- defN 23-Apr-19 02:02 rapid_table/rapid_table.py
+Zip file size: 7077382 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-15 14:14 rapid_table/__init__.py
+-rw-r--r--  2.0 unx     2759 b- defN 23-Jun-15 14:14 rapid_table/rapid_table.py
+-rw-r--r--  2.0 unx     2707 b- defN 23-Jun-15 14:14 rapid_table/utils.py
 -rw-r--r--  2.0 unx  7704409 b- defN 22-Dec-19 09:03 rapid_table/models/en_ppstructure_mobile_v2_SLANet.onnx
--rw-r--r--  2.0 unx      106 b- defN 23-Apr-19 02:02 rapid_table/table_matcher/__init__.py
--rw-r--r--  2.0 unx     6670 b- defN 23-Apr-19 02:02 rapid_table/table_matcher/matcher.py
--rw-r--r--  2.0 unx    10045 b- defN 23-Apr-19 02:02 rapid_table/table_matcher/utils.py
--rw-r--r--  2.0 unx      653 b- defN 23-Apr-19 02:02 rapid_table/table_structure/__init__.py
--rw-r--r--  2.0 unx     1945 b- defN 23-Apr-19 02:02 rapid_table/table_structure/table_structure.py
--rw-r--r--  2.0 unx    12116 b- defN 23-Apr-19 02:02 rapid_table/table_structure/utils.py
--rw-r--r--  2.0 unx     4883 b- defN 23-Apr-19 02:03 rapid_table-0.0.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 02:03 rapid_table-0.0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 23-Apr-19 02:03 rapid_table-0.0.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-19 02:03 rapid_table-0.0.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1260 b- defN 23-Apr-19 02:03 rapid_table-0.0.9.dist-info/RECORD
-14 files, 7745504 bytes uncompressed, 7074290 bytes compressed:  8.7%
+-rw-r--r--  2.0 unx      106 b- defN 23-Jun-15 14:14 rapid_table/table_matcher/__init__.py
+-rw-r--r--  2.0 unx     6670 b- defN 23-Jun-15 14:14 rapid_table/table_matcher/matcher.py
+-rw-r--r--  2.0 unx    10019 b- defN 23-Jun-15 14:14 rapid_table/table_matcher/utils.py
+-rw-r--r--  2.0 unx      653 b- defN 23-Jun-15 14:14 rapid_table/table_structure/__init__.py
+-rw-r--r--  2.0 unx     1945 b- defN 23-Jun-15 14:14 rapid_table/table_structure/table_structure.py
+-rw-r--r--  2.0 unx    12009 b- defN 23-Jun-15 14:14 rapid_table/table_structure/utils.py
+-rw-r--r--  2.0 unx     4967 b- defN 23-Jun-15 14:15 rapid_table-3.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 14:15 rapid_table-3.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-15 14:15 rapid_table-3.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-15 14:15 rapid_table-3.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1327 b- defN 23-Jun-15 14:15 rapid_table-3.6.dist-info/RECORD
+15 files, 7747846 bytes uncompressed, 7075160 bytes compressed:  8.7%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: rapid_table/__init__.py
 Comment: 
 
 Filename: rapid_table/rapid_table.py
 Comment: 
 
+Filename: rapid_table/utils.py
+Comment: 
+
 Filename: rapid_table/models/en_ppstructure_mobile_v2_SLANet.onnx
 Comment: 
 
 Filename: rapid_table/table_matcher/__init__.py
 Comment: 
 
 Filename: rapid_table/table_matcher/matcher.py
@@ -21,23 +24,23 @@
 
 Filename: rapid_table/table_structure/table_structure.py
 Comment: 
 
 Filename: rapid_table/table_structure/utils.py
 Comment: 
 
-Filename: rapid_table-0.0.9.dist-info/METADATA
+Filename: rapid_table-3.6.dist-info/METADATA
 Comment: 
 
-Filename: rapid_table-0.0.9.dist-info/WHEEL
+Filename: rapid_table-3.6.dist-info/WHEEL
 Comment: 
 
-Filename: rapid_table-0.0.9.dist-info/entry_points.txt
+Filename: rapid_table-3.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapid_table-0.0.9.dist-info/top_level.txt
+Filename: rapid_table-3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: rapid_table-0.0.9.dist-info/RECORD
+Filename: rapid_table-3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapid_table/rapid_table.py

```diff
@@ -1,36 +1,42 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
 import argparse
 import copy
 import time
 from pathlib import Path
+from typing import Union
 
 import cv2
 import numpy as np
 from rapidocr_onnxruntime import RapidOCR
 
 from .table_matcher import TableMatch
 from .table_structure import TableStructurer
+from .utils import LoadImage, vis_table
 
 root_dir = Path(__file__).resolve().parent
 
 
 class RapidTable():
     def __init__(self, model_path: str = None):
         self.ocr_sys = RapidOCR()
 
         if model_path is None:
             model_path = str(root_dir / 'models' / 'en_ppstructure_mobile_v2_SLANet.onnx')
 
         self.table_structure = TableStructurer(model_path)
         self.table_matcher = TableMatch()
 
-    def __call__(self, img):
+        self.load_img = LoadImage()
+
+    def __call__(self, img_content: Union[str, np.ndarray, bytes, Path]):
+        img = self.load_img(img_content)
+
         s = time.time()
         dt_boxes, rec_res = self._ocr(copy.deepcopy(img))
 
         structure_res, _ = self.table_structure(copy.deepcopy(img))
         pred_html = self.table_matcher(structure_res, dt_boxes, rec_res)
 
         elapse = time.time() - s
@@ -52,26 +58,14 @@
             y_max = min(h, box[:, 1].max() + 1)
             box = [x_min, y_min, x_max, y_max]
             r_boxes.append(box)
         dt_boxes = np.array(r_boxes)
         return dt_boxes, rec_res
 
 
-def vis_table(table_res: str, save_path: str) -> None:
-    style_res = '''<style>td {border-left: 1px solid;border-bottom:1px solid;}
-                   table, th {border-top:1px solid;font-size: 10px;
-                   border-collapse: collapse;border-right: 1px solid;}
-                </style>'''
-    prefix_table, suffix_table = table_res.split('<body>')
-    new_table_res = f'{prefix_table}{style_res}<body>{suffix_table}'
-    with open(save_path, 'w', encoding='utf-8') as f:
-        f.write(new_table_res)
-    print(f'The infer result has saved in {save_path}')
-
-
 def main() -> None:
     parser = argparse.ArgumentParser()
     parser.add_argument('-v', '--vis', action='store_true',
                         help='Wheter to visualize the layout results.')
     parser.add_argument('-img', '--img_path', type=str, required=True,
                         help='Path to image for layout.')
     parser.add_argument('-m', '--model_path', type=str,
```

## rapid_table/table_matcher/utils.py

```diff
@@ -8,15 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # -*- encoding: utf-8 -*-
-# -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
 import re
 
 
 def deal_isolate_span(thead_part):
     """
```

## rapid_table/table_structure/utils.py

```diff
@@ -68,15 +68,14 @@
 
 
 class ONNXRuntimeError(Exception):
     pass
 
 
 class TableLabelDecode():
-    """  """
     def __init__(self,
                  dict_character,
                  merge_no_span_structure=True,
                  **kwargs):
         if merge_no_span_structure:
             if "<td></td>" not in dict_character:
                 dict_character.append("<td></td>")
@@ -172,15 +171,15 @@
         result = {
             'bbox_batch_list': bbox_batch_list,
             'structure_batch_list': structure_batch_list,
         }
         return result
 
     def _bbox_decode(self, bbox, shape):
-        h, w, ratio_h, ratio_w, pad_h, pad_w = shape
+        h, w = shape[:2]
         bbox[0::2] *= w
         bbox[1::2] *= h
         return bbox
 
     def get_ignored_tokens(self):
         beg_idx = self.get_beg_end_flag_idx("beg")
         end_idx = self.get_beg_end_flag_idx("end")
@@ -195,15 +194,14 @@
             assert False, "unsupport type %s in get_beg_end_flag_idx" \
                           % beg_or_end
         return idx
 
     def add_special_char(self, dict_character):
         self.beg_str = "sos"
         self.end_str = "eos"
-        dict_character = dict_character
         dict_character = [self.beg_str] + dict_character + [self.end_str]
         return dict_character
 
 
 class TablePreprocess():
     def __init__(self):
         self.table_max_len = 488
@@ -258,16 +256,15 @@
         keep_keys_op = {'KeepKeys': {'keep_keys': ['image', 'shape']}}
         self.pre_process_list = [
             resize_op, normalize_op, pad_op, to_chw_op, keep_keys_op
         ]
 
 
 class ResizeTableImage():
-    def __init__(self, max_len, resize_bboxes=False, infer_mode=False,
-                **kwargs):
+    def __init__(self, max_len, resize_bboxes=False, infer_mode=False):
         super(ResizeTableImage, self).__init__()
         self.max_len = max_len
         self.resize_bboxes = resize_bboxes
         self.infer_mode = infer_mode
 
     def __call__(self, data):
         img = data['image']
```

## Comparing `rapid_table-0.0.9.dist-info/METADATA` & `rapid_table-3.6.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: rapid-table
-Version: 0.0.9
+Version: 3.6
 Summary: Tools for parsing table structures based ONNXRuntime.
 Home-page: https://github.com/RapidAI/RapidStructure
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: ppstructure,table,rapidocr,rapid_table
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
 Requires-Dist: rapidocr-onnxruntime (>=1.1.18)
+Requires-Dist: Pillow
 
 ## rapid-table
 <p align="left">
-    <a href=""><img src="https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg"></a>
+    <a href=""><img src="https://img.shields.io/badge/Python->=3.6,<=3.11-aff.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg"></a>
     <a href="https://pypi.org/project/rapid-table/"><img alt="PyPI" src="https://img.shields.io/pypi/v/rapid-table"></a>
     <a href="https://pepy.tech/project/rapid-table"><img src="https://static.pepy.tech/personalized-badge/rapid-table?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads"></a>
 </p>
 
 ### 1. Install package by pypi.
 ```bash
@@ -36,20 +38,20 @@
 
 ### 2. Run by script.
 - RapidTable has the default `model_path` value, you can set the different value of `model_path` to use different models, e.g. `table_engine = RapidTable(model_path='ch_ppstructure_mobile_v2_SLANet.onnx')`
 - See details, for [README_Table](https://github.com/RapidAI/RapidStructure/blob/main/docs/README_Table.md) .
 - 📌 `table.jpg` source: [link](https://github.com/RapidAI/RapidStructure/blob/main/test_images/table.jpg)
 
 ```python
-import cv2
 from rapid_table import RapidTable
 
 table_engine = RapidTable()
 
-img = cv2.imread('table.jpg')
+with open('table.jpg', 'rb') as f:
+    img = f.read()
 table_html_str, _ = table_engine(img)
 print(table_html_str)
 ```
 
 ### 3. Run by command line.
 ```bash
 $ rapid_table -v -img table.jpg
```

### html2text {}

```diff
@@ -1,33 +1,34 @@
-Metadata-Version: 2.1 Name: rapid-table Version: 0.0.9 Summary: Tools for
-parsing table structures based ONNXRuntime. Home-page: https://github.com/
-RapidAI/RapidStructure Author: SWHL Author-email: liekkaskono@163.com License:
-Apache-2.0 Keywords: ppstructure,table,rapidocr,rapid_table Platform: Any
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Requires-Python: >=3.6,<=3.10 Description-Content-
-Type: text/markdown Requires-Dist: onnxruntime (>=1.7.0) Requires-Dist: PyYAML
-(>=6.0) Requires-Dist: opencv-python (>=4.5.1.48) Requires-Dist: numpy
-(>=1.21.6) Requires-Dist: rapidocr-onnxruntime (>=1.1.18) ## rapid-table
-[https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
+Metadata-Version: 2.1 Name: rapid-table Version: 3.6 Summary: Tools for parsing
+table structures based ONNXRuntime. Home-page: https://github.com/RapidAI/
+RapidStructure Author: SWHL Author-email: liekkaskono@163.com License: Apache-
+2.0 Keywords: ppstructure,table,rapidocr,rapid_table Platform: Any Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.6,<=3.11 Description-Content-Type: text/markdown Requires-Dist:
+onnxruntime (>=1.7.0) Requires-Dist: PyYAML (>=6.0) Requires-Dist: opencv-
+python (>=4.5.1.48) Requires-Dist: numpy (>=1.21.6) Requires-Dist: rapidocr-
+onnxruntime (>=1.1.18) Requires-Dist: Pillow ## rapid-table
+[https://img.shields.io/badge/Python->=3.6,<=3.11-aff.svg] [https://
 img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg] [PyPI] [https://
 static.pepy.tech/personalized-badge/rapid-
 table?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads]
 ### 1. Install package by pypi. ```bash $ pip install rapid-table ``` ### 2.
 Run by script. - RapidTable has the default `model_path` value, you can set the
 different value of `model_path` to use different models, e.g. `table_engine =
 RapidTable(model_path='ch_ppstructure_mobile_v2_SLANet.onnx')` - See details,
 for [README_Table](https://github.com/RapidAI/RapidStructure/blob/main/docs/
 README_Table.md) . - ð `table.jpg` source: [link](https://github.com/
-RapidAI/RapidStructure/blob/main/test_images/table.jpg) ```python import cv2
-from rapid_table import RapidTable table_engine = RapidTable() img = cv2.imread
-('table.jpg') table_html_str, _ = table_engine(img) print(table_html_str) ```
-### 3. Run by command line. ```bash $ rapid_table -v -img table.jpg ``` ### 4.
-Result. - Return value. ```html
+RapidAI/RapidStructure/blob/main/test_images/table.jpg) ```python from
+rapid_table import RapidTable table_engine = RapidTable() with open
+('table.jpg', 'rb') as f: img = f.read() table_html_str, _ = table_engine(img)
+print(table_html_str) ``` ### 3. Run by command line. ```bash $ rapid_table -
+v -img table.jpg ``` ### 4. Result. - Return value. ```html
 Methods                            FPS
 SegLink [26]   70.0  86d>    77.0  8.9
                      0
 PixelLink [4]  73.2  83.0    77.8
 TextSnake [18] 73.9  83.2    78.3  1.1
 TextField [37] 75.9  87.4    81.3  5.2
 MSR[38]        76.7  87.87.4 81.7
```

## Comparing `rapid_table-0.0.9.dist-info/RECORD` & `rapid_table-3.6.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 rapid_table/__init__.py,sha256=qdYnOhgN-tNAExRe48Dzib6eorDhoWQTJ0FHAMws1kI,110
-rapid_table/rapid_table.py,sha256=lXtXazDr9s0E_V2XnChA3PHeNq4hMA0r2p-pn_qhLGw,3142
+rapid_table/rapid_table.py,sha256=-U88HJT20ClcKsX9-Yj3N2tAAyeRjxOkxihJ8MWqFus,2759
+rapid_table/utils.py,sha256=EERheshF9IFWMALJ1_GnANxWonGihmexZtiPHfUbm8s,2707
 rapid_table/models/en_ppstructure_mobile_v2_SLANet.onnx,sha256=LK4X0WoW-d9yKeIWZf4_vgbzyoWyAkdy7j4xQulVqmA,7704409
 rapid_table/table_matcher/__init__.py,sha256=MG5RnW1TllQdYPDoCEAWjhcAKEez44kaNHegLOW--Gk,106
 rapid_table/table_matcher/matcher.py,sha256=A8gVZ2XQJqWA87HK5b-_Ql8raY94rauS9g3QOjnha6w,6670
-rapid_table/table_matcher/utils.py,sha256=sqOCUuelNGzbfvs7mb8JHbKmn-pvNjQtHp2fhgDG6Fs,10045
+rapid_table/table_matcher/utils.py,sha256=2TbkdclD0Y9lOVO_xuqlGcdR_kVwpuAYW4eu3UJwUvA,10019
 rapid_table/table_structure/__init__.py,sha256=N_1OGAgiMrF4LB5_sP_OSOrh6pnBGZrrnph8RfQ3VHA,653
 rapid_table/table_structure/table_structure.py,sha256=0QyKU9c6J-H5kCGET09NVjkHV-xa5pMC-JERvMnY-Ow,1945
-rapid_table/table_structure/utils.py,sha256=_aeKapmhI_U-DzmizrhyTZ4iK8YD-eefS3pFKuUy_oQ,12116
-rapid_table-0.0.9.dist-info/METADATA,sha256=iH6zLmmBuOa8ZrNyvKBy3BLorndQup0wUCQmq6eJJFE,4883
-rapid_table-0.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rapid_table-0.0.9.dist-info/entry_points.txt,sha256=a4UsMSxd7Ex1mZvdIT5AmkuiUAvB__awLj-NeYU8bsQ,61
-rapid_table-0.0.9.dist-info/top_level.txt,sha256=DkBPZpaze8SaoAvCufxilNpITY4n-rHH1lgHr6KHPgA,12
-rapid_table-0.0.9.dist-info/RECORD,,
+rapid_table/table_structure/utils.py,sha256=fDK5G9N6DfG-IGE_fZ4l85ypjXSR33cK4R5P5X5l1Ws,12009
+rapid_table-3.6.dist-info/METADATA,sha256=e83v94q0OqFaLMB5fOatNvPnY_AiwvuLwhICSDVyJvo,4967
+rapid_table-3.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rapid_table-3.6.dist-info/entry_points.txt,sha256=a4UsMSxd7Ex1mZvdIT5AmkuiUAvB__awLj-NeYU8bsQ,61
+rapid_table-3.6.dist-info/top_level.txt,sha256=DkBPZpaze8SaoAvCufxilNpITY4n-rHH1lgHr6KHPgA,12
+rapid_table-3.6.dist-info/RECORD,,
```

