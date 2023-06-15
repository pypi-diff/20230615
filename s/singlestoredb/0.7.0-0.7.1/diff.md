# Comparing `tmp/singlestoredb-0.7.0.tar.gz` & `tmp/singlestoredb-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singlestoredb-0.7.0.tar", last modified: Fri Jun  9 20:35:47 2023, max compression
+gzip compressed data, was "singlestoredb-0.7.1.tar", last modified: Thu Jun 15 18:35:43 2023, max compression
```

## Comparing `singlestoredb-0.7.0.tar` & `singlestoredb-0.7.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.335817 singlestoredb-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11341 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     7340 2023-06-09 20:35:47.335817 singlestoredb-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6299 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     2055 2023-06-09 20:35:47.335817 singlestoredb-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.323817 singlestoredb-0.7.0/singlestoredb/
--rw-r--r--   0 runner    (1001) docker     (122)      842 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7599 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     5914 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    43133 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/connection.py
--rw-r--r--   0 runner    (1001) docker     (122)    12515 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/converters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2459 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.323817 singlestoredb-0.7.0/singlestoredb/http/
--rw-r--r--   0 runner    (1001) docker     (122)      912 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    29142 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/http/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.327817 singlestoredb-0.7.0/singlestoredb/management/
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14097 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/management/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     6501 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/management/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/management/region.py
--rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/management/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    18491 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/management/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.327817 singlestoredb-0.7.0/singlestoredb/mysql/
--rw-r--r--   0 runner    (1001) docker     (122)     4363 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7985 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)    57359 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/accel.c
--rw-r--r--   0 runner    (1001) docker     (122)    10324 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/charset.py
--rw-r--r--   0 runner    (1001) docker     (122)    58819 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.327817 singlestoredb-0.7.0/singlestoredb/mysql/constants/
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/constants/CLIENT.py
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/constants/COMMAND.py
--rw-r--r--   0 runner    (1001) docker     (122)     2335 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/constants/CR.py
--rw-r--r--   0 runner    (1001) docker     (122)    12311 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/constants/ER.py
--rw-r--r--   0 runner    (1001) docker     (122)      385 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/constants/FIELD_TYPE.py
--rw-r--r--   0 runner    (1001) docker     (122)      229 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/constants/FLAG.py
--rw-r--r--   0 runner    (1001) docker     (122)      348 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/constants/SERVER_STATUS.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5630 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/converters.py
--rw-r--r--   0 runner    (1001) docker     (122)    21092 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/cursors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/err.py
--rw-r--r--   0 runner    (1001) docker     (122)      589 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/optionfile.py
--rw-r--r--   0 runner    (1001) docker     (122)    12081 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.331817 singlestoredb-0.7.0/singlestoredb/mysql/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      997 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4025 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_DictCursor.py
--rw-r--r--   0 runner    (1001) docker     (122)     4306 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_SSCursor.py
--rw-r--r--   0 runner    (1001) docker     (122)    15465 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (122)    32297 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (122)     5045 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_cursor.py
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_err.py
--rw-r--r--   0 runner    (1001) docker     (122)    18965 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_issues.py
--rw-r--r--   0 runner    (1001) docker     (122)     2502 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_load_local.py
--rw-r--r--   0 runner    (1001) docker     (122)     2725 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_nextset.py
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/test_optionfile.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.331817 singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.331817 singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10171 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (122)    31414 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (122)     8022 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (122)     2819 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
--rw-r--r--   0 runner    (1001) docker     (122)      435 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/mysql/times.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.331817 singlestoredb-0.7.0/singlestoredb/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/empty.sql
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/local_infile.csv
--rw-r--r--   0 runner    (1001) docker     (122)     8968 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test.sql
--rwxr-xr-x   0 runner    (1001) docker     (122)    40220 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test_basics.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11184 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    49962 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)      652 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test_dbapi.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1131 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test_exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     8580 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test_http.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     9721 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test_management.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6582 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test_results.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4500 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test_types.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    10408 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/test_xdict.py
--rw-r--r--   0 runner    (1001) docker     (122)     4673 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9969 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.335817 singlestoredb-0.7.0/singlestoredb/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24503 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/utils/convert_rows.py
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (122)     5204 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/utils/results.py
--rw-r--r--   0 runner    (1001) docker     (122)    12896 2023-06-09 20:35:21.000000 singlestoredb-0.7.0/singlestoredb/utils/xdict.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 20:35:47.323817 singlestoredb-0.7.0/singlestoredb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7340 2023-06-09 20:35:47.000000 singlestoredb-0.7.0/singlestoredb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3095 2023-06-09 20:35:47.000000 singlestoredb-0.7.0/singlestoredb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 20:35:47.000000 singlestoredb-0.7.0/singlestoredb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-06-09 20:35:47.000000 singlestoredb-0.7.0/singlestoredb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-06-09 20:35:47.000000 singlestoredb-0.7.0/singlestoredb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.492792 singlestoredb-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    11341 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     7340 2023-06-15 18:35:43.492792 singlestoredb-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6299 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2055 2023-06-15 18:35:43.492792 singlestoredb-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.484792 singlestoredb-0.7.1/singlestoredb/
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7599 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6314 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43470 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12515 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2459 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.484792 singlestoredb-0.7.1/singlestoredb/http/
+-rw-r--r--   0 runner    (1001) docker     (122)      912 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29448 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/http/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.484792 singlestoredb-0.7.1/singlestoredb/management/
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14097 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/management/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6501 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/management/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/management/region.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/management/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18491 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/management/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.484792 singlestoredb-0.7.1/singlestoredb/mysql/
+-rw-r--r--   0 runner    (1001) docker     (122)     4363 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7985 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57359 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/accel.c
+-rw-r--r--   0 runner    (1001) docker     (122)    10324 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/charset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58930 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.488792 singlestoredb-0.7.1/singlestoredb/mysql/constants/
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/constants/CLIENT.py
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/constants/COMMAND.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2335 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/constants/CR.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12311 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/constants/ER.py
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/constants/FIELD_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (122)      229 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/constants/FLAG.py
+-rw-r--r--   0 runner    (1001) docker     (122)      348 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/constants/SERVER_STATUS.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5630 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21092 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/cursors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/err.py
+-rw-r--r--   0 runner    (1001) docker     (122)      589 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/optionfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12081 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.488792 singlestoredb-0.7.1/singlestoredb/mysql/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      997 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4025 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_DictCursor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4306 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_SSCursor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15465 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32297 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5045 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_err.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18965 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_issues.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2502 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_load_local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2725 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_nextset.py
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_optionfile.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.488792 singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.488792 singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10171 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31414 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8022 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2819 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/times.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.492792 singlestoredb-0.7.1/singlestoredb/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/empty.sql
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/local_infile.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     8968 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test.sql
+-rwxr-xr-x   0 runner    (1001) docker     (122)    40220 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test_basics.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11184 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    50732 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test_dbapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1131 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test_exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8580 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test_http.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     9721 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test_management.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6582 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test_results.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4500 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test_types.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10408 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test_xdict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4673 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9969 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.492792 singlestoredb-0.7.1/singlestoredb/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24503 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/utils/convert_rows.py
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5204 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/utils/results.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12896 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/utils/xdict.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.484792 singlestoredb-0.7.1/singlestoredb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7340 2023-06-15 18:35:43.000000 singlestoredb-0.7.1/singlestoredb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3095 2023-06-15 18:35:43.000000 singlestoredb-0.7.1/singlestoredb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 18:35:43.000000 singlestoredb-0.7.1/singlestoredb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-06-15 18:35:43.000000 singlestoredb-0.7.1/singlestoredb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-06-15 18:35:43.000000 singlestoredb-0.7.1/singlestoredb.egg-info/top_level.txt
```

### Comparing `singlestoredb-0.7.0/LICENSE` & `singlestoredb-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/PKG-INFO` & `singlestoredb-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singlestoredb
-Version: 0.7.0
+Version: 0.7.1
 Summary: Interface to the SingleStore database and cluster management APIs
 Home-page: https://github.com/singlestore-labs/singlestoredb-python
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `singlestoredb-0.7.0/README.md` & `singlestoredb-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/setup.cfg` & `singlestoredb-0.7.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = singlestoredb
-version = 0.7.0
+version = 0.7.1
 description = Interface to the SingleStore database and cluster management APIs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/singlestore-labs/singlestoredb-python
 author = SingleStore
 author_email = support@singlestore.com
 license = Apache-2.0
```

### Comparing `singlestoredb-0.7.0/setup.py` & `singlestoredb-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/__init__.py` & `singlestoredb-0.7.1/singlestoredb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 >>> cur = conn.cursor()
 >>> cur.execute('select * from customers')
 >>> for row in cur:
 ...     print(row)
 
 """
 
-__version__ = '0.7.0'
+__version__ = '0.7.1'
 
 from .config import options, get_option, set_option, describe_option
 from .connection import connect, apilevel, threadsafety, paramstyle
 from .exceptions import (
     Warning, Error, InterfaceError, DatabaseError, OperationalError,
     IntegrityError, InternalError, ProgrammingError, NotSupportedError,
     DataError, ManagementError,
```

### Comparing `singlestoredb-0.7.0/singlestoredb/auth.py` & `singlestoredb-0.7.1/singlestoredb/auth.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/config.py` & `singlestoredb-0.7.1/singlestoredb/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,20 @@
 register_option(
     'local_infile', 'bool', check_bool, False,
     'Should it be possible to load local files?',
     environ='SINGLESTOREDB_LOCAL_INFILE',
 )
 
 register_option(
+    'multi_statements', 'bool', check_bool, False,
+    'Should it be possible use multiple statements in one query?',
+    environ='SINGLESTOREDB_MULTI_STATEMENTS',
+)
+
+register_option(
     'ssl_key', 'str', check_str, None,
     'File containing SSL key',
     environ='SINGLESTOREDB_SSL_KEY',
 )
 
 register_option(
     'ssl_cert', 'str', check_str, None,
@@ -171,14 +177,21 @@
 
 register_option(
     'buffered', 'bool', check_bool, True,
     'Should query results be buffered before processing?',
     environ='SINGLESTOREDB_BUFFERED',
 )
 
+register_option(
+    'connect_timeout', 'int', check_int, 10,
+    'The timeout for connecting to the database in seconds. '
+    '(default: 10, min: 1, max: 31536000)',
+    environ='SINGLESTOREDB_CONNECT_TIMEOUT',
+)
+
 #
 # Query results options
 #
 register_option(
     'results.type', 'string',
     functools.partial(
         check_str,
```

### Comparing `singlestoredb-0.7.0/singlestoredb/connection.py` & `singlestoredb-0.7.1/singlestoredb/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1272,14 +1272,16 @@
     credential_type: Optional[str] = None,
     autocommit: Optional[bool] = None,
     results_type: Optional[str] = None,
     buffered: Optional[bool] = None,
     results_format: Optional[str] = None,
     program_name: Optional[str] = None,
     conn_attrs: Optional[Dict[str, str]] = None,
+    multi_statements: Optional[bool] = None,
+    connect_timeout: Optional[int] = None,
 ) -> Connection:
     """
     Return a SingleStoreDB connection.
 
     Parameters
     ----------
     host : str, optional
@@ -1333,14 +1335,19 @@
     results_format : str, optional
         Deprecated. This option has been renamed to results_type.
     program_name: str, optional
         Name of the program
     conn_attrs: dict, optional
         Additional connection attributes for telemetry. Example:
         {'program_version': "1.0.2", "_connector_name": "dbt connector"}
+    multi_statements: bool, optional
+        Should multiple statements be allowed within a single query?
+    connect_timeout: int, optional
+        The timeout for connecting to the database in seconds.
+        (default: 10, min: 1, max: 31536000)
 
     Examples
     --------
     Standard database connection
 
     >>> conn = s2.connect('me:p455w0rd@s2-host.com/my_db')
```

### Comparing `singlestoredb-0.7.0/singlestoredb/converters.py` & `singlestoredb-0.7.1/singlestoredb/converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/exceptions.py` & `singlestoredb-0.7.1/singlestoredb/exceptions.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/http/__init__.py` & `singlestoredb-0.7.1/singlestoredb/http/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/http/connection.py` & `singlestoredb-0.7.1/singlestoredb/http/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -805,14 +805,20 @@
             if ssl_ca:
                 self._sess.verify = ssl_ca
 
             ssl_verify_cert = kwargs.get('ssl_verify_cert', True)
             if not ssl_verify_cert:
                 self._sess.verify = False
 
+        if kwargs.get('multi_statements', False):
+            raise self.InterfaceError(
+                0, 'The Data API does not allow multiple '
+                'statements within a query',
+            )
+
         version = kwargs.get('version', 'v2')
         self.driver = kwargs.get('driver', 'https')
 
         self._database = kwargs.get('database', get_option('database'))
         self._url = f'{self.driver}://{host}:{port}/api/{version}/'
         self._messages: List[Tuple[int, str]] = []
         self._autocommit: bool = True
@@ -842,14 +848,16 @@
         Returns
         -------
         requests.Response
 
         """
         if self._sess is None:
             raise InterfaceError(errno=2048, msg='Connection is closed.')
+        if 'timeout' not in kwargs:
+            kwargs['timeout'] = get_option('connect_timeout')
         return self._sess.post(urljoin(self._url, path), *args, **kwargs)
 
     def close(self) -> None:
         """Close the connection."""
         if self._sess is None:
             raise Error(errno=2048, msg='Connection is closed')
         self._sess = None
```

### Comparing `singlestoredb-0.7.0/singlestoredb/management/cluster.py` & `singlestoredb-0.7.1/singlestoredb/management/cluster.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/management/manager.py` & `singlestoredb-0.7.1/singlestoredb/management/manager.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/management/region.py` & `singlestoredb-0.7.1/singlestoredb/management/region.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/management/utils.py` & `singlestoredb-0.7.1/singlestoredb/management/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/management/workspace.py` & `singlestoredb-0.7.1/singlestoredb/management/workspace.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/__init__.py` & `singlestoredb-0.7.1/singlestoredb/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/_auth.py` & `singlestoredb-0.7.1/singlestoredb/mysql/_auth.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/accel.c` & `singlestoredb-0.7.1/singlestoredb/mysql/accel.c`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/charset.py` & `singlestoredb-0.7.1/singlestoredb/mysql/charset.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/connection.py` & `singlestoredb-0.7.1/singlestoredb/mysql/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,14 +288,15 @@
         results_type='tuples',
         compress=None,  # not supported
         named_pipe=None,  # not supported
         passwd=None,  # deprecated
         db=None,  # deprecated
         driver=None,  # internal use
         conn_attrs=None,
+        multi_statements=None,
     ):
         BaseConnection.__init__(**dict(locals()))
 
         if db is not None and database is None:
             # We will raise warning in 2022 or later.
             # See https://github.com/PyMySQL/PyMySQL/issues/939
             # warnings.warn("'db' is deprecated, use 'database'", DeprecationWarning, 3)
@@ -312,14 +313,16 @@
             raise NotImplementedError(
                 'compress and named_pipe arguments are not supported',
             )
 
         self._local_infile = bool(local_infile)
         if self._local_infile:
             client_flag |= CLIENT.LOCAL_FILES
+        if multi_statements:
+            client_flag |= CLIENT.MULTI_STATEMENTS
 
         if read_default_group and not read_default_file:
             if sys.platform.startswith('win'):
                 read_default_file = 'c:\\my.ini'
             else:
                 read_default_file = '/etc/my.cnf'
```

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/constants/CLIENT.py` & `singlestoredb-0.7.1/singlestoredb/mysql/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/constants/COMMAND.py` & `singlestoredb-0.7.1/singlestoredb/mysql/constants/COMMAND.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/constants/CR.py` & `singlestoredb-0.7.1/singlestoredb/mysql/constants/CR.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/constants/ER.py` & `singlestoredb-0.7.1/singlestoredb/mysql/constants/ER.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/converters.py` & `singlestoredb-0.7.1/singlestoredb/mysql/converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/cursors.py` & `singlestoredb-0.7.1/singlestoredb/mysql/cursors.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/err.py` & `singlestoredb-0.7.1/singlestoredb/mysql/err.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/optionfile.py` & `singlestoredb-0.7.1/singlestoredb/mysql/optionfile.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/protocol.py` & `singlestoredb-0.7.1/singlestoredb/mysql/protocol.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/tests/__init__.py` & `singlestoredb-0.7.1/singlestoredb/mysql/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/tests/base.py` & `singlestoredb-0.7.1/singlestoredb/mysql/tests/base.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/tests/conftest.py` & `singlestoredb-0.7.1/singlestoredb/mysql/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/tests/test_DictCursor.py` & `singlestoredb-0.7.1/singlestoredb/mysql/tests/test_DictCursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/tests/test_SSCursor.py` & `singlestoredb-0.7.1/singlestoredb/mysql/tests/test_SSCursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/tests/test_basic.py` & `singlestoredb-0.7.1/singlestoredb/mysql/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/tests/test_connection.py` & `singlestoredb-0.7.1/singlestoredb/mysql/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/tests/test_converters.py` & `singlestoredb-0.7.1/singlestoredb/mysql/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/tests/test_cursor.py` & `singlestoredb-0.7.1/singlestoredb/mysql/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/tests/test_issues.py` & `singlestoredb-0.7.1/singlestoredb/mysql/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/tests/test_load_local.py` & `singlestoredb-0.7.1/singlestoredb/mysql/tests/test_load_local.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/tests/test_nextset.py` & `singlestoredb-0.7.1/singlestoredb/mysql/tests/test_nextset.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/tests/test_optionfile.py` & `singlestoredb-0.7.1/singlestoredb/mysql/tests/test_optionfile.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py` & `singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py` & `singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py` & `singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py` & `singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py` & `singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/tests/test.sql` & `singlestoredb-0.7.1/singlestoredb/tests/test.sql`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/tests/test_basics.py` & `singlestoredb-0.7.1/singlestoredb/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/tests/test_config.py` & `singlestoredb-0.7.1/singlestoredb/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/tests/test_connection.py` & `singlestoredb-0.7.1/singlestoredb/tests/test_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1353,14 +1353,33 @@
         with self.assertWarns(DeprecationWarning):
             with s2.connect(database=type(self).dbname, results_format='dicts') as conn:
                 with conn.cursor() as cur:
                     cur.execute('select * from alltypes')
                     out = cur.fetchall()
                     assert type(out[0]) is dict, type(out)
 
+    def test_multi_statements(self):
+        if self.conn.driver not in ['http', 'https']:
+            with s2.connect(database=type(self).dbname, multi_statements=True) as conn:
+                with conn.cursor() as cur:
+                    cur.execute('SELECT 1; SELECT 2;')
+                    self.assertEqual([(1,)], list(cur))
+
+                    r = cur.nextset()
+                    self.assertTrue(r)
+
+                    self.assertEqual([(2,)], list(cur))
+                    self.assertIsNone(cur.nextset())
+
+    def test_connect_timeout(self):
+        with s2.connect(database=type(self).dbname, connect_timeout=8) as conn:
+            with conn.cursor() as cur:
+                cur.execute('SELECT 1')
+                self.assertEqual([(1,)], list(cur))
+
     def test_show_accessors(self):
         out = self.conn.show.columns('data')
         assert out.columns == [
             'Name', 'Type', 'Null',
             'Key', 'Default', 'Extra',
         ], out.columns
         assert out.Name == ['id', 'name', 'value'], out.Name
```

### Comparing `singlestoredb-0.7.0/singlestoredb/tests/test_dbapi.py` & `singlestoredb-0.7.1/singlestoredb/tests/test_dbapi.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/tests/test_exceptions.py` & `singlestoredb-0.7.1/singlestoredb/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/tests/test_http.py` & `singlestoredb-0.7.1/singlestoredb/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/tests/test_management.py` & `singlestoredb-0.7.1/singlestoredb/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/tests/test_results.py` & `singlestoredb-0.7.1/singlestoredb/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/tests/test_types.py` & `singlestoredb-0.7.1/singlestoredb/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/tests/test_xdict.py` & `singlestoredb-0.7.1/singlestoredb/tests/test_xdict.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/tests/utils.py` & `singlestoredb-0.7.1/singlestoredb/tests/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/types.py` & `singlestoredb-0.7.1/singlestoredb/types.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/utils/config.py` & `singlestoredb-0.7.1/singlestoredb/utils/config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/utils/convert_rows.py` & `singlestoredb-0.7.1/singlestoredb/utils/convert_rows.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/utils/results.py` & `singlestoredb-0.7.1/singlestoredb/utils/results.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb/utils/xdict.py` & `singlestoredb-0.7.1/singlestoredb/utils/xdict.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.0/singlestoredb.egg-info/PKG-INFO` & `singlestoredb-0.7.1/singlestoredb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singlestoredb
-Version: 0.7.0
+Version: 0.7.1
 Summary: Interface to the SingleStore database and cluster management APIs
 Home-page: https://github.com/singlestore-labs/singlestoredb-python
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `singlestoredb-0.7.0/singlestoredb.egg-info/SOURCES.txt` & `singlestoredb-0.7.1/singlestoredb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

