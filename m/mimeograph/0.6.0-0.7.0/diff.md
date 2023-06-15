# Comparing `tmp/mimeograph-0.6.0.tar.gz` & `tmp/mimeograph-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimeograph-0.6.0.tar", last modified: Sat May 20 16:31:41 2023, max compression
+gzip compressed data, was "mimeograph-0.7.0.tar", last modified: Thu Jun 15 08:33:35 2023, max compression
```

## Comparing `mimeograph-0.6.0.tar` & `mimeograph-0.7.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.902028 mimeograph-0.6.0/
--rw-r--r--   0 tom        (501) staff       (20)     1075 2023-03-12 16:41:41.000000 mimeograph-0.6.0/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)       30 2023-05-09 15:53:05.000000 mimeograph-0.6.0/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)    26854 2023-05-20 16:31:41.901820 mimeograph-0.6.0/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)    24498 2023-05-17 16:22:49.000000 mimeograph-0.6.0/README.md
--rw-r--r--   0 tom        (501) staff       (20)     3768 2023-05-20 16:30:13.000000 mimeograph-0.6.0/pyproject.toml
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-05-20 16:31:41.902087 mimeograph-0.6.0/setup.cfg
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.879002 mimeograph-0.6.0/src/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.880912 mimeograph-0.6.0/src/mimeo/
--rw-r--r--   0 tom        (501) staff       (20)     1327 2023-05-20 16:30:13.000000 mimeograph-0.6.0/src/mimeo/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      408 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/__main__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.882493 mimeograph-0.6.0/src/mimeo/cli/
--rw-r--r--   0 tom        (501) staff       (20)      761 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/cli/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     2290 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/cli/exc.py
--rw-r--r--   0 tom        (501) staff       (20)     4408 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/cli/job.py
--rw-r--r--   0 tom        (501) staff       (20)    16721 2023-05-20 16:30:13.000000 mimeograph-0.6.0/src/mimeo/cli/parsers.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.883461 mimeograph-0.6.0/src/mimeo/config/
--rw-r--r--   0 tom        (501) staff       (20)      691 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/config/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     5718 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/config/constants.py
--rw-r--r--   0 tom        (501) staff       (20)    10653 2023-05-20 16:17:22.000000 mimeograph-0.6.0/src/mimeo/config/exc.py
--rw-r--r--   0 tom        (501) staff       (20)    23424 2023-05-20 16:17:22.000000 mimeograph-0.6.0/src/mimeo/config/mimeo_config.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.885840 mimeograph-0.6.0/src/mimeo/consumers/
--rw-r--r--   0 tom        (501) staff       (20)     1322 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/consumers/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1402 2023-05-13 05:35:39.000000 mimeograph-0.6.0/src/mimeo/consumers/consumer.py
--rw-r--r--   0 tom        (501) staff       (20)     2131 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/consumers/consumer_factory.py
--rw-r--r--   0 tom        (501) staff       (20)     2364 2023-05-13 05:35:39.000000 mimeograph-0.6.0/src/mimeo/consumers/file_consumer.py
--rw-r--r--   0 tom        (501) staff       (20)     3032 2023-05-13 05:35:39.000000 mimeograph-0.6.0/src/mimeo/consumers/http_consumer.py
--rw-r--r--   0 tom        (501) staff       (20)     1018 2023-05-13 05:35:39.000000 mimeograph-0.6.0/src/mimeo/consumers/raw_consumer.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.887511 mimeograph-0.6.0/src/mimeo/context/
--rw-r--r--   0 tom        (501) staff       (20)     1001 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/context/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     4261 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/context/decorators.py
--rw-r--r--   0 tom        (501) staff       (20)     5087 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/context/exc.py
--rw-r--r--   0 tom        (501) staff       (20)    18138 2023-05-20 16:17:22.000000 mimeograph-0.6.0/src/mimeo/context/mimeo_context.py
--rw-r--r--   0 tom        (501) staff       (20)     5111 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/context/mimeo_context_manager.py
--rw-r--r--   0 tom        (501) staff       (20)     2888 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/context/mimeo_iteration.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.889805 mimeograph-0.6.0/src/mimeo/database/
--rw-r--r--   0 tom        (501) staff       (20)     1805 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/database/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     5507 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/database/cities.py
--rw-r--r--   0 tom        (501) staff       (20)     5775 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/database/countries.py
--rw-r--r--   0 tom        (501) staff       (20)     5613 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/database/currencies.py
--rw-r--r--   0 tom        (501) staff       (20)     6200 2023-05-20 16:17:22.000000 mimeograph-0.6.0/src/mimeo/database/exc.py
--rw-r--r--   0 tom        (501) staff       (20)     5471 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/database/first_names.py
--rw-r--r--   0 tom        (501) staff       (20)     2180 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/database/last_names.py
--rw-r--r--   0 tom        (501) staff       (20)    10209 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/database/mimeo_db.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.890918 mimeograph-0.6.0/src/mimeo/generators/
--rw-r--r--   0 tom        (501) staff       (20)      981 2023-05-13 05:35:39.000000 mimeograph-0.6.0/src/mimeo/generators/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1117 2023-05-13 05:35:39.000000 mimeograph-0.6.0/src/mimeo/generators/exc.py
--rw-r--r--   0 tom        (501) staff       (20)     2685 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/generators/generator.py
--rw-r--r--   0 tom        (501) staff       (20)     1654 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/generators/generator_factory.py
--rw-r--r--   0 tom        (501) staff       (20)    24157 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/generators/xml_generator.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.891411 mimeograph-0.6.0/src/mimeo/logging/
--rw-r--r--   0 tom        (501) staff       (20)     1364 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/logging/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1743 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/logging/filters.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.892087 mimeograph-0.6.0/src/mimeo/meta/
--rw-r--r--   0 tom        (501) staff       (20)      652 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/meta/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     4033 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/meta/alive.py
--rw-r--r--   0 tom        (501) staff       (20)      656 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/meta/exc.py
--rw-r--r--   0 tom        (501) staff       (20)     1525 2023-05-13 05:35:39.000000 mimeograph-0.6.0/src/mimeo/mimeo.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.896837 mimeograph-0.6.0/src/mimeo/resources/
--rw-r--r--   0 tom        (501) staff       (20)      362 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/resources/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)  1541655 2023-03-30 16:49:35.000000 mimeograph-0.6.0/src/mimeo/resources/cities.csv
--rw-r--r--   0 tom        (501) staff       (20)     1467 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/resources/constants.yaml
--rw-r--r--   0 tom        (501) staff       (20)     4205 2023-03-30 16:49:35.000000 mimeograph-0.6.0/src/mimeo/resources/countries.csv
--rw-r--r--   0 tom        (501) staff       (20)     7268 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/resources/currencies.csv
--rw-r--r--   0 tom        (501) staff       (20)      783 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/resources/exc.py
--rw-r--r--   0 tom        (501) staff       (20)    66313 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/resources/forenames.csv
--rw-r--r--   0 tom        (501) staff       (20)      719 2023-03-30 16:49:35.000000 mimeograph-0.6.0/src/mimeo/resources/logging.yaml
--rw-r--r--   0 tom        (501) staff       (20)  1197769 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/resources/surnames.txt
--rw-r--r--   0 tom        (501) staff       (20)     1035 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/tools.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.899729 mimeograph-0.6.0/src/mimeo/utils/
--rw-r--r--   0 tom        (501) staff       (20)     2193 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/utils/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     6226 2023-05-20 16:17:22.000000 mimeograph-0.6.0/src/mimeo/utils/exc.py
--rw-r--r--   0 tom        (501) staff       (20)    29122 2023-05-20 16:17:22.000000 mimeograph-0.6.0/src/mimeo/utils/mimeo_utils.py
--rw-r--r--   0 tom        (501) staff       (20)    20118 2023-05-20 16:17:22.000000 mimeograph-0.6.0/src/mimeo/utils/renderers.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.900924 mimeograph-0.6.0/src/mimeograph.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)    26854 2023-05-20 16:31:41.000000 mimeograph-0.6.0/src/mimeograph.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     1987 2023-05-20 16:31:41.000000 mimeograph-0.6.0/src/mimeograph.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-05-20 16:31:41.000000 mimeograph-0.6.0/src/mimeograph.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)       46 2023-05-20 16:31:41.000000 mimeograph-0.6.0/src/mimeograph.egg-info/entry_points.txt
--rw-r--r--   0 tom        (501) staff       (20)      212 2023-05-20 16:31:41.000000 mimeograph-0.6.0/src/mimeograph.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)        6 2023-05-20 16:31:41.000000 mimeograph-0.6.0/src/mimeograph.egg-info/top_level.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.901434 mimeograph-0.6.0/tests/
--rw-r--r--   0 tom        (501) staff       (20)     1828 2023-05-13 05:35:39.000000 mimeograph-0.6.0/tests/test_mimeograph.py
--rw-r--r--   0 tom        (501) staff       (20)      502 2023-05-20 16:17:22.000000 mimeograph-0.6.0/tests/test_tools.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.192970 mimeograph-0.7.0/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-0.7.0/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)       30 2023-05-11 05:33:09.000000 mimeograph-0.7.0/MANIFEST.in
+-rw-rw-r--   0 tom       (1000) tom       (1000)    27826 2023-06-15 08:33:35.192970 mimeograph-0.7.0/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)    25470 2023-06-12 07:59:15.000000 mimeograph-0.7.0/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3894 2023-06-15 08:31:52.000000 mimeograph-0.7.0/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-06-15 08:33:35.192970 mimeograph-0.7.0/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.184970 mimeograph-0.7.0/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.184970 mimeograph-0.7.0/src/mimeo/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1440 2023-06-15 08:31:52.000000 mimeograph-0.7.0/src/mimeo/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      408 2023-05-11 13:41:23.000000 mimeograph-0.7.0/src/mimeo/__main__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.184970 mimeograph-0.7.0/src/mimeo/cli/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      761 2023-05-11 05:33:09.000000 mimeograph-0.7.0/src/mimeo/cli/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2290 2023-05-17 08:57:29.000000 mimeograph-0.7.0/src/mimeo/cli/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4117 2023-05-27 06:14:50.000000 mimeograph-0.7.0/src/mimeo/cli/job.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    16834 2023-06-15 08:31:52.000000 mimeograph-0.7.0/src/mimeo/cli/parsers.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.184970 mimeograph-0.7.0/src/mimeo/config/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      837 2023-05-27 06:14:50.000000 mimeograph-0.7.0/src/mimeo/config/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5938 2023-06-15 08:27:49.000000 mimeograph-0.7.0/src/mimeo/config/constants.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    12311 2023-05-27 06:14:50.000000 mimeograph-0.7.0/src/mimeo/config/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    34682 2023-06-15 08:27:49.000000 mimeograph-0.7.0/src/mimeo/config/mimeo_config.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.188970 mimeograph-0.7.0/src/mimeo/consumers/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1322 2023-05-11 05:33:09.000000 mimeograph-0.7.0/src/mimeo/consumers/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1402 2023-05-12 09:42:23.000000 mimeograph-0.7.0/src/mimeo/consumers/consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2131 2023-05-17 08:14:52.000000 mimeograph-0.7.0/src/mimeo/consumers/consumer_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2364 2023-05-12 09:42:23.000000 mimeograph-0.7.0/src/mimeo/consumers/file_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3032 2023-06-15 08:27:49.000000 mimeograph-0.7.0/src/mimeo/consumers/http_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1018 2023-05-12 09:42:23.000000 mimeograph-0.7.0/src/mimeo/consumers/raw_consumer.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.188970 mimeograph-0.7.0/src/mimeo/context/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1001 2023-05-11 05:33:09.000000 mimeograph-0.7.0/src/mimeo/context/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4261 2023-05-11 05:33:09.000000 mimeograph-0.7.0/src/mimeo/context/decorators.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5087 2023-05-11 05:33:09.000000 mimeograph-0.7.0/src/mimeo/context/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    18138 2023-05-22 07:52:53.000000 mimeograph-0.7.0/src/mimeo/context/mimeo_context.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5111 2023-05-17 13:09:43.000000 mimeograph-0.7.0/src/mimeo/context/mimeo_context_manager.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2888 2023-05-11 05:33:09.000000 mimeograph-0.7.0/src/mimeo/context/mimeo_iteration.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.188970 mimeograph-0.7.0/src/mimeo/database/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1805 2023-05-16 10:04:29.000000 mimeograph-0.7.0/src/mimeo/database/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5507 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/database/cities.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5775 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/database/countries.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5613 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/database/currencies.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6200 2023-05-22 07:52:53.000000 mimeograph-0.7.0/src/mimeo/database/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5471 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/database/first_names.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2180 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/database/last_names.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10209 2023-05-16 10:04:29.000000 mimeograph-0.7.0/src/mimeo/database/mimeo_db.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.188970 mimeograph-0.7.0/src/mimeo/generators/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      981 2023-06-15 08:27:49.000000 mimeograph-0.7.0/src/mimeo/generators/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1117 2023-06-15 08:27:49.000000 mimeograph-0.7.0/src/mimeo/generators/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2685 2023-06-15 08:27:49.000000 mimeograph-0.7.0/src/mimeo/generators/generator.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1654 2023-06-15 08:27:49.000000 mimeograph-0.7.0/src/mimeo/generators/generator_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    21089 2023-06-15 08:27:49.000000 mimeograph-0.7.0/src/mimeo/generators/xml_generator.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.188970 mimeograph-0.7.0/src/mimeo/logging/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1364 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/logging/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1743 2023-05-11 05:33:09.000000 mimeograph-0.7.0/src/mimeo/logging/filters.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.188970 mimeograph-0.7.0/src/mimeo/meta/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      652 2023-05-11 05:33:09.000000 mimeograph-0.7.0/src/mimeo/meta/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4033 2023-05-17 13:09:43.000000 mimeograph-0.7.0/src/mimeo/meta/alive.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      656 2023-05-17 13:09:43.000000 mimeograph-0.7.0/src/mimeo/meta/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1525 2023-05-12 09:42:23.000000 mimeograph-0.7.0/src/mimeo/mimeo.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.192970 mimeograph-0.7.0/src/mimeo/resources/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      362 2023-05-17 13:09:43.000000 mimeograph-0.7.0/src/mimeo/resources/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1541655 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/resources/cities.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1538 2023-06-15 08:27:49.000000 mimeograph-0.7.0/src/mimeo/resources/constants.yaml
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/resources/countries.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7268 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/resources/currencies.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      783 2023-05-17 13:09:43.000000 mimeograph-0.7.0/src/mimeo/resources/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    66313 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/resources/forenames.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      719 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/resources/logging.yaml
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1197769 2023-05-16 15:27:55.000000 mimeograph-0.7.0/src/mimeo/resources/surnames.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1035 2023-05-17 13:09:43.000000 mimeograph-0.7.0/src/mimeo/tools.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.192970 mimeograph-0.7.0/src/mimeo/utils/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2193 2023-05-16 10:04:29.000000 mimeograph-0.7.0/src/mimeo/utils/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6224 2023-06-12 07:59:15.000000 mimeograph-0.7.0/src/mimeo/utils/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    29122 2023-05-22 07:52:53.000000 mimeograph-0.7.0/src/mimeo/utils/mimeo_utils.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    20108 2023-06-12 07:59:15.000000 mimeograph-0.7.0/src/mimeo/utils/renderers.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.192970 mimeograph-0.7.0/src/mimeograph.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    27826 2023-06-15 08:33:35.000000 mimeograph-0.7.0/src/mimeograph.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1987 2023-06-15 08:33:35.000000 mimeograph-0.7.0/src/mimeograph.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-06-15 08:33:35.000000 mimeograph-0.7.0/src/mimeograph.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-06-15 08:33:35.000000 mimeograph-0.7.0/src/mimeograph.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)      222 2023-06-15 08:33:35.000000 mimeograph-0.7.0/src/mimeograph.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-06-15 08:33:35.000000 mimeograph-0.7.0/src/mimeograph.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-15 08:33:35.192970 mimeograph-0.7.0/tests/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1848 2023-06-15 08:27:49.000000 mimeograph-0.7.0/tests/test_mimeograph.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      502 2023-05-22 07:52:53.000000 mimeograph-0.7.0/tests/test_tools.py
```

### Comparing `mimeograph-0.6.0/LICENSE` & `mimeograph-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/PKG-INFO` & `mimeograph-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimeograph
-Version: 0.6.0
+Version: 0.7.0
 Summary: Generate data based on a simple template
 Author-email: "T.A. Programming Svcs." <tomasz.maciej.aniolowski@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tomasz Aniołowski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -70,74 +70,97 @@
 
 
 ## Usage/Examples
 
 ### Mimeo Configuration
 
 Prepare Mimeo Configuration first
-- for a command line tool: in a JSON file
-- for a `Mimeograph` python class: in a `dict`
+- for a command line tool: in a JSON or XML file
+- for a `Mimeograph` python class: in a `dict` or stringified XML
 
 ```json
 {
   "_templates_": [
     {
       "count": 30,
       "model": {
         "SomeEntity": {
-          "_attrs": {
-            "xmlns": "http://mimeo.arch.com/default-namespace",
-            "xmlns:pn": "http://mimeo.arch.com/prefixed-namespace"
-          },
+          "@xmlns": "http://mimeo.arch.com/default-namespace",
+          "@xmlns:pn": "http://mimeo.arch.com/prefixed-namespace",
           "ChildNode1": 1,
           "ChildNode2": "value-2",
           "ChildNode3": true
         }
       }
     }
   ]
 }
 ```
+```xml
+<mimeo_configuration>
+    <_templates_>
+        <_template_>
+            <count>30</count>
+            <model>
+
+                <SomeEntity
+                    xmlns="http://mimeo.arch.com/default-namespace"
+                    xmlns:pn="http://mimeo.arch.com/prefixed-namespace">
+                    <ChildNode1>1</ChildNode1>
+                    <pn:ChildNode2>value-2</pn:ChildNode2>
+                    <ChildNode3>true</ChildNode3>
+                </SomeEntity>
+
+            </model>
+        </_template_>
+    </_templates_>
+</mimeo_configuration>
+```
 _You can find more configuration examples in the `examples` folder._
 
 ### Mimeograph
 
 #### Command line tool
 
 ```sh
 mimeo SomeEntity-config.json
+mimeo SomeEntity-config.xml
 ```
 
 #### Python library
 
 ```python
-from mimeo import MimeoConfig, Mimeograph
+from mimeo import MimeoConfigFactory, Mimeograph
 
 config = {
-    # Your configuration
+    # Your configuration in a dict
 }
-mimeo_config = MimeoConfig(config)
+config = """
+    Your configuration in a stringified XML node
+"""
+config = ""  # A file path to your configuration (JSON / XML)
+mimeo_config = MimeoConfigFactory.parse(config)
 Mimeograph(mimeo_config).process()
 ```
 ***
 The Mimeo Configuration above will produce 2 files:
 
 ```xml
 <!-- mimeo-output/mimeo-output-1.xml-->
 <SomeEntity xmlns="http://mimeo.arch.com/default-namespace" xmlns:pn="http://mimeo.arch.com/prefixed-namespace">
     <ChildNode1>1</ChildNode1>
-    <ChildNode2>value-2</ChildNode2>
+    <pn:ChildNode2>value-2</pn:ChildNode2>
     <ChildNode3>true</ChildNode3>
 </SomeEntity>
 ```
 ```xml
 <!-- mimeo-output/mimeo-output-2.xml-->
 <SomeEntity xmlns="http://mimeo.arch.com/default-namespace" xmlns:pn="http://mimeo.arch.com/prefixed-namespace">
     <ChildNode1>1</ChildNode1>
-    <ChildNode2>value-2</ChildNode2>
+    <pn:ChildNode2>value-2</pn:ChildNode2>
     <ChildNode3>true</ChildNode3>
 </SomeEntity>
 ```
 ***
 
 ### Mimeo Utils
 
@@ -152,14 +175,28 @@
       "id": "{auto_increment}",
       "randomstring": "{random_str}",
       "randomint": "{random_int}"
     }
   }
 }
 ```
+```xml
+<_template_>
+    <count>2</count>
+    <model>
+        
+        <SomeEntity>
+            <id>{auto_increment}</id>
+            <randomstring>{random_str}</randomstring>
+            <randomint>{random_int}</randomint>
+        </SomeEntity>
+        
+    </model>
+</_template_>
+```
 
 **XML Data**
 ```xml
 <SomeEntity>
     <id>00001</id>
     <randomstring>mCApsYZprayYkmKnYWxe</randomstring>
     <randomint>8</randomint>
@@ -178,30 +215,30 @@
 
 ### Mimeo CLI
 
 #### Mimeo Configuration arguments
 
 When using Mimeo command line tool you can overwrite Mimeo Configuration properties:
 
-| Short option | Long option         | Description                                                                  |
-|:------------:|:--------------------|:-----------------------------------------------------------------------------|
+| Short option | Long option         | Description                                                          |
+|:------------:|:--------------------|:---------------------------------------------------------------------|
 |     `-o`     | `--output`          | overwrite the `output/direction` property                            |
 |     `-x`     | `--xml-declaration` | overwrite the `output/xml_declaration` property                      |
 |     `-i`     | `--indent`          | overwrite the `output/indent` property                               |
 |     `-d`     | `--directory`       | overwrite the `output/directory_path` property                       |
 |     `-f`     | `--file`            | overwrite the `output/file_name` property                            |
 |     `-H`     | `--http-host`       | overwrite the `output/host` property                                 |
 |     `-p`     | `--http-port`       | overwrite the `output/port` property                                 |
 |     `-E`     | `--http-endpoint`   | overwrite the `output/endpoint` property                             |
 |     `-U`     | `--http-user`       | overwrite the `output/username` property                             |
 |     `-P`     | `--http-password`   | overwrite the `output/password` property                             |
 |              | `--http-method`     | overwrite the `output/method` property                               |
 |              | `--http-protocol`   | overwrite the `output/protocol` property                             |
 |     `-e`     | `--http-env`        | overwrite the output http properties using a mimeo env configuration |
-|              | `--http-envs-file`  | use a custom environments file (by default: mimeo.envs.json)                 |
+|              | `--http-envs-file`  | use a custom environments file (by default: mimeo.envs.json)         |
 
 #### Logging arguments
 
 | Short option | Long option | Description       |
 |:------------:|:------------|:------------------|
 |              | `--silent`  | disable INFO logs |
 |              | `--debug`   | enable DEBUG mode |
@@ -319,28 +356,27 @@
 }
 ```
 
 #### Mimeo Special Fields
 
 In Mimeo Template you can use so-called _special fields_.
 Every field in a template can be stored in memory (_provided_) and used later as a value of other fields (_injected_).
-To provide and inject a special field use curly brackets and colons: [`{:SomeField:}`].
-You provide a field when you use this format in a field name (JSON property name),
-and inject by applying it in a field value.  
+To provide a special field, wrap its name with colons: [`:SomeField:`]. To inject, use additionally curly braces to
+let interpreter know it should be rendered [`{:SomeField:}`].
 They can be injected as partial values, similarly to Mimeo Vars.
 
 Example
 ```json
 {
   "_templates_": [
     {
       "count": 5,
       "model": {
         "SomeEntity": {
-          "{:ChildNode1:}": "custom-value",
+          ":ChildNode1:": "custom-value",
           "ChildNode2": "{:ChildNode1:}",
           "ChildNode3": "{:ChildNode1:}-with-suffix"
         }
       }
     }
   ]
 }
```

### Comparing `mimeograph-0.6.0/README.md` & `mimeograph-0.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,74 +20,97 @@
 
 
 ## Usage/Examples
 
 ### Mimeo Configuration
 
 Prepare Mimeo Configuration first
-- for a command line tool: in a JSON file
-- for a `Mimeograph` python class: in a `dict`
+- for a command line tool: in a JSON or XML file
+- for a `Mimeograph` python class: in a `dict` or stringified XML
 
 ```json
 {
   "_templates_": [
     {
       "count": 30,
       "model": {
         "SomeEntity": {
-          "_attrs": {
-            "xmlns": "http://mimeo.arch.com/default-namespace",
-            "xmlns:pn": "http://mimeo.arch.com/prefixed-namespace"
-          },
+          "@xmlns": "http://mimeo.arch.com/default-namespace",
+          "@xmlns:pn": "http://mimeo.arch.com/prefixed-namespace",
           "ChildNode1": 1,
           "ChildNode2": "value-2",
           "ChildNode3": true
         }
       }
     }
   ]
 }
 ```
+```xml
+<mimeo_configuration>
+    <_templates_>
+        <_template_>
+            <count>30</count>
+            <model>
+
+                <SomeEntity
+                    xmlns="http://mimeo.arch.com/default-namespace"
+                    xmlns:pn="http://mimeo.arch.com/prefixed-namespace">
+                    <ChildNode1>1</ChildNode1>
+                    <pn:ChildNode2>value-2</pn:ChildNode2>
+                    <ChildNode3>true</ChildNode3>
+                </SomeEntity>
+
+            </model>
+        </_template_>
+    </_templates_>
+</mimeo_configuration>
+```
 _You can find more configuration examples in the `examples` folder._
 
 ### Mimeograph
 
 #### Command line tool
 
 ```sh
 mimeo SomeEntity-config.json
+mimeo SomeEntity-config.xml
 ```
 
 #### Python library
 
 ```python
-from mimeo import MimeoConfig, Mimeograph
+from mimeo import MimeoConfigFactory, Mimeograph
 
 config = {
-    # Your configuration
+    # Your configuration in a dict
 }
-mimeo_config = MimeoConfig(config)
+config = """
+    Your configuration in a stringified XML node
+"""
+config = ""  # A file path to your configuration (JSON / XML)
+mimeo_config = MimeoConfigFactory.parse(config)
 Mimeograph(mimeo_config).process()
 ```
 ***
 The Mimeo Configuration above will produce 2 files:
 
 ```xml
 <!-- mimeo-output/mimeo-output-1.xml-->
 <SomeEntity xmlns="http://mimeo.arch.com/default-namespace" xmlns:pn="http://mimeo.arch.com/prefixed-namespace">
     <ChildNode1>1</ChildNode1>
-    <ChildNode2>value-2</ChildNode2>
+    <pn:ChildNode2>value-2</pn:ChildNode2>
     <ChildNode3>true</ChildNode3>
 </SomeEntity>
 ```
 ```xml
 <!-- mimeo-output/mimeo-output-2.xml-->
 <SomeEntity xmlns="http://mimeo.arch.com/default-namespace" xmlns:pn="http://mimeo.arch.com/prefixed-namespace">
     <ChildNode1>1</ChildNode1>
-    <ChildNode2>value-2</ChildNode2>
+    <pn:ChildNode2>value-2</pn:ChildNode2>
     <ChildNode3>true</ChildNode3>
 </SomeEntity>
 ```
 ***
 
 ### Mimeo Utils
 
@@ -102,14 +125,28 @@
       "id": "{auto_increment}",
       "randomstring": "{random_str}",
       "randomint": "{random_int}"
     }
   }
 }
 ```
+```xml
+<_template_>
+    <count>2</count>
+    <model>
+        
+        <SomeEntity>
+            <id>{auto_increment}</id>
+            <randomstring>{random_str}</randomstring>
+            <randomint>{random_int}</randomint>
+        </SomeEntity>
+        
+    </model>
+</_template_>
+```
 
 **XML Data**
 ```xml
 <SomeEntity>
     <id>00001</id>
     <randomstring>mCApsYZprayYkmKnYWxe</randomstring>
     <randomint>8</randomint>
@@ -128,30 +165,30 @@
 
 ### Mimeo CLI
 
 #### Mimeo Configuration arguments
 
 When using Mimeo command line tool you can overwrite Mimeo Configuration properties:
 
-| Short option | Long option         | Description                                                                  |
-|:------------:|:--------------------|:-----------------------------------------------------------------------------|
+| Short option | Long option         | Description                                                          |
+|:------------:|:--------------------|:---------------------------------------------------------------------|
 |     `-o`     | `--output`          | overwrite the `output/direction` property                            |
 |     `-x`     | `--xml-declaration` | overwrite the `output/xml_declaration` property                      |
 |     `-i`     | `--indent`          | overwrite the `output/indent` property                               |
 |     `-d`     | `--directory`       | overwrite the `output/directory_path` property                       |
 |     `-f`     | `--file`            | overwrite the `output/file_name` property                            |
 |     `-H`     | `--http-host`       | overwrite the `output/host` property                                 |
 |     `-p`     | `--http-port`       | overwrite the `output/port` property                                 |
 |     `-E`     | `--http-endpoint`   | overwrite the `output/endpoint` property                             |
 |     `-U`     | `--http-user`       | overwrite the `output/username` property                             |
 |     `-P`     | `--http-password`   | overwrite the `output/password` property                             |
 |              | `--http-method`     | overwrite the `output/method` property                               |
 |              | `--http-protocol`   | overwrite the `output/protocol` property                             |
 |     `-e`     | `--http-env`        | overwrite the output http properties using a mimeo env configuration |
-|              | `--http-envs-file`  | use a custom environments file (by default: mimeo.envs.json)                 |
+|              | `--http-envs-file`  | use a custom environments file (by default: mimeo.envs.json)         |
 
 #### Logging arguments
 
 | Short option | Long option | Description       |
 |:------------:|:------------|:------------------|
 |              | `--silent`  | disable INFO logs |
 |              | `--debug`   | enable DEBUG mode |
@@ -269,28 +306,27 @@
 }
 ```
 
 #### Mimeo Special Fields
 
 In Mimeo Template you can use so-called _special fields_.
 Every field in a template can be stored in memory (_provided_) and used later as a value of other fields (_injected_).
-To provide and inject a special field use curly brackets and colons: [`{:SomeField:}`].
-You provide a field when you use this format in a field name (JSON property name),
-and inject by applying it in a field value.  
+To provide a special field, wrap its name with colons: [`:SomeField:`]. To inject, use additionally curly braces to
+let interpreter know it should be rendered [`{:SomeField:}`].
 They can be injected as partial values, similarly to Mimeo Vars.
 
 Example
 ```json
 {
   "_templates_": [
     {
       "count": 5,
       "model": {
         "SomeEntity": {
-          "{:ChildNode1:}": "custom-value",
+          ":ChildNode1:": "custom-value",
           "ChildNode2": "{:ChildNode1:}",
           "ChildNode3": "{:ChildNode1:}-with-suffix"
         }
       }
     }
   ]
 }
```

### Comparing `mimeograph-0.6.0/pyproject.toml` & `mimeograph-0.7.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mimeograph"
-version = "0.6.0"
+version = "0.7.0"
 description = "Generate data based on a simple template"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [{ name = "T.A. Programming Svcs.", email = "tomasz.maciej.aniolowski@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -25,14 +25,15 @@
     "Topic :: Database",
     "Topic :: Software Development",
     "Topic :: Software Development :: Testing",
     "Topic :: Utilities",
 ]
 keywords = ["mimeograph", "mimeo", "generate", "generator", "data", "xml"]
 dependencies = [
+    "xmltodict",
     "aiohttp",
     "aiofiles",
     "pandas",
     "pyyaml",
     "haggis"
 ]
 
@@ -60,15 +61,15 @@
     "pytest-asyncio"
 ]
 
 [project.scripts]
 mimeo = "mimeo.__main__:main"
 
 [tool.bumpver]
-current_version = "0.6.0"
+current_version = "0.7.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} to {new_version}"
 commit          = true
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
@@ -141,10 +142,13 @@
 ]
 "src/mimeo/logging/filters.py" = [
     "A003" # an external superclass
 ]
 "src/mimeo/utils/mimeo_utils.py" = [
     "ARG002" # ignore unexpected keyword arguments
 ]
+"tests/cli/test_mimeo_cli.py" = [
+    "PLR0913" # allow for many function arguments in setup with fixtures
+]
 "tests/utils/test_mimeo_util.py" = [
     "N802" # the test scenario requires uppercased function name
 ]
```

### Comparing `mimeograph-0.6.0/src/mimeo/__init__.py` & `mimeograph-0.7.0/src/mimeo/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """The Mimeo package.
 
 This package provides the Mimeo functionality with the highest level
 class together with the Mimeo Configuration class:
 * MimeoConfig
     A class representing Mimeo Configuration.
+* MimeoConfigFactory
+    A factory class to instantiate a MimeoConfig.
 * Mimeograph
     A class responsible for the Mimeo processing.
 
 It includes __main__.py module to provide a Command Line Interface
 for the Mimeo.
 
 This package is not meant to be used directly on low-level classes.
@@ -41,12 +43,12 @@
     The Mimeo Tools module
 
 To use this package, simply import the desired classes:
     from mimeo import MimeoConfig, Mimeograph
 """
 from __future__ import annotations
 
-from .config import MimeoConfig
+from .config import MimeoConfig, MimeoConfigFactory
 from .mimeo import Mimeograph
 
-__version__ = "0.6.0"
-__all__ = ["MimeoConfig", "Mimeograph"]
+__version__ = "0.7.0"
+__all__ = ["MimeoConfig", "MimeoConfigFactory", "Mimeograph"]
```

### Comparing `mimeograph-0.6.0/src/mimeo/cli/__init__.py` & `mimeograph-0.7.0/src/mimeo/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/cli/exc.py` & `mimeograph-0.7.0/src/mimeo/cli/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/cli/job.py` & `mimeograph-0.7.0/src/mimeo/cli/job.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 It exports a single class:
     * MimeoJob
         A class representing a single Mimeo processing job.
 """
 from __future__ import annotations
 
 import asyncio
-import json
 import logging
 from argparse import Namespace
 from os import walk
 from pathlib import Path
 
 from mimeo import MimeoConfig, Mimeograph
 from mimeo.cli import MimeoArgumentParser, MimeoConfigParser
@@ -91,17 +90,19 @@
             A list of file paths
         """
         file_paths = []
         for file_path in paths:
             if Path(file_path).is_dir():
                 for dir_path, _, file_names in walk(file_path):
                     for file_name in file_names:
-                        file_paths.append(Path(f"{dir_path}/{file_name}"))
+                        path = Path(f"{dir_path}/{file_name}")
+                        file_paths.append(str(path))
             elif Path(file_path).is_file():
-                file_paths.append(Path(file_path))
+                path = Path(file_path)
+                file_paths.append(str(path))
             else:
                 raise PathNotFoundError(file_path)
         return file_paths
 
     @classmethod
     def _get_mimeo_config(
             cls,
@@ -128,19 +129,9 @@
         Raises
         ------
         EnvironmentsFileNotFoundError
             If environments file does not exist.
         EnvironmentNotFoundError
             If the http environment is not defined in the environments file
         """
-        config = cls._get_raw_config(config_path)
-        mimeo_config_parser = MimeoConfigParser(config, args)
+        mimeo_config_parser = MimeoConfigParser(config_path, args)
         return mimeo_config_parser.parse_config()
-
-    @staticmethod
-    def _get_raw_config(
-            config_path: str,
-    ) -> dict:
-        """Load configuration file to a dictionary."""
-        logger.info("Reading Mimeo Configuration: %s", config_path)
-        with Path(config_path).open() as config_file:
-            return json.load(config_file)
```

### Comparing `mimeograph-0.6.0/src/mimeo/cli/parsers.py` & `mimeograph-0.7.0/src/mimeo/cli/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import logging
 from argparse import ArgumentParser, Namespace
 from pathlib import Path
 
 from mimeo import MimeoConfig
 from mimeo.cli.exc import (EnvironmentNotFoundError,
                            EnvironmentsFileNotFoundError)
+from mimeo.config import MimeoConfigFactory
 from mimeo.config import constants as cc
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_ENVS_PATH = "mimeo.envs.json"
 
 
@@ -96,15 +97,15 @@
             self,
     ):
         """Add positional arguments."""
         self.add_argument(
             "-v",
             "--version",
             action="version",
-            version="%(prog)s v0.6.0")
+            version="%(prog)s v0.7.0")
         self.add_argument(
             "paths",
             nargs="+",
             type=str,
             help="take paths to Mimeo Configuration files")
 
     def _add_mimeo_configuration_arguments(
@@ -268,27 +269,27 @@
         "http_password": {
             "entry_path": [cc.OUTPUT_KEY, cc.OUTPUT_PASSWORD_KEY],
         },
     }
 
     def __init__(
             self,
-            config: dict,
+            config_path: str,
             args: Namespace,
     ):
         """Initialize MimeoConfigParser class.
 
         Parameters
         ----------
-        config:
-            A source config dictionary
-        args
+        config_path: str
+            A source config path
+        args: Namespace
             Arguments parsed by MimeoArgumentParser
         """
-        self._raw_config = config
+        self._raw_config = MimeoConfigFactory.parse_source(config_path)
         self._args = args
 
     def parse_config(
             self,
     ) -> MimeoConfig:
         """Parse a Mimeo Configuration using Mimeo arguments.
 
@@ -311,15 +312,15 @@
         EnvironmentNotFoundError
             If the http environment is not defined in the environments file
         """
         logger.info("Parsing Mimeo Configuration")
         config = dict(self._raw_config)
         config = self._parse_with_http_environment(config)
         config = self._parse_with_specific_args(config)
-        mimeo_config = MimeoConfig(config)
+        mimeo_config = MimeoConfigFactory.parse(config)
         logger.fine("Parsed Mimeo Configuration: [%s]", mimeo_config)
         return mimeo_config
 
     def _parse_with_http_environment(
             self,
             config: dict,
     ) -> dict:
```

### Comparing `mimeograph-0.6.0/src/mimeo/config/__init__.py` & `mimeograph-0.7.0/src/mimeo/config/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,21 +5,23 @@
     The Mimeo Configuration module
 * constants
     The Mimeo Configuration Constants module
 * exc
     The Mimeo Configuration Exceptions module
 
 The Mimeo Configuration package exports a class representing
-root Mimeo Configuration component:
+root Mimeo Configuration component and a factory:
 * MimeoConfig
     A MimeoDTO class representing Mimeo Configuration
+* MimeoConfigFactory
+    A factory class to instantiate a MimeoConfig
 
 To use this package, simply import it:
-    from mimeo.config import MimeoConfig
+    from mimeo.config import MimeoConfigFactory, MimeoConfig
     from mimeo.config import constants as cc
     from mimeo.config.exc import UnsupportedPropertyValueError
 """
 from __future__ import annotations
 
-from .mimeo_config import MimeoConfig
+from .mimeo_config import MimeoConfig, MimeoConfigFactory
 
-__all__ = ["MimeoConfig"]
+__all__ = ["MimeoConfig", "MimeoConfigFactory"]
```

### Comparing `mimeograph-0.6.0/src/mimeo/config/constants.py` & `mimeograph-0.7.0/src/mimeo/config/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """The Mimeo Configuration Constants module."""
+from __future__ import annotations
+
 import yaml
 
 from mimeo import tools
 
 with tools.get_resource("constants.yaml") as config_file:
     constants = yaml.safe_load(config_file.read())
     _cc = constants["mimeo-config"]
 
+CONFIG_XML_ROOT_NAME = _cc["key"]
+
 ########################################################################################
 #                                    OUTPUT DETAILS                                    #
 ########################################################################################
 _output_constants = _cc["output"]
 OUTPUT_KEY = _output_constants["key"]
 OUTPUT_FORMAT_KEY = _output_constants["format"]["key"]
 OUTPUT_DIRECTION_KEY = _output_constants["direction"]["key"]
@@ -72,27 +76,29 @@
 VARS_KEY = _vars_constants["key"]
 
 ########################################################################################
 #                                   MIMEO TEMPLATES                                    #
 ########################################################################################
 _templates_constants = _cc["templates"]
 TEMPLATES_KEY = _templates_constants["key"]
+TEMPLATES_XML_TEMPLATE_TAG = _templates_constants["xml-template-tag"]["key"]
 TEMPLATES_COUNT_KEY = _templates_constants["count"]["key"]
 TEMPLATES_MODEL_KEY = _templates_constants["model"]["key"]
 
 ########################################################################################
 # -------------------------------- Mimeo Model level --------------------------------- #
 _model_constants = _templates_constants["model"]
 MODEL_CONTEXT_KEY = _model_constants["context"]["key"]
 MODEL_ATTRIBUTES_KEY = _model_constants["attributes"]["key"]
-MODEL_VALUE_KEY = _model_constants["text-node-value"]["key"]
+MODEL_TEXT_VALUE_KEY = _model_constants["text-node-value"]["key"]
 MODEL_MIMEO_UTIL_KEY = _model_constants["mimeo-util"]["key"]
 MODEL_MIMEO_UTIL_NAME_KEY = _model_constants["mimeo-util"]["name"]["key"]
 
 __all__ = [
+    "CONFIG_XML_ROOT_NAME",
     "OUTPUT_KEY",
     "OUTPUT_FORMAT_KEY",
     "OUTPUT_DIRECTION_KEY",
     "SUPPORTED_OUTPUT_FORMATS",
     "OUTPUT_FORMAT_XML",
     "OUTPUT_XML_DECLARATION_KEY",
     "OUTPUT_INDENT_KEY",
@@ -114,15 +120,16 @@
     "OUTPUT_HTTP_REQUEST_POST",
     "OUTPUT_HTTP_REQUEST_PUT",
     "SUPPORTED_REQUEST_PROTOCOLS",
     "OUTPUT_PROTOCOL_HTTP",
     "OUTPUT_PROTOCOL_HTTPS",
     "VARS_KEY",
     "TEMPLATES_KEY",
+    "TEMPLATES_XML_TEMPLATE_TAG",
     "TEMPLATES_COUNT_KEY",
     "TEMPLATES_MODEL_KEY",
     "MODEL_CONTEXT_KEY",
     "MODEL_ATTRIBUTES_KEY",
-    "MODEL_VALUE_KEY",
+    "MODEL_TEXT_VALUE_KEY",
     "MODEL_MIMEO_UTIL_KEY",
     "MODEL_MIMEO_UTIL_NAME_KEY",
 ]
```

### Comparing `mimeograph-0.6.0/src/mimeo/config/exc.py` & `mimeograph-0.7.0/src/mimeo/config/exc.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,20 +17,25 @@
         An Enumeration class for InvalidMimeoModelError error codes.
     * InvalidMimeoTemplateError
         A custom Exception class for invalid template configuration.
     * InvalidMimeoConfigError
         A custom Exception class for invalid mimeo configuration.
     * InvalidMimeoConfigError.Code
         An Enumeration class for InvalidMimeoConfigError error codes.
+    * UnsupportedMimeoConfigSourceError
+        A custom Exception class for unsupported Mimeo Configuration source.
+    * MimeoConfigurationNotFoundError
+        A custom Exception class for no mimeo_configuration node in source xml.
 """
 
 
 from __future__ import annotations
 
 from enum import Enum
+from typing import Any
 
 
 class UnsupportedPropertyValueError(Exception):
     """A custom Exception class for unsupported properties' values.
 
     Raised when a Mimeo Configuration property points to a value
     not being supported by Mimeo.
@@ -362,7 +367,53 @@
         if code == cls.Code.ERR_1:
             return f"No templates in the Mimeo Config: {details['config']}"
         if code == cls.Code.ERR_2:
             return f"_templates_ property does not store an array: {details['config']}"
 
         msg = f"Provided error code is not a {cls.__name__}.Code enum!"
         raise ValueError(msg)
+
+
+class UnsupportedMimeoConfigSourceError(Exception):
+    """A custom Exception class for unsupported Mimeo Configuration source.
+
+    Raised when an XML Mimeo Configuration's source is neither a dict nor str.
+    """
+
+    def __init__(
+            self,
+            source: Any,
+    ):
+        """Initialize UnsupportedMimeoConfigSourceError exception with details.
+
+        Extends Exception constructor with a custom message.
+
+        Parameters
+        ----------
+        source : Any
+            An actual root name
+        """
+        super().__init__(f"Mimeo Configuration source [{source}] is unsupported. "
+                         "Use a file path, stringified configuration or a dictionary.")
+
+
+class MimeoConfigurationNotFoundError(Exception):
+    """A custom Exception class for no mimeo_configuration node in source xml.
+
+    Raised when an XML Mimeo Configuration's root node is not <mimeo_configuration/>.
+    """
+
+    def __init__(
+            self,
+            root_name: str,
+    ):
+        """Initialize MimeoConfigurationNotFoundError exception with details.
+
+        Extends Exception constructor with a custom message.
+
+        Parameters
+        ----------
+        root_name : str
+            An actual root name
+        """
+        super().__init__(f"<mimeo_configuration/> not found! {root_name} is not "
+                         f"a proper Mimeo Configuration root node.")
```

### Comparing `mimeograph-0.6.0/src/mimeo/consumers/__init__.py` & `mimeograph-0.7.0/src/mimeo/consumers/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/consumers/consumer.py` & `mimeograph-0.7.0/src/mimeo/consumers/consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/consumers/consumer_factory.py` & `mimeograph-0.7.0/src/mimeo/consumers/consumer_factory.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/consumers/file_consumer.py` & `mimeograph-0.7.0/src/mimeo/consumers/file_consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/consumers/http_consumer.py` & `mimeograph-0.7.0/src/mimeo/consumers/http_consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/consumers/raw_consumer.py` & `mimeograph-0.7.0/src/mimeo/consumers/raw_consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/context/__init__.py` & `mimeograph-0.7.0/src/mimeo/context/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/context/decorators.py` & `mimeograph-0.7.0/src/mimeo/context/decorators.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/context/exc.py` & `mimeograph-0.7.0/src/mimeo/context/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/context/mimeo_context.py` & `mimeograph-0.7.0/src/mimeo/context/mimeo_context.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/context/mimeo_context_manager.py` & `mimeograph-0.7.0/src/mimeo/context/mimeo_context_manager.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/context/mimeo_iteration.py` & `mimeograph-0.7.0/src/mimeo/context/mimeo_iteration.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/database/__init__.py` & `mimeograph-0.7.0/src/mimeo/database/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/database/cities.py` & `mimeograph-0.7.0/src/mimeo/database/cities.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/database/countries.py` & `mimeograph-0.7.0/src/mimeo/database/countries.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/database/currencies.py` & `mimeograph-0.7.0/src/mimeo/database/currencies.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/database/exc.py` & `mimeograph-0.7.0/src/mimeo/database/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/database/first_names.py` & `mimeograph-0.7.0/src/mimeo/database/first_names.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/database/last_names.py` & `mimeograph-0.7.0/src/mimeo/database/last_names.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/database/mimeo_db.py` & `mimeograph-0.7.0/src/mimeo/database/mimeo_db.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/generators/__init__.py` & `mimeograph-0.7.0/src/mimeo/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/generators/exc.py` & `mimeograph-0.7.0/src/mimeo/generators/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/generators/generator.py` & `mimeograph-0.7.0/src/mimeo/generators/generator.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/generators/generator_factory.py` & `mimeograph-0.7.0/src/mimeo/generators/generator_factory.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/generators/xml_generator.py` & `mimeograph-0.7.0/src/mimeo/generators/xml_generator.py`

 * *Files 9% similar despite different names*

```diff
@@ -246,19 +246,19 @@
     ) -> dict:
         """Pre-process element's metadata.
 
         This function adjusts existing element's metadata and completes it with custom
         properties:
         * the tag property is changed only for special fields
           - field name is extracted
-        * the value property is being modified for dicts including '_attrs' key
-          - the 'attrs' key is removed from the dict
+        * the value property is being modified for dicts including attributes
+          - properties starting with '@' are being removed from the dict
         * the attrs property
-          - takes the '_attrs' property value from dicts including '_attrs' key
-          - takes the default value (an empty dict) when is None
+          - is being populated by all properties starting with '@'
+          - takes the default value (an empty dict) when there's no such properties
         * the mimeo_util property is being initialized
           - True if element's value is a parametrized mimeo_util. Otherwise, False.
         * the special property is being initialized
           - True, when a field is special. Otherwise, False.
 
         Parameters
         ----------
@@ -268,25 +268,25 @@
         Returns
         -------
         dict
             Complete element's metadata
         """
         tag = element_meta["tag"]
         value = element_meta["value"]
-        attrs = element_meta["attrs"]
+        attrs = {}
         is_mimeo_util = MimeoRenderer.is_parametrized_mimeo_util(value)
         is_special_field = MimeoRenderer.is_special_field(tag)
         if is_special_field:
             tag = MimeoRenderer.get_special_field_name(tag)
-        if isinstance(value, dict) and cc.MODEL_ATTRIBUTES_KEY in value:
-            value = dict(value)
-            attrs = value.pop(cc.MODEL_ATTRIBUTES_KEY)
-            value = value.get(cc.MODEL_VALUE_KEY, value)
-        if attrs is None:
-            attrs = {}
+        if isinstance(value, dict):
+            value_copy = dict(value)
+            for prop in value:
+                if prop.startswith(cc.MODEL_ATTRIBUTES_KEY):
+                    attrs[prop[1:]] = value_copy.pop(prop)
+            value = value.get(cc.MODEL_TEXT_VALUE_KEY, value_copy)
 
         return cls._element_meta(
             tag,
             value,
             attrs,
             is_mimeo_util,
             is_special_field)
@@ -407,15 +407,16 @@
     def _process_list_value(
             cls,
             parent: ElemTree.Element,
             element_meta: dict,
     ) -> ElemTree.Element:
         """Process a node with a list value.
 
-        The node is processed accordingly to its children types.
+        It iterates through the list items and processes each of them: generates
+        a child element for each value as direct children of the parent.
 
         Parameters
         ----------
         parent : ElemTree.Element | None
             A parent node
         element_meta : dict
             Element's metadata
@@ -424,148 +425,52 @@
         -------
         ElemTree.Element
             A processed node
 
         Raises
         ------
         UnsupportedStructureError
-            If the list value elements are not atomic-only or dict-only.
+            If any of the list value element is a list.
         InvalidSpecialFieldValueError
             If the special field value is dict or list
         SpecialFieldNotFoundError
             If the special field does not exist.
-        """
-        has_only_atomic_values = all(
-            not isinstance(child, (list, dict)) or
-            MimeoRenderer.is_parametrized_mimeo_util(child)
-            for child in element_meta["value"])
-        if has_only_atomic_values:
-            return cls._process_list_value_with_atomic_children(parent, element_meta)
-
-        has_only_dict_values = all(
-            isinstance(child, dict) and
-            not MimeoRenderer.is_parametrized_mimeo_util(child)
-            for child in element_meta["value"])
-        if has_only_dict_values:
-            return cls._process_list_value_with_complex_children(parent, element_meta)
-
-        raise UnsupportedStructureError(element_meta["tag"], element_meta["value"])
-
-    @classmethod
-    def _process_list_value_with_atomic_children(
-            cls,
-            parent: ElemTree.Element,
-            element_meta: dict,
-    ) -> ElemTree.Element:
-        """Process a node with a list value having atomic children.
-
-        This method generates a child element for each atomic value as direct children
-        of the parent.
-
-        Parameters
-        ----------
-        parent : ElemTree.Element | None
-            A parent node
-        element_meta : dict
-            Element's metadata
-
-        Returns
-        -------
-        ElemTree.Element
-            A processed node
-
-        Raises
-        ------
-        UnsupportedStructureError
-            If a list value elements are not atomic-only or dict-only.
-        InvalidSpecialFieldValueError
-            If a special field value is dict or list
-        SpecialFieldNotFoundError
-            If a special field does not exist.
 
         Examples
         --------
         parent = ElemTree.Element("Root")
         element_meta = cls._element_meta(
             tag="SomeField",
-            value=[],
+            value=[
+                'value-1',
+                {'SomeChild1': True, 'SomeChild2': False},
+                {'_mimeo_util': {'_name': 'auto_increment', 'pattern': '{}'}}
+            ],
         )
         cls._process_list_value_with_atomic_children(parent, element_meta)
         ->
         <Root>
+            <SomeField>value-1</SomeField>
+            <SomeField>
+                <SomeChild1>true</SomeChild1>
+                <SomeChild2>false</SomeChild2>
+            </SomeField>
             <SomeField>1</SomeField>
-            <SomeField>2</SomeField>
         </Root>
         """
         for child in element_meta["value"]:
+            if isinstance(child, list):
+                raise UnsupportedStructureError(
+                    element_meta["tag"],
+                    element_meta["value"])
             element_meta = cls._element_meta(element_meta["tag"], child)
             cls._process_node(parent, element_meta)
         return parent
 
     @classmethod
-    def _process_list_value_with_complex_children(
-            cls,
-            parent: ElemTree.Element,
-            element_meta: dict,
-    ) -> ElemTree.Element:
-        """Process a node with a list value having complex children.
-
-        It iterates through the list items and processes each of them.
-
-        Parameters
-        ----------
-        parent : ElemTree.Element | None
-            A parent node
-        element_meta : dict
-            Element's metadata
-
-        Returns
-        -------
-        ElemTree.Element
-            A processed node
-
-        Raises
-        ------
-        UnsupportedStructureError
-            If a list value elements are not atomic-only or dict-only.
-        InvalidSpecialFieldValueError
-            If a special field value is dict or list
-        SpecialFieldNotFoundError
-            If a special field does not exist.
-
-        Examples
-        --------
-        parent = ElemTree.Element("Root")
-        element_meta = cls._element_meta(
-            tag="SomeField",
-            value=[{"SomeChild": {"SomeGrandChild1": 1, "SomeGrandChild2": 2}},
-                   {"SomeChild": {"SomeGrandChild1": 'A', "SomeGrandChild2": 'B'}}],
-        )
-        cls._process_list_value_with_complex_children(parent, element_meta)
-        ->
-        <SomeField>
-            <SomeChild>
-                <SomeGrandChild1>1</SomeGrandChild1>
-                <SomeGrandChild2>2</SomeGrandChild2>
-            </SomeChild>
-            <SomeChild>
-                <SomeGrandChild1>A</SomeGrandChild1>
-                <SomeGrandChild2>B</SomeGrandChild2>
-            </SomeChild>
-        </SomeField>
-        """
-        element = cls._create_xml_element(parent, element_meta)
-        for child in element_meta["value"]:
-            grand_child_tag = next(iter(child))
-            grand_child_data = child[grand_child_tag]
-            element_meta = cls._element_meta(grand_child_tag, grand_child_data)
-            cls._process_node(element, element_meta)
-        return element
-
-    @classmethod
     def _process_templates_value(
             cls,
             parent: ElemTree.Element,
             element_meta: dict,
     ) -> ElemTree.Element:
         """Process a node with a dictionary value storing templates.
```

### Comparing `mimeograph-0.6.0/src/mimeo/logging/__init__.py` & `mimeograph-0.7.0/src/mimeo/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/logging/filters.py` & `mimeograph-0.7.0/src/mimeo/logging/filters.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/meta/__init__.py` & `mimeograph-0.7.0/src/mimeo/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/meta/alive.py` & `mimeograph-0.7.0/src/mimeo/meta/alive.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/meta/exc.py` & `mimeograph-0.7.0/src/mimeo/meta/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/mimeo.py` & `mimeograph-0.7.0/src/mimeo/mimeo.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/resources/cities.csv` & `mimeograph-0.7.0/src/mimeo/resources/cities.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/resources/constants.yaml` & `mimeograph-0.7.0/src/mimeo/resources/constants.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 ---
 mimeo-config:
+  key: mimeo_configuration
+
   output:
     key: output
 
     direction:
       key: direction
       values:
         std-out:
@@ -58,22 +60,25 @@
   vars:
     key: vars
 
 
   templates:
     key: _templates_
 
+    xml-template-tag:
+      key: _template_
+
     count:
       key: count
 
     model:
       key: model
       context:
         key: context
       attributes:
-        key: _attrs
+        key: "@"
       text-node-value:
-        key: _value
+        key: "#text"
       mimeo-util:
         key: _mimeo_util
         name:
           key: _name
```

### Comparing `mimeograph-0.6.0/src/mimeo/resources/countries.csv` & `mimeograph-0.7.0/src/mimeo/resources/countries.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/resources/currencies.csv` & `mimeograph-0.7.0/src/mimeo/resources/currencies.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/resources/exc.py` & `mimeograph-0.7.0/src/mimeo/resources/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/resources/forenames.csv` & `mimeograph-0.7.0/src/mimeo/resources/forenames.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/resources/logging.yaml` & `mimeograph-0.7.0/src/mimeo/resources/logging.yaml`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/resources/surnames.txt` & `mimeograph-0.7.0/src/mimeo/resources/surnames.txt`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/tools.py` & `mimeograph-0.7.0/src/mimeo/tools.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/utils/__init__.py` & `mimeograph-0.7.0/src/mimeo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/utils/exc.py` & `mimeograph-0.7.0/src/mimeo/utils/exc.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,9 +201,9 @@
         Extends Exception constructor with a custom message.
 
         Parameters
         ----------
         field_name : str
             A field name
         """
-        msg = f"Provided field [{field_name}] is not a special one (use {'{:NAME:}'})!"
+        msg = f"Provided field [{field_name}] is not a special one (use {':NAME:'})!"
         super().__init__(msg)
```

### Comparing `mimeograph-0.6.0/src/mimeo/utils/mimeo_utils.py` & `mimeograph-0.7.0/src/mimeo/utils/mimeo_utils.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/src/mimeo/utils/renderers.py` & `mimeograph-0.7.0/src/mimeo/utils/renderers.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,50 +351,50 @@
     ) -> str:
         """Extract a special field name.
 
         Parameters
         ----------
         wrapped_field_name : str
             A field name wrapped with curly braces and colons,
-            e.g. {:Field:}
+            e.g. :Field:
 
         Returns
         -------
         str
             A special field name
 
         Raises
         ------
         NotASpecialFieldError
-            If the `wrapped_field_name` is not of form {:FIELD_NAME:}
+            If the `wrapped_field_name` is not of form :FIELD_NAME:
         """
         if not cls.is_special_field(wrapped_field_name):
             raise NotASpecialFieldError(wrapped_field_name)
 
-        return wrapped_field_name[2:][:-2]
+        return wrapped_field_name[1:][:-1]
 
     @classmethod
     def is_special_field(
             cls,
             special_field: str,
     ) -> bool:
-        """Verify if the field is special (of form {:FIELD_NAME:}).
+        """Verify if the field is special (of form :FIELD_NAME:).
 
         Parameters
         ----------
         special_field : str
             A special field
 
         Returns
         -------
         bool
-            True if the field is of form {:FIELD_NAME:}. Otherwise,
+            True if the field is of form :FIELD_NAME:. Otherwise,
             False.
         """
-        return bool(re.match(r"^{:([a-zA-Z]+:)?[-_a-zA-Z0-9]+:}$", special_field))
+        return bool(re.match(r"^:([a-zA-Z]+:)?[-_a-zA-Z0-9]+:$", special_field))
 
     @classmethod
     def is_raw_mimeo_util(
             cls,
             value: str,
     ) -> bool:
         """Verify if the value is a raw Mimeo Util.
```

### Comparing `mimeograph-0.6.0/src/mimeograph.egg-info/PKG-INFO` & `mimeograph-0.7.0/src/mimeograph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimeograph
-Version: 0.6.0
+Version: 0.7.0
 Summary: Generate data based on a simple template
 Author-email: "T.A. Programming Svcs." <tomasz.maciej.aniolowski@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tomasz Aniołowski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -70,74 +70,97 @@
 
 
 ## Usage/Examples
 
 ### Mimeo Configuration
 
 Prepare Mimeo Configuration first
-- for a command line tool: in a JSON file
-- for a `Mimeograph` python class: in a `dict`
+- for a command line tool: in a JSON or XML file
+- for a `Mimeograph` python class: in a `dict` or stringified XML
 
 ```json
 {
   "_templates_": [
     {
       "count": 30,
       "model": {
         "SomeEntity": {
-          "_attrs": {
-            "xmlns": "http://mimeo.arch.com/default-namespace",
-            "xmlns:pn": "http://mimeo.arch.com/prefixed-namespace"
-          },
+          "@xmlns": "http://mimeo.arch.com/default-namespace",
+          "@xmlns:pn": "http://mimeo.arch.com/prefixed-namespace",
           "ChildNode1": 1,
           "ChildNode2": "value-2",
           "ChildNode3": true
         }
       }
     }
   ]
 }
 ```
+```xml
+<mimeo_configuration>
+    <_templates_>
+        <_template_>
+            <count>30</count>
+            <model>
+
+                <SomeEntity
+                    xmlns="http://mimeo.arch.com/default-namespace"
+                    xmlns:pn="http://mimeo.arch.com/prefixed-namespace">
+                    <ChildNode1>1</ChildNode1>
+                    <pn:ChildNode2>value-2</pn:ChildNode2>
+                    <ChildNode3>true</ChildNode3>
+                </SomeEntity>
+
+            </model>
+        </_template_>
+    </_templates_>
+</mimeo_configuration>
+```
 _You can find more configuration examples in the `examples` folder._
 
 ### Mimeograph
 
 #### Command line tool
 
 ```sh
 mimeo SomeEntity-config.json
+mimeo SomeEntity-config.xml
 ```
 
 #### Python library
 
 ```python
-from mimeo import MimeoConfig, Mimeograph
+from mimeo import MimeoConfigFactory, Mimeograph
 
 config = {
-    # Your configuration
+    # Your configuration in a dict
 }
-mimeo_config = MimeoConfig(config)
+config = """
+    Your configuration in a stringified XML node
+"""
+config = ""  # A file path to your configuration (JSON / XML)
+mimeo_config = MimeoConfigFactory.parse(config)
 Mimeograph(mimeo_config).process()
 ```
 ***
 The Mimeo Configuration above will produce 2 files:
 
 ```xml
 <!-- mimeo-output/mimeo-output-1.xml-->
 <SomeEntity xmlns="http://mimeo.arch.com/default-namespace" xmlns:pn="http://mimeo.arch.com/prefixed-namespace">
     <ChildNode1>1</ChildNode1>
-    <ChildNode2>value-2</ChildNode2>
+    <pn:ChildNode2>value-2</pn:ChildNode2>
     <ChildNode3>true</ChildNode3>
 </SomeEntity>
 ```
 ```xml
 <!-- mimeo-output/mimeo-output-2.xml-->
 <SomeEntity xmlns="http://mimeo.arch.com/default-namespace" xmlns:pn="http://mimeo.arch.com/prefixed-namespace">
     <ChildNode1>1</ChildNode1>
-    <ChildNode2>value-2</ChildNode2>
+    <pn:ChildNode2>value-2</pn:ChildNode2>
     <ChildNode3>true</ChildNode3>
 </SomeEntity>
 ```
 ***
 
 ### Mimeo Utils
 
@@ -152,14 +175,28 @@
       "id": "{auto_increment}",
       "randomstring": "{random_str}",
       "randomint": "{random_int}"
     }
   }
 }
 ```
+```xml
+<_template_>
+    <count>2</count>
+    <model>
+        
+        <SomeEntity>
+            <id>{auto_increment}</id>
+            <randomstring>{random_str}</randomstring>
+            <randomint>{random_int}</randomint>
+        </SomeEntity>
+        
+    </model>
+</_template_>
+```
 
 **XML Data**
 ```xml
 <SomeEntity>
     <id>00001</id>
     <randomstring>mCApsYZprayYkmKnYWxe</randomstring>
     <randomint>8</randomint>
@@ -178,30 +215,30 @@
 
 ### Mimeo CLI
 
 #### Mimeo Configuration arguments
 
 When using Mimeo command line tool you can overwrite Mimeo Configuration properties:
 
-| Short option | Long option         | Description                                                                  |
-|:------------:|:--------------------|:-----------------------------------------------------------------------------|
+| Short option | Long option         | Description                                                          |
+|:------------:|:--------------------|:---------------------------------------------------------------------|
 |     `-o`     | `--output`          | overwrite the `output/direction` property                            |
 |     `-x`     | `--xml-declaration` | overwrite the `output/xml_declaration` property                      |
 |     `-i`     | `--indent`          | overwrite the `output/indent` property                               |
 |     `-d`     | `--directory`       | overwrite the `output/directory_path` property                       |
 |     `-f`     | `--file`            | overwrite the `output/file_name` property                            |
 |     `-H`     | `--http-host`       | overwrite the `output/host` property                                 |
 |     `-p`     | `--http-port`       | overwrite the `output/port` property                                 |
 |     `-E`     | `--http-endpoint`   | overwrite the `output/endpoint` property                             |
 |     `-U`     | `--http-user`       | overwrite the `output/username` property                             |
 |     `-P`     | `--http-password`   | overwrite the `output/password` property                             |
 |              | `--http-method`     | overwrite the `output/method` property                               |
 |              | `--http-protocol`   | overwrite the `output/protocol` property                             |
 |     `-e`     | `--http-env`        | overwrite the output http properties using a mimeo env configuration |
-|              | `--http-envs-file`  | use a custom environments file (by default: mimeo.envs.json)                 |
+|              | `--http-envs-file`  | use a custom environments file (by default: mimeo.envs.json)         |
 
 #### Logging arguments
 
 | Short option | Long option | Description       |
 |:------------:|:------------|:------------------|
 |              | `--silent`  | disable INFO logs |
 |              | `--debug`   | enable DEBUG mode |
@@ -319,28 +356,27 @@
 }
 ```
 
 #### Mimeo Special Fields
 
 In Mimeo Template you can use so-called _special fields_.
 Every field in a template can be stored in memory (_provided_) and used later as a value of other fields (_injected_).
-To provide and inject a special field use curly brackets and colons: [`{:SomeField:}`].
-You provide a field when you use this format in a field name (JSON property name),
-and inject by applying it in a field value.  
+To provide a special field, wrap its name with colons: [`:SomeField:`]. To inject, use additionally curly braces to
+let interpreter know it should be rendered [`{:SomeField:}`].
 They can be injected as partial values, similarly to Mimeo Vars.
 
 Example
 ```json
 {
   "_templates_": [
     {
       "count": 5,
       "model": {
         "SomeEntity": {
-          "{:ChildNode1:}": "custom-value",
+          ":ChildNode1:": "custom-value",
           "ChildNode2": "{:ChildNode1:}",
           "ChildNode3": "{:ChildNode1:}-with-suffix"
         }
       }
     }
   ]
 }
```

### Comparing `mimeograph-0.6.0/src/mimeograph.egg-info/SOURCES.txt` & `mimeograph-0.7.0/src/mimeograph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mimeograph-0.6.0/tests/test_mimeograph.py` & `mimeograph-0.7.0/tests/test_mimeograph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import shutil
 from pathlib import Path
 
 import pytest
 
 from mimeo import Mimeograph
-from mimeo.config import MimeoConfig
+from mimeo.config import MimeoConfigFactory
 from mimeo.context import MimeoContextManager
 
 
 @pytest.fixture(autouse=True)
 def _teardown():
     yield
     # Teardown
@@ -35,15 +35,15 @@
                         "ChildNode2": "value-2",
                         "ChildNode3": True,
                     },
                 },
             },
         ],
     }
-    mimeo_config = MimeoConfig(config)
+    mimeo_config = MimeoConfigFactory.parse(config)
     with MimeoContextManager(mimeo_config):
         mimeo = Mimeograph(mimeo_config)
 
         assert not Path("test_mimeograph-dir").exists()
         await mimeo.process()
         assert Path("test_mimeograph-dir").exists()
         for i in range(1, 11):
```

