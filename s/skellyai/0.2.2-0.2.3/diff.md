# Comparing `tmp/skellyai-0.2.2.tar.gz` & `tmp/skellyai-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/skellyai-0.2.2.tar", last modified: Tue Jun 13 04:09:34 2023, max compression
+gzip compressed data, was "dist/skellyai-0.2.3.tar", last modified: Thu Jun 15 17:53:37 2023, max compression
```

## Comparing `skellyai-0.2.2.tar` & `skellyai-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-13 04:09:34.165656 skellyai-0.2.2/
--rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-06-13 04:09:34.165063 skellyai-0.2.2/PKG-INFO
--rw-r--r--   0 bennicholl   (501) staff       (20)       38 2023-06-13 04:09:34.165833 skellyai-0.2.2/setup.cfg
--rw-r--r--   0 bennicholl   (501) staff       (20)      713 2023-06-13 04:07:51.000000 skellyai-0.2.2/setup.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-13 04:09:34.158360 skellyai-0.2.2/skellyai/
--rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.2.2/skellyai/__init__.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-13 04:09:34.161947 skellyai-0.2.2/skellyai/get_multi_labels/
--rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.2.2/skellyai/get_multi_labels/__init__.py
--rw-r--r--   0 bennicholl   (501) staff       (20)     1686 2023-05-19 20:23:21.000000 skellyai-0.2.2/skellyai/get_multi_labels/get_multi_labels.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-13 04:09:34.164361 skellyai-0.2.2/skellyai/perform_inference/
--rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.2.2/skellyai/perform_inference/__init__.py
--rw-r--r--   0 bennicholl   (501) staff       (20)      838 2023-06-09 19:43:52.000000 skellyai-0.2.2/skellyai/perform_inference/get_probs.py
--rw-r--r--   0 bennicholl   (501) staff       (20)     2821 2023-06-13 04:07:29.000000 skellyai-0.2.2/skellyai/perform_inference/get_probs_mult_keywords.py
--rw-r--r--   0 bennicholl   (501) staff       (20)     3183 2023-05-18 18:08:51.000000 skellyai-0.2.2/skellyai/train_transformer.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-13 04:09:34.160920 skellyai-0.2.2/skellyai.egg-info/
--rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-06-13 04:09:33.000000 skellyai-0.2.2/skellyai.egg-info/PKG-INFO
--rw-r--r--   0 bennicholl   (501) staff       (20)      435 2023-06-13 04:09:34.000000 skellyai-0.2.2/skellyai.egg-info/SOURCES.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)        1 2023-06-13 04:09:33.000000 skellyai-0.2.2/skellyai.egg-info/dependency_links.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)       33 2023-06-13 04:09:33.000000 skellyai-0.2.2/skellyai.egg-info/requires.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)       62 2023-06-13 04:09:33.000000 skellyai-0.2.2/skellyai.egg-info/top_level.txt
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-15 17:53:37.908238 skellyai-0.2.3/
+-rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-06-15 17:53:37.907896 skellyai-0.2.3/PKG-INFO
+-rw-r--r--   0 bennicholl   (501) staff       (20)       38 2023-06-15 17:53:37.908354 skellyai-0.2.3/setup.cfg
+-rw-r--r--   0 bennicholl   (501) staff       (20)      713 2023-06-15 17:51:18.000000 skellyai-0.2.3/setup.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-15 17:53:37.901695 skellyai-0.2.3/skellyai/
+-rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.2.3/skellyai/__init__.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-15 17:53:37.905362 skellyai-0.2.3/skellyai/get_multi_labels/
+-rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.2.3/skellyai/get_multi_labels/__init__.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)     1686 2023-05-19 20:23:21.000000 skellyai-0.2.3/skellyai/get_multi_labels/get_multi_labels.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-15 17:53:37.907368 skellyai-0.2.3/skellyai/perform_inference/
+-rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.2.3/skellyai/perform_inference/__init__.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)      838 2023-06-09 19:43:52.000000 skellyai-0.2.3/skellyai/perform_inference/get_probs.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)     2983 2023-06-15 17:49:38.000000 skellyai-0.2.3/skellyai/perform_inference/get_probs_mult_keywords.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)     3183 2023-05-18 18:08:51.000000 skellyai-0.2.3/skellyai/train_transformer.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-15 17:53:37.904429 skellyai-0.2.3/skellyai.egg-info/
+-rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-06-15 17:53:37.000000 skellyai-0.2.3/skellyai.egg-info/PKG-INFO
+-rw-r--r--   0 bennicholl   (501) staff       (20)      435 2023-06-15 17:53:37.000000 skellyai-0.2.3/skellyai.egg-info/SOURCES.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)        1 2023-06-15 17:53:37.000000 skellyai-0.2.3/skellyai.egg-info/dependency_links.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)       33 2023-06-15 17:53:37.000000 skellyai-0.2.3/skellyai.egg-info/requires.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)       62 2023-06-15 17:53:37.000000 skellyai-0.2.3/skellyai.egg-info/top_level.txt
```

### Comparing `skellyai-0.2.2/setup.py` & `skellyai-0.2.3/setup.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-from setuptools import setup
+from setuptools import setup
```

### Comparing `skellyai-0.2.2/skellyai/get_multi_labels/get_multi_labels.py` & `skellyai-0.2.3/skellyai/get_multi_labels/get_multi_labels.py`

 * *Files identical despite different names*

### Comparing `skellyai-0.2.2/skellyai/perform_inference/get_probs.py` & `skellyai-0.2.3/skellyai/perform_inference/get_probs.py`

 * *Files identical despite different names*

### Comparing `skellyai-0.2.2/skellyai/perform_inference/get_probs_mult_keywords.py` & `skellyai-0.2.3/skellyai/perform_inference/get_probs_mult_keywords.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-import pandas as pd
+import pandas as pd
```

### Comparing `skellyai-0.2.2/skellyai/train_transformer.py` & `skellyai-0.2.3/skellyai/train_transformer.py`

 * *Files identical despite different names*
