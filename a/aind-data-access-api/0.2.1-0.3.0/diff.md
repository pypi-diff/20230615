# Comparing `tmp/aind-data-access-api-0.2.1.tar.gz` & `tmp/aind-data-access-api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind-data-access-api-0.2.1.tar", last modified: Wed Apr 19 23:17:31 2023, max compression
+gzip compressed data, was "aind-data-access-api-0.3.0.tar", last modified: Wed Jun 14 23:45:52 2023, max compression
```

## Comparing `aind-data-access-api-0.2.1.tar` & `aind-data-access-api-0.3.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.355052 aind-data-access-api-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.347052 aind-data-access-api-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.351052 aind-data-access-api-0.2.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.351052 aind-data-access-api-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/.github/workflows/init.yml
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-04-19 23:17:31.355052 aind-data-access-api-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.351052 aind-data-access-api-0.2.1/doc_template/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.351052 aind-data-access-api-0.2.1/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.351052 aind-data-access-api-0.2.1/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)   259838 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 23:17:31.355052 aind-data-access-api-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.351052 aind-data-access-api-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.351052 aind-data-access-api-0.2.1/src/aind_data_access_api/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/src/aind_data_access_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/src/aind_data_access_api/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/src/aind_data_access_api/document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/src/aind_data_access_api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/src/aind_data_access_api/rds_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/src/aind_data_access_api/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.355052 aind-data-access-api-0.2.1/src/aind_data_access_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-04-19 23:17:31.000000 aind-data-access-api-0.2.1/src/aind_data_access_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-19 23:17:31.000000 aind-data-access-api-0.2.1/src/aind_data_access_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:17:31.000000 aind-data-access-api-0.2.1/src/aind_data_access_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-19 23:17:31.000000 aind-data-access-api-0.2.1/src/aind_data_access_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-19 23:17:31.000000 aind-data-access-api-0.2.1/src/aind_data_access_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:17:31.355052 aind-data-access-api-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/tests/test_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/tests/test_rds_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-04-19 23:17:16.000000 aind-data-access-api-0.2.1/tests/test_secrets_access.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 23:45:52.970585 aind-data-access-api-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 23:45:52.962585 aind-data-access-api-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 23:45:52.966585 aind-data-access-api-0.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 23:45:52.966585 aind-data-access-api-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/.github/workflows/init.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-06-14 23:45:52.970585 aind-data-access-api-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 23:45:52.966585 aind-data-access-api-0.3.0/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 23:45:52.966585 aind-data-access-api-0.3.0/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 23:45:52.966585 aind-data-access-api-0.3.0/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   259838 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 23:45:52.970585 aind-data-access-api-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 23:45:52.962585 aind-data-access-api-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 23:45:52.966585 aind-data-access-api-0.3.0/src/aind_data_access_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 23:45:38.000000 aind-data-access-api-0.3.0/src/aind_data_access_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/src/aind_data_access_api/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/src/aind_data_access_api/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/src/aind_data_access_api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/src/aind_data_access_api/rds_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/src/aind_data_access_api/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 23:45:52.966585 aind-data-access-api-0.3.0/src/aind_data_access_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-06-14 23:45:52.000000 aind-data-access-api-0.3.0/src/aind_data_access_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-14 23:45:52.000000 aind-data-access-api-0.3.0/src/aind_data_access_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 23:45:52.000000 aind-data-access-api-0.3.0/src/aind_data_access_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-14 23:45:52.000000 aind-data-access-api-0.3.0/src/aind_data_access_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-14 23:45:52.000000 aind-data-access-api-0.3.0/src/aind_data_access_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 23:45:52.970585 aind-data-access-api-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/tests/test_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/tests/test_rds_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-14 23:45:37.000000 aind-data-access-api-0.3.0/tests/test_secrets_access.py
```

### Comparing `aind-data-access-api-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md` & `aind-data-access-api-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md` & `aind-data-access-api-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/.github/ISSUE_TEMPLATE/user-story.md` & `aind-data-access-api-0.3.0/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/.github/workflows/init.yml` & `aind-data-access-api-0.3.0/.github/workflows/init.yml`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/.github/workflows/tag_and_publish.yml` & `aind-data-access-api-0.3.0/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/.github/workflows/test_and_lint.yml` & `aind-data-access-api-0.3.0/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/.gitignore` & `aind-data-access-api-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/LICENSE` & `aind-data-access-api-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/PKG-INFO` & `aind-data-access-api-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-data-access-api
-Version: 0.2.1
+Version: 0.3.0
 Summary: API to interact with a few AIND databases
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind-data-access-api-0.2.1/README.md` & `aind-data-access-api-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/doc_template/Makefile` & `aind-data-access-api-0.3.0/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/doc_template/make.bat` & `aind-data-access-api-0.3.0/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/doc_template/source/_static/dark-logo.svg` & `aind-data-access-api-0.3.0/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/doc_template/source/_static/favicon.ico` & `aind-data-access-api-0.3.0/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/doc_template/source/_static/light-logo.svg` & `aind-data-access-api-0.3.0/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/doc_template/source/conf.py` & `aind-data-access-api-0.3.0/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/pyproject.toml` & `aind-data-access-api-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/src/aind_data_access_api/credentials.py` & `aind-data-access-api-0.3.0/src/aind_data_access_api/credentials.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/src/aind_data_access_api/document_store.py` & `aind-data-access-api-0.3.0/src/aind_data_access_api/document_store.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,29 +23,35 @@
 class Client:
     """Class to establish a document store client."""
 
     def __init__(
         self,
         credentials: DocumentStoreCredentials,
         collection_name: Optional[str] = None,
+        retry_writes: Optional[bool] = True,
     ):
         """
         Construct a client to interface with a document store.
         Parameters
         ----------
         credentials: CoreCredentials
         collection_name : Optional[str]
+        retry_writes : Optional[bool]
+          Whether supported write operations executed within the MongoClient
+          will be retried once after a network error. Default is True. Set to
+          False if writing to AWS DocumentDB.
         """
         self.credentials = credentials
         self.collection_name = collection_name
         self._client = MongoClient(
             credentials.host,
             port=credentials.port,
             username=credentials.username,
             password=credentials.password.get_secret_value(),
+            retryWrites=retry_writes,
         )
 
     @property
     def collection(self):
         """Collection of records in Document Store database to access."""
         db = self._client[self.credentials.database]
         collection = (
```

### Comparing `aind-data-access-api-0.2.1/src/aind_data_access_api/models.py` & `aind-data-access-api-0.3.0/src/aind_data_access_api/models.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/src/aind_data_access_api/rds_tables.py` & `aind-data-access-api-0.3.0/src/aind_data_access_api/rds_tables.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/src/aind_data_access_api/secrets.py` & `aind-data-access-api-0.3.0/src/aind_data_access_api/secrets.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/src/aind_data_access_api.egg-info/PKG-INFO` & `aind-data-access-api-0.3.0/src/aind_data_access_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-data-access-api
-Version: 0.2.1
+Version: 0.3.0
 Summary: API to interact with a few AIND databases
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind-data-access-api-0.2.1/src/aind_data_access_api.egg-info/SOURCES.txt` & `aind-data-access-api-0.3.0/src/aind_data_access_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/tests/test_credentials.py` & `aind-data-access-api-0.3.0/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/tests/test_document_store.py` & `aind-data-access-api-0.3.0/tests/test_document_store.py`

 * *Files 11% similar despite different names*

```diff
@@ -163,10 +163,39 @@
             ),
         ]
 
         mock_bulk_write.assert_called_once_with(operations)
 
         mock_log_info.assert_called_once_with("Documents Upserted")
 
+    def test_retry_writes(self):
+        """Tests that the retryWrites option can be set."""
+        ds_client1 = Client(
+            credentials=DocumentStoreCredentials(
+                username="user",
+                password="password",
+                host="localhost",
+                database="db",
+            ),
+            collection_name="coll",
+        )
+        ds_client2 = Client(
+            credentials=DocumentStoreCredentials(
+                username="user",
+                password="password",
+                host="localhost",
+                database="db",
+            ),
+            collection_name="coll",
+            retry_writes=False,
+        )
+
+        self.assertTrue(
+            ds_client1._client._MongoClient__options._options["retryWrites"]
+        )
+        self.assertFalse(
+            ds_client2._client._MongoClient__options._options["retryWrites"]
+        )
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `aind-data-access-api-0.2.1/tests/test_models.py` & `aind-data-access-api-0.3.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/tests/test_rds_tables.py` & `aind-data-access-api-0.3.0/tests/test_rds_tables.py`

 * *Files identical despite different names*

### Comparing `aind-data-access-api-0.2.1/tests/test_secrets_access.py` & `aind-data-access-api-0.3.0/tests/test_secrets_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Test secrets_access module."""
 import unittest
-from unittest.mock import patch, Mock
+from unittest.mock import Mock, patch
+
 from botocore.exceptions import ClientError
-from aind_data_access_api.secrets import get_secret, get_parameter
+
+from aind_data_access_api.secrets import get_parameter, get_secret
 
 
 class TestSecretAccess(unittest.TestCase):
     """Test methods in secrets_access module"""
 
     @patch("boto3.client")
     def test_get_secret_success(self, mock_boto3_client):
```

