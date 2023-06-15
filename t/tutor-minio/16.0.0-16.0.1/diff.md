# Comparing `tmp/tutor-minio-16.0.0.tar.gz` & `tmp/tutor-minio-16.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-minio-16.0.0.tar", last modified: Wed Jun 14 23:00:08 2023, max compression
+gzip compressed data, was "tutor-minio-16.0.1.tar", last modified: Thu Jun 15 01:38:21 2023, max compression
```

## Comparing `tutor-minio-16.0.0.tar` & `tutor-minio-16.0.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:00:08.139840 tutor-minio-16.0.0/
--rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/LICENSE.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       79 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     4259 2023-06-14 23:00:08.136507 tutor-minio-16.0.0/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     3210 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/pyproject.toml
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-14 23:00:08.139840 tutor-minio-16.0.0/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1698 2023-06-14 23:00:00.000000 tutor-minio-16.0.0/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:00:08.123173 tutor-minio-16.0.0/tutor_minio.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     4259 2023-06-14 23:00:08.000000 tutor-minio-16.0.0/tutor_minio.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     1158 2023-06-14 23:00:08.000000 tutor-minio-16.0.0/tutor_minio.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-06-14 23:00:08.000000 tutor-minio-16.0.0/tutor_minio.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       44 2023-06-14 23:00:08.000000 tutor-minio-16.0.0/tutor_minio.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-06-14 23:00:08.000000 tutor-minio-16.0.0/tutor_minio.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       11 2023-06-14 23:00:08.000000 tutor-minio-16.0.0/tutor_minio.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:00:08.126507 tutor-minio-16.0.0/tutorminio/
--rw-r--r--   0 ci        (1000) ci        (1000)      175 2023-06-14 23:00:00.000000 tutor-minio-16.0.0/tutorminio/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:00:08.136507 tutor-minio-16.0.0/tutorminio/patches/
--rw-r--r--   0 ci        (1000) ci        (1000)      158 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)     1223 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/k8s-deployments
--rw-r--r--   0 ci        (1000) ci        (1000)      474 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/k8s-jobs
--rw-r--r--   0 ci        (1000) ci        (1000)      260 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/k8s-services
--rw-r--r--   0 ci        (1000) ci        (1000)      281 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/k8s-volumes
--rw-r--r--   0 ci        (1000) ci        (1000)       21 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/local-docker-compose-caddy-aliases
--rw-r--r--   0 ci        (1000) ci        (1000)        7 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/local-docker-compose-cms-dependencies
--rw-r--r--   0 ci        (1000) ci        (1000)      141 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/local-docker-compose-dev-services
--rw-r--r--   0 ci        (1000) ci        (1000)      227 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/local-docker-compose-jobs-services
--rw-r--r--   0 ci        (1000) ci        (1000)        7 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/local-docker-compose-lms-dependencies
--rw-r--r--   0 ci        (1000) ci        (1000)      491 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/local-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)      103 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/openedx-auth
--rw-r--r--   0 ci        (1000) ci        (1000)       59 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/openedx-cms-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     1364 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/openedx-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)       90 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/openedx-development-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      313 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/openedx-lms-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      404 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/richie-settings-common
--rw-r--r--   0 ci        (1000) ci        (1000)      404 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/xqueue-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     2803 2023-06-14 22:59:52.000000 tutor-minio-16.0.0/tutorminio/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:00:08.119840 tutor-minio-16.0.0/tutorminio/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:00:08.119840 tutor-minio-16.0.0/tutorminio/templates/minio/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:00:08.119840 tutor-minio-16.0.0/tutorminio/templates/minio/tasks/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:00:08.136507 tutor-minio-16.0.0/tutorminio/templates/minio/tasks/minio/
--rw-r--r--   0 ci        (1000) ci        (1000)      563 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/templates/minio/tasks/minio/init.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 01:38:21.361015 tutor-minio-16.0.1/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       79 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     4259 2023-06-15 01:38:21.361015 tutor-minio-16.0.1/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     3210 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/pyproject.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-15 01:38:21.361015 tutor-minio-16.0.1/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1698 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 01:38:21.341015 tutor-minio-16.0.1/tutor_minio.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     4259 2023-06-15 01:38:21.000000 tutor-minio-16.0.1/tutor_minio.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     1158 2023-06-15 01:38:21.000000 tutor-minio-16.0.1/tutor_minio.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-06-15 01:38:21.000000 tutor-minio-16.0.1/tutor_minio.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       44 2023-06-15 01:38:21.000000 tutor-minio-16.0.1/tutor_minio.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-06-15 01:38:21.000000 tutor-minio-16.0.1/tutor_minio.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       11 2023-06-15 01:38:21.000000 tutor-minio-16.0.1/tutor_minio.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 01:38:21.341015 tutor-minio-16.0.1/tutorminio/
+-rw-r--r--   0 ci        (1000) ci        (1000)      175 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 01:38:21.354349 tutor-minio-16.0.1/tutorminio/patches/
+-rw-r--r--   0 ci        (1000) ci        (1000)      158 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/patches/caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)     1223 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/patches/k8s-deployments
+-rw-r--r--   0 ci        (1000) ci        (1000)      474 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/patches/k8s-jobs
+-rw-r--r--   0 ci        (1000) ci        (1000)      260 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/patches/k8s-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      281 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/patches/k8s-volumes
+-rw-r--r--   0 ci        (1000) ci        (1000)       21 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/patches/local-docker-compose-caddy-aliases
+-rw-r--r--   0 ci        (1000) ci        (1000)        7 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/patches/local-docker-compose-cms-dependencies
+-rw-r--r--   0 ci        (1000) ci        (1000)      141 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/patches/local-docker-compose-dev-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      227 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 ci        (1000) ci        (1000)        7 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/patches/local-docker-compose-lms-dependencies
+-rw-r--r--   0 ci        (1000) ci        (1000)      491 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/patches/local-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      103 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/patches/openedx-auth
+-rw-r--r--   0 ci        (1000) ci        (1000)       59 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/patches/openedx-cms-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)     1364 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/patches/openedx-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)       90 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/patches/openedx-development-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      313 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/patches/openedx-lms-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      404 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/patches/richie-settings-common
+-rw-r--r--   0 ci        (1000) ci        (1000)      404 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/patches/xqueue-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)     2839 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 01:38:21.334349 tutor-minio-16.0.1/tutorminio/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 01:38:21.334349 tutor-minio-16.0.1/tutorminio/templates/minio/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 01:38:21.337682 tutor-minio-16.0.1/tutorminio/templates/minio/tasks/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 01:38:21.354349 tutor-minio-16.0.1/tutorminio/templates/minio/tasks/minio/
+-rw-r--r--   0 ci        (1000) ci        (1000)      563 2023-06-15 01:38:10.000000 tutor-minio-16.0.1/tutorminio/templates/minio/tasks/minio/init.sh
```

### Comparing `tutor-minio-16.0.0/LICENSE.txt` & `tutor-minio-16.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutor-minio-16.0.0/PKG-INFO` & `tutor-minio-16.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-minio
-Version: 16.0.0
+Version: 16.0.1
 Summary: A Tutor plugin for object storage in MinIO
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: Overhang.IO
 Maintainer-email: regis@overhang.io
 License: AGPLv3
```

### Comparing `tutor-minio-16.0.0/README.rst` & `tutor-minio-16.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-minio-16.0.0/setup.py` & `tutor-minio-16.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-minio-16.0.0/tutor_minio.egg-info/PKG-INFO` & `tutor-minio-16.0.1/tutor_minio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-minio
-Version: 16.0.0
+Version: 16.0.1
 Summary: A Tutor plugin for object storage in MinIO
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: Overhang.IO
 Maintainer-email: regis@overhang.io
 License: AGPLv3
```

### Comparing `tutor-minio-16.0.0/tutor_minio.egg-info/SOURCES.txt` & `tutor-minio-16.0.1/tutor_minio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tutor-minio-16.0.0/tutorminio/patches/k8s-deployments` & `tutor-minio-16.0.1/tutorminio/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-minio-16.0.0/tutorminio/patches/openedx-common-settings` & `tutor-minio-16.0.1/tutorminio/patches/openedx-common-settings`

 * *Files identical despite different names*

### Comparing `tutor-minio-16.0.0/tutorminio/plugin.py` & `tutor-minio-16.0.1/tutorminio/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 from glob import glob
 from typing import Literal
 
 import pkg_resources
 
 from tutor import hooks as tutor_hooks
```

### Comparing `tutor-minio-16.0.0/tutorminio/templates/minio/tasks/minio/init.sh` & `tutor-minio-16.0.1/tutorminio/templates/minio/tasks/minio/init.sh`

 * *Files identical despite different names*

