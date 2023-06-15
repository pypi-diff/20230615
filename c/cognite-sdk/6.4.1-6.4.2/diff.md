# Comparing `tmp/cognite_sdk-6.4.1.tar.gz` & `tmp/cognite_sdk-6.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.4.1.tar", max compression
+gzip compressed data, was "cognite_sdk-6.4.2.tar", max compression
```

## Comparing `cognite_sdk-6.4.1.tar` & `cognite_sdk-6.4.2.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0    11349 2023-06-14 13:13:51.165082 cognite_sdk-6.4.1/LICENSE
--rw-r--r--   0        0        0     3945 2023-06-14 13:13:51.165082 cognite_sdk-6.4.1/README.md
--rw-r--r--   0        0        0      574 2023-06-14 13:13:51.165082 cognite_sdk-6.4.1/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 13:13:51.165082 cognite_sdk-6.4.1/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     6979 2023-06-14 13:13:51.165082 cognite_sdk-6.4.1/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    49083 2023-06-14 13:13:51.165082 cognite_sdk-6.4.1/cognite/client/_api/assets.py
--rw-r--r--   0        0        0     1157 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/data_modeling/__init__.py
--rw-r--r--   0        0        0     7867 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/data_modeling/containers.py
--rw-r--r--   0        0        0     8393 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/data_modeling/data_models.py
--rw-r--r--   0        0        0    24419 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/data_modeling/instances.py
--rw-r--r--   0        0        0     6424 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/data_modeling/spaces.py
--rw-r--r--   0        0        0     7857 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/data_modeling/views.py
--rw-r--r--   0        0        0    11025 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87459 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12424 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    21276 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17192 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41485 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/files.py
--rw-r--r--   0        0        0    45301 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    49823 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9466 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6052 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24648 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22824 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    37975 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7909 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32072 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    27887 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19140 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    21811 2023-06-14 13:13:51.169082 cognite_sdk-6.4.1/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     4983 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4589 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9525 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     1869 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    38099 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/_api_client.py
--rw-r--r--   0        0        0     5391 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      215 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/_constants.py
--rw-r--r--   0        0        0     6937 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/beta.py
--rw-r--r--   0        0        0     4508 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/config.py
--rw-r--r--   0        0        0    19252 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/credentials.py
--rw-r--r--   0        0        0     8794 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    19074 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8753 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34185 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33708 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     3689 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/__init__.py
--rw-r--r--   0        0        0     1224 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/_core.py
--rw-r--r--   0        0        0     1239 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/_validation.py
--rw-r--r--   0        0        0    12373 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/containers.py
--rw-r--r--   0        0        0     7267 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/data_models.py
--rw-r--r--   0        0        0     3739 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/data_types.py
--rw-r--r--   0        0        0     9519 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/filters.py
--rw-r--r--   0        0        0     5911 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/ids.py
--rw-r--r--   0        0        0    28421 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/instances.py
--rw-r--r--   0        0        0     2543 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/spaces.py
--rw-r--r--   0        0        0    14642 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/views.py
--rw-r--r--   0        0        0     6691 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33969 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11015 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14376 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13671 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16695 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16556 2023-06-14 13:13:51.173082 cognite_sdk-6.4.1/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6037 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5885 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4120 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12267 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17675 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16892 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11855 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12090 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    23040 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    12116 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11469 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2382 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2475 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2770 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9383 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/py.typed
--rw-r--r--   0        0        0     9006 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     8165 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9853 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     7684 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4260 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2981 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    24536 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-06-14 13:13:51.177082 cognite_sdk-6.4.1/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2151 2023-06-14 13:13:51.181082 cognite_sdk-6.4.1/pyproject.toml
--rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-06-15 14:53:11.021824 cognite_sdk-6.4.2/LICENSE
+-rw-r--r--   0        0        0     3945 2023-06-15 14:53:11.021824 cognite_sdk-6.4.2/README.md
+-rw-r--r--   0        0        0      574 2023-06-15 14:53:11.021824 cognite_sdk-6.4.2/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 14:53:11.021824 cognite_sdk-6.4.2/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     6979 2023-06-15 14:53:11.021824 cognite_sdk-6.4.2/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    49083 2023-06-15 14:53:11.021824 cognite_sdk-6.4.2/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0     1157 2023-06-15 14:53:11.021824 cognite_sdk-6.4.2/cognite/client/_api/data_modeling/__init__.py
+-rw-r--r--   0        0        0     7867 2023-06-15 14:53:11.021824 cognite_sdk-6.4.2/cognite/client/_api/data_modeling/containers.py
+-rw-r--r--   0        0        0     8393 2023-06-15 14:53:11.021824 cognite_sdk-6.4.2/cognite/client/_api/data_modeling/data_models.py
+-rw-r--r--   0        0        0    24410 2023-06-15 14:53:11.021824 cognite_sdk-6.4.2/cognite/client/_api/data_modeling/instances.py
+-rw-r--r--   0        0        0     6424 2023-06-15 14:53:11.021824 cognite_sdk-6.4.2/cognite/client/_api/data_modeling/spaces.py
+-rw-r--r--   0        0        0     7857 2023-06-15 14:53:11.021824 cognite_sdk-6.4.2/cognite/client/_api/data_modeling/views.py
+-rw-r--r--   0        0        0    11025 2023-06-15 14:53:11.021824 cognite_sdk-6.4.2/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87459 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12424 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    21276 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17192 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41485 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    45301 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    49823 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9466 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6052 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24648 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22824 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    37975 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7909 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32072 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    27887 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19140 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    21811 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     4983 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4589 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9525 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     1869 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    38099 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     5391 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      215 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6937 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/beta.py
+-rw-r--r--   0        0        0     4508 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/config.py
+-rw-r--r--   0        0        0    19252 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    19074 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8753 2023-06-15 14:53:11.025824 cognite_sdk-6.4.2/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34185 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33708 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     3689 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/__init__.py
+-rw-r--r--   0        0        0     1224 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/_core.py
+-rw-r--r--   0        0        0     1239 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/_validation.py
+-rw-r--r--   0        0        0    12373 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/containers.py
+-rw-r--r--   0        0        0     7267 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/data_models.py
+-rw-r--r--   0        0        0     3739 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/data_types.py
+-rw-r--r--   0        0        0     9519 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/filters.py
+-rw-r--r--   0        0        0     5880 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/ids.py
+-rw-r--r--   0        0        0    28421 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/instances.py
+-rw-r--r--   0        0        0     2543 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/spaces.py
+-rw-r--r--   0        0        0    14642 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/views.py
+-rw-r--r--   0        0        0     6691 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33969 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11015 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14376 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13671 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16695 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16556 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6037 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5885 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4120 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12267 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17675 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16892 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11855 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12090 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    23040 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    12116 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11469 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2382 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2475 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2770 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9383 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/py.typed
+-rw-r--r--   0        0        0     9006 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     8165 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9853 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     7684 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4260 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2981 2023-06-15 14:53:11.029824 cognite_sdk-6.4.2/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24536 2023-06-15 14:53:11.033824 cognite_sdk-6.4.2/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-06-15 14:53:11.033824 cognite_sdk-6.4.2/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-06-15 14:53:11.033824 cognite_sdk-6.4.2/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2151 2023-06-15 14:53:11.033824 cognite_sdk-6.4.2/pyproject.toml
+-rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.4.2/PKG-INFO
```

### Comparing `cognite_sdk-6.4.1/LICENSE` & `cognite_sdk-6.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/README.md` & `cognite_sdk-6.4.2/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/__init__.py` & `cognite_sdk-6.4.2/cognite/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/annotations.py` & `cognite_sdk-6.4.2/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/assets.py` & `cognite_sdk-6.4.2/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/data_modeling/__init__.py` & `cognite_sdk-6.4.2/cognite/client/_api/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/data_modeling/containers.py` & `cognite_sdk-6.4.2/cognite/client/_api/data_modeling/containers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/data_modeling/data_models.py` & `cognite_sdk-6.4.2/cognite/client/_api/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/data_modeling/instances.py` & `cognite_sdk-6.4.2/cognite/client/_api/data_modeling/instances.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
 
         Examples:
 
             Delete instances by id:
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
-                >>> res = c.data_modeling.instances.retrieve(('node', 'mySpace', 'myNode'))
+                >>> res = c.data_modeling.instances.retrieve(('mySpace', 'myNode'))
 
             Delete nodes an edger using the built in data class
 
                 >>> from cognite.client import CogniteClient
                 >>> import cognite.client.data_modeling as dm
                 >>> c = CogniteClient()
                 >>> c.data_modeling.instances.retrieve(dm.NodeId("mySpace", "myNode"),
@@ -279,15 +279,15 @@
             edges_seq = edges  # type: ignore[assignment]
 
         identifiers = []
         if nodes_seq:
             node_ids = _load_identifier(nodes_seq, "node")
             identifiers.extend(node_ids._identifiers)
         if edges_seq:
-            edge_ids = _load_identifier(edges_seq, "node")
+            edge_ids = _load_identifier(edges_seq, "edge")
             identifiers.extend(edge_ids._identifiers)
 
         return DataModelingIdentifierSequence(identifiers, is_singleton=False)
 
     def delete(
         self,
         nodes: NodeId | Sequence[NodeId] | tuple[str, str] | Sequence[tuple[str, str]] | None = None,
@@ -304,17 +304,17 @@
 
         Examples:
 
             Delete instances by id:
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
-                >>> c.data_modeling.instances.delete(("node", "myNode", "mySpace"))
+                >>> c.data_modeling.instances.delete(nodes=("myNode", "mySpace"))
 
-            Delete nodes an edger using the built in data class
+            Delete nodes and edges using the built in data class
 
                 >>> from cognite.client import CogniteClient
                 >>> import cognite.client.data_modeling as dm
                 >>> c = CogniteClient()
                 >>> c.data_modeling.instances.delete(dm.NodeId('mySpace', 'myNode'), dm.EdgeId('mySpace', 'myEdge'))
         """
         identifiers = self._load_node_and_edge_ids(nodes, edges)
```

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/data_modeling/spaces.py` & `cognite_sdk-6.4.2/cognite/client/_api/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/data_modeling/views.py` & `cognite_sdk-6.4.2/cognite/client/_api/data_modeling/views.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/data_sets.py` & `cognite_sdk-6.4.2/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.4.2/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/datapoints.py` & `cognite_sdk-6.4.2/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/diagrams.py` & `cognite_sdk-6.4.2/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.4.2/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/events.py` & `cognite_sdk-6.4.2/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.4.2/cognite/client/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/files.py` & `cognite_sdk-6.4.2/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/functions.py` & `cognite_sdk-6.4.2/cognite/client/_api/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/geospatial.py` & `cognite_sdk-6.4.2/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/iam.py` & `cognite_sdk-6.4.2/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/labels.py` & `cognite_sdk-6.4.2/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/raw.py` & `cognite_sdk-6.4.2/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/relationships.py` & `cognite_sdk-6.4.2/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/sequences.py` & `cognite_sdk-6.4.2/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.4.2/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/templates.py` & `cognite_sdk-6.4.2/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/three_d.py` & `cognite_sdk-6.4.2/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/time_series.py` & `cognite_sdk-6.4.2/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.4.2/cognite/client/_api/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.4.2/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.4.2/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.4.2/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.4.2/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api/vision.py` & `cognite_sdk-6.4.2/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_api_client.py` & `cognite_sdk-6.4.2/cognite/client/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_cognite_client.py` & `cognite_sdk-6.4.2/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_http_client.py` & `cognite_sdk-6.4.2/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.4.2/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.4.2/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.4.2/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.4.2/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.4.2/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.4.2/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.4.2/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.4.2/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.4.2/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.4.2/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/config.py` & `cognite_sdk-6.4.2/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/credentials.py` & `cognite_sdk-6.4.2/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/_base.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/assets.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/__init__.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/_core.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/_validation.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/containers.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/containers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/data_models.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/data_types.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/data_types.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/filters.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/filters.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/ids.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/ids.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,28 +132,28 @@
 NodeIdentifier = Union[NodeId, Tuple[str, str, str]]
 EdgeIdentifier = Union[EdgeId, Tuple[str, str, str]]
 
 Id = Union[Tuple[str, str], Tuple[str, str, str], DataModelingId, VersionedDataModelingId, NodeId, EdgeId, InstanceId]
 
 
 def _load_identifier(
-    ids: Id | Sequence[Id], id_type: Literal["container", "view", "data_model", "node", "edge", "all"]
+    ids: Id | Sequence[Id], id_type: Literal["container", "view", "data_model", "node", "edge"]
 ) -> DataModelingIdentifierSequence:
     is_sequence = isinstance(ids, Sequence) and not (isinstance(ids, tuple) and isinstance(ids[0], str))
     is_view_or_data_model = id_type in {"view", "data_model"}
-    is_instance = id_type in {"node", "edge", "all"}
+    is_instance = id_type in {"node", "edge"}
     id_list = cast(Sequence, ids)
     if not is_sequence:
         id_list = [ids]
 
     def create_args(id_: Id) -> tuple[str, str, Optional[str], Optional[Literal["node", "edge"]]]:
         if isinstance(id_, tuple) and is_instance:
-            if len(id_) == 3:
-                return id_[1], id_[2], None, id_type  # type: ignore[misc, return-value]
-            raise ValueError("Instance given as a tuple must have three elements, (instanceType, space, externalId)")
+            if len(id_) == 2:
+                return id_[0], id_[1], None, id_type  # type: ignore[misc, return-value]
+            raise ValueError("Instance given as a tuple must have two elements (space, externalId)")
         if isinstance(id_, tuple):
             return id_[0], id_[1], id_[2] if len(id_) == 3 else None, None  # type: ignore[misc]
         instance_type = None
         if is_instance:
             instance_type = "node" if isinstance(id_, NodeId) else "edge"
         return id_.space, id_.external_id, getattr(id_, "version", None), instance_type  # type: ignore[return-value]
```

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/instances.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/instances.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/spaces.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/data_modeling/views.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/data_modeling/views.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/events.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/files.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/functions.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/iam.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/labels.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/raw.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/shared.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/templates.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.4.2/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/exceptions.py` & `cognite_sdk-6.4.2/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/testing.py` & `cognite_sdk-6.4.2/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/utils/__init__.py` & `cognite_sdk-6.4.2/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.4.2/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.4.2/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/utils/_graph.py` & `cognite_sdk-6.4.2/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/utils/_identifier.py` & `cognite_sdk-6.4.2/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/utils/_logging.py` & `cognite_sdk-6.4.2/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.4.2/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.4.2/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.4.2/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/utils/_text.py` & `cognite_sdk-6.4.2/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/utils/_time.py` & `cognite_sdk-6.4.2/cognite/client/utils/_time.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/utils/_validation.py` & `cognite_sdk-6.4.2/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.4.2/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.1/pyproject.toml` & `cognite_sdk-6.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.4.1"
+version = "6.4.2"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 license = "Apache-2.0"
```

### Comparing `cognite_sdk-6.4.1/PKG-INFO` & `cognite_sdk-6.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.4.1
+Version: 6.4.2
 Summary: Cognite Python SDK
 License: Apache-2.0
 Author: Erlend Vollset
 Author-email: erlend.vollset@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.4.1 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.4.2 Summary: Cognite Python
 SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
 erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
 Extra: all Provides-Extra: functions Provides-Extra: geo Provides-Extra: numpy
```

