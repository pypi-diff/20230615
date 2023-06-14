# Comparing `tmp/persian-gender-detection-1.1.0.tar.gz` & `tmp/persian-gender-detection-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "persian-gender-detection-1.1.0.tar", last modified: Wed Jun 14 06:13:03 2023, max compression
+gzip compressed data, was "persian-gender-detection-1.2.1.tar", last modified: Wed Jun 14 22:39:38 2023, max compression
```

## Comparing `persian-gender-detection-1.1.0.tar` & `persian-gender-detection-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-14 06:13:03.499870 persian-gender-detection-1.1.0/
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1068 2023-06-07 16:19:28.000000 persian-gender-detection-1.1.0/LICENSE
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     2251 2023-06-14 06:13:03.499870 persian-gender-detection-1.1.0/PKG-INFO
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)      932 2023-06-12 09:45:11.000000 persian-gender-detection-1.1.0/README.md
-drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-14 06:13:03.483870 persian-gender-detection-1.1.0/persian_gender_detection/
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       40 2023-06-07 16:13:42.000000 persian-gender-detection-1.1.0/persian_gender_detection/__init__.py
-drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-14 06:13:03.495870 persian-gender-detection-1.1.0/persian_gender_detection/gender/
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)   410371 2023-06-08 06:15:17.000000 persian-gender-detection-1.1.0/persian_gender_detection/gender/iranianNamesDataset.csv
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)   436494 2023-06-12 09:12:51.000000 persian-gender-detection-1.1.0/persian_gender_detection/gender/iranianNamesDataset.py
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)      923 2023-06-12 09:38:15.000000 persian-gender-detection-1.1.0/persian_gender_detection/persian_gender_detection.py
-drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-14 06:13:03.487870 persian-gender-detection-1.1.0/persian_gender_detection.egg-info/
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     2251 2023-06-14 06:13:03.000000 persian-gender-detection-1.1.0/persian_gender_detection.egg-info/PKG-INFO
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)      467 2023-06-14 06:13:03.000000 persian-gender-detection-1.1.0/persian_gender_detection.egg-info/SOURCES.txt
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)        1 2023-06-14 06:13:03.000000 persian-gender-detection-1.1.0/persian_gender_detection.egg-info/dependency_links.txt
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       25 2023-06-14 06:13:03.000000 persian-gender-detection-1.1.0/persian_gender_detection.egg-info/top_level.txt
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       38 2023-06-14 06:13:03.499870 persian-gender-detection-1.1.0/setup.cfg
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1732 2023-06-14 06:12:52.000000 persian-gender-detection-1.1.0/setup.py
-drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-14 06:13:03.499870 persian-gender-detection-1.1.0/test/
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1438 2023-06-07 16:03:13.000000 persian-gender-detection-1.1.0/test/test_clean_name.py
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1940 2023-06-12 09:31:58.000000 persian-gender-detection-1.1.0/test/test_get_gender.py
+drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-14 22:39:38.566149 persian-gender-detection-1.2.1/
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1068 2023-06-07 16:19:28.000000 persian-gender-detection-1.2.1/LICENSE
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     2890 2023-06-14 22:39:38.566149 persian-gender-detection-1.2.1/PKG-INFO
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1571 2023-06-14 22:38:45.000000 persian-gender-detection-1.2.1/README.md
+drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-14 22:39:38.562149 persian-gender-detection-1.2.1/persian_gender_detection/
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       40 2023-06-07 16:13:42.000000 persian-gender-detection-1.2.1/persian_gender_detection/__init__.py
+drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-14 22:39:38.562149 persian-gender-detection-1.2.1/persian_gender_detection/gender/
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)   410371 2023-06-08 06:15:17.000000 persian-gender-detection-1.2.1/persian_gender_detection/gender/iranianNamesDataset.csv
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)   436494 2023-06-12 09:12:51.000000 persian-gender-detection-1.2.1/persian_gender_detection/gender/iranianNamesDataset.py
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1108 2023-06-14 22:31:58.000000 persian-gender-detection-1.2.1/persian_gender_detection/persian_gender_detection.py
+drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-14 22:39:38.562149 persian-gender-detection-1.2.1/persian_gender_detection.egg-info/
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     2890 2023-06-14 22:39:38.000000 persian-gender-detection-1.2.1/persian_gender_detection.egg-info/PKG-INFO
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)      467 2023-06-14 22:39:38.000000 persian-gender-detection-1.2.1/persian_gender_detection.egg-info/SOURCES.txt
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)        1 2023-06-14 22:39:38.000000 persian-gender-detection-1.2.1/persian_gender_detection.egg-info/dependency_links.txt
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       25 2023-06-14 22:39:38.000000 persian-gender-detection-1.2.1/persian_gender_detection.egg-info/top_level.txt
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       38 2023-06-14 22:39:38.566149 persian-gender-detection-1.2.1/setup.cfg
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1732 2023-06-14 22:33:09.000000 persian-gender-detection-1.2.1/setup.py
+drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-14 22:39:38.566149 persian-gender-detection-1.2.1/test/
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1438 2023-06-07 16:03:13.000000 persian-gender-detection-1.2.1/test/test_clean_name.py
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     2119 2023-06-14 22:37:51.000000 persian-gender-detection-1.2.1/test/test_get_gender.py
```

### Comparing `persian-gender-detection-1.1.0/LICENSE` & `persian-gender-detection-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `persian-gender-detection-1.1.0/PKG-INFO` & `persian-gender-detection-1.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persian-gender-detection
-Version: 1.1.0
+Version: 1.2.1
 Summary: A simple python package to detect gender by Persian first name. (With more than 19K names).
 Home-page: https://github.com/zeoses/persian-gender-detection
 Author: Mehraban
 License: MIT License
 Project-URL: Source, https://github.com/zeoses/persian-gender-detection
 Project-URL: Documentation, https://github.com/zeoses/persian-gender-detection
 Keywords: persian-gender-detection,farsi gender,iranian gender,name gender,persian gender detection,gender detection
@@ -46,15 +46,33 @@
 
 # Detect gender
 get_gender('  عــــلی  ')         # MALE
 get_gender('نرگـــ😉ــس')         # FEMALE
 get_gender('حســ😎ــن')           # MALE
 get_gender('۱۲۳۹۹۳محمدعلی123')    # MALE
 get_gender('۱۲۳مهناز۱۲۳')         # FEMALE
+get_gender('فاطمه زهرا')          # UNKNOWN
+get_gender('فاطمه زهرا', 
+          find_nearest_name=True) # (FEMALE, 'فاطمه')
+get_gender('محمدنیسنممدیتیس', 
+          find_nearest_name=True) # ('MALE', 'محمد')
+
 ```
+Changelog
+------
+1.2.1
+* Fixed issues in two-part names and added find_nearst_name flag to find and return the nearest name. 
+
+1.1.0  
+* Increasing the dataset of names from 6k to 19k
+* convert names dataset from JSON to Python dictionary
+* If a name does not exist in the dataset, it finds the gender in two-part names using the first part.  
+
+1.0.5
+* First version with 6k name dataset
 
 Issues
 ------
 
 Feel free to submit issues and enhancement requests.
 
 Contributing
```

### Comparing `persian-gender-detection-1.1.0/persian_gender_detection/gender/iranianNamesDataset.csv` & `persian-gender-detection-1.2.1/persian_gender_detection/gender/iranianNamesDataset.csv`

 * *Files identical despite different names*

### Comparing `persian-gender-detection-1.1.0/persian_gender_detection/gender/iranianNamesDataset.py` & `persian-gender-detection-1.2.1/persian_gender_detection/gender/iranianNamesDataset.py`

 * *Files identical despite different names*

### Comparing `persian-gender-detection-1.1.0/persian_gender_detection.egg-info/PKG-INFO` & `persian-gender-detection-1.2.1/persian_gender_detection.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persian-gender-detection
-Version: 1.1.0
+Version: 1.2.1
 Summary: A simple python package to detect gender by Persian first name. (With more than 19K names).
 Home-page: https://github.com/zeoses/persian-gender-detection
 Author: Mehraban
 License: MIT License
 Project-URL: Source, https://github.com/zeoses/persian-gender-detection
 Project-URL: Documentation, https://github.com/zeoses/persian-gender-detection
 Keywords: persian-gender-detection,farsi gender,iranian gender,name gender,persian gender detection,gender detection
@@ -46,15 +46,33 @@
 
 # Detect gender
 get_gender('  عــــلی  ')         # MALE
 get_gender('نرگـــ😉ــس')         # FEMALE
 get_gender('حســ😎ــن')           # MALE
 get_gender('۱۲۳۹۹۳محمدعلی123')    # MALE
 get_gender('۱۲۳مهناز۱۲۳')         # FEMALE
+get_gender('فاطمه زهرا')          # UNKNOWN
+get_gender('فاطمه زهرا', 
+          find_nearest_name=True) # (FEMALE, 'فاطمه')
+get_gender('محمدنیسنممدیتیس', 
+          find_nearest_name=True) # ('MALE', 'محمد')
+
 ```
+Changelog
+------
+1.2.1
+* Fixed issues in two-part names and added find_nearst_name flag to find and return the nearest name. 
+
+1.1.0  
+* Increasing the dataset of names from 6k to 19k
+* convert names dataset from JSON to Python dictionary
+* If a name does not exist in the dataset, it finds the gender in two-part names using the first part.  
+
+1.0.5
+* First version with 6k name dataset
 
 Issues
 ------
 
 Feel free to submit issues and enhancement requests.
 
 Contributing
```

### Comparing `persian-gender-detection-1.1.0/setup.py` & `persian-gender-detection-1.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('./README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='persian-gender-detection',
-    version='1.1.0',
+    version='1.2.1',
     packages=['persian_gender_detection'],
     include_package_data=True,
     data_files=[('', [
         'persian_gender_detection/gender/iranianNamesDataset.py',
         'persian_gender_detection/gender/iranianNamesDataset.csv',
     ])],
     url='https://github.com/zeoses/persian-gender-detection',
```

### Comparing `persian-gender-detection-1.1.0/test/test_clean_name.py` & `persian-gender-detection-1.2.1/test/test_clean_name.py`

 * *Files identical despite different names*

### Comparing `persian-gender-detection-1.1.0/test/test_get_gender.py` & `persian-gender-detection-1.2.1/test/test_get_gender.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import unittest
 from persian_gender_detection.persian_gender_detection import get_gender
 
 
 class TestCleanName(unittest.TestCase):
 
     def test_detect_male(self):
-        self.assertEqual(get_gender('محمدمسیحا'), 'MALE')
+        self.assertEqual(get_gender('محمدمسیحا', True), ('MALE', 'محمد'))
+        self.assertEqual(get_gender('محمدنیسنممدیتیس', True), ('MALE', 'محمد'))
         self.assertEqual(get_gender('علي'), 'MALE')
         self.assertEqual(get_gender('مسیحا'), 'MALE')
         self.assertEqual(get_gender('سعید     '), 'MALE')
         self.assertEqual(get_gender('هــــادی'), 'MALE')
         self.assertEqual(get_gender('محمد   رضا'), 'MALE')
         self.assertEqual(get_gender('احسا   ن'), 'MALE')
         self.assertEqual(get_gender('كامران'), 'MALE')
         self.assertEqual(get_gender('  پیمـــان  '), 'MALE')
-        self.assertEqual(get_gender('حســ😎ــن'), 'MALE')
+        self.assertEqual(get_gender('حســ😎ــن', True), ('MALE', 'حسن'))
         self.assertEqual(get_gender('۱۲۳۹۹۳محمدعلی123'), 'MALE')
         self.assertEqual(get_gender('<<محمد>>'), 'MALE')
 
     def test_detect_female(self):
         self.assertEqual(get_gender('فاطمه'), 'FEMALE')
         self.assertEqual(get_gender('آذر     '), 'FEMALE')
         self.assertEqual(get_gender('الـــناز'), 'FEMALE')
-        self.assertEqual(get_gender('فاطمه زهرا'), 'FEMALE')
+        self.assertEqual(get_gender('فاطمه زهرا', True), ('FEMALE', "فاطمه"))
         self.assertEqual(get_gender('یلـــ❤️ــدا'), 'FEMALE')
         self.assertEqual(get_gender('  مریم  '), 'FEMALE')
         self.assertEqual(get_gender('صغری'), 'FEMALE')
         self.assertEqual(get_gender('حانیه'), 'FEMALE')
-        self.assertEqual(get_gender('جانان'), 'FEMALE')
+        self.assertEqual(get_gender('جانان', True), ('FEMALE', 'جانا'))
         self.assertEqual(get_gender('۱۲۳مهناز۱۲۳'), 'FEMALE')
         self.assertEqual(get_gender('فاطی'), 'FEMALE')
 
 
     def test_detect_unkown(self):
         self.assertEqual(get_gender('(فاطمه)'), 'UNKNOWN')
         self.assertEqual(get_gender('fateme'), 'UNKNOWN')
```

