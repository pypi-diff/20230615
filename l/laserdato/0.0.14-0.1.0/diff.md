# Comparing `tmp/laserdato-0.0.14.tar.gz` & `tmp/laserdato-0.1.0.tar.gz`

## Comparing `laserdato-0.0.14.tar` & `laserdato-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 laserdato-0.0.14/main.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/__init__.py
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/align.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/get_model.py
--rw-r--r--   0        0        0     5583 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/laser.py
--rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/embed/embed.py
--rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/embed/encoder.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/embed/laserLstmEncoder.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/embed/laserTransformerEncoder.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/embed/multiGpuEncoder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/lib/__init__.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/lib/constants.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/lib/text_processing.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 laserdato-0.0.14/settings.json/settings.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 laserdato-0.0.14/LICENSE
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 laserdato-0.0.14/README.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 laserdato-0.0.14/pyproject.toml
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 laserdato-0.0.14/PKG-INFO
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 laserdato-0.1.0/main.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 laserdato-0.1.0/laserdato/__init__.py
+-rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 laserdato-0.1.0/laserdato/align.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 laserdato-0.1.0/laserdato/get_model.py
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 laserdato-0.1.0/laserdato/laser.py
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 laserdato-0.1.0/laserdato/embed/embed.py
+-rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 laserdato-0.1.0/laserdato/embed/encoder.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 laserdato-0.1.0/laserdato/embed/laserLstmEncoder.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 laserdato-0.1.0/laserdato/embed/laserTransformerEncoder.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 laserdato-0.1.0/laserdato/embed/multiGpuEncoder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 laserdato-0.1.0/laserdato/lib/__init__.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 laserdato-0.1.0/laserdato/lib/constants.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 laserdato-0.1.0/laserdato/lib/text_processing.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 laserdato-0.1.0/settings.json/settings.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 laserdato-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 laserdato-0.1.0/README.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 laserdato-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 laserdato-0.1.0/PKG-INFO
```

### Comparing `laserdato-0.0.14/laserdato/align.py` & `laserdato-0.1.0/laserdato/align.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 
 logging.getLogger("faiss.loader").setLevel(logging.ERROR)
 
 import faiss
+
 from enum import Enum
 import numpy as np
 from collections import OrderedDict
 
 
 def match_sentences_with_best_neighbors(
     sentences_lang0, sentences_lang1, best_neighbors, scores, remove_bad_matched=False
```

### Comparing `laserdato-0.0.14/laserdato/get_model.py` & `laserdato-0.1.0/laserdato/get_model.py`

 * *Files identical despite different names*

### Comparing `laserdato-0.0.14/laserdato/laser.py` & `laserdato-0.1.0/laserdato/laser.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,24 +34,25 @@
         self,
         hugging_face=False,
         max_sentences=10000,
         max_tokens=12000,
         sort_kind="mergesort",
     ):
         version = 0
-        if self.lang is not None:
+        if self.lang:
             version = 1
             pt = load_or_download_file(f"laser3-{self.lang}.v{version}.pt")
-            if self.lang in langs_with_specific_vocab:
-                spm = load_or_download_file(
-                    f"laser3-{self.lang}.v{version}.spm"
-                ).as_posix()
-                load_or_download_file(f"laser3-{self.lang}.v{version}.cvocab")
         else:
             pt = load_or_download_file("laser2.pt")
+        if self.lang and self.lang in langs_with_specific_vocab:
+            self.spm = load_or_download_file(
+                f"laser3-{self.lang}.v{version}.spm"
+            ).as_posix()
+            load_or_download_file(f"laser3-{self.lang}.v{version}.cvocab")
+        else:
             self.spm = str(load_or_download_file("laser2.spm").as_posix())
             load_or_download_file("laser2.cvocab")
         encoder = load_model(
             encoder=str(pt),
             spm_model=self.spm,
             verbose=self.verbose,
             hugging_face=hugging_face,
@@ -87,34 +88,32 @@
         self.verbose = verbose
 
     def set_lang(self, lang: str):
         if lang and lang not in laser3_langs:
             raise ValueError(f"Language {lang} not supported")
         self.lang = lang
 
-    def launchMultiGpuEncoder(self, target_devices: list[int]):
+    def activateMultiGpuEncoder(self, target_devices: list[int]):
         """
         :param target_devices: list of GPU ids to use for embedding
         Don't forget to close the encoder with closeMultiGpuEncoder
         """
         if self.cpu:
             raise ValueError("Cannot launch multiGpuEncoder with cpu=True")
         new_encoder = self._load_encoder()
         self.multiGpuEncoder = MultiGpuEncoder(target_devices, new_encoder)
         self.multiGpu = True
 
-    def closeMultiGpuEncoder(self):
+    def deactivateMultiGpuEncoder(self):
         if self.multiGpu == False:
             raise ValueError("Cannot close multiGpuEncoder, it is not open")
-        self.encoder.delete()
+        self.multiGpuEncoder.delete()
         self.multiGpu = False
 
-    def embed_sentences(
-        self, sentences: list[str], verbose: bool = False
-    ) -> list[np.ndarray]:
+    def embed_sentences(self, sentences: list[str]) -> list[np.ndarray]:
         """
         :param sentences: list of sentences to embed
         :return: list of embeddings
         """
         embeddings = embed_sentences(
             sentences=sentences,
             encoder=self.encoder,
@@ -130,23 +129,19 @@
         remove_bad_matched: bool = False,
     ) -> list[tuple[str, str, int]]:
         """
         Not compatible with laser3, if you want to use laser3 lang, use align_with_embeddings directly
         Align two lists of sentences using xSIM and the LASER embeddings
         :param sentences_lang0: list of sentences in lang0
         :param sentences_lang1: list of sentences in lang1
-        :param remove_bad_matched: if False it keep sentence with no match as (sentence_1, "",0), if True it remove them
+        :param remove_bad_matched: if False it keep sentence with no match as (sentence_1, "",0), if True it removes them
         :return: list of tuples with at each time the lang0 sentence in order, the lang1 corresponding sentence and the alignment score
         """
-        embeddings_lang0 = self.embed_sentences(
-            sentences=sentences_lang0, verbose=self.verbose
-        )
-        embeddings_lang1 = self.embed_sentences(
-            sentences=sentences_lang1, verbose=self.verbose
-        )
+        embeddings_lang0 = self.embed_sentences(sentences=sentences_lang0)
+        embeddings_lang1 = self.embed_sentences(sentences=sentences_lang1)
         return align_with_embeddings(
             embeddings_lang0,
             embeddings_lang1,
             sentences_lang0,
             sentences_lang1,
             remove_bad_matched=remove_bad_matched,
         )
```

### Comparing `laserdato-0.0.14/laserdato/embed/embed.py` & `laserdato-0.1.0/laserdato/embed/embed.py`

 * *Files 7% similar despite different names*

```diff
@@ -101,23 +101,12 @@
     else:
         logging.getLogger().setLevel(logging.ERROR)
     assert encoder or encoder_path, "Provide initialised encoder or encoder_path"
     buffer_size = max(buffer_size, 1)
     assert (
         not max_sentences or max_sentences <= buffer_size
     ), "--max-sentences/--batch-size cannot be larger than --buffer-size"
-    if encoder_path:
-        raise NotImplementedError("encoder_path not implemented with laserdato")
-        encoder = load_model(
-            encoder_path,
-            spm_model,
-            verbose=verbose,
-            hugging_face=hugging_face,
-            max_sentences=max_sentences,
-            max_tokens=max_tokens,
-            sort_kind=sort_kind,
-        )
     tSMP = time.time()
     sentences = SPMApply(sentences, spm_model, spm_lang)
     if verbose:
         logger.info(f" - Preprocessing finished at {time.time() - tSMP}")
     return EncodeText(encoder, sentences, fp16=fp16, verbose=verbose)
```

### Comparing `laserdato-0.0.14/laserdato/embed/encoder.py` & `laserdato-0.1.0/laserdato/embed/encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         if self.use_cuda:
             if self.verbose:
                 logger.info("transfer encoder to GPU")
                 if device is not None:
                     logger.info(f"device: {device}")
                 else:
                     logger.info("Choosing default GPU device")
-                self.encoder.cuda(self.device)
+            self.encoder.cuda(self.device)
         else:
             if device is not None:
                 raise ValueError(
                     "Cannot specify device because CUDA did not find GPU or cpu is set to True."
                 )
 
     def _process_batch(self, batch):
```

### Comparing `laserdato-0.0.14/laserdato/embed/laserLstmEncoder.py` & `laserdato-0.1.0/laserdato/embed/laserLstmEncoder.py`

 * *Files identical despite different names*

### Comparing `laserdato-0.0.14/laserdato/embed/laserTransformerEncoder.py` & `laserdato-0.1.0/laserdato/embed/laserTransformerEncoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+import logging
+
+logging.getLogger("fairseq.tasks.text_to_speech").setLevel(logging.ERROR)
+
+
 from fairseq.data.dictionary import Dictionary
 from fairseq.models.transformer import (
     Embedding,
     TransformerEncoder,
 )
 from fairseq.modules import LayerNorm
```

### Comparing `laserdato-0.0.14/laserdato/embed/multiGpuEncoder.py` & `laserdato-0.1.0/laserdato/embed/multiGpuEncoder.py`

 * *Files identical despite different names*

### Comparing `laserdato-0.0.14/laserdato/lib/constants.py` & `laserdato-0.1.0/laserdato/lib/constants.py`

 * *Files identical despite different names*

### Comparing `laserdato-0.0.14/laserdato/lib/text_processing.py` & `laserdato-0.1.0/laserdato/lib/text_processing.py`

 * *Files identical despite different names*

### Comparing `laserdato-0.0.14/LICENSE` & `laserdato-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `laserdato-0.0.14/pyproject.toml` & `laserdato-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "laserdato"
-version = "0.0.14"
+version = "0.1.0"
 authors = [
   { name="Lingua Custodia", email="" },
 ]
 description = "A small example package"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.7",
```

