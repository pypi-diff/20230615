# Comparing `tmp/langdash-1.3.4b2.tar.gz` & `tmp/langdash-1.3.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-1.3.4b2.tar", last modified: Tue Jun 13 06:54:01 2023, max compression
+gzip compressed data, was "langdash-1.3.5b0.tar", last modified: Wed Jun 14 22:44:35 2023, max compression
```

## Comparing `langdash-1.3.4b2.tar` & `langdash-1.3.5b0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 06:54:01.720600 langdash-1.3.4b2/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.3.4b2/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.3.4b2/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     3727 2023-06-13 06:54:01.720600 langdash-1.3.4b2/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2788 2023-06-12 09:16:01.000000 langdash-1.3.4b2/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 06:54:01.712598 langdash-1.3.4b2/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       78 2023-06-13 06:53:56.000000 langdash-1.3.4b2/langdash/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 06:54:01.716599 langdash-1.3.4b2/langdash/chains/
--rw-rw-r--   0 user      (1000) user      (1000)      178 2023-06-11 03:43:22.000000 langdash-1.3.4b2/langdash/chains/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    14686 2023-06-12 18:40:51.000000 langdash-1.3.4b2/langdash/chains/chains.py
--rw-rw-r--   0 user      (1000) user      (1000)     8176 2023-06-12 18:40:51.000000 langdash-1.3.4b2/langdash/chains/nodes.py
--rw-rw-r--   0 user      (1000) user      (1000)      253 2023-06-11 03:43:22.000000 langdash-1.3.4b2/langdash/chains/typing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 06:54:01.712598 langdash-1.3.4b2/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.3.4b2/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.3.4b2/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     6400 2023-06-12 02:43:18.000000 langdash-1.3.4b2/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)      777 2023-06-11 03:43:22.000000 langdash-1.3.4b2/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-06-06 03:06:05.000000 langdash-1.3.4b2/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     7160 2023-06-10 00:53:03.000000 langdash-1.3.4b2/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 06:54:01.716599 langdash-1.3.4b2/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.3.4b2/langdash/models/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 06:54:01.716599 langdash-1.3.4b2/langdash/models/_mixins/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.3.4b2/langdash/models/_mixins/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3355 2023-06-12 18:40:51.000000 langdash-1.3.4b2/langdash/models/_mixins/tensor_based_infer_mixin.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 06:54:01.716599 langdash-1.3.4b2/langdash/models/_tokenizer/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.3.4b2/langdash/models/_tokenizer/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.3.4b2/langdash/models/_tokenizer/_bpe.py
--rw-rw-r--   0 user      (1000) user      (1000)     1532 2023-06-13 05:07:37.000000 langdash-1.3.4b2/langdash/models/_tokenizer/bytes_dict_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1810 2023-06-13 05:07:37.000000 langdash-1.3.4b2/langdash/models/_tokenizer/hf_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1429 2023-06-13 05:07:37.000000 langdash-1.3.4b2/langdash/models/_tokenizer/rwkv_20b_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)      664 2023-06-13 05:07:37.000000 langdash-1.3.4b2/langdash/models/_tokenizer/tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     5135 2023-06-12 18:40:51.000000 langdash-1.3.4b2/langdash/models/ctransformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     4744 2023-06-13 05:07:37.000000 langdash-1.3.4b2/langdash/models/llama_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.3.4b2/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)     7765 2023-06-12 18:40:51.000000 langdash-1.3.4b2/langdash/models/rwkv_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-12 18:40:51.000000 langdash-1.3.4b2/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5472 2023-06-13 05:07:37.000000 langdash-1.3.4b2/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.3.4b2/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     2753 2023-06-12 18:40:51.000000 langdash-1.3.4b2/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 06:54:01.712598 langdash-1.3.4b2/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.3.4b2/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.3.4b2/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.3.4b2/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2832 2023-06-09 18:58:51.000000 langdash-1.3.4b2/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 06:54:01.716599 langdash-1.3.4b2/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3727 2023-06-13 06:54:01.000000 langdash-1.3.4b2/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1658 2023-06-13 06:54:01.000000 langdash-1.3.4b2/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-13 06:54:01.000000 langdash-1.3.4b2/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      289 2023-06-13 06:54:01.000000 langdash-1.3.4b2/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-13 06:54:01.000000 langdash-1.3.4b2/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-13 06:54:01.720600 langdash-1.3.4b2/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1696 2023-06-13 00:28:09.000000 langdash-1.3.4b2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-14 22:44:35.744075 langdash-1.3.5b0/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.3.5b0/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.3.5b0/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     3727 2023-06-14 22:44:35.744075 langdash-1.3.5b0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2788 2023-06-12 09:16:01.000000 langdash-1.3.5b0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-14 22:44:35.736075 langdash-1.3.5b0/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       78 2023-06-14 22:44:24.000000 langdash-1.3.5b0/langdash/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-14 22:44:35.740075 langdash-1.3.5b0/langdash/chains/
+-rw-rw-r--   0 user      (1000) user      (1000)      178 2023-06-11 03:43:22.000000 langdash-1.3.5b0/langdash/chains/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14686 2023-06-12 18:40:51.000000 langdash-1.3.5b0/langdash/chains/chains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8176 2023-06-12 18:40:51.000000 langdash-1.3.5b0/langdash/chains/nodes.py
+-rw-rw-r--   0 user      (1000) user      (1000)      253 2023-06-11 03:43:22.000000 langdash-1.3.5b0/langdash/chains/typing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-14 22:44:35.736075 langdash-1.3.5b0/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.3.5b0/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.3.5b0/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6400 2023-06-12 02:43:18.000000 langdash-1.3.5b0/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1150 2023-06-14 22:44:24.000000 langdash-1.3.5b0/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-06-06 03:06:05.000000 langdash-1.3.5b0/langdash/llm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7160 2023-06-10 00:53:03.000000 langdash-1.3.5b0/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-14 22:44:35.740075 langdash-1.3.5b0/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.3.5b0/langdash/models/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-14 22:44:35.740075 langdash-1.3.5b0/langdash/models/_mixins/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.3.5b0/langdash/models/_mixins/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3355 2023-06-12 18:40:51.000000 langdash-1.3.5b0/langdash/models/_mixins/tensor_based_infer_mixin.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-14 22:44:35.744075 langdash-1.3.5b0/langdash/models/_tokenizer/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.3.5b0/langdash/models/_tokenizer/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.3.5b0/langdash/models/_tokenizer/_bpe.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1532 2023-06-13 05:07:37.000000 langdash-1.3.5b0/langdash/models/_tokenizer/bytes_dict_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1810 2023-06-13 05:07:37.000000 langdash-1.3.5b0/langdash/models/_tokenizer/hf_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1564 2023-06-14 22:44:24.000000 langdash-1.3.5b0/langdash/models/_tokenizer/rwkv_20b_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)      664 2023-06-13 05:07:37.000000 langdash-1.3.5b0/langdash/models/_tokenizer/tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5135 2023-06-12 18:40:51.000000 langdash-1.3.5b0/langdash/models/ctransformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4744 2023-06-13 05:07:37.000000 langdash-1.3.5b0/langdash/models/llama_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.3.5b0/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7586 2023-06-14 22:44:24.000000 langdash-1.3.5b0/langdash/models/rwkv_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-12 18:40:51.000000 langdash-1.3.5b0/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5472 2023-06-13 05:07:37.000000 langdash-1.3.5b0/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.3.5b0/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.3.5b0/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-14 22:44:35.736075 langdash-1.3.5b0/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.3.5b0/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.3.5b0/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.3.5b0/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2832 2023-06-09 18:58:51.000000 langdash-1.3.5b0/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-14 22:44:35.740075 langdash-1.3.5b0/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3727 2023-06-14 22:44:35.000000 langdash-1.3.5b0/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1658 2023-06-14 22:44:35.000000 langdash-1.3.5b0/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-14 22:44:35.000000 langdash-1.3.5b0/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      289 2023-06-14 22:44:35.000000 langdash-1.3.5b0/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-14 22:44:35.000000 langdash-1.3.5b0/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-14 22:44:35.744075 langdash-1.3.5b0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1696 2023-06-13 00:28:09.000000 langdash-1.3.5b0/setup.py
```

### Comparing `langdash-1.3.4b2/LICENSE.txt` & `langdash-1.3.5b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/PKG-INFO` & `langdash-1.3.5b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.3.4b2
+Version: 1.3.5b0
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langdash-1.3.4b2/README.md` & `langdash-1.3.5b0/README.md`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/langdash/chains/chains.py` & `langdash-1.3.5b0/langdash/chains/chains.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/langdash/chains/nodes.py` & `langdash-1.3.5b0/langdash/chains/nodes.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/langdash/classify/token_qa.py` & `langdash-1.3.5b0/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/langdash/core.py` & `langdash-1.3.5b0/langdash/core.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/langdash/llm.py` & `langdash-1.3.5b0/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/langdash/llm_session.py` & `langdash-1.3.5b0/langdash/llm_session.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/langdash/models/_mixins/tensor_based_infer_mixin.py` & `langdash-1.3.5b0/langdash/models/_mixins/tensor_based_infer_mixin.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/langdash/models/_tokenizer/_bpe.py` & `langdash-1.3.5b0/langdash/models/_tokenizer/_bpe.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/langdash/models/_tokenizer/bytes_dict_tokenizer.py` & `langdash-1.3.5b0/langdash/models/_tokenizer/bytes_dict_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/langdash/models/_tokenizer/hf_tokenizer.py` & `langdash-1.3.5b0/langdash/models/_tokenizer/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/langdash/models/_tokenizer/rwkv_20b_tokenizer.py` & `langdash-1.3.5b0/langdash/models/_tokenizer/rwkv_20b_tokenizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from typing import List, Union, Dict, Optional, Generator
 from .tokenizer import Tokenizer, BufferedToken
+from ._bpe import decode as bpe_decode
 
 
 class Rwkv20BTokenizer(Tokenizer):
 
-  def __init__(self, tokenizer, vocab: Dict[str, int]):
+  def __init__(self, tokenizer):
     self.tokenizer = tokenizer
-    self.vocab = vocab
+    self.vocab = {
+      bpe_decode(logits_tokstr): logits_tokid
+      for logits_tokstr, logits_tokid in tokenizer.get_vocab().items()
+    }
 
   def encode(self, text: str, add_special_tokens: bool = False) -> List[int]:
     return self.tokenizer.encode(
       text, add_special_tokens=add_special_tokens
     ).ids
 
   def decode(self, tokens: List[int]) -> str:
```

### Comparing `langdash-1.3.4b2/langdash/models/_tokenizer/tokenizer.py` & `langdash-1.3.5b0/langdash/models/_tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/langdash/models/ctransformers.py` & `langdash-1.3.5b0/langdash/models/ctransformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/langdash/models/llama_cpp.py` & `langdash-1.3.5b0/langdash/models/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/langdash/models/mock.py` & `langdash-1.3.5b0/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/langdash/models/rwkv_cpp.py` & `langdash-1.3.5b0/langdash/models/rwkv_cpp.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import sys
 import torch
 import tokenizers  # type: ignore
 
 from langdash.llm import LLM
 from langdash.llm_session import LLMGenerationSessionForRawText, LLMState
 import langdash.sampling as sampling
-import langdash.models._bpe as bpe
 from ._tokenizer.rwkv_20b_tokenizer import Rwkv20BTokenizer
 from ._mixins.tensor_based_infer_mixin import TensorBasedInferMixin
 
 _rwkv_lib: Optional[str] = None
 _rwkv_cpp_folder: Optional[str] = None
 
 RWKV_CPP_COMMIT_DEFAULT = "82c4ac78f4d10ef1af87104fc051ea2119eaaddf"
@@ -133,19 +132,15 @@
     )
     if llm._tokenizer_type == "20B":
       tokenizer = tokenizers.Tokenizer.from_file(llm._tokenizer_path)
     elif llm._tokenizer_type == "world":
       tokenizer = rwkv_tokenizer.TRIE_TOKENIZER(llm._tokenizer_path)
     else:
       raise ValueError(f"unknown tokenizer type {llm._tokenizer_type}")
-    vocab = {
-      bpe.decode(logits_tokstr): logits_tokid
-      for logits_tokstr, logits_tokid in tokenizer.get_vocab().items()
-    }
-    self.tokenizer = Rwkv20BTokenizer(tokenizer, vocab)
+    self.tokenizer = Rwkv20BTokenizer(tokenizer)
     self.eos_token = 0
 
   def eval(self, tokid, state) -> Tuple[torch.Tensor, torch.Tensor]:
     return self.model.eval(tokid, state)
 
 
 class RwkvCppSession(
```

### Comparing `langdash-1.3.4b2/langdash/models/sentence_transformers.py` & `langdash-1.3.5b0/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/langdash/models/transformers.py` & `langdash-1.3.5b0/langdash/models/transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/langdash/response.py` & `langdash-1.3.5b0/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/langdash/sampling.py` & `langdash-1.3.5b0/langdash/sampling.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,35 @@
   cumulative_probs = torch.cumsum(sorted_probs, dim=-1)
   cutoff = float(sorted_probs[torch.argmax((cumulative_probs > top_p).long())])
   probs[probs < cutoff] = 0
   return probs
 
 
 @torch.jit.script
+def _sample_top_k(probs: torch.Tensor, top_k: int, top_p: float):
+  assert 0 <= top_k <= probs.shape[0], "top_k must be in [0, len]"
+  assert 0.0 <= top_p <= 1.0, "top_p must be in [0.0, 1.0]"
+  sorted_probs, indices = torch.sort(probs, descending=True)
+  probs[indices[top_k:]] = 0.
+
+  if top_p > 0.:
+    mag = torch.sum(sorted_probs)
+    probs /= mag
+    sorted_probs /= mag
+
+    cumulative_probs = torch.cumsum(sorted_probs, dim=-1)
+    cutoff = float(
+      sorted_probs[torch.argmax((cumulative_probs > top_p).long())]
+    )
+    probs[probs < cutoff] = 0.
+
+  return probs
+
+
+@torch.jit.script
 def _sample_typical(
   probs: torch.Tensor, logits: torch.Tensor, mass: float
 ) -> torch.Tensor:
   # https://github.com/huggingface/transformers/compare/main...cimeister:typicalsampling:typical-pr
   assert 0.0 <= mass <= 1.0, "typical mass must be in [0.0, 1.0]"
   normalized = -torch.log(probs)
   ent = torch.nansum(normalized * probs, dim=-1, keepdim=True)
@@ -55,18 +76,21 @@
         logits[tok] /= rep_penalty
 
   probs = logits_to_probs(logits)
 
   if args.temperature == 0.0:
     probs = _sample_greedy(probs)
   else:
-    if args.typical_mass > 0.0:
-      probs = _sample_typical(probs, logits, args.typical_mass)
-    if args.top_p > 0.0:
-      probs = _sample_top_p(probs, args.top_p)
+    if args.top_k > 0:
+      probs = _sample_top_k(probs, args.top_k, args.top_p)
+    else:
+      if args.typical_mass > 0.0:
+        probs = _sample_typical(probs, logits, args.typical_mass)
+      if args.top_p > 0.0:
+        probs = _sample_top_p(probs, args.top_p)
     if args.temperature != 1.0:
       probs = probs.pow(1.0 / args.temperature)
 
   return probs
 
 
 def sample(*args, **kwargs) -> int:
```

### Comparing `langdash-1.3.4b2/langdash/search/embedding_search.py` & `langdash-1.3.5b0/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/langdash/search/engine.py` & `langdash-1.3.5b0/langdash/search/engine.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/langdash/search/multichoice_search.py` & `langdash-1.3.5b0/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/langdash.egg-info/PKG-INFO` & `langdash-1.3.5b0/langdash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.3.4b2
+Version: 1.3.5b0
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langdash-1.3.4b2/langdash.egg-info/SOURCES.txt` & `langdash-1.3.5b0/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.3.4b2/setup.py` & `langdash-1.3.5b0/setup.py`

 * *Files identical despite different names*

