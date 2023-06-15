# Comparing `tmp/sagemaker_training-4.5.0.tar.gz` & `tmp/sagemaker_training-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sagemaker_training-4.5.0.tar", last modified: Wed Apr 26 16:46:59 2023, max compression
+gzip compressed data, was "dist/sagemaker_training-4.6.0.tar", last modified: Thu Jun 15 16:46:28 2023, max compression
```

## Comparing `sagemaker_training-4.5.0.tar` & `sagemaker_training-4.6.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/
--rw-rw-r--   0 root         (0) root         (0)    11358 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      156 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)      100 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11326 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8922 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/README.md
--rw-rw-r--   0 root         (0) root         (0)        6 2023-04-26 16:16:54.000000 sagemaker_training-4.5.0/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/sagemaker_training.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11326 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/sagemaker_training.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1374 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/sagemaker_training.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/sagemaker_training.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/sagemaker_training.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      265 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/sagemaker_training.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/sagemaker_training.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      108 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2902 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/src/sagemaker_training/
--rw-rw-r--   0 root         (0) root         (0)     2547 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1664 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/_entry_point_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/src/sagemaker_training/c/
--rw-rw-r--   0 root         (0) root         (0)     3533 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/c/gethostname.c
--rw-rw-r--   0 root         (0) root         (0)     7980 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/c/jsmn.c
--rw-rw-r--   0 root         (0) root         (0)     1759 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/c/jsmn.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/src/sagemaker_training/cli/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/cli/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      802 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/cli/train.py
--rw-rw-r--   0 root         (0) root         (0)      781 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/content_types.py
--rw-rw-r--   0 root         (0) root         (0)     7816 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/encoders.py
--rw-rw-r--   0 root         (0) root         (0)     5806 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/entry_point.py
--rw-rw-r--   0 root         (0) root         (0)    49952 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/environment.py
--rw-rw-r--   0 root         (0) root         (0)     3645 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/errors.py
--rw-rw-r--   0 root         (0) root         (0)     5871 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/files.py
--rw-rw-r--   0 root         (0) root         (0)     3013 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/functions.py
--rw-rw-r--   0 root         (0) root         (0)     8362 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/intermediate_output.py
--rw-rw-r--   0 root         (0) root         (0)     2164 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/logging_config.py
--rw-rw-r--   0 root         (0) root         (0)     6411 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/mapping.py
--rw-rw-r--   0 root         (0) root         (0)     5569 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/modules.py
--rw-rw-r--   0 root         (0) root         (0)    20049 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/mpi.py
--rw-rw-r--   0 root         (0) root         (0)     3297 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/params.py
--rw-rw-r--   0 root         (0) root         (0)    15951 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/process.py
--rw-rw-r--   0 root         (0) root         (0)     6583 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/pytorch_xla.py
--rw-rw-r--   0 root         (0) root         (0)    25554 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/record_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     8275 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/recordio.py
--rw-rw-r--   0 root         (0) root         (0)     5574 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/runner.py
--rw-rw-r--   0 root         (0) root         (0)    15735 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/smdataparallel.py
--rw-rw-r--   0 root         (0) root         (0)     1796 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/timeout.py
--rw-rw-r--   0 root         (0) root         (0)     5374 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/torch_distributed.py
--rw-rw-r--   0 root         (0) root         (0)     4459 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 16:46:28.000000 sagemaker_training-4.6.0/
+-rw-rw-r--   0 root         (0) root         (0)    11358 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      156 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)      100 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11326 2023-06-15 16:46:28.000000 sagemaker_training-4.6.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8922 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/README.md
+-rw-rw-r--   0 root         (0) root         (0)        6 2023-06-15 16:17:03.000000 sagemaker_training-4.6.0/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 16:46:28.000000 sagemaker_training-4.6.0/sagemaker_training.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11326 2023-06-15 16:46:28.000000 sagemaker_training-4.6.0/sagemaker_training.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-06-15 16:46:28.000000 sagemaker_training-4.6.0/sagemaker_training.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 16:46:28.000000 sagemaker_training-4.6.0/sagemaker_training.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-06-15 16:46:28.000000 sagemaker_training-4.6.0/sagemaker_training.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      265 2023-06-15 16:46:28.000000 sagemaker_training-4.6.0/sagemaker_training.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-15 16:46:28.000000 sagemaker_training-4.6.0/sagemaker_training.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      108 2023-06-15 16:46:28.000000 sagemaker_training-4.6.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2902 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 16:46:28.000000 sagemaker_training-4.6.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 16:46:28.000000 sagemaker_training-4.6.0/src/sagemaker_training/
+-rw-rw-r--   0 root         (0) root         (0)     2547 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1664 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/_entry_point_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 16:46:28.000000 sagemaker_training-4.6.0/src/sagemaker_training/c/
+-rw-rw-r--   0 root         (0) root         (0)     3533 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/c/gethostname.c
+-rw-rw-r--   0 root         (0) root         (0)     7980 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/c/jsmn.c
+-rw-rw-r--   0 root         (0) root         (0)     1759 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/c/jsmn.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 16:46:28.000000 sagemaker_training-4.6.0/src/sagemaker_training/cli/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/cli/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      802 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/cli/train.py
+-rw-rw-r--   0 root         (0) root         (0)      781 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/content_types.py
+-rw-rw-r--   0 root         (0) root         (0)     7816 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/encoders.py
+-rw-rw-r--   0 root         (0) root         (0)     5806 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/entry_point.py
+-rw-rw-r--   0 root         (0) root         (0)    49952 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/environment.py
+-rw-rw-r--   0 root         (0) root         (0)     3645 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/errors.py
+-rw-rw-r--   0 root         (0) root         (0)     5871 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/files.py
+-rw-rw-r--   0 root         (0) root         (0)     3013 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/functions.py
+-rw-rw-r--   0 root         (0) root         (0)     8362 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/intermediate_output.py
+-rw-rw-r--   0 root         (0) root         (0)     2164 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/logging_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6411 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/mapping.py
+-rw-rw-r--   0 root         (0) root         (0)     5569 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/modules.py
+-rw-rw-r--   0 root         (0) root         (0)    20196 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/mpi.py
+-rw-rw-r--   0 root         (0) root         (0)     3297 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/params.py
+-rw-rw-r--   0 root         (0) root         (0)    15951 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/process.py
+-rw-rw-r--   0 root         (0) root         (0)     6583 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/pytorch_xla.py
+-rw-rw-r--   0 root         (0) root         (0)    25554 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/record_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     8275 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/recordio.py
+-rw-rw-r--   0 root         (0) root         (0)     5574 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/runner.py
+-rw-rw-r--   0 root         (0) root         (0)    15735 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/smdataparallel.py
+-rw-rw-r--   0 root         (0) root         (0)     1796 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/timeout.py
+-rw-rw-r--   0 root         (0) root         (0)     5374 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/torch_distributed.py
+-rw-rw-r--   0 root         (0) root         (0)     4459 2023-06-14 22:52:14.000000 sagemaker_training-4.6.0/src/sagemaker_training/trainer.py
```

### Comparing `sagemaker_training-4.5.0/LICENSE` & `sagemaker_training-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/PKG-INFO` & `sagemaker_training-4.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker_training
-Version: 4.5.0
+Version: 4.6.0
 Summary: Open source library for creating containers to run on Amazon SageMaker.
 Home-page: https://github.com/aws/sagemaker-training-toolkit/
 Author: Amazon Web Services
 License: Apache License 2.0
 Description: ![SageMaker](https://github.com/aws/sagemaker-training-toolkit/raw/master/branding/icon/sagemaker-banner.png)
         
         # SageMaker Training Toolkit
```

### Comparing `sagemaker_training-4.5.0/README.md` & `sagemaker_training-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/sagemaker_training.egg-info/PKG-INFO` & `sagemaker_training-4.6.0/sagemaker_training.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-training
-Version: 4.5.0
+Version: 4.6.0
 Summary: Open source library for creating containers to run on Amazon SageMaker.
 Home-page: https://github.com/aws/sagemaker-training-toolkit/
 Author: Amazon Web Services
 License: Apache License 2.0
 Description: ![SageMaker](https://github.com/aws/sagemaker-training-toolkit/raw/master/branding/icon/sagemaker-banner.png)
         
         # SageMaker Training Toolkit
```

### Comparing `sagemaker_training-4.5.0/sagemaker_training.egg-info/SOURCES.txt` & `sagemaker_training-4.6.0/sagemaker_training.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/setup.py` & `sagemaker_training-4.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/__init__.py` & `sagemaker_training-4.6.0/src/sagemaker_training/__init__.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/_entry_point_type.py` & `sagemaker_training-4.6.0/src/sagemaker_training/_entry_point_type.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/c/gethostname.c` & `sagemaker_training-4.6.0/src/sagemaker_training/c/gethostname.c`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/c/jsmn.c` & `sagemaker_training-4.6.0/src/sagemaker_training/c/jsmn.c`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/c/jsmn.h` & `sagemaker_training-4.6.0/src/sagemaker_training/c/jsmn.h`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/cli/train.py` & `sagemaker_training-4.6.0/src/sagemaker_training/cli/train.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/content_types.py` & `sagemaker_training-4.6.0/src/sagemaker_training/content_types.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/encoders.py` & `sagemaker_training-4.6.0/src/sagemaker_training/encoders.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/entry_point.py` & `sagemaker_training-4.6.0/src/sagemaker_training/entry_point.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/environment.py` & `sagemaker_training-4.6.0/src/sagemaker_training/environment.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/errors.py` & `sagemaker_training-4.6.0/src/sagemaker_training/errors.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/files.py` & `sagemaker_training-4.6.0/src/sagemaker_training/files.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/functions.py` & `sagemaker_training-4.6.0/src/sagemaker_training/functions.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/intermediate_output.py` & `sagemaker_training-4.6.0/src/sagemaker_training/intermediate_output.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/logging_config.py` & `sagemaker_training-4.6.0/src/sagemaker_training/logging_config.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/mapping.py` & `sagemaker_training-4.6.0/src/sagemaker_training/mapping.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/modules.py` & `sagemaker_training-4.6.0/src/sagemaker_training/modules.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/mpi.py` & `sagemaker_training-4.6.0/src/sagemaker_training/mpi.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     logging_config,
     params,
     process,
     SM_EFA_NCCL_INSTANCES,
     SM_EFA_RDMA_INSTANCES,
     timeout,
 )
+from sagemaker_training.smdataparallel import get_dataparallel_exception_classes
 
 logger = logging_config.get_logger()
 logging.getLogger("paramiko").setLevel(logging.INFO)
 
 MPI_FINISHED_STATUS_FILE = "/tmp/done"
 DEFAULT_ERROR_CLASS = errors.ExecuteUserScriptError
 
@@ -401,14 +402,15 @@
 
         training_env = environment.Environment()
         exception_classes = []
         exception_classes += process.get_debugger_exception_classes()
         exception_classes += process.get_tensorflow_exception_classes()
         if training_env.is_modelparallel_enabled:
             exception_classes += get_modelparallel_exception_classes()
+        exception_classes += get_dataparallel_exception_classes()
         # remove potential duplication
         exception_classes = list(set(exception_classes))
         if wait:
             process_spawned = process.check_error(
                 cmd,
                 exception_classes,
                 self._processes_per_host,
```

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/params.py` & `sagemaker_training-4.6.0/src/sagemaker_training/params.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/process.py` & `sagemaker_training-4.6.0/src/sagemaker_training/process.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/pytorch_xla.py` & `sagemaker_training-4.6.0/src/sagemaker_training/pytorch_xla.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/record_pb2.py` & `sagemaker_training-4.6.0/src/sagemaker_training/record_pb2.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/recordio.py` & `sagemaker_training-4.6.0/src/sagemaker_training/recordio.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/runner.py` & `sagemaker_training-4.6.0/src/sagemaker_training/runner.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/smdataparallel.py` & `sagemaker_training-4.6.0/src/sagemaker_training/smdataparallel.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/timeout.py` & `sagemaker_training-4.6.0/src/sagemaker_training/timeout.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/torch_distributed.py` & `sagemaker_training-4.6.0/src/sagemaker_training/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.5.0/src/sagemaker_training/trainer.py` & `sagemaker_training-4.6.0/src/sagemaker_training/trainer.py`

 * *Files identical despite different names*

