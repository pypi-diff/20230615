# Comparing `tmp/mnzipcode-0.0.8.tar.gz` & `tmp/mnzipcode-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnzipcode-0.0.8.tar", last modified: Thu Jun 15 09:47:03 2023, max compression
+gzip compressed data, was "mnzipcode-0.0.9.tar", last modified: Thu Jun 15 10:02:53 2023, max compression
```

## Comparing `mnzipcode-0.0.8.tar` & `mnzipcode-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-06-15 09:47:03.307377 mnzipcode-0.0.8/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1033 2023-06-15 09:47:03.307377 mnzipcode-0.0.8/PKG-INFO
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1000 2023-06-15 09:22:59.000000 mnzipcode-0.0.8/README.md
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-06-15 09:47:03.303377 mnzipcode-0.0.8/mnzipcode/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       25 2023-05-07 07:52:13.000000 mnzipcode-0.0.8/mnzipcode/__init__.py
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-06-15 09:47:03.303377 mnzipcode-0.0.8/mnzipcode/data/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     2107 2023-06-15 09:46:17.000000 mnzipcode-0.0.8/mnzipcode/data/duureg_info.json
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     2981 2023-05-07 07:22:37.000000 mnzipcode-0.0.8/mnzipcode/data/province_info.json
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)        0 2023-05-07 06:16:51.000000 mnzipcode-0.0.8/mnzipcode/data/sum_info.json
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)   140107 2023-05-07 07:07:44.000000 mnzipcode-0.0.8/mnzipcode/data/zip.json
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     4156 2023-06-15 09:46:32.000000 mnzipcode-0.0.8/mnzipcode/mnZipCodes.py
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-06-15 09:47:03.303377 mnzipcode-0.0.8/mnzipcode.egg-info/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1033 2023-06-15 09:47:03.000000 mnzipcode-0.0.8/mnzipcode.egg-info/PKG-INFO
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      315 2023-06-15 09:47:03.000000 mnzipcode-0.0.8/mnzipcode.egg-info/SOURCES.txt
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)        1 2023-06-15 09:47:03.000000 mnzipcode-0.0.8/mnzipcode.egg-info/dependency_links.txt
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       10 2023-06-15 09:47:03.000000 mnzipcode-0.0.8/mnzipcode.egg-info/top_level.txt
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       38 2023-06-15 09:47:03.307377 mnzipcode-0.0.8/setup.cfg
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1184 2023-06-15 09:46:52.000000 mnzipcode-0.0.8/setup.py
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-06-15 10:02:53.185593 mnzipcode-0.0.9/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1033 2023-06-15 10:02:53.185593 mnzipcode-0.0.9/PKG-INFO
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1000 2023-06-15 09:22:59.000000 mnzipcode-0.0.9/README.md
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-06-15 10:02:53.181593 mnzipcode-0.0.9/mnzipcode/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       25 2023-05-07 07:52:13.000000 mnzipcode-0.0.9/mnzipcode/__init__.py
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-06-15 10:02:53.185593 mnzipcode-0.0.9/mnzipcode/data/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     2107 2023-06-15 09:46:17.000000 mnzipcode-0.0.9/mnzipcode/data/duureg_info.json
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     2981 2023-05-07 07:22:37.000000 mnzipcode-0.0.9/mnzipcode/data/province_info.json
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)        0 2023-05-07 06:16:51.000000 mnzipcode-0.0.9/mnzipcode/data/sum_info.json
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)   140107 2023-05-07 07:07:44.000000 mnzipcode-0.0.9/mnzipcode/data/zip.json
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     4275 2023-06-15 09:58:58.000000 mnzipcode-0.0.9/mnzipcode/mnZipCodes.py
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-06-15 10:02:53.181593 mnzipcode-0.0.9/mnzipcode.egg-info/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1033 2023-06-15 10:02:53.000000 mnzipcode-0.0.9/mnzipcode.egg-info/PKG-INFO
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      315 2023-06-15 10:02:53.000000 mnzipcode-0.0.9/mnzipcode.egg-info/SOURCES.txt
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)        1 2023-06-15 10:02:53.000000 mnzipcode-0.0.9/mnzipcode.egg-info/dependency_links.txt
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       10 2023-06-15 10:02:53.000000 mnzipcode-0.0.9/mnzipcode.egg-info/top_level.txt
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       38 2023-06-15 10:02:53.185593 mnzipcode-0.0.9/setup.cfg
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1184 2023-06-15 09:59:31.000000 mnzipcode-0.0.9/setup.py
```

### Comparing `mnzipcode-0.0.8/PKG-INFO` & `mnzipcode-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnzipcode
-Version: 0.0.8
+Version: 0.0.9
 Summary: mnzipcodes is a simple library for querying Mongolian zip codes.
 Author: Bekkage
 Description-Content-Type: text/markdown
 
 
 mnzipcode is a simple library for querying Mongolian zip codes.
```

### Comparing `mnzipcode-0.0.8/README.md` & `mnzipcode-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mnzipcode-0.0.8/mnzipcode/data/duureg_info.json` & `mnzipcode-0.0.9/mnzipcode/data/duureg_info.json`

 * *Files identical despite different names*

### Comparing `mnzipcode-0.0.8/mnzipcode/data/province_info.json` & `mnzipcode-0.0.9/mnzipcode/data/province_info.json`

 * *Files identical despite different names*

### Comparing `mnzipcode-0.0.8/mnzipcode/data/zip.json` & `mnzipcode-0.0.9/mnzipcode/data/zip.json`

 * *Files identical despite different names*

### Comparing `mnzipcode-0.0.8/mnzipcode/mnZipCodes.py` & `mnzipcode-0.0.9/mnzipcode/mnZipCodes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #!/usr/bin/env python3 
 import json 
 import re
+from os import path
 
 class ZipCode:
   def __init__(self) -> None:
     # LOAD ZIP CODE
-    with open('mnzipcode/data/zip.json', 'r') as f: 
+    current_script_dir = path.dirname(path.realpath(__file__))
+    with open(f'{current_script_dir}/data/zip.json', 'r') as f: 
       self.zip_codes = json.loads(f.read())
 
     # LOAD PROVINCE info
-    with open('mnzipcode/data/province_info.json', 'r') as f: 
+    with open(f'{current_script_dir}/data/province_info.json', 'r') as f: 
       self.province_info = json.loads(f.read())
 
     # LOAD DUUREG info
-    with open('mnzipcode/data/duureg_info.json', 'r') as f: 
+    with open(f'{current_script_dir}/data/duureg_info.json', 'r') as f: 
       self.duureg_info = json.loads(f.read())
 
   @staticmethod
   def flatten_list(lst):
     result = []
     for item in lst:
       if isinstance(item, dict):
```

### Comparing `mnzipcode-0.0.8/mnzipcode.egg-info/PKG-INFO` & `mnzipcode-0.0.9/mnzipcode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnzipcode
-Version: 0.0.8
+Version: 0.0.9
 Summary: mnzipcodes is a simple library for querying Mongolian zip codes.
 Author: Bekkage
 Description-Content-Type: text/markdown
 
 
 mnzipcode is a simple library for querying Mongolian zip codes.
```

### Comparing `mnzipcode-0.0.8/setup.py` & `mnzipcode-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools 
 
 setuptools.setup(
   name='mnzipcode',
-  version='0.0.8',
+  version='0.0.9',
   author='Bekkage',
   description='mnzipcodes is a simple library for querying Mongolian zip codes.',
   package_data={
     'mnzipcode': ['data/*.json']
   },
   long_description_content_type= 'text/markdown',
   long_description="""
```

