# Comparing `tmp/tutor-xqueue-15.0.1.tar.gz` & `tmp/tutor-xqueue-16.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tutor-xqueue-15.0.1.tar", last modified: Sun Mar 19 14:43:58 2023, max compression
+gzip compressed data, was "tutor-xqueue-16.0.0.tar", last modified: Thu Jun 15 00:19:06 2023, max compression
```

## Comparing `tutor-xqueue-15.0.1.tar` & `tutor-xqueue-16.0.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-19 14:43:58.000000 tutor-xqueue-15.0.1/
--rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-03-19 14:43:50.000000 tutor-xqueue-15.0.1/LICENSE.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       81 2023-03-19 14:43:50.000000 tutor-xqueue-15.0.1/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     6521 2023-03-19 14:43:58.000000 tutor-xqueue-15.0.1/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     5476 2023-03-19 14:43:50.000000 tutor-xqueue-15.0.1/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-03-19 14:43:58.000000 tutor-xqueue-15.0.1/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1714 2023-03-19 14:43:50.000000 tutor-xqueue-15.0.1/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-19 14:43:58.000000 tutor-xqueue-15.0.1/tutor_xqueue.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     6521 2023-03-19 14:43:58.000000 tutor-xqueue-15.0.1/tutor_xqueue.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)      914 2023-03-19 14:43:58.000000 tutor-xqueue-15.0.1/tutor_xqueue.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-03-19 14:43:58.000000 tutor-xqueue-15.0.1/tutor_xqueue.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       46 2023-03-19 14:43:58.000000 tutor-xqueue-15.0.1/tutor_xqueue.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       31 2023-03-19 14:43:58.000000 tutor-xqueue-15.0.1/tutor_xqueue.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       12 2023-03-19 14:43:58.000000 tutor-xqueue-15.0.1/tutor_xqueue.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-19 14:43:58.000000 tutor-xqueue-15.0.1/tutorxqueue/
--rw-r--r--   0 ci        (1000) ci        (1000)       23 2023-03-19 14:43:50.000000 tutor-xqueue-15.0.1/tutorxqueue/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-03-19 14:43:50.000000 tutor-xqueue-15.0.1/tutorxqueue/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-19 14:43:58.000000 tutor-xqueue-15.0.1/tutorxqueue/patches/
--rw-r--r--   0 ci        (1000) ci        (1000)       82 2023-03-19 14:43:50.000000 tutor-xqueue-15.0.1/tutorxqueue/patches/caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)     1184 2023-03-19 14:43:50.000000 tutor-xqueue-15.0.1/tutorxqueue/patches/k8s-deployments
--rw-r--r--   0 ci        (1000) ci        (1000)      578 2023-03-19 14:43:50.000000 tutor-xqueue-15.0.1/tutorxqueue/patches/k8s-jobs
--rw-r--r--   0 ci        (1000) ci        (1000)      173 2023-03-19 14:43:50.000000 tutor-xqueue-15.0.1/tutorxqueue/patches/k8s-services
--rw-r--r--   0 ci        (1000) ci        (1000)       76 2023-03-19 14:43:50.000000 tutor-xqueue-15.0.1/tutorxqueue/patches/kustomization-configmapgenerator
--rw-r--r--   0 ci        (1000) ci        (1000)       88 2023-03-19 14:43:50.000000 tutor-xqueue-15.0.1/tutorxqueue/patches/local-docker-compose-dev-services
--rw-r--r--   0 ci        (1000) ci        (1000)      221 2023-03-19 14:43:50.000000 tutor-xqueue-15.0.1/tutorxqueue/patches/local-docker-compose-jobs-services
--rw-r--r--   0 ci        (1000) ci        (1000)      967 2023-03-19 14:43:50.000000 tutor-xqueue-15.0.1/tutorxqueue/patches/local-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)      204 2023-03-19 14:43:50.000000 tutor-xqueue-15.0.1/tutorxqueue/patches/openedx-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     7949 2023-03-19 14:43:50.000000 tutor-xqueue-15.0.1/tutorxqueue/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-19 14:43:58.000000 tutor-xqueue-15.0.1/tutorxqueue/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-19 14:43:58.000000 tutor-xqueue-15.0.1/tutorxqueue/templates/xqueue/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-19 14:43:58.000000 tutor-xqueue-15.0.1/tutorxqueue/templates/xqueue/apps/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-19 14:43:58.000000 tutor-xqueue-15.0.1/tutorxqueue/templates/xqueue/apps/settings/
--rw-r--r--   0 ci        (1000) ci        (1000)      956 2023-03-19 14:43:50.000000 tutor-xqueue-15.0.1/tutorxqueue/templates/xqueue/apps/settings/tutor.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-19 14:43:58.000000 tutor-xqueue-15.0.1/tutorxqueue/templates/xqueue/build/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-19 14:43:58.000000 tutor-xqueue-15.0.1/tutorxqueue/templates/xqueue/build/xqueue/
--rw-r--r--   0 ci        (1000) ci        (1000)      909 2023-03-19 14:43:50.000000 tutor-xqueue-15.0.1/tutorxqueue/templates/xqueue/build/xqueue/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-19 14:43:58.000000 tutor-xqueue-15.0.1/tutorxqueue/templates/xqueue/tasks/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-19 14:43:58.000000 tutor-xqueue-15.0.1/tutorxqueue/templates/xqueue/tasks/mysql/
--rw-r--r--   0 ci        (1000) ci        (1000)      803 2023-03-19 14:43:50.000000 tutor-xqueue-15.0.1/tutorxqueue/templates/xqueue/tasks/mysql/init
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-19 14:43:58.000000 tutor-xqueue-15.0.1/tutorxqueue/templates/xqueue/tasks/xqueue/
--rw-r--r--   0 ci        (1000) ci        (1000)       45 2023-03-19 14:43:50.000000 tutor-xqueue-15.0.1/tutorxqueue/templates/xqueue/tasks/xqueue/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.507030 tutor-xqueue-16.0.0/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       81 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     6676 2023-06-15 00:19:06.507030 tutor-xqueue-16.0.0/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     5630 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/pyproject.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-15 00:19:06.507030 tutor-xqueue-16.0.0/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1715 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.500363 tutor-xqueue-16.0.0/tutor_xqueue.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     6676 2023-06-15 00:19:06.000000 tutor-xqueue-16.0.0/tutor_xqueue.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)      929 2023-06-15 00:19:06.000000 tutor-xqueue-16.0.0/tutor_xqueue.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-06-15 00:19:06.000000 tutor-xqueue-16.0.0/tutor_xqueue.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       46 2023-06-15 00:19:06.000000 tutor-xqueue-16.0.0/tutor_xqueue.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       31 2023-06-15 00:19:06.000000 tutor-xqueue-16.0.0/tutor_xqueue.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       12 2023-06-15 00:19:06.000000 tutor-xqueue-16.0.0/tutor_xqueue.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.500363 tutor-xqueue-16.0.0/tutorxqueue/
+-rw-r--r--   0 ci        (1000) ci        (1000)      175 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.503696 tutor-xqueue-16.0.0/tutorxqueue/patches/
+-rw-r--r--   0 ci        (1000) ci        (1000)       82 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/patches/caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)     1184 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/patches/k8s-deployments
+-rw-r--r--   0 ci        (1000) ci        (1000)      578 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/patches/k8s-jobs
+-rw-r--r--   0 ci        (1000) ci        (1000)      173 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/patches/k8s-services
+-rw-r--r--   0 ci        (1000) ci        (1000)       76 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/patches/kustomization-configmapgenerator
+-rw-r--r--   0 ci        (1000) ci        (1000)       88 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/patches/local-docker-compose-dev-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      221 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      967 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/patches/local-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      204 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/patches/openedx-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)     9235 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.493696 tutor-xqueue-16.0.0/tutorxqueue/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.493696 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.493696 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/apps/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.503696 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/apps/settings/
+-rw-r--r--   0 ci        (1000) ci        (1000)      956 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/apps/settings/tutor.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.493696 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/build/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.503696 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/build/xqueue/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1641 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/build/xqueue/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.497030 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/tasks/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.503696 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/tasks/mysql/
+-rw-r--r--   0 ci        (1000) ci        (1000)      803 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/tasks/mysql/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.507030 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/tasks/xqueue/
+-rw-r--r--   0 ci        (1000) ci        (1000)       45 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/tasks/xqueue/init
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tutor-xqueue-15.0.1/LICENSE.txt` & `tutor-xqueue-16.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutor-xqueue-15.0.1/PKG-INFO` & `tutor-xqueue-16.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-xqueue
-Version: 15.0.1
+Version: 16.0.0
 Summary: A Tutor plugin for Xqueue (external grading system)
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: eduNEXT
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
@@ -12,39 +12,39 @@
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-xqueue/issues
 Project-URL: Community, https://discuss.openedx.org
 Classifier: Development Status :: 3 - Alpha
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
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 Xqueue external grading system plugin for `Tutor <https://docs.tutor.overhang.io>`_
 ===================================================================================
 
 This is a plugin for `Tutor <https://docs.tutor.overhang.io>`_ that provides the Xqueue external grading system for Open edX platforms. If you don't know what it is, you probably don't need it.
 
 Installation
 ------------
 
 The plugin is currently bundled with the `binary releases of Tutor <https://github.com/overhangio/tutor/releases>`__. If you have installed Tutor from source, you will have to install this plugin from source, too::
 
-    pip install tutor-xqueue
+    tutor plugins install xqueue
 
 Then, to enable this plugin, run::
 
     tutor plugins enable xqueue
 
-You should then run the initialisation scripts. The easiest way to do this is to run ``tutor local quickstart``.
+You should then run the initialisation scripts. The easiest way to do this is to run ``tutor local launch``.
 
 Usage
 -----
 
 In the Open edX studio, edit a course and add a new "Advanced blank problem" ("Problem" 🠆 "Advanced" 🠆  "Blank Advanced Problem"). Then, click "Edit" and copy-paste the following in the editor::
 
 
@@ -130,17 +130,19 @@
 -------------
 
 - ``XQUEUE_AUTH_PASSWORD`` (default: ``"{{ 8|random_string }}"``)
 - ``XQUEUE_AUTH_USERNAME`` (default: ``"lms"``)
 - ``XQUEUE_DOCKER_IMAGE`` (default: ``"{{ DOCKER_REGISTRY }}overhangio/openedx-xqueue:{{ TUTOR_VERSION }}"``)
 - ``XQUEUE_HOST`` (default: ``"xqueue.{{ LMS_HOST }}"``)
 - ``XQUEUE_MYSQL_PASSWORD`` (default: ``"{{ 8|random_string }}"``)
-- ``XQUEUE_MYSQL_DATABASE`` (default: ``"xqueue"``
+- ``XQUEUE_MYSQL_DATABASE`` (default: ``"xqueue"``)
 - ``XQUEUE_MYSQL_USERNAME`` (default: ``"xqueue"``)
 - ``XQUEUE_SECRET_KEY`` (default: ``"{{ 24|random_string }}"``)
+- ``XQUEUE_REPOSITORY`` (default: ``"https://github.com/openedx/xqueue"``)
+- ``XQUEUE_REPOSITORY_VERSION`` (default: ``"{{ OPENEDX_COMMON_VERSION }}"``)
 
 These values can be modified with ``tutor config save --set PARAM_NAME=VALUE`` commands.
 
 Debugging
 ---------
 
 To debug the xqueue service, you are encouraged to mount the xqueue repo from the host in the development container:
```

### Comparing `tutor-xqueue-15.0.1/README.rst` & `tutor-xqueue-16.0.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 This is a plugin for `Tutor <https://docs.tutor.overhang.io>`_ that provides the Xqueue external grading system for Open edX platforms. If you don't know what it is, you probably don't need it.
 
 Installation
 ------------
 
 The plugin is currently bundled with the `binary releases of Tutor <https://github.com/overhangio/tutor/releases>`__. If you have installed Tutor from source, you will have to install this plugin from source, too::
 
-    pip install tutor-xqueue
+    tutor plugins install xqueue
 
 Then, to enable this plugin, run::
 
     tutor plugins enable xqueue
 
-You should then run the initialisation scripts. The easiest way to do this is to run ``tutor local quickstart``.
+You should then run the initialisation scripts. The easiest way to do this is to run ``tutor local launch``.
 
 Usage
 -----
 
 In the Open edX studio, edit a course and add a new "Advanced blank problem" ("Problem" 🠆 "Advanced" 🠆  "Blank Advanced Problem"). Then, click "Edit" and copy-paste the following in the editor::
 
 
@@ -104,17 +104,19 @@
 -------------
 
 - ``XQUEUE_AUTH_PASSWORD`` (default: ``"{{ 8|random_string }}"``)
 - ``XQUEUE_AUTH_USERNAME`` (default: ``"lms"``)
 - ``XQUEUE_DOCKER_IMAGE`` (default: ``"{{ DOCKER_REGISTRY }}overhangio/openedx-xqueue:{{ TUTOR_VERSION }}"``)
 - ``XQUEUE_HOST`` (default: ``"xqueue.{{ LMS_HOST }}"``)
 - ``XQUEUE_MYSQL_PASSWORD`` (default: ``"{{ 8|random_string }}"``)
-- ``XQUEUE_MYSQL_DATABASE`` (default: ``"xqueue"``
+- ``XQUEUE_MYSQL_DATABASE`` (default: ``"xqueue"``)
 - ``XQUEUE_MYSQL_USERNAME`` (default: ``"xqueue"``)
 - ``XQUEUE_SECRET_KEY`` (default: ``"{{ 24|random_string }}"``)
+- ``XQUEUE_REPOSITORY`` (default: ``"https://github.com/openedx/xqueue"``)
+- ``XQUEUE_REPOSITORY_VERSION`` (default: ``"{{ OPENEDX_COMMON_VERSION }}"``)
 
 These values can be modified with ``tutor config save --set PARAM_NAME=VALUE`` commands.
 
 Debugging
 ---------
 
 To debug the xqueue service, you are encouraged to mount the xqueue repo from the host in the development container:
```

### Comparing `tutor-xqueue-15.0.1/setup.py` & `tutor-xqueue-16.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,22 +28,22 @@
     author_email="contact@overhang.io",
     maintainer="eduNEXT",
     description="A Tutor plugin for Xqueue (external grading system)",
     long_description=readme,
     long_description_content_type="text/x-rst",
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
-    python_requires=">=3.7",
-    install_requires=["tutor>=15.0.0,<16.0.0", "requests"],
+    python_requires=">=3.8",
+    install_requires=["tutor>=16.0.0,<17.0.0", "requests"],
     entry_points={"tutor.plugin.v1": ["xqueue = tutorxqueue.plugin"]},
     classifiers=[
         "Development Status :: 3 - Alpha",
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

### Comparing `tutor-xqueue-15.0.1/tutor_xqueue.egg-info/PKG-INFO` & `tutor-xqueue-16.0.0/tutor_xqueue.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-xqueue
-Version: 15.0.1
+Version: 16.0.0
 Summary: A Tutor plugin for Xqueue (external grading system)
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: eduNEXT
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
@@ -12,39 +12,39 @@
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-xqueue/issues
 Project-URL: Community, https://discuss.openedx.org
 Classifier: Development Status :: 3 - Alpha
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
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 Xqueue external grading system plugin for `Tutor <https://docs.tutor.overhang.io>`_
 ===================================================================================
 
 This is a plugin for `Tutor <https://docs.tutor.overhang.io>`_ that provides the Xqueue external grading system for Open edX platforms. If you don't know what it is, you probably don't need it.
 
 Installation
 ------------
 
 The plugin is currently bundled with the `binary releases of Tutor <https://github.com/overhangio/tutor/releases>`__. If you have installed Tutor from source, you will have to install this plugin from source, too::
 
-    pip install tutor-xqueue
+    tutor plugins install xqueue
 
 Then, to enable this plugin, run::
 
     tutor plugins enable xqueue
 
-You should then run the initialisation scripts. The easiest way to do this is to run ``tutor local quickstart``.
+You should then run the initialisation scripts. The easiest way to do this is to run ``tutor local launch``.
 
 Usage
 -----
 
 In the Open edX studio, edit a course and add a new "Advanced blank problem" ("Problem" 🠆 "Advanced" 🠆  "Blank Advanced Problem"). Then, click "Edit" and copy-paste the following in the editor::
 
 
@@ -130,17 +130,19 @@
 -------------
 
 - ``XQUEUE_AUTH_PASSWORD`` (default: ``"{{ 8|random_string }}"``)
 - ``XQUEUE_AUTH_USERNAME`` (default: ``"lms"``)
 - ``XQUEUE_DOCKER_IMAGE`` (default: ``"{{ DOCKER_REGISTRY }}overhangio/openedx-xqueue:{{ TUTOR_VERSION }}"``)
 - ``XQUEUE_HOST`` (default: ``"xqueue.{{ LMS_HOST }}"``)
 - ``XQUEUE_MYSQL_PASSWORD`` (default: ``"{{ 8|random_string }}"``)
-- ``XQUEUE_MYSQL_DATABASE`` (default: ``"xqueue"``
+- ``XQUEUE_MYSQL_DATABASE`` (default: ``"xqueue"``)
 - ``XQUEUE_MYSQL_USERNAME`` (default: ``"xqueue"``)
 - ``XQUEUE_SECRET_KEY`` (default: ``"{{ 24|random_string }}"``)
+- ``XQUEUE_REPOSITORY`` (default: ``"https://github.com/openedx/xqueue"``)
+- ``XQUEUE_REPOSITORY_VERSION`` (default: ``"{{ OPENEDX_COMMON_VERSION }}"``)
 
 These values can be modified with ``tutor config save --set PARAM_NAME=VALUE`` commands.
 
 Debugging
 ---------
 
 To debug the xqueue service, you are encouraged to mount the xqueue repo from the host in the development container:
```

### Comparing `tutor-xqueue-15.0.1/tutor_xqueue.egg-info/SOURCES.txt` & `tutor-xqueue-16.0.0/tutor_xqueue.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.py
 tutor_xqueue.egg-info/PKG-INFO
 tutor_xqueue.egg-info/SOURCES.txt
 tutor_xqueue.egg-info/dependency_links.txt
 tutor_xqueue.egg-info/entry_points.txt
 tutor_xqueue.egg-info/requires.txt
 tutor_xqueue.egg-info/top_level.txt
```

### Comparing `tutor-xqueue-15.0.1/tutorxqueue/patches/k8s-deployments` & `tutor-xqueue-16.0.0/tutorxqueue/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-xqueue-15.0.1/tutorxqueue/patches/k8s-jobs` & `tutor-xqueue-16.0.0/tutorxqueue/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-xqueue-15.0.1/tutorxqueue/patches/local-docker-compose-services` & `tutor-xqueue-16.0.0/tutorxqueue/patches/local-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-xqueue-15.0.1/tutorxqueue/plugin.py` & `tutor-xqueue-16.0.0/tutorxqueue/plugin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,65 @@
-from glob import glob
+from __future__ import annotations
+
 import json
 import os
+import typing as t
+from glob import glob
 
 import click
 import pkg_resources
 import requests
 
 from tutor import config as tutor_config
+from tutor import exceptions
 from tutor import hooks as tutor_hooks
-from tutor.exceptions import TutorError
 
 from .__about__ import __version__
 
-
 config = {
     "unique": {
         "AUTH_PASSWORD": "{{ 8|random_string }}",
         "MYSQL_PASSWORD": "{{ 8|random_string }}",
         "SECRET_KEY": "{{ 24|random_string }}",
     },
     "defaults": {
         "VERSION": __version__,
         "AUTH_USERNAME": "lms",
         "DOCKER_IMAGE": "{{ DOCKER_REGISTRY }}overhangio/openedx-xqueue:{{ XQUEUE_VERSION }}",
         "HOST": "xqueue.{{ LMS_HOST }}",
         "MYSQL_DATABASE": "xqueue",
         "MYSQL_USERNAME": "xqueue",
+        "REPOSITORY": "https://github.com/openedx/xqueue",
+        "REPOSITORY_VERSION": "{{ OPENEDX_COMMON_VERSION }}",
     },
 }
 
-# Inizialization hooks
-tutor_hooks.Filters.COMMANDS_INIT.add_item((
-    "mysql",
-    ("xqueue", "tasks", "mysql", "init"),
-))
+# Initialization hooks
 
-tutor_hooks.Filters.COMMANDS_INIT.add_item((
-    "xqueue",
-    ("xqueue", "tasks", "xqueue", "init"),
-))
+# To add a custom initialization task, create a bash script template under:
+# tutorcodejail/templates/codejail/tasks/
+# and then add it to the MY_INIT_TASKS list. Each task is in the format:
+# ("<service>", ("<path>", "<to>", "<script>", "<template>"))
+MY_INIT_TASKS: list[tuple[str, tuple[str, ...]]] = [
+    ("mysql", ("xqueue", "tasks", "mysql", "init")),
+    ("xqueue", ("xqueue", "tasks", "xqueue", "init")),
+]
+
+# For each task added to MY_INIT_TASKS, we load the task template
+# and add it to the CLI_DO_INIT_TASKS filter, which tells Tutor to
+# run it as part of the `init` job.
+for service, template_path in MY_INIT_TASKS:
+    full_path: str = pkg_resources.resource_filename(
+        "tutorxqueue", os.path.join("templates", *template_path)
+    )
+    with open(full_path, encoding="utf-8") as init_task_file:
+        init_task: str = init_task_file.read()
+    tutor_hooks.Filters.CLI_DO_INIT_TASKS.add_item((service, init_task))
 
-# Image managment
+# Image management
 tutor_hooks.Filters.IMAGES_BUILD.add_item((
     "xqueue",
     ("plugins", "xqueue", "build", "xqueue"),
     "{{ XQUEUE_DOCKER_IMAGE }}",
     (),
 ))
 
@@ -53,28 +68,30 @@
     "{{ XQUEUE_DOCKER_IMAGE }}",
 ))
 tutor_hooks.Filters.IMAGES_PUSH.add_item((
     "xqueue",
     "{{ XQUEUE_DOCKER_IMAGE }}",
 ))
 
+
 @tutor_hooks.Filters.COMPOSE_MOUNTS.add()
 def _mount_xqueue(volumes, name):
     """
     When mounting xqueue with `--mount=/path/to/xqueue`,
     bind-mount the host repo in the xqueue container.
     """
     if name == "xqueue":
         path = "/openedx/xqueue"
         volumes += [
             ("xqueue", path),
             ("xqueue-job", path),
         ]
     return volumes
 
+
 @click.group(help="Interact with the Xqueue server", name="xqueue")
 def command():
     pass
 
 
 @click.group(help="List and grade submissions")
 @click.pass_obj
@@ -161,15 +178,15 @@
         response = self.request(
             "/xqueue/login/",
             method="POST",
             data={"username": self.username, "password": self.password},
         )
         message = response.get("content")
         if message != "Logged in":
-            raise TutorError(
+            raise exceptions.TutorError(
                 "Could not login to xqueue server at {}. Response: '{}'".format(
                     self.base_url, message
                 )
             )
 
     def show_submission(self, queue):
         response = self.request("/xqueue/get_submission/", params={"queue_name": queue})
@@ -239,26 +256,39 @@
 for path in glob(
     os.path.join(
         pkg_resources.resource_filename("tutorxqueue", "patches"),
         "*",
     )
 ):
     with open(path, encoding="utf-8") as patch_file:
-        tutor_hooks.Filters.ENV_PATCHES.add_item((os.path.basename(path), patch_file.read()))
+        tutor_hooks.Filters.ENV_PATCHES.add_item(
+            (os.path.basename(path), patch_file.read())
+        )
 
 # Add cli commands filter
 tutor_hooks.Filters.CLI_COMMANDS.add_item(command)
 
 # Add configuration entries
 tutor_hooks.Filters.CONFIG_DEFAULTS.add_items(
-    [
-        (f"XQUEUE_{key}", value)
-        for key, value in config.get("defaults", {}).items()
-    ]
+    [(f"XQUEUE_{key}", value) for key, value in config.get("defaults", {}).items()]
 )
 tutor_hooks.Filters.CONFIG_UNIQUE.add_items(
-    [
-        (f"XQUEUE_{key}", value)
-        for key, value in config.get("unique", {}).items()
-    ]
+    [(f"XQUEUE_{key}", value) for key, value in config.get("unique", {}).items()]
+)
+tutor_hooks.Filters.CONFIG_OVERRIDES.add_items(
+    list(config.get("overrides", {}).items())
 )
-tutor_hooks.Filters.CONFIG_OVERRIDES.add_items(list(config.get("overrides", {}).items()))
+
+
+########################################
+# Xqueue Public Host
+########################################
+
+@tutor_hooks.Filters.APP_PUBLIC_HOSTS.add()
+def _xqueue_public_hosts(
+    hosts: list[str], context_name: t.Literal["local", "dev"]
+) -> list[str]:
+    if context_name == "dev":
+        hosts += ["{{ XQUEUE_HOST }}:8000"]
+    else:
+        hosts += ["{{ XQUEUE_HOST }}"]
+    return hosts
```

### Comparing `tutor-xqueue-15.0.1/tutorxqueue/templates/xqueue/apps/settings/tutor.py` & `tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/apps/settings/tutor.py`

 * *Files identical despite different names*

### Comparing `tutor-xqueue-15.0.1/tutorxqueue/templates/xqueue/tasks/mysql/init` & `tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/tasks/mysql/init`

 * *Files identical despite different names*

