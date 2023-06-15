# Comparing `tmp/spetlr-tools-0.1.33.tar.gz` & `tmp/spetlr-tools-0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spetlr-tools-0.1.33.tar", last modified: Wed Jun  7 16:09:23 2023, max compression
+gzip compressed data, was "spetlr-tools-0.1.34.tar", last modified: Thu Jun 15 08:47:35 2023, max compression
```

## Comparing `spetlr-tools-0.1.33.tar` & `spetlr-tools-0.1.34.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.897007 spetlr-tools-0.1.33/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-07 16:09:23.897007 spetlr-tools-0.1.33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-07 16:09:23.897007 spetlr-tools-0.1.33/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.877006 spetlr-tools-0.1.33/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.881006 spetlr-tools-0.1.33/src/spetlr_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-07 16:09:23.000000 spetlr-tools-0.1.33/src/spetlr_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-07 16:09:23.000000 spetlr-tools-0.1.33/src/spetlr_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:09:23.000000 spetlr-tools-0.1.33/src/spetlr_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-07 16:09:23.000000 spetlr-tools-0.1.33/src/spetlr_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:09:23.000000 spetlr-tools-0.1.33/src/spetlr_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-07 16:09:23.000000 spetlr-tools-0.1.33/src/spetlr_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 16:09:23.000000 spetlr-tools-0.1.33/src/spetlr_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.885006 spetlr-tools-0.1.33/src/spetlrtools/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.885006 spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/AuthLinkOpener.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/get_ad_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/get_impersonation_authorization_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.889007 spetlr-tools-0.1.33/src/spetlrtools/diagrams/
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/diagrams/DiagramMarkupLibraryParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/diagrams/DrawioDiagramParser.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/diagrams/Edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/diagrams/HTMLStripper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/diagrams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/diagrams/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.889007 spetlr-tools-0.1.33/src/spetlrtools/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/entry_points/task_entry_point_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.889007 spetlr-tools-0.1.33/src/spetlrtools/format/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/format/validate_camelcased_cols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.889007 spetlr-tools-0.1.33/src/spetlrtools/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/helpers/ExtractEncodedBody.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/helpers/get_difference_between_two_dfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/helpers/module_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/manipulate_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.893007 spetlr-tools-0.1.33/src/spetlrtools/test_job/
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/test_job/RunDetails.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/test_job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/test_job/dbcli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/test_job/dbfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/test_job/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/test_job/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/test_job/submit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/test_job/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.893007 spetlr-tools-0.1.33/src/spetlrtools/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/testing/DataframeTestCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/testing/TestHandle.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:09:23.897007 spetlr-tools-0.1.33/src/spetlrtools/time/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/time/TimeSequence.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-07 16:09:10.000000 spetlr-tools-0.1.33/src/spetlrtools/time/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:47:35.120368 spetlr-tools-0.1.34/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-15 08:47:35.120368 spetlr-tools-0.1.34/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-15 08:47:35.124368 spetlr-tools-0.1.34/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:47:35.116368 spetlr-tools-0.1.34/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:47:35.116368 spetlr-tools-0.1.34/src/spetlr_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-15 08:47:34.000000 spetlr-tools-0.1.34/src/spetlr_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-15 08:47:35.000000 spetlr-tools-0.1.34/src/spetlr_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 08:47:34.000000 spetlr-tools-0.1.34/src/spetlr_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-15 08:47:34.000000 spetlr-tools-0.1.34/src/spetlr_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 08:47:34.000000 spetlr-tools-0.1.34/src/spetlr_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-15 08:47:34.000000 spetlr-tools-0.1.34/src/spetlr_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 08:47:34.000000 spetlr-tools-0.1.34/src/spetlr_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:47:35.120368 spetlr-tools-0.1.34/src/spetlrtools/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:47:35.120368 spetlr-tools-0.1.34/src/spetlrtools/az_databricks_token/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/az_databricks_token/AuthLinkOpener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/az_databricks_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/az_databricks_token/get_ad_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/az_databricks_token/get_impersonation_authorization_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/az_databricks_token/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/az_databricks_token/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:47:35.120368 spetlr-tools-0.1.34/src/spetlrtools/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/diagrams/DiagramMarkupLibraryParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/diagrams/DrawioDiagramParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/diagrams/Edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/diagrams/HTMLStripper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/diagrams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/diagrams/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:47:35.120368 spetlr-tools-0.1.34/src/spetlrtools/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/entry_points/task_entry_point_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:47:35.120368 spetlr-tools-0.1.34/src/spetlrtools/format/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/format/validate_camelcased_cols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:47:35.120368 spetlr-tools-0.1.34/src/spetlrtools/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/helpers/ExtractEncodedBody.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/helpers/get_difference_between_two_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/helpers/module_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/manipulate_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:47:35.120368 spetlr-tools-0.1.34/src/spetlrtools/test_job/
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/test_job/RunDetails.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/test_job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/test_job/dbcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/test_job/dbfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/test_job/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/test_job/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11987 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/test_job/submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/test_job/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:47:35.120368 spetlr-tools-0.1.34/src/spetlrtools/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/testing/DataframeTestCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/testing/TestHandle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:47:35.120368 spetlr-tools-0.1.34/src/spetlrtools/time/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/time/TimeSequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-15 08:47:21.000000 spetlr-tools-0.1.34/src/spetlrtools/time/__init__.py
```

### Comparing `spetlr-tools-0.1.33/LICENSE` & `spetlr-tools-0.1.34/LICENSE`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/PKG-INFO` & `spetlr-tools-0.1.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spetlr-tools
-Version: 0.1.33
+Version: 0.1.34
 Summary: Supplements to the python SPark ETL libRary (SPETLR) for Databricks.
 Home-page: https://github.com/spetlr-org/spetlr-tools
 Author: Spetlr.Org
 Author-email: spetlr.org@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/spetlr-org/spetlr-tools
 Project-URL: Bug Reports, https://github.com/spetlr-org/spetlr-tools/issues
```

### Comparing `spetlr-tools-0.1.33/README.md` & `spetlr-tools-0.1.34/README.md`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/setup.cfg` & `spetlr-tools-0.1.34/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 	=src
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	spetlr
 	pyyaml==6.0
 	importlib_metadata
-	requests
+	requests<2.29.0,>=2.28.1  # required by databricks-sdk
 	dateparser
 	pytest
 	packaging
 	numpy<=1.24 # Numpy does not support 3.8 if above 1.24
 	urllib3<2.0.0
 
 [options.packages.find]
```

### Comparing `spetlr-tools-0.1.33/src/spetlr_tools.egg-info/PKG-INFO` & `spetlr-tools-0.1.34/src/spetlr_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spetlr-tools
-Version: 0.1.33
+Version: 0.1.34
 Summary: Supplements to the python SPark ETL libRary (SPETLR) for Databricks.
 Home-page: https://github.com/spetlr-org/spetlr-tools
 Author: Spetlr.Org
 Author-email: spetlr.org@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/spetlr-org/spetlr-tools
 Project-URL: Bug Reports, https://github.com/spetlr-org/spetlr-tools/issues
```

### Comparing `spetlr-tools-0.1.33/src/spetlr_tools.egg-info/SOURCES.txt` & `spetlr-tools-0.1.34/src/spetlr_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/AuthLinkOpener.py` & `spetlr-tools-0.1.34/src/spetlrtools/az_databricks_token/AuthLinkOpener.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/__init__.py` & `spetlr-tools-0.1.34/src/spetlrtools/az_databricks_token/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/get_ad_access_token.py` & `spetlr-tools-0.1.34/src/spetlrtools/az_databricks_token/get_ad_access_token.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/get_impersonation_authorization_code.py` & `spetlr-tools-0.1.34/src/spetlrtools/az_databricks_token/get_impersonation_authorization_code.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/main.py` & `spetlr-tools-0.1.34/src/spetlrtools/az_databricks_token/main.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/az_databricks_token/server.py` & `spetlr-tools-0.1.34/src/spetlrtools/az_databricks_token/server.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/diagrams/DiagramMarkupLibraryParser.py` & `spetlr-tools-0.1.34/src/spetlrtools/diagrams/DiagramMarkupLibraryParser.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/diagrams/DrawioDiagramParser.py` & `spetlr-tools-0.1.34/src/spetlrtools/diagrams/DrawioDiagramParser.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/diagrams/Edge.py` & `spetlr-tools-0.1.34/src/spetlrtools/diagrams/Edge.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/diagrams/HTMLStripper.py` & `spetlr-tools-0.1.34/src/spetlrtools/diagrams/HTMLStripper.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/diagrams/main.py` & `spetlr-tools-0.1.34/src/spetlrtools/diagrams/main.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/entry_points/task_entry_point_helper.py` & `spetlr-tools-0.1.34/src/spetlrtools/entry_points/task_entry_point_helper.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/format/validate_camelcased_cols.py` & `spetlr-tools-0.1.34/src/spetlrtools/format/validate_camelcased_cols.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/helpers/ExtractEncodedBody.py` & `spetlr-tools-0.1.34/src/spetlrtools/helpers/ExtractEncodedBody.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/helpers/get_difference_between_two_dfs.py` & `spetlr-tools-0.1.34/src/spetlrtools/helpers/get_difference_between_two_dfs.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/helpers/module_helper.py` & `spetlr-tools-0.1.34/src/spetlrtools/helpers/module_helper.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/manipulate_version.py` & `spetlr-tools-0.1.34/src/spetlrtools/manipulate_version.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/requirements.py` & `spetlr-tools-0.1.34/src/spetlrtools/requirements.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/test_job/RunDetails.py` & `spetlr-tools-0.1.34/src/spetlrtools/test_job/RunDetails.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/test_job/dbcli.py` & `spetlr-tools-0.1.34/src/spetlrtools/test_job/dbcli.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/test_job/dbfs.py` & `spetlr-tools-0.1.34/src/spetlrtools/test_job/dbfs.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/test_job/fetch.py` & `spetlr-tools-0.1.34/src/spetlrtools/test_job/fetch.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/test_job/submit.py` & `spetlr-tools-0.1.34/src/spetlrtools/test_job/submit.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 - return the ID - also to file
 """
 import argparse
 import copy
 import datetime
 import inspect
 import json
+import re
 import shutil
+import subprocess
 import tempfile
 import uuid
 from pathlib import Path
 from typing import List, Union
 from typing.io import IO
 
 from . import test_main
@@ -282,15 +284,15 @@
         if parallelize:
             # subtasks will be ['tests/cluster/job1', 'tests/cluster/job2'] or similar
             tasks = discover_job_tasks(test_path, task)
         else:
             tasks = [verify_and_resolve_task(test_path, task)]
 
         for task in tasks:
-            task_sub = task.replace("/", "_")
+            task_sub = re.sub(r"[^a-zA-Z0-9_-]", "_", task)
             task_cluster = copy.deepcopy(cluster)
             task_cluster["cluster_log_conf"] = {
                 "dbfs": {"destination": f"{test_folder.remote}/{task_sub}"}
             }
 
             workflow["tasks"].append(
                 dict(
@@ -310,19 +312,27 @@
                             # additional arguments to pass to pytest
                             f"--pytestargs={json.dumps(pytest_args)}",
                         ],
                     ),
                     new_cluster=task_cluster,
                 )
             )
+
     with tempfile.TemporaryDirectory() as tmp:
         jobfile = f"{tmp}/job.json"
         with open(jobfile, "w") as f:
             json.dump(workflow, f)
-        res = dbjcall(f"runs submit --json-file {jobfile}")
+
+        try:
+            res = dbjcall(f"runs submit --json-file {jobfile}")
+        except subprocess.CalledProcessError:
+            print("Json contents:")
+            print(json.dumps(workflow, indent=4))
+            raise
+
         try:
             run_id = res["run_id"]
         except KeyError:
             print(res)
             raise
 
     # now we have the run_id
```

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/test_job/test_main.py` & `spetlr-tools-0.1.34/src/spetlrtools/test_job/test_main.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/testing/DataframeTestCase.py` & `spetlr-tools-0.1.34/src/spetlrtools/testing/DataframeTestCase.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/testing/TestHandle.py` & `spetlr-tools-0.1.34/src/spetlrtools/testing/TestHandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-tools-0.1.33/src/spetlrtools/time/TimeSequence.py` & `spetlr-tools-0.1.34/src/spetlrtools/time/TimeSequence.py`

 * *Files identical despite different names*

