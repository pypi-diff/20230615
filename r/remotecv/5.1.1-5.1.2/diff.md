# Comparing `tmp/remotecv-5.1.1.tar.gz` & `tmp/remotecv-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotecv-5.1.1.tar", last modified: Thu Feb 23 13:31:05 2023, max compression
+gzip compressed data, was "remotecv-5.1.2.tar", last modified: Thu Jun 15 17:25:07 2023, max compression
```

## Comparing `remotecv-5.1.1.tar` & `remotecv-5.1.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:31:05.836261 remotecv-5.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-02-23 13:31:02.000000 remotecv-5.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-23 13:31:02.000000 remotecv-5.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-02-23 13:31:05.836261 remotecv-5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-02-23 13:31:02.000000 remotecv-5.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-23 13:31:02.000000 remotecv-5.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:31:05.824261 remotecv-5.1.1/remotecv/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/celery_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:31:05.824261 remotecv-5.1.1/remotecv/detectors/
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:31:05.824261 remotecv-5.1.1/remotecv/detectors/complete_detector/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/detectors/complete_detector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:31:05.832261 remotecv-5.1.1/remotecv/detectors/face_detector/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/detectors/face_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   676709 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/detectors/face_detector/haarcascade_frontalface_alt.xml
--rw-r--r--   0 runner    (1001) docker     (123)   540616 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/detectors/face_detector/haarcascade_frontalface_alt2.xml
--rw-r--r--   0 runner    (1001) docker     (123)  2689040 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/detectors/face_detector/haarcascade_frontalface_alt_tree.xml
--rw-r--r--   0 runner    (1001) docker     (123)   930127 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/detectors/face_detector/haarcascade_frontalface_default.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:31:05.832261 remotecv-5.1.1/remotecv/detectors/feature_detector/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/detectors/feature_detector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:31:05.832261 remotecv-5.1.1/remotecv/detectors/glasses_detector/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/detectors/glasses_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   601661 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/detectors/glasses_detector/haarcascade_eye_tree_eyeglasses.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:31:05.832261 remotecv-5.1.1/remotecv/detectors/profile_detector/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/detectors/profile_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   828514 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/detectors/profile_detector/haarcascade_profileface.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/http_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/image_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:31:05.832261 remotecv-5.1.1/remotecv/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/metrics/logger_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/pyres_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:31:05.832261 remotecv-5.1.1/remotecv/result_store/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/result_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/result_store/memcache_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/result_store/redis_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/unique_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-02-23 13:31:02.000000 remotecv-5.1.1/remotecv/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:31:05.836261 remotecv-5.1.1/remotecv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-02-23 13:31:05.000000 remotecv-5.1.1/remotecv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-02-23 13:31:05.000000 remotecv-5.1.1/remotecv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 13:31:05.000000 remotecv-5.1.1/remotecv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-23 13:31:05.000000 remotecv-5.1.1/remotecv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-02-23 13:31:05.000000 remotecv-5.1.1/remotecv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-23 13:31:05.000000 remotecv-5.1.1/remotecv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-23 13:31:05.836261 remotecv-5.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-02-23 13:31:02.000000 remotecv-5.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.399847 remotecv-5.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-15 17:24:55.000000 remotecv-5.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 17:24:55.000000 remotecv-5.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-06-15 17:25:07.399847 remotecv-5.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-15 17:24:55.000000 remotecv-5.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-15 17:24:55.000000 remotecv-5.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.387847 remotecv-5.1.2/remotecv/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/celery_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.387847 remotecv-5.1.2/remotecv/detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.387847 remotecv-5.1.2/remotecv/detectors/complete_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/complete_detector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.391847 remotecv-5.1.2/remotecv/detectors/face_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/face_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   676709 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/face_detector/haarcascade_frontalface_alt.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   540616 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/face_detector/haarcascade_frontalface_alt2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)  2689040 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/face_detector/haarcascade_frontalface_alt_tree.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   930127 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/face_detector/haarcascade_frontalface_default.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.395847 remotecv-5.1.2/remotecv/detectors/feature_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/feature_detector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.395847 remotecv-5.1.2/remotecv/detectors/glasses_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/glasses_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   601661 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/glasses_detector/haarcascade_eye_tree_eyeglasses.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.395847 remotecv-5.1.2/remotecv/detectors/profile_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/profile_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   828514 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/detectors/profile_detector/haarcascade_profileface.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/http_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/image_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.395847 remotecv-5.1.2/remotecv/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/metrics/logger_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/pyres_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.395847 remotecv-5.1.2/remotecv/result_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/result_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/result_store/memcache_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/result_store/redis_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/unique_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-06-15 17:24:55.000000 remotecv-5.1.2/remotecv/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:25:07.399847 remotecv-5.1.2/remotecv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-06-15 17:25:07.000000 remotecv-5.1.2/remotecv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-15 17:25:07.000000 remotecv-5.1.2/remotecv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 17:25:07.000000 remotecv-5.1.2/remotecv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 17:25:07.000000 remotecv-5.1.2/remotecv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-15 17:25:07.000000 remotecv-5.1.2/remotecv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 17:25:07.000000 remotecv-5.1.2/remotecv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-15 17:25:07.399847 remotecv-5.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-15 17:24:55.000000 remotecv-5.1.2/setup.py
```

### Comparing `remotecv-5.1.1/LICENSE` & `remotecv-5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/PKG-INFO` & `remotecv-5.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotecv
-Version: 5.1.1
+Version: 5.1.2
 Summary: remotecv is an OpenCV worker for facial and feature recognition
 Author: Bernardo Heynemann
 Author-email: heynemann@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `remotecv-5.1.1/README.md` & `remotecv-5.1.2/README.md`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/celery_tasks.py` & `remotecv-5.1.2/remotecv/celery_tasks.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/detectors/__init__.py` & `remotecv-5.1.2/remotecv/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/detectors/complete_detector/__init__.py` & `remotecv-5.1.2/remotecv/detectors/complete_detector/__init__.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/detectors/face_detector/__init__.py` & `remotecv-5.1.2/remotecv/detectors/face_detector/__init__.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/detectors/face_detector/haarcascade_frontalface_alt.xml` & `remotecv-5.1.2/remotecv/detectors/face_detector/haarcascade_frontalface_alt.xml`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/detectors/face_detector/haarcascade_frontalface_alt2.xml` & `remotecv-5.1.2/remotecv/detectors/face_detector/haarcascade_frontalface_alt2.xml`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/detectors/face_detector/haarcascade_frontalface_alt_tree.xml` & `remotecv-5.1.2/remotecv/detectors/face_detector/haarcascade_frontalface_alt_tree.xml`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/detectors/face_detector/haarcascade_frontalface_default.xml` & `remotecv-5.1.2/remotecv/detectors/face_detector/haarcascade_frontalface_default.xml`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/detectors/feature_detector/__init__.py` & `remotecv-5.1.2/remotecv/detectors/feature_detector/__init__.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/detectors/glasses_detector/haarcascade_eye_tree_eyeglasses.xml` & `remotecv-5.1.2/remotecv/detectors/glasses_detector/haarcascade_eye_tree_eyeglasses.xml`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/detectors/profile_detector/haarcascade_profileface.xml` & `remotecv-5.1.2/remotecv/detectors/profile_detector/haarcascade_profileface.xml`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/error_handler.py` & `remotecv-5.1.2/remotecv/error_handler.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/http_loader.py` & `remotecv-5.1.2/remotecv/http_loader.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/image.py` & `remotecv-5.1.2/remotecv/image.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/image_processor.py` & `remotecv-5.1.2/remotecv/image_processor.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/metrics/logger_metrics.py` & `remotecv-5.1.2/remotecv/metrics/logger_metrics.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/pyres_tasks.py` & `remotecv-5.1.2/remotecv/pyres_tasks.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/result_store/__init__.py` & `remotecv-5.1.2/remotecv/result_store/__init__.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/result_store/memcache_store.py` & `remotecv-5.1.2/remotecv/result_store/memcache_store.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/result_store/redis_store.py` & `remotecv-5.1.2/remotecv/result_store/redis_store.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from remotecv.result_store import BaseStore
 from remotecv.utils import logger, redis_client
 
 
 class ResultStore(BaseStore):
 
-    WEEK = 604800
     redis_instance = None
 
     def __init__(self, config):
         super().__init__(config)
 
         if not ResultStore.redis_instance:
             ResultStore.redis_instance = redis_client()
+
+        self.redis_key_expire_time = config.redis_key_expire_time
         self.storage = ResultStore.redis_instance
 
     def store(self, key, points):
         result = self.serialize(points)
         logger.debug("Points found: %s", result)
         redis_key = f"thumbor-detector-{key}"
-        self.storage.setex(
+        self.storage.set(
             name=redis_key,
             value=result,
-            time=2 * self.WEEK,
+            ex=self.redis_key_expire_time,
         )
```

### Comparing `remotecv-5.1.1/remotecv/unique_queue.py` & `remotecv-5.1.2/remotecv/unique_queue.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/utils.py` & `remotecv-5.1.2/remotecv/utils.py`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv/worker.py` & `remotecv-5.1.2/remotecv/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,21 @@
     envvar="REDIS_MODE",
     show_envvar=True,
     default=SINGLE_NODE,
     type=click.Choice([SINGLE_NODE, SENTINEL]),
     help="Redis mode",
 )
 @optgroup.option(
+    "--redis-key-expire-time",
+    envvar="REDIS_KEY_EXPIRE_TIME",
+    show_envvar=True,
+    default=1209600,
+    help="Redis key expiration time in seconds",
+)
+@optgroup.option(
     "--sentinel-instances",
     envvar="REDIS_SENTINEL_INSTANCES",
     show_envvar=True,
     default="localhost:26376",
     help="Redis Sentinel instances e.g. 'localhost:26376,localhost:26377'",
 )
 @optgroup.option(
@@ -289,14 +296,15 @@
 
     config.backend = params["backend"]
     config.redis_host = params["host"]
     config.redis_port = params["port"]
     config.redis_database = params["database"]
     config.redis_password = params["password"]
     config.redis_mode = params["redis_mode"]
+    config.redis_key_expire_time = params["redis_key_expire_time"]
     config.redis_sentinel_instances = params["sentinel_instances"]
     config.redis_sentinel_password = params["sentinel_password"]
     config.redis_sentinel_socket_timeout = params["socket_timeout"]
     config.redis_sentinel_master_instance = params["master_instance"]
     config.redis_sentinel_master_password = params["master_password"]
     config.redis_sentinel_master_database = params["master_database"]
```

### Comparing `remotecv-5.1.1/remotecv.egg-info/PKG-INFO` & `remotecv-5.1.2/remotecv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotecv
-Version: 5.1.1
+Version: 5.1.2
 Summary: remotecv is an OpenCV worker for facial and feature recognition
 Author: Bernardo Heynemann
 Author-email: heynemann@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `remotecv-5.1.1/remotecv.egg-info/SOURCES.txt` & `remotecv-5.1.2/remotecv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/remotecv.egg-info/requires.txt` & `remotecv-5.1.2/remotecv.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `remotecv-5.1.1/setup.py` & `remotecv-5.1.2/setup.py`

 * *Files identical despite different names*

