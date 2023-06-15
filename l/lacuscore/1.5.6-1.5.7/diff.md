# Comparing `tmp/lacuscore-1.5.6.tar.gz` & `tmp/lacuscore-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacuscore-1.5.6.tar", max compression
+gzip compressed data, was "lacuscore-1.5.7.tar", max compression
```

## Comparing `lacuscore-1.5.6.tar` & `lacuscore-1.5.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.5.6/LICENSE
--rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.5.6/README.md
--rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.5.6/lacuscore/__init__.py
--rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.5.6/lacuscore/lacus_monitoring.py
--rw-r--r--   0        0        0    30864 2023-06-12 13:01:08.565874 lacuscore-1.5.6/lacuscore/lacuscore.py
--rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.5.6/lacuscore/py.typed
--rw-r--r--   0        0        0     1596 2023-06-12 13:42:13.284994 lacuscore-1.5.6/pyproject.toml
--rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 lacuscore-1.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.5.7/LICENSE
+-rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.5.7/README.md
+-rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.5.7/lacuscore/__init__.py
+-rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.5.7/lacuscore/lacus_monitoring.py
+-rw-r--r--   0        0        0    30864 2023-06-12 13:01:08.565874 lacuscore-1.5.7/lacuscore/lacuscore.py
+-rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.5.7/lacuscore/py.typed
+-rw-r--r--   0        0        0     1596 2023-06-15 16:21:38.611923 lacuscore-1.5.7/pyproject.toml
+-rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 lacuscore-1.5.7/PKG-INFO
```

### Comparing `lacuscore-1.5.6/LICENSE` & `lacuscore-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lacuscore-1.5.6/README.md` & `lacuscore-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `lacuscore-1.5.6/lacuscore/lacus_monitoring.py` & `lacuscore-1.5.7/lacuscore/lacus_monitoring.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.5.6/lacuscore/lacuscore.py` & `lacuscore-1.5.7/lacuscore/lacuscore.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.5.6/pyproject.toml` & `lacuscore-1.5.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacuscore"
-version = "1.5.6"
+version = "1.5.7"
 description = "Core of Lacus, usable as a module"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ail-project/LacusCore"
 documentation = "https://lacuscore.readthedocs.io/en/latest/"
 
 readme = "README.md"
@@ -28,15 +28,15 @@
 
 include = ['README.md']
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.31.0"
 Sphinx = { version = "^7.0.1", optional = true }
-playwrightcapture = {extras = ["recaptcha"], version = "^1.20.4"}
+playwrightcapture = {extras = ["recaptcha"], version = "^1.20.5"}
 defang = "^0.5.3"
 ua-parser = "^0.16.1"
 redis = {version = "^4.5.5", extras = ["hiredis"]}
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
```

### Comparing `lacuscore-1.5.6/PKG-INFO` & `lacuscore-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lacuscore
-Version: 1.5.6
+Version: 1.5.7
 Summary: Core of Lacus, usable as a module
 Home-page: https://github.com/ail-project/LacusCore
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=7.0.1,<8.0.0) ; extra == "docs"
 Requires-Dist: defang (>=0.5.3,<0.6.0)
-Requires-Dist: playwrightcapture[recaptcha] (>=1.20.4,<2.0.0)
+Requires-Dist: playwrightcapture[recaptcha] (>=1.20.5,<2.0.0)
 Requires-Dist: redis[hiredis] (>=4.5.5,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: ua-parser (>=0.16.1,<0.17.0)
 Project-URL: Documentation, https://lacuscore.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/ail-project/LacusCore
 Description-Content-Type: text/markdown
```

