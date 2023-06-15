# Comparing `tmp/hyutils-hyutil-hoyun-lab-0.0.4.tar.gz` & `tmp/hyutils-hyutil-hoyun-lab-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.4.tar", last modified: Fri Jun  9 06:29:08 2023, max compression
+gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.5.tar", last modified: Thu Jun 15 01:28:23 2023, max compression
```

## Comparing `hyutils-hyutil-hoyun-lab-0.0.4.tar` & `hyutils-hyutil-hoyun-lab-0.0.5.tar`

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
+drwxrwxrwx   0        0        0        0 2023-06-15 01:28:23.645887 hyutils-hyutil-hoyun-lab-0.0.5/
+-rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      598 2023-06-15 01:28:23.645357 hyutils-hyutil-hoyun-lab-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.5/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-15 01:28:23.645887 hyutils-hyutil-hoyun-lab-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      850 2023-06-15 01:27:58.000000 hyutils-hyutil-hoyun-lab-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:28:23.621033 hyutils-hyutil-hoyun-lab-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-15 01:28:23.636888 hyutils-hyutil-hoyun-lab-0.0.5/src/hyutil_hoyun_lab/
+-rw-rw-rw-   0        0        0      345 2023-06-15 01:27:47.000000 hyutils-hyutil-hoyun-lab-0.0.5/src/hyutil_hoyun_lab/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.5/src/hyutil_hoyun_lab/appcontrol.py
+-rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.5/src/hyutil_hoyun_lab/date_time.py
+-rw-rw-rw-   0        0        0     1170 2023-06-15 01:27:01.000000 hyutils-hyutil-hoyun-lab-0.0.5/src/hyutil_hoyun_lab/dirjob.py
+-rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.5/src/hyutil_hoyun_lab/hashing.py
+-rw-rw-rw-   0        0        0    13711 2023-06-09 05:56:06.000000 hyutils-hyutil-hoyun-lab-0.0.5/src/hyutil_hoyun_lab/tfrecrod_utils.py
+-rw-rw-rw-   0        0        0     3842 2023-06-08 04:01:29.000000 hyutils-hyutil-hoyun-lab-0.0.5/src/hyutil_hoyun_lab/xml_util.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:28:23.643888 hyutils-hyutil-hoyun-lab-0.0.5/src/hyutils_hyutil_hoyun_lab.egg-info/
+-rw-rw-rw-   0        0        0      598 2023-06-15 01:28:23.000000 hyutils-hyutil-hoyun-lab-0.0.5/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-06-15 01:28:23.000000 hyutils-hyutil-hoyun-lab-0.0.5/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 01:28:23.000000 hyutils-hyutil-hoyun-lab-0.0.5/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-15 01:28:23.000000 hyutils-hyutil-hoyun-lab-0.0.5/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.4/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.4
+Version: 0.0.5
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.4/setup.py` & `hyutils-hyutil-hoyun-lab-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 
 setuptools.setup(
     name="hyutils-hyutil-hoyun-lab",
-    version="0.0.4",
+    version="0.0.5",
     url="https://www.hoyun.co.kr",
     license="MIT",
     author="nohgan im",
     author_email="fory2k@hoyun.co.kr",
     description="Hoyun Lab Python Utils",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/date_time.py` & `hyutils-hyutil-hoyun-lab-0.0.5/src/hyutil_hoyun_lab/date_time.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/dirjob.py` & `hyutils-hyutil-hoyun-lab-0.0.5/src/hyutil_hoyun_lab/dirjob.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,24 @@
 def files_ext(path, ext):
     for file in os.listdir(path):
         if os.path.isfile(os.path.join(path, file)):
             extension = os.path.splitext(file)[1]
             if extension == ext:
                 yield file
 
+def files_ext_sub(path, ext):
+    for file in os.listdir(path):
+        if os.path.isfile(os.path.join(path, file)):
+            extension = os.path.splitext(file)[1]
+            if extension == ext:
+                yield file
+
+        else:
+            files_ext_sub(os.path.join(path, file), ext)
+
 def dirs(path):
     for file in os.listdir(path):
         if os.path.isdir(os.path.join(path, file)):
             yield file
 
 def get_entry_count(path):
 	listing = os.listdir(path)
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/hashing.py` & `hyutils-hyutil-hoyun-lab-0.0.5/src/hyutil_hoyun_lab/hashing.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/tfrecrod_utils.py` & `hyutils-hyutil-hoyun-lab-0.0.5/src/hyutil_hoyun_lab/tfrecrod_utils.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.4/src/hyutil_hoyun_lab/xml_util.py` & `hyutils-hyutil-hoyun-lab-0.0.5/src/hyutil_hoyun_lab/xml_util.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.4/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.5/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.4
+Version: 0.0.5
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

