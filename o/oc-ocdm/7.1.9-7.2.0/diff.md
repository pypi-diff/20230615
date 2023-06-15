# Comparing `tmp/oc_ocdm-7.1.9.tar.gz` & `tmp/oc_ocdm-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oc_ocdm-7.1.9.tar", max compression
+gzip compressed data, was "oc_ocdm-7.2.0.tar", max compression
```

## Comparing `oc_ocdm-7.1.9.tar` & `oc_ocdm-7.2.0.tar`

### file list

```diff
@@ -1,94 +1,99 @@
--rw-r--r--   0        0        0      795 2022-12-20 14:08:57.539390 oc_ocdm-7.1.9/LICENSE.md
--rw-r--r--   0        0        0      932 2022-12-20 14:08:57.555020 oc_ocdm-7.1.9/oc_ocdm/__init__.py
--rw-r--r--   0        0        0     8012 2023-01-31 16:12:47.420934 oc_ocdm-7.1.9/oc_ocdm/abstract_entity.py
--rw-r--r--   0        0        0     2890 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/abstract_set.py
--rw-r--r--   0        0        0     1082 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/counter_handler/__init__.py
--rw-r--r--   0        0        0     6419 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/counter_handler/counter_handler.py
--rw-r--r--   0        0        0    16145 2023-02-01 15:10:49.023094 oc_ocdm-7.1.9/oc_ocdm/counter_handler/filesystem_counter_handler.py
--rw-r--r--   0        0        0    12543 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/counter_handler/in_memory_counter_handler.py
--rw-r--r--   0        0        0     2647 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/decorators.py
--rw-r--r--   0        0        0      937 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/__init__.py
--rw-r--r--   0        0        0      974 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/__init__.py
--rw-r--r--   0        0        0     1680 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/__init__.py
--rw-r--r--   0        0        0     8436 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/agent_role.py
--rw-r--r--   0        0        0     9064 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/bibliographic_reference.py
--rw-r--r--   0        0        0    48177 2023-01-30 10:39:34.563112 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/bibliographic_resource.py
--rw-r--r--   0        0        0    16277 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/citation.py
--rw-r--r--   0        0        0    21579 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/discourse_element.py
--rw-r--r--   0        0        0     6313 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/pointer_list.py
--rw-r--r--   0        0        0     4907 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/reference_annotation.py
--rw-r--r--   0        0        0    10131 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/reference_pointer.py
--rw-r--r--   0        0        0    10359 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/resource_embodiment.py
--rw-r--r--   0        0        0     8831 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/responsible_agent.py
--rw-r--r--   0        0        0     6582 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic_entity.py
--rw-r--r--   0        0        0    18025 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/graph/entities/identifier.py
--rw-r--r--   0        0        0    15453 2023-01-30 10:39:34.563112 oc_ocdm-7.1.9/oc_ocdm/graph/graph_entity.py
--rw-r--r--   0        0        0    19992 2023-01-31 16:12:50.015484 oc_ocdm-7.1.9/oc_ocdm/graph/graph_set.py
--rw-r--r--   0        0        0      955 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/metadata/__init__.py
--rw-r--r--   0        0        0      959 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/metadata/entities/__init__.py
--rw-r--r--   0        0        0    19262 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/metadata/entities/dataset.py
--rw-r--r--   0        0        0    12483 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/metadata/entities/distribution.py
--rw-r--r--   0        0        0     7586 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/metadata/metadata_entity.py
--rw-r--r--   0        0        0     6549 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/metadata/metadata_set.py
--rw-r--r--   0        0        0      931 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/prov/__init__.py
--rw-r--r--   0        0        0      905 2022-12-20 14:08:57.570646 oc_ocdm-7.1.9/oc_ocdm/prov/entities/__init__.py
--rw-r--r--   0        0        0    13642 2023-01-31 14:34:56.084004 oc_ocdm-7.1.9/oc_ocdm/prov/entities/snapshot_entity.py
--rw-r--r--   0        0        0     3759 2023-01-31 16:12:50.016485 oc_ocdm-7.1.9/oc_ocdm/prov/prov_entity.py
--rw-r--r--   0        0        0    14189 2023-02-12 15:32:09.388098 oc_ocdm-7.1.9/oc_ocdm/prov/prov_set.py
--rw-r--r--   0        0        0    11957 2023-03-03 13:42:56.995864 oc_ocdm-7.1.9/oc_ocdm/reader.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/resources/__init__.py
--rw-r--r--   0        0        0     1361 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/resources/querymap.txt
--rw-r--r--   0        0        0    22001 2023-03-01 17:12:50.977316 oc_ocdm-7.1.9/oc_ocdm/resources/shacle.ttl
--rw-r--r--   0        0        0    12513 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/resources/shexc.txt
--rw-r--r--   0        0        0    12611 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/resources/shexc_closed.txt
--rw-r--r--   0        0        0    16225 2023-01-31 16:12:50.022417 oc_ocdm-7.1.9/oc_ocdm/storer.py
--rw-r--r--   0        0        0     1354 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/support/__init__.py
--rw-r--r--   0        0        0     3543 2023-01-31 16:12:50.024415 oc_ocdm-7.1.9/oc_ocdm/support/query_utils.py
--rw-r--r--   0        0        0     2615 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/support/reporter.py
--rw-r--r--   0        0        0    15017 2023-01-31 16:12:50.025415 oc_ocdm-7.1.9/oc_ocdm/support/support.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/__init__.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/counter_handler/__init__.py
--rw-r--r--   0        0        0     8681 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/counter_handler/test_filesystem_counter_handler.py
--rw-r--r--   0        0        0    11192 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/counter_handler/test_in_memory_counter_handler.py
--rw-r--r--   0        0        0    69632 2023-03-03 14:12:10.094268 oc_ocdm-7.1.9/oc_ocdm/test/coverage/.coverage
--rw-r--r--   0        0        0      109 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/coverage/.coveragerc
--rw-r--r--   0        0        0      925 2023-03-03 14:12:10.096270 oc_ocdm-7.1.9/oc_ocdm/test/coverage/coverage.svg
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/__init__.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/__init__.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/__init__.py
--rw-r--r--   0        0        0     2679 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_agent_role.py
--rw-r--r--   0        0        0     2209 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_reference.py
--rw-r--r--   0        0        0    12671 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_resource.py
--rw-r--r--   0        0        0     6506 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_citation.py
--rw-r--r--   0        0        0     4915 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_discourse_element.py
--rw-r--r--   0        0        0     1908 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_pointer_list.py
--rw-r--r--   0        0        0     1740 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_reference_annotation.py
--rw-r--r--   0        0        0     2501 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_reference_pointer.py
--rw-r--r--   0        0        0     2990 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_resource_embodiment.py
--rw-r--r--   0        0        0     2535 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_responsible_agent.py
--rw-r--r--   0        0        0     2980 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/test_bibliographic_entity.py
--rw-r--r--   0        0        0     7501 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/test_identifier.py
--rw-r--r--   0        0        0      964 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/graph/test_graph_entity.py
--rw-r--r--   0        0        0     6675 2023-01-31 16:12:47.427934 oc_ocdm-7.1.9/oc_ocdm/test/graph/test_graph_set.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/metadata/__init__.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/metadata/entities/__init__.py
--rw-r--r--   0        0        0     4691 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/metadata/entities/test_dataset.py
--rw-r--r--   0        0        0     3601 2022-12-20 14:08:57.586271 oc_ocdm-7.1.9/oc_ocdm/test/metadata/entities/test_distribution.py
--rw-r--r--   0        0        0     2738 2022-12-20 14:08:57.601896 oc_ocdm-7.1.9/oc_ocdm/test/metadata/test_metadata_set.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.1.9/oc_ocdm/test/prov/__init__.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.1.9/oc_ocdm/test/prov/entities/__init__.py
--rw-r--r--   0        0        0     4248 2022-12-20 14:08:57.601896 oc_ocdm-7.1.9/oc_ocdm/test/prov/entities/test_snapshot_entity.py
--rw-r--r--   0        0        0    11157 2023-01-31 16:12:47.428933 oc_ocdm-7.1.9/oc_ocdm/test/prov/test_prov_set.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.1.9/oc_ocdm/test/resources/__init__.py
--rw-r--r--   0        0        0     6627 2023-03-01 17:12:20.402368 oc_ocdm-7.1.9/oc_ocdm/test/resources/data.json
--rw-r--r--   0        0        0     6627 2023-03-01 17:12:20.402368 oc_ocdm-7.1.9/oc_ocdm/test/resources/data_reader.json
--rw-r--r--   0        0        0     6628 2023-03-03 13:05:35.809618 oc_ocdm-7.1.9/oc_ocdm/test/resources/data_reader_invalid.json
--rw-r--r--   0        0        0     2531 2023-03-03 13:43:32.199458 oc_ocdm-7.1.9/oc_ocdm/test/resources/test_shacle.py
--rw-r--r--   0        0        0      841 2022-12-20 14:08:57.601896 oc_ocdm-7.1.9/oc_ocdm/test/storer/__init__.py
--rw-r--r--   0        0        0    11462 2022-12-20 14:08:57.601896 oc_ocdm-7.1.9/oc_ocdm/test/storer/test_storer.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.1.9/oc_ocdm/test/support/__init__.py
--rw-r--r--   0        0        0     5485 2023-01-31 16:12:50.030419 oc_ocdm-7.1.9/oc_ocdm/test/support/test_support.py
--rw-r--r--   0        0        0     1576 2023-03-03 14:12:50.570092 oc_ocdm-7.1.9/pyproject.toml
--rw-r--r--   0        0        0     4373 2022-12-20 14:08:57.539390 oc_ocdm-7.1.9/README.md
--rw-r--r--   0        0        0     5904 1970-01-01 00:00:00.000000 oc_ocdm-7.1.9/setup.py
--rw-r--r--   0        0        0     5694 1970-01-01 00:00:00.000000 oc_ocdm-7.1.9/PKG-INFO
+-rw-r--r--   0        0        0      795 2022-12-20 14:08:57.539390 oc_ocdm-7.2.0/LICENSE.md
+-rw-r--r--   0        0        0      932 2022-12-20 14:08:57.555020 oc_ocdm-7.2.0/oc_ocdm/__init__.py
+-rw-r--r--   0        0        0     8012 2023-01-31 16:12:47.420934 oc_ocdm-7.2.0/oc_ocdm/abstract_entity.py
+-rw-r--r--   0        0        0     2890 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/abstract_set.py
+-rw-r--r--   0        0        0     1082 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/counter_handler/__init__.py
+-rw-r--r--   0        0        0     6419 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/counter_handler/counter_handler.py
+-rw-r--r--   0        0        0    16145 2023-02-01 15:10:49.023094 oc_ocdm-7.2.0/oc_ocdm/counter_handler/filesystem_counter_handler.py
+-rw-r--r--   0        0        0    12543 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/counter_handler/in_memory_counter_handler.py
+-rw-r--r--   0        0        0     3676 2023-06-08 09:32:26.643046 oc_ocdm-7.2.0/oc_ocdm/counter_handler/sqlite_counter_handler.py
+-rw-r--r--   0        0        0     2647 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/decorators.py
+-rw-r--r--   0        0        0      937 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/__init__.py
+-rw-r--r--   0        0        0      974 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/__init__.py
+-rw-r--r--   0        0        0     1680 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/__init__.py
+-rw-r--r--   0        0        0     8436 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/agent_role.py
+-rw-r--r--   0        0        0     9064 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/bibliographic_reference.py
+-rw-r--r--   0        0        0    49262 2023-06-15 09:24:33.053664 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/bibliographic_resource.py
+-rw-r--r--   0        0        0    16277 2023-03-08 10:55:02.484160 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/citation.py
+-rw-r--r--   0        0        0    21579 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/discourse_element.py
+-rw-r--r--   0        0        0     6313 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/pointer_list.py
+-rw-r--r--   0        0        0     4907 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/reference_annotation.py
+-rw-r--r--   0        0        0    10131 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/reference_pointer.py
+-rw-r--r--   0        0        0    10359 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/resource_embodiment.py
+-rw-r--r--   0        0        0     8831 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/responsible_agent.py
+-rw-r--r--   0        0        0     6582 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic_entity.py
+-rw-r--r--   0        0        0    18802 2023-06-15 09:27:55.194188 oc_ocdm-7.2.0/oc_ocdm/graph/entities/identifier.py
+-rw-r--r--   0        0        0    15524 2023-06-15 09:19:46.065312 oc_ocdm-7.2.0/oc_ocdm/graph/graph_entity.py
+-rw-r--r--   0        0        0    19992 2023-03-08 11:57:00.994531 oc_ocdm-7.2.0/oc_ocdm/graph/graph_set.py
+-rw-r--r--   0        0        0      955 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/metadata/__init__.py
+-rw-r--r--   0        0        0      959 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/metadata/entities/__init__.py
+-rw-r--r--   0        0        0    19262 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/metadata/entities/dataset.py
+-rw-r--r--   0        0        0    12483 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/metadata/entities/distribution.py
+-rw-r--r--   0        0        0     7586 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/metadata/metadata_entity.py
+-rw-r--r--   0        0        0     6549 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/metadata/metadata_set.py
+-rw-r--r--   0        0        0      931 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/prov/__init__.py
+-rw-r--r--   0        0        0      905 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/prov/entities/__init__.py
+-rw-r--r--   0        0        0    13642 2023-01-31 14:34:56.084004 oc_ocdm-7.2.0/oc_ocdm/prov/entities/snapshot_entity.py
+-rw-r--r--   0        0        0     3759 2023-03-08 15:28:49.049031 oc_ocdm-7.2.0/oc_ocdm/prov/prov_entity.py
+-rw-r--r--   0        0        0    16537 2023-06-08 09:32:26.643046 oc_ocdm-7.2.0/oc_ocdm/prov/prov_set.py
+-rw-r--r--   0        0        0    11895 2023-06-08 09:32:26.644056 oc_ocdm-7.2.0/oc_ocdm/reader.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/resources/__init__.py
+-rw-r--r--   0        0        0     1361 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/resources/querymap.txt
+-rw-r--r--   0        0        0    22001 2023-03-01 17:12:50.977316 oc_ocdm-7.2.0/oc_ocdm/resources/shacle.ttl
+-rw-r--r--   0        0        0    12513 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/resources/shexc.txt
+-rw-r--r--   0        0        0    12611 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/resources/shexc_closed.txt
+-rw-r--r--   0        0        0    16523 2023-06-08 09:32:26.645057 oc_ocdm-7.2.0/oc_ocdm/storer.py
+-rw-r--r--   0        0        0     1354 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/support/__init__.py
+-rw-r--r--   0        0        0     3539 2023-03-05 18:46:51.846163 oc_ocdm-7.2.0/oc_ocdm/support/query_utils.py
+-rw-r--r--   0        0        0     2615 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/support/reporter.py
+-rw-r--r--   0        0        0    15049 2023-06-15 09:14:53.068272 oc_ocdm-7.2.0/oc_ocdm/support/support.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/__init__.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/counter_handler/__init__.py
+-rw-r--r--   0        0        0     8681 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/counter_handler/test_filesystem_counter_handler.py
+-rw-r--r--   0        0        0    11192 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/counter_handler/test_in_memory_counter_handler.py
+-rw-r--r--   0        0        0    69632 2023-03-05 14:39:21.650226 oc_ocdm-7.2.0/oc_ocdm/test/coverage/.coverage
+-rw-r--r--   0        0        0      109 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/coverage/.coveragerc
+-rw-r--r--   0        0        0      925 2023-03-03 14:13:32.590309 oc_ocdm-7.2.0/oc_ocdm/test/coverage/coverage.svg
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/__init__.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/__init__.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/__init__.py
+-rw-r--r--   0        0        0     2679 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_agent_role.py
+-rw-r--r--   0        0        0     2209 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_reference.py
+-rw-r--r--   0        0        0    12671 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_resource.py
+-rw-r--r--   0        0        0     6887 2023-03-08 14:23:54.735495 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_citation.py
+-rw-r--r--   0        0        0     4915 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_discourse_element.py
+-rw-r--r--   0        0        0     1908 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_pointer_list.py
+-rw-r--r--   0        0        0     1740 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_reference_annotation.py
+-rw-r--r--   0        0        0     2501 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_reference_pointer.py
+-rw-r--r--   0        0        0     2990 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_resource_embodiment.py
+-rw-r--r--   0        0        0     2535 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_responsible_agent.py
+-rw-r--r--   0        0        0     2980 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/test_bibliographic_entity.py
+-rw-r--r--   0        0        0     8109 2023-03-08 11:33:47.672369 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/test_identifier.py
+-rw-r--r--   0        0        0      964 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/test_graph_entity.py
+-rw-r--r--   0        0        0     6675 2023-01-31 16:12:47.427934 oc_ocdm-7.2.0/oc_ocdm/test/graph/test_graph_set.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/metadata/__init__.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/metadata/entities/__init__.py
+-rw-r--r--   0        0        0     4691 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/metadata/entities/test_dataset.py
+-rw-r--r--   0        0        0     3601 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/metadata/entities/test_distribution.py
+-rw-r--r--   0        0        0     2738 2022-12-20 14:08:57.601896 oc_ocdm-7.2.0/oc_ocdm/test/metadata/test_metadata_set.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.2.0/oc_ocdm/test/prov/__init__.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.2.0/oc_ocdm/test/prov/entities/__init__.py
+-rw-r--r--   0        0        0     4248 2022-12-20 14:08:57.601896 oc_ocdm-7.2.0/oc_ocdm/test/prov/entities/test_snapshot_entity.py
+-rw-r--r--   0        0        0    12288 2023-03-08 15:11:17.576967 oc_ocdm-7.2.0/oc_ocdm/test/prov/prov_counter.db
+-rw-r--r--   0        0        0    13027 2023-06-08 09:32:26.647057 oc_ocdm-7.2.0/oc_ocdm/test/prov/test_prov_set.py
+-rw-r--r--   0        0        0        0 2023-03-05 14:27:05.796485 oc_ocdm-7.2.0/oc_ocdm/test/reader/__init__.py
+-rw-r--r--   0        0        0     2542 2023-03-05 17:46:14.507023 oc_ocdm-7.2.0/oc_ocdm/test/reader/br.nt
+-rw-r--r--   0        0        0     1898 2023-03-05 17:47:28.794428 oc_ocdm-7.2.0/oc_ocdm/test/reader/test_reader.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.2.0/oc_ocdm/test/resources/__init__.py
+-rw-r--r--   0        0        0     6627 2023-03-01 17:12:20.402368 oc_ocdm-7.2.0/oc_ocdm/test/resources/data.json
+-rw-r--r--   0        0        0     6627 2023-03-01 17:12:20.402368 oc_ocdm-7.2.0/oc_ocdm/test/resources/data_reader.json
+-rw-r--r--   0        0        0     6628 2023-03-03 13:05:35.809618 oc_ocdm-7.2.0/oc_ocdm/test/resources/data_reader_invalid.json
+-rw-r--r--   0        0        0     2531 2023-03-03 13:43:32.199458 oc_ocdm-7.2.0/oc_ocdm/test/resources/test_shacle.py
+-rw-r--r--   0        0        0      841 2022-12-20 14:08:57.601896 oc_ocdm-7.2.0/oc_ocdm/test/storer/__init__.py
+-rw-r--r--   0        0        0    11519 2023-06-08 09:32:26.648059 oc_ocdm-7.2.0/oc_ocdm/test/storer/test_storer.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.2.0/oc_ocdm/test/support/__init__.py
+-rw-r--r--   0        0        0     5485 2023-01-31 16:12:50.030419 oc_ocdm-7.2.0/oc_ocdm/test/support/test_support.py
+-rw-r--r--   0        0        0     1590 2023-06-15 09:33:17.989306 oc_ocdm-7.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4373 2022-12-20 14:08:57.539390 oc_ocdm-7.2.0/README.md
+-rw-r--r--   0        0        0     5921 1970-01-01 00:00:00.000000 oc_ocdm-7.2.0/setup.py
+-rw-r--r--   0        0        0     5687 1970-01-01 00:00:00.000000 oc_ocdm-7.2.0/PKG-INFO
```

### Comparing `oc_ocdm-7.1.9/LICENSE.md` & `oc_ocdm-7.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/abstract_entity.py` & `oc_ocdm-7.2.0/oc_ocdm/abstract_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/abstract_set.py` & `oc_ocdm-7.2.0/oc_ocdm/abstract_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/counter_handler/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/counter_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/counter_handler/counter_handler.py` & `oc_ocdm-7.2.0/oc_ocdm/counter_handler/counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/counter_handler/filesystem_counter_handler.py` & `oc_ocdm-7.2.0/oc_ocdm/counter_handler/filesystem_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/counter_handler/in_memory_counter_handler.py` & `oc_ocdm-7.2.0/oc_ocdm/counter_handler/in_memory_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/decorators.py` & `oc_ocdm-7.2.0/oc_ocdm/decorators.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/graph/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/graph/entities/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/graph/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/agent_role.py` & `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/agent_role.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/bibliographic_reference.py` & `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/bibliographic_reference.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/bibliographic_resource.py` & `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/bibliographic_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -833,14 +833,29 @@
 
         `The type of the bibliographic resource`
 
         :return: None
         """
         self._create_type(GraphEntity.iri_book)
 
+    def create_editorial(self) -> None:
+        """
+        Setter method corresponding to the ``rdf:type`` RDF predicate.
+        It implicitly sets the object value ``fabio:Editorial``.
+
+        **WARNING: the OCDM specification admits at most two types for an entity.
+        The main type cannot be edited or removed. Any existing secondary type
+        will be overwritten!**
+
+        `The type of the bibliographic resource`
+
+        :return: None
+        """
+        self._create_type(GraphEntity.iri_editorial)
+
     def create_journal_article(self) -> None:
         """
         Setter method corresponding to the ``rdf:type`` RDF predicate.
         It implicitly sets the object value ``fabio:JournalArticle``.
 
         **WARNING: the OCDM specification admits at most two types for an entity.
         The main type cannot be edited or removed. Any existing secondary type
@@ -923,29 +938,44 @@
 
         `The type of the bibliographic resource`
 
         :return: None
         """
         self._create_type(GraphEntity.iri_book)
 
-    def create_newspaper_article(self) -> None:
+    def create_newspaper(self) -> None:
         """
         Setter method corresponding to the ``rdf:type`` RDF predicate.
         It implicitly sets the object value ``fabio:Newspaper``.
 
         **WARNING: the OCDM specification admits at most two types for an entity.
         The main type cannot be edited or removed. Any existing secondary type
         will be overwritten!**
 
         `The type of the bibliographic resource`
 
         :return: None
         """
         self._create_type(GraphEntity.iri_newspaper)
 
+    def create_newspaper_article(self) -> None:
+        """
+        Setter method corresponding to the ``rdf:type`` RDF predicate.
+        It implicitly sets the object value ``fabio:NewspaperArticle``.
+
+        **WARNING: the OCDM specification admits at most two types for an entity.
+        The main type cannot be edited or removed. Any existing secondary type
+        will be overwritten!**
+
+        `The type of the bibliographic resource`
+
+        :return: None
+        """
+        self._create_type(GraphEntity.iri_newspaper_article)
+
     def create_newspaper_editorial(self) -> None:
         """
         Setter method corresponding to the ``rdf:type`` RDF predicate.
         It implicitly sets the object value ``fabio:NewspaperEditorial``.
 
         **WARNING: the OCDM specification admits at most two types for an entity.
         The main type cannot be edited or removed. Any existing secondary type
```

### Comparing `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/citation.py` & `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/citation.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/discourse_element.py` & `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/discourse_element.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/pointer_list.py` & `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/pointer_list.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/reference_annotation.py` & `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/reference_annotation.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/reference_pointer.py` & `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/reference_pointer.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/resource_embodiment.py` & `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/resource_embodiment.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic/responsible_agent.py` & `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/responsible_agent.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/graph/entities/bibliographic_entity.py` & `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/graph/entities/identifier.py` & `oc_ocdm-7.2.0/oc_ocdm/graph/entities/identifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,14 +128,31 @@
         :type string: str
         :raises TypeError: if the parameter is of the wrong type
         :return: None
         """
         self._associate_identifier_with_scheme(string.lower(), GraphEntity.iri_doi)
 
     @accepts_only('literal')
+    def create_jid(self, string: str) -> None:
+        """
+        Setter method corresponding to both the ``literal:hasLiteralValue`` and the
+        ``datacite:usesIdentifierScheme`` RDF predicate.
+        It implicitly sets the object value ``datacite:jid`` for the
+        ``datacite:usesIdentifierScheme`` RDF predicate.
+
+        **WARNING: this is a functional property, hence any existing value will be overwritten!**
+
+        :param string: The value that will be set as the object of the property related to this method
+        :type string: str
+        :raises TypeError: if the parameter is of the wrong type
+        :return: None
+        """
+        self._associate_identifier_with_scheme(string, GraphEntity.iri_jid)
+
+    @accepts_only('literal')
     def create_pmid(self, string: str) -> None:
         """
         Setter method corresponding to both the ``literal:hasLiteralValue`` and the
         ``datacite:usesIdentifierScheme`` RDF predicate.
         It implicitly sets the object value ``datacite:pmid`` for the
         ``datacite:usesIdentifierScheme`` RDF predicate.
```

### Comparing `oc_ocdm-7.1.9/oc_ocdm/graph/graph_entity.py` & `oc_ocdm-7.2.0/oc_ocdm/graph/graph_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,16 +104,16 @@
     iri_journal_article: ClassVar[URIRef] = FABIO.JournalArticle
     iri_journal_editorial: ClassVar[URIRef] = FABIO.JournalEditorial
     iri_journal_issue: ClassVar[URIRef] = FABIO.JournalIssue
     iri_journal_volume: ClassVar[URIRef] = FABIO.JournalVolume
     iri_manifestation: ClassVar[URIRef] = FABIO.Manifestation
     iri_newspaper: ClassVar[URIRef] = FABIO.Newspaper
     iri_newspaper_article: ClassVar[URIRef] = FABIO.NewspaperArticle
-    iri_newspaper_issue: ClassVar[URIRef] = FABIO.NewspaperIssue
     iri_newspaper_editorial: ClassVar[URIRef] = FABIO.NewspaperEditorial
+    iri_newspaper_issue: ClassVar[URIRef] = FABIO.NewspaperIssue
     iri_peer_review: ClassVar[URIRef] = FR.ReviewVersion
     iri_preprint: ClassVar[URIRef] = FABIO.Preprint
     iri_presentation: ClassVar[URIRef] = FABIO.Presentation
     iri_proceedings_paper: ClassVar[URIRef] = FABIO.ProceedingsPaper
     iri_proceedings_series: ClassVar[URIRef] = FABIO.Series
     iri_reference_book: ClassVar[URIRef] = FABIO.ReferenceBook
     iri_reference_entry: ClassVar[URIRef] = FABIO.ReferenceEntry
@@ -145,14 +145,15 @@
     iri_has_body: ClassVar[URIRef] = OA.hasBody
     iri_has_annotation: ClassVar[URIRef] = OCO.hasAnnotation  # inverse of OA.hasTarget
     iri_has_next: ClassVar[URIRef] = OCO.hasNext
     iri_archival_document: ClassVar[URIRef] = FABIO.ArchivalDocument
     iri_viaf: ClassVar[URIRef] = DATACITE.viaf
     iri_crossref: ClassVar[URIRef] = DATACITE.crossref  # TODO: add to datacite!
     iri_datacite: ClassVar[URIRef] = DATACITE.datacite  # TODO: add to datacite!
+    iri_jid: ClassVar[URIRef] = DATACITE.jid # TODO: add to datacite!
     iri_wikidata: ClassVar[URIRef] = DATACITE.wikidata  # TODO: add to datacite!
     iri_wikipedia: ClassVar[URIRef] = DATACITE.wikipedia  # TODO: add to datacite!
     iri_has_edition: ClassVar[URIRef] = PRISM.edition
     iri_relation: ClassVar[URIRef] = DCTERMS.relation
     iri_has_citation_creation_date: ClassVar[URIRef] = CITO.hasCitationCreationDate
     iri_has_citation_time_span: ClassVar[URIRef] = CITO.hasCitationTimeSpan
     iri_digital_manifestation: ClassVar[URIRef] = FABIO.DigitalManifestation
```

### Comparing `oc_ocdm-7.1.9/oc_ocdm/graph/graph_set.py` & `oc_ocdm-7.2.0/oc_ocdm/graph/graph_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/metadata/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/metadata/entities/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/metadata/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/metadata/entities/dataset.py` & `oc_ocdm-7.2.0/oc_ocdm/metadata/entities/dataset.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/metadata/entities/distribution.py` & `oc_ocdm-7.2.0/oc_ocdm/metadata/entities/distribution.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/metadata/metadata_entity.py` & `oc_ocdm-7.2.0/oc_ocdm/metadata/metadata_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/metadata/metadata_set.py` & `oc_ocdm-7.2.0/oc_ocdm/metadata/metadata_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/prov/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/prov/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/prov/entities/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/prov/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/prov/entities/snapshot_entity.py` & `oc_ocdm-7.2.0/oc_ocdm/prov/entities/snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/prov/prov_entity.py` & `oc_ocdm-7.2.0/oc_ocdm/prov/prov_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/prov/prov_set.py` & `oc_ocdm-7.2.0/oc_ocdm/prov/prov_set.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,47 +30,59 @@
 from rdflib import Graph, URIRef
 
 from oc_ocdm.counter_handler.counter_handler import CounterHandler
 from oc_ocdm.counter_handler.filesystem_counter_handler import \
     FilesystemCounterHandler
 from oc_ocdm.counter_handler.in_memory_counter_handler import \
     InMemoryCounterHandler
+from oc_ocdm.counter_handler.sqlite_counter_handler import SqliteCounterHandler
 from oc_ocdm.graph.graph_set import GraphSet
 from oc_ocdm.prov.prov_entity import ProvEntity
 from oc_ocdm.support.support import (get_count, get_prefix, get_short_name,
                                      has_supplier_prefix)
 
 
 class ProvSet(AbstractSet):
     # Labels
     labels: ClassVar[Dict[str, str]] = {
         "se": "snapshot of entity metadata"
     }
 
     def __init__(self, prov_subj_graph_set: GraphSet, base_iri: str, info_dir: str = "",
-                 wanted_label: bool = True) -> None:
+                 wanted_label: bool = True, custom_counters : dict = dict()) -> None:
         super(ProvSet, self).__init__()
         self.prov_g: GraphSet = prov_subj_graph_set
         # The following variable maps a URIRef with the related provenance entity
         self.res_to_entity: Dict[URIRef, ProvEntity] = {}
         self.base_iri: str = base_iri
         self.wanted_label: bool = wanted_label
         self.info_dir = info_dir
-        if self.info_dir is not None and self.info_dir != "":
-            self.counter_handler: CounterHandler = FilesystemCounterHandler(info_dir)
+        short_names = ["an", "ar", "be", "br", "ci", "de", "id", "pl", "ra", "re", "rp"]
+        self.counter_handlers : Dict[str, CounterHandler] = dict()
+        self.custom_counters = custom_counters
+        if info_dir is not None and info_dir != "":
+            for short_name in short_names:
+                if short_name not in custom_counters:
+                    self.counter_handlers[short_name] = FilesystemCounterHandler(info_dir)
+                else:
+                    self.counter_handlers[short_name] = custom_counters[short_name]
         else:
-            self.counter_handler: CounterHandler = InMemoryCounterHandler()
+            for short_name in short_names:
+                if short_name not in custom_counters:
+                    self.counter_handlers[short_name] = InMemoryCounterHandler()
+                else:
+                    self.counter_handlers[short_name] = custom_counters[short_name]        
 
     def get_entity(self, res: URIRef) -> Optional[ProvEntity]:
         if res in self.res_to_entity:
             return self.res_to_entity[res]
 
     def add_se(self, prov_subject: GraphEntity, res: URIRef = None) -> SnapshotEntity:
         if res is not None and get_short_name(res) != "se":
-            raise ValueError(f"Given res: <{res}> is inappropriate for an SnapshotEntity entity.")
+            raise ValueError(f"Given res: <{res}> is inappropriate for a SnapshotEntity entity.")
         if res is not None and res in self.res_to_entity:
             return self.res_to_entity[res]
         g_prov: str = str(prov_subject) + "/prov/"
         cur_g, count, label = self._add_prov(g_prov, "se", prov_subject, res)
         return SnapshotEntity(prov_subject, cur_g, self, res, prov_subject.resp_agent,
                               prov_subject.source, ProvEntity.iri_entity, count, label, "se")
 
@@ -101,15 +113,17 @@
                 merge_description += f" with '{snapshot.prov_subject.res}'"
                 is_first = False
             else:
                 merge_description += f", '{snapshot.prov_subject.res}'"
         merge_description += "."
         return merge_description
 
-    def generate_provenance(self, c_time: float = None) -> None:
+    def generate_provenance(self, c_time: float = None) -> set:
+        modified_entities = set()
+
         if c_time is None:
             cur_time: str = datetime.now(tz=timezone.utc).replace(microsecond=0).isoformat(sep="T")
         else:
             cur_time: str = datetime.fromtimestamp(c_time, tz=timezone.utc).replace(microsecond=0).isoformat(sep="T")
 
         # MERGED ENTITIES
         for cur_subj in self.prov_g.res_to_entity.values():
@@ -119,40 +133,43 @@
 
             # Previous snapshot
             last_snapshot_res: Optional[URIRef] = self._retrieve_last_snapshot(cur_subj.res)
             if last_snapshot_res is None:
                 # CREATION SNAPSHOT
                 cur_snapshot: SnapshotEntity = self._create_snapshot(cur_subj, cur_time)
                 cur_snapshot.has_description(f"The entity '{cur_subj.res}' has been created.")
+                modified_entities.add(cur_subj.res)
             else:
                 update_query: str = get_update_query(cur_subj, entity_type="graph")[0]
                 was_modified: bool = (update_query != "")
                 snapshots_list: List[SnapshotEntity] = self._get_snapshots_from_merge_list(cur_subj)
 
                 if was_modified and len(snapshots_list) <= 0:
                     # MODIFICATION SNAPSHOT
                     last_snapshot: SnapshotEntity = self.add_se(prov_subject=cur_subj, res=last_snapshot_res)
                     last_snapshot.has_invalidation_time(cur_time)
 
                     cur_snapshot: SnapshotEntity = self._create_snapshot(cur_subj, cur_time)
                     cur_snapshot.derives_from(last_snapshot)
                     cur_snapshot.has_update_action(update_query)
                     cur_snapshot.has_description(f"The entity '{cur_subj.res}' has been modified.")
+                    modified_entities.add(cur_subj.res)
                 elif len(snapshots_list) > 0:
                     # MERGE SNAPSHOT
                     last_snapshot: SnapshotEntity = self.add_se(prov_subject=cur_subj, res=last_snapshot_res)
                     last_snapshot.has_invalidation_time(cur_time)
 
                     cur_snapshot: SnapshotEntity = self._create_snapshot(cur_subj, cur_time)
                     cur_snapshot.derives_from(last_snapshot)
                     for snapshot in snapshots_list:
                         cur_snapshot.derives_from(snapshot)
                     if update_query:
                         cur_snapshot.has_update_action(update_query)
                     cur_snapshot.has_description(self._get_merge_description(cur_subj, snapshots_list))
+                    modified_entities.add(cur_subj.res)
 
         # EVERY OTHER ENTITY
         for cur_subj in self.prov_g.res_to_entity.values():
             if cur_subj is None or (cur_subj.was_merged and not cur_subj.to_be_deleted):
                 # Here we must skip every entity which was merged while not being marked as to be deleted,
                 # since we already processed those entities in the previous loop.
                 continue
@@ -162,74 +179,88 @@
                 if cur_subj.to_be_deleted:
                     # We can ignore this entity because it was deleted even before being created.
                     pass
                 else:
                     # CREATION SNAPSHOT
                     cur_snapshot: SnapshotEntity = self._create_snapshot(cur_subj, cur_time)
                     cur_snapshot.has_description(f"The entity '{cur_subj.res}' has been created.")
+                    modified_entities.add(cur_subj.res)
             else:
                 update_query: str = get_update_query(cur_subj, entity_type="graph")[0]
                 was_modified: bool = (update_query != "")
-
                 if cur_subj.to_be_deleted:
                     # DELETION SNAPSHOT
                     last_snapshot: SnapshotEntity = self.add_se(prov_subject=cur_subj, res=last_snapshot_res)
                     last_snapshot.has_invalidation_time(cur_time)
 
                     cur_snapshot: SnapshotEntity = self._create_snapshot(cur_subj, cur_time)
                     cur_snapshot.derives_from(last_snapshot)
                     cur_snapshot.has_invalidation_time(cur_time)
                     cur_snapshot.has_description(f"The entity '{cur_subj.res}' has been deleted.")
                     cur_snapshot.has_update_action(update_query)
+                    modified_entities.add(cur_subj.res)
                 elif was_modified:
                     # MODIFICATION SNAPSHOT
                     last_snapshot: SnapshotEntity = self.add_se(prov_subject=cur_subj, res=last_snapshot_res)
                     last_snapshot.has_invalidation_time(cur_time)
 
                     cur_snapshot: SnapshotEntity = self._create_snapshot(cur_subj, cur_time)
                     cur_snapshot.derives_from(last_snapshot)
                     cur_snapshot.has_description(f"The entity '{cur_subj.res}' has been modified.")
                     cur_snapshot.has_update_action(update_query)
+                    modified_entities.add(cur_subj.res)
+        return modified_entities
     
     def _fix_info_dir(self, prov_subject: URIRef) -> None:
-        if self.info_dir is None or self.info_dir == "":
+        short_name = get_short_name(prov_subject)
+        if not short_name or self.info_dir is None or self.info_dir == "":
+            return
+        if not isinstance(self.counter_handlers[short_name], FilesystemCounterHandler):
             return
         if has_supplier_prefix(prov_subject, self.base_iri):
             supplier_prefix = get_prefix(prov_subject)
             info_dir_folders = os.path.normpath(self.info_dir).split(os.sep)
             info_dir_prefix = [
                 folder for folder in info_dir_folders 
                 if folder.startswith('0') and folder.endswith('0') and folder.isdigit() and len(folder) > 2]
             if info_dir_prefix:
                 info_dir_prefix = info_dir_prefix[-1]
                 if supplier_prefix != info_dir_prefix:
                     new_info_dir = os.sep.join([folder if folder != info_dir_prefix else supplier_prefix for folder in info_dir_folders])
                     self.info_dir = new_info_dir
-                    self.counter_handler: CounterHandler = FilesystemCounterHandler(new_info_dir)
+                    self.counter_handlers[short_name]: CounterHandler = FilesystemCounterHandler(new_info_dir)
 
     def _add_prov(self, graph_url: str, short_name: str, prov_subject: GraphEntity,
                   res: URIRef = None) -> Tuple[Graph, Optional[str], Optional[str]]:
         self._fix_info_dir(prov_subject.res)
         cur_g: Graph = Graph(identifier=graph_url)
         self._set_ns(cur_g)
 
         count: Optional[str] = None
         label: Optional[str] = None
+
         if res is not None:
             try:
                 res_count: int = int(get_count(res))
             except ValueError:
                 res_count: int = -1
-            if res_count > self.counter_handler.read_counter(prov_subject.short_name, "se",
-                                                             int(get_count(prov_subject.res))):
-                self.counter_handler.set_counter(res_count, prov_subject.short_name, "se",
-                                                 int(get_count(prov_subject.res)))
+            if isinstance(self.counter_handlers[prov_subject.short_name], SqliteCounterHandler):
+                cur_count: str = self.counter_handlers[prov_subject.short_name].read_counter(prov_subject)
+            else:
+                cur_count: str = self.counter_handlers[prov_subject.short_name].read_counter(prov_subject.short_name, "se", int(get_count(prov_subject.res)))
+            if res_count > cur_count:
+                if isinstance(self.counter_handlers[prov_subject.short_name], SqliteCounterHandler):
+                    self.counter_handlers[prov_subject.short_name].set_counter(int(get_count(prov_subject.res)), prov_subject)
+                else:
+                    self.counter_handlers[prov_subject.short_name].set_counter(res_count, prov_subject.short_name, "se", int(get_count(prov_subject.res)))
             return cur_g, count, label
-        count = str(self.counter_handler.increment_counter(
-            prov_subject.short_name, "se", int(get_count(prov_subject.res))))
+        if isinstance(self.counter_handlers[prov_subject.short_name], SqliteCounterHandler):
+            count = str(self.counter_handlers[prov_subject.short_name].increment_counter(prov_subject))
+        else:
+            count = str(self.counter_handlers[prov_subject.short_name].increment_counter(prov_subject.short_name, "se", int(get_count(prov_subject.res))))
         if self.wanted_label:
             cur_short_name = prov_subject.short_name
             cur_entity_count = get_count(prov_subject.res)
             cur_entity_prefix = get_prefix(prov_subject.res)
 
             related_to_label = "related to %s %s%s" % (GraphSet.labels[cur_short_name], cur_entity_prefix,
                                                        cur_entity_count)
@@ -244,22 +275,25 @@
     def _set_ns(g: Graph) -> None:
         g.namespace_manager.bind("prov", ProvEntity.PROV)
 
     def _retrieve_last_snapshot(self, prov_subject: URIRef) -> Optional[URIRef]:
         self._fix_info_dir(prov_subject)
         subj_short_name: str = get_short_name(prov_subject)
         subj_count: str = get_count(prov_subject)
-        try:
-            if int(subj_count) <= 0:
-                raise ValueError('prov_subject is not a valid URIRef. Extracted count value should be a positive '
-                                 'non-zero integer number!')
-        except ValueError:
-            raise ValueError('prov_subject is not a valid URIRef. Unable to extract the count value!')
-
-        last_snapshot_count: str = str(self.counter_handler.read_counter(subj_short_name, "se", int(subj_count)))
+        if subj_short_name not in self.custom_counters:
+            try:
+                if int(subj_count) <= 0:
+                    raise ValueError('prov_subject is not a valid URIRef. Extracted count value should be a positive '
+                                    'non-zero integer number!')
+            except ValueError:
+                raise ValueError('prov_subject is not a valid URIRef. Unable to extract the count value!')
+        if isinstance(self.counter_handlers[subj_short_name], SqliteCounterHandler):
+            last_snapshot_count: str = str(self.counter_handlers[subj_short_name].read_counter(prov_subject))
+        else:
+            last_snapshot_count: str = str(self.counter_handlers[subj_short_name].read_counter(subj_short_name, "se", int(subj_count)))
         if int(last_snapshot_count) <= 0:
             return None
         else:
             return URIRef(str(prov_subject) + '/prov/se/' + last_snapshot_count)
 
     def get_se(self) -> Tuple[SnapshotEntity]:
         result: Tuple[SnapshotEntity] = tuple()
```

### Comparing `oc_ocdm-7.1.9/oc_ocdm/reader.py` & `oc_ocdm-7.2.0/oc_ocdm/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,25 +18,22 @@
 import json
 import os
 from typing import TYPE_CHECKING
 from zipfile import ZipFile
 
 import rdflib
 from filelock import FileLock
-from rdflib import RDF, ConjunctiveGraph, Graph, Namespace, URIRef
-from SPARQLWrapper import RDFXML, SPARQLWrapper
+from rdflib import RDF, ConjunctiveGraph, Graph, URIRef
+from SPARQLWrapper import XML, SPARQLWrapper
 
 from oc_ocdm.graph.graph_entity import GraphEntity
 from oc_ocdm.support.reporter import Reporter
 
 if TYPE_CHECKING:
     from typing import Any, Dict, List, Optional, Set
-
-    from rdflib import term
-
     from oc_ocdm.graph.graph_set import GraphSet
 
 from pyshacl import validate
 
 
 class Reader(object):
 
@@ -171,15 +168,15 @@
     def import_entities_from_graph(g_set: GraphSet, graph: Graph, resp_agent: str,
                                    enable_validation: bool = False, closed: bool = False) -> List[GraphEntity]:
         if enable_validation:
             reader = Reader()
             graph = reader.graph_validation(graph, closed)
         imported_entities: List[GraphEntity] = []
         for subject in Reader._extract_subjects(graph):
-            types: List[term] = []
+            types = []
             for o in graph.objects(subject, RDF.type):
                 types.append(o)
             # ReferenceAnnotation
             if GraphEntity.iri_note in types:
                 imported_entities.append(g_set.add_an(resp_agent=resp_agent, res=subject,
                                          preexisting_graph=Reader.get_graph_from_subject(graph, subject)))
             # AgentRole
@@ -227,16 +224,16 @@
     @staticmethod
     def import_entity_from_triplestore(g_set: GraphSet, ts_url: str, res: URIRef, resp_agent: str,
                                        enable_validation: bool = False) -> GraphEntity:
         sparql: SPARQLWrapper = SPARQLWrapper(ts_url)
         query: str = f"CONSTRUCT {{<{res}> ?p ?o}} WHERE {{<{res}> ?p ?o}}"
         sparql.setQuery(query)
         sparql.setMethod('GET')
-        sparql.setReturnFormat(RDFXML)
-        result: ConjunctiveGraph = sparql.query().convert()
+        sparql.setReturnFormat(XML)
+        result: ConjunctiveGraph = sparql.queryAndConvert()
         if result is not None:
             imported_entities: List[GraphEntity] = Reader.import_entities_from_graph(g_set, result,
                                                                                      resp_agent, enable_validation)
             if len(imported_entities) <= 0:
                 raise ValueError("The requested entity was not found or was not recognized as a proper OCDM entity.")
             else:
                 return imported_entities[0]
```

### Comparing `oc_ocdm-7.1.9/oc_ocdm/resources/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/resources/querymap.txt` & `oc_ocdm-7.2.0/oc_ocdm/resources/querymap.txt`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/resources/shacle.ttl` & `oc_ocdm-7.2.0/oc_ocdm/resources/shacle.ttl`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/resources/shexc.txt` & `oc_ocdm-7.2.0/oc_ocdm/resources/shexc.txt`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/resources/shexc_closed.txt` & `oc_ocdm-7.2.0/oc_ocdm/resources/shexc_closed.txt`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/storer.py` & `oc_ocdm-7.2.0/oc_ocdm/storer.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     from oc_ocdm.abstract_set import AbstractSet
 
 
 class Storer(object):
 
     def __init__(self, abstract_set: AbstractSet, repok: Reporter = None, reperr: Reporter = None,
                  context_map: Dict[str, Any] = None, default_dir: str = "_", dir_split: int = 0,
-                 n_file_item: int = 1, output_format: str = "json-ld", zip_output: bool = False) -> None:
+                 n_file_item: int = 1, output_format: str = "json-ld", zip_output: bool = False, modified_entities: set = None) -> None:
         # We only accept format strings that:
         # 1. are supported by rdflib
         # 2. correspond to an output format which is effectively either NT or NQ
         # The only exception to this rule is the 'json-ld' format, which is the default value of 'output_format'.
         supported_formats: Set[str] = {'application/n-triples', 'ntriples', 'nt', 'nt11',
                                        'application/n-quads', 'nquads', 'json-ld'}
         if output_format not in supported_formats:
@@ -59,14 +59,15 @@
         else:
             self.output_format: str = output_format
         self.zip_output = zip_output
         self.dir_split: int = dir_split
         self.n_file_item: int = n_file_item
         self.default_dir: str = default_dir if default_dir != "" else "_"
         self.a_set: AbstractSet = abstract_set
+        self.modified_entities = modified_entities
 
         if context_map is not None:
             self.context_map: Dict[str, Any] = context_map
         else:
             self.context_map: Dict[str, Any] = {}
 
         if self.output_format == "json-ld":
@@ -146,19 +147,23 @@
         self.repok.new_article()
         self.reperr.new_article()
 
         self.repok.add_sentence("Starting the process")
 
         relevant_paths: Dict[str, list] = dict()
         for entity in self.a_set.res_to_entity.values():
-            cur_dir_path, cur_file_path = self._dir_and_file_paths(entity.res, base_dir, base_iri)
-            if not os.path.exists(cur_dir_path):
-                os.makedirs(cur_dir_path)
-            relevant_paths.setdefault(cur_file_path, list())
-            relevant_paths[cur_file_path].append(entity)
+            is_relevant = True
+            if self.modified_entities is not None and entity.res not in self.modified_entities:
+                is_relevant = False
+            if is_relevant:
+                cur_dir_path, cur_file_path = self._dir_and_file_paths(entity.res, base_dir, base_iri)
+                if not os.path.exists(cur_dir_path):
+                    os.makedirs(cur_dir_path)
+                relevant_paths.setdefault(cur_file_path, list())
+                relevant_paths[cur_file_path].append(entity)
 
         for relevant_path, entities_in_path in relevant_paths.items():
             stored_g = None
             # Here we try to obtain a reference to the currently stored graph
             output_filepath = relevant_path.replace(os.path.splitext(relevant_path)[1], ".zip") if self.zip_output else relevant_path
             if os.path.exists(output_filepath):
                 stored_g = Reader(context_map=self.context_map).load(output_filepath)
```

### Comparing `oc_ocdm-7.1.9/oc_ocdm/support/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/support/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/support/query_utils.py` & `oc_ocdm-7.2.0/oc_ocdm/support/query_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,25 +28,25 @@
 
 
 def get_delete_query(graph_iri: URIRef, data: Graph) -> Tuple[str, int]:
     num_of_statements: int = len(data)
     if num_of_statements <= 0:
         return "", 0
     else:
-        statements: str = data.serialize(format="nt11").replace('\n\n', '')
+        statements: str = data.serialize(format="nt11").replace('\n', '')
         delete_string: str = f"DELETE DATA {{ GRAPH <{graph_iri}> {{ {statements} }} }}"
         return delete_string, num_of_statements
 
 
 def get_insert_query(graph_iri: URIRef, data: Graph) -> Tuple[str, int]:
     num_of_statements: int = len(data)
     if num_of_statements <= 0:
         return "", 0
     else:
-        statements: str = data.serialize(format="nt11").replace('\n\n', '')
+        statements: str = data.serialize(format="nt11").replace('\n', '')
         insert_string: str = f"INSERT DATA {{ GRAPH <{graph_iri}> {{ {statements} }} }}"
         return insert_string, num_of_statements
 
 
 def get_update_query(entity: AbstractEntity, entity_type: str = "graph") -> Tuple[str, int, int]:
     if entity_type in ["graph", "metadata"]:
         to_be_deleted: bool = entity.to_be_deleted
```

### Comparing `oc_ocdm-7.1.9/oc_ocdm/support/reporter.py` & `oc_ocdm-7.2.0/oc_ocdm/support/reporter.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/support/support.py` & `oc_ocdm-7.2.0/oc_ocdm/support/support.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,16 +164,16 @@
 
 
 def is_string_empty(string: str) -> bool:
     return string is None or string.strip() == ""
 
 
 # Variable used in several functions
-entity_regex: str = r"^(.+)/([a-z][a-z])/(0[1-9]+0)?([1-9][0-9]*)$"
-prov_regex: str = r"^(.+)/([a-z][a-z])/(0[1-9]+0)?([1-9][0-9]*)/prov/([a-z][a-z])/([1-9][0-9]*)$"
+entity_regex: str = r"^(.+)/([a-z][a-z])/(0[1-9]+0)?((?:[1-9][0-9]*)|(?:\d+-\d+))$"
+prov_regex: str = r"^(.+)/([a-z][a-z])/(0[1-9]+0)?((?:[1-9][0-9]*)|(?:\d+-\d+))/prov/([a-z][a-z])/([1-9][0-9]*)$"
 
 
 def _get_match(regex: str, group: int, string: str) -> str:
     match: Match = re.match(regex, string)
     if match is not None:
         return match.group(group)
     else:
```

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/test/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/counter_handler/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/test/counter_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/counter_handler/test_filesystem_counter_handler.py` & `oc_ocdm-7.2.0/oc_ocdm/test/counter_handler/test_filesystem_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/counter_handler/test_in_memory_counter_handler.py` & `oc_ocdm-7.2.0/oc_ocdm/test/counter_handler/test_in_memory_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/coverage/.coverage` & `oc_ocdm-7.2.0/oc_ocdm/test/coverage/.coverage`

 * *Files 2% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -14,15 +14,15 @@
     --  'has_arcs' boolean      -- Is this data recording branches?
     --  'sys_argv' text         -- The coverage command line that recorded the data.
     --  'version' text          -- The version of coverage.py that made the file.
     --  'when' text             -- Datetime when the file was created.
 );
 INSERT INTO meta VALUES('sys_argv','[''python -m unittest'', ''discover'', ''-s'', ''oc_ocdm/test'', ''-p'', ''test_*.py'']');
 INSERT INTO meta VALUES('version','6.5.0');
-INSERT INTO meta VALUES('when','2023-02-12 15:35:45');
+INSERT INTO meta VALUES('when','2023-03-03 14:14:14');
 INSERT INTO meta VALUES('has_arcs','0');
 CREATE TABLE file (
     -- A row per file measured.
     id integer primary key,
     path text,
     unique (path)
 );
@@ -93,18 +93,20 @@
 INSERT INTO file VALUES(65,'/home/runner/work/oc_ocdm/oc_ocdm/oc_ocdm/test/metadata/entities/test_dataset.py');
 INSERT INTO file VALUES(66,'/home/runner/work/oc_ocdm/oc_ocdm/oc_ocdm/test/metadata/entities/test_distribution.py');
 INSERT INTO file VALUES(67,'/home/runner/work/oc_ocdm/oc_ocdm/oc_ocdm/test/metadata/test_metadata_set.py');
 INSERT INTO file VALUES(68,'/home/runner/work/oc_ocdm/oc_ocdm/oc_ocdm/test/prov/__init__.py');
 INSERT INTO file VALUES(69,'/home/runner/work/oc_ocdm/oc_ocdm/oc_ocdm/test/prov/entities/__init__.py');
 INSERT INTO file VALUES(70,'/home/runner/work/oc_ocdm/oc_ocdm/oc_ocdm/test/prov/entities/test_snapshot_entity.py');
 INSERT INTO file VALUES(71,'/home/runner/work/oc_ocdm/oc_ocdm/oc_ocdm/test/prov/test_prov_set.py');
-INSERT INTO file VALUES(72,'/home/runner/work/oc_ocdm/oc_ocdm/oc_ocdm/test/storer/__init__.py');
-INSERT INTO file VALUES(73,'/home/runner/work/oc_ocdm/oc_ocdm/oc_ocdm/test/storer/test_storer.py');
-INSERT INTO file VALUES(74,'/home/runner/work/oc_ocdm/oc_ocdm/oc_ocdm/test/support/__init__.py');
-INSERT INTO file VALUES(75,'/home/runner/work/oc_ocdm/oc_ocdm/oc_ocdm/test/support/test_support.py');
+INSERT INTO file VALUES(72,'/home/runner/work/oc_ocdm/oc_ocdm/oc_ocdm/test/resources/__init__.py');
+INSERT INTO file VALUES(73,'/home/runner/work/oc_ocdm/oc_ocdm/oc_ocdm/test/resources/test_shacle.py');
+INSERT INTO file VALUES(74,'/home/runner/work/oc_ocdm/oc_ocdm/oc_ocdm/test/storer/__init__.py');
+INSERT INTO file VALUES(75,'/home/runner/work/oc_ocdm/oc_ocdm/oc_ocdm/test/storer/test_storer.py');
+INSERT INTO file VALUES(76,'/home/runner/work/oc_ocdm/oc_ocdm/oc_ocdm/test/support/__init__.py');
+INSERT INTO file VALUES(77,'/home/runner/work/oc_ocdm/oc_ocdm/oc_ocdm/test/support/test_support.py');
 CREATE TABLE context (
     -- A row per context measured.
     id integer primary key,
     context text,
     unique (context)
 );
 INSERT INTO context VALUES(1,'');
@@ -117,55 +119,55 @@
     foreign key (file_id) references file (id),
     foreign key (context_id) references context (id),
     unique (file_id, context_id)
 );
 INSERT INTO line_bits VALUES(1,1,X'02');
 INSERT INTO line_bits VALUES(2,1,X'0000cb77affbfdbbffffefdffbfbfbbffd7dfdfdaff704');
 INSERT INTO line_bits VALUES(3,1,X'00000d');
-INSERT INTO line_bits VALUES(4,1,X'00007df71720c2f11b036304207eff006ff7aebfedebfe13822f2100c0052000000000808040');
+INSERT INTO line_bits VALUES(4,1,X'00007df717a040f11b036304207eff006ff7aebfedebfe13822f1100c00d2000000000808020');
 INSERT INTO line_bits VALUES(5,1,X'000006');
-INSERT INTO line_bits VALUES(6,1,X'000055c1fffffefffffffffffffffffffffffffffff37ff86f8c16005355955300e07033743e');
-INSERT INTO line_bits VALUES(7,1,X'00006d212a2e00090a000101408205c002340b00fe029fbbcf06');
+INSERT INTO line_bits VALUES(6,1,X'000055c1fffffefffffffffffffffffffffffffffffb7ff26fac163c7377975300e07033743e');
+INSERT INTO line_bits VALUES(7,1,X'00006d61282e00090a000101408205c002340b00fe029fbbcf06');
 INSERT INTO line_bits VALUES(8,1,X'000062');
-INSERT INTO line_bits VALUES(9,1,X'0000bd400900a8f195feafc11bf7defdffa45ce6cc989780978793879380970040a0202f7afd622f0300000040e7');
+INSERT INTO line_bits VALUES(9,1,X'0000bd400900a8f195feafc11bf7defdffa45ce6cc989780978793879380970020a0200d6afc722f0300000040e7');
 INSERT INTO line_bits VALUES(10,1,X'000015fbfdfc121001');
 INSERT INTO line_bits VALUES(11,1,X'000015cc03e73c9cee6b');
-INSERT INTO line_bits VALUES(12,1,X'0000d5456b6dd5e4ffd8c3ffad633dfb59cf7ad6b39efdac673dfb59ef16a0f4ef2b00e0f9ffff7f017f010101010101017f01');
-INSERT INTO line_bits VALUES(13,1,X'0000ad101505be000880');
-INSERT INTO line_bits VALUES(14,1,X'00007ddf020a0000040040000000008000018101000000000000002800000000000028');
+INSERT INTO line_bits VALUES(12,1,X'0000d5456b6dd5f4ffd4c3ffad53bdfa55af7ad5ab5efdaa57bdfa55ef76aef4ef2b00e0f9ffff7f017f010101010101017f01');
+INSERT INTO line_bits VALUES(13,1,X'0000ad301405be011880');
+INSERT INTO line_bits VALUES(14,1,X'0000bdb7402a036304004000000000807fbfe7ffffed5f5c5cc4c55d1a');
 INSERT INTO line_bits VALUES(15,1,X'00000e');
-INSERT INTO line_bits VALUES(16,1,X'000059010060000006006000c00060');
-INSERT INTO line_bits VALUES(17,1,X'0000bd4c2d20f92700000001005300c0b6eddef57f74edfdbbd5fbeb4fa5bb3f599bef05000010800d01d806');
-INSERT INTO line_bits VALUES(18,1,X'00009554fc0900c0f66d2900c0be3d0500d8b7cd02806d29005b5200b60c');
+INSERT INTO line_bits VALUES(16,1,X'0000d9010060000006006000c00060');
+INSERT INTO line_bits VALUES(17,1,X'0000bdcc2c20f91700000001005300c0b6eddef57f74edfdbbd5fbfb4fa5bb3fd99be705000010800d01d806');
+INSERT INTO line_bits VALUES(18,1,X'0000954cfc0500c0f66d2900c0be3d0500d8b7cd02806d29005b5200b60c');
 INSERT INTO line_bits VALUES(19,1,X'000006');
-INSERT INTO line_bits VALUES(20,1,X'0000556401d020c117003400a40020e1df0d');
+INSERT INTO line_bits VALUES(20,1,X'0000556401d020c137003400a40020e1df0d');
 INSERT INTO line_bits VALUES(21,1,X'0000ad1200d03f0c');
-INSERT INTO line_bits VALUES(22,1,X'00002d4e0a00809ea0600100020005005000a000400100b800000a0080020005000a00140028005000a000400180bec0');
+INSERT INTO line_bits VALUES(22,1,X'00002dce1800809ea060030006000d00d000a001400300b801001a008006000d001a0034006800d000a001400380bec0');
 INSERT INTO line_bits VALUES(23,1,X'0000fe07');
-INSERT INTO line_bits VALUES(24,1,X'000055cc0200000000820b002c487001c082040bc002b0002c08');
-INSERT INTO line_bits VALUES(25,1,X'0000559850000000000202008005098000d000000410002c08');
-INSERT INTO line_bits VALUES(26,1,X'0000b5c05400007433333333332328005890a00060418209002c487005800600202800f0820457006800008202002c4850006041822b00340000c115001a0080e00ba001200916003400800080005000200014000a000580024001a00050002800100008000580024001a0004000280014000a00050002000180004000200010000a000500024001a0005000280010000a000580024001800010');
-INSERT INTO line_bits VALUES(27,1,X'0000d562020a00000000400001c0820410002c484000002f484000c08204080016240005a00014800250000a400108');
-INSERT INTO line_bits VALUES(28,1,X'00005598280000000000000101c08204400068000002080016240002400300100001a0010008080016242000106000001000140014001400140014001400140004');
-INSERT INTO line_bits VALUES(29,1,X'0000554c0a0000000404c08204400068');
-INSERT INTO line_bits VALUES(30,1,X'0000554ca00000000410005810');
-INSERT INTO line_bits VALUES(31,1,X'00005598280000000010100058900002000b124000604102200068');
-INSERT INTO line_bits VALUES(32,1,X'00002d4e05000000000204000b121000c02948400000a7200102800509000580');
-INSERT INTO line_bits VALUES(33,1,X'0000552605000000000202000b1210002c484000b02001024003');
+INSERT INTO line_bits VALUES(24,1,X'000055cc0600000000821b002c487003c082040bc002b0002c08');
+INSERT INTO line_bits VALUES(25,1,X'00005598c1000000000206008005098001d000000430002c08');
+INSERT INTO line_bits VALUES(26,1,X'0000b5c0cc00007433333333332368005890a00160418219002c48700d800600206800f08204d7006800008206002c48d0006041826b00340000c135001a0080e01ba001200936003400800080005000200014000a000580024001a00050002800100008000580024001a0004000280014000a00050002000180004000200010000a000500024001a0005000280010000a000580024001800010');
+INSERT INTO line_bits VALUES(27,1,X'0000d562061800000000400003c0820430002c48c000002f48c000c08204180016240005a00014800250000a400108');
+INSERT INTO line_bits VALUES(28,1,X'00005598610000000000000103c08204c00068000002180016240006400300100003a0010008180016246000106000001000140014001400140014001400140004');
+INSERT INTO line_bits VALUES(29,1,X'000055cc18000000040cc08204c00068');
+INSERT INTO line_bits VALUES(30,1,X'000055cc800100000430005810');
+INSERT INTO line_bits VALUES(31,1,X'00005598610000000010300058900006000b12c000604102600068');
+INSERT INTO line_bits VALUES(32,1,X'00002dce0c00000000020c000b123000c02948c00000a7200106800509000580');
+INSERT INTO line_bits VALUES(33,1,X'000055660c000000000206000b1230002c48c000b02001064003');
 INSERT INTO line_bits VALUES(34,1,X'000006');
-INSERT INTO line_bits VALUES(35,1,X'0000b5f0f6ff33f8bff1d102605a1111400000000010');
-INSERT INTO line_bits VALUES(36,1,X'0000f54b93d935cec2b39e5b004b411710');
+INSERT INTO line_bits VALUES(35,1,X'0000b5f0f6ff3bf1bff1d102605e3313400000000010');
+INSERT INTO line_bits VALUES(36,1,X'0000f54bd3d935aec2ab5e5b004bc11710');
 INSERT INTO line_bits VALUES(37,1,X'000006');
-INSERT INTO line_bits VALUES(38,1,X'0000754105000000000000000202800509080016242000b0200101800509088006002040003400000101c0820440003400000102800509800068');
-INSERT INTO line_bits VALUES(39,1,X'0000d5420500000000002020005890800060410202000b121000589080006041020280050908001604');
+INSERT INTO line_bits VALUES(38,1,X'000075c10c000000000000000206800509180016246000b02001038005091880060020c0003400000103c08204c0003400000106800509800168');
+INSERT INTO line_bits VALUES(39,1,X'0000d5c20c00000000002060005890800160410206000b123000589080016041020680050918001604');
 INSERT INTO line_bits VALUES(40,1,X'000006');
-INSERT INTO line_bits VALUES(41,1,X'0000d58250ff09ee633453');
-INSERT INTO line_bits VALUES(42,1,X'0000dd45eb48dcafdbefbbbf7e7619b66bdffe4c97adfdf61e00bc033800aa9f5d01');
+INSERT INTO line_bits VALUES(41,1,X'0000d58241ff4dec633473');
+INSERT INTO line_bits VALUES(42,1,X'0000dd45eb68daafdbefbbbf7f7619b66bdffe4c97adfdf61e00ba033800ba9f5d01');
 INSERT INTO line_bits VALUES(43,1,X'000002');
-INSERT INTO line_bits VALUES(44,1,X'0000d50591a0008005090a00b020c102c08204b700d000000408002c48500060418202002c48b000b020');
+INSERT INTO line_bits VALUES(44,1,X'0000d50583a0018005091a00b020c102c08204b701d000000418002c48d00060418206002c48b001b020');
 INSERT INTO line_bits VALUES(45,1,X'0000a5bdbffffdefbff7fbefbfbff7f7bffffdfbfefe7dbfdff7f727');
 INSERT INTO line_bits VALUES(46,1,X'02');
 INSERT INTO line_bits VALUES(47,1,X'02');
 INSERT INTO line_bits VALUES(48,1,X'02');
 INSERT INTO line_bits VALUES(49,1,X'0000cdeebbdd6eb79b');
 INSERT INTO line_bits VALUES(50,1,X'000035bbf776bb09');
 INSERT INTO line_bits VALUES(51,1,X'000035bbbfb7b7dbedf7efdfdddede6eb7dbdbed76bbdd6eb7dbed76bbdd6eb7dbed76bbdd6eb7dbed76bb09');
@@ -186,17 +188,19 @@
 INSERT INTO line_bits VALUES(66,1,X'000035bbbdbdbd7b7b7b7b27');
 INSERT INTO line_bits VALUES(67,1,X'0000d5d97ebbdd7f3f01');
 INSERT INTO line_bits VALUES(68,1,X'02');
 INSERT INTO line_bits VALUES(69,1,X'02');
 INSERT INTO line_bits VALUES(70,1,X'000075f6de77dfbddddededede04');
 INSERT INTO line_bits VALUES(71,1,X'0000757677f7f6db8ff6df3ddbffaddfde7e7bfb68ffd66f7febb7fbde3601');
 INSERT INTO line_bits VALUES(72,1,X'02');
-INSERT INTO line_bits VALUES(73,1,X'0000bfcedffeffffffffffffff0fffff3ffc27');
+INSERT INTO line_bits VALUES(73,1,X'b6f9ffbf3f803f');
 INSERT INTO line_bits VALUES(74,1,X'02');
-INSERT INTO line_bits VALUES(75,1,X'0000ebb8ab9e76b3f2f576b75afdef7f02');
+INSERT INTO line_bits VALUES(75,1,X'0000bfcedffeffffffffffffff0fffff3ffc27');
+INSERT INTO line_bits VALUES(76,1,X'02');
+INSERT INTO line_bits VALUES(77,1,X'0000ebb8ab9e76b3f6f576b75afdef7f02');
 CREATE TABLE arc (
     -- If recording branches, a row per context per from/to line transition executed.
     file_id integer,            -- foreign key to `file`.
     context_id integer,         -- foreign key to `context`.
     fromno integer,             -- line number jumped from.
     tono integer,               -- line number jumped to.
     foreign key (file_id) references file (id),
```

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/coverage/coverage.svg` & `oc_ocdm-7.2.0/oc_ocdm/test/coverage/coverage.svg`

 * *Files 2% similar despite different names*

```diff
@@ -47,12 +47,12 @@
 000002e0: 6765 3c2f 7465 7874 3e0d 0a20 2020 2020  ge</text>..     
 000002f0: 2020 203c 7465 7874 2078 3d22 3331 2e35     <text x="31.5
 00000300: 2220 793d 2231 3422 3e63 6f76 6572 6167  " y="14">coverag
 00000310: 653c 2f74 6578 743e 0d0a 2020 2020 2020  e</text>..      
 00000320: 2020 3c74 6578 7420 783d 2238 3022 2079    <text x="80" y
 00000330: 3d22 3135 2220 6669 6c6c 3d22 2330 3130  ="15" fill="#010
 00000340: 3130 3122 2066 696c 6c2d 6f70 6163 6974  101" fill-opacit
-00000350: 793d 222e 3322 3e37 3925 3c2f 7465 7874  y=".3">79%</text
+00000350: 793d 222e 3322 3e38 3125 3c2f 7465 7874  y=".3">81%</text
 00000360: 3e0d 0a20 2020 2020 2020 203c 7465 7874  >..        <text
-00000370: 2078 3d22 3830 2220 793d 2231 3422 3e37   x="80" y="14">7
-00000380: 3925 3c2f 7465 7874 3e0d 0a20 2020 203c  9%</text>..    <
+00000370: 2078 3d22 3830 2220 793d 2231 3422 3e38   x="80" y="14">8
+00000380: 3125 3c2f 7465 7874 3e0d 0a20 2020 203c  1%</text>..    <
 00000390: 2f67 3e0d 0a3c 2f73 7667 3e0d 0a         /g>..</svg>..
```

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/graph/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/test/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_agent_role.py` & `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_agent_role.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_reference.py` & `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_reference.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_resource.py` & `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_resource.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_citation.py` & `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_citation.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,26 +16,29 @@
 import unittest
 
 from rdflib import URIRef, XSD, Literal, RDF
 
 from oc_ocdm.graph.graph_entity import GraphEntity
 from oc_ocdm.graph.graph_set import GraphSet
 
+from oc_ocdm.counter_handler.sqlite_counter_handler import SqliteCounterHandler
+
 
 class TestCitation(unittest.TestCase):
     resp_agent = 'http://resp_agent.test/'
 
     @classmethod
     def setUpClass(cls) -> None:
-        cls.graph_set = GraphSet("http://test/", "./info_dir/", "", False)
+        cls.graph_set = GraphSet("https://w3id.org/oc/index/coci/", "./info_dir/", "", False)
 
     def setUp(self):
         self.br1 = self.graph_set.add_br(self.resp_agent)
         self.br2 = self.graph_set.add_br(self.resp_agent)
         self.ci = self.graph_set.add_ci(self.resp_agent)
+        self.ci_oci = self.graph_set.add_ci(self.resp_agent, res=URIRef('https://w3id.org/oc/index/coci/ci/020010000023601000907630001040258020000010008010559090238044008040338381018136312231227010309014203370037122439026325-020010305093619112227370109090937010437073701020309'))
 
     def test_has_citing_entity(self):
         result = self.ci.has_citing_entity(self.br1)
         self.assertIsNone(result)
 
         triple = self.ci.res, GraphEntity.iri_has_citing_entity, self.br1.res
         self.assertIn(triple, self.ci.g)
@@ -142,14 +145,13 @@
 
         triple = self.ci.res, RDF.type, GraphEntity.iri_journal_cartel_citation
         self.assertIn(triple, self.ci.g)
 
     def test_create_distant_citation(self):
         result = self.ci.create_distant_citation()
         self.assertIsNone(result)
-
         triple = self.ci.res, RDF.type, GraphEntity.iri_distant_citation
         self.assertIn(triple, self.ci.g)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_discourse_element.py` & `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_discourse_element.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_pointer_list.py` & `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_pointer_list.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_reference_annotation.py` & `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_reference_annotation.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_reference_pointer.py` & `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_reference_pointer.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_resource_embodiment.py` & `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_resource_embodiment.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/bibliographic/test_responsible_agent.py` & `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_responsible_agent.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/test_bibliographic_entity.py` & `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/test_bibliographic_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/graph/entities/test_identifier.py` & `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/test_identifier.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,177 +25,177 @@
     resp_agent = 'http://resp_agent.test/'
 
     @classmethod
     def setUpClass(cls) -> None:
         cls.graph_set = GraphSet("http://test/", "./info_dir/", "", False)
 
     def setUp(self):
-        self.id = self.graph_set.add_id(self.resp_agent)
+        self.identifier = self.graph_set.add_id(self.resp_agent)
 
     def test_create_orcid(self):
         orcid = "abcdefghi"
-        result = self.id.create_orcid(orcid)
+        result = self.identifier.create_orcid(orcid)
         self.assertIsNone(result)
 
-        triple = self.id.res, GraphEntity.iri_has_literal_value, Literal(orcid)
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_has_literal_value, Literal(orcid)
+        self.assertIn(triple, self.identifier.g)
 
-        triple = self.id.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_orcid
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_orcid
+        self.assertIn(triple, self.identifier.g)
 
     def test_create_doi(self):
         doi = "abcdefghi"
-        result = self.id.create_doi(doi)
+        result = self.identifier.create_doi(doi)
         self.assertIsNone(result)
 
-        triple = self.id.res, GraphEntity.iri_has_literal_value, Literal(doi)
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_has_literal_value, Literal(doi)
+        self.assertIn(triple, self.identifier.g)
 
-        triple = self.id.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_doi
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_doi
+        self.assertIn(triple, self.identifier.g)
 
     def test_create_pmid(self):
         pmid = "abcdefghi"
-        result = self.id.create_pmid(pmid)
+        result = self.identifier.create_pmid(pmid)
         self.assertIsNone(result)
 
-        triple = self.id.res, GraphEntity.iri_has_literal_value, Literal(pmid)
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_has_literal_value, Literal(pmid)
+        self.assertIn(triple, self.identifier.g)
 
-        triple = self.id.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_pmid
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_pmid
+        self.assertIn(triple, self.identifier.g)
 
     def test_create_pmcid(self):
         pmcid = "abcdefghi"
-        result = self.id.create_pmcid(pmcid)
+        result = self.identifier.create_pmcid(pmcid)
         self.assertIsNone(result)
 
-        triple = self.id.res, GraphEntity.iri_has_literal_value, Literal(pmcid)
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_has_literal_value, Literal(pmcid)
+        self.assertIn(triple, self.identifier.g)
 
-        triple = self.id.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_pmcid
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_pmcid
+        self.assertIn(triple, self.identifier.g)
 
     def test_create_issn(self):
         issn = "abcdefghi"
-        result = self.id.create_issn(issn)
+        result = self.identifier.create_issn(issn)
         self.assertIsNone(result)
 
-        triple = self.id.res, GraphEntity.iri_has_literal_value, Literal(issn)
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_has_literal_value, Literal(issn)
+        self.assertIn(triple, self.identifier.g)
 
-        triple = self.id.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_issn
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_issn
+        self.assertIn(triple, self.identifier.g)
 
     def test_create_isbn(self):
         isbn = "abcdefghi"
-        result = self.id.create_isbn(isbn)
+        result = self.identifier.create_isbn(isbn)
         self.assertIsNone(result)
 
-        triple = self.id.res, GraphEntity.iri_has_literal_value, Literal(isbn)
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_has_literal_value, Literal(isbn)
+        self.assertIn(triple, self.identifier.g)
 
-        triple = self.id.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_isbn
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_isbn
+        self.assertIn(triple, self.identifier.g)
 
     def test_create_url(self):
         url = "abcdefghi"
-        result = self.id.create_url(url)
+        result = self.identifier.create_url(url)
         self.assertIsNone(result)
 
-        triple = self.id.res, GraphEntity.iri_has_literal_value, Literal(url)
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_has_literal_value, Literal(url)
+        self.assertIn(triple, self.identifier.g)
 
-        triple = self.id.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_url
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_url
+        self.assertIn(triple, self.identifier.g)
 
     def test_create_xpath(self):
         xpath = "abcdefghi"
-        result = self.id.create_xpath(xpath)
+        result = self.identifier.create_xpath(xpath)
         self.assertIsNone(result)
 
-        triple = self.id.res, GraphEntity.iri_has_literal_value, Literal(xpath)
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_has_literal_value, Literal(xpath)
+        self.assertIn(triple, self.identifier.g)
 
-        triple = self.id.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_xpath
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_xpath
+        self.assertIn(triple, self.identifier.g)
 
     def test_create_intrepid(self):
         intrepid = "abcdefghi"
-        result = self.id.create_intrepid(intrepid)
+        result = self.identifier.create_intrepid(intrepid)
         self.assertIsNone(result)
 
-        triple = self.id.res, GraphEntity.iri_has_literal_value, Literal(intrepid)
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_has_literal_value, Literal(intrepid)
+        self.assertIn(triple, self.identifier.g)
 
-        triple = self.id.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_intrepid
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_intrepid
+        self.assertIn(triple, self.identifier.g)
 
     def test_create_xmlid(self):
         xmlid = "abcdefghi"
-        result = self.id.create_xmlid(xmlid)
+        result = self.identifier.create_xmlid(xmlid)
         self.assertIsNone(result)
 
-        triple = self.id.res, GraphEntity.iri_has_literal_value, Literal(xmlid)
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_has_literal_value, Literal(xmlid)
+        self.assertIn(triple, self.identifier.g)
 
-        triple = self.id.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_xmlid
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_xmlid
+        self.assertIn(triple, self.identifier.g)
 
     def test_create_wikidata(self):
         wikidata = "abcdefghi"
-        result = self.id.create_wikidata(wikidata)
+        result = self.identifier.create_wikidata(wikidata)
         self.assertIsNone(result)
 
-        triple = self.id.res, GraphEntity.iri_has_literal_value, Literal(wikidata)
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_has_literal_value, Literal(wikidata)
+        self.assertIn(triple, self.identifier.g)
 
-        triple = self.id.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_wikidata
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_wikidata
+        self.assertIn(triple, self.identifier.g)
 
     def test_create_wikipedia(self):
         wikipedia = "abcdefghi"
-        result = self.id.create_wikipedia(wikipedia)
+        result = self.identifier.create_wikipedia(wikipedia)
         self.assertIsNone(result)
 
-        triple = self.id.res, GraphEntity.iri_has_literal_value, Literal(wikipedia)
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_has_literal_value, Literal(wikipedia)
+        self.assertIn(triple, self.identifier.g)
 
-        triple = self.id.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_wikipedia
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_wikipedia
+        self.assertIn(triple, self.identifier.g)
 
     def test_create_crossref(self):
         crossref = "abcdefghi"
-        result = self.id.create_crossref(crossref)
+        result = self.identifier.create_crossref(crossref)
         self.assertIsNone(result)
 
-        triple = self.id.res, GraphEntity.iri_has_literal_value, Literal(crossref)
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_has_literal_value, Literal(crossref)
+        self.assertIn(triple, self.identifier.g)
 
-        triple = self.id.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_crossref
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_crossref
+        self.assertIn(triple, self.identifier.g)
 
     def test_create_datacite(self):
         datacite = "332"
-        result = self.id.create_datacite(datacite)
+        result = self.identifier.create_datacite(datacite)
         self.assertIsNone(result)
 
-        triple = self.id.res, GraphEntity.iri_has_literal_value, Literal(datacite)
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_has_literal_value, Literal(datacite)
+        self.assertIn(triple, self.identifier.g)
 
-        triple = self.id.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_datacite
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_datacite
+        self.assertIn(triple, self.identifier.g)
 
     def test_create_viaf(self):
         viaf = "abcdefghi"
-        result = self.id.create_viaf(viaf)
+        result = self.identifier.create_viaf(viaf)
         self.assertIsNone(result)
 
-        triple = self.id.res, GraphEntity.iri_has_literal_value, Literal(viaf)
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_has_literal_value, Literal(viaf)
+        self.assertIn(triple, self.identifier.g)
 
-        triple = self.id.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_viaf
-        self.assertIn(triple, self.id.g)
+        triple = self.identifier.res, GraphEntity.iri_uses_identifier_scheme, GraphEntity.iri_viaf
+        self.assertIn(triple, self.identifier.g)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/graph/test_graph_entity.py` & `oc_ocdm-7.2.0/oc_ocdm/test/graph/test_graph_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/graph/test_graph_set.py` & `oc_ocdm-7.2.0/oc_ocdm/test/graph/test_graph_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/metadata/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/test/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/metadata/entities/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/test/metadata/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/metadata/entities/test_dataset.py` & `oc_ocdm-7.2.0/oc_ocdm/test/metadata/entities/test_dataset.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/metadata/entities/test_distribution.py` & `oc_ocdm-7.2.0/oc_ocdm/test/metadata/entities/test_distribution.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/metadata/test_metadata_set.py` & `oc_ocdm-7.2.0/oc_ocdm/test/metadata/test_metadata_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/prov/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/test/prov/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/prov/entities/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/test/prov/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/prov/entities/test_snapshot_entity.py` & `oc_ocdm-7.2.0/oc_ocdm/test/prov/entities/test_snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/prov/test_prov_set.py` & `oc_ocdm-7.2.0/oc_ocdm/test/prov/test_prov_set.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,27 +11,28 @@
 # FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
 # OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
 # DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
 # ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
 # SOFTWARE.
 import unittest
 
-from rdflib import URIRef
+from rdflib import Graph, Literal, URIRef
 
+from oc_ocdm.counter_handler.sqlite_counter_handler import SqliteCounterHandler
 from oc_ocdm.graph.graph_set import GraphSet
-from oc_ocdm.prov.prov_set import ProvSet
 from oc_ocdm.prov.entities.snapshot_entity import SnapshotEntity
+from oc_ocdm.prov.prov_set import ProvSet
 
 
 class TestProvSet(unittest.TestCase):
     resp_agent = 'http://resp_agent.test/'
 
     def setUp(self):
         self.graph_set = GraphSet("http://test/", "./info_dir/", "", False)
-        self.prov_set = ProvSet(self.graph_set, "http://test/", "./info_dir/", False)
+        self.prov_set = ProvSet(self.graph_set, "http://test/", "./info_dir/", False, custom_counters={'ci': SqliteCounterHandler('oc_ocdm/test/prov/prov_counter.db')})
 
     def test_add_se(self):
         prov_subj = self.graph_set.add_br(self.resp_agent)
         se = self.prov_set.add_se(prov_subj)
 
         self.assertIsNotNone(se)
         self.assertIsInstance(se, SnapshotEntity)
@@ -43,15 +44,14 @@
 
         with self.subTest('Creation [Merged entity]'):
             a = self.graph_set.add_br(self.resp_agent)
             b = self.graph_set.add_br(self.resp_agent)
             a.merge(b)
 
             result = self.prov_set.generate_provenance(cur_time)
-            self.assertIsNone(result)
 
             se_a = self.prov_set.get_entity(URIRef(a.res + '/prov/se/1'))
             self.assertIsNotNone(se_a)
             self.assertIsInstance(se_a, SnapshotEntity)
             self.assertEqual(a.res, se_a.get_is_snapshot_of())
             self.assertEqual(cur_time_str, se_a.get_generation_time())
             if a.source is not None:
@@ -67,28 +67,28 @@
             se_a_1 = self.prov_set.add_se(a)
 
             # This avoids that the presence of the mandatory rdf:type gets interpreted
             # as a modification with respect to an empty preexisting_graph:
             a.remove_every_triple()
 
             result = self.prov_set.generate_provenance(cur_time)
-            self.assertIsNone(result)
+            
 
             se_a_2 = self.prov_set.get_entity(URIRef(a.res + '/prov/se/2'))
             self.assertIsNone(se_a_2)
         with self.subTest('Modification [Merged entity]'):
             title = "TEST TITLE"
             a = self.graph_set.add_br(self.resp_agent)
             b = self.graph_set.add_br(self.resp_agent)
             b.has_title(title)
             a.merge(b)
             se_a_1 = self.prov_set.add_se(a)
 
             result = self.prov_set.generate_provenance(cur_time)
-            self.assertIsNone(result)
+            
             self.assertEqual(cur_time_str, se_a_1.get_invalidation_time())
 
             se_a_2 = self.prov_set.get_entity(URIRef(a.res + '/prov/se/2'))
             self.assertIsNotNone(se_a_2)
             self.assertIsInstance(se_a_2, SnapshotEntity)
             self.assertEqual(a.res, se_a_2.get_is_snapshot_of())
 
@@ -108,15 +108,15 @@
             c = self.graph_set.add_br(self.resp_agent)
             a.merge(b)
             a.merge(c)
             se_a_1 = self.prov_set.add_se(a)
             se_b_1 = self.prov_set.add_se(b)
 
             result = self.prov_set.generate_provenance(cur_time)
-            self.assertIsNone(result)
+            
 
             self.assertEqual(cur_time_str, se_a_1.get_invalidation_time())
 
             se_a_2 = self.prov_set.get_entity(URIRef(a.res + '/prov/se/2'))
             self.assertIsNotNone(se_a_2)
             self.assertIsInstance(se_a_2, SnapshotEntity)
             self.assertEqual(a.res, se_a_2.get_is_snapshot_of())
@@ -128,15 +128,15 @@
 
             self.assertSetEqual({se_a_1, se_b_1}, set(se_a_2.get_derives_from()))
             self.assertEqual(f"The entity '{a.res}' has been merged with '{b.res}'.", se_a_2.get_description())
         with self.subTest('Creation [Non-Merged entity]'):
             a = self.graph_set.add_br(self.resp_agent)
 
             result = self.prov_set.generate_provenance(cur_time)
-            self.assertIsNone(result)
+            
 
             se_a = self.prov_set.get_entity(URIRef(a.res + '/prov/se/1'))
             self.assertIsNotNone(se_a)
             self.assertIsInstance(se_a, SnapshotEntity)
             self.assertEqual(a.res, se_a.get_is_snapshot_of())
             self.assertEqual(cur_time_str, se_a.get_generation_time())
             if a.source is not None:
@@ -146,40 +146,40 @@
 
             self.assertEqual(f"The entity '{a.res}' has been created.", se_a.get_description())
         with self.subTest('No snapshot [Non-Merged entity] (Scenario 1)'):
             a = self.graph_set.add_br(self.resp_agent)
             a.mark_as_to_be_deleted()
 
             result = self.prov_set.generate_provenance(cur_time)
-            self.assertIsNone(result)
+            
 
             se_a = self.prov_set.get_entity(URIRef(a.res + '/prov/se/1'))
             self.assertIsNone(se_a)
         with self.subTest('No snapshot [Merged entity] (Scenario 2)'):
             a = self.graph_set.add_br(self.resp_agent)
             se_a_1 = self.prov_set.add_se(a)
 
             # This avoids that the presence of the mandatory rdf:type gets interpreted
             # as a modification with respect to an empty preexisting_graph:
             a.remove_every_triple()
 
             result = self.prov_set.generate_provenance(cur_time)
-            self.assertIsNone(result)
+            
 
             se_a_2 = self.prov_set.get_entity(URIRef(a.res + '/prov/se/2'))
             self.assertIsNone(se_a_2)
         with self.subTest('Deletion [Non-Merged entity]'):
             title = "TEST TITLE"
             a = self.graph_set.add_br(self.resp_agent)
             se_a_1 = self.prov_set.add_se(a)
             a.has_title(title)
             a.mark_as_to_be_deleted()
 
             result = self.prov_set.generate_provenance(cur_time)
-            self.assertIsNone(result)
+            
 
             self.assertEqual(cur_time_str, se_a_1.get_invalidation_time())
 
             se_a_2 = self.prov_set.get_entity(URIRef(a.res + '/prov/se/2'))
             self.assertIsNotNone(se_a_2)
             self.assertIsInstance(se_a_2, SnapshotEntity)
             self.assertEqual(a.res, se_a_2.get_is_snapshot_of())
@@ -194,15 +194,15 @@
         with self.subTest('Modification [Non-Merged entity]'):
             title = "TEST TITLE"
             a = self.graph_set.add_br(self.resp_agent)
             se_a_1 = self.prov_set.add_se(a)
             a.has_title(title)
 
             result = self.prov_set.generate_provenance(cur_time)
-            self.assertIsNone(result)
+            
 
             self.assertEqual(cur_time_str, se_a_1.get_invalidation_time())
 
             se_a_2 = self.prov_set.get_entity(URIRef(a.res + '/prov/se/2'))
             self.assertIsNotNone(se_a_2)
             self.assertIsInstance(se_a_2, SnapshotEntity)
             self.assertEqual(a.res, se_a_2.get_is_snapshot_of())
@@ -232,10 +232,27 @@
 
         prov_subject = URIRef('https://w3id.org/oc/corpus/br/-1')
         self.assertRaises(ValueError, self.prov_set._retrieve_last_snapshot, prov_subject)
 
         prov_subject = URIRef('https://w3id.org/oc/corpus/br/abc')
         self.assertRaises(ValueError, self.prov_set._retrieve_last_snapshot, prov_subject)
 
+    def test_generate_provenance_for_citations(self):
+        preexisting_graph = Graph()
+        preexisting_graph.add((
+            URIRef('https://w3id.org/oc/index/coci/ci/020010000023601000907630001040258020000010008010559090238044008040338381018136312231227010309014203370037122439026325-020010305093619112227370109090937010437073701020309'),
+            URIRef('http://www.w3.org/1999/02/22-rdf-syntax-ns#type'),
+            URIRef('http://purl.org/spar/cito/Citation')))
+        preexisting_graph.add((
+            URIRef('https://w3id.org/oc/index/coci/ci/020010000023601000907630001040258020000010008010559090238044008040338381018136312231227010309014203370037122439026325-020010305093619112227370109090937010437073701020309'),
+            URIRef('http://purl.org/spar/cito/hasCitationCreationDate'),
+            Literal('2022', datatype='http://www.w3.org/2001/XMLSchema#gYear')))
+        ci = self.graph_set.add_ci(self.resp_agent, res=URIRef('https://w3id.org/oc/index/coci/ci/020010000023601000907630001040258020000010008010559090238044008040338381018136312231227010309014203370037122439026325-020010305093619112227370109090937010437073701020309'), preexisting_graph=preexisting_graph)
+        self.prov_set.generate_provenance()
+        self.graph_set.commit_changes()
+        ci.has_citation_creation_date('2022')
+        self.prov_set.generate_provenance()
+        prov_entity = self.prov_set._retrieve_last_snapshot(URIRef('https://w3id.org/oc/index/coci/ci/020010000023601000907630001040258020000010008010559090238044008040338381018136312231227010309014203370037122439026325-020010305093619112227370109090937010437073701020309'))
+        self.assertEqual(prov_entity, URIRef('https://w3id.org/oc/index/coci/ci/020010000023601000907630001040258020000010008010559090238044008040338381018136312231227010309014203370037122439026325-020010305093619112227370109090937010437073701020309/prov/se/1'))
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/resources/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/test/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/resources/data.json` & `oc_ocdm-7.2.0/oc_ocdm/test/resources/data.json`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/resources/data_reader.json` & `oc_ocdm-7.2.0/oc_ocdm/test/resources/data_reader.json`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/resources/data_reader_invalid.json` & `oc_ocdm-7.2.0/oc_ocdm/test/resources/data_reader_invalid.json`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/resources/test_shacle.py` & `oc_ocdm-7.2.0/oc_ocdm/test/resources/test_shacle.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/storer/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/test/storer/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/storer/test_storer.py` & `oc_ocdm-7.2.0/oc_ocdm/test/storer/test_storer.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,17 +38,17 @@
     def tearDown(self):
         rmtree(os.path.join("oc_ocdm", "test", "storer", "data"))
 
     def test_store_graphs_in_file(self):
         base_dir = os.path.join("oc_ocdm", "test", "storer", "data", "rdf") + os.sep
         is_unix = system() != "Windows"
         with self.subTest("output_format=json-ld, zip_output=True"):
-            storer = Storer(self.graph_set, context_map={}, dir_split=10000, n_file_item=1000, default_dir="_", output_format='json-ld', zip_output=True)
-            self.prov_set.generate_provenance()
+            modified_entities = self.prov_set.generate_provenance()
             prov_storer = Storer(self.prov_set, context_map={}, dir_split=10000, n_file_item=1000, default_dir="_", output_format='json-ld', zip_output=True)
+            storer = Storer(self.graph_set, context_map={}, dir_split=10000, n_file_item=1000, default_dir="_", output_format='json-ld', zip_output=True, modified_entities=modified_entities)
             storer.store_all(base_dir, self.base_iri)
             prov_storer.store_all(base_dir, self.base_iri)
             self.graph_set.commit_changes()
             with ZipFile(os.path.join(base_dir, "br", "060", "10000", "1000.zip"), mode="r") as archive:
                 with archive.open("1000.json") as f:
                     data = json.load(f)
                     self.assertEqual(data, [{'@graph': [{'@id': 'http://test/br/0601', '@type': ['http://purl.org/spar/fabio/Expression']}], '@id': 'http://test/br/'}])
```

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/support/__init__.py` & `oc_ocdm-7.2.0/oc_ocdm/test/support/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/oc_ocdm/test/support/test_support.py` & `oc_ocdm-7.2.0/oc_ocdm/test/support/test_support.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/pyproject.toml` & `oc_ocdm-7.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oc_ocdm"
-version = "7.1.9"
+version = "7.2.0"
 description = "Object mapping library for manipulating RDF graphs that are compliant with the OpenCitations datamodel."
 authors = [
     "Silvio Peroni <essepuntato@gmail.com>",
     "Marilena Daquino <marilena.daquino2@unibo.it>",
     "Fabio Mariani <fabio.mariani6@studio.unibo.it>",
     "Simone Persiani <iosonopersia@gmail.com>",
     "Arcangelo Massari <arcangelo.massari@unibo.it>"
@@ -28,25 +28,26 @@
     "Topic :: System :: Archiving",
     "Typing :: Typed"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7.4"
 rdflib = "^6.0.0"
-SPARQLWrapper = "^1.8.5"
+SPARQLWrapper = "2.0.0"
 filelock = "^3.6.0"
 pyshacl = "^0.20.0"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^4.4.0"
 sphinx_rtd_theme = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^6.5.0"
 coverage-badge = "^1.1.0"
+wget = "^3.2"
 
 [build-system]
 requires = ["poetry>=1.1.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry.scripts]
-test = 'scripts:test'
+test = 'scripts:main'
```

### Comparing `oc_ocdm-7.1.9/README.md` & `oc_ocdm-7.2.0/README.md`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.1.9/setup.py` & `oc_ocdm-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,33 +18,34 @@
  'oc_ocdm.test.graph',
  'oc_ocdm.test.graph.entities',
  'oc_ocdm.test.graph.entities.bibliographic',
  'oc_ocdm.test.metadata',
  'oc_ocdm.test.metadata.entities',
  'oc_ocdm.test.prov',
  'oc_ocdm.test.prov.entities',
+ 'oc_ocdm.test.reader',
  'oc_ocdm.test.resources',
  'oc_ocdm.test.storer',
  'oc_ocdm.test.support']
 
 package_data = \
 {'': ['*'], 'oc_ocdm.test': ['coverage/*']}
 
 install_requires = \
-['SPARQLWrapper>=1.8.5,<2.0.0',
+['SPARQLWrapper==2.0.0',
  'filelock>=3.6.0,<4.0.0',
  'pyshacl>=0.20.0,<0.21.0',
  'rdflib>=6.0.0,<7.0.0']
 
 entry_points = \
-{'console_scripts': ['test = scripts:test']}
+{'console_scripts': ['test = scripts:main']}
 
 setup_kwargs = {
     'name': 'oc-ocdm',
-    'version': '7.1.9',
+    'version': '7.2.0',
     'description': 'Object mapping library for manipulating RDF graphs that are compliant with the OpenCitations datamodel.',
     'long_description': '# oc_ocdm\n[<img src="https://img.shields.io/badge/powered%20by-OpenCitations-%239931FC?labelColor=2D22DE" />](http://opencitations.net)\n[![Run tests](https://github.com/opencitations/oc_ocdm/actions/workflows/run_tests.yml/badge.svg)](https://github.com/opencitations/oc_ocdm/actions/workflows/run_tests.yml)\n![Coverage](https://raw.githubusercontent.com/opencitations/oc_ocdm/master/oc_ocdm/test/coverage/coverage.svg)\n[![Documentation Status](https://readthedocs.org/projects/oc-ocdm/badge/?version=latest)](https://oc-ocdm.readthedocs.io/en/latest/?badge=latest)\n[![PyPI version](https://badge.fury.io/py/oc-ocdm.svg)](https://badge.fury.io/py/oc-ocdm)\n![PyPI](https://img.shields.io/pypi/pyversions/oc_meta)\n\n[![DOI](https://zenodo.org/badge/322327342.svg)](https://zenodo.org/badge/latestdoi/322327342)\n[![License: ISC](https://img.shields.io/badge/License-ISC-blue.svg)](https://opensource.org/licenses/ISC)\n\nDocumentation can be found here: [https://oc-ocdm.readthedocs.io](https://oc-ocdm.readthedocs.io).\n\n**oc_ocdm** is a Python &ge;3.7 library that enables the user to import, produce, modify and export RDF data\nstructures which are compliant with the [OCDM v2.0.1](https://figshare.com/articles/Metadata_for_the_OpenCitations_Corpus/3443876) specification.\n\n## User\'s guide\nThis package can be simply installed with **pip**:\n``` bash\n    pip install oc_ocdm\n```\n**Please, have a look at the notebooks [available here](https://github.com/opencitations/oc_ocdm/blob/master/notebooks/).**\n\n## Developer\'s guide\n\n### First steps\n  1. Install Poetry:\n``` bash\n    pip install poetry\n```\n  2. Clone this repository:\n``` bash\n    git clone https://github.com/iosonopersia/oc_ocdm\n    cd ./oc_ocdm\n```\n  3. Install all the dependencies:\n``` bash\n    poetry install\n```\n  4. Build the package (_output dir:_ `dist`):\n``` bash\n    poetry build\n```\n  5. Globally install the package (_alternatively, you can also install it inside a virtual-env,\n  by providing the full path to the .tar.gz archive_):\n``` bash\n    pip install ./dist/oc_ocdm-<VERSION>.tar.gz\n```\n  6. If everything went the right way, than you should be able to use the `oc_ocdm` library in your Python modules as follows:\n``` python\n    from oc_ocdm.graph import GraphSet\n    from oc_ocdm.graph.entities.bibliographic import AgentRole\n    # ...\n```\n\n### How to run the tests\nJust run the following command inside the root project folder:\n``` bash\n    poetry run test\n```\n\n### How to manage the project using Poetry\nSee [Poetry commands documentation](https://python-poetry.org/docs/cli/).\n\n**AAA: when adding a non-dev dependency via `poetry add`, always remember to add\nthat same dependency to the `autodoc_mock_imports` list in `docs/source/conf.py`**\n(otherwise "Read the Docs" won\'t be able to compile the documentation correctly!).\n\n### How to publish the package onto Pypi\n``` bash\n    poetry publish --build\n```\n### Install dependencies needed for the documentation\n``` bash\n    pip install Sphinx sphinx_rtd_theme\n```\n### How to generate the documentation\n``` bash\n    rm ./docs/source/modules/*\n    sphinx-apidoc  -o ./docs/source/modules oc_ocdm *test*\n```\n\n### How to build the documentation\n___\n**Warning! In order to avoid getting the following `WARNING: html_static_path entry \'_static\' does not exist`, you\'ll\nneed to manually create an empty `_static` folder with the command:**\n``` bash\n    mkdir docs/source/_static\n```\n___\n  1. Always remember to move inside the `docs` folder:\n``` bash\n    cd docs\n```\n  2. Use the Makefile provided to build the docs:\n      + _on Windows_\n        ```\n            make.bat html\n        ```\n      + _on Linux and MacOs_\n        ```\n            make html\n        ```\n  3. Open the `build/html/index.html` file with a web browser of your choice!\n\n## Acknowledgements\nThis work has been funded by the project “Open Biomedical Citations in Context Corpus”\n(Wellcome Trust, Grant n. 214471/Z/18/Z) and the project “Wikipedia Citations in Wikidata”\n(Wikimedia Foundation, https://meta.wikimedia.org/wiki/Wikicite/grant/Wikipedia_Citations_in_Wikidata).\n\nWe would like to thank (in alphabetic order) Fabio Mariani (@FabioMariani), Arcangelo\nMassari (@arcangelo7), and Gabriele Pisciotta (@GabrielePisciotta) for the constructive feedback.\n',
     'author': 'Silvio Peroni',
     'author_email': 'essepuntato@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://opencitations.net',
```

### Comparing `oc_ocdm-7.1.9/PKG-INFO` & `oc_ocdm-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oc-ocdm
-Version: 7.1.9
+Version: 7.2.0
 Summary: Object mapping library for manipulating RDF graphs that are compliant with the OpenCitations datamodel.
 Home-page: https://opencitations.net
 License: ISC
 Keywords: opencitations,openscience,datamodel,mapping
 Author: Silvio Peroni
 Author-email: essepuntato@gmail.com
 Requires-Python: >=3.7.4,<4.0.0
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving
 Classifier: Typing :: Typed
-Requires-Dist: SPARQLWrapper (>=1.8.5,<2.0.0)
+Requires-Dist: SPARQLWrapper (==2.0.0)
 Requires-Dist: filelock (>=3.6.0,<4.0.0)
 Requires-Dist: pyshacl (>=0.20.0,<0.21.0)
 Requires-Dist: rdflib (>=6.0.0,<7.0.0)
 Project-URL: Documentation, https://oc-ocdm.readthedocs.io
 Project-URL: Repository, https://github.com/opencitations/oc_ocdm
 Description-Content-Type: text/markdown
```

