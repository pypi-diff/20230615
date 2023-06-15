# Comparing `tmp/mypy-boto3-efs-1.26.52.tar.gz` & `tmp/mypy-boto3-efs-1.26.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-efs-1.26.52.tar", last modified: Wed Jan 18 21:22:51 2023, max compression
+gzip compressed data, was "mypy-boto3-efs-1.26.72.tar", last modified: Wed Feb 15 22:27:56 2023, max compression
```

## Comparing `mypy-boto3-efs-1.26.52.tar` & `mypy-boto3-efs-1.26.72.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 21:22:51.428996 mypy-boto3-efs-1.26.52/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-18 21:22:36.000000 mypy-boto3-efs-1.26.52/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-01-18 21:22:51.428996 mypy-boto3-efs-1.26.52/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-01-18 21:22:36.000000 mypy-boto3-efs-1.26.52/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 21:22:51.428996 mypy-boto3-efs-1.26.52/mypy_boto3_efs/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-01-18 21:22:36.000000 mypy-boto3-efs-1.26.52/mypy_boto3_efs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-01-18 21:22:36.000000 mypy-boto3-efs-1.26.52/mypy_boto3_efs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-01-18 21:22:36.000000 mypy-boto3-efs-1.26.52/mypy_boto3_efs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23575 2023-01-18 21:22:36.000000 mypy-boto3-efs-1.26.52/mypy_boto3_efs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23535 2023-01-18 21:22:36.000000 mypy-boto3-efs-1.26.52/mypy_boto3_efs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-01-18 21:22:36.000000 mypy-boto3-efs-1.26.52/mypy_boto3_efs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-01-18 21:22:36.000000 mypy-boto3-efs-1.26.52/mypy_boto3_efs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-01-18 21:22:36.000000 mypy-boto3-efs-1.26.52/mypy_boto3_efs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-01-18 21:22:36.000000 mypy-boto3-efs-1.26.52/mypy_boto3_efs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 21:22:36.000000 mypy-boto3-efs-1.26.52/mypy_boto3_efs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24226 2023-01-18 21:22:36.000000 mypy-boto3-efs-1.26.52/mypy_boto3_efs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24197 2023-01-18 21:22:36.000000 mypy-boto3-efs-1.26.52/mypy_boto3_efs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-18 21:22:36.000000 mypy-boto3-efs-1.26.52/mypy_boto3_efs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 21:22:51.428996 mypy-boto3-efs-1.26.52/mypy_boto3_efs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-01-18 21:22:51.000000 mypy-boto3-efs-1.26.52/mypy_boto3_efs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-01-18 21:22:51.000000 mypy-boto3-efs-1.26.52/mypy_boto3_efs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 21:22:51.000000 mypy-boto3-efs-1.26.52/mypy_boto3_efs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 21:22:51.000000 mypy-boto3-efs-1.26.52/mypy_boto3_efs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-18 21:22:51.000000 mypy-boto3-efs-1.26.52/mypy_boto3_efs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-18 21:22:51.000000 mypy-boto3-efs-1.26.52/mypy_boto3_efs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-18 21:22:51.428996 mypy-boto3-efs-1.26.52/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-01-18 21:22:35.000000 mypy-boto3-efs-1.26.52/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.842126 mypy-boto3-efs-1.26.72/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-02-15 22:27:56.842126 mypy-boto3-efs-1.26.72/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.842126 mypy-boto3-efs-1.26.72/mypy_boto3_efs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23575 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23535 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9184 2023-02-15 22:27:06.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-02-15 22:27:06.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24226 2023-02-15 22:27:06.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24197 2023-02-15 22:27:06.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.842126 mypy-boto3-efs-1.26.72/mypy_boto3_efs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-02-15 22:27:56.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-15 22:27:56.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:27:56.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:27:56.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-15 22:27:56.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-15 22:27:56.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 22:27:56.842126 mypy-boto3-efs-1.26.72/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/setup.py
```

### Comparing `mypy-boto3-efs-1.26.52/LICENSE` & `mypy-boto3-efs-1.26.72/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.26.52/PKG-INFO` & `mypy-boto3-efs-1.26.72/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-efs
-Version: 1.26.52
-Summary: Type annotations for boto3.EFS 1.26.52 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.72
+Summary: Type annotations for boto3.EFS 1.26.72 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-efs.svg?color=blue)](https://pypi.org/project/mypy-boto3-efs)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-efs?color=blue)](https://pypistats.org/packages/mypy-boto3-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EFS 1.26.52](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
+[boto3.EFS 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-efs-1.26.52/README.md` & `mypy-boto3-efs-1.26.72/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-efs.svg?color=blue)](https://pypi.org/project/mypy-boto3-efs)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-efs?color=blue)](https://pypistats.org/packages/mypy-boto3-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EFS 1.26.52](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
+[boto3.EFS 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-efs-1.26.52/mypy_boto3_efs/__init__.py` & `mypy-boto3-efs-1.26.72/mypy_boto3_efs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.26.52/mypy_boto3_efs/__init__.pyi` & `mypy-boto3-efs-1.26.72/mypy_boto3_efs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.26.52/mypy_boto3_efs/__main__.py` & `mypy-boto3-efs-1.26.72/mypy_boto3_efs/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EFS 1.26.52\nVersion:         1.26.52\nBuilder version:"
+        "Type annotations for boto3.EFS 1.26.72\nVersion:         1.26.72\nBuilder version:"
         " 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.52")
+    print("1.26.72")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-efs-1.26.52/mypy_boto3_efs/client.py` & `mypy-boto3-efs-1.26.72/mypy_boto3_efs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.26.52/mypy_boto3_efs/client.pyi` & `mypy-boto3-efs-1.26.72/mypy_boto3_efs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.26.52/mypy_boto3_efs/literals.py` & `mypy-boto3-efs-1.26.72/mypy_boto3_efs/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -424,14 +425,15 @@
     "ap-southeast-2",
     "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-efs-1.26.52/mypy_boto3_efs/literals.pyi` & `mypy-boto3-efs-1.26.72/mypy_boto3_efs/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -108,14 +108,15 @@
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -422,14 +423,15 @@
     "ap-southeast-2",
     "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-efs-1.26.52/mypy_boto3_efs/paginator.py` & `mypy-boto3-efs-1.26.72/mypy_boto3_efs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.26.52/mypy_boto3_efs/paginator.pyi` & `mypy-boto3-efs-1.26.72/mypy_boto3_efs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.26.52/mypy_boto3_efs/type_defs.py` & `mypy-boto3-efs-1.26.72/mypy_boto3_efs/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.26.52/mypy_boto3_efs/type_defs.pyi` & `mypy-boto3-efs-1.26.72/mypy_boto3_efs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.26.52/mypy_boto3_efs.egg-info/PKG-INFO` & `mypy-boto3-efs-1.26.72/mypy_boto3_efs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-efs
-Version: 1.26.52
-Summary: Type annotations for boto3.EFS 1.26.52 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.72
+Summary: Type annotations for boto3.EFS 1.26.72 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-efs.svg?color=blue)](https://pypi.org/project/mypy-boto3-efs)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-efs?color=blue)](https://pypistats.org/packages/mypy-boto3-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EFS 1.26.52](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
+[boto3.EFS 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-efs-1.26.52/mypy_boto3_efs.egg-info/SOURCES.txt` & `mypy-boto3-efs-1.26.72/mypy_boto3_efs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.26.52/setup.py` & `mypy-boto3-efs-1.26.72/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-efs",
-    version="1.26.52",
+    version="1.26.72",
     packages=["mypy_boto3_efs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EFS 1.26.52 service generated with mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.EFS 1.26.72 service generated with mypy-boto3-builder 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

