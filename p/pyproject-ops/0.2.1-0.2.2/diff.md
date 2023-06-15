# Comparing `tmp/pyproject_ops-0.2.1.tar.gz` & `tmp/pyproject_ops-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject_ops-0.2.1.tar", last modified: Wed Jun 14 13:32:01 2023, max compression
+gzip compressed data, was "pyproject_ops-0.2.2.tar", last modified: Thu Jun 15 01:00:46 2023, max compression
```

## Comparing `pyproject_ops-0.2.1.tar` & `pyproject_ops-0.2.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 13:32:01.436212 pyproject_ops-0.2.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-23 02:11:51.000000 pyproject_ops-0.2.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1123 2023-05-23 02:11:51.000000 pyproject_ops-0.2.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      321 2023-05-23 02:11:51.000000 pyproject_ops-0.2.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)    10325 2023-06-14 13:32:01.435939 pyproject_ops-0.2.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     9171 2023-06-14 13:29:02.000000 pyproject_ops-0.2.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 13:32:01.432904 pyproject_ops-0.2.1/pyproject_ops/
--rw-r--r--   0 sanhehu    (501) staff       (20)      423 2023-06-03 06:48:33.000000 pyproject_ops-0.2.1/pyproject_ops/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-14 13:24:31.000000 pyproject_ops-0.2.1/pyproject_ops/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-03 05:51:29.000000 pyproject_ops-0.2.1/pyproject_ops/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5074 2023-06-14 13:23:51.000000 pyproject_ops-0.2.1/pyproject_ops/cli.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      163 2023-05-22 19:51:02.000000 pyproject_ops-0.2.1/pyproject_ops/compat.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 13:32:01.433719 pyproject_ops-0.2.1/pyproject_ops/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-23 02:11:51.000000 pyproject_ops-0.2.1/pyproject_ops/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      219 2023-04-27 16:12:50.000000 pyproject_ops-0.2.1/pyproject_ops/helpers.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      154 2023-05-23 00:56:49.000000 pyproject_ops-0.2.1/pyproject_ops/logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      144 2023-05-23 01:06:08.000000 pyproject_ops-0.2.1/pyproject_ops/operation_system.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1020 2023-06-03 06:39:10.000000 pyproject_ops-0.2.1/pyproject_ops/ops.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      657 2023-05-22 19:25:03.000000 pyproject_ops-0.2.1/pyproject_ops/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      470 2023-06-03 06:22:27.000000 pyproject_ops-0.2.1/pyproject_ops/pyproject_aws.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3885 2023-06-03 06:21:16.000000 pyproject_ops-0.2.1/pyproject_ops/pyproject_aws_lambda.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1305 2023-06-03 06:09:59.000000 pyproject_ops-0.2.1/pyproject_ops/pyproject_build.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1206 2023-06-03 06:02:21.000000 pyproject_ops-0.2.1/pyproject_ops/pyproject_config_management.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    13420 2023-06-03 05:59:35.000000 pyproject_ops-0.2.1/pyproject_ops/pyproject_deps.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3399 2023-06-03 05:59:07.000000 pyproject_ops-0.2.1/pyproject_ops/pyproject_docs.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    12633 2023-06-14 13:22:05.000000 pyproject_ops-0.2.1/pyproject_ops/pyproject_paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-06-03 06:38:24.000000 pyproject_ops-0.2.1/pyproject_ops/pyproject_publish.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2416 2023-06-14 13:23:14.000000 pyproject_ops-0.2.1/pyproject_ops/pyproject_tests.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1997 2023-06-03 05:56:13.000000 pyproject_ops-0.2.1/pyproject_ops/pyproject_venv.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 13:32:01.434133 pyproject_ops-0.2.1/pyproject_ops/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-05-22 19:25:03.000000 pyproject_ops-0.2.1/pyproject_ops/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-05-23 01:08:52.000000 pyproject_ops-0.2.1/pyproject_ops/tests/helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 13:32:01.435231 pyproject_ops-0.2.1/pyproject_ops/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-05-23 00:53:52.000000 pyproject_ops-0.2.1/pyproject_ops/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3224 2023-06-03 06:06:50.000000 pyproject_ops-0.2.1/pyproject_ops/vendor/build_dist.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1406 2023-06-03 06:50:12.000000 pyproject_ops-0.2.1/pyproject_ops/vendor/jsonutils.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    17911 2023-05-23 00:53:57.000000 pyproject_ops-0.2.1/pyproject_ops/vendor/nested_logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      469 2023-05-23 00:54:59.000000 pyproject_ops-0.2.1/pyproject_ops/vendor/os_platform.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-23 00:54:22.000000 pyproject_ops-0.2.1/pyproject_ops/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 13:32:01.433608 pyproject_ops-0.2.1/pyproject_ops.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)    10325 2023-06-14 13:32:01.000000 pyproject_ops-0.2.1/pyproject_ops.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1354 2023-06-14 13:32:01.000000 pyproject_ops-0.2.1/pyproject_ops.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-14 13:32:01.000000 pyproject_ops-0.2.1/pyproject_ops.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       49 2023-06-14 13:32:01.000000 pyproject_ops-0.2.1/pyproject_ops.egg-info/entry_points.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      253 2023-06-14 13:32:01.000000 pyproject_ops-0.2.1/pyproject_ops.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       14 2023-06-14 13:32:01.000000 pyproject_ops-0.2.1/pyproject_ops.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      943 2023-06-14 13:25:07.000000 pyproject_ops-0.2.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)       37 2023-05-23 02:30:18.000000 pyproject_ops-0.2.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      352 2023-05-23 02:18:02.000000 pyproject_ops-0.2.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-03 06:28:54.000000 pyproject_ops-0.2.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      400 2023-06-03 07:40:12.000000 pyproject_ops-0.2.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-03 07:42:45.000000 pyproject_ops-0.2.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-14 13:32:01.436258 pyproject_ops-0.2.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7839 2023-06-14 13:30:02.000000 pyproject_ops-0.2.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-14 13:32:01.435588 pyproject_ops-0.2.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      214 2023-06-03 07:45:37.000000 pyproject_ops-0.2.1/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1733 2023-06-03 07:14:18.000000 pyproject_ops-0.2.1/tests/test_pyproject_ops.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 01:00:46.810494 pyproject_ops-0.2.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-23 02:11:51.000000 pyproject_ops-0.2.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1123 2023-05-23 02:11:51.000000 pyproject_ops-0.2.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      321 2023-05-23 02:11:51.000000 pyproject_ops-0.2.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)    10325 2023-06-15 01:00:46.810310 pyproject_ops-0.2.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     9171 2023-06-14 13:29:02.000000 pyproject_ops-0.2.2/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 01:00:46.806795 pyproject_ops-0.2.2/pyproject_ops/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      423 2023-06-03 06:48:33.000000 pyproject_ops-0.2.2/pyproject_ops/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-15 00:58:08.000000 pyproject_ops-0.2.2/pyproject_ops/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-03 05:51:29.000000 pyproject_ops-0.2.2/pyproject_ops/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5122 2023-06-15 00:58:04.000000 pyproject_ops-0.2.2/pyproject_ops/cli.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      163 2023-05-22 19:51:02.000000 pyproject_ops-0.2.2/pyproject_ops/compat.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 01:00:46.807638 pyproject_ops-0.2.2/pyproject_ops/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-23 02:11:51.000000 pyproject_ops-0.2.2/pyproject_ops/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      219 2023-04-27 16:12:50.000000 pyproject_ops-0.2.2/pyproject_ops/helpers.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      154 2023-05-23 00:56:49.000000 pyproject_ops-0.2.2/pyproject_ops/logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      144 2023-05-23 01:06:08.000000 pyproject_ops-0.2.2/pyproject_ops/operation_system.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1020 2023-06-03 06:39:10.000000 pyproject_ops-0.2.2/pyproject_ops/ops.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      657 2023-05-22 19:25:03.000000 pyproject_ops-0.2.2/pyproject_ops/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      470 2023-06-03 06:22:27.000000 pyproject_ops-0.2.2/pyproject_ops/pyproject_aws.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3885 2023-06-03 06:21:16.000000 pyproject_ops-0.2.2/pyproject_ops/pyproject_aws_lambda.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1305 2023-06-03 06:09:59.000000 pyproject_ops-0.2.2/pyproject_ops/pyproject_build.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1206 2023-06-03 06:02:21.000000 pyproject_ops-0.2.2/pyproject_ops/pyproject_config_management.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    13420 2023-06-03 05:59:35.000000 pyproject_ops-0.2.2/pyproject_ops/pyproject_deps.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3399 2023-06-03 05:59:07.000000 pyproject_ops-0.2.2/pyproject_ops/pyproject_docs.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    12633 2023-06-14 13:22:05.000000 pyproject_ops-0.2.2/pyproject_ops/pyproject_paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-06-03 06:38:24.000000 pyproject_ops-0.2.2/pyproject_ops/pyproject_publish.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2416 2023-06-14 13:23:14.000000 pyproject_ops-0.2.2/pyproject_ops/pyproject_tests.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1997 2023-06-03 05:56:13.000000 pyproject_ops-0.2.2/pyproject_ops/pyproject_venv.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 01:00:46.808330 pyproject_ops-0.2.2/pyproject_ops/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-05-22 19:25:03.000000 pyproject_ops-0.2.2/pyproject_ops/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-05-23 01:08:52.000000 pyproject_ops-0.2.2/pyproject_ops/tests/helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 01:00:46.809573 pyproject_ops-0.2.2/pyproject_ops/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-05-23 00:53:52.000000 pyproject_ops-0.2.2/pyproject_ops/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3224 2023-06-03 06:06:50.000000 pyproject_ops-0.2.2/pyproject_ops/vendor/build_dist.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1406 2023-06-03 06:50:12.000000 pyproject_ops-0.2.2/pyproject_ops/vendor/jsonutils.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    17911 2023-05-23 00:53:57.000000 pyproject_ops-0.2.2/pyproject_ops/vendor/nested_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      469 2023-05-23 00:54:59.000000 pyproject_ops-0.2.2/pyproject_ops/vendor/os_platform.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-23 00:54:22.000000 pyproject_ops-0.2.2/pyproject_ops/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 01:00:46.807512 pyproject_ops-0.2.2/pyproject_ops.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)    10325 2023-06-15 01:00:46.000000 pyproject_ops-0.2.2/pyproject_ops.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1354 2023-06-15 01:00:46.000000 pyproject_ops-0.2.2/pyproject_ops.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-15 01:00:46.000000 pyproject_ops-0.2.2/pyproject_ops.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       49 2023-06-15 01:00:46.000000 pyproject_ops-0.2.2/pyproject_ops.egg-info/entry_points.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      253 2023-06-15 01:00:46.000000 pyproject_ops-0.2.2/pyproject_ops.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       14 2023-06-15 01:00:46.000000 pyproject_ops-0.2.2/pyproject_ops.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1226 2023-06-15 01:00:02.000000 pyproject_ops-0.2.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)       37 2023-05-23 02:30:18.000000 pyproject_ops-0.2.2/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      352 2023-05-23 02:18:02.000000 pyproject_ops-0.2.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-03 06:28:54.000000 pyproject_ops-0.2.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      400 2023-06-03 07:40:12.000000 pyproject_ops-0.2.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-15 00:58:31.000000 pyproject_ops-0.2.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-15 01:00:46.810539 pyproject_ops-0.2.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7839 2023-06-14 13:30:02.000000 pyproject_ops-0.2.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 01:00:46.810012 pyproject_ops-0.2.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      214 2023-06-03 07:45:37.000000 pyproject_ops-0.2.2/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1733 2023-06-03 07:14:18.000000 pyproject_ops-0.2.2/tests/test_pyproject_ops.py
```

### Comparing `pyproject_ops-0.2.1/LICENSE.txt` & `pyproject_ops-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.1/PKG-INFO` & `pyproject_ops-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyproject_ops
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python project Ops automation.
 Home-page: https://github.com/MacHu-GWU/pyproject_ops-project
-Download-URL: https://pypi.python.org/pypi/pyproject_ops/0.2.1#downloads
+Download-URL: https://pypi.python.org/pypi/pyproject_ops/0.2.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `pyproject_ops-0.2.1/README.rst` & `pyproject_ops-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.1/pyproject_ops/cli.py` & `pyproject_ops-0.2.2/pyproject_ops/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # -*- coding: utf-8 -*-
 
 import typing as T
-import json
 import dataclasses
 
 import fire
 from pathlib_mate import Path
 
 from .vendor.jsonutils import json_loads
 from .ops import PyProjectOps
@@ -198,13 +197,15 @@
         """
         pyops.view_latest_doc(bucket=pyops_config.doc_host_s3_bucket)
 
     def publish(self):
         """
         Publish package to PyPI
         """
+        pyops.pip_install()
+        pyops.pip_install_dev()
         pyops.python_build()
         pyops.twine_upload()
 
 
 def main():
     fire.Fire(Command)
```

### Comparing `pyproject_ops-0.2.1/pyproject_ops/ops.py` & `pyproject_ops-0.2.2/pyproject_ops/ops.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.1/pyproject_ops/paths.py` & `pyproject_ops-0.2.2/pyproject_ops/paths.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.1/pyproject_ops/pyproject_aws_lambda.py` & `pyproject_ops-0.2.2/pyproject_ops/pyproject_aws_lambda.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.1/pyproject_ops/pyproject_build.py` & `pyproject_ops-0.2.2/pyproject_ops/pyproject_build.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.1/pyproject_ops/pyproject_config_management.py` & `pyproject_ops-0.2.2/pyproject_ops/pyproject_config_management.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.1/pyproject_ops/pyproject_deps.py` & `pyproject_ops-0.2.2/pyproject_ops/pyproject_deps.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.1/pyproject_ops/pyproject_docs.py` & `pyproject_ops-0.2.2/pyproject_ops/pyproject_docs.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.1/pyproject_ops/pyproject_paths.py` & `pyproject_ops-0.2.2/pyproject_ops/pyproject_paths.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.1/pyproject_ops/pyproject_publish.py` & `pyproject_ops-0.2.2/pyproject_ops/pyproject_publish.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.1/pyproject_ops/pyproject_tests.py` & `pyproject_ops-0.2.2/pyproject_ops/pyproject_tests.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.1/pyproject_ops/pyproject_venv.py` & `pyproject_ops-0.2.2/pyproject_ops/pyproject_venv.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.1/pyproject_ops/vendor/build_dist.py` & `pyproject_ops-0.2.2/pyproject_ops/vendor/build_dist.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.1/pyproject_ops/vendor/jsonutils.py` & `pyproject_ops-0.2.2/pyproject_ops/vendor/jsonutils.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.1/pyproject_ops/vendor/nested_logger.py` & `pyproject_ops-0.2.2/pyproject_ops/vendor/nested_logger.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.1/pyproject_ops/vendor/pytest_cov_helper.py` & `pyproject_ops-0.2.2/pyproject_ops/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.1/pyproject_ops.egg-info/PKG-INFO` & `pyproject_ops-0.2.2/pyproject_ops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyproject-ops
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python project Ops automation.
 Home-page: https://github.com/MacHu-GWU/pyproject_ops-project
-Download-URL: https://pypi.python.org/pypi/pyproject_ops/0.2.1#downloads
+Download-URL: https://pypi.python.org/pypi/pyproject_ops/0.2.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `pyproject_ops-0.2.1/pyproject_ops.egg-info/SOURCES.txt` & `pyproject_ops-0.2.2/pyproject_ops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.1/release-history.rst` & `pyproject_ops-0.2.2/release-history.rst`

 * *Files 24% similar despite different names*

```diff
@@ -11,14 +11,25 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.2.2 (2023-06-14)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Bugfixes**
+
+- fix a bug that ``pyops publish`` command forget to install dev dependencies.
+
+**Miscellaneous**
+
+- loosen the ``fire`` dependency version requirements to ``>=0.1.3``.
+
+
 0.2.1 (2023-06-14)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - add ``pyops view-cov`` command to view coverage test output html file locally in web browser.
```

### Comparing `pyproject_ops-0.2.1/requirements-doc.txt` & `pyproject_ops-0.2.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.1/setup.py` & `pyproject_ops-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.1/tests/test_pyproject_ops.py` & `pyproject_ops-0.2.2/tests/test_pyproject_ops.py`

 * *Files identical despite different names*

