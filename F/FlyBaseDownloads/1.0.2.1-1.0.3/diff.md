# Comparing `tmp/FlyBaseDownloads-1.0.2.1.tar.gz` & `tmp/FlyBaseDownloads-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlyBaseDownloads-1.0.2.1.tar", last modified: Wed Jun 14 23:07:12 2023, max compression
+gzip compressed data, was "FlyBaseDownloads-1.0.3.tar", last modified: Wed Jun 14 23:46:06 2023, max compression
```

## Comparing `FlyBaseDownloads-1.0.2.1.tar` & `FlyBaseDownloads-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-14 23:07:12.904120 FlyBaseDownloads-1.0.2.1/
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-14 23:07:12.904120 FlyBaseDownloads-1.0.2.1/FlyBaseDownloads/
--rw-rw-r--   0 usuario   (1000) usuario   (1000)    18483 2023-06-14 22:58:15.000000 FlyBaseDownloads-1.0.2.1/FlyBaseDownloads/FBD.py
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      702 2023-06-14 22:55:23.000000 FlyBaseDownloads-1.0.2.1/FlyBaseDownloads/__init__.py
-drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-14 23:07:12.904120 FlyBaseDownloads-1.0.2.1/FlyBaseDownloads.egg-info/
--rw-rw-r--   0 usuario   (1000) usuario   (1000)    26504 2023-06-14 23:07:12.000000 FlyBaseDownloads-1.0.2.1/FlyBaseDownloads.egg-info/PKG-INFO
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      280 2023-06-14 23:07:12.000000 FlyBaseDownloads-1.0.2.1/FlyBaseDownloads.egg-info/SOURCES.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)        1 2023-06-14 23:07:12.000000 FlyBaseDownloads-1.0.2.1/FlyBaseDownloads.egg-info/dependency_links.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       14 2023-06-14 23:07:12.000000 FlyBaseDownloads-1.0.2.1/FlyBaseDownloads.egg-info/requires.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       17 2023-06-14 23:07:12.000000 FlyBaseDownloads-1.0.2.1/FlyBaseDownloads.egg-info/top_level.txt
--rw-rw-r--   0 usuario   (1000) usuario   (1000)    26504 2023-06-14 23:07:12.904120 FlyBaseDownloads-1.0.2.1/PKG-INFO
--rw-rw-r--   0 usuario   (1000) usuario   (1000)    25940 2023-06-14 23:03:31.000000 FlyBaseDownloads-1.0.2.1/README.md
--rw-rw-r--   0 usuario   (1000) usuario   (1000)       79 2023-06-14 23:07:12.904120 FlyBaseDownloads-1.0.2.1/setup.cfg
--rw-rw-r--   0 usuario   (1000) usuario   (1000)      910 2023-06-14 22:00:23.000000 FlyBaseDownloads-1.0.2.1/setup.py
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-14 23:46:06.610985 FlyBaseDownloads-1.0.3/
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-14 23:46:06.610985 FlyBaseDownloads-1.0.3/FlyBaseDownloads/
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    18514 2023-06-14 23:41:00.000000 FlyBaseDownloads-1.0.3/FlyBaseDownloads/FBD.py
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      702 2023-06-14 22:55:23.000000 FlyBaseDownloads-1.0.3/FlyBaseDownloads/__init__.py
+drwxrwxr-x   0 usuario   (1000) usuario   (1000)        0 2023-06-14 23:46:06.610985 FlyBaseDownloads-1.0.3/FlyBaseDownloads.egg-info/
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    26511 2023-06-14 23:46:06.000000 FlyBaseDownloads-1.0.3/FlyBaseDownloads.egg-info/PKG-INFO
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      280 2023-06-14 23:46:06.000000 FlyBaseDownloads-1.0.3/FlyBaseDownloads.egg-info/SOURCES.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)        1 2023-06-14 23:46:06.000000 FlyBaseDownloads-1.0.3/FlyBaseDownloads.egg-info/dependency_links.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       14 2023-06-14 23:46:06.000000 FlyBaseDownloads-1.0.3/FlyBaseDownloads.egg-info/requires.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       17 2023-06-14 23:46:06.000000 FlyBaseDownloads-1.0.3/FlyBaseDownloads.egg-info/top_level.txt
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    26511 2023-06-14 23:46:06.610985 FlyBaseDownloads-1.0.3/PKG-INFO
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)    25940 2023-06-14 23:03:31.000000 FlyBaseDownloads-1.0.3/README.md
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)       79 2023-06-14 23:46:06.614985 FlyBaseDownloads-1.0.3/setup.cfg
+-rw-rw-r--   0 usuario   (1000) usuario   (1000)      917 2023-06-14 23:45:28.000000 FlyBaseDownloads-1.0.3/setup.py
```

### Comparing `FlyBaseDownloads-1.0.2.1/FlyBaseDownloads/FBD.py` & `FlyBaseDownloads-1.0.3/FlyBaseDownloads/FBD.py`

 * *Files 0% similar despite different names*

```diff
@@ -454,14 +454,15 @@
     class Ontology_Terms():
         
         def __init__(self, fbd_instance):
             self.db = fbd_instance
         
             self.main_url = self.db.main_url
             self.go_url = 'ontologies/'
+            self.header = None
             
         def get(self):
             
             url = self.main_url + self.go_url + self.un_url
             descargas = self.db.Downloads(url)
             
             return descargas.get(self.header)
```

### Comparing `FlyBaseDownloads-1.0.2.1/FlyBaseDownloads/__init__.py` & `FlyBaseDownloads-1.0.3/FlyBaseDownloads/__init__.py`

 * *Files identical despite different names*

### Comparing `FlyBaseDownloads-1.0.2.1/FlyBaseDownloads.egg-info/PKG-INFO` & `FlyBaseDownloads-1.0.3/FlyBaseDownloads.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: FlyBaseDownloads
-Version: 1.0.2.1
+Version: 1.0.3
 Summary: Package to download Flybase data in Python, easily and quickly.
 Home-page: https://github.com/JavieraQuirozO/FlyBaseDownloads
 Author: Javiera Quiroz Olave
 Author-email: javiera.quiroz@biomedica.udec.cl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Healthcare Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # FlyBaseDownloads
 
 Python package to facilitate the data download from FlyBase. Most of the available data from their official wiki can be downloaded. One of the purposes of this library is to organize the data as closely as possible to the source, **FlyBase**. Despite not being the official package, it is organized by data class/type and provides direct downloads of the current bulk data files from the FTP site.
 For more information, visit the [official FlyBase wiki](https://wiki.flybase.org/wiki/FlyBase:Downloads_Overview).
```

### Comparing `FlyBaseDownloads-1.0.2.1/PKG-INFO` & `FlyBaseDownloads-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: FlyBaseDownloads
-Version: 1.0.2.1
+Version: 1.0.3
 Summary: Package to download Flybase data in Python, easily and quickly.
 Home-page: https://github.com/JavieraQuirozO/FlyBaseDownloads
 Author: Javiera Quiroz Olave
 Author-email: javiera.quiroz@biomedica.udec.cl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Healthcare Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # FlyBaseDownloads
 
 Python package to facilitate the data download from FlyBase. Most of the available data from their official wiki can be downloaded. One of the purposes of this library is to organize the data as closely as possible to the source, **FlyBase**. Despite not being the official package, it is organized by data class/type and provides direct downloads of the current bulk data files from the FTP site.
 For more information, visit the [official FlyBase wiki](https://wiki.flybase.org/wiki/FlyBase:Downloads_Overview).
```

### Comparing `FlyBaseDownloads-1.0.2.1/README.md` & `FlyBaseDownloads-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `FlyBaseDownloads-1.0.2.1/setup.py` & `FlyBaseDownloads-1.0.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 @author: javiera.quiroz
 """
 
 from setuptools import setup
 
 setup(
     name='FlyBaseDownloads',
-    version='1.0.2.1',
+    version='1.0.3',
     license='MIT',
     author='Javiera Quiroz Olave',
     url= 'https://github.com/JavieraQuirozO/FlyBaseDownloads',
     author_email='javiera.quiroz@biomedica.udec.cl',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=open('requirements.txt').readlines(),
     description='Package to download Flybase data in Python, easily and quickly.',
     packages=['FlyBaseDownloads'],
     classifiers=[
         'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
+        'Intended Audience :: Science/Research',
+        'Intended Audience :: Healthcare Industry',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.9',
     ],
 )
```

