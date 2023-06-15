# Comparing `tmp/mnzipcode-0.0.7.tar.gz` & `tmp/mnzipcode-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnzipcode-0.0.7.tar", last modified: Thu Jun 15 09:09:23 2023, max compression
+gzip compressed data, was "mnzipcode-0.0.8.tar", last modified: Thu Jun 15 09:47:03 2023, max compression
```

## Comparing `mnzipcode-0.0.7.tar` & `mnzipcode-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-06-15 09:09:23.816557 mnzipcode-0.0.7/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1034 2023-06-15 09:09:23.816557 mnzipcode-0.0.7/PKG-INFO
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      265 2023-03-23 09:39:39.000000 mnzipcode-0.0.7/README.md
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-06-15 09:09:23.816557 mnzipcode-0.0.7/mnzipcode/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       25 2023-05-07 07:52:13.000000 mnzipcode-0.0.7/mnzipcode/__init__.py
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-06-15 09:09:23.816557 mnzipcode-0.0.7/mnzipcode/data/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     2981 2023-05-07 07:22:37.000000 mnzipcode-0.0.7/mnzipcode/data/province_info.json
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)        0 2023-05-07 06:16:51.000000 mnzipcode-0.0.7/mnzipcode/data/sum_info.json
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)   140107 2023-05-07 07:07:44.000000 mnzipcode-0.0.7/mnzipcode/data/zip.json
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     3632 2023-06-15 09:08:27.000000 mnzipcode-0.0.7/mnzipcode/mnZipCodes.py
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-06-15 09:09:23.816557 mnzipcode-0.0.7/mnzipcode.egg-info/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1034 2023-06-15 09:09:23.000000 mnzipcode-0.0.7/mnzipcode.egg-info/PKG-INFO
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      283 2023-06-15 09:09:23.000000 mnzipcode-0.0.7/mnzipcode.egg-info/SOURCES.txt
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)        1 2023-06-15 09:09:23.000000 mnzipcode-0.0.7/mnzipcode.egg-info/dependency_links.txt
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       10 2023-06-15 09:09:23.000000 mnzipcode-0.0.7/mnzipcode.egg-info/top_level.txt
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       38 2023-06-15 09:09:23.816557 mnzipcode-0.0.7/setup.cfg
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1185 2023-06-15 09:05:18.000000 mnzipcode-0.0.7/setup.py
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-06-15 09:47:03.307377 mnzipcode-0.0.8/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1033 2023-06-15 09:47:03.307377 mnzipcode-0.0.8/PKG-INFO
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1000 2023-06-15 09:22:59.000000 mnzipcode-0.0.8/README.md
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-06-15 09:47:03.303377 mnzipcode-0.0.8/mnzipcode/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       25 2023-05-07 07:52:13.000000 mnzipcode-0.0.8/mnzipcode/__init__.py
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-06-15 09:47:03.303377 mnzipcode-0.0.8/mnzipcode/data/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     2107 2023-06-15 09:46:17.000000 mnzipcode-0.0.8/mnzipcode/data/duureg_info.json
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     2981 2023-05-07 07:22:37.000000 mnzipcode-0.0.8/mnzipcode/data/province_info.json
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)        0 2023-05-07 06:16:51.000000 mnzipcode-0.0.8/mnzipcode/data/sum_info.json
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)   140107 2023-05-07 07:07:44.000000 mnzipcode-0.0.8/mnzipcode/data/zip.json
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     4156 2023-06-15 09:46:32.000000 mnzipcode-0.0.8/mnzipcode/mnZipCodes.py
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-06-15 09:47:03.303377 mnzipcode-0.0.8/mnzipcode.egg-info/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1033 2023-06-15 09:47:03.000000 mnzipcode-0.0.8/mnzipcode.egg-info/PKG-INFO
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      315 2023-06-15 09:47:03.000000 mnzipcode-0.0.8/mnzipcode.egg-info/SOURCES.txt
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)        1 2023-06-15 09:47:03.000000 mnzipcode-0.0.8/mnzipcode.egg-info/dependency_links.txt
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       10 2023-06-15 09:47:03.000000 mnzipcode-0.0.8/mnzipcode.egg-info/top_level.txt
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       38 2023-06-15 09:47:03.307377 mnzipcode-0.0.8/setup.cfg
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1184 2023-06-15 09:46:52.000000 mnzipcode-0.0.8/setup.py
```

### Comparing `mnzipcode-0.0.7/PKG-INFO` & `mnzipcode-0.0.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,29 @@
-Metadata-Version: 2.1
-Name: mnzipcode
-Version: 0.0.7
-Summary: mnzipcodes is a simple library for querying Mongolian zip codes.
-Author: Bekkage
-Description-Content-Type: text/markdown
-
-
+# mnzipcodes
 mnzipcodes is a simple library for querying Mongolian zip codes.
 
+  - Video introduction: [YOUTUBE](https://www.youtube.com/watch?v=vml3CxglLko)
+  - PYPI: [MNZIPCODE](https://pypi.org/project/mnzipcode/)
+
 ### Installation
 
 mnzipcode is available on PyPi:
 ```
 # python -m pip install mnzipcode
 ```
 
-Example usage:
+### Example usage:
 
 ```python
 >>> import mnzipcode
 >>> 
 >>> obj = mnzipcode.ZipCode()
 >>> 
 >>> obj.matching_by_zipcode(11000)
 {'name': 'Ulaanbaatar', 'stat': 'province', 'mnname': 'Улаанбаатар', 'year_established': 1942, 'area': 4704.4, 'population': 1539810, 'density': 327}
 >>> 
 >>> obj.matching_by_name('Дархан-Уул')
 [{'name': 'Darkhan-Uul', 'zipcode': '45000', 'stat': 'province', 'mnname': 'Дархан-Уул', 'year_established': 1994, 'area': 3275.0, 'population': 107018, 'density': 33}, {'name': 'Дархан-Уул', 'zipcode': '81041', 'stat': 'bag'}, {'name': 'Дархан-Уул', 'zipcode': '81063', 'stat': 'bag'}]
 >>> 
 >>> obj.isReal(11000)
 True
-```
-
-  
+```
```

### Comparing `mnzipcode-0.0.7/mnzipcode/data/province_info.json` & `mnzipcode-0.0.8/mnzipcode/data/province_info.json`

 * *Files identical despite different names*

### Comparing `mnzipcode-0.0.7/mnzipcode/data/zip.json` & `mnzipcode-0.0.8/mnzipcode/data/zip.json`

 * *Files identical despite different names*

### Comparing `mnzipcode-0.0.7/mnzipcode/mnZipCodes.py` & `mnzipcode-0.0.8/mnzipcode/mnZipCodes.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,14 +8,18 @@
     with open('mnzipcode/data/zip.json', 'r') as f: 
       self.zip_codes = json.loads(f.read())
 
     # LOAD PROVINCE info
     with open('mnzipcode/data/province_info.json', 'r') as f: 
       self.province_info = json.loads(f.read())
 
+    # LOAD DUUREG info
+    with open('mnzipcode/data/duureg_info.json', 'r') as f: 
+      self.duureg_info = json.loads(f.read())
+
   @staticmethod
   def flatten_list(lst):
     result = []
     for item in lst:
       if isinstance(item, dict):
         result.append(item)
       elif isinstance(item, list):
@@ -92,34 +96,43 @@
 
     return ZipCode.flatten_list(results)
   
   def get_province_info(self, province_mn_name: str) -> dict:
     for province in self.province_info:
       if province['mnname'] == province_mn_name:
         return province
+      
+  def get_duureg_info(self, duureg_mn_name: str) -> dict: 
+    for duureg in self.duureg_info:
+      if duureg['mnname'] == duureg_mn_name:
+        return duureg
 
   # 1
   def matching_by_zipcode(self, zipcode: int) -> dict:
     result = self.find_label_by_zipcode(zipcode)
 
     if result!=None:
       if result['stat'] == 'province':
         return {**result, **self.get_province_info(result['name'])}
+      elif result['stat'] == 'duureg':
+        return {**result, **self.get_duureg_info(result['name'])}
       else:
         return result
       
   # 2
   def matching_by_name(self, name: str) -> list:
     results = self.find_zipcode_by_name(name)
 
     ret_data: list = []
     if results != []:
       for result in results:
         if result['stat'] == 'province':
           ret_data.append({**result, **self.get_province_info(result['name'])})
+        elif result['stat'] == 'duureg':
+          ret_data.append({**result, **self.get_duureg_info(result['name'])})
         else:
           ret_data.append(result)
 
       return ret_data 
     
   #3
   def isReal(self, zipcode: int) -> bool:
```

### Comparing `mnzipcode-0.0.7/mnzipcode.egg-info/PKG-INFO` & `mnzipcode-0.0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-Metadata-Version: 2.1
-Name: mnzipcode
-Version: 0.0.7
-Summary: mnzipcodes is a simple library for querying Mongolian zip codes.
-Author: Bekkage
-Description-Content-Type: text/markdown
+import setuptools 
 
-
-mnzipcodes is a simple library for querying Mongolian zip codes.
+setuptools.setup(
+  name='mnzipcode',
+  version='0.0.8',
+  author='Bekkage',
+  description='mnzipcodes is a simple library for querying Mongolian zip codes.',
+  package_data={
+    'mnzipcode': ['data/*.json']
+  },
+  long_description_content_type= 'text/markdown',
+  long_description="""
+mnzipcode is a simple library for querying Mongolian zip codes.
 
 ### Installation
 
 mnzipcode is available on PyPi:
 ```
 # python -m pip install mnzipcode
 ```
@@ -28,8 +32,10 @@
 >>> obj.matching_by_name('Дархан-Уул')
 [{'name': 'Darkhan-Uul', 'zipcode': '45000', 'stat': 'province', 'mnname': 'Дархан-Уул', 'year_established': 1994, 'area': 3275.0, 'population': 107018, 'density': 33}, {'name': 'Дархан-Уул', 'zipcode': '81041', 'stat': 'bag'}, {'name': 'Дархан-Уул', 'zipcode': '81063', 'stat': 'bag'}]
 >>> 
 >>> obj.isReal(11000)
 True
 ```
 
-  
+  """,
+  package=['mnzipcode']
+)
```

### Comparing `mnzipcode-0.0.7/setup.py` & `mnzipcode-0.0.8/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-import setuptools 
+Metadata-Version: 2.1
+Name: mnzipcode
+Version: 0.0.8
+Summary: mnzipcodes is a simple library for querying Mongolian zip codes.
+Author: Bekkage
+Description-Content-Type: text/markdown
 
-setuptools.setup(
-  name='mnzipcode',
-  version='0.0.7',
-  author='Bekkage',
-  description='mnzipcodes is a simple library for querying Mongolian zip codes.',
-  package_data={
-    'mnzipcode': ['data/*.json']
-  },
-  long_description_content_type= 'text/markdown',
-  long_description="""
-mnzipcodes is a simple library for querying Mongolian zip codes.
+
+mnzipcode is a simple library for querying Mongolian zip codes.
 
 ### Installation
 
 mnzipcode is available on PyPi:
 ```
 # python -m pip install mnzipcode
 ```
@@ -32,10 +28,8 @@
 >>> obj.matching_by_name('Дархан-Уул')
 [{'name': 'Darkhan-Uul', 'zipcode': '45000', 'stat': 'province', 'mnname': 'Дархан-Уул', 'year_established': 1994, 'area': 3275.0, 'population': 107018, 'density': 33}, {'name': 'Дархан-Уул', 'zipcode': '81041', 'stat': 'bag'}, {'name': 'Дархан-Уул', 'zipcode': '81063', 'stat': 'bag'}]
 >>> 
 >>> obj.isReal(11000)
 True
 ```
 
-  """,
-  package=['mnzipcode']
-)
+
```

