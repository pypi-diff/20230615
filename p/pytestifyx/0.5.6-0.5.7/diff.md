# Comparing `tmp/pytestifyx-0.5.6-py2.py3-none-any.whl.zip` & `tmp/pytestifyx-0.5.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 50905 bytes, number of entries: 58
--rw-r--r--  2.0 unx      208 b- defN 23-Jun-12 13:54 pytestifyx/__init__.py
+Zip file size: 50930 bytes, number of entries: 58
+-rw-r--r--  2.0 unx      208 b- defN 23-Jun-15 14:38 pytestifyx/__init__.py
 -rw-r--r--  2.0 unx      302 b- defN 23-May-10 13:55 pytestifyx/chinese_fix.py
 -rw-r--r--  2.0 unx     1131 b- defN 23-May-29 13:01 pytestifyx/cli.py
 -rw-r--r--  2.0 unx     1611 b- defN 23-May-22 23:17 pytestifyx/config.py
 -rw-r--r--  2.0 unx      895 b- defN 23-May-22 23:17 pytestifyx/core.py
 -rw-r--r--  2.0 unx    16511 b- defN 23-Jun-12 13:50 pytestifyx/parse.py
 -rw-r--r--  2.0 unx     2085 b- defN 23-Apr-02 11:05 pytestifyx/scaffold.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-12 12:47 pytestifyx/driver/__init__.py
--rw-r--r--  2.0 unx    10813 b- defN 23-Jun-12 13:53 pytestifyx/driver/api.py
+-rw-r--r--  2.0 unx    10870 b- defN 23-Jun-15 14:38 pytestifyx/driver/api.py
 -rw-r--r--  2.0 unx     4770 b- defN 23-May-25 12:51 pytestifyx/driver/web.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-16 14:56 pytestifyx/utils/__init__.py
 -rw-r--r--  2.0 unx       75 b- defN 23-Apr-02 08:51 pytestifyx/utils/data_factory/__init__.py
 -rw-r--r--  2.0 unx      497 b- defN 23-Apr-02 08:50 pytestifyx/utils/data_factory/run.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 08:48 pytestifyx/utils/data_factory/core/__init__.py
 -rw-r--r--  2.0 unx      256 b- defN 23-Apr-02 08:52 pytestifyx/utils/data_factory/core/config.py
 -rw-r--r--  2.0 unx      949 b- defN 23-Apr-02 08:48 pytestifyx/utils/data_factory/core/factory.py
@@ -47,14 +47,14 @@
 -rw-r--r--  2.0 unx      712 b- defN 23-May-22 23:18 pytestifyx/utils/public/get_project_path.py
 -rw-r--r--  2.0 unx      300 b- defN 23-Feb-23 12:06 pytestifyx/utils/public/img_to_base64.py
 -rw-r--r--  2.0 unx      372 b- defN 23-May-10 13:35 pytestifyx/utils/public/printify_table.py
 -rw-r--r--  2.0 unx      712 b- defN 23-Jun-07 16:25 pytestifyx/utils/public/trans_param_style.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-19 04:37 pytestifyx/utils/requests/__init__.py
 -rw-r--r--  2.0 unx      464 b- defN 22-Nov-21 14:29 pytestifyx/utils/requests/reload_all.py
 -rw-r--r--  2.0 unx     2485 b- defN 23-May-22 23:17 pytestifyx/utils/requests/requests_config.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-12 13:54 pytestifyx-0.5.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     1124 b- defN 23-Jun-12 13:54 pytestifyx-0.5.6.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-12 13:54 pytestifyx-0.5.6.dist-info/WHEEL
--rw-r--r--  2.0 unx      132 b- defN 23-Jun-12 13:54 pytestifyx-0.5.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-12 13:54 pytestifyx-0.5.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5364 b- defN 23-Jun-12 13:54 pytestifyx-0.5.6.dist-info/RECORD
-58 files, 141688 bytes uncompressed, 42133 bytes compressed:  70.3%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-15 14:39 pytestifyx-0.5.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1124 b- defN 23-Jun-15 14:39 pytestifyx-0.5.7.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-15 14:39 pytestifyx-0.5.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx      132 b- defN 23-Jun-15 14:39 pytestifyx-0.5.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-15 14:39 pytestifyx-0.5.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5364 b- defN 23-Jun-15 14:39 pytestifyx-0.5.7.dist-info/RECORD
+58 files, 141745 bytes uncompressed, 42158 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -150,26 +150,26 @@
 
 Filename: pytestifyx/utils/requests/reload_all.py
 Comment: 
 
 Filename: pytestifyx/utils/requests/requests_config.py
 Comment: 
 
-Filename: pytestifyx-0.5.6.dist-info/LICENSE
+Filename: pytestifyx-0.5.7.dist-info/LICENSE
 Comment: 
 
-Filename: pytestifyx-0.5.6.dist-info/METADATA
+Filename: pytestifyx-0.5.7.dist-info/METADATA
 Comment: 
 
-Filename: pytestifyx-0.5.6.dist-info/WHEEL
+Filename: pytestifyx-0.5.7.dist-info/WHEEL
 Comment: 
 
-Filename: pytestifyx-0.5.6.dist-info/entry_points.txt
+Filename: pytestifyx-0.5.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: pytestifyx-0.5.6.dist-info/top_level.txt
+Filename: pytestifyx-0.5.7.dist-info/top_level.txt
 Comment: 
 
-Filename: pytestifyx-0.5.6.dist-info/RECORD
+Filename: pytestifyx-0.5.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytestifyx/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .core import TestCase
 from .utils.logs.core import log
 
 __author__ = "luyh"
 
-__version__ = "0.5.6"
+__version__ = "0.5.7"
 
 __description__ = "pytestifyx is a pytest-based automation testing framework for api, ui, app testing"
```

## pytestifyx/driver/api.py

```diff
@@ -1,7 +1,8 @@
+import copy
 import importlib
 import json
 
 from requests_toolbelt import MultipartEncoder
 import requests
 from typing import Dict
 
@@ -97,15 +98,15 @@
     def base_init_prepare_request(self, config, templates: dict, func_name: str):
         url_prefix_ = get_template_value(templates['url'], 'url_prefix' + f'_{config.env_name}')
         path = get_template_value(templates['url'], config.request_method.upper() + '_' + func_name)
         url = url_prefix_ + path
         headers = get_template_value(templates['headers'], func_name + '_headers')
         data = get_template_value(templates['body'], config.request_method.upper() + '_' + func_name)
         query_params = get_template_value(templates['body'], config.request_method.upper() + '_' + func_name + '_query_params')
-        return url, headers, data, query_params, templates
+        return url, copy.deepcopy(headers), copy.deepcopy(data), copy.deepcopy(query_params), templates
 
     @staticmethod
     def import_template(path: str, module_name: str):
         import_module_body = path.replace('\\', '.').replace('/', '.') + module_name
         template_body = importlib.import_module(import_module_body, 'api_test')
         return template_body
```

## Comparing `pytestifyx-0.5.6.dist-info/LICENSE` & `pytestifyx-0.5.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pytestifyx-0.5.6.dist-info/METADATA` & `pytestifyx-0.5.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytestifyx
-Version: 0.5.6
+Version: 0.5.7
 Summary: pytestifyx is a pytest-based automation testing framework for api, ui, app testing
 Home-page: https://github.com/jaylu2018/PyTestifyx
 Author: luyh
 Author-email: jaylu1995@outlook.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `pytestifyx-0.5.6.dist-info/RECORD` & `pytestifyx-0.5.7.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-pytestifyx/__init__.py,sha256=xLAgWvCuVm1jMUnQ4JfAkJptramtUz4VKs_fXl1kYVM,208
+pytestifyx/__init__.py,sha256=U8VaDLzOeLuOJ3EaZ4JUC_fRrt0E-tLo39-ASueR06E,208
 pytestifyx/chinese_fix.py,sha256=qFkCAFR4EspSMgeBwuiAZ9zl51SEESgp4wKqEFqzGe8,302
 pytestifyx/cli.py,sha256=0nHxXP3NGN7Sdzw3l8p2hGBRIqehO3LWMDCHgSVCD-o,1131
 pytestifyx/config.py,sha256=M9ViILKvF2T4dDjofHDPlCrYlZOlkQ0tExFaNsSN-e0,1611
 pytestifyx/core.py,sha256=XHbqbn2dtB6v40-k4guU449wXhF3W3aCkYa6Wm1hsOA,895
 pytestifyx/parse.py,sha256=M6cmJkmVjrVrilb5klm5xAkveoKxi1wozOasPOZ5Apg,16511
 pytestifyx/scaffold.py,sha256=c-zhigz3Zqo2zwt3r9H6Wu-6MQPR27-Q4qU6M3-cQGc,2085
 pytestifyx/driver/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pytestifyx/driver/api.py,sha256=gTa_yvO1AkjUuuKNPbZY8ZOI4BAWpDHtoEKxKFt8wXQ,10813
+pytestifyx/driver/api.py,sha256=mgkAXFYhJOMHD6all3tONH3MvBh9xJqpG9D8F3ihNLs,10870
 pytestifyx/driver/web.py,sha256=cVX0WeZ-plJc96Otwl--p9680CwphPihhN-JxXCJzus,4770
 pytestifyx/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pytestifyx/utils/data_factory/__init__.py,sha256=8TuB8mau5EXZDTDDBxbJ58j8K4RA1GphaexLHo51u8E,75
 pytestifyx/utils/data_factory/run.py,sha256=iX7-A7e0B8Aw31Lmad59rCo2zBqogytqw0jNVPQXU3g,497
 pytestifyx/utils/data_factory/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pytestifyx/utils/data_factory/core/config.py,sha256=fX11vxyJaIa5mv7PQEog_sBHz5f7vtsrx9p_uc8YT1c,256
 pytestifyx/utils/data_factory/core/factory.py,sha256=JEpr2vSlLPyHSFMAjloABCX_swzI_hOY9hknyhiCA0M,949
@@ -46,13 +46,13 @@
 pytestifyx/utils/public/get_project_path.py,sha256=JqweA7jeZZc_bUeNOpcm0NnOGoE9WVBCdRIfDKHuq0Q,712
 pytestifyx/utils/public/img_to_base64.py,sha256=IxTLg8b_QINdixlU-HTiWQ57CT4F8Yu3VXIcms2QRHo,300
 pytestifyx/utils/public/printify_table.py,sha256=9fWgPBfsDwnnkFJKi57tHFZtdFARdYoWS-3le4I_Jpk,372
 pytestifyx/utils/public/trans_param_style.py,sha256=TgYsiCidJt_VL_QB25Vzcei7hue-9ci8exbRlXXhR_g,712
 pytestifyx/utils/requests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pytestifyx/utils/requests/reload_all.py,sha256=rB3ORnl1cYZ7vkAUitzVNOg2TV2Ao1OlvQqmZVopZ6w,464
 pytestifyx/utils/requests/requests_config.py,sha256=JDJTRBNGEfcemJtR4E0aZc89tnzCvYtX4PcSZzencKo,2485
-pytestifyx-0.5.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-pytestifyx-0.5.6.dist-info/METADATA,sha256=Y_8ug9e-0VSQLkDakineV1KKfJpTERePnjY7GdKoJRc,1124
-pytestifyx-0.5.6.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
-pytestifyx-0.5.6.dist-info/entry_points.txt,sha256=_NGX3x3KtjAIOUbVkx_ThOrqE5vJzHT3WemSc0ZHEn0,132
-pytestifyx-0.5.6.dist-info/top_level.txt,sha256=23Gy2nqjjqGWQb8BZflCf5s-b45IGeZf8rn1Xnwzey4,11
-pytestifyx-0.5.6.dist-info/RECORD,,
+pytestifyx-0.5.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pytestifyx-0.5.7.dist-info/METADATA,sha256=c0BmnpsIm1btCrbBCTWXPbRcEJ7N6EpKnwSGEHeFZbI,1124
+pytestifyx-0.5.7.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
+pytestifyx-0.5.7.dist-info/entry_points.txt,sha256=_NGX3x3KtjAIOUbVkx_ThOrqE5vJzHT3WemSc0ZHEn0,132
+pytestifyx-0.5.7.dist-info/top_level.txt,sha256=23Gy2nqjjqGWQb8BZflCf5s-b45IGeZf8rn1Xnwzey4,11
+pytestifyx-0.5.7.dist-info/RECORD,,
```

