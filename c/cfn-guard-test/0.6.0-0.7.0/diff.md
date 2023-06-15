# Comparing `tmp/cfn-guard-test-0.6.0.tar.gz` & `tmp/cfn_guard_test-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfn-guard-test-0.6.0.tar", last modified: Mon Mar  6 09:30:36 2023, max compression
+gzip compressed data, was "cfn_guard_test-0.7.0.tar", max compression
```

## Comparing `cfn-guard-test-0.6.0.tar` & `cfn_guard_test-0.7.0.tar`

### file list

```diff
@@ -1,28 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:30:36.614240 cfn-guard-test-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-06 09:30:04.000000 cfn-guard-test-0.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-03-06 09:30:36.614240 cfn-guard-test-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-03-06 09:30:04.000000 cfn-guard-test-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:30:36.614240 cfn-guard-test-0.6.0/cfn_guard_test/
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-03-06 09:30:04.000000 cfn-guard-test-0.6.0/cfn_guard_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-03-06 09:30:04.000000 cfn-guard-test-0.6.0/cfn_guard_test/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-06 09:30:04.000000 cfn-guard-test-0.6.0/cfn_guard_test/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-03-06 09:30:04.000000 cfn-guard-test-0.6.0/cfn_guard_test/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-06 09:30:04.000000 cfn-guard-test-0.6.0/cfn_guard_test/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-03-06 09:30:04.000000 cfn-guard-test-0.6.0/cfn_guard_test/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-03-06 09:30:04.000000 cfn-guard-test-0.6.0/cfn_guard_test/suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-03-06 09:30:04.000000 cfn-guard-test-0.6.0/cfn_guard_test/suites.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:30:36.614240 cfn-guard-test-0.6.0/cfn_guard_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-03-06 09:30:36.000000 cfn-guard-test-0.6.0/cfn_guard_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-06 09:30:36.000000 cfn-guard-test-0.6.0/cfn_guard_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 09:30:36.000000 cfn-guard-test-0.6.0/cfn_guard_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-06 09:30:36.000000 cfn-guard-test-0.6.0/cfn_guard_test.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-06 09:30:36.000000 cfn-guard-test-0.6.0/cfn_guard_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-06 09:30:36.000000 cfn-guard-test-0.6.0/cfn_guard_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-06 09:30:04.000000 cfn-guard-test-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-06 09:30:36.614240 cfn-guard-test-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-03-06 09:30:04.000000 cfn-guard-test-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:30:36.614240 cfn-guard-test-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 09:30:04.000000 cfn-guard-test-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-06 09:30:04.000000 cfn-guard-test-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-03-06 09:30:04.000000 cfn-guard-test-0.6.0/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-06 09:30:04.000000 cfn-guard-test-0.6.0/tests/test_custom_set.py
+-rw-r--r--   0        0        0     1052 2023-06-15 14:00:59.241530 cfn_guard_test-0.7.0/LICENSE.md
+-rw-r--r--   0        0        0     3144 2023-06-15 14:01:00.009542 cfn_guard_test-0.7.0/cfn_guard_test/__init__.py
+-rw-r--r--   0        0        0     2379 2023-06-15 14:00:59.241530 cfn_guard_test-0.7.0/cfn_guard_test/case.py
+-rw-r--r--   0        0        0     2781 2023-06-15 14:00:59.241530 cfn_guard_test-0.7.0/cfn_guard_test/reader.py
+-rw-r--r--   0        0        0     2412 2023-06-15 14:00:59.241530 cfn_guard_test-0.7.0/cfn_guard_test/report.py
+-rw-r--r--   0        0        0     1135 2023-06-15 14:00:59.241530 cfn_guard_test-0.7.0/cfn_guard_test/rule.py
+-rw-r--r--   0        0        0     1962 2023-06-15 14:00:59.241530 cfn_guard_test-0.7.0/cfn_guard_test/runner.py
+-rw-r--r--   0        0        0     2317 2023-06-15 14:00:59.241530 cfn_guard_test-0.7.0/cfn_guard_test/suite.py
+-rw-r--r--   0        0        0     1835 2023-06-15 14:00:59.241530 cfn_guard_test-0.7.0/cfn_guard_test/suites.py
+-rw-r--r--   0        0        0      950 2023-06-15 14:01:00.009542 cfn_guard_test-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 cfn_guard_test-0.7.0/PKG-INFO
```

### Comparing `cfn-guard-test-0.6.0/LICENSE.md` & `cfn_guard_test-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cfn-guard-test-0.6.0/cfn_guard_test/__init__.py` & `cfn_guard_test-0.7.0/cfn_guard_test/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from cfn_guard_test.rule import CfnGuardRule
 from cfn_guard_test.runner import CfnGuardRunner
 from cfn_guard_test.suite import CfnGuardTestSuite
 from cfn_guard_test.suites import CfnGuardTestSuites
 from cfn_guard_test.reader import CfnGuardReader
 
 
+__version__ = "0.7.0"
+
+
 def validate_cfn_guard_path(
     ctx: click.Context, _: click.Option, value: Optional[str]
 ) -> str:
     if not value or ctx.resilient_parsing:
         return "cfn-guard"
 
     if value.split("/")[-1] != "cfn-guard":
```

### Comparing `cfn-guard-test-0.6.0/cfn_guard_test/case.py` & `cfn_guard_test-0.7.0/cfn_guard_test/case.py`

 * *Files identical despite different names*

### Comparing `cfn-guard-test-0.6.0/cfn_guard_test/reader.py` & `cfn_guard_test-0.7.0/cfn_guard_test/reader.py`

 * *Files identical despite different names*

### Comparing `cfn-guard-test-0.6.0/cfn_guard_test/report.py` & `cfn_guard_test-0.7.0/cfn_guard_test/report.py`

 * *Files identical despite different names*

### Comparing `cfn-guard-test-0.6.0/cfn_guard_test/rule.py` & `cfn_guard_test-0.7.0/cfn_guard_test/rule.py`

 * *Files identical despite different names*

### Comparing `cfn-guard-test-0.6.0/cfn_guard_test/runner.py` & `cfn_guard_test-0.7.0/cfn_guard_test/runner.py`

 * *Files identical despite different names*

### Comparing `cfn-guard-test-0.6.0/cfn_guard_test/suite.py` & `cfn_guard_test-0.7.0/cfn_guard_test/suite.py`

 * *Files identical despite different names*

### Comparing `cfn-guard-test-0.6.0/cfn_guard_test/suites.py` & `cfn_guard_test-0.7.0/cfn_guard_test/suites.py`

 * *Files identical despite different names*

### Comparing `cfn-guard-test-0.6.0/pyproject.toml` & `cfn_guard_test-0.7.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 [tool.poetry]
 name = "cfn-guard-test"
-version = "0.6.0"
+version = "0.7.0"
 description = "cfn-guard-test is a wrapper for cfn-guard that allows you to run unit tests for your cfn-guard rules."
 authors = ["Joris Conijn <joris@conijnonline.nl>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 junit-xml = "^1.9"
 click = "^8.0.3"
 
 [tool.poetry.dev-dependencies]
-black = "^23.1"
-mypy = "^1.0"
-pytest = "^7.2.1"
-pytest-cov = "^4.0.0"
+black = "^23.3"
+mypy = "^1.3"
+pytest = "^7.3.2"
+pytest-cov = "^4.1.0"
 pytest-mypy = "^0.10.3"
 toml = "^0.10.2"
 types-toml = "^0.10.8"
-twine = "^4.0.2"
 xenon = "^0.9.0"
 radon = "^5.1.0"
+python-semantic-release = "^7.34.4"
 
 [tool.poetry.scripts]
 cfn-guard-test = "cfn_guard_test:main"
 
+[tool.semantic_release]
+version_variable = [
+    "cfn_guard_test/__init__.py:__version__",
+    "pyproject.toml:version"
+]
+branch = "main"
+upload_to_pypi = true
+upload_to_release = true
+build_command = "pip install poetry && poetry build"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

