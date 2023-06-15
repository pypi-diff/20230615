# Comparing `tmp/paddleocr_convert-0.0.8-py3-none-any.whl.zip` & `tmp/paddleocr_convert-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11548 bytes, number of entries: 9
--rw-r--r--  2.0 unx      701 b- defN 23-Mar-06 01:27 paddleocr_convert/__init__.py
--rw-r--r--  2.0 unx     6317 b- defN 23-Mar-06 01:27 paddleocr_convert/main.py
--rw-r--r--  2.0 unx     3336 b- defN 23-Mar-06 01:27 paddleocr_convert/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Mar-06 01:28 paddleocr_convert-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     3749 b- defN 23-Mar-06 01:28 paddleocr_convert-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-06 01:28 paddleocr_convert-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       66 b- defN 23-Mar-06 01:28 paddleocr_convert-0.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 23-Mar-06 01:28 paddleocr_convert-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      792 b- defN 23-Mar-06 01:28 paddleocr_convert-0.0.8.dist-info/RECORD
-9 files, 26428 bytes uncompressed, 10164 bytes compressed:  61.5%
+Zip file size: 11867 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     1249 b- defN 23-Mar-06 06:27 paddleocr_convert/__init__.py
+-rw-r--r--  2.0 unx     6317 b- defN 23-Mar-06 06:27 paddleocr_convert/main.py
+-rw-r--r--  2.0 unx     3336 b- defN 23-Mar-06 06:27 paddleocr_convert/utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Mar-06 06:27 paddleocr_convert-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3977 b- defN 23-Mar-06 06:27 paddleocr_convert-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Mar-06 06:27 paddleocr_convert-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       66 b- defN 23-Mar-06 06:27 paddleocr_convert-0.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 23-Mar-06 06:27 paddleocr_convert-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      793 b- defN 23-Mar-06 06:27 paddleocr_convert-0.0.9.dist-info/RECORD
+9 files, 27205 bytes uncompressed, 10483 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: paddleocr_convert/main.py
 Comment: 
 
 Filename: paddleocr_convert/utils.py
 Comment: 
 
-Filename: paddleocr_convert-0.0.8.dist-info/LICENSE
+Filename: paddleocr_convert-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: paddleocr_convert-0.0.8.dist-info/METADATA
+Filename: paddleocr_convert-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: paddleocr_convert-0.0.8.dist-info/WHEEL
+Filename: paddleocr_convert-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: paddleocr_convert-0.0.8.dist-info/entry_points.txt
+Filename: paddleocr_convert-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: paddleocr_convert-0.0.8.dist-info/top_level.txt
+Filename: paddleocr_convert-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: paddleocr_convert-0.0.8.dist-info/RECORD
+Filename: paddleocr_convert-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## paddleocr_convert/__init__.py

```diff
@@ -1,44 +1,79 @@
 00000000: 2320 2d2a 2d20 656e 636f 6469 6e67 3a20  # -*- encoding: 
 00000010: 7574 662d 3820 2d2a 2d0a 2320 4041 7574  utf-8 -*-.# @Aut
 00000020: 686f 723a 2053 5748 4c0a 2320 4043 6f6e  hor: SWHL.# @Con
 00000030: 7461 6374 3a20 6c69 656b 6b61 736b 6f6e  tact: liekkaskon
-00000040: 6f40 3136 332e 636f 6d0a 2222 220a e8af  o@163.com."""...
-00000050: a5e6 a8a1 e59d 97e6 98af 7061 6464 6c65  ..........paddle
-00000060: 6f63 725f 636f 6e76 6572 74e8 bdac e68d  ocr_convert.....
-00000070: a2e6 a8a1 e59e 8be7 9a84 e6a0 b8e5 bf83  ................
-00000080: e4bb a3e7 a081 e380 82e4 b8bb e8a6 81e5  ................
-00000090: 8c85 e68b ace4 b88b e8bd bde6 a8a1 e59e  ................
-000000a0: 8be3 8081 e8a7 a3e5 8e8b e6a8 a1e5 9e8b  ................
-000000b0: e380 81e8 bdac e68d a2e6 a8a1 e59e 8be5  ................
-000000c0: 928c e69b b4e6 94b9 e6a8 a1e5 9e8b e4b8  ................
-000000d0: bae5 8aa8 e680 81e8 be93 e585 a5e5 9b9b  ................
-000000e0: e983 a8e5 8886 e380 820a e794 b1e4 ba8e  ................
-000000f0: e79b aee5 898d 6070 6164 646c 6532 6f6e  ......`paddle2on
-00000100: 6e78 60e8 bdac e68d a2e5 b7a5 e585 b7e8  nx`.............
-00000110: be83 e4b8 bae6 8890 e786 9fef bc8c e58f  ................
-00000120: afe4 bba5 e5b0 b1e6 b2a1 e69c 89e6 b7bb  ................
-00000130: e58a a0e8 bdac e68d a2e5 898d e590 8ee6  ................
-00000140: a8a1 e59e 8be7 b2be e5ba a6e9 aa8c e8af  ................
-00000150: 81e6 98af e590 a6e6 bba1 e8b6 b3e8 a681  ................
-00000160: e6b1 82e7 9a84 e693 8de4 bd9c e380 820a  ................
-00000170: 0ae6 94af e68c 81e6 a8a1 e59e 8be7 9a84  ................
-00000180: 7572 6ce5 928c e69c ace5 9cb0 e8b7 afe5  url.............
-00000190: be84 e4b8 a4e7 a78d e8be 93e5 85a5 e696  ................
-000001a0: b9e5 bc8f e380 82e5 85b6 e4b8 ade9 9288  ................
-000001b0: e5af b960 7265 6360 e79a 84e6 a8a1 e59e  ...`rec`........
-000001c0: 8bef bc8c e99c 80e8 a681 e68f 90e4 be9b  ................
-000001d0: e5af b9e5 ba94 e79a 84e5 ad97 e585 b8e6  ................
-000001e0: 9687 e4bb b6ef bc8c e8af a5e5 ba93 e4bc  ................
-000001f0: 9ae8 87aa e58a a8e5 b086 e5ad 97e5 85b8  ................
-00000200: e696 87e4 bbb6 e586 99e5 85a5 e588 b06f  ...............o
-00000210: 6e6e 78e4 b8ad e380 820a e8bf 99e9 878c  nnx.............
-00000220: e99c 80e8 a681 e690 ade9 858d 5b52 6170  ............[Rap
-00000230: 6964 4f43 525d 2868 7474 7073 3a2f 2f67  idOCR](https://g
-00000240: 6974 6875 622e 636f 6d2f 5261 7069 6441  ithub.com/RapidA
-00000250: 492f 5261 7069 644f 4352 29e6 8ea8 e790  I/RapidOCR).....
-00000260: 86e4 bba3 e7a0 81e4 bdbf e794 a80a 0a22  ..............."
-00000270: 2222 0a0a 6672 6f6d 202e 6d61 696e 2069  ""..from .main i
-00000280: 6d70 6f72 7420 5061 6464 6c65 4f43 524d  mport PaddleOCRM
-00000290: 6f64 656c 436f 6e76 6572 740a 6672 6f6d  odelConvert.from
-000002a0: 202e 7574 696c 7320 696d 706f 7274 2064   .utils import d
-000002b0: 6f77 6e6c 6f61 645f 6669 6c65 0a         ownload_file.
+00000040: 6f40 3136 332e 636f 6d0a 2222 220a 3c70  o@163.com.""".<p
+00000050: 3e0a 2020 2020 3c61 2068 7265 663d 2222  >.    <a href=""
+00000060: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+00000070: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000080: 6f2f 6261 6467 652f 5079 7468 6f6e 2d3e  o/badge/Python->
+00000090: 3d33 2e37 2c3c 3d33 2e31 302d 6166 662e  =3.7,<=3.10-aff.
+000000a0: 7376 6722 3e3c 2f61 3e0a 2020 2020 3c61  svg"></a>.    <a
+000000b0: 2068 7265 663d 2222 3e3c 696d 6720 7372   href=""><img sr
+000000c0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+000000d0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+000000e0: 4f53 2d4c 696e 7578 2532 4325 3230 5769  OS-Linux%2C%20Wi
+000000f0: 6e25 3243 2532 304d 6163 2d70 696e 6b2e  n%2C%20Mac-pink.
+00000100: 7376 6722 3e3c 2f61 3e0a 2020 2020 3c61  svg"></a>.    <a
+00000110: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
+00000120: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+00000130: 7061 6464 6c65 6f63 725f 636f 6e76 6572  paddleocr_conver
+00000140: 742f 223e 3c69 6d67 2061 6c74 3d22 5079  t/"><img alt="Py
+00000150: 5049 2220 7372 633d 2268 7474 7073 3a2f  PI" src="https:/
+00000160: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000170: 7079 7069 2f76 2f70 6164 646c 656f 6372  pypi/v/paddleocr
+00000180: 5f63 6f6e 7665 7274 223e 3c2f 613e 0a20  _convert"></a>. 
+00000190: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
+000001a0: 733a 2f2f 7065 7079 2e74 6563 682f 7072  s://pepy.tech/pr
+000001b0: 6f6a 6563 742f 7061 6464 6c65 6f63 725f  oject/paddleocr_
+000001c0: 636f 6e76 6572 7422 3e3c 696d 6720 7372  convert"><img sr
+000001d0: 633d 2268 7474 7073 3a2f 2f73 7461 7469  c="https://stati
+000001e0: 632e 7065 7079 2e74 6563 682f 7065 7273  c.pepy.tech/pers
+000001f0: 6f6e 616c 697a 6564 2d62 6164 6765 2f70  onalized-badge/p
+00000200: 6164 646c 656f 6372 5f63 6f6e 7665 7274  addleocr_convert
+00000210: 3f70 6572 696f 643d 746f 7461 6c26 756e  ?period=total&un
+00000220: 6974 733d 6162 6272 6576 6961 7469 6f6e  its=abbreviation
+00000230: 266c 6566 745f 636f 6c6f 723d 6772 6579  &left_color=grey
+00000240: 2672 6967 6874 5f63 6f6c 6f72 3d62 6c75  &right_color=blu
+00000250: 6526 6c65 6674 5f74 6578 743d 446f 776e  e&left_text=Down
+00000260: 6c6f 6164 7322 3e3c 2f61 3e0a 3c2f 703e  loads"></a>.</p>
+00000270: 0a0a e8af a5e6 a8a1 e59d 97e6 98af 7061  ..............pa
+00000280: 6464 6c65 6f63 725f 636f 6e76 6572 74e8  ddleocr_convert.
+00000290: bdac e68d a2e6 a8a1 e59e 8be7 9a84 e6a0  ................
+000002a0: b8e5 bf83 e4bb a3e7 a081 e380 82e4 b8bb  ................
+000002b0: e8a6 81e5 8c85 e68b ace4 b88b e8bd bde6  ................
+000002c0: a8a1 e59e 8be3 8081 e8a7 a3e5 8e8b e6a8  ................
+000002d0: a1e5 9e8b e380 81e8 bdac e68d a2e6 a8a1  ................
+000002e0: e59e 8be5 928c e69b b4e6 94b9 e6a8 a1e5  ................
+000002f0: 9e8b e4b8 bae5 8aa8 e680 81e8 be93 e585  ................
+00000300: a5e5 9b9b e983 a8e5 8886 e380 820a e794  ................
+00000310: b1e4 ba8e e79b aee5 898d 6070 6164 646c  ..........`paddl
+00000320: 6532 6f6e 6e78 60e8 bdac e68d a2e5 b7a5  e2onnx`.........
+00000330: e585 b7e8 be83 e4b8 bae6 8890 e786 9fef  ................
+00000340: bc8c e58f afe4 bba5 e5b0 b1e6 b2a1 e69c  ................
+00000350: 89e6 b7bb e58a a0e8 bdac e68d a2e5 898d  ................
+00000360: e590 8ee6 a8a1 e59e 8be7 b2be e5ba a6e9  ................
+00000370: aa8c e8af 81e6 98af e590 a6e6 bba1 e8b6  ................
+00000380: b3e8 a681 e6b1 82e7 9a84 e693 8de4 bd9c  ................
+00000390: e380 820a 0ae6 94af e68c 81e6 a8a1 e59e  ................
+000003a0: 8be7 9a84 7572 6ce5 928c e69c ace5 9cb0  ....url.........
+000003b0: e8b7 afe5 be84 e4b8 a4e7 a78d e8be 93e5  ................
+000003c0: 85a5 e696 b9e5 bc8f e380 82e5 85b6 e4b8  ................
+000003d0: ade9 9288 e5af b960 7265 6360 e79a 84e6  .......`rec`....
+000003e0: a8a1 e59e 8bef bc8c e99c 80e8 a681 e68f  ................
+000003f0: 90e4 be9b e5af b9e5 ba94 e79a 84e5 ad97  ................
+00000400: e585 b8e6 9687 e4bb b6ef bc8c e8af a5e5  ................
+00000410: ba93 e4bc 9ae8 87aa e58a a8e5 b086 e5ad  ................
+00000420: 97e5 85b8 e696 87e4 bbb6 e586 99e5 85a5  ................
+00000430: e588 b06f 6e6e 78e4 b8ad e380 820a e8bf  ...onnx.........
+00000440: 99e9 878c e99c 80e8 a681 e690 ade9 858d  ................
+00000450: 5b52 6170 6964 4f43 525d 2868 7474 7073  [RapidOCR](https
+00000460: 3a2f 2f67 6974 6875 622e 636f 6d2f 5261  ://github.com/Ra
+00000470: 7069 6441 492f 5261 7069 644f 4352 29e6  pidAI/RapidOCR).
+00000480: 8ea8 e790 86e4 bba3 e7a0 81e4 bdbf e794  ................
+00000490: a80a 0a22 2222 0a0a 6672 6f6d 202e 6d61  ..."""..from .ma
+000004a0: 696e 2069 6d70 6f72 7420 5061 6464 6c65  in import Paddle
+000004b0: 4f43 524d 6f64 656c 436f 6e76 6572 740a  OCRModelConvert.
+000004c0: 6672 6f6d 202e 7574 696c 7320 696d 706f  from .utils impo
+000004d0: 7274 2064 6f77 6e6c 6f61 645f 6669 6c65  rt download_file
+000004e0: 0a                                       .
```

## Comparing `paddleocr_convert-0.0.8.dist-info/LICENSE` & `paddleocr_convert-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `paddleocr_convert-0.0.8.dist-info/METADATA` & `paddleocr_convert-0.0.9.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddleocr-convert
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tool for converting the PaddleOCR model to onnx format.
 Home-page: https://github.com/RapidAI/PaddleOCRModelConverter
 Download-URL: https://github.com/RapidAI/PaddleOCRModelConverter.git
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: ocr,text_detection,text_recognition,db,onnxruntime,paddleocr,openvino,rapidocr
@@ -23,14 +23,15 @@
 
 ## paddleocr_convert
 <p>
     <a href=""><img src="https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg"></a>
     <a href="https://pypi.org/project/paddleocr_convert/"><img alt="PyPI" src="https://img.shields.io/pypi/v/paddleocr_convert"></a>
     <a href="https://pepy.tech/project/paddleocr_convert"><img src="https://static.pepy.tech/personalized-badge/paddleocr_convert?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads"></a>
+    <a href="http://rapidai-team.com/PaddleOCRModelConverter/paddleocr_convert.html"><img height="20" alt="paddleocr_convert documentation" src="https://shields.mitmproxy.org/badge/API Docs-paddocr_convert-brightgreen.svg"></a>
 </p>
 
 ### 1. Install package by pypi.
 ```bash
 pip install paddleocr_convert
 ```
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: paddleocr-convert Version: 0.0.8 Summary: Tool for
+Metadata-Version: 2.1 Name: paddleocr-convert Version: 0.0.9 Summary: Tool for
 converting the PaddleOCR model to onnx format. Home-page: https://github.com/
 RapidAI/PaddleOCRModelConverter Download-URL: https://github.com/RapidAI/
 PaddleOCRModelConverter.git Author: SWHL Author-email: liekkaskono@163.com
 License: Apache-2.0 Keywords:
 ocr,text_detection,text_recognition,db,onnxruntime,paddleocr,openvino,rapidocr
 Platform: Any Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
@@ -11,14 +11,15 @@
 License-File: LICENSE Requires-Dist: paddle2onnx (>=1.0.0) Requires-Dist:
 requests (>=2.27.1) Requires-Dist: tqdm (>=4.64.1) Requires-Dist: onnx
 (>=1.12.0) ## paddleocr_convert
 [https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
 img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg] [PyPI] [https://
 static.pepy.tech/personalized-badge/
 paddleocr_convert?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads]
+[paddleocr_convert_documentation]
 ### 1. Install package by pypi. ```bash pip install paddleocr_convert ``` ###
 2. Run by command line. - Usage: ```bash $ paddleocr_convert -h usage:
 paddleocr_convert [-h] [-p MODEL_PATH] [-o SAVE_DIR] [-txt_path TXT_PATH]
 optional arguments: -h, --help show this help message and exit -p MODEL_PATH, -
 -model_path MODEL_PATH The inference model url or local path of paddleocr. e.g.
 https://paddleocr.bj.bcebos.com/PP- OCRv3/chinese/ch_PP-OCRv3_det_infer.tar or
 models/ch_PP-OCRv3_det_infer.tar -o SAVE_DIR, --save_dir SAVE_DIR The directory
```

