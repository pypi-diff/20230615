# Comparing `tmp/beetl-0.1.0.tar.gz` & `tmp/beetl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beetl-0.1.0.tar", last modified: Tue Mar 14 10:15:51 2023, max compression
+gzip compressed data, was "beetl-0.1.1.tar", last modified: Tue Mar 14 16:05:57 2023, max compression
```

## Comparing `beetl-0.1.0.tar` & `beetl-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,33 @@
-drwxrwxr-x   0 larsch    (1003) larsch    (1003)        0 2023-03-14 10:15:51.793161 beetl-0.1.0/
--rw-rw-r--   0 larsch    (1003) larsch    (1003)     3720 2023-03-14 10:15:51.793161 beetl-0.1.0/PKG-INFO
--rw-rw-r--   0 larsch    (1003) larsch    (1003)     3116 2023-02-15 09:21:51.000000 beetl-0.1.0/README.md
--rw-rw-r--   0 larsch    (1003) larsch    (1003)       38 2023-03-14 10:15:51.793161 beetl-0.1.0/setup.cfg
--rw-rw-r--   0 larsch    (1003) larsch    (1003)     1626 2023-02-09 16:24:56.000000 beetl-0.1.0/setup.py
-drwxrwxr-x   0 larsch    (1003) larsch    (1003)        0 2023-03-14 10:15:51.789160 beetl-0.1.0/src/
-drwxrwxr-x   0 larsch    (1003) larsch    (1003)        0 2023-03-14 10:15:51.789160 beetl-0.1.0/src/beetl/
--rw-rw-r--   0 larsch    (1003) larsch    (1003)       36 2023-02-09 16:27:50.000000 beetl-0.1.0/src/beetl/__init__.py
--rw-rw-r--   0 larsch    (1003) larsch    (1003)      658 2023-03-14 10:15:47.000000 beetl-0.1.0/src/beetl/__version__.py
--rw-rw-r--   0 larsch    (1003) larsch    (1003)      561 2023-02-09 16:36:56.000000 beetl-0.1.0/src/beetl/beetl.py
--rw-rw-r--   0 larsch    (1003) larsch    (1003)        0 2023-02-09 16:27:59.000000 beetl-0.1.0/src/beetl/models.py
--rw-rw-r--   0 larsch    (1003) larsch    (1003)     2766 2023-02-15 08:46:18.000000 beetl-0.1.0/src/beetl/sources.py
--rw-rw-r--   0 larsch    (1003) larsch    (1003)     1718 2023-02-15 10:46:36.000000 beetl-0.1.0/src/beetl/transformers.py
-drwxrwxr-x   0 larsch    (1003) larsch    (1003)        0 2023-03-14 10:15:51.793161 beetl-0.1.0/src/beetl.egg-info/
--rw-rw-r--   0 larsch    (1003) larsch    (1003)     3720 2023-03-14 10:15:51.000000 beetl-0.1.0/src/beetl.egg-info/PKG-INFO
--rw-rw-r--   0 larsch    (1003) larsch    (1003)      379 2023-03-14 10:15:51.000000 beetl-0.1.0/src/beetl.egg-info/SOURCES.txt
--rw-rw-r--   0 larsch    (1003) larsch    (1003)        1 2023-03-14 10:15:51.000000 beetl-0.1.0/src/beetl.egg-info/dependency_links.txt
--rw-rw-r--   0 larsch    (1003) larsch    (1003)       52 2023-03-14 10:15:51.000000 beetl-0.1.0/src/beetl.egg-info/entry_points.txt
--rw-rw-r--   0 larsch    (1003) larsch    (1003)       38 2023-03-14 10:15:51.000000 beetl-0.1.0/src/beetl.egg-info/requires.txt
--rw-rw-r--   0 larsch    (1003) larsch    (1003)        6 2023-03-14 10:15:51.000000 beetl-0.1.0/src/beetl.egg-info/top_level.txt
--rw-rw-r--   0 larsch    (1003) larsch    (1003)        1 2023-03-14 10:15:51.000000 beetl-0.1.0/src/beetl.egg-info/zip-safe
+drwxrwxr-x   0 larsch    (1003) larsch    (1003)        0 2023-03-14 16:05:57.980746 beetl-0.1.1/
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)     5808 2023-03-14 16:05:57.980746 beetl-0.1.1/PKG-INFO
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)     5204 2023-03-14 15:45:18.000000 beetl-0.1.1/README.md
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)       38 2023-03-14 16:05:57.980746 beetl-0.1.1/setup.cfg
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)     1626 2023-03-14 16:03:52.000000 beetl-0.1.1/setup.py
+drwxrwxr-x   0 larsch    (1003) larsch    (1003)        0 2023-03-14 16:05:57.976746 beetl-0.1.1/src/
+drwxrwxr-x   0 larsch    (1003) larsch    (1003)        0 2023-03-14 16:05:57.976746 beetl-0.1.1/src/beetl/
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)       36 2023-02-09 16:27:50.000000 beetl-0.1.1/src/beetl/__init__.py
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)      658 2023-03-14 16:05:44.000000 beetl-0.1.1/src/beetl/__version__.py
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)     2070 2023-03-14 15:36:40.000000 beetl-0.1.1/src/beetl/beetl.py
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)     3158 2023-03-14 15:51:40.000000 beetl-0.1.1/src/beetl/config.py
+drwxrwxr-x   0 larsch    (1003) larsch    (1003)        0 2023-03-14 16:05:57.980746 beetl-0.1.1/src/beetl/field_transformers/
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)        0 2023-03-14 15:52:38.000000 beetl-0.1.1/src/beetl/field_transformers/__init__.py
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)        0 2023-03-14 15:52:34.000000 beetl-0.1.1/src/beetl/field_transformers/interface.py
+drwxrwxr-x   0 larsch    (1003) larsch    (1003)        0 2023-03-14 16:05:57.980746 beetl-0.1.1/src/beetl/source_transformers/
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)        0 2023-03-14 15:52:43.000000 beetl-0.1.1/src/beetl/source_transformers/__init__.py
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)        0 2023-03-14 15:52:48.000000 beetl-0.1.1/src/beetl/source_transformers/interface.py
+drwxrwxr-x   0 larsch    (1003) larsch    (1003)        0 2023-03-14 16:05:57.980746 beetl-0.1.1/src/beetl/sources/
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)        0 2023-03-14 10:18:50.000000 beetl-0.1.1/src/beetl/sources/__init__.py
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)     3185 2023-03-14 15:37:34.000000 beetl-0.1.1/src/beetl/sources/file.py
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)     3587 2023-03-14 15:30:34.000000 beetl-0.1.1/src/beetl/sources/interface.py
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)     2632 2023-03-14 14:59:13.000000 beetl-0.1.1/src/beetl/sources/mysql.py
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)      940 2023-03-14 14:10:45.000000 beetl-0.1.1/src/beetl/sources/sqlserver.py
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)     2150 2023-03-14 10:21:37.000000 beetl-0.1.1/src/beetl/sources.py
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)     1718 2023-02-15 10:46:36.000000 beetl-0.1.1/src/beetl/transformers.py
+drwxrwxr-x   0 larsch    (1003) larsch    (1003)        0 2023-03-14 16:05:57.980746 beetl-0.1.1/src/beetl.egg-info/
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)     5808 2023-03-14 16:05:57.000000 beetl-0.1.1/src/beetl.egg-info/PKG-INFO
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)      692 2023-03-14 16:05:57.000000 beetl-0.1.1/src/beetl.egg-info/SOURCES.txt
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)        1 2023-03-14 16:05:57.000000 beetl-0.1.1/src/beetl.egg-info/dependency_links.txt
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)       52 2023-03-14 16:05:57.000000 beetl-0.1.1/src/beetl.egg-info/entry_points.txt
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)       75 2023-03-14 16:05:57.000000 beetl-0.1.1/src/beetl.egg-info/requires.txt
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)        6 2023-03-14 16:05:57.000000 beetl-0.1.1/src/beetl.egg-info/top_level.txt
+-rw-rw-r--   0 larsch    (1003) larsch    (1003)        1 2023-03-14 10:15:51.000000 beetl-0.1.1/src/beetl.egg-info/zip-safe
```

### Comparing `beetl-0.1.0/setup.py` & `beetl-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 import os
 from setuptools import setup, find_packages
 
 repository_name = 'beetl'
 module_name = 'beetl'
-python_min_version = ">=3.6"
+python_min_version = ">=3.8"
 
 with open('requirements.txt', 'r') as f:
     required_packages = f.read().splitlines()
 
 # Get key package details
 about = {}  # type: ignore
 here = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `beetl-0.1.0/src/beetl/__version__.py` & `beetl-0.1.1/src/beetl/__version__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 __title__ = "beetl"
 __description__ = """
     Bee ETL is a Python package for extracting data from one source, transforming it and loading it into another
 """
 
 # The version and build number
 # Without specifying a unique number, you cannot overwrite packages in the PyPi repo
-__version__ = os.getenv("RELEASE_NAME", "0.1.0" + os.getenv("GITHUB_RUN_ID", ""))
+__version__ = os.getenv("RELEASE_NAME", "0.1.1" + os.getenv("GITHUB_RUN_ID", ""))
 
 # Author and license information
 __author__ = "Lars Scheibling"
 __author_email__ = "lars.scheibling@hoglandet.se"
 __license__ = "GnuPG 3.0"
 
 # URL to the project
```

### Comparing `beetl-0.1.0/src/beetl/sources.py` & `beetl-0.1.1/src/beetl/sources.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,13 @@
 from typing import List 
 import polars
 import sqlalchemy as sqla
 import sqlalchemy.sql as sqf
-from abc import ABC, abstractmethod
 
-class SourceInterface(ABC):
-    """Interface for a connection to a data source, either for reading or writing data"""
-    connection = None
-    
-    def __init__(self, config):
-        self._configure(config)
-    
-    def query(self, *args, **kwargs) -> polars.DataFrame:
-        return self._parse(self._retrieve(*args, **kwargs))
-    
-    @abstractmethod
-    def _configure(self, config):
-        pass
-    
-    @abstractmethod
-    def _retrieve(self, *args, **kwargs):
-        pass
-    
-    @abstractmethod
-    def _parse(self, *args, **kwargs) -> polars.DataFrame:
-        pass
+
 
 class FileSource(SourceInterface):
     """ 
         Interface for sources from the filesystem
         Needs a path to the file and charset
     """
     def _configure(self, path: str, charset: str = "utf-8"):
```

### Comparing `beetl-0.1.0/src/beetl/transformers.py` & `beetl-0.1.1/src/beetl/transformers.py`

 * *Files identical despite different names*

