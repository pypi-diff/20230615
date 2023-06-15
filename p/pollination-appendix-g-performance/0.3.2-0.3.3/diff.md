# Comparing `tmp/pollination-appendix-g-performance-0.3.2.tar.gz` & `tmp/pollination-appendix-g-performance-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-appendix-g-performance-0.3.2.tar", last modified: Mon Feb 27 21:06:03 2023, max compression
+gzip compressed data, was "dist/pollination-appendix-g-performance-0.3.3.tar", last modified: Thu Jun 15 17:37:16 2023, max compression
```

## Comparing `pollination-appendix-g-performance-0.3.2.tar` & `pollination-appendix-g-performance-0.3.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 21:06:03.000000 pollination-appendix-g-performance-0.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 21:06:03.000000 pollination-appendix-g-performance-0.3.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-02-27 21:05:11.000000 pollination-appendix-g-performance-0.3.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 21:06:03.000000 pollination-appendix-g-performance-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-02-27 21:05:11.000000 pollination-appendix-g-performance-0.3.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-02-27 21:05:11.000000 pollination-appendix-g-performance-0.3.2/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-27 21:05:11.000000 pollination-appendix-g-performance-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-27 21:05:11.000000 pollination-appendix-g-performance-0.3.2/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-02-27 21:05:11.000000 pollination-appendix-g-performance-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-02-27 21:06:03.000000 pollination-appendix-g-performance-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-02-27 21:05:11.000000 pollination-appendix-g-performance-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-27 21:05:11.000000 pollination-appendix-g-performance-0.3.2/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-27 21:05:11.000000 pollination-appendix-g-performance-0.3.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 21:06:03.000000 pollination-appendix-g-performance-0.3.2/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 21:06:03.000000 pollination-appendix-g-performance-0.3.2/pollination/appendix_g_performance/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-27 21:05:11.000000 pollination-appendix-g-performance-0.3.2/pollination/appendix_g_performance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13189 2023-02-27 21:05:11.000000 pollination-appendix-g-performance-0.3.2/pollination/appendix_g_performance/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 21:06:03.000000 pollination-appendix-g-performance-0.3.2/pollination_appendix_g_performance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-02-27 21:06:03.000000 pollination-appendix-g-performance-0.3.2/pollination_appendix_g_performance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-02-27 21:06:03.000000 pollination-appendix-g-performance-0.3.2/pollination_appendix_g_performance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 21:06:03.000000 pollination-appendix-g-performance-0.3.2/pollination_appendix_g_performance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 21:05:29.000000 pollination-appendix-g-performance-0.3.2/pollination_appendix_g_performance.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-27 21:06:03.000000 pollination-appendix-g-performance-0.3.2/pollination_appendix_g_performance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-27 21:06:03.000000 pollination-appendix-g-performance-0.3.2/pollination_appendix_g_performance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-27 21:05:11.000000 pollination-appendix-g-performance-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-27 21:06:03.000000 pollination-appendix-g-performance-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-02-27 21:05:11.000000 pollination-appendix-g-performance-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 21:06:03.000000 pollination-appendix-g-performance-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 21:05:11.000000 pollination-appendix-g-performance-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-02-27 21:05:11.000000 pollination-appendix-g-performance-0.3.2/tests/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:37:16.000000 pollination-appendix-g-performance-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:37:16.000000 pollination-appendix-g-performance-0.3.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-15 17:36:11.000000 pollination-appendix-g-performance-0.3.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:37:16.000000 pollination-appendix-g-performance-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-15 17:36:11.000000 pollination-appendix-g-performance-0.3.3/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-15 17:36:11.000000 pollination-appendix-g-performance-0.3.3/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-15 17:36:11.000000 pollination-appendix-g-performance-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-15 17:36:11.000000 pollination-appendix-g-performance-0.3.3/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-15 17:36:11.000000 pollination-appendix-g-performance-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-15 17:37:16.000000 pollination-appendix-g-performance-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-15 17:36:11.000000 pollination-appendix-g-performance-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-15 17:36:11.000000 pollination-appendix-g-performance-0.3.3/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 17:36:11.000000 pollination-appendix-g-performance-0.3.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:37:16.000000 pollination-appendix-g-performance-0.3.3/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:37:16.000000 pollination-appendix-g-performance-0.3.3/pollination/appendix_g_performance/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-15 17:36:11.000000 pollination-appendix-g-performance-0.3.3/pollination/appendix_g_performance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13189 2023-06-15 17:36:11.000000 pollination-appendix-g-performance-0.3.3/pollination/appendix_g_performance/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:37:16.000000 pollination-appendix-g-performance-0.3.3/pollination_appendix_g_performance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-15 17:37:16.000000 pollination-appendix-g-performance-0.3.3/pollination_appendix_g_performance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-15 17:37:16.000000 pollination-appendix-g-performance-0.3.3/pollination_appendix_g_performance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 17:37:16.000000 pollination-appendix-g-performance-0.3.3/pollination_appendix_g_performance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 17:36:37.000000 pollination-appendix-g-performance-0.3.3/pollination_appendix_g_performance.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 17:37:16.000000 pollination-appendix-g-performance-0.3.3/pollination_appendix_g_performance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 17:37:16.000000 pollination-appendix-g-performance-0.3.3/pollination_appendix_g_performance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 17:36:11.000000 pollination-appendix-g-performance-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-15 17:37:16.000000 pollination-appendix-g-performance-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-15 17:36:11.000000 pollination-appendix-g-performance-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:37:16.000000 pollination-appendix-g-performance-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:36:11.000000 pollination-appendix-g-performance-0.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-15 17:36:11.000000 pollination-appendix-g-performance-0.3.3/tests/validation_test.py
```

### Comparing `pollination-appendix-g-performance-0.3.2/.github/workflows/ci.yaml` & `pollination-appendix-g-performance-0.3.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-appendix-g-performance-0.3.2/.github/workflows/tests.yaml` & `pollination-appendix-g-performance-0.3.3/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-appendix-g-performance-0.3.2/LICENSE` & `pollination-appendix-g-performance-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-appendix-g-performance-0.3.2/PKG-INFO` & `pollination-appendix-g-performance-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-appendix-g-performance
-Version: 0.3.2
+Version: 0.3.3
 Summary: Run an ASHRAE 90.1 Appendix G simulation and compute the Performance Cost Index (PCI) as well as LEED energy points.
 Home-page: https://github.com/pollination/appendix-g-performance
 Author: pollination
 Author-email: info@ladybug.tools
 Maintainer: chris, ladybug-tools
 Maintainer-email: chris@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-appendix-g-performance-0.3.2/README.md` & `pollination-appendix-g-performance-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pollination-appendix-g-performance-0.3.2/pollination/appendix_g_performance/entry.py` & `pollination-appendix-g-performance-0.3.3/pollination/appendix_g_performance/entry.py`

 * *Files identical despite different names*

### Comparing `pollination-appendix-g-performance-0.3.2/pollination_appendix_g_performance.egg-info/PKG-INFO` & `pollination-appendix-g-performance-0.3.3/pollination_appendix_g_performance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-appendix-g-performance
-Version: 0.3.2
+Version: 0.3.3
 Summary: Run an ASHRAE 90.1 Appendix G simulation and compute the Performance Cost Index (PCI) as well as LEED energy points.
 Home-page: https://github.com/pollination/appendix-g-performance
 Author: pollination
 Author-email: info@ladybug.tools
 Maintainer: chris, ladybug-tools
 Maintainer-email: chris@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-appendix-g-performance-0.3.2/pollination_appendix_g_performance.egg-info/SOURCES.txt` & `pollination-appendix-g-performance-0.3.3/pollination_appendix_g_performance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-appendix-g-performance-0.3.2/setup.py` & `pollination-appendix-g-performance-0.3.3/setup.py`

 * *Files identical despite different names*

