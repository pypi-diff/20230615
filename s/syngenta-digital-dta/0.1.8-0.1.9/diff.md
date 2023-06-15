# Comparing `tmp/syngenta_digital_dta-0.1.8.tar.gz` & `tmp/syngenta_digital_dta-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/syngenta_digital_dta-0.1.8.tar", last modified: Wed Jun 14 16:11:19 2023, max compression
+gzip compressed data, was "dist/syngenta_digital_dta-0.1.9.tar", last modified: Thu Jun 15 16:38:16 2023, max compression
```

## Comparing `syngenta_digital_dta-0.1.8.tar` & `syngenta_digital_dta-0.1.9.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:19.870626 syngenta_digital_dta-0.1.8/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)    20885 2023-06-14 16:11:19.870626 syngenta_digital_dta-0.1.8/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    20114 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2023-06-14 16:11:19.870626 syngenta_digital_dta-0.1.8/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1199 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:19.862626 syngenta_digital_dta-0.1.8/syngenta_digital_dta/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2858 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:19.862626 syngenta_digital_dta-0.1.8/syngenta_digital_dta/common/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/common/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2616 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/common/base_adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1867 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/common/dict_merger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      290 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/common/json_helper.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      279 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/common/logger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      880 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/common/publisher.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      298 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/common/schema_loader.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1602 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/common/schema_mapper.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:19.862626 syngenta_digital_dta-0.1.8/syngenta_digital_dta/dynamodb/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/dynamodb/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5733 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/dynamodb/adapter.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:19.862626 syngenta_digital_dta-0.1.8/syngenta_digital_dta/elasticsearch/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/elasticsearch/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9053 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/elasticsearch/adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      402 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/elasticsearch/es_connection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1834 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/elasticsearch/es_connector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2548 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/elasticsearch/es_mapper.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:19.862626 syngenta_digital_dta-0.1.8/syngenta_digital_dta/file_system/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/file_system/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3122 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/file_system/adapter.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:19.862626 syngenta_digital_dta-0.1.8/syngenta_digital_dta/mongo/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/mongo/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5377 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/mongo/adapter.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:19.866626 syngenta_digital_dta-0.1.8/syngenta_digital_dta/postgres/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/postgres/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11758 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/postgres/adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2585 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/postgres/json_formatting.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      640 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/postgres/sql_connection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1127 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/postgres/sql_connector.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:19.866626 syngenta_digital_dta-0.1.8/syngenta_digital_dta/s3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/s3/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10287 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta/s3/adapter.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:19.862626 syngenta_digital_dta-0.1.8/syngenta_digital_dta.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    20885 2023-06-14 16:11:19.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2801 2023-06-14 16:11:19.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-14 16:11:19.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       83 2023-06-14 16:11:19.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2023-06-14 16:11:19.000000 syngenta_digital_dta-0.1.8/syngenta_digital_dta.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:19.866626 syngenta_digital_dta-0.1.8/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:19.866626 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:19.866626 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/common/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/common/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5690 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/common/test_base_adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1363 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/common/test_dict_merger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      628 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/common/test_publisher.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2126 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/common/test_schema_mapper.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:19.866626 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/dynamodb/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/dynamodb/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2598 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/dynamodb/mock_table.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12446 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/dynamodb/test_adapter.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:19.866626 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/elasticsearch/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/elasticsearch/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4440 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/elasticsearch/mocks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10020 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/elasticsearch/test_adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2056 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/elasticsearch/test_es_connector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2074 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/elasticsearch/test_es_mapper.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:19.866626 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/file_system/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/file_system/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3405 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/file_system/test_adapter.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:19.866626 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/mongo/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/mongo/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1441 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/mongo/mock_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6651 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/mongo/test_mongo.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:19.870626 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/postgres/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/postgres/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6675 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/postgres/test_json_formatting.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11884 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/postgres/test_postgres.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:19.870626 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/redshift/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/redshift/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10680 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/redshift/test_redshift.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:19.870626 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/s3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/s3/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8911 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/s3/test_s3.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3147 2023-06-14 16:11:06.000000 syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/test__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:38:16.706003 syngenta_digital_dta-0.1.9/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    20885 2023-06-15 16:38:16.706003 syngenta_digital_dta-0.1.9/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    20114 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2023-06-15 16:38:16.706003 syngenta_digital_dta-0.1.9/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1199 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:38:16.690003 syngenta_digital_dta-0.1.9/syngenta_digital_dta/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2858 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:38:16.694002 syngenta_digital_dta-0.1.9/syngenta_digital_dta/common/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/common/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2616 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/common/base_adapter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1867 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/common/dict_merger.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      290 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/common/json_helper.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      279 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/common/logger.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      880 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/common/publisher.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      298 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/common/schema_loader.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1602 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/common/schema_mapper.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:38:16.694002 syngenta_digital_dta-0.1.9/syngenta_digital_dta/dynamodb/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/dynamodb/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5733 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/dynamodb/adapter.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:38:16.694002 syngenta_digital_dta-0.1.9/syngenta_digital_dta/elasticsearch/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/elasticsearch/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9067 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/elasticsearch/adapter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      402 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/elasticsearch/es_connection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1834 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/elasticsearch/es_connector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2548 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/elasticsearch/es_mapper.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:38:16.694002 syngenta_digital_dta-0.1.9/syngenta_digital_dta/file_system/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/file_system/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3122 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/file_system/adapter.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:38:16.694002 syngenta_digital_dta-0.1.9/syngenta_digital_dta/mongo/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/mongo/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5377 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/mongo/adapter.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:38:16.698002 syngenta_digital_dta-0.1.9/syngenta_digital_dta/postgres/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/postgres/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11758 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/postgres/adapter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2585 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/postgres/json_formatting.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      640 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/postgres/sql_connection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1127 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/postgres/sql_connector.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:38:16.698002 syngenta_digital_dta-0.1.9/syngenta_digital_dta/s3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/s3/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10287 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta/s3/adapter.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:38:16.690003 syngenta_digital_dta-0.1.9/syngenta_digital_dta.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    20885 2023-06-15 16:38:16.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2801 2023-06-15 16:38:16.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-15 16:38:16.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       83 2023-06-15 16:38:16.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2023-06-15 16:38:16.000000 syngenta_digital_dta-0.1.9/syngenta_digital_dta.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:38:16.698002 syngenta_digital_dta-0.1.9/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:38:16.698002 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:38:16.698002 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/common/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/common/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5690 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/common/test_base_adapter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1363 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/common/test_dict_merger.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      628 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/common/test_publisher.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2126 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/common/test_schema_mapper.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:38:16.698002 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/dynamodb/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/dynamodb/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2598 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/dynamodb/mock_table.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12446 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/dynamodb/test_adapter.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:38:16.702003 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/elasticsearch/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/elasticsearch/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4440 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/elasticsearch/mocks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10020 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/elasticsearch/test_adapter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2056 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/elasticsearch/test_es_connector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2074 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/elasticsearch/test_es_mapper.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:38:16.702003 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/file_system/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/file_system/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3405 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/file_system/test_adapter.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:38:16.702003 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/mongo/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/mongo/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1441 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/mongo/mock_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6651 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/mongo/test_mongo.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:38:16.702003 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/postgres/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/postgres/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6675 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/postgres/test_json_formatting.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11884 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/postgres/test_postgres.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:38:16.702003 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/redshift/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/redshift/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10680 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/redshift/test_redshift.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:38:16.702003 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/s3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/s3/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8911 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/s3/test_s3.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3147 2023-06-15 16:37:46.000000 syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/test__init__.py
```

### Comparing `syngenta_digital_dta-0.1.8/LICENSE` & `syngenta_digital_dta-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/PKG-INFO` & `syngenta_digital_dta-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngenta_digital_dta
-Version: 0.1.8
+Version: 0.1.9
 Summary: A DRY multi-database normalizer.
 Home-page: https://github.com/syngenta-digital/package-python-dta.git
 Author: Paul Cruse III, Engineering Lead, Syngenta Digital
 Author-email: paul.cruse@syngenta.com
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
```

### Comparing `syngenta_digital_dta-0.1.8/README.md` & `syngenta_digital_dta-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/setup.py` & `syngenta_digital_dta-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/syngenta_digital_dta/__init__.py` & `syngenta_digital_dta-0.1.9/syngenta_digital_dta/__init__.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/syngenta_digital_dta/common/base_adapter.py` & `syngenta_digital_dta-0.1.9/syngenta_digital_dta/common/base_adapter.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/syngenta_digital_dta/common/dict_merger.py` & `syngenta_digital_dta-0.1.9/syngenta_digital_dta/common/dict_merger.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/syngenta_digital_dta/common/publisher.py` & `syngenta_digital_dta-0.1.9/syngenta_digital_dta/common/publisher.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/syngenta_digital_dta/common/schema_mapper.py` & `syngenta_digital_dta-0.1.9/syngenta_digital_dta/common/schema_mapper.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/syngenta_digital_dta/dynamodb/adapter.py` & `syngenta_digital_dta-0.1.9/syngenta_digital_dta/dynamodb/adapter.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/syngenta_digital_dta/elasticsearch/adapter.py` & `syngenta_digital_dta-0.1.9/syngenta_digital_dta/elasticsearch/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         )
         super().publish('overwrite', data, **kwargs)
         return response
 
     def upsert(self, **kwargs):
         operation = kwargs.get('operation', 'update')
 
-        if self.connection.exists(index=self.index, id=kwargs['data'][self.model_identifier]):
+        if self.connection.exists(index=self.index, id=kwargs['data'][self.model_identifier], refresh=True):
             if operation == 'update':
                 return self.update(**kwargs)
 
             if operation == 'overwrite':
                 return self.overwrite(**kwargs)
 
             raise Exception(f'Input operation "{operation}" not supported!')
```

### Comparing `syngenta_digital_dta-0.1.8/syngenta_digital_dta/elasticsearch/es_connector.py` & `syngenta_digital_dta-0.1.9/syngenta_digital_dta/elasticsearch/es_connector.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/syngenta_digital_dta/elasticsearch/es_mapper.py` & `syngenta_digital_dta-0.1.9/syngenta_digital_dta/elasticsearch/es_mapper.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/syngenta_digital_dta/file_system/adapter.py` & `syngenta_digital_dta-0.1.9/syngenta_digital_dta/file_system/adapter.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/syngenta_digital_dta/mongo/adapter.py` & `syngenta_digital_dta-0.1.9/syngenta_digital_dta/mongo/adapter.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/syngenta_digital_dta/postgres/adapter.py` & `syngenta_digital_dta-0.1.9/syngenta_digital_dta/postgres/adapter.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/syngenta_digital_dta/postgres/json_formatting.py` & `syngenta_digital_dta-0.1.9/syngenta_digital_dta/postgres/json_formatting.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/syngenta_digital_dta/postgres/sql_connection.py` & `syngenta_digital_dta-0.1.9/syngenta_digital_dta/postgres/sql_connection.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/syngenta_digital_dta/postgres/sql_connector.py` & `syngenta_digital_dta-0.1.9/syngenta_digital_dta/postgres/sql_connector.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/syngenta_digital_dta/s3/adapter.py` & `syngenta_digital_dta-0.1.9/syngenta_digital_dta/s3/adapter.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/syngenta_digital_dta.egg-info/PKG-INFO` & `syngenta_digital_dta-0.1.9/syngenta_digital_dta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngenta-digital-dta
-Version: 0.1.8
+Version: 0.1.9
 Summary: A DRY multi-database normalizer.
 Home-page: https://github.com/syngenta-digital/package-python-dta.git
 Author: Paul Cruse III, Engineering Lead, Syngenta Digital
 Author-email: paul.cruse@syngenta.com
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
```

### Comparing `syngenta_digital_dta-0.1.8/syngenta_digital_dta.egg-info/SOURCES.txt` & `syngenta_digital_dta-0.1.9/syngenta_digital_dta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/common/test_base_adapter.py` & `syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/common/test_base_adapter.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/common/test_dict_merger.py` & `syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/common/test_dict_merger.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/common/test_publisher.py` & `syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/common/test_publisher.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/common/test_schema_mapper.py` & `syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/common/test_schema_mapper.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/dynamodb/mock_table.py` & `syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/dynamodb/mock_table.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/dynamodb/test_adapter.py` & `syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/dynamodb/test_adapter.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/elasticsearch/mocks.py` & `syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/elasticsearch/mocks.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/elasticsearch/test_adapter.py` & `syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/elasticsearch/test_adapter.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/elasticsearch/test_es_connector.py` & `syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/elasticsearch/test_es_connector.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/elasticsearch/test_es_mapper.py` & `syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/elasticsearch/test_es_mapper.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/file_system/test_adapter.py` & `syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/file_system/test_adapter.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/mongo/mock_data.py` & `syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/mongo/mock_data.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/mongo/test_mongo.py` & `syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/mongo/test_mongo.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/postgres/test_json_formatting.py` & `syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/postgres/test_json_formatting.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/postgres/test_postgres.py` & `syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/postgres/test_postgres.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/redshift/test_redshift.py` & `syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/redshift/test_redshift.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/s3/test_s3.py` & `syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/s3/test_s3.py`

 * *Files identical despite different names*

### Comparing `syngenta_digital_dta-0.1.8/tests/syngenta_digital_dta/test__init__.py` & `syngenta_digital_dta-0.1.9/tests/syngenta_digital_dta/test__init__.py`

 * *Files identical despite different names*

