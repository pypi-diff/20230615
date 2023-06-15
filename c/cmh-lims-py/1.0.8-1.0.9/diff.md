# Comparing `tmp/cmh_lims_py-1.0.8.tar.gz` & `tmp/cmh_lims_py-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmh_lims_py-1.0.8.tar", last modified: Wed Jun 14 21:00:08 2023, max compression
+gzip compressed data, was "cmh_lims_py-1.0.9.tar", last modified: Wed Jun 14 21:04:57 2023, max compression
```

## Comparing `cmh_lims_py-1.0.8.tar` & `cmh_lims_py-1.0.9.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 mkumar1  (574770668) 838579111        0 2023-06-14 21:00:08.236126 cmh_lims_py-1.0.8/
--rw-r--r--   0 mkumar1  (574770668) 838579111        0 2023-06-06 21:06:48.000000 cmh_lims_py-1.0.8/LICENSE.txt
--rw-r--r--   0 mkumar1  (574770668) 838579111      582 2023-06-14 21:00:08.235841 cmh_lims_py-1.0.8/PKG-INFO
--rw-r--r--   0 mkumar1  (574770668) 838579111      242 2023-06-13 04:14:46.000000 cmh_lims_py-1.0.8/README.md
-drwxr-xr-x   0 mkumar1  (574770668) 838579111        0 2023-06-14 21:00:08.228993 cmh_lims_py-1.0.8/cmh_lims_py.egg-info/
--rw-r--r--   0 mkumar1  (574770668) 838579111      582 2023-06-14 21:00:08.000000 cmh_lims_py-1.0.8/cmh_lims_py.egg-info/PKG-INFO
--rw-r--r--   0 mkumar1  (574770668) 838579111      504 2023-06-14 21:00:08.000000 cmh_lims_py-1.0.8/cmh_lims_py.egg-info/SOURCES.txt
--rw-r--r--   0 mkumar1  (574770668) 838579111        1 2023-06-14 21:00:08.000000 cmh_lims_py-1.0.8/cmh_lims_py.egg-info/dependency_links.txt
--rw-r--r--   0 mkumar1  (574770668) 838579111       22 2023-06-14 21:00:08.000000 cmh_lims_py-1.0.8/cmh_lims_py.egg-info/requires.txt
--rw-r--r--   0 mkumar1  (574770668) 838579111       14 2023-06-14 21:00:08.000000 cmh_lims_py-1.0.8/cmh_lims_py.egg-info/top_level.txt
-drwxr-xr-x   0 mkumar1  (574770668) 838579111        0 2023-06-14 21:00:08.232362 cmh_lims_py-1.0.8/cmhlims/
--rw-r--r--   0 mkumar1  (574770668) 838579111        0 2023-06-13 01:51:34.000000 cmh_lims_py-1.0.8/cmhlims/__init__.py
--rw-r--r--   0 mkumar1  (574770668) 838579111     1614 2023-06-14 20:53:10.000000 cmh_lims_py-1.0.8/cmhlims/connectToLIMS.py
--rw-r--r--   0 mkumar1  (574770668) 838579111     2422 2023-06-14 20:56:37.000000 cmh_lims_py-1.0.8/cmhlims/getAnalysis.py
--rw-r--r--   0 mkumar1  (574770668) 838579111     1746 2023-06-14 20:57:55.000000 cmh_lims_py-1.0.8/cmhlims/getAnalysisFiles.py
--rw-r--r--   0 mkumar1  (574770668) 838579111      701 2023-06-14 20:59:57.000000 cmh_lims_py-1.0.8/cmhlims/getSampleNames.py
--rw-r--r--   0 mkumar1  (574770668) 838579111      958 2023-06-14 20:36:42.000000 cmh_lims_py-1.0.8/cmhlims/set_config.py
--rw-r--r--   0 mkumar1  (574770668) 838579111      520 2023-06-14 19:54:03.000000 cmh_lims_py-1.0.8/cmhlims/set_variable.py
--rw-r--r--   0 mkumar1  (574770668) 838579111       38 2023-06-14 21:00:08.236239 cmh_lims_py-1.0.8/setup.cfg
--rw-r--r--   0 mkumar1  (574770668) 838579111      743 2023-06-14 20:54:51.000000 cmh_lims_py-1.0.8/setup.py
-drwxr-xr-x   0 mkumar1  (574770668) 838579111        0 2023-06-14 21:00:08.234969 cmh_lims_py-1.0.8/tests/
--rw-r--r--   0 mkumar1  (574770668) 838579111        0 2023-06-13 02:48:46.000000 cmh_lims_py-1.0.8/tests/__init__.py
--rw-r--r--   0 mkumar1  (574770668) 838579111     3414 2023-06-13 04:40:13.000000 cmh_lims_py-1.0.8/tests/test_connectToLIMS.py
--rw-r--r--   0 mkumar1  (574770668) 838579111     3062 2023-06-06 22:08:19.000000 cmh_lims_py-1.0.8/tests/test_getAnalysis.py
--rw-r--r--   0 mkumar1  (574770668) 838579111     2763 2023-06-06 22:08:40.000000 cmh_lims_py-1.0.8/tests/test_getAnalysisFiles.py
--rw-r--r--   0 mkumar1  (574770668) 838579111     1974 2023-06-13 04:47:07.000000 cmh_lims_py-1.0.8/tests/test_getSampleNames.py
+drwxr-xr-x   0 mkumar1  (574770668) 838579111        0 2023-06-14 21:04:57.335799 cmh_lims_py-1.0.9/
+-rw-r--r--   0 mkumar1  (574770668) 838579111        0 2023-06-06 21:06:48.000000 cmh_lims_py-1.0.9/LICENSE.txt
+-rw-r--r--   0 mkumar1  (574770668) 838579111      582 2023-06-14 21:04:57.335526 cmh_lims_py-1.0.9/PKG-INFO
+-rw-r--r--   0 mkumar1  (574770668) 838579111      242 2023-06-13 04:14:46.000000 cmh_lims_py-1.0.9/README.md
+drwxr-xr-x   0 mkumar1  (574770668) 838579111        0 2023-06-14 21:04:57.327938 cmh_lims_py-1.0.9/cmh_lims_py.egg-info/
+-rw-r--r--   0 mkumar1  (574770668) 838579111      582 2023-06-14 21:04:57.000000 cmh_lims_py-1.0.9/cmh_lims_py.egg-info/PKG-INFO
+-rw-r--r--   0 mkumar1  (574770668) 838579111      479 2023-06-14 21:04:57.000000 cmh_lims_py-1.0.9/cmh_lims_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mkumar1  (574770668) 838579111        1 2023-06-14 21:04:57.000000 cmh_lims_py-1.0.9/cmh_lims_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mkumar1  (574770668) 838579111       22 2023-06-14 21:04:57.000000 cmh_lims_py-1.0.9/cmh_lims_py.egg-info/requires.txt
+-rw-r--r--   0 mkumar1  (574770668) 838579111       14 2023-06-14 21:04:57.000000 cmh_lims_py-1.0.9/cmh_lims_py.egg-info/top_level.txt
+drwxr-xr-x   0 mkumar1  (574770668) 838579111        0 2023-06-14 21:04:57.331932 cmh_lims_py-1.0.9/cmhlims/
+-rw-r--r--   0 mkumar1  (574770668) 838579111        0 2023-06-13 01:51:34.000000 cmh_lims_py-1.0.9/cmhlims/__init__.py
+-rw-r--r--   0 mkumar1  (574770668) 838579111     1524 2023-06-14 21:02:45.000000 cmh_lims_py-1.0.9/cmhlims/connectToLIMS.py
+-rw-r--r--   0 mkumar1  (574770668) 838579111     2422 2023-06-14 20:56:37.000000 cmh_lims_py-1.0.9/cmhlims/getAnalysis.py
+-rw-r--r--   0 mkumar1  (574770668) 838579111     1746 2023-06-14 20:57:55.000000 cmh_lims_py-1.0.9/cmhlims/getAnalysisFiles.py
+-rw-r--r--   0 mkumar1  (574770668) 838579111      701 2023-06-14 20:59:57.000000 cmh_lims_py-1.0.9/cmhlims/getSampleNames.py
+-rw-r--r--   0 mkumar1  (574770668) 838579111      958 2023-06-14 20:36:42.000000 cmh_lims_py-1.0.9/cmhlims/setConfig.py
+-rw-r--r--   0 mkumar1  (574770668) 838579111       38 2023-06-14 21:04:57.335914 cmh_lims_py-1.0.9/setup.cfg
+-rw-r--r--   0 mkumar1  (574770668) 838579111      743 2023-06-14 21:04:15.000000 cmh_lims_py-1.0.9/setup.py
+drwxr-xr-x   0 mkumar1  (574770668) 838579111        0 2023-06-14 21:04:57.334730 cmh_lims_py-1.0.9/tests/
+-rw-r--r--   0 mkumar1  (574770668) 838579111        0 2023-06-13 02:48:46.000000 cmh_lims_py-1.0.9/tests/__init__.py
+-rw-r--r--   0 mkumar1  (574770668) 838579111     3414 2023-06-13 04:40:13.000000 cmh_lims_py-1.0.9/tests/test_connectToLIMS.py
+-rw-r--r--   0 mkumar1  (574770668) 838579111     3062 2023-06-06 22:08:19.000000 cmh_lims_py-1.0.9/tests/test_getAnalysis.py
+-rw-r--r--   0 mkumar1  (574770668) 838579111     2763 2023-06-06 22:08:40.000000 cmh_lims_py-1.0.9/tests/test_getAnalysisFiles.py
+-rw-r--r--   0 mkumar1  (574770668) 838579111     1974 2023-06-13 04:47:07.000000 cmh_lims_py-1.0.9/tests/test_getSampleNames.py
```

### Comparing `cmh_lims_py-1.0.8/PKG-INFO` & `cmh_lims_py-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmh_lims_py
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python module for basic querying of LIMS samples, analyses, and analysis files
 Home-page: https://dev.azure.com/CMHResearchIS/GMC/_git/cmhlims_py
 Author: Manish Kumar
 Author-email: mkumar1@cmh.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cmh_lims_py-1.0.8/cmh_lims_py.egg-info/PKG-INFO` & `cmh_lims_py-1.0.9/cmh_lims_py.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmh-lims-py
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python module for basic querying of LIMS samples, analyses, and analysis files
 Home-page: https://dev.azure.com/CMHResearchIS/GMC/_git/cmhlims_py
 Author: Manish Kumar
 Author-email: mkumar1@cmh.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cmh_lims_py-1.0.8/cmhlims/connectToLIMS.py` & `cmh_lims_py-1.0.9/cmhlims/connectToLIMS.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 import yaml
 import pymysql
-import os
-import set_config as sc
 import configparser
 
 
 def connect_to_lims(config=None, environment=None):
     config = configparser.ConfigParser()
     config.read('config.ini')
 
     config_file = config.get('shared', 'config_file')
     environment = config.get('shared', 'environment')
+
+    '''
     print("------------------")
     print(config_file)
     print(environment)
     print("------------------")
+    '''
+
     if config_file is None or environment is None:
         raise ValueError("Options cmhlims.lims_config_yaml and cmhlims.lims_environment must be set before using cmhlims functions.")
 
     with open(config_file, 'r') as file:
         lims_config = yaml.safe_load(file)
-    print(lims_config)
+
     if environment not in lims_config:
         raise ValueError("LIMS environment not found in configuration YAML: " + environment)
 
     lims_config = lims_config[environment]
-    #print(lims_config['username'])
+
     db_con = pymysql.connect(
         user=lims_config['username'],
         password=lims_config['password'],
         host=lims_config['host'],
         database=lims_config['database'],
         ssl_ca=lims_config['sslca'],
         autocommit=True
     )
-    print(db_con)
+
     '''
     cur = db_con.cursor()
     sql = 'SELECT * FROM samples LIMIT 10'
     cur.execute(sql)
     results = cur.fetchall()
     db_con.close()
```

### Comparing `cmh_lims_py-1.0.8/cmhlims/getAnalysis.py` & `cmh_lims_py-1.0.9/cmhlims/getAnalysis.py`

 * *Files identical despite different names*

### Comparing `cmh_lims_py-1.0.8/cmhlims/getAnalysisFiles.py` & `cmh_lims_py-1.0.9/cmhlims/getAnalysisFiles.py`

 * *Files identical despite different names*

### Comparing `cmh_lims_py-1.0.8/cmhlims/getSampleNames.py` & `cmh_lims_py-1.0.9/cmhlims/getSampleNames.py`

 * *Files identical despite different names*

### Comparing `cmh_lims_py-1.0.8/cmhlims/set_config.py` & `cmh_lims_py-1.0.9/cmhlims/setConfig.py`

 * *Files identical despite different names*

### Comparing `cmh_lims_py-1.0.8/setup.py` & `cmh_lims_py-1.0.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cmh_lims_py',
-    version='1.0.8',
+    version='1.0.9',
     packages=find_packages(),
     include_package_data=True,
     author='Manish Kumar',
     author_email='mkumar1@cmh.edu',
     description='Python module for basic querying of LIMS samples, analyses, and analysis files',
     url='https://dev.azure.com/CMHResearchIS/GMC/_git/cmhlims_py',
     install_requires=[
```

### Comparing `cmh_lims_py-1.0.8/tests/test_connectToLIMS.py` & `cmh_lims_py-1.0.9/tests/test_connectToLIMS.py`

 * *Files identical despite different names*

### Comparing `cmh_lims_py-1.0.8/tests/test_getAnalysis.py` & `cmh_lims_py-1.0.9/tests/test_getAnalysis.py`

 * *Files identical despite different names*

### Comparing `cmh_lims_py-1.0.8/tests/test_getAnalysisFiles.py` & `cmh_lims_py-1.0.9/tests/test_getAnalysisFiles.py`

 * *Files identical despite different names*

### Comparing `cmh_lims_py-1.0.8/tests/test_getSampleNames.py` & `cmh_lims_py-1.0.9/tests/test_getSampleNames.py`

 * *Files identical despite different names*

