# Comparing `tmp/scrapy_arweave-0.0.2.tar.gz` & `tmp/scrapy_arweave-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy_arweave-0.0.2.tar", last modified: Thu Jun 15 04:27:20 2023, max compression
+gzip compressed data, was "scrapy_arweave-0.1.0.tar", last modified: Thu Jun 15 14:19:12 2023, max compression
```

## Comparing `scrapy_arweave-0.0.2.tar` & `scrapy_arweave-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 blokchainaholic   (501) staff       (20)        0 2023-06-15 04:27:20.882945 scrapy_arweave-0.0.2/
--rw-r--r--   0 blokchainaholic   (501) staff       (20)     1056 2023-05-15 03:22:58.000000 scrapy_arweave-0.0.2/LICENSE.txt
--rw-r--r--   0 blokchainaholic   (501) staff       (20)     4809 2023-06-15 04:27:20.882798 scrapy_arweave-0.0.2/PKG-INFO
--rw-r--r--   0 blokchainaholic   (501) staff       (20)     3877 2023-06-15 04:25:39.000000 scrapy_arweave-0.0.2/README.md
--rw-r--r--   0 blokchainaholic   (501) staff       (20)      297 2023-05-15 04:39:09.000000 scrapy_arweave-0.0.2/pyproject.toml
-drwxr-xr-x   0 blokchainaholic   (501) staff       (20)        0 2023-06-15 04:27:20.881877 scrapy_arweave-0.0.2/scrapy_arweave/
--rw-r--r--   0 blokchainaholic   (501) staff       (20)       22 2023-05-15 02:52:23.000000 scrapy_arweave-0.0.2/scrapy_arweave/__init__.py
--rw-r--r--   0 blokchainaholic   (501) staff       (20)     2955 2023-05-16 12:13:37.000000 scrapy_arweave-0.0.2/scrapy_arweave/client.py
--rw-r--r--   0 blokchainaholic   (501) staff       (20)     1053 2023-05-16 07:57:09.000000 scrapy_arweave-0.0.2/scrapy_arweave/feedexport.py
--rw-r--r--   0 blokchainaholic   (501) staff       (20)    12532 2023-05-16 12:51:28.000000 scrapy_arweave-0.0.2/scrapy_arweave/pipelines.py
-drwxr-xr-x   0 blokchainaholic   (501) staff       (20)        0 2023-06-15 04:27:20.882583 scrapy_arweave-0.0.2/scrapy_arweave.egg-info/
--rw-r--r--   0 blokchainaholic   (501) staff       (20)     4809 2023-06-15 04:27:20.000000 scrapy_arweave-0.0.2/scrapy_arweave.egg-info/PKG-INFO
--rw-r--r--   0 blokchainaholic   (501) staff       (20)      343 2023-06-15 04:27:20.000000 scrapy_arweave-0.0.2/scrapy_arweave.egg-info/SOURCES.txt
--rw-r--r--   0 blokchainaholic   (501) staff       (20)        1 2023-06-15 04:27:20.000000 scrapy_arweave-0.0.2/scrapy_arweave.egg-info/dependency_links.txt
--rw-r--r--   0 blokchainaholic   (501) staff       (20)       23 2023-06-15 04:27:20.000000 scrapy_arweave-0.0.2/scrapy_arweave.egg-info/requires.txt
--rw-r--r--   0 blokchainaholic   (501) staff       (20)       15 2023-06-15 04:27:20.000000 scrapy_arweave-0.0.2/scrapy_arweave.egg-info/top_level.txt
--rw-r--r--   0 blokchainaholic   (501) staff       (20)       38 2023-06-15 04:27:20.882996 scrapy_arweave-0.0.2/setup.cfg
--rw-r--r--   0 blokchainaholic   (501) staff       (20)     4614 2023-06-15 04:25:42.000000 scrapy_arweave-0.0.2/setup.py
+drwxr-xr-x   0 blokchainaholic   (501) staff       (20)        0 2023-06-15 14:19:12.508804 scrapy_arweave-0.1.0/
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     1056 2023-05-15 03:22:58.000000 scrapy_arweave-0.1.0/LICENSE.txt
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     4894 2023-06-15 14:19:12.508668 scrapy_arweave-0.1.0/PKG-INFO
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     3962 2023-06-15 14:17:16.000000 scrapy_arweave-0.1.0/README.md
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)      297 2023-05-15 04:39:09.000000 scrapy_arweave-0.1.0/pyproject.toml
+drwxr-xr-x   0 blokchainaholic   (501) staff       (20)        0 2023-06-15 14:19:12.507706 scrapy_arweave-0.1.0/scrapy_arweave/
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)       22 2023-05-15 02:52:23.000000 scrapy_arweave-0.1.0/scrapy_arweave/__init__.py
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     3709 2023-06-15 13:21:45.000000 scrapy_arweave-0.1.0/scrapy_arweave/client.py
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     1201 2023-06-15 13:47:16.000000 scrapy_arweave-0.1.0/scrapy_arweave/feedexport.py
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)    12965 2023-06-15 13:54:29.000000 scrapy_arweave-0.1.0/scrapy_arweave/pipelines.py
+drwxr-xr-x   0 blokchainaholic   (501) staff       (20)        0 2023-06-15 14:19:12.508453 scrapy_arweave-0.1.0/scrapy_arweave.egg-info/
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     4894 2023-06-15 14:19:12.000000 scrapy_arweave-0.1.0/scrapy_arweave.egg-info/PKG-INFO
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)      343 2023-06-15 14:19:12.000000 scrapy_arweave-0.1.0/scrapy_arweave.egg-info/SOURCES.txt
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)        1 2023-06-15 14:19:12.000000 scrapy_arweave-0.1.0/scrapy_arweave.egg-info/dependency_links.txt
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)       23 2023-06-15 14:19:12.000000 scrapy_arweave-0.1.0/scrapy_arweave.egg-info/requires.txt
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)       15 2023-06-15 14:19:12.000000 scrapy_arweave-0.1.0/scrapy_arweave.egg-info/top_level.txt
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)       38 2023-06-15 14:19:12.508854 scrapy_arweave-0.1.0/setup.cfg
+-rw-r--r--   0 blokchainaholic   (501) staff       (20)     4614 2023-06-15 14:17:04.000000 scrapy_arweave-0.1.0/setup.py
```

### Comparing `scrapy_arweave-0.0.2/LICENSE.txt` & `scrapy_arweave-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapy_arweave-0.0.2/PKG-INFO` & `scrapy_arweave-0.1.0/scrapy_arweave.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: scrapy_arweave
-Version: 0.0.2
+Name: scrapy-arweave
+Version: 0.1.0
 Summary: Scrapy is a popular open-source and collaborative python framework for extracting the data you need from websites. scrapy-arweave provides scrapy pipelines and feed exports to store items into Arweave.
 Home-page: https://github.com/pawanpaudel93/scrapy-arweave
 Author: Pawan Paudel
 Author-email: pawanpaudel93@gmail.com
 License: ISC
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
@@ -20,30 +20,31 @@
 License-File: LICENSE.txt
 
 
 <p align="center"><img src="logo.png" alt="original" width="100%" height="100%"></p>
 
 <h1 align="center">Welcome to Scrapy-Arweave</h1>
 <p>
-  <img alt="Version" src="https://img.shields.io/badge/version-0.0.2-blue.svg?cacheSeconds=2592000" />
+  <img alt="Version" src="https://img.shields.io/badge/version-0.1.0-blue.svg?cacheSeconds=2592000" />
 </p>
 
 Scrapy is a popular open-source and collaborative python framework for extracting the data you need from websites. scrapy-arweave provides scrapy pipelines and feed exports to store items into [Arweave](https://arweave.org/).
 
 ### 🏠 [Homepage](https://github.com/pawanpaudel93/scrapy-arweave)
 
 ## Install
 
 ```shell
 pip install scrapy-arweave
 ```
 
-## Example
+## Examples
 
-[scrapy-arweave-example](https://github.com/pawanpaudel93/scrapy-arweave-example)
+- [scrapy-arweave-example](https://github.com/pawanpaudel93/scrapy-arweave-example)
+- [scrapy-arweave-douban](https://github.com/pawanpaudel93/scrapy-arweave-douban)
 
 ## Usage
 
 1. Install scrapy-arweave and some additional requirements.
 
  ```shell
  pip install scrapy-arweave
```

### Comparing `scrapy_arweave-0.0.2/README.md` & `scrapy_arweave-0.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 <p align="center"><img src="logo.png" alt="original" width="100%" height="100%"></p>
 
 <h1 align="center">Welcome to Scrapy-Arweave</h1>
 <p>
-  <img alt="Version" src="https://img.shields.io/badge/version-0.0.2-blue.svg?cacheSeconds=2592000" />
+  <img alt="Version" src="https://img.shields.io/badge/version-0.1.0-blue.svg?cacheSeconds=2592000" />
 </p>
 
 Scrapy is a popular open-source and collaborative python framework for extracting the data you need from websites. scrapy-arweave provides scrapy pipelines and feed exports to store items into [Arweave](https://arweave.org/).
 
 ### 🏠 [Homepage](https://github.com/pawanpaudel93/scrapy-arweave)
 
 ## Install
 
 ```shell
 pip install scrapy-arweave
 ```
 
-## Example
+## Examples
 
-[scrapy-arweave-example](https://github.com/pawanpaudel93/scrapy-arweave-example)
+- [scrapy-arweave-example](https://github.com/pawanpaudel93/scrapy-arweave-example)
+- [scrapy-arweave-douban](https://github.com/pawanpaudel93/scrapy-arweave-douban)
 
 ## Usage
 
 1. Install scrapy-arweave and some additional requirements.
 
  ```shell
  pip install scrapy-arweave
```

### Comparing `scrapy_arweave-0.0.2/scrapy_arweave/client.py` & `scrapy_arweave-0.1.0/scrapy_arweave/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import hashlib
 import mimetypes
 import os
 from urllib.parse import urljoin
 
+import requests
 from ar import ANS104DataItemHeader, DataItem, Wallet
+from ar.peer import HTTPClient, Peer
 from ar.transaction import Transaction
 from ar.utils.transaction_uploader import create_tag, get_uploader
 from bundlr import Node
 
 
 class ArweaveStorageClient:
     wallet = None
 
     def __init__(self, wallet_jwk, gateway_url) -> None:
         self.GATEWAY_URL = gateway_url
         self.load_wallet(wallet_jwk)
         self.node = Node()
+        self.peer = Peer()
 
     def calculate_hash(self, filepath, algorithm='sha256', chunk_size=65536):
         """
         Calculate the hash of a file using the specified algorithm.
         Returns the hash value as a hexadecimal string.
         """
         # Create a hash object using the specified algorithm
@@ -55,38 +58,60 @@
                 import magic
 
                 mimetype = magic.from_file(file_path, mime=True)
             except ImportError:
                 pass
         return mimetype
 
-    def upload(self, file_path, file_buffer):
+    def upload(self, file_path, file_buffer, hash=None):
         mime_type = self._get_mime_type(file_path)
         try:
             tags = [create_tag("Content-Type", mime_type, True)]
+            if hash:
+                tags.append(create_tag("File-Hash", hash, True))
             dataitem = DataItem(data=file_buffer, header=ANS104DataItemHeader(tags=tags))
             dataitem.sign(self.wallet.rsa)
             result = self.node.send_tx(dataitem.tobytes())
             txid = result['id']
             return txid
         except:
             pass
 
         try:
             with open(file_path, 'rb', buffering=0) as file_handler:
                 tx = Transaction(self.wallet, file_handler=file_handler, file_path=file_path)
                 tx.api_url = self.GATEWAY_URL
                 tx.add_tag('Content-Type', mime_type)
+                if hash:
+                    tx.add_tag('File-Hash', hash)
                 tx.sign()
 
                 uploader = get_uploader(tx, file_handler)
 
                 while not uploader.is_complete:
                     uploader.upload_chunk()
                 return tx.id
         except:
             pass
 
         raise Exception("Upload Error")
 
+    def get_tx_id(self, hash):
+        query = '''query {
+            transactions(
+                first: 1,
+                tags: [{ name: "File-Hash", values: ["%s"]}]
+            ) {
+                edges {
+                    node {
+                        id
+                    }
+                }
+            }
+        }''' % (
+            hash
+        )
+        response = self.peer.graphql(query)
+        return response.get("data").get("transactions").get("edges")[0].get("node").get("id")
+
     def get_url(self, tx_id):
         return urljoin(self.GATEWAY_URL, tx_id)
```

### Comparing `scrapy_arweave-0.0.2/scrapy_arweave/feedexport.py` & `scrapy_arweave-0.1.0/scrapy_arweave/feedexport.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,19 @@
         self.file_name = u.path if u.path else u.netloc
         gateway_url = settings.get("GATEWAY_URL", "https://arweave.net")
         wallet_jwk = settings.get("WALLET_JWK")
         self.client = ArweaveStorageClient(wallet_jwk, gateway_url)
 
     def _store_in_thread(self, file):
         file.seek(0)
-        tx_id = self.client.upload(file.name, file.read())
+        try:
+            file_hash = self.client.calculate_hash(file.name)
+            tx_id = self.client.get_tx_id(file_hash)
+        except:
+            tx_id = self.client.upload(file.name, file.read())
         permalink = self.client.get_url(tx_id)
         logging.info(permalink)
         file.close()
 
 
 def get_feed_storages():
     return {
```

### Comparing `scrapy_arweave-0.0.2/scrapy_arweave/pipelines.py` & `scrapy_arweave-0.1.0/scrapy_arweave/pipelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from scrapy.pipelines.files import FilesPipeline as ParentFilesPipeline
 from scrapy.pipelines.files import FSFilesStore
 from scrapy.pipelines.images import ImageException
 from scrapy.settings import Settings
 from scrapy.utils.log import failure_to_exc_info
 from scrapy.utils.python import get_func_args, to_bytes
 from scrapy.utils.request import referer_str
-from twisted.internet import defer
+from twisted.internet import defer, threads
 
 logger = logging.getLogger(__name__)
 
 
 class ArweaveFilesStore(FSFilesStore):
     WALLET_JWK = ""
     GATEWAY_URL = ""
@@ -32,18 +32,23 @@
 
         super().__init__(basedir)
         self.client = ArweaveStorageClient(self.WALLET_JWK, self.GATEWAY_URL)
 
     def persist_file(self, path, buf, info, meta=None, headers=None):
         absolute_path = self._get_filesystem_path(path)
         super().persist_file(path, buf, info, meta, headers)
-        return self.client.upload(absolute_path, buf.getvalue())
+        file_hash = self.client.calculate_hash(absolute_path)
+        dfd = threads.deferToThread(self.client.upload, absolute_path, buf.getvalue(), file_hash)
+        return dfd
 
     def stat_file(self, path, info):
-        return {}
+        absolute_path = self._get_filesystem_path(path)
+        file_hash = self.client.calculate_hash(absolute_path)
+        dfd = threads.deferToThread(self.client.get_tx_id, file_hash)
+        return dfd.addCallback(lambda tx_id: {"tx_id": tx_id})
 
 
 class FilesPipeline(ParentFilesPipeline):
     """Custom Files Abstract pipeline that implement the file downloading"""
 
     STORE_SCHEMES = {
         '': ArweaveFilesStore,
@@ -123,16 +128,23 @@
             'File (%(status)s): Downloaded file from %(request)s referred in ' '<%(referer)s>',
             {'status': status, 'request': request, 'referer': referer},
             extra={'spider': info.spider},
         )
         self.inc_stats(info.spider, status)
 
         try:
-            path = self.file_path(request, response=response, info=info, item=item)
-            tx_id = self.file_downloaded(response, request, info, item=item)
+            dfd = self.file_downloaded(response, request, info, item=item)
+
+            def _onsuccess(tx_id):
+                permalink = self.store.client.get_url(tx_id)
+                return {'url': request.url, 'tx_id': tx_id, "permalink": permalink}
+
+            if dfd:
+                dfd.addCallbacks(_onsuccess, lambda _: None)
+            return dfd
         except FileException as exc:
             logger.warning(
                 'File (error): Error processing file from %(request)s ' 'referred in <%(referer)s>: %(errormsg)s',
                 {'request': request, 'referer': referer, 'errormsg': str(exc)},
                 extra={'spider': info.spider},
                 exc_info=True,
             )
@@ -141,16 +153,14 @@
             logger.error(
                 'File (unknown-error): Error processing file from %(request)s ' 'referred in <%(referer)s>',
                 {'request': request, 'referer': referer},
                 exc_info=True,
                 extra={'spider': info.spider},
             )
             raise FileException(str(exc))
-        permalink = self.store.client.get_url(tx_id)
-        return {'url': request.url, 'tx_id': tx_id, "permalink": permalink}
 
     def file_downloaded(self, response, request, info, *, item=None):
         path = self.file_path(request, response=response, info=info, item=item)
         buf = BytesIO(response.body)
         buf.seek(0)
         return self.store.persist_file(path, buf, info)
 
@@ -204,24 +214,26 @@
         store_uri = settings['IMAGES_STORE']
         return cls(store_uri, settings=settings)
 
     def file_downloaded(self, response, request, info, *, item=None):
         return self.image_downloaded(response, request, info, item=item)
 
     def image_downloaded(self, response, request, info, *, item=None):
-        tx_id = None
+        result = None
         for path, image, buf in self.get_images(response, request, info, item=item):
             buf.seek(0)
             width, height = image.size
             result = self.store.persist_file(
-                path, buf, info, meta={'width': width, 'height': height}, headers={'Content-Type': 'image/jpeg'}
+                path,
+                buf,
+                info,
+                meta={'width': width, 'height': height},
+                headers={'Content-Type': 'image/jpeg'},
             )
-            if tx_id is None:
-                tx_id = result
-        return tx_id
+        return result
 
     def get_images(self, response, request, info, *, item=None):
         path = self.file_path(request, response=response, info=info, item=item)
         orig_image = self._Image.open(BytesIO(response.body))
 
         width, height = orig_image.size
         if width < self.min_width or height < self.min_height:
```

### Comparing `scrapy_arweave-0.0.2/scrapy_arweave.egg-info/PKG-INFO` & `scrapy_arweave-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: scrapy-arweave
-Version: 0.0.2
+Name: scrapy_arweave
+Version: 0.1.0
 Summary: Scrapy is a popular open-source and collaborative python framework for extracting the data you need from websites. scrapy-arweave provides scrapy pipelines and feed exports to store items into Arweave.
 Home-page: https://github.com/pawanpaudel93/scrapy-arweave
 Author: Pawan Paudel
 Author-email: pawanpaudel93@gmail.com
 License: ISC
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
@@ -20,30 +20,31 @@
 License-File: LICENSE.txt
 
 
 <p align="center"><img src="logo.png" alt="original" width="100%" height="100%"></p>
 
 <h1 align="center">Welcome to Scrapy-Arweave</h1>
 <p>
-  <img alt="Version" src="https://img.shields.io/badge/version-0.0.2-blue.svg?cacheSeconds=2592000" />
+  <img alt="Version" src="https://img.shields.io/badge/version-0.1.0-blue.svg?cacheSeconds=2592000" />
 </p>
 
 Scrapy is a popular open-source and collaborative python framework for extracting the data you need from websites. scrapy-arweave provides scrapy pipelines and feed exports to store items into [Arweave](https://arweave.org/).
 
 ### 🏠 [Homepage](https://github.com/pawanpaudel93/scrapy-arweave)
 
 ## Install
 
 ```shell
 pip install scrapy-arweave
 ```
 
-## Example
+## Examples
 
-[scrapy-arweave-example](https://github.com/pawanpaudel93/scrapy-arweave-example)
+- [scrapy-arweave-example](https://github.com/pawanpaudel93/scrapy-arweave-example)
+- [scrapy-arweave-douban](https://github.com/pawanpaudel93/scrapy-arweave-douban)
 
 ## Usage
 
 1. Install scrapy-arweave and some additional requirements.
 
  ```shell
  pip install scrapy-arweave
```

### Comparing `scrapy_arweave-0.0.2/setup.py` & `scrapy_arweave-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 # Package meta-data.
 NAME = "scrapy_arweave"
 DESCRIPTION = "Scrapy is a popular open-source and collaborative python framework for extracting the data you need from websites. scrapy-arweave provides scrapy pipelines and feed exports to store items into Arweave."
 URL = "https://github.com/pawanpaudel93/scrapy-arweave"
 EMAIL = "pawanpaudel93@gmail.com"
 AUTHOR = "Pawan Paudel"
 REQUIRES_PYTHON = ">=3.0"
-VERSION = "0.0.2"
+VERSION = "0.1.0"
 
 REQUIRED = [
     "python-magic",
     "pyarweave",
 ]
 
 EXTRAS = {
```

