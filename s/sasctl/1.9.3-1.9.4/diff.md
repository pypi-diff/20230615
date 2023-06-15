# Comparing `tmp/sasctl-1.9.3.tar.gz` & `tmp/sasctl-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sasctl-1.9.3.tar", last modified: Thu Jun  8 18:32:49 2023, max compression
+gzip compressed data, was "sasctl-1.9.4.tar", last modified: Thu Jun 15 17:34:00 2023, max compression
```

## Comparing `sasctl-1.9.3.tar` & `sasctl-1.9.4.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.928073 sasctl-1.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)    19437 2023-06-08 18:32:36.000000 sasctl-1.9.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-08 18:32:36.000000 sasctl-1.9.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-06-08 18:32:36.000000 sasctl-1.9.3/ContributorAgreement.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 18:32:36.000000 sasctl-1.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-08 18:32:36.000000 sasctl-1.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-06-08 18:32:49.928073 sasctl-1.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-06-08 18:32:36.000000 sasctl-1.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-08 18:32:36.000000 sasctl-1.9.3/SUPPORT.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 18:32:49.928073 sasctl-1.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-08 18:32:36.000000 sasctl-1.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.912073 sasctl-1.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.916072 sasctl-1.9.3/src/sasctl/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.920072 sasctl-1.9.3/src/sasctl/_services/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/cas_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/concepts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/data_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/folders.py
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/microanalytic_score.py
--rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/model_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/model_publish.py
--rw-r--r--   0 runner    (1001) docker     (123)    28696 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/model_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/report_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/saslogon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/sentiment_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/text_categorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/text_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    74999 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.924072 sasctl-1.9.3/src/sasctl/pzmm/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17973 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/git_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/import_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/mlflow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/model_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/pickle_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.924072 sasctl-1.9.3/src/sasctl/pzmm/template_files/
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/template_files/dmcas_fitstat.json
--rw-r--r--   0 runner    (1001) docker     (123)    51874 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/template_files/dmcas_lift.json
--rw-r--r--   0 runner    (1001) docker     (123)   193713 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/template_files/dmcas_roc.json
--rw-r--r--   0 runner    (1001) docker     (123)    82560 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/write_json_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    63812 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/write_score_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/zip_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/services.py
--rw-r--r--   0 runner    (1001) docker     (123)    33574 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.924072 sasctl-1.9.3/src/sasctl/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16435 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/astore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/model_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.924072 sasctl-1.9.3/src/sasctl/utils/pymas/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pymas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22824 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pymas/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pymas/ds2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pymas/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.924072 sasctl-1.9.3/src/sasctl/utils/pyml2ds/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pyml2ds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.924072 sasctl-1.9.3/src/sasctl/utils/pyml2ds/basic/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pyml2ds/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pyml2ds/basic/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.924072 sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.928073 sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/ensembles/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/ensembles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/ensembles/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/ensembles/lgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/ensembles/pmml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/ensembles/xgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pyml2ds/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.916072 sasctl-1.9.3/src/sasctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-06-08 18:32:49.000000 sasctl-1.9.3/src/sasctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-08 18:32:49.000000 sasctl-1.9.3/src/sasctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:32:49.000000 sasctl-1.9.3/src/sasctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 18:32:49.000000 sasctl-1.9.3/src/sasctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-08 18:32:49.000000 sasctl-1.9.3/src/sasctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 18:32:49.000000 sasctl-1.9.3/src/sasctl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:34:00.191305 sasctl-1.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    20287 2023-06-15 17:33:51.000000 sasctl-1.9.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-15 17:33:51.000000 sasctl-1.9.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-06-15 17:33:51.000000 sasctl-1.9.4/ContributorAgreement.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 17:33:51.000000 sasctl-1.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-15 17:33:51.000000 sasctl-1.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-06-15 17:34:00.191305 sasctl-1.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-06-15 17:33:51.000000 sasctl-1.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-15 17:33:51.000000 sasctl-1.9.4/SUPPORT.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 17:34:00.191305 sasctl-1.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-15 17:33:51.000000 sasctl-1.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:34:00.183305 sasctl-1.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:34:00.183305 sasctl-1.9.4/src/sasctl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:34:00.187305 sasctl-1.9.4/src/sasctl/_services/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/_services/cas_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/_services/concepts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/_services/data_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/_services/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/_services/folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/_services/microanalytic_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/_services/model_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/_services/model_publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28696 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/_services/model_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/_services/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/_services/relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/_services/report_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/_services/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/_services/saslogon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/_services/sentiment_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/_services/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/_services/text_categorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/_services/text_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/_services/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74999 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:34:00.187305 sasctl-1.9.4/src/sasctl/pzmm/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/pzmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17973 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/pzmm/git_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/pzmm/import_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/pzmm/mlflow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/pzmm/model_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/pzmm/pickle_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:34:00.191305 sasctl-1.9.4/src/sasctl/pzmm/template_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/pzmm/template_files/dmcas_fitstat.json
+-rw-r--r--   0 runner    (1001) docker     (123)    51874 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/pzmm/template_files/dmcas_lift.json
+-rw-r--r--   0 runner    (1001) docker     (123)   193713 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/pzmm/template_files/dmcas_roc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    82560 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/pzmm/write_json_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63829 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/pzmm/write_score_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/pzmm/zip_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33574 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:34:00.191305 sasctl-1.9.4/src/sasctl/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16435 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/utils/astore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/utils/model_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:34:00.191305 sasctl-1.9.4/src/sasctl/utils/pymas/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/utils/pymas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22824 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/utils/pymas/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/utils/pymas/ds2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/utils/pymas/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:34:00.191305 sasctl-1.9.4/src/sasctl/utils/pyml2ds/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/utils/pyml2ds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:34:00.191305 sasctl-1.9.4/src/sasctl/utils/pyml2ds/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/utils/pyml2ds/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/utils/pyml2ds/basic/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:34:00.191305 sasctl-1.9.4/src/sasctl/utils/pyml2ds/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/utils/pyml2ds/connectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:34:00.191305 sasctl-1.9.4/src/sasctl/utils/pyml2ds/connectors/ensembles/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/utils/pyml2ds/connectors/ensembles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/utils/pyml2ds/connectors/ensembles/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/utils/pyml2ds/connectors/ensembles/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/utils/pyml2ds/connectors/ensembles/pmml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/utils/pyml2ds/connectors/ensembles/xgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-15 17:33:51.000000 sasctl-1.9.4/src/sasctl/utils/pyml2ds/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:34:00.187305 sasctl-1.9.4/src/sasctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-06-15 17:34:00.000000 sasctl-1.9.4/src/sasctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-15 17:34:00.000000 sasctl-1.9.4/src/sasctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 17:34:00.000000 sasctl-1.9.4/src/sasctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 17:34:00.000000 sasctl-1.9.4/src/sasctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-15 17:34:00.000000 sasctl-1.9.4/src/sasctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 17:34:00.000000 sasctl-1.9.4/src/sasctl.egg-info/top_level.txt
```

### Comparing `sasctl-1.9.3/CHANGELOG.md` & `sasctl-1.9.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 Unreleased
 ----------
 **Improvements**
  - Refactor `tasks.py` to utilize `sasctl.pzmm` functions.
  - Add `model_info` class to better capture model information.
+ - Test `/examples` Jupyter notebooks within normal test suite.
+
+v1.9.4 (2023-06-15)
+----------
+**Improvements**
+ - Created pytest fixture to begin running Jupyter notebooks within the GitHub automated test actions.
+ - Updated examples:
+   - Custom KPI and model parameters example now checks for the performance job's status.
+   - Update H2O example to show model being published and scored using the "maslocal" destination.
+   - Updated models to be more realistic for `pzmm_binary_classification_model_import.ipynb`.
+
+**Bugfixes**
+ - Adjust `pzmm.ScoreCode.write_score_code()` function to be compatible with future versions of pandas.
+ - Reworked H2O section of `pzmm.ScoreCode.write_score_code()` to properly call H2OFrame values.
+ - Fixed call to `pzmm.JSONFiles.calculate_model_statistics()` in `pzmm_binary_classification_model_import.ipynb`.
 
 v1.9.3 (2023-06-08)
 ----------
 **Improvements**
  - Refactored gitIntegration.py to `git_integration.py` and added unit tests for better test coverage.
 
 **Bugfixes**
```

### Comparing `sasctl-1.9.3/CONTRIBUTING.md` & `sasctl-1.9.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/ContributorAgreement.txt` & `sasctl-1.9.4/ContributorAgreement.txt`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/LICENSE` & `sasctl-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/PKG-INFO` & `sasctl-1.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sasctl
-Version: 1.9.3
+Version: 1.9.4
 Summary: SAS Viya Python Client
 Home-page: https://github.com/sassoftware/python-sasctl/
 Author: SAS
 License: Apache v2.0
 Project-URL: Bug Tracker, https://github.com/sassoftware/python-sasctl/issues
 Project-URL: Documentation, https://sassoftware.github.io/python-sasctl/
 Project-URL: Source Code, https://github.com/sassoftware/python-sasctl
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sasctl Version: 1.9.3 Summary: SAS Viya Python
+Metadata-Version: 2.1 Name: sasctl Version: 1.9.4 Summary: SAS Viya Python
 Client Home-page: https://github.com/sassoftware/python-sasctl/ Author: SAS
 License: Apache v2.0 Project-URL: Bug Tracker, https://github.com/sassoftware/
 python-sasctl/issues Project-URL: Documentation, https://sassoftware.github.io/
 python-sasctl/ Project-URL: Source Code, https://github.com/sassoftware/python-
 sasctl Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Environment ::
 Console Classifier: Intended Audience :: Science/Research Classifier: Intended
```

### Comparing `sasctl-1.9.3/README.md` & `sasctl-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/setup.py` & `sasctl-1.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/__init__.py` & `sasctl-1.9.4/src/sasctl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # encoding: utf-8
 #
 # Copyright © 2019, SAS Institute Inc., Cary, NC, USA.  All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 
-__version__ = "1.9.3"
+__version__ = "1.9.4"
 __author__ = "SAS"
 __credits__ = [
     "Yi Jian Ching",
     "Lucas De Paula",
     "James Kochuba",
     "Peter Tobac",
     "Chris Toth",
```

### Comparing `sasctl-1.9.3/src/sasctl/_services/cas_management.py` & `sasctl-1.9.4/src/sasctl/_services/cas_management.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/_services/concepts.py` & `sasctl-1.9.4/src/sasctl/_services/concepts.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/_services/data_sources.py` & `sasctl-1.9.4/src/sasctl/_services/data_sources.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/_services/files.py` & `sasctl-1.9.4/src/sasctl/_services/files.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/_services/folders.py` & `sasctl-1.9.4/src/sasctl/_services/folders.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/_services/microanalytic_score.py` & `sasctl-1.9.4/src/sasctl/_services/microanalytic_score.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/_services/model_management.py` & `sasctl-1.9.4/src/sasctl/_services/model_management.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/_services/model_publish.py` & `sasctl-1.9.4/src/sasctl/_services/model_publish.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/_services/model_repository.py` & `sasctl-1.9.4/src/sasctl/_services/model_repository.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/_services/projects.py` & `sasctl-1.9.4/src/sasctl/_services/projects.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/_services/relationships.py` & `sasctl-1.9.4/src/sasctl/_services/relationships.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/_services/report_images.py` & `sasctl-1.9.4/src/sasctl/_services/report_images.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/_services/reports.py` & `sasctl-1.9.4/src/sasctl/_services/reports.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/_services/saslogon.py` & `sasctl-1.9.4/src/sasctl/_services/saslogon.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/_services/sentiment_analysis.py` & `sasctl-1.9.4/src/sasctl/_services/sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/_services/service.py` & `sasctl-1.9.4/src/sasctl/_services/service.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/_services/text_categorization.py` & `sasctl-1.9.4/src/sasctl/_services/text_categorization.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/_services/text_parsing.py` & `sasctl-1.9.4/src/sasctl/_services/text_parsing.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/_services/workflow.py` & `sasctl-1.9.4/src/sasctl/_services/workflow.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/core.py` & `sasctl-1.9.4/src/sasctl/core.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/exceptions.py` & `sasctl-1.9.4/src/sasctl/exceptions.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/pzmm/git_integration.py` & `sasctl-1.9.4/src/sasctl/pzmm/git_integration.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/pzmm/import_model.py` & `sasctl-1.9.4/src/sasctl/pzmm/import_model.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/pzmm/mlflow_model.py` & `sasctl-1.9.4/src/sasctl/pzmm/mlflow_model.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/pzmm/model_parameters.py` & `sasctl-1.9.4/src/sasctl/pzmm/model_parameters.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/pzmm/pickle_model.py` & `sasctl-1.9.4/src/sasctl/pzmm/pickle_model.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/pzmm/template_files/dmcas_fitstat.json` & `sasctl-1.9.4/src/sasctl/pzmm/template_files/dmcas_fitstat.json`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/pzmm/template_files/dmcas_lift.json` & `sasctl-1.9.4/src/sasctl/pzmm/template_files/dmcas_lift.json`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/pzmm/template_files/dmcas_roc.json` & `sasctl-1.9.4/src/sasctl/pzmm/template_files/dmcas_roc.json`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/pzmm/write_json_files.py` & `sasctl-1.9.4/src/sasctl/pzmm/write_json_files.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/pzmm/write_score_code.py` & `sasctl-1.9.4/src/sasctl/pzmm/write_score_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,17 +396,15 @@
             warn(
                 "No current session connection was found to a SAS Viya server. Score "
                 "code will be written under the assumption that the target server is "
                 "SAS Viya 4."
             )
 
         if mojo_model or binary_h2o_model:
-            cls.score_code += (
-                "import h2o\nimport gzip\nimport shutil\nimport os\n\nh2o.init()\n\n"
-            )
+            cls.score_code += "import h2o\n\nh2o.init()\n\n"
         elif binary_string:
             cls.score_code += (
                 f'import codecs\n\nbinary_string = "{binary_string}"'
                 f"\nmodel = {pickle_type}.loads(codecs.decode(binary_string"
                 '.encode(), "base64"))\n\n'
             )
 
@@ -505,38 +503,38 @@
             is None.
         """
         pickle_type = pickle_type if pickle_type else "pickle"
 
         if mojo_model:
             cls.score_code += (
                 f"model = h2o.import_mojo(str(Path(settings.pickle_path"
-                f") / {model_file_name}))\n\n"
+                f') / "{model_file_name}"))\n\n'
             )
             return (
                 f"{'':8}model = h2o.import_mojo(str(Path(settings.pickle_path) / "
-                f"{model_file_name}))\n\n"
+                f'"{model_file_name}"))\n\n'
             )
         elif binary_h2o_model:
             cls.score_code += (
                 f"model = h2o.load(str(Path(settings.pickle_path) / "
                 f"{model_file_name}))\n\n"
             )
             return (
                 f"{'':8}model = h2o.load(str(Path(settings.pickle_path) / "
                 f"{model_file_name}))\n\n"
             )
         else:
             cls.score_code += (
                 f"with open(Path(settings.pickle_path) / "
-                f'"{model_file_name}", "rb") as pickle_model:\n    '
-                f"model = {pickle_type}.load(pickle_model)\n\n"
+                f'"{model_file_name}", "rb") as pickle_model:\n'
+                f"{'':4}model = {pickle_type}.load(pickle_model)\n\n"
             )
             return (
                 f"{'':8}with open(Path(settings.pickle_path) / "
-                f'"{model_file_name}", "rb") as pickle_model:\n    '
+                f'"{model_file_name}", "rb") as pickle_model:\n'
                 f"{'':12}model = {pickle_type}.load(pickle_model)\n\n"
             )
 
     @classmethod
     def _impute_missing_values(
         cls, data: DataFrame, var_list: List[str], dtype_list: List[str]
     ) -> None:
@@ -628,45 +626,47 @@
         statsmodels_model : bool, optional
             Flag to indicate that the model is a statsmodels model. The default value is
             False.
         """
         column_names = ", ".join(f'"{col}"' for col in var_list)
         # H2O models
         if dtype_list:
-            column_types = []
+            column_types = "{"
             for var, dtype in zip(var_list, dtype_list):
                 if any(x in dtype for x in ["int", "float"]):
                     col_type = "numeric"
                 else:
                     col_type = "string"
-                column_types.append(f'"{var}" : "{col_type}"')
+                column_types += f'"{var}" : "{col_type}", '
+            column_types = column_types.rstrip(", ")
+            column_types += "}"
             cls.score_code += (
                 f"{'':4}input_array = pd.DataFrame("
                 f"[[{', '.join(var_list)}]],\n{'':31}columns=["
-                f"{column_names}],\n{'':31}dtype=float,\n{'':31}"
+                f"{column_names}],\n{'':31}dtype=object,\n{'':31}"
                 f"index=[0])\n{'':4}column_types = {column_types}\n"
                 f"{'':4}h2o_array = h2o.H2OFrame(input_array, "
                 f"column_types=column_types)\n{'':4}prediction = "
                 f"model.{method.__name__}(h2o_array)\n{'':4}prediction"
                 f" = h2o.as_list(prediction, use_pandas=False)\n"
             )
         # Statsmodels models
         elif statsmodels_model:
             cls.score_code += (
                 f"{'':4}inputArray = pd.DataFrame("
                 f"[[1.0, {', '.join(var_list)}]],\n{'':29}columns=["
-                f"\"const\", {column_names}],\n{'':29}dtype=float)\n"
+                f"\"const\", {column_names}],\n{'':29}dtype=object)\n"
                 f"{'':4}prediction = model.{method.__name__}"
                 f"(input_array)\n"
             )
         else:
             cls.score_code += (
                 f"{'':4}input_array = pd.DataFrame("
                 f"[[{', '.join(var_list)}]],\n{'':30}columns=["
-                f"{column_names}],\n{'':30}dtype=float)\n{'':4}"
+                f"{column_names}],\n{'':30}dtype=object)\n{'':4}"
                 f"prediction = model.{method.__name__}(input_array)\n"
             )
 
     @classmethod
     def _determine_score_metrics(
         cls,
         predict_returns: List[Any],
```

### Comparing `sasctl-1.9.3/src/sasctl/pzmm/zip_model.py` & `sasctl-1.9.4/src/sasctl/pzmm/zip_model.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/services.py` & `sasctl-1.9.4/src/sasctl/services.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/tasks.py` & `sasctl-1.9.4/src/sasctl/tasks.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/utils/astore.py` & `sasctl-1.9.4/src/sasctl/utils/astore.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/utils/cli.py` & `sasctl-1.9.4/src/sasctl/utils/cli.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/utils/decorators.py` & `sasctl-1.9.4/src/sasctl/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/utils/misc.py` & `sasctl-1.9.4/src/sasctl/utils/misc.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/utils/model_migration.py` & `sasctl-1.9.4/src/sasctl/utils/model_migration.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/utils/pymas/core.py` & `sasctl-1.9.4/src/sasctl/utils/pymas/core.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/utils/pymas/ds2.py` & `sasctl-1.9.4/src/sasctl/utils/pymas/ds2.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/utils/pymas/python.py` & `sasctl-1.9.4/src/sasctl/utils/pymas/python.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/utils/pyml2ds/basic/tree.py` & `sasctl-1.9.4/src/sasctl/utils/pyml2ds/basic/tree.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/ensembles/core.py` & `sasctl-1.9.4/src/sasctl/utils/pyml2ds/connectors/ensembles/core.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/ensembles/lgb.py` & `sasctl-1.9.4/src/sasctl/utils/pyml2ds/connectors/ensembles/lgb.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/ensembles/pmml.py` & `sasctl-1.9.4/src/sasctl/utils/pyml2ds/connectors/ensembles/pmml.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/ensembles/xgb.py` & `sasctl-1.9.4/src/sasctl/utils/pyml2ds/connectors/ensembles/xgb.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl/utils/pyml2ds/core.py` & `sasctl-1.9.4/src/sasctl/utils/pyml2ds/core.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.3/src/sasctl.egg-info/PKG-INFO` & `sasctl-1.9.4/src/sasctl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sasctl
-Version: 1.9.3
+Version: 1.9.4
 Summary: SAS Viya Python Client
 Home-page: https://github.com/sassoftware/python-sasctl/
 Author: SAS
 License: Apache v2.0
 Project-URL: Bug Tracker, https://github.com/sassoftware/python-sasctl/issues
 Project-URL: Documentation, https://sassoftware.github.io/python-sasctl/
 Project-URL: Source Code, https://github.com/sassoftware/python-sasctl
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sasctl Version: 1.9.3 Summary: SAS Viya Python
+Metadata-Version: 2.1 Name: sasctl Version: 1.9.4 Summary: SAS Viya Python
 Client Home-page: https://github.com/sassoftware/python-sasctl/ Author: SAS
 License: Apache v2.0 Project-URL: Bug Tracker, https://github.com/sassoftware/
 python-sasctl/issues Project-URL: Documentation, https://sassoftware.github.io/
 python-sasctl/ Project-URL: Source Code, https://github.com/sassoftware/python-
 sasctl Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Environment ::
 Console Classifier: Intended Audience :: Science/Research Classifier: Intended
```

### Comparing `sasctl-1.9.3/src/sasctl.egg-info/SOURCES.txt` & `sasctl-1.9.4/src/sasctl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

