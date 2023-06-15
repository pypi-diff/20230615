# Comparing `tmp/anaml-client-0.8.0.tar.gz` & `tmp/anaml-client-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anaml-client-0.8.0.tar", last modified: Thu Sep 30 03:04:40 2021, max compression
+gzip compressed data, was "anaml-client-0.9.0.tar", last modified: Thu Oct 14 00:00:37 2021, max compression
```

## Comparing `anaml-client-0.8.0.tar` & `anaml-client-0.9.0.tar`

### file list

```diff
@@ -1,142 +1,134 @@
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.623324 anaml-client-0.8.0/
--rw-r--r--   0 iain       (501) staff       (20)      968 2021-09-30 03:04:40.622112 anaml-client-0.8.0/PKG-INFO
--rw-r--r--   0 iain       (501) staff       (20)     2678 2021-09-23 23:29:52.000000 anaml-client-0.8.0/README.md
--rw-r--r--   0 iain       (501) staff       (20)       38 2021-09-30 03:04:40.623488 anaml-client-0.8.0/setup.cfg
--rw-r--r--   0 iain       (501) staff       (20)     3809 2021-09-23 23:29:52.000000 anaml-client-0.8.0/setup.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.361433 anaml-client-0.8.0/src/
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.406833 anaml-client-0.8.0/src/anaml_client/
--rw-r--r--   0 iain       (501) staff       (20)    39338 2021-09-30 01:46:17.000000 anaml-client-0.8.0/src/anaml_client/__init__.py
--rw-r--r--   0 iain       (501) staff       (20)     1614 2021-09-30 01:46:17.000000 anaml-client-0.8.0/src/anaml_client/exceptions.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.416983 anaml-client-0.8.0/src/anaml_client/models/
--rw-r--r--   0 iain       (501) staff       (20)      307 2021-09-21 03:02:21.000000 anaml-client-0.8.0/src/anaml_client/models/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.419241 anaml-client-0.8.0/src/anaml_client/models/aggregate/
--rw-r--r--   0 iain       (501) staff       (20)     3613 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/aggregate/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.421679 anaml-client-0.8.0/src/anaml_client/models/anaml_object/
--rw-r--r--   0 iain       (501) staff       (20)    16757 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/anaml_object/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.424728 anaml-client-0.8.0/src/anaml_client/models/attribute/
--rw-r--r--   0 iain       (501) staff       (20)     4343 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/attribute/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.427541 anaml-client-0.8.0/src/anaml_client/models/branch/
--rw-r--r--   0 iain       (501) staff       (20)     6244 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/branch/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.430065 anaml-client-0.8.0/src/anaml_client/models/branch_protection/
--rw-r--r--   0 iain       (501) staff       (20)    29099 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/branch_protection/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.433079 anaml-client-0.8.0/src/anaml_client/models/checks/
--rw-r--r--   0 iain       (501) staff       (20)    19647 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/checks/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.435025 anaml-client-0.8.0/src/anaml_client/models/cluster/
--rw-r--r--   0 iain       (501) staff       (20)    22238 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/cluster/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.437358 anaml-client-0.8.0/src/anaml_client/models/cluster_creation_request/
--rw-r--r--   0 iain       (501) staff       (20)    11872 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/cluster_creation_request/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.442139 anaml-client-0.8.0/src/anaml_client/models/commit/
--rw-r--r--   0 iain       (501) staff       (20)     5319 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/commit/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.444212 anaml-client-0.8.0/src/anaml_client/models/credentials_provider_config/
--rw-r--r--   0 iain       (501) staff       (20)    10169 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/credentials_provider_config/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.448008 anaml-client-0.8.0/src/anaml_client/models/destination/
--rw-r--r--   0 iain       (501) staff       (20)    65746 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/destination/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.450694 anaml-client-0.8.0/src/anaml_client/models/destination_creation_request/
--rw-r--r--   0 iain       (501) staff       (20)    43428 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/destination_creation_request/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.458415 anaml-client-0.8.0/src/anaml_client/models/destination_reference/
--rw-r--r--   0 iain       (501) staff       (20)     9996 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/destination_reference/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.459096 anaml-client-0.8.0/src/anaml_client/models/empty/
--rw-r--r--   0 iain       (501) staff       (20)      371 2021-09-21 03:02:21.000000 anaml-client-0.8.0/src/anaml_client/models/empty/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.467960 anaml-client-0.8.0/src/anaml_client/models/entity/
--rw-r--r--   0 iain       (501) staff       (20)     9456 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/entity/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.468645 anaml-client-0.8.0/src/anaml_client/models/entity_creation_request/
--rw-r--r--   0 iain       (501) staff       (20)     4159 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/entity_creation_request/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.472998 anaml-client-0.8.0/src/anaml_client/models/entity_mapping/
--rw-r--r--   0 iain       (501) staff       (20)     7035 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/entity_mapping/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.476259 anaml-client-0.8.0/src/anaml_client/models/entity_mapping_creation_request/
--rw-r--r--   0 iain       (501) staff       (20)     2773 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/entity_mapping_creation_request/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.481027 anaml-client-0.8.0/src/anaml_client/models/event/
--rw-r--r--   0 iain       (501) staff       (20)    19436 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/event/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.481790 anaml-client-0.8.0/src/anaml_client/models/event_description/
--rw-r--r--   0 iain       (501) staff       (20)     5030 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/event_description/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.485812 anaml-client-0.8.0/src/anaml_client/models/event_window/
--rw-r--r--   0 iain       (501) staff       (20)     8089 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/event_window/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.488649 anaml-client-0.8.0/src/anaml_client/models/feature/
--rw-r--r--   0 iain       (501) staff       (20)    16067 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/feature/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.492886 anaml-client-0.8.0/src/anaml_client/models/feature_creation_request/
--rw-r--r--   0 iain       (501) staff       (20)    15262 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/feature_creation_request/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.493766 anaml-client-0.8.0/src/anaml_client/models/feature_id/
--rw-r--r--   0 iain       (501) staff       (20)     5931 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/feature_id/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.499215 anaml-client-0.8.0/src/anaml_client/models/feature_run_summaries/
--rw-r--r--   0 iain       (501) staff       (20)     4113 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/feature_run_summaries/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.499945 anaml-client-0.8.0/src/anaml_client/models/feature_set/
--rw-r--r--   0 iain       (501) staff       (20)    10022 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/feature_set/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.500663 anaml-client-0.8.0/src/anaml_client/models/feature_set_creation_request/
--rw-r--r--   0 iain       (501) staff       (20)     4112 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/feature_set_creation_request/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.509622 anaml-client-0.8.0/src/anaml_client/models/feature_store/
--rw-r--r--   0 iain       (501) staff       (20)    18949 2021-09-30 01:46:17.000000 anaml-client-0.8.0/src/anaml_client/models/feature_store/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.510442 anaml-client-0.8.0/src/anaml_client/models/feature_store_creation_request/
--rw-r--r--   0 iain       (501) staff       (20)     6862 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/feature_store_creation_request/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.520484 anaml-client-0.8.0/src/anaml_client/models/feature_store_run/
--rw-r--r--   0 iain       (501) staff       (20)    14531 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/feature_store_run/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.522838 anaml-client-0.8.0/src/anaml_client/models/feature_template/
--rw-r--r--   0 iain       (501) staff       (20)    20986 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/feature_template/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.525341 anaml-client-0.8.0/src/anaml_client/models/feature_template_creation_request/
--rw-r--r--   0 iain       (501) staff       (20)    14653 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/feature_template_creation_request/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.526175 anaml-client-0.8.0/src/anaml_client/models/file_format/
--rw-r--r--   0 iain       (501) staff       (20)     7827 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/file_format/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.528580 anaml-client-0.8.0/src/anaml_client/models/filter_expression/
--rw-r--r--   0 iain       (501) staff       (20)     2134 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/filter_expression/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.533084 anaml-client-0.8.0/src/anaml_client/models/generated_features/
--rw-r--r--   0 iain       (501) staff       (20)     4844 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/generated_features/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.535926 anaml-client-0.8.0/src/anaml_client/models/item/
--rw-r--r--   0 iain       (501) staff       (20)     5855 2021-09-21 03:02:21.000000 anaml-client-0.8.0/src/anaml_client/models/item/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.538027 anaml-client-0.8.0/src/anaml_client/models/job_metrics/
--rw-r--r--   0 iain       (501) staff       (20)     6982 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/job_metrics/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.539633 anaml-client-0.8.0/src/anaml_client/models/jobs/
--rw-r--r--   0 iain       (501) staff       (20)    12466 2021-09-24 00:23:24.000000 anaml-client-0.8.0/src/anaml_client/models/jobs/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.544814 anaml-client-0.8.0/src/anaml_client/models/label/
--rw-r--r--   0 iain       (501) staff       (20)     2161 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/label/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.547067 anaml-client-0.8.0/src/anaml_client/models/merge_request/
--rw-r--r--   0 iain       (501) staff       (20)    27879 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/merge_request/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.549314 anaml-client-0.8.0/src/anaml_client/models/post_aggregate_expression/
--rw-r--r--   0 iain       (501) staff       (20)     2169 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/post_aggregate_expression/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.551439 anaml-client-0.8.0/src/anaml_client/models/quality_rating/
--rw-r--r--   0 iain       (501) staff       (20)     2784 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/quality_rating/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.552299 anaml-client-0.8.0/src/anaml_client/models/ref/
--rw-r--r--   0 iain       (501) staff       (20)     6347 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/ref/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.553592 anaml-client-0.8.0/src/anaml_client/models/reports/
--rw-r--r--   0 iain       (501) staff       (20)     6130 2021-09-30 01:46:17.000000 anaml-client-0.8.0/src/anaml_client/models/reports/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.555383 anaml-client-0.8.0/src/anaml_client/models/restrictions/
--rw-r--r--   0 iain       (501) staff       (20)     9532 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/restrictions/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.556769 anaml-client-0.8.0/src/anaml_client/models/roles/
--rw-r--r--   0 iain       (501) staff       (20)     2122 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/roles/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.589657 anaml-client-0.8.0/src/anaml_client/models/schedule/
--rw-r--r--   0 iain       (501) staff       (20)    19487 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/schedule/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.590971 anaml-client-0.8.0/src/anaml_client/models/secrets_config/
--rw-r--r--   0 iain       (501) staff       (20)     8936 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/secrets_config/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.592728 anaml-client-0.8.0/src/anaml_client/models/select_expression/
--rw-r--r--   0 iain       (501) staff       (20)     2129 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/select_expression/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.594179 anaml-client-0.8.0/src/anaml_client/models/source/
--rw-r--r--   0 iain       (501) staff       (20)    52516 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/source/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.598487 anaml-client-0.8.0/src/anaml_client/models/source_creation_request/
--rw-r--r--   0 iain       (501) staff       (20)    38317 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/source_creation_request/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.601396 anaml-client-0.8.0/src/anaml_client/models/source_reference/
--rw-r--r--   0 iain       (501) staff       (20)     9611 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/source_reference/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.602405 anaml-client-0.8.0/src/anaml_client/models/summary_statistics/
--rw-r--r--   0 iain       (501) staff       (20)    26998 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/summary_statistics/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.603156 anaml-client-0.8.0/src/anaml_client/models/table/
--rw-r--r--   0 iain       (501) staff       (20)    24436 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/table/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.603891 anaml-client-0.8.0/src/anaml_client/models/table_creation_request/
--rw-r--r--   0 iain       (501) staff       (20)    17926 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/table_creation_request/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.606844 anaml-client-0.8.0/src/anaml_client/models/table_preview/
--rw-r--r--   0 iain       (501) staff       (20)    17591 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/table_preview/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.609045 anaml-client-0.8.0/src/anaml_client/models/task_statistics/
--rw-r--r--   0 iain       (501) staff       (20)    14504 2021-09-21 03:02:21.000000 anaml-client-0.8.0/src/anaml_client/models/task_statistics/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.610898 anaml-client-0.8.0/src/anaml_client/models/user/
--rw-r--r--   0 iain       (501) staff       (20)    19156 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/user/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.611585 anaml-client-0.8.0/src/anaml_client/models/user_group/
--rw-r--r--   0 iain       (501) staff       (20)    19449 2021-09-23 23:29:52.000000 anaml-client-0.8.0/src/anaml_client/models/user_group/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.614401 anaml-client-0.8.0/src/anaml_client/models/webhook/
--rw-r--r--   0 iain       (501) staff       (20)    23531 2021-09-30 01:46:17.000000 anaml-client-0.8.0/src/anaml_client/models/webhook/__init__.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.620676 anaml-client-0.8.0/src/anaml_client/utils/
--rw-r--r--   0 iain       (501) staff       (20)     1388 2021-08-13 04:51:02.000000 anaml-client-0.8.0/src/anaml_client/utils/__init__.py
--rw-r--r--   0 iain       (501) staff       (20)     5728 2021-08-19 23:01:18.000000 anaml-client-0.8.0/src/anaml_client/utils/persistent.py
--rw-r--r--   0 iain       (501) staff       (20)     5836 2021-08-13 04:51:02.000000 anaml-client-0.8.0/src/anaml_client/utils/serialisation.py
--rw-r--r--   0 iain       (501) staff       (20)      267 2021-09-30 03:04:39.000000 anaml-client-0.8.0/src/anaml_client/version.py
-drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-09-30 03:04:40.414818 anaml-client-0.8.0/src/anaml_client.egg-info/
--rw-r--r--   0 iain       (501) staff       (20)      968 2021-09-30 03:04:39.000000 anaml-client-0.8.0/src/anaml_client.egg-info/PKG-INFO
--rw-r--r--   0 iain       (501) staff       (20)     3506 2021-09-30 03:04:39.000000 anaml-client-0.8.0/src/anaml_client.egg-info/SOURCES.txt
--rw-r--r--   0 iain       (501) staff       (20)        1 2021-09-30 03:04:39.000000 anaml-client-0.8.0/src/anaml_client.egg-info/dependency_links.txt
--rw-r--r--   0 iain       (501) staff       (20)      314 2021-09-30 03:04:39.000000 anaml-client-0.8.0/src/anaml_client.egg-info/requires.txt
--rw-r--r--   0 iain       (501) staff       (20)       13 2021-09-30 03:04:39.000000 anaml-client-0.8.0/src/anaml_client.egg-info/top_level.txt
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:37.009903 anaml-client-0.9.0/
+-rw-r--r--   0 iain       (501) staff       (20)      901 2021-10-14 00:00:37.006747 anaml-client-0.9.0/PKG-INFO
+-rw-r--r--   0 iain       (501) staff       (20)     2678 2021-09-23 23:29:52.000000 anaml-client-0.9.0/README.md
+-rw-r--r--   0 iain       (501) staff       (20)       38 2021-10-14 00:00:37.016315 anaml-client-0.9.0/setup.cfg
+-rw-r--r--   0 iain       (501) staff       (20)     3809 2021-09-23 23:29:52.000000 anaml-client-0.9.0/setup.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.846453 anaml-client-0.9.0/src/
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.876884 anaml-client-0.9.0/src/anaml_client/
+-rw-r--r--   0 iain       (501) staff       (20)    39643 2021-10-13 22:52:23.000000 anaml-client-0.9.0/src/anaml_client/__init__.py
+-rw-r--r--   0 iain       (501) staff       (20)     1614 2021-09-30 01:46:17.000000 anaml-client-0.9.0/src/anaml_client/exceptions.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.884227 anaml-client-0.9.0/src/anaml_client/models/
+-rw-r--r--   0 iain       (501) staff       (20)      307 2021-09-21 03:02:21.000000 anaml-client-0.9.0/src/anaml_client/models/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.885147 anaml-client-0.9.0/src/anaml_client/models/aggregate/
+-rw-r--r--   0 iain       (501) staff       (20)     3613 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/aggregate/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.891411 anaml-client-0.9.0/src/anaml_client/models/anaml_object/
+-rw-r--r--   0 iain       (501) staff       (20)    16757 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/anaml_object/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.894110 anaml-client-0.9.0/src/anaml_client/models/attribute/
+-rw-r--r--   0 iain       (501) staff       (20)     4343 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/attribute/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.895357 anaml-client-0.9.0/src/anaml_client/models/branch/
+-rw-r--r--   0 iain       (501) staff       (20)     6244 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/branch/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.897338 anaml-client-0.9.0/src/anaml_client/models/branch_protection/
+-rw-r--r--   0 iain       (501) staff       (20)    29099 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/branch_protection/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.899504 anaml-client-0.9.0/src/anaml_client/models/checks/
+-rw-r--r--   0 iain       (501) staff       (20)    19647 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/checks/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.902175 anaml-client-0.9.0/src/anaml_client/models/cluster/
+-rw-r--r--   0 iain       (501) staff       (20)    20946 2021-10-13 22:52:23.000000 anaml-client-0.9.0/src/anaml_client/models/cluster/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.903023 anaml-client-0.9.0/src/anaml_client/models/cluster_creation_request/
+-rw-r--r--   0 iain       (501) staff       (20)    11872 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/cluster_creation_request/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.904182 anaml-client-0.9.0/src/anaml_client/models/commit/
+-rw-r--r--   0 iain       (501) staff       (20)     5319 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/commit/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.905527 anaml-client-0.9.0/src/anaml_client/models/credentials_provider_config/
+-rw-r--r--   0 iain       (501) staff       (20)    10169 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/credentials_provider_config/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.907479 anaml-client-0.9.0/src/anaml_client/models/destination/
+-rw-r--r--   0 iain       (501) staff       (20)    59606 2021-10-13 22:52:23.000000 anaml-client-0.9.0/src/anaml_client/models/destination/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.908679 anaml-client-0.9.0/src/anaml_client/models/destination_creation_request/
+-rw-r--r--   0 iain       (501) staff       (20)    43428 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/destination_creation_request/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.910404 anaml-client-0.9.0/src/anaml_client/models/destination_reference/
+-rw-r--r--   0 iain       (501) staff       (20)     9996 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/destination_reference/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.912018 anaml-client-0.9.0/src/anaml_client/models/entity/
+-rw-r--r--   0 iain       (501) staff       (20)     9456 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/entity/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.913093 anaml-client-0.9.0/src/anaml_client/models/entity_creation_request/
+-rw-r--r--   0 iain       (501) staff       (20)     4159 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/entity_creation_request/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.914458 anaml-client-0.9.0/src/anaml_client/models/entity_mapping/
+-rw-r--r--   0 iain       (501) staff       (20)     7035 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/entity_mapping/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.915550 anaml-client-0.9.0/src/anaml_client/models/entity_mapping_creation_request/
+-rw-r--r--   0 iain       (501) staff       (20)     2773 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/entity_mapping_creation_request/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.916660 anaml-client-0.9.0/src/anaml_client/models/event/
+-rw-r--r--   0 iain       (501) staff       (20)    19436 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/event/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.918307 anaml-client-0.9.0/src/anaml_client/models/event_description/
+-rw-r--r--   0 iain       (501) staff       (20)     5030 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/event_description/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.920254 anaml-client-0.9.0/src/anaml_client/models/event_window/
+-rw-r--r--   0 iain       (501) staff       (20)     8089 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/event_window/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.924737 anaml-client-0.9.0/src/anaml_client/models/feature/
+-rw-r--r--   0 iain       (501) staff       (20)    14730 2021-10-13 22:52:23.000000 anaml-client-0.9.0/src/anaml_client/models/feature/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.927970 anaml-client-0.9.0/src/anaml_client/models/feature_creation_request/
+-rw-r--r--   0 iain       (501) staff       (20)    13925 2021-10-13 22:52:23.000000 anaml-client-0.9.0/src/anaml_client/models/feature_creation_request/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.928589 anaml-client-0.9.0/src/anaml_client/models/feature_id/
+-rw-r--r--   0 iain       (501) staff       (20)     5931 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/feature_id/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.930089 anaml-client-0.9.0/src/anaml_client/models/feature_run_summaries/
+-rw-r--r--   0 iain       (501) staff       (20)     4113 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/feature_run_summaries/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.931053 anaml-client-0.9.0/src/anaml_client/models/feature_set/
+-rw-r--r--   0 iain       (501) staff       (20)    10022 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/feature_set/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.932132 anaml-client-0.9.0/src/anaml_client/models/feature_set_creation_request/
+-rw-r--r--   0 iain       (501) staff       (20)     4112 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/feature_set_creation_request/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.933594 anaml-client-0.9.0/src/anaml_client/models/feature_store/
+-rw-r--r--   0 iain       (501) staff       (20)    18949 2021-09-30 01:46:17.000000 anaml-client-0.9.0/src/anaml_client/models/feature_store/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.935774 anaml-client-0.9.0/src/anaml_client/models/feature_store_creation_request/
+-rw-r--r--   0 iain       (501) staff       (20)     6862 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/feature_store_creation_request/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.937252 anaml-client-0.9.0/src/anaml_client/models/feature_store_run/
+-rw-r--r--   0 iain       (501) staff       (20)    14531 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/feature_store_run/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.939602 anaml-client-0.9.0/src/anaml_client/models/feature_template/
+-rw-r--r--   0 iain       (501) staff       (20)    19649 2021-10-13 22:52:23.000000 anaml-client-0.9.0/src/anaml_client/models/feature_template/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.941082 anaml-client-0.9.0/src/anaml_client/models/feature_template_creation_request/
+-rw-r--r--   0 iain       (501) staff       (20)    13316 2021-10-13 22:52:23.000000 anaml-client-0.9.0/src/anaml_client/models/feature_template_creation_request/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.942322 anaml-client-0.9.0/src/anaml_client/models/file_format/
+-rw-r--r--   0 iain       (501) staff       (20)    12448 2021-10-13 22:52:23.000000 anaml-client-0.9.0/src/anaml_client/models/file_format/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.942968 anaml-client-0.9.0/src/anaml_client/models/filter_expression/
+-rw-r--r--   0 iain       (501) staff       (20)     2134 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/filter_expression/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.946760 anaml-client-0.9.0/src/anaml_client/models/generated_features/
+-rw-r--r--   0 iain       (501) staff       (20)     4844 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/generated_features/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.948184 anaml-client-0.9.0/src/anaml_client/models/job_metrics/
+-rw-r--r--   0 iain       (501) staff       (20)     6982 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/job_metrics/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.949362 anaml-client-0.9.0/src/anaml_client/models/jobs/
+-rw-r--r--   0 iain       (501) staff       (20)    12466 2021-09-24 00:23:24.000000 anaml-client-0.9.0/src/anaml_client/models/jobs/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.951321 anaml-client-0.9.0/src/anaml_client/models/label/
+-rw-r--r--   0 iain       (501) staff       (20)     2161 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/label/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.952021 anaml-client-0.9.0/src/anaml_client/models/merge_request/
+-rw-r--r--   0 iain       (501) staff       (20)    27879 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/merge_request/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.956453 anaml-client-0.9.0/src/anaml_client/models/post_aggregate_expression/
+-rw-r--r--   0 iain       (501) staff       (20)     2169 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/post_aggregate_expression/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.958182 anaml-client-0.9.0/src/anaml_client/models/ref/
+-rw-r--r--   0 iain       (501) staff       (20)     6347 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/ref/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.961357 anaml-client-0.9.0/src/anaml_client/models/reports/
+-rw-r--r--   0 iain       (501) staff       (20)     5819 2021-10-13 22:52:23.000000 anaml-client-0.9.0/src/anaml_client/models/reports/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.962218 anaml-client-0.9.0/src/anaml_client/models/restrictions/
+-rw-r--r--   0 iain       (501) staff       (20)    24477 2021-10-13 22:52:23.000000 anaml-client-0.9.0/src/anaml_client/models/restrictions/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.962729 anaml-client-0.9.0/src/anaml_client/models/roles/
+-rw-r--r--   0 iain       (501) staff       (20)     3781 2021-10-13 22:52:23.000000 anaml-client-0.9.0/src/anaml_client/models/roles/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.964379 anaml-client-0.9.0/src/anaml_client/models/schedule/
+-rw-r--r--   0 iain       (501) staff       (20)    19487 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/schedule/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.966767 anaml-client-0.9.0/src/anaml_client/models/secrets_config/
+-rw-r--r--   0 iain       (501) staff       (20)     8936 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/secrets_config/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.967785 anaml-client-0.9.0/src/anaml_client/models/select_expression/
+-rw-r--r--   0 iain       (501) staff       (20)     2129 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/select_expression/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.969508 anaml-client-0.9.0/src/anaml_client/models/source/
+-rw-r--r--   0 iain       (501) staff       (20)    47167 2021-10-13 22:52:23.000000 anaml-client-0.9.0/src/anaml_client/models/source/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.971986 anaml-client-0.9.0/src/anaml_client/models/source_creation_request/
+-rw-r--r--   0 iain       (501) staff       (20)    38317 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/source_creation_request/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.976819 anaml-client-0.9.0/src/anaml_client/models/source_reference/
+-rw-r--r--   0 iain       (501) staff       (20)     9611 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/source_reference/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.983506 anaml-client-0.9.0/src/anaml_client/models/summary_statistics/
+-rw-r--r--   0 iain       (501) staff       (20)    26998 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/summary_statistics/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.986286 anaml-client-0.9.0/src/anaml_client/models/table/
+-rw-r--r--   0 iain       (501) staff       (20)    22512 2021-10-13 22:52:23.000000 anaml-client-0.9.0/src/anaml_client/models/table/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.987928 anaml-client-0.9.0/src/anaml_client/models/table_creation_request/
+-rw-r--r--   0 iain       (501) staff       (20)    16002 2021-10-13 22:52:23.000000 anaml-client-0.9.0/src/anaml_client/models/table_creation_request/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.990262 anaml-client-0.9.0/src/anaml_client/models/table_preview/
+-rw-r--r--   0 iain       (501) staff       (20)    17591 2021-09-23 23:29:52.000000 anaml-client-0.9.0/src/anaml_client/models/table_preview/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.993620 anaml-client-0.9.0/src/anaml_client/models/user/
+-rw-r--r--   0 iain       (501) staff       (20)    18547 2021-10-13 22:52:23.000000 anaml-client-0.9.0/src/anaml_client/models/user/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.994267 anaml-client-0.9.0/src/anaml_client/models/user_group/
+-rw-r--r--   0 iain       (501) staff       (20)    20739 2021-10-13 22:52:23.000000 anaml-client-0.9.0/src/anaml_client/models/user_group/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.999720 anaml-client-0.9.0/src/anaml_client/models/webhook/
+-rw-r--r--   0 iain       (501) staff       (20)    25707 2021-10-13 22:52:23.000000 anaml-client-0.9.0/src/anaml_client/models/webhook/__init__.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:37.004797 anaml-client-0.9.0/src/anaml_client/utils/
+-rw-r--r--   0 iain       (501) staff       (20)     1388 2021-08-13 04:51:02.000000 anaml-client-0.9.0/src/anaml_client/utils/__init__.py
+-rw-r--r--   0 iain       (501) staff       (20)     5728 2021-08-19 23:01:18.000000 anaml-client-0.9.0/src/anaml_client/utils/persistent.py
+-rw-r--r--   0 iain       (501) staff       (20)     5836 2021-08-13 04:51:02.000000 anaml-client-0.9.0/src/anaml_client/utils/serialisation.py
+-rw-r--r--   0 iain       (501) staff       (20)      267 2021-10-14 00:00:36.000000 anaml-client-0.9.0/src/anaml_client/version.py
+drwxr-xr-x   0 iain       (501) staff       (20)        0 2021-10-14 00:00:36.883625 anaml-client-0.9.0/src/anaml_client.egg-info/
+-rw-r--r--   0 iain       (501) staff       (20)      901 2021-10-14 00:00:36.000000 anaml-client-0.9.0/src/anaml_client.egg-info/PKG-INFO
+-rw-r--r--   0 iain       (501) staff       (20)     3320 2021-10-14 00:00:36.000000 anaml-client-0.9.0/src/anaml_client.egg-info/SOURCES.txt
+-rw-r--r--   0 iain       (501) staff       (20)        1 2021-10-14 00:00:36.000000 anaml-client-0.9.0/src/anaml_client.egg-info/dependency_links.txt
+-rw-r--r--   0 iain       (501) staff       (20)      314 2021-10-14 00:00:36.000000 anaml-client-0.9.0/src/anaml_client.egg-info/requires.txt
+-rw-r--r--   0 iain       (501) staff       (20)       13 2021-10-14 00:00:36.000000 anaml-client-0.9.0/src/anaml_client.egg-info/top_level.txt
```

### Comparing `anaml-client-0.8.0/PKG-INFO` & `anaml-client-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: anaml-client
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python SDK for Anaml
 Home-page: https://anaml.com
 Author: Simple Machines
 Author-email: hello@simplemachines.com.au
 License: Copyright 2020 Simple Machines Pty Ltd. All Rights Reserved
-Description: 
-        The Anaml Python SDK makes it easy to interact with the [Anaml][1] feature
-        engineering platform from Python. The SDK provides datatypes and methods to
-        interact with the Anaml REST API and to load Anaml feature data into Pandas
-        and/or Spark data frames.
-        
-        [1]: https://www.anaml.com/
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: Other/Proprietary License
 Requires-Python: >=3.7.10
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: plotting
 Provides-Extra: pandas
 Provides-Extra: spark
 Provides-Extra: aws
 Provides-Extra: google
+
+
+The Anaml Python SDK makes it easy to interact with the [Anaml][1] feature
+engineering platform from Python. The SDK provides datatypes and methods to
+interact with the Anaml REST API and to load Anaml feature data into Pandas
+and/or Spark data frames.
+
+[1]: https://www.anaml.com/
+
+
```

### Comparing `anaml-client-0.8.0/README.md` & `anaml-client-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/setup.py` & `anaml-client-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/__init__.py` & `anaml-client-0.9.0/src/anaml_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # in type annotations without insisting that every user install PySpark whether
 # or not they will use it.
 #
 # NB: This relies on the __future__ import changing the way that type annotations
 # are processed.
 #
 # This is supported in Python 3.7+
-from .exceptions import AnamlError
+from .exceptions import AnamlError, Reason
 from .models.summary_statistics import SummaryStatistics
 
 if typing.TYPE_CHECKING:
     import pandas
     import pyspark.sql
     import s3fs
     from google.cloud import bigquery
@@ -974,26 +974,30 @@
             self._log.warning(_NO_FEATURES.format(thefeatures=', '.join(features)))
 
     def _json_or_handle_errors(self, r: requests.Response):
         if r.ok:
             try:
                 result = r.json()
                 return result
-            except json.JSONDecodeError:
+            except json.decoder.JSONDecodeError:
                 # Sorry, (no or invalid) JSON here
                 self._log.error("No or invalid JSON received from server")
                 self._log.error("Response content: " + r.text)
-                r.raise_for_status()
+                raise AnamlError(errors=[Reason(message="Expected JSON but the server did not return any")])
         else:
-            response_json = r.json()
-            if "errors" in response_json:
-                ex = AnamlError.from_json(response_json)
-                self._log.error("The Anaml server reported an error", ex)
-                raise ex
-        r.raise_for_status()
+            try:
+                response_json = r.json()
+                if "errors" in response_json:
+                    ex = AnamlError.from_json(response_json)
+                    self._log.error("The Anaml server reported an error", ex)
+                    raise ex
+            except json.decoder.JSONDecodeError:
+                # This is not unexpected. 404 responses, in particular, often have no JSON error message.
+                pass
+            r.raise_for_status()
 
     def _int_or_handle_errors(self, r):
         if r.ok:
             return int(r.text)
         else:
             if "errors" in r:
                 self._log.error(json.dumps(r._get("errors"), indent=4))
```

### Comparing `anaml-client-0.8.0/src/anaml_client/exceptions.py` & `anaml-client-0.9.0/src/anaml_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/aggregate/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/aggregate/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/anaml_object/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/anaml_object/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/attribute/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/attribute/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/branch/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/branch/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/branch_protection/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/branch_protection/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/checks/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/cluster/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/cluster/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -314,29 +314,27 @@
     Args:
         attributes (typing.List[Attribute]): A data field.
         description (str): A data field.
         id (ClusterId): A data field.
         isPreviewCluster (bool): A data field.
         labels (typing.List[Label]): A data field.
         name (ClusterName): A data field.
-        predecessor (typing.Optional[ClusterVersionId]): A data field.
         sparkConfig (SparkConfig): A data field.
         version (ClusterVersionId): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = ""
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     attributes: typing.List[Attribute]
     description: str
     id: ClusterId
     isPreviewCluster: bool
     labels: typing.List[Label]
     name: ClusterName
-    predecessor: typing.Optional[ClusterVersionId]
     sparkConfig: SparkConfig
     version: ClusterVersionId
     
     @classmethod
     def json_schema(cls):
         """JSON schema for variant Cluster.
         
@@ -403,15 +401,14 @@
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
         isPreviewCluster (bool): A data field.
         anamlServerUrl (str): A data field.
         credentialsProvider (CredentialsProviderConfig): A data field.
         sparkConfig (SparkConfig): A data field.
         version (ClusterVersionId): A data field.
-        predecessor (typing.Optional[ClusterVersionId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "local"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: ClusterId
     name: ClusterName
@@ -419,15 +416,14 @@
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
     isPreviewCluster: bool
     anamlServerUrl: str
     credentialsProvider: CredentialsProviderConfig
     sparkConfig: SparkConfig
     version: ClusterVersionId
-    predecessor: typing.Optional[ClusterVersionId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for LocalCluster data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -456,21 +452,15 @@
                     "type": "boolean"
                 },
                 "anamlServerUrl": {
                     "type": "string"
                 },
                 "credentialsProvider": CredentialsProviderConfig.json_schema(),
                 "sparkConfig": SparkConfig.json_schema(),
-                "version": ClusterVersionId.json_schema(),
-                "predecessor": {
-                    "oneOf": [
-                        {"type": "null"},
-                        ClusterVersionId.json_schema(),
-                    ]
-                }
+                "version": ClusterVersionId.json_schema()
             },
             "required": [
                 "adt_type",
                 "id",
                 "name",
                 "description",
                 "labels",
@@ -506,19 +496,14 @@
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
                 isPreviewCluster=bool(data["isPreviewCluster"]),
                 anamlServerUrl=str(data["anamlServerUrl"]),
                 credentialsProvider=CredentialsProviderConfig.from_json(data["credentialsProvider"]),
                 sparkConfig=SparkConfig.from_json(data["sparkConfig"]),
                 version=ClusterVersionId.from_json(data["version"]),
-                predecessor=(
-                    lambda v: v and ClusterVersionId.from_json(v)
-                )(
-                    data.get("predecessor", None)
-                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing LocalCluster",
                 exc_info=ex
             )
             raise
@@ -536,16 +521,15 @@
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
             "isPreviewCluster": self.isPreviewCluster,
             "anamlServerUrl": str(self.anamlServerUrl),
             "credentialsProvider": self.credentialsProvider.to_json(),
             "sparkConfig": self.sparkConfig.to_json(),
-            "version": self.version.to_json(),
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "version": self.version.to_json()
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class SparkServerCluster(Cluster):
     """Job execution cluster managed by a Spark Server.
     
@@ -555,30 +539,28 @@
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
         isPreviewCluster (bool): A data field.
         sparkServerUrl (str): A data field.
         sparkConfig (SparkConfig): A data field.
         version (ClusterVersionId): A data field.
-        predecessor (typing.Optional[ClusterVersionId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "sparkserver"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: ClusterId
     name: ClusterName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
     isPreviewCluster: bool
     sparkServerUrl: str
     sparkConfig: SparkConfig
     version: ClusterVersionId
-    predecessor: typing.Optional[ClusterVersionId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for SparkServerCluster data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -606,21 +588,15 @@
                 "isPreviewCluster": {
                     "type": "boolean"
                 },
                 "sparkServerUrl": {
                     "type": "string"
                 },
                 "sparkConfig": SparkConfig.json_schema(),
-                "version": ClusterVersionId.json_schema(),
-                "predecessor": {
-                    "oneOf": [
-                        {"type": "null"},
-                        ClusterVersionId.json_schema(),
-                    ]
-                }
+                "version": ClusterVersionId.json_schema()
             },
             "required": [
                 "adt_type",
                 "id",
                 "name",
                 "description",
                 "labels",
@@ -654,19 +630,14 @@
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
                 isPreviewCluster=bool(data["isPreviewCluster"]),
                 sparkServerUrl=str(data["sparkServerUrl"]),
                 sparkConfig=SparkConfig.from_json(data["sparkConfig"]),
                 version=ClusterVersionId.from_json(data["version"]),
-                predecessor=(
-                    lambda v: v and ClusterVersionId.from_json(v)
-                )(
-                    data.get("predecessor", None)
-                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing SparkServerCluster",
                 exc_info=ex
             )
             raise
@@ -683,10 +654,9 @@
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
             "isPreviewCluster": self.isPreviewCluster,
             "sparkServerUrl": str(self.sparkServerUrl),
             "sparkConfig": self.sparkConfig.to_json(),
-            "version": self.version.to_json(),
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "version": self.version.to_json()
         }
```

### Comparing `anaml-client-0.8.0/src/anaml_client/models/cluster_creation_request/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/cluster_creation_request/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/commit/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/commit/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/credentials_provider_config/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/credentials_provider_config/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/destination/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/destination/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -452,27 +452,25 @@
     
     Args:
         attributes (typing.List[Attribute]): A data field.
         description (str): A data field.
         id (DestinationId): A data field.
         labels (typing.List[Label]): A data field.
         name (DestinationName): A data field.
-        predecessor (typing.Optional[DestinationVersionId]): A data field.
         version (DestinationVersionId): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = ""
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     attributes: typing.List[Attribute]
     description: str
     id: DestinationId
     labels: typing.List[Label]
     name: DestinationName
-    predecessor: typing.Optional[DestinationVersionId]
     version: DestinationVersionId
     
     @classmethod
     def json_schema(cls):
         """JSON schema for variant Destination.
         
         Returns:
@@ -537,30 +535,28 @@
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
         bucket (str): A data field.
         path (str): A data field.
         fileFormat (FileFormat): A data field.
         version (DestinationVersionId): A data field.
-        predecessor (typing.Optional[DestinationVersionId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "s3"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: DestinationId
     name: DestinationName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
     bucket: str
     path: str
     fileFormat: FileFormat
     version: DestinationVersionId
-    predecessor: typing.Optional[DestinationVersionId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for S3Destination data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -588,21 +584,15 @@
                 "bucket": {
                     "type": "string"
                 },
                 "path": {
                     "type": "string"
                 },
                 "fileFormat": FileFormat.json_schema(),
-                "version": DestinationVersionId.json_schema(),
-                "predecessor": {
-                    "oneOf": [
-                        {"type": "null"},
-                        DestinationVersionId.json_schema(),
-                    ]
-                }
+                "version": DestinationVersionId.json_schema()
             },
             "required": [
                 "adt_type",
                 "id",
                 "name",
                 "description",
                 "labels",
@@ -636,19 +626,14 @@
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
                 bucket=str(data["bucket"]),
                 path=str(data["path"]),
                 fileFormat=FileFormat.from_json(data["fileFormat"]),
                 version=DestinationVersionId.from_json(data["version"]),
-                predecessor=(
-                    lambda v: v and DestinationVersionId.from_json(v)
-                )(
-                    data.get("predecessor", None)
-                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing S3Destination",
                 exc_info=ex
             )
             raise
@@ -665,16 +650,15 @@
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
             "bucket": str(self.bucket),
             "path": str(self.path),
             "fileFormat": self.fileFormat.to_json(),
-            "version": self.version.to_json(),
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "version": self.version.to_json()
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class S3ADestination(Destination):
     """A data destination using the S3 protocol.
     
@@ -687,15 +671,14 @@
         bucket (str): A data field.
         path (str): A data field.
         fileFormat (FileFormat): A data field.
         endpoint (str): A data field.
         accessKey (str): A data field.
         secretKey (str): A data field.
         version (DestinationVersionId): A data field.
-        predecessor (typing.Optional[DestinationVersionId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "s3a"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: DestinationId
     name: DestinationName
@@ -705,15 +688,14 @@
     bucket: str
     path: str
     fileFormat: FileFormat
     endpoint: str
     accessKey: str
     secretKey: str
     version: DestinationVersionId
-    predecessor: typing.Optional[DestinationVersionId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for S3ADestination data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -750,21 +732,15 @@
                 },
                 "accessKey": {
                     "type": "string"
                 },
                 "secretKey": {
                     "type": "string"
                 },
-                "version": DestinationVersionId.json_schema(),
-                "predecessor": {
-                    "oneOf": [
-                        {"type": "null"},
-                        DestinationVersionId.json_schema(),
-                    ]
-                }
+                "version": DestinationVersionId.json_schema()
             },
             "required": [
                 "adt_type",
                 "id",
                 "name",
                 "description",
                 "labels",
@@ -804,19 +780,14 @@
                 bucket=str(data["bucket"]),
                 path=str(data["path"]),
                 fileFormat=FileFormat.from_json(data["fileFormat"]),
                 endpoint=str(data["endpoint"]),
                 accessKey=str(data["accessKey"]),
                 secretKey=str(data["secretKey"]),
                 version=DestinationVersionId.from_json(data["version"]),
-                predecessor=(
-                    lambda v: v and DestinationVersionId.from_json(v)
-                )(
-                    data.get("predecessor", None)
-                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing S3ADestination",
                 exc_info=ex
             )
             raise
@@ -836,16 +807,15 @@
             "attributes": [v.to_json() for v in self.attributes],
             "bucket": str(self.bucket),
             "path": str(self.path),
             "fileFormat": self.fileFormat.to_json(),
             "endpoint": str(self.endpoint),
             "accessKey": str(self.accessKey),
             "secretKey": str(self.secretKey),
-            "version": self.version.to_json(),
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "version": self.version.to_json()
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class JDBCDestination(Destination):
     """A data destination using JDBC.
     
@@ -855,30 +825,28 @@
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
         url (str): A data field.
         schema (str): A data field.
         credentialsProvider (CredentialsProviderConfig): A data field.
         version (DestinationVersionId): A data field.
-        predecessor (typing.Optional[DestinationVersionId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "jdbc"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: DestinationId
     name: DestinationName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
     url: str
     schema: str
     credentialsProvider: CredentialsProviderConfig
     version: DestinationVersionId
-    predecessor: typing.Optional[DestinationVersionId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for JDBCDestination data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -906,21 +874,15 @@
                 "url": {
                     "type": "string"
                 },
                 "schema": {
                     "type": "string"
                 },
                 "credentialsProvider": CredentialsProviderConfig.json_schema(),
-                "version": DestinationVersionId.json_schema(),
-                "predecessor": {
-                    "oneOf": [
-                        {"type": "null"},
-                        DestinationVersionId.json_schema(),
-                    ]
-                }
+                "version": DestinationVersionId.json_schema()
             },
             "required": [
                 "adt_type",
                 "id",
                 "name",
                 "description",
                 "labels",
@@ -954,19 +916,14 @@
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
                 url=str(data["url"]),
                 schema=str(data["schema"]),
                 credentialsProvider=CredentialsProviderConfig.from_json(data["credentialsProvider"]),
                 version=DestinationVersionId.from_json(data["version"]),
-                predecessor=(
-                    lambda v: v and DestinationVersionId.from_json(v)
-                )(
-                    data.get("predecessor", None)
-                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing JDBCDestination",
                 exc_info=ex
             )
             raise
@@ -983,16 +940,15 @@
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
             "url": str(self.url),
             "schema": str(self.schema),
             "credentialsProvider": self.credentialsProvider.to_json(),
-            "version": self.version.to_json(),
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "version": self.version.to_json()
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class HiveDestination(Destination):
     """A data destination in Hive.
     
@@ -1000,28 +956,26 @@
         id (DestinationId): A data field.
         name (DestinationName): A data field.
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
         database (str): A data field.
         version (DestinationVersionId): A data field.
-        predecessor (typing.Optional[DestinationVersionId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "hive"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: DestinationId
     name: DestinationName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
     database: str
     version: DestinationVersionId
-    predecessor: typing.Optional[DestinationVersionId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for HiveDestination data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -1045,21 +999,15 @@
                 "attributes": {
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
                 "database": {
                     "type": "string"
                 },
-                "version": DestinationVersionId.json_schema(),
-                "predecessor": {
-                    "oneOf": [
-                        {"type": "null"},
-                        DestinationVersionId.json_schema(),
-                    ]
-                }
+                "version": DestinationVersionId.json_schema()
             },
             "required": [
                 "adt_type",
                 "id",
                 "name",
                 "description",
                 "labels",
@@ -1089,19 +1037,14 @@
                 id=DestinationId.from_json(data["id"]),
                 name=DestinationName.from_json(data["name"]),
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
                 database=str(data["database"]),
                 version=DestinationVersionId.from_json(data["version"]),
-                predecessor=(
-                    lambda v: v and DestinationVersionId.from_json(v)
-                )(
-                    data.get("predecessor", None)
-                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing HiveDestination",
                 exc_info=ex
             )
             raise
@@ -1116,16 +1059,15 @@
             "adt_type": self.ADT_TYPE,
             "id": self.id.to_json(),
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
             "database": str(self.database),
-            "version": self.version.to_json(),
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "version": self.version.to_json()
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class BigQueryDestination(Destination):
     """A data destination in Google BigQuery.
     
@@ -1134,29 +1076,27 @@
         name (DestinationName): A data field.
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
         path (str): A data field.
         stagingArea (GCSStagingArea): A data field.
         version (DestinationVersionId): A data field.
-        predecessor (typing.Optional[DestinationVersionId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "bigquery"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: DestinationId
     name: DestinationName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
     path: str
     stagingArea: GCSStagingArea
     version: DestinationVersionId
-    predecessor: typing.Optional[DestinationVersionId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for BigQueryDestination data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -1181,21 +1121,15 @@
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
                 "path": {
                     "type": "string"
                 },
                 "stagingArea": GCSStagingArea.json_schema(),
-                "version": DestinationVersionId.json_schema(),
-                "predecessor": {
-                    "oneOf": [
-                        {"type": "null"},
-                        DestinationVersionId.json_schema(),
-                    ]
-                }
+                "version": DestinationVersionId.json_schema()
             },
             "required": [
                 "adt_type",
                 "id",
                 "name",
                 "description",
                 "labels",
@@ -1227,19 +1161,14 @@
                 name=DestinationName.from_json(data["name"]),
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
                 path=str(data["path"]),
                 stagingArea=GCSStagingArea.from_json(data["stagingArea"]),
                 version=DestinationVersionId.from_json(data["version"]),
-                predecessor=(
-                    lambda v: v and DestinationVersionId.from_json(v)
-                )(
-                    data.get("predecessor", None)
-                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing BigQueryDestination",
                 exc_info=ex
             )
             raise
@@ -1255,16 +1184,15 @@
             "id": self.id.to_json(),
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
             "path": str(self.path),
             "stagingArea": self.stagingArea.to_json(),
-            "version": self.version.to_json(),
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "version": self.version.to_json()
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class GCSDestination(Destination):
     """A data destination in Google Cloud Storage.
     
@@ -1274,30 +1202,28 @@
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
         bucket (str): A data field.
         path (str): A data field.
         fileFormat (FileFormat): A data field.
         version (DestinationVersionId): A data field.
-        predecessor (typing.Optional[DestinationVersionId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "gcs"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: DestinationId
     name: DestinationName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
     bucket: str
     path: str
     fileFormat: FileFormat
     version: DestinationVersionId
-    predecessor: typing.Optional[DestinationVersionId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for GCSDestination data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -1325,21 +1251,15 @@
                 "bucket": {
                     "type": "string"
                 },
                 "path": {
                     "type": "string"
                 },
                 "fileFormat": FileFormat.json_schema(),
-                "version": DestinationVersionId.json_schema(),
-                "predecessor": {
-                    "oneOf": [
-                        {"type": "null"},
-                        DestinationVersionId.json_schema(),
-                    ]
-                }
+                "version": DestinationVersionId.json_schema()
             },
             "required": [
                 "adt_type",
                 "id",
                 "name",
                 "description",
                 "labels",
@@ -1373,19 +1293,14 @@
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
                 bucket=str(data["bucket"]),
                 path=str(data["path"]),
                 fileFormat=FileFormat.from_json(data["fileFormat"]),
                 version=DestinationVersionId.from_json(data["version"]),
-                predecessor=(
-                    lambda v: v and DestinationVersionId.from_json(v)
-                )(
-                    data.get("predecessor", None)
-                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing GCSDestination",
                 exc_info=ex
             )
             raise
@@ -1402,16 +1317,15 @@
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
             "bucket": str(self.bucket),
             "path": str(self.path),
             "fileFormat": self.fileFormat.to_json(),
-            "version": self.version.to_json(),
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "version": self.version.to_json()
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class OnlineFeatureStoreDestination(Destination):
     """A data destination on an online feature store.
     
@@ -1421,30 +1335,28 @@
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
         url (str): A data field.
         schema (str): A data field.
         credentialsProvider (CredentialsProviderConfig): A data field.
         version (DestinationVersionId): A data field.
-        predecessor (typing.Optional[DestinationVersionId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "onlinefeaturestore"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: DestinationId
     name: DestinationName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
     url: str
     schema: str
     credentialsProvider: CredentialsProviderConfig
     version: DestinationVersionId
-    predecessor: typing.Optional[DestinationVersionId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for OnlineFeatureStoreDestination data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -1472,21 +1384,15 @@
                 "url": {
                     "type": "string"
                 },
                 "schema": {
                     "type": "string"
                 },
                 "credentialsProvider": CredentialsProviderConfig.json_schema(),
-                "version": DestinationVersionId.json_schema(),
-                "predecessor": {
-                    "oneOf": [
-                        {"type": "null"},
-                        DestinationVersionId.json_schema(),
-                    ]
-                }
+                "version": DestinationVersionId.json_schema()
             },
             "required": [
                 "adt_type",
                 "id",
                 "name",
                 "description",
                 "labels",
@@ -1520,19 +1426,14 @@
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
                 url=str(data["url"]),
                 schema=str(data["schema"]),
                 credentialsProvider=CredentialsProviderConfig.from_json(data["credentialsProvider"]),
                 version=DestinationVersionId.from_json(data["version"]),
-                predecessor=(
-                    lambda v: v and DestinationVersionId.from_json(v)
-                )(
-                    data.get("predecessor", None)
-                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing OnlineFeatureStoreDestination",
                 exc_info=ex
             )
             raise
@@ -1549,16 +1450,15 @@
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
             "url": str(self.url),
             "schema": str(self.schema),
             "credentialsProvider": self.credentialsProvider.to_json(),
-            "version": self.version.to_json(),
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "version": self.version.to_json()
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class LocalDestination(Destination):
     """A data destination on the local filesystem.
     
@@ -1567,29 +1467,27 @@
         name (DestinationName): A data field.
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
         path (str): A data field.
         fileFormat (FileFormat): A data field.
         version (DestinationVersionId): A data field.
-        predecessor (typing.Optional[DestinationVersionId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "local"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: DestinationId
     name: DestinationName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
     path: str
     fileFormat: FileFormat
     version: DestinationVersionId
-    predecessor: typing.Optional[DestinationVersionId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for LocalDestination data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -1614,21 +1512,15 @@
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
                 "path": {
                     "type": "string"
                 },
                 "fileFormat": FileFormat.json_schema(),
-                "version": DestinationVersionId.json_schema(),
-                "predecessor": {
-                    "oneOf": [
-                        {"type": "null"},
-                        DestinationVersionId.json_schema(),
-                    ]
-                }
+                "version": DestinationVersionId.json_schema()
             },
             "required": [
                 "adt_type",
                 "id",
                 "name",
                 "description",
                 "labels",
@@ -1660,19 +1552,14 @@
                 name=DestinationName.from_json(data["name"]),
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
                 path=str(data["path"]),
                 fileFormat=FileFormat.from_json(data["fileFormat"]),
                 version=DestinationVersionId.from_json(data["version"]),
-                predecessor=(
-                    lambda v: v and DestinationVersionId.from_json(v)
-                )(
-                    data.get("predecessor", None)
-                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing LocalDestination",
                 exc_info=ex
             )
             raise
@@ -1688,16 +1575,15 @@
             "id": self.id.to_json(),
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
             "path": str(self.path),
             "fileFormat": self.fileFormat.to_json(),
-            "version": self.version.to_json(),
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "version": self.version.to_json()
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class HDFSDestination(Destination):
     """A data destination in HDFS.
     
@@ -1706,29 +1592,27 @@
         name (DestinationName): A data field.
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
         path (str): A data field.
         fileFormat (FileFormat): A data field.
         version (DestinationVersionId): A data field.
-        predecessor (typing.Optional[DestinationVersionId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "hdfs"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: DestinationId
     name: DestinationName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
     path: str
     fileFormat: FileFormat
     version: DestinationVersionId
-    predecessor: typing.Optional[DestinationVersionId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for HDFSDestination data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -1753,21 +1637,15 @@
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
                 "path": {
                     "type": "string"
                 },
                 "fileFormat": FileFormat.json_schema(),
-                "version": DestinationVersionId.json_schema(),
-                "predecessor": {
-                    "oneOf": [
-                        {"type": "null"},
-                        DestinationVersionId.json_schema(),
-                    ]
-                }
+                "version": DestinationVersionId.json_schema()
             },
             "required": [
                 "adt_type",
                 "id",
                 "name",
                 "description",
                 "labels",
@@ -1799,19 +1677,14 @@
                 name=DestinationName.from_json(data["name"]),
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
                 path=str(data["path"]),
                 fileFormat=FileFormat.from_json(data["fileFormat"]),
                 version=DestinationVersionId.from_json(data["version"]),
-                predecessor=(
-                    lambda v: v and DestinationVersionId.from_json(v)
-                )(
-                    data.get("predecessor", None)
-                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing HDFSDestination",
                 exc_info=ex
             )
             raise
@@ -1827,16 +1700,15 @@
             "id": self.id.to_json(),
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
             "path": str(self.path),
             "fileFormat": self.fileFormat.to_json(),
-            "version": self.version.to_json(),
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "version": self.version.to_json()
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class KafkaDestination(Destination):
     """A data destination in a Kafka cluster.
     
@@ -1846,30 +1718,28 @@
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
         bootstrapServers (str): A data field.
         schemaRegistryUrl (str): A data field.
         kafkaPropertiesProviders (typing.List[SensitiveAttribute]): A data field.
         version (DestinationVersionId): A data field.
-        predecessor (typing.Optional[DestinationVersionId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "kafka"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: DestinationId
     name: DestinationName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
     bootstrapServers: str
     schemaRegistryUrl: str
     kafkaPropertiesProviders: typing.List[SensitiveAttribute]
     version: DestinationVersionId
-    predecessor: typing.Optional[DestinationVersionId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for KafkaDestination data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -1900,21 +1770,15 @@
                 "schemaRegistryUrl": {
                     "type": "string"
                 },
                 "kafkaPropertiesProviders": {
                     "type": "array",
                     "item": SensitiveAttribute.json_schema()
                 },
-                "version": DestinationVersionId.json_schema(),
-                "predecessor": {
-                    "oneOf": [
-                        {"type": "null"},
-                        DestinationVersionId.json_schema(),
-                    ]
-                }
+                "version": DestinationVersionId.json_schema()
             },
             "required": [
                 "adt_type",
                 "id",
                 "name",
                 "description",
                 "labels",
@@ -1948,19 +1812,14 @@
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
                 bootstrapServers=str(data["bootstrapServers"]),
                 schemaRegistryUrl=str(data["schemaRegistryUrl"]),
                 kafkaPropertiesProviders=[SensitiveAttribute.from_json(v) for v in data["kafkaPropertiesProviders"]],
                 version=DestinationVersionId.from_json(data["version"]),
-                predecessor=(
-                    lambda v: v and DestinationVersionId.from_json(v)
-                )(
-                    data.get("predecessor", None)
-                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing KafkaDestination",
                 exc_info=ex
             )
             raise
@@ -1977,10 +1836,9 @@
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
             "bootstrapServers": str(self.bootstrapServers),
             "schemaRegistryUrl": str(self.schemaRegistryUrl),
             "kafkaPropertiesProviders": [v.to_json() for v in self.kafkaPropertiesProviders],
-            "version": self.version.to_json(),
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "version": self.version.to_json()
         }
```

### Comparing `anaml-client-0.8.0/src/anaml_client/models/destination_creation_request/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/destination_creation_request/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/destination_reference/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/destination_reference/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/entity/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/entity_creation_request/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/entity_creation_request/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/entity_mapping/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/entity_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/entity_mapping_creation_request/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/entity_mapping_creation_request/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/event/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/event/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/event_description/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/event_description/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/event_window/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/event_window/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/feature/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/feature/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,44 +21,41 @@
 from ..entity import EntityId
 from ..event_window import EventWindow
 from ..feature_id import FeatureId, FeatureName, FeatureVersionId
 from ..feature_template import TemplateId
 from ..filter_expression import FilterExpression
 from ..label import Label
 from ..post_aggregate_expression import PostAggregateExpression
-from ..quality_rating import QualityRating
 from ..select_expression import SelectExpression
 from ..table import TableId
 
 
 @dataclasses.dataclass(frozen=True)
 class Feature(abc.ABC):
     """Details of a single feature.
     
     Args:
         attributes (typing.List[Attribute]): A data field.
         description (str): A data field.
         id (FeatureId): A data field.
         labels (typing.List[Label]): A data field.
         name (FeatureName): A data field.
-        qualityRating (typing.Optional[QualityRating]): A data field.
         select (SelectExpression): A data field.
         template (typing.Optional[TemplateId]): A data field.
         version (FeatureVersionId): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = ""
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     attributes: typing.List[Attribute]
     description: str
     id: FeatureId
     labels: typing.List[Label]
     name: FeatureName
-    qualityRating: typing.Optional[QualityRating]
     select: SelectExpression
     template: typing.Optional[TemplateId]
     version: FeatureVersionId
     
     @classmethod
     def json_schema(cls):
         """JSON schema for variant Feature.
@@ -121,15 +118,14 @@
     
     Args:
         id (FeatureId): A data field.
         name (FeatureName): A data field.
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
-        qualityRating (typing.Optional[QualityRating]): A data field.
         table (TableId): A data field.
         window (EventWindow): A data field.
         select (SelectExpression): A data field.
         filter (typing.Optional[FilterExpression]): A data field.
         aggregate (AggregateExpression): A data field.
         postAggregateExpr (typing.Optional[PostAggregateExpression]): A data field.
         template (typing.Optional[TemplateId]): A data field.
@@ -140,15 +136,14 @@
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: FeatureId
     name: FeatureName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
-    qualityRating: typing.Optional[QualityRating]
     table: TableId
     window: EventWindow
     select: SelectExpression
     filter: typing.Optional[FilterExpression]
     aggregate: AggregateExpression
     postAggregateExpr: typing.Optional[PostAggregateExpression]
     template: typing.Optional[TemplateId]
@@ -177,20 +172,14 @@
                     "type": "array",
                     "item": Label.json_schema()
                 },
                 "attributes": {
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
-                "qualityRating": {
-                    "oneOf": [
-                        {"type": "null"},
-                        QualityRating.json_schema(),
-                    ]
-                },
                 "table": TableId.json_schema(),
                 "window": EventWindow.json_schema(),
                 "select": SelectExpression.json_schema(),
                 "filter": {
                     "oneOf": [
                         {"type": "null"},
                         FilterExpression.json_schema(),
@@ -244,19 +233,14 @@
             jsonschema.validate(data, cls.json_schema())
             return EventFeature(
                 id=FeatureId.from_json(data["id"]),
                 name=FeatureName.from_json(data["name"]),
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
-                qualityRating=(
-                    lambda v: v and QualityRating.from_json(v)
-                )(
-                    data.get("qualityRating", None)
-                ),
                 table=TableId.from_json(data["table"]),
                 window=EventWindow.from_json(data["window"]),
                 select=SelectExpression.from_json(data["select"]),
                 filter=(
                     lambda v: v and FilterExpression.from_json(v)
                 )(
                     data.get("filter", None)
@@ -286,15 +270,14 @@
         return {
             "adt_type": self.ADT_TYPE,
             "id": self.id.to_json(),
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
-            "qualityRating": (lambda v: v and v.to_json())(self.qualityRating),
             "table": self.table.to_json(),
             "window": self.window.to_json(),
             "select": self.select.to_json(),
             "filter": (lambda v: v and v.to_json())(self.filter),
             "aggregate": self.aggregate.to_json(),
             "postAggregateExpr": (lambda v: v and v.to_json())(self.postAggregateExpr),
             "template": (lambda v: v and v.to_json())(self.template),
@@ -308,15 +291,14 @@
     
     Args:
         id (FeatureId): A data field.
         name (FeatureName): A data field.
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
-        qualityRating (typing.Optional[QualityRating]): A data field.
         over (typing.List[FeatureId]): A data field.
         select (SelectExpression): A data field.
         entityId (EntityId): A data field.
         template (typing.Optional[TemplateId]): A data field.
         version (FeatureVersionId): A data field.
     """
     
@@ -324,15 +306,14 @@
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: FeatureId
     name: FeatureName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
-    qualityRating: typing.Optional[QualityRating]
     over: typing.List[FeatureId]
     select: SelectExpression
     entityId: EntityId
     template: typing.Optional[TemplateId]
     version: FeatureVersionId
     
     @classmethod
@@ -358,20 +339,14 @@
                     "type": "array",
                     "item": Label.json_schema()
                 },
                 "attributes": {
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
-                "qualityRating": {
-                    "oneOf": [
-                        {"type": "null"},
-                        QualityRating.json_schema(),
-                    ]
-                },
                 "over": {
                     "type": "array",
                     "item": FeatureId.json_schema()
                 },
                 "select": SelectExpression.json_schema(),
                 "entityId": EntityId.json_schema(),
                 "template": {
@@ -414,19 +389,14 @@
             jsonschema.validate(data, cls.json_schema())
             return RowFeature(
                 id=FeatureId.from_json(data["id"]),
                 name=FeatureName.from_json(data["name"]),
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
-                qualityRating=(
-                    lambda v: v and QualityRating.from_json(v)
-                )(
-                    data.get("qualityRating", None)
-                ),
                 over=[FeatureId.from_json(v) for v in data["over"]],
                 select=SelectExpression.from_json(data["select"]),
                 entityId=EntityId.from_json(data["entityId"]),
                 template=(lambda v: v and TemplateId.from_json(v))(data.get("template", None)),
                 version=FeatureVersionId.from_json(data["version"]),
             )
         except jsonschema.exceptions.ValidationError as ex:
@@ -445,14 +415,13 @@
         return {
             "adt_type": self.ADT_TYPE,
             "id": self.id.to_json(),
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
-            "qualityRating": (lambda v: v and v.to_json())(self.qualityRating),
             "over": [v.to_json() for v in self.over],
             "select": self.select.to_json(),
             "entityId": self.entityId.to_json(),
             "template": (lambda v: v and v.to_json())(self.template),
             "version": self.version.to_json()
         }
```

### Comparing `anaml-client-0.8.0/src/anaml_client/models/feature_creation_request/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/feature_template_creation_request/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-"""Generated implementation of feature_creation_request."""
+"""Generated implementation of feature_template_creation_request."""
 
 # WARNING DO NOT EDIT
-# This code was generated from feature-creation-request.mcn
+# This code was generated from feature-template-creation-request.mcn
 
 from __future__ import annotations
 
 import abc  # noqa: F401
 import dataclasses  # noqa: F401
 import datetime  # noqa: F401
 import enum  # noqa: F401
@@ -16,52 +16,47 @@
 import typing  # noqa: F401
 import uuid  # noqa: F401
 
 from ..aggregate import AggregateExpression
 from ..attribute import Attribute
 from ..entity import EntityId
 from ..event_window import EventWindow
-from ..feature_id import FeatureId, FeatureName
-from ..feature_template import TemplateId
+from ..feature_id import FeatureId
+from ..feature_template import TemplateName
 from ..filter_expression import FilterExpression
 from ..label import Label
 from ..post_aggregate_expression import PostAggregateExpression
-from ..quality_rating import QualityRating
 from ..select_expression import SelectExpression
 from ..table import TableId
 
 
 @dataclasses.dataclass(frozen=True)
-class FeatureCreationRequest(abc.ABC):
-    """Request to create a new feature.
+class FeatureTemplateCreationRequest(abc.ABC):
+    """Request to create a new feature template.
     
     Args:
         attributes (typing.List[Attribute]): A data field.
         description (str): A data field.
         labels (typing.List[Label]): A data field.
-        name (FeatureName): A data field.
-        qualityRating (typing.Optional[QualityRating]): A data field.
+        name (TemplateName): A data field.
         select (SelectExpression): A data field.
-        template (typing.Optional[TemplateId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = ""
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     attributes: typing.List[Attribute]
     description: str
     labels: typing.List[Label]
-    name: FeatureName
-    qualityRating: typing.Optional[QualityRating]
+    name: TemplateName
     select: SelectExpression
-    template: typing.Optional[TemplateId]
     
     @classmethod
     def json_schema(cls):
-        """JSON schema for variant FeatureCreationRequest.
+        """JSON schema for variant FeatureTemplateCreationRequest.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         adt_types = [klass.ADT_TYPE for klass in cls.__subclasses__()]
         return {
             "type": "object",
@@ -74,195 +69,181 @@
             "required": [
                 "adt_type",
             ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
-        """Validate and parse JSON data into an instance of FeatureCreationRequest.
+        """Validate and parse JSON data into an instance of FeatureTemplateCreationRequest.
         
         Args:
             data (dict): JSON data to validate and parse.
         
         Returns:
-            An instance of FeatureCreationRequest.
+            An instance of FeatureTemplateCreationRequest.
         
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
             adt_type = data.get("adt_type", None)
             for klass in cls.__subclasses__():
                 if klass.ADT_TYPE == adt_type:
                     return klass.from_json(data)
             raise ValueError("Unknown adt_type: '{ty}'".format(ty=adt_type))
         except jsonschema.exceptions.ValidationError as ex:
-            logging.debug("Invalid JSON data received while parsing FeatureCreationRequest", exc_info=ex)
+            logging.debug("Invalid JSON data received while parsing FeatureTemplateCreationRequest", exc_info=ex)
             raise
     
     @abc.abstractmethod
     def to_json(self):
         """Serialise this instance as JSON.
         
         Returns:
             Data ready to serialise as JSON.
         """
         raise NotImplementedError
 
 
 @dataclasses.dataclass(frozen=True)
-class EventFeatureCreationRequest(FeatureCreationRequest):
-    """Request to create a new feature defined on events.
+class EventFeatureTemplateCreationRequest(FeatureTemplateCreationRequest):
+    """Create a new event feature template.
     
     Args:
-        name (FeatureName): A data field.
+        name (TemplateName): A data field.
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
-        qualityRating (typing.Optional[QualityRating]): A data field.
         table (TableId): A data field.
         window (EventWindow): A data field.
         select (SelectExpression): A data field.
         filter (typing.Optional[FilterExpression]): A data field.
-        aggregate (AggregateExpression): A data field.
+        aggregate (typing.Optional[AggregateExpression]): A data field.
         postAggregateExpr (typing.Optional[PostAggregateExpression]): A data field.
-        template (typing.Optional[TemplateId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "event"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
-    name: FeatureName
+    name: TemplateName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
-    qualityRating: typing.Optional[QualityRating]
     table: TableId
     window: EventWindow
     select: SelectExpression
     filter: typing.Optional[FilterExpression]
-    aggregate: AggregateExpression
+    aggregate: typing.Optional[AggregateExpression]
     postAggregateExpr: typing.Optional[PostAggregateExpression]
-    template: typing.Optional[TemplateId]
     
     @classmethod
     def json_schema(cls):
-        """Return the JSON schema for EventFeatureCreationRequest data.
+        """Return the JSON schema for EventFeatureTemplateCreationRequest data.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         return {
             "type": "object",
             "properties": {
                 "adt_type": {
                     "type": "string",
                     "enum": [cls.ADT_TYPE]
                 },
-                "name": FeatureName.json_schema(),
+                "name": TemplateName.json_schema(),
                 "description": {
                     "type": "string"
                 },
                 "labels": {
                     "type": "array",
                     "item": Label.json_schema()
                 },
                 "attributes": {
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
-                "qualityRating": {
-                    "oneOf": [
-                        {"type": "null"},
-                        QualityRating.json_schema(),
-                    ]
-                },
                 "table": TableId.json_schema(),
                 "window": EventWindow.json_schema(),
                 "select": SelectExpression.json_schema(),
                 "filter": {
                     "oneOf": [
                         {"type": "null"},
                         FilterExpression.json_schema(),
                     ]
                 },
-                "aggregate": AggregateExpression.json_schema(),
-                "postAggregateExpr": {
+                "aggregate": {
                     "oneOf": [
                         {"type": "null"},
-                        PostAggregateExpression.json_schema(),
+                        AggregateExpression.json_schema(),
                     ]
                 },
-                "template": {
+                "postAggregateExpr": {
                     "oneOf": [
                         {"type": "null"},
-                        TemplateId.json_schema(),
+                        PostAggregateExpression.json_schema(),
                     ]
                 }
             },
             "required": [
                 "adt_type",
                 "name",
                 "description",
                 "labels",
                 "attributes",
                 "table",
                 "window",
                 "select",
-                "aggregate",
             ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
-        """Validate and parse JSON data into an instance of EventFeatureCreationRequest.
+        """Validate and parse JSON data into an instance of EventFeatureTemplateCreationRequest.
         
         Args:
             data (dict): JSON data to validate and parse.
         
         Returns:
-            An instance of EventFeatureCreationRequest.
+            An instance of EventFeatureTemplateCreationRequest.
         
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
-            return EventFeatureCreationRequest(
-                name=FeatureName.from_json(data["name"]),
+            return EventFeatureTemplateCreationRequest(
+                name=TemplateName.from_json(data["name"]),
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
-                qualityRating=(
-                    lambda v: v and QualityRating.from_json(v)
-                )(
-                    data.get("qualityRating", None)
-                ),
                 table=TableId.from_json(data["table"]),
                 window=EventWindow.from_json(data["window"]),
                 select=SelectExpression.from_json(data["select"]),
                 filter=(
                     lambda v: v and FilterExpression.from_json(v)
                 )(
                     data.get("filter", None)
                 ),
-                aggregate=AggregateExpression.from_json(data["aggregate"]),
+                aggregate=(
+                    lambda v: v and AggregateExpression.from_json(v)
+                )(
+                    data.get("aggregate", None)
+                ),
                 postAggregateExpr=(
                     lambda v: v and PostAggregateExpression.from_json(v)
                 )(
                     data.get("postAggregateExpr", None)
                 ),
-                template=(lambda v: v and TemplateId.from_json(v))(data.get("template", None)),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
-                "Invalid JSON data received while parsing EventFeatureCreationRequest",
+                "Invalid JSON data received while parsing EventFeatureTemplateCreationRequest",
                 exc_info=ex
             )
             raise
     
     def to_json(self):
         """Serialise this instance as JSON.
         
@@ -271,98 +252,80 @@
         """
         return {
             "adt_type": self.ADT_TYPE,
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
-            "qualityRating": (lambda v: v and v.to_json())(self.qualityRating),
             "table": self.table.to_json(),
             "window": self.window.to_json(),
             "select": self.select.to_json(),
             "filter": (lambda v: v and v.to_json())(self.filter),
-            "aggregate": self.aggregate.to_json(),
-            "postAggregateExpr": (lambda v: v and v.to_json())(self.postAggregateExpr),
-            "template": (lambda v: v and v.to_json())(self.template)
+            "aggregate": (lambda v: v and v.to_json())(self.aggregate),
+            "postAggregateExpr": (lambda v: v and v.to_json())(self.postAggregateExpr)
         }
 
 
 @dataclasses.dataclass(frozen=True)
-class RowFeatureCreationRequest(FeatureCreationRequest):
-    """Request to create a new feature defined on rows.
+class RowFeatureTemplateCreationRequest(FeatureTemplateCreationRequest):
+    """Create a new row feature template.
     
     Args:
-        name (FeatureName): A data field.
+        name (TemplateName): A data field.
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
-        qualityRating (typing.Optional[QualityRating]): A data field.
         over (typing.List[FeatureId]): A data field.
         select (SelectExpression): A data field.
         entityId (EntityId): A data field.
-        template (typing.Optional[TemplateId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "row"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
-    name: FeatureName
+    name: TemplateName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
-    qualityRating: typing.Optional[QualityRating]
     over: typing.List[FeatureId]
     select: SelectExpression
     entityId: EntityId
-    template: typing.Optional[TemplateId]
     
     @classmethod
     def json_schema(cls):
-        """Return the JSON schema for RowFeatureCreationRequest data.
+        """Return the JSON schema for RowFeatureTemplateCreationRequest data.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         return {
             "type": "object",
             "properties": {
                 "adt_type": {
                     "type": "string",
                     "enum": [cls.ADT_TYPE]
                 },
-                "name": FeatureName.json_schema(),
+                "name": TemplateName.json_schema(),
                 "description": {
                     "type": "string"
                 },
                 "labels": {
                     "type": "array",
                     "item": Label.json_schema()
                 },
                 "attributes": {
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
-                "qualityRating": {
-                    "oneOf": [
-                        {"type": "null"},
-                        QualityRating.json_schema(),
-                    ]
-                },
                 "over": {
                     "type": "array",
                     "item": FeatureId.json_schema()
                 },
                 "select": SelectExpression.json_schema(),
-                "entityId": EntityId.json_schema(),
-                "template": {
-                    "oneOf": [
-                        {"type": "null"},
-                        TemplateId.json_schema(),
-                    ]
-                }
+                "entityId": EntityId.json_schema()
             },
             "required": [
                 "adt_type",
                 "name",
                 "description",
                 "labels",
                 "attributes",
@@ -370,46 +333,40 @@
                 "select",
                 "entityId",
             ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
-        """Validate and parse JSON data into an instance of RowFeatureCreationRequest.
+        """Validate and parse JSON data into an instance of RowFeatureTemplateCreationRequest.
         
         Args:
             data (dict): JSON data to validate and parse.
         
         Returns:
-            An instance of RowFeatureCreationRequest.
+            An instance of RowFeatureTemplateCreationRequest.
         
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
-            return RowFeatureCreationRequest(
-                name=FeatureName.from_json(data["name"]),
+            return RowFeatureTemplateCreationRequest(
+                name=TemplateName.from_json(data["name"]),
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
-                qualityRating=(
-                    lambda v: v and QualityRating.from_json(v)
-                )(
-                    data.get("qualityRating", None)
-                ),
                 over=[FeatureId.from_json(v) for v in data["over"]],
                 select=SelectExpression.from_json(data["select"]),
                 entityId=EntityId.from_json(data["entityId"]),
-                template=(lambda v: v and TemplateId.from_json(v))(data.get("template", None)),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
-                "Invalid JSON data received while parsing RowFeatureCreationRequest",
+                "Invalid JSON data received while parsing RowFeatureTemplateCreationRequest",
                 exc_info=ex
             )
             raise
     
     def to_json(self):
         """Serialise this instance as JSON.
         
@@ -418,13 +375,11 @@
         """
         return {
             "adt_type": self.ADT_TYPE,
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
-            "qualityRating": (lambda v: v and v.to_json())(self.qualityRating),
             "over": [v.to_json() for v in self.over],
             "select": self.select.to_json(),
-            "entityId": self.entityId.to_json(),
-            "template": (lambda v: v and v.to_json())(self.template)
+            "entityId": self.entityId.to_json()
         }
```

### Comparing `anaml-client-0.8.0/src/anaml_client/models/feature_id/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/feature_id/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/feature_run_summaries/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/feature_run_summaries/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/feature_set/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/feature_set/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/feature_set_creation_request/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/feature_set_creation_request/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/feature_store/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/feature_store/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/feature_store_creation_request/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/feature_store_creation_request/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/feature_store_run/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/feature_store_run/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/feature_template/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/feature_template/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from ..attribute import Attribute
 from ..entity import EntityId
 from ..event_window import EventWindow
 from ..feature_id import FeatureId
 from ..filter_expression import FilterExpression
 from ..label import Label
 from ..post_aggregate_expression import PostAggregateExpression
-from ..quality_rating import QualityRating
 from ..select_expression import SelectExpression
 from ..table import TableId
 
 
 @dataclasses.dataclass(frozen=True)
 class TemplateId:
     """Unique identifier for a feature template.
@@ -232,28 +231,26 @@
     
     Args:
         attributes (typing.List[Attribute]): A data field.
         description (str): A data field.
         id (TemplateId): A data field.
         labels (typing.List[Label]): A data field.
         name (TemplateName): A data field.
-        qualityRating (typing.Optional[QualityRating]): A data field.
         select (SelectExpression): A data field.
         version (TemplateVersionId): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = ""
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     attributes: typing.List[Attribute]
     description: str
     id: TemplateId
     labels: typing.List[Label]
     name: TemplateName
-    qualityRating: typing.Optional[QualityRating]
     select: SelectExpression
     version: TemplateVersionId
     
     @classmethod
     def json_schema(cls):
         """JSON schema for variant FeatureTemplate.
         
@@ -315,15 +312,14 @@
     
     Args:
         id (TemplateId): A data field.
         name (TemplateName): A data field.
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
-        qualityRating (typing.Optional[QualityRating]): A data field.
         table (TableId): A data field.
         window (EventWindow): A data field.
         select (SelectExpression): A data field.
         filter (typing.Optional[FilterExpression]): A data field.
         aggregate (typing.Optional[AggregateExpression]): A data field.
         postAggregateExpr (typing.Optional[PostAggregateExpression]): A data field.
         version (TemplateVersionId): A data field.
@@ -333,15 +329,14 @@
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: TemplateId
     name: TemplateName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
-    qualityRating: typing.Optional[QualityRating]
     table: TableId
     window: EventWindow
     select: SelectExpression
     filter: typing.Optional[FilterExpression]
     aggregate: typing.Optional[AggregateExpression]
     postAggregateExpr: typing.Optional[PostAggregateExpression]
     version: TemplateVersionId
@@ -369,20 +364,14 @@
                     "type": "array",
                     "item": Label.json_schema()
                 },
                 "attributes": {
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
-                "qualityRating": {
-                    "oneOf": [
-                        {"type": "null"},
-                        QualityRating.json_schema(),
-                    ]
-                },
                 "table": TableId.json_schema(),
                 "window": EventWindow.json_schema(),
                 "select": SelectExpression.json_schema(),
                 "filter": {
                     "oneOf": [
                         {"type": "null"},
                         FilterExpression.json_schema(),
@@ -434,19 +423,14 @@
             jsonschema.validate(data, cls.json_schema())
             return EventFeatureTemplate(
                 id=TemplateId.from_json(data["id"]),
                 name=TemplateName.from_json(data["name"]),
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
-                qualityRating=(
-                    lambda v: v and QualityRating.from_json(v)
-                )(
-                    data.get("qualityRating", None)
-                ),
                 table=TableId.from_json(data["table"]),
                 window=EventWindow.from_json(data["window"]),
                 select=SelectExpression.from_json(data["select"]),
                 filter=(
                     lambda v: v and FilterExpression.from_json(v)
                 )(
                     data.get("filter", None)
@@ -479,15 +463,14 @@
         return {
             "adt_type": self.ADT_TYPE,
             "id": self.id.to_json(),
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
-            "qualityRating": (lambda v: v and v.to_json())(self.qualityRating),
             "table": self.table.to_json(),
             "window": self.window.to_json(),
             "select": self.select.to_json(),
             "filter": (lambda v: v and v.to_json())(self.filter),
             "aggregate": (lambda v: v and v.to_json())(self.aggregate),
             "postAggregateExpr": (lambda v: v and v.to_json())(self.postAggregateExpr),
             "version": self.version.to_json()
@@ -500,30 +483,28 @@
     
     Args:
         id (TemplateId): A data field.
         name (TemplateName): A data field.
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
-        qualityRating (typing.Optional[QualityRating]): A data field.
         over (typing.List[FeatureId]): A data field.
         select (SelectExpression): A data field.
         entityId (EntityId): A data field.
         version (TemplateVersionId): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "row"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: TemplateId
     name: TemplateName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
-    qualityRating: typing.Optional[QualityRating]
     over: typing.List[FeatureId]
     select: SelectExpression
     entityId: EntityId
     version: TemplateVersionId
     
     @classmethod
     def json_schema(cls):
@@ -548,20 +529,14 @@
                     "type": "array",
                     "item": Label.json_schema()
                 },
                 "attributes": {
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
-                "qualityRating": {
-                    "oneOf": [
-                        {"type": "null"},
-                        QualityRating.json_schema(),
-                    ]
-                },
                 "over": {
                     "type": "array",
                     "item": FeatureId.json_schema()
                 },
                 "select": SelectExpression.json_schema(),
                 "entityId": EntityId.json_schema(),
                 "version": TemplateVersionId.json_schema()
@@ -598,19 +573,14 @@
             jsonschema.validate(data, cls.json_schema())
             return RowFeatureTemplate(
                 id=TemplateId.from_json(data["id"]),
                 name=TemplateName.from_json(data["name"]),
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
-                qualityRating=(
-                    lambda v: v and QualityRating.from_json(v)
-                )(
-                    data.get("qualityRating", None)
-                ),
                 over=[FeatureId.from_json(v) for v in data["over"]],
                 select=SelectExpression.from_json(data["select"]),
                 entityId=EntityId.from_json(data["entityId"]),
                 version=TemplateVersionId.from_json(data["version"]),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
@@ -628,13 +598,12 @@
         return {
             "adt_type": self.ADT_TYPE,
             "id": self.id.to_json(),
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
-            "qualityRating": (lambda v: v and v.to_json())(self.qualityRating),
             "over": [v.to_json() for v in self.over],
             "select": self.select.to_json(),
             "entityId": self.entityId.to_json(),
             "version": self.version.to_json()
         }
```

### Comparing `anaml-client-0.8.0/src/anaml_client/models/feature_template_creation_request/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/feature_creation_request/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-"""Generated implementation of feature_template_creation_request."""
+"""Generated implementation of feature_creation_request."""
 
 # WARNING DO NOT EDIT
-# This code was generated from feature-template-creation-request.mcn
+# This code was generated from feature-creation-request.mcn
 
 from __future__ import annotations
 
 import abc  # noqa: F401
 import dataclasses  # noqa: F401
 import datetime  # noqa: F401
 import enum  # noqa: F401
@@ -16,50 +16,49 @@
 import typing  # noqa: F401
 import uuid  # noqa: F401
 
 from ..aggregate import AggregateExpression
 from ..attribute import Attribute
 from ..entity import EntityId
 from ..event_window import EventWindow
-from ..feature_id import FeatureId
-from ..feature_template import TemplateName
+from ..feature_id import FeatureId, FeatureName
+from ..feature_template import TemplateId
 from ..filter_expression import FilterExpression
 from ..label import Label
 from ..post_aggregate_expression import PostAggregateExpression
-from ..quality_rating import QualityRating
 from ..select_expression import SelectExpression
 from ..table import TableId
 
 
 @dataclasses.dataclass(frozen=True)
-class FeatureTemplateCreationRequest(abc.ABC):
-    """Request to create a new feature template.
+class FeatureCreationRequest(abc.ABC):
+    """Request to create a new feature.
     
     Args:
         attributes (typing.List[Attribute]): A data field.
         description (str): A data field.
         labels (typing.List[Label]): A data field.
-        name (TemplateName): A data field.
-        qualityRating (typing.Optional[QualityRating]): A data field.
+        name (FeatureName): A data field.
         select (SelectExpression): A data field.
+        template (typing.Optional[TemplateId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = ""
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     attributes: typing.List[Attribute]
     description: str
     labels: typing.List[Label]
-    name: TemplateName
-    qualityRating: typing.Optional[QualityRating]
+    name: FeatureName
     select: SelectExpression
+    template: typing.Optional[TemplateId]
     
     @classmethod
     def json_schema(cls):
-        """JSON schema for variant FeatureTemplateCreationRequest.
+        """JSON schema for variant FeatureCreationRequest.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         adt_types = [klass.ADT_TYPE for klass in cls.__subclasses__()]
         return {
             "type": "object",
@@ -72,194 +71,182 @@
             "required": [
                 "adt_type",
             ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
-        """Validate and parse JSON data into an instance of FeatureTemplateCreationRequest.
+        """Validate and parse JSON data into an instance of FeatureCreationRequest.
         
         Args:
             data (dict): JSON data to validate and parse.
         
         Returns:
-            An instance of FeatureTemplateCreationRequest.
+            An instance of FeatureCreationRequest.
         
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
             adt_type = data.get("adt_type", None)
             for klass in cls.__subclasses__():
                 if klass.ADT_TYPE == adt_type:
                     return klass.from_json(data)
             raise ValueError("Unknown adt_type: '{ty}'".format(ty=adt_type))
         except jsonschema.exceptions.ValidationError as ex:
-            logging.debug("Invalid JSON data received while parsing FeatureTemplateCreationRequest", exc_info=ex)
+            logging.debug("Invalid JSON data received while parsing FeatureCreationRequest", exc_info=ex)
             raise
     
     @abc.abstractmethod
     def to_json(self):
         """Serialise this instance as JSON.
         
         Returns:
             Data ready to serialise as JSON.
         """
         raise NotImplementedError
 
 
 @dataclasses.dataclass(frozen=True)
-class EventFeatureTemplateCreationRequest(FeatureTemplateCreationRequest):
-    """Create a new event feature template.
+class EventFeatureCreationRequest(FeatureCreationRequest):
+    """Request to create a new feature defined on events.
     
     Args:
-        name (TemplateName): A data field.
+        name (FeatureName): A data field.
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
-        qualityRating (typing.Optional[QualityRating]): A data field.
         table (TableId): A data field.
         window (EventWindow): A data field.
         select (SelectExpression): A data field.
         filter (typing.Optional[FilterExpression]): A data field.
-        aggregate (typing.Optional[AggregateExpression]): A data field.
+        aggregate (AggregateExpression): A data field.
         postAggregateExpr (typing.Optional[PostAggregateExpression]): A data field.
+        template (typing.Optional[TemplateId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "event"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
-    name: TemplateName
+    name: FeatureName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
-    qualityRating: typing.Optional[QualityRating]
     table: TableId
     window: EventWindow
     select: SelectExpression
     filter: typing.Optional[FilterExpression]
-    aggregate: typing.Optional[AggregateExpression]
+    aggregate: AggregateExpression
     postAggregateExpr: typing.Optional[PostAggregateExpression]
+    template: typing.Optional[TemplateId]
     
     @classmethod
     def json_schema(cls):
-        """Return the JSON schema for EventFeatureTemplateCreationRequest data.
+        """Return the JSON schema for EventFeatureCreationRequest data.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         return {
             "type": "object",
             "properties": {
                 "adt_type": {
                     "type": "string",
                     "enum": [cls.ADT_TYPE]
                 },
-                "name": TemplateName.json_schema(),
+                "name": FeatureName.json_schema(),
                 "description": {
                     "type": "string"
                 },
                 "labels": {
                     "type": "array",
                     "item": Label.json_schema()
                 },
                 "attributes": {
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
-                "qualityRating": {
-                    "oneOf": [
-                        {"type": "null"},
-                        QualityRating.json_schema(),
-                    ]
-                },
                 "table": TableId.json_schema(),
                 "window": EventWindow.json_schema(),
                 "select": SelectExpression.json_schema(),
                 "filter": {
                     "oneOf": [
                         {"type": "null"},
                         FilterExpression.json_schema(),
                     ]
                 },
-                "aggregate": {
+                "aggregate": AggregateExpression.json_schema(),
+                "postAggregateExpr": {
                     "oneOf": [
                         {"type": "null"},
-                        AggregateExpression.json_schema(),
+                        PostAggregateExpression.json_schema(),
                     ]
                 },
-                "postAggregateExpr": {
+                "template": {
                     "oneOf": [
                         {"type": "null"},
-                        PostAggregateExpression.json_schema(),
+                        TemplateId.json_schema(),
                     ]
                 }
             },
             "required": [
                 "adt_type",
                 "name",
                 "description",
                 "labels",
                 "attributes",
                 "table",
                 "window",
                 "select",
+                "aggregate",
             ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
-        """Validate and parse JSON data into an instance of EventFeatureTemplateCreationRequest.
+        """Validate and parse JSON data into an instance of EventFeatureCreationRequest.
         
         Args:
             data (dict): JSON data to validate and parse.
         
         Returns:
-            An instance of EventFeatureTemplateCreationRequest.
+            An instance of EventFeatureCreationRequest.
         
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
-            return EventFeatureTemplateCreationRequest(
-                name=TemplateName.from_json(data["name"]),
+            return EventFeatureCreationRequest(
+                name=FeatureName.from_json(data["name"]),
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
-                qualityRating=(
-                    lambda v: v and QualityRating.from_json(v)
-                )(
-                    data.get("qualityRating", None)
-                ),
                 table=TableId.from_json(data["table"]),
                 window=EventWindow.from_json(data["window"]),
                 select=SelectExpression.from_json(data["select"]),
                 filter=(
                     lambda v: v and FilterExpression.from_json(v)
                 )(
                     data.get("filter", None)
                 ),
-                aggregate=(
-                    lambda v: v and AggregateExpression.from_json(v)
-                )(
-                    data.get("aggregate", None)
-                ),
+                aggregate=AggregateExpression.from_json(data["aggregate"]),
                 postAggregateExpr=(
                     lambda v: v and PostAggregateExpression.from_json(v)
                 )(
                     data.get("postAggregateExpr", None)
                 ),
+                template=(lambda v: v and TemplateId.from_json(v))(data.get("template", None)),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
-                "Invalid JSON data received while parsing EventFeatureTemplateCreationRequest",
+                "Invalid JSON data received while parsing EventFeatureCreationRequest",
                 exc_info=ex
             )
             raise
     
     def to_json(self):
         """Serialise this instance as JSON.
         
@@ -268,89 +255,89 @@
         """
         return {
             "adt_type": self.ADT_TYPE,
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
-            "qualityRating": (lambda v: v and v.to_json())(self.qualityRating),
             "table": self.table.to_json(),
             "window": self.window.to_json(),
             "select": self.select.to_json(),
             "filter": (lambda v: v and v.to_json())(self.filter),
-            "aggregate": (lambda v: v and v.to_json())(self.aggregate),
-            "postAggregateExpr": (lambda v: v and v.to_json())(self.postAggregateExpr)
+            "aggregate": self.aggregate.to_json(),
+            "postAggregateExpr": (lambda v: v and v.to_json())(self.postAggregateExpr),
+            "template": (lambda v: v and v.to_json())(self.template)
         }
 
 
 @dataclasses.dataclass(frozen=True)
-class RowFeatureTemplateCreationRequest(FeatureTemplateCreationRequest):
-    """Create a new row feature template.
+class RowFeatureCreationRequest(FeatureCreationRequest):
+    """Request to create a new feature defined on rows.
     
     Args:
-        name (TemplateName): A data field.
+        name (FeatureName): A data field.
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
-        qualityRating (typing.Optional[QualityRating]): A data field.
         over (typing.List[FeatureId]): A data field.
         select (SelectExpression): A data field.
         entityId (EntityId): A data field.
+        template (typing.Optional[TemplateId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "row"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
-    name: TemplateName
+    name: FeatureName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
-    qualityRating: typing.Optional[QualityRating]
     over: typing.List[FeatureId]
     select: SelectExpression
     entityId: EntityId
+    template: typing.Optional[TemplateId]
     
     @classmethod
     def json_schema(cls):
-        """Return the JSON schema for RowFeatureTemplateCreationRequest data.
+        """Return the JSON schema for RowFeatureCreationRequest data.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         return {
             "type": "object",
             "properties": {
                 "adt_type": {
                     "type": "string",
                     "enum": [cls.ADT_TYPE]
                 },
-                "name": TemplateName.json_schema(),
+                "name": FeatureName.json_schema(),
                 "description": {
                     "type": "string"
                 },
                 "labels": {
                     "type": "array",
                     "item": Label.json_schema()
                 },
                 "attributes": {
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
-                "qualityRating": {
-                    "oneOf": [
-                        {"type": "null"},
-                        QualityRating.json_schema(),
-                    ]
-                },
                 "over": {
                     "type": "array",
                     "item": FeatureId.json_schema()
                 },
                 "select": SelectExpression.json_schema(),
-                "entityId": EntityId.json_schema()
+                "entityId": EntityId.json_schema(),
+                "template": {
+                    "oneOf": [
+                        {"type": "null"},
+                        TemplateId.json_schema(),
+                    ]
+                }
             },
             "required": [
                 "adt_type",
                 "name",
                 "description",
                 "labels",
                 "attributes",
@@ -358,45 +345,41 @@
                 "select",
                 "entityId",
             ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
-        """Validate and parse JSON data into an instance of RowFeatureTemplateCreationRequest.
+        """Validate and parse JSON data into an instance of RowFeatureCreationRequest.
         
         Args:
             data (dict): JSON data to validate and parse.
         
         Returns:
-            An instance of RowFeatureTemplateCreationRequest.
+            An instance of RowFeatureCreationRequest.
         
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
-            return RowFeatureTemplateCreationRequest(
-                name=TemplateName.from_json(data["name"]),
+            return RowFeatureCreationRequest(
+                name=FeatureName.from_json(data["name"]),
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
-                qualityRating=(
-                    lambda v: v and QualityRating.from_json(v)
-                )(
-                    data.get("qualityRating", None)
-                ),
                 over=[FeatureId.from_json(v) for v in data["over"]],
                 select=SelectExpression.from_json(data["select"]),
                 entityId=EntityId.from_json(data["entityId"]),
+                template=(lambda v: v and TemplateId.from_json(v))(data.get("template", None)),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
-                "Invalid JSON data received while parsing RowFeatureTemplateCreationRequest",
+                "Invalid JSON data received while parsing RowFeatureCreationRequest",
                 exc_info=ex
             )
             raise
     
     def to_json(self):
         """Serialise this instance as JSON.
         
@@ -405,12 +388,12 @@
         """
         return {
             "adt_type": self.ADT_TYPE,
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
-            "qualityRating": (lambda v: v and v.to_json())(self.qualityRating),
             "over": [v.to_json() for v in self.over],
             "select": self.select.to_json(),
-            "entityId": self.entityId.to_json()
+            "entityId": self.entityId.to_json(),
+            "template": (lambda v: v and v.to_json())(self.template)
         }
```

### Comparing `anaml-client-0.8.0/src/anaml_client/models/file_format/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/ref/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-"""Generated implementation of file_format."""
+"""Generated implementation of ref."""
 
 # WARNING DO NOT EDIT
-# This code was generated from file-format.mcn
+# This code was generated from ref.mcn
 
 from __future__ import annotations
 
 import abc  # noqa: F401
 import dataclasses  # noqa: F401
 import datetime  # noqa: F401
 import enum  # noqa: F401
@@ -14,23 +14,29 @@
 import jsonschema  # noqa: F401
 import logging  # noqa: F401
 import typing  # noqa: F401
 import uuid  # noqa: F401
 
 
 @dataclasses.dataclass(frozen=True)
-class FileFormat(abc.ABC):
-    """Supported data store file formats."""
+class Ref(abc.ABC):
+    """A reference to a branch or commit.
+    
+    Args:
+        ref (str): A data field.
+    """
     
     ADT_TYPE: typing.ClassVar[str] = ""
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
+    ref: str
+    
     @classmethod
     def json_schema(cls):
-        """JSON schema for variant FileFormat.
+        """JSON schema for variant Ref.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         adt_types = [klass.ADT_TYPE for klass in cls.__subclasses__()]
         return {
             "type": "object",
@@ -43,241 +49,188 @@
             "required": [
                 "adt_type",
             ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
-        """Validate and parse JSON data into an instance of FileFormat.
+        """Validate and parse JSON data into an instance of Ref.
         
         Args:
             data (dict): JSON data to validate and parse.
         
         Returns:
-            An instance of FileFormat.
+            An instance of Ref.
         
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
             adt_type = data.get("adt_type", None)
             for klass in cls.__subclasses__():
                 if klass.ADT_TYPE == adt_type:
                     return klass.from_json(data)
             raise ValueError("Unknown adt_type: '{ty}'".format(ty=adt_type))
         except jsonschema.exceptions.ValidationError as ex:
-            logging.debug("Invalid JSON data received while parsing FileFormat", exc_info=ex)
+            logging.debug("Invalid JSON data received while parsing Ref", exc_info=ex)
             raise
     
     @abc.abstractmethod
     def to_json(self):
         """Serialise this instance as JSON.
         
         Returns:
             Data ready to serialise as JSON.
         """
         raise NotImplementedError
 
 
 @dataclasses.dataclass(frozen=True)
-class Parquet(FileFormat):
-    """Apache Parquet format."""
-    
-    ADT_TYPE: typing.ClassVar[str] = "parquet"
-    adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
-    
-    @classmethod
-    def json_schema(cls):
-        """Return the JSON schema for Parquet data.
-        
-        Returns:
-            A Python dictionary describing the JSON schema.
-        """
-        return {
-            "type": "object",
-            "properties": {
-                "adt_type": {
-                    "type": "string",
-                    "enum": [cls.ADT_TYPE]
-                }
-            },
-            "required": [
-                "adt_type",
-            ]
-        }
-    
-    @classmethod
-    def from_json(cls, data: dict):
-        """Validate and parse JSON data into an instance of Parquet.
-        
-        Args:
-            data (dict): JSON data to validate and parse.
-        
-        Returns:
-            An instance of Parquet.
-        
-        Raises:
-            ValidationError: When schema validation fails.
-            KeyError: When a required field is missing from the JSON.
-        """
-        try:
-            jsonschema.validate(data, cls.json_schema())
-            return Parquet(
-                
-            )
-        except jsonschema.exceptions.ValidationError as ex:
-            logging.debug(
-                "Invalid JSON data received while parsing Parquet",
-                exc_info=ex
-            )
-            raise
+class CommitRef(Ref):
+    """A reference to a specific commit.
     
-    def to_json(self):
-        """Serialise this instance as JSON.
-        
-        Returns:
-            Data ready to serialise as JSON.
-        """
-        return {
-            "adt_type": self.ADT_TYPE
-        }
-
-
-@dataclasses.dataclass(frozen=True)
-class Orc(FileFormat):
-    """Apache Orc format."""
+    Args:
+        ref (str): A data field.
+    """
     
-    ADT_TYPE: typing.ClassVar[str] = "orc"
+    ADT_TYPE: typing.ClassVar[str] = "commit"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
+    ref: str
+    
     @classmethod
     def json_schema(cls):
-        """Return the JSON schema for Orc data.
+        """Return the JSON schema for CommitRef data.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         return {
             "type": "object",
             "properties": {
                 "adt_type": {
                     "type": "string",
                     "enum": [cls.ADT_TYPE]
+                },
+                "ref": {
+                    "type": "string"
                 }
             },
             "required": [
                 "adt_type",
+                "ref",
             ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
-        """Validate and parse JSON data into an instance of Orc.
+        """Validate and parse JSON data into an instance of CommitRef.
         
         Args:
             data (dict): JSON data to validate and parse.
         
         Returns:
-            An instance of Orc.
+            An instance of CommitRef.
         
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
-            return Orc(
-                
+            return CommitRef(
+                ref=str(data["ref"]),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
-                "Invalid JSON data received while parsing Orc",
+                "Invalid JSON data received while parsing CommitRef",
                 exc_info=ex
             )
             raise
     
     def to_json(self):
         """Serialise this instance as JSON.
         
         Returns:
             Data ready to serialise as JSON.
         """
         return {
-            "adt_type": self.ADT_TYPE
+            "adt_type": self.ADT_TYPE,
+            "ref": str(self.ref)
         }
 
 
 @dataclasses.dataclass(frozen=True)
-class CSV(FileFormat):
-    """Comma separated value format.
+class BranchRef(Ref):
+    """A reference to a branch.
     
     Args:
-        includeHeader (bool): A data field.
+        ref (str): A data field.
     """
     
-    ADT_TYPE: typing.ClassVar[str] = "csv"
+    ADT_TYPE: typing.ClassVar[str] = "branch"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
-    includeHeader: bool
+    ref: str
     
     @classmethod
     def json_schema(cls):
-        """Return the JSON schema for CSV data.
+        """Return the JSON schema for BranchRef data.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         return {
             "type": "object",
             "properties": {
                 "adt_type": {
                     "type": "string",
                     "enum": [cls.ADT_TYPE]
                 },
-                "includeHeader": {
-                    "type": "boolean"
+                "ref": {
+                    "type": "string"
                 }
             },
             "required": [
                 "adt_type",
-                "includeHeader",
+                "ref",
             ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
-        """Validate and parse JSON data into an instance of CSV.
+        """Validate and parse JSON data into an instance of BranchRef.
         
         Args:
             data (dict): JSON data to validate and parse.
         
         Returns:
-            An instance of CSV.
+            An instance of BranchRef.
         
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
-            return CSV(
-                includeHeader=bool(data["includeHeader"]),
+            return BranchRef(
+                ref=str(data["ref"]),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
-                "Invalid JSON data received while parsing CSV",
+                "Invalid JSON data received while parsing BranchRef",
                 exc_info=ex
             )
             raise
     
     def to_json(self):
         """Serialise this instance as JSON.
         
         Returns:
             Data ready to serialise as JSON.
         """
         return {
             "adt_type": self.ADT_TYPE,
-            "includeHeader": self.includeHeader
+            "ref": str(self.ref)
         }
```

### Comparing `anaml-client-0.8.0/src/anaml_client/models/filter_expression/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/filter_expression/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/generated_features/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/generated_features/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/item/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/reports/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,212 +1,204 @@
-"""Generated implementation of item."""
+"""Generated implementation of reports."""
 
 # WARNING DO NOT EDIT
-# This code was generated from item.mcn
+# This code was generated from reports.mcn
 
 from __future__ import annotations
 
 import abc  # noqa: F401
 import dataclasses  # noqa: F401
 import datetime  # noqa: F401
 import enum  # noqa: F401
+import isodate  # noqa: F401
+import json  # noqa: F401
+import jsonschema  # noqa: F401
 import logging  # noqa: F401
-import uuid  # noqa: F401
 import typing  # noqa: F401
-import jsonschema  # noqa: F401
-
-
-@dataclasses.dataclass(frozen=True)
-class ItemId:
-    """Identifier of item and unique per ItemType.
-    
-    Args:
-        value (int): A data field.
-    """
-    
-    value: int
-    
-    def __str__(self):
-        """Return a str of the wrapped value."""
-        return str(self.value)
-    
-    def __int__(self):
-        """Return an int of the wrapped value."""
-        return int(self.value)
-    
-    @classmethod
-    def json_schema(cls):
-        """Return the JSON schema for ItemId data.
-        
-        Returns:
-            A Python dictionary describing the JSON schema.
-        """
-        return {
-            "type": "integer"
-        }
-    
-    @classmethod
-    def from_json(cls, data: int):
-        """Validate and parse JSON data into an instance of ItemId.
-        
-        Args:
-            data (int): JSON data to validate and parse.
-        
-        Returns:
-            An instance of ItemId.
-        
-        Raises:
-            ValidationError: When schema validation fails.
-            KeyError: When a required field is missing from the JSON.
-        """
-        try:
-            jsonschema.validate(data, cls.json_schema())
-            return ItemId(int(data))
-        except jsonschema.exceptions.ValidationError as ex:
-            logging.debug("Invalid JSON data received while parsing ItemId", exc_info=ex)
-            raise
-    
-    def to_json(self):
-        """Serialise this instance as JSON.
-        
-        Returns:
-            Data ready to serialise as JSON.
-        """
-        return int(self.value)
+import uuid  # noqa: F401
 
 
-class ItemType(enum.Enum):
-    """Type of item."""
-    EntityItemType = "entityitemtype"
-    EntityMappingItemType = "entitymappingitemtype"
-    FeatureItemType = "featureitemtype"
-    FeatureTemplateItemType = "featuretemplateitemtype"
-    FeatureSetItemType = "featuresetitemtype"
-    FeatureStoreItemType = "featurestoreitemtype"
-    TableItemType = "tableitemtype"
+class ActionType(enum.Enum):
+    """Actions to be reported."""
+    Create = "create"
+    Update = "update"
+    Delete = "delete"
     
     @classmethod
     def json_schema(cls):
-        """JSON schema for 'ItemType'.
+        """JSON schema for 'ActionType'.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         return {
             "type": "object",
             "properties": {
                 "adt_type": {
                     "type": "string",
                     "enum": [
-                        "entityitemtype",
-                        "entitymappingitemtype",
-                        "featureitemtype",
-                        "featuretemplateitemtype",
-                        "featuresetitemtype",
-                        "featurestoreitemtype",
-                        "tableitemtype",
+                        "create",
+                        "update",
+                        "delete",
                     ]
                 }
             },
             "required": [
                 "adt_type",
             ]
         }
     
     @classmethod
-    def from_json(cls, data: str):
-        """Validate and parse JSON data into an instance of ItemType.
+    def from_json(cls, data: dict):
+        """Validate and parse JSON data into an instance of ActionType.
         
         Args:
             data (str): JSON data to validate and parse.
         
         Returns:
-            An instance of ItemType.
+            An instance of ActionType.
         
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
-            return ItemType(str(data['adt_type']))
+            return ActionType(str(data['adt_type']))
         except jsonschema.exceptions.ValidationError as ex:
-            logging.debug("Invalid JSON data received while parsing ItemType", exc_info=ex)
+            logging.debug("Invalid JSON data received while parsing ActionType", exc_info=ex)
             raise
     
     def to_json(self):
         """Serialise this instance as JSON.
         
         Returns:
             JSON data ready to be serialised.
         """
         return {'adt_type': self.value}
+    
+    @classmethod
+    def from_json_key(cls, data: str):
+        """Validate and parse a value from a JSON dictionary key.
+        
+        Args:
+            data (str): JSON data to validate and parse.
+        
+        Returns:
+            An instance of ActionType.
+        """
+        return ActionType(str(data))
+    
+    def to_json_key(self):
+        """Serialised this instanse as a JSON string for use as a dictionary key.
+        
+        Returns:
+            A JSON string ready to be used as a key.
+        """
+        return str(self.value)
 
 
 @dataclasses.dataclass(frozen=True)
-class ItemData:
-    """Item data including id and type.
+class ReportAction:
+    """Report of an action performed by a user.
+    
+    Reports are computed asynchronously after the fact.
     
     Args:
-        id (ItemId): A data field.
-        type (ItemType): A data field.
+        timestamp (datetime.datetime): A data field.
+        branch (str): A data field.
+        user (str): A data field.
+        action (ActionType): A data field.
+        object_type (str): A data field.
+        object_id (int): A data field.
     """
     
-    id: ItemId
-    type: ItemType
+    timestamp: datetime.datetime
+    branch: str
+    user: str
+    action: ActionType
+    object_type: str
+    object_id: int
     
     @classmethod
     def json_schema(cls):
-        """Return the JSON schema for ItemData data.
+        """Return the JSON schema for ReportAction data.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         return {
             "type": "object",
             "properties": {
-                "id": ItemId.json_schema(),
-                "type": ItemType.json_schema()
+                "timestamp": {
+                    "type": "string",
+                    "format": "date-time"
+                },
+                "branch": {
+                    "type": "string"
+                },
+                "user": {
+                    "type": "string"
+                },
+                "action": ActionType.json_schema(),
+                "object_type": {
+                    "type": "string"
+                },
+                "object_id": {
+                    "type": "integer"
+                }
             },
             "required": [
-                "id",
-                "type",
+                "timestamp",
+                "branch",
+                "user",
+                "action",
+                "object_type",
+                "object_id",
             ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
-        """Validate and parse JSON data into an instance of ItemData.
+        """Validate and parse JSON data into an instance of ReportAction.
         
         Args:
             data (dict): JSON data to validate and parse.
         
         Returns:
-            An instance of ItemData.
+            An instance of ReportAction.
         
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
-            return ItemData(
-                id=ItemId.from_json(data["id"]),
-                type=ItemType.from_json(data["type"]),
+            return ReportAction(
+                timestamp=isodate.parse_datetime(data["timestamp"]),
+                branch=str(data["branch"]),
+                user=str(data["user"]),
+                action=ActionType.from_json(data["action"]),
+                object_type=str(data["object_type"]),
+                object_id=int(data["object_id"]),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
-                "Invalid JSON data received while parsing ItemData",
+                "Invalid JSON data received while parsing ReportAction",
                 exc_info=ex
             )
             raise
     
     def to_json(self):
         """Serialise this instance as JSON.
         
         Returns:
             Data ready to serialise as JSON.
         """
         return {
-            "id": self.id.to_json(),
-            "type": self.type.to_json()
+            "timestamp": self.timestamp.strftime('%Y-%m-%dT%H:%M:%S.%f%z'),
+            "branch": str(self.branch),
+            "user": str(self.user),
+            "action": self.action.to_json(),
+            "object_type": str(self.object_type),
+            "object_id": int(self.object_id)
         }
```

### Comparing `anaml-client-0.8.0/src/anaml_client/models/job_metrics/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/job_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/jobs/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/label/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/label/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/merge_request/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/merge_request/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/post_aggregate_expression/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/post_aggregate_expression/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/quality_rating/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/roles/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-"""Generated implementation of quality_rating."""
+"""Generated implementation of roles."""
 
 # WARNING DO NOT EDIT
-# This code was generated from quality-rating.mcn
+# This code was generated from roles.mcn
 
 from __future__ import annotations
 
 import abc  # noqa: F401
 import dataclasses  # noqa: F401
 import datetime  # noqa: F401
 import enum  # noqa: F401
@@ -13,67 +13,90 @@
 import json  # noqa: F401
 import jsonschema  # noqa: F401
 import logging  # noqa: F401
 import typing  # noqa: F401
 import uuid  # noqa: F401
 
 
-class QualityRating(enum.Enum):
-    """Data quality ratings."""
-    Tin = "tin"
-    Bronze = "bronze"
-    Silver = "silver"
-    Gold = "gold"
-    Platinum = "platinum"
+class Role(enum.Enum):
+    """Roles/permissions."""
+    Author = "author"
+    """Grants permission to create and manage feature definitions."""
+    AdminBranchPerms = "adminbranchperms"
+    """Grants permission to manage branch permissions."""
+    AdminGroups = "admingroups"
+    """Grants permission to manage user groups."""
+    AdminSystem = "adminsystem"
+    """Grants permission to manage system configuration."""
+    AdminUsers = "adminusers"
+    """Grants permission to manage users."""
+    AdminWebhooks = "adminwebhooks"
+    """Grants permission to manage webhooks."""
+    RunCaching = "runcaching"
+    """Grants permission to run caching jobs."""
+    RunFeatureGen = "runfeaturegen"
+    """Grants permission to run feature generation jobs."""
+    RunMonitoring = "runmonitoring"
+    """Grants permission to run table monitoring jobs."""
+    SuperUser = "superuser"
+    """Grants full access."""
+    ViewReports = "viewreports"
+    """Grants permission to view reports."""
     
     @classmethod
     def json_schema(cls):
-        """JSON schema for 'QualityRating'.
+        """JSON schema for 'Role'.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         return {
             "type": "object",
             "properties": {
                 "adt_type": {
                     "type": "string",
                     "enum": [
-                        "tin",
-                        "bronze",
-                        "silver",
-                        "gold",
-                        "platinum",
+                        "author",
+                        "adminbranchperms",
+                        "admingroups",
+                        "adminsystem",
+                        "adminusers",
+                        "adminwebhooks",
+                        "runcaching",
+                        "runfeaturegen",
+                        "runmonitoring",
+                        "superuser",
+                        "viewreports",
                     ]
                 }
             },
             "required": [
                 "adt_type",
             ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
-        """Validate and parse JSON data into an instance of QualityRating.
+        """Validate and parse JSON data into an instance of Role.
         
         Args:
             data (str): JSON data to validate and parse.
         
         Returns:
-            An instance of QualityRating.
+            An instance of Role.
         
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
-            return QualityRating(str(data['adt_type']))
+            return Role(str(data['adt_type']))
         except jsonschema.exceptions.ValidationError as ex:
-            logging.debug("Invalid JSON data received while parsing QualityRating", exc_info=ex)
+            logging.debug("Invalid JSON data received while parsing Role", exc_info=ex)
             raise
     
     def to_json(self):
         """Serialise this instance as JSON.
         
         Returns:
             JSON data ready to be serialised.
@@ -84,17 +107,17 @@
     def from_json_key(cls, data: str):
         """Validate and parse a value from a JSON dictionary key.
         
         Args:
             data (str): JSON data to validate and parse.
         
         Returns:
-            An instance of QualityRating.
+            An instance of Role.
         """
-        return QualityRating(str(data))
+        return Role(str(data))
     
     def to_json_key(self):
         """Serialised this instanse as a JSON string for use as a dictionary key.
         
         Returns:
             A JSON string ready to be used as a key.
         """
```

### Comparing `anaml-client-0.8.0/src/anaml_client/models/ref/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/secrets_config/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-"""Generated implementation of ref."""
+"""Generated implementation of secrets_config."""
 
 # WARNING DO NOT EDIT
-# This code was generated from ref.mcn
+# This code was generated from secrets-config.mcn
 
 from __future__ import annotations
 
 import abc  # noqa: F401
 import dataclasses  # noqa: F401
 import datetime  # noqa: F401
 import enum  # noqa: F401
@@ -14,29 +14,23 @@
 import jsonschema  # noqa: F401
 import logging  # noqa: F401
 import typing  # noqa: F401
 import uuid  # noqa: F401
 
 
 @dataclasses.dataclass(frozen=True)
-class Ref(abc.ABC):
-    """A reference to a branch or commit.
-    
-    Args:
-        ref (str): A data field.
-    """
+class SecretsConfig(abc.ABC):
+    """Configuration for a secret configuration item."""
     
     ADT_TYPE: typing.ClassVar[str] = ""
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
-    ref: str
-    
     @classmethod
     def json_schema(cls):
-        """JSON schema for variant Ref.
+        """JSON schema for variant SecretsConfig.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         adt_types = [klass.ADT_TYPE for klass in cls.__subclasses__()]
         return {
             "type": "object",
@@ -49,188 +43,271 @@
             "required": [
                 "adt_type",
             ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
-        """Validate and parse JSON data into an instance of Ref.
+        """Validate and parse JSON data into an instance of SecretsConfig.
         
         Args:
             data (dict): JSON data to validate and parse.
         
         Returns:
-            An instance of Ref.
+            An instance of SecretsConfig.
         
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
             adt_type = data.get("adt_type", None)
             for klass in cls.__subclasses__():
                 if klass.ADT_TYPE == adt_type:
                     return klass.from_json(data)
             raise ValueError("Unknown adt_type: '{ty}'".format(ty=adt_type))
         except jsonschema.exceptions.ValidationError as ex:
-            logging.debug("Invalid JSON data received while parsing Ref", exc_info=ex)
+            logging.debug("Invalid JSON data received while parsing SecretsConfig", exc_info=ex)
             raise
     
     @abc.abstractmethod
     def to_json(self):
         """Serialise this instance as JSON.
         
         Returns:
             Data ready to serialise as JSON.
         """
         raise NotImplementedError
 
 
 @dataclasses.dataclass(frozen=True)
-class CommitRef(Ref):
-    """A reference to a specific commit.
+class BasicSecretsConfig(SecretsConfig):
+    """A secret passed directly.
     
     Args:
-        ref (str): A data field.
+        secret (str): A data field.
     """
     
-    ADT_TYPE: typing.ClassVar[str] = "commit"
+    ADT_TYPE: typing.ClassVar[str] = "basic"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
-    ref: str
+    secret: str
     
     @classmethod
     def json_schema(cls):
-        """Return the JSON schema for CommitRef data.
+        """Return the JSON schema for BasicSecretsConfig data.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         return {
             "type": "object",
             "properties": {
                 "adt_type": {
                     "type": "string",
                     "enum": [cls.ADT_TYPE]
                 },
-                "ref": {
+                "secret": {
                     "type": "string"
                 }
             },
             "required": [
                 "adt_type",
-                "ref",
+                "secret",
             ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
-        """Validate and parse JSON data into an instance of CommitRef.
+        """Validate and parse JSON data into an instance of BasicSecretsConfig.
         
         Args:
             data (dict): JSON data to validate and parse.
         
         Returns:
-            An instance of CommitRef.
+            An instance of BasicSecretsConfig.
         
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
-            return CommitRef(
-                ref=str(data["ref"]),
+            return BasicSecretsConfig(
+                secret=str(data["secret"]),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
-                "Invalid JSON data received while parsing CommitRef",
+                "Invalid JSON data received while parsing BasicSecretsConfig",
                 exc_info=ex
             )
             raise
     
     def to_json(self):
         """Serialise this instance as JSON.
         
         Returns:
             Data ready to serialise as JSON.
         """
         return {
             "adt_type": self.ADT_TYPE,
-            "ref": str(self.ref)
+            "secret": str(self.secret)
         }
 
 
 @dataclasses.dataclass(frozen=True)
-class BranchRef(Ref):
-    """A reference to a branch.
+class AWSSMSecretsConfig(SecretsConfig):
+    """A secret stored in AWS Secret Manager.
     
     Args:
-        ref (str): A data field.
+        secretId (str): A data field.
     """
     
-    ADT_TYPE: typing.ClassVar[str] = "branch"
+    ADT_TYPE: typing.ClassVar[str] = "awssm"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
-    ref: str
+    secretId: str
     
     @classmethod
     def json_schema(cls):
-        """Return the JSON schema for BranchRef data.
+        """Return the JSON schema for AWSSMSecretsConfig data.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         return {
             "type": "object",
             "properties": {
                 "adt_type": {
                     "type": "string",
                     "enum": [cls.ADT_TYPE]
                 },
-                "ref": {
+                "secretId": {
+                    "type": "string"
+                }
+            },
+            "required": [
+                "adt_type",
+                "secretId",
+            ]
+        }
+    
+    @classmethod
+    def from_json(cls, data: dict):
+        """Validate and parse JSON data into an instance of AWSSMSecretsConfig.
+        
+        Args:
+            data (dict): JSON data to validate and parse.
+        
+        Returns:
+            An instance of AWSSMSecretsConfig.
+        
+        Raises:
+            ValidationError: When schema validation fails.
+            KeyError: When a required field is missing from the JSON.
+        """
+        try:
+            jsonschema.validate(data, cls.json_schema())
+            return AWSSMSecretsConfig(
+                secretId=str(data["secretId"]),
+            )
+        except jsonschema.exceptions.ValidationError as ex:
+            logging.debug(
+                "Invalid JSON data received while parsing AWSSMSecretsConfig",
+                exc_info=ex
+            )
+            raise
+    
+    def to_json(self):
+        """Serialise this instance as JSON.
+        
+        Returns:
+            Data ready to serialise as JSON.
+        """
+        return {
+            "adt_type": self.ADT_TYPE,
+            "secretId": str(self.secretId)
+        }
+
+
+@dataclasses.dataclass(frozen=True)
+class GCPSMSecretsConfig(SecretsConfig):
+    """A secret stored in GCP Secret Manager.
+    
+    Args:
+        secretProject (str): A data field.
+        secretId (str): A data field.
+    """
+    
+    ADT_TYPE: typing.ClassVar[str] = "gcpsm"
+    adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
+    
+    secretProject: str
+    secretId: str
+    
+    @classmethod
+    def json_schema(cls):
+        """Return the JSON schema for GCPSMSecretsConfig data.
+        
+        Returns:
+            A Python dictionary describing the JSON schema.
+        """
+        return {
+            "type": "object",
+            "properties": {
+                "adt_type": {
+                    "type": "string",
+                    "enum": [cls.ADT_TYPE]
+                },
+                "secretProject": {
+                    "type": "string"
+                },
+                "secretId": {
                     "type": "string"
                 }
             },
             "required": [
                 "adt_type",
-                "ref",
+                "secretProject",
+                "secretId",
             ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
-        """Validate and parse JSON data into an instance of BranchRef.
+        """Validate and parse JSON data into an instance of GCPSMSecretsConfig.
         
         Args:
             data (dict): JSON data to validate and parse.
         
         Returns:
-            An instance of BranchRef.
+            An instance of GCPSMSecretsConfig.
         
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
-            return BranchRef(
-                ref=str(data["ref"]),
+            return GCPSMSecretsConfig(
+                secretProject=str(data["secretProject"]),
+                secretId=str(data["secretId"]),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
-                "Invalid JSON data received while parsing BranchRef",
+                "Invalid JSON data received while parsing GCPSMSecretsConfig",
                 exc_info=ex
             )
             raise
     
     def to_json(self):
         """Serialise this instance as JSON.
         
         Returns:
             Data ready to serialise as JSON.
         """
         return {
             "adt_type": self.ADT_TYPE,
-            "ref": str(self.ref)
+            "secretProject": str(self.secretProject),
+            "secretId": str(self.secretId)
         }
```

### Comparing `anaml-client-0.8.0/src/anaml_client/models/restrictions/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/source_reference/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,321 +1,331 @@
-"""Generated implementation of restrictions."""
+"""Generated implementation of source_reference."""
 
 # WARNING DO NOT EDIT
-# This code was generated from restrictions.mcn
+# This code was generated from source-reference.mcn
 
 from __future__ import annotations
 
 import abc  # noqa: F401
 import dataclasses  # noqa: F401
 import datetime  # noqa: F401
 import enum  # noqa: F401
 import isodate  # noqa: F401
 import json  # noqa: F401
 import jsonschema  # noqa: F401
 import logging  # noqa: F401
 import typing  # noqa: F401
 import uuid  # noqa: F401
 
+from ..source import SourceId
+
 
 @dataclasses.dataclass(frozen=True)
-class AttributeRestriction:
-    """Attribute restriction rule.
+class SourceReference(abc.ABC):
+    """A location to read input in a source data store.
     
     Args:
-        key (str): A data field.
-        values (typing.Optional[typing.List[str]]): A data field.
+        sourceId (SourceId): A data field.
     """
     
-    key: str
-    values: typing.Optional[typing.List[str]]
+    ADT_TYPE: typing.ClassVar[str] = ""
+    adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
+    
+    sourceId: SourceId
     
     @classmethod
     def json_schema(cls):
-        """Return the JSON schema for AttributeRestriction data.
+        """JSON schema for variant SourceReference.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
+        adt_types = [klass.ADT_TYPE for klass in cls.__subclasses__()]
         return {
             "type": "object",
             "properties": {
-                "key": {
-                    "type": "string"
-                },
-                "values": {
-                    "oneOf": [
-                        {"type": "null"},
-                        {"type": "array", "item": {"type": "string"}},
-                    ]
+                "adt_type": {
+                    "type": "string",
+                    "enum": adt_types
                 }
             },
             "required": [
-                "key",
+                "adt_type",
             ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
-        """Validate and parse JSON data into an instance of AttributeRestriction.
+        """Validate and parse JSON data into an instance of SourceReference.
         
         Args:
             data (dict): JSON data to validate and parse.
         
         Returns:
-            An instance of AttributeRestriction.
+            An instance of SourceReference.
         
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
-            return AttributeRestriction(
-                key=str(data["key"]),
-                values=(lambda v: v and [str(v) for v in v])(data.get("values", None)),
-            )
+            adt_type = data.get("adt_type", None)
+            for klass in cls.__subclasses__():
+                if klass.ADT_TYPE == adt_type:
+                    return klass.from_json(data)
+            raise ValueError("Unknown adt_type: '{ty}'".format(ty=adt_type))
         except jsonschema.exceptions.ValidationError as ex:
-            logging.debug(
-                "Invalid JSON data received while parsing AttributeRestriction",
-                exc_info=ex
-            )
+            logging.debug("Invalid JSON data received while parsing SourceReference", exc_info=ex)
             raise
     
+    @abc.abstractmethod
     def to_json(self):
         """Serialise this instance as JSON.
         
         Returns:
             Data ready to serialise as JSON.
         """
-        return {
-            "key": str(self.key),
-            "values": (lambda v: v and [str(v) for v in v])(self.values)
-        }
+        raise NotImplementedError
 
 
 @dataclasses.dataclass(frozen=True)
-class LabelRestriction:
-    """Label restriction rule.
+class FolderSourceReference(SourceReference):
+    """Read input from a folder in the given source.
     
     Args:
-        text (str): A data field.
-        emoji (typing.Optional[str]): A data field.
-        colour (typing.Optional[str]): A data field.
+        sourceId (SourceId): A data field.
+        folder (str): A data field.
     """
     
-    text: str
-    emoji: typing.Optional[str]
-    colour: typing.Optional[str]
+    ADT_TYPE: typing.ClassVar[str] = "folder"
+    adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
+    
+    sourceId: SourceId
+    folder: str
     
     @classmethod
     def json_schema(cls):
-        """Return the JSON schema for LabelRestriction data.
+        """Return the JSON schema for FolderSourceReference data.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         return {
             "type": "object",
             "properties": {
-                "text": {
-                    "type": "string"
+                "adt_type": {
+                    "type": "string",
+                    "enum": [cls.ADT_TYPE]
                 },
-                "emoji": {
-                    "oneOf": [
-                        {"type": "null"},
-                        {"type": "string"},
-                    ]
-                },
-                "colour": {
-                    "oneOf": [
-                        {"type": "null"},
-                        {"type": "string"},
-                    ]
+                "sourceId": SourceId.json_schema(),
+                "folder": {
+                    "type": "string"
                 }
             },
             "required": [
-                "text",
+                "adt_type",
+                "sourceId",
+                "folder",
             ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
-        """Validate and parse JSON data into an instance of LabelRestriction.
+        """Validate and parse JSON data into an instance of FolderSourceReference.
         
         Args:
             data (dict): JSON data to validate and parse.
         
         Returns:
-            An instance of LabelRestriction.
+            An instance of FolderSourceReference.
         
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
-            return LabelRestriction(
-                text=str(data["text"]),
-                emoji=(lambda v: v and str(v))(data.get("emoji", None)),
-                colour=(lambda v: v and str(v))(data.get("colour", None)),
+            return FolderSourceReference(
+                sourceId=SourceId.from_json(data["sourceId"]),
+                folder=str(data["folder"]),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
-                "Invalid JSON data received while parsing LabelRestriction",
+                "Invalid JSON data received while parsing FolderSourceReference",
                 exc_info=ex
             )
             raise
     
     def to_json(self):
         """Serialise this instance as JSON.
         
         Returns:
             Data ready to serialise as JSON.
         """
         return {
-            "text": str(self.text),
-            "emoji": (lambda v: v and str(v))(self.emoji),
-            "colour": (lambda v: v and str(v))(self.colour)
+            "adt_type": self.ADT_TYPE,
+            "sourceId": self.sourceId.to_json(),
+            "folder": str(self.folder)
         }
 
 
 @dataclasses.dataclass(frozen=True)
-class AllowedLabelsResponse:
-    """Policy for labels permitted by the server configuration.
+class TableSourceReference(SourceReference):
+    """Read input from a table in the given source.
     
     Args:
-        allowedLabels (typing.Optional[typing.List[LabelRestriction]]): A data field.
+        sourceId (SourceId): A data field.
+        tableName (str): A data field.
     """
     
-    allowedLabels: typing.Optional[typing.List[LabelRestriction]]
+    ADT_TYPE: typing.ClassVar[str] = "table"
+    adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
+    
+    sourceId: SourceId
+    tableName: str
     
     @classmethod
     def json_schema(cls):
-        """Return the JSON schema for AllowedLabelsResponse data.
+        """Return the JSON schema for TableSourceReference data.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         return {
             "type": "object",
             "properties": {
-                "allowedLabels": {
-                    "oneOf": [
-                        {"type": "null"},
-                        {"type": "array", "item": LabelRestriction.json_schema()},
-                    ]
+                "adt_type": {
+                    "type": "string",
+                    "enum": [cls.ADT_TYPE]
+                },
+                "sourceId": SourceId.json_schema(),
+                "tableName": {
+                    "type": "string"
                 }
             },
-            "required": []
+            "required": [
+                "adt_type",
+                "sourceId",
+                "tableName",
+            ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
-        """Validate and parse JSON data into an instance of AllowedLabelsResponse.
+        """Validate and parse JSON data into an instance of TableSourceReference.
         
         Args:
             data (dict): JSON data to validate and parse.
         
         Returns:
-            An instance of AllowedLabelsResponse.
+            An instance of TableSourceReference.
         
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
-            return AllowedLabelsResponse(
-                allowedLabels=(
-                    lambda v: v and [LabelRestriction.from_json(v) for v in v]
-                )(
-                    data.get("allowedLabels", None)
-                ),
+            return TableSourceReference(
+                sourceId=SourceId.from_json(data["sourceId"]),
+                tableName=str(data["tableName"]),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
-                "Invalid JSON data received while parsing AllowedLabelsResponse",
+                "Invalid JSON data received while parsing TableSourceReference",
                 exc_info=ex
             )
             raise
     
     def to_json(self):
         """Serialise this instance as JSON.
         
         Returns:
             Data ready to serialise as JSON.
         """
         return {
-            "allowedLabels": (lambda v: v and [v.to_json() for v in v])(self.allowedLabels)
+            "adt_type": self.ADT_TYPE,
+            "sourceId": self.sourceId.to_json(),
+            "tableName": str(self.tableName)
         }
 
 
 @dataclasses.dataclass(frozen=True)
-class AllowedAttributesResponse:
-    """Policy for attributes permitted by the server configuration.
+class TopicSourceReference(SourceReference):
+    """Read input from a topic in the given source.
     
     Args:
-        allowedAttributes (typing.Optional[typing.List[AttributeRestriction]]): A data field.
+        sourceId (SourceId): A data field.
+        topic (str): A data field.
     """
     
-    allowedAttributes: typing.Optional[typing.List[AttributeRestriction]]
+    ADT_TYPE: typing.ClassVar[str] = "topic"
+    adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
+    
+    sourceId: SourceId
+    topic: str
     
     @classmethod
     def json_schema(cls):
-        """Return the JSON schema for AllowedAttributesResponse data.
+        """Return the JSON schema for TopicSourceReference data.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         return {
             "type": "object",
             "properties": {
-                "allowedAttributes": {
-                    "oneOf": [
-                        {"type": "null"},
-                        {"type": "array", "item": AttributeRestriction.json_schema()},
-                    ]
+                "adt_type": {
+                    "type": "string",
+                    "enum": [cls.ADT_TYPE]
+                },
+                "sourceId": SourceId.json_schema(),
+                "topic": {
+                    "type": "string"
                 }
             },
-            "required": []
+            "required": [
+                "adt_type",
+                "sourceId",
+                "topic",
+            ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
-        """Validate and parse JSON data into an instance of AllowedAttributesResponse.
+        """Validate and parse JSON data into an instance of TopicSourceReference.
         
         Args:
             data (dict): JSON data to validate and parse.
         
         Returns:
-            An instance of AllowedAttributesResponse.
+            An instance of TopicSourceReference.
         
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
-            return AllowedAttributesResponse(
-                allowedAttributes=(
-                    lambda v: v and [AttributeRestriction.from_json(v) for v in v]
-                )(
-                    data.get("allowedAttributes", None)
-                ),
+            return TopicSourceReference(
+                sourceId=SourceId.from_json(data["sourceId"]),
+                topic=str(data["topic"]),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
-                "Invalid JSON data received while parsing AllowedAttributesResponse",
+                "Invalid JSON data received while parsing TopicSourceReference",
                 exc_info=ex
             )
             raise
     
     def to_json(self):
         """Serialise this instance as JSON.
         
         Returns:
             Data ready to serialise as JSON.
         """
         return {
-            "allowedAttributes": (lambda v: v and [v.to_json() for v in v])(self.allowedAttributes)
+            "adt_type": self.ADT_TYPE,
+            "sourceId": self.sourceId.to_json(),
+            "topic": str(self.topic)
         }
```

### Comparing `anaml-client-0.8.0/src/anaml_client/models/roles/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/select_expression/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-"""Generated implementation of roles."""
+"""Generated implementation of select_expression."""
 
 # WARNING DO NOT EDIT
-# This code was generated from roles.mcn
+# This code was generated from select-expression.mcn
 
 from __future__ import annotations
 
 import abc  # noqa: F401
 import dataclasses  # noqa: F401
 import datetime  # noqa: F401
 import enum  # noqa: F401
@@ -14,68 +14,70 @@
 import jsonschema  # noqa: F401
 import logging  # noqa: F401
 import typing  # noqa: F401
 import uuid  # noqa: F401
 
 
 @dataclasses.dataclass(frozen=True)
-class Role:
-    """Unique name of a role.
+class SelectExpression:
+    """SQL expression for select clause.
     
     Args:
-        value (str): A data field.
+        sql (str): A data field.
     """
     
-    value: str
-    
-    def __str__(self):
-        """Return a str of the wrapped value."""
-        return str(self.value)
+    sql: str
     
     @classmethod
     def json_schema(cls):
-        """Return the JSON schema for Role data.
+        """Return the JSON schema for SelectExpression data.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         return {
-            "type": "string"
+            "type": "object",
+            "properties": {
+                "sql": {
+                    "type": "string"
+                }
+            },
+            "required": [
+                "sql",
+            ]
         }
     
     @classmethod
-    def from_json(cls, data: str):
-        """Validate and parse JSON data into an instance of Role.
+    def from_json(cls, data: dict):
+        """Validate and parse JSON data into an instance of SelectExpression.
         
         Args:
-            data (str): JSON data to validate and parse.
+            data (dict): JSON data to validate and parse.
         
         Returns:
-            An instance of Role.
+            An instance of SelectExpression.
         
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
-            return Role(str(data))
+            return SelectExpression(
+                sql=str(data["sql"]),
+            )
         except jsonschema.exceptions.ValidationError as ex:
-            logging.debug("Invalid JSON data received while parsing Role", exc_info=ex)
+            logging.debug(
+                "Invalid JSON data received while parsing SelectExpression",
+                exc_info=ex
+            )
             raise
     
     def to_json(self):
         """Serialise this instance as JSON.
         
         Returns:
             Data ready to serialise as JSON.
         """
-        return str(self.value)
-    
-    @classmethod
-    def from_json_key(cls, data: str):
-        """Parse a JSON string such as a dictionary key."""
-        return Role(str(data))
-    
-    def to_json_key(self):
-        """Serialise as a JSON string suitable for use as a dictionary key."""
-        return str(self.value)
+        return {
+            "sql": str(self.sql)
+        }
```

### Comparing `anaml-client-0.8.0/src/anaml_client/models/schedule/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/source/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/source/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -225,27 +225,25 @@
     
     Args:
         attributes (typing.List[Attribute]): A data field.
         description (str): A data field.
         id (SourceId): A data field.
         labels (typing.List[Label]): A data field.
         name (SourceName): A data field.
-        predecessor (typing.Optional[SourceVersionId]): A data field.
         version (SourceVersionId): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = ""
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     attributes: typing.List[Attribute]
     description: str
     id: SourceId
     labels: typing.List[Label]
     name: SourceName
-    predecessor: typing.Optional[SourceVersionId]
     version: SourceVersionId
     
     @classmethod
     def json_schema(cls):
         """JSON schema for variant Source.
         
         Returns:
@@ -310,30 +308,28 @@
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
         bucket (str): A data field.
         path (str): A data field.
         fileFormat (FileFormat): A data field.
         version (SourceVersionId): A data field.
-        predecessor (typing.Optional[SourceVersionId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "s3"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: SourceId
     name: SourceName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
     bucket: str
     path: str
     fileFormat: FileFormat
     version: SourceVersionId
-    predecessor: typing.Optional[SourceVersionId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for S3Source data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -361,21 +357,15 @@
                 "bucket": {
                     "type": "string"
                 },
                 "path": {
                     "type": "string"
                 },
                 "fileFormat": FileFormat.json_schema(),
-                "version": SourceVersionId.json_schema(),
-                "predecessor": {
-                    "oneOf": [
-                        {"type": "null"},
-                        SourceVersionId.json_schema(),
-                    ]
-                }
+                "version": SourceVersionId.json_schema()
             },
             "required": [
                 "adt_type",
                 "id",
                 "name",
                 "description",
                 "labels",
@@ -409,19 +399,14 @@
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
                 bucket=str(data["bucket"]),
                 path=str(data["path"]),
                 fileFormat=FileFormat.from_json(data["fileFormat"]),
                 version=SourceVersionId.from_json(data["version"]),
-                predecessor=(
-                    lambda v: v and SourceVersionId.from_json(v)
-                )(
-                    data.get("predecessor", None)
-                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing S3Source",
                 exc_info=ex
             )
             raise
@@ -438,16 +423,15 @@
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
             "bucket": str(self.bucket),
             "path": str(self.path),
             "fileFormat": self.fileFormat.to_json(),
-            "version": self.version.to_json(),
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "version": self.version.to_json()
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class S3ASource(Source):
     """An input data source on S3-compatible object storage.
     
@@ -460,15 +444,14 @@
         bucket (str): A data field.
         path (str): A data field.
         fileFormat (FileFormat): A data field.
         endpoint (str): A data field.
         accessKey (str): A data field.
         secretKey (str): A data field.
         version (SourceVersionId): A data field.
-        predecessor (typing.Optional[SourceVersionId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "s3a"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: SourceId
     name: SourceName
@@ -478,15 +461,14 @@
     bucket: str
     path: str
     fileFormat: FileFormat
     endpoint: str
     accessKey: str
     secretKey: str
     version: SourceVersionId
-    predecessor: typing.Optional[SourceVersionId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for S3ASource data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -523,21 +505,15 @@
                 },
                 "accessKey": {
                     "type": "string"
                 },
                 "secretKey": {
                     "type": "string"
                 },
-                "version": SourceVersionId.json_schema(),
-                "predecessor": {
-                    "oneOf": [
-                        {"type": "null"},
-                        SourceVersionId.json_schema(),
-                    ]
-                }
+                "version": SourceVersionId.json_schema()
             },
             "required": [
                 "adt_type",
                 "id",
                 "name",
                 "description",
                 "labels",
@@ -577,19 +553,14 @@
                 bucket=str(data["bucket"]),
                 path=str(data["path"]),
                 fileFormat=FileFormat.from_json(data["fileFormat"]),
                 endpoint=str(data["endpoint"]),
                 accessKey=str(data["accessKey"]),
                 secretKey=str(data["secretKey"]),
                 version=SourceVersionId.from_json(data["version"]),
-                predecessor=(
-                    lambda v: v and SourceVersionId.from_json(v)
-                )(
-                    data.get("predecessor", None)
-                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing S3ASource",
                 exc_info=ex
             )
             raise
@@ -609,16 +580,15 @@
             "attributes": [v.to_json() for v in self.attributes],
             "bucket": str(self.bucket),
             "path": str(self.path),
             "fileFormat": self.fileFormat.to_json(),
             "endpoint": str(self.endpoint),
             "accessKey": str(self.accessKey),
             "secretKey": str(self.secretKey),
-            "version": self.version.to_json(),
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "version": self.version.to_json()
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class JDBCSource(Source):
     """An input data source using JDBC.
     
@@ -628,30 +598,28 @@
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
         url (str): A data field.
         schema (str): A data field.
         credentialsProvider (CredentialsProviderConfig): A data field.
         version (SourceVersionId): A data field.
-        predecessor (typing.Optional[SourceVersionId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "jdbc"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: SourceId
     name: SourceName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
     url: str
     schema: str
     credentialsProvider: CredentialsProviderConfig
     version: SourceVersionId
-    predecessor: typing.Optional[SourceVersionId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for JDBCSource data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -679,21 +647,15 @@
                 "url": {
                     "type": "string"
                 },
                 "schema": {
                     "type": "string"
                 },
                 "credentialsProvider": CredentialsProviderConfig.json_schema(),
-                "version": SourceVersionId.json_schema(),
-                "predecessor": {
-                    "oneOf": [
-                        {"type": "null"},
-                        SourceVersionId.json_schema(),
-                    ]
-                }
+                "version": SourceVersionId.json_schema()
             },
             "required": [
                 "adt_type",
                 "id",
                 "name",
                 "description",
                 "labels",
@@ -727,19 +689,14 @@
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
                 url=str(data["url"]),
                 schema=str(data["schema"]),
                 credentialsProvider=CredentialsProviderConfig.from_json(data["credentialsProvider"]),
                 version=SourceVersionId.from_json(data["version"]),
-                predecessor=(
-                    lambda v: v and SourceVersionId.from_json(v)
-                )(
-                    data.get("predecessor", None)
-                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing JDBCSource",
                 exc_info=ex
             )
             raise
@@ -756,16 +713,15 @@
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
             "url": str(self.url),
             "schema": str(self.schema),
             "credentialsProvider": self.credentialsProvider.to_json(),
-            "version": self.version.to_json(),
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "version": self.version.to_json()
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class HiveSource(Source):
     """An input data source on Hive.
     
@@ -773,28 +729,26 @@
         id (SourceId): A data field.
         name (SourceName): A data field.
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
         database (str): A data field.
         version (SourceVersionId): A data field.
-        predecessor (typing.Optional[SourceVersionId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "hive"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: SourceId
     name: SourceName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
     database: str
     version: SourceVersionId
-    predecessor: typing.Optional[SourceVersionId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for HiveSource data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -818,21 +772,15 @@
                 "attributes": {
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
                 "database": {
                     "type": "string"
                 },
-                "version": SourceVersionId.json_schema(),
-                "predecessor": {
-                    "oneOf": [
-                        {"type": "null"},
-                        SourceVersionId.json_schema(),
-                    ]
-                }
+                "version": SourceVersionId.json_schema()
             },
             "required": [
                 "adt_type",
                 "id",
                 "name",
                 "description",
                 "labels",
@@ -862,19 +810,14 @@
                 id=SourceId.from_json(data["id"]),
                 name=SourceName.from_json(data["name"]),
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
                 database=str(data["database"]),
                 version=SourceVersionId.from_json(data["version"]),
-                predecessor=(
-                    lambda v: v and SourceVersionId.from_json(v)
-                )(
-                    data.get("predecessor", None)
-                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing HiveSource",
                 exc_info=ex
             )
             raise
@@ -889,16 +832,15 @@
             "adt_type": self.ADT_TYPE,
             "id": self.id.to_json(),
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
             "database": str(self.database),
-            "version": self.version.to_json(),
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "version": self.version.to_json()
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class BigQuerySource(Source):
     """An input data source on Google BigQuery.
     
@@ -906,28 +848,26 @@
         id (SourceId): A data field.
         name (SourceName): A data field.
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
         path (str): A data field.
         version (SourceVersionId): A data field.
-        predecessor (typing.Optional[SourceVersionId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "bigquery"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: SourceId
     name: SourceName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
     path: str
     version: SourceVersionId
-    predecessor: typing.Optional[SourceVersionId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for BigQuerySource data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -951,21 +891,15 @@
                 "attributes": {
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
                 "path": {
                     "type": "string"
                 },
-                "version": SourceVersionId.json_schema(),
-                "predecessor": {
-                    "oneOf": [
-                        {"type": "null"},
-                        SourceVersionId.json_schema(),
-                    ]
-                }
+                "version": SourceVersionId.json_schema()
             },
             "required": [
                 "adt_type",
                 "id",
                 "name",
                 "description",
                 "labels",
@@ -995,19 +929,14 @@
                 id=SourceId.from_json(data["id"]),
                 name=SourceName.from_json(data["name"]),
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
                 path=str(data["path"]),
                 version=SourceVersionId.from_json(data["version"]),
-                predecessor=(
-                    lambda v: v and SourceVersionId.from_json(v)
-                )(
-                    data.get("predecessor", None)
-                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing BigQuerySource",
                 exc_info=ex
             )
             raise
@@ -1022,16 +951,15 @@
             "adt_type": self.ADT_TYPE,
             "id": self.id.to_json(),
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
             "path": str(self.path),
-            "version": self.version.to_json(),
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "version": self.version.to_json()
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class GCSSource(Source):
     """An input data source on Google Cloud Storage.
     
@@ -1041,30 +969,28 @@
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
         bucket (str): A data field.
         path (str): A data field.
         fileFormat (FileFormat): A data field.
         version (SourceVersionId): A data field.
-        predecessor (typing.Optional[SourceVersionId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "gcs"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: SourceId
     name: SourceName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
     bucket: str
     path: str
     fileFormat: FileFormat
     version: SourceVersionId
-    predecessor: typing.Optional[SourceVersionId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for GCSSource data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -1092,21 +1018,15 @@
                 "bucket": {
                     "type": "string"
                 },
                 "path": {
                     "type": "string"
                 },
                 "fileFormat": FileFormat.json_schema(),
-                "version": SourceVersionId.json_schema(),
-                "predecessor": {
-                    "oneOf": [
-                        {"type": "null"},
-                        SourceVersionId.json_schema(),
-                    ]
-                }
+                "version": SourceVersionId.json_schema()
             },
             "required": [
                 "adt_type",
                 "id",
                 "name",
                 "description",
                 "labels",
@@ -1140,19 +1060,14 @@
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
                 bucket=str(data["bucket"]),
                 path=str(data["path"]),
                 fileFormat=FileFormat.from_json(data["fileFormat"]),
                 version=SourceVersionId.from_json(data["version"]),
-                predecessor=(
-                    lambda v: v and SourceVersionId.from_json(v)
-                )(
-                    data.get("predecessor", None)
-                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing GCSSource",
                 exc_info=ex
             )
             raise
@@ -1169,16 +1084,15 @@
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
             "bucket": str(self.bucket),
             "path": str(self.path),
             "fileFormat": self.fileFormat.to_json(),
-            "version": self.version.to_json(),
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "version": self.version.to_json()
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class LocalSource(Source):
     """An input data source on the local filesystem.
     
@@ -1187,29 +1101,27 @@
         name (SourceName): A data field.
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
         path (str): A data field.
         fileFormat (FileFormat): A data field.
         version (SourceVersionId): A data field.
-        predecessor (typing.Optional[SourceVersionId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "local"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: SourceId
     name: SourceName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
     path: str
     fileFormat: FileFormat
     version: SourceVersionId
-    predecessor: typing.Optional[SourceVersionId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for LocalSource data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -1234,21 +1146,15 @@
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
                 "path": {
                     "type": "string"
                 },
                 "fileFormat": FileFormat.json_schema(),
-                "version": SourceVersionId.json_schema(),
-                "predecessor": {
-                    "oneOf": [
-                        {"type": "null"},
-                        SourceVersionId.json_schema(),
-                    ]
-                }
+                "version": SourceVersionId.json_schema()
             },
             "required": [
                 "adt_type",
                 "id",
                 "name",
                 "description",
                 "labels",
@@ -1280,19 +1186,14 @@
                 name=SourceName.from_json(data["name"]),
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
                 path=str(data["path"]),
                 fileFormat=FileFormat.from_json(data["fileFormat"]),
                 version=SourceVersionId.from_json(data["version"]),
-                predecessor=(
-                    lambda v: v and SourceVersionId.from_json(v)
-                )(
-                    data.get("predecessor", None)
-                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing LocalSource",
                 exc_info=ex
             )
             raise
@@ -1308,16 +1209,15 @@
             "id": self.id.to_json(),
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
             "path": str(self.path),
             "fileFormat": self.fileFormat.to_json(),
-            "version": self.version.to_json(),
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "version": self.version.to_json()
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class HDFSSource(Source):
     """An input data source on HDFS.
     
@@ -1326,29 +1226,27 @@
         name (SourceName): A data field.
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
         path (str): A data field.
         fileFormat (FileFormat): A data field.
         version (SourceVersionId): A data field.
-        predecessor (typing.Optional[SourceVersionId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "hdfs"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: SourceId
     name: SourceName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
     path: str
     fileFormat: FileFormat
     version: SourceVersionId
-    predecessor: typing.Optional[SourceVersionId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for HDFSSource data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -1373,21 +1271,15 @@
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
                 "path": {
                     "type": "string"
                 },
                 "fileFormat": FileFormat.json_schema(),
-                "version": SourceVersionId.json_schema(),
-                "predecessor": {
-                    "oneOf": [
-                        {"type": "null"},
-                        SourceVersionId.json_schema(),
-                    ]
-                }
+                "version": SourceVersionId.json_schema()
             },
             "required": [
                 "adt_type",
                 "id",
                 "name",
                 "description",
                 "labels",
@@ -1419,19 +1311,14 @@
                 name=SourceName.from_json(data["name"]),
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
                 path=str(data["path"]),
                 fileFormat=FileFormat.from_json(data["fileFormat"]),
                 version=SourceVersionId.from_json(data["version"]),
-                predecessor=(
-                    lambda v: v and SourceVersionId.from_json(v)
-                )(
-                    data.get("predecessor", None)
-                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing HDFSSource",
                 exc_info=ex
             )
             raise
@@ -1447,16 +1334,15 @@
             "id": self.id.to_json(),
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
             "path": str(self.path),
             "fileFormat": self.fileFormat.to_json(),
-            "version": self.version.to_json(),
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "version": self.version.to_json()
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class KafkaSource(Source):
     """An input data source on Kafka.
     
@@ -1466,30 +1352,28 @@
         description (str): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
         bootstrapServers (str): A data field.
         schemaRegistryUrl (str): A data field.
         kafkaPropertiesProviders (typing.List[SensitiveAttribute]): A data field.
         version (SourceVersionId): A data field.
-        predecessor (typing.Optional[SourceVersionId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "kafka"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: SourceId
     name: SourceName
     description: str
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
     bootstrapServers: str
     schemaRegistryUrl: str
     kafkaPropertiesProviders: typing.List[SensitiveAttribute]
     version: SourceVersionId
-    predecessor: typing.Optional[SourceVersionId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for KafkaSource data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -1520,21 +1404,15 @@
                 "schemaRegistryUrl": {
                     "type": "string"
                 },
                 "kafkaPropertiesProviders": {
                     "type": "array",
                     "item": SensitiveAttribute.json_schema()
                 },
-                "version": SourceVersionId.json_schema(),
-                "predecessor": {
-                    "oneOf": [
-                        {"type": "null"},
-                        SourceVersionId.json_schema(),
-                    ]
-                }
+                "version": SourceVersionId.json_schema()
             },
             "required": [
                 "adt_type",
                 "id",
                 "name",
                 "description",
                 "labels",
@@ -1568,19 +1446,14 @@
                 description=str(data["description"]),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
                 bootstrapServers=str(data["bootstrapServers"]),
                 schemaRegistryUrl=str(data["schemaRegistryUrl"]),
                 kafkaPropertiesProviders=[SensitiveAttribute.from_json(v) for v in data["kafkaPropertiesProviders"]],
                 version=SourceVersionId.from_json(data["version"]),
-                predecessor=(
-                    lambda v: v and SourceVersionId.from_json(v)
-                )(
-                    data.get("predecessor", None)
-                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing KafkaSource",
                 exc_info=ex
             )
             raise
@@ -1597,10 +1470,9 @@
             "name": self.name.to_json(),
             "description": str(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
             "bootstrapServers": str(self.bootstrapServers),
             "schemaRegistryUrl": str(self.schemaRegistryUrl),
             "kafkaPropertiesProviders": [v.to_json() for v in self.kafkaPropertiesProviders],
-            "version": self.version.to_json(),
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "version": self.version.to_json()
         }
```

### Comparing `anaml-client-0.8.0/src/anaml_client/models/source_creation_request/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/source_creation_request/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/summary_statistics/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/summary_statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/table/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/table/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import uuid  # noqa: F401
 
 from ..attribute import Attribute
 from ..entity_mapping import EntityMappingId
 from ..event_description import EventDescription
 from ..feature_id import FeatureId
 from ..label import Label
-from ..quality_rating import QualityRating
 from ..source_reference import SourceReference
 
 
 @dataclasses.dataclass(frozen=True)
 class TableId:
     """Unique identifier for a table.
     
@@ -228,27 +227,25 @@
     
     Args:
         attributes (typing.List[Attribute]): A data field.
         description (typing.Optional[str]): A data field.
         id (TableId): A data field.
         labels (typing.List[Label]): A data field.
         name (TableName): A data field.
-        qualityRating (typing.Optional[QualityRating]): A data field.
         version (TableVersionId): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = ""
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     attributes: typing.List[Attribute]
     description: typing.Optional[str]
     id: TableId
     labels: typing.List[Label]
     name: TableName
-    qualityRating: typing.Optional[QualityRating]
     version: TableVersionId
     
     @classmethod
     def json_schema(cls):
         """JSON schema for variant Table.
         
         Returns:
@@ -309,29 +306,27 @@
     
     Args:
         id (TableId): A data field.
         name (TableName): A data field.
         description (typing.Optional[str]): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
-        qualityRating (typing.Optional[QualityRating]): A data field.
         eventDescription (typing.Optional[EventDescription]): A data field.
         source (SourceReference): A data field.
         version (TableVersionId): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "root"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: TableId
     name: TableName
     description: typing.Optional[str]
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
-    qualityRating: typing.Optional[QualityRating]
     eventDescription: typing.Optional[EventDescription]
     source: SourceReference
     version: TableVersionId
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for RootTable data.
@@ -358,20 +353,14 @@
                     "type": "array",
                     "item": Label.json_schema()
                 },
                 "attributes": {
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
-                "qualityRating": {
-                    "oneOf": [
-                        {"type": "null"},
-                        QualityRating.json_schema(),
-                    ]
-                },
                 "eventDescription": {
                     "oneOf": [
                         {"type": "null"},
                         EventDescription.json_schema(),
                     ]
                 },
                 "source": SourceReference.json_schema(),
@@ -406,19 +395,14 @@
             jsonschema.validate(data, cls.json_schema())
             return RootTable(
                 id=TableId.from_json(data["id"]),
                 name=TableName.from_json(data["name"]),
                 description=(lambda v: v and str(v))(data.get("description", None)),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
-                qualityRating=(
-                    lambda v: v and QualityRating.from_json(v)
-                )(
-                    data.get("qualityRating", None)
-                ),
                 eventDescription=(
                     lambda v: v and EventDescription.from_json(v)
                 )(
                     data.get("eventDescription", None)
                 ),
                 source=SourceReference.from_json(data["source"]),
                 version=TableVersionId.from_json(data["version"]),
@@ -439,15 +423,14 @@
         return {
             "adt_type": self.ADT_TYPE,
             "id": self.id.to_json(),
             "name": self.name.to_json(),
             "description": (lambda v: v and str(v))(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
-            "qualityRating": (lambda v: v and v.to_json())(self.qualityRating),
             "eventDescription": (lambda v: v and v.to_json())(self.eventDescription),
             "source": self.source.to_json(),
             "version": self.version.to_json()
         }
 
 
 @dataclasses.dataclass(frozen=True)
@@ -456,30 +439,28 @@
     
     Args:
         id (TableId): A data field.
         name (TableName): A data field.
         description (typing.Optional[str]): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
-        qualityRating (typing.Optional[QualityRating]): A data field.
         eventDescription (typing.Optional[EventDescription]): A data field.
         expression (str): A data field.
         sources (typing.List[TableId]): A data field.
         version (TableVersionId): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "view"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: TableId
     name: TableName
     description: typing.Optional[str]
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
-    qualityRating: typing.Optional[QualityRating]
     eventDescription: typing.Optional[EventDescription]
     expression: str
     sources: typing.List[TableId]
     version: TableVersionId
     
     @classmethod
     def json_schema(cls):
@@ -507,20 +488,14 @@
                     "type": "array",
                     "item": Label.json_schema()
                 },
                 "attributes": {
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
-                "qualityRating": {
-                    "oneOf": [
-                        {"type": "null"},
-                        QualityRating.json_schema(),
-                    ]
-                },
                 "eventDescription": {
                     "oneOf": [
                         {"type": "null"},
                         EventDescription.json_schema(),
                     ]
                 },
                 "expression": {
@@ -562,19 +537,14 @@
             jsonschema.validate(data, cls.json_schema())
             return ViewTable(
                 id=TableId.from_json(data["id"]),
                 name=TableName.from_json(data["name"]),
                 description=(lambda v: v and str(v))(data.get("description", None)),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
-                qualityRating=(
-                    lambda v: v and QualityRating.from_json(v)
-                )(
-                    data.get("qualityRating", None)
-                ),
                 eventDescription=(
                     lambda v: v and EventDescription.from_json(v)
                 )(
                     data.get("eventDescription", None)
                 ),
                 expression=str(data["expression"]),
                 sources=[TableId.from_json(v) for v in data["sources"]],
@@ -596,15 +566,14 @@
         return {
             "adt_type": self.ADT_TYPE,
             "id": self.id.to_json(),
             "name": self.name.to_json(),
             "description": (lambda v: v and str(v))(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
-            "qualityRating": (lambda v: v and v.to_json())(self.qualityRating),
             "eventDescription": (lambda v: v and v.to_json())(self.eventDescription),
             "expression": str(self.expression),
             "sources": [v.to_json() for v in self.sources],
             "version": self.version.to_json()
         }
 
 
@@ -614,29 +583,27 @@
     
     Args:
         id (TableId): A data field.
         name (TableName): A data field.
         description (typing.Optional[str]): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
-        qualityRating (typing.Optional[QualityRating]): A data field.
         entityMapping (EntityMappingId): A data field.
         extraFeatures (typing.List[FeatureId]): A data field.
         version (TableVersionId): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "pivot"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     id: TableId
     name: TableName
     description: typing.Optional[str]
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
-    qualityRating: typing.Optional[QualityRating]
     entityMapping: EntityMappingId
     extraFeatures: typing.List[FeatureId]
     version: TableVersionId
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for PivotTable data.
@@ -663,20 +630,14 @@
                     "type": "array",
                     "item": Label.json_schema()
                 },
                 "attributes": {
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
-                "qualityRating": {
-                    "oneOf": [
-                        {"type": "null"},
-                        QualityRating.json_schema(),
-                    ]
-                },
                 "entityMapping": EntityMappingId.json_schema(),
                 "extraFeatures": {
                     "type": "array",
                     "item": FeatureId.json_schema()
                 },
                 "version": TableVersionId.json_schema()
             },
@@ -710,19 +671,14 @@
             jsonschema.validate(data, cls.json_schema())
             return PivotTable(
                 id=TableId.from_json(data["id"]),
                 name=TableName.from_json(data["name"]),
                 description=(lambda v: v and str(v))(data.get("description", None)),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
-                qualityRating=(
-                    lambda v: v and QualityRating.from_json(v)
-                )(
-                    data.get("qualityRating", None)
-                ),
                 entityMapping=EntityMappingId.from_json(data["entityMapping"]),
                 extraFeatures=[FeatureId.from_json(v) for v in data["extraFeatures"]],
                 version=TableVersionId.from_json(data["version"]),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing PivotTable",
@@ -739,12 +695,11 @@
         return {
             "adt_type": self.ADT_TYPE,
             "id": self.id.to_json(),
             "name": self.name.to_json(),
             "description": (lambda v: v and str(v))(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
-            "qualityRating": (lambda v: v and v.to_json())(self.qualityRating),
             "entityMapping": self.entityMapping.to_json(),
             "extraFeatures": [v.to_json() for v in self.extraFeatures],
             "version": self.version.to_json()
         }
```

### Comparing `anaml-client-0.8.0/src/anaml_client/models/table_creation_request/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/table_creation_request/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,39 +17,36 @@
 import uuid  # noqa: F401
 
 from ..attribute import Attribute
 from ..entity_mapping import EntityMappingId
 from ..event_description import EventDescription
 from ..feature_id import FeatureId
 from ..label import Label
-from ..quality_rating import QualityRating
 from ..source_reference import SourceReference
 from ..table import TableId, TableName
 
 
 @dataclasses.dataclass(frozen=True)
 class TableCreationRequest(abc.ABC):
     """Request to create a new table containing source data.
     
     Args:
         attributes (typing.List[Attribute]): A data field.
         description (typing.Optional[str]): A data field.
         labels (typing.List[Label]): A data field.
         name (TableName): A data field.
-        qualityRating (typing.Optional[QualityRating]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = ""
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     attributes: typing.List[Attribute]
     description: typing.Optional[str]
     labels: typing.List[Label]
     name: TableName
-    qualityRating: typing.Optional[QualityRating]
     
     @classmethod
     def json_schema(cls):
         """JSON schema for variant TableCreationRequest.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -108,27 +105,25 @@
     """Request to create a new physical table.
     
     Args:
         name (TableName): A data field.
         description (typing.Optional[str]): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
-        qualityRating (typing.Optional[QualityRating]): A data field.
         eventDescription (typing.Optional[EventDescription]): A data field.
         source (SourceReference): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "root"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     name: TableName
     description: typing.Optional[str]
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
-    qualityRating: typing.Optional[QualityRating]
     eventDescription: typing.Optional[EventDescription]
     source: SourceReference
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for RootTableCreationRequest data.
         
@@ -153,20 +148,14 @@
                     "type": "array",
                     "item": Label.json_schema()
                 },
                 "attributes": {
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
-                "qualityRating": {
-                    "oneOf": [
-                        {"type": "null"},
-                        QualityRating.json_schema(),
-                    ]
-                },
                 "eventDescription": {
                     "oneOf": [
                         {"type": "null"},
                         EventDescription.json_schema(),
                     ]
                 },
                 "source": SourceReference.json_schema()
@@ -197,19 +186,14 @@
         try:
             jsonschema.validate(data, cls.json_schema())
             return RootTableCreationRequest(
                 name=TableName.from_json(data["name"]),
                 description=(lambda v: v and str(v))(data.get("description", None)),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
-                qualityRating=(
-                    lambda v: v and QualityRating.from_json(v)
-                )(
-                    data.get("qualityRating", None)
-                ),
                 eventDescription=(
                     lambda v: v and EventDescription.from_json(v)
                 )(
                     data.get("eventDescription", None)
                 ),
                 source=SourceReference.from_json(data["source"]),
             )
@@ -228,43 +212,40 @@
         """
         return {
             "adt_type": self.ADT_TYPE,
             "name": self.name.to_json(),
             "description": (lambda v: v and str(v))(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
-            "qualityRating": (lambda v: v and v.to_json())(self.qualityRating),
             "eventDescription": (lambda v: v and v.to_json())(self.eventDescription),
             "source": self.source.to_json()
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class ViewTableCreationRequest(TableCreationRequest):
     """Request to create a new view table.
     
     Args:
         name (TableName): A data field.
         description (typing.Optional[str]): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
-        qualityRating (typing.Optional[QualityRating]): A data field.
         eventDescription (typing.Optional[EventDescription]): A data field.
         expression (str): A data field.
         sources (typing.List[TableId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "view"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     name: TableName
     description: typing.Optional[str]
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
-    qualityRating: typing.Optional[QualityRating]
     eventDescription: typing.Optional[EventDescription]
     expression: str
     sources: typing.List[TableId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for ViewTableCreationRequest data.
@@ -290,20 +271,14 @@
                     "type": "array",
                     "item": Label.json_schema()
                 },
                 "attributes": {
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
-                "qualityRating": {
-                    "oneOf": [
-                        {"type": "null"},
-                        QualityRating.json_schema(),
-                    ]
-                },
                 "eventDescription": {
                     "oneOf": [
                         {"type": "null"},
                         EventDescription.json_schema(),
                     ]
                 },
                 "expression": {
@@ -341,19 +316,14 @@
         try:
             jsonschema.validate(data, cls.json_schema())
             return ViewTableCreationRequest(
                 name=TableName.from_json(data["name"]),
                 description=(lambda v: v and str(v))(data.get("description", None)),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
-                qualityRating=(
-                    lambda v: v and QualityRating.from_json(v)
-                )(
-                    data.get("qualityRating", None)
-                ),
                 eventDescription=(
                     lambda v: v and EventDescription.from_json(v)
                 )(
                     data.get("eventDescription", None)
                 ),
                 expression=str(data["expression"]),
                 sources=[TableId.from_json(v) for v in data["sources"]],
@@ -373,15 +343,14 @@
         """
         return {
             "adt_type": self.ADT_TYPE,
             "name": self.name.to_json(),
             "description": (lambda v: v and str(v))(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
-            "qualityRating": (lambda v: v and v.to_json())(self.qualityRating),
             "eventDescription": (lambda v: v and v.to_json())(self.eventDescription),
             "expression": str(self.expression),
             "sources": [v.to_json() for v in self.sources]
         }
 
 
 @dataclasses.dataclass(frozen=True)
@@ -389,27 +358,25 @@
     """Request to create a new pivot table.
     
     Args:
         name (TableName): A data field.
         description (typing.Optional[str]): A data field.
         labels (typing.List[Label]): A data field.
         attributes (typing.List[Attribute]): A data field.
-        qualityRating (typing.Optional[QualityRating]): A data field.
         entityMapping (EntityMappingId): A data field.
         extraFeatures (typing.List[FeatureId]): A data field.
     """
     
     ADT_TYPE: typing.ClassVar[str] = "pivot"
     adt_type: str = dataclasses.field(init=False, repr=False, default=ADT_TYPE)
     
     name: TableName
     description: typing.Optional[str]
     labels: typing.List[Label]
     attributes: typing.List[Attribute]
-    qualityRating: typing.Optional[QualityRating]
     entityMapping: EntityMappingId
     extraFeatures: typing.List[FeatureId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for PivotTableCreationRequest data.
         
@@ -434,20 +401,14 @@
                     "type": "array",
                     "item": Label.json_schema()
                 },
                 "attributes": {
                     "type": "array",
                     "item": Attribute.json_schema()
                 },
-                "qualityRating": {
-                    "oneOf": [
-                        {"type": "null"},
-                        QualityRating.json_schema(),
-                    ]
-                },
                 "entityMapping": EntityMappingId.json_schema(),
                 "extraFeatures": {
                     "type": "array",
                     "item": FeatureId.json_schema()
                 }
             },
             "required": [
@@ -477,19 +438,14 @@
         try:
             jsonschema.validate(data, cls.json_schema())
             return PivotTableCreationRequest(
                 name=TableName.from_json(data["name"]),
                 description=(lambda v: v and str(v))(data.get("description", None)),
                 labels=[Label.from_json(v) for v in data["labels"]],
                 attributes=[Attribute.from_json(v) for v in data["attributes"]],
-                qualityRating=(
-                    lambda v: v and QualityRating.from_json(v)
-                )(
-                    data.get("qualityRating", None)
-                ),
                 entityMapping=EntityMappingId.from_json(data["entityMapping"]),
                 extraFeatures=[FeatureId.from_json(v) for v in data["extraFeatures"]],
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing PivotTableCreationRequest",
                 exc_info=ex
@@ -504,11 +460,10 @@
         """
         return {
             "adt_type": self.ADT_TYPE,
             "name": self.name.to_json(),
             "description": (lambda v: v and str(v))(self.description),
             "labels": [v.to_json() for v in self.labels],
             "attributes": [v.to_json() for v in self.attributes],
-            "qualityRating": (lambda v: v and v.to_json())(self.qualityRating),
             "entityMapping": self.entityMapping.to_json(),
             "extraFeatures": [v.to_json() for v in self.extraFeatures]
         }
```

### Comparing `anaml-client-0.8.0/src/anaml_client/models/table_preview/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/table_preview/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/models/user/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/user/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import uuid  # noqa: F401
 
 from ..roles import Role
 
 
 @dataclasses.dataclass(frozen=True)
 class UserId:
-    """Unique identifier of a user.
+    """Unique identifier of a user, internal to Anaml.
     
     Args:
         value (int): A data field.
     """
     
     value: int
     
@@ -84,96 +84,96 @@
     
     def to_json_key(self):
         """Serialise as a JSON string suitable for use as a dictionary key."""
         return str(self.value)
 
 
 @dataclasses.dataclass(frozen=True)
-class UserName:
-    """Unique name of a user.
+class UserEmail:
+    """Unique email of a user.
     
     Args:
         value (str): A data field.
     """
     
     value: str
     
     def __str__(self):
         """Return a str of the wrapped value."""
         return str(self.value)
     
     @classmethod
     def json_schema(cls):
-        """Return the JSON schema for UserName data.
+        """Return the JSON schema for UserEmail data.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         return {
             "type": "string"
         }
     
     @classmethod
     def from_json(cls, data: str):
-        """Validate and parse JSON data into an instance of UserName.
+        """Validate and parse JSON data into an instance of UserEmail.
         
         Args:
             data (str): JSON data to validate and parse.
         
         Returns:
-            An instance of UserName.
+            An instance of UserEmail.
         
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
-            return UserName(str(data))
+            return UserEmail(str(data))
         except jsonschema.exceptions.ValidationError as ex:
-            logging.debug("Invalid JSON data received while parsing UserName", exc_info=ex)
+            logging.debug("Invalid JSON data received while parsing UserEmail", exc_info=ex)
             raise
     
     def to_json(self):
         """Serialise this instance as JSON.
         
         Returns:
             Data ready to serialise as JSON.
         """
         return str(self.value)
     
     @classmethod
     def from_json_key(cls, data: str):
         """Parse a JSON string such as a dictionary key."""
-        return UserName(str(data))
+        return UserEmail(str(data))
     
     def to_json_key(self):
         """Serialise as a JSON string suitable for use as a dictionary key."""
         return str(self.value)
 
 
 @dataclasses.dataclass(frozen=True)
 class User:
     """Details of a user account.
     
     Args:
         id (UserId): A data field.
-        name (UserName): A data field.
-        email (typing.Optional[str]): A data field.
+        email (UserEmail): A data field.
+        name (str): A data field.
         givenName (typing.Optional[str]): A data field.
         surname (typing.Optional[str]): A data field.
         lastLogin (typing.Optional[datetime.datetime]): A data field.
         created (typing.Optional[datetime.datetime]): A data field.
         modified (typing.Optional[datetime.datetime]): A data field.
         roles (typing.List[Role]): A data field.
     """
     
     id: UserId
-    name: UserName
-    email: typing.Optional[str]
+    email: UserEmail
+    name: str
     givenName: typing.Optional[str]
     surname: typing.Optional[str]
     lastLogin: typing.Optional[datetime.datetime]
     created: typing.Optional[datetime.datetime]
     modified: typing.Optional[datetime.datetime]
     roles: typing.List[Role]
     
@@ -184,20 +184,17 @@
         Returns:
             A Python dictionary describing the JSON schema.
         """
         return {
             "type": "object",
             "properties": {
                 "id": UserId.json_schema(),
-                "name": UserName.json_schema(),
-                "email": {
-                    "oneOf": [
-                        {"type": "null"},
-                        {"type": "string"},
-                    ]
+                "email": UserEmail.json_schema(),
+                "name": {
+                    "type": "string"
                 },
                 "givenName": {
                     "oneOf": [
                         {"type": "null"},
                         {"type": "string"},
                     ]
                 },
@@ -228,14 +225,15 @@
                 "roles": {
                     "type": "array",
                     "item": Role.json_schema()
                 }
             },
             "required": [
                 "id",
+                "email",
                 "name",
                 "roles",
             ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
@@ -251,16 +249,16 @@
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
             return User(
                 id=UserId.from_json(data["id"]),
-                name=UserName.from_json(data["name"]),
-                email=(lambda v: v and str(v))(data.get("email", None)),
+                email=UserEmail.from_json(data["email"]),
+                name=str(data["name"]),
                 givenName=(lambda v: v and str(v))(data.get("givenName", None)),
                 surname=(lambda v: v and str(v))(data.get("surname", None)),
                 lastLogin=(
                     lambda v: v and isodate.parse_datetime(v)
                 )(
                     data.get("lastLogin", None)
                 ),
@@ -283,67 +281,64 @@
         """Serialise this instance as JSON.
         
         Returns:
             Data ready to serialise as JSON.
         """
         return {
             "id": self.id.to_json(),
-            "name": self.name.to_json(),
-            "email": (lambda v: v and str(v))(self.email),
+            "email": self.email.to_json(),
+            "name": str(self.name),
             "givenName": (lambda v: v and str(v))(self.givenName),
             "surname": (lambda v: v and str(v))(self.surname),
             "lastLogin": (lambda v: v and v.strftime('%Y-%m-%dT%H:%M:%S.%f%z'))(self.lastLogin),
             "created": (lambda v: v and v.strftime('%Y-%m-%dT%H:%M:%S.%f%z'))(self.created),
             "modified": (lambda v: v and v.strftime('%Y-%m-%dT%H:%M:%S.%f%z'))(self.modified),
             "roles": [v.to_json() for v in self.roles]
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class UserCreationRequest:
     """Request to create a new user account.
     
     Args:
-        name (UserName): A data field.
+        email (UserEmail): A data field.
         password (typing.Optional[str]): A data field.
-        email (typing.Optional[str]): A data field.
+        name (str): A data field.
         givenName (typing.Optional[str]): A data field.
         surname (typing.Optional[str]): A data field.
         roles (typing.List[Role]): A data field.
     """
     
-    name: UserName
+    email: UserEmail
     password: typing.Optional[str]
-    email: typing.Optional[str]
+    name: str
     givenName: typing.Optional[str]
     surname: typing.Optional[str]
     roles: typing.List[Role]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for UserCreationRequest data.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         return {
             "type": "object",
             "properties": {
-                "name": UserName.json_schema(),
+                "email": UserEmail.json_schema(),
                 "password": {
                     "oneOf": [
                         {"type": "null"},
                         {"type": "string"},
                     ]
                 },
-                "email": {
-                    "oneOf": [
-                        {"type": "null"},
-                        {"type": "string"},
-                    ]
+                "name": {
+                    "type": "string"
                 },
                 "givenName": {
                     "oneOf": [
                         {"type": "null"},
                         {"type": "string"},
                     ]
                 },
@@ -355,14 +350,15 @@
                 },
                 "roles": {
                     "type": "array",
                     "item": Role.json_schema()
                 }
             },
             "required": [
+                "email",
                 "name",
                 "roles",
             ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
@@ -377,17 +373,17 @@
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
             return UserCreationRequest(
-                name=UserName.from_json(data["name"]),
+                email=UserEmail.from_json(data["email"]),
                 password=(lambda v: v and str(v))(data.get("password", None)),
-                email=(lambda v: v and str(v))(data.get("email", None)),
+                name=str(data["name"]),
                 givenName=(lambda v: v and str(v))(data.get("givenName", None)),
                 surname=(lambda v: v and str(v))(data.get("surname", None)),
                 roles=[Role.from_json(v) for v in data["roles"]],
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing UserCreationRequest",
@@ -398,55 +394,52 @@
     def to_json(self):
         """Serialise this instance as JSON.
         
         Returns:
             Data ready to serialise as JSON.
         """
         return {
-            "name": self.name.to_json(),
+            "email": self.email.to_json(),
             "password": (lambda v: v and str(v))(self.password),
-            "email": (lambda v: v and str(v))(self.email),
+            "name": str(self.name),
             "givenName": (lambda v: v and str(v))(self.givenName),
             "surname": (lambda v: v and str(v))(self.surname),
             "roles": [v.to_json() for v in self.roles]
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class UserUpdateRequest:
     """Request to update a user account.
     
     Args:
-        name (UserName): A data field.
-        email (typing.Optional[str]): A data field.
+        email (UserEmail): A data field.
+        name (str): A data field.
         givenName (typing.Optional[str]): A data field.
         surname (typing.Optional[str]): A data field.
     """
     
-    name: UserName
-    email: typing.Optional[str]
+    email: UserEmail
+    name: str
     givenName: typing.Optional[str]
     surname: typing.Optional[str]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for UserUpdateRequest data.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         return {
             "type": "object",
             "properties": {
-                "name": UserName.json_schema(),
-                "email": {
-                    "oneOf": [
-                        {"type": "null"},
-                        {"type": "string"},
-                    ]
+                "email": UserEmail.json_schema(),
+                "name": {
+                    "type": "string"
                 },
                 "givenName": {
                     "oneOf": [
                         {"type": "null"},
                         {"type": "string"},
                     ]
                 },
@@ -454,14 +447,15 @@
                     "oneOf": [
                         {"type": "null"},
                         {"type": "string"},
                     ]
                 }
             },
             "required": [
+                "email",
                 "name",
             ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
         """Validate and parse JSON data into an instance of UserUpdateRequest.
@@ -475,16 +469,16 @@
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
             return UserUpdateRequest(
-                name=UserName.from_json(data["name"]),
-                email=(lambda v: v and str(v))(data.get("email", None)),
+                email=UserEmail.from_json(data["email"]),
+                name=str(data["name"]),
                 givenName=(lambda v: v and str(v))(data.get("givenName", None)),
                 surname=(lambda v: v and str(v))(data.get("surname", None)),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing UserUpdateRequest",
                 exc_info=ex
@@ -494,55 +488,52 @@
     def to_json(self):
         """Serialise this instance as JSON.
         
         Returns:
             Data ready to serialise as JSON.
         """
         return {
-            "name": self.name.to_json(),
-            "email": (lambda v: v and str(v))(self.email),
+            "email": self.email.to_json(),
+            "name": str(self.name),
             "givenName": (lambda v: v and str(v))(self.givenName),
             "surname": (lambda v: v and str(v))(self.surname)
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class UserUpdateRequestWithRoles:
     """Request to update a user account and roles they are assigned.
     
     Args:
-        name (UserName): A data field.
-        email (typing.Optional[str]): A data field.
+        email (UserEmail): A data field.
+        name (str): A data field.
         givenName (typing.Optional[str]): A data field.
         surname (typing.Optional[str]): A data field.
         roles (typing.List[Role]): A data field.
     """
     
-    name: UserName
-    email: typing.Optional[str]
+    email: UserEmail
+    name: str
     givenName: typing.Optional[str]
     surname: typing.Optional[str]
     roles: typing.List[Role]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for UserUpdateRequestWithRoles data.
         
         Returns:
             A Python dictionary describing the JSON schema.
         """
         return {
             "type": "object",
             "properties": {
-                "name": UserName.json_schema(),
-                "email": {
-                    "oneOf": [
-                        {"type": "null"},
-                        {"type": "string"},
-                    ]
+                "email": UserEmail.json_schema(),
+                "name": {
+                    "type": "string"
                 },
                 "givenName": {
                     "oneOf": [
                         {"type": "null"},
                         {"type": "string"},
                     ]
                 },
@@ -554,14 +545,15 @@
                 },
                 "roles": {
                     "type": "array",
                     "item": Role.json_schema()
                 }
             },
             "required": [
+                "email",
                 "name",
                 "roles",
             ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
@@ -576,16 +568,16 @@
         Raises:
             ValidationError: When schema validation fails.
             KeyError: When a required field is missing from the JSON.
         """
         try:
             jsonschema.validate(data, cls.json_schema())
             return UserUpdateRequestWithRoles(
-                name=UserName.from_json(data["name"]),
-                email=(lambda v: v and str(v))(data.get("email", None)),
+                email=UserEmail.from_json(data["email"]),
+                name=str(data["name"]),
                 givenName=(lambda v: v and str(v))(data.get("givenName", None)),
                 surname=(lambda v: v and str(v))(data.get("surname", None)),
                 roles=[Role.from_json(v) for v in data["roles"]],
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing UserUpdateRequestWithRoles",
@@ -596,13 +588,13 @@
     def to_json(self):
         """Serialise this instance as JSON.
         
         Returns:
             Data ready to serialise as JSON.
         """
         return {
-            "name": self.name.to_json(),
-            "email": (lambda v: v and str(v))(self.email),
+            "email": self.email.to_json(),
+            "name": str(self.name),
             "givenName": (lambda v: v and str(v))(self.givenName),
             "surname": (lambda v: v and str(v))(self.surname),
             "roles": [v.to_json() for v in self.roles]
         }
```

### Comparing `anaml-client-0.8.0/src/anaml_client/models/user_group/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/user_group/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -436,30 +436,32 @@
     """Group of Anaml users.
     
     Args:
         id (UserGroupId): A data field.
         version (UserGroupVersionId): A data field.
         name (UserGroupName): A data field.
         description (str): A data field.
-        members (typing.List[UserId]): A data field.
+        members (typing.List[UserGroupMember]): A data field.
         created (datetime.datetime): A data field.
         modified (datetime.datetime): A data field.
         roles (typing.List[Role]): A data field.
         predecessor (typing.Optional[UserGroupVersionId]): A data field.
+        externalGroupId (typing.Optional[ExternalGroupId]): A data field.
     """
     
     id: UserGroupId
     version: UserGroupVersionId
     name: UserGroupName
     description: str
-    members: typing.List[UserId]
+    members: typing.List[UserGroupMember]
     created: datetime.datetime
     modified: datetime.datetime
     roles: typing.List[Role]
     predecessor: typing.Optional[UserGroupVersionId]
+    externalGroupId: typing.Optional[ExternalGroupId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for UserGroup data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -471,15 +473,15 @@
                 "version": UserGroupVersionId.json_schema(),
                 "name": UserGroupName.json_schema(),
                 "description": {
                     "type": "string"
                 },
                 "members": {
                     "type": "array",
-                    "item": UserId.json_schema()
+                    "item": UserGroupMember.json_schema()
                 },
                 "created": {
                     "type": "string",
                     "format": "date-time"
                 },
                 "modified": {
                     "type": "string",
@@ -490,14 +492,20 @@
                     "item": Role.json_schema()
                 },
                 "predecessor": {
                     "oneOf": [
                         {"type": "null"},
                         UserGroupVersionId.json_schema(),
                     ]
+                },
+                "externalGroupId": {
+                    "oneOf": [
+                        {"type": "null"},
+                        ExternalGroupId.json_schema(),
+                    ]
                 }
             },
             "required": [
                 "id",
                 "version",
                 "name",
                 "description",
@@ -525,23 +533,28 @@
         try:
             jsonschema.validate(data, cls.json_schema())
             return UserGroup(
                 id=UserGroupId.from_json(data["id"]),
                 version=UserGroupVersionId.from_json(data["version"]),
                 name=UserGroupName.from_json(data["name"]),
                 description=str(data["description"]),
-                members=[UserId.from_json(v) for v in data["members"]],
+                members=[UserGroupMember.from_json(v) for v in data["members"]],
                 created=isodate.parse_datetime(data["created"]),
                 modified=isodate.parse_datetime(data["modified"]),
                 roles=[Role.from_json(v) for v in data["roles"]],
                 predecessor=(
                     lambda v: v and UserGroupVersionId.from_json(v)
                 )(
                     data.get("predecessor", None)
                 ),
+                externalGroupId=(
+                    lambda v: v and ExternalGroupId.from_json(v)
+                )(
+                    data.get("externalGroupId", None)
+                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing UserGroup",
                 exc_info=ex
             )
             raise
@@ -557,33 +570,36 @@
             "version": self.version.to_json(),
             "name": self.name.to_json(),
             "description": str(self.description),
             "members": [v.to_json() for v in self.members],
             "created": self.created.strftime('%Y-%m-%dT%H:%M:%S.%f%z'),
             "modified": self.modified.strftime('%Y-%m-%dT%H:%M:%S.%f%z'),
             "roles": [v.to_json() for v in self.roles],
-            "predecessor": (lambda v: v and v.to_json())(self.predecessor)
+            "predecessor": (lambda v: v and v.to_json())(self.predecessor),
+            "externalGroupId": (lambda v: v and v.to_json())(self.externalGroupId)
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class UserGroupCreationRequest:
     """Request to create a new user group.
     
     Args:
         name (UserGroupName): A data field.
         description (str): A data field.
         roles (typing.List[Role]): A data field.
-        members (typing.List[UserId]): A data field.
+        members (typing.List[UserGroupMember]): A data field.
+        externalGroupId (typing.Optional[ExternalGroupId]): A data field.
     """
     
     name: UserGroupName
     description: str
     roles: typing.List[Role]
-    members: typing.List[UserId]
+    members: typing.List[UserGroupMember]
+    externalGroupId: typing.Optional[ExternalGroupId]
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for UserGroupCreationRequest data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -597,15 +613,21 @@
                 },
                 "roles": {
                     "type": "array",
                     "item": Role.json_schema()
                 },
                 "members": {
                     "type": "array",
-                    "item": UserId.json_schema()
+                    "item": UserGroupMember.json_schema()
+                },
+                "externalGroupId": {
+                    "oneOf": [
+                        {"type": "null"},
+                        ExternalGroupId.json_schema(),
+                    ]
                 }
             },
             "required": [
                 "name",
                 "description",
                 "roles",
                 "members",
@@ -628,15 +650,20 @@
         """
         try:
             jsonschema.validate(data, cls.json_schema())
             return UserGroupCreationRequest(
                 name=UserGroupName.from_json(data["name"]),
                 description=str(data["description"]),
                 roles=[Role.from_json(v) for v in data["roles"]],
-                members=[UserId.from_json(v) for v in data["members"]],
+                members=[UserGroupMember.from_json(v) for v in data["members"]],
+                externalGroupId=(
+                    lambda v: v and ExternalGroupId.from_json(v)
+                )(
+                    data.get("externalGroupId", None)
+                ),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing UserGroupCreationRequest",
                 exc_info=ex
             )
             raise
@@ -647,9 +674,10 @@
         Returns:
             Data ready to serialise as JSON.
         """
         return {
             "name": self.name.to_json(),
             "description": str(self.description),
             "roles": [v.to_json() for v in self.roles],
-            "members": [v.to_json() for v in self.members]
+            "members": [v.to_json() for v in self.members],
+            "externalGroupId": (lambda v: v and v.to_json())(self.externalGroupId)
         }
```

### Comparing `anaml-client-0.8.0/src/anaml_client/models/webhook/__init__.py` & `anaml-client-0.9.0/src/anaml_client/models/webhook/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,14 +146,79 @@
     
     def to_json_key(self):
         """Serialise as a JSON string suitable for use as a dictionary key."""
         return str(self.value)
 
 
 @dataclasses.dataclass(frozen=True)
+class WebhookVersionId:
+    """Unique identifier of a specific version of a webhook.
+    
+    Args:
+        value (uuid.UUID): A data field.
+    """
+    
+    value: uuid.UUID
+    
+    def __str__(self):
+        """Return a str of the wrapped value."""
+        return str(self.value)
+    
+    @classmethod
+    def json_schema(cls):
+        """Return the JSON schema for WebhookVersionId data.
+        
+        Returns:
+            A Python dictionary describing the JSON schema.
+        """
+        return {
+            "type": "string",
+            "format": "uuid"
+        }
+    
+    @classmethod
+    def from_json(cls, data: str):
+        """Validate and parse JSON data into an instance of WebhookVersionId.
+        
+        Args:
+            data (uuid.UUID): JSON data to validate and parse.
+        
+        Returns:
+            An instance of WebhookVersionId.
+        
+        Raises:
+            ValidationError: When schema validation fails.
+            KeyError: When a required field is missing from the JSON.
+        """
+        try:
+            jsonschema.validate(data, cls.json_schema())
+            return WebhookVersionId(uuid.UUID(hex=data))
+        except jsonschema.exceptions.ValidationError as ex:
+            logging.debug("Invalid JSON data received while parsing WebhookVersionId", exc_info=ex)
+            raise
+    
+    def to_json(self):
+        """Serialise this instance as JSON.
+        
+        Returns:
+            Data ready to serialise as JSON.
+        """
+        return str(self.value)
+    
+    @classmethod
+    def from_json_key(cls, data: str):
+        """Parse a JSON string such as a dictionary key."""
+        return WebhookVersionId((lambda s: uuid.UUID(hex=s))(data))
+    
+    def to_json_key(self):
+        """Serialise as a JSON string suitable for use as a dictionary key."""
+        return str(self.value)
+
+
+@dataclasses.dataclass(frozen=True)
 class EventConfiguration:
     """Webhook configuration for a specific event type."""
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for EventConfiguration data.
         
@@ -216,26 +281,28 @@
         url (str): A data field.
         mergeRequests (typing.Optional[EventConfiguration]): A data field.
         mergeRequestComments (typing.Optional[EventConfiguration]): A data field.
         commits (typing.Optional[EventConfiguration]): A data field.
         featureStoreRuns (typing.Optional[EventConfiguration]): A data field.
         monitoringRuns (typing.Optional[EventConfiguration]): A data field.
         cachingRuns (typing.Optional[EventConfiguration]): A data field.
+        version (WebhookVersionId): A data field.
     """
     
     id: WebhookId
     name: WebhookName
     description: str
     url: str
     mergeRequests: typing.Optional[EventConfiguration]
     mergeRequestComments: typing.Optional[EventConfiguration]
     commits: typing.Optional[EventConfiguration]
     featureStoreRuns: typing.Optional[EventConfiguration]
     monitoringRuns: typing.Optional[EventConfiguration]
     cachingRuns: typing.Optional[EventConfiguration]
+    version: WebhookVersionId
     
     @classmethod
     def json_schema(cls):
         """Return the JSON schema for Webhook data.
         
         Returns:
             A Python dictionary describing the JSON schema.
@@ -282,21 +349,23 @@
                     ]
                 },
                 "cachingRuns": {
                     "oneOf": [
                         {"type": "null"},
                         EventConfiguration.json_schema(),
                     ]
-                }
+                },
+                "version": WebhookVersionId.json_schema()
             },
             "required": [
                 "id",
                 "name",
                 "description",
                 "url",
+                "version",
             ]
         }
     
     @classmethod
     def from_json(cls, data: dict):
         """Validate and parse JSON data into an instance of Webhook.
         
@@ -343,14 +412,15 @@
                     data.get("monitoringRuns", None)
                 ),
                 cachingRuns=(
                     lambda v: v and EventConfiguration.from_json(v)
                 )(
                     data.get("cachingRuns", None)
                 ),
+                version=WebhookVersionId.from_json(data["version"]),
             )
         except jsonschema.exceptions.ValidationError as ex:
             logging.debug(
                 "Invalid JSON data received while parsing Webhook",
                 exc_info=ex
             )
             raise
@@ -367,15 +437,16 @@
             "description": str(self.description),
             "url": str(self.url),
             "mergeRequests": (lambda v: v and v.to_json())(self.mergeRequests),
             "mergeRequestComments": (lambda v: v and v.to_json())(self.mergeRequestComments),
             "commits": (lambda v: v and v.to_json())(self.commits),
             "featureStoreRuns": (lambda v: v and v.to_json())(self.featureStoreRuns),
             "monitoringRuns": (lambda v: v and v.to_json())(self.monitoringRuns),
-            "cachingRuns": (lambda v: v and v.to_json())(self.cachingRuns)
+            "cachingRuns": (lambda v: v and v.to_json())(self.cachingRuns),
+            "version": self.version.to_json()
         }
 
 
 @dataclasses.dataclass(frozen=True)
 class WebhookCreationRequest:
     """Request to create or update a webhook.
```

### Comparing `anaml-client-0.8.0/src/anaml_client/utils/__init__.py` & `anaml-client-0.9.0/src/anaml_client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/utils/persistent.py` & `anaml-client-0.9.0/src/anaml_client/utils/persistent.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client/utils/serialisation.py` & `anaml-client-0.9.0/src/anaml_client/utils/serialisation.py`

 * *Files identical despite different names*

### Comparing `anaml-client-0.8.0/src/anaml_client.egg-info/PKG-INFO` & `anaml-client-0.9.0/src/anaml_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: anaml-client
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python SDK for Anaml
 Home-page: https://anaml.com
 Author: Simple Machines
 Author-email: hello@simplemachines.com.au
 License: Copyright 2020 Simple Machines Pty Ltd. All Rights Reserved
-Description: 
-        The Anaml Python SDK makes it easy to interact with the [Anaml][1] feature
-        engineering platform from Python. The SDK provides datatypes and methods to
-        interact with the Anaml REST API and to load Anaml feature data into Pandas
-        and/or Spark data frames.
-        
-        [1]: https://www.anaml.com/
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: Other/Proprietary License
 Requires-Python: >=3.7.10
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: plotting
 Provides-Extra: pandas
 Provides-Extra: spark
 Provides-Extra: aws
 Provides-Extra: google
+
+
+The Anaml Python SDK makes it easy to interact with the [Anaml][1] feature
+engineering platform from Python. The SDK provides datatypes and methods to
+interact with the Anaml REST API and to load Anaml feature data into Pandas
+and/or Spark data frames.
+
+[1]: https://www.anaml.com/
+
+
```

### Comparing `anaml-client-0.8.0/src/anaml_client.egg-info/SOURCES.txt` & `anaml-client-0.9.0/src/anaml_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 src/anaml_client/models/cluster/__init__.py
 src/anaml_client/models/cluster_creation_request/__init__.py
 src/anaml_client/models/commit/__init__.py
 src/anaml_client/models/credentials_provider_config/__init__.py
 src/anaml_client/models/destination/__init__.py
 src/anaml_client/models/destination_creation_request/__init__.py
 src/anaml_client/models/destination_reference/__init__.py
-src/anaml_client/models/empty/__init__.py
 src/anaml_client/models/entity/__init__.py
 src/anaml_client/models/entity_creation_request/__init__.py
 src/anaml_client/models/entity_mapping/__init__.py
 src/anaml_client/models/entity_mapping_creation_request/__init__.py
 src/anaml_client/models/event/__init__.py
 src/anaml_client/models/event_description/__init__.py
 src/anaml_client/models/event_window/__init__.py
@@ -40,35 +39,32 @@
 src/anaml_client/models/feature_store_creation_request/__init__.py
 src/anaml_client/models/feature_store_run/__init__.py
 src/anaml_client/models/feature_template/__init__.py
 src/anaml_client/models/feature_template_creation_request/__init__.py
 src/anaml_client/models/file_format/__init__.py
 src/anaml_client/models/filter_expression/__init__.py
 src/anaml_client/models/generated_features/__init__.py
-src/anaml_client/models/item/__init__.py
 src/anaml_client/models/job_metrics/__init__.py
 src/anaml_client/models/jobs/__init__.py
 src/anaml_client/models/label/__init__.py
 src/anaml_client/models/merge_request/__init__.py
 src/anaml_client/models/post_aggregate_expression/__init__.py
-src/anaml_client/models/quality_rating/__init__.py
 src/anaml_client/models/ref/__init__.py
 src/anaml_client/models/reports/__init__.py
 src/anaml_client/models/restrictions/__init__.py
 src/anaml_client/models/roles/__init__.py
 src/anaml_client/models/schedule/__init__.py
 src/anaml_client/models/secrets_config/__init__.py
 src/anaml_client/models/select_expression/__init__.py
 src/anaml_client/models/source/__init__.py
 src/anaml_client/models/source_creation_request/__init__.py
 src/anaml_client/models/source_reference/__init__.py
 src/anaml_client/models/summary_statistics/__init__.py
 src/anaml_client/models/table/__init__.py
 src/anaml_client/models/table_creation_request/__init__.py
 src/anaml_client/models/table_preview/__init__.py
-src/anaml_client/models/task_statistics/__init__.py
 src/anaml_client/models/user/__init__.py
 src/anaml_client/models/user_group/__init__.py
 src/anaml_client/models/webhook/__init__.py
 src/anaml_client/utils/__init__.py
 src/anaml_client/utils/persistent.py
 src/anaml_client/utils/serialisation.py
```

