# Comparing `tmp/beau-ssi-converter-0.3.0.tar.gz` & `tmp/beau-ssi-converter-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beau-ssi-converter-0.3.0.tar", last modified: Mon Oct 24 04:48:16 2022, max compression
+gzip compressed data, was "beau-ssi-converter-0.4.0.tar", last modified: Thu Jun 15 07:37:22 2023, max compression
```

## Comparing `beau-ssi-converter-0.3.0.tar` & `beau-ssi-converter-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 04:48:16.158235 beau-ssi-converter-0.3.0/
--rw-r--r--   0 root         (0) root         (0)     1066 2022-10-24 04:48:13.000000 beau-ssi-converter-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      980 2022-10-24 04:48:16.158235 beau-ssi-converter-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      383 2022-10-24 04:48:13.000000 beau-ssi-converter-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 04:48:16.158235 beau-ssi-converter-0.3.0/beau_ssi_converter.egg-info/
--rw-r--r--   0 root         (0) root         (0)      980 2022-10-24 04:48:16.000000 beau-ssi-converter-0.3.0/beau_ssi_converter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      204 2022-10-24 04:48:16.000000 beau-ssi-converter-0.3.0/beau_ssi_converter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-24 04:48:16.000000 beau-ssi-converter-0.3.0/beau_ssi_converter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-24 04:48:16.000000 beau-ssi-converter-0.3.0/beau_ssi_converter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      143 2022-10-24 04:48:16.158235 beau-ssi-converter-0.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      999 2022-10-24 04:48:13.000000 beau-ssi-converter-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 07:37:22.385538 beau-ssi-converter-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-06-15 07:37:19.000000 beau-ssi-converter-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      964 2023-06-15 07:37:22.385538 beau-ssi-converter-0.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      387 2023-06-15 07:37:19.000000 beau-ssi-converter-0.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 07:37:22.385538 beau-ssi-converter-0.4.0/beau_ssi_converter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      964 2023-06-15 07:37:22.000000 beau-ssi-converter-0.4.0/beau_ssi_converter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-15 07:37:22.000000 beau-ssi-converter-0.4.0/beau_ssi_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 07:37:22.000000 beau-ssi-converter-0.4.0/beau_ssi_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-15 07:37:22.000000 beau-ssi-converter-0.4.0/beau_ssi_converter.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 07:37:22.385538 beau-ssi-converter-0.4.0/converter/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-15 07:37:20.000000 beau-ssi-converter-0.4.0/converter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      301 2023-06-15 07:37:19.000000 beau-ssi-converter-0.4.0/converter/main.py
+-rw-r--r--   0 root         (0) root         (0)      143 2023-06-15 07:37:22.385538 beau-ssi-converter-0.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      999 2023-06-15 07:37:19.000000 beau-ssi-converter-0.4.0/setup.py
```

### Comparing `beau-ssi-converter-0.3.0/LICENSE` & `beau-ssi-converter-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beau-ssi-converter-0.3.0/PKG-INFO` & `beau-ssi-converter-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: beau-ssi-converter
-Version: 0.3.0
+Version: 0.4.0
 Summary: Automatic Semantic Versioning for Python projects
 Home-page: http://github.com/thuongnn/github-actions-learning-python
 Author: Nguyen Nhu Thuong
 Author-email: thuongnn@ssi.com.vn
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 
 # Converter
+abc
 
 Convert XML to JSON
 
 ### prerequisite
 - you need to install below library using pip
 - $ pip install xmltodict
  
@@ -33,9 +33,7 @@
 - The Output will be shown below as output.json
 
 ## *Author Name*
 Azhad Ghufran
 
 
 # Testing
-
-
```

### Comparing `beau-ssi-converter-0.3.0/beau_ssi_converter.egg-info/PKG-INFO` & `beau-ssi-converter-0.4.0/beau_ssi_converter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: beau-ssi-converter
-Version: 0.3.0
+Version: 0.4.0
 Summary: Automatic Semantic Versioning for Python projects
 Home-page: http://github.com/thuongnn/github-actions-learning-python
 Author: Nguyen Nhu Thuong
 Author-email: thuongnn@ssi.com.vn
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 
 # Converter
+abc
 
 Convert XML to JSON
 
 ### prerequisite
 - you need to install below library using pip
 - $ pip install xmltodict
  
@@ -33,9 +33,7 @@
 - The Output will be shown below as output.json
 
 ## *Author Name*
 Azhad Ghufran
 
 
 # Testing
-
-
```

### Comparing `beau-ssi-converter-0.3.0/setup.py` & `beau-ssi-converter-0.4.0/setup.py`

 * *Files identical despite different names*

