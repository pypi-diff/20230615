# Comparing `tmp/qase-pytest-5.0.0.tar.gz` & `tmp/qase-pytest-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase-pytest-5.0.0.tar", last modified: Thu Jun  8 07:33:18 2023, max compression
+gzip compressed data, was "qase-pytest-5.0.1.tar", last modified: Thu Jun 15 15:49:56 2023, max compression
```

## Comparing `qase-pytest-5.0.0.tar` & `qase-pytest-5.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:33:18.970138 qase-pytest-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/CONFIGURATION.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-08 07:33:18.970138 qase-pytest-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/UPGRADE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:33:18.966138 qase-pytest-5.0.0/example/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/example/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-08 07:33:18.970138 qase-pytest-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:33:18.966138 qase-pytest-5.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:33:18.970138 qase-pytest-5.0.0/src/qase_pytest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-08 07:33:18.000000 qase-pytest-5.0.0/src/qase_pytest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-08 07:33:18.000000 qase-pytest-5.0.0/src/qase_pytest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:33:18.000000 qase-pytest-5.0.0/src/qase_pytest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 07:33:18.000000 qase-pytest-5.0.0/src/qase_pytest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 07:33:18.000000 qase-pytest-5.0.0/src/qase_pytest.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:33:18.000000 qase-pytest-5.0.0/src/qase_pytest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-08 07:33:18.000000 qase-pytest-5.0.0/src/qase_pytest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 07:33:18.000000 qase-pytest-5.0.0/src/qase_pytest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:33:18.966138 qase-pytest-5.0.0/src/qaseio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:33:18.970138 qase-pytest-5.0.0/src/qaseio/pytest/
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/src/qaseio/pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/src/qaseio/pytest/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/src/qaseio/pytest/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/src/qaseio/pytest/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:33:18.970138 qase-pytest-5.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:49:56.489991 qase-pytest-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/CONFIGURATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-15 15:49:56.489991 qase-pytest-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/UPGRADE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:49:56.485991 qase-pytest-5.0.1/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/example/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-15 15:49:56.489991 qase-pytest-5.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:49:56.481991 qase-pytest-5.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:49:56.485991 qase-pytest-5.0.1/src/qase_pytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-15 15:49:56.000000 qase-pytest-5.0.1/src/qase_pytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-15 15:49:56.000000 qase-pytest-5.0.1/src/qase_pytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:49:56.000000 qase-pytest-5.0.1/src/qase_pytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 15:49:56.000000 qase-pytest-5.0.1/src/qase_pytest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 15:49:56.000000 qase-pytest-5.0.1/src/qase_pytest.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:49:56.000000 qase-pytest-5.0.1/src/qase_pytest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-15 15:49:56.000000 qase-pytest-5.0.1/src/qase_pytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 15:49:56.000000 qase-pytest-5.0.1/src/qase_pytest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:49:56.481991 qase-pytest-5.0.1/src/qaseio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:49:56.485991 qase-pytest-5.0.1/src/qaseio/pytest/
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/src/qaseio/pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/src/qaseio/pytest/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/src/qaseio/pytest/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/src/qaseio/pytest/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:49:56.485991 qase-pytest-5.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-15 15:49:51.000000 qase-pytest-5.0.1/tox.ini
```

### Comparing `qase-pytest-5.0.0/.coveragerc` & `qase-pytest-5.0.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.0/.gitignore` & `qase-pytest-5.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.0/.pre-commit-config.yaml` & `qase-pytest-5.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.0/CONFIGURATION.md` & `qase-pytest-5.0.1/CONFIGURATION.md`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.0/LICENSE.txt` & `qase-pytest-5.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.0/PKG-INFO` & `qase-pytest-5.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-pytest
-Version: 5.0.0
+Version: 5.0.1
 Summary: Qase Pytest Plugin for Qase TestOps and Qase Report
 Home-page: https://github.com/qase-tms/qase-python/tree/master/qase-pytest
 Author: Qase Team
 Author-email: support@qase.io
 License: apache
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `qase-pytest-5.0.0/README.md` & `qase-pytest-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.0/UPGRADE.md` & `qase-pytest-5.0.1/UPGRADE.md`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.0/setup.cfg` & `qase-pytest-5.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 author = Qase Team
 author-email = support@qase.io
 license = apache
 long-description = file: README.md
 long-description-content-type = text/markdown; charset=UTF-8; variant=GFM
 url = https://github.com/qase-tms/qase-python/tree/master/qase-pytest
 platforms = any
-version = 5.0.0
+version = 5.0.1
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Pytest
 	Programming Language :: Python
 
 [options]
 zip_safe = False
```

### Comparing `qase-pytest-5.0.0/setup.py` & `qase-pytest-5.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     PyScaffold helps you to put up the scaffold of your new Python project.
     Learn more under: https://pyscaffold.org/
 """
 import sys
 from pkg_resources import VersionConflict, require
 from setuptools import setup
 
-VERSION = "5.0.0"
+VERSION = "5.0.1"
 
 try:
     require("setuptools>=38.3")
 except VersionConflict:
     print("Error: version of setuptools is too old (<38.3)!")
     sys.exit(1)
```

### Comparing `qase-pytest-5.0.0/src/qase_pytest.egg-info/PKG-INFO` & `qase-pytest-5.0.1/src/qase_pytest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-pytest
-Version: 5.0.0
+Version: 5.0.1
 Summary: Qase Pytest Plugin for Qase TestOps and Qase Report
 Home-page: https://github.com/qase-tms/qase-python/tree/master/qase-pytest
 Author: Qase Team
 Author-email: support@qase.io
 License: apache
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `qase-pytest-5.0.0/src/qase_pytest.egg-info/SOURCES.txt` & `qase-pytest-5.0.1/src/qase_pytest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.0/src/qaseio/pytest/__init__.py` & `qase-pytest-5.0.1/src/qaseio/pytest/__init__.py`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.0/src/qaseio/pytest/conftest.py` & `qase-pytest-5.0.1/src/qaseio/pytest/conftest.py`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.0/src/qaseio/pytest/options.py` & `qase-pytest-5.0.1/src/qaseio/pytest/options.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,22 @@
             default="qase_execution_plan.json",
             help="Path to file with execution plan"
         )
 
         QasePytestOptions.add_option_ini(
             parser,
             group,
+            "--qase-testops-project",
+            dest="qase_testops_project",
+            help="Project code in Qase TestOps"
+        )
+
+        QasePytestOptions.add_option_ini(
+            parser,
+            group,
             "--qase-testops-api-token",
             dest="qase_testops_api_token",
             help="API token for Qase TestOps"
         )
 
         QasePytestOptions.add_option_ini(
             parser,
@@ -55,14 +63,22 @@
             default="qase.io",
             help="API host for Qase TestOps"
         )
 
         QasePytestOptions.add_option_ini(
             parser,
             group,
+            "--qase-testops-plan-id",
+            dest="qase_testops_plan_id",
+            help="Test Plan ID in Qase TestOps"
+        )
+
+        QasePytestOptions.add_option_ini(
+            parser,
+            group,
             "--qase-testops-run-id",
             dest="qase_testops_run_id",
             help="Test Run ID in Qase TestOps"
         )
 
         QasePytestOptions.add_option_ini(
             parser,
```

### Comparing `qase-pytest-5.0.0/src/qaseio/pytest/plugin.py` & `qase-pytest-5.0.1/src/qaseio/pytest/plugin.py`

 * *Files identical despite different names*

