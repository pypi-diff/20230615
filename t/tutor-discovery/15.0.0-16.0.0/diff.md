# Comparing `tmp/tutor-discovery-15.0.0.tar.gz` & `tmp/tutor-discovery-16.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tutor-discovery-15.0.0.tar", last modified: Mon Dec 12 18:43:09 2022, max compression
+gzip compressed data, was "tutor-discovery-16.0.0.tar", last modified: Wed Jun 14 23:03:16 2023, max compression
```

## Comparing `tutor-discovery-15.0.0.tar` & `tutor-discovery-16.0.0.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 18:43:09.000000 tutor-discovery-15.0.0/
--rw-r--r--   0 ci        (1000) ci        (1000)       88 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     7043 2022-12-12 18:43:09.000000 tutor-discovery-15.0.0/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     4949 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2022-12-12 18:43:09.000000 tutor-discovery-15.0.0/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1850 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 18:43:09.000000 tutor-discovery-15.0.0/tutor_discovery.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     7043 2022-12-12 18:43:08.000000 tutor-discovery-15.0.0/tutor_discovery.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     1431 2022-12-12 18:43:08.000000 tutor-discovery-15.0.0/tutor_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2022-12-12 18:43:08.000000 tutor-discovery-15.0.0/tutor_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       53 2022-12-12 18:43:08.000000 tutor-discovery-15.0.0/tutor_discovery.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       22 2022-12-12 18:43:08.000000 tutor-discovery-15.0.0/tutor_discovery.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       15 2022-12-12 18:43:08.000000 tutor-discovery-15.0.0/tutor_discovery.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 18:43:09.000000 tutor-discovery-15.0.0/tutordiscovery/
--rw-r--r--   0 ci        (1000) ci        (1000)       24 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 18:43:09.000000 tutor-discovery-15.0.0/tutordiscovery/patches/
--rw-r--r--   0 ci        (1000) ci        (1000)      139 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/patches/caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)      132 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/patches/dev-docker-compose-jobs-services
--rw-r--r--   0 ci        (1000) ci        (1000)      846 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/patches/k8s-deployments
--rw-r--r--   0 ci        (1000) ci        (1000)      623 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/patches/k8s-jobs
--rw-r--r--   0 ci        (1000) ci        (1000)      180 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/patches/k8s-services
--rw-r--r--   0 ci        (1000) ci        (1000)       94 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/patches/kustomization-configmapgenerator
--rw-r--r--   0 ci        (1000) ci        (1000)       23 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/patches/local-docker-compose-caddy-aliases
--rw-r--r--   0 ci        (1000) ci        (1000)      275 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/patches/local-docker-compose-dev-services
--rw-r--r--   0 ci        (1000) ci        (1000)      283 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/patches/local-docker-compose-jobs-services
--rw-r--r--   0 ci        (1000) ci        (1000)      380 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/patches/local-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)       43 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/patches/openedx-lms-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     3239 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 18:43:09.000000 tutor-discovery-15.0.0/tutordiscovery/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 18:43:09.000000 tutor-discovery-15.0.0/tutordiscovery/templates/discovery/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 18:43:09.000000 tutor-discovery-15.0.0/tutordiscovery/templates/discovery/apps/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 18:43:09.000000 tutor-discovery-15.0.0/tutordiscovery/templates/discovery/apps/settings/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 18:43:09.000000 tutor-discovery-15.0.0/tutordiscovery/templates/discovery/apps/settings/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)     3044 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/templates/discovery/apps/settings/partials/common.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 18:43:09.000000 tutor-discovery-15.0.0/tutordiscovery/templates/discovery/apps/settings/tutor/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/templates/discovery/apps/settings/tutor/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      836 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/templates/discovery/apps/settings/tutor/development.py
--rw-r--r--   0 ci        (1000) ci        (1000)      863 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/templates/discovery/apps/settings/tutor/production.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 18:43:09.000000 tutor-discovery-15.0.0/tutordiscovery/templates/discovery/build/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 18:43:09.000000 tutor-discovery-15.0.0/tutordiscovery/templates/discovery/build/discovery/
--rw-r--r--   0 ci        (1000) ci        (1000)     2563 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/templates/discovery/build/discovery/Dockerfile
--rw-r--r--   0 ci        (1000) ci        (1000)      260 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/templates/discovery/build/discovery/assets.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 18:43:09.000000 tutor-discovery-15.0.0/tutordiscovery/templates/discovery/tasks/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 18:43:09.000000 tutor-discovery-15.0.0/tutordiscovery/templates/discovery/tasks/discovery/
--rw-r--r--   0 ci        (1000) ci        (1000)      974 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/templates/discovery/tasks/discovery/init
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 18:43:09.000000 tutor-discovery-15.0.0/tutordiscovery/templates/discovery/tasks/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)     2827 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/templates/discovery/tasks/lms/init
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 18:43:09.000000 tutor-discovery-15.0.0/tutordiscovery/templates/discovery/tasks/mysql/
--rw-r--r--   0 ci        (1000) ci        (1000)      821 2022-12-12 18:43:03.000000 tutor-discovery-15.0.0/tutordiscovery/templates/discovery/tasks/mysql/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:03:16.887456 tutor-discovery-16.0.0/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       88 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     7233 2023-06-14 23:03:16.884123 tutor-discovery-16.0.0/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     6055 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/pyproject.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-14 23:03:16.887456 tutor-discovery-16.0.0/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1851 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:03:16.877456 tutor-discovery-16.0.0/tutor_discovery.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     7233 2023-06-14 23:03:16.000000 tutor-discovery-16.0.0/tutor_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     1458 2023-06-14 23:03:16.000000 tutor-discovery-16.0.0/tutor_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-06-14 23:03:16.000000 tutor-discovery-16.0.0/tutor_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       52 2023-06-14 23:03:16.000000 tutor-discovery-16.0.0/tutor_discovery.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-06-14 23:03:16.000000 tutor-discovery-16.0.0/tutor_discovery.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       15 2023-06-14 23:03:16.000000 tutor-discovery-16.0.0/tutor_discovery.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:03:16.880789 tutor-discovery-16.0.0/tutordiscovery/
+-rw-r--r--   0 ci        (1000) ci        (1000)      176 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:03:16.884123 tutor-discovery-16.0.0/tutordiscovery/patches/
+-rw-r--r--   0 ci        (1000) ci        (1000)      139 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/patches/caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      132 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/patches/dev-docker-compose-jobs-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      846 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/patches/k8s-deployments
+-rw-r--r--   0 ci        (1000) ci        (1000)      623 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/patches/k8s-jobs
+-rw-r--r--   0 ci        (1000) ci        (1000)      180 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/patches/k8s-services
+-rw-r--r--   0 ci        (1000) ci        (1000)       94 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/patches/kustomization-configmapgenerator
+-rw-r--r--   0 ci        (1000) ci        (1000)       23 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/patches/local-docker-compose-caddy-aliases
+-rw-r--r--   0 ci        (1000) ci        (1000)      275 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/patches/local-docker-compose-dev-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      280 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      396 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/patches/local-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)       43 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/patches/openedx-lms-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)     4113 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:03:16.874123 tutor-discovery-16.0.0/tutordiscovery/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:03:16.874123 tutor-discovery-16.0.0/tutordiscovery/templates/discovery/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:03:16.874123 tutor-discovery-16.0.0/tutordiscovery/templates/discovery/apps/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:03:16.874123 tutor-discovery-16.0.0/tutordiscovery/templates/discovery/apps/settings/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:03:16.884123 tutor-discovery-16.0.0/tutordiscovery/templates/discovery/apps/settings/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)     3044 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/templates/discovery/apps/settings/partials/common.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:03:16.884123 tutor-discovery-16.0.0/tutordiscovery/templates/discovery/apps/settings/tutor/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/templates/discovery/apps/settings/tutor/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      836 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/templates/discovery/apps/settings/tutor/development.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      863 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/templates/discovery/apps/settings/tutor/production.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:03:16.874123 tutor-discovery-16.0.0/tutordiscovery/templates/discovery/build/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:03:16.884123 tutor-discovery-16.0.0/tutordiscovery/templates/discovery/build/discovery/
+-rw-r--r--   0 ci        (1000) ci        (1000)     3869 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/templates/discovery/build/discovery/Dockerfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      260 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/templates/discovery/build/discovery/assets.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:03:16.877456 tutor-discovery-16.0.0/tutordiscovery/templates/discovery/tasks/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:03:16.884123 tutor-discovery-16.0.0/tutordiscovery/templates/discovery/tasks/discovery/
+-rw-r--r--   0 ci        (1000) ci        (1000)      974 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/templates/discovery/tasks/discovery/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:03:16.884123 tutor-discovery-16.0.0/tutordiscovery/templates/discovery/tasks/lms/
+-rw-r--r--   0 ci        (1000) ci        (1000)     2827 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/templates/discovery/tasks/lms/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:03:16.884123 tutor-discovery-16.0.0/tutordiscovery/templates/discovery/tasks/mysql/
+-rw-r--r--   0 ci        (1000) ci        (1000)      821 2023-06-14 23:03:09.000000 tutor-discovery-16.0.0/tutordiscovery/templates/discovery/tasks/mysql/init
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tutor-discovery-15.0.0/PKG-INFO` & `tutor-discovery-16.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,141 +1,158 @@
 Metadata-Version: 2.1
 Name: tutor-discovery
-Version: 15.0.0
+Version: 16.0.0
 Summary: A Tutor plugin for course discovery, the Open edX service for providing access to consolidated course and program metadata
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: Overhang.IO
 Maintainer-email: regis@overhang.io
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
 Project-URL: Code, https://github.com/overhangio/tutor-discovery
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-discovery/issues
 Project-URL: Community, https://discuss.openedx.org
-Description: Course Discovery plugin for `Tutor <https://docs.tutor.overhang.io>`_
-        =====================================================================
-        
-        This is a plugin for `Tutor <https://docs.tutor.overhang.io>`_ that integrates the `Course Discovery <https://github.com/edx/course-discovery/>`__ application in an Open edX platform. it is useful for integration with, for example, `Ecommerce <https://github.com/edx/ecommerce>`__ or an external course catalog.
-        
-        Installation
-        ------------
-        
-        This plugin requires tutor>=3.6.0. If you have installed tutor from a pre-compiled binary, it already comes bundled with the discovery plugin. Otherwise::
-        
-            pip install tutor-discovery
-        
-        Then, to enable this plugin, run::
-        
-            tutor plugins enable discovery
-        
-        You will have to re-generate the environment::
-        
-            tutor config save
-        
-        Then, run migrations::
-        
-            tutor local init
-        
-        This last step is unnecessary if you run instead ``tutor local launch``.
-        
-        Operations
-        ----------
-        
-        Creating a user
-        ~~~~~~~~~~~~~~~
-        
-        The discovery user interface will be available at http://discovery.local.overhang.io for a local test instance, and at ``DISCOVERY_HOST`` (by default: http(s)://discovery.<your lms host>) in production. In order to run commands from the UI, a user must be created::
-        
-            tutor local run discovery ./manage.py createsuperuser
-        
-        Then, you must login with this user at http://discovery.local.overhang.io/admin.
-        
-        Alternatively, you can login with oauth2 using a pre-existing user created on the LMS/CMS by accessing http(s)://discovery.<your lms host>/login. To do so, the proper domain names must exist and point to the production server.
-        
-        Index configuration
-        ~~~~~~~~~~~~~~~~~~~
-        
-        Discovery uses separate indices for different models (the names are: course, course_run, person and program by default). And you can overwrite theses
-        names by configuring ``DISCOVERY_INDEX_OVERRIDES``::
-        
-            DISCOVERY_INDEX_OVERRIDES:
-              course_discovery.apps.course_metadata.search_indexes.documents.course: your-course-index-name
-              course_discovery.apps.course_metadata.search_indexes.documents.course_run: your-course-run-index-name
-              course_discovery.apps.course_metadata.search_indexes.documents.person: your-person-index-name
-              course_discovery.apps.course_metadata.search_indexes.documents.program: your-program-index-name
-        
-        Re-indexing courses
-        ~~~~~~~~~~~~~~~~~~~
-        
-        ::
-        
-            tutor local run discovery ./manage.py refresh_course_metadata --partner_code=openedx
-            tutor local run discovery ./manage.py update_index --disable-change-limit
-        
-        Caching programs
-        ~~~~~~~~~~~~~~~~
-        
-        In order to cache programs in the LMS, you will need to manually create a catalog integration. This step should be performed just once::
-        
-            tutor local run lms ./manage.py lms create_catalog_integrations --enabled \
-                --internal_api_url="" \
-                --service_username=lms_catalog_service_user
-        
-        Then::
-        
-            tutor local run lms ./manage.py lms cache_programs
-        
-        This last step should be performed every time you create new or make changes to existing programs.
-        
-        Debugging
-        ---------
-        
-        To debug the course discovery service, you are encouraged to mount the course-discovery repo from the host in the development container:
-        
-            tutor dev start --mount /path/to/course-discovery/ discovery
-        
-        You can then access the development server at http://discovery.local.overhang.io:8381. Feel free to add breakpoints (``import pdb; pdb.set_trace()``) anywhere in your source code to debug your application.
-        
-        Once a local repository is mounted in the image, you will have to install nodejs dependencies and collect static assets::
-        
-            tutor dev run discovery npm install --development
-            tutor dev run discovery make static.dev
-        
-        Troubleshooting
-        ---------------
-        
-        This Tutor plugin is maintained by Régis Behmo from `Overhang.IO <https://overhang.io>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
-        
-        
-        `Max retries exceeded with url`
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        When running in production with HTTPS enabled, you may face this error during the `init` phase of `tutor local launch`:
-        
-        ```
-        requests.exceptions.ConnectionError: HTTPSConnectionPool(host='<LMS_HOST>', port=443): Max retries exceeded with url: /api/courses/v1/courses/?page=1&page_size=10&username=discovery
-        ```
-        
-        This error may be due to an incorrect DNS resolution of the LMS DNS record. With some cloud providers (for instance: [DigitalOcean](https://digitalocean.com/)) the `/etc/hosts` file on the host automatically contains the following entry::
-        
-            127.0.1.1 <LMS HOST>
-        
-        This entry may be present if you named your server with the LMS hostname.
-        
-        License
-        -------
-        
-        This work is licensed under the terms of the `GNU Affero General Public License (AGPL) <https://github.com/overhangio/tutor/blob/master/LICENSE.txt>`_.
-        
-Platform: UNKNOWN
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
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
+Course Discovery plugin for `Tutor <https://docs.tutor.overhang.io>`_
+=====================================================================
+
+This is a plugin for `Tutor <https://docs.tutor.overhang.io>`_ that integrates the `Course Discovery <https://github.com/edx/course-discovery/>`__ application in an Open edX platform. it is useful for integration with, for example, `Ecommerce <https://github.com/edx/ecommerce>`__ or an external course catalog.
+
+Installation
+------------
+
+This plugin requires tutor>=3.6.0. If you have installed tutor from a pre-compiled binary, it already comes bundled with the discovery plugin. Otherwise::
+
+    tutor plugins install discovery
+
+Then, to enable this plugin, run::
+
+    tutor plugins enable discovery
+
+You will have to re-generate the environment::
+
+    tutor config save
+
+Then, run migrations::
+
+    tutor local init
+
+This last step is unnecessary if you run instead ``tutor local launch``.
+
+Operations
+----------
+
+Creating a user
+~~~~~~~~~~~~~~~
+
+The discovery user interface will be available at http://discovery.local.overhang.io for a local test instance, and at ``DISCOVERY_HOST`` (by default: http(s)://discovery.<your lms host>) in production. In order to run commands from the UI, a user must be created::
+
+    tutor local run discovery ./manage.py createsuperuser
+
+Then, you must login with this user at http://discovery.local.overhang.io/admin.
+
+Alternatively, you can login with oauth2 using a pre-existing user created on the LMS/CMS by accessing http(s)://discovery.<your lms host>/login. To do so, the proper domain names must exist and point to the production server.
+
+Index configuration
+~~~~~~~~~~~~~~~~~~~
+
+Discovery uses separate indices for different models (the names are: course, course_run, person and program by default). And you can overwrite theses
+names by configuring ``DISCOVERY_INDEX_OVERRIDES``::
+
+    DISCOVERY_INDEX_OVERRIDES:
+      course_discovery.apps.course_metadata.search_indexes.documents.course: your-course-index-name
+      course_discovery.apps.course_metadata.search_indexes.documents.course_run: your-course-run-index-name
+      course_discovery.apps.course_metadata.search_indexes.documents.person: your-person-index-name
+      course_discovery.apps.course_metadata.search_indexes.documents.program: your-program-index-name
+
+Re-indexing courses
+~~~~~~~~~~~~~~~~~~~
+
+::
+
+    tutor local run discovery ./manage.py refresh_course_metadata --partner_code=openedx
+    tutor local run discovery ./manage.py update_index --disable-change-limit
+
+Caching programs
+~~~~~~~~~~~~~~~~
+
+In order to cache programs in the LMS, you will need to manually create a catalog integration. Make sure you use staff user for the below command. If ``lms_catalog_service_user`` is not a staff user, then make it a staff user in your LMS User model. This step should be performed just once::
+
+    tutor local run lms ./manage.py lms create_catalog_integrations --enabled \
+        --internal_api_url="" \
+        --service_username=lms_catalog_service_user
+
+Then run the below command, this command will cause errors every time as it tries to cache programs from all sites that are added to your LMS sites model::
+
+    tutor local run lms ./manage.py lms cache_programs
+
+If you don't want the errors, then make use of an extra argumet to the command .i.e. ``--domain``. This argument will be equal to ``local.overhang.io`` if you are running tutor local and ``local.overhang.io:8000`` if you are running tutor dev::
+    tutor local run lms ./manage.py lms cache_programs --domain="local.overhang.io"
+    or
+    tutor dev run lms ./manage.py lms cache_programs --domain="local.overhang.io:8000"
+
+This last step should be performed every time you create new or make changes to existing programs.
+
+Install extra requirements
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+In order to install extra requirements, use DISCOVERY_EXTRA_PIP_REQUIREMENTS and re-build the docker image.::
+
+  tutor config save \
+    --set 'DISCOVERY_EXTRA_PIP_REQUIREMENTS=["git+https://github.com/myusername/myplugin"]'
+
+Then, build the image, pointing to your fork if necessary::
+
+  tutor images build discovery
+
+Debugging
+---------
+
+To debug the course discovery service, you are encouraged to mount the course-discovery repo from the host in the development container:
+
+    tutor dev start --mount /path/to/course-discovery/ discovery
+
+You can then access the development server at http://discovery.local.overhang.io:8381. Feel free to add breakpoints (``import pdb; pdb.set_trace()``) anywhere in your source code to debug your application.
+
+Once a local repository is mounted in the image, you will have to install nodejs dependencies and collect static assets::
+
+    tutor dev run discovery npm install --development
+    tutor dev run discovery make static.dev
+
+Troubleshooting
+---------------
+
+This Tutor plugin is maintained by Régis Behmo from `Overhang.IO <https://overhang.io>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
+
+
+`Max retries exceeded with url`
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+When running in production with HTTPS enabled, you may face this error during the `init` phase of `tutor local launch`:
+
+```
+requests.exceptions.ConnectionError: HTTPSConnectionPool(host='<LMS_HOST>', port=443): Max retries exceeded with url: /api/courses/v1/courses/?page=1&page_size=10&username=discovery
+```
+
+This error may be due to an incorrect DNS resolution of the LMS DNS record. With some cloud providers (for instance: [DigitalOcean](https://digitalocean.com/)) the `/etc/hosts` file on the host automatically contains the following entry::
+
+    127.0.1.1 <LMS HOST>
+
+This entry may be present if you named your server with the LMS hostname.
+
+License
+-------
+
+This work is licensed under the terms of the `GNU Affero General Public License (AGPL) <https://github.com/overhangio/tutor/blob/master/LICENSE.txt>`_.
```

### Comparing `tutor-discovery-15.0.0/README.rst` & `tutor-discovery-16.0.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This is a plugin for `Tutor <https://docs.tutor.overhang.io>`_ that integrates the `Course Discovery <https://github.com/edx/course-discovery/>`__ application in an Open edX platform. it is useful for integration with, for example, `Ecommerce <https://github.com/edx/ecommerce>`__ or an external course catalog.
 
 Installation
 ------------
 
 This plugin requires tutor>=3.6.0. If you have installed tutor from a pre-compiled binary, it already comes bundled with the discovery plugin. Otherwise::
 
-    pip install tutor-discovery
+    tutor plugins install discovery
 
 Then, to enable this plugin, run::
 
     tutor plugins enable discovery
 
 You will have to re-generate the environment::
 
@@ -57,26 +57,43 @@
 
     tutor local run discovery ./manage.py refresh_course_metadata --partner_code=openedx
     tutor local run discovery ./manage.py update_index --disable-change-limit
 
 Caching programs
 ~~~~~~~~~~~~~~~~
 
-In order to cache programs in the LMS, you will need to manually create a catalog integration. This step should be performed just once::
+In order to cache programs in the LMS, you will need to manually create a catalog integration. Make sure you use staff user for the below command. If ``lms_catalog_service_user`` is not a staff user, then make it a staff user in your LMS User model. This step should be performed just once::
 
     tutor local run lms ./manage.py lms create_catalog_integrations --enabled \
         --internal_api_url="" \
         --service_username=lms_catalog_service_user
 
-Then::
+Then run the below command, this command will cause errors every time as it tries to cache programs from all sites that are added to your LMS sites model::
 
     tutor local run lms ./manage.py lms cache_programs
 
+If you don't want the errors, then make use of an extra argumet to the command .i.e. ``--domain``. This argument will be equal to ``local.overhang.io`` if you are running tutor local and ``local.overhang.io:8000`` if you are running tutor dev::
+    tutor local run lms ./manage.py lms cache_programs --domain="local.overhang.io"
+    or
+    tutor dev run lms ./manage.py lms cache_programs --domain="local.overhang.io:8000"
+
 This last step should be performed every time you create new or make changes to existing programs.
 
+Install extra requirements
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+In order to install extra requirements, use DISCOVERY_EXTRA_PIP_REQUIREMENTS and re-build the docker image.::
+
+  tutor config save \
+    --set 'DISCOVERY_EXTRA_PIP_REQUIREMENTS=["git+https://github.com/myusername/myplugin"]'
+
+Then, build the image, pointing to your fork if necessary::
+
+  tutor images build discovery
+
 Debugging
 ---------
 
 To debug the course discovery service, you are encouraged to mount the course-discovery repo from the host in the development container:
 
     tutor dev start --mount /path/to/course-discovery/ discovery
```

### Comparing `tutor-discovery-15.0.0/setup.py` & `tutor-discovery-16.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,22 +30,22 @@
     maintainer="Overhang.IO",
     maintainer_email="regis@overhang.io",
     description="A Tutor plugin for course discovery, the Open edX service for providing access to consolidated course and program metadata",
     long_description=readme,
     long_description_content_type="text/x-rst",
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
-    install_requires=["tutor>=15.0.0,<16.0.0"],
-    python_requires=">=3.7",
+    install_requires=["tutor>=16.0.0,<17.0.0"],
+    python_requires=">=3.8",
     entry_points={"tutor.plugin.v1": ["discovery = tutordiscovery.plugin"]},
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

### Comparing `tutor-discovery-15.0.0/tutor_discovery.egg-info/PKG-INFO` & `tutor-discovery-16.0.0/tutor_discovery.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,141 +1,158 @@
 Metadata-Version: 2.1
 Name: tutor-discovery
-Version: 15.0.0
+Version: 16.0.0
 Summary: A Tutor plugin for course discovery, the Open edX service for providing access to consolidated course and program metadata
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: Overhang.IO
 Maintainer-email: regis@overhang.io
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
 Project-URL: Code, https://github.com/overhangio/tutor-discovery
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-discovery/issues
 Project-URL: Community, https://discuss.openedx.org
-Description: Course Discovery plugin for `Tutor <https://docs.tutor.overhang.io>`_
-        =====================================================================
-        
-        This is a plugin for `Tutor <https://docs.tutor.overhang.io>`_ that integrates the `Course Discovery <https://github.com/edx/course-discovery/>`__ application in an Open edX platform. it is useful for integration with, for example, `Ecommerce <https://github.com/edx/ecommerce>`__ or an external course catalog.
-        
-        Installation
-        ------------
-        
-        This plugin requires tutor>=3.6.0. If you have installed tutor from a pre-compiled binary, it already comes bundled with the discovery plugin. Otherwise::
-        
-            pip install tutor-discovery
-        
-        Then, to enable this plugin, run::
-        
-            tutor plugins enable discovery
-        
-        You will have to re-generate the environment::
-        
-            tutor config save
-        
-        Then, run migrations::
-        
-            tutor local init
-        
-        This last step is unnecessary if you run instead ``tutor local launch``.
-        
-        Operations
-        ----------
-        
-        Creating a user
-        ~~~~~~~~~~~~~~~
-        
-        The discovery user interface will be available at http://discovery.local.overhang.io for a local test instance, and at ``DISCOVERY_HOST`` (by default: http(s)://discovery.<your lms host>) in production. In order to run commands from the UI, a user must be created::
-        
-            tutor local run discovery ./manage.py createsuperuser
-        
-        Then, you must login with this user at http://discovery.local.overhang.io/admin.
-        
-        Alternatively, you can login with oauth2 using a pre-existing user created on the LMS/CMS by accessing http(s)://discovery.<your lms host>/login. To do so, the proper domain names must exist and point to the production server.
-        
-        Index configuration
-        ~~~~~~~~~~~~~~~~~~~
-        
-        Discovery uses separate indices for different models (the names are: course, course_run, person and program by default). And you can overwrite theses
-        names by configuring ``DISCOVERY_INDEX_OVERRIDES``::
-        
-            DISCOVERY_INDEX_OVERRIDES:
-              course_discovery.apps.course_metadata.search_indexes.documents.course: your-course-index-name
-              course_discovery.apps.course_metadata.search_indexes.documents.course_run: your-course-run-index-name
-              course_discovery.apps.course_metadata.search_indexes.documents.person: your-person-index-name
-              course_discovery.apps.course_metadata.search_indexes.documents.program: your-program-index-name
-        
-        Re-indexing courses
-        ~~~~~~~~~~~~~~~~~~~
-        
-        ::
-        
-            tutor local run discovery ./manage.py refresh_course_metadata --partner_code=openedx
-            tutor local run discovery ./manage.py update_index --disable-change-limit
-        
-        Caching programs
-        ~~~~~~~~~~~~~~~~
-        
-        In order to cache programs in the LMS, you will need to manually create a catalog integration. This step should be performed just once::
-        
-            tutor local run lms ./manage.py lms create_catalog_integrations --enabled \
-                --internal_api_url="" \
-                --service_username=lms_catalog_service_user
-        
-        Then::
-        
-            tutor local run lms ./manage.py lms cache_programs
-        
-        This last step should be performed every time you create new or make changes to existing programs.
-        
-        Debugging
-        ---------
-        
-        To debug the course discovery service, you are encouraged to mount the course-discovery repo from the host in the development container:
-        
-            tutor dev start --mount /path/to/course-discovery/ discovery
-        
-        You can then access the development server at http://discovery.local.overhang.io:8381. Feel free to add breakpoints (``import pdb; pdb.set_trace()``) anywhere in your source code to debug your application.
-        
-        Once a local repository is mounted in the image, you will have to install nodejs dependencies and collect static assets::
-        
-            tutor dev run discovery npm install --development
-            tutor dev run discovery make static.dev
-        
-        Troubleshooting
-        ---------------
-        
-        This Tutor plugin is maintained by Régis Behmo from `Overhang.IO <https://overhang.io>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
-        
-        
-        `Max retries exceeded with url`
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        When running in production with HTTPS enabled, you may face this error during the `init` phase of `tutor local launch`:
-        
-        ```
-        requests.exceptions.ConnectionError: HTTPSConnectionPool(host='<LMS_HOST>', port=443): Max retries exceeded with url: /api/courses/v1/courses/?page=1&page_size=10&username=discovery
-        ```
-        
-        This error may be due to an incorrect DNS resolution of the LMS DNS record. With some cloud providers (for instance: [DigitalOcean](https://digitalocean.com/)) the `/etc/hosts` file on the host automatically contains the following entry::
-        
-            127.0.1.1 <LMS HOST>
-        
-        This entry may be present if you named your server with the LMS hostname.
-        
-        License
-        -------
-        
-        This work is licensed under the terms of the `GNU Affero General Public License (AGPL) <https://github.com/overhangio/tutor/blob/master/LICENSE.txt>`_.
-        
-Platform: UNKNOWN
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
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
+Course Discovery plugin for `Tutor <https://docs.tutor.overhang.io>`_
+=====================================================================
+
+This is a plugin for `Tutor <https://docs.tutor.overhang.io>`_ that integrates the `Course Discovery <https://github.com/edx/course-discovery/>`__ application in an Open edX platform. it is useful for integration with, for example, `Ecommerce <https://github.com/edx/ecommerce>`__ or an external course catalog.
+
+Installation
+------------
+
+This plugin requires tutor>=3.6.0. If you have installed tutor from a pre-compiled binary, it already comes bundled with the discovery plugin. Otherwise::
+
+    tutor plugins install discovery
+
+Then, to enable this plugin, run::
+
+    tutor plugins enable discovery
+
+You will have to re-generate the environment::
+
+    tutor config save
+
+Then, run migrations::
+
+    tutor local init
+
+This last step is unnecessary if you run instead ``tutor local launch``.
+
+Operations
+----------
+
+Creating a user
+~~~~~~~~~~~~~~~
+
+The discovery user interface will be available at http://discovery.local.overhang.io for a local test instance, and at ``DISCOVERY_HOST`` (by default: http(s)://discovery.<your lms host>) in production. In order to run commands from the UI, a user must be created::
+
+    tutor local run discovery ./manage.py createsuperuser
+
+Then, you must login with this user at http://discovery.local.overhang.io/admin.
+
+Alternatively, you can login with oauth2 using a pre-existing user created on the LMS/CMS by accessing http(s)://discovery.<your lms host>/login. To do so, the proper domain names must exist and point to the production server.
+
+Index configuration
+~~~~~~~~~~~~~~~~~~~
+
+Discovery uses separate indices for different models (the names are: course, course_run, person and program by default). And you can overwrite theses
+names by configuring ``DISCOVERY_INDEX_OVERRIDES``::
+
+    DISCOVERY_INDEX_OVERRIDES:
+      course_discovery.apps.course_metadata.search_indexes.documents.course: your-course-index-name
+      course_discovery.apps.course_metadata.search_indexes.documents.course_run: your-course-run-index-name
+      course_discovery.apps.course_metadata.search_indexes.documents.person: your-person-index-name
+      course_discovery.apps.course_metadata.search_indexes.documents.program: your-program-index-name
+
+Re-indexing courses
+~~~~~~~~~~~~~~~~~~~
+
+::
+
+    tutor local run discovery ./manage.py refresh_course_metadata --partner_code=openedx
+    tutor local run discovery ./manage.py update_index --disable-change-limit
+
+Caching programs
+~~~~~~~~~~~~~~~~
+
+In order to cache programs in the LMS, you will need to manually create a catalog integration. Make sure you use staff user for the below command. If ``lms_catalog_service_user`` is not a staff user, then make it a staff user in your LMS User model. This step should be performed just once::
+
+    tutor local run lms ./manage.py lms create_catalog_integrations --enabled \
+        --internal_api_url="" \
+        --service_username=lms_catalog_service_user
+
+Then run the below command, this command will cause errors every time as it tries to cache programs from all sites that are added to your LMS sites model::
+
+    tutor local run lms ./manage.py lms cache_programs
+
+If you don't want the errors, then make use of an extra argumet to the command .i.e. ``--domain``. This argument will be equal to ``local.overhang.io`` if you are running tutor local and ``local.overhang.io:8000`` if you are running tutor dev::
+    tutor local run lms ./manage.py lms cache_programs --domain="local.overhang.io"
+    or
+    tutor dev run lms ./manage.py lms cache_programs --domain="local.overhang.io:8000"
+
+This last step should be performed every time you create new or make changes to existing programs.
+
+Install extra requirements
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+In order to install extra requirements, use DISCOVERY_EXTRA_PIP_REQUIREMENTS and re-build the docker image.::
+
+  tutor config save \
+    --set 'DISCOVERY_EXTRA_PIP_REQUIREMENTS=["git+https://github.com/myusername/myplugin"]'
+
+Then, build the image, pointing to your fork if necessary::
+
+  tutor images build discovery
+
+Debugging
+---------
+
+To debug the course discovery service, you are encouraged to mount the course-discovery repo from the host in the development container:
+
+    tutor dev start --mount /path/to/course-discovery/ discovery
+
+You can then access the development server at http://discovery.local.overhang.io:8381. Feel free to add breakpoints (``import pdb; pdb.set_trace()``) anywhere in your source code to debug your application.
+
+Once a local repository is mounted in the image, you will have to install nodejs dependencies and collect static assets::
+
+    tutor dev run discovery npm install --development
+    tutor dev run discovery make static.dev
+
+Troubleshooting
+---------------
+
+This Tutor plugin is maintained by Régis Behmo from `Overhang.IO <https://overhang.io>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
+
+
+`Max retries exceeded with url`
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+When running in production with HTTPS enabled, you may face this error during the `init` phase of `tutor local launch`:
+
+```
+requests.exceptions.ConnectionError: HTTPSConnectionPool(host='<LMS_HOST>', port=443): Max retries exceeded with url: /api/courses/v1/courses/?page=1&page_size=10&username=discovery
+```
+
+This error may be due to an incorrect DNS resolution of the LMS DNS record. With some cloud providers (for instance: [DigitalOcean](https://digitalocean.com/)) the `/etc/hosts` file on the host automatically contains the following entry::
+
+    127.0.1.1 <LMS HOST>
+
+This entry may be present if you named your server with the LMS hostname.
+
+License
+-------
+
+This work is licensed under the terms of the `GNU Affero General Public License (AGPL) <https://github.com/overhangio/tutor/blob/master/LICENSE.txt>`_.
```

### Comparing `tutor-discovery-15.0.0/tutor_discovery.egg-info/SOURCES.txt` & `tutor-discovery-16.0.0/tutor_discovery.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+LICENSE.txt
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.py
 tutor_discovery.egg-info/PKG-INFO
 tutor_discovery.egg-info/SOURCES.txt
 tutor_discovery.egg-info/dependency_links.txt
 tutor_discovery.egg-info/entry_points.txt
 tutor_discovery.egg-info/requires.txt
 tutor_discovery.egg-info/top_level.txt
```

### Comparing `tutor-discovery-15.0.0/tutordiscovery/patches/k8s-deployments` & `tutor-discovery-16.0.0/tutordiscovery/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-discovery-15.0.0/tutordiscovery/patches/k8s-jobs` & `tutor-discovery-16.0.0/tutordiscovery/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-discovery-15.0.0/tutordiscovery/plugin.py` & `tutor-discovery-16.0.0/tutordiscovery/plugin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+from __future__ import annotations
+
 from glob import glob
 import os
 import pkg_resources
+import typing as t
 
 from tutor import hooks as tutor_hooks
 
 from .__about__ import __version__
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 
@@ -24,14 +27,15 @@
         "MYSQL_DATABASE": "discovery",
         "MYSQL_USERNAME": "discovery",
         "OAUTH2_KEY": "discovery",
         "OAUTH2_KEY_DEV": "discovery-dev",
         "OAUTH2_KEY_SSO": "discovery-sso",
         "OAUTH2_KEY_SSO_DEV": "discovery-sso-dev",
         "CACHE_REDIS_DB": "{{ OPENEDX_CACHE_REDIS_DB }}",
+        "EXTRA_PIP_REQUIREMENTS": [],
     },
 }
 
 # Initialization tasks
 init_tasks = ("mysql", "lms", "discovery")
 for service in init_tasks:
     with open(
@@ -69,19 +73,34 @@
 tutor_hooks.Filters.IMAGES_PUSH.add_item(
     (
         "discovery",
         "{{ DISCOVERY_DOCKER_IMAGE }}",
     )
 )
 
+
+REPO_NAME = "course-discovery"
+APP_NAME = "discovery"
+
+
 # Automount /openedx/discovery folder from the container
 @tutor_hooks.Filters.COMPOSE_MOUNTS.add()
 def _mount_course_discovery(mounts, name):
-    if name == "course-discovery":
-        mounts.append(("discovery", "/openedx/discovery"))
+    if name == REPO_NAME:
+        mounts.append((APP_NAME, "/openedx/discovery"))
+    return mounts
+
+
+# Bind-mount repo at build-time, both for prod and dev images
+@tutor_hooks.Filters.IMAGES_BUILD_MOUNTS.add()
+def _mount_course_discovery_on_build(mounts: list[tuple[str, str]], host_path: str) -> list[tuple[str, str]]:
+    path_basename = os.path.basename(host_path)
+    if path_basename == REPO_NAME:
+        mounts.append((APP_NAME, f"{APP_NAME}-src"))
+        mounts.append((f"{APP_NAME}-dev", f"{APP_NAME}-src"))
     return mounts
 
 
 ####### Boilerplate code
 # Add the "templates" folder as a template root
 tutor_hooks.Filters.ENV_TEMPLATE_ROOTS.add_item(
     pkg_resources.resource_filename("tutordiscovery", "templates")
@@ -110,7 +129,16 @@
 )
 tutor_hooks.Filters.CONFIG_UNIQUE.add_items(
     [(f"DISCOVERY_{key}", value) for key, value in config.get("unique", {}).items()]
 )
 tutor_hooks.Filters.CONFIG_OVERRIDES.add_items(
     list(config.get("overrides", {}).items())
 )
+
+
+@tutor_hooks.Filters.APP_PUBLIC_HOSTS.add()
+def _print_discovery_public_hosts(hosts: list[str], context_name: t.Literal["local", "dev"]) -> list[str]:
+    if context_name == "dev":
+        hosts += ["{{ DISCOVERY_HOST }}:8381"]
+    else:
+        hosts += ["{{ DISCOVERY_HOST }}"]
+    return hosts
```

### Comparing `tutor-discovery-15.0.0/tutordiscovery/templates/discovery/apps/settings/partials/common.py` & `tutor-discovery-16.0.0/tutordiscovery/templates/discovery/apps/settings/partials/common.py`

 * *Files identical despite different names*

### Comparing `tutor-discovery-15.0.0/tutordiscovery/templates/discovery/apps/settings/tutor/development.py` & `tutor-discovery-16.0.0/tutordiscovery/templates/discovery/apps/settings/tutor/development.py`

 * *Files identical despite different names*

### Comparing `tutor-discovery-15.0.0/tutordiscovery/templates/discovery/apps/settings/tutor/production.py` & `tutor-discovery-16.0.0/tutordiscovery/templates/discovery/apps/settings/tutor/production.py`

 * *Files identical despite different names*

### Comparing `tutor-discovery-15.0.0/tutordiscovery/templates/discovery/tasks/discovery/init` & `tutor-discovery-16.0.0/tutordiscovery/templates/discovery/tasks/discovery/init`

 * *Files identical despite different names*

### Comparing `tutor-discovery-15.0.0/tutordiscovery/templates/discovery/tasks/lms/init` & `tutor-discovery-16.0.0/tutordiscovery/templates/discovery/tasks/lms/init`

 * *Files identical despite different names*

### Comparing `tutor-discovery-15.0.0/tutordiscovery/templates/discovery/tasks/mysql/init` & `tutor-discovery-16.0.0/tutordiscovery/templates/discovery/tasks/mysql/init`

 * *Files identical despite different names*

