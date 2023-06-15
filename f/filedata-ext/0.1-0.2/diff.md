# Comparing `tmp/filedata-ext-0.1.tar.gz` & `tmp/filedata-ext-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filedata-ext-0.1.tar", last modified: Wed Jun 14 08:37:08 2023, max compression
+gzip compressed data, was "filedata-ext-0.2.tar", last modified: Thu Jun 15 00:27:12 2023, max compression
```

## Comparing `filedata-ext-0.1.tar` & `filedata-ext-0.2.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 08:37:08.253218 filedata-ext-0.1/
--rwxrwxrwx   0 root         (0) root         (0)      111 2023-06-13 00:03:29.000000 filedata-ext-0.1/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)      556 2023-06-14 08:37:08.253218 filedata-ext-0.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       65 2023-06-13 00:03:29.000000 filedata-ext-0.1/README.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 08:37:07.749996 filedata-ext-0.1/filedata_ext/
--rwxrwxrwx   0 root         (0) root         (0)       20 2023-06-14 08:35:29.000000 filedata-ext-0.1/filedata_ext/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       83 2023-06-14 00:46:36.000000 filedata-ext-0.1/filedata_ext/constants.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 08:37:07.953905 filedata-ext-0.1/filedata_ext/data_models/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.1/filedata_ext/data_models/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1553 2023-06-13 00:03:29.000000 filedata-ext-0.1/filedata_ext/data_models/doc_feature.py
--rwxrwxrwx   0 root         (0) root         (0)      378 2023-06-14 05:25:29.000000 filedata-ext-0.1/filedata_ext/data_models/file_info.py
--rwxrwxrwx   0 root         (0) root         (0)      368 2023-06-13 09:47:04.000000 filedata-ext-0.1/filedata_ext/data_models/ocr.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 08:37:08.032697 filedata-ext-0.1/filedata_ext/services/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.1/filedata_ext/services/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8500 2023-06-14 05:26:37.000000 filedata-ext-0.1/filedata_ext/services/file_handler.py
--rwxrwxrwx   0 root         (0) root         (0)     5824 2023-06-14 00:47:21.000000 filedata-ext-0.1/filedata_ext/services/filedata_cache.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 08:37:08.079873 filedata-ext-0.1/filedata_ext/utils/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.1/filedata_ext/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      450 2023-06-13 00:03:29.000000 filedata-ext-0.1/filedata_ext/utils/video.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 08:37:07.859382 filedata-ext-0.1/filedata_ext.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      556 2023-06-14 08:37:07.000000 filedata-ext-0.1/filedata_ext.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      766 2023-06-14 08:37:07.000000 filedata-ext-0.1/filedata_ext.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-14 08:37:07.000000 filedata-ext-0.1/filedata_ext.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-14 08:37:07.000000 filedata-ext-0.1/filedata_ext.egg-info/not-zip-safe
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-06-14 08:37:07.000000 filedata-ext-0.1/filedata_ext.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2023-06-14 08:37:07.000000 filedata-ext-0.1/filedata_ext.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 08:37:08.096415 filedata-ext-0.1/requirements/
--rwxrwxrwx   0 root         (0) root         (0)       18 2023-06-13 00:03:29.000000 filedata-ext-0.1/requirements/test.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-14 08:37:08.253218 filedata-ext-0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1453 2023-06-13 00:03:29.000000 filedata-ext-0.1/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 08:37:08.143903 filedata-ext-0.1/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.1/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1748 2023-06-14 05:29:55.000000 filedata-ext-0.1/tests/file_handler_test.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 08:37:08.221962 filedata-ext-0.1/tests/resources/
--rwxrwxrwx   0 root         (0) root         (0)    18180 2023-06-14 00:39:13.000000 filedata-ext-0.1/tests/resources/example.docx
--rwxrwxrwx   0 root         (0) root         (0)   130941 2023-06-14 00:42:50.000000 filedata-ext-0.1/tests/resources/example.pdf
--rwxrwxrwx   0 root         (0) root         (0)   231039 2023-06-14 00:27:17.000000 filedata-ext-0.1/tests/resources/example.png
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 00:27:12.191193 filedata-ext-0.2/
+-rwxrwxrwx   0 root         (0) root         (0)      111 2023-06-13 00:03:29.000000 filedata-ext-0.2/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)      556 2023-06-15 00:27:12.191193 filedata-ext-0.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       65 2023-06-13 00:03:29.000000 filedata-ext-0.2/README.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 00:27:11.503532 filedata-ext-0.2/filedata_ext/
+-rwxrwxrwx   0 root         (0) root         (0)       20 2023-06-15 00:25:09.000000 filedata-ext-0.2/filedata_ext/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       83 2023-06-14 00:46:36.000000 filedata-ext-0.2/filedata_ext/constants.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 00:27:11.800405 filedata-ext-0.2/filedata_ext/data_models/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.2/filedata_ext/data_models/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      378 2023-06-14 05:25:29.000000 filedata-ext-0.2/filedata_ext/data_models/file_info.py
+-rwxrwxrwx   0 root         (0) root         (0)      368 2023-06-13 09:47:04.000000 filedata-ext-0.2/filedata_ext/data_models/ocr.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 00:27:11.925412 filedata-ext-0.2/filedata_ext/services/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.2/filedata_ext/services/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8500 2023-06-14 05:26:37.000000 filedata-ext-0.2/filedata_ext/services/file_handler.py
+-rwxrwxrwx   0 root         (0) root         (0)     5666 2023-06-15 00:21:33.000000 filedata-ext-0.2/filedata_ext/services/filedata_cache.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 00:27:11.972281 filedata-ext-0.2/filedata_ext/utils/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.2/filedata_ext/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      450 2023-06-13 00:03:29.000000 filedata-ext-0.2/filedata_ext/utils/video.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 00:27:11.675417 filedata-ext-0.2/filedata_ext.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      556 2023-06-15 00:27:10.000000 filedata-ext-0.2/filedata_ext.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      726 2023-06-15 00:27:11.000000 filedata-ext-0.2/filedata_ext.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-15 00:27:10.000000 filedata-ext-0.2/filedata_ext.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-14 08:37:07.000000 filedata-ext-0.2/filedata_ext.egg-info/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-06-15 00:27:11.000000 filedata-ext-0.2/filedata_ext.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2023-06-15 00:27:11.000000 filedata-ext-0.2/filedata_ext.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 00:27:12.003537 filedata-ext-0.2/requirements/
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-06-13 00:03:29.000000 filedata-ext-0.2/requirements/test.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-15 00:27:12.191193 filedata-ext-0.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1453 2023-06-13 00:03:29.000000 filedata-ext-0.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 00:27:12.050412 filedata-ext-0.2/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.2/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1748 2023-06-14 05:29:55.000000 filedata-ext-0.2/tests/file_handler_test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 00:27:12.144314 filedata-ext-0.2/tests/resources/
+-rwxrwxrwx   0 root         (0) root         (0)    18180 2023-06-14 00:39:13.000000 filedata-ext-0.2/tests/resources/example.docx
+-rwxrwxrwx   0 root         (0) root         (0)   130941 2023-06-14 00:42:50.000000 filedata-ext-0.2/tests/resources/example.pdf
+-rwxrwxrwx   0 root         (0) root         (0)   231039 2023-06-14 00:27:17.000000 filedata-ext-0.2/tests/resources/example.png
```

### Comparing `filedata-ext-0.1/PKG-INFO` & `filedata-ext-0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filedata-ext
-Version: 0.1
+Version: 0.2
 Summary: Extensions of filedata for guniflask
 Home-page: UNKNOWN
 Author: jadbin
 Author-email: jadbin.com@hotmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `filedata-ext-0.1/filedata_ext/services/file_handler.py` & `filedata-ext-0.2/filedata_ext/services/file_handler.py`

 * *Files identical despite different names*

### Comparing `filedata-ext-0.1/filedata_ext/services/filedata_cache.py` & `filedata-ext-0.2/filedata_ext/services/filedata_cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import io
-from typing import List, Optional, Any
+from typing import List, Optional, Any, Type, TypeVar
 
 import gevent
 import requests
 from PIL import Image
 from filedata.image import ocr_with_angle_correction, OCRResult
 from filedata.pdf import pdf_to_image
 from filedata.retry import retry_api
 from guniflask.config import settings
 from kikyo import Kikyo, OSS
 from kikyo.bundle.search import EsBasedSearch
 from pydantic import BaseModel
 
 from filedata_ext.constants import FILEDATA_CACHE_ENDPOINT, THUMBNAIL_NUM
-from filedata_ext.data_models.doc_feature import DocFeature
 from filedata_ext.data_models.file_info import FileInfo
 from filedata_ext.data_models.ocr import OCRCache, OCRMeta
 
 
 class Cache(BaseModel):
     filename: str = None
     md5: str
     file_link: str = None
     data: Any
 
 
 class CacheKey:
     OCR = 'ocr'
-    FEATURES = 'features'
-    HIT_INFO = 'hit_info'
     FILE_INFO = 'file_info'
 
 
+T = TypeVar('T')
+
+
 class FiledataCacheService:
     def __init__(self, kikyo_client: Kikyo):
         self.kikyo_search = kikyo_client.component(cls=EsBasedSearch)
         self.files_bucket = kikyo_client.component(cls=OSS).bucket('files')
 
         self.session = requests.Session()
         try:
@@ -138,24 +138,14 @@
         if cache is None:
             return
         return OCRCache(**cache.data)
 
     def save_ocr_cache(self, ocr_cache: OCRCache):
         self.save_cache(key=CacheKey.OCR, cache=Cache(md5=ocr_cache.md5, data=ocr_cache))
 
-    def get_features_cache(self, md5: str) -> Optional[List[DocFeature]]:
-        cache = self.get_cache(key=CacheKey.FEATURES, md5=md5)
-        if cache is None:
-            return
-        result = [DocFeature(**i) for i in cache.data]
-        return result
-
-    def save_features_cache(self, md5: str, features: List[DocFeature]):
-        self.save_cache(key=CacheKey.FEATURES, cache=Cache(md5=md5, data=features))
-
     def get_file_info_cache(self, md5: str) -> Optional[FileInfo]:
         cache = self.get_cache(key=CacheKey.FILE_INFO, md5=md5)
         if cache is None:
             return
         return FileInfo(**cache.data)
 
     def save_file_info_cache(self, md5: str, file_info_cache: FileInfo):
@@ -181,7 +171,16 @@
             f'{self.endpoint}api/cache',
             json=cache.dict(),
             params={
                 'key': key,
             },
             timeout=20,
         )
+
+    def get_typed_cache(self, key: str, md5: str, cls: Type[T]) -> Optional[T]:
+        cache = self.get_cache(key=key, md5=md5)
+        if cache is None:
+            return
+        return cls(**cache.data)
+
+    def save_typed_cache(self, key: str, md5: str, data: Any):
+        self.save_cache(key=key, cache=Cache(md5=md5, data=data))
```

### Comparing `filedata-ext-0.1/filedata_ext.egg-info/PKG-INFO` & `filedata-ext-0.2/filedata_ext.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filedata-ext
-Version: 0.1
+Version: 0.2
 Summary: Extensions of filedata for guniflask
 Home-page: UNKNOWN
 Author: jadbin
 Author-email: jadbin.com@hotmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `filedata-ext-0.1/filedata_ext.egg-info/SOURCES.txt` & `filedata-ext-0.2/filedata_ext.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 filedata_ext.egg-info/PKG-INFO
 filedata_ext.egg-info/SOURCES.txt
 filedata_ext.egg-info/dependency_links.txt
 filedata_ext.egg-info/not-zip-safe
 filedata_ext.egg-info/requires.txt
 filedata_ext.egg-info/top_level.txt
 filedata_ext/data_models/__init__.py
-filedata_ext/data_models/doc_feature.py
 filedata_ext/data_models/file_info.py
 filedata_ext/data_models/ocr.py
 filedata_ext/services/__init__.py
 filedata_ext/services/file_handler.py
 filedata_ext/services/filedata_cache.py
 filedata_ext/utils/__init__.py
 filedata_ext/utils/video.py
```

### Comparing `filedata-ext-0.1/setup.py` & `filedata-ext-0.2/setup.py`

 * *Files identical despite different names*

### Comparing `filedata-ext-0.1/tests/file_handler_test.py` & `filedata-ext-0.2/tests/file_handler_test.py`

 * *Files identical despite different names*

### Comparing `filedata-ext-0.1/tests/resources/example.docx` & `filedata-ext-0.2/tests/resources/example.docx`

 * *Files identical despite different names*

### Comparing `filedata-ext-0.1/tests/resources/example.pdf` & `filedata-ext-0.2/tests/resources/example.pdf`

 * *Files identical despite different names*

### Comparing `filedata-ext-0.1/tests/resources/example.png` & `filedata-ext-0.2/tests/resources/example.png`

 * *Files identical despite different names*

