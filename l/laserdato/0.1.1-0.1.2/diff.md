# Comparing `tmp/laserdato-0.1.1.tar.gz` & `tmp/laserdato-0.1.2.tar.gz`

## Comparing `laserdato-0.1.1.tar` & `laserdato-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 laserdato-0.1.1/main.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 laserdato-0.1.1/laserdato/__init__.py
--rw-r--r--   0        0        0     5021 2020-02-02 00:00:00.000000 laserdato-0.1.1/laserdato/align.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 laserdato-0.1.1/laserdato/get_model.py
--rw-r--r--   0        0        0     5691 2020-02-02 00:00:00.000000 laserdato-0.1.1/laserdato/laser.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 laserdato-0.1.1/laserdato/embed/embed.py
--rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 laserdato-0.1.1/laserdato/embed/encoder.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 laserdato-0.1.1/laserdato/embed/laserLstmEncoder.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 laserdato-0.1.1/laserdato/embed/laserTransformerEncoder.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 laserdato-0.1.1/laserdato/embed/multiGpuEncoder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 laserdato-0.1.1/laserdato/lib/__init__.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 laserdato-0.1.1/laserdato/lib/constants.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 laserdato-0.1.1/laserdato/lib/text_processing.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 laserdato-0.1.1/settings.json/settings.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 laserdato-0.1.1/LICENSE
--rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 laserdato-0.1.1/README.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 laserdato-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 laserdato-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 laserdato-0.1.2/main.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 laserdato-0.1.2/laserdato/__init__.py
+-rw-r--r--   0        0        0     5021 2020-02-02 00:00:00.000000 laserdato-0.1.2/laserdato/align.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 laserdato-0.1.2/laserdato/get_model.py
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 laserdato-0.1.2/laserdato/laser.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 laserdato-0.1.2/laserdato/embed/embed.py
+-rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 laserdato-0.1.2/laserdato/embed/encoder.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 laserdato-0.1.2/laserdato/embed/laserLstmEncoder.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 laserdato-0.1.2/laserdato/embed/laserTransformerEncoder.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 laserdato-0.1.2/laserdato/embed/multiGpuEncoder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 laserdato-0.1.2/laserdato/lib/__init__.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 laserdato-0.1.2/laserdato/lib/constants.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 laserdato-0.1.2/laserdato/lib/text_processing.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 laserdato-0.1.2/settings.json/settings.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 laserdato-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 laserdato-0.1.2/README.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 laserdato-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 laserdato-0.1.2/PKG-INFO
```

### Comparing `laserdato-0.1.1/main.py` & `laserdato-0.1.2/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # print(embeddings)
 # # print(sp.EncodeAsPieces(tes))
 # # print(sp.encode_as_pieces("test"))
 import logging
 import sys
 
 
-from laser import Laser
+from laserdato import Laser
 
 
 # def main():
 #     laser = Laser(verbose=True)
 #     laser.activateMultiGpuEncoder([0, 1])
 #     lang0 = [
 #         "I believe",
```

### Comparing `laserdato-0.1.1/laserdato/align.py` & `laserdato-0.1.2/laserdato/align.py`

 * *Files identical despite different names*

### Comparing `laserdato-0.1.1/laserdato/get_model.py` & `laserdato-0.1.2/laserdato/get_model.py`

 * *Files identical despite different names*

### Comparing `laserdato-0.1.1/laserdato/laser.py` & `laserdato-0.1.2/laserdato/laser.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,26 +90,26 @@
         self.verbose = verbose
 
     def set_lang(self, lang: str):
         if lang and lang not in laser3_langs:
             raise ValueError(f"Language {lang} not supported")
         self.lang = lang
 
-    def activateMultiGpuEncoder(self, target_devices: list[int]):
+    def activate_multi_mpu_encoder(self, target_devices: list[int]):
         """
         :param target_devices: list of GPU ids to use for embedding
         Don't forget to close the encoder with closeMultiGpuEncoder
         """
         if self.cpu:
             raise ValueError("Cannot launch multiGpuEncoder with cpu=True")
         new_encoder = self._load_encoder()
         self.multiGpuEncoder = MultiGpuEncoder(target_devices, new_encoder)
         self.multiGpu = True
 
-    def deactivateMultiGpuEncoder(self):
+    def deactivate_multi_gpu_encoder(self):
         if self.multiGpu == False:
             raise ValueError("Cannot close multiGpuEncoder, it is not open")
         self.multiGpuEncoder.delete()
         self.multiGpu = False
 
     def embed_sentences(self, sentences: list[str]) -> list[np.ndarray]:
         """
```

### Comparing `laserdato-0.1.1/laserdato/embed/embed.py` & `laserdato-0.1.2/laserdato/embed/embed.py`

 * *Files identical despite different names*

### Comparing `laserdato-0.1.1/laserdato/embed/encoder.py` & `laserdato-0.1.2/laserdato/embed/encoder.py`

 * *Files identical despite different names*

### Comparing `laserdato-0.1.1/laserdato/embed/laserLstmEncoder.py` & `laserdato-0.1.2/laserdato/embed/laserLstmEncoder.py`

 * *Files identical despite different names*

### Comparing `laserdato-0.1.1/laserdato/embed/laserTransformerEncoder.py` & `laserdato-0.1.2/laserdato/embed/laserTransformerEncoder.py`

 * *Files identical despite different names*

### Comparing `laserdato-0.1.1/laserdato/embed/multiGpuEncoder.py` & `laserdato-0.1.2/laserdato/embed/multiGpuEncoder.py`

 * *Files identical despite different names*

### Comparing `laserdato-0.1.1/laserdato/lib/constants.py` & `laserdato-0.1.2/laserdato/lib/constants.py`

 * *Files identical despite different names*

### Comparing `laserdato-0.1.1/laserdato/lib/text_processing.py` & `laserdato-0.1.2/laserdato/lib/text_processing.py`

 * *Files identical despite different names*

### Comparing `laserdato-0.1.1/LICENSE` & `laserdato-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `laserdato-0.1.1/README.md` & `laserdato-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `laserdato-0.1.1/pyproject.toml` & `laserdato-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "laserdato"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="temp", email="" },
 ]
 description = "A small example package"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.7",
```

### Comparing `laserdato-0.1.1/PKG-INFO` & `laserdato-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laserdato
-Version: 0.1.1
+Version: 0.1.2
 Summary: A small example package
 Author: temp
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
```

