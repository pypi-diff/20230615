# Comparing `tmp/tutor-notes-15.0.4.tar.gz` & `tmp/tutor-notes-16.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tutor-notes-15.0.4.tar", last modified: Thu Apr 13 15:48:20 2023, max compression
+gzip compressed data, was "tutor-notes-16.0.0.tar", last modified: Wed Jun 14 23:42:28 2023, max compression
```

## Comparing `tutor-notes-15.0.4.tar` & `tutor-notes-16.0.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/
--rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/LICENSE.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       79 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     4302 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     3304 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1641 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutor_notes.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     4302 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutor_notes.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     1078 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutor_notes.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutor_notes.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       44 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutor_notes.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutor_notes.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       11 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutor_notes.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/
--rw-r--r--   0 ci        (1000) ci        (1000)       23 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/patches/
--rw-r--r--   0 ci        (1000) ci        (1000)       79 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)      903 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/k8s-deployments
--rw-r--r--   0 ci        (1000) ci        (1000)      606 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/k8s-jobs
--rw-r--r--   0 ci        (1000) ci        (1000)      217 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/k8s-services
--rw-r--r--   0 ci        (1000) ci        (1000)       74 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/kustomization-configmapgenerator
--rw-r--r--   0 ci        (1000) ci        (1000)      111 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/local-docker-compose-dev-services
--rw-r--r--   0 ci        (1000) ci        (1000)      275 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/local-docker-compose-jobs-services
--rw-r--r--   0 ci        (1000) ci        (1000)      576 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/local-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)       51 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/openedx-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)       47 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/openedx-lms-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      111 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/openedx-lms-development-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      143 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/openedx-lms-production-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     2867 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/templates/notes/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/templates/notes/apps/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/templates/notes/apps/settings/
--rw-r--r--   0 ci        (1000) ci        (1000)     1073 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/templates/notes/apps/settings/tutor.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/templates/notes/build/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/templates/notes/build/notes/
--rw-r--r--   0 ci        (1000) ci        (1000)      868 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/templates/notes/build/notes/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/templates/notes/tasks/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/templates/notes/tasks/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)      574 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/templates/notes/tasks/lms/init
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/templates/notes/tasks/mysql/
--rw-r--r--   0 ci        (1000) ci        (1000)      797 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/templates/notes/tasks/mysql/init
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/templates/notes/tasks/notes/
--rw-r--r--   0 ci        (1000) ci        (1000)       58 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/templates/notes/tasks/notes/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.939294 tutor-notes-16.0.0/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       79 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     4305 2023-06-14 23:42:28.939294 tutor-notes-16.0.0/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     3306 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/pyproject.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-14 23:42:28.939294 tutor-notes-16.0.0/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1642 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.932627 tutor-notes-16.0.0/tutor_notes.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     4305 2023-06-14 23:42:28.000000 tutor-notes-16.0.0/tutor_notes.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     1093 2023-06-14 23:42:28.000000 tutor-notes-16.0.0/tutor_notes.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-06-14 23:42:28.000000 tutor-notes-16.0.0/tutor_notes.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       44 2023-06-14 23:42:28.000000 tutor-notes-16.0.0/tutor_notes.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-06-14 23:42:28.000000 tutor-notes-16.0.0/tutor_notes.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       11 2023-06-14 23:42:28.000000 tutor-notes-16.0.0/tutor_notes.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.932627 tutor-notes-16.0.0/tutornotes/
+-rw-r--r--   0 ci        (1000) ci        (1000)      175 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.939294 tutor-notes-16.0.0/tutornotes/patches/
+-rw-r--r--   0 ci        (1000) ci        (1000)       79 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      903 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/k8s-deployments
+-rw-r--r--   0 ci        (1000) ci        (1000)      606 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/k8s-jobs
+-rw-r--r--   0 ci        (1000) ci        (1000)      217 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/k8s-services
+-rw-r--r--   0 ci        (1000) ci        (1000)       74 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/kustomization-configmapgenerator
+-rw-r--r--   0 ci        (1000) ci        (1000)      111 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/local-docker-compose-dev-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      275 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      576 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/local-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)       51 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/openedx-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)       47 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/openedx-lms-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      111 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/openedx-lms-development-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      143 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/openedx-lms-production-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)     3930 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.929294 tutor-notes-16.0.0/tutornotes/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.929294 tutor-notes-16.0.0/tutornotes/templates/notes/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.929294 tutor-notes-16.0.0/tutornotes/templates/notes/apps/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.939294 tutor-notes-16.0.0/tutornotes/templates/notes/apps/settings/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1073 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/templates/notes/apps/settings/tutor.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.929294 tutor-notes-16.0.0/tutornotes/templates/notes/build/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.939294 tutor-notes-16.0.0/tutornotes/templates/notes/build/notes/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1364 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/templates/notes/build/notes/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.929294 tutor-notes-16.0.0/tutornotes/templates/notes/tasks/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.939294 tutor-notes-16.0.0/tutornotes/templates/notes/tasks/lms/
+-rw-r--r--   0 ci        (1000) ci        (1000)      574 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/templates/notes/tasks/lms/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.939294 tutor-notes-16.0.0/tutornotes/templates/notes/tasks/mysql/
+-rw-r--r--   0 ci        (1000) ci        (1000)      797 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/templates/notes/tasks/mysql/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.939294 tutor-notes-16.0.0/tutornotes/templates/notes/tasks/notes/
+-rw-r--r--   0 ci        (1000) ci        (1000)       58 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/templates/notes/tasks/notes/init
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tutor-notes-15.0.4/LICENSE.txt` & `tutor-notes-16.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutor-notes-15.0.4/PKG-INFO` & `tutor-notes-16.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-notes
-Version: 15.0.4
+Version: 16.0.0
 Summary: A Tutor plugin for student notes
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: eduNEXT
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
@@ -12,35 +12,35 @@
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-notes/issues
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
 
 Students notes plugin for `Tutor <https://docs.tutor.overhang.io>`_
 ===================================================================
 
-This is a plugin for `Tutor <https://docs.tutor.overhang.io>`_ to easily add the `Open edX note-taking app <https://github.com/openedx/edx-notes-api>`_ to an Open edX platform. This app allows students to annotate portions of the courseware (see `the official documentation <https://edx.readthedocs.io/projects/open-edx-building-and-running-a-course/en/open-release-olive.master/exercises_tools/notes.html>`_).
+This is a plugin for `Tutor <https://docs.tutor.overhang.io>`_ to easily add the `Open edX note-taking app <https://github.com/openedx/edx-notes-api>`_ to an Open edX platform. This app allows students to annotate portions of the courseware (see `the official documentation <https://edx.readthedocs.io/projects/open-edx-building-and-running-a-course/en/open-release-palm.master/exercises_tools/notes.html>`_).
 
-.. image:: https://edx.readthedocs.io/projects/open-edx-building-and-running-a-course/en/open-release-olive.master/_images/SFD_SN_bodyexample.png
+.. image:: https://edx.readthedocs.io/projects/open-edx-building-and-running-a-course/en/open-release-palm.master/_images/SFD_SN_bodyexample.png
     :alt: Notes in action
 
 Installation
 ------------
 
 The plugin is currently bundled with the `binary releases of Tutor <https://github.com/overhangio/tutor/releases>`_. If you have installed Tutor from source, you will have to install this plugin from source, too::
 
-    pip install tutor-notes
+    tutor plugins install notes
 
 Then, to enable this plugin, run::
 
     tutor plugins enable notes
 
 You should beware that the ``notes.<LMS_HOST>`` domain name should exist and point to your server. For instance, if your LMS is hosted at http://myopenedx.com, the notes service should be found at http://notes.myopenedx.com.
```

### Comparing `tutor-notes-15.0.4/README.rst` & `tutor-notes-16.0.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Students notes plugin for `Tutor <https://docs.tutor.overhang.io>`_
 ===================================================================
 
-This is a plugin for `Tutor <https://docs.tutor.overhang.io>`_ to easily add the `Open edX note-taking app <https://github.com/openedx/edx-notes-api>`_ to an Open edX platform. This app allows students to annotate portions of the courseware (see `the official documentation <https://edx.readthedocs.io/projects/open-edx-building-and-running-a-course/en/open-release-olive.master/exercises_tools/notes.html>`_).
+This is a plugin for `Tutor <https://docs.tutor.overhang.io>`_ to easily add the `Open edX note-taking app <https://github.com/openedx/edx-notes-api>`_ to an Open edX platform. This app allows students to annotate portions of the courseware (see `the official documentation <https://edx.readthedocs.io/projects/open-edx-building-and-running-a-course/en/open-release-palm.master/exercises_tools/notes.html>`_).
 
-.. image:: https://edx.readthedocs.io/projects/open-edx-building-and-running-a-course/en/open-release-olive.master/_images/SFD_SN_bodyexample.png
+.. image:: https://edx.readthedocs.io/projects/open-edx-building-and-running-a-course/en/open-release-palm.master/_images/SFD_SN_bodyexample.png
     :alt: Notes in action
 
 Installation
 ------------
 
 The plugin is currently bundled with the `binary releases of Tutor <https://github.com/overhangio/tutor/releases>`_. If you have installed Tutor from source, you will have to install this plugin from source, too::
 
-    pip install tutor-notes
+    tutor plugins install notes
 
 Then, to enable this plugin, run::
 
     tutor plugins enable notes
 
 You should beware that the ``notes.<LMS_HOST>`` domain name should exist and point to your server. For instance, if your LMS is hosted at http://myopenedx.com, the notes service should be found at http://notes.myopenedx.com.
```

### Comparing `tutor-notes-15.0.4/setup.py` & `tutor-notes-16.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,22 +27,22 @@
     author="Overhang.IO",
     author_email="contact@overhang.io",
     maintainer="eduNEXT",
     description="A Tutor plugin for student notes",
     long_description=readme,
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
-    python_requires=">=3.7",
-    install_requires=["tutor>=15.0.0,<16.0.0"],
+    python_requires=">=3.8",
+    install_requires=["tutor>=16.0.0,<17.0.0"],
     entry_points={"tutor.plugin.v1": ["notes = tutornotes.plugin"]},
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

### Comparing `tutor-notes-15.0.4/tutor_notes.egg-info/PKG-INFO` & `tutor-notes-16.0.0/tutor_notes.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-notes
-Version: 15.0.4
+Version: 16.0.0
 Summary: A Tutor plugin for student notes
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: eduNEXT
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
@@ -12,35 +12,35 @@
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-notes/issues
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
 
 Students notes plugin for `Tutor <https://docs.tutor.overhang.io>`_
 ===================================================================
 
-This is a plugin for `Tutor <https://docs.tutor.overhang.io>`_ to easily add the `Open edX note-taking app <https://github.com/openedx/edx-notes-api>`_ to an Open edX platform. This app allows students to annotate portions of the courseware (see `the official documentation <https://edx.readthedocs.io/projects/open-edx-building-and-running-a-course/en/open-release-olive.master/exercises_tools/notes.html>`_).
+This is a plugin for `Tutor <https://docs.tutor.overhang.io>`_ to easily add the `Open edX note-taking app <https://github.com/openedx/edx-notes-api>`_ to an Open edX platform. This app allows students to annotate portions of the courseware (see `the official documentation <https://edx.readthedocs.io/projects/open-edx-building-and-running-a-course/en/open-release-palm.master/exercises_tools/notes.html>`_).
 
-.. image:: https://edx.readthedocs.io/projects/open-edx-building-and-running-a-course/en/open-release-olive.master/_images/SFD_SN_bodyexample.png
+.. image:: https://edx.readthedocs.io/projects/open-edx-building-and-running-a-course/en/open-release-palm.master/_images/SFD_SN_bodyexample.png
     :alt: Notes in action
 
 Installation
 ------------
 
 The plugin is currently bundled with the `binary releases of Tutor <https://github.com/overhangio/tutor/releases>`_. If you have installed Tutor from source, you will have to install this plugin from source, too::
 
-    pip install tutor-notes
+    tutor plugins install notes
 
 Then, to enable this plugin, run::
 
     tutor plugins enable notes
 
 You should beware that the ``notes.<LMS_HOST>`` domain name should exist and point to your server. For instance, if your LMS is hosted at http://myopenedx.com, the notes service should be found at http://notes.myopenedx.com.
```

### Comparing `tutor-notes-15.0.4/tutor_notes.egg-info/SOURCES.txt` & `tutor-notes-16.0.0/tutor_notes.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.py
 tutor_notes.egg-info/PKG-INFO
 tutor_notes.egg-info/SOURCES.txt
 tutor_notes.egg-info/dependency_links.txt
 tutor_notes.egg-info/entry_points.txt
 tutor_notes.egg-info/requires.txt
 tutor_notes.egg-info/top_level.txt
```

### Comparing `tutor-notes-15.0.4/tutornotes/patches/k8s-deployments` & `tutor-notes-16.0.0/tutornotes/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-notes-15.0.4/tutornotes/patches/k8s-jobs` & `tutor-notes-16.0.0/tutornotes/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-notes-15.0.4/tutornotes/patches/local-docker-compose-services` & `tutor-notes-16.0.0/tutornotes/patches/local-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-notes-15.0.4/tutornotes/templates/notes/apps/settings/tutor.py` & `tutor-notes-16.0.0/tutornotes/templates/notes/apps/settings/tutor.py`

 * *Files identical despite different names*

### Comparing `tutor-notes-15.0.4/tutornotes/templates/notes/tasks/lms/init` & `tutor-notes-16.0.0/tutornotes/templates/notes/tasks/lms/init`

 * *Files identical despite different names*

### Comparing `tutor-notes-15.0.4/tutornotes/templates/notes/tasks/mysql/init` & `tutor-notes-16.0.0/tutornotes/templates/notes/tasks/mysql/init`

 * *Files identical despite different names*

