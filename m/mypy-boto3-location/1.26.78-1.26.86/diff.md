# Comparing `tmp/mypy-boto3-location-1.26.78.tar.gz` & `tmp/mypy-boto3-location-1.26.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-location-1.26.78.tar", last modified: Thu Feb 23 20:34:57 2023, max compression
+gzip compressed data, was "mypy-boto3-location-1.26.86.tar", last modified: Tue Mar  7 20:27:21 2023, max compression
```

## Comparing `mypy-boto3-location-1.26.78.tar` & `mypy-boto3-location-1.26.86.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.320421 mypy-boto3-location-1.26.78/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-23 20:34:36.000000 mypy-boto3-location-1.26.78/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21041 2023-02-23 20:34:57.320421 mypy-boto3-location-1.26.78/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19543 2023-02-23 20:34:36.000000 mypy-boto3-location-1.26.78/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.316421 mypy-boto3-location-1.26.78/mypy_boto3_location/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-02-23 20:34:36.000000 mypy-boto3-location-1.26.78/mypy_boto3_location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-02-23 20:34:36.000000 mypy-boto3-location-1.26.78/mypy_boto3_location/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-02-23 20:34:36.000000 mypy-boto3-location-1.26.78/mypy_boto3_location/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45004 2023-02-23 20:34:36.000000 mypy-boto3-location-1.26.78/mypy_boto3_location/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    44929 2023-02-23 20:34:36.000000 mypy-boto3-location-1.26.78/mypy_boto3_location/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-02-23 20:34:36.000000 mypy-boto3-location-1.26.78/mypy_boto3_location/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-02-23 20:34:36.000000 mypy-boto3-location-1.26.78/mypy_boto3_location/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-02-23 20:34:36.000000 mypy-boto3-location-1.26.78/mypy_boto3_location/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-02-23 20:34:36.000000 mypy-boto3-location-1.26.78/mypy_boto3_location/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:36.000000 mypy-boto3-location-1.26.78/mypy_boto3_location/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    62800 2023-02-23 20:34:38.000000 mypy-boto3-location-1.26.78/mypy_boto3_location/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    62697 2023-02-23 20:34:38.000000 mypy-boto3-location-1.26.78/mypy_boto3_location/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-23 20:34:36.000000 mypy-boto3-location-1.26.78/mypy_boto3_location/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.320421 mypy-boto3-location-1.26.78/mypy_boto3_location.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21041 2023-02-23 20:34:57.000000 mypy-boto3-location-1.26.78/mypy_boto3_location.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-02-23 20:34:57.000000 mypy-boto3-location-1.26.78/mypy_boto3_location.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:34:57.000000 mypy-boto3-location-1.26.78/mypy_boto3_location.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:34:57.000000 mypy-boto3-location-1.26.78/mypy_boto3_location.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-23 20:34:57.000000 mypy-boto3-location-1.26.78/mypy_boto3_location.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-23 20:34:57.000000 mypy-boto3-location-1.26.78/mypy_boto3_location.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 20:34:57.320421 mypy-boto3-location-1.26.78/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-02-23 20:34:36.000000 mypy-boto3-location-1.26.78/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:27:21.143664 mypy-boto3-location-1.26.86/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-07 20:27:08.000000 mypy-boto3-location-1.26.86/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21041 2023-03-07 20:27:21.143664 mypy-boto3-location-1.26.86/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19543 2023-03-07 20:27:08.000000 mypy-boto3-location-1.26.86/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:27:21.135664 mypy-boto3-location-1.26.86/mypy_boto3_location/
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-03-07 20:27:08.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-03-07 20:27:08.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-07 20:27:08.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45004 2023-03-07 20:27:09.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44929 2023-03-07 20:27:08.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-03-07 20:27:09.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-03-07 20:27:09.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-03-07 20:27:09.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-03-07 20:27:09.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 20:27:08.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    62800 2023-03-07 20:27:11.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62697 2023-03-07 20:27:10.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-07 20:27:08.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:27:21.143664 mypy-boto3-location-1.26.86/mypy_boto3_location.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21041 2023-03-07 20:27:21.000000 mypy-boto3-location-1.26.86/mypy_boto3_location.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-07 20:27:21.000000 mypy-boto3-location-1.26.86/mypy_boto3_location.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 20:27:21.000000 mypy-boto3-location-1.26.86/mypy_boto3_location.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 20:27:21.000000 mypy-boto3-location-1.26.86/mypy_boto3_location.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-07 20:27:21.000000 mypy-boto3-location-1.26.86/mypy_boto3_location.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-07 20:27:21.000000 mypy-boto3-location-1.26.86/mypy_boto3_location.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 20:27:21.143664 mypy-boto3-location-1.26.86/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-07 20:27:08.000000 mypy-boto3-location-1.26.86/setup.py
```

### Comparing `mypy-boto3-location-1.26.78/LICENSE` & `mypy-boto3-location-1.26.86/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.26.78/PKG-INFO` & `mypy-boto3-location-1.26.86/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-location
-Version: 1.26.78
-Summary: Type annotations for boto3.LocationService 1.26.78 service generated with mypy-boto3-builder 7.12.4
+Version: 1.26.86
+Summary: Type annotations for boto3.LocationService 1.26.86 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-location?color=blue)](https://pypistats.org/packages/mypy-boto3-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LocationService 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[boto3.LocationService 1.26.86](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-location docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-location-1.26.78/README.md` & `mypy-boto3-location-1.26.86/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-location?color=blue)](https://pypistats.org/packages/mypy-boto3-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LocationService 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[boto3.LocationService 1.26.86](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-location docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-location-1.26.78/mypy_boto3_location/__init__.py` & `mypy-boto3-location-1.26.86/mypy_boto3_location/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.26.78/mypy_boto3_location/__init__.pyi` & `mypy-boto3-location-1.26.86/mypy_boto3_location/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.26.78/mypy_boto3_location/__main__.py` & `mypy-boto3-location-1.26.86/mypy_boto3_location/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LocationService 1.26.78\nVersion:         1.26.78\nBuilder"
-        " version: 7.12.4\nDocs:           "
+        "Type annotations for boto3.LocationService 1.26.86\nVersion:         1.26.86\nBuilder"
+        " version: 7.12.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.78")
+    print("1.26.86")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-location-1.26.78/mypy_boto3_location/client.py` & `mypy-boto3-location-1.26.86/mypy_boto3_location/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.26.78/mypy_boto3_location/client.pyi` & `mypy-boto3-location-1.26.86/mypy_boto3_location/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.26.78/mypy_boto3_location/literals.py` & `mypy-boto3-location-1.26.86/mypy_boto3_location/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,14 +227,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
```

### Comparing `mypy-boto3-location-1.26.78/mypy_boto3_location/literals.pyi` & `mypy-boto3-location-1.26.86/mypy_boto3_location/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -225,14 +225,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
```

### Comparing `mypy-boto3-location-1.26.78/mypy_boto3_location/paginator.py` & `mypy-boto3-location-1.26.86/mypy_boto3_location/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.26.78/mypy_boto3_location/paginator.pyi` & `mypy-boto3-location-1.26.86/mypy_boto3_location/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.26.78/mypy_boto3_location/type_defs.py` & `mypy-boto3-location-1.26.86/mypy_boto3_location/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.26.78/mypy_boto3_location/type_defs.pyi` & `mypy-boto3-location-1.26.86/mypy_boto3_location/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.26.78/mypy_boto3_location.egg-info/PKG-INFO` & `mypy-boto3-location-1.26.86/mypy_boto3_location.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-location
-Version: 1.26.78
-Summary: Type annotations for boto3.LocationService 1.26.78 service generated with mypy-boto3-builder 7.12.4
+Version: 1.26.86
+Summary: Type annotations for boto3.LocationService 1.26.86 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-location?color=blue)](https://pypistats.org/packages/mypy-boto3-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LocationService 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[boto3.LocationService 1.26.86](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-location docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-location-1.26.78/mypy_boto3_location.egg-info/SOURCES.txt` & `mypy-boto3-location-1.26.86/mypy_boto3_location.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.26.78/setup.py` & `mypy-boto3-location-1.26.86/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-location",
-    version="1.26.78",
+    version="1.26.86",
     packages=["mypy_boto3_location"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LocationService 1.26.78 service generated with"
-        " mypy-boto3-builder 7.12.4"
+        "Type annotations for boto3.LocationService 1.26.86 service generated with"
+        " mypy-boto3-builder 7.12.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

