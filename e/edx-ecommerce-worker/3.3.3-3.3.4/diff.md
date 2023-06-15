# Comparing `tmp/edx-ecommerce-worker-3.3.3.tar.gz` & `tmp/edx-ecommerce-worker-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-ecommerce-worker-3.3.3.tar", last modified: Fri May 12 06:13:42 2023, max compression
+gzip compressed data, was "edx-ecommerce-worker-3.3.4.tar", last modified: Thu Jun 15 15:38:21 2023, max compression
```

## Comparing `edx-ecommerce-worker-3.3.3.tar` & `edx-ecommerce-worker-3.3.4.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.619126 edx-ecommerce-worker-3.3.3/
--rw-r--r--   0 runner    (1001) docker     (122)    35116 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      197 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5629 2023-05-12 06:13:42.619126 edx-ecommerce-worker-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4325 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.607126 edx-ecommerce-worker-3.3.3/ecommerce_worker/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1706 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/celery_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.607126 edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/
--rw-r--r--   0 runner    (1001) docker     (122)      512 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4154 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      932 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/devstack.py
--rw-r--r--   0 runner    (1001) docker     (122)      744 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     3195 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/production.py
--rw-r--r--   0 runner    (1001) docker     (122)      627 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.611126 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.611126 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.611126 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20998 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    11061 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.611126 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17952 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (122)    16988 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (122)     6718 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.615126 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      689 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4305 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.615126 edx-ecommerce-worker-3.3.3/ecommerce_worker/fulfillment/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/fulfillment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.615126 edx-ecommerce-worker-3.3.3/ecommerce_worker/fulfillment/v1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/fulfillment/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2693 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/fulfillment/v1/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.615126 edx-ecommerce-worker-3.3.3/ecommerce_worker/fulfillment/v1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/fulfillment/v1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5752 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/fulfillment/v1/tests/test_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.615126 edx-ecommerce-worker-3.3.3/ecommerce_worker/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2928 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.615126 edx-ecommerce-worker-3.3.3/edx_ecommerce_worker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5629 2023-05-12 06:13:42.000000 edx-ecommerce-worker-3.3.3/edx_ecommerce_worker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1892 2023-05-12 06:13:42.000000 edx-ecommerce-worker-3.3.3/edx_ecommerce_worker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 06:13:42.000000 edx-ecommerce-worker-3.3.3/edx_ecommerce_worker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       54 2023-05-12 06:13:42.000000 edx-ecommerce-worker-3.3.3/edx_ecommerce_worker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-12 06:13:42.000000 edx-ecommerce-worker-3.3.3/edx_ecommerce_worker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.619126 edx-ecommerce-worker-3.3.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       74 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)     1633 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1573 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/requirements/common_constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      817 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      166 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/requirements/optional.txt
--rw-r--r--   0 runner    (1001) docker     (122)      334 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/requirements/pip.txt
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/requirements/pip_tools.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/requirements/production.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4691 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)      589 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/requirements/tox.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-12 06:13:42.619126 edx-ecommerce-worker-3.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:21.388467 edx-ecommerce-worker-3.3.4/
+-rw-r--r--   0 runner    (1001) docker     (122)    35116 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5629 2023-06-15 15:38:21.388467 edx-ecommerce-worker-3.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4325 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:21.380467 edx-ecommerce-worker-3.3.4/ecommerce_worker/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1706 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/celery_app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:21.380467 edx-ecommerce-worker-3.3.4/ecommerce_worker/configuration/
+-rw-r--r--   0 runner    (1001) docker     (122)      512 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4154 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/configuration/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      932 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/configuration/devstack.py
+-rw-r--r--   0 runner    (1001) docker     (122)      744 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/configuration/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3195 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/configuration/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/configuration/production.py
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/configuration/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:21.380467 edx-ecommerce-worker-3.3.4/ecommerce_worker/email/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/email/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:21.380467 edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:21.384467 edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/braze/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/braze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20998 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/braze/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/braze/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11061 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/braze/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:21.384467 edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/braze/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/braze/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17952 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/braze/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16988 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/braze/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6718 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:21.384467 edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      689 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4305 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:21.384467 edx-ecommerce-worker-3.3.4/ecommerce_worker/fulfillment/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/fulfillment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:21.384467 edx-ecommerce-worker-3.3.4/ecommerce_worker/fulfillment/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/fulfillment/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2693 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/fulfillment/v1/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:21.384467 edx-ecommerce-worker-3.3.4/ecommerce_worker/fulfillment/v1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/fulfillment/v1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5752 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/fulfillment/v1/tests/test_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:21.384467 edx-ecommerce-worker-3.3.4/ecommerce_worker/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2928 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/ecommerce_worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:21.384467 edx-ecommerce-worker-3.3.4/edx_ecommerce_worker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5629 2023-06-15 15:38:21.000000 edx-ecommerce-worker-3.3.4/edx_ecommerce_worker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1892 2023-06-15 15:38:21.000000 edx-ecommerce-worker-3.3.4/edx_ecommerce_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 15:38:21.000000 edx-ecommerce-worker-3.3.4/edx_ecommerce_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       54 2023-06-15 15:38:21.000000 edx-ecommerce-worker-3.3.4/edx_ecommerce_worker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-15 15:38:21.000000 edx-ecommerce-worker-3.3.4/edx_ecommerce_worker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 15:38:21.388467 edx-ecommerce-worker-3.3.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1633 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1573 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/requirements/common_constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      817 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/requirements/optional.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      334 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/requirements/pip.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/requirements/pip_tools.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/requirements/production.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4691 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      589 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/requirements/tox.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-15 15:38:21.388467 edx-ecommerce-worker-3.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-06-15 15:38:16.000000 edx-ecommerce-worker-3.3.4/setup.py
```

### Comparing `edx-ecommerce-worker-3.3.3/LICENSE.txt` & `edx-ecommerce-worker-3.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/PKG-INFO` & `edx-ecommerce-worker-3.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-ecommerce-worker
-Version: 3.3.3
+Version: 3.3.4
 Summary: Celery tasks supporting the operations of edX's ecommerce service
 Home-page: https://github.com/openedx/ecommerce-worker
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
 Description: DEPRECATION WARNING
         ====================
```

### Comparing `edx-ecommerce-worker-3.3.3/README.rst` & `edx-ecommerce-worker-3.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/cache.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/cache.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/__init__.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/base.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/configuration/base.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/devstack.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/configuration/devstack.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/local.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/configuration/local.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/logger.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/configuration/logger.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/production.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/configuration/production.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 logger_config = get_logger_config()
 dictConfig(logger_config)
 # END LOGGING
 
 
 filename = get_overrides_filename('ECOMMERCE_WORKER_CFG')
 with open(filename) as f:
-    config_from_yaml = yaml.load(f)
+    config_from_yaml = yaml.safe_load(f)
 
 # Override base configuration with values from disk.
 vars().update(config_from_yaml)
```

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/test.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/configuration/test.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/client.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/braze/client.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/exceptions.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/braze/exceptions.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/tasks.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/braze/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/tests/test_client.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/braze/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/tests/test_tasks.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/braze/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/tasks.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/tests/test_api.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/tests/test_utils.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/utils.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/email/v1/utils.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/fulfillment/v1/tasks.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/fulfillment/v1/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/fulfillment/v1/tests/test_tasks.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/fulfillment/v1/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/tests/test_cache.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/tests/test_utils.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/ecommerce_worker/utils.py` & `edx-ecommerce-worker-3.3.4/ecommerce_worker/utils.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/edx_ecommerce_worker.egg-info/PKG-INFO` & `edx-ecommerce-worker-3.3.4/edx_ecommerce_worker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-ecommerce-worker
-Version: 3.3.3
+Version: 3.3.4
 Summary: Celery tasks supporting the operations of edX's ecommerce service
 Home-page: https://github.com/openedx/ecommerce-worker
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
 Description: DEPRECATION WARNING
         ====================
```

### Comparing `edx-ecommerce-worker-3.3.3/edx_ecommerce_worker.egg-info/SOURCES.txt` & `edx-ecommerce-worker-3.3.4/edx_ecommerce_worker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/requirements/base.txt` & `edx-ecommerce-worker-3.3.4/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/requirements/common_constraints.txt` & `edx-ecommerce-worker-3.3.4/requirements/common_constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/requirements/constraints.txt` & `edx-ecommerce-worker-3.3.4/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/requirements/production.txt` & `edx-ecommerce-worker-3.3.4/requirements/production.txt`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/requirements/test.txt` & `edx-ecommerce-worker-3.3.4/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/requirements/tox.txt` & `edx-ecommerce-worker-3.3.4/requirements/tox.txt`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.3/setup.py` & `edx-ecommerce-worker-3.3.4/setup.py`

 * *Files identical despite different names*

