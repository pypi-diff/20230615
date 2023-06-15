# Comparing `tmp/jscc-0.2.0.tar.gz` & `tmp/jscc-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jscc-0.2.0.tar", last modified: Thu Jun 15 03:46:45 2023, max compression
+gzip compressed data, was "jscc-0.2.1.tar", last modified: Thu Jun 15 03:54:43 2023, max compression
```

## Comparing `jscc-0.2.0.tar` & `jscc-0.2.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.161881 jscc-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-15 03:46:32.000000 jscc-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-15 03:46:32.000000 jscc-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-15 03:46:45.161881 jscc-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-15 03:46:32.000000 jscc-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.145881 jscc-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.145881 jscc-0.2.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/api/schema.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.145881 jscc-0.2.0/docs/api/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/api/testing/checks.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/api/testing/filesystem.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/api/testing/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/api/testing/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.149881 jscc-0.2.0/jscc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:32.000000 jscc-0.2.0/jscc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-15 03:46:32.000000 jscc-0.2.0/jscc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-15 03:46:32.000000 jscc-0.2.0/jscc/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.149881 jscc-0.2.0/jscc/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:32.000000 jscc-0.2.0/jscc/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31563 2023-06-15 03:46:32.000000 jscc-0.2.0/jscc/testing/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-15 03:46:32.000000 jscc-0.2.0/jscc/testing/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-15 03:46:32.000000 jscc-0.2.0/jscc/testing/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.149881 jscc-0.2.0/jscc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-15 03:46:45.000000 jscc-0.2.0/jscc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-15 03:46:45.000000 jscc-0.2.0/jscc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 03:46:45.000000 jscc-0.2.0/jscc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-15 03:46:45.000000 jscc-0.2.0/jscc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 03:46:45.000000 jscc-0.2.0/jscc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 03:46:32.000000 jscc-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-15 03:46:45.161881 jscc-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.149881 jscc-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.149881 jscc-0.2.0/tests/cassettes/
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/cassettes/test_http_get_error.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/cassettes/test_http_head_error.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.153881 jscc-0.2.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/codelist.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.153881 jscc-0.2.0/tests/fixtures/csv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/csv/empty.csv
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/csv/valid.csv
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.153881 jscc-0.2.0/tests/fixtures/empty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/empty-array.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/empty-object.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/empty-string.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/false.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.153881 jscc-0.2.0/tests/fixtures/empty/htmlcov/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/htmlcov/empty.txt
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/null.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/whitespace-string.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/whitespace.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/whitespace.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/zero-float.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/zero-int.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.157881 jscc-0.2.0/tests/fixtures/indent/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/indent/ascii.json
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/indent/compact.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/indent/indented.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/indent/invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/indent/no-newline.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.157881 jscc-0.2.0/tests/fixtures/json/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/json/duplicate-key.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/json/invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/json/valid.json
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/meta-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/patch.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.157881 jscc-0.2.0/tests/fixtures/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/array_items.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.161881 jscc-0.2.0/tests/fixtures/schema/build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/build/ignore.json
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/codelist_enum.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.161881 jscc-0.2.0/tests/fixtures/schema/codelists/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/codelists/+nonexistent.csv
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/codelists/extra.csv
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/codelists/failClosedArray.csv
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/codelists/failClosedString.csv
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/codelists/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/deep_properties.json
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/items_type.json
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/letter_case.json
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/merge_properties.json
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/metadata_presence.json
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/null_type.json
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/object_id.json
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/ref.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:43.819081 jscc-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-15 03:54:32.000000 jscc-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-15 03:54:32.000000 jscc-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-15 03:54:43.819081 jscc-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-15 03:54:32.000000 jscc-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:43.803081 jscc-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-15 03:54:32.000000 jscc-0.2.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:43.803081 jscc-0.2.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 03:54:32.000000 jscc-0.2.1/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-15 03:54:32.000000 jscc-0.2.1/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 03:54:32.000000 jscc-0.2.1/docs/api/schema.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:43.807081 jscc-0.2.1/docs/api/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-15 03:54:32.000000 jscc-0.2.1/docs/api/testing/checks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 03:54:32.000000 jscc-0.2.1/docs/api/testing/filesystem.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 03:54:32.000000 jscc-0.2.1/docs/api/testing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 03:54:32.000000 jscc-0.2.1/docs/api/testing/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-15 03:54:32.000000 jscc-0.2.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-15 03:54:32.000000 jscc-0.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-15 03:54:32.000000 jscc-0.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 03:54:32.000000 jscc-0.2.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:43.807081 jscc-0.2.1/jscc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:32.000000 jscc-0.2.1/jscc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-15 03:54:32.000000 jscc-0.2.1/jscc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-15 03:54:32.000000 jscc-0.2.1/jscc/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:43.807081 jscc-0.2.1/jscc/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:32.000000 jscc-0.2.1/jscc/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31480 2023-06-15 03:54:32.000000 jscc-0.2.1/jscc/testing/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-15 03:54:32.000000 jscc-0.2.1/jscc/testing/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-15 03:54:32.000000 jscc-0.2.1/jscc/testing/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:43.807081 jscc-0.2.1/jscc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-15 03:54:43.000000 jscc-0.2.1/jscc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-15 03:54:43.000000 jscc-0.2.1/jscc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 03:54:43.000000 jscc-0.2.1/jscc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-15 03:54:43.000000 jscc-0.2.1/jscc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 03:54:43.000000 jscc-0.2.1/jscc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 03:54:32.000000 jscc-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-15 03:54:43.819081 jscc-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:43.811081 jscc-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:43.811081 jscc-0.2.1/tests/cassettes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/cassettes/test_http_get_error.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/cassettes/test_http_head_error.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:43.811081 jscc-0.2.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/codelist.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:43.811081 jscc-0.2.1/tests/fixtures/csv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/csv/empty.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/csv/valid.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:43.815081 jscc-0.2.1/tests/fixtures/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/empty/empty-array.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/empty/empty-object.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/empty/empty-string.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/empty/false.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:43.815081 jscc-0.2.1/tests/fixtures/empty/htmlcov/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/empty/htmlcov/empty.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/empty/invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/empty/null.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/empty/whitespace-string.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/empty/whitespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/empty/whitespace.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/empty/zero-float.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/empty/zero-int.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:43.815081 jscc-0.2.1/tests/fixtures/indent/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/indent/ascii.json
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/indent/compact.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/indent/indented.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/indent/invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/indent/no-newline.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:43.815081 jscc-0.2.1/tests/fixtures/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/json/duplicate-key.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/json/invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/json/valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/meta-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/patch.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:43.819081 jscc-0.2.1/tests/fixtures/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/schema/array_items.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:43.819081 jscc-0.2.1/tests/fixtures/schema/build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/schema/build/ignore.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/schema/codelist_enum.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:54:43.819081 jscc-0.2.1/tests/fixtures/schema/codelists/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/schema/codelists/+nonexistent.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/schema/codelists/extra.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/schema/codelists/failClosedArray.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/schema/codelists/failClosedString.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/schema/codelists/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/schema/deep_properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/schema/items_type.json
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/schema/letter_case.json
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/schema/merge_properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/schema/metadata_presence.json
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/schema/null_type.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/schema/object_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/schema/ref.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/schema/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/fixtures/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12487 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-15 03:54:32.000000 jscc-0.2.1/tests/test_util.py
```

### Comparing `jscc-0.2.0/LICENSE` & `jscc-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jscc-0.2.0/PKG-INFO` & `jscc-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jscc
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tools for data standards that use JSON Schema and CSV codelists
 Home-page: https://github.com/open-contracting/jscc
 Author: Open Contracting Partnership and Open Data Services Co-operative Limited
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `jscc-0.2.0/README.rst` & `jscc-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `jscc-0.2.0/docs/Makefile` & `jscc-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jscc-0.2.0/docs/changelog.rst` & `jscc-0.2.1/docs/changelog.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+0.2.1 (2023-06-14)
+------------------
+
+Changed
+~~~~~~~
+
+-  :meth:`~jscc.testing.checks.validate_schema` no longer accepts a ``schema`` argument.
+
 0.2.0 (2023-06-14)
 ------------------
 
 Changed
 ~~~~~~~
 
 -  :meth:`~jscc.testing.checks.validate_schema` accepts a ``validator`` argument, instead of using JSON Schema Draft 4.
@@ -18,19 +26,17 @@
    to:
 
    .. code-block:: python
 
       from jsonschema import FormatChecker
       from jsonschema.validators import Draft4Validator
 
-      # Declare this at the module level, to minimize initializations.
-      validator = Draft4Validator(Draft4Validator.META_SCHEMA, format_checker=FormatChecker())
+      validator = Draft4Validator(schema, format_checker=FormatChecker())
 
-      # Meanwhile, elsewhere...
-      validate_schema(path, data, schema, validator)
+      validate_schema(path, data, validator)
 
 0.1.1 (2023-04-19)
 ------------------
 
 Changed
 ~~~~~~~
```

### Comparing `jscc-0.2.0/docs/conf.py` & `jscc-0.2.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "JSON Schema and CSV Codelists"
 copyright = "2020, Open Contracting Partnership and Open Data Services Co-operative Limited"
 author = "Open Contracting Partnership and Open Data Services Co-operative Limited"
 
 # The short X.Y version
-version = "0.2.0"
+version = "0.2.1"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `jscc-0.2.0/jscc/exceptions.py` & `jscc-0.2.1/jscc/exceptions.py`

 * *Files identical despite different names*

### Comparing `jscc-0.2.0/jscc/schema.py` & `jscc-0.2.1/jscc/schema.py`

 * *Files identical despite different names*

### Comparing `jscc-0.2.0/jscc/testing/checks.py` & `jscc-0.2.1/jscc/testing/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
    validator = Draft4Validator(Draft4Validator.META_SCHEMA, format_checker=FormatChecker())
 
 
    def validate_json_schema(path, name, data, schema):
        errors = 0
 
-       errors += validate_schema(path, data, schema, validator)
+       errors += validate_schema(path, data, validator)
        errors += validate_array_items(path, data)
        errors += validate_items_type(path, data)
        errors += validate_codelist_enum(path, data)
        errors += validate_letter_case(path, data)
        errors += validate_merge_properties(path, data)
        errors += validate_ref(path, data)
        errors += validate_metadata_presence(path, data)
@@ -230,21 +230,20 @@
             with open(path, newline='') as f:
                 try:
                     csv.DictReader(f)
                 except csv.Error as e:
                     yield path, e
 
 
-def validate_schema(path, data, schema, validator):
+def validate_schema(path, data, validator):
     """
     Warns and returns the number of errors relating to JSON Schema validation.
 
     Uses the `jsonschema <https://python-jsonschema.readthedocs.io/>`__ module.
 
-    :param object schema: the metaschema against which to validate
     :param validator: The validator to use
     :returns: the number of errors
     :rtype: int
     """
     errors = 0
 
     for error in validator.iter_errors(data):
```

### Comparing `jscc-0.2.0/jscc/testing/filesystem.py` & `jscc-0.2.1/jscc/testing/filesystem.py`

 * *Files identical despite different names*

### Comparing `jscc-0.2.0/jscc/testing/util.py` & `jscc-0.2.1/jscc/testing/util.py`

 * *Files identical despite different names*

### Comparing `jscc-0.2.0/jscc.egg-info/PKG-INFO` & `jscc-0.2.1/jscc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jscc
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tools for data standards that use JSON Schema and CSV codelists
 Home-page: https://github.com/open-contracting/jscc
 Author: Open Contracting Partnership and Open Data Services Co-operative Limited
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `jscc-0.2.0/jscc.egg-info/SOURCES.txt` & `jscc-0.2.1/jscc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jscc-0.2.0/setup.cfg` & `jscc-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jscc
-version = 0.2.0
+version = 0.2.1
 author = Open Contracting Partnership and Open Data Services Co-operative Limited
 author_email = data@open-contracting.org
 license = BSD
 description = Tools for data standards that use JSON Schema and CSV codelists
 url = https://github.com/open-contracting/jscc
 long_description = file: README.rst
 long_description_content_type = text/x-rst
```

### Comparing `jscc-0.2.0/tests/cassettes/test_http_get_error.yaml` & `jscc-0.2.1/tests/cassettes/test_http_get_error.yaml`

 * *Files identical despite different names*

### Comparing `jscc-0.2.0/tests/cassettes/test_http_head_error.yaml` & `jscc-0.2.1/tests/cassettes/test_http_head_error.yaml`

 * *Files identical despite different names*

### Comparing `jscc-0.2.0/tests/fixtures/meta-schema.json` & `jscc-0.2.1/tests/fixtures/meta-schema.json`

 * *Files identical despite different names*

### Comparing `jscc-0.2.0/tests/fixtures/schema/codelist_enum.json` & `jscc-0.2.1/tests/fixtures/schema/codelist_enum.json`

 * *Files identical despite different names*

### Comparing `jscc-0.2.0/tests/fixtures/schema/null_type.json` & `jscc-0.2.1/tests/fixtures/schema/null_type.json`

 * *Files identical despite different names*

### Comparing `jscc-0.2.0/tests/fixtures/schema/object_id.json` & `jscc-0.2.1/tests/fixtures/schema/object_id.json`

 * *Files identical despite different names*

### Comparing `jscc-0.2.0/tests/fixtures/schema.json` & `jscc-0.2.1/tests/fixtures/schema.json`

 * *Files identical despite different names*

### Comparing `jscc-0.2.0/tests/test_checks.py` & `jscc-0.2.1/tests/test_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,17 +256,17 @@
     assert sorted(str(record.message) for record in records) == [
         t("tests/fixtures/schema/ref.json has Error while resolving `#/definitions/Fail`: Unresolvable JSON pointer: '/definitions/Fail' at properties/fail"),  # noqa: E501
     ]
     assert errors == len(records) == 1
 
 
 def test_validate_schema():
-    validator = Draft4Validator(Draft4Validator.META_SCHEMA, format_checker=FormatChecker())
+    validator = Draft4Validator(parse('meta-schema.json'), format_checker=FormatChecker())
     with pytest.warns(UserWarning) as records:
-        errors = validate('schema', parse('meta-schema.json'), validator)
+        errors = validate('schema', validator)
 
     assert [str(record.message) for record in records] == [
         "[]\n[] is not of type 'object' (properties/properties/type)\n",
     ]
     assert errors == len(records) == 1
```

### Comparing `jscc-0.2.0/tests/test_schema.py` & `jscc-0.2.1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `jscc-0.2.0/tests/test_util.py` & `jscc-0.2.1/tests/test_util.py`

 * *Files identical despite different names*

