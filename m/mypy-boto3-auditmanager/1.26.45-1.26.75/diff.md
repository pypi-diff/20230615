# Comparing `tmp/mypy-boto3-auditmanager-1.26.45.tar.gz` & `tmp/mypy-boto3-auditmanager-1.26.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-auditmanager-1.26.45.tar", last modified: Fri Jan  6 20:32:17 2023, max compression
+gzip compressed data, was "mypy-boto3-auditmanager-1.26.75.tar", last modified: Mon Feb 20 20:25:59 2023, max compression
```

## Comparing `mypy-boto3-auditmanager-1.26.45.tar` & `mypy-boto3-auditmanager-1.26.75.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:32:17.790611 mypy-boto3-auditmanager-1.26.45/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-06 20:32:08.000000 mypy-boto3-auditmanager-1.26.45/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19481 2023-01-06 20:32:17.790611 mypy-boto3-auditmanager-1.26.45/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-01-06 20:32:08.000000 mypy-boto3-auditmanager-1.26.45/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:32:17.790611 mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-01-06 20:32:08.000000 mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-01-06 20:32:08.000000 mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-01-06 20:32:08.000000 mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42581 2023-01-06 20:32:08.000000 mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42514 2023-01-06 20:32:08.000000 mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10199 2023-01-06 20:32:09.000000 mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-01-06 20:32:08.000000 mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 20:32:08.000000 mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    56795 2023-01-06 20:32:09.000000 mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    56750 2023-01-06 20:32:09.000000 mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-06 20:32:08.000000 mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:32:17.790611 mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19481 2023-01-06 20:32:17.000000 mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-01-06 20:32:17.000000 mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 20:32:17.000000 mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 20:32:17.000000 mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-06 20:32:17.000000 mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-06 20:32:17.000000 mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-06 20:32:17.790611 mypy-boto3-auditmanager-1.26.45/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-01-06 20:32:08.000000 mypy-boto3-auditmanager-1.26.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 20:25:59.228019 mypy-boto3-auditmanager-1.26.75/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19481 2023-02-20 20:25:59.228019 mypy-boto3-auditmanager-1.26.75/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 20:25:59.228019 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42576 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42509 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    56795 2023-02-20 20:25:43.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56750 2023-02-20 20:25:42.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 20:25:59.228019 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19481 2023-02-20 20:25:59.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-02-20 20:25:59.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 20:25:59.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 20:25:59.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 20:25:59.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-20 20:25:59.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 20:25:59.228019 mypy-boto3-auditmanager-1.26.75/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/setup.py
```

### Comparing `mypy-boto3-auditmanager-1.26.45/LICENSE` & `mypy-boto3-auditmanager-1.26.75/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.26.45/PKG-INFO` & `mypy-boto3-auditmanager-1.26.75/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-auditmanager
-Version: 1.26.45
-Summary: Type annotations for boto3.AuditManager 1.26.45 service generated with mypy-boto3-builder 7.12.2
+Version: 1.26.75
+Summary: Type annotations for boto3.AuditManager 1.26.75 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-auditmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-auditmanager)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-auditmanager?color=blue)](https://pypistats.org/packages/mypy-boto3-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AuditManager 1.26.45](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
+[boto3.AuditManager 1.26.75](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-auditmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-auditmanager-1.26.45/README.md` & `mypy-boto3-auditmanager-1.26.75/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-auditmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-auditmanager)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-auditmanager?color=blue)](https://pypistats.org/packages/mypy-boto3-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AuditManager 1.26.45](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
+[boto3.AuditManager 1.26.75](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-auditmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager/__main__.py` & `mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AuditManager 1.26.45\nVersion:         1.26.45\nBuilder"
-        " version: 7.12.2\nDocs:           "
+        "Type annotations for boto3.AuditManager 1.26.75\nVersion:         1.26.75\nBuilder"
+        " version: 7.12.4\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.45")
+    print("1.26.75")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager/client.py` & `mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -827,15 +827,15 @@
         defaultAssessmentReportsDestination: AssessmentReportsDestinationTypeDef = ...,
         defaultProcessOwners: Sequence[RoleTypeDef] = ...,
         kmsKey: str = ...,
         evidenceFinderEnabled: bool = ...,
         deregistrationPolicy: DeregistrationPolicyTypeDef = ...
     ) -> UpdateSettingsResponseTypeDef:
         """
-        Updates Audit Manager settings for the current user account.
+        Updates Audit Manager settings for the current account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.update_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#update_settings)
         """
 
     def validate_assessment_report_integrity(
         self, *, s3RelativePath: str
```

### Comparing `mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager/client.pyi` & `mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -761,15 +761,15 @@
         defaultAssessmentReportsDestination: AssessmentReportsDestinationTypeDef = ...,
         defaultProcessOwners: Sequence[RoleTypeDef] = ...,
         kmsKey: str = ...,
         evidenceFinderEnabled: bool = ...,
         deregistrationPolicy: DeregistrationPolicyTypeDef = ...
     ) -> UpdateSettingsResponseTypeDef:
         """
-        Updates Audit Manager settings for the current user account.
+        Updates Audit Manager settings for the current account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.update_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#update_settings)
         """
     def validate_assessment_report_integrity(
         self, *, s3RelativePath: str
     ) -> ValidateAssessmentReportIntegrityResponseTypeDef:
```

### Comparing `mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager/literals.py` & `mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,24 +140,26 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
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
@@ -265,14 +267,15 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
```

### Comparing `mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager/literals.pyi` & `mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -138,24 +138,26 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
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
@@ -263,14 +265,15 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
```

### Comparing `mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager/type_defs.py` & `mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager/type_defs.pyi` & `mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager.egg-info/PKG-INFO` & `mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-auditmanager
-Version: 1.26.45
-Summary: Type annotations for boto3.AuditManager 1.26.45 service generated with mypy-boto3-builder 7.12.2
+Version: 1.26.75
+Summary: Type annotations for boto3.AuditManager 1.26.75 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-auditmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-auditmanager)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-auditmanager?color=blue)](https://pypistats.org/packages/mypy-boto3-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AuditManager 1.26.45](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
+[boto3.AuditManager 1.26.75](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-auditmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-auditmanager-1.26.45/mypy_boto3_auditmanager.egg-info/SOURCES.txt` & `mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.26.45/setup.py` & `mypy-boto3-auditmanager-1.26.75/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-auditmanager",
-    version="1.26.45",
+    version="1.26.75",
     packages=["mypy_boto3_auditmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AuditManager 1.26.45 service generated with mypy-boto3-builder"
-        " 7.12.2"
+        "Type annotations for boto3.AuditManager 1.26.75 service generated with mypy-boto3-builder"
+        " 7.12.4"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

