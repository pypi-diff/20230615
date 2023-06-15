# Comparing `tmp/openi-beta-0.0.8.tar.gz` & `tmp/openi-beta-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-0.0.8.tar", last modified: Wed Jun 14 08:24:28 2023, max compression
+gzip compressed data, was "openi-beta-0.0.9.tar", last modified: Thu Jun 15 03:56:11 2023, max compression
```

## Comparing `openi-beta-0.0.8.tar` & `openi-beta-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-14 08:24:28.338122 openi-beta-0.0.8/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-14 08:24:28.337989 openi-beta-0.0.8/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-14 08:18:21.000000 openi-beta-0.0.8/README.md
--rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-14 08:24:28.338165 openi-beta-0.0.8/setup.cfg
--rw-r--r--   0 jochen10518   (501) staff       (20)      910 2023-06-14 08:23:10.000000 openi-beta-0.0.8/setup.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-14 08:24:28.335952 openi-beta-0.0.8/src/
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-14 08:24:28.336624 openi-beta-0.0.8/src/openi/
--rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-14 08:18:21.000000 openi-beta-0.0.8/src/openi/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)      290 2023-06-14 08:18:21.000000 openi-beta-0.0.8/src/openi/constants.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-14 08:24:28.337091 openi-beta-0.0.8/src/openi/dataset/
--rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-05-30 08:31:28.000000 openi-beta-0.0.8/src/openi/dataset/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     9661 2023-06-14 08:22:19.000000 openi-beta-0.0.8/src/openi/dataset/dataset.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-14 08:24:28.337792 openi-beta-0.0.8/src/openi_beta.egg-info/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-14 08:24:28.000000 openi-beta-0.0.8/src/openi_beta.egg-info/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)      311 2023-06-14 08:24:28.000000 openi-beta-0.0.8/src/openi_beta.egg-info/SOURCES.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-14 08:24:28.000000 openi-beta-0.0.8/src/openi_beta.egg-info/dependency_links.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-14 08:24:28.000000 openi-beta-0.0.8/src/openi_beta.egg-info/requires.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-14 08:24:28.000000 openi-beta-0.0.8/src/openi_beta.egg-info/top_level.txt
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-15 03:56:11.825851 openi-beta-0.0.9/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-15 03:56:11.825730 openi-beta-0.0.9/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-15 01:12:38.000000 openi-beta-0.0.9/README.md
+-rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-15 03:56:11.825898 openi-beta-0.0.9/setup.cfg
+-rw-r--r--   0 jochen10518   (501) staff       (20)      967 2023-06-15 03:56:11.000000 openi-beta-0.0.9/setup.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-15 03:56:11.823413 openi-beta-0.0.9/src/
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-15 03:56:11.824155 openi-beta-0.0.9/src/openi/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-15 01:12:38.000000 openi-beta-0.0.9/src/openi/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)      357 2023-06-15 02:29:50.000000 openi-beta-0.0.9/src/openi/constants.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-15 03:56:11.824554 openi-beta-0.0.9/src/openi/dataset/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-05-30 08:31:28.000000 openi-beta-0.0.9/src/openi/dataset/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)    10840 2023-06-15 03:54:20.000000 openi-beta-0.0.9/src/openi/dataset/dataset.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-15 03:56:11.824702 openi-beta-0.0.9/src/openi/utils/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      417 2023-06-15 03:06:17.000000 openi-beta-0.0.9/src/openi/utils/logger.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-15 03:56:11.825401 openi-beta-0.0.9/src/openi_beta.egg-info/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-15 03:56:11.000000 openi-beta-0.0.9/src/openi_beta.egg-info/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)      363 2023-06-15 03:56:11.000000 openi-beta-0.0.9/src/openi_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-15 03:56:11.000000 openi-beta-0.0.9/src/openi_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-15 03:56:11.000000 openi-beta-0.0.9/src/openi_beta.egg-info/requires.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-15 03:56:11.000000 openi-beta-0.0.9/src/openi_beta.egg-info/top_level.txt
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-15 03:56:11.825551 openi-beta-0.0.9/test/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      627 2023-06-15 01:13:48.000000 openi-beta-0.0.9/test/test_upload_multi.py
```

### Comparing `openi-beta-0.0.8/PKG-INFO` & `openi-beta-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.0.8
+Version: 0.0.9
 Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-0.0.8/README.md` & `openi-beta-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `openi-beta-0.0.8/setup.py` & `openi-beta-0.0.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+# python setup.py sdist bdist_wheel
+#
+
 from setuptools import find_packages, setup
 
-with open('README.md', 'r') as f:
+with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='openi-beta',
-    version='0.0.8',
+    version='0.0.9',
     description='A test package for openi pypi',
     package_dir={'': 'src'},
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi',
     author='chenzh05',
     author_email='chenzh.ds@outlook.com',
```

### Comparing `openi-beta-0.0.8/src/openi/dataset/dataset.py` & `openi-beta-0.0.9/src/openi/dataset/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,16 @@
 import hashlib
 from tqdm import tqdm
 from collections import OrderedDict
 from datetime import datetime
 from ..constants import *
 
 import logging
-
-LOG_FORMAT = "%(asctime)s [%(levelname)s] - %(funcName)s() %(lineno)d: %(message)s"
-DATE_FORMAT = "%Y/%m/%d %H:%M:%S"
-logging.basicConfig(filename='openi.log', level=logging.DEBUG, format=LOG_FORMAT, datefmt=DATE_FORMAT)
-
+from openi.utils.logger import setup_logging
+setup_logging()
 
 class DatasetUploadFile:
     """
     Build APIs calls for uploading a file to openi platform.
     This class will start upload process immediatelly once being initialized. 
     """
 
@@ -55,15 +52,14 @@
 
         self.size = os.path.getsize(self.filepath)
         self.upload_url = dict()
 
     """
     APIs implementation
     """
-
     def getChunks(self):
         params = {
             "access_token": self.token,
             "dataset_id": self.dataset_id,
             "md5": self.md5,
             "file_name": self.filename,
             "type": self.upload_type,
@@ -74,29 +70,32 @@
             self.uuid = x.json()["uuid"]
             self.uploaded_chunks = x.json()["chunks"]
             if x.json()["uploaded"] == '1':
                 self.uploaded = True
             else:
                 self.uploaded = False
         else:
+            logging.error(f'{x} {x.reason} {x.text} | FileObject: {self.__dict__}')
             raise ConnectionRefusedError(
                 f'❌ <{x.status_code} {x.reason}> {x.text}')
 
     def getDatasetID(self):
         params = {"access_token": self.token}
         x = requests.get('{}datasets/{}/{}/'.format(self.app_url, self.username, self.repo), params=params)
         if x.status_code == 200:
             try:
                 self.dataset_id = x.json()["data"][0]["id"]
             except:
+                logging.error(f'{x} {x.reason} {x.text} | FileObject: {self.__dict__}')
                 print(
                     f'❌ repo [{self.username}/{self.repo}]: dataset does not exist, please create dataset before uploading files.')
         else:
+            logging.error(f'{x} {x.reason} | FileObject: {self.__dict__}')
             raise ConnectionRefusedError(
-                f'❌ <{x.status_code} {x.reason}> {x.text}')
+                f'❌ <{x.status_code} {x.reason}>')
 
     def newMultipart(self):
         params = {
             "access_token": self.token,
             "dataset_id": self.dataset_id,
             "md5": self.md5,
             "file_name": self.filename,
@@ -105,14 +104,15 @@
             "size": self.size
         }
         x = requests.get('{}attachments/new_multipart'.format(self.app_url), params=params)
         if x.json()["result_code"] == "0":
             self.upload_id = x.json()["uploadID"]
             self.uuid = x.json()["uuid"]
         else:
+            logging.info(f'{x} {x.reason} {x.json()} | FileObject: {self.__dict__}')
             raise ConnectionRefusedError(
                 f'❌ <{x.status_code} {x.reason}> {x.json()["msg"]}')
 
     def getMultipartURL(self, chunk_number, chunk_size):
         params = {
             "access_token": self.token,
             "dataset_id": self.dataset_id,
@@ -123,59 +123,67 @@
             "uploadID": self.upload_id,
             "uuid": self.uuid
         }
         x = requests.get('{}attachments/get_multipart_url'.format(self.app_url), params=params)
         if x.status_code == 200:
             self.upload_url[chunk_number] = x.json()["url"]
         else:
+            logging.error(f'{x} {x.reason} {x.text} | FileObject: {self.__dict__}')
             raise ConnectionRefusedError(
                 f'❌ <{x.status_code} {x.reason}> {x.text}')
 
     def putUpload(self, chunk_number, start, chunk_size):
         headers = {"Content-Type": "text/plain"} if self.upload_type == 0 else {}
         file_chunk_data = None
         with open(self.filepath, 'rb') as f:
             f.seek(start)
             file_chunk_data = f.read(chunk_size)
         x = requests.put(self.upload_url[chunk_number], data=file_chunk_data, headers=headers)
+        logging.info(f'putUpload {x} {x.reason} - {self.username}/{self.filename}/{self.cluster} - chunk #{chunk_number}, uploading bytes {start} to {start + chunk_size}')
         if x.status_code != 200:
+            logging.error(f'{x} {x.reason} {x.text} | FileObject: {self.__dict__}')
             raise ConnectionRefusedError(
                 f'❌ <{x.status_code} {x.reason}> "upload chunk [{chunk_number}] failed."')
 
     def completeMultipart(self):
         params = {
             "access_token": self.token,
             "dataset_id": self.dataset_id,
             "file_name": self.filename,
             "type": self.upload_type,
             "size": self.size,
             "uploadID": self.upload_id,
             "uuid": self.uuid
         }
         x = requests.post('{}attachments/complete_multipart'.format(self.app_url), params=params)
+        logging.info(f'completeMultipart - {x} {x.reason} - {self.username}/{self.filename}/{self.cluster}')
         if x.status_code != 200:
+            logging.error(f'{x} {x.reason} {x.text} | FileObject: {self.__dict__}')
             raise ConnectionRefusedError(
                 f'❌ <{x.status_code} {x.reason}> {x.text}')
         if x.json()["result_code"] == "-1":
+            logging.error(f'{x} {x.reason} {x.json()} | FileObject: {self.__dict__}')
             raise ConnectionRefusedError(
                 f'❌ <{x.status_code} {x.reason}> {x.json()["msg"]}')
 
     """
     utils functions
     """
 
     def stdOut(self, message=""):
         asctime = datetime.now().strftime("%H:%M:%S")
         return (f'{asctime}|{self.filename}|{self.cluster}|{message}')
 
     def filePreprocess(self):
         if self.size == 0:
+            logging.error(f'[{self.filename}] File size is 0 | FileObject: {self.__dict__}')
             raise ValueError(
                 f'❌ [{self.filename}] File size is 0')
         if self.size > MAX_FILE_SIZE:
+            logging.error(f'[{self.filename}] File size exceeds 200GB | FileObject: {self.__dict__}')
             raise ValueError(
                 f'❌ [{self.filename}] File size exceeds 200GB')
 
         chunk_size = SMALL_FILE_CHUNK_SIZE if self.size < SMALL_FILE_SIZE else LARGE_FILE_CHUNK_SIZE
         self.total_chunk_counts = math.ceil(self.size / chunk_size)
         self.chunks = {n: (n - 1) * chunk_size for n in range(1, self.total_chunk_counts + 1)}
 
@@ -207,27 +215,28 @@
 
             # upload chunks
             for n, v in chunks.items():
                 chunk_size = min(self.size - v, self.size, chunk_size)
                 self.getMultipartURL(n, chunk_size)
                 self.putUpload(n, v, chunk_size)
                 pbar.update(chunk_size)
-                logging.info(f"[{self.filename}]: chunk {n} to {n + chunk_size}")
+                #logging.info(f"[{self.filename}]: chunk {n} - uploaded bytes {v} to {v+ chunk_size}.")
 
     def uploadMain(self):
 
         print(self.stdOut('dataset file processing & checking...'))
         # preprocess
         self.filePreprocess()
         # checking upload status
         self.getChunks()
 
         # upload starts
         if self.uuid != '':
             if self.uploaded:
+                logging.error(f'Upload failed: [{self.filename} - {self.cluster}], already exists, cannot be uploaded again. | File size exceeds 200GB | FileObject: {self.__dict__}')
                 raise ValueError(
                     f'❌ Upload failed: [{self.filename} - {self.cluster}], already exists, cannot be uploaded again.')
             else:
                 print(self.stdOut('continue upload...'))
                 uploaded_chunks = [int(i.split('-')[0]) for i in self.uploaded_chunks.split(',') if i != '']
                 continue_chunks = {i: self.chunks[i] for i in self.chunks if i not in uploaded_chunks}
                 # re-upload last chunk from checkpoint
```

### Comparing `openi-beta-0.0.8/src/openi_beta.egg-info/PKG-INFO` & `openi-beta-0.0.9/src/openi_beta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.0.8
+Version: 0.0.9
 Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

