# Comparing `tmp/qase-python-commons-2.0.1.tar.gz` & `tmp/qase-python-commons-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase-python-commons-2.0.1.tar", last modified: Thu Jun  8 07:29:00 2023, max compression
+gzip compressed data, was "qase-python-commons-2.0.2.tar", last modified: Thu Jun 15 15:03:52 2023, max compression
```

## Comparing `qase-python-commons-2.0.1.tar` & `qase-python-commons-2.0.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:29:00.419452 qase-python-commons-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-08 07:29:00.419452 qase-python-commons-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-08 07:29:00.419452 qase-python-commons-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:29:00.415452 qase-python-commons-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:29:00.415452 qase-python-commons-2.0.1/src/qase_python_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-08 07:29:00.000000 qase-python-commons-2.0.1/src/qase_python_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-08 07:29:00.000000 qase-python-commons-2.0.1/src/qase_python_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:29:00.000000 qase-python-commons-2.0.1/src/qase_python_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 07:29:00.000000 qase-python-commons-2.0.1/src/qase_python_commons.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:29:00.000000 qase-python-commons-2.0.1/src/qase_python_commons.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-08 07:29:00.000000 qase-python-commons-2.0.1/src/qase_python_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 07:29:00.000000 qase-python-commons-2.0.1/src/qase_python_commons.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:29:00.415452 qase-python-commons-2.0.1/src/qaseio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:29:00.415452 qase-python-commons-2.0.1/src/qaseio/commons/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:29:00.419452 qase-python-commons-2.0.1/src/qaseio/commons/models/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/models/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/models/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/models/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/models/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/models/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/models/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/models/suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/testops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:29:00.419452 qase-python-commons-2.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:29:00.419452 qase-python-commons-2.0.1/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/tests/models/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:03:52.808604 qase-python-commons-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-15 15:03:52.808604 qase-python-commons-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-15 15:03:52.808604 qase-python-commons-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:03:52.800604 qase-python-commons-2.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:03:52.804604 qase-python-commons-2.0.2/src/qase_python_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-15 15:03:52.000000 qase-python-commons-2.0.2/src/qase_python_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-15 15:03:52.000000 qase-python-commons-2.0.2/src/qase_python_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:03:52.000000 qase-python-commons-2.0.2/src/qase_python_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 15:03:52.000000 qase-python-commons-2.0.2/src/qase_python_commons.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:03:52.000000 qase-python-commons-2.0.2/src/qase_python_commons.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-15 15:03:52.000000 qase-python-commons-2.0.2/src/qase_python_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 15:03:52.000000 qase-python-commons-2.0.2/src/qase_python_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:03:52.800604 qase-python-commons-2.0.2/src/qaseio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:03:52.804604 qase-python-commons-2.0.2/src/qaseio/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/src/qaseio/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/src/qaseio/commons/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/src/qaseio/commons/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/src/qaseio/commons/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:03:52.804604 qase-python-commons-2.0.2/src/qaseio/commons/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/src/qaseio/commons/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/src/qaseio/commons/models/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/src/qaseio/commons/models/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/src/qaseio/commons/models/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/src/qaseio/commons/models/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/src/qaseio/commons/models/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/src/qaseio/commons/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/src/qaseio/commons/models/suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/src/qaseio/commons/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/src/qaseio/commons/testops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/src/qaseio/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:03:52.808604 qase-python-commons-2.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:03:52.808604 qase-python-commons-2.0.2/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/tests/models/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-15 15:03:48.000000 qase-python-commons-2.0.2/tox.ini
```

### Comparing `qase-python-commons-2.0.1/.gitignore` & `qase-python-commons-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.1/.pre-commit-config.yaml` & `qase-python-commons-2.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.1/PKG-INFO` & `qase-python-commons-2.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 2.0.1
+Version: 2.0.2
 Summary: A library for Qase TestOps and Qase Report
 Home-page: https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Author: Qase Team
 Author-email: support@qase.io
 License: apache
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `qase-python-commons-2.0.1/license.txt` & `qase-python-commons-2.0.2/license.txt`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.1/setup.cfg` & `qase-python-commons-2.0.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 author = Qase Team
 author-email = support@qase.io
 license = apache
 long-description = file: README.md
 long-description-content-type = text/markdown; charset=UTF-8; variant=GFM
 url = https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 platforms = any
-version = 2.0.0
+version = 2.0.2
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Programming Language :: Python
 
 [options]
 zip_safe = False
 packages = find_namespace:
```

### Comparing `qase-python-commons-2.0.1/setup.py` & `qase-python-commons-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.1/src/qase_python_commons.egg-info/PKG-INFO` & `qase-python-commons-2.0.2/src/qase_python_commons.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 2.0.1
+Version: 2.0.2
 Summary: A library for Qase TestOps and Qase Report
 Home-page: https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Author: Qase Team
 Author-email: support@qase.io
 License: apache
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `qase-python-commons-2.0.1/src/qase_python_commons.egg-info/SOURCES.txt` & `qase-python-commons-2.0.2/src/qase_python_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.1/src/qaseio/commons/config.py` & `qase-python-commons-2.0.2/src/qaseio/commons/config.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.1/src/qaseio/commons/interceptor.py` & `qase-python-commons-2.0.2/src/qaseio/commons/interceptor.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.1/src/qaseio/commons/loader.py` & `qase-python-commons-2.0.2/src/qaseio/commons/loader.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.1/src/qaseio/commons/models/attachment.py` & `qase-python-commons-2.0.2/src/qaseio/commons/models/attachment.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.1/src/qaseio/commons/models/result.py` & `qase-python-commons-2.0.2/src/qaseio/commons/models/result.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.1/src/qaseio/commons/models/run.py` & `qase-python-commons-2.0.2/src/qaseio/commons/models/run.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.1/src/qaseio/commons/models/runtime.py` & `qase-python-commons-2.0.2/src/qaseio/commons/models/runtime.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.1/src/qaseio/commons/models/step.py` & `qase-python-commons-2.0.2/src/qaseio/commons/models/step.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.1/src/qaseio/commons/report.py` & `qase-python-commons-2.0.2/src/qaseio/commons/report.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.1/src/qaseio/commons/testops.py` & `qase-python-commons-2.0.2/src/qaseio/commons/testops.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
         self.project_code = project_code
         self.run_id = int(run_id) if run_id else run_id
         self.plan_id = plan_id
         self.bulk = bulk
         self.defect = defect
         self.complete_after_run = complete_run
+        self.environment = None
         if environment:
             if isinstance(environment, str):
                 self.environment = self._get_environment(environment)
             elif isinstance(environment, int):
                 self.environment_id = environment
         self.host = host
         self.enabled = True
```

### Comparing `qase-python-commons-2.0.1/src/qaseio/commons/utils.py` & `qase-python-commons-2.0.2/src/qaseio/commons/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import platform
 import threading
 import sys
 import pip
 
 class QaseUtils:
 
     @staticmethod
@@ -31,20 +32,23 @@
     
     @staticmethod
     def get_thread_name() -> str:
         return f"{os.getpid()}-{threading.current_thread().name}"
     
     @staticmethod
     def get_host_data() -> dict:
-        return {
-            "system": os.uname().sysname,
-            "node": os.uname().nodename,
-            "release": os.uname().release,
-            "version": os.uname().version,
-            "machine": os.uname().machine,
-            'python': '.'.join(map(str, sys.version_info)),
-            'pip': pip.__version__
-        }
+        try: 
+            return {
+                "system": platform.uname().system,
+                "node": platform.uname().node,
+                "release": platform.uname().release,
+                "version": platform.uname().version,
+                "machine": platform.uname().machine,
+                'python': '.'.join(map(str, sys.version_info)),
+                'pip': pip.__version__
+            }
+        except Exception as e:
+            return {}
     
     @staticmethod
     def get_filename(path) -> str:
         return os.path.basename(path)
```

### Comparing `qase-python-commons-2.0.1/tests/models/test_run.py` & `qase-python-commons-2.0.2/tests/models/test_run.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.1/tests/test_config.py` & `qase-python-commons-2.0.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.1/tests/test_report.py` & `qase-python-commons-2.0.2/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.1/tests/test_utils.py` & `qase-python-commons-2.0.2/tests/test_utils.py`

 * *Files identical despite different names*

