# Comparing `tmp/blob_mounting_helper_utility-1.0.0.tar.gz` & `tmp/blob_mounting_helper_utility-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blob_mounting_helper_utility-1.0.0.tar", last modified: Thu Jun 15 11:13:05 2023, max compression
+gzip compressed data, was "blob_mounting_helper_utility-1.0.1.tar", last modified: Thu Jun 15 11:29:04 2023, max compression
```

## Comparing `blob_mounting_helper_utility-1.0.0.tar` & `blob_mounting_helper_utility-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-15 11:13:05.615901 blob_mounting_helper_utility-1.0.0/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     2189 2023-06-15 11:13:05.615901 blob_mounting_helper_utility-1.0.0/PKG-INFO
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     1352 2023-06-15 10:58:51.000000 blob_mounting_helper_utility-1.0.0/README.md
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-15 11:13:05.611901 blob_mounting_helper_utility-1.0.0/blob_mounting_helper_utility/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       37 2023-06-15 11:11:15.000000 blob_mounting_helper_utility-1.0.0/blob_mounting_helper_utility/__init__.py
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     4230 2023-06-15 10:51:13.000000 blob_mounting_helper_utility-1.0.0/blob_mounting_helper_utility/utils.py
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-15 11:13:05.611901 blob_mounting_helper_utility-1.0.0/blob_mounting_helper_utility.egg-info/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     2189 2023-06-15 11:13:05.000000 blob_mounting_helper_utility-1.0.0/blob_mounting_helper_utility.egg-info/PKG-INFO
--rw-rw-r--   0 ivica     (1000) ivica     (1000)      305 2023-06-15 11:13:05.000000 blob_mounting_helper_utility-1.0.0/blob_mounting_helper_utility.egg-info/SOURCES.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)        1 2023-06-15 11:13:05.000000 blob_mounting_helper_utility-1.0.0/blob_mounting_helper_utility.egg-info/dependency_links.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       29 2023-06-15 11:13:05.000000 blob_mounting_helper_utility-1.0.0/blob_mounting_helper_utility.egg-info/top_level.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       38 2023-06-15 11:13:05.615901 blob_mounting_helper_utility-1.0.0/setup.cfg
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     1028 2023-06-15 11:10:26.000000 blob_mounting_helper_utility-1.0.0/setup.py
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-15 11:29:04.616184 blob_mounting_helper_utility-1.0.1/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     3012 2023-06-15 11:29:04.616184 blob_mounting_helper_utility-1.0.1/PKG-INFO
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     2023 2023-06-15 11:26:52.000000 blob_mounting_helper_utility-1.0.1/README.md
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-15 11:29:04.616184 blob_mounting_helper_utility-1.0.1/blob_mounting_helper_utility/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       37 2023-06-15 11:11:15.000000 blob_mounting_helper_utility-1.0.1/blob_mounting_helper_utility/__init__.py
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     4230 2023-06-15 10:51:13.000000 blob_mounting_helper_utility-1.0.1/blob_mounting_helper_utility/utils.py
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-15 11:29:04.616184 blob_mounting_helper_utility-1.0.1/blob_mounting_helper_utility.egg-info/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     3012 2023-06-15 11:29:04.000000 blob_mounting_helper_utility-1.0.1/blob_mounting_helper_utility.egg-info/PKG-INFO
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)      305 2023-06-15 11:29:04.000000 blob_mounting_helper_utility-1.0.1/blob_mounting_helper_utility.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)        1 2023-06-15 11:29:04.000000 blob_mounting_helper_utility-1.0.1/blob_mounting_helper_utility.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       29 2023-06-15 11:29:04.000000 blob_mounting_helper_utility-1.0.1/blob_mounting_helper_utility.egg-info/top_level.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       38 2023-06-15 11:29:04.616184 blob_mounting_helper_utility-1.0.1/setup.cfg
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     1028 2023-06-15 11:28:17.000000 blob_mounting_helper_utility-1.0.1/setup.py
```

### Comparing `blob_mounting_helper_utility-1.0.0/PKG-INFO` & `blob_mounting_helper_utility-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blob_mounting_helper_utility
-Version: 1.0.0
+Version: 1.0.1
 Summary: Blob mapping utility for easy translation between azure urls and local paths
 Home-page: UNKNOWN
 Author: Ivica Matic
 Author-email: <ivica.matic@spatialdays.com>
 License: UNKNOWN
 Description: 
         # Blob mapping utility
@@ -14,40 +14,59 @@
         
         Configuration file example:
         
         ``` json
         {
           "blob_mounting_configurations": [
             {
-              "storage_account_name": "oseoinfrastagingstrgacc",
-              "storage_account_url": "https://oseoinfrastagingstrgacc.blob.core.windows.net/",
-              "container_name": "heightstore-dsm1m-raw",
-              "mount_point": "/mnt/heightstore-dsm1m-raw"
+              "storage_account_name": "examplestagingstrgacc",
+              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+              "container_name": "heightstore-example1-raw",
+              "mount_point": "/mnt/heightstore-example1-raw"
             },
             {
-              "storage_account_name": "oseoinfrastagingstrgacc",
-              "storage_account_url": "https://oseoinfrastagingstrgacc.blob.core.windows.net/",
-              "container_name": "heightstore-dsm25cm-raw",
-              "mount_point": "/mnt/heightstore-dsm25cm-raw"
+              "storage_account_name": "examplestagingstrgacc",
+              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+              "container_name": "heightstore-example2-raw",
+              "mount_point": "/mnt/heightstore-example2-raw"
             },
             {
-              "storage_account_name": "oseoinfrastagingstrgacc",
-              "storage_account_url": "https://oseoinfrastagingstrgacc.blob.core.windows.net/",
-              "container_name": "heightstore-dtm1m-raw",
-              "mount_point": "/mnt/heightstore-dtm1m-raw"
+              "storage_account_name": "examplestagingstrgacc",
+              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+              "container_name": "heightstore-example3-raw",
+              "mount_point": "/mnt/heightstore-example3-raw"
             },
             {
-              "storage_account_name": "oseoinfrastagingstrgacc",
-              "storage_account_url": "https://oseoinfrastagingstrgacc.blob.core.windows.net/",
-              "container_name": "rss-rgbi25cm16bittiff-raw",
-              "mount_point": "/mnt/rss-rgbi25cm16bittiff-raw"
+              "storage_account_name": "examplestagingstrgacc",
+              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+              "container_name": "example-container-raw",
+              "mount_point": "/mnt/example-container-raw"
             }
           ]
         }
         ```
+        
+        ## How to use
+        
+        ```python
+        from blob_mapping_utility import BlobMappingUtility
+        json_config_file = "blob_mapping_config.json"
+        
+        # read the file into a dictionary
+        with open(json_config_file) as json_file:
+            config = json.load(json_file)["blob_mounting_configurations"]
+        
+        # create the utility object
+        blob_mapping_utility = BlobMappingUtility(config)
+        
+        filepath1 = "/mnt/example-container-raw/cool_picture.png
+        blob_url = blob_mapping_utility.get_url_from_mounted_filepath(mount_point) # -> https://examplestagingstrgacc.blob.core.windows.net/example-container-raw/cool_picture.png
+        
+        filepath2 = get_mounted_filepath_from_url(blob_url) # -> /mnt/example-container-raw/cool_picture.png
+        ```
 Keywords: python,azure,blob,mount
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
```

### Comparing `blob_mounting_helper_utility-1.0.0/blob_mounting_helper_utility/utils.py` & `blob_mounting_helper_utility-1.0.1/blob_mounting_helper_utility/utils.py`

 * *Files identical despite different names*

### Comparing `blob_mounting_helper_utility-1.0.0/blob_mounting_helper_utility.egg-info/PKG-INFO` & `blob_mounting_helper_utility-1.0.1/blob_mounting_helper_utility.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blob-mounting-helper-utility
-Version: 1.0.0
+Version: 1.0.1
 Summary: Blob mapping utility for easy translation between azure urls and local paths
 Home-page: UNKNOWN
 Author: Ivica Matic
 Author-email: <ivica.matic@spatialdays.com>
 License: UNKNOWN
 Description: 
         # Blob mapping utility
@@ -14,40 +14,59 @@
         
         Configuration file example:
         
         ``` json
         {
           "blob_mounting_configurations": [
             {
-              "storage_account_name": "oseoinfrastagingstrgacc",
-              "storage_account_url": "https://oseoinfrastagingstrgacc.blob.core.windows.net/",
-              "container_name": "heightstore-dsm1m-raw",
-              "mount_point": "/mnt/heightstore-dsm1m-raw"
+              "storage_account_name": "examplestagingstrgacc",
+              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+              "container_name": "heightstore-example1-raw",
+              "mount_point": "/mnt/heightstore-example1-raw"
             },
             {
-              "storage_account_name": "oseoinfrastagingstrgacc",
-              "storage_account_url": "https://oseoinfrastagingstrgacc.blob.core.windows.net/",
-              "container_name": "heightstore-dsm25cm-raw",
-              "mount_point": "/mnt/heightstore-dsm25cm-raw"
+              "storage_account_name": "examplestagingstrgacc",
+              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+              "container_name": "heightstore-example2-raw",
+              "mount_point": "/mnt/heightstore-example2-raw"
             },
             {
-              "storage_account_name": "oseoinfrastagingstrgacc",
-              "storage_account_url": "https://oseoinfrastagingstrgacc.blob.core.windows.net/",
-              "container_name": "heightstore-dtm1m-raw",
-              "mount_point": "/mnt/heightstore-dtm1m-raw"
+              "storage_account_name": "examplestagingstrgacc",
+              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+              "container_name": "heightstore-example3-raw",
+              "mount_point": "/mnt/heightstore-example3-raw"
             },
             {
-              "storage_account_name": "oseoinfrastagingstrgacc",
-              "storage_account_url": "https://oseoinfrastagingstrgacc.blob.core.windows.net/",
-              "container_name": "rss-rgbi25cm16bittiff-raw",
-              "mount_point": "/mnt/rss-rgbi25cm16bittiff-raw"
+              "storage_account_name": "examplestagingstrgacc",
+              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+              "container_name": "example-container-raw",
+              "mount_point": "/mnt/example-container-raw"
             }
           ]
         }
         ```
+        
+        ## How to use
+        
+        ```python
+        from blob_mapping_utility import BlobMappingUtility
+        json_config_file = "blob_mapping_config.json"
+        
+        # read the file into a dictionary
+        with open(json_config_file) as json_file:
+            config = json.load(json_file)["blob_mounting_configurations"]
+        
+        # create the utility object
+        blob_mapping_utility = BlobMappingUtility(config)
+        
+        filepath1 = "/mnt/example-container-raw/cool_picture.png
+        blob_url = blob_mapping_utility.get_url_from_mounted_filepath(mount_point) # -> https://examplestagingstrgacc.blob.core.windows.net/example-container-raw/cool_picture.png
+        
+        filepath2 = get_mounted_filepath_from_url(blob_url) # -> /mnt/example-container-raw/cool_picture.png
+        ```
 Keywords: python,azure,blob,mount
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
```

### Comparing `blob_mounting_helper_utility-1.0.0/setup.py` & `blob_mounting_helper_utility-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'Blob mapping utility for easy translation between azure urls and local paths'
 LONG_DESCRIPTION = 'Blob mapping utility for easy translation between azure urls and local paths'
 
 # Setting up
 setup(
     name="blob_mounting_helper_utility",
     version=VERSION,
```

