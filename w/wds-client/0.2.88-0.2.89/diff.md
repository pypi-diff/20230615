# Comparing `tmp/wds-client-0.2.88.tar.gz` & `tmp/wds-client-0.2.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wds-client-0.2.88.tar", last modified: Thu Jun 15 19:12:50 2023, max compression
+gzip compressed data, was "wds-client-0.2.89.tar", last modified: Thu Jun 15 19:47:17 2023, max compression
```

## Comparing `wds-client-0.2.88.tar` & `wds-client-0.2.89.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:12:50.169639 wds-client-0.2.88/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-15 19:12:50.173639 wds-client-0.2.88/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-06-15 19:11:27.000000 wds-client-0.2.88/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 19:12:50.173639 wds-client-0.2.88/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-15 19:11:27.000000 wds-client-0.2.88/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:12:50.165639 wds-client-0.2.88/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-15 19:11:26.000000 wds-client-0.2.88/test/test_attribute_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-15 19:11:26.000000 wds-client-0.2.88/test/test_backup_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-15 19:11:26.000000 wds-client-0.2.88/test/test_batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-15 19:11:26.000000 wds-client-0.2.88/test/test_batch_record_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-15 19:11:26.000000 wds-client-0.2.88/test/test_batch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-15 19:11:26.000000 wds-client-0.2.88/test/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_cloning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-15 19:11:26.000000 wds-client-0.2.88/test/test_commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-15 19:11:26.000000 wds-client-0.2.88/test/test_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-15 19:11:26.000000 wds-client-0.2.88/test/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-15 19:11:26.000000 wds-client-0.2.88/test/test_db_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-15 19:11:26.000000 wds-client-0.2.88/test/test_db_validationcomponent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_db_validationcomponent_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_disk_space_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_disk_space_component_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_general_wds_information_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_inline_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_instances_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_record_attribute_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_record_query_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_record_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_record_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_record_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_records_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_request_body_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_search_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_search_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_stack_trace_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_tsv_upload_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-15 19:11:27.000000 wds-client-0.2.88/test/test_version_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:12:50.165639 wds-client-0.2.88/wds_client/
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:12:50.165639 wds-client-0.2.88/wds_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/api/cloning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/api/general_wds_information_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17329 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/api/instances_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    61562 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/api/records_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19354 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/api/schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/api/snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26217 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:12:50.169639 wds-client-0.2.88/wds_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-15 19:11:26.000000 wds-client-0.2.88/wds_client/models/attribute_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-15 19:11:26.000000 wds-client-0.2.88/wds_client/models/backup_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-06-15 19:11:26.000000 wds-client-0.2.88/wds_client/models/batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-06-15 19:11:26.000000 wds-client-0.2.88/wds_client/models/batch_record_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-15 19:11:26.000000 wds-client-0.2.88/wds_client/models/batch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-15 19:11:26.000000 wds-client-0.2.88/wds_client/models/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-15 19:11:26.000000 wds-client-0.2.88/wds_client/models/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-15 19:11:26.000000 wds-client-0.2.88/wds_client/models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-06-15 19:11:26.000000 wds-client-0.2.88/wds_client/models/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-15 19:11:26.000000 wds-client-0.2.88/wds_client/models/db_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-15 19:11:26.000000 wds-client-0.2.88/wds_client/models/db_validationcomponent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-06-15 19:11:26.000000 wds-client-0.2.88/wds_client/models/db_validationcomponent_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/models/disk_space_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/models/disk_space_component_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/models/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/models/inline_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/models/record_attribute_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/models/record_query_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/models/record_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/models/record_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/models/record_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/models/request_body_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/models/search_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/models/search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/models/search_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/models/stack_trace_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/models/status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/models/tsv_upload_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/models/version_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-06-15 19:11:27.000000 wds-client-0.2.88/wds_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:12:50.165639 wds-client-0.2.88/wds_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-15 19:12:50.000000 wds-client-0.2.88/wds_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-15 19:12:50.000000 wds-client-0.2.88/wds_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:12:50.000000 wds-client-0.2.88/wds_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 19:12:50.000000 wds-client-0.2.88/wds_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 19:12:50.000000 wds-client-0.2.88/wds_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:47:17.325692 wds-client-0.2.89/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-15 19:47:17.325692 wds-client-0.2.89/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-06-15 19:46:12.000000 wds-client-0.2.89/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 19:47:17.325692 wds-client-0.2.89/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-15 19:46:12.000000 wds-client-0.2.89/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:47:17.317692 wds-client-0.2.89/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_attribute_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_backup_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_batch_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_cloning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_db_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_db_validationcomponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_db_validationcomponent_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_disk_space_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_disk_space_component_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_general_wds_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_instances_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_record_attribute_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_record_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_record_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_record_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_records_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_request_body_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_search_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_search_sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_stack_trace_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_tsv_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-15 19:46:12.000000 wds-client-0.2.89/test/test_version_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:47:17.317692 wds-client-0.2.89/wds_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:47:17.321692 wds-client-0.2.89/wds_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/api/cloning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/api/general_wds_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17329 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/api/instances_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61562 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/api/records_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19354 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/api/schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/api/snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26217 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:47:17.325692 wds-client-0.2.89/wds_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/attribute_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/backup_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/batch_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/db_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/db_validationcomponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/db_validationcomponent_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/disk_space_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/disk_space_component_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/record_attribute_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/record_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/record_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/record_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/record_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/request_body_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/search_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/search_sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/stack_trace_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/tsv_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/models/version_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-06-15 19:46:12.000000 wds-client-0.2.89/wds_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:47:17.321692 wds-client-0.2.89/wds_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-15 19:47:17.000000 wds-client-0.2.89/wds_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-15 19:47:17.000000 wds-client-0.2.89/wds_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:47:17.000000 wds-client-0.2.89/wds_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 19:47:17.000000 wds-client-0.2.89/wds_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 19:47:17.000000 wds-client-0.2.89/wds_client.egg-info/top_level.txt
```

### Comparing `wds-client-0.2.88/README.md` & `wds-client-0.2.89/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This page lists current APIs.
 As of v0.2, all APIs are subject to change without notice.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v0.2
-- Package version: 0.2.88
+- Package version: 0.2.89
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
```

### Comparing `wds-client-0.2.88/setup.py` & `wds-client-0.2.89/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "wds-client"
-VERSION = "0.2.88"
+VERSION = "0.2.89"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `wds-client-0.2.88/test/test_attribute_schema.py` & `wds-client-0.2.89/test/test_attribute_schema.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_backup_response.py` & `wds-client-0.2.89/test/test_backup_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_batch_operation.py` & `wds-client-0.2.89/test/test_batch_operation.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_batch_record_request.py` & `wds-client-0.2.89/test/test_batch_record_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_batch_response.py` & `wds-client-0.2.89/test/test_batch_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_build.py` & `wds-client-0.2.89/test/test_build.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_cloning_api.py` & `wds-client-0.2.89/test/test_cloning_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_commit.py` & `wds-client-0.2.89/test/test_commit.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_component.py` & `wds-client-0.2.89/test/test_component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_components.py` & `wds-client-0.2.89/test/test_components.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_db_component.py` & `wds-client-0.2.89/test/test_db_component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_db_validationcomponent.py` & `wds-client-0.2.89/test/test_db_validationcomponent.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_db_validationcomponent_details.py` & `wds-client-0.2.89/test/test_db_validationcomponent_details.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_disk_space_component.py` & `wds-client-0.2.89/test/test_disk_space_component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_disk_space_component_details.py` & `wds-client-0.2.89/test/test_disk_space_component_details.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_error_response.py` & `wds-client-0.2.89/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_general_wds_information_api.py` & `wds-client-0.2.89/test/test_general_wds_information_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_git.py` & `wds-client-0.2.89/test/test_git.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_inline_object.py` & `wds-client-0.2.89/test/test_inline_object.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_instances_api.py` & `wds-client-0.2.89/test/test_instances_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_record_attribute_definition.py` & `wds-client-0.2.89/test/test_record_attribute_definition.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_record_query_response.py` & `wds-client-0.2.89/test/test_record_query_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_record_request.py` & `wds-client-0.2.89/test/test_record_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_record_response.py` & `wds-client-0.2.89/test/test_record_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_record_type_schema.py` & `wds-client-0.2.89/test/test_record_type_schema.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_records_api.py` & `wds-client-0.2.89/test/test_records_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_request_body_search.py` & `wds-client-0.2.89/test/test_request_body_search.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_schema_api.py` & `wds-client-0.2.89/test/test_schema_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_search_operator.py` & `wds-client-0.2.89/test/test_search_operator.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_search_request.py` & `wds-client-0.2.89/test/test_search_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_search_sort_direction.py` & `wds-client-0.2.89/test/test_search_sort_direction.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_snapshots_api.py` & `wds-client-0.2.89/test/test_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_stack_trace_element.py` & `wds-client-0.2.89/test/test_stack_trace_element.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_status_response.py` & `wds-client-0.2.89/test/test_status_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_tsv_upload_response.py` & `wds-client-0.2.89/test/test_tsv_upload_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/test/test_version_response.py` & `wds-client-0.2.89/test/test_version_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/__init__.py` & `wds-client-0.2.89/wds_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.2.88"
+__version__ = "0.2.89"
 
 # import apis into sdk package
 from wds_client.api.cloning_api import CloningApi
 from wds_client.api.general_wds_information_api import GeneralWDSInformationApi
 from wds_client.api.instances_api import InstancesApi
 from wds_client.api.records_api import RecordsApi
 from wds_client.api.schema_api import SchemaApi
```

### Comparing `wds-client-0.2.88/wds_client/api/cloning_api.py` & `wds-client-0.2.89/wds_client/api/cloning_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/api/general_wds_information_api.py` & `wds-client-0.2.89/wds_client/api/general_wds_information_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/api/instances_api.py` & `wds-client-0.2.89/wds_client/api/instances_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/api/records_api.py` & `wds-client-0.2.89/wds_client/api/records_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/api/schema_api.py` & `wds-client-0.2.89/wds_client/api/schema_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/api/snapshots_api.py` & `wds-client-0.2.89/wds_client/api/snapshots_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/api_client.py` & `wds-client-0.2.89/wds_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.2.88/python'
+        self.user_agent = 'OpenAPI-Generator/0.2.89/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `wds-client-0.2.88/wds_client/configuration.py` & `wds-client-0.2.89/wds_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v0.2\n"\
-               "SDK Package Version: 0.2.88".\
+               "SDK Package Version: 0.2.89".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `wds-client-0.2.88/wds_client/exceptions.py` & `wds-client-0.2.89/wds_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/__init__.py` & `wds-client-0.2.89/wds_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/attribute_schema.py` & `wds-client-0.2.89/wds_client/models/attribute_schema.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/backup_response.py` & `wds-client-0.2.89/wds_client/models/backup_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/batch_operation.py` & `wds-client-0.2.89/wds_client/models/batch_operation.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/batch_record_request.py` & `wds-client-0.2.89/wds_client/models/batch_record_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/batch_response.py` & `wds-client-0.2.89/wds_client/models/batch_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/build.py` & `wds-client-0.2.89/wds_client/models/build.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/commit.py` & `wds-client-0.2.89/wds_client/models/commit.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/component.py` & `wds-client-0.2.89/wds_client/models/component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/components.py` & `wds-client-0.2.89/wds_client/models/components.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/db_component.py` & `wds-client-0.2.89/wds_client/models/db_component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/db_validationcomponent.py` & `wds-client-0.2.89/wds_client/models/db_validationcomponent.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/db_validationcomponent_details.py` & `wds-client-0.2.89/wds_client/models/db_validationcomponent_details.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/disk_space_component.py` & `wds-client-0.2.89/wds_client/models/disk_space_component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/disk_space_component_details.py` & `wds-client-0.2.89/wds_client/models/disk_space_component_details.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/error_response.py` & `wds-client-0.2.89/wds_client/models/error_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/git.py` & `wds-client-0.2.89/wds_client/models/git.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/inline_object.py` & `wds-client-0.2.89/wds_client/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/record_attribute_definition.py` & `wds-client-0.2.89/wds_client/models/record_attribute_definition.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/record_query_response.py` & `wds-client-0.2.89/wds_client/models/record_query_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/record_request.py` & `wds-client-0.2.89/wds_client/models/record_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/record_response.py` & `wds-client-0.2.89/wds_client/models/record_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/record_type_schema.py` & `wds-client-0.2.89/wds_client/models/record_type_schema.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/request_body_search.py` & `wds-client-0.2.89/wds_client/models/request_body_search.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/search_operator.py` & `wds-client-0.2.89/wds_client/models/search_operator.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/search_request.py` & `wds-client-0.2.89/wds_client/models/search_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/search_sort_direction.py` & `wds-client-0.2.89/wds_client/models/search_sort_direction.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/stack_trace_element.py` & `wds-client-0.2.89/wds_client/models/stack_trace_element.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/status_response.py` & `wds-client-0.2.89/wds_client/models/status_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/tsv_upload_response.py` & `wds-client-0.2.89/wds_client/models/tsv_upload_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/models/version_response.py` & `wds-client-0.2.89/wds_client/models/version_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client/rest.py` & `wds-client-0.2.89/wds_client/rest.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.88/wds_client.egg-info/SOURCES.txt` & `wds-client-0.2.89/wds_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

