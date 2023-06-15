# Comparing `tmp/filedata-ext-0.2.tar.gz` & `tmp/filedata-ext-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filedata-ext-0.2.tar", last modified: Thu Jun 15 00:27:12 2023, max compression
+gzip compressed data, was "filedata-ext-0.2.1.tar", last modified: Thu Jun 15 10:27:58 2023, max compression
```

## Comparing `filedata-ext-0.2.tar` & `filedata-ext-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 00:27:12.191193 filedata-ext-0.2/
--rwxrwxrwx   0 root         (0) root         (0)      111 2023-06-13 00:03:29.000000 filedata-ext-0.2/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)      556 2023-06-15 00:27:12.191193 filedata-ext-0.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       65 2023-06-13 00:03:29.000000 filedata-ext-0.2/README.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 00:27:11.503532 filedata-ext-0.2/filedata_ext/
--rwxrwxrwx   0 root         (0) root         (0)       20 2023-06-15 00:25:09.000000 filedata-ext-0.2/filedata_ext/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       83 2023-06-14 00:46:36.000000 filedata-ext-0.2/filedata_ext/constants.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 00:27:11.800405 filedata-ext-0.2/filedata_ext/data_models/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.2/filedata_ext/data_models/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      378 2023-06-14 05:25:29.000000 filedata-ext-0.2/filedata_ext/data_models/file_info.py
--rwxrwxrwx   0 root         (0) root         (0)      368 2023-06-13 09:47:04.000000 filedata-ext-0.2/filedata_ext/data_models/ocr.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 00:27:11.925412 filedata-ext-0.2/filedata_ext/services/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.2/filedata_ext/services/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8500 2023-06-14 05:26:37.000000 filedata-ext-0.2/filedata_ext/services/file_handler.py
--rwxrwxrwx   0 root         (0) root         (0)     5666 2023-06-15 00:21:33.000000 filedata-ext-0.2/filedata_ext/services/filedata_cache.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 00:27:11.972281 filedata-ext-0.2/filedata_ext/utils/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.2/filedata_ext/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      450 2023-06-13 00:03:29.000000 filedata-ext-0.2/filedata_ext/utils/video.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 00:27:11.675417 filedata-ext-0.2/filedata_ext.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      556 2023-06-15 00:27:10.000000 filedata-ext-0.2/filedata_ext.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      726 2023-06-15 00:27:11.000000 filedata-ext-0.2/filedata_ext.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-15 00:27:10.000000 filedata-ext-0.2/filedata_ext.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-14 08:37:07.000000 filedata-ext-0.2/filedata_ext.egg-info/not-zip-safe
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-06-15 00:27:11.000000 filedata-ext-0.2/filedata_ext.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2023-06-15 00:27:11.000000 filedata-ext-0.2/filedata_ext.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 00:27:12.003537 filedata-ext-0.2/requirements/
--rwxrwxrwx   0 root         (0) root         (0)       18 2023-06-13 00:03:29.000000 filedata-ext-0.2/requirements/test.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-15 00:27:12.191193 filedata-ext-0.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1453 2023-06-13 00:03:29.000000 filedata-ext-0.2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 00:27:12.050412 filedata-ext-0.2/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.2/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1748 2023-06-14 05:29:55.000000 filedata-ext-0.2/tests/file_handler_test.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 00:27:12.144314 filedata-ext-0.2/tests/resources/
--rwxrwxrwx   0 root         (0) root         (0)    18180 2023-06-14 00:39:13.000000 filedata-ext-0.2/tests/resources/example.docx
--rwxrwxrwx   0 root         (0) root         (0)   130941 2023-06-14 00:42:50.000000 filedata-ext-0.2/tests/resources/example.pdf
--rwxrwxrwx   0 root         (0) root         (0)   231039 2023-06-14 00:27:17.000000 filedata-ext-0.2/tests/resources/example.png
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 10:27:58.450572 filedata-ext-0.2.1/
+-rwxrwxrwx   0 root         (0) root         (0)      111 2023-06-13 00:03:29.000000 filedata-ext-0.2.1/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)      558 2023-06-15 10:27:58.450572 filedata-ext-0.2.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       65 2023-06-13 00:03:29.000000 filedata-ext-0.2.1/README.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 10:27:57.807084 filedata-ext-0.2.1/filedata_ext/
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-06-15 10:27:12.000000 filedata-ext-0.2.1/filedata_ext/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       83 2023-06-14 00:46:36.000000 filedata-ext-0.2.1/filedata_ext/constants.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 10:27:58.090324 filedata-ext-0.2.1/filedata_ext/data_models/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.2.1/filedata_ext/data_models/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      378 2023-06-14 05:25:29.000000 filedata-ext-0.2.1/filedata_ext/data_models/file_info.py
+-rwxrwxrwx   0 root         (0) root         (0)      368 2023-06-13 09:47:04.000000 filedata-ext-0.2.1/filedata_ext/data_models/ocr.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 10:27:58.200069 filedata-ext-0.2.1/filedata_ext/services/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.2.1/filedata_ext/services/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8500 2023-06-14 05:26:37.000000 filedata-ext-0.2.1/filedata_ext/services/file_handler.py
+-rwxrwxrwx   0 root         (0) root         (0)     5911 2023-06-15 10:26:31.000000 filedata-ext-0.2.1/filedata_ext/services/filedata_cache.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 10:27:58.246944 filedata-ext-0.2.1/filedata_ext/utils/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.2.1/filedata_ext/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      450 2023-06-13 00:03:29.000000 filedata-ext-0.2.1/filedata_ext/utils/video.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 10:27:57.933092 filedata-ext-0.2.1/filedata_ext.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      558 2023-06-15 10:27:57.000000 filedata-ext-0.2.1/filedata_ext.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      726 2023-06-15 10:27:57.000000 filedata-ext-0.2.1/filedata_ext.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-15 10:27:57.000000 filedata-ext-0.2.1/filedata_ext.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-14 08:37:07.000000 filedata-ext-0.2.1/filedata_ext.egg-info/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-06-15 10:27:57.000000 filedata-ext-0.2.1/filedata_ext.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2023-06-15 10:27:57.000000 filedata-ext-0.2.1/filedata_ext.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 10:27:58.278202 filedata-ext-0.2.1/requirements/
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-06-13 00:03:29.000000 filedata-ext-0.2.1/requirements/test.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-15 10:27:58.450572 filedata-ext-0.2.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1453 2023-06-13 00:03:29.000000 filedata-ext-0.2.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 10:27:58.325562 filedata-ext-0.2.1/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.2.1/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1748 2023-06-14 05:29:55.000000 filedata-ext-0.2.1/tests/file_handler_test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 10:27:58.419324 filedata-ext-0.2.1/tests/resources/
+-rwxrwxrwx   0 root         (0) root         (0)    18180 2023-06-14 00:39:13.000000 filedata-ext-0.2.1/tests/resources/example.docx
+-rwxrwxrwx   0 root         (0) root         (0)   130941 2023-06-14 00:42:50.000000 filedata-ext-0.2.1/tests/resources/example.pdf
+-rwxrwxrwx   0 root         (0) root         (0)   231039 2023-06-14 00:27:17.000000 filedata-ext-0.2.1/tests/resources/example.png
```

### Comparing `filedata-ext-0.2/PKG-INFO` & `filedata-ext-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filedata-ext
-Version: 0.2
+Version: 0.2.1
 Summary: Extensions of filedata for guniflask
 Home-page: UNKNOWN
 Author: jadbin
 Author-email: jadbin.com@hotmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `filedata-ext-0.2/filedata_ext/services/file_handler.py` & `filedata-ext-0.2.1/filedata_ext/services/file_handler.py`

 * *Files identical despite different names*

### Comparing `filedata-ext-0.2/filedata_ext/services/filedata_cache.py` & `filedata-ext-0.2.1/filedata_ext/services/filedata_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,14 +172,24 @@
             json=cache.dict(),
             params={
                 'key': key,
             },
             timeout=20,
         )
 
+    def remove_cache(self, key: str, md5: str):
+        self.session.delete(
+            f'{self.endpoint}api/cache',
+            params={
+                'md5': md5,
+                'key': key,
+            },
+            timeout=20,
+        )
+
     def get_typed_cache(self, key: str, md5: str, cls: Type[T]) -> Optional[T]:
         cache = self.get_cache(key=key, md5=md5)
         if cache is None:
             return
         return cls(**cache.data)
 
     def save_typed_cache(self, key: str, md5: str, data: Any):
```

### Comparing `filedata-ext-0.2/filedata_ext.egg-info/PKG-INFO` & `filedata-ext-0.2.1/filedata_ext.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filedata-ext
-Version: 0.2
+Version: 0.2.1
 Summary: Extensions of filedata for guniflask
 Home-page: UNKNOWN
 Author: jadbin
 Author-email: jadbin.com@hotmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `filedata-ext-0.2/filedata_ext.egg-info/SOURCES.txt` & `filedata-ext-0.2.1/filedata_ext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `filedata-ext-0.2/setup.py` & `filedata-ext-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `filedata-ext-0.2/tests/file_handler_test.py` & `filedata-ext-0.2.1/tests/file_handler_test.py`

 * *Files identical despite different names*

### Comparing `filedata-ext-0.2/tests/resources/example.docx` & `filedata-ext-0.2.1/tests/resources/example.docx`

 * *Files identical despite different names*

### Comparing `filedata-ext-0.2/tests/resources/example.pdf` & `filedata-ext-0.2.1/tests/resources/example.pdf`

 * *Files identical despite different names*

### Comparing `filedata-ext-0.2/tests/resources/example.png` & `filedata-ext-0.2.1/tests/resources/example.png`

 * *Files identical despite different names*

