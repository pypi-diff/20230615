# Comparing `tmp/prelude-sdk-1.2.4.tar.gz` & `tmp/prelude-sdk-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-sdk-1.2.4.tar", last modified: Thu Jun  8 13:36:36 2023, max compression
+gzip compressed data, was "prelude-sdk-1.2.5.tar", last modified: Thu Jun 15 14:39:13 2023, max compression
```

## Comparing `prelude-sdk-1.2.4.tar` & `prelude-sdk-1.2.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-08 13:36:36.552817 prelude-sdk-1.2.4/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.2.4/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-06-08 13:36:36.552891 prelude-sdk-1.2.4/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.2.4/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-08 13:36:36.548054 prelude-sdk-1.2.4/prelude_sdk/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.4/prelude_sdk/__init__.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-08 13:36:36.550263 prelude-sdk-1.2.4/prelude_sdk/controllers/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.4/prelude_sdk/controllers/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2248 2023-06-06 22:22:58.000000 prelude-sdk-1.2.4/prelude_sdk/controllers/build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     5438 2023-06-06 22:22:58.000000 prelude-sdk-1.2.4/prelude_sdk/controllers/detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3711 2023-06-08 13:35:49.000000 prelude-sdk-1.2.4/prelude_sdk/controllers/iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     2057 2023-05-23 21:42:11.000000 prelude-sdk-1.2.4/prelude_sdk/controllers/partner_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      443 2023-05-03 13:30:52.000000 prelude-sdk-1.2.4/prelude_sdk/controllers/probe_controller.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-08 13:36:36.551000 prelude-sdk-1.2.4/prelude_sdk/models/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.4/prelude_sdk/models/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2816 2023-04-07 19:23:14.000000 prelude-sdk-1.2.4/prelude_sdk/models/account.py
--rw-r--r--   0 pack       (501) staff       (20)     2555 2023-05-22 15:57:51.000000 prelude-sdk-1.2.4/prelude_sdk/models/codes.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-08 13:36:36.548678 prelude-sdk-1.2.4/prelude_sdk.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-06-08 13:36:36.000000 prelude-sdk-1.2.4/prelude_sdk.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      773 2023-06-08 13:36:36.000000 prelude-sdk-1.2.4/prelude_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-06-08 13:36:36.000000 prelude-sdk-1.2.4/prelude_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)        9 2023-06-08 13:36:36.000000 prelude-sdk-1.2.4/prelude_sdk.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       18 2023-06-08 13:36:36.000000 prelude-sdk-1.2.4/prelude_sdk.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.2.4/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      532 2023-06-08 13:36:36.553367 prelude-sdk-1.2.4/setup.cfg
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-08 13:36:36.552479 prelude-sdk-1.2.4/tests/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.2.4/tests/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1097 2023-05-17 16:29:25.000000 prelude-sdk-1.2.4/tests/conftest.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-08 13:36:36.552713 prelude-sdk-1.2.4/tests/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.2.4/tests/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2075 2023-06-06 22:22:58.000000 prelude-sdk-1.2.4/tests/test_build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     5045 2023-06-06 22:22:58.000000 prelude-sdk-1.2.4/tests/test_detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3350 2023-06-07 19:10:37.000000 prelude-sdk-1.2.4/tests/test_iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-1.2.4/tests/test_probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-15 14:39:13.133209 prelude-sdk-1.2.5/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.2.5/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-06-15 14:39:13.133266 prelude-sdk-1.2.5/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.2.5/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-15 14:39:13.129296 prelude-sdk-1.2.5/prelude_sdk/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.5/prelude_sdk/__init__.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-15 14:39:13.131111 prelude-sdk-1.2.5/prelude_sdk/controllers/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.5/prelude_sdk/controllers/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2248 2023-06-06 22:22:58.000000 prelude-sdk-1.2.5/prelude_sdk/controllers/build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     5438 2023-06-06 22:22:58.000000 prelude-sdk-1.2.5/prelude_sdk/controllers/detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3711 2023-06-08 13:35:49.000000 prelude-sdk-1.2.5/prelude_sdk/controllers/iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     2057 2023-05-23 21:42:11.000000 prelude-sdk-1.2.5/prelude_sdk/controllers/partner_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      443 2023-05-03 13:30:52.000000 prelude-sdk-1.2.5/prelude_sdk/controllers/probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-15 14:39:13.131724 prelude-sdk-1.2.5/prelude_sdk/models/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.5/prelude_sdk/models/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2816 2023-04-07 19:23:14.000000 prelude-sdk-1.2.5/prelude_sdk/models/account.py
+-rw-r--r--   0 pack       (501) staff       (20)     2555 2023-05-22 15:57:51.000000 prelude-sdk-1.2.5/prelude_sdk/models/codes.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-15 14:39:13.129815 prelude-sdk-1.2.5/prelude_sdk.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-06-15 14:39:13.000000 prelude-sdk-1.2.5/prelude_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      773 2023-06-15 14:39:13.000000 prelude-sdk-1.2.5/prelude_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-06-15 14:39:13.000000 prelude-sdk-1.2.5/prelude_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)        9 2023-06-15 14:39:13.000000 prelude-sdk-1.2.5/prelude_sdk.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       18 2023-06-15 14:39:13.000000 prelude-sdk-1.2.5/prelude_sdk.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.2.5/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      532 2023-06-15 14:39:13.133490 prelude-sdk-1.2.5/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-15 14:39:13.132888 prelude-sdk-1.2.5/tests/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.2.5/tests/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1097 2023-05-17 16:29:25.000000 prelude-sdk-1.2.5/tests/conftest.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-15 14:39:13.133109 prelude-sdk-1.2.5/tests/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.2.5/tests/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2075 2023-06-06 22:22:58.000000 prelude-sdk-1.2.5/tests/test_build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     5045 2023-06-06 22:22:58.000000 prelude-sdk-1.2.5/tests/test_detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3350 2023-06-07 19:10:37.000000 prelude-sdk-1.2.5/tests/test_iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-1.2.5/tests/test_probe_controller.py
```

### Comparing `prelude-sdk-1.2.4/LICENSE` & `prelude-sdk-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.4/PKG-INFO` & `prelude-sdk-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.2.4
+Version: 1.2.5
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.2.4/README.md` & `prelude-sdk-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.4/prelude_sdk/controllers/build_controller.py` & `prelude-sdk-1.2.5/prelude_sdk/controllers/build_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.4/prelude_sdk/controllers/detect_controller.py` & `prelude-sdk-1.2.5/prelude_sdk/controllers/detect_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.4/prelude_sdk/controllers/iam_controller.py` & `prelude-sdk-1.2.5/prelude_sdk/controllers/iam_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.4/prelude_sdk/controllers/partner_controller.py` & `prelude-sdk-1.2.5/prelude_sdk/controllers/partner_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.4/prelude_sdk/models/account.py` & `prelude-sdk-1.2.5/prelude_sdk/models/account.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.4/prelude_sdk/models/codes.py` & `prelude-sdk-1.2.5/prelude_sdk/models/codes.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.4/prelude_sdk.egg-info/PKG-INFO` & `prelude-sdk-1.2.5/prelude_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.2.4
+Version: 1.2.5
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.2.4/prelude_sdk.egg-info/SOURCES.txt` & `prelude-sdk-1.2.5/prelude_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.4/setup.cfg` & `prelude-sdk-1.2.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-sdk
-version = 1.2.4
+version = 1.2.5
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers =
```

### Comparing `prelude-sdk-1.2.4/tests/conftest.py` & `prelude-sdk-1.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.4/tests/test_build_controller.py` & `prelude-sdk-1.2.5/tests/test_build_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.4/tests/test_detect_controller.py` & `prelude-sdk-1.2.5/tests/test_detect_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.4/tests/test_iam_controller.py` & `prelude-sdk-1.2.5/tests/test_iam_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.4/tests/test_probe_controller.py` & `prelude-sdk-1.2.5/tests/test_probe_controller.py`

 * *Files identical despite different names*

