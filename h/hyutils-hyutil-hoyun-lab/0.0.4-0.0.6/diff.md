# Comparing `tmp/hyutils-hyutil-hoyun-lab-0.0.4.tar.gz` & `tmp/hyutils-hyutil-hoyun-lab-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.4.tar", last modified: Fri Jun  9 06:29:08 2023, max compression
+gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.6.tar", last modified: Thu Jun 15 02:11:46 2023, max compression
```

## Comparing `hyutils-hyutil-hoyun-lab-0.0.4.tar` & `hyutils-hyutil-hoyun-lab-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 06:29:08.969145 hyutils-hyutil-hoyun-lab-0.0.4/
--rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      598 2023-06-09 06:29:08.968047 hyutils-hyutil-hoyun-lab-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.4/README.md
--rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 06:29:08.969464 hyutils-hyutil-hoyun-lab-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      850 2023-06-09 06:28:21.000000 hyutils-hyutil-hoyun-lab-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:29:08.926258 hyutils-hyutil-hoyun-lab-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 06:29:08.954029 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/
--rw-rw-rw-   0        0        0      345 2023-06-09 06:28:05.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/__init__.py
--rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/appcontrol.py
--rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/date_time.py
--rw-rw-rw-   0        0        0      860 2023-06-07 07:24:26.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/dirjob.py
--rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/hashing.py
--rw-rw-rw-   0        0        0    13711 2023-06-09 05:56:06.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/tfrecrod_utils.py
--rw-rw-rw-   0        0        0     3842 2023-06-08 04:01:29.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/xml_util.py
-drwxrwxrwx   0        0        0        0 2023-06-09 06:29:08.965491 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutils_hyutil_hoyun_lab.egg-info/
--rw-rw-rw-   0        0        0      598 2023-06-09 06:29:08.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-06-09 06:29:08.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 06:29:08.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-09 06:29:08.000000 hyutils-hyutil-hoyun-lab-0.0.4/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 02:11:46.138114 hyutils-hyutil-hoyun-lab-0.0.6/
+-rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      598 2023-06-15 02:11:46.137415 hyutils-hyutil-hoyun-lab-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.6/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-15 02:11:46.138373 hyutils-hyutil-hoyun-lab-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      850 2023-06-15 02:11:17.000000 hyutils-hyutil-hoyun-lab-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:11:46.113129 hyutils-hyutil-hoyun-lab-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-15 02:11:46.129974 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/
+-rw-rw-rw-   0        0        0      345 2023-06-15 02:11:17.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/appcontrol.py
+-rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/date_time.py
+-rw-rw-rw-   0        0        0     1155 2023-06-15 01:43:34.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/dirjob.py
+-rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/hashing.py
+-rw-rw-rw-   0        0        0    13711 2023-06-09 05:56:06.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/tfrecrod_utils.py
+-rw-rw-rw-   0        0        0     3842 2023-06-08 04:01:29.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/xml_util.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:11:46.135135 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutils_hyutil_hoyun_lab.egg-info/
+-rw-rw-rw-   0        0        0      598 2023-06-15 02:11:46.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-06-15 02:11:46.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 02:11:46.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-15 02:11:46.000000 hyutils-hyutil-hoyun-lab-0.0.6/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.4/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.4
+Version: 0.0.6
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.4/setup.py` & `hyutils-hyutil-hoyun-lab-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 
 setuptools.setup(
     name="hyutils-hyutil-hoyun-lab",
-    version="0.0.4",
+    version="0.0.6",
     url="https://www.hoyun.co.kr",
     license="MIT",
     author="nohgan im",
     author_email="fory2k@hoyun.co.kr",
     description="Hoyun Lab Python Utils",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/date_time.py` & `hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/date_time.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/hashing.py` & `hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/hashing.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/tfrecrod_utils.py` & `hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/tfrecrod_utils.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/xml_util.py` & `hyutils-hyutil-hoyun-lab-0.0.6/src/hyutil_hoyun_lab/xml_util.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.4/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.6/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.4
+Version: 0.0.6
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

