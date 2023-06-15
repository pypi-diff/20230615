# Comparing `tmp/ccf-openapi-1.1.3.tar.gz` & `tmp/ccf-openapi-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccf-openapi-1.1.3.tar", last modified: Wed Jun 14 15:26:58 2023, max compression
+gzip compressed data, was "ccf-openapi-1.1.4.tar", last modified: Thu Jun 15 15:03:43 2023, max compression
```

## Comparing `ccf-openapi-1.1.3.tar` & `ccf-openapi-1.1.4.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-14 15:26:58.989572 ccf-openapi-1.1.3/
--rw-r--r--   0 bherr     (1000) bherr     (1000)      449 2023-06-14 15:26:58.989572 ccf-openapi-1.1.3/PKG-INFO
--rw-r--r--   0 bherr     (1000) bherr     (1000)     9274 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/README.md
-drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-14 15:26:58.969572 ccf-openapi-1.1.3/ccf_openapi.egg-info/
--rw-r--r--   0 bherr     (1000) bherr     (1000)      449 2023-06-14 15:26:58.000000 ccf-openapi-1.1.3/ccf_openapi.egg-info/PKG-INFO
--rw-r--r--   0 bherr     (1000) bherr     (1000)     2880 2023-06-14 15:26:58.000000 ccf-openapi-1.1.3/ccf_openapi.egg-info/SOURCES.txt
--rw-r--r--   0 bherr     (1000) bherr     (1000)        1 2023-06-14 15:26:58.000000 ccf-openapi-1.1.3/ccf_openapi.egg-info/dependency_links.txt
--rw-r--r--   0 bherr     (1000) bherr     (1000)       32 2023-06-14 15:26:58.000000 ccf-openapi-1.1.3/ccf_openapi.egg-info/requires.txt
--rw-r--r--   0 bherr     (1000) bherr     (1000)       19 2023-06-14 15:26:58.000000 ccf-openapi-1.1.3/ccf_openapi.egg-info/top_level.txt
-drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-14 15:26:58.979572 ccf-openapi-1.1.3/ccf_openapi_client/
--rw-r--r--   0 bherr     (1000) bherr     (1000)      850 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/__init__.py
-drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-14 15:26:58.979572 ccf-openapi-1.1.3/ccf_openapi_client/api/
--rw-r--r--   0 bherr     (1000) bherr     (1000)      222 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/api/__init__.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)   104876 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/api/default_api.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    37737 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/api_client.py
-drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-14 15:26:58.979572 ccf-openapi-1.1.3/ccf_openapi_client/apis/
--rw-r--r--   0 bherr     (1000) bherr     (1000)      471 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/apis/__init__.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    16559 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/configuration.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     5140 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/exceptions.py
-drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-14 15:26:58.979572 ccf-openapi-1.1.3/ccf_openapi_client/model/
--rw-r--r--   0 bherr     (1000) bherr     (1000)      348 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/__init__.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    11524 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/aggregate_count.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    12078 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/database_status.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    11108 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/error_message.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    16430 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/flat_spatial_placement.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    11732 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/get_spatial_placement_request.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    10915 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/json_ld_object.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    11255 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/min_max.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    11747 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/ontology_tree.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    14402 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/ontology_tree_node.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    11443 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/rgba.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    11164 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/sparql_query_request.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    19757 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_entity.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    12267 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_entity_common.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    12072 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_entity_creator.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    12370 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_entity_dimensions.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    13721 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_object_reference.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    16736 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_placement.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    16857 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_placement_common.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    12287 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_placement_rotation.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    12190 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_placement_scaling.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    12474 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_placement_translation.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    18061 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_scene_node.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    11807 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_search.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    16643 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_block.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    11549 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_common.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    14111 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_dataset.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    13916 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_donor.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    11680 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_sample_common.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    14726 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_section.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    82158 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/model_utils.py
-drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-14 15:26:58.979572 ccf-openapi-1.1.3/ccf_openapi_client/models/
--rw-r--r--   0 bherr     (1000) bherr     (1000)     2495 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/models/__init__.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    14268 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/rest.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)       69 2023-06-14 15:26:58.989572 ccf-openapi-1.1.3/setup.cfg
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1181 2023-06-14 15:26:54.000000 ccf-openapi-1.1.3/setup.py
-drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-14 15:26:58.989572 ccf-openapi-1.1.3/test/
--rw-r--r--   0 bherr     (1000) bherr     (1000)      840 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_aggregate_count.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      840 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_database_status.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     3580 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/test/test_default_api.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      826 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_error_message.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1029 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_flat_spatial_placement.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1035 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_get_spatial_placement_request.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      827 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_json_ld_object.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      784 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_min_max.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      948 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_ontology_tree.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      961 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_ontology_tree_node.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      769 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_rgba.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      869 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_sparql_query_request.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1579 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_entity.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      876 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_entity_common.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      883 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_entity_creator.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      904 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_entity_dimensions.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1003 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_object_reference.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1109 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_placement.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1473 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_placement_common.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      911 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_placement_rotation.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      904 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_placement_scaling.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      932 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_placement_translation.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1167 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_scene_node.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      833 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_search.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1479 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_tissue_block.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      826 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_tissue_common.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1044 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_tissue_dataset.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1030 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_tissue_donor.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      978 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_tissue_sample_common.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1283 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_tissue_section.py
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-15 15:03:43.899940 ccf-openapi-1.1.4/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      449 2023-06-15 15:03:43.899940 ccf-openapi-1.1.4/PKG-INFO
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     9274 2023-06-15 15:01:49.000000 ccf-openapi-1.1.4/README.md
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-15 15:03:43.878274 ccf-openapi-1.1.4/ccf_openapi.egg-info/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      449 2023-06-15 15:03:43.000000 ccf-openapi-1.1.4/ccf_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     2880 2023-06-15 15:03:43.000000 ccf-openapi-1.1.4/ccf_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 bherr     (1000) bherr     (1000)        1 2023-06-15 15:03:43.000000 ccf-openapi-1.1.4/ccf_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 bherr     (1000) bherr     (1000)       32 2023-06-15 15:03:43.000000 ccf-openapi-1.1.4/ccf_openapi.egg-info/requires.txt
+-rw-r--r--   0 bherr     (1000) bherr     (1000)       19 2023-06-15 15:03:43.000000 ccf-openapi-1.1.4/ccf_openapi.egg-info/top_level.txt
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-15 15:03:43.878274 ccf-openapi-1.1.4/ccf_openapi_client/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      850 2023-06-15 15:01:49.000000 ccf-openapi-1.1.4/ccf_openapi_client/__init__.py
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-15 15:03:43.878274 ccf-openapi-1.1.4/ccf_openapi_client/api/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      222 2023-06-15 15:01:49.000000 ccf-openapi-1.1.4/ccf_openapi_client/api/__init__.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)   104876 2023-06-15 15:01:49.000000 ccf-openapi-1.1.4/ccf_openapi_client/api/default_api.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    37737 2023-06-15 15:01:49.000000 ccf-openapi-1.1.4/ccf_openapi_client/api_client.py
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-15 15:03:43.878274 ccf-openapi-1.1.4/ccf_openapi_client/apis/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      471 2023-06-15 15:01:49.000000 ccf-openapi-1.1.4/ccf_openapi_client/apis/__init__.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    16559 2023-06-15 15:01:49.000000 ccf-openapi-1.1.4/ccf_openapi_client/configuration.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     5140 2023-06-15 15:01:49.000000 ccf-openapi-1.1.4/ccf_openapi_client/exceptions.py
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-15 15:03:43.889107 ccf-openapi-1.1.4/ccf_openapi_client/model/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      348 2023-06-15 15:01:49.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/__init__.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11524 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/aggregate_count.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    12078 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/database_status.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11108 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/error_message.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    16430 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/flat_spatial_placement.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11732 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/get_spatial_placement_request.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    10915 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/json_ld_object.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11255 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/min_max.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11747 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/ontology_tree.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    14402 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/ontology_tree_node.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11443 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/rgba.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11164 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/sparql_query_request.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    19757 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_entity.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    12267 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_entity_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    12072 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_entity_creator.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    12370 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_entity_dimensions.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    13721 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_object_reference.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    16736 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_placement.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    16857 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_placement_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    12287 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_placement_rotation.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    12190 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_placement_scaling.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    12474 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_placement_translation.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    18061 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_scene_node.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11807 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_search.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    16643 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/tissue_block.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11549 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/tissue_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    14111 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/tissue_dataset.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    13916 2023-06-15 15:01:49.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/tissue_donor.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11680 2023-06-15 15:01:49.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/tissue_sample_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    14726 2023-06-15 15:01:49.000000 ccf-openapi-1.1.4/ccf_openapi_client/model/tissue_section.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    82158 2023-06-15 15:01:49.000000 ccf-openapi-1.1.4/ccf_openapi_client/model_utils.py
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-15 15:03:43.889107 ccf-openapi-1.1.4/ccf_openapi_client/models/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     2495 2023-06-15 15:01:49.000000 ccf-openapi-1.1.4/ccf_openapi_client/models/__init__.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    14268 2023-06-15 15:01:49.000000 ccf-openapi-1.1.4/ccf_openapi_client/rest.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)       69 2023-06-15 15:03:43.899940 ccf-openapi-1.1.4/setup.cfg
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1181 2023-06-15 15:03:18.000000 ccf-openapi-1.1.4/setup.py
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-15 15:03:43.899940 ccf-openapi-1.1.4/test/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      840 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_aggregate_count.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      840 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_database_status.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     3580 2023-06-15 15:01:49.000000 ccf-openapi-1.1.4/test/test_default_api.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      826 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_error_message.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1029 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_flat_spatial_placement.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1035 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_get_spatial_placement_request.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      827 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_json_ld_object.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      784 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_min_max.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      948 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_ontology_tree.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      961 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_ontology_tree_node.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      769 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_rgba.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      869 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_sparql_query_request.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1579 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_spatial_entity.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      876 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_spatial_entity_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      883 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_spatial_entity_creator.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      904 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_spatial_entity_dimensions.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1003 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_spatial_object_reference.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1109 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_spatial_placement.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1473 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_spatial_placement_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      911 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_spatial_placement_rotation.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      904 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_spatial_placement_scaling.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      932 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_spatial_placement_translation.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1167 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_spatial_scene_node.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      833 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_spatial_search.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1479 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_tissue_block.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      826 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_tissue_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1044 2023-06-15 15:01:48.000000 ccf-openapi-1.1.4/test/test_tissue_dataset.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1030 2023-06-15 15:01:49.000000 ccf-openapi-1.1.4/test/test_tissue_donor.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      978 2023-06-15 15:01:49.000000 ccf-openapi-1.1.4/test/test_tissue_sample_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1283 2023-06-15 15:01:49.000000 ccf-openapi-1.1.4/test/test_tissue_section.py
```

### Comparing `ccf-openapi-1.1.3/README.md` & `ccf-openapi-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi.egg-info/SOURCES.txt` & `ccf-openapi-1.1.4/ccf_openapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/__init__.py` & `ccf-openapi-1.1.4/ccf_openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/api/default_api.py` & `ccf-openapi-1.1.4/ccf_openapi_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/api_client.py` & `ccf-openapi-1.1.4/ccf_openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/configuration.py` & `ccf-openapi-1.1.4/ccf_openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/exceptions.py` & `ccf-openapi-1.1.4/ccf_openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/aggregate_count.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/aggregate_count.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/database_status.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/database_status.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/error_message.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/error_message.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/flat_spatial_placement.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/flat_spatial_placement.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/get_spatial_placement_request.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/get_spatial_placement_request.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/json_ld_object.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/json_ld_object.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/min_max.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/min_max.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/ontology_tree.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/ontology_tree.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/ontology_tree_node.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/ontology_tree_node.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/rgba.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/rgba.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/sparql_query_request.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/sparql_query_request.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_entity.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_entity.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_entity_common.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_entity_common.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_entity_creator.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_entity_creator.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_entity_dimensions.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_entity_dimensions.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_object_reference.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_object_reference.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_placement.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_placement.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_placement_common.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_placement_common.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_placement_rotation.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_placement_rotation.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_placement_scaling.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_placement_scaling.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_placement_translation.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_placement_translation.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_scene_node.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_scene_node.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_search.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/spatial_search.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_block.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/tissue_block.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_common.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/tissue_common.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_dataset.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/tissue_dataset.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_donor.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/tissue_donor.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_sample_common.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/tissue_sample_common.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_section.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model/tissue_section.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/model_utils.py` & `ccf-openapi-1.1.4/ccf_openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/models/__init__.py` & `ccf-openapi-1.1.4/ccf_openapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/ccf_openapi_client/rest.py` & `ccf-openapi-1.1.4/ccf_openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/setup.py` & `ccf-openapi-1.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
     CCF-API
 
     This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3
+    The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "ccf-openapi"
-VERSION = "1.1.3"
+VERSION = "1.1.4"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `ccf-openapi-1.1.3/test/test_aggregate_count.py` & `ccf-openapi-1.1.4/test/test_aggregate_count.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_database_status.py` & `ccf-openapi-1.1.4/test/test_database_status.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_default_api.py` & `ccf-openapi-1.1.4/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_error_message.py` & `ccf-openapi-1.1.4/test/test_error_message.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_flat_spatial_placement.py` & `ccf-openapi-1.1.4/test/test_flat_spatial_placement.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_get_spatial_placement_request.py` & `ccf-openapi-1.1.4/test/test_get_spatial_placement_request.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_json_ld_object.py` & `ccf-openapi-1.1.4/test/test_json_ld_object.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_min_max.py` & `ccf-openapi-1.1.4/test/test_min_max.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_ontology_tree.py` & `ccf-openapi-1.1.4/test/test_ontology_tree.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_ontology_tree_node.py` & `ccf-openapi-1.1.4/test/test_ontology_tree_node.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_rgba.py` & `ccf-openapi-1.1.4/test/test_rgba.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_sparql_query_request.py` & `ccf-openapi-1.1.4/test/test_sparql_query_request.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_spatial_entity.py` & `ccf-openapi-1.1.4/test/test_spatial_entity.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_spatial_entity_common.py` & `ccf-openapi-1.1.4/test/test_spatial_entity_common.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_spatial_entity_creator.py` & `ccf-openapi-1.1.4/test/test_spatial_entity_creator.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_spatial_entity_dimensions.py` & `ccf-openapi-1.1.4/test/test_spatial_entity_dimensions.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_spatial_object_reference.py` & `ccf-openapi-1.1.4/test/test_spatial_object_reference.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_spatial_placement.py` & `ccf-openapi-1.1.4/test/test_spatial_placement.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_spatial_placement_common.py` & `ccf-openapi-1.1.4/test/test_spatial_placement_common.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_spatial_placement_rotation.py` & `ccf-openapi-1.1.4/test/test_spatial_placement_rotation.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_spatial_placement_scaling.py` & `ccf-openapi-1.1.4/test/test_spatial_placement_scaling.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_spatial_placement_translation.py` & `ccf-openapi-1.1.4/test/test_spatial_placement_translation.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_spatial_scene_node.py` & `ccf-openapi-1.1.4/test/test_spatial_scene_node.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_spatial_search.py` & `ccf-openapi-1.1.4/test/test_spatial_search.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_tissue_block.py` & `ccf-openapi-1.1.4/test/test_tissue_block.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_tissue_common.py` & `ccf-openapi-1.1.4/test/test_tissue_common.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_tissue_dataset.py` & `ccf-openapi-1.1.4/test/test_tissue_dataset.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_tissue_donor.py` & `ccf-openapi-1.1.4/test/test_tissue_donor.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_tissue_sample_common.py` & `ccf-openapi-1.1.4/test/test_tissue_sample_common.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.3/test/test_tissue_section.py` & `ccf-openapi-1.1.4/test/test_tissue_section.py`

 * *Files identical despite different names*

