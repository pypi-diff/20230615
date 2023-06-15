# Comparing `tmp/dagster-aws-0.9.9.tar.gz` & `tmp/dagster-aws-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-aws-0.9.9.tar", last modified: Thu Sep 17 21:27:59 2020, max compression
+gzip compressed data, was "dist/dagster-aws-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:21 2020, max compression
```

## Comparing `dagster-aws-0.9.9.tar` & `dagster-aws-0.9.9rc1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)      165 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      629 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      119 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws/
--rw-r--r--   0 bobchen    (501) staff       (20)      154 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws/cloudwatch/
--rw-r--r--   0 bobchen    (501) staff       (20)       39 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/cloudwatch/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     9246 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/cloudwatch/loggers.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws/ecs/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/ecs/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     9702 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/ecs/client.py
--rw-r--r--   0 bobchen    (501) staff       (20)     6841 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/ecs/launcher.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws/emr/
--rw-r--r--   0 bobchen    (501) staff       (20)      227 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/emr/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    51135 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/emr/configs.py
--rw-r--r--   0 bobchen    (501) staff       (20)    16339 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/emr/emr.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2956 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/emr/emr_step_main.py
--rw-r--r--   0 bobchen    (501) staff       (20)      489 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/emr/main.py.template
--rw-r--r--   0 bobchen    (501) staff       (20)    13976 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/emr/pyspark_step_launcher.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3633 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/emr/types.py
--rw-r--r--   0 bobchen    (501) staff       (20)      602 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/emr/utils.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws/redshift/
--rw-r--r--   0 bobchen    (501) staff       (20)      145 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/redshift/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)    16518 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/redshift/resources.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws/s3/
--rw-r--r--   0 bobchen    (501) staff       (20)      622 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/s3/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     7595 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/s3/compute_log_manager.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1788 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/s3/file_cache.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3216 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/s3/file_manager.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1270 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/s3/intermediate_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)     5183 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/s3/object_store.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4213 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/s3/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2344 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/s3/s3_fake_resource.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2411 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/s3/solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4660 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/s3/system_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)      689 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/s3/utils.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws/utils/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/utils/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws/utils/mrjob/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/utils/mrjob/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4449 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/utils/mrjob/log4j.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4843 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/utils/mrjob/retry.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3589 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/utils/mrjob/utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      629 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)     2610 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       71 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       30 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws_tests/cloudwatch_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/cloudwatch_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      665 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/cloudwatch_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3586 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/cloudwatch_tests/test_loggers.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws_tests/ecs_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/ecs_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     5302 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/ecs_tests/test_ecs_client.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws_tests/emr_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/emr_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1120 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/emr_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)     7576 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/emr_tests/test_emr.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2152 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/emr_tests/test_emr_step_main.py
--rw-r--r--   0 bobchen    (501) staff       (20)     7699 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/emr_tests/test_pyspark.py
--rw-r--r--   0 bobchen    (501) staff       (20)      958 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/emr_tests/test_pyspark_step_launcher.py
--rw-r--r--   0 bobchen    (501) staff       (20)      760 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/emr_tests/test_utils.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws_tests/redshift_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/redshift_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      102 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/redshift_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)     6642 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/redshift_tests/test_resources.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws_tests/s3_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/s3_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      102 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/s3_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4218 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/s3_tests/test_compute_log_manager.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1722 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/s3_tests/test_file_handle_to_s3.py
--rw-r--r--   0 bobchen    (501) staff       (20)    15946 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/s3_tests/test_intermediate_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1052 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/s3_tests/test_object_store.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1441 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/s3_tests/test_s3_file_cache.py
--rw-r--r--   0 bobchen    (501) staff       (20)     7083 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/s3_tests/test_s3_file_manager.py
--rw-r--r--   0 bobchen    (501) staff       (20)       89 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/test_version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws_tests/utils_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/utils_tests/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/dagster_aws_tests/utils_tests/mrjob_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/utils_tests/mrjob_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3840 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/utils_tests/mrjob_tests/test_log4j.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2410 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/dagster_aws_tests/utils_tests/mrjob_tests/test_utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:27:59.000000 dagster-aws-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1184 2020-09-17 21:24:45.000000 dagster-aws-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/LICENSE
+-rw-r--r--   0 bobchen    (501) staff       (20)      165 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/MANIFEST.in
+-rw-r--r--   0 bobchen    (501) staff       (20)      632 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      119 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws/
+-rw-r--r--   0 bobchen    (501) staff       (20)      154 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/__init__.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws/cloudwatch/
+-rw-r--r--   0 bobchen    (501) staff       (20)       39 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/cloudwatch/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     9246 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/cloudwatch/loggers.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws/ecs/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/ecs/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     9702 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/ecs/client.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     6841 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/ecs/launcher.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws/emr/
+-rw-r--r--   0 bobchen    (501) staff       (20)      227 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/emr/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    51135 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/emr/configs.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    16339 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/emr/emr.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2956 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/emr/emr_step_main.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      489 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/emr/main.py.template
+-rw-r--r--   0 bobchen    (501) staff       (20)    13976 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/emr/pyspark_step_launcher.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     3633 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/emr/types.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      602 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/emr/utils.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws/redshift/
+-rw-r--r--   0 bobchen    (501) staff       (20)      145 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/redshift/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    16518 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/redshift/resources.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/
+-rw-r--r--   0 bobchen    (501) staff       (20)      622 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     7595 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/compute_log_manager.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1788 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/file_cache.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     3216 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/file_manager.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1270 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/intermediate_storage.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     5183 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/object_store.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     4213 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2344 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/s3_fake_resource.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2411 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/solids.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     4660 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/system_storage.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      689 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/s3/utils.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws/utils/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/utils/__init__.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws/utils/mrjob/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/utils/mrjob/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     4449 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/utils/mrjob/log4j.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     4843 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/utils/mrjob/retry.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     3589 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/utils/mrjob/utils.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      632 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)     2610 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)       71 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       30 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/__init__.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/cloudwatch_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/cloudwatch_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      665 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/cloudwatch_tests/conftest.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     3586 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/cloudwatch_tests/test_loggers.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/ecs_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/ecs_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     5302 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/ecs_tests/test_ecs_client.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1120 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/conftest.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     7576 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/test_emr.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2152 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/test_emr_step_main.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     7699 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/test_pyspark.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      958 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/test_pyspark_step_launcher.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      760 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/test_utils.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/redshift_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/redshift_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      102 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/redshift_tests/conftest.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     6642 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/redshift_tests/test_resources.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      102 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/conftest.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     4218 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/test_compute_log_manager.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1722 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/test_file_handle_to_s3.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    15946 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/test_intermediate_storage.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1052 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/test_object_store.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1441 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/test_s3_file_cache.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     7083 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/test_s3_file_manager.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       89 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/test_version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/utils_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/utils_tests/__init__.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/utils_tests/mrjob_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/utils_tests/mrjob_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     3840 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/utils_tests/mrjob_tests/test_log4j.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2410 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/dagster_aws_tests/utils_tests/mrjob_tests/test_utils.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:21.000000 dagster-aws-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1184 2020-09-17 21:04:59.000000 dagster-aws-0.9.9rc1/setup.py
```

### Comparing `dagster-aws-0.9.9/LICENSE` & `dagster-aws-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/PKG-INFO` & `dagster-aws-0.9.9rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-aws
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for AWS-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-aws
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-aws-0.9.9/dagster_aws/cloudwatch/loggers.py` & `dagster-aws-0.9.9rc1/dagster_aws/cloudwatch/loggers.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/ecs/client.py` & `dagster-aws-0.9.9rc1/dagster_aws/ecs/client.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/ecs/launcher.py` & `dagster-aws-0.9.9rc1/dagster_aws/ecs/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/emr/configs.py` & `dagster-aws-0.9.9rc1/dagster_aws/emr/configs.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/emr/emr.py` & `dagster-aws-0.9.9rc1/dagster_aws/emr/emr.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/emr/emr_step_main.py` & `dagster-aws-0.9.9rc1/dagster_aws/emr/emr_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/emr/pyspark_step_launcher.py` & `dagster-aws-0.9.9rc1/dagster_aws/emr/pyspark_step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/emr/types.py` & `dagster-aws-0.9.9rc1/dagster_aws/emr/types.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/emr/utils.py` & `dagster-aws-0.9.9rc1/dagster_aws/emr/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/redshift/resources.py` & `dagster-aws-0.9.9rc1/dagster_aws/redshift/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/s3/__init__.py` & `dagster-aws-0.9.9rc1/dagster_aws/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/s3/compute_log_manager.py` & `dagster-aws-0.9.9rc1/dagster_aws/s3/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/s3/file_cache.py` & `dagster-aws-0.9.9rc1/dagster_aws/s3/file_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/s3/file_manager.py` & `dagster-aws-0.9.9rc1/dagster_aws/s3/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/s3/intermediate_storage.py` & `dagster-aws-0.9.9rc1/dagster_aws/s3/intermediate_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/s3/object_store.py` & `dagster-aws-0.9.9rc1/dagster_aws/s3/object_store.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/s3/resources.py` & `dagster-aws-0.9.9rc1/dagster_aws/s3/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/s3/s3_fake_resource.py` & `dagster-aws-0.9.9rc1/dagster_aws/s3/s3_fake_resource.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/s3/solids.py` & `dagster-aws-0.9.9rc1/dagster_aws/s3/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/s3/system_storage.py` & `dagster-aws-0.9.9rc1/dagster_aws/s3/system_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/s3/utils.py` & `dagster-aws-0.9.9rc1/dagster_aws/s3/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/utils/mrjob/log4j.py` & `dagster-aws-0.9.9rc1/dagster_aws/utils/mrjob/log4j.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/utils/mrjob/retry.py` & `dagster-aws-0.9.9rc1/dagster_aws/utils/mrjob/retry.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws/utils/mrjob/utils.py` & `dagster-aws-0.9.9rc1/dagster_aws/utils/mrjob/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws.egg-info/PKG-INFO` & `dagster-aws-0.9.9rc1/dagster_aws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-aws
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for AWS-specific Dagster framework solid and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-aws
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-aws-0.9.9/dagster_aws.egg-info/SOURCES.txt` & `dagster-aws-0.9.9rc1/dagster_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws_tests/cloudwatch_tests/conftest.py` & `dagster-aws-0.9.9rc1/dagster_aws_tests/cloudwatch_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws_tests/cloudwatch_tests/test_loggers.py` & `dagster-aws-0.9.9rc1/dagster_aws_tests/cloudwatch_tests/test_loggers.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws_tests/ecs_tests/test_ecs_client.py` & `dagster-aws-0.9.9rc1/dagster_aws_tests/ecs_tests/test_ecs_client.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws_tests/emr_tests/conftest.py` & `dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws_tests/emr_tests/test_emr.py` & `dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/test_emr.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws_tests/emr_tests/test_emr_step_main.py` & `dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/test_emr_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws_tests/emr_tests/test_pyspark.py` & `dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/test_pyspark.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws_tests/emr_tests/test_pyspark_step_launcher.py` & `dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/test_pyspark_step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws_tests/emr_tests/test_utils.py` & `dagster-aws-0.9.9rc1/dagster_aws_tests/emr_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws_tests/redshift_tests/test_resources.py` & `dagster-aws-0.9.9rc1/dagster_aws_tests/redshift_tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws_tests/s3_tests/test_compute_log_manager.py` & `dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/test_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws_tests/s3_tests/test_file_handle_to_s3.py` & `dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/test_file_handle_to_s3.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws_tests/s3_tests/test_intermediate_storage.py` & `dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/test_intermediate_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws_tests/s3_tests/test_object_store.py` & `dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/test_object_store.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws_tests/s3_tests/test_s3_file_cache.py` & `dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/test_s3_file_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws_tests/s3_tests/test_s3_file_manager.py` & `dagster-aws-0.9.9rc1/dagster_aws_tests/s3_tests/test_s3_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws_tests/utils_tests/mrjob_tests/test_log4j.py` & `dagster-aws-0.9.9rc1/dagster_aws_tests/utils_tests/mrjob_tests/test_log4j.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/dagster_aws_tests/utils_tests/mrjob_tests/test_utils.py` & `dagster-aws-0.9.9rc1/dagster_aws_tests/utils_tests/mrjob_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-aws-0.9.9/setup.py` & `dagster-aws-0.9.9rc1/setup.py`

 * *Files identical despite different names*

