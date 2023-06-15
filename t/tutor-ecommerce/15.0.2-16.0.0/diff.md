# Comparing `tmp/tutor-ecommerce-15.0.2.tar.gz` & `tmp/tutor-ecommerce-16.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tutor-ecommerce-15.0.2.tar", last modified: Thu Dec 22 16:01:39 2022, max compression
+gzip compressed data, was "tutor-ecommerce-16.0.0.tar", last modified: Thu Jun 15 00:58:45 2023, max compression
```

## Comparing `tutor-ecommerce-15.0.2.tar` & `tutor-ecommerce-16.0.0.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/
--rw-r--r--   0 ci        (1000) ci        (1000)    34523 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/LICENSE.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       88 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     8940 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     7884 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1775 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/tutor_ecommerce.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     8940 2022-12-22 16:01:38.000000 tutor-ecommerce-15.0.2/tutor_ecommerce.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     1830 2022-12-22 16:01:38.000000 tutor-ecommerce-15.0.2/tutor_ecommerce.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2022-12-22 16:01:38.000000 tutor-ecommerce-15.0.2/tutor_ecommerce.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       52 2022-12-22 16:01:38.000000 tutor-ecommerce-15.0.2/tutor_ecommerce.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       80 2022-12-22 16:01:38.000000 tutor-ecommerce-15.0.2/tutor_ecommerce.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       15 2022-12-22 16:01:38.000000 tutor-ecommerce-15.0.2/tutor_ecommerce.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/tutorecommerce/
--rw-r--r--   0 ci        (1000) ci        (1000)       24 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/tutorecommerce/patches/
--rw-r--r--   0 ci        (1000) ci        (1000)      139 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/patches/caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)     2051 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/patches/k8s-deployments
--rw-r--r--   0 ci        (1000) ci        (1000)      644 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/patches/k8s-jobs
--rw-r--r--   0 ci        (1000) ci        (1000)      180 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/patches/k8s-services
--rw-r--r--   0 ci        (1000) ci        (1000)      209 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/patches/kustomization-configmapgenerator
--rw-r--r--   0 ci        (1000) ci        (1000)       22 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/patches/local-docker-compose-caddy-aliases
--rw-r--r--   0 ci        (1000) ci        (1000)      394 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/patches/local-docker-compose-dev-services
--rw-r--r--   0 ci        (1000) ci        (1000)      303 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/patches/local-docker-compose-jobs-services
--rw-r--r--   0 ci        (1000) ci        (1000)      738 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/patches/local-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)      598 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/patches/openedx-lms-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      389 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/patches/openedx-lms-development-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      446 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/patches/openedx-lms-production-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     6051 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/apps/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      543 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/development.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)     3371 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/partials/common.py
--rw-r--r--   0 ci        (1000) ci        (1000)      496 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/production.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce-worker/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce-worker/settings/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce-worker/settings/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      888 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce-worker/settings/production.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/build/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/build/ecommerce/
--rw-r--r--   0 ci        (1000) ci        (1000)     2675 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/build/ecommerce/Dockerfile
--rw-r--r--   0 ci        (1000) ci        (1000)      211 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/build/ecommerce/assets.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/build/ecommerce/requirements/
--rw-r--r--   0 ci        (1000) ci        (1000)      316 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/build/ecommerce/requirements/private-sample.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/build/ecommerce-worker/
--rw-r--r--   0 ci        (1000) ci        (1000)      861 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/build/ecommerce-worker/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/tasks/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/tasks/ecommerce/
--rw-r--r--   0 ci        (1000) ci        (1000)     2420 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/tasks/ecommerce/init
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/tasks/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)     2266 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/tasks/lms/init
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-22 16:01:39.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/tasks/mysql/
--rw-r--r--   0 ci        (1000) ci        (1000)      821 2022-12-22 16:01:33.000000 tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/tasks/mysql/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:45.425697 tutor-ecommerce-16.0.0/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       88 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     9156 2023-06-15 00:58:45.425697 tutor-ecommerce-16.0.0/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     8079 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/pyproject.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-15 00:58:45.425697 tutor-ecommerce-16.0.0/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1852 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:45.415697 tutor-ecommerce-16.0.0/tutor_ecommerce.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     9156 2023-06-15 00:58:45.000000 tutor-ecommerce-16.0.0/tutor_ecommerce.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     1927 2023-06-15 00:58:45.000000 tutor-ecommerce-16.0.0/tutor_ecommerce.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-06-15 00:58:45.000000 tutor-ecommerce-16.0.0/tutor_ecommerce.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       52 2023-06-15 00:58:45.000000 tutor-ecommerce-16.0.0/tutor_ecommerce.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       93 2023-06-15 00:58:45.000000 tutor-ecommerce-16.0.0/tutor_ecommerce.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       15 2023-06-15 00:58:45.000000 tutor-ecommerce-16.0.0/tutor_ecommerce.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:45.415697 tutor-ecommerce-16.0.0/tutorecommerce/
+-rw-r--r--   0 ci        (1000) ci        (1000)      176 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:45.419030 tutor-ecommerce-16.0.0/tutorecommerce/patches/
+-rw-r--r--   0 ci        (1000) ci        (1000)      139 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/patches/caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)     2051 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/patches/k8s-deployments
+-rw-r--r--   0 ci        (1000) ci        (1000)      644 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/patches/k8s-jobs
+-rw-r--r--   0 ci        (1000) ci        (1000)      180 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/patches/k8s-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      209 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/patches/kustomization-configmapgenerator
+-rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/patches/local-docker-compose-caddy-aliases
+-rw-r--r--   0 ci        (1000) ci        (1000)      394 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/patches/local-docker-compose-dev-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      303 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      711 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/patches/local-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      598 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/patches/openedx-lms-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      389 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/patches/openedx-lms-development-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      446 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/patches/openedx-lms-production-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)     8099 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:45.409030 tutor-ecommerce-16.0.0/tutorecommerce/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:45.412363 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:45.412363 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/apps/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:45.412363 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/apps/ecommerce/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:45.422364 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      543 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/development.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:45.422364 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)     3682 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/partials/common.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       52 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/paymentprocessors.json
+-rw-r--r--   0 ci        (1000) ci        (1000)      496 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/production.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:45.409030 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/apps/ecommerce-worker/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:45.419030 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/apps/ecommerce-worker/settings/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/apps/ecommerce-worker/settings/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      888 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/apps/ecommerce-worker/settings/production.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:45.412363 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/build/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:45.422364 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/build/ecommerce/
+-rw-r--r--   0 ci        (1000) ci        (1000)     3733 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/build/ecommerce/Dockerfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      211 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/build/ecommerce/assets.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:45.422364 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/build/ecommerce/requirements/
+-rw-r--r--   0 ci        (1000) ci        (1000)      316 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/build/ecommerce/requirements/private-sample.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:45.422364 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/build/ecommerce-worker/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1505 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/build/ecommerce-worker/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:45.412363 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/tasks/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:45.422364 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/tasks/ecommerce/
+-rw-r--r--   0 ci        (1000) ci        (1000)     2420 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/tasks/ecommerce/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:45.422364 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/tasks/lms/
+-rw-r--r--   0 ci        (1000) ci        (1000)     2266 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/tasks/lms/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:58:45.422364 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/tasks/mysql/
+-rw-r--r--   0 ci        (1000) ci        (1000)      821 2023-06-15 00:58:38.000000 tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/tasks/mysql/init
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tutor-ecommerce-15.0.2/LICENSE.txt` & `tutor-ecommerce-16.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-15.0.2/PKG-INFO` & `tutor-ecommerce-16.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-ecommerce
-Version: 15.0.2
+Version: 16.0.0
 Summary: A Tutor plugin for Open edX E-Commerce
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: Overhang.IO
 Maintainer-email: regis@overhang.io
 License: AGPLv3
@@ -13,19 +13,20 @@
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-ecommerce/issues
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
+Provides-Extra: dev
 License-File: LICENSE.txt
 
 E-Commerce plugin for `Tutor <https://docs.tutor.overhang.io>`_
 ===============================================================
 
 This is a plugin for `Tutor <https://docs.tutor.overhang.io>`_ that integrates the `E-Commerce <https://github.com/edx/ecommerce/>`__ application in an Open edX platform.
 
@@ -34,15 +35,15 @@
 
 This plugin requires tutor>=12.0.0, the `Discovery plugin <https://github.com/overhangio/tutor-discovery>`__ and the `MFE plugin <https://github.com/overhangio/tutor-mfe>`__. If you have installed Tutor by downloading the pre-compiled binary, then both plugins should be automatically installed. You can confirm by running::
 
     tutor plugins list
 
 But if you have installed tutor from source, then you also need to install the plugin from source::
 
-    pip install tutor-ecommerce
+    tutor plugins install ecommerce
 
 Then, in any case you need to enable the plugins::
 
     tutor plugins enable discovery ecommerce mfe
 
 Services will have to be re-configured and restarted, so you are probably better off just running launch again::
 
@@ -169,11 +170,16 @@
     tutor dev start ecommerce
 
 Troubleshooting
 ---------------
 
 This Tutor plugin is maintained by Régis Behmo from `Overhang.IO <https://overhang.io>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
 
+Contributing
+------------
+
+Pull requests are welcome! Please read the `"contributing" section from the Tutor documentation <https://docs.tutor.overhang.io/tutor.html#contributing>`__.
+
 License
 -------
 
-This work is licensed under the terms of the `GNU Affero General Public License (AGPL) <https://github.com/overhangio/ecommerce/blob/master/LICENSE.txt>`_.
+This work is licensed under the terms of the `GNU Affero General Public License (AGPL) <https://github.com/overhangio/tutor-ecommerce/blob/master/LICENSE.txt>`_.
```

### Comparing `tutor-ecommerce-15.0.2/README.rst` & `tutor-ecommerce-16.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 This plugin requires tutor>=12.0.0, the `Discovery plugin <https://github.com/overhangio/tutor-discovery>`__ and the `MFE plugin <https://github.com/overhangio/tutor-mfe>`__. If you have installed Tutor by downloading the pre-compiled binary, then both plugins should be automatically installed. You can confirm by running::
 
     tutor plugins list
 
 But if you have installed tutor from source, then you also need to install the plugin from source::
 
-    pip install tutor-ecommerce
+    tutor plugins install ecommerce
 
 Then, in any case you need to enable the plugins::
 
     tutor plugins enable discovery ecommerce mfe
 
 Services will have to be re-configured and restarted, so you are probably better off just running launch again::
 
@@ -143,11 +143,16 @@
     tutor dev start ecommerce
 
 Troubleshooting
 ---------------
 
 This Tutor plugin is maintained by Régis Behmo from `Overhang.IO <https://overhang.io>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
 
+Contributing
+------------
+
+Pull requests are welcome! Please read the `"contributing" section from the Tutor documentation <https://docs.tutor.overhang.io/tutor.html#contributing>`__.
+
 License
 -------
 
-This work is licensed under the terms of the `GNU Affero General Public License (AGPL) <https://github.com/overhangio/ecommerce/blob/master/LICENSE.txt>`_.
+This work is licensed under the terms of the `GNU Affero General Public License (AGPL) <https://github.com/overhangio/tutor-ecommerce/blob/master/LICENSE.txt>`_.
```

### Comparing `tutor-ecommerce-15.0.2/setup.py` & `tutor-ecommerce-16.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with io.open(os.path.join(here, "README.rst"), "rt", encoding="utf8") as f:
     readme = f.read()
 
 about = {}
-with io.open(os.path.join(here, "tutorecommerce", "__about__.py"), "rt", encoding="utf-8") as f:
+with io.open(
+    os.path.join(here, "tutorecommerce", "__about__.py"), "rt", encoding="utf-8"
+) as f:
     exec(f.read(), about)
 
 setup(
     name="tutor-ecommerce",
     version=about["__version__"],
     url="https://docs.tutor.overhang.io/",
     project_urls={
@@ -26,22 +28,27 @@
     author_email="contact@overhang.io",
     maintainer="Overhang.IO",
     maintainer_email="regis@overhang.io",
     description="A Tutor plugin for Open edX E-Commerce",
     long_description=readme,
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
-    python_requires=">=3.7",
-    install_requires=["tutor>=15.0.0,<16.0.0", "tutor-discovery>=15.0.0,<16.0.0", "tutor-mfe>=15.0.0,<16.0.0"],
+    python_requires=">=3.8",
+    install_requires=[
+        "tutor>=16.0.0,<17.0.0",
+        "tutor-discovery>=16.0.0,<17.0.0",
+        "tutor-mfe>=16.0.0,<17.0.0",
+    ],
+    extras_require={"dev": ["scriv"]},
     entry_points={"tutor.plugin.v1": ["ecommerce = tutorecommerce.plugin"]},
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

### Comparing `tutor-ecommerce-15.0.2/tutor_ecommerce.egg-info/PKG-INFO` & `tutor-ecommerce-16.0.0/tutor_ecommerce.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-ecommerce
-Version: 15.0.2
+Version: 16.0.0
 Summary: A Tutor plugin for Open edX E-Commerce
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: Overhang.IO
 Maintainer-email: regis@overhang.io
 License: AGPLv3
@@ -13,19 +13,20 @@
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-ecommerce/issues
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
+Provides-Extra: dev
 License-File: LICENSE.txt
 
 E-Commerce plugin for `Tutor <https://docs.tutor.overhang.io>`_
 ===============================================================
 
 This is a plugin for `Tutor <https://docs.tutor.overhang.io>`_ that integrates the `E-Commerce <https://github.com/edx/ecommerce/>`__ application in an Open edX platform.
 
@@ -34,15 +35,15 @@
 
 This plugin requires tutor>=12.0.0, the `Discovery plugin <https://github.com/overhangio/tutor-discovery>`__ and the `MFE plugin <https://github.com/overhangio/tutor-mfe>`__. If you have installed Tutor by downloading the pre-compiled binary, then both plugins should be automatically installed. You can confirm by running::
 
     tutor plugins list
 
 But if you have installed tutor from source, then you also need to install the plugin from source::
 
-    pip install tutor-ecommerce
+    tutor plugins install ecommerce
 
 Then, in any case you need to enable the plugins::
 
     tutor plugins enable discovery ecommerce mfe
 
 Services will have to be re-configured and restarted, so you are probably better off just running launch again::
 
@@ -169,11 +170,16 @@
     tutor dev start ecommerce
 
 Troubleshooting
 ---------------
 
 This Tutor plugin is maintained by Régis Behmo from `Overhang.IO <https://overhang.io>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
 
+Contributing
+------------
+
+Pull requests are welcome! Please read the `"contributing" section from the Tutor documentation <https://docs.tutor.overhang.io/tutor.html#contributing>`__.
+
 License
 -------
 
-This work is licensed under the terms of the `GNU Affero General Public License (AGPL) <https://github.com/overhangio/ecommerce/blob/master/LICENSE.txt>`_.
+This work is licensed under the terms of the `GNU Affero General Public License (AGPL) <https://github.com/overhangio/tutor-ecommerce/blob/master/LICENSE.txt>`_.
```

### Comparing `tutor-ecommerce-15.0.2/tutor_ecommerce.egg-info/SOURCES.txt` & `tutor-ecommerce-16.0.0/tutor_ecommerce.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.py
 tutor_ecommerce.egg-info/PKG-INFO
 tutor_ecommerce.egg-info/SOURCES.txt
 tutor_ecommerce.egg-info/dependency_links.txt
 tutor_ecommerce.egg-info/entry_points.txt
 tutor_ecommerce.egg-info/requires.txt
 tutor_ecommerce.egg-info/top_level.txt
@@ -23,14 +24,15 @@
 tutorecommerce/patches/openedx-lms-common-settings
 tutorecommerce/patches/openedx-lms-development-settings
 tutorecommerce/patches/openedx-lms-production-settings
 tutorecommerce/templates/ecommerce/apps/ecommerce-worker/settings/__init__.py
 tutorecommerce/templates/ecommerce/apps/ecommerce-worker/settings/production.py
 tutorecommerce/templates/ecommerce/apps/ecommerce/settings/__init__.py
 tutorecommerce/templates/ecommerce/apps/ecommerce/settings/development.py
+tutorecommerce/templates/ecommerce/apps/ecommerce/settings/paymentprocessors.json
 tutorecommerce/templates/ecommerce/apps/ecommerce/settings/production.py
 tutorecommerce/templates/ecommerce/apps/ecommerce/settings/partials/common.py
 tutorecommerce/templates/ecommerce/build/ecommerce/Dockerfile
 tutorecommerce/templates/ecommerce/build/ecommerce/assets.py
 tutorecommerce/templates/ecommerce/build/ecommerce-worker/Dockerfile
 tutorecommerce/templates/ecommerce/build/ecommerce/requirements/private-sample.txt
 tutorecommerce/templates/ecommerce/tasks/ecommerce/init
```

### Comparing `tutor-ecommerce-15.0.2/tutorecommerce/patches/k8s-deployments` & `tutor-ecommerce-16.0.0/tutorecommerce/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-15.0.2/tutorecommerce/patches/k8s-jobs` & `tutor-ecommerce-16.0.0/tutorecommerce/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-15.0.2/tutorecommerce/patches/local-docker-compose-services` & `tutor-ecommerce-16.0.0/tutorecommerce/patches/local-docker-compose-services`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,16 @@
   environment:
     DJANGO_SETTINGS_MODULE: ecommerce.settings.tutor.production
   restart: unless-stopped
   volumes:
     - ../plugins/ecommerce/apps/ecommerce/settings:/openedx/ecommerce/ecommerce/settings/tutor:ro
   depends_on:
     - discovery
+    - lms
     {% if RUN_MYSQL %}- mysql{% endif %}
-    {% if RUN_LMS %}- lms{% endif %}
 
 ecommerce-worker:
     image: {{ ECOMMERCE_WORKER_DOCKER_IMAGE }}
     environment:
       WORKER_CONFIGURATION_MODULE: ecommerce_worker.configuration.tutor.production
     restart: unless-stopped
     volumes:
```

### Comparing `tutor-ecommerce-15.0.2/tutorecommerce/patches/openedx-lms-common-settings` & `tutor-ecommerce-16.0.0/tutorecommerce/patches/openedx-lms-common-settings`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/development.py` & `tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/development.py`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/partials/common.py` & `tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/partials/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import os
 
 SECRET_KEY = "{{ ECOMMERCE_SECRET_KEY }}"
 ALLOWED_HOSTS = [
     "{{ ECOMMERCE_HOST }}",
     "ecommerce",
 ]
 PLATFORM_NAME = "{{ PLATFORM_NAME }}"
@@ -73,22 +74,35 @@
 ENTERPRISE_API_URL = urljoin(ENTERPRISE_SERVICE_URL, 'api/v1/')
 
 # Get rid of local logger
 LOGGING["handlers"].pop("local")
 for logger in LOGGING["loggers"].values():
     logger["handlers"].remove("local")
 
-common_payment_processor_config = json.loads("""{{ ECOMMERCE_PAYMENT_PROCESSORS|tojson(indent=4) }}""")
+# Load payment processors
+with open(
+    os.path.join(os.path.dirname(__file__), "paymentprocessors.json"),
+    encoding="utf8"
+) as payment_processors_file:
+    common_payment_processor_config = json.load(payment_processors_file)
+
 # Fix cybersource-rest configuration
 if "cybersource" in common_payment_processor_config and "cybersource-rest" not in common_payment_processor_config:
     common_payment_processor_config["cybersource-rest"] = common_payment_processor_config["cybersource"]
 PAYMENT_PROCESSOR_CONFIG = {
     "openedx": common_payment_processor_config,
     "dev": common_payment_processor_config,
 }
+# Dummy config is required to bypass a KeyError
+PAYMENT_PROCESSOR_CONFIG["edx"] = {
+    "stripe": {
+        "secret_key": "",
+        "webhook_endpoint_secret": "",
+    }
+}
 PAYMENT_PROCESSORS = list(PAYMENT_PROCESSORS) + {{ ECOMMERCE_EXTRA_PAYMENT_PROCESSOR_CLASSES }}
 
 {% for payment_processor, urls_module in ECOMMERCE_EXTRA_PAYMENT_PROCESSOR_URLS.items() %}
 EXTRA_PAYMENT_PROCESSOR_URLS["{{ payment_processor }}"] = "{{ urls_module }}"
 {% endfor %}
 
 {{ patch("ecommerce-settings-common") }}
```

### Comparing `tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce-worker/settings/production.py` & `tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/apps/ecommerce-worker/settings/production.py`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/tasks/ecommerce/init` & `tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/tasks/ecommerce/init`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/tasks/lms/init` & `tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/tasks/lms/init`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-15.0.2/tutorecommerce/templates/ecommerce/tasks/mysql/init` & `tutor-ecommerce-16.0.0/tutorecommerce/templates/ecommerce/tasks/mysql/init`

 * *Files identical despite different names*

