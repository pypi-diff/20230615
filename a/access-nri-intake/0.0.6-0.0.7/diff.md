# Comparing `tmp/access_nri_intake-0.0.6.tar.gz` & `tmp/access_nri_intake-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "access_nri_intake-0.0.6.tar", last modified: Tue Jun  6 02:40:58 2023, max compression
+gzip compressed data, was "access_nri_intake-0.0.7.tar", last modified: Thu Jun 15 00:02:09 2023, max compression
```

## Comparing `access_nri_intake-0.0.6.tar` & `access_nri_intake-0.0.7.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:40:58.751484 access_nri_intake-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-06 02:40:58.751484 access_nri_intake-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 02:40:58.751484 access_nri_intake-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:40:58.747485 access_nri_intake-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:40:58.751484 access_nri_intake-0.0.6/src/access_nri_intake/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-06 02:40:58.751484 access_nri_intake-0.0.6/src/access_nri_intake/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:40:58.751484 access_nri_intake-0.0.6/src/access_nri_intake/cat/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/cat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/cat/catalog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:40:58.751484 access_nri_intake-0.0.6/src/access_nri_intake/esmcat/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/esmcat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/esmcat/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/esmcat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:40:58.751484 access_nri_intake-0.0.6/src/access_nri_intake/metacat/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/metacat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/metacat/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/metacat/translators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:40:58.751484 access_nri_intake-0.0.6/src/access_nri_intake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-06 02:40:58.000000 access_nri_intake-0.0.6/src/access_nri_intake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-06 02:40:58.000000 access_nri_intake-0.0.6/src/access_nri_intake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 02:40:58.000000 access_nri_intake-0.0.6/src/access_nri_intake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-06 02:40:58.000000 access_nri_intake-0.0.6/src/access_nri_intake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-06 02:40:58.000000 access_nri_intake-0.0.6/src/access_nri_intake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 02:40:58.000000 access_nri_intake-0.0.6/src/access_nri_intake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83751 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:02:09.094477 access_nri_intake-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-15 00:02:09.094477 access_nri_intake-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 00:02:09.094477 access_nri_intake-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:02:09.086476 access_nri_intake-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:02:09.094477 access_nri_intake-0.0.7/src/access_nri_intake/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-15 00:02:09.094477 access_nri_intake-0.0.7/src/access_nri_intake/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:02:09.094477 access_nri_intake-0.0.7/src/access_nri_intake/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/catalog/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/catalog/translators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:02:09.094477 access_nri_intake-0.0.7/src/access_nri_intake/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/data/catalog.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:02:09.094477 access_nri_intake-0.0.7/src/access_nri_intake/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12554 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/source/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/source/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:02:09.090477 access_nri_intake-0.0.7/src/access_nri_intake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-15 00:02:09.000000 access_nri_intake-0.0.7/src/access_nri_intake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-15 00:02:09.000000 access_nri_intake-0.0.7/src/access_nri_intake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 00:02:09.000000 access_nri_intake-0.0.7/src/access_nri_intake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-15 00:02:09.000000 access_nri_intake-0.0.7/src/access_nri_intake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-15 00:02:09.000000 access_nri_intake-0.0.7/src/access_nri_intake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 00:02:09.000000 access_nri_intake-0.0.7/src/access_nri_intake.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:02:09.094477 access_nri_intake-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/tests/test_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83751 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/versioneer.py
```

### Comparing `access_nri_intake-0.0.6/LICENSE` & `access_nri_intake-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.6/PKG-INFO` & `access_nri_intake-0.0.7/src/access_nri_intake.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: access_nri_intake
-Version: 0.0.6
+Name: access-nri-intake
+Version: 0.0.7
 Summary: Intake catalog managed by ACCESS-NRI and associated tools
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -23,17 +23,17 @@
 ------------
 
 +---------------+----------------------+
 | Documentation | |docs|               |
 +---------------+----------------------+
 | Package       | |pypi| |conda|       |
 +---------------+----------------------+
-| CI/CD         | |pre-commit| |cd|    |
+| CI/CD         | |ci| |cd|            |
 +---------------+----------------------+
-| Development   | |black|              |
+| Development   | |codecov| |black|    |
 +---------------+----------------------+
 | License       | |license|            |
 +---------------+----------------------+
 
 .. |docs| image:: https://readthedocs.org/projects/access-nri-intake-catalog/badge/?version=latest
     :target: https://access-nri-intake-catalog.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
@@ -42,21 +42,25 @@
         :target: https://pypi.org/project/access-nri-intake/
         :alt: PyPI package
         
 .. |conda| image:: https://img.shields.io/conda/v/accessnri/access-nri-intake
         :target: https://anaconda.org/accessnri/access-nri-intake
         :alt: Conda package
 
-.. |pre-commit| image:: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/pre-commit.yaml/badge.svg
-        :target: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/pre-commit.yaml
-        :alt: Pre-commit status
+.. |ci| image:: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/ci.yml/badge.svg
+        :target: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/ci.yml
+        :alt: Package CI status
         
 .. |cd| image:: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/cd.yml/badge.svg
         :target: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/cd.yml
         :alt: Package CD status
+
+.. |codecov| image:: https://codecov.io/gh/ACCESS-NRI/access-nri-intake-catalog/branch/main/graph/badge.svg?token=DAC1NK32LM
+        :target: https://codecov.io/gh/ACCESS-NRI/access-nri-intake-catalog
+        :alt: Code test coverage
         
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
         :target: https://github.com/python/black
         :alt: Black code formatter
         
 .. |license| image:: https://img.shields.io/github/license/ACCESS-NRI/intake-dataframe-catalog
         :target: https://github.com/ACCESS-NRI/intake-dataframe-catalog/blob/main/LICENSE
```

### Comparing `access_nri_intake-0.0.6/README.rst` & `access_nri_intake-0.0.7/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 ------------
 
 +---------------+----------------------+
 | Documentation | |docs|               |
 +---------------+----------------------+
 | Package       | |pypi| |conda|       |
 +---------------+----------------------+
-| CI/CD         | |pre-commit| |cd|    |
+| CI/CD         | |ci| |cd|            |
 +---------------+----------------------+
-| Development   | |black|              |
+| Development   | |codecov| |black|    |
 +---------------+----------------------+
 | License       | |license|            |
 +---------------+----------------------+
 
 .. |docs| image:: https://readthedocs.org/projects/access-nri-intake-catalog/badge/?version=latest
     :target: https://access-nri-intake-catalog.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
@@ -28,21 +28,25 @@
         :target: https://pypi.org/project/access-nri-intake/
         :alt: PyPI package
         
 .. |conda| image:: https://img.shields.io/conda/v/accessnri/access-nri-intake
         :target: https://anaconda.org/accessnri/access-nri-intake
         :alt: Conda package
 
-.. |pre-commit| image:: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/pre-commit.yaml/badge.svg
-        :target: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/pre-commit.yaml
-        :alt: Pre-commit status
+.. |ci| image:: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/ci.yml/badge.svg
+        :target: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/ci.yml
+        :alt: Package CI status
         
 .. |cd| image:: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/cd.yml/badge.svg
         :target: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/cd.yml
         :alt: Package CD status
+
+.. |codecov| image:: https://codecov.io/gh/ACCESS-NRI/access-nri-intake-catalog/branch/main/graph/badge.svg?token=DAC1NK32LM
+        :target: https://codecov.io/gh/ACCESS-NRI/access-nri-intake-catalog
+        :alt: Code test coverage
         
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
         :target: https://github.com/python/black
         :alt: Black code formatter
         
 .. |license| image:: https://img.shields.io/github/license/ACCESS-NRI/intake-dataframe-catalog
         :target: https://github.com/ACCESS-NRI/intake-dataframe-catalog/blob/main/LICENSE
```

### Comparing `access_nri_intake-0.0.6/pyproject.toml` & `access_nri_intake-0.0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -22,40 +22,48 @@
     "jsonschema",
     "pooch",
     "xarray",
 ]
 dynamic = ["version"]
 
 [project.scripts]
-metacat-build = "access_nri_intake.cli:build"
+catalog-build = "access_nri_intake.cli:build"
 
 [project.entry-points."intake.catalogs"]
-access_nri = "access_nri_intake.cat:data"
+access_nri = "access_nri_intake.data:data"
 
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = [
   "setuptools >= 61.0.0",
   "versioneer[toml]",
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
-access_nri_intake = ["cat/catalog.yaml"]
+access_nri_intake = ["data/catalog.yaml"]
 
 [tool.versioneer]
 VCS = "git"
 style = "pep440"
 versionfile_source = "src/access_nri_intake/_version.py"
 versionfile_build = "access_nri_intake/_version.py"
 tag_prefix = "v"
 parentdir_prefix = "access-nri-intake-"
 
+[tool.pytest.ini_options]
+addopts = "--cov=./src --cov-report=xml"
+
+[tool.coverage.run]
+omit = [
+    "src/access_nri_intake/_version.py",
+]
+
 [tool.ruff]
 target-version = "py39"
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
```

### Comparing `access_nri_intake-0.0.6/src/access_nri_intake/cat/catalog.yaml` & `access_nri_intake-0.0.7/src/access_nri_intake/data/catalog.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -13,10 +13,10 @@
     description: ACCESS-NRI intake catalog
     driver: intake_dataframe_catalog.core.DfFileCatalog
     metadata:
       storage: gdata/cj50+gdata/p73+gdata/ik11+gdata/dk92
       version: '{{version}}'
     parameters:
       version:
-        default: v0.0.6
+        default: v0.0.7
         description: Catalog version
         type: str
```

### Comparing `access_nri_intake-0.0.6/src/access_nri_intake/cli.py` & `access_nri_intake-0.0.7/src/access_nri_intake/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # Copyright 2023 ACCESS-NRI and contributors. See the top-level COPYRIGHT file for details.
 # SPDX-License-Identifier: Apache-2.0
 
+""" Command line interface for access-nri-intake """
+
 import argparse
 import logging
 import os
 
 import jsonschema
 import yaml
 
 from . import __version__
-from .esmcat import builders
-from .metacat import METADATA_JSONSCHEMA, manager, translators
+from .catalog import EXP_JSONSCHEMA, translators
+from .catalog.manager import CatalogManager
+from .source import builders
 from .utils import load_metadata_yaml, validate_against_schema
 
 
 class MetadataCheckError(Exception):
     pass
 
 
 def _parse_inputs(config_yamls, build_path):
     """
-    Parse inputs into a list of tuples of MetacatManager methods and args to
+    Parse inputs into a list of tuples of CatalogManager methods and args to
     pass to the methods
     """
 
     args = []
     for config_yaml in config_yamls:
         with open(config_yaml) as f:
             config = yaml.safe_load(f)
@@ -58,24 +61,24 @@
             args.append((method, source_args | kwargs))
 
     return args
 
 
 def _check_args(args_list):
     """
-    Run some checks on the parsed argmuents to be passed to the MetacatManager
+    Run some checks on the parsed argmuents to be passed to the CatalogManager
     """
 
     names = []
     uuids = []
     for args in args_list:
         names.append(args["name"])
         uuids.append(args["metadata"]["experiment_uuid"])
         try:
-            validate_against_schema(args["metadata"], METADATA_JSONSCHEMA)
+            validate_against_schema(args["metadata"], EXP_JSONSCHEMA)
         except jsonschema.exceptions.ValidationError:
             raise MetadataCheckError(
                 f"Failed to validate metadata.yaml for {args['name']}. See traceback for details."
             )
 
     if len(names) != len(set(names)):
         seen = set()
@@ -88,80 +91,82 @@
         raise MetadataCheckError(
             f"There are experiments with the same experiment_uuid: {dupes}"
         )
 
 
 def build():
     """
-    Build an intake-dataframe-catalog metacatalog from YAML configuration file(s).
+    Build an intake-dataframe-catalog from YAML configuration file(s).
     """
 
     log_fmt = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
     logging.basicConfig(level=logging.INFO, format=log_fmt)
     logger = logging.getLogger(__name__)
 
     parser = argparse.ArgumentParser(
-        description="Build an intake-dataframe-catalog metacatalog from YAML configuration file(s)."
+        description="Build an intake-dataframe-catalog from YAML configuration file(s)."
     )
     parser.add_argument(
         "config_yaml",
         type=str,
         nargs="+",
-        help="Configuration YAML file(s) specifying the intake source(s) to add.",
+        help="Configuration YAML file(s) specifying the Intake source(s) to add.",
     )
 
     parser.add_argument(
         "--build_base_path",
         type=str,
         default="./",
         help=(
-            "Directory in which to build the intake metacatalog and source(s). A directory with name equal to "
-            "the version (see the `--version` argument) of the catalog being built will be created here. The "
-            "metacatalog file (see the `--metacatalog_file` argument) will be written into this version "
-            "directory, and any new intake source(s) will be written into a 'source' directory within the version "
-            "directory.",
+            "Directory in which to build the catalog and source(s). A directory with name equal to the "
+            "version (see the `--version` argument) of the catalog being built will be created here. The "
+            "catalog file (see the `--catalog_file` argument) will be written into this version directory, "
+            "and any new intake source(s) will be written into a 'source' directory within the version "
+            "directory. Defaults to the current work directory."
         ),
     )
 
     parser.add_argument(
-        "--metacatalog_file",
+        "--catalog_file",
         type=str,
         default="metacatalog.csv",
-        help="The name of the intake-dataframe-catalog metacatalog.",
+        help="The name of the intake-dataframe-catalog. Defaults to 'metacatalog.csv'",
     )
 
     parser.add_argument(
         "--version",
         type=str,
         default=__version__,
-        help=("The version of the catalog to build/add to."),
+        help=(
+            "The version of the catalog to build/add to. Defaults to the current version of access-nri-intake."
+        ),
     )
 
     args = parser.parse_args()
     config_yamls = args.config_yaml
     build_base_path = args.build_base_path
-    metacatalog_file = args.metacatalog_file
+    catalog_file = args.catalog_file
     version = args.version
 
     if not version.startswith("v"):
         version = f"v{version}"
 
     # Create the build directories
     build_base_path = os.path.abspath(build_base_path)
     build_path = os.path.join(build_base_path, version, "source")
-    metacatalog_path = os.path.join(build_base_path, version, metacatalog_file)
+    metacatalog_path = os.path.join(build_base_path, version, catalog_file)
     os.makedirs(build_path, exist_ok=True)
 
-    # Parse inputs to pass to MetacatManager
+    # Parse inputs to pass to CatalogManager
     parsed_sources = _parse_inputs(config_yamls, build_path)
     _check_args([parsed_source[1] for parsed_source in parsed_sources])
 
     # Build the catalog
     for (method, args) in parsed_sources:
-        man = manager.MetacatManager(path=metacatalog_path)
+        man = CatalogManager(path=metacatalog_path)
         logger.info(f"Adding '{args['name']}' to metacatalog '{metacatalog_path}'")
         getattr(man, method)(**args).add()
 
     # Write catalog yaml file
     storage = set()
     for (_, args) in parsed_sources:
         storage |= {
@@ -170,21 +175,21 @@
 
     cat = man.dfcat
     cat.name = "access_nri"
     cat.description = "ACCESS-NRI intake catalog"
     yaml_dict = yaml.safe_load(cat.yaml())
 
     yaml_dict["sources"]["access_nri"]["args"]["path"] = os.path.join(
-        build_base_path, "{{version}}", metacatalog_file
+        build_base_path, "{{version}}", catalog_file
     )
     yaml_dict["sources"]["access_nri"]["args"]["mode"] = "r"
     yaml_dict["sources"]["access_nri"]["metadata"] = {
         "version": "{{version}}",
         "storage": "+".join(list(storage)),
     }
     yaml_dict["sources"]["access_nri"]["parameters"] = {
         "version": {"description": "Catalog version", "type": "str", "default": version}
     }
 
     _here = os.path.abspath(os.path.dirname(__file__))
-    with open(os.path.join(_here, "cat", "catalog.yaml"), "w") as fobj:
+    with open(os.path.join(_here, "data", "catalog.yaml"), "w") as fobj:
         yaml.dump(yaml_dict, fobj)
```

### Comparing `access_nri_intake-0.0.6/src/access_nri_intake/esmcat/__init__.py` & `access_nri_intake-0.0.7/src/access_nri_intake/source/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2023 ACCESS-NRI and contributors. See the top-level COPYRIGHT file for details.
 # SPDX-License-Identifier: Apache-2.0
 
-""" Tools for generating intake-esm catalogs """
+""" Tools for generating Intake-ESM catalogs """
 
 
-from ..utils import get_catalog_jsonschema
+from ..utils import get_jsonschema
 
 CORE_COLUMNS = [
     "path",
     "realm",
     "frequency",
     "variable",
     "start_date",
@@ -16,10 +16,10 @@
 ]
 PATH_COLUMN = "path"
 VARIABLE_COLUMN = "variable"
 
 SCHEMA_URL = "https://raw.githubusercontent.com/ACCESS-NRI/schema/4e3d10e563d7c1c9f66e9ab92a2926cdec3d6893/file_asset.json"
 SCHEMA_HASH = "2a09030653f495939c90a22e95dd1c4587c8695f7f07e17b9129a6491469f9fc"
 
-_, CATALOG_JSONSCHEMA = get_catalog_jsonschema(
+_, ESM_JSONSCHEMA = get_jsonschema(
     url=SCHEMA_URL, known_hash=SCHEMA_HASH, required=CORE_COLUMNS
 )
```

### Comparing `access_nri_intake-0.0.6/src/access_nri_intake/esmcat/builders.py` & `access_nri_intake-0.0.7/src/access_nri_intake/source/builders.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # Copyright 2023 ACCESS-NRI and contributors. See the top-level COPYRIGHT file for details.
 # SPDX-License-Identifier: Apache-2.0
 
-""" Builders for generating intake-esm catalogs """
+""" Builders for generating Intake-ESM datastores """
 
 import multiprocessing
 import re
 import traceback
 from pathlib import Path
 
 import xarray as xr
 from ecgtools.builder import INVALID_ASSET, TRACEBACK, Builder
 
 from ..utils import validate_against_schema
-from . import CATALOG_JSONSCHEMA, PATH_COLUMN, VARIABLE_COLUMN
-from .utils import get_timeinfo, strip_pattern_rh
+from . import ESM_JSONSCHEMA, PATH_COLUMN, VARIABLE_COLUMN
+from .utils import get_timeinfo, redact_time_stamps
 
 
 class ParserError(Exception):
     pass
 
 
 class BaseBuilder(Builder):
     """
-    Base class for creating intake-esm catalog builders. Not intended for direct use.
+    Base class for creating Intake-ESM datastore builders. Not intended for direct use.
     This builds on the ecgtools.Builder class.
     """
 
     def __init__(
         self,
         path,
         depth=0,
@@ -103,29 +103,29 @@
             directory=directory,
             catalog_type="file",
             to_csv_kwargs={"compression": "gzip"},
         )
 
     def save(self, name, description, directory=None):
         """
-        Save catalog contents to a file.
+        Save datastore contents to a file.
 
         Parameters
         ----------
         name: str
-            The name of the file to save the catalog to.
+            The name of the file to save the datastore to.
         description : str
             Detailed multi-line description of the collection.
         directory: str, optional
-            The directory to save the catalog to. If None, use the current directory.
+            The directory to save the datastore to. If None, use the current directory.
         """
 
         if self.df.empty:
             raise ValueError(
-                "intake-esm catalog has not yet been built. Please run `.build()` first"
+                "Intake-ESM datastore has not yet been built. Please run `.build()` first"
             )
 
         self._save(name, description, directory)
 
     def validate_parser(self):
         """
         Run the parser on a single file and check the schema of the info being parsed
@@ -135,24 +135,24 @@
             raise ValueError(
                 "asset list provided is None. Please run `.get_assets()` first"
             )
 
         for asset in self.assets:
             info = self.parser(asset)
             if INVALID_ASSET not in info:
-                validate_against_schema(info, CATALOG_JSONSCHEMA)
+                validate_against_schema(info, ESM_JSONSCHEMA)
                 return self
 
         raise ParserError(
             "Parser returns no valid assets. Try parsing a single file with Builder.parser(file)"
         )
 
     def build(self):
         """
-        Builds a catalog from a list of netCDF files or zarr stores.
+        Builds a datastore from a list of netCDF files or zarr stores.
         """
 
         self.get_assets().validate_parser().parse().clean_dataframe()
 
         return self
 
     @property
@@ -179,19 +179,19 @@
 
         Parameters
         ----------
         file: str
             The path to the file
         """
         # This method should be overwritten
-        pass
+        raise NotImplementedError
 
 
 class AccessOm2Builder(BaseBuilder):
-    """Intake-esm catalog builder for ACCESS-OM2 COSIMA datasets"""
+    """Intake-ESM datastore builder for ACCESS-OM2 COSIMA datasets"""
 
     def __init__(self, path):
         """
         Initialise a AccessOm2Builder
 
         Parameters
         ----------
@@ -231,28 +231,16 @@
             realm = match_groups[2]
 
             if realm == "ice":
                 realm = "seaIce"
 
             filename = Path(file).stem
 
-            # Get file id without any dates
-            # - ocean-3d-v-1-monthly-pow02-ym_1958_04.nc
-            # - iceh.057-daily.nc
-            # - oceanbgc-3d-caco3-1-yearly-mean-y_2015.nc
-            file_id = strip_pattern_rh(
-                [
-                    r"\d{4}[-_]\d{2}[-_]\d{2}",
-                    r"\d{4}[-_]\d{2}",
-                    r"\d{4}",
-                    r"\d{3}",
-                    r"\d{2}",
-                ],
-                filename,
-            )
+            # Get file id from filename without any time stamps
+            file_id = redact_time_stamps(filename)
 
             with xr.open_dataset(
                 file,
                 chunks={},
                 decode_cf=False,
                 decode_times=False,
                 decode_coords=False,
@@ -290,15 +278,15 @@
             return info
 
         except Exception:
             return {INVALID_ASSET: file, TRACEBACK: traceback.format_exc()}
 
 
 class AccessEsm15Builder(BaseBuilder):
-    """Intake-esm catalog builder for ACCESS-ESM1.5 datasets"""
+    """Intake-ESM datastore builder for ACCESS-ESM1.5 datasets"""
 
     def __init__(self, path, ensemble=False):
         """
         Initialise a AccessEsm15Builder
 
         Parameters
         ----------
@@ -346,25 +334,17 @@
             realm = match_groups[1]
 
             realm_mapping = {"atm": "atmos", "ocn": "ocean", "ice": "seaIce"}
             realm = realm_mapping[realm]
 
             filename = Path(file).stem
 
-            # Get file id without any dates or exp_id
-            # - iceh_m.2014-06.nc
-            # - bz687a.pm107912_mon.nc
-            # - bz687a.p7107912_mon.nc
-            # - PI-GWL-B2035.pe-109904_dai.nc
-            # - PI-1pct-02.pe-011802_dai.nc_dai.nc
-            # - ocean_daily.nc-02531231
-            file_id = strip_pattern_rh(
-                [r"\d{4}[-_]\d{2}", r"\d{8}", r"\d{6}"], filename
-            )
-            file_id = strip_pattern_rh([exp_id], file_id)
+            # Get file id from filename without any time stamps or exp_id
+            file_id = re.sub(exp_id, "", filename)
+            file_id = redact_time_stamps(file_id)
 
             with xr.open_dataset(
                 file,
                 chunks={},
                 decode_cf=False,
                 decode_times=False,
                 decode_coords=False,
@@ -404,10 +384,10 @@
 
         except Exception:
             return {INVALID_ASSET: file, TRACEBACK: traceback.format_exc()}
 
 
 # Include this so it is in the documentation
 class AccessCm2Builder(AccessEsm15Builder):
-    """Intake-esm catalog builder for ACCESS-CM2 datasets"""
+    """Intake-ESM datastore builder for ACCESS-CM2 datasets"""
 
     pass
```

### Comparing `access_nri_intake-0.0.6/src/access_nri_intake/esmcat/utils.py` & `access_nri_intake-0.0.7/src/access_nri_intake/source/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright 2023 ACCESS-NRI and contributors. See the top-level COPYRIGHT file for details.
 # SPDX-License-Identifier: Apache-2.0
 
-""" Shared utilities for writing intake-esm builders and their parsers """
+""" Shared utilities for writing Intake-ESM builders and their parsers """
 
 import re
 
 import cftime
 
 
 def get_timeinfo(ds, time_dim="time"):
@@ -64,33 +64,48 @@
     return (
         start_time.strftime("%Y-%m-%d, %H:%M:%S"),
         end_time.strftime("%Y-%m-%d, %H:%M:%S"),
         frequency,
     )
 
 
-def strip_pattern_rh(patterns, string):
+def redact_time_stamps(string, fill="X"):
     """
-    Sequentially strip a list of regex patterns from a string, starting from the right
-    hand side. Then replace any "-" and "." with "_" and then remove double or dangling "_".
+    Sequentially try to redact time stamps from a filename string, starting from the right hand side.
+    Then replace any "-" and "." with "_". E.g. "bz687a.pm107912_mon.nc" is redacted to
+    bz687a.pmXXXXXX_mon.nc
 
-    Parameters:
-    -----------
-    patterns: list of str
-        The list of regex patterns to strip
+    Parameters
+    ----------
     string: str
-        A filename with the suffixe (e.g. .nc) removed
+        A filename with the suffix (e.g. .nc) removed
+    fill: str, optional
+        The string to replace the digits in the time stamp with
     """
 
+    # TODO: this function is a horrible hack
+
+    # Patterns are removed in this order. Matching stops once a match is made
+    patterns = [
+        r"\d{4}[-_]\d{2}[-_]\d{2}",
+        r"\d{4}[-_]\d{2}",
+        r"\d{8}",
+        r"\d{6}",
+        r"\d{4}",
+        r"\d{3}",
+        r"\d{2}",
+    ]
+
     # Strip first matched pattern
     stripped = string
     for pattern in patterns:
         match = re.match(rf"^.*({pattern}(?!.*{pattern})).*$", stripped)
         if match:
-            stripped = stripped[: match.start(1)] + stripped[match.end(1) :]
+            replace = re.sub(r"\d", fill, match.group(1))
+            stripped = stripped[: match.start(1)] + replace + stripped[match.end(1) :]
             break
 
     # Enforce Python characters
     stripped = re.sub(r"[-.]", "_", stripped)
 
     # Remove any double or dangling _
     return re.sub(r"__", "_", stripped).strip("_")
```

### Comparing `access_nri_intake-0.0.6/src/access_nri_intake/metacat/__init__.py` & `access_nri_intake-0.0.7/src/access_nri_intake/catalog/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2023 ACCESS-NRI and contributors. See the top-level COPYRIGHT file for details.
 # SPDX-License-Identifier: Apache-2.0
 
-""" Tools for managing intake-dataframe-catalog metacatalogs """
+""" Tools for managing intake-dataframe-catalogs like the ACCESS-NRI catalog """
 
 
-from ..utils import get_catalog_jsonschema
+from ..utils import get_jsonschema
 
 CORE_COLUMNS = [
     "name",
     "model",
     "description",
     "realm",
     "frequency",
@@ -17,15 +17,15 @@
 YAML_COLUMN = "yaml"
 NAME_COLUMN = "name"
 TRANSLATOR_GROUPBY_COLUMNS = ["model", "realm", "frequency"]
 
 SCHEMA_URL = "https://raw.githubusercontent.com/ACCESS-NRI/schema/4e3d10e563d7c1c9f66e9ab92a2926cdec3d6893/experiment_asset.json"
 SCHEMA_HASH = "b18cf5bdd06a6f5bcdc71dfc80f7336c63eb49f6d6f75c2cd3371e59eee5488b"
 
-METADATA_JSONSCHEMA, CATALOG_JSONSCHEMA = get_catalog_jsonschema(
+EXP_JSONSCHEMA, CATALOG_JSONSCHEMA = get_jsonschema(
     url=SCHEMA_URL, known_hash=SCHEMA_HASH, required=CORE_COLUMNS
 )
 
 COLUMNS_WITH_ITERABLES = [
     col
     for col in CORE_COLUMNS
     if CATALOG_JSONSCHEMA["properties"][col]["type"] == "array"
```

### Comparing `access_nri_intake-0.0.6/src/access_nri_intake/metacat/manager.py` & `access_nri_intake-0.0.7/src/access_nri_intake/catalog/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright 2023 ACCESS-NRI and contributors. See the top-level COPYRIGHT file for details.
 # SPDX-License-Identifier: Apache-2.0
 
-""" Manager for adding/updating intake catalogs in an intake-dataframe-catalog (metacatalogs) """
+""" Manager for adding/updating intake sources in an intake-dataframe-catalog like the ACCESS-NRI catalog """
 
 import os
 
 import intake
 from intake_dataframe_catalog.core import DfFileCatalog
 
 from ..utils import validate_against_schema
@@ -16,28 +16,28 @@
     NAME_COLUMN,
     TRANSLATOR_GROUPBY_COLUMNS,
     YAML_COLUMN,
 )
 from .translators import DefaultTranslator
 
 
-class CatalogExistsError(Exception):
-    "Exception for trying to write catalog that already exists"
+class CatalogManagerError(Exception):
+    "Generic Exception for the CatalogManager class"
     pass
 
 
-class MetacatManager:
+class CatalogManager:
     """
-    Add/update intake sources in an intake-dataframe-catalog (metacatalog)
+    Add/update intake sources in an intake-dataframe-catalog like the ACCESS-NRI catalog
     """
 
     def __init__(self, path):
         """
         Initialise a CatalogManager instance to add/update intake sources in a
-        intake-dataframe-catalog metacatalog
+        intake-dataframe-catalog like the ACCESS-NRI catalog
 
         Parameters
         ----------
         path: str
             The path to the intake-dataframe-catalog
         """
 
@@ -97,15 +97,15 @@
         """
 
         metadata = metadata or {}
 
         json_file = os.path.abspath(f"{os.path.join(directory, name)}.json")
         if os.path.isfile(json_file):
             if not overwrite:
-                raise CatalogExistsError(
+                raise CatalogManagerError(
                     f"A catalog already exists for {name}. To overwrite, "
                     "pass `overwrite=True` to CatalogBuilder.build"
                 )
 
         builder = builder(path, **kwargs).build()
         builder.save(name=name, description=description, directory=directory)
 
@@ -126,15 +126,15 @@
         description,
         path,
         translator,
         metadata=None,
         **kwargs,
     ):
         """
-        Load an existing intake catalog and add it to the metacatalog
+        Load an existing intake catalog and add it to the catalog
 
         Parameters
         ----------
         name: str
             The name of the catalog
         description: str
             Description of the contents of the catalog
@@ -163,33 +163,38 @@
             path, name, description, metadata, translator, **kwargs
         )
 
         return self
 
     def add(self, **kwargs):
         """
-        Add the catalog to an intake-dataframe-catalog
+        Add a source to the catalog
 
         Parameters
         ----------
         kwargs: dict, optional
             Additional keyword arguments passed to :py:func:`~pandas.DataFrame.to_csv`.
         """
 
+        if self.source is None:
+            raise CatalogManagerError(
+                "To add a source to the catalog you must first load or build the source"
+            )
+
         # Overwrite the catalog name with the name_column entry in metadata
         name = self.source_metadata[NAME_COLUMN].unique()
         if len(name) != 1:
             raise ValueError(
                 f"Metadata column '{NAME_COLUMN}' must be the same for all rows "
                 "since this corresponds to the catalog name"
             )
         name = name[0]
         self.source.name = name
 
-        # Validate df_metadata against schema
+        # Validate source_metadata against schema
         for idx, row in self.source_metadata.iterrows():
             validate_against_schema(row.to_dict(), CATALOG_JSONSCHEMA)
 
         overwrite = True
         for _, row in self.source_metadata.iterrows():
             self.dfcat.add(self.source, row.to_dict(), overwrite=overwrite)
             overwrite = False
```

### Comparing `access_nri_intake-0.0.6/src/access_nri_intake/metacat/translators.py` & `access_nri_intake-0.0.7/src/access_nri_intake/catalog/translators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,99 @@
 # Copyright 2023 ACCESS-NRI and contributors. See the top-level COPYRIGHT file for details.
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Tools for translating metadata in an intake source into a metadata table to use in an intake-dataframe-catalog
+like the ACCESS-NRI catalog
 """
 
 import re
 from functools import partial
 
 import pandas as pd
 import tlz
 
 from . import COLUMNS_WITH_ITERABLES
 
 
 class TranslatorError(Exception):
+    "Generic Exception for the Translator classes"
     pass
 
 
 class DefaultTranslator:
     """
-    Default Translator for translating metadata in an intake catalog into a :py:class:`~pandas.DataFrame`
+    Default Translator for translating metadata in an intake datastore into a :py:class:`~pandas.DataFrame`
     of metadata for use in an intake-dataframe-catalog.
     """
 
-    def __init__(self, cat, columns):
+    def __init__(self, source, columns):
         """
         Initialise a DefaultTranslator. This Translator works as follows:
 
-        - If the input catalog is an intake-esm catalog, the translator will first look for the column in the
-             esmcat.df attribute, casting iterable columns to tuples. If the catalog is not an intake-esm catalog,
-             this step is skipped.
-        - If that fails, the translator will then look for the column name as an attribute on the catalog itself
-        - If that fails, the translator will then look for the column name in the metadata attribute of the catalog
+        - If the input source is an intake-esm datastore, the translator will first look for the column in the
+          esmcat.df attribute, casting iterable columns to tuples. If the source is not an intake-esm datastore,
+          this step is skipped.
+        - If that fails, the translator will then look for the column name as an attribute on the source itself
+        - If that fails, the translator will then look for the column name in the metadata attribute of the source
 
         Parameters
         ----------
-        cat: :py:class:`~intake.DataSource`
-            The catalog to use to do the translations
+        source: :py:class:`~intake.DataSource`
+            The source to translate from
         columns: list of str
-            The columns to translate
+            The columns to translate to (these are the core columns in the intake-dataframe-catalog)
         """
 
-        self.cat = cat
+        self.source = source
         self.columns = columns
         self._dispatch = {
             column: partial(self._default_translator, column=column)
             for column in columns
         }
 
     def _default_translator(self, column):
         """
-        Try to translate a column from a catalog using the default translator. This translator works as follows:
-        - If the input catalog is an intake-esm catalog, the translator will first look for the column in the
-             esmcat.df attribute, casting iterable columns to tuples. If the catalog is not an intake-esm catalog,
+        Try to translate a column from a source using the default translator. This translator works as follows:
+        - If the input source is an intake-esm datastore, the translator will first look for the column in the
+             esmcat.df attribute, casting iterable columns to tuples. If the source is not an intake-esm datastore,
              this step is skipped.
-        - If that fails, the translator will then look for the column name as an attribute on the catalog itself
-        - If that fails, the translator will then look for the column name in the metadata attribute of the catalog
+        - If that fails, the translator will then look for the column name as an attribute on the source itself
+        - If that fails, the translator will then look for the column name in the metadata attribute of the source
 
         Parameters
         ----------
         column: str
             The column to translate, e.g. "frequency"
         """
-        if hasattr(self.cat, "esmcat"):
+        if hasattr(self.source, "esmcat"):
             try:
-                series = self.cat.df[column]
+                series = self.source.df[column]
 
                 # Cast to tuples
-                if column in self.cat.esmcat.columns_with_iterables:
+                if column in self.source.esmcat.columns_with_iterables:
                     return series.apply(tuple)
                 elif column in COLUMNS_WITH_ITERABLES:
                     return to_tuple(series)
                 else:
                     return series
             except KeyError:
-                len_df = len(self.cat.df)
+                len_df = len(self.source.df)
         else:
             len_df = 1
 
-        if hasattr(self.cat, column):
-            val = getattr(self.cat, column)
-        elif column in self.cat.metadata:
-            val = self.cat.metadata[column]
+        if hasattr(self.source, column):
+            val = getattr(self.source, column)
+        elif column in self.source.metadata:
+            val = self.source.metadata[column]
             if isinstance(val, list):
                 val = tuple(val)
         else:
             raise TranslatorError(
-                f"Could not translate '{column}' from {self.cat.name} using {self.__class__.__name__}"
+                f"Could not translate '{column}' from {self.source.name} using {self.__class__.__name__}"
             )
 
         return pd.Series([val] * len_df)
 
     def translate(self, groupby):
         """
         Return the translated :py:class:`~pandas.DataFrame` of metadata and merge into set of
@@ -135,133 +137,133 @@
         )
 
         return df_grouped[self.columns]  # Preserve ordering
 
 
 class Cmip6Translator(DefaultTranslator):
     """
-    CMIP6 Translator for translating metadata from the NCI CMIP6 intake catalogs.
+    CMIP6 Translator for translating metadata from the NCI CMIP6 intake datastores.
     """
 
-    def __init__(self, cat, columns):
+    def __init__(self, source, columns):
         """
         Initialise a Cmip6Translator
 
         Parameters
         ----------
-        cat: :py:class:`~intake.DataSource`
-            The NCI CMIP6 intake-esm catalog
+        source: :py:class:`~intake.DataSource`
+            The NCI CMIP6 intake-esm datastore
         columns: list of str
-            The columns to translate
+            The columns to translate to (these are the core columns in the intake-dataframe-catalog)
         """
 
-        super().__init__(cat, columns)
+        super().__init__(source, columns)
         self._dispatch["model"] = self._model_translator
         self._dispatch["realm"] = self._realm_translator
         self._dispatch["frequency"] = self._frequency_translator
         self._dispatch["variable"] = self._variable_translator
 
     def _model_translator(self):
         """
         Return model from source_id
         """
-        return to_tuple(self.cat.df["source_id"])
+        return to_tuple(self.source.df["source_id"])
 
     def _realm_translator(self):
         """
         Return realm, fixing a few issues
         """
-        return _cmip_realm_translator(self.cat.df)
+        return _cmip_realm_translator(self.source.df)
 
     def _frequency_translator(self):
         """
         Return frequency, fixing a few issues
         """
-        return _cmip_frequency_translator(self.cat.df)
+        return _cmip_frequency_translator(self.source.df)
 
     def _variable_translator(self):
         """
         Return variable as a tuple
         """
-        return to_tuple(self.cat.df["variable_id"])
+        return to_tuple(self.source.df["variable_id"])
 
 
 class Cmip5Translator(DefaultTranslator):
     """
-    CMIP5 Translator for translating metadata from the NCI CMIP5 intake catalogs.
+    CMIP5 Translator for translating metadata from the NCI CMIP5 intake datastores.
     """
 
-    def __init__(self, cat, columns):
+    def __init__(self, source, columns):
         """
         Initialise a Cmip5Translator
 
         Parameters
         ----------
-        cat: :py:class:`~intake.DataSource`
-            The NCI CMIP5 intake-esm catalog
+        source: :py:class:`~intake.DataSource`
+            The NCI CMIP5 intake-esm datastore
         columns: list of str
-            The columns to translate
+            The columns to translate to (these are the core columns in the intake-dataframe-catalog)
         """
 
-        super().__init__(cat, columns)
+        super().__init__(source, columns)
         self._dispatch["model"] = self._model_translator
         self._dispatch["realm"] = self._realm_translator
         self._dispatch["frequency"] = self._frequency_translator
         self._dispatch["variable"] = self._variable_translator
 
     def _model_translator(self):
         """
         Return variable as a tuple
         """
-        return to_tuple(self.cat.df["model"])
+        return to_tuple(self.source.df["model"])
 
     def _realm_translator(self):
         """
         Return realm, fixing a few issues
         """
-        return _cmip_realm_translator(self.cat.df)
+        return _cmip_realm_translator(self.source.df)
 
     def _frequency_translator(self):
         """
         Return frequency, fixing a few issues
         """
-        return _cmip_frequency_translator(self.cat.df)
+        return _cmip_frequency_translator(self.source.df)
 
     def _variable_translator(self):
         """
         Return variable as a tuple
         """
-        return to_tuple(self.cat.df["variable"])
+        return to_tuple(self.source.df["variable"])
 
 
 class EraiTranslator(DefaultTranslator):
     """
-    ERAI Translator for translating metadata from the NCI ERA-Interim intake catalogs.
+    ERAI Translator for translating metadata from the NCI ERA-Interim intake datastore.
     """
 
-    def __init__(self, cat, columns):
+    def __init__(self, source, columns):
         """
         Initialise a EraiTranslator
 
         Parameters
         ----------
-        cat: :py:class:`~intake.DataSource`
-            The NCI ERA-Interim intake-esm catalog
+        source: :py:class:`~intake.DataSource`
+            The NCI ERA-Interim intake-esm datastore
         columns: list of str
-            The columns to translate
+            The columns to translate (these are the core columns in the intake-dataframe-catalog)
         """
 
-        super().__init__(cat, columns)
+        super().__init__(source, columns)
         self._dispatch["variable"] = self._variable_translator
 
     def _variable_translator(self):
         """
         Return variable as a tuple
         """
-        return to_tuple(self.cat.df["variable"])
+        return to_tuple(self.source.df["variable"])
 
 
 def _cmip_frequency_translator(df):
     """
     Return frequency from CMIP frequency metadata
     """
```

### Comparing `access_nri_intake-0.0.6/src/access_nri_intake/utils.py` & `access_nri_intake-0.0.7/src/access_nri_intake/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Copyright 2023 ACCESS-NRI and contributors. See the top-level COPYRIGHT file for details.
 # SPDX-License-Identifier: Apache-2.0
 
-""" Utility functions """
+""" General utility functions  for access-rni-intake """
 
 import json
 from warnings import warn
 
 import jsonschema
 import pooch
 import yaml
 
 
-def get_catalog_jsonschema(url, known_hash, required):
+def get_jsonschema(url, known_hash, required):
     """
     Download a jsonschema from a url. Returns the unaltered jsonschema and a version with the "required" key
     matching the properties provided.
 
     Parameters
     ----------
     url: str
@@ -28,27 +28,27 @@
     """
 
     schema_file = pooch.retrieve(url=url, known_hash=known_hash)
 
     with open(schema_file) as fpath:
         schema = json.load(fpath)
 
-    catalog_schema = schema.copy()
+    schema_required = schema.copy()
     req = []
     for col in required:
-        if col not in catalog_schema["properties"]:
+        if col not in schema_required["properties"]:
             warn(
                 f"Required column {col} does not exist in schema. Entries in this column will not be validated"
             )
         else:
             req.append(col)
 
-    catalog_schema["required"] = req
+    schema_required["required"] = req
 
-    return schema, catalog_schema
+    return schema, schema_required
 
 
 def load_metadata_yaml(path):
     """
     Load a metadata.yaml file, leaving dates as strings
 
     Parameters
```

### Comparing `access_nri_intake-0.0.6/src/access_nri_intake.egg-info/PKG-INFO` & `access_nri_intake-0.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: access-nri-intake
-Version: 0.0.6
+Name: access_nri_intake
+Version: 0.0.7
 Summary: Intake catalog managed by ACCESS-NRI and associated tools
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -23,17 +23,17 @@
 ------------
 
 +---------------+----------------------+
 | Documentation | |docs|               |
 +---------------+----------------------+
 | Package       | |pypi| |conda|       |
 +---------------+----------------------+
-| CI/CD         | |pre-commit| |cd|    |
+| CI/CD         | |ci| |cd|            |
 +---------------+----------------------+
-| Development   | |black|              |
+| Development   | |codecov| |black|    |
 +---------------+----------------------+
 | License       | |license|            |
 +---------------+----------------------+
 
 .. |docs| image:: https://readthedocs.org/projects/access-nri-intake-catalog/badge/?version=latest
     :target: https://access-nri-intake-catalog.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
@@ -42,21 +42,25 @@
         :target: https://pypi.org/project/access-nri-intake/
         :alt: PyPI package
         
 .. |conda| image:: https://img.shields.io/conda/v/accessnri/access-nri-intake
         :target: https://anaconda.org/accessnri/access-nri-intake
         :alt: Conda package
 
-.. |pre-commit| image:: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/pre-commit.yaml/badge.svg
-        :target: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/pre-commit.yaml
-        :alt: Pre-commit status
+.. |ci| image:: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/ci.yml/badge.svg
+        :target: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/ci.yml
+        :alt: Package CI status
         
 .. |cd| image:: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/cd.yml/badge.svg
         :target: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/cd.yml
         :alt: Package CD status
+
+.. |codecov| image:: https://codecov.io/gh/ACCESS-NRI/access-nri-intake-catalog/branch/main/graph/badge.svg?token=DAC1NK32LM
+        :target: https://codecov.io/gh/ACCESS-NRI/access-nri-intake-catalog
+        :alt: Code test coverage
         
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
         :target: https://github.com/python/black
         :alt: Black code formatter
         
 .. |license| image:: https://img.shields.io/github/license/ACCESS-NRI/intake-dataframe-catalog
         :target: https://github.com/ACCESS-NRI/intake-dataframe-catalog/blob/main/LICENSE
```

### Comparing `access_nri_intake-0.0.6/src/access_nri_intake.egg-info/SOURCES.txt` & `access_nri_intake-0.0.7/src/access_nri_intake.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 src/access_nri_intake/utils.py
 src/access_nri_intake.egg-info/PKG-INFO
 src/access_nri_intake.egg-info/SOURCES.txt
 src/access_nri_intake.egg-info/dependency_links.txt
 src/access_nri_intake.egg-info/entry_points.txt
 src/access_nri_intake.egg-info/requires.txt
 src/access_nri_intake.egg-info/top_level.txt
-src/access_nri_intake/cat/__init__.py
-src/access_nri_intake/cat/catalog.yaml
-src/access_nri_intake/esmcat/__init__.py
-src/access_nri_intake/esmcat/builders.py
-src/access_nri_intake/esmcat/utils.py
-src/access_nri_intake/metacat/__init__.py
-src/access_nri_intake/metacat/manager.py
-src/access_nri_intake/metacat/translators.py
+src/access_nri_intake/catalog/__init__.py
+src/access_nri_intake/catalog/manager.py
+src/access_nri_intake/catalog/translators.py
+src/access_nri_intake/data/__init__.py
+src/access_nri_intake/data/catalog.yaml
+src/access_nri_intake/source/__init__.py
+src/access_nri_intake/source/builders.py
+src/access_nri_intake/source/utils.py
+tests/test_builders.py
```

### Comparing `access_nri_intake-0.0.6/versioneer.py` & `access_nri_intake-0.0.7/versioneer.py`

 * *Files identical despite different names*

