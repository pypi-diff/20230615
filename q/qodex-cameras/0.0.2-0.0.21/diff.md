# Comparing `tmp/qodex_cameras-0.0.2-py3-none-any.whl.zip` & `tmp/qodex_cameras-0.0.21-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 38229 bytes, number of entries: 17
+Zip file size: 38256 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-27 06:46 qodex_cameras/__init__.py
 -rw-rw-rw-  2.0 fat      166 b- defN 23-May-02 11:08 qodex_cameras/functions.py
 -rw-rw-rw-  2.0 fat     1820 b- defN 23-May-12 09:26 qodex_cameras/main.py
--rw-rw-rw-  2.0 fat     2496 b- defN 23-May-12 09:26 qodex_cameras/mixins.py
+-rw-rw-rw-  2.0 fat     2578 b- defN 23-Jun-15 06:19 qodex_cameras/mixins.py
 -rw-rw-rw-  2.0 fat      384 b- defN 23-May-12 08:58 qodex_cameras/settings.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-02 04:44 qodex_cameras/other/__init__.py
 -rw-rw-rw-  2.0 fat     6078 b- defN 23-May-02 04:46 qodex_cameras/other/pyhik_mode.py
 -rw-rw-rw-  2.0 fat     7365 b- defN 23-May-12 06:25 qodex_cameras/photos/Test.png
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-12 05:38 qodex_cameras/photos/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-02 12:07 qodex_cameras/tests/__init__.py
 -rw-rw-rw-  2.0 fat     1198 b- defN 23-May-12 09:01 qodex_cameras/tests/main_tests.py
 -rw-rw-rw-  2.0 fat    26529 b- defN 23-May-12 08:58 qodex_cameras/tests/test.png
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-12 09:26 qodex_cameras-0.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      306 b- defN 23-May-12 09:26 qodex_cameras-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-12 09:26 qodex_cameras-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-May-12 09:26 qodex_cameras-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1423 b- defN 23-May-12 09:26 qodex_cameras-0.0.2.dist-info/RECORD
-17 files, 48962 bytes uncompressed, 35863 bytes compressed:  26.8%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-15 06:19 qodex_cameras-0.0.21.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      307 b- defN 23-Jun-15 06:19 qodex_cameras-0.0.21.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-15 06:19 qodex_cameras-0.0.21.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-15 06:19 qodex_cameras-0.0.21.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1428 b- defN 23-Jun-15 06:19 qodex_cameras-0.0.21.dist-info/RECORD
+17 files, 49050 bytes uncompressed, 35880 bytes compressed:  26.9%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: qodex_cameras/tests/main_tests.py
 Comment: 
 
 Filename: qodex_cameras/tests/test.png
 Comment: 
 
-Filename: qodex_cameras-0.0.2.dist-info/LICENSE
+Filename: qodex_cameras-0.0.21.dist-info/LICENSE
 Comment: 
 
-Filename: qodex_cameras-0.0.2.dist-info/METADATA
+Filename: qodex_cameras-0.0.21.dist-info/METADATA
 Comment: 
 
-Filename: qodex_cameras-0.0.2.dist-info/WHEEL
+Filename: qodex_cameras-0.0.21.dist-info/WHEEL
 Comment: 
 
-Filename: qodex_cameras-0.0.2.dist-info/top_level.txt
+Filename: qodex_cameras-0.0.21.dist-info/top_level.txt
 Comment: 
 
-Filename: qodex_cameras-0.0.2.dist-info/RECORD
+Filename: qodex_cameras-0.0.21.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qodex_cameras/mixins.py

```diff
@@ -57,27 +57,28 @@
         try:
             return self.get_photo_rest()
         except ConnectionError:
             logging.error(
                 f"Connection error: {traceback.format_exc()}")
 
 
-
 class HttpMakePic:
     auth_method = None
     cam_login = None
     cam_pass = None
     get_photo_url = None
+    get_pic_timeout = 5
 
     def get_http_photo(self):
-        print(self.get_photo_url)
         if self.auth_method == "Basic":
             response = requests.get(
                 self.get_photo_url,
-                auth=HTTPBasicAuth(self.cam_login, self.cam_pass))
+                auth=HTTPBasicAuth(self.cam_login, self.cam_pass),
+                timeout=self.get_pic_timeout)
         elif self.auth_method == "Digest":
             response = requests.get(
                 self.get_photo_url,
-                auth=HTTPDigestAuth(self.cam_login, self.cam_pass))
+                auth=HTTPDigestAuth(self.cam_login, self.cam_pass),
+                timeout=self.get_pic_timeout)
         else:
             return
         return response.content
```

## Comparing `qodex_cameras-0.0.2.dist-info/LICENSE` & `qodex_cameras-0.0.21.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qodex_cameras-0.0.2.dist-info/RECORD` & `qodex_cameras-0.0.21.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 qodex_cameras/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qodex_cameras/functions.py,sha256=elNHnnx3zelcKnAOLK3E6ETMpV3PZPXfWclPRYSqiZA,166
 qodex_cameras/main.py,sha256=o7lAuj2a2cvgov7hkjgwXpd8ZX2BWuVJFghWWqi6RTo,1820
-qodex_cameras/mixins.py,sha256=21icQrwqZWvhAG2OtBlhrqJXkO3awc9IS3eqDGI8tc4,2496
+qodex_cameras/mixins.py,sha256=MXgX16rlo26n5mJmgHZKBo00lnWjMg8zHv-vTtdThzI,2578
 qodex_cameras/settings.py,sha256=xupNck2qOhJLj0WQjB47Z6dm179vhVF1FJ-dDcgX4c0,384
 qodex_cameras/other/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qodex_cameras/other/pyhik_mode.py,sha256=FyG_QWVdcTi5dnSwv3Iq-L0H4PYW6wKBeVJpkYRt58Q,6078
 qodex_cameras/photos/Test.png,sha256=v54Of9PyXTQ-X6_ji_105kC2ISyuxG6UxJDBzcdV4ac,7365
 qodex_cameras/photos/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qodex_cameras/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qodex_cameras/tests/main_tests.py,sha256=XcEz6hkhzaBtMuTSOotk5BAj0RZpfB840EdoVzZhMUA,1198
 qodex_cameras/tests/test.png,sha256=EZ4YZtPhTRLJBM2ZMr-ZyXqVMKgYlmW-25syShwy_8s,26529
-qodex_cameras-0.0.2.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-qodex_cameras-0.0.2.dist-info/METADATA,sha256=4wOnu4bSABF0EZib4IN6cvxRqIxahtQ8kfApf0djw3Y,306
-qodex_cameras-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-qodex_cameras-0.0.2.dist-info/top_level.txt,sha256=TUs_F_ccN29bu8q7TOb4gyqz9ZJY8Jb93IueSTAuBHA,14
-qodex_cameras-0.0.2.dist-info/RECORD,,
+qodex_cameras-0.0.21.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+qodex_cameras-0.0.21.dist-info/METADATA,sha256=MnYWfFH-OCm0H24zMTdoyb6N_vzDdGyXo41arAXi5Zo,307
+qodex_cameras-0.0.21.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+qodex_cameras-0.0.21.dist-info/top_level.txt,sha256=TUs_F_ccN29bu8q7TOb4gyqz9ZJY8Jb93IueSTAuBHA,14
+qodex_cameras-0.0.21.dist-info/RECORD,,
```

