# Comparing `tmp/fabric_fim-1.5.0b4.tar.gz` & `tmp/fabric_fim-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric_fim-1.5.0b4.tar", last modified: Wed May 10 19:22:12 2023, max compression
+gzip compressed data, was "fabric_fim-1.5.1.tar", last modified: Thu Jun 15 15:31:12 2023, max compression
```

## Comparing `fabric_fim-1.5.0b4.tar` & `fabric_fim-1.5.1.tar`

### file list

```diff
@@ -1,119 +1,114 @@
--rw-r--r--   0        0        0     2179 2023-05-10 17:49:37.304171 fabric_fim-1.5.0b4/.gitignore
--rw-r--r--   0        0        0       26 2020-07-24 21:42:44.564662 fabric_fim-1.5.0b4/AUTHORS
--rw-r--r--   0        0        0     1071 2020-07-14 22:09:49.459777 fabric_fim-1.5.0b4/LICENSE
--rw-r--r--   0        0        0      146 2022-04-27 22:22:19.297089 fabric_fim-1.5.0b4/MANIFEST.in
--rw-r--r--   0        0        0    11151 2023-05-10 17:57:26.155153 fabric_fim-1.5.0b4/README.md
--rw-r--r--   0        0        0    18690 2021-05-25 21:09:37.024101 fabric_fim-1.5.0b4/figs/fim-structure.png
--rw-r--r--   0        0        0      557 2021-03-15 22:13:52.784044 fabric_fim-1.5.0b4/fim/README.md
--rw-r--r--   0        0        0      105 2023-05-10 19:22:01.400252 fabric_fim-1.5.0b4/fim/__init__.py
--rw-r--r--   0        0        0        1 2022-04-27 22:22:19.299449 fabric_fim-1.5.0b4/fim/authz/__init__.py
--rw-r--r--   0        0        0    16139 2023-02-02 01:41:56.403069 fabric_fim-1.5.0b4/fim/authz/attribute_collector.py
--rw-r--r--   0        0        0      334 2020-09-12 23:24:52.369007 fabric_fim-1.5.0b4/fim/graph/README.md
--rw-r--r--   0        0        0        1 2020-09-02 18:31:38.004468 fabric_fim-1.5.0b4/fim/graph/__init__.py
--rw-r--r--   0        0        0    69843 2023-05-10 14:54:24.395497 fabric_fim-1.5.0b4/fim/graph/abc_property_graph.py
--rw-r--r--   0        0        0     4093 2023-02-02 01:41:56.406333 fabric_fim-1.5.0b4/fim/graph/abc_property_graph_constants.py
--rw-r--r--   0        0        0        1 2020-08-18 21:34:07.036009 fabric_fim-1.5.0b4/fim/graph/data/__init__.py
--rw-r--r--   0        0        0      283 2020-09-03 22:10:53.500264 fabric_fim-1.5.0b4/fim/graph/data/capacity_types.json
--rw-r--r--   0        0        0      100 2020-08-27 20:41:23.401941 fabric_fim-1.5.0b4/fim/graph/data/constraint_types.json
--rw-r--r--   0        0        0     3886 2023-05-10 14:54:24.398493 fabric_fim-1.5.0b4/fim/graph/data/graph_validation_rules.json
--rw-r--r--   0        0        0     3845 2023-05-10 14:54:24.398661 fabric_fim-1.5.0b4/fim/graph/data/graph_validation_rules_neo4j_v4.json
--rw-r--r--   0        0        0      547 2020-09-03 22:10:39.822590 fabric_fim-1.5.0b4/fim/graph/data/label_types.json
--rw-r--r--   0        0        0       91 2020-08-27 20:40:54.261031 fabric_fim-1.5.0b4/fim/graph/data/location_types.json
--rw-r--r--   0        0        0      861 2023-05-10 14:54:24.189132 fabric_fim-1.5.0b4/fim/graph/data/neo4j_indexes.json
--rw-r--r--   0        0        0     3320 2023-05-10 14:54:24.398812 fabric_fim-1.5.0b4/fim/graph/graph_util.py
--rw-r--r--   0        0        0    44293 2023-05-10 14:54:24.429886 fabric_fim-1.5.0b4/fim/graph/neo4j_property_graph.py
--rw-r--r--   0        0        0     6160 2022-10-06 17:38:08.214224 fabric_fim-1.5.0b4/fim/graph/networkx_mixin.py
--rw-r--r--   0        0        0    42211 2023-05-10 14:54:24.400876 fabric_fim-1.5.0b4/fim/graph/networkx_property_graph.py
--rw-r--r--   0        0        0     8354 2022-10-07 03:05:34.849246 fabric_fim-1.5.0b4/fim/graph/networkx_property_graph_disjoint.py
--rw-r--r--   0        0        0     1501 2021-03-15 22:13:52.788626 fabric_fim-1.5.0b4/fim/graph/resources/README.md
--rw-r--r--   0        0        0        1 2020-09-02 18:32:04.638774 fabric_fim-1.5.0b4/fim/graph/resources/__init__.py
--rw-r--r--   0        0        0     4484 2021-05-25 21:09:37.029370 fabric_fim-1.5.0b4/fim/graph/resources/abc_adm.py
--rw-r--r--   0        0        0    13570 2023-05-10 14:54:24.193783 fabric_fim-1.5.0b4/fim/graph/resources/abc_arm.py
--rw-r--r--   0        0        0     2991 2022-02-18 19:27:15.586527 fabric_fim-1.5.0b4/fim/graph/resources/abc_bqm.py
--rw-r--r--   0        0        0     4547 2021-03-31 01:14:29.518807 fabric_fim-1.5.0b4/fim/graph/resources/abc_cbm.py
--rw-r--r--   0        0        0     2297 2021-03-07 22:42:30.018249 fabric_fim-1.5.0b4/fim/graph/resources/neo4j_adm.py
--rw-r--r--   0        0        0     2106 2021-05-25 21:09:37.031668 fabric_fim-1.5.0b4/fim/graph/resources/neo4j_arm.py
--rw-r--r--   0        0        0    18591 2023-05-10 14:57:18.798602 fabric_fim-1.5.0b4/fim/graph/resources/neo4j_cbm.py
--rw-r--r--   0        0        0     5017 2022-02-18 19:27:15.587881 fabric_fim-1.5.0b4/fim/graph/resources/networkx_abqm.py
--rw-r--r--   0        0        0     2341 2021-03-07 22:42:30.020154 fabric_fim-1.5.0b4/fim/graph/resources/networkx_adm.py
--rw-r--r--   0        0        0     2122 2021-05-25 21:09:37.033196 fabric_fim-1.5.0b4/fim/graph/resources/networkx_arm.py
--rw-r--r--   0        0        0      301 2021-03-15 22:13:52.789768 fabric_fim-1.5.0b4/fim/graph/slices/README.md
--rw-r--r--   0        0        0        1 2020-09-02 18:32:24.788341 fabric_fim-1.5.0b4/fim/graph/slices/__init__.py
--rw-r--r--   0        0        0     8223 2022-02-18 19:27:15.588460 fabric_fim-1.5.0b4/fim/graph/slices/abc_asm.py
--rw-r--r--   0        0        0     3733 2023-05-10 14:54:24.196715 fabric_fim-1.5.0b4/fim/graph/slices/neo4j_asm.py
--rw-r--r--   0        0        0     4298 2021-06-04 19:43:14.989790 fabric_fim-1.5.0b4/fim/graph/slices/networkx_asm.py
--rw-r--r--   0        0        0     8615 2021-03-03 19:57:54.288231 fabric_fim-1.5.0b4/fim/graph/typed_tuples.py
--rw-r--r--   0        0        0        0 2023-02-02 01:41:56.409002 fabric_fim-1.5.0b4/fim/logging/__init__.py
--rw-r--r--   0        0        0     9071 2023-02-02 01:41:56.410072 fabric_fim-1.5.0b4/fim/logging/log_collector.py
--rw-r--r--   0        0        0     9555 2021-03-24 00:18:51.063382 fabric_fim-1.5.0b4/fim/pluggable.py
--rw-r--r--   0        0        0      189 2021-06-04 19:43:14.990352 fabric_fim-1.5.0b4/fim/slivers/README.md
--rw-r--r--   0        0        0      217 2021-06-14 18:36:21.931262 fabric_fim-1.5.0b4/fim/slivers/__init__.py
--rw-r--r--   0        0        0     3641 2023-02-02 01:41:56.410512 fabric_fim-1.5.0b4/fim/slivers/attached_components.py
--rw-r--r--   0        0        0    13021 2023-02-02 01:41:56.411041 fabric_fim-1.5.0b4/fim/slivers/base_sliver.py
--rw-r--r--   0        0        0    24182 2023-05-10 14:54:24.198919 fabric_fim-1.5.0b4/fim/slivers/capacities_labels.py
--rw-r--r--   0        0        0    11537 2023-05-10 14:54:24.200146 fabric_fim-1.5.0b4/fim/slivers/component_catalog.py
--rw-r--r--   0        0        0        1 2021-03-03 19:57:54.291739 fabric_fim-1.5.0b4/fim/slivers/data/__init__.py
--rw-r--r--   0        0        0     1691 2023-05-10 14:54:24.202981 fabric_fim-1.5.0b4/fim/slivers/data/component_catalog.json
--rw-r--r--   0        0        0    76943 2022-09-10 21:18:41.714675 fabric_fim-1.5.0b4/fim/slivers/data/instance_sizes.json
--rw-r--r--   0        0        0    23524 2022-02-18 19:27:15.591229 fabric_fim-1.5.0b4/fim/slivers/delegations.py
--rw-r--r--   0        0        0     3593 2022-02-18 19:27:15.591744 fabric_fim-1.5.0b4/fim/slivers/gateway.py
--rw-r--r--   0        0        0      919 2021-06-29 20:04:13.972162 fabric_fim-1.5.0b4/fim/slivers/identifiers.py
--rw-r--r--   0        0        0     3444 2022-02-18 19:27:15.592250 fabric_fim-1.5.0b4/fim/slivers/instance_catalog.py
--rw-r--r--   0        0        0     3225 2023-02-02 01:41:56.413360 fabric_fim-1.5.0b4/fim/slivers/interface_info.py
--rw-r--r--   0        0        0     2702 2021-09-22 14:46:40.423027 fabric_fim-1.5.0b4/fim/slivers/json.py
--rw-r--r--   0        0        0     3869 2023-02-02 01:41:56.413720 fabric_fim-1.5.0b4/fim/slivers/json_data.py
--rw-r--r--   0        0        0     5983 2023-02-02 01:41:56.414203 fabric_fim-1.5.0b4/fim/slivers/maintenance_mode.py
--rw-r--r--   0        0        0     1566 2021-03-03 19:57:54.294274 fabric_fim-1.5.0b4/fim/slivers/network_attached_storage.py
--rw-r--r--   0        0        0     3910 2023-02-02 01:41:56.414662 fabric_fim-1.5.0b4/fim/slivers/network_link.py
--rw-r--r--   0        0        0    10209 2023-02-02 01:41:56.415082 fabric_fim-1.5.0b4/fim/slivers/network_node.py
--rw-r--r--   0        0        0    22026 2023-05-10 14:54:24.204710 fabric_fim-1.5.0b4/fim/slivers/network_service.py
--rw-r--r--   0        0        0     6795 2021-06-04 19:43:14.993329 fabric_fim-1.5.0b4/fim/slivers/path_info.py
--rw-r--r--   0        0        0     3024 2022-02-18 19:27:15.594931 fabric_fim-1.5.0b4/fim/slivers/tags.py
--rw-r--r--   0        0        0     2622 2023-02-02 01:41:56.416090 fabric_fim-1.5.0b4/fim/slivers/topology_diff.py
--rw-r--r--   0        0        0     8706 2022-02-18 19:27:15.595505 fabric_fim-1.5.0b4/fim/user/README.md
--rw-r--r--   0        0        0     1914 2023-02-02 01:41:56.417286 fabric_fim-1.5.0b4/fim/user/__init__.py
--rw-r--r--   0        0        0    11730 2022-09-10 21:18:41.716394 fabric_fim-1.5.0b4/fim/user/component.py
--rw-r--r--   0        0        0     5668 2022-09-10 21:18:41.716675 fabric_fim-1.5.0b4/fim/user/composite_node.py
--rw-r--r--   0        0        0     7660 2023-02-02 01:41:56.418568 fabric_fim-1.5.0b4/fim/user/interface.py
--rw-r--r--   0        0        0     8381 2022-09-10 21:18:41.717280 fabric_fim-1.5.0b4/fim/user/link.py
--rw-r--r--   0        0        0     1219 2021-03-03 19:57:54.300001 fabric_fim-1.5.0b4/fim/user/measurement.py
--rw-r--r--   0        0        0     9668 2023-04-05 18:48:29.319327 fabric_fim-1.5.0b4/fim/user/model_element.py
--rw-r--r--   0        0        0    29219 2023-05-10 14:54:24.206616 fabric_fim-1.5.0b4/fim/user/network_service.py
--rw-r--r--   0        0        0    22636 2023-02-14 21:58:39.970039 fabric_fim-1.5.0b4/fim/user/node.py
--rw-r--r--   0        0        0    58158 2023-02-14 21:58:39.970995 fabric_fim-1.5.0b4/fim/user/topology.py
--rw-r--r--   0        0        0        2 2023-05-10 15:46:29.821869 fabric_fim-1.5.0b4/fim/util/__init__.py
--rw-r--r--   0        0        0    14139 2023-05-10 19:21:51.713927 fabric_fim-1.5.0b4/fim/util/fim_util.py
--rwxr-xr-x   0        0        0      480 2020-10-01 22:44:51.231545 fabric_fim-1.5.0b4/fim/util/load_graphs.sh
--rwxr-xr-x   0        0        0      316 2023-03-01 03:21:45.408058 fabric_fim-1.5.0b4/fim/util/merge_dev.sh
--rwxr-xr-x   0        0        0      563 2023-02-10 01:56:08.037222 fabric_fim-1.5.0b4/fim/util/merge_production.sh
--rwxr-xr-x   0        0        0      258 2020-10-09 19:51:30.191532 fabric_fim-1.5.0b4/fim/util/test_ws.bash
--rw-r--r--   0        0        0      595 2021-03-13 20:40:37.643107 fabric_fim-1.5.0b4/fim/view_only_dict.py
--rw-r--r--   0        0        0        0 2023-02-02 01:41:56.421372 fabric_fim-1.5.0b4/neo4j/data/.empty
--rw-r--r--   0        0        0        0 2023-02-02 01:41:56.421489 fabric_fim-1.5.0b4/neo4j/imports/.empty
--rw-r--r--   0        0        0      812 2023-05-10 18:56:39.987355 fabric_fim-1.5.0b4/pyproject.toml
--rw-r--r--   0        0        0      130 2023-05-10 18:36:12.072054 fabric_fim-1.5.0b4/requirements.txt
--rw-r--r--   0        0        0     4632 2022-03-09 00:58:31.583145 fabric_fim-1.5.0b4/test/ad_topology_test.py
--rw-r--r--   0        0        0     4834 2022-09-10 21:18:41.719406 fabric_fim-1.5.0b4/test/after.graphml
--rw-r--r--   0        0        0    17201 2023-02-02 01:41:56.423227 fabric_fim-1.5.0b4/test/attribute_collector_test.py
--rw-r--r--   0        0        0     4696 2022-09-10 21:18:41.719615 fabric_fim-1.5.0b4/test/before.graphml
--rw-r--r--   0        0        0     2729 2022-09-10 21:18:41.719876 fabric_fim-1.5.0b4/test/catalog_test.py
--rw-r--r--   0        0        0     4319 2022-02-18 19:27:15.602412 fabric_fim-1.5.0b4/test/delegation_label_test.py
--rw-r--r--   0        0        0     1653 2023-02-02 01:41:56.423551 fabric_fim-1.5.0b4/test/maintenance_test.py
--rw-r--r--   0        0        0    51613 2023-05-10 17:34:04.562843 fabric_fim-1.5.0b4/test/models/advertised_topo.graphml
--rw-r--r--   0        0        0    49696 2023-05-10 17:34:04.565992 fabric_fim-1.5.0b4/test/models/graph-template.graphml
--rw-r--r--   0        0        0    82994 2023-05-10 17:34:04.568753 fabric_fim-1.5.0b4/test/models/network-am-ad.graphml
--rw-r--r--   0        0        0    57411 2023-05-10 17:34:04.571919 fabric_fim-1.5.0b4/test/models/site-2-am-1broker-ad.graphml
--rw-r--r--   0        0        0    52887 2023-05-10 17:34:04.574274 fabric_fim-1.5.0b4/test/models/site-3-am-1broker-ad.graphml
--rw-r--r--   0        0        0   131407 2023-05-10 17:34:04.575177 fabric_fim-1.5.0b4/test/models/site-am-2broker-ad.graphml
--rw-r--r--   0        0        0    17363 2023-05-10 14:57:53.569975 fabric_fim-1.5.0b4/test/modify_test.py
--rw-r--r--   0        0        0    13135 2021-05-23 19:50:30.753072 fabric_fim-1.5.0b4/test/networkxx_pg_disjoint_test.py
--rw-r--r--   0        0        0    14091 2021-05-23 19:50:30.753595 fabric_fim-1.5.0b4/test/networkxx_pg_test.py
--rw-r--r--   0        0        0     2572 2021-03-24 00:18:51.064667 fabric_fim-1.5.0b4/test/pluggable_test.py
--rw-r--r--   0        0        0    42433 2023-05-10 14:57:53.570145 fabric_fim-1.5.0b4/test/slice_topology_test.py
--rw-r--r--   0        0        0     1869 2022-04-27 22:22:19.322857 fabric_fim-1.5.0b4/test/sliver_json_test.py
--rw-r--r--   0        0        0     5604 2023-05-10 14:54:24.209787 fabric_fim-1.5.0b4/test/sliver_test.py
--rw-r--r--   0        0        0    97162 2023-02-02 01:41:56.427682 fabric_fim-1.5.0b4/test/substrate_topology_test.py
--rw-r--r--   0        0        0      654 2022-02-18 19:27:15.604787 fabric_fim-1.5.0b4/test/test_load.py
--rw-r--r--   0        0        0     2362 2022-02-18 19:27:15.605244 fabric_fim-1.5.0b4/test/tuple_test.py
--rw-r--r--   0        0        0    15663 2023-05-10 14:57:53.570342 fabric_fim-1.5.0b4/test/zz_neo4j_pg_test.py
--rw-r--r--   0        0        0    11872 1970-01-01 00:00:00.000000 fabric_fim-1.5.0b4/PKG-INFO
+-rw-r--r--   0        0        0     2208 2023-06-15 15:30:40.226765 fabric_fim-1.5.1/.gitignore
+-rw-r--r--   0        0        0       26 2020-07-24 21:42:44.564662 fabric_fim-1.5.1/AUTHORS
+-rw-r--r--   0        0        0     1071 2020-07-14 22:09:49.459777 fabric_fim-1.5.1/LICENSE
+-rw-r--r--   0        0        0    11110 2023-06-15 15:20:12.737600 fabric_fim-1.5.1/README.md
+-rw-r--r--   0        0        0    18690 2021-05-25 21:09:37.024101 fabric_fim-1.5.1/figs/fim-structure.png
+-rw-r--r--   0        0        0      557 2021-03-15 22:13:52.784044 fabric_fim-1.5.1/fim/README.md
+-rw-r--r--   0        0        0      103 2023-06-15 15:24:42.351103 fabric_fim-1.5.1/fim/__init__.py
+-rw-r--r--   0        0        0        1 2022-04-27 22:22:19.299449 fabric_fim-1.5.1/fim/authz/__init__.py
+-rw-r--r--   0        0        0    16139 2023-02-02 01:41:56.403069 fabric_fim-1.5.1/fim/authz/attribute_collector.py
+-rw-r--r--   0        0        0      334 2020-09-12 23:24:52.369007 fabric_fim-1.5.1/fim/graph/README.md
+-rw-r--r--   0        0        0        1 2020-09-02 18:31:38.004468 fabric_fim-1.5.1/fim/graph/__init__.py
+-rw-r--r--   0        0        0    69843 2023-06-15 15:19:01.141154 fabric_fim-1.5.1/fim/graph/abc_property_graph.py
+-rw-r--r--   0        0        0     4093 2023-02-02 01:41:56.406333 fabric_fim-1.5.1/fim/graph/abc_property_graph_constants.py
+-rw-r--r--   0        0        0        1 2020-08-18 21:34:07.036009 fabric_fim-1.5.1/fim/graph/data/__init__.py
+-rw-r--r--   0        0        0      283 2020-09-03 22:10:53.500264 fabric_fim-1.5.1/fim/graph/data/capacity_types.json
+-rw-r--r--   0        0        0      100 2020-08-27 20:41:23.401941 fabric_fim-1.5.1/fim/graph/data/constraint_types.json
+-rw-r--r--   0        0        0     3886 2023-06-15 15:19:01.141376 fabric_fim-1.5.1/fim/graph/data/graph_validation_rules.json
+-rw-r--r--   0        0        0     3845 2023-06-15 15:19:01.141499 fabric_fim-1.5.1/fim/graph/data/graph_validation_rules_neo4j_v4.json
+-rw-r--r--   0        0        0      547 2020-09-03 22:10:39.822590 fabric_fim-1.5.1/fim/graph/data/label_types.json
+-rw-r--r--   0        0        0       91 2020-08-27 20:40:54.261031 fabric_fim-1.5.1/fim/graph/data/location_types.json
+-rw-r--r--   0        0        0      861 2023-05-10 14:54:24.189132 fabric_fim-1.5.1/fim/graph/data/neo4j_indexes.json
+-rw-r--r--   0        0        0     3320 2023-06-15 15:19:01.141615 fabric_fim-1.5.1/fim/graph/graph_util.py
+-rw-r--r--   0        0        0    44293 2023-06-15 15:19:01.154588 fabric_fim-1.5.1/fim/graph/neo4j_property_graph.py
+-rw-r--r--   0        0        0     6160 2022-10-06 17:38:08.214224 fabric_fim-1.5.1/fim/graph/networkx_mixin.py
+-rw-r--r--   0        0        0    42211 2023-06-15 15:19:01.141889 fabric_fim-1.5.1/fim/graph/networkx_property_graph.py
+-rw-r--r--   0        0        0     8354 2022-10-07 03:05:34.849246 fabric_fim-1.5.1/fim/graph/networkx_property_graph_disjoint.py
+-rw-r--r--   0        0        0     1501 2021-03-15 22:13:52.788626 fabric_fim-1.5.1/fim/graph/resources/README.md
+-rw-r--r--   0        0        0        1 2020-09-02 18:32:04.638774 fabric_fim-1.5.1/fim/graph/resources/__init__.py
+-rw-r--r--   0        0        0     4484 2021-05-25 21:09:37.029370 fabric_fim-1.5.1/fim/graph/resources/abc_adm.py
+-rw-r--r--   0        0        0    13570 2023-05-10 14:54:24.193783 fabric_fim-1.5.1/fim/graph/resources/abc_arm.py
+-rw-r--r--   0        0        0     2991 2022-02-18 19:27:15.586527 fabric_fim-1.5.1/fim/graph/resources/abc_bqm.py
+-rw-r--r--   0        0        0     4547 2021-03-31 01:14:29.518807 fabric_fim-1.5.1/fim/graph/resources/abc_cbm.py
+-rw-r--r--   0        0        0     2297 2021-03-07 22:42:30.018249 fabric_fim-1.5.1/fim/graph/resources/neo4j_adm.py
+-rw-r--r--   0        0        0     2106 2021-05-25 21:09:37.031668 fabric_fim-1.5.1/fim/graph/resources/neo4j_arm.py
+-rw-r--r--   0        0        0    18591 2023-06-15 15:19:01.148045 fabric_fim-1.5.1/fim/graph/resources/neo4j_cbm.py
+-rw-r--r--   0        0        0     5017 2022-02-18 19:27:15.587881 fabric_fim-1.5.1/fim/graph/resources/networkx_abqm.py
+-rw-r--r--   0        0        0     2341 2021-03-07 22:42:30.020154 fabric_fim-1.5.1/fim/graph/resources/networkx_adm.py
+-rw-r--r--   0        0        0     2122 2021-05-25 21:09:37.033196 fabric_fim-1.5.1/fim/graph/resources/networkx_arm.py
+-rw-r--r--   0        0        0      301 2021-03-15 22:13:52.789768 fabric_fim-1.5.1/fim/graph/slices/README.md
+-rw-r--r--   0        0        0        1 2020-09-02 18:32:24.788341 fabric_fim-1.5.1/fim/graph/slices/__init__.py
+-rw-r--r--   0        0        0     8223 2022-02-18 19:27:15.588460 fabric_fim-1.5.1/fim/graph/slices/abc_asm.py
+-rw-r--r--   0        0        0     3733 2023-05-10 14:54:24.196715 fabric_fim-1.5.1/fim/graph/slices/neo4j_asm.py
+-rw-r--r--   0        0        0     4298 2021-06-04 19:43:14.989790 fabric_fim-1.5.1/fim/graph/slices/networkx_asm.py
+-rw-r--r--   0        0        0     8615 2021-03-03 19:57:54.288231 fabric_fim-1.5.1/fim/graph/typed_tuples.py
+-rw-r--r--   0        0        0        0 2023-02-02 01:41:56.409002 fabric_fim-1.5.1/fim/logging/__init__.py
+-rw-r--r--   0        0        0     1526 2023-06-15 15:19:01.033709 fabric_fim-1.5.1/fim/logging/fim_logger.py
+-rw-r--r--   0        0        0     9071 2023-02-02 01:41:56.410072 fabric_fim-1.5.1/fim/logging/log_collector.py
+-rw-r--r--   0        0        0     9555 2021-03-24 00:18:51.063382 fabric_fim-1.5.1/fim/pluggable.py
+-rw-r--r--   0        0        0      189 2021-06-04 19:43:14.990352 fabric_fim-1.5.1/fim/slivers/README.md
+-rw-r--r--   0        0        0      217 2021-06-14 18:36:21.931262 fabric_fim-1.5.1/fim/slivers/__init__.py
+-rw-r--r--   0        0        0     3641 2023-02-02 01:41:56.410512 fabric_fim-1.5.1/fim/slivers/attached_components.py
+-rw-r--r--   0        0        0    13021 2023-02-02 01:41:56.411041 fabric_fim-1.5.1/fim/slivers/base_sliver.py
+-rw-r--r--   0        0        0    26010 2023-06-15 15:20:12.767056 fabric_fim-1.5.1/fim/slivers/capacities_labels.py
+-rw-r--r--   0        0        0    11537 2023-06-13 15:16:11.169736 fabric_fim-1.5.1/fim/slivers/component_catalog.py
+-rw-r--r--   0        0        0        1 2021-03-03 19:57:54.291739 fabric_fim-1.5.1/fim/slivers/data/__init__.py
+-rw-r--r--   0        0        0     1691 2023-05-10 14:54:24.202981 fabric_fim-1.5.1/fim/slivers/data/component_catalog.json
+-rw-r--r--   0        0        0    76943 2022-09-10 21:18:41.714675 fabric_fim-1.5.1/fim/slivers/data/instance_sizes.json
+-rw-r--r--   0        0        0    23524 2022-02-18 19:27:15.591229 fabric_fim-1.5.1/fim/slivers/delegations.py
+-rw-r--r--   0        0        0     3593 2022-02-18 19:27:15.591744 fabric_fim-1.5.1/fim/slivers/gateway.py
+-rw-r--r--   0        0        0      919 2021-06-29 20:04:13.972162 fabric_fim-1.5.1/fim/slivers/identifiers.py
+-rw-r--r--   0        0        0     3444 2022-02-18 19:27:15.592250 fabric_fim-1.5.1/fim/slivers/instance_catalog.py
+-rw-r--r--   0        0        0     3225 2023-02-02 01:41:56.413360 fabric_fim-1.5.1/fim/slivers/interface_info.py
+-rw-r--r--   0        0        0     2702 2021-09-22 14:46:40.423027 fabric_fim-1.5.1/fim/slivers/json.py
+-rw-r--r--   0        0        0     3869 2023-02-02 01:41:56.413720 fabric_fim-1.5.1/fim/slivers/json_data.py
+-rw-r--r--   0        0        0     5983 2023-02-02 01:41:56.414203 fabric_fim-1.5.1/fim/slivers/maintenance_mode.py
+-rw-r--r--   0        0        0     1566 2021-03-03 19:57:54.294274 fabric_fim-1.5.1/fim/slivers/network_attached_storage.py
+-rw-r--r--   0        0        0     3910 2023-02-02 01:41:56.414662 fabric_fim-1.5.1/fim/slivers/network_link.py
+-rw-r--r--   0        0        0    10209 2023-02-02 01:41:56.415082 fabric_fim-1.5.1/fim/slivers/network_node.py
+-rw-r--r--   0        0        0    22026 2023-05-10 14:54:24.204710 fabric_fim-1.5.1/fim/slivers/network_service.py
+-rw-r--r--   0        0        0     6795 2021-06-04 19:43:14.993329 fabric_fim-1.5.1/fim/slivers/path_info.py
+-rw-r--r--   0        0        0     3024 2022-02-18 19:27:15.594931 fabric_fim-1.5.1/fim/slivers/tags.py
+-rw-r--r--   0        0        0     2622 2023-02-02 01:41:56.416090 fabric_fim-1.5.1/fim/slivers/topology_diff.py
+-rw-r--r--   0        0        0     8706 2022-02-18 19:27:15.595505 fabric_fim-1.5.1/fim/user/README.md
+-rw-r--r--   0        0        0     1914 2023-02-02 01:41:56.417286 fabric_fim-1.5.1/fim/user/__init__.py
+-rw-r--r--   0        0        0    11730 2022-09-10 21:18:41.716394 fabric_fim-1.5.1/fim/user/component.py
+-rw-r--r--   0        0        0     5668 2022-09-10 21:18:41.716675 fabric_fim-1.5.1/fim/user/composite_node.py
+-rw-r--r--   0        0        0     7660 2023-02-02 01:41:56.418568 fabric_fim-1.5.1/fim/user/interface.py
+-rw-r--r--   0        0        0     8381 2022-09-10 21:18:41.717280 fabric_fim-1.5.1/fim/user/link.py
+-rw-r--r--   0        0        0     1219 2021-03-03 19:57:54.300001 fabric_fim-1.5.1/fim/user/measurement.py
+-rw-r--r--   0        0        0     9668 2023-04-05 18:48:29.319327 fabric_fim-1.5.1/fim/user/model_element.py
+-rw-r--r--   0        0        0    29219 2023-05-10 14:54:24.206616 fabric_fim-1.5.1/fim/user/network_service.py
+-rw-r--r--   0        0        0    22636 2023-02-14 21:58:39.970039 fabric_fim-1.5.1/fim/user/node.py
+-rw-r--r--   0        0        0    58158 2023-06-01 15:42:31.904936 fabric_fim-1.5.1/fim/user/topology.py
+-rw-r--r--   0        0        0        2 2023-06-15 15:19:24.419545 fabric_fim-1.5.1/fim/util/__init__.py
+-rw-r--r--   0        0        0    14139 2023-06-15 15:20:12.712509 fabric_fim-1.5.1/fim/util/fim_util.py
+-rw-r--r--   0        0        0      595 2021-03-13 20:40:37.643107 fabric_fim-1.5.1/fim/view_only_dict.py
+-rw-r--r--   0        0        0        0 2023-02-02 01:41:56.421372 fabric_fim-1.5.1/neo4j/data/.empty
+-rw-r--r--   0        0        0        0 2023-02-02 01:41:56.421489 fabric_fim-1.5.1/neo4j/imports/.empty
+-rw-r--r--   0        0        0      863 2023-06-15 15:20:12.720926 fabric_fim-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4632 2022-03-09 00:58:31.583145 fabric_fim-1.5.1/test/ad_topology_test.py
+-rw-r--r--   0        0        0     4834 2022-09-10 21:18:41.719406 fabric_fim-1.5.1/test/after.graphml
+-rw-r--r--   0        0        0    17550 2023-06-15 15:20:12.731835 fabric_fim-1.5.1/test/attribute_collector_test.py
+-rw-r--r--   0        0        0     4696 2022-09-10 21:18:41.719615 fabric_fim-1.5.1/test/before.graphml
+-rw-r--r--   0        0        0     2729 2022-09-10 21:18:41.719876 fabric_fim-1.5.1/test/catalog_test.py
+-rw-r--r--   0        0        0     4319 2022-02-18 19:27:15.602412 fabric_fim-1.5.1/test/delegation_label_test.py
+-rw-r--r--   0        0        0     1653 2023-02-02 01:41:56.423551 fabric_fim-1.5.1/test/maintenance_test.py
+-rw-r--r--   0        0        0    51613 2023-05-10 17:34:04.562843 fabric_fim-1.5.1/test/models/advertised_topo.graphml
+-rw-r--r--   0        0        0    49696 2023-05-10 17:34:04.565992 fabric_fim-1.5.1/test/models/graph-template.graphml
+-rw-r--r--   0        0        0    82994 2023-05-10 17:34:04.568753 fabric_fim-1.5.1/test/models/network-am-ad.graphml
+-rw-r--r--   0        0        0    57411 2023-05-10 17:34:04.571919 fabric_fim-1.5.1/test/models/site-2-am-1broker-ad.graphml
+-rw-r--r--   0        0        0    52887 2023-05-10 17:34:04.574274 fabric_fim-1.5.1/test/models/site-3-am-1broker-ad.graphml
+-rw-r--r--   0        0        0   131407 2023-05-10 17:34:04.575177 fabric_fim-1.5.1/test/models/site-am-2broker-ad.graphml
+-rw-r--r--   0        0        0    17363 2023-06-15 15:19:01.186506 fabric_fim-1.5.1/test/modify_test.py
+-rw-r--r--   0        0        0    13135 2021-05-23 19:50:30.753072 fabric_fim-1.5.1/test/networkxx_pg_disjoint_test.py
+-rw-r--r--   0        0        0    14091 2021-05-23 19:50:30.753595 fabric_fim-1.5.1/test/networkxx_pg_test.py
+-rw-r--r--   0        0        0     2572 2021-03-24 00:18:51.064667 fabric_fim-1.5.1/test/pluggable_test.py
+-rw-r--r--   0        0        0    42428 2023-06-15 15:20:12.777803 fabric_fim-1.5.1/test/slice_topology_test.py
+-rw-r--r--   0        0        0     1869 2022-04-27 22:22:19.322857 fabric_fim-1.5.1/test/sliver_json_test.py
+-rw-r--r--   0        0        0     6030 2023-06-15 15:20:12.763581 fabric_fim-1.5.1/test/sliver_test.py
+-rw-r--r--   0        0        0    97162 2023-02-02 01:41:56.427682 fabric_fim-1.5.1/test/substrate_topology_test.py
+-rw-r--r--   0        0        0      654 2022-02-18 19:27:15.604787 fabric_fim-1.5.1/test/test_load.py
+-rw-r--r--   0        0        0     2362 2022-02-18 19:27:15.605244 fabric_fim-1.5.1/test/tuple_test.py
+-rw-r--r--   0        0        0    15663 2023-06-15 15:19:01.186763 fabric_fim-1.5.1/test/zz_neo4j_pg_test.py
+-rw-r--r--   0        0        0    11890 1970-01-01 00:00:00.000000 fabric_fim-1.5.1/PKG-INFO
```

### Comparing `fabric_fim-1.5.0b4/.gitignore` & `fabric_fim-1.5.1/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -143,11 +143,13 @@
 /single-site.cyt.json
 /single-site.json
 /two-site.cyt.json
 /two-site.json
 /neo4j/data/databases/
 /neo4j/data/dbms/
 /neo4j/data/transactions/
+/neo4j/imports
 fim/util/*.graphml
 fim/util/*.yaml
 fim/util/*.json
 fim/util/*.JSON
+fim/util/*.sh
```

### Comparing `fabric_fim-1.5.0b4/LICENSE` & `fabric_fim-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/README.md` & `fabric_fim-1.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -163,20 +163,20 @@
 ```console
 $ pytest [-s] test
 ```
 
 This will produce substrate ARM models and save them into file in project root folder.
 
 To build and publish run 
-```commandline
+```console
 $ flit build
 $ flit publish
 ```
 or just (assuming your .pypirc is setup with the token to access PyPi)
-```commandline
+```console
 $ flit publish
 ```
 
 ## Graph validation
 
 All graphs loaded into Neo4j (whether from files or being passed in as part of query or delegation) 
 must conform to a set of rules expressed as Cypher queries. The basic set of rules for all 
@@ -184,15 +184,15 @@
 
 Prior to ingestion graphs are also tested on general syntax validity of JSON-formatted fields.  
 
 Additional rule files specific to model types may govern the validity of specific models.
 
 NetworkX-based graphs also undergo validation, but more limited in scope due to lack of tools.
 
-## Using fim_util.py utility
+## Using fim_util utility
 
 The utility supports a number of operations on GraphML files - enumerating nodes (for graphs)
 coming out of yEd, loading into an instance of Neo4j, deleting graphs from Neo4j.
 
 Start the appropriate version of [Neo4j-APOC docker container](https://github.com/fabric-testbed/fabric-docker-images/tree/master/neo4j-apoc)
 
 Create fim_config.yaml with the following structure under `util/`:
@@ -206,19 +206,19 @@
   import_dir: /imports
 ```
 Parameters `password` and `import_host_dir` depend on how the Docker container is started in
 the procedure above. Other parameters should remain unchanged from what is shown. 
 
 Run the utility for detailed help for the various operations:
 ```
-(infomodel) $ python fim_util.py -h
+(infomodel) $ fim_util -h
 ```
 
-Generally the utility is good for e.g. loading a graph file: `python fim_util.py -l -f -r <graphml file>` or
-merging multiple advertisements: `python fim_util.py -m -f <file1> -f <file2>`. Most options take multiple `-f`
+Generally the utility is good for e.g. loading a graph file: `fim_util -l -f -r <graphml file>` or
+merging multiple advertisements: `fim_util -m -f <file1> -f <file2>`. Most options take multiple `-f`
 and related options so can e.g. load multiple files at once.
 
 When testing large graphs, note that by default Neo4j visualizes the first 300 nodes in a browser. If you
 want to see a full graph, increase this limit (at neo4j prompt):
 ```
 :config initialNodeDisplay: 5000
 ```
```

### Comparing `fabric_fim-1.5.0b4/figs/fim-structure.png` & `fabric_fim-1.5.1/figs/fim-structure.png`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/README.md` & `fabric_fim-1.5.1/fim/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/authz/attribute_collector.py` & `fabric_fim-1.5.1/fim/authz/attribute_collector.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/abc_property_graph.py` & `fabric_fim-1.5.1/fim/graph/abc_property_graph.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/abc_property_graph_constants.py` & `fabric_fim-1.5.1/fim/graph/abc_property_graph_constants.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/data/graph_validation_rules.json` & `fabric_fim-1.5.1/fim/graph/data/graph_validation_rules.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/data/graph_validation_rules_neo4j_v4.json` & `fabric_fim-1.5.1/fim/graph/data/graph_validation_rules_neo4j_v4.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/data/label_types.json` & `fabric_fim-1.5.1/fim/graph/data/label_types.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/data/neo4j_indexes.json` & `fabric_fim-1.5.1/fim/graph/data/neo4j_indexes.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/graph_util.py` & `fabric_fim-1.5.1/fim/graph/graph_util.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/neo4j_property_graph.py` & `fabric_fim-1.5.1/fim/graph/neo4j_property_graph.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/networkx_mixin.py` & `fabric_fim-1.5.1/fim/graph/networkx_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/networkx_property_graph.py` & `fabric_fim-1.5.1/fim/graph/networkx_property_graph.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/networkx_property_graph_disjoint.py` & `fabric_fim-1.5.1/fim/graph/networkx_property_graph_disjoint.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/resources/README.md` & `fabric_fim-1.5.1/fim/graph/resources/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/resources/abc_adm.py` & `fabric_fim-1.5.1/fim/graph/resources/abc_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/resources/abc_arm.py` & `fabric_fim-1.5.1/fim/graph/resources/abc_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/resources/abc_bqm.py` & `fabric_fim-1.5.1/fim/graph/resources/abc_bqm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/resources/abc_cbm.py` & `fabric_fim-1.5.1/fim/graph/resources/abc_cbm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/resources/neo4j_adm.py` & `fabric_fim-1.5.1/fim/graph/resources/neo4j_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/resources/neo4j_arm.py` & `fabric_fim-1.5.1/fim/graph/resources/neo4j_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/resources/neo4j_cbm.py` & `fabric_fim-1.5.1/fim/graph/resources/neo4j_cbm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/resources/networkx_abqm.py` & `fabric_fim-1.5.1/fim/graph/resources/networkx_abqm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/resources/networkx_adm.py` & `fabric_fim-1.5.1/fim/graph/resources/networkx_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/resources/networkx_arm.py` & `fabric_fim-1.5.1/fim/graph/resources/networkx_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/slices/abc_asm.py` & `fabric_fim-1.5.1/fim/graph/slices/abc_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/slices/neo4j_asm.py` & `fabric_fim-1.5.1/fim/graph/slices/neo4j_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/slices/networkx_asm.py` & `fabric_fim-1.5.1/fim/graph/slices/networkx_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/graph/typed_tuples.py` & `fabric_fim-1.5.1/fim/graph/typed_tuples.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/logging/log_collector.py` & `fabric_fim-1.5.1/fim/logging/log_collector.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/pluggable.py` & `fabric_fim-1.5.1/fim/pluggable.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/slivers/attached_components.py` & `fabric_fim-1.5.1/fim/slivers/attached_components.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/slivers/base_sliver.py` & `fabric_fim-1.5.1/fim/slivers/base_sliver.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/slivers/capacities_labels.py` & `fabric_fim-1.5.1/fim/slivers/capacities_labels.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 from abc import ABC, abstractmethod
 
 import requests
 import urllib.parse
 
 from fim.graph.abc_property_graph_constants import ABCPropertyGraphConstants
-
+import fim.logging.fim_logger as fl
 
 class JSONField(ABC):
 
     @classmethod
     def update(cls, lab, **kwargs):
         """
         quasi-copy constructor if kwargs are ommitted,
@@ -52,15 +52,15 @@
         inst = lab.__class__()
         for k, v in lab.__dict__.items():
             inst.__setattr__(k, v)
         inst._set_fields(**kwargs)
         return inst
 
     @abstractmethod
-    def _set_fields(self, **kwargs):
+    def _set_fields(self, forgiving=False, **kwargs):
         """
         Abstract private set_fields method
         :param kwargs:
         :return:
         """
 
     def to_json(self) -> str:
@@ -85,15 +85,17 @@
         :param json_string:
         :return: object
         """
         if json_string is None or len(json_string) == 0 or json_string == ABCPropertyGraphConstants.NEO4j_NONE:
             return None
         d = json.loads(json_string)
         ret = cls()
-        ret._set_fields(**d)
+        # we make constructing from JSON more forgiving to allow some limited
+        # forward compatibility, in case the fields change
+        ret._set_fields(forgiving=True, **d)
         return ret
 
     def to_dict(self) -> Dict[str, str] or None:
         """
         Convert to a dictionary skipping empty fields. Returns None
         if all fields are empty
         :return:
@@ -136,15 +138,15 @@
         self.disk = 0
         self.bw = 0
         self.burst_size = 0
         self.unit = 0
         self.mtu = 0
         self._set_fields(**kwargs)
 
-    def _set_fields(self, **kwargs):
+    def _set_fields(self, forgiving=False, **kwargs):
         """
         Universal integer setter for all fields.
         Values should be non-negative integers. Throws a CapacityException
         if you try to set a non-existent field.
         :param kwargs:
         :return: self to support call chaining
         """
@@ -153,16 +155,20 @@
                 assert v >= 0
                 assert isinstance(v, int)
             try:
                 # will toss an exception if field is not defined
                 self.__getattribute__(k)
                 self.__setattr__(k, v)
             except AttributeError:
-                raise CapacityException(f"Unable to set field {k} of capacity, no such field available "
-                                        f"{[k for k in self.__dict__.keys()]}")
+                report = f"Unable to set field {k} of capacity, no such field available "\
+                       f"{[k for k in self.__dict__.keys()]}"
+                if forgiving:
+                    fl.get_logger().warning(report)
+                else:
+                    raise CapacityException(report)
         return self
 
     def __add__(self, other):
         assert isinstance(other, Capacities)
         ret = Capacities()
         for f, v in self.__dict__.items():
             ret.__dict__[f] = self.__dict__[f] + other.__dict__[f]
@@ -193,15 +199,19 @@
         return True
 
     def __eq__(self, other):
         if not other:
             return False
         assert isinstance(other, Capacities)
         for f, v in self.__dict__.items():
-            if v != other.__dict__[f]:
+            # since we may be dealing with pickled versions
+            # of Capcities created with older version of FIM
+            # need to be careful not to assume all the same
+            # fields are present
+            if v != other.__dict__.get(f, 0):
                 return False
         return True
 
     def negative_fields(self) -> List[str]:
         """
         returns list of fields that are negative
         :return:
@@ -282,30 +292,34 @@
     e.g. an instance size name. They have to be mappable to actual capacities
     via e.g. a catalog.
     """
     def __init__(self, **kwargs):
         self.instance_type = None
         self._set_fields(**kwargs)
 
-    def _set_fields(self, **kwargs):
+    def _set_fields(self, forgiving=False, **kwargs):
         """
         Universal setter for all fields. Values should be strings.
         Throws a LabelException if you try to set a non-existent field.
         :param kwargs:
         :return: self to support call chaining
         """
         for k, v in kwargs.items():
             assert v is not None  # could be strings
             assert isinstance(v, str)
             try:
                 # will toss an exception if field is not defined
                 self.__getattribute__(k)
                 self.__setattr__(k, v)
             except AttributeError:
-                raise CapacityHintException(f"Unable to set field {k} of capacity hints, no such field available")
+                report = f"Unable to set field {k} of capacity hints, no such field available"
+                if forgiving:
+                    fl.get_logger().warning(report)
+                else:
+                    raise CapacityHintException(report)
         # to support call chaining
         return self
 
     def __add__(self, other):
         assert isinstance(other, Labels)
         raise RuntimeError("Not Implemented")
 
@@ -361,15 +375,16 @@
     LAMBDA_VALIDATORS = {
         'vlan': ((lambda v: True if 0 <= int(v) <= 4096 else False), "0-4096"),
         'inner_vlan': ((lambda v: True if 0 <= int(v) <= 4096 else False), "0-4096"),
         'vlan_range': ((lambda v: True if 0 <= int(v.split('-')[0]) <= 4096 and
                                           0 <= int(v.split('-')[1]) <= 4096 and
                                           int(v.split('-')[0]) <= int(v.split('-')[1]) else False),
                        "0-4096"),
-        'asn': ((lambda a: True if 0 < int(a) < 2**32 else False), "1-4294967295")
+        'asn': ((lambda a: True if 0 < int(a) < 2**32 else False), "1-4294967295"),
+        'numa': ((lambda a: True if -1 <= int(a) < 8 else False), "-1 or 0-7")
     }
 
     def __init__(self, **kwargs):
         self.bdf = None
         self.mac = None
         self.ipv4 = None
         self.ipv4_range = None
@@ -386,17 +401,18 @@
         self.local_name = None
         self.local_type = None
         self.device_name = None
         self.bgp_key = None
         self.account_id = None
         self.region = None
         self.usb_id = None
+        self.numa = None
         self._set_fields(**kwargs)
 
-    def _set_fields(self, **kwargs):
+    def _set_fields(self, forgiving=False, **kwargs):
         """
         Universal setter for all fields. Values should be strings or lists of strings.
         Throws a LabelException if you try to set a non-existent field.
         :param kwargs:
         :return: self to support call chaining
         """
         for k, v in kwargs.items():
@@ -430,16 +446,20 @@
                         res = self.LAMBDA_VALIDATORS[k][0](v)
                         if res is False:
                             raise LabelException(f'Provided label value {v} for {k} must be in a valid '
                                                  f'range {self.LAMBDA_VALIDATORS[k][1]}')
 
                 self.__setattr__(k, v)
             except AttributeError:
-                raise LabelException(f"Unable to set field {k} of labels, no such field available "
-                                     f"{[k for k in self.__dict__.keys()]}")
+                report = f"Using logger {fl.get_logger()} Unable to set field {k} of labels, no such field available "\
+                         f"{[k for k in self.__dict__.keys()]}"
+                if forgiving:
+                    fl.get_logger().warning(report)
+                else:
+                    raise LabelException(report)
         # to support call chaining
         return self
 
     def __add__(self, other):
         assert isinstance(other, Labels)
         # FIXME: does ADD mean finding a union of label sets per type?
         raise RuntimeError("Not Implemented")
@@ -457,15 +477,19 @@
         return ret[:-2] + "}"
 
     def __eq__(self, other):
         if not other:
             return False
         assert isinstance(other, Labels)
         for f, v in self.__dict__.items():
-            if v != other.__dict__[f]:
+            # since we may be dealing with pickled versions
+            # of Labels created with older version of FIM
+            # need to be careful not to assume all the same
+            # fields are present
+            if v != other.__dict__.get(f):
                 return False
         return True
 
 
 class ReservationInfo(JSONField):
     """
     Reservation info structure for ASM sliver objects
@@ -473,31 +497,35 @@
 
     def __init__(self, **kwargs):
         self.reservation_id = None
         self.reservation_state = None
         self.error_message = None
         self._set_fields(**kwargs)
 
-    def _set_fields(self, **kwargs):
+    def _set_fields(self, forgiving=False, **kwargs):
         """
         Universal setter for all fields. Values should be strings or lists of strings.
         Throws a ReservationInfoException if you try to set a non-existent field.
         :param kwargs:
         :return: self to support call chaining
         """
         for k, v in kwargs.items():
             assert v is not None  # could be strings or lists of strings
             assert isinstance(v, str) or isinstance(v, list)
             try:
                 # will toss an exception if field is not defined
                 self.__getattribute__(k)
                 self.__setattr__(k, v)
             except AttributeError:
-                raise ReservationInfoException(f"Unable to set field {k} of reservation info, no such field "
-                                               f"available {[k for k in self.__dict__.keys()]}")
+                report = f"Unable to set field {k} of reservation info, no such field "\
+                         f"available {[k for k in self.__dict__.keys()]}"
+                if forgiving:
+                    fl.get_logger().warning(report)
+                else:
+                    raise ReservationInfoException(report)
         # to support call chaining
         return self
 
 
 class StructuralInfo(JSONField):
     """
     Structural info on the for sliver objects (things like - is it a stitching node,
@@ -505,57 +533,65 @@
     """
     def __init__(self, **kwargs):
         self.sub_graph_id = None
         self.parent_graph_id = None
         self.adm_graph_ids = None
         self._set_fields(**kwargs)
 
-    def _set_fields(self, **kwargs):
+    def _set_fields(self, forgiving=False, **kwargs):
         """
         Universal setter for all fields. Values are strings or boolean.
         Throws a
         :param kwargs:
         :return:
         """
         for k, v in kwargs.items():
             assert v is not None  # could be strings or lists of strings
             assert isinstance(v, str) or isinstance(v, list)
             try:
                 # will toss an exception if field is not defined
                 self.__getattribute__(k)
                 self.__setattr__(k, v)
             except AttributeError:
-                raise StructuralInfoException(f"Unable to set field {k} of structural info, no such field available")
+                report = f"Unable to set field {k} of structural info, no such field available"
+                if forgiving:
+                    fl.get_logger().warning(report)
+                else:
+                    raise StructuralInfoException(report)
         # to support call chaining
         return self
 
 
 class Location(JSONField):
     """
     Location representation (as address, coordinates or any other useful way)
     """
     def __init__(self, **kwargs):
         self.postal = None
         self._set_fields(**kwargs)
 
-    def _set_fields(self, **kwargs):
+    def _set_fields(self, forgiving=False, **kwargs):
         """
         Universal setter for location fields. Values are strings.
         :param kwargs:
         :return:
         """
         for k, v in kwargs.items():
             assert v is not None
             assert isinstance(v, str)
             try:
                 # will throw exception if field is not defined
                 self.__getattribute__(k)
                 self.__setattr__(k, v)
             except AttributeError:
-                raise LocationException(f"Unable to set field {k} of location, no such field available")
+                report = f"Unable to set field {k} of location, no such field available"
+                if forgiving:
+                    fl.get_logger().warning(report)
+                else:
+                    raise LocationException(report)
         return self
 
     def to_latlon(self) -> Tuple[float, float]:
         """
         Return a tuple of floats indicating Lat/Lon of the location. Uses Nomatim OpenStreetMaps
         service.
         :return:
@@ -586,24 +622,28 @@
     def __init__(self, **kwargs):
         self.auto_config = False # primarily for interfaces
         self.auto_mount = False # primarily for storage components
         self.ipv4_management = False # request ipv4 management IP
         self.ptp = False # for advertisements of nodes/sites
         self._set_fields(**kwargs)
 
-    def _set_fields(self, **kwargs):
+    def _set_fields(self, forgiving=False, **kwargs):
         for k, v in kwargs.items():
             assert v is not None
             assert isinstance(v, bool)
             try:
                 # will throw exception if field is not defined
                 self.__getattribute__(k)
                 self.__setattr__(k, v)
             except AttributeError:
-                raise FlagException(f"Unable to set field {k} of flags, no such field available")
+                report = f"Unable to set field {k} of flags, no such field available"
+                if forgiving:
+                    fl.get_logger().warning(report)
+                else:
+                    raise FlagException(report)
         return self
 
     def to_json(self) -> str:
         """
         Dumps to JSON the __dict__ of the instance. Be careful as the fields in this
         class should only be those that can be present in JSON output.
         Specialized for boolean values from the generic implementation in JSONFields
```

### Comparing `fabric_fim-1.5.0b4/fim/slivers/component_catalog.py` & `fabric_fim-1.5.1/fim/slivers/component_catalog.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/slivers/data/component_catalog.json` & `fabric_fim-1.5.1/fim/slivers/data/component_catalog.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/slivers/data/instance_sizes.json` & `fabric_fim-1.5.1/fim/slivers/data/instance_sizes.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/slivers/delegations.py` & `fabric_fim-1.5.1/fim/slivers/delegations.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/slivers/gateway.py` & `fabric_fim-1.5.1/fim/slivers/gateway.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/slivers/identifiers.py` & `fabric_fim-1.5.1/fim/slivers/identifiers.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/slivers/instance_catalog.py` & `fabric_fim-1.5.1/fim/slivers/instance_catalog.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/slivers/interface_info.py` & `fabric_fim-1.5.1/fim/slivers/interface_info.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/slivers/json.py` & `fabric_fim-1.5.1/fim/slivers/json.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/slivers/json_data.py` & `fabric_fim-1.5.1/fim/slivers/json_data.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/slivers/maintenance_mode.py` & `fabric_fim-1.5.1/fim/slivers/maintenance_mode.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/slivers/network_attached_storage.py` & `fabric_fim-1.5.1/fim/slivers/network_attached_storage.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/slivers/network_link.py` & `fabric_fim-1.5.1/fim/slivers/network_link.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/slivers/network_node.py` & `fabric_fim-1.5.1/fim/slivers/network_node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/slivers/network_service.py` & `fabric_fim-1.5.1/fim/slivers/network_service.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/slivers/path_info.py` & `fabric_fim-1.5.1/fim/slivers/path_info.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/slivers/tags.py` & `fabric_fim-1.5.1/fim/slivers/tags.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/slivers/topology_diff.py` & `fabric_fim-1.5.1/fim/slivers/topology_diff.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/user/README.md` & `fabric_fim-1.5.1/fim/user/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/user/__init__.py` & `fabric_fim-1.5.1/fim/user/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/user/component.py` & `fabric_fim-1.5.1/fim/user/component.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/user/composite_node.py` & `fabric_fim-1.5.1/fim/user/composite_node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/user/interface.py` & `fabric_fim-1.5.1/fim/user/interface.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/user/link.py` & `fabric_fim-1.5.1/fim/user/link.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/user/measurement.py` & `fabric_fim-1.5.1/fim/user/measurement.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/user/model_element.py` & `fabric_fim-1.5.1/fim/user/model_element.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/user/network_service.py` & `fabric_fim-1.5.1/fim/user/network_service.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/user/node.py` & `fabric_fim-1.5.1/fim/user/node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/user/topology.py` & `fabric_fim-1.5.1/fim/user/topology.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/util/fim_util.py` & `fabric_fim-1.5.1/fim/util/fim_util.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/fim/view_only_dict.py` & `fabric_fim-1.5.1/fim/view_only_dict.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/pyproject.toml` & `fabric_fim-1.5.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 		"Programming Language :: Python :: 3",
 		"Operating System :: OS Independent"]
 dynamic = ["version", "description"]
 requires-python = '>=3.9'
 keywords = ["Neo4j"]
 dependencies = [ 
 	"matplotlib >= 3.6.0",
-	"neo4j >= 5.2.0",
+	"neo4j >= 5.3.0",
 	"networkx >= 2.8.7",
 	"networkx_query >= 1.0.1",
 	"PyYAML >= 6.0",
 	"recordclass >= 0.17.5",
 	"requests >= 2.28.1",
 	"lxml >= 4.9.2"
 	]
@@ -29,7 +29,10 @@
 
 [project.urls]
 Home = "https://github.com/fabric-testbed/InformationModel"
 
 [tool.flit.module]
 name = "fim"
 
+[project.optional-dependencies]
+test = ["pytest"]
+
```

### Comparing `fabric_fim-1.5.0b4/test/ad_topology_test.py` & `fabric_fim-1.5.1/test/ad_topology_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/test/after.graphml` & `fabric_fim-1.5.1/test/after.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/test/attribute_collector_test.py` & `fabric_fim-1.5.1/test/attribute_collector_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,20 @@
         t = ExperimentTopology()
         n1 = t.add_node(name='n1', site='RENC', capacities=Capacities(core=1, ram=10, disk=25))
         c1 = n1.add_component(name='c1', model_type=ComponentModelType.SmartNIC_ConnectX_6)
         c2 = n1.add_component(name='c2', model_type=ComponentModelType.SharedNIC_ConnectX_6)
         n1.add_component(name='c3', model_type=ComponentModelType.NVME_P4510)
         n2 = t.add_node(name='n2', site='UKY', capacities=Capacities(core=10, ram=10, disk=35))
         c4 = n2.add_component(name='c4', model_type=ComponentModelType.SmartNIC_ConnectX_5)
+        c5 = n2.add_component(name='c5', model_type=ComponentModelType.FPGA_Xilinx_U280)
         s1 = t.add_network_service(name='s1', nstype=ServiceType.L2PTP,
                                    interfaces=[c1.interface_list[0], c4.interface_list[0]],
                                    capacities=Capacities(bw=12))
+        s2 = t.add_network_service(name='s2', nstype=ServiceType.L2Bridge,
+                                   interfaces=[c5.interface_list[0], c5.interface_list[1]])
         fac1 = t.add_facility(name='RENCI-DTN', site='RENC', capacities=Capacities(bw=10))
         sfac = t.add_network_service(name='s-fac', nstype=ServiceType.L2STS,
                                      interfaces=[fac1.interface_list[0],
                                                  c2.interface_list[0]])
         # this will take just about anything - an ASM, a Node, a NetworkService,
         # a sliver. So it can be called in AM, Broker or Orchestrator
         #
@@ -38,14 +41,15 @@
         # generally you also want to set the lifetime (provided externally)
         now = datetime.now(timezone.utc)
         delta = timedelta(days=13, hours=11, minutes=7, seconds=4, milliseconds=10)
         future = now + delta
         az.set_lifetime(future)
         print(az)
         self.assertTrue('SmartNIC' in az.attributes[ResourceAuthZAttributes.RESOURCE_COMPONENT])
+        self.assertTrue('FPGA' in az.attributes[ResourceAuthZAttributes.RESOURCE_COMPONENT])
         self.assertTrue('NVME' in az.attributes[ResourceAuthZAttributes.RESOURCE_COMPONENT])
         self.assertTrue(25 in az.attributes[ResourceAuthZAttributes.RESOURCE_DISK])
         self.assertTrue(12 in az.attributes[ResourceAuthZAttributes.RESOURCE_BW])
         self.assertTrue('RENC' in az.attributes[ResourceAuthZAttributes.RESOURCE_SITE])
         self.assertTrue('UKY' in az.attributes[ResourceAuthZAttributes.RESOURCE_SITE])
         self.assertTrue('P13DT11H7M4S' in az.attributes[ResourceAuthZAttributes.RESOURCE_LIFETIME])
         self.assertEqual(az.attributes[ResourceAuthZAttributes.RESOURCE_TYPE], ["sliver"])
```

### Comparing `fabric_fim-1.5.0b4/test/before.graphml` & `fabric_fim-1.5.1/test/before.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/test/catalog_test.py` & `fabric_fim-1.5.1/test/catalog_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/test/delegation_label_test.py` & `fabric_fim-1.5.1/test/delegation_label_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/test/maintenance_test.py` & `fabric_fim-1.5.1/test/maintenance_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/test/models/advertised_topo.graphml` & `fabric_fim-1.5.1/test/models/advertised_topo.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/test/models/graph-template.graphml` & `fabric_fim-1.5.1/test/models/graph-template.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/test/models/network-am-ad.graphml` & `fabric_fim-1.5.1/test/models/network-am-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/test/models/site-2-am-1broker-ad.graphml` & `fabric_fim-1.5.1/test/models/site-2-am-1broker-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/test/models/site-3-am-1broker-ad.graphml` & `fabric_fim-1.5.1/test/models/site-3-am-1broker-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/test/models/site-am-2broker-ad.graphml` & `fabric_fim-1.5.1/test/models/site-am-2broker-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/test/modify_test.py` & `fabric_fim-1.5.1/test/modify_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/test/networkxx_pg_disjoint_test.py` & `fabric_fim-1.5.1/test/networkxx_pg_disjoint_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/test/networkxx_pg_test.py` & `fabric_fim-1.5.1/test/networkxx_pg_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/test/pluggable_test.py` & `fabric_fim-1.5.1/test/pluggable_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/test/slice_topology_test.py` & `fabric_fim-1.5.1/test/slice_topology_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -502,15 +502,15 @@
         topo.add_node(name='n3', site='RENC')
         topo.nodes['n1'].add_component(model_type=f.ComponentModelType.SharedNIC_ConnectX_6, name='nic1')
         topo.nodes['n1'].add_component(model_type=f.ComponentModelType.NVME_P4510, name='drive1')
         topo.nodes['n2'].add_component(model_type=f.ComponentModelType.SmartNIC_ConnectX_6, name='nic1')
         topo.nodes['n2'].add_component(model_type=f.ComponentModelType.GPU_RTX6000, name='gpu1')
         topo.nodes['n3'].add_component(model_type=f.ComponentModelType.SmartNIC_ConnectX_5, name='nic1')
         topo.add_network_service(name='bridge1', nstype=f.ServiceType.L2Bridge,
-                                      interfaces=self.topo.interface_list)
+                                      interfaces=topo.interface_list)
         topo.serialize(file_name='single-site-neo4jimp.graphml')
         topo.validate()
 
     def testBasicTwoSiteSlice(self):
         # create a basic slice and export to GraphML and JSON
         self.topo.add_node(name='n1', site='RENC', ntype=f.NodeType.VM, capacities=Capacities(core=4))
         self.topo.add_node(name='n2', site='RENC')
```

### Comparing `fabric_fim-1.5.0b4/test/sliver_json_test.py` & `fabric_fim-1.5.1/test/sliver_json_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/test/sliver_test.py` & `fabric_fim-1.5.1/test/sliver_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,21 +87,35 @@
 
         with self.assertRaises(LabelException):
             Labels(vlan='4098')
 
         with self.assertRaises(LabelException):
             Labels(inner_vlan='6000')
 
+    def testNuma(self):
+        ns = NodeSliver()
+        cap_hint = CapacityHints(instance_type='blah')
+        lab = Labels(numa='-1')
+        ns.set_properties(labels=lab, capacity_hints=cap_hint)
+
+        self.assertEqual(ns.labels.numa, '-1')
+
+        with self.assertRaises(LabelException):
+            Labels(numa='-5')
+
+        with self.assertRaises(LabelException):
+            Labels(numa='8')
+
     def testLabelEq(self):
-        lab = Labels(vlan_range='1-4096', asn='123')
+        lab = Labels(vlan_range='1-4096', asn='123', numa='0')
         lab1 = Labels(vlan_range='1-1024', asn='345')
 
         self.assertNotEqual(lab, lab1)
 
-        lab2 = Labels(vlan_range='1-4096', asn='123')
+        lab2 = Labels(vlan_range='1-4096', asn='123', numa='0')
         self.assertEqual(lab, lab2)
 
         lab2 = Labels(vlan_range='1-4096', asn='123', local_name='myvlan')
         self.assertNotEqual(lab, lab2)
 
     def testFlagsAndTags(self):
         isl = InterfaceSliver()
```

### Comparing `fabric_fim-1.5.0b4/test/substrate_topology_test.py` & `fabric_fim-1.5.1/test/substrate_topology_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/test/test_load.py` & `fabric_fim-1.5.1/test/test_load.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/test/tuple_test.py` & `fabric_fim-1.5.1/test/tuple_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/test/zz_neo4j_pg_test.py` & `fabric_fim-1.5.1/test/zz_neo4j_pg_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.0b4/PKG-INFO` & `fabric_fim-1.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: fabric_fim
-Version: 1.5.0b4
+Version: 1.5.1
 Summary: FABRIC Information Model library and utilities
 Keywords: Neo4j
 Author-email: Ilya Baldin <ibaldin@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Dist: matplotlib >= 3.6.0
-Requires-Dist: neo4j >= 5.2.0
+Requires-Dist: neo4j >= 5.3.0
 Requires-Dist: networkx >= 2.8.7
 Requires-Dist: networkx_query >= 1.0.1
 Requires-Dist: PyYAML >= 6.0
 Requires-Dist: recordclass >= 0.17.5
 Requires-Dist: requests >= 2.28.1
 Requires-Dist: lxml >= 4.9.2
+Requires-Dist: pytest ; extra == "test"
 Project-URL: Home, https://github.com/fabric-testbed/InformationModel
+Provides-Extra: test
 
 [![PyPI](https://img.shields.io/pypi/v/fabric-fim?style=plastic)](https://pypi.org/project/fabric-fim/)
 
 # Information Model
 
 ## Basic Graph Abstractions
 
@@ -184,20 +186,20 @@
 ```console
 $ pytest [-s] test
 ```
 
 This will produce substrate ARM models and save them into file in project root folder.
 
 To build and publish run 
-```commandline
+```console
 $ flit build
 $ flit publish
 ```
 or just (assuming your .pypirc is setup with the token to access PyPi)
-```commandline
+```console
 $ flit publish
 ```
 
 ## Graph validation
 
 All graphs loaded into Neo4j (whether from files or being passed in as part of query or delegation) 
 must conform to a set of rules expressed as Cypher queries. The basic set of rules for all 
@@ -205,15 +207,15 @@
 
 Prior to ingestion graphs are also tested on general syntax validity of JSON-formatted fields.  
 
 Additional rule files specific to model types may govern the validity of specific models.
 
 NetworkX-based graphs also undergo validation, but more limited in scope due to lack of tools.
 
-## Using fim_util.py utility
+## Using fim_util utility
 
 The utility supports a number of operations on GraphML files - enumerating nodes (for graphs)
 coming out of yEd, loading into an instance of Neo4j, deleting graphs from Neo4j.
 
 Start the appropriate version of [Neo4j-APOC docker container](https://github.com/fabric-testbed/fabric-docker-images/tree/master/neo4j-apoc)
 
 Create fim_config.yaml with the following structure under `util/`:
@@ -227,19 +229,19 @@
   import_dir: /imports
 ```
 Parameters `password` and `import_host_dir` depend on how the Docker container is started in
 the procedure above. Other parameters should remain unchanged from what is shown. 
 
 Run the utility for detailed help for the various operations:
 ```
-(infomodel) $ python fim_util.py -h
+(infomodel) $ fim_util -h
 ```
 
-Generally the utility is good for e.g. loading a graph file: `python fim_util.py -l -f -r <graphml file>` or
-merging multiple advertisements: `python fim_util.py -m -f <file1> -f <file2>`. Most options take multiple `-f`
+Generally the utility is good for e.g. loading a graph file: `fim_util -l -f -r <graphml file>` or
+merging multiple advertisements: `fim_util -m -f <file1> -f <file2>`. Most options take multiple `-f`
 and related options so can e.g. load multiple files at once.
 
 When testing large graphs, note that by default Neo4j visualizes the first 300 nodes in a browser. If you
 want to see a full graph, increase this limit (at neo4j prompt):
 ```
 :config initialNodeDisplay: 5000
 ```
```

