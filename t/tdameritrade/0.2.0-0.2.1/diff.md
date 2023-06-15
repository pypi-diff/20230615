# Comparing `tmp/tdameritrade-0.2.0.tar.gz` & `tmp/tdameritrade-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdameritrade-0.2.0.tar", last modified: Tue Jun 13 15:26:32 2023, max compression
+gzip compressed data, was "tdameritrade-0.2.1.tar", last modified: Thu Jun 15 18:42:04 2023, max compression
```

## Comparing `tdameritrade-0.2.0.tar` & `tdameritrade-0.2.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:26:32.858173 tdameritrade-0.2.0/
--rw-r--r--   0 timkpaine   (501) staff       (20)      292 2023-06-13 15:26:29.000000 tdameritrade-0.2.0/.bumpversion.cfg
--rw-r--r--   0 timkpaine   (501) staff       (20)    11357 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/LICENSE
--rw-r--r--   0 timkpaine   (501) staff       (20)      344 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/MANIFEST.in
--rw-r--r--   0 timkpaine   (501) staff       (20)     1305 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/Makefile
--rw-r--r--   0 timkpaine   (501) staff       (20)     2699 2023-06-13 15:26:32.858237 tdameritrade-0.2.0/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)     2137 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/README.md
--rw-r--r--   0 timkpaine   (501) staff       (20)      106 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/pyproject.toml
--rw-r--r--   0 timkpaine   (501) staff       (20)      236 2023-06-13 15:26:32.858467 tdameritrade-0.2.0/setup.cfg
--rw-r--r--   0 timkpaine   (501) staff       (20)     1550 2023-06-13 15:26:29.000000 tdameritrade-0.2.0/setup.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:26:32.854059 tdameritrade-0.2.0/tdameritrade/
--rw-r--r--   0 timkpaine   (501) staff       (20)       66 2023-06-13 15:26:29.000000 tdameritrade-0.2.0/tdameritrade/__init__.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:26:32.855093 tdameritrade-0.2.0/tdameritrade/auth/
--rw-r--r--   0 timkpaine   (501) staff       (20)     4111 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/auth/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)       62 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/auth/__main__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    26183 2023-06-13 15:15:32.000000 tdameritrade-0.2.0/tdameritrade/client.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2351 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/enums.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1347 2023-06-13 15:15:32.000000 tdameritrade-0.2.0/tdameritrade/exceptions.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2671 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/order.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:26:32.855674 tdameritrade-0.2.0/tdameritrade/orders/
--rw-r--r--   0 timkpaine   (501) staff       (20)      457 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5737 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/constants.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1363 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/leg_builder.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:26:32.856628 tdameritrade-0.2.0/tdameritrade/orders/models/
--rw-r--r--   0 timkpaine   (501) staff       (20)      128 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/models/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      698 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/models/activities.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2155 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/models/base.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2047 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/models/instruments.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      458 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/models/json_encoder.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2936 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/models/leg.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2146 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/models/orders.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5031 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/order_builder.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1647 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/session.py
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/streaming.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:26:32.857323 tdameritrade-0.2.0/tdameritrade/tests/
--rw-r--r--   0 timkpaine   (501) staff       (20)      315 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/tests/JSONS.py
--rw-r--r--   0 timkpaine   (501) staff       (20)       42 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/tests/test_all.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5783 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/tests/test_client.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      430 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/tests/test_exceptions.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1810 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/tests/test_session.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:26:32.857470 tdameritrade-0.2.0/tdameritrade/tests/unit/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/tests/unit/__init__.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:26:32.857773 tdameritrade-0.2.0/tdameritrade/tests/unit/orders/
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:26:32.858031 tdameritrade-0.2.0/tdameritrade/tests/unit/orders/models/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/tests/unit/orders/models/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      178 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/tests/unit/orders/models/test_base.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      158 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/tests/unit/orders/test_constants.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3284 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/tests/unit/orders/test_order_builder.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6569 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/urls.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:26:32.854852 tdameritrade-0.2.0/tdameritrade.egg-info/
--rw-r--r--   0 timkpaine   (501) staff       (20)     2699 2023-06-13 15:26:32.000000 tdameritrade-0.2.0/tdameritrade.egg-info/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)     1405 2023-06-13 15:26:32.000000 tdameritrade-0.2.0/tdameritrade.egg-info/SOURCES.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        1 2023-06-13 15:26:32.000000 tdameritrade-0.2.0/tdameritrade.egg-info/dependency_links.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       61 2023-06-13 15:26:32.000000 tdameritrade-0.2.0/tdameritrade.egg-info/entry_points.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        1 2023-06-13 15:26:32.000000 tdameritrade-0.2.0/tdameritrade.egg-info/not-zip-safe
--rw-r--r--   0 timkpaine   (501) staff       (20)      335 2023-06-13 15:26:32.000000 tdameritrade-0.2.0/tdameritrade.egg-info/requires.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       13 2023-06-13 15:26:32.000000 tdameritrade-0.2.0/tdameritrade.egg-info/top_level.txt
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-15 18:42:04.923412 tdameritrade-0.2.1/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      292 2023-06-15 18:41:59.000000 tdameritrade-0.2.1/.bumpversion.cfg
+-rw-r--r--   0 timkpaine   (501) staff       (20)    11357 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/LICENSE
+-rw-r--r--   0 timkpaine   (501) staff       (20)      344 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/MANIFEST.in
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1305 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/Makefile
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2720 2023-06-15 18:42:04.923521 tdameritrade-0.2.1/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2137 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/README.md
+-rw-r--r--   0 timkpaine   (501) staff       (20)      106 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/pyproject.toml
+-rw-r--r--   0 timkpaine   (501) staff       (20)      236 2023-06-15 18:42:04.923827 tdameritrade-0.2.1/setup.cfg
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1612 2023-06-15 18:41:59.000000 tdameritrade-0.2.1/setup.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-15 18:42:04.918357 tdameritrade-0.2.1/tdameritrade/
+-rw-r--r--   0 timkpaine   (501) staff       (20)       66 2023-06-15 18:41:59.000000 tdameritrade-0.2.1/tdameritrade/__init__.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-15 18:42:04.919860 tdameritrade-0.2.1/tdameritrade/auth/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4000 2023-06-15 18:32:02.000000 tdameritrade-0.2.1/tdameritrade/auth/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)       62 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/auth/__main__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    26183 2023-06-13 15:15:32.000000 tdameritrade-0.2.1/tdameritrade/client.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2351 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/enums.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1347 2023-06-13 15:15:32.000000 tdameritrade-0.2.1/tdameritrade/exceptions.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2671 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/order.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-15 18:42:04.920569 tdameritrade-0.2.1/tdameritrade/orders/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      457 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/orders/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5737 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/orders/constants.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1363 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/orders/leg_builder.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-15 18:42:04.921695 tdameritrade-0.2.1/tdameritrade/orders/models/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      128 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/orders/models/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      698 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/orders/models/activities.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2155 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/orders/models/base.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2047 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/orders/models/instruments.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      458 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/orders/models/json_encoder.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2936 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/orders/models/leg.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2146 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/orders/models/orders.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5031 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/orders/order_builder.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1647 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/session.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/streaming.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-15 18:42:04.922528 tdameritrade-0.2.1/tdameritrade/tests/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      315 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/tests/JSONS.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)       42 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/tests/test_all.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5783 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/tests/test_client.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      430 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/tests/test_exceptions.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1810 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/tests/test_session.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-15 18:42:04.922732 tdameritrade-0.2.1/tdameritrade/tests/unit/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/tests/unit/__init__.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-15 18:42:04.922997 tdameritrade-0.2.1/tdameritrade/tests/unit/orders/
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-15 18:42:04.923254 tdameritrade-0.2.1/tdameritrade/tests/unit/orders/models/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/tests/unit/orders/models/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      178 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/tests/unit/orders/models/test_base.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      158 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/tests/unit/orders/test_constants.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3284 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/tests/unit/orders/test_order_builder.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     6569 2023-06-13 15:00:28.000000 tdameritrade-0.2.1/tdameritrade/urls.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-15 18:42:04.919464 tdameritrade-0.2.1/tdameritrade.egg-info/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2720 2023-06-15 18:42:04.000000 tdameritrade-0.2.1/tdameritrade.egg-info/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1405 2023-06-15 18:42:04.000000 tdameritrade-0.2.1/tdameritrade.egg-info/SOURCES.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2023-06-15 18:42:04.000000 tdameritrade-0.2.1/tdameritrade.egg-info/dependency_links.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       61 2023-06-15 18:42:04.000000 tdameritrade-0.2.1/tdameritrade.egg-info/entry_points.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2023-06-13 15:26:32.000000 tdameritrade-0.2.1/tdameritrade.egg-info/not-zip-safe
+-rw-r--r--   0 timkpaine   (501) staff       (20)      261 2023-06-15 18:42:04.000000 tdameritrade-0.2.1/tdameritrade.egg-info/requires.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       13 2023-06-15 18:42:04.000000 tdameritrade-0.2.1/tdameritrade.egg-info/top_level.txt
```

### Comparing `tdameritrade-0.2.0/LICENSE` & `tdameritrade-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.2.0/Makefile` & `tdameritrade-0.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.2.0/PKG-INFO` & `tdameritrade-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: tdameritrade
-Version: 0.2.0
+Version: 0.2.1
 Summary: APIs for TD Ameritrade
 Home-page: https://github.com/timkpaine/tdameritrade
 Author: Tim Paine
 Author-email: t.paine154@gmail.com
 License: Apache 2.0
 Keywords: finance data
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
+Provides-Extra: auth
 Provides-Extra: dev
 License-File: LICENSE
 
 # tdameritrade
 Python interface to TD Ameritrade Api
 
 [![Build Status](https://github.com/timkpaine/tdameritrade/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/timkpaine/tdameritrade/actions?query=workflow%3A%22Build+Status%22)
```

### Comparing `tdameritrade-0.2.0/README.md` & `tdameritrade-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.2.0/setup.py` & `tdameritrade-0.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,37 +7,41 @@
 here = os.path.abspath(os.path.dirname(__file__))
 name = "tdameritrade"
 
 with open(pjoin(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read().replace("\r\n", "\n")
 
 requires = [
-    "ipython>=7.0.1",
     "pandas>=0.22.0",
-    "pillow>=5.3.0",
     "requests>=2.23.0",
+]
+
+requires_auth = [
     "selenium>=3.141.0",
-    "ujson>=1.35",
 ]
 
-requires_dev = [
-    "black>=23",
-    "bump2version>=1.0.0",
-    "flake8>=3.7.8",
-    "flake8-black>=0.2.1",
-    "mock",
-    "pytest>=4.3.0",
-    "pytest-cov>=2.6.1",
-    "Sphinx>=1.8.4",
-    "sphinx-markdown-builder>=0.5.2",
-] + requires
+requires_dev = (
+    [
+        "black>=23",
+        "bump2version>=1.0.0",
+        "flake8>=3.7.8",
+        "flake8-black>=0.2.1",
+        "mock",
+        "pytest>=4.3.0",
+        "pytest-cov>=2.6.1",
+        "Sphinx>=1.8.4",
+        "sphinx-markdown-builder>=0.5.2",
+    ]
+    + requires
+    + requires_auth
+)
 
 setup(
     name=name,
-    version="0.2.0",
+    version="0.2.1",
     description="APIs for TD Ameritrade",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/timkpaine/{name}".format(name=name),
     author="Tim Paine",
     author_email="t.paine154@gmail.com",
     license="Apache 2.0",
@@ -50,10 +54,11 @@
     ],
     keywords="finance data",
     zip_safe=False,
     packages=find_packages(exclude=[]),
     entry_points={"console_scripts": ["tdameritrade-auth = tdameritrade.auth:main"]},
     install_requires=requires,
     extras_require={
+        "auth": requires_auth,
         "dev": requires_dev,
     },
 )
```

### Comparing `tdameritrade-0.2.0/tdameritrade/auth/__init__.py` & `tdameritrade-0.2.1/tdameritrade/auth/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,16 +49,15 @@
                 "C:/Program Files (x86)/Google/Chrome/Application/chrome.exe"
             )
         elif os.path.exists("C:/Program Files/Google/Chrome/Application/chrome.exe"):
             options.binary_location = (
                 "C:/Program Files/Google/Chrome/Application/chrome.exe"
             )
 
-    chrome_driver_binary = which("chromedriver") or "/usr/local/bin/chromedriver"
-    driver = webdriver.Chrome(chrome_driver_binary, chrome_options=options)
+    driver = webdriver.Chrome(options=options)
 
     driver.get(url)
 
     # Set tdauser and tdapass from environemnt if TDAUSER and TDAPASS environment variables were defined
     tdauser = tdauser or os.environ.get("TDAUSER", "")
     tdapass = tdapass or os.environ.get("TDAPASS", "")
```

### Comparing `tdameritrade-0.2.0/tdameritrade/client.py` & `tdameritrade-0.2.1/tdameritrade/client.py`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.2.0/tdameritrade/enums.py` & `tdameritrade-0.2.1/tdameritrade/enums.py`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.2.0/tdameritrade/exceptions.py` & `tdameritrade-0.2.1/tdameritrade/exceptions.py`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.2.0/tdameritrade/order.py` & `tdameritrade-0.2.1/tdameritrade/order.py`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.2.0/tdameritrade/orders/constants.py` & `tdameritrade-0.2.1/tdameritrade/orders/constants.py`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.2.0/tdameritrade/orders/leg_builder.py` & `tdameritrade-0.2.1/tdameritrade/orders/leg_builder.py`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.2.0/tdameritrade/orders/models/activities.py` & `tdameritrade-0.2.1/tdameritrade/orders/models/activities.py`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.2.0/tdameritrade/orders/models/base.py` & `tdameritrade-0.2.1/tdameritrade/orders/models/base.py`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.2.0/tdameritrade/orders/models/instruments.py` & `tdameritrade-0.2.1/tdameritrade/orders/models/instruments.py`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.2.0/tdameritrade/orders/models/leg.py` & `tdameritrade-0.2.1/tdameritrade/orders/models/leg.py`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.2.0/tdameritrade/orders/models/orders.py` & `tdameritrade-0.2.1/tdameritrade/orders/models/orders.py`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.2.0/tdameritrade/orders/order_builder.py` & `tdameritrade-0.2.1/tdameritrade/orders/order_builder.py`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.2.0/tdameritrade/session.py` & `tdameritrade-0.2.1/tdameritrade/session.py`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.2.0/tdameritrade/tests/test_client.py` & `tdameritrade-0.2.1/tdameritrade/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.2.0/tdameritrade/tests/test_session.py` & `tdameritrade-0.2.1/tdameritrade/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.2.0/tdameritrade/tests/unit/orders/test_order_builder.py` & `tdameritrade-0.2.1/tdameritrade/tests/unit/orders/test_order_builder.py`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.2.0/tdameritrade/urls.py` & `tdameritrade-0.2.1/tdameritrade/urls.py`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.2.0/tdameritrade.egg-info/PKG-INFO` & `tdameritrade-0.2.1/tdameritrade.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: tdameritrade
-Version: 0.2.0
+Version: 0.2.1
 Summary: APIs for TD Ameritrade
 Home-page: https://github.com/timkpaine/tdameritrade
 Author: Tim Paine
 Author-email: t.paine154@gmail.com
 License: Apache 2.0
 Keywords: finance data
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
+Provides-Extra: auth
 Provides-Extra: dev
 License-File: LICENSE
 
 # tdameritrade
 Python interface to TD Ameritrade Api
 
 [![Build Status](https://github.com/timkpaine/tdameritrade/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/timkpaine/tdameritrade/actions?query=workflow%3A%22Build+Status%22)
```

### Comparing `tdameritrade-0.2.0/tdameritrade.egg-info/SOURCES.txt` & `tdameritrade-0.2.1/tdameritrade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

