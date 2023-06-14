# Comparing `tmp/hierarchical_conf-1.0.2.tar.gz` & `tmp/hierarchical_conf-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hierarchical_conf-1.0.2.tar", last modified: Tue Aug 23 14:58:33 2022, max compression
+gzip compressed data, was "dist/hierarchical_conf-1.0.3.tar", last modified: Wed Jun 14 22:42:06 2023, max compression
```

## Comparing `hierarchical_conf-1.0.2.tar` & `hierarchical_conf-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 14:58:33.000000 hierarchical_conf-1.0.2/
--rw-r--r--   0 root         (0) root         (0)     6324 2022-08-23 14:58:33.000000 hierarchical_conf-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5701 2022-08-23 14:58:33.000000 hierarchical_conf-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 14:58:33.000000 hierarchical_conf-1.0.2/hierarchical_conf/
--rw-r--r--   0 root         (0) root         (0)       65 2022-08-23 14:58:33.000000 hierarchical_conf-1.0.2/hierarchical_conf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4888 2022-08-23 14:58:33.000000 hierarchical_conf-1.0.2/hierarchical_conf/hierarchical_conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 14:58:33.000000 hierarchical_conf-1.0.2/hierarchical_conf.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6324 2022-08-23 14:58:33.000000 hierarchical_conf-1.0.2/hierarchical_conf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      301 2022-08-23 14:58:33.000000 hierarchical_conf-1.0.2/hierarchical_conf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-23 14:58:33.000000 hierarchical_conf-1.0.2/hierarchical_conf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-08-23 14:58:33.000000 hierarchical_conf-1.0.2/hierarchical_conf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-08-23 14:58:33.000000 hierarchical_conf-1.0.2/hierarchical_conf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      869 2022-08-23 14:58:33.000000 hierarchical_conf-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1451 2022-08-23 14:58:33.000000 hierarchical_conf-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:42:06.000000 hierarchical_conf-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)     6324 2023-06-14 22:42:06.000000 hierarchical_conf-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5701 2023-06-14 22:42:06.000000 hierarchical_conf-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:42:06.000000 hierarchical_conf-1.0.3/hierarchical_conf/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 22:42:06.000000 hierarchical_conf-1.0.3/hierarchical_conf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4723 2023-06-14 22:42:06.000000 hierarchical_conf-1.0.3/hierarchical_conf/hierarchical_conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:42:06.000000 hierarchical_conf-1.0.3/hierarchical_conf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6324 2023-06-14 22:42:06.000000 hierarchical_conf-1.0.3/hierarchical_conf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      301 2023-06-14 22:42:06.000000 hierarchical_conf-1.0.3/hierarchical_conf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 22:42:06.000000 hierarchical_conf-1.0.3/hierarchical_conf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-14 22:42:06.000000 hierarchical_conf-1.0.3/hierarchical_conf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-14 22:42:06.000000 hierarchical_conf-1.0.3/hierarchical_conf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      869 2023-06-14 22:42:06.000000 hierarchical_conf-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1402 2023-06-14 22:42:06.000000 hierarchical_conf-1.0.3/setup.py
```

### Comparing `hierarchical_conf-1.0.2/PKG-INFO` & `hierarchical_conf-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hierarchical_conf
-Version: 1.0.2
+Version: 1.0.3
 Summary: A tool for loading settings from files hierarchically
 Home-page: https://github.com/quintoandar/hierarchical-conf
 Author: QuintoAndar
 License: UNKNOWN
 Keywords: hierarchical-conf,configuration by environment,configuration files,configuration as code,hierarchical configuration
 Platform: UNKNOWN
 Classifier: Natural Language :: English
```

### Comparing `hierarchical_conf-1.0.2/README.md` & `hierarchical_conf-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hierarchical_conf-1.0.2/hierarchical_conf/hierarchical_conf.py` & `hierarchical_conf-1.0.3/hierarchical_conf/hierarchical_conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Hierarchical Conf main class."""
-import logging
 import os
 from collections.abc import Mapping
 from os.path import isfile
 from typing import Union, List, Dict, Any, Mapping as MappingType
 
 import yaml
 
@@ -82,18 +81,14 @@
         Checks if the configuration file path exists.
 
         :param config_file_path: the configuration file path
         """
         if isfile(config_file_path):
             return True
 
-        logging.warning(
-            f"msg=This configuration file was not found in the given path,"
-            f"file={config_file_path}"
-        )
         return False
 
     @staticmethod
     def _read_configuration(conf_file_path: str) -> Union[Any, Dict[str, Any]]:
         """
         Open files.
```

### Comparing `hierarchical_conf-1.0.2/hierarchical_conf.egg-info/PKG-INFO` & `hierarchical_conf-1.0.3/hierarchical_conf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hierarchical-conf
-Version: 1.0.2
+Version: 1.0.3
 Summary: A tool for loading settings from files hierarchically
 Home-page: https://github.com/quintoandar/hierarchical-conf
 Author: QuintoAndar
 License: UNKNOWN
 Keywords: hierarchical-conf,configuration by environment,configuration files,configuration as code,hierarchical configuration
 Platform: UNKNOWN
 Classifier: Natural Language :: English
```

### Comparing `hierarchical_conf-1.0.2/setup.cfg` & `hierarchical_conf-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `hierarchical_conf-1.0.2/setup.py` & `hierarchical_conf-1.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 __package_name__ = "hierarchical_conf"
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 __repository_url__ = "https://github.com/quintoandar/hierarchical-conf"
 
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
 with open("requirements.txt") as f:
@@ -24,20 +24,15 @@
         "configuration by environment",
         "configuration files",
         "configuration as code",
         "hierarchical configuration",
     ],
     version=__version__,
     url=__repository_url__,
-    packages=find_packages(
-        include=[
-            "hierarchical_conf",
-            "hierarchical_conf.*",
-        ]
-    ),
+    packages=find_packages(include=["hierarchical_conf", "hierarchical_conf.*"]),
     author="QuintoAndar",
     install_requires=requirements,
     python_requires=">=3.7, <4",
     classifiers=[
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
```

