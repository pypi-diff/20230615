# Comparing `tmp/tutor-mfe-15.0.7.tar.gz` & `tmp/tutor-mfe-16.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tutor-mfe-15.0.7.tar", last modified: Fri May 26 15:34:40 2023, max compression
+gzip compressed data, was "tutor-mfe-16.0.0.tar", last modified: Wed Jun 14 23:13:31 2023, max compression
```

## Comparing `tutor-mfe-15.0.7.tar` & `tutor-mfe-16.0.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/
--rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/LICENSE.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       76 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)    15577 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)    14515 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/pyproject.toml
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1849 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/tutor_mfe.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)    15577 2023-05-26 15:34:39.000000 tutor-mfe-15.0.7/tutor_mfe.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     1189 2023-05-26 15:34:39.000000 tutor-mfe-15.0.7/tutor_mfe.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-05-26 15:34:39.000000 tutor-mfe-15.0.7/tutor_mfe.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       40 2023-05-26 15:34:39.000000 tutor-mfe-15.0.7/tutor_mfe.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-05-26 15:34:39.000000 tutor-mfe-15.0.7/tutor_mfe.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        9 2023-05-26 15:34:39.000000 tutor-mfe-15.0.7/tutor_mfe.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/tutormfe/
--rw-r--r--   0 ci        (1000) ci        (1000)       24 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/tutormfe/patches/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/.gitignore
--rw-r--r--   0 ci        (1000) ci        (1000)      333 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)      605 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/k8s-deployments
--rw-r--r--   0 ci        (1000) ci        (1000)      168 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/k8s-services
--rw-r--r--   0 ci        (1000) ci        (1000)      130 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/kustomization-configmapgenerator
--rw-r--r--   0 ci        (1000) ci        (1000)      460 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/local-docker-compose-dev-services
--rw-r--r--   0 ci        (1000) ci        (1000)      184 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/local-docker-compose-prod-services
--rw-r--r--   0 ci        (1000) ci        (1000)      476 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/openedx-cms-development-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      405 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/openedx-cms-production-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      357 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/openedx-lms-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     3306 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/openedx-lms-development-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     3796 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/openedx-lms-production-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     5356 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:39.000000 tutor-mfe-15.0.7/tutormfe/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:39.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/apps/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/apps/.gitignore
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/apps/mfe/
--rw-r--r--   0 ci        (1000) ci        (1000)      629 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/apps/mfe/Caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)      749 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/apps/mfe/webpack.dev-tutor.config.js
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/build/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/build/.gitignore
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/build/mfe/
--rw-r--r--   0 ci        (1000) ci        (1000)     3700 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/build/mfe/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/build/mfe/i18n/
--rwxr-xr-x   0 ci        (1000) ci        (1000)     1489 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/build/mfe/i18n/i18n-merge.js
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/tasks/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/tasks/.gitignore
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/tasks/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)     3717 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/tasks/lms/init
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-06-14 23:13:31.847755 tutor-mfe-16.0.0/
+-rw-rw-r--   0 regis     (1000) regis     (1000)    34523 2023-05-16 11:36:57.000000 tutor-mfe-16.0.0/LICENSE.txt
+-rw-r--r--   0 regis     (1000) regis     (1000)       76 2020-12-08 13:54:21.000000 tutor-mfe-16.0.0/MANIFEST.in
+-rw-rw-r--   0 regis     (1000) regis     (1000)    16200 2023-06-14 23:13:31.847755 tutor-mfe-16.0.0/PKG-INFO
+-rw-rw-r--   0 regis     (1000) regis     (1000)    15118 2023-06-14 20:30:21.000000 tutor-mfe-16.0.0/README.rst
+-rw-rw-r--   0 regis     (1000) regis     (1000)       50 2023-06-14 10:06:49.000000 tutor-mfe-16.0.0/pyproject.toml
+-rw-rw-r--   0 regis     (1000) regis     (1000)       38 2023-06-14 23:13:31.847755 tutor-mfe-16.0.0/setup.cfg
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1857 2023-06-14 20:30:21.000000 tutor-mfe-16.0.0/setup.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-06-14 23:13:31.843755 tutor-mfe-16.0.0/tutor_mfe.egg-info/
+-rw-r--r--   0 regis     (1000) regis     (1000)    16200 2023-06-14 23:13:31.000000 tutor-mfe-16.0.0/tutor_mfe.egg-info/PKG-INFO
+-rw-r--r--   0 regis     (1000) regis     (1000)     1207 2023-06-14 23:13:31.000000 tutor-mfe-16.0.0/tutor_mfe.egg-info/SOURCES.txt
+-rw-r--r--   0 regis     (1000) regis     (1000)        1 2023-06-14 23:13:31.000000 tutor-mfe-16.0.0/tutor_mfe.egg-info/dependency_links.txt
+-rw-r--r--   0 regis     (1000) regis     (1000)       41 2023-06-14 23:13:31.000000 tutor-mfe-16.0.0/tutor_mfe.egg-info/entry_points.txt
+-rw-r--r--   0 regis     (1000) regis     (1000)       22 2023-06-14 23:13:31.000000 tutor-mfe-16.0.0/tutor_mfe.egg-info/requires.txt
+-rw-r--r--   0 regis     (1000) regis     (1000)        9 2023-06-14 23:13:31.000000 tutor-mfe-16.0.0/tutor_mfe.egg-info/top_level.txt
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-06-14 23:13:31.843755 tutor-mfe-16.0.0/tutormfe/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      210 2023-06-14 22:45:08.000000 tutor-mfe-16.0.0/tutormfe/__about__.py
+-rw-r--r--   0 regis     (1000) regis     (1000)        0 2020-12-08 13:54:21.000000 tutor-mfe-16.0.0/tutormfe/__init__.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)      417 2023-06-14 20:30:21.000000 tutor-mfe-16.0.0/tutormfe/hooks.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-06-14 23:13:31.847755 tutor-mfe-16.0.0/tutormfe/patches/
+-rw-r--r--   0 regis     (1000) regis     (1000)        0 2020-12-08 13:54:21.000000 tutor-mfe-16.0.0/tutormfe/patches/.gitignore
+-rw-rw-r--   0 regis     (1000) regis     (1000)      333 2023-05-16 11:36:57.000000 tutor-mfe-16.0.0/tutormfe/patches/caddyfile
+-rw-rw-r--   0 regis     (1000) regis     (1000)      605 2023-05-16 11:36:57.000000 tutor-mfe-16.0.0/tutormfe/patches/k8s-deployments
+-rw-rw-r--   0 regis     (1000) regis     (1000)      168 2021-06-08 20:38:48.000000 tutor-mfe-16.0.0/tutormfe/patches/k8s-services
+-rw-rw-r--   0 regis     (1000) regis     (1000)      130 2023-05-16 11:36:57.000000 tutor-mfe-16.0.0/tutormfe/patches/kustomization-configmapgenerator
+-rw-rw-r--   0 regis     (1000) regis     (1000)      542 2023-06-14 20:30:21.000000 tutor-mfe-16.0.0/tutormfe/patches/local-docker-compose-dev-services
+-rw-rw-r--   0 regis     (1000) regis     (1000)      184 2023-05-16 11:36:57.000000 tutor-mfe-16.0.0/tutormfe/patches/local-docker-compose-prod-services
+-rw-rw-r--   0 regis     (1000) regis     (1000)      428 2023-06-14 20:30:21.000000 tutor-mfe-16.0.0/tutormfe/patches/openedx-cms-development-settings
+-rw-rw-r--   0 regis     (1000) regis     (1000)      457 2023-06-14 20:30:21.000000 tutor-mfe-16.0.0/tutormfe/patches/openedx-cms-production-settings
+-rw-rw-r--   0 regis     (1000) regis     (1000)      527 2023-06-14 20:30:21.000000 tutor-mfe-16.0.0/tutormfe/patches/openedx-lms-common-settings
+-rw-rw-r--   0 regis     (1000) regis     (1000)     3197 2023-06-14 20:30:21.000000 tutor-mfe-16.0.0/tutormfe/patches/openedx-lms-development-settings
+-rw-rw-r--   0 regis     (1000) regis     (1000)     3829 2023-06-14 20:30:21.000000 tutor-mfe-16.0.0/tutormfe/patches/openedx-lms-production-settings
+-rw-rw-r--   0 regis     (1000) regis     (1000)     7449 2023-06-14 20:30:21.000000 tutor-mfe-16.0.0/tutormfe/plugin.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-06-14 23:13:31.807755 tutor-mfe-16.0.0/tutormfe/templates/
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-06-14 23:13:31.807755 tutor-mfe-16.0.0/tutormfe/templates/mfe/
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-06-14 23:13:31.847755 tutor-mfe-16.0.0/tutormfe/templates/mfe/apps/
+-rw-r--r--   0 regis     (1000) regis     (1000)        0 2020-12-08 13:54:21.000000 tutor-mfe-16.0.0/tutormfe/templates/mfe/apps/.gitignore
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-06-14 23:13:31.847755 tutor-mfe-16.0.0/tutormfe/templates/mfe/apps/mfe/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      597 2023-06-14 20:30:21.000000 tutor-mfe-16.0.0/tutormfe/templates/mfe/apps/mfe/Caddyfile
+-rw-rw-r--   0 regis     (1000) regis     (1000)      749 2022-12-13 07:01:03.000000 tutor-mfe-16.0.0/tutormfe/templates/mfe/apps/mfe/webpack.dev-tutor.config.js
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-06-14 23:13:31.847755 tutor-mfe-16.0.0/tutormfe/templates/mfe/build/
+-rw-r--r--   0 regis     (1000) regis     (1000)        0 2020-12-08 13:54:21.000000 tutor-mfe-16.0.0/tutormfe/templates/mfe/build/.gitignore
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-06-14 23:13:31.847755 tutor-mfe-16.0.0/tutormfe/templates/mfe/build/mfe/
+-rw-rw-r--   0 regis     (1000) regis     (1000)     3974 2023-06-14 20:30:21.000000 tutor-mfe-16.0.0/tutormfe/templates/mfe/build/mfe/Dockerfile
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-06-14 23:13:31.847755 tutor-mfe-16.0.0/tutormfe/templates/mfe/build/mfe/i18n/
+-rwxrwxr-x   0 regis     (1000) regis     (1000)     1489 2021-11-30 08:53:17.000000 tutor-mfe-16.0.0/tutormfe/templates/mfe/build/mfe/i18n/i18n-merge.js
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-06-14 23:13:31.847755 tutor-mfe-16.0.0/tutormfe/templates/mfe/tasks/
+-rw-rw-r--   0 regis     (1000) regis     (1000)        0 2022-10-03 10:29:37.000000 tutor-mfe-16.0.0/tutormfe/templates/mfe/tasks/.gitignore
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-06-14 23:13:31.847755 tutor-mfe-16.0.0/tutormfe/templates/mfe/tasks/lms/
+-rw-rw-r--   0 regis     (1000) regis     (1000)     4099 2023-06-14 20:30:21.000000 tutor-mfe-16.0.0/tutormfe/templates/mfe/tasks/lms/init
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tutor-mfe-15.0.7/LICENSE.txt` & `tutor-mfe-16.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutor-mfe-15.0.7/PKG-INFO` & `tutor-mfe-16.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: tutor-mfe
-Version: 15.0.7
+Version: 16.0.0
 Summary: mfe plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-mfe
 Author: Overhang.IO
 Maintainer: tCRIL
 Maintainer-email: adolfo@tcril.org
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-mfe
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-mfe/issues
 Project-URL: Community, https://discuss.openedx.org/tag/tutor
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -28,21 +29,23 @@
 Micro Frontend base plugin for `Tutor <https://docs.tutor.overhang.io>`__
 =========================================================================
 
 This plugin makes it possible to easily add micro frontend (MFE) applications on top of an Open edX platform that runs with Tutor. To learn more about MFEs, please check the `official Open edX documentation <https://edx.readthedocs.io/projects/edx-developer-docs/en/latest/developers_guide/micro_frontends_in_open_edx.html>`__.
 
 In addition, this plugin comes with a few MFEs which are enabled by default:
 
+- `Authn <https://github.com/openedx/frontend-app-authn/>`__
 - `Account <https://github.com/openedx/frontend-app-account/>`__
+- `Communications <https://github.com/openedx/frontend-app-communications/>`__
+- `Course Authoring <https://github.com/openedx/frontend-app-course-authoring/>`__
+- `Discussions <https://github.com/openedx/frontend-app-discussions/>`__
 - `Gradebook <https://github.com/openedx/frontend-app-gradebook/>`__
 - `Learning <https://github.com/openedx/frontend-app-learning/>`__
+- `ORA Grading <https://github.com/openedx/frontend-app-ora-grading/>`__
 - `Profile <https://github.com/openedx/frontend-app-profile/>`__
-- `Course Authoring <https://github.com/openedx/frontend-app-course-authoring/>`__
-- `Discussions <https://github.com/openedx/frontend-app-discussions/>`__
-- `Authn <https://github.com/openedx/frontend-app-authn/>`__
 
 Instructions for using each of these MFEs are given below.
 
 Installation
 ------------
 
 ::
@@ -55,27 +58,58 @@
 To enable this plugin, run::
 
     tutor plugins enable mfe
     tutor local launch
 
 When running the plugin in production, it is recommended that you set up a catch-all CNAME for subdomains at the DNS provider: see the `Configuring DNS Records <https://docs.tutor.overhang.io/install.html#configuring-dns-records>`__ section in the Tutor documentation for more details.  This way, the plugin will work out of the box with no additional configuration.  Which is to say, if your ``LMS_HOST`` is set to `myopenedx.com` the MFEs this plugin provides will be accessible under `apps.myopenedx.com` by default.
 
-To check what the current value of `MFE_HOST` is actually set to, run the following::
+To check what the current value of `MFE_HOST` is actually set to, run::
 
     tutor config printvalue MFE_HOST
 
+Authn
+~~~~~~~~~
+
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/authn.png
+    :alt: Authn MFE screenshot
+
+This is a micro-frontend application responsible for the login, registration and password reset functionality.
 
 Account
 ~~~~~~~
 
 .. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/account.png
     :alt: Account MFE screenshot
 
 An MFE to manage account-specific information for every LMS user. Each user's account page is available at ``http(s)://{{ MFE_HOST }}/account``. For instance, when running locally: https://apps.local.overhang.io/account.
 
+Communications
+~~~~~~~~~~~~~~
+
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/communications.png
+    :alt: Communications MFE screenshot
+
+The Communications micro-frontend exposes an interface for course teams to communicate with learners.  It achieves this by allowing instructors to send out emails in bulk, either by scheduling them or on demand.
+
+Course Authoring
+~~~~~~~~~~~~~~~~
+
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/course-authoring.png
+    :alt: Course Authoring MFE screenshot
+
+This MFE is meant for course authors and maintainers. For a given course, it exposes a "Pages & Resources" menu in Studio where one can enable or disable a variety of features, including, for example, the Wiki and Discussions.  Optionally, it allows authors to replace the legacy HTML, Video, and Problem authoring tools with experimental React-based versions, as well as exposing a new proctoring interface that can be enabled if the `edx-exams <https://github.com/edx/edx-exams>`_ service is available.
+
+Discussions
+~~~~~~~~~~~
+
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/discussions.png
+    :alt: Discussions MFE screenshot
+
+The Discussions MFE updates the previous discussions UI with a new look and better features.
+
 Gradebook
 ~~~~~~~~~
 
 .. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/gradebook.png
     :alt: Gradebook MFE screenshot
 
 This instructor-only MFE is for viewing individual and aggregated grade results for a course. To access this MFE, go to a course 🡒 🡒 Instructor tab 🡒 Student Admin 🡒 View gradebook. The URL should be: ``http(s)://{{ MFE_HOST }}/gradebook/{{ course ID }}``. When running locally, the gradebook of the demo course is available at: http://apps.local.overhang.io/gradebook/course-v1:edX+DemoX+Demo_Course
@@ -84,78 +118,65 @@
 ~~~~~~~~
 
 .. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/learning.png
     :alt: Learning MFE screenshot
 
 The Learning MFE replaces the former courseware, which is the core part of the LMS where students follow courses.
 
+ORA Grading
+~~~~~~~~~~~
+
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/ora-grading.png
+    :alt: ORA Grading MFE screenshot
+
+When enabled, Open Response Assesments ("ORA") that have a staff grading step will link to this new MFE, either when clicking "Grade Available Responses" from the exercise itself, or via a link in the Instructor Dashboard.  It is meant to streamline the grading process with better previews of submitted content.
+
 Profile
 ~~~~~~~~~
 
 .. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/profile.png
     :alt: Profile MFE screenshot
 
 Edit and display user-specific profile information. The profile page of every user is visible at ``http(s)://{{ MFE_HOST }}/profile/u/{{ username }}``. For instance, when running locally, the profile page of the "admin" user is: http://apps.local.overhang.io/profile/u/admin.
 
-Course Authoring
-~~~~~~~~~~~~~~~~
-
-.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/course-authoring.png
-    :alt: Course Authoring MFE screenshot
-
-This MFE is meant for course authors and maintainers. For a given course, it exposes a "Pages & Resources" menu in Studio where one can enable or disable a variety of features, including, for example, the Wiki and Discussions.  Optionally, it allows authors to replace the legacy HTML, Video, and Problem authoring tools with experimental React-based versions, as well as exposing a new proctoring interface that can be enabled if the `edx-exams <https://github.com/edx/edx-exams>`_ service is available.
-
-Discussions
-~~~~~~~~~~~
-
-.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/discussions.png
-    :alt: Discussions MFE screenshot
-
-The Discussions MFE updates the previous discussions UI with a new look and better features.
-
-Authn
-~~~~~~~~~
-
-.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/authn.png
-    :alt: Authn MFE screenshot
-
-This is a micro-frontend application responsible for the login, registration and password reset functionality.
 
 MFE management
 --------------
 
 Adding new MFEs
 ~~~~~~~~~~~~~~~
 
-Other Tutor plugin developers can take advantage of this plugin to deploy their own MFEs. To declare a new MFE, a new configuration setting should be created with the "_MFE_APP" suffix. This configuration setting should include the name, git repository (and optionally: git branch) and development port. For example::
+.. warning:: As of Tutor v16 (Palm release) it is no longer possible to add new MFEs by creating ``*_MFE_APP`` settings. Instead, users must implement the approach described here.
+
+Other MFE developers can take advantage of this plugin to deploy their own MFEs. To declare a new MFE, create a Tutor plugin and add your MFE configuration to the ``tutormfe.hooks.MFE_APPS`` filter. This configuration should include the name, git repository (and optionally: git branch) and development port. For example::
 
-    config = {
-        "defaults": {
-            "MYMFE_MFE_APP": {
-                "name": "mymfe",
-                "repository": "https://github.com/myorg/mymfe",
-                "port": 2001,
-                "version": "me/my-custom-branch", # optional
-            }
+    from tutormfe.hooks import MFE_APPS
+
+    @MFE_APPS.add()
+    def _add_my_mfe(mfes):
+        mfes["mymfe"] = {
+            "repository": "https://github.com/myorg/mymfe",
+            "port": 2001,
+            "version": "me/my-custom-branch", # optional, will default to the Open edX current tag.
         }
-    }
+        return mfes
 
-The MFE assets will then be bundled in the "mfe" Docker image whenever it is rebuilt with ``tutor images build mfe``. Assets will be served at ``http(s)://{{ MFE_HOST }}/{{ MYMFE_MFE_APP["name"] }}``. Developers are free to add extra template patches to their plugins, as usual: for instance LMS setting patches to make sure that the LMS correctly connects to the MFEs.
+The MFE assets will then be bundled in the "mfe" Docker image whenever it is rebuilt with ``tutor images build mfe``. Assets will be served at ``http(s)://{{ MFE_HOST }}/mymfe``. Developers are free to add extra template patches to their plugins, as usual: for instance LMS setting patches to make sure that the LMS correctly connects to the MFEs.
 
 Disabling individual MFEs
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-To disable an existing MFE, set its corresponding configuration setting to "null". For instance, to disable the MFEs that ship with this plugin::
+To disable an existing MFE, remove the corresponding entry from the ``MFE_APPS`` filter. For instance, to disable some of the MFEs that ship with this plugin::
 
-    tutor config save --set MFE_ACCOUNT_MFE_APP=null
-    tutor config save --set MFE_GRADEBOOK_MFE_APP=null
-    tutor config save --set MFE_PROFILE_MFE_APP=null
-    tutor config save --set MFE_COURSE_AUTHORING_MFE_APP=null
-    tutor config save --set MFE_DISCUSSIONS_MFE_APP=null
-    tutor config save --set MFE_AUTHN_MFE_APP=null
+
+    @MFE_APPS.add()
+    def _remove_some_my_mfe(mfes):
+        mfes.pop("account")
+        mfes.pop("profile")
+        ...
 
 Adding custom translations to your MFEs
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 This plugin makes it possible to change existing and add new translation strings to MFEs. Here is how to do it:
 
 1. Identify the ID of the string you would like to translate. For instance, the ID of the "Account Information" string in the account MFE is "account.settings.section.account.information" (see `source <https://github.com/edx/frontend-app-account/blob/1444831833cad4746b9ed14618a499b425ccc907/src/account-settings/AccountSettingsPage.messages.jsx#L34>`__).
@@ -268,39 +289,24 @@
 
     tutor dev start profile
 
 Then, access http://apps.local.overhang.io:1995/profile/u/YOURUSERNAME
 
 You can also bind-mount your own fork of an MFE. For example::
 
-    cd /path/to/frontend-app-profile
-    npm install  # Ensure NPM requirements are installed into your fork.
-    tutor dev start --mount=. profile
+    tutor config save --append MOUNTS=/path/to/frontend-app-profile
+    tutor dev launch
 
-The changes you make to your fork will be automatically picked up and hot-reloaded by your development server.
+With this change, the "profile-dev" image will be automatically re-built during ``launch``. Your host repository will then be bind-mounted at runtime in the "profile" container. This means that changes you make to the host repository will be automatically picked up and hot-reloaded by your development server.
 
 This works for custom MFEs, as well. For example, if you added your own MFE named frontend-app-myapp, then you can bind-mount it like so::
 
-    cd /path/to/frontend-app-myapp
-    npm install
-    tutor dev start --mount=. myapp
-
-However, if you try to bind-mount an unknown MFE, you will see a Docker Compose error such as::
-
-  ERROR: The Compose file is invalid because:
-  Service myapp has neither an image nor a build context specified. At least one must be provided.
-
-Please note that bind-mounting a fork is only available for development (``tutor dev ...``), since production MFEs are compiled and served out of a single container. If you want to use a fork of an MFE in production, then you will need to set the repository URL in ``$(tutor config printroot)/config.yml``::
+    tutor config save --append MOUNTS=/path/to/frontend-app-myapp
 
-    MFE_PROFILE_MFE_APP
-        name: profile
-        repository: "https://github.com/YOUR_FORK_ORGANIZATION/frontend-app-profile"
-        port: 1995
-
-and then rebuild the MFE container image with ``tutor images build mfe``.
+Similarly, in production, the "mfe" Docker image will be rebuilt automatically during ``tutor local launch``.
 
 Uninstall
 ---------
 
 To disable this plugin run::
 
     tutor plugins disable mfe
@@ -321,20 +327,25 @@
     # MFE discussions
     tutor local run lms ./manage.py lms waffle_delete --flags discussions.enable_discussions_mfe
     tutor local run lms ./manage.py lms waffle_delete --flags discussions.enable_learners_tab_in_discussions_mfe
     tutor local run lms ./manage.py lms waffle_delete --flags discussions.enable_moderation_reason_codes
     tutor local run lms ./manage.py lms waffle_delete --flags discussions.enable_reported_content_email_notifications
     tutor local run lms ./manage.py lms waffle_delete --flags discussions.enable_learners_stats
 
+    # MFE ora-grading
+    tutor local run lms ./manage.py lms waffle_delete --flags openresponseassessment.enhanced_staff_grader
+
 Finally, restart the platform with::
 
     tutor local launch
 
 Troubleshooting
 ---------------
 
 This Tutor plugin is maintained by Adolfo Brandes from `tCRIL <https://openedx.org>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
 
 License
 -------
 
 This software is licensed under the terms of the `GNU Affero General Public License (AGPL) <https://github.com/overhangio/tutor-mfe/blob/master/LICENSE.txt>`_.
+
+
```

### Comparing `tutor-mfe-15.0.7/README.rst` & `tutor-mfe-16.0.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Micro Frontend base plugin for `Tutor <https://docs.tutor.overhang.io>`__
 =========================================================================
 
 This plugin makes it possible to easily add micro frontend (MFE) applications on top of an Open edX platform that runs with Tutor. To learn more about MFEs, please check the `official Open edX documentation <https://edx.readthedocs.io/projects/edx-developer-docs/en/latest/developers_guide/micro_frontends_in_open_edx.html>`__.
 
 In addition, this plugin comes with a few MFEs which are enabled by default:
 
+- `Authn <https://github.com/openedx/frontend-app-authn/>`__
 - `Account <https://github.com/openedx/frontend-app-account/>`__
+- `Communications <https://github.com/openedx/frontend-app-communications/>`__
+- `Course Authoring <https://github.com/openedx/frontend-app-course-authoring/>`__
+- `Discussions <https://github.com/openedx/frontend-app-discussions/>`__
 - `Gradebook <https://github.com/openedx/frontend-app-gradebook/>`__
 - `Learning <https://github.com/openedx/frontend-app-learning/>`__
+- `ORA Grading <https://github.com/openedx/frontend-app-ora-grading/>`__
 - `Profile <https://github.com/openedx/frontend-app-profile/>`__
-- `Course Authoring <https://github.com/openedx/frontend-app-course-authoring/>`__
-- `Discussions <https://github.com/openedx/frontend-app-discussions/>`__
-- `Authn <https://github.com/openedx/frontend-app-authn/>`__
 
 Instructions for using each of these MFEs are given below.
 
 Installation
 ------------
 
 ::
@@ -28,27 +30,58 @@
 To enable this plugin, run::
 
     tutor plugins enable mfe
     tutor local launch
 
 When running the plugin in production, it is recommended that you set up a catch-all CNAME for subdomains at the DNS provider: see the `Configuring DNS Records <https://docs.tutor.overhang.io/install.html#configuring-dns-records>`__ section in the Tutor documentation for more details.  This way, the plugin will work out of the box with no additional configuration.  Which is to say, if your ``LMS_HOST`` is set to `myopenedx.com` the MFEs this plugin provides will be accessible under `apps.myopenedx.com` by default.
 
-To check what the current value of `MFE_HOST` is actually set to, run the following::
+To check what the current value of `MFE_HOST` is actually set to, run::
 
     tutor config printvalue MFE_HOST
 
+Authn
+~~~~~~~~~
+
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/authn.png
+    :alt: Authn MFE screenshot
+
+This is a micro-frontend application responsible for the login, registration and password reset functionality.
 
 Account
 ~~~~~~~
 
 .. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/account.png
     :alt: Account MFE screenshot
 
 An MFE to manage account-specific information for every LMS user. Each user's account page is available at ``http(s)://{{ MFE_HOST }}/account``. For instance, when running locally: https://apps.local.overhang.io/account.
 
+Communications
+~~~~~~~~~~~~~~
+
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/communications.png
+    :alt: Communications MFE screenshot
+
+The Communications micro-frontend exposes an interface for course teams to communicate with learners.  It achieves this by allowing instructors to send out emails in bulk, either by scheduling them or on demand.
+
+Course Authoring
+~~~~~~~~~~~~~~~~
+
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/course-authoring.png
+    :alt: Course Authoring MFE screenshot
+
+This MFE is meant for course authors and maintainers. For a given course, it exposes a "Pages & Resources" menu in Studio where one can enable or disable a variety of features, including, for example, the Wiki and Discussions.  Optionally, it allows authors to replace the legacy HTML, Video, and Problem authoring tools with experimental React-based versions, as well as exposing a new proctoring interface that can be enabled if the `edx-exams <https://github.com/edx/edx-exams>`_ service is available.
+
+Discussions
+~~~~~~~~~~~
+
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/discussions.png
+    :alt: Discussions MFE screenshot
+
+The Discussions MFE updates the previous discussions UI with a new look and better features.
+
 Gradebook
 ~~~~~~~~~
 
 .. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/gradebook.png
     :alt: Gradebook MFE screenshot
 
 This instructor-only MFE is for viewing individual and aggregated grade results for a course. To access this MFE, go to a course 🡒 🡒 Instructor tab 🡒 Student Admin 🡒 View gradebook. The URL should be: ``http(s)://{{ MFE_HOST }}/gradebook/{{ course ID }}``. When running locally, the gradebook of the demo course is available at: http://apps.local.overhang.io/gradebook/course-v1:edX+DemoX+Demo_Course
@@ -57,78 +90,65 @@
 ~~~~~~~~
 
 .. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/learning.png
     :alt: Learning MFE screenshot
 
 The Learning MFE replaces the former courseware, which is the core part of the LMS where students follow courses.
 
+ORA Grading
+~~~~~~~~~~~
+
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/ora-grading.png
+    :alt: ORA Grading MFE screenshot
+
+When enabled, Open Response Assesments ("ORA") that have a staff grading step will link to this new MFE, either when clicking "Grade Available Responses" from the exercise itself, or via a link in the Instructor Dashboard.  It is meant to streamline the grading process with better previews of submitted content.
+
 Profile
 ~~~~~~~~~
 
 .. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/profile.png
     :alt: Profile MFE screenshot
 
 Edit and display user-specific profile information. The profile page of every user is visible at ``http(s)://{{ MFE_HOST }}/profile/u/{{ username }}``. For instance, when running locally, the profile page of the "admin" user is: http://apps.local.overhang.io/profile/u/admin.
 
-Course Authoring
-~~~~~~~~~~~~~~~~
-
-.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/course-authoring.png
-    :alt: Course Authoring MFE screenshot
-
-This MFE is meant for course authors and maintainers. For a given course, it exposes a "Pages & Resources" menu in Studio where one can enable or disable a variety of features, including, for example, the Wiki and Discussions.  Optionally, it allows authors to replace the legacy HTML, Video, and Problem authoring tools with experimental React-based versions, as well as exposing a new proctoring interface that can be enabled if the `edx-exams <https://github.com/edx/edx-exams>`_ service is available.
-
-Discussions
-~~~~~~~~~~~
-
-.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/discussions.png
-    :alt: Discussions MFE screenshot
-
-The Discussions MFE updates the previous discussions UI with a new look and better features.
-
-Authn
-~~~~~~~~~
-
-.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/authn.png
-    :alt: Authn MFE screenshot
-
-This is a micro-frontend application responsible for the login, registration and password reset functionality.
 
 MFE management
 --------------
 
 Adding new MFEs
 ~~~~~~~~~~~~~~~
 
-Other Tutor plugin developers can take advantage of this plugin to deploy their own MFEs. To declare a new MFE, a new configuration setting should be created with the "_MFE_APP" suffix. This configuration setting should include the name, git repository (and optionally: git branch) and development port. For example::
+.. warning:: As of Tutor v16 (Palm release) it is no longer possible to add new MFEs by creating ``*_MFE_APP`` settings. Instead, users must implement the approach described here.
+
+Other MFE developers can take advantage of this plugin to deploy their own MFEs. To declare a new MFE, create a Tutor plugin and add your MFE configuration to the ``tutormfe.hooks.MFE_APPS`` filter. This configuration should include the name, git repository (and optionally: git branch) and development port. For example::
 
-    config = {
-        "defaults": {
-            "MYMFE_MFE_APP": {
-                "name": "mymfe",
-                "repository": "https://github.com/myorg/mymfe",
-                "port": 2001,
-                "version": "me/my-custom-branch", # optional
-            }
+    from tutormfe.hooks import MFE_APPS
+
+    @MFE_APPS.add()
+    def _add_my_mfe(mfes):
+        mfes["mymfe"] = {
+            "repository": "https://github.com/myorg/mymfe",
+            "port": 2001,
+            "version": "me/my-custom-branch", # optional, will default to the Open edX current tag.
         }
-    }
+        return mfes
 
-The MFE assets will then be bundled in the "mfe" Docker image whenever it is rebuilt with ``tutor images build mfe``. Assets will be served at ``http(s)://{{ MFE_HOST }}/{{ MYMFE_MFE_APP["name"] }}``. Developers are free to add extra template patches to their plugins, as usual: for instance LMS setting patches to make sure that the LMS correctly connects to the MFEs.
+The MFE assets will then be bundled in the "mfe" Docker image whenever it is rebuilt with ``tutor images build mfe``. Assets will be served at ``http(s)://{{ MFE_HOST }}/mymfe``. Developers are free to add extra template patches to their plugins, as usual: for instance LMS setting patches to make sure that the LMS correctly connects to the MFEs.
 
 Disabling individual MFEs
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-To disable an existing MFE, set its corresponding configuration setting to "null". For instance, to disable the MFEs that ship with this plugin::
+To disable an existing MFE, remove the corresponding entry from the ``MFE_APPS`` filter. For instance, to disable some of the MFEs that ship with this plugin::
 
-    tutor config save --set MFE_ACCOUNT_MFE_APP=null
-    tutor config save --set MFE_GRADEBOOK_MFE_APP=null
-    tutor config save --set MFE_PROFILE_MFE_APP=null
-    tutor config save --set MFE_COURSE_AUTHORING_MFE_APP=null
-    tutor config save --set MFE_DISCUSSIONS_MFE_APP=null
-    tutor config save --set MFE_AUTHN_MFE_APP=null
+
+    @MFE_APPS.add()
+    def _remove_some_my_mfe(mfes):
+        mfes.pop("account")
+        mfes.pop("profile")
+        ...
 
 Adding custom translations to your MFEs
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 This plugin makes it possible to change existing and add new translation strings to MFEs. Here is how to do it:
 
 1. Identify the ID of the string you would like to translate. For instance, the ID of the "Account Information" string in the account MFE is "account.settings.section.account.information" (see `source <https://github.com/edx/frontend-app-account/blob/1444831833cad4746b9ed14618a499b425ccc907/src/account-settings/AccountSettingsPage.messages.jsx#L34>`__).
@@ -241,39 +261,24 @@
 
     tutor dev start profile
 
 Then, access http://apps.local.overhang.io:1995/profile/u/YOURUSERNAME
 
 You can also bind-mount your own fork of an MFE. For example::
 
-    cd /path/to/frontend-app-profile
-    npm install  # Ensure NPM requirements are installed into your fork.
-    tutor dev start --mount=. profile
+    tutor config save --append MOUNTS=/path/to/frontend-app-profile
+    tutor dev launch
 
-The changes you make to your fork will be automatically picked up and hot-reloaded by your development server.
+With this change, the "profile-dev" image will be automatically re-built during ``launch``. Your host repository will then be bind-mounted at runtime in the "profile" container. This means that changes you make to the host repository will be automatically picked up and hot-reloaded by your development server.
 
 This works for custom MFEs, as well. For example, if you added your own MFE named frontend-app-myapp, then you can bind-mount it like so::
 
-    cd /path/to/frontend-app-myapp
-    npm install
-    tutor dev start --mount=. myapp
-
-However, if you try to bind-mount an unknown MFE, you will see a Docker Compose error such as::
+    tutor config save --append MOUNTS=/path/to/frontend-app-myapp
 
-  ERROR: The Compose file is invalid because:
-  Service myapp has neither an image nor a build context specified. At least one must be provided.
-
-Please note that bind-mounting a fork is only available for development (``tutor dev ...``), since production MFEs are compiled and served out of a single container. If you want to use a fork of an MFE in production, then you will need to set the repository URL in ``$(tutor config printroot)/config.yml``::
-
-    MFE_PROFILE_MFE_APP
-        name: profile
-        repository: "https://github.com/YOUR_FORK_ORGANIZATION/frontend-app-profile"
-        port: 1995
-
-and then rebuild the MFE container image with ``tutor images build mfe``.
+Similarly, in production, the "mfe" Docker image will be rebuilt automatically during ``tutor local launch``.
 
 Uninstall
 ---------
 
 To disable this plugin run::
 
     tutor plugins disable mfe
@@ -294,14 +299,17 @@
     # MFE discussions
     tutor local run lms ./manage.py lms waffle_delete --flags discussions.enable_discussions_mfe
     tutor local run lms ./manage.py lms waffle_delete --flags discussions.enable_learners_tab_in_discussions_mfe
     tutor local run lms ./manage.py lms waffle_delete --flags discussions.enable_moderation_reason_codes
     tutor local run lms ./manage.py lms waffle_delete --flags discussions.enable_reported_content_email_notifications
     tutor local run lms ./manage.py lms waffle_delete --flags discussions.enable_learners_stats
 
+    # MFE ora-grading
+    tutor local run lms ./manage.py lms waffle_delete --flags openresponseassessment.enhanced_staff_grader
+
 Finally, restart the platform with::
 
     tutor local launch
 
 Troubleshooting
 ---------------
```

### Comparing `tutor-mfe-15.0.7/setup.py` & `tutor-mfe-16.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     return about
 
 
 ABOUT = load_about()
 
 setup(
     name="tutor-mfe",
-    version=ABOUT["__version__"],
+    version=ABOUT["__package_version__"],
     url="https://github.com/overhangio/tutor-mfe",
     project_urls={
         "Code": "https://github.com/overhangio/tutor-mfe",
         "Issue tracker": "https://github.com/overhangio/tutor-mfe/issues",
         "Community": "https://discuss.openedx.org/tag/tutor",
     },
     license="AGPLv3",
@@ -36,15 +36,15 @@
     maintainer_email="adolfo@tcril.org",
     description="mfe plugin for Tutor",
     long_description=load_readme(),
     long_description_content_type="text/x-rst",
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
     python_requires=">=3.5",
-    install_requires=["tutor>=15.0.0,<16.0.0"],
+    install_requires=["tutor>=16.0.0,<17.0.0"],
     entry_points={"tutor.plugin.v1": ["mfe = tutormfe.plugin"]},
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
```

### Comparing `tutor-mfe-15.0.7/tutor_mfe.egg-info/PKG-INFO` & `tutor-mfe-16.0.0/tutor_mfe.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: tutor-mfe
-Version: 15.0.7
+Version: 16.0.0
 Summary: mfe plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-mfe
 Author: Overhang.IO
 Maintainer: tCRIL
 Maintainer-email: adolfo@tcril.org
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-mfe
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-mfe/issues
 Project-URL: Community, https://discuss.openedx.org/tag/tutor
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -28,21 +29,23 @@
 Micro Frontend base plugin for `Tutor <https://docs.tutor.overhang.io>`__
 =========================================================================
 
 This plugin makes it possible to easily add micro frontend (MFE) applications on top of an Open edX platform that runs with Tutor. To learn more about MFEs, please check the `official Open edX documentation <https://edx.readthedocs.io/projects/edx-developer-docs/en/latest/developers_guide/micro_frontends_in_open_edx.html>`__.
 
 In addition, this plugin comes with a few MFEs which are enabled by default:
 
+- `Authn <https://github.com/openedx/frontend-app-authn/>`__
 - `Account <https://github.com/openedx/frontend-app-account/>`__
+- `Communications <https://github.com/openedx/frontend-app-communications/>`__
+- `Course Authoring <https://github.com/openedx/frontend-app-course-authoring/>`__
+- `Discussions <https://github.com/openedx/frontend-app-discussions/>`__
 - `Gradebook <https://github.com/openedx/frontend-app-gradebook/>`__
 - `Learning <https://github.com/openedx/frontend-app-learning/>`__
+- `ORA Grading <https://github.com/openedx/frontend-app-ora-grading/>`__
 - `Profile <https://github.com/openedx/frontend-app-profile/>`__
-- `Course Authoring <https://github.com/openedx/frontend-app-course-authoring/>`__
-- `Discussions <https://github.com/openedx/frontend-app-discussions/>`__
-- `Authn <https://github.com/openedx/frontend-app-authn/>`__
 
 Instructions for using each of these MFEs are given below.
 
 Installation
 ------------
 
 ::
@@ -55,27 +58,58 @@
 To enable this plugin, run::
 
     tutor plugins enable mfe
     tutor local launch
 
 When running the plugin in production, it is recommended that you set up a catch-all CNAME for subdomains at the DNS provider: see the `Configuring DNS Records <https://docs.tutor.overhang.io/install.html#configuring-dns-records>`__ section in the Tutor documentation for more details.  This way, the plugin will work out of the box with no additional configuration.  Which is to say, if your ``LMS_HOST`` is set to `myopenedx.com` the MFEs this plugin provides will be accessible under `apps.myopenedx.com` by default.
 
-To check what the current value of `MFE_HOST` is actually set to, run the following::
+To check what the current value of `MFE_HOST` is actually set to, run::
 
     tutor config printvalue MFE_HOST
 
+Authn
+~~~~~~~~~
+
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/authn.png
+    :alt: Authn MFE screenshot
+
+This is a micro-frontend application responsible for the login, registration and password reset functionality.
 
 Account
 ~~~~~~~
 
 .. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/account.png
     :alt: Account MFE screenshot
 
 An MFE to manage account-specific information for every LMS user. Each user's account page is available at ``http(s)://{{ MFE_HOST }}/account``. For instance, when running locally: https://apps.local.overhang.io/account.
 
+Communications
+~~~~~~~~~~~~~~
+
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/communications.png
+    :alt: Communications MFE screenshot
+
+The Communications micro-frontend exposes an interface for course teams to communicate with learners.  It achieves this by allowing instructors to send out emails in bulk, either by scheduling them or on demand.
+
+Course Authoring
+~~~~~~~~~~~~~~~~
+
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/course-authoring.png
+    :alt: Course Authoring MFE screenshot
+
+This MFE is meant for course authors and maintainers. For a given course, it exposes a "Pages & Resources" menu in Studio where one can enable or disable a variety of features, including, for example, the Wiki and Discussions.  Optionally, it allows authors to replace the legacy HTML, Video, and Problem authoring tools with experimental React-based versions, as well as exposing a new proctoring interface that can be enabled if the `edx-exams <https://github.com/edx/edx-exams>`_ service is available.
+
+Discussions
+~~~~~~~~~~~
+
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/discussions.png
+    :alt: Discussions MFE screenshot
+
+The Discussions MFE updates the previous discussions UI with a new look and better features.
+
 Gradebook
 ~~~~~~~~~
 
 .. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/gradebook.png
     :alt: Gradebook MFE screenshot
 
 This instructor-only MFE is for viewing individual and aggregated grade results for a course. To access this MFE, go to a course 🡒 🡒 Instructor tab 🡒 Student Admin 🡒 View gradebook. The URL should be: ``http(s)://{{ MFE_HOST }}/gradebook/{{ course ID }}``. When running locally, the gradebook of the demo course is available at: http://apps.local.overhang.io/gradebook/course-v1:edX+DemoX+Demo_Course
@@ -84,78 +118,65 @@
 ~~~~~~~~
 
 .. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/learning.png
     :alt: Learning MFE screenshot
 
 The Learning MFE replaces the former courseware, which is the core part of the LMS where students follow courses.
 
+ORA Grading
+~~~~~~~~~~~
+
+.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/ora-grading.png
+    :alt: ORA Grading MFE screenshot
+
+When enabled, Open Response Assesments ("ORA") that have a staff grading step will link to this new MFE, either when clicking "Grade Available Responses" from the exercise itself, or via a link in the Instructor Dashboard.  It is meant to streamline the grading process with better previews of submitted content.
+
 Profile
 ~~~~~~~~~
 
 .. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/profile.png
     :alt: Profile MFE screenshot
 
 Edit and display user-specific profile information. The profile page of every user is visible at ``http(s)://{{ MFE_HOST }}/profile/u/{{ username }}``. For instance, when running locally, the profile page of the "admin" user is: http://apps.local.overhang.io/profile/u/admin.
 
-Course Authoring
-~~~~~~~~~~~~~~~~
-
-.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/course-authoring.png
-    :alt: Course Authoring MFE screenshot
-
-This MFE is meant for course authors and maintainers. For a given course, it exposes a "Pages & Resources" menu in Studio where one can enable or disable a variety of features, including, for example, the Wiki and Discussions.  Optionally, it allows authors to replace the legacy HTML, Video, and Problem authoring tools with experimental React-based versions, as well as exposing a new proctoring interface that can be enabled if the `edx-exams <https://github.com/edx/edx-exams>`_ service is available.
-
-Discussions
-~~~~~~~~~~~
-
-.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/discussions.png
-    :alt: Discussions MFE screenshot
-
-The Discussions MFE updates the previous discussions UI with a new look and better features.
-
-Authn
-~~~~~~~~~
-
-.. image:: https://raw.githubusercontent.com/overhangio/tutor-mfe/master/screenshots/authn.png
-    :alt: Authn MFE screenshot
-
-This is a micro-frontend application responsible for the login, registration and password reset functionality.
 
 MFE management
 --------------
 
 Adding new MFEs
 ~~~~~~~~~~~~~~~
 
-Other Tutor plugin developers can take advantage of this plugin to deploy their own MFEs. To declare a new MFE, a new configuration setting should be created with the "_MFE_APP" suffix. This configuration setting should include the name, git repository (and optionally: git branch) and development port. For example::
+.. warning:: As of Tutor v16 (Palm release) it is no longer possible to add new MFEs by creating ``*_MFE_APP`` settings. Instead, users must implement the approach described here.
+
+Other MFE developers can take advantage of this plugin to deploy their own MFEs. To declare a new MFE, create a Tutor plugin and add your MFE configuration to the ``tutormfe.hooks.MFE_APPS`` filter. This configuration should include the name, git repository (and optionally: git branch) and development port. For example::
 
-    config = {
-        "defaults": {
-            "MYMFE_MFE_APP": {
-                "name": "mymfe",
-                "repository": "https://github.com/myorg/mymfe",
-                "port": 2001,
-                "version": "me/my-custom-branch", # optional
-            }
+    from tutormfe.hooks import MFE_APPS
+
+    @MFE_APPS.add()
+    def _add_my_mfe(mfes):
+        mfes["mymfe"] = {
+            "repository": "https://github.com/myorg/mymfe",
+            "port": 2001,
+            "version": "me/my-custom-branch", # optional, will default to the Open edX current tag.
         }
-    }
+        return mfes
 
-The MFE assets will then be bundled in the "mfe" Docker image whenever it is rebuilt with ``tutor images build mfe``. Assets will be served at ``http(s)://{{ MFE_HOST }}/{{ MYMFE_MFE_APP["name"] }}``. Developers are free to add extra template patches to their plugins, as usual: for instance LMS setting patches to make sure that the LMS correctly connects to the MFEs.
+The MFE assets will then be bundled in the "mfe" Docker image whenever it is rebuilt with ``tutor images build mfe``. Assets will be served at ``http(s)://{{ MFE_HOST }}/mymfe``. Developers are free to add extra template patches to their plugins, as usual: for instance LMS setting patches to make sure that the LMS correctly connects to the MFEs.
 
 Disabling individual MFEs
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-To disable an existing MFE, set its corresponding configuration setting to "null". For instance, to disable the MFEs that ship with this plugin::
+To disable an existing MFE, remove the corresponding entry from the ``MFE_APPS`` filter. For instance, to disable some of the MFEs that ship with this plugin::
 
-    tutor config save --set MFE_ACCOUNT_MFE_APP=null
-    tutor config save --set MFE_GRADEBOOK_MFE_APP=null
-    tutor config save --set MFE_PROFILE_MFE_APP=null
-    tutor config save --set MFE_COURSE_AUTHORING_MFE_APP=null
-    tutor config save --set MFE_DISCUSSIONS_MFE_APP=null
-    tutor config save --set MFE_AUTHN_MFE_APP=null
+
+    @MFE_APPS.add()
+    def _remove_some_my_mfe(mfes):
+        mfes.pop("account")
+        mfes.pop("profile")
+        ...
 
 Adding custom translations to your MFEs
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 This plugin makes it possible to change existing and add new translation strings to MFEs. Here is how to do it:
 
 1. Identify the ID of the string you would like to translate. For instance, the ID of the "Account Information" string in the account MFE is "account.settings.section.account.information" (see `source <https://github.com/edx/frontend-app-account/blob/1444831833cad4746b9ed14618a499b425ccc907/src/account-settings/AccountSettingsPage.messages.jsx#L34>`__).
@@ -268,39 +289,24 @@
 
     tutor dev start profile
 
 Then, access http://apps.local.overhang.io:1995/profile/u/YOURUSERNAME
 
 You can also bind-mount your own fork of an MFE. For example::
 
-    cd /path/to/frontend-app-profile
-    npm install  # Ensure NPM requirements are installed into your fork.
-    tutor dev start --mount=. profile
+    tutor config save --append MOUNTS=/path/to/frontend-app-profile
+    tutor dev launch
 
-The changes you make to your fork will be automatically picked up and hot-reloaded by your development server.
+With this change, the "profile-dev" image will be automatically re-built during ``launch``. Your host repository will then be bind-mounted at runtime in the "profile" container. This means that changes you make to the host repository will be automatically picked up and hot-reloaded by your development server.
 
 This works for custom MFEs, as well. For example, if you added your own MFE named frontend-app-myapp, then you can bind-mount it like so::
 
-    cd /path/to/frontend-app-myapp
-    npm install
-    tutor dev start --mount=. myapp
-
-However, if you try to bind-mount an unknown MFE, you will see a Docker Compose error such as::
-
-  ERROR: The Compose file is invalid because:
-  Service myapp has neither an image nor a build context specified. At least one must be provided.
-
-Please note that bind-mounting a fork is only available for development (``tutor dev ...``), since production MFEs are compiled and served out of a single container. If you want to use a fork of an MFE in production, then you will need to set the repository URL in ``$(tutor config printroot)/config.yml``::
+    tutor config save --append MOUNTS=/path/to/frontend-app-myapp
 
-    MFE_PROFILE_MFE_APP
-        name: profile
-        repository: "https://github.com/YOUR_FORK_ORGANIZATION/frontend-app-profile"
-        port: 1995
-
-and then rebuild the MFE container image with ``tutor images build mfe``.
+Similarly, in production, the "mfe" Docker image will be rebuilt automatically during ``tutor local launch``.
 
 Uninstall
 ---------
 
 To disable this plugin run::
 
     tutor plugins disable mfe
@@ -321,20 +327,25 @@
     # MFE discussions
     tutor local run lms ./manage.py lms waffle_delete --flags discussions.enable_discussions_mfe
     tutor local run lms ./manage.py lms waffle_delete --flags discussions.enable_learners_tab_in_discussions_mfe
     tutor local run lms ./manage.py lms waffle_delete --flags discussions.enable_moderation_reason_codes
     tutor local run lms ./manage.py lms waffle_delete --flags discussions.enable_reported_content_email_notifications
     tutor local run lms ./manage.py lms waffle_delete --flags discussions.enable_learners_stats
 
+    # MFE ora-grading
+    tutor local run lms ./manage.py lms waffle_delete --flags openresponseassessment.enhanced_staff_grader
+
 Finally, restart the platform with::
 
     tutor local launch
 
 Troubleshooting
 ---------------
 
 This Tutor plugin is maintained by Adolfo Brandes from `tCRIL <https://openedx.org>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
 
 License
 -------
 
 This software is licensed under the terms of the `GNU Affero General Public License (AGPL) <https://github.com/overhangio/tutor-mfe/blob/master/LICENSE.txt>`_.
+
+
```

### Comparing `tutor-mfe-15.0.7/tutor_mfe.egg-info/SOURCES.txt` & `tutor-mfe-16.0.0/tutor_mfe.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 tutor_mfe.egg-info/SOURCES.txt
 tutor_mfe.egg-info/dependency_links.txt
 tutor_mfe.egg-info/entry_points.txt
 tutor_mfe.egg-info/requires.txt
 tutor_mfe.egg-info/top_level.txt
 tutormfe/__about__.py
 tutormfe/__init__.py
+tutormfe/hooks.py
 tutormfe/plugin.py
 tutormfe/patches/.gitignore
 tutormfe/patches/caddyfile
 tutormfe/patches/k8s-deployments
 tutormfe/patches/k8s-services
 tutormfe/patches/kustomization-configmapgenerator
 tutormfe/patches/local-docker-compose-dev-services
```

### Comparing `tutor-mfe-15.0.7/tutormfe/patches/k8s-deployments` & `tutor-mfe-16.0.0/tutormfe/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-mfe-15.0.7/tutormfe/patches/openedx-lms-production-settings` & `tutor-mfe-16.0.0/tutormfe/patches/openedx-lms-production-settings`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,12 @@
-{% if MFE_ACCOUNT_MFE_APP %}
-ACCOUNT_MICROFRONTEND_URL = "{% if ENABLE_HTTPS %}https://{% else %}http://{% endif %}{{ MFE_HOST }}/{{ MFE_ACCOUNT_MFE_APP["name"] }}"
-{% endif %}
-{% if MFE_GRADEBOOK_MFE_APP %}
-WRITABLE_GRADEBOOK_URL = "{% if ENABLE_HTTPS %}https://{% else %}http://{% endif %}{{ MFE_HOST }}/{{ MFE_GRADEBOOK_MFE_APP["name"] }}"
-{% endif %}
-{% if MFE_LEARNING_MFE_APP %}
-LEARNING_MICROFRONTEND_URL = "{% if ENABLE_HTTPS %}https://{% else %}http://{% endif %}{{ MFE_HOST }}/{{ MFE_LEARNING_MFE_APP["name"] }}"
-{% endif %}
-{% if MFE_PROFILE_MFE_APP %}
-PROFILE_MICROFRONTEND_URL = "{% if ENABLE_HTTPS %}https://{% else %}http://{% endif %}{{ MFE_HOST }}/{{ MFE_PROFILE_MFE_APP["name"] }}/u/"
-{% endif %}
-{% if MFE_DISCUSSIONS_MFE_APP %}
-DISCUSSIONS_MICROFRONTEND_URL = "{% if ENABLE_HTTPS %}https://{% else %}http://{% endif %}{{ MFE_HOST }}/{{ MFE_DISCUSSIONS_MFE_APP["name"] }}"
-DISCUSSIONS_MFE_FEEDBACK_URL = None
-{% endif %}
-
-{% if MFE_AUTHN_MFE_APP %}
-AUTHN_MICROFRONTEND_URL = "{% if ENABLE_HTTPS %}https://{% else %}http://{% endif %}{{ MFE_HOST }}/{{ MFE_AUTHN_MFE_APP["name"] }}"
-AUTHN_MICROFRONTEND_DOMAIN  = "{{ MFE_HOST }}/{{ MFE_AUTHN_MFE_APP["name"] }}"
-{% endif %}
-
-LOGIN_REDIRECT_WHITELIST.append("{{ MFE_HOST }}")
-CORS_ORIGIN_WHITELIST.append("{% if ENABLE_HTTPS %}https://{% else %}http://{% endif %}{{ MFE_HOST }}")
-CSRF_TRUSTED_ORIGINS.append("{{ MFE_HOST }}")
-
 # Dynamic config API settings
 # https://openedx.github.io/frontend-platform/module-Config.html
 MFE_CONFIG = {
     "BASE_URL": "{{ MFE_HOST }}",
     "CSRF_TOKEN_API_PATH": "/csrf/api/v1/token",
-{%- if MFE_ACCOUNT_MFE_APP %}
-    "ACCOUNT_SETTINGS_URL": ACCOUNT_MICROFRONTEND_URL,
-{%- endif %}
-{%- if MFE_PROFILE_MFE_APP %}
-    "ACCOUNT_PROFILE_URL": "{% if ENABLE_HTTPS %}https://{% else %}http://{% endif %}{{ MFE_HOST }}/{{ MFE_PROFILE_MFE_APP["name"] }}",
-{%- endif %}
     "CREDENTIALS_BASE_URL": "",
     "DISCOVERY_API_BASE_URL": "{% if DISCOVERY_HOST is defined %}{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ DISCOVERY_HOST }}{% endif %}",
     "FAVICON_URL": "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ LMS_HOST }}/favicon.ico",
     "LANGUAGE_PREFERENCE_COOKIE_NAME": "openedx-language-preference",
     "LMS_BASE_URL": "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ LMS_HOST }}",
     "LOGIN_URL": "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ LMS_HOST }}/login",
     "LOGO_URL": "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ LMS_HOST }}/theming/asset/images/logo.png",
@@ -47,21 +15,46 @@
     "LOGOUT_URL": "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ LMS_HOST }}/logout",
     "MARKETING_SITE_BASE_URL": "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ LMS_HOST }}",
     "REFRESH_ACCESS_TOKEN_ENDPOINT": "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ LMS_HOST }}/login_refresh",
     "SITE_NAME": "{{ PLATFORM_NAME }}",
     "STUDIO_BASE_URL": "{{ "https" if ENABLE_HTTPS else "http" }}://{{ CMS_HOST }}",
     "USER_INFO_COOKIE_NAME": "user-info",
     "ACCESS_TOKEN_COOKIE_NAME": "edx-jwt-cookie-header-payload",
-{%- if MFE_LEARNING_MFE_APP %}
-    "LEARNING_BASE_URL": "{{ "https" if ENABLE_HTTPS else "http" }}://{{ MFE_HOST }}/{{ MFE_LEARNING_MFE_APP["name"] }}",
-{%- endif %}
-{%- if MFE_COURSE_AUTHORING_MFE_APP %}
-    "ENABLE_NEW_EDITOR_PAGES": True,
-    "ENABLE_PROGRESS_GRAPH_SETTINGS": True,
-{%- endif %}
-{%- if MFE_AUTHN_MFE_APP %}
-    "DISABLE_ENTERPRISE_LOGIN": True,
-{%- endif %}
 }
 
+# MFE-specific settings
+{% for app_name, app in iter_mfes() %}
+{% if app_name == "authn" %}
+AUTHN_MICROFRONTEND_URL = "{% if ENABLE_HTTPS %}https://{% else %}http://{% endif %}{{ MFE_HOST }}/authn"
+AUTHN_MICROFRONTEND_DOMAIN  = "{{ MFE_HOST }}/authn"
+MFE_CONFIG["DISABLE_ENTERPRISE_LOGIN"] = True
+{% elif app_name == "account" %}
+ACCOUNT_MICROFRONTEND_URL = "{% if ENABLE_HTTPS %}https://{% else %}http://{% endif %}{{ MFE_HOST }}/account"
+MFE_CONFIG["ACCOUNT_SETTINGS_URL"] = ACCOUNT_MICROFRONTEND_URL
+{% elif app_name == "course-authoring" %}
+MFE_CONFIG["ENABLE_NEW_EDITOR_PAGES"] = True
+MFE_CONFIG["ENABLE_PROGRESS_GRAPH_SETTINGS"] = True
+{% elif app_name == "discussions" %}
+DISCUSSIONS_MICROFRONTEND_URL = "{% if ENABLE_HTTPS %}https://{% else %}http://{% endif %}{{ MFE_HOST }}/discussions"
+DISCUSSIONS_MFE_FEEDBACK_URL = None
+{% elif app_name == "gradebook" %}
+WRITABLE_GRADEBOOK_URL = "{% if ENABLE_HTTPS %}https://{% else %}http://{% endif %}{{ MFE_HOST }}/gradebook"
+{% elif app_name == "learning" %}
+LEARNING_MICROFRONTEND_URL = "{% if ENABLE_HTTPS %}https://{% else %}http://{% endif %}{{ MFE_HOST }}/learning"
+MFE_CONFIG["LEARNING_BASE_URL"] = "{{ "https" if ENABLE_HTTPS else "http" }}://{{ MFE_HOST }}/learning"
+{% elif app_name == "ora-grading" %}
+ORA_GRADING_MICROFRONTEND_URL = "{% if ENABLE_HTTPS %}https://{% else %}http://{% endif %}{{ MFE_HOST }}/ora-grading"
+{% elif app_name == "profile" %}
+PROFILE_MICROFRONTEND_URL = "{% if ENABLE_HTTPS %}https://{% else %}http://{% endif %}{{ MFE_HOST }}/profile/u/"
+MFE_CONFIG["ACCOUNT_PROFILE_URL"] = "{% if ENABLE_HTTPS %}https://{% else %}http://{% endif %}{{ MFE_HOST }}/profile"
+{% elif app_name == "communications" %}
+COMMUNICATIONS_MICROFRONTEND_URL = "{% if ENABLE_HTTPS %}https://{% else %}http://{% endif %}{{ MFE_HOST }}/communications"
+MFE_CONFIG["SCHEDULE_EMAIL_SECTION"] = True
+{% endif %}
+{% endfor %}
+
+LOGIN_REDIRECT_WHITELIST.append("{{ MFE_HOST }}")
+CORS_ORIGIN_WHITELIST.append("{% if ENABLE_HTTPS %}https://{% else %}http://{% endif %}{{ MFE_HOST }}")
+CSRF_TRUSTED_ORIGINS.append("{{ MFE_HOST }}")
+
 {{ patch("mfe-lms-common-settings") }}
 {{ patch("mfe-lms-production-settings") }}
```

### Comparing `tutor-mfe-15.0.7/tutormfe/plugin.py` & `tutor-mfe-16.0.0/tutormfe/plugin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,104 @@
+from __future__ import annotations
+
 from glob import glob
 import os
+import typing as t
+
 import pkg_resources
 
 from tutor import hooks as tutor_hooks
 from tutor.hooks import priorities
 
 from .__about__ import __version__
+from .hooks import MFE_ATTRS_TYPE, MFE_APPS
 
 config = {
     "defaults": {
         "VERSION": __version__,
         "DOCKER_IMAGE": "{{ DOCKER_REGISTRY }}overhangio/openedx-mfe:{{ MFE_VERSION }}",
         "HOST": "apps.{{ LMS_HOST }}",
         "COMMON_VERSION": "{{ OPENEDX_COMMON_VERSION }}",
         "CADDY_DOCKER_IMAGE": "{{ DOCKER_IMAGE_CADDY }}",
-        "AUTHN_MFE_APP": {
-            "name": "authn",
-            "repository": "https://github.com/openedx/frontend-app-authn",
-            "port": 1999,
-        },
-        "ACCOUNT_MFE_APP": {
-            "name": "account",
-            "repository": "https://github.com/openedx/frontend-app-account",
-            "port": 1997,
-        },
-        "COURSE_AUTHORING_MFE_APP": {
-            "name": "course-authoring",
-            "repository": "https://github.com/openedx/frontend-app-course-authoring",
-            "port": 2001,
-        },
-        "DISCUSSIONS_MFE_APP": {
-            "name": "discussions",
-            "repository": "https://github.com/openedx/frontend-app-discussions",
-            "port": 2002,
-        },
-        "GRADEBOOK_MFE_APP": {
-            "name": "gradebook",
-            "repository": "https://github.com/openedx/frontend-app-gradebook",
-            "port": 1994,
-        },
-        "LEARNING_MFE_APP": {
-            "name": "learning",
-            "repository": "https://github.com/openedx/frontend-app-learning",
-            "port": 2000,
-        },
-        "PROFILE_MFE_APP": {
-            "name": "profile",
-            "repository": "https://github.com/openedx/frontend-app-profile",
-            "port": 1995,
-        },
     },
 }
-ALL_MFES = (
-    "account",
-    "course-authoring",
-    "discussions",
-    "authn",
-    "gradebook",
-    "learning",
-    "profile",
+
+
+CORE_MFE_APPS: dict[str, MFE_ATTRS_TYPE] = {
+    "authn": {
+        "repository": "https://github.com/openedx/frontend-app-authn",
+        "port": 1999,
+    },
+    "account": {
+        "repository": "https://github.com/openedx/frontend-app-account",
+        "port": 1997,
+    },
+    "communications": {
+        "repository": "https://github.com/openedx/frontend-app-communications",
+        "port": 1984,
+    },
+    "course-authoring": {
+        "repository": "https://github.com/openedx/frontend-app-course-authoring",
+        "port": 2001,
+    },
+    "discussions": {
+        "repository": "https://github.com/openedx/frontend-app-discussions",
+        "port": 2002,
+    },
+    "gradebook": {
+        "repository": "https://github.com/openedx/frontend-app-gradebook",
+        "port": 1994,
+    },
+    "learning": {
+        "repository": "https://github.com/openedx/frontend-app-learning",
+        "port": 2000,
+    },
+    "ora-grading": {
+        "repository": "https://github.com/openedx/frontend-app-ora-grading",
+        "port": 1993,
+    },
+    "profile": {
+        "repository": "https://github.com/openedx/frontend-app-profile",
+        "port": 1995,
+    },
+}
+
+
+# The core MFEs are added with a high priority, such that other users can override or
+# remove them.
+@MFE_APPS.add(priority=tutor_hooks.priorities.HIGH)
+def _add_core_mfe_apps(apps: dict[str, MFE_ATTRS_TYPE]) -> dict[str, MFE_ATTRS_TYPE]:
+    apps.update(CORE_MFE_APPS)
+    return apps
+
+
+def iter_mfes() -> t.Iterable[tuple[str, MFE_ATTRS_TYPE]]:
+    """
+    Yield:
+
+        (name, dict)
+    """
+    yield from MFE_APPS.apply({}).items()
+
+
+def is_mfe_enabled(mfe_name: str) -> bool:
+    return mfe_name in MFE_APPS.apply({})
+
+
+# Make the mfe functions available within templates
+tutor_hooks.Filters.ENV_TEMPLATE_VARIABLES.add_items(
+    [("iter_mfes", iter_mfes), ("is_mfe_enabled", is_mfe_enabled)]
 )
 
-with open(
-    os.path.join(
-        pkg_resources.resource_filename("tutormfe", "templates"),
-        "mfe",
-        "tasks",
-        "lms",
-        "init",
-    ),
-    encoding="utf-8",
-) as task_file:
-    tutor_hooks.Filters.CLI_DO_INIT_TASKS.add_item(("lms", task_file.read()))
 
 # Build, pull and push mfe base image
 tutor_hooks.Filters.IMAGES_BUILD.add_item(
     (
         "mfe",
-        ("plugins", "mfe", "build", "mfe"),
+        os.path.join("plugins", "mfe", "build", "mfe"),
         "{{ MFE_DOCKER_IMAGE }}",
         (),
     )
 )
 tutor_hooks.Filters.IMAGES_PULL.add_item(
     (
         "mfe",
@@ -91,49 +108,103 @@
 tutor_hooks.Filters.IMAGES_PUSH.add_item(
     (
         "mfe",
         "{{ MFE_DOCKER_IMAGE }}",
     )
 )
 
+
 # Build, pull and push {mfe}-dev images
-for mfe in ALL_MFES:
-    name = f"{mfe}-dev"
-    tag = "{{ DOCKER_REGISTRY }}overhangio/openedx-" + mfe + "-dev:{{ MFE_VERSION }}"
+for mfe_name, mfe_attrs in iter_mfes():
+    name = f"{mfe_name}-dev"
+    tag = "{{ DOCKER_REGISTRY }}overhangio/openedx-" + name + ":{{ MFE_VERSION }}"
     tutor_hooks.Filters.IMAGES_BUILD.add_item(
         (
             name,
-            ("plugins", "mfe", "build", "mfe"),
+            os.path.join("plugins", "mfe", "build", "mfe"),
             tag,
-            (f"--target={mfe}-dev",),
+            (f"--target={mfe_name}-dev",),
         )
     )
     tutor_hooks.Filters.IMAGES_PULL.add_item((name, tag))
     tutor_hooks.Filters.IMAGES_PUSH.add_item((name, tag))
 
 
+# init script
+with open(
+    os.path.join(
+        pkg_resources.resource_filename("tutormfe", "templates"),
+        "mfe",
+        "tasks",
+        "lms",
+        "init",
+    ),
+    encoding="utf-8",
+) as task_file:
+    tutor_hooks.Filters.CLI_DO_INIT_TASKS.add_item(("lms", task_file.read()))
+
+REPO_PREFIX = "frontend-app-"
+
+
 @tutor_hooks.Filters.COMPOSE_MOUNTS.add()
-def _mount_frontend_apps(volumes, name):
+def _mount_frontend_apps(volumes, path_basename):
     """
     If the user mounts any repo named frontend-app-APPNAME, then make sure
     it's available in the APPNAME service container. This is only applicable
     in dev mode, because in production, all MFEs are built and hosted on the
     singular 'mfe' service container.
     """
-    prefix = "frontend-app-"
-    if name.startswith(prefix):
+    if path_basename.startswith(REPO_PREFIX):
         # Assumption:
         # For each repo named frontend-app-APPNAME, there is an associated
         # docker-compose service named APPNAME. If this assumption is broken,
         # then Tutor will try to mount the repo in a service that doesn't exist.
-        app_name = name.split(prefix)[1]
+        app_name = path_basename[len(REPO_PREFIX) :]
         volumes += [(app_name, "/openedx/app")]
     return volumes
 
 
+@tutor_hooks.Filters.IMAGES_BUILD_MOUNTS.add()
+def _mount_frontend_apps_on_build(
+    mounts: list[tuple[str, str]], host_path: str
+) -> list[tuple[str, str]]:
+    path_basename = os.path.basename(host_path)
+    if path_basename.startswith(REPO_PREFIX):
+        # Bind-mount repo at build-time, both for prod and dev images
+        app_name = path_basename[len(REPO_PREFIX) :]
+        mounts.append(("mfe", f"{app_name}-src"))
+        mounts.append((f"{app_name}-dev", f"{app_name}-src"))
+    return mounts
+
+
+@tutor_hooks.Filters.APP_PUBLIC_HOSTS.add()
+def _print_mfe_public_hosts(
+    hostnames: list[str], context_name: t.Literal["local", "dev"]
+) -> list[str]:
+    if context_name == "local":
+        hostnames.append("{{ MFE_HOST }}")
+    else:
+        for mfe_name, mfe_attrs in iter_mfes():
+            hostnames.append("{{ MFE_HOST }}" + f":{mfe_attrs['port']}/{mfe_name}")
+    return hostnames
+
+
+@tutor_hooks.Filters.IMAGES_BUILD_REQUIRED.add()
+def _build_3rd_party_dev_mfes_on_launch(
+    image_names: list[str], context_name: t.Literal["local", "dev"]
+) -> list[str]:
+    if context_name == "dev":
+        for mfe_name, _mfe_attrs in iter_mfes():
+            if mfe_name not in CORE_MFE_APPS:
+                # We don't require to build core MFEs because images are available from
+                # the public registry.
+                image_names.append(f"{mfe_name}-dev")
+    return image_names
+
+
 # Boilerplate code
 # Add the "templates" folder as a template root
 tutor_hooks.Filters.ENV_TEMPLATE_ROOTS.add_item(
     pkg_resources.resource_filename("tutormfe", "templates")
 )
 # Render the "build" and "apps" folders
 tutor_hooks.Filters.ENV_TEMPLATE_TARGETS.add_items(
```

### Comparing `tutor-mfe-15.0.7/tutormfe/templates/mfe/apps/mfe/webpack.dev-tutor.config.js` & `tutor-mfe-16.0.0/tutormfe/templates/mfe/apps/mfe/webpack.dev-tutor.config.js`

 * *Files identical despite different names*

### Comparing `tutor-mfe-15.0.7/tutormfe/templates/mfe/build/mfe/Dockerfile` & `tutor-mfe-16.0.0/tutormfe/templates/mfe/build/mfe/Dockerfile`

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,98 @@
-FROM docker.io/node:16.14-bullseye-slim AS base
+# https://hub.docker.com/_/node/tags
+FROM docker.io/node:18.16.0-bullseye-slim AS base
 
 RUN apt update \
   && apt install -y git \
     # required for cwebp-bin
     gcc libgl1 libxi6 make \
     # required for gifsicle, mozjpeg, and optipng (on arm)
     autoconf libtool pkg-config zlib1g-dev \
     # required for node-sass (on arm)
     python g++ \
     # required for image-webpack-loader (on arm)
-    libpng-dev
+    libpng-dev \
+    # required for building node-canvas (on arm, for course-authoring)
+    # https://www.npmjs.com/package/canvas
+    libcairo2-dev libpango1.0-dev libjpeg-dev libgif-dev librsvg2-dev
 
 RUN mkdir -p /openedx/app /openedx/env
 WORKDIR /openedx/app
 ENV PATH ./node_modules/.bin:${PATH}
 
 ######## i18n strings
 FROM base AS i18n
 COPY ./i18n /openedx/i18n
 RUN chmod a+x /openedx/i18n/*.js
 RUN echo "copying i18n data" \
-  {%- for app in iter_values_named(suffix="MFE_APP") %}
-  && mkdir -p /openedx/i18n/{{ app["name"] }} \
+  {%- for app_name, app in iter_mfes() %}
+  && mkdir -p /openedx/i18n/{{ app_name }} \
   {%- endfor %}
   echo "done."
-{% for app in iter_values_named(suffix="MFE_APP") %}
-################ {{ app["name"] }} MFE
-######## {{ app["name"] }} (src)
-FROM base AS {{ app["name"] }}-src
+
+{% for app_name, app in iter_mfes() %}
+####################### {{ app_name }} MFE
+######## {{ app_name }} (git)
+FROM base AS {{ app_name }}-git
 RUN git clone {{ app["repository"] }} --branch {{ app.get("version", MFE_COMMON_VERSION) }} --depth 1 .
-RUN stat /openedx/app/src/i18n/messages 2> /dev/null || (echo "missing messages folder" && mkdir -p /openedx/app/src/i18n/messages)
 
-######## {{ app["name"] }} (i18n)
-FROM base AS {{ app["name"] }}-i18n
-COPY --from={{ app["name"] }}-src /openedx/app/src/i18n/messages /openedx/app/src/i18n/messages
-COPY --from=i18n /openedx/i18n/{{ app["name"] }} /openedx/i18n/{{ app["name"] }}
+######## {{ app_name }} (src)
+# Empty layer with just the repo at the root, for build-time bind-mounts
+FROM scratch as {{ app_name }}-src
+COPY --from={{ app_name }}-git /openedx/app /
+
+######## {{ app_name }} (i18n)
+FROM base AS {{ app_name }}-i18n
+COPY --from={{ app_name }}-src / /openedx/app
+COPY --from=i18n /openedx/i18n/{{ app_name }} /openedx/i18n/{{ app_name }}
 COPY --from=i18n /openedx/i18n/i18n-merge.js /openedx/i18n/i18n-merge.js
-RUN /openedx/i18n/i18n-merge.js /openedx/app/src/i18n/messages /openedx/i18n/{{ app["name"] }} /openedx/app/src/i18n/messages
+RUN stat /openedx/app/src/i18n/messages 2> /dev/null || (echo "missing messages folder" && mkdir -p /openedx/app/src/i18n/messages)
+RUN /openedx/i18n/i18n-merge.js /openedx/app/src/i18n/messages /openedx/i18n/{{ app_name }} /openedx/app/src/i18n/messages
 
-######## {{ app["name"] }} (common)
-FROM base AS {{ app["name"] }}-common
-COPY --from={{ app["name"] }}-src /openedx/app/package.json /openedx/app/package.json
-COPY --from={{ app["name"] }}-src /openedx/app/package-lock.json /openedx/app/package-lock.json
+######## {{ app_name }} (common)
+FROM base AS {{ app_name }}-common
+COPY --from={{ app_name }}-src /package.json /openedx/app/package.json
+COPY --from={{ app_name }}-src /package-lock.json /openedx/app/package-lock.json
 ARG NPM_REGISTRY={{ NPM_REGISTRY }}
 {{ patch("mfe-dockerfile-pre-npm-install") }}
 {#- Required for building optipng on M1 #}
 ENV CPPFLAGS=-DPNG_ARM_NEON_OPT=0
 {#- We define this environment variable to bypass an issue with the installation of pact https://github.com/pact-foundation/pact-js-core/issues/264 #}
 ENV PACT_SKIP_BINARY_INSTALL=true
-RUN npm clean-install --no-audit --no-fund --registry=$NPM_REGISTRY \
-  && rm -rf ~/.npm
+RUN {% if is_buildkit_enabled() %}--mount=type=cache,target=/root/.npm,sharing=shared {% endif %}npm clean-install --no-audit --no-fund --registry=$NPM_REGISTRY
 {{ patch("mfe-dockerfile-post-npm-install") }}
-COPY --from={{ app["name"] }}-src /openedx/app /openedx/app
-COPY --from={{ app["name"] }}-i18n /openedx/app/src/i18n/messages /openedx/app/src/i18n/messages
+COPY --from={{ app_name }}-src / /openedx/app
+COPY --from={{ app_name }}-i18n /openedx/app/src/i18n/messages /openedx/app/src/i18n/messages
 EXPOSE {{ app['port'] }}
 
 # Configuration needed at build time
-ENV APP_ID={{ app["name"] }}
-ENV PUBLIC_PATH='/{{ app["name"] }}/'
+ENV APP_ID={{ app_name }}
+ENV PUBLIC_PATH='/{{ app_name }}/'
 # We could in theory point the mfe_config API directly to the LMS. But for that we would
 # have to code the LMS url into the mfe image, and this configuration is user-dependent.
 # So we point to a relative url that will be a proxy for the LMS.
 ENV MFE_CONFIG_API_URL=/api/mfe_config/v1
 ARG ENABLE_NEW_RELIC=false
 
-######## {{ app["name"] }} (dev)
-FROM {{ app["name"] }}-common AS {{ app["name"] }}-dev
+######## {{ app_name }} (dev)
+FROM {{ app_name }}-common AS {{ app_name }}-dev
 ENV NODE_ENV=development
 CMD ["/bin/bash", "-c", "npm run start --- --config ./webpack.dev-tutor.config.js"]
 {% endfor %}
 
 # Production images are last to accelerate dev image building
-{%- for app in iter_values_named(suffix="MFE_APP") %}
-######## {{ app["name"] }} (production)
-FROM {{ app["name"] }}-common AS {{ app["name"] }}-prod
+{%- for app_name, app in iter_mfes() %}
+######## {{ app_name }} (production)
+FROM {{ app_name }}-common AS {{ app_name }}-prod
 ENV NODE_ENV=production
 RUN npm run build
 {% endfor %}
 
 ####### final production image with all static assets
 FROM {{ MFE_CADDY_DOCKER_IMAGE }} as production
 
 RUN mkdir -p /openedx/dist
 
 # Copy static assets
-{% for app in iter_values_named(suffix="MFE_APP") %}
-COPY --from={{ app["name"] }}-prod /openedx/app/dist /openedx/dist/{{ app["name"] }}
+{% for app_name, app in iter_mfes() %}
+COPY --from={{ app_name }}-prod /openedx/app/dist /openedx/dist/{{ app_name }}
 {% endfor %}
```

### Comparing `tutor-mfe-15.0.7/tutormfe/templates/mfe/build/mfe/i18n/i18n-merge.js` & `tutor-mfe-16.0.0/tutormfe/templates/mfe/build/mfe/i18n/i18n-merge.js`

 * *Files identical despite different names*

### Comparing `tutor-mfe-15.0.7/tutormfe/templates/mfe/tasks/lms/init` & `tutor-mfe-16.0.0/tutormfe/templates/mfe/tasks/lms/init`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,55 @@
-{% if MFE_ACCOUNT_MFE_APP %}
+# MFE-specific tasks
+{% if is_mfe_enabled("account") %}
 (./manage.py lms waffle_flag --list | grep account.redirect_to_microfrontend) || ./manage.py lms waffle_flag --create --everyone account.redirect_to_microfrontend
 ./manage.py lms populate_retirement_states
 {% else %}
 ./manage.py lms waffle_delete --flags account.redirect_to_microfrontend
 {% endif %}
 
-{% if MFE_PROFILE_MFE_APP %}
+{% if is_mfe_enabled("profile") %}
 (./manage.py lms waffle_flag --list | grep learner_profile.redirect_to_microfrontend) || ./manage.py lms waffle_flag --create --everyone learner_profile.redirect_to_microfrontend
 site-configuration set --domain={{ LMS_HOST }} ENABLE_PROFILE_MICROFRONTEND true
 site-configuration set --domain={{ LMS_HOST }}:8000 ENABLE_PROFILE_MICROFRONTEND true
 {% else %}
 site-configuration unset --domain={{ LMS_HOST }} ENABLE_PROFILE_MICROFRONTEND
 site-configuration unset --domain={{ LMS_HOST }}:8000 ENABLE_PROFILE_MICROFRONTEND
 ./manage.py lms waffle_delete --flags learner_profile.redirect_to_microfrontend
 {% endif %}
 
-{% if MFE_LEARNING_MFE_APP %}
+{% if is_mfe_enabled("learning") %}
 (./manage.py lms waffle_flag --list | grep course_home.course_home_mfe_progress_tab) || ./manage.py lms waffle_flag --create --everyone course_home.course_home_mfe_progress_tab
 {% else %}
 ./manage.py lms waffle_delete --flags course_home.course_home_mfe_progress_tab
 {% endif %}
 
-{% if MFE_COURSE_AUTHORING_MFE_APP %}
+{% if is_mfe_enabled("course-authoring") %}
 (./manage.py lms waffle_flag --list | grep discussions.pages_and_resources_mfe) || ./manage.py lms waffle_flag --create --everyone discussions.pages_and_resources_mfe
 (./manage.py lms waffle_flag --list | grep new_core_editors.use_new_text_editor) || ./manage.py lms waffle_flag --create --deactivate new_core_editors.use_new_text_editor
 (./manage.py lms waffle_flag --list | grep new_core_editors.use_new_video_editor) || ./manage.py lms waffle_flag --create --deactivate new_core_editors.use_new_video_editor
 (./manage.py lms waffle_flag --list | grep new_core_editors.use_new_problem_editor) || ./manage.py lms waffle_flag --create --deactivate new_core_editors.use_new_problem_editor
 {% else %}
 ./manage.py lms waffle_delete --flags discussions.pages_and_resources_mfe
 ./manage.py lms waffle_delete --flags new_core_editors.use_new_text_editor
 ./manage.py lms waffle_delete --flags new_core_editors.use_new_video_editor
 ./manage.py lms waffle_delete --flags new_core_editors.use_new_problem_editor
 {% endif %}
 
-{% if MFE_DISCUSSIONS_MFE_APP %}
+{% if is_mfe_enabled("discussions") %}
 (./manage.py lms waffle_flag --list | grep discussions.enable_discussions_mfe ) || ./manage.py lms waffle_flag --create --everyone discussions.enable_discussions_mfe
 (./manage.py lms waffle_flag --list | grep discussions.enable_learners_tab_in_discussions_mfe ) || ./manage.py lms waffle_flag --create --everyone discussions.enable_learners_tab_in_discussions_mfe
 (./manage.py lms waffle_flag --list | grep discussions.enable_moderation_reason_codes ) || ./manage.py lms waffle_flag --create --everyone discussions.enable_moderation_reason_codes
 (./manage.py lms waffle_flag --list | grep discussions.enable_reported_content_email_notifications ) || ./manage.py lms waffle_flag --create --everyone discussions.enable_reported_content_email_notifications
 (./manage.py lms waffle_flag --list | grep discussions.enable_learners_stats ) || ./manage.py lms waffle_flag --create --everyone discussions.enable_learners_stats
 {% else %}
 ./manage.py lms waffle_delete --flags discussions.enable_discussions_mfe
 ./manage.py lms waffle_delete --flags discussions.enable_learners_tab_in_discussions_mfe
 ./manage.py lms waffle_delete --flags discussions.enable_moderation_reason_codes
 ./manage.py lms waffle_delete --flags discussions.enable_reported_content_email_notifications
 ./manage.py lms waffle_delete --flags discussions.enable_learners_stats
 {% endif %}
+
+{% if is_mfe_enabled("ora-grading") %}
+(./manage.py lms waffle_flag --list | grep openresponseassessment.enhanced_staff_grader) || ./manage.py lms waffle_flag --create --everyone openresponseassessment.enhanced_staff_grader
+{% else %}
+./manage.py lms waffle_delete --flags openresponseassessment.enhanced_staff_grader
+{% endif %}
```

