# Comparing `tmp/tutor-minio-15.1.0.tar.gz` & `tmp/tutor-minio-16.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tutor-minio-15.1.0.tar", last modified: Mon Feb 27 10:45:00 2023, max compression
+gzip compressed data, was "tutor-minio-16.0.0.tar", last modified: Wed Jun 14 23:00:08 2023, max compression
```

## Comparing `tutor-minio-15.1.0.tar` & `tutor-minio-16.0.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-02-27 10:45:00.000000 tutor-minio-15.1.0/
--rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/LICENSE.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       79 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     4254 2023-02-27 10:45:00.000000 tutor-minio-15.1.0/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     3206 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-02-27 10:45:00.000000 tutor-minio-15.1.0/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1697 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-02-27 10:45:00.000000 tutor-minio-15.1.0/tutor_minio.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     4254 2023-02-27 10:45:00.000000 tutor-minio-15.1.0/tutor_minio.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     1143 2023-02-27 10:45:00.000000 tutor-minio-15.1.0/tutor_minio.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-02-27 10:45:00.000000 tutor-minio-15.1.0/tutor_minio.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       44 2023-02-27 10:45:00.000000 tutor-minio-15.1.0/tutor_minio.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-02-27 10:45:00.000000 tutor-minio-15.1.0/tutor_minio.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       11 2023-02-27 10:45:00.000000 tutor-minio-15.1.0/tutor_minio.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-02-27 10:45:00.000000 tutor-minio-15.1.0/tutorminio/
--rw-r--r--   0 ci        (1000) ci        (1000)       23 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-02-27 10:45:00.000000 tutor-minio-15.1.0/tutorminio/patches/
--rw-r--r--   0 ci        (1000) ci        (1000)      158 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/patches/caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)     1223 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/patches/k8s-deployments
--rw-r--r--   0 ci        (1000) ci        (1000)      474 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/patches/k8s-jobs
--rw-r--r--   0 ci        (1000) ci        (1000)      260 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/patches/k8s-services
--rw-r--r--   0 ci        (1000) ci        (1000)      281 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/patches/k8s-volumes
--rw-r--r--   0 ci        (1000) ci        (1000)       21 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/patches/local-docker-compose-caddy-aliases
--rw-r--r--   0 ci        (1000) ci        (1000)        7 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/patches/local-docker-compose-cms-dependencies
--rw-r--r--   0 ci        (1000) ci        (1000)      141 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/patches/local-docker-compose-dev-services
--rw-r--r--   0 ci        (1000) ci        (1000)      227 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/patches/local-docker-compose-jobs-services
--rw-r--r--   0 ci        (1000) ci        (1000)        7 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/patches/local-docker-compose-lms-dependencies
--rw-r--r--   0 ci        (1000) ci        (1000)      491 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/patches/local-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)      103 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/patches/openedx-auth
--rw-r--r--   0 ci        (1000) ci        (1000)       59 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/patches/openedx-cms-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     1364 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/patches/openedx-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)       90 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/patches/openedx-development-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      313 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/patches/openedx-lms-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      404 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/patches/richie-settings-common
--rw-r--r--   0 ci        (1000) ci        (1000)      404 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/patches/xqueue-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     2461 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-02-27 10:45:00.000000 tutor-minio-15.1.0/tutorminio/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-02-27 10:45:00.000000 tutor-minio-15.1.0/tutorminio/templates/minio/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-02-27 10:45:00.000000 tutor-minio-15.1.0/tutorminio/templates/minio/tasks/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-02-27 10:45:00.000000 tutor-minio-15.1.0/tutorminio/templates/minio/tasks/minio/
--rw-r--r--   0 ci        (1000) ci        (1000)      563 2023-02-27 10:44:51.000000 tutor-minio-15.1.0/tutorminio/templates/minio/tasks/minio/init.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:00:08.139840 tutor-minio-16.0.0/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       79 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     4259 2023-06-14 23:00:08.136507 tutor-minio-16.0.0/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     3210 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/pyproject.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-14 23:00:08.139840 tutor-minio-16.0.0/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1698 2023-06-14 23:00:00.000000 tutor-minio-16.0.0/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:00:08.123173 tutor-minio-16.0.0/tutor_minio.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     4259 2023-06-14 23:00:08.000000 tutor-minio-16.0.0/tutor_minio.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     1158 2023-06-14 23:00:08.000000 tutor-minio-16.0.0/tutor_minio.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-06-14 23:00:08.000000 tutor-minio-16.0.0/tutor_minio.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       44 2023-06-14 23:00:08.000000 tutor-minio-16.0.0/tutor_minio.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-06-14 23:00:08.000000 tutor-minio-16.0.0/tutor_minio.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       11 2023-06-14 23:00:08.000000 tutor-minio-16.0.0/tutor_minio.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:00:08.126507 tutor-minio-16.0.0/tutorminio/
+-rw-r--r--   0 ci        (1000) ci        (1000)      175 2023-06-14 23:00:00.000000 tutor-minio-16.0.0/tutorminio/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:00:08.136507 tutor-minio-16.0.0/tutorminio/patches/
+-rw-r--r--   0 ci        (1000) ci        (1000)      158 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)     1223 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/k8s-deployments
+-rw-r--r--   0 ci        (1000) ci        (1000)      474 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/k8s-jobs
+-rw-r--r--   0 ci        (1000) ci        (1000)      260 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/k8s-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      281 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/k8s-volumes
+-rw-r--r--   0 ci        (1000) ci        (1000)       21 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/local-docker-compose-caddy-aliases
+-rw-r--r--   0 ci        (1000) ci        (1000)        7 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/local-docker-compose-cms-dependencies
+-rw-r--r--   0 ci        (1000) ci        (1000)      141 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/local-docker-compose-dev-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      227 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 ci        (1000) ci        (1000)        7 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/local-docker-compose-lms-dependencies
+-rw-r--r--   0 ci        (1000) ci        (1000)      491 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/local-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      103 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/openedx-auth
+-rw-r--r--   0 ci        (1000) ci        (1000)       59 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/openedx-cms-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)     1364 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/openedx-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)       90 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/openedx-development-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      313 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/openedx-lms-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      404 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/richie-settings-common
+-rw-r--r--   0 ci        (1000) ci        (1000)      404 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/patches/xqueue-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)     2803 2023-06-14 22:59:52.000000 tutor-minio-16.0.0/tutorminio/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:00:08.119840 tutor-minio-16.0.0/tutorminio/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:00:08.119840 tutor-minio-16.0.0/tutorminio/templates/minio/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:00:08.119840 tutor-minio-16.0.0/tutorminio/templates/minio/tasks/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:00:08.136507 tutor-minio-16.0.0/tutorminio/templates/minio/tasks/minio/
+-rw-r--r--   0 ci        (1000) ci        (1000)      563 2023-06-14 22:59:42.000000 tutor-minio-16.0.0/tutorminio/templates/minio/tasks/minio/init.sh
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tutor-minio-15.1.0/LICENSE.txt` & `tutor-minio-16.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutor-minio-15.1.0/PKG-INFO` & `tutor-minio-16.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-minio
-Version: 15.1.0
+Version: 16.0.0
 Summary: A Tutor plugin for object storage in MinIO
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: Overhang.IO
 Maintainer-email: regis@overhang.io
 License: AGPLv3
@@ -13,34 +13,34 @@
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-minio/issues
 Project-URL: Community, https://discuss.openedx.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 
 Object storage for Open edX with `MinIO <https://www.minio.io/>`_
 =================================================================
 
 This is a plugin for `Tutor <https://docs.tutor.overhang.io>`_ that provides S3-like object storage for Open edX platforms. It's S3, but without the dependency on AWS. This is achieved thanks to `MinIO <https://www.minio.io/>`_, an open source project that provides object storage with an API compatible with S3.
 
 In particular, this plugin is essential for `Kubernetes deployment <https://docs.tutor.overhang.io/k8s.html>`_.
 
 Installation
 ------------
 
 The plugin is currently bundled with the `binary releases of Tutor <https://github.com/overhangio/tutor/releases>`_. If you have installed Tutor from source, you will have to install this plugin from source, too::
 
-    pip install tutor-minio
+    tutor plugins install minio
 
 Then, to enable this plugin, run::
 
     tutor plugins enable minio
 
 Configuration
 -------------
```

### Comparing `tutor-minio-15.1.0/README.rst` & `tutor-minio-16.0.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -44,158 +44,158 @@
 000002b0: 6f72 2f72 656c 6561 7365 733e 605f 2e20  or/releases>`_. 
 000002c0: 4966 2079 6f75 2068 6176 6520 696e 7374  If you have inst
 000002d0: 616c 6c65 6420 5475 746f 7220 6672 6f6d  alled Tutor from
 000002e0: 2073 6f75 7263 652c 2079 6f75 2077 696c   source, you wil
 000002f0: 6c20 6861 7665 2074 6f20 696e 7374 616c  l have to instal
 00000300: 6c20 7468 6973 2070 6c75 6769 6e20 6672  l this plugin fr
 00000310: 6f6d 2073 6f75 7263 652c 2074 6f6f 3a3a  om source, too::
-00000320: 0a0a 2020 2020 7069 7020 696e 7374 616c  ..    pip instal
-00000330: 6c20 7475 746f 722d 6d69 6e69 6f0a 0a54  l tutor-minio..T
-00000340: 6865 6e2c 2074 6f20 656e 6162 6c65 2074  hen, to enable t
-00000350: 6869 7320 706c 7567 696e 2c20 7275 6e3a  his plugin, run:
-00000360: 3a0a 0a20 2020 2074 7574 6f72 2070 6c75  :..    tutor plu
-00000370: 6769 6e73 2065 6e61 626c 6520 6d69 6e69  gins enable mini
-00000380: 6f0a 0a43 6f6e 6669 6775 7261 7469 6f6e  o..Configuration
-00000390: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  .-------------..
-000003a0: 2d20 6060 4f50 454e 4544 585f 4157 535f  - ``OPENEDX_AWS_
-000003b0: 4143 4345 5353 5f4b 4559 6060 2028 6465  ACCESS_KEY`` (de
-000003c0: 6661 756c 743a 2060 6022 6f70 656e 6564  fault: ``"opened
-000003d0: 7822 6060 290a 2d20 6060 4f50 454e 4544  x"``).- ``OPENED
-000003e0: 585f 4157 535f 5345 4352 4554 5f41 4343  X_AWS_SECRET_ACC
-000003f0: 4553 535f 4b45 5960 6020 2864 6566 6175  ESS_KEY`` (defau
-00000400: 6c74 3a20 6060 227b 7b20 3234 7c72 616e  lt: ``"{{ 24|ran
-00000410: 646f 6d5f 7374 7269 6e67 207d 7d22 6060  dom_string }}"``
-00000420: 290a 2d20 6060 4d49 4e49 4f5f 4255 434b  ).- ``MINIO_BUCK
-00000430: 4554 5f4e 414d 4560 6020 2864 6566 6175  ET_NAME`` (defau
-00000440: 6c74 3a20 6060 226f 7065 6e65 6478 2260  lt: ``"openedx"`
-00000450: 6029 0a2d 2060 604d 494e 494f 5f46 494c  `).- ``MINIO_FIL
-00000460: 455f 5550 4c4f 4144 5f42 5543 4b45 545f  E_UPLOAD_BUCKET_
-00000470: 4e41 4d45 6060 2028 6465 6661 756c 743a  NAME`` (default:
-00000480: 2060 6022 6f70 656e 6564 7875 706c 6f61   ``"openedxuploa
-00000490: 6473 2260 6029 0a2d 2060 604d 494e 494f  ds"``).- ``MINIO
-000004a0: 5f48 4f53 5460 6020 2864 6566 6175 6c74  _HOST`` (default
-000004b0: 3a20 6060 2266 696c 6573 2e7b 7b20 4c4d  : ``"files.{{ LM
-000004c0: 535f 484f 5354 207d 7d22 6060 290a 2d20  S_HOST }}"``).- 
-000004d0: 6060 4d49 4e49 4f5f 434f 4e53 4f4c 455f  ``MINIO_CONSOLE_
-000004e0: 484f 5354 6060 2028 6465 6661 756c 743a  HOST`` (default:
-000004f0: 2060 6022 6d69 6e69 6f2e 7b7b 204c 4d53   ``"minio.{{ LMS
-00000500: 5f48 4f53 5420 7d7d 2260 6029 0a2d 2060  _HOST }}"``).- `
-00000510: 604d 494e 494f 5f44 4f43 4b45 525f 494d  `MINIO_DOCKER_IM
-00000520: 4147 4560 6020 2864 6566 6175 6c74 3a20  AGE`` (default: 
-00000530: 6060 2264 6f63 6b65 722e 696f 2f6d 696e  ``"docker.io/min
-00000540: 696f 2f6d 696e 696f 3a52 454c 4541 5345  io/minio:RELEASE
-00000550: 2e32 3032 322d 3035 2d30 3854 3233 2d35  .2022-05-08T23-5
-00000560: 302d 3331 5a22 6060 290a 2d20 6060 4d49  0-31Z"``).- ``MI
-00000570: 4e49 4f5f 4d43 5f44 4f43 4b45 525f 494d  NIO_MC_DOCKER_IM
-00000580: 4147 4560 6020 2864 6566 6175 6c74 3a20  AGE`` (default: 
-00000590: 6060 2264 6f63 6b65 722e 696f 2f6d 696e  ``"docker.io/min
-000005a0: 696f 2f6d 633a 5245 4c45 4153 452e 3230  io/mc:RELEASE.20
-000005b0: 3232 2d30 352d 3039 5430 342d 3038 2d32  22-05-09T04-08-2
-000005c0: 365a 2260 6029 0a0a 5468 6573 6520 7661  6Z"``)..These va
-000005d0: 6c75 6573 2063 616e 2062 6520 6d6f 6469  lues can be modi
-000005e0: 6669 6564 2077 6974 6820 6060 7475 746f  fied with ``tuto
-000005f0: 7220 636f 6e66 6967 2073 6176 6520 2d2d  r config save --
-00000600: 7365 7420 5041 5241 4d5f 4e41 4d45 3d56  set PARAM_NAME=V
-00000610: 414c 5545 6060 2063 6f6d 6d61 6e64 732e  ALUE`` commands.
-00000620: 0a0a 2d20 6060 4d49 4e49 4f5f 4741 5445  ..- ``MINIO_GATE
-00000630: 5741 5960 6020 2864 6566 6175 6c74 3a20  WAY`` (default: 
-00000640: 6060 6e75 6c6c 6060 290a 0a54 6869 7320  ``null``)..This 
-00000650: 6665 6174 7572 6520 616c 6c6f 7773 2079  feature allows y
-00000660: 6f75 7220 746f 2072 756e 2074 6865 204d  our to run the M
-00000670: 696e 494f 2073 6572 7665 7220 6173 2061  inIO server as a
-00000680: 2067 6174 6577 6179 2074 6f20 616e 6f74   gateway to anot
-00000690: 6865 7220 6f62 6a65 6374 2073 746f 7261  her object stora
-000006a0: 6765 2073 6f6c 7574 696f 6e2c 2073 7563  ge solution, suc
-000006b0: 6820 6173 2060 5333 203c 6874 7470 733a  h as `S3 <https:
-000006c0: 2f2f 646f 6373 2e6d 696e 696f 2e69 6f2f  //docs.minio.io/
-000006d0: 646f 6373 2f6d 696e 696f 2d67 6174 6577  docs/minio-gatew
-000006e0: 6179 2d66 6f72 2d73 332e 6874 6d6c 3e60  ay-for-s3.html>`
-000006f0: 5f5f 206f 7220 6041 7a75 7265 203c 6874  __ or `Azure <ht
-00000700: 7470 733a 2f2f 646f 6373 2e6d 696e 696f  tps://docs.minio
-00000710: 2e69 6f2f 646f 6373 2f6d 696e 696f 2d67  .io/docs/minio-g
-00000720: 6174 6577 6179 2d66 6f72 2d61 7a75 7265  ateway-for-azure
-00000730: 2e68 746d 6c3e 605f 5f2e 2054 6861 7420  .html>`__. That 
-00000740: 7761 792c 2073 7461 7469 6320 6173 7365  way, static asse
-00000750: 7473 2063 616e 2062 6520 7374 6f72 6564  ts can be stored
-00000760: 206f 6e20 7468 6573 6520 6f62 6a65 6374   on these object
-00000770: 2073 746f 7261 6765 2062 6163 6b65 6e64   storage backend
-00000780: 7320 7769 7468 6f75 7420 6578 7465 6e73  s without extens
-00000790: 6976 6520 6368 616e 6765 7320 746f 2074  ive changes to t
-000007a0: 6865 204f 7065 6e20 6564 5820 7275 6e74  he Open edX runt
-000007b0: 696d 6520 656e 7669 726f 6e6d 656e 742e  ime environment.
-000007c0: 0a0a 4e6f 7465 2074 6f20 417a 7572 6520  ..Note to Azure 
-000007d0: 7573 6572 733a 2079 6f75 2077 696c 6c20  users: you will 
-000007e0: 6861 7665 2074 6f20 6d61 6e75 616c 6c79  have to manually
-000007f0: 2067 7261 6e74 2070 7562 6c69 6320 6163   grant public ac
-00000800: 6365 7373 2072 6967 6874 7320 746f 2074  cess rights to t
-00000810: 6865 2060 604d 494e 494f 5f42 5543 4b45  he ``MINIO_BUCKE
-00000820: 545f 4e41 4d45 6060 2028 226f 7065 6e65  T_NAME`` ("opene
-00000830: 6478 2229 2062 7563 6b65 742e 0a0a 444e  dx") bucket...DN
-00000840: 5320 7265 636f 7264 730a 2d2d 2d2d 2d2d  S records.------
-00000850: 2d2d 2d2d 2d0a 0a49 7420 6973 2061 7373  -----..It is ass
-00000860: 756d 6564 2074 6861 7420 7468 6520 6060  umed that the ``
-00000870: 4d49 4e49 4f5f 484f 5354 6060 2044 4e53  MINIO_HOST`` DNS
-00000880: 2072 6563 6f72 6420 706f 696e 7473 2074   record points t
-00000890: 6f20 796f 7572 2073 6572 7665 722e 2057  o your server. W
-000008a0: 6865 6e20 7275 6e6e 696e 6720 4d69 6e49  hen running MinI
-000008b0: 4f20 6f6e 2079 6f75 7220 6c61 7074 6f70  O on your laptop
-000008c0: 2c20 7468 6520 4d69 6e49 4f20 5765 6220  , the MinIO Web 
-000008d0: 5549 2077 696c 6c20 6265 2061 7661 696c  UI will be avail
-000008e0: 6162 6c65 2061 7420 6874 7470 3a2f 2f6d  able at http://m
-000008f0: 696e 696f 2e6c 6f63 616c 2e6f 7665 7268  inio.local.overh
-00000900: 616e 672e 696f 2e20 496e 2064 6576 656c  ang.io. In devel
-00000910: 6f70 6d65 6e74 206d 6f64 652c 2074 6865  opment mode, the
-00000920: 204d 696e 494f 2069 6e74 6572 6661 6365   MinIO interface
-00000930: 2077 696c 6c20 6265 2061 7661 696c 6162   will be availab
-00000940: 6c65 2061 7420 6874 7470 3a2f 2f6d 696e  le at http://min
-00000950: 696f 2e6c 6f63 616c 2e6f 7665 7268 616e  io.local.overhan
-00000960: 672e 696f 3a39 3030 312e 0a0a 5765 6220  g.io:9001...Web 
-00000970: 5549 0a2d 2d2d 2d2d 2d0a 0a54 6865 204d  UI.------..The M
-00000980: 696e 494f 2077 6562 2055 4920 6361 6e20  inIO web UI can 
-00000990: 6265 2061 6363 6573 7365 6420 6174 2068  be accessed at h
-000009a0: 7474 703a 2f2f 3c4d 494e 494f 5f48 4f53  ttp://<MINIO_HOS
-000009b0: 543e 2e20 5468 6520 6372 6564 656e 7469  T>. The credenti
-000009c0: 616c 7320 666f 7220 6163 6365 7373 696e  als for accessin
-000009d0: 6720 7468 6520 5549 2063 616e 2062 6520  g the UI can be 
-000009e0: 6f62 7461 696e 6564 2077 6974 683a 3a0a  obtained with::.
-000009f0: 0a20 2074 7574 6f72 2063 6f6e 6669 6720  .  tutor config 
-00000a00: 7072 696e 7476 616c 7565 204f 5045 4e45  printvalue OPENE
-00000a10: 4458 5f41 5753 5f41 4343 4553 535f 4b45  DX_AWS_ACCESS_KE
-00000a20: 590a 2020 7475 746f 7220 636f 6e66 6967  Y.  tutor config
-00000a30: 2070 7269 6e74 7661 6c75 6520 4f50 454e   printvalue OPEN
-00000a40: 4544 585f 4157 535f 5345 4352 4554 5f41  EDX_AWS_SECRET_A
-00000a50: 4343 4553 535f 4b45 590a 0a54 726f 7562  CCESS_KEY..Troub
-00000a60: 6c65 7368 6f6f 7469 6e67 0a2d 2d2d 2d2d  leshooting.-----
-00000a70: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 5468 6973  ----------..This
-00000a80: 2054 7574 6f72 2070 6c75 6769 6e20 6973   Tutor plugin is
-00000a90: 206d 6169 6e74 6169 6e65 6420 6279 2052   maintained by R
-00000aa0: c3a9 6769 7320 4265 686d 6f20 6672 6f6d  ..gis Behmo from
-00000ab0: 2060 4f76 6572 6861 6e67 2e49 4f20 3c68   `Overhang.IO <h
-00000ac0: 7474 7073 3a2f 2f6f 7665 7268 616e 672e  ttps://overhang.
-00000ad0: 696f 3e60 5f5f 2e20 436f 6d6d 756e 6974  io>`__. Communit
-00000ae0: 7920 7375 7070 6f72 7420 6973 2061 7661  y support is ava
-00000af0: 696c 6162 6c65 2066 726f 6d20 7468 6520  ilable from the 
-00000b00: 6f66 6669 6369 616c 2060 4f70 656e 2065  official `Open e
-00000b10: 6458 2066 6f72 756d 203c 6874 7470 733a  dX forum <https:
-00000b20: 2f2f 6469 7363 7573 732e 6f70 656e 6564  //discuss.opened
-00000b30: 782e 6f72 673e 605f 5f2e 2044 6f20 796f  x.org>`__. Do yo
-00000b40: 7520 6e65 6564 2068 656c 7020 7769 7468  u need help with
-00000b50: 2074 6869 7320 706c 7567 696e 3f20 5365   this plugin? Se
-00000b60: 6520 7468 6520 6074 726f 7562 6c65 7368  e the `troublesh
-00000b70: 6f6f 7469 6e67 203c 6874 7470 733a 2f2f  ooting <https://
-00000b80: 646f 6373 2e74 7574 6f72 2e6f 7665 7268  docs.tutor.overh
-00000b90: 616e 672e 696f 2f74 726f 7562 6c65 7368  ang.io/troublesh
-00000ba0: 6f6f 7469 6e67 2e68 746d 6c3e 605f 5f20  ooting.html>`__ 
-00000bb0: 7365 6374 696f 6e20 6672 6f6d 2074 6865  section from the
-00000bc0: 2054 7574 6f72 2064 6f63 756d 656e 7461   Tutor documenta
-00000bd0: 7469 6f6e 2e0a 0a4c 6963 656e 7365 0a2d  tion...License.-
-00000be0: 2d2d 2d2d 2d2d 0a0a 5468 6973 2077 6f72  ------..This wor
-00000bf0: 6b20 6973 206c 6963 656e 7365 6420 756e  k is licensed un
-00000c00: 6465 7220 7468 6520 7465 726d 7320 6f66  der the terms of
-00000c10: 2074 6865 2060 474e 5520 4166 6665 726f   the `GNU Affero
-00000c20: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
-00000c30: 4c69 6365 6e73 6520 2841 4750 4c29 203c  License (AGPL) <
-00000c40: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000c50: 6f6d 2f6f 7665 7268 616e 6769 6f2f 7475  om/overhangio/tu
-00000c60: 746f 722d 6d69 6e69 6f2f 626c 6f62 2f6d  tor-minio/blob/m
-00000c70: 6173 7465 722f 4c49 4345 4e53 452e 7478  aster/LICENSE.tx
-00000c80: 743e 605f 2e0a                           t>`_..
+00000320: 0a0a 2020 2020 7475 746f 7220 706c 7567  ..    tutor plug
+00000330: 696e 7320 696e 7374 616c 6c20 6d69 6e69  ins install mini
+00000340: 6f0a 0a54 6865 6e2c 2074 6f20 656e 6162  o..Then, to enab
+00000350: 6c65 2074 6869 7320 706c 7567 696e 2c20  le this plugin, 
+00000360: 7275 6e3a 3a0a 0a20 2020 2074 7574 6f72  run::..    tutor
+00000370: 2070 6c75 6769 6e73 2065 6e61 626c 6520   plugins enable 
+00000380: 6d69 6e69 6f0a 0a43 6f6e 6669 6775 7261  minio..Configura
+00000390: 7469 6f6e 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  tion.-----------
+000003a0: 2d2d 0a0a 2d20 6060 4f50 454e 4544 585f  --..- ``OPENEDX_
+000003b0: 4157 535f 4143 4345 5353 5f4b 4559 6060  AWS_ACCESS_KEY``
+000003c0: 2028 6465 6661 756c 743a 2060 6022 6f70   (default: ``"op
+000003d0: 656e 6564 7822 6060 290a 2d20 6060 4f50  enedx"``).- ``OP
+000003e0: 454e 4544 585f 4157 535f 5345 4352 4554  ENEDX_AWS_SECRET
+000003f0: 5f41 4343 4553 535f 4b45 5960 6020 2864  _ACCESS_KEY`` (d
+00000400: 6566 6175 6c74 3a20 6060 227b 7b20 3234  efault: ``"{{ 24
+00000410: 7c72 616e 646f 6d5f 7374 7269 6e67 207d  |random_string }
+00000420: 7d22 6060 290a 2d20 6060 4d49 4e49 4f5f  }"``).- ``MINIO_
+00000430: 4255 434b 4554 5f4e 414d 4560 6020 2864  BUCKET_NAME`` (d
+00000440: 6566 6175 6c74 3a20 6060 226f 7065 6e65  efault: ``"opene
+00000450: 6478 2260 6029 0a2d 2060 604d 494e 494f  dx"``).- ``MINIO
+00000460: 5f46 494c 455f 5550 4c4f 4144 5f42 5543  _FILE_UPLOAD_BUC
+00000470: 4b45 545f 4e41 4d45 6060 2028 6465 6661  KET_NAME`` (defa
+00000480: 756c 743a 2060 6022 6f70 656e 6564 7875  ult: ``"openedxu
+00000490: 706c 6f61 6473 2260 6029 0a2d 2060 604d  ploads"``).- ``M
+000004a0: 494e 494f 5f48 4f53 5460 6020 2864 6566  INIO_HOST`` (def
+000004b0: 6175 6c74 3a20 6060 2266 696c 6573 2e7b  ault: ``"files.{
+000004c0: 7b20 4c4d 535f 484f 5354 207d 7d22 6060  { LMS_HOST }}"``
+000004d0: 290a 2d20 6060 4d49 4e49 4f5f 434f 4e53  ).- ``MINIO_CONS
+000004e0: 4f4c 455f 484f 5354 6060 2028 6465 6661  OLE_HOST`` (defa
+000004f0: 756c 743a 2060 6022 6d69 6e69 6f2e 7b7b  ult: ``"minio.{{
+00000500: 204c 4d53 5f48 4f53 5420 7d7d 2260 6029   LMS_HOST }}"``)
+00000510: 0a2d 2060 604d 494e 494f 5f44 4f43 4b45  .- ``MINIO_DOCKE
+00000520: 525f 494d 4147 4560 6020 2864 6566 6175  R_IMAGE`` (defau
+00000530: 6c74 3a20 6060 2264 6f63 6b65 722e 696f  lt: ``"docker.io
+00000540: 2f6d 696e 696f 2f6d 696e 696f 3a52 454c  /minio/minio:REL
+00000550: 4541 5345 2e32 3032 322d 3035 2d30 3854  EASE.2022-05-08T
+00000560: 3233 2d35 302d 3331 5a22 6060 290a 2d20  23-50-31Z"``).- 
+00000570: 6060 4d49 4e49 4f5f 4d43 5f44 4f43 4b45  ``MINIO_MC_DOCKE
+00000580: 525f 494d 4147 4560 6020 2864 6566 6175  R_IMAGE`` (defau
+00000590: 6c74 3a20 6060 2264 6f63 6b65 722e 696f  lt: ``"docker.io
+000005a0: 2f6d 696e 696f 2f6d 633a 5245 4c45 4153  /minio/mc:RELEAS
+000005b0: 452e 3230 3232 2d30 352d 3039 5430 342d  E.2022-05-09T04-
+000005c0: 3038 2d32 365a 2260 6029 0a0a 5468 6573  08-26Z"``)..Thes
+000005d0: 6520 7661 6c75 6573 2063 616e 2062 6520  e values can be 
+000005e0: 6d6f 6469 6669 6564 2077 6974 6820 6060  modified with ``
+000005f0: 7475 746f 7220 636f 6e66 6967 2073 6176  tutor config sav
+00000600: 6520 2d2d 7365 7420 5041 5241 4d5f 4e41  e --set PARAM_NA
+00000610: 4d45 3d56 414c 5545 6060 2063 6f6d 6d61  ME=VALUE`` comma
+00000620: 6e64 732e 0a0a 2d20 6060 4d49 4e49 4f5f  nds...- ``MINIO_
+00000630: 4741 5445 5741 5960 6020 2864 6566 6175  GATEWAY`` (defau
+00000640: 6c74 3a20 6060 6e75 6c6c 6060 290a 0a54  lt: ``null``)..T
+00000650: 6869 7320 6665 6174 7572 6520 616c 6c6f  his feature allo
+00000660: 7773 2079 6f75 7220 746f 2072 756e 2074  ws your to run t
+00000670: 6865 204d 696e 494f 2073 6572 7665 7220  he MinIO server 
+00000680: 6173 2061 2067 6174 6577 6179 2074 6f20  as a gateway to 
+00000690: 616e 6f74 6865 7220 6f62 6a65 6374 2073  another object s
+000006a0: 746f 7261 6765 2073 6f6c 7574 696f 6e2c  torage solution,
+000006b0: 2073 7563 6820 6173 2060 5333 203c 6874   such as `S3 <ht
+000006c0: 7470 733a 2f2f 646f 6373 2e6d 696e 696f  tps://docs.minio
+000006d0: 2e69 6f2f 646f 6373 2f6d 696e 696f 2d67  .io/docs/minio-g
+000006e0: 6174 6577 6179 2d66 6f72 2d73 332e 6874  ateway-for-s3.ht
+000006f0: 6d6c 3e60 5f5f 206f 7220 6041 7a75 7265  ml>`__ or `Azure
+00000700: 203c 6874 7470 733a 2f2f 646f 6373 2e6d   <https://docs.m
+00000710: 696e 696f 2e69 6f2f 646f 6373 2f6d 696e  inio.io/docs/min
+00000720: 696f 2d67 6174 6577 6179 2d66 6f72 2d61  io-gateway-for-a
+00000730: 7a75 7265 2e68 746d 6c3e 605f 5f2e 2054  zure.html>`__. T
+00000740: 6861 7420 7761 792c 2073 7461 7469 6320  hat way, static 
+00000750: 6173 7365 7473 2063 616e 2062 6520 7374  assets can be st
+00000760: 6f72 6564 206f 6e20 7468 6573 6520 6f62  ored on these ob
+00000770: 6a65 6374 2073 746f 7261 6765 2062 6163  ject storage bac
+00000780: 6b65 6e64 7320 7769 7468 6f75 7420 6578  kends without ex
+00000790: 7465 6e73 6976 6520 6368 616e 6765 7320  tensive changes 
+000007a0: 746f 2074 6865 204f 7065 6e20 6564 5820  to the Open edX 
+000007b0: 7275 6e74 696d 6520 656e 7669 726f 6e6d  runtime environm
+000007c0: 656e 742e 0a0a 4e6f 7465 2074 6f20 417a  ent...Note to Az
+000007d0: 7572 6520 7573 6572 733a 2079 6f75 2077  ure users: you w
+000007e0: 696c 6c20 6861 7665 2074 6f20 6d61 6e75  ill have to manu
+000007f0: 616c 6c79 2067 7261 6e74 2070 7562 6c69  ally grant publi
+00000800: 6320 6163 6365 7373 2072 6967 6874 7320  c access rights 
+00000810: 746f 2074 6865 2060 604d 494e 494f 5f42  to the ``MINIO_B
+00000820: 5543 4b45 545f 4e41 4d45 6060 2028 226f  UCKET_NAME`` ("o
+00000830: 7065 6e65 6478 2229 2062 7563 6b65 742e  penedx") bucket.
+00000840: 0a0a 444e 5320 7265 636f 7264 730a 2d2d  ..DNS records.--
+00000850: 2d2d 2d2d 2d2d 2d2d 2d0a 0a49 7420 6973  ---------..It is
+00000860: 2061 7373 756d 6564 2074 6861 7420 7468   assumed that th
+00000870: 6520 6060 4d49 4e49 4f5f 484f 5354 6060  e ``MINIO_HOST``
+00000880: 2044 4e53 2072 6563 6f72 6420 706f 696e   DNS record poin
+00000890: 7473 2074 6f20 796f 7572 2073 6572 7665  ts to your serve
+000008a0: 722e 2057 6865 6e20 7275 6e6e 696e 6720  r. When running 
+000008b0: 4d69 6e49 4f20 6f6e 2079 6f75 7220 6c61  MinIO on your la
+000008c0: 7074 6f70 2c20 7468 6520 4d69 6e49 4f20  ptop, the MinIO 
+000008d0: 5765 6220 5549 2077 696c 6c20 6265 2061  Web UI will be a
+000008e0: 7661 696c 6162 6c65 2061 7420 6874 7470  vailable at http
+000008f0: 3a2f 2f6d 696e 696f 2e6c 6f63 616c 2e6f  ://minio.local.o
+00000900: 7665 7268 616e 672e 696f 2e20 496e 2064  verhang.io. In d
+00000910: 6576 656c 6f70 6d65 6e74 206d 6f64 652c  evelopment mode,
+00000920: 2074 6865 204d 696e 494f 2069 6e74 6572   the MinIO inter
+00000930: 6661 6365 2077 696c 6c20 6265 2061 7661  face will be ava
+00000940: 696c 6162 6c65 2061 7420 6874 7470 3a2f  ilable at http:/
+00000950: 2f6d 696e 696f 2e6c 6f63 616c 2e6f 7665  /minio.local.ove
+00000960: 7268 616e 672e 696f 3a39 3030 312e 0a0a  rhang.io:9001...
+00000970: 5765 6220 5549 0a2d 2d2d 2d2d 2d0a 0a54  Web UI.------..T
+00000980: 6865 204d 696e 494f 2077 6562 2055 4920  he MinIO web UI 
+00000990: 6361 6e20 6265 2061 6363 6573 7365 6420  can be accessed 
+000009a0: 6174 2068 7474 703a 2f2f 3c4d 494e 494f  at http://<MINIO
+000009b0: 5f48 4f53 543e 2e20 5468 6520 6372 6564  _HOST>. The cred
+000009c0: 656e 7469 616c 7320 666f 7220 6163 6365  entials for acce
+000009d0: 7373 696e 6720 7468 6520 5549 2063 616e  ssing the UI can
+000009e0: 2062 6520 6f62 7461 696e 6564 2077 6974   be obtained wit
+000009f0: 683a 3a0a 0a20 2074 7574 6f72 2063 6f6e  h::..  tutor con
+00000a00: 6669 6720 7072 696e 7476 616c 7565 204f  fig printvalue O
+00000a10: 5045 4e45 4458 5f41 5753 5f41 4343 4553  PENEDX_AWS_ACCES
+00000a20: 535f 4b45 590a 2020 7475 746f 7220 636f  S_KEY.  tutor co
+00000a30: 6e66 6967 2070 7269 6e74 7661 6c75 6520  nfig printvalue 
+00000a40: 4f50 454e 4544 585f 4157 535f 5345 4352  OPENEDX_AWS_SECR
+00000a50: 4554 5f41 4343 4553 535f 4b45 590a 0a54  ET_ACCESS_KEY..T
+00000a60: 726f 7562 6c65 7368 6f6f 7469 6e67 0a2d  roubleshooting.-
+00000a70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
+00000a80: 5468 6973 2054 7574 6f72 2070 6c75 6769  This Tutor plugi
+00000a90: 6e20 6973 206d 6169 6e74 6169 6e65 6420  n is maintained 
+00000aa0: 6279 2052 c3a9 6769 7320 4265 686d 6f20  by R..gis Behmo 
+00000ab0: 6672 6f6d 2060 4f76 6572 6861 6e67 2e49  from `Overhang.I
+00000ac0: 4f20 3c68 7474 7073 3a2f 2f6f 7665 7268  O <https://overh
+00000ad0: 616e 672e 696f 3e60 5f5f 2e20 436f 6d6d  ang.io>`__. Comm
+00000ae0: 756e 6974 7920 7375 7070 6f72 7420 6973  unity support is
+00000af0: 2061 7661 696c 6162 6c65 2066 726f 6d20   available from 
+00000b00: 7468 6520 6f66 6669 6369 616c 2060 4f70  the official `Op
+00000b10: 656e 2065 6458 2066 6f72 756d 203c 6874  en edX forum <ht
+00000b20: 7470 733a 2f2f 6469 7363 7573 732e 6f70  tps://discuss.op
+00000b30: 656e 6564 782e 6f72 673e 605f 5f2e 2044  enedx.org>`__. D
+00000b40: 6f20 796f 7520 6e65 6564 2068 656c 7020  o you need help 
+00000b50: 7769 7468 2074 6869 7320 706c 7567 696e  with this plugin
+00000b60: 3f20 5365 6520 7468 6520 6074 726f 7562  ? See the `troub
+00000b70: 6c65 7368 6f6f 7469 6e67 203c 6874 7470  leshooting <http
+00000b80: 733a 2f2f 646f 6373 2e74 7574 6f72 2e6f  s://docs.tutor.o
+00000b90: 7665 7268 616e 672e 696f 2f74 726f 7562  verhang.io/troub
+00000ba0: 6c65 7368 6f6f 7469 6e67 2e68 746d 6c3e  leshooting.html>
+00000bb0: 605f 5f20 7365 6374 696f 6e20 6672 6f6d  `__ section from
+00000bc0: 2074 6865 2054 7574 6f72 2064 6f63 756d   the Tutor docum
+00000bd0: 656e 7461 7469 6f6e 2e0a 0a4c 6963 656e  entation...Licen
+00000be0: 7365 0a2d 2d2d 2d2d 2d2d 0a0a 5468 6973  se.-------..This
+00000bf0: 2077 6f72 6b20 6973 206c 6963 656e 7365   work is license
+00000c00: 6420 756e 6465 7220 7468 6520 7465 726d  d under the term
+00000c10: 7320 6f66 2074 6865 2060 474e 5520 4166  s of the `GNU Af
+00000c20: 6665 726f 2047 656e 6572 616c 2050 7562  fero General Pub
+00000c30: 6c69 6320 4c69 6365 6e73 6520 2841 4750  lic License (AGP
+00000c40: 4c29 203c 6874 7470 733a 2f2f 6769 7468  L) <https://gith
+00000c50: 7562 2e63 6f6d 2f6f 7665 7268 616e 6769  ub.com/overhangi
+00000c60: 6f2f 7475 746f 722d 6d69 6e69 6f2f 626c  o/tutor-minio/bl
+00000c70: 6f62 2f6d 6173 7465 722f 4c49 4345 4e53  ob/master/LICENS
+00000c80: 452e 7478 743e 605f 2e0a                 E.txt>`_..
```

### Comparing `tutor-minio-15.1.0/setup.py` & `tutor-minio-16.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,22 +28,22 @@
     author_email="contact@overhang.io",
     maintainer="Overhang.IO",
     maintainer_email="regis@overhang.io",
     description="A Tutor plugin for object storage in MinIO",
     long_description=readme,
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
-    python_requires=">=3.7",
-    install_requires=["tutor>=15.0.0,<16.0.0"],
+    python_requires=">=3.8",
+    install_requires=["tutor>=16.0.0,<17.0.0"],
     entry_points={"tutor.plugin.v1": ["minio = tutorminio.plugin"]},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `tutor-minio-15.1.0/tutor_minio.egg-info/PKG-INFO` & `tutor-minio-16.0.0/tutor_minio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-minio
-Version: 15.1.0
+Version: 16.0.0
 Summary: A Tutor plugin for object storage in MinIO
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: Overhang.IO
 Maintainer-email: regis@overhang.io
 License: AGPLv3
@@ -13,34 +13,34 @@
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-minio/issues
 Project-URL: Community, https://discuss.openedx.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 
 Object storage for Open edX with `MinIO <https://www.minio.io/>`_
 =================================================================
 
 This is a plugin for `Tutor <https://docs.tutor.overhang.io>`_ that provides S3-like object storage for Open edX platforms. It's S3, but without the dependency on AWS. This is achieved thanks to `MinIO <https://www.minio.io/>`_, an open source project that provides object storage with an API compatible with S3.
 
 In particular, this plugin is essential for `Kubernetes deployment <https://docs.tutor.overhang.io/k8s.html>`_.
 
 Installation
 ------------
 
 The plugin is currently bundled with the `binary releases of Tutor <https://github.com/overhangio/tutor/releases>`_. If you have installed Tutor from source, you will have to install this plugin from source, too::
 
-    pip install tutor-minio
+    tutor plugins install minio
 
 Then, to enable this plugin, run::
 
     tutor plugins enable minio
 
 Configuration
 -------------
```

### Comparing `tutor-minio-15.1.0/tutor_minio.egg-info/SOURCES.txt` & `tutor-minio-16.0.0/tutor_minio.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.py
 tutor_minio.egg-info/PKG-INFO
 tutor_minio.egg-info/SOURCES.txt
 tutor_minio.egg-info/dependency_links.txt
 tutor_minio.egg-info/entry_points.txt
 tutor_minio.egg-info/requires.txt
 tutor_minio.egg-info/top_level.txt
```

### Comparing `tutor-minio-15.1.0/tutorminio/patches/k8s-deployments` & `tutor-minio-16.0.0/tutorminio/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-minio-15.1.0/tutorminio/patches/openedx-common-settings` & `tutor-minio-16.0.0/tutorminio/patches/openedx-common-settings`

 * *Files identical despite different names*

### Comparing `tutor-minio-15.1.0/tutorminio/plugin.py` & `tutor-minio-16.0.0/tutorminio/plugin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 from glob import glob
+from typing import Literal
 
 import pkg_resources
 
 from tutor import hooks as tutor_hooks
 
 from .__about__ import __version__
 
@@ -40,14 +41,25 @@
 tutor_hooks.Filters.CONFIG_OVERRIDES.add_items(
     [
         ("OPENEDX_AWS_ACCESS_KEY", "openedx"),
         ("OPENEDX_AWS_SECRET_ACCESS_KEY", "{{ MINIO_AWS_SECRET_ACCESS_KEY }}"),
     ]
 )
 
+@tutor_hooks.Filters.APP_PUBLIC_HOSTS.add()
+def add_minio_hosts(
+    hosts: list[str], context_name: Literal["local", "dev"]
+    ) -> list[str]:
+    if context_name == "dev":
+        hosts.append("{{ MINIO_CONSOLE_HOST }}:9001")
+    else:
+        hosts.append("{{ MINIO_CONSOLE_HOST }}")
+        
+    return hosts
+
 # Add pre-init script as init task with high priority
 with open(
     os.path.join(HERE, "templates", "minio", "tasks", "minio", "init.sh"),
     encoding="utf-8",
 ) as fi:
     tutor_hooks.Filters.CLI_DO_INIT_TASKS.add_item(
         ("minio", fi.read()), priority=tutor_hooks.priorities.HIGH
```

### Comparing `tutor-minio-15.1.0/tutorminio/templates/minio/tasks/minio/init.sh` & `tutor-minio-16.0.0/tutorminio/templates/minio/tasks/minio/init.sh`

 * *Files identical despite different names*

