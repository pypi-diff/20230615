# Comparing `tmp/jscc-0.1.1.tar.gz` & `tmp/jscc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jscc-0.1.1.tar", last modified: Wed Apr 19 22:54:10 2023, max compression
+gzip compressed data, was "jscc-0.2.0.tar", last modified: Thu Jun 15 03:46:45 2023, max compression
```

## Comparing `jscc-0.1.1.tar` & `jscc-0.2.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.417623 jscc-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-19 22:54:01.000000 jscc-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-19 22:54:01.000000 jscc-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-19 22:54:10.417623 jscc-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-19 22:54:01.000000 jscc-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.405623 jscc-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.409623 jscc-0.1.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/api/schema.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.409623 jscc-0.1.1/docs/api/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/api/testing/checks.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/api/testing/filesystem.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/api/testing/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/api/testing/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 22:54:01.000000 jscc-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.409623 jscc-0.1.1/jscc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:01.000000 jscc-0.1.1/jscc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-19 22:54:01.000000 jscc-0.1.1/jscc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-04-19 22:54:01.000000 jscc-0.1.1/jscc/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.409623 jscc-0.1.1/jscc/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:01.000000 jscc-0.1.1/jscc/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31444 2023-04-19 22:54:01.000000 jscc-0.1.1/jscc/testing/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-19 22:54:01.000000 jscc-0.1.1/jscc/testing/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-19 22:54:01.000000 jscc-0.1.1/jscc/testing/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.409623 jscc-0.1.1/jscc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-19 22:54:10.000000 jscc-0.1.1/jscc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-19 22:54:10.000000 jscc-0.1.1/jscc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 22:54:10.000000 jscc-0.1.1/jscc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-19 22:54:10.000000 jscc-0.1.1/jscc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 22:54:10.000000 jscc-0.1.1/jscc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-19 22:54:01.000000 jscc-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-19 22:54:10.417623 jscc-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.409623 jscc-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.409623 jscc-0.1.1/tests/cassettes/
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/cassettes/test_http_get_error.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/cassettes/test_http_head_error.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.409623 jscc-0.1.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/codelist.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.409623 jscc-0.1.1/tests/fixtures/csv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/csv/empty.csv
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/csv/valid.csv
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.413623 jscc-0.1.1/tests/fixtures/empty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/empty-array.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/empty-object.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/empty-string.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/false.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.413623 jscc-0.1.1/tests/fixtures/empty/htmlcov/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/htmlcov/empty.txt
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/null.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/whitespace-string.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/whitespace.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/whitespace.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/zero-float.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/empty/zero-int.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.413623 jscc-0.1.1/tests/fixtures/indent/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/indent/ascii.json
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/indent/compact.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/indent/indented.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/indent/invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/indent/no-newline.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.413623 jscc-0.1.1/tests/fixtures/json/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/json/duplicate-key.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/json/invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/json/valid.json
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/meta-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/patch.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.413623 jscc-0.1.1/tests/fixtures/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/array_items.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.413623 jscc-0.1.1/tests/fixtures/schema/build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/build/ignore.json
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/codelist_enum.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:54:10.417623 jscc-0.1.1/tests/fixtures/schema/codelists/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/codelists/+nonexistent.csv
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/codelists/extra.csv
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/codelists/failClosedArray.csv
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/codelists/failClosedString.csv
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/codelists/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/deep_properties.json
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/items_type.json
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/letter_case.json
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/merge_properties.json
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/metadata_presence.json
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/null_type.json
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/object_id.json
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/ref.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/fixtures/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    12325 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-19 22:54:01.000000 jscc-0.1.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.161881 jscc-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-15 03:46:32.000000 jscc-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-15 03:46:32.000000 jscc-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-15 03:46:45.161881 jscc-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-15 03:46:32.000000 jscc-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.145881 jscc-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.145881 jscc-0.2.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/api/schema.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.145881 jscc-0.2.0/docs/api/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/api/testing/checks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/api/testing/filesystem.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/api/testing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/api/testing/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 03:46:32.000000 jscc-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.149881 jscc-0.2.0/jscc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:32.000000 jscc-0.2.0/jscc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-15 03:46:32.000000 jscc-0.2.0/jscc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-15 03:46:32.000000 jscc-0.2.0/jscc/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.149881 jscc-0.2.0/jscc/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:32.000000 jscc-0.2.0/jscc/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31563 2023-06-15 03:46:32.000000 jscc-0.2.0/jscc/testing/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-15 03:46:32.000000 jscc-0.2.0/jscc/testing/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-15 03:46:32.000000 jscc-0.2.0/jscc/testing/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.149881 jscc-0.2.0/jscc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-15 03:46:45.000000 jscc-0.2.0/jscc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-15 03:46:45.000000 jscc-0.2.0/jscc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 03:46:45.000000 jscc-0.2.0/jscc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-15 03:46:45.000000 jscc-0.2.0/jscc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 03:46:45.000000 jscc-0.2.0/jscc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 03:46:32.000000 jscc-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-15 03:46:45.161881 jscc-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.149881 jscc-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.149881 jscc-0.2.0/tests/cassettes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/cassettes/test_http_get_error.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/cassettes/test_http_head_error.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.153881 jscc-0.2.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/codelist.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.153881 jscc-0.2.0/tests/fixtures/csv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/csv/empty.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/csv/valid.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.153881 jscc-0.2.0/tests/fixtures/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/empty-array.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/empty-object.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/empty-string.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/false.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.153881 jscc-0.2.0/tests/fixtures/empty/htmlcov/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/htmlcov/empty.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/null.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/whitespace-string.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/whitespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/whitespace.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/zero-float.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/empty/zero-int.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.157881 jscc-0.2.0/tests/fixtures/indent/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/indent/ascii.json
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/indent/compact.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/indent/indented.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/indent/invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/indent/no-newline.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.157881 jscc-0.2.0/tests/fixtures/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/json/duplicate-key.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/json/invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/json/valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/meta-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/patch.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.157881 jscc-0.2.0/tests/fixtures/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/array_items.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.161881 jscc-0.2.0/tests/fixtures/schema/build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/build/ignore.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/codelist_enum.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:46:45.161881 jscc-0.2.0/tests/fixtures/schema/codelists/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/codelists/+nonexistent.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/codelists/extra.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/codelists/failClosedArray.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/codelists/failClosedString.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/codelists/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/deep_properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/items_type.json
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/letter_case.json
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/merge_properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/metadata_presence.json
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/null_type.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/object_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/ref.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/fixtures/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-15 03:46:32.000000 jscc-0.2.0/tests/test_util.py
```

### Comparing `jscc-0.1.1/LICENSE` & `jscc-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jscc-0.1.1/PKG-INFO` & `jscc-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jscc
-Version: 0.1.1
+Version: 0.2.0
 Summary: Tools for data standards that use JSON Schema and CSV codelists
 Home-page: https://github.com/open-contracting/jscc
 Author: Open Contracting Partnership and Open Data Services Co-operative Limited
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `jscc-0.1.1/README.rst` & `jscc-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `jscc-0.1.1/docs/Makefile` & `jscc-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jscc-0.1.1/docs/conf.py` & `jscc-0.2.0/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "JSON Schema and CSV Codelists"
 copyright = "2020, Open Contracting Partnership and Open Data Services Co-operative Limited"
 author = "Open Contracting Partnership and Open Data Services Co-operative Limited"
 
 # The short X.Y version
-version = "0.1.0"
+version = "0.2.0"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `jscc-0.1.1/jscc/exceptions.py` & `jscc-0.2.0/jscc/exceptions.py`

 * *Files identical despite different names*

### Comparing `jscc-0.1.1/jscc/schema.py` & `jscc-0.2.0/jscc/schema.py`

 * *Files identical despite different names*

### Comparing `jscc-0.1.1/jscc/testing/checks.py` & `jscc-0.2.0/jscc/testing/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,36 +22,50 @@
 
 You can edit ``metaschema`` to be more strict and/or to add new properties. Then, define the ``validate_json_schema``
 method that uses the ``validate_*`` methods. For example:
 
 .. code-block:: python
 
    import jsonref
-   from jscc.schema import (validate_array_items, validate_codelist_enum, validate_deep_properties,
-                            validate_items_type, validate_letter_case, validate_merge_properties,
-                            validate_metadata_presence, validate_null_type, validate_object_id, validate_ref,
-                            validate_schema)
+   from jscc.testing.checks import (
+       validate_array_items,
+       validate_codelist_enum,
+       validate_deep_properties,
+       validate_items_type,
+       validate_letter_case,
+       validate_merge_properties,
+       validate_metadata_presence,
+       validate_null_type,
+       validate_object_id,
+       validate_ref,
+       validate_schema,
+   )
+   from jsonschema import FormatChecker
+   from jsonschema.validators import Draft4Validator
+
+   validator = Draft4Validator(Draft4Validator.META_SCHEMA, format_checker=FormatChecker())
+
 
    def validate_json_schema(path, name, data, schema):
        errors = 0
 
-       errors += validate_schema(path, data, schema)
+       errors += validate_schema(path, data, schema, validator)
        errors += validate_array_items(path, data)
        errors += validate_items_type(path, data)
        errors += validate_codelist_enum(path, data)
        errors += validate_letter_case(path, data)
        errors += validate_merge_properties(path, data)
        errors += validate_ref(path, data)
        errors += validate_metadata_presence(path, data)
        errors += validate_object_id(path, jsonref.replace_refs(data))
        errors += validate_null_type(path, data)
        # Here, we don't add to `errors`, in order to not count these warnings as errors.
        validate_deep_properties(path, data)
 
-       assert not errors, 'One or more JSON Schema files are invalid. See warnings below.'
+       assert not errors, "One or more JSON Schema files are invalid. See warnings below."
 
 You can monkeypatch ``warnings.formatwarning`` to customize and abbreviate the warning messages:
 
 .. code-block:: python
 
    import os
    import warnings
@@ -76,16 +90,14 @@
 import csv
 import json
 import os
 import re
 from warnings import warn
 
 import jsonref
-from jsonschema import FormatChecker
-from jsonschema.validators import Draft4Validator as validator
 
 from jscc.exceptions import (CodelistEnumWarning, DeepPropertiesWarning, DuplicateKeyError, ItemsTypeWarning,
                              LetterCaseWarning, MergePropertiesWarning, MetadataPresenceWarning, NullTypeWarning,
                              ObjectIdWarning, RefWarning, SchemaCodelistsMatchWarning, SchemaWarning)
 from jscc.schema import get_types, is_array_of_objects, is_codelist, is_missing_property, rejecting_dict
 from jscc.testing.filesystem import tracked, walk, walk_csv_data, walk_json_data
 from jscc.testing.util import difference
@@ -218,27 +230,28 @@
             with open(path, newline='') as f:
                 try:
                     csv.DictReader(f)
                 except csv.Error as e:
                     yield path, e
 
 
-def validate_schema(path, data, schema):
+def validate_schema(path, data, schema, validator):
     """
     Warns and returns the number of errors relating to JSON Schema validation.
 
     Uses the `jsonschema <https://python-jsonschema.readthedocs.io/>`__ module.
 
     :param object schema: the metaschema against which to validate
+    :param validator: The validator to use
     :returns: the number of errors
     :rtype: int
     """
     errors = 0
 
-    for error in validator(schema, format_checker=FormatChecker()).iter_errors(data):
+    for error in validator.iter_errors(data):
         errors += 1
         warn(f"{json.dumps(error.instance, indent=2)}\n{error.message} ({'/'.join(error.absolute_schema_path)})\n",
              SchemaWarning)
 
     return errors
```

### Comparing `jscc-0.1.1/jscc/testing/filesystem.py` & `jscc-0.2.0/jscc/testing/filesystem.py`

 * *Files identical despite different names*

### Comparing `jscc-0.1.1/jscc/testing/util.py` & `jscc-0.2.0/jscc/testing/util.py`

 * *Files identical despite different names*

### Comparing `jscc-0.1.1/jscc.egg-info/PKG-INFO` & `jscc-0.2.0/jscc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jscc
-Version: 0.1.1
+Version: 0.2.0
 Summary: Tools for data standards that use JSON Schema and CSV codelists
 Home-page: https://github.com/open-contracting/jscc
 Author: Open Contracting Partnership and Open Data Services Co-operative Limited
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `jscc-0.1.1/jscc.egg-info/SOURCES.txt` & `jscc-0.2.0/jscc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jscc-0.1.1/setup.cfg` & `jscc-0.2.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jscc
-version = 0.1.1
+version = 0.2.0
 author = Open Contracting Partnership and Open Data Services Co-operative Limited
 author_email = data@open-contracting.org
 license = BSD
 description = Tools for data standards that use JSON Schema and CSV codelists
 url = https://github.com/open-contracting/jscc
 long_description = file: README.rst
 long_description_content_type = text/x-rst
@@ -20,27 +20,25 @@
 	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
 packages = find:
 install_requires = 
 	json-merge-patch
 	jsonref>=1
-	jsonschema
 	requests
-	rfc3339-validator
-	rfc3986-validator
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
 
 [options.extras_require]
 test = 
 	coveralls
+	jsonschema
 	pytest
 	pytest-cov
 	pytest-vcr
 docs = 
 	furo
 	sphinx
 	sphinx-autobuild
```

### Comparing `jscc-0.1.1/tests/cassettes/test_http_get_error.yaml` & `jscc-0.2.0/tests/cassettes/test_http_get_error.yaml`

 * *Files identical despite different names*

### Comparing `jscc-0.1.1/tests/cassettes/test_http_head_error.yaml` & `jscc-0.2.0/tests/cassettes/test_http_head_error.yaml`

 * *Files identical despite different names*

### Comparing `jscc-0.1.1/tests/fixtures/meta-schema.json` & `jscc-0.2.0/tests/fixtures/meta-schema.json`

 * *Files identical despite different names*

### Comparing `jscc-0.1.1/tests/fixtures/schema/codelist_enum.json` & `jscc-0.2.0/tests/fixtures/schema/codelist_enum.json`

 * *Files identical despite different names*

### Comparing `jscc-0.1.1/tests/fixtures/schema/null_type.json` & `jscc-0.2.0/tests/fixtures/schema/null_type.json`

 * *Files identical despite different names*

### Comparing `jscc-0.1.1/tests/fixtures/schema/object_id.json` & `jscc-0.2.0/tests/fixtures/schema/object_id.json`

 * *Files identical despite different names*

### Comparing `jscc-0.1.1/tests/fixtures/schema.json` & `jscc-0.2.0/tests/fixtures/schema.json`

 * *Files identical despite different names*

### Comparing `jscc-0.1.1/tests/test_checks.py` & `jscc-0.2.0/tests/test_checks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import contextlib
 import json
 import os
 import warnings
 
 import jsonref
 import pytest
+from jsonschema import FormatChecker
+from jsonschema.validators import Draft4Validator
 
 import jscc.testing.checks
 from jscc.exceptions import DuplicateKeyError
 from jscc.testing.checks import (get_empty_files, get_invalid_csv_files, get_invalid_json_files, get_misindented_files,
                                  validate_codelist_enum, validate_object_id, validate_ref,
                                  validate_schema_codelists_match)
 from tests import parse, path
@@ -254,16 +256,17 @@
     assert sorted(str(record.message) for record in records) == [
         t("tests/fixtures/schema/ref.json has Error while resolving `#/definitions/Fail`: Unresolvable JSON pointer: '/definitions/Fail' at properties/fail"),  # noqa: E501
     ]
     assert errors == len(records) == 1
 
 
 def test_validate_schema():
+    validator = Draft4Validator(Draft4Validator.META_SCHEMA, format_checker=FormatChecker())
     with pytest.warns(UserWarning) as records:
-        errors = validate('schema', parse('meta-schema.json'))
+        errors = validate('schema', parse('meta-schema.json'), validator)
 
     assert [str(record.message) for record in records] == [
         "[]\n[] is not of type 'object' (properties/properties/type)\n",
     ]
     assert errors == len(records) == 1
```

### Comparing `jscc-0.1.1/tests/test_schema.py` & `jscc-0.2.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `jscc-0.1.1/tests/test_util.py` & `jscc-0.2.0/tests/test_util.py`

 * *Files identical despite different names*

