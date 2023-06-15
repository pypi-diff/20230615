# Comparing `tmp/qiskit-iqm-8.3.tar.gz` & `tmp/qiskit-iqm-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-iqm-8.3.tar", last modified: Mon Jun  5 07:52:48 2023, max compression
+gzip compressed data, was "qiskit-iqm-9.0.tar", last modified: Thu Jun  8 08:10:40 2023, max compression
```

## Comparing `qiskit-iqm-8.3.tar` & `qiskit-iqm-9.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.821072 qiskit-iqm-8.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.813072 qiskit-iqm-8.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.813072 qiskit-iqm-8.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/.github/workflows/tag_and_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-06-05 07:52:48.821072 qiskit-iqm-8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.817072 qiskit-iqm-8.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/API.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.817072 qiskit-iqm-8.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/_static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.817072 qiskit-iqm-8.3/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/_static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)   194362 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/_static/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.817072 qiskit-iqm-8.3/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/_templates/autosummary-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/_templates/autosummary-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/_templates/versioning.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/docs/user_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.817072 qiskit-iqm-8.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/examples/bell_measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 07:52:48.821072 qiskit-iqm-8.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.813072 qiskit-iqm-8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.817072 qiskit-iqm-8.3/src/qiskit_iqm/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/src/qiskit_iqm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.817072 qiskit-iqm-8.3/src/qiskit_iqm/fake_backends/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/src/qiskit_iqm/fake_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/src/qiskit_iqm/fake_backends/fake_adonis.py
--rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/src/qiskit_iqm/fake_backends/iqm_fake_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/src/qiskit_iqm/iqm_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/src/qiskit_iqm/iqm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/src/qiskit_iqm/iqm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/src/qiskit_iqm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/src/qiskit_iqm/qiskit_to_iqm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.817072 qiskit-iqm-8.3/src/qiskit_iqm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-06-05 07:52:48.000000 qiskit-iqm-8.3/src/qiskit_iqm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-05 07:52:48.000000 qiskit-iqm-8.3/src/qiskit_iqm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 07:52:48.000000 qiskit-iqm-8.3/src/qiskit_iqm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-05 07:52:48.000000 qiskit-iqm-8.3/src/qiskit_iqm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 07:52:48.000000 qiskit-iqm-8.3/src/qiskit_iqm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tag-from-pipeline.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.821072 qiskit-iqm-8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:52:48.821072 qiskit-iqm-8.3/tests/fake_backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/fake_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/fake_backends/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/fake_backends/test_fake_adonis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/fake_backends/test_iqm_fake_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/test_iqm_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/test_iqm_facade_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/test_iqm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    15596 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/test_iqm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tests/test_qiskit_to_iqm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-05 07:51:54.000000 qiskit-iqm-8.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:10:40.802617 qiskit-iqm-9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:10:40.790617 qiskit-iqm-9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:10:40.794617 qiskit-iqm-9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/.github/workflows/tag_and_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-06-08 08:10:40.802617 qiskit-iqm-9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:10:40.794617 qiskit-iqm-9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/docs/API.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:10:40.794617 qiskit-iqm-9.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/docs/_static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:10:40.794617 qiskit-iqm-9.0/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/docs/_static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   194362 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/docs/_static/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:10:40.794617 qiskit-iqm-9.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/docs/_templates/autosummary-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/docs/_templates/autosummary-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/docs/_templates/versioning.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17637 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/docs/user_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:10:40.794617 qiskit-iqm-9.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/examples/bell_measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 08:10:40.802617 qiskit-iqm-9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:10:40.790617 qiskit-iqm-9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:10:40.798617 qiskit-iqm-9.0/src/qiskit_iqm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/src/qiskit_iqm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:10:40.798617 qiskit-iqm-9.0/src/qiskit_iqm/fake_backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/src/qiskit_iqm/fake_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/src/qiskit_iqm/fake_backends/fake_adonis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14286 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/src/qiskit_iqm/fake_backends/iqm_fake_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/src/qiskit_iqm/iqm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/src/qiskit_iqm/iqm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/src/qiskit_iqm/iqm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/src/qiskit_iqm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/src/qiskit_iqm/qiskit_to_iqm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:10:40.798617 qiskit-iqm-9.0/src/qiskit_iqm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-06-08 08:10:40.000000 qiskit-iqm-9.0/src/qiskit_iqm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-08 08:10:40.000000 qiskit-iqm-9.0/src/qiskit_iqm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 08:10:40.000000 qiskit-iqm-9.0/src/qiskit_iqm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-08 08:10:40.000000 qiskit-iqm-9.0/src/qiskit_iqm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 08:10:40.000000 qiskit-iqm-9.0/src/qiskit_iqm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/tag-from-pipeline.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:10:40.798617 qiskit-iqm-9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:10:40.802617 qiskit-iqm-9.0/tests/fake_backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/tests/fake_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/tests/fake_backends/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/tests/fake_backends/test_fake_adonis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/tests/fake_backends/test_iqm_fake_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/tests/test_iqm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/tests/test_iqm_facade_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/tests/test_iqm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15596 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/tests/test_iqm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/tests/test_qiskit_to_iqm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-08 08:09:26.000000 qiskit-iqm-9.0/tox.ini
```

### Comparing `qiskit-iqm-8.3/.github/workflows/ci.yml` & `qiskit-iqm-9.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/.github/workflows/publish.yml` & `qiskit-iqm-9.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/.github/workflows/tag_and_release.yml` & `qiskit-iqm-9.0/.github/workflows/tag_and_release.yml`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/CHANGELOG.rst` & `qiskit-iqm-9.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 =========
 Changelog
 =========
 
+Version 9.0
+============
+* Add readout errors to ``IQMErrorProfile``. `#50 <https://github.com/iqm-finland/qiskit-on-iqm/pull/50>`_
+
 Version 8.3
 ============
 
 * Bugfixes for ``heralding`` run with zero shots returned. `#65 <https://github.com/iqm-finland/qiskit-on-iqm/pull/65>`_
 * Allow specifying ``calibration_set_id`` both as string and as ``UUID``. `#65 <https://github.com/iqm-finland/qiskit-on-iqm/pull/65>`_
 
 Version 8.2
```

### Comparing `qiskit-iqm-8.3/CONTRIBUTING.rst` & `qiskit-iqm-9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/LICENSE` & `qiskit-iqm-9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/PKG-INFO` & `qiskit-iqm-9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-iqm
-Version: 8.3
+Version: 9.0
 Summary: Qiskit adapter for IQM's quantum architectures
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `qiskit-iqm-8.3/README.rst` & `qiskit-iqm-9.0/README.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/docs/Makefile` & `qiskit-iqm-9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/docs/_static/images/favicon.ico` & `qiskit-iqm-9.0/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/docs/_static/images/logo.png` & `qiskit-iqm-9.0/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/docs/_templates/autosummary-class-template.rst` & `qiskit-iqm-9.0/docs/_templates/autosummary-class-template.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/docs/_templates/autosummary-module-template.rst` & `qiskit-iqm-9.0/docs/_templates/autosummary-module-template.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/docs/_templates/page.html` & `qiskit-iqm-9.0/docs/_templates/page.html`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/docs/_templates/versioning.html` & `qiskit-iqm-9.0/docs/_templates/versioning.html`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/docs/conf.py` & `qiskit-iqm-9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/docs/index.rst` & `qiskit-iqm-9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/docs/user_guide.rst` & `qiskit-iqm-9.0/docs/user_guide.rst`

 * *Files 1% similar despite different names*

```diff
@@ -226,16 +226,16 @@
            meas_0: ═════════════════════════════════════════════════════════════════════╩══╬══╬═
                                                                                            ║  ║
            meas_1: ════════════════════════════════════════════════════════════════════════╩══╬═
                                                                                               ║
            meas_2: ═══════════════════════════════════════════════════════════════════════════╩═
 
 
-Simulating the execution of a transpiled circuit locally
---------------------------------------------------------
+Noisy simulation of quantum circuit execution
+---------------------------------------------
 
 The execution of circuits can be simulated locally, with a noise model to mimic the real hardware as much as possible.
 To this end, Qiskit on IQM provides the class  :class:`.IQMFakeBackend` that can be instantiated with properties of a
 certain QPU, or subclasses of it such as :class:`.IQMFakeAdonis` that represent certain quantum architectures with
 pre-populated properties and noise model.
 
 .. code-block:: python
@@ -249,17 +249,18 @@
     circuit.measure_all()
 
     backend = IQMFakeAdonis()
     job = execute(circuit, backend, shots=1000)
     job.result().get_counts()
 
 
-Above, we use an :class:`.IQMFakeAdonis` instance to run a noisy simulation of ``circuit`` on a simulated 5-qubit Adonis
-chip. If you want to customize the noise model instead of using the default one provided by :class:`.IQMFakeAdonis`, you
-can create a copy of the fake Adonis instance with updated error profile:
+Above, we use an :class:`.IQMFakeAdonis` instance to run a noisy simulation of ``circuit`` on a simulated 5-qubit Adonis chip.
+The noise model includes relaxation (:math:`T_1`) and dephasing (:math:`T_2`), gate infidelities and readout errors.
+If you want to customize the noise model instead of using the default one provided by :class:`.IQMFakeAdonis`, you can create
+a copy of the fake Adonis instance with updated error profile:
 
 .. code-block:: python
 
     error_profile = backend.error_profile
     error_profile.t1s['QB2'] = 30000.0  # Change T1 time of QB2 as example
     custom_fake_backend = backend.copy_with_error_profile(error_profile)
```

### Comparing `qiskit-iqm-8.3/examples/bell_measure.py` & `qiskit-iqm-9.0/examples/bell_measure.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/pyproject.toml` & `qiskit-iqm-9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/src/qiskit_iqm/__init__.py` & `qiskit-iqm-9.0/src/qiskit_iqm/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/src/qiskit_iqm/fake_backends/__init__.py` & `qiskit-iqm-9.0/src/qiskit_iqm/fake_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/src/qiskit_iqm/fake_backends/fake_adonis.py` & `qiskit-iqm-9.0/src/qiskit_iqm/fake_backends/fake_adonis.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Fake (i.e. simulated) backend for IQM Adonis QPU.
+"""Fake backend for IQM Adonis QPU.
 """
 from iqm_client import QuantumArchitectureSpecification
 
 from qiskit_iqm.fake_backends.iqm_fake_backend import IQMErrorProfile, IQMFakeBackend
 
 
 def IQMFakeAdonis() -> IQMFakeBackend:
@@ -33,11 +33,18 @@
             "phased_rx": {"QB1": 0.0006, "QB2": 0.0054, "QB3": 0.0001, "QB4": 0.0, "QB5": 0.0005}
         },
         two_qubit_gate_depolarizing_error_parameters={
             "cz": {("QB1", "QB3"): 0.0335, ("QB2", "QB3"): 0.0344, ("QB3", "QB4"): 0.0192, ("QB3", "QB5"): 0.0373}
         },
         single_qubit_gate_durations={"phased_rx": 40.0},
         two_qubit_gate_durations={"cz": 80.0},
+        readout_errors={
+            "QB1": {"0": 0.021, "1": 0.021},
+            "QB2": {"0": 0.018, "1": 0.018},
+            "QB3": {"0": 0.056, "1": 0.056},
+            "QB4": {"0": 0.021, "1": 0.021},
+            "QB5": {"0": 0.023, "1": 0.023},
+        },
         id_="sample-chip",
     )
 
     return IQMFakeBackend(architecture, error_profile)
```

### Comparing `qiskit-iqm-8.3/src/qiskit_iqm/fake_backends/iqm_fake_backend.py` & `qiskit-iqm-9.0/src/qiskit_iqm/fake_backends/iqm_fake_backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,61 +26,69 @@
 from qiskit_aer import AerSimulator
 from qiskit_aer.noise import NoiseModel
 from qiskit_aer.noise.errors import depolarizing_error, thermal_relaxation_error
 
 from qiskit_iqm.iqm_backend import IQM_TO_QISKIT_GATE_NAME, IQMBackendBase
 
 
+# pylint: disable=too-many-instance-attributes
 @dataclass
 class IQMErrorProfile:
-    """Collection of various properties of an IQM QPU to be used for constructing error model.
+    r"""Collection of various properties of an IQM QPU to be used for constructing error model.
 
     Args:
         t1s: :math:`T_1` times (in ns) for each qubit of the chip, corresponding key is the physical qubit name.
         t2s: :math:`T_2` times (in ns) for each qubit of the chip, corresponding key is the physical qubit name.
         single_qubit_gate_depolarizing_error_parameters: Depolarizing error parameters for single-qubit gates of each
             qubit. Using the values in the depolarizing channel, concatenated with a thermal relaxation channel,
             lead to average gate fidelities that would be determined by benchmarking.
         two_qubit_gate_depolarizing_error_parameters: Depolarizing error parameters for two-qubit gates of each
             connection. Using the values in the depolarizing channel, concatenated with a thermal relaxation channel,
             lead to average gate fidelities that would be determined by benchmarking.
         single_qubit_gate_durations: Gate duration (in ns) for each single-qubit gate
         two_qubit_gate_durations: Gate duration (in ns) for each two-qubit gate.
+        readout_errors: Maps physical qubit names to dicts that describe their single-qubit readout errors.
+            For each qubit, the inner dict maps the state labels "0" and "1" to the probability :math:`P(\neg x|x)`
+            of observing the state :math:`\ket{\neg x}` given the true state is :math:`\ket{x}`.
         id_: Identifier of the chip sample. Defaults to None.
 
     Example:
         .. code-block::
 
             IQMErrorProfile(
                 t1s={"QB1": 10000.0, "QB2": 12000.0, "QB3": 14000.0},
                 t2s={"QB1": 10000.0, "QB2": 12000.0, "QB3": 13000.0},
                 single_qubit_gate_depolarizing_error_parameters={"r": {"QB1": 0.0005, "QB2": 0.0004, "QB3": 0.0010}},
                 two_qubit_gate_depolarizing_error_parameters={"cz": {("QB1", "QB2"): 0.08, ("QB2", "QB3"): 0.03}},
                 single_qubit_gate_durations={"r": 50.},
                 two_qubit_gate_durations={"cz": 100.},
+                readout_errors={"QB1": {"0": 0.02, "1": 0.03},
+                                "QB2": {"0": 0.02, "1": 0.03},
+                                "QB3": {"0": 0.02, "1": 0.03}},
                 id_="threequbit-example_sample"
             )
     """
 
     t1s: dict[str, float]
     t2s: dict[str, float]
     single_qubit_gate_depolarizing_error_parameters: dict[str, dict[str, float]]
     two_qubit_gate_depolarizing_error_parameters: dict[str, dict[tuple[str, str], float]]
     single_qubit_gate_durations: dict[str, float]
     two_qubit_gate_durations: dict[str, float]
+    readout_errors: dict[str, dict[str, float]]
     id_: Union[str, None] = None
 
 
 class IQMFakeBackend(IQMBackendBase):
     """Fake backend that mimics the behaviour of IQM quantum computers. Can be used to perform noisy gate-level
     simulations of quantum circuit execution on IQM hardware.
 
     A fake backend contains information about a specific IQM system, such as the quantum architecture (number of qubits,
     connectivity), the native gate set, and a noise model based on system parameters such as relaxation (:math:`T_1`)
-    and decoherence (:math:`T_2`) times and gate infidelities.
+    and decoherence (:math:`T_2`) times, gate infidelities and readout errors.
 
     Args:
         architecture: Description of the quantum architecture associated with the backend instance.
         chip_sample: Describes the characteristics of a specific chip sample.
     """
 
     def __init__(self, architecture: QuantumArchitectureSpecification, error_profile: IQMErrorProfile, **kwargs):
@@ -182,14 +190,20 @@
                     raise ValueError(
                         (
                             f"Gate `{gate}` in `gate_{property_name}` "
                             "is not supported by quantum architecture `{self.quantum_architecture.id_}`. "
                             f"Valid gates: {architecture.operations}"
                         )
                     )
+        if set(error_profile.readout_errors.keys()) != set(architecture.qubits):
+            raise ValueError(
+                f"The qubits specified in readout errors ({set(error_profile.readout_errors.keys())}) "
+                f"don't match the qubits of the quantum architecture "
+                f"`{architecture.name}` ({architecture.qubits})."
+            )
 
     def _create_noise_model(
         self, architecture: QuantumArchitectureSpecification, error_profile: IQMErrorProfile
     ) -> NoiseModel:
         """
         Builds a noise model from the attributes.
         """
@@ -227,14 +241,19 @@
                 full_error_channel = thermal_relaxation_channel.compose(depolarizing_channel)
                 noise_model.add_quantum_error(
                     full_error_channel,
                     IQM_TO_QISKIT_GATE_NAME[gate],
                     [self.qubit_name_to_index(qb1), self.qubit_name_to_index(qb2)],
                 )
 
+        # Add readout errors
+        for qb, readout_error in error_profile.readout_errors.items():
+            probabilities = [[1 - readout_error["0"], readout_error["0"]], [readout_error["1"], 1 - readout_error["1"]]]
+            noise_model.add_readout_error(probabilities, [self.qubit_name_to_index(qb)])
+
         return noise_model
 
     @classmethod
     def _default_options(cls) -> Options:
         return Options(shots=1024, calibration_set_id=None)
 
     @property
```

### Comparing `qiskit-iqm-8.3/src/qiskit_iqm/iqm_backend.py` & `qiskit-iqm-9.0/src/qiskit_iqm/iqm_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/src/qiskit_iqm/iqm_job.py` & `qiskit-iqm-9.0/src/qiskit_iqm/iqm_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/src/qiskit_iqm/iqm_provider.py` & `qiskit-iqm-9.0/src/qiskit_iqm/iqm_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/src/qiskit_iqm/qiskit_to_iqm.py` & `qiskit-iqm-9.0/src/qiskit_iqm/qiskit_to_iqm.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/src/qiskit_iqm.egg-info/PKG-INFO` & `qiskit-iqm-9.0/src/qiskit_iqm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-iqm
-Version: 8.3
+Version: 9.0
 Summary: Qiskit adapter for IQM's quantum architectures
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `qiskit-iqm-8.3/src/qiskit_iqm.egg-info/SOURCES.txt` & `qiskit-iqm-9.0/src/qiskit_iqm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/tag-from-pipeline.sh` & `qiskit-iqm-9.0/tag-from-pipeline.sh`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/tests/conftest.py` & `qiskit-iqm-9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/tests/fake_backends/conftest.py` & `qiskit-iqm-9.0/tests/fake_backends/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,13 +27,18 @@
         error_profile_contents = {
             "t1s": {"QB1": 2000, "QB2": 2000, "QB3": 2000},
             "t2s": {"QB1": 1000, "QB2": 1000, "QB3": 1000},
             "single_qubit_gate_depolarizing_error_parameters": {"phased_rx": {"QB1": 0.0001, "QB2": 0.0001, "QB3": 0}},
             "two_qubit_gate_depolarizing_error_parameters": {"cz": {("QB1", "QB2"): 0.001, ("QB2", "QB3"): 0.001}},
             "single_qubit_gate_durations": {"phased_rx": 1.0},
             "two_qubit_gate_durations": {"cz": 1.5},
+            "readout_errors": {
+                "QB1": {"0": 0.02, "1": 0.03},
+                "QB2": {"0": 0.02, "1": 0.03},
+                "QB3": {"0": 0.02, "1": 0.03},
+            },
             "id_": "adonis-example_sample",
         }
         error_profile_contents.update(kwargs)
         return IQMErrorProfile(**error_profile_contents)
 
     return error_profile
```

### Comparing `qiskit-iqm-8.3/tests/fake_backends/test_fake_adonis.py` & `qiskit-iqm-9.0/tests/fake_backends/test_fake_adonis.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/tests/fake_backends/test_iqm_fake_backend.py` & `qiskit-iqm-9.0/tests/fake_backends/test_iqm_fake_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -203,7 +203,31 @@
     """
     Tests if the noise model has some noise terms, i.e., tests if the noise model
     doesn't have no noise terms.
     """
     noise_model = backend.noise_model
 
     assert not noise_model.is_ideal()
+
+
+def test_fake_backend_with_readout_errors_more_qubits_than_in_quantum_architecture(
+    linear_architecture_3q,
+    create_3q_error_profile,
+):
+    """Test that ChipSample construction fails if readout errors are provided for
+    other qubits than specified in the quantum architecture"""
+    with pytest.raises(ValueError, match="The qubits specified in readout errors"):
+        error_profile = create_3q_error_profile(
+            readout_errors={
+                "QB1": {"0": 0.02, "1": 0.03},
+                "QB2": {"0": 0.02, "1": 0.03},
+                "QB4": {"0": 0.02, "1": 0.03},
+            },
+        )
+        IQMFakeBackend(linear_architecture_3q, error_profile)
+
+
+def test_noise_model_contains_all_errors(backend):
+    """
+    Test that the noise model contains all necessary errors.
+    """
+    assert set(backend.noise_model.noise_instructions) == {"r", "cz", "measure"}
```

### Comparing `qiskit-iqm-8.3/tests/test_iqm_backend.py` & `qiskit-iqm-9.0/tests/test_iqm_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/tests/test_iqm_facade_backend.py` & `qiskit-iqm-9.0/tests/test_iqm_facade_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/tests/test_iqm_job.py` & `qiskit-iqm-9.0/tests/test_iqm_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/tests/test_iqm_provider.py` & `qiskit-iqm-9.0/tests/test_iqm_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/tests/test_qiskit_to_iqm.py` & `qiskit-iqm-9.0/tests/test_qiskit_to_iqm.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.3/tox.ini` & `qiskit-iqm-9.0/tox.ini`

 * *Files identical despite different names*

