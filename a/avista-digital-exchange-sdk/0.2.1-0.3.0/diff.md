# Comparing `tmp/avista_digital_exchange_sdk-0.2.1.tar.gz` & `tmp/avista_digital_exchange_sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/Justin/urbanova-cloud/Avista Digital Exchange/avista-digital-exchange-sdk/dist/.tmp-wa85lzy1/avista_digital_exchange_sdk", last modified: Wed Feb 15 19:38:30 2023, max compression
+gzip compressed data, was "avista_digital_exchange_sdk-0.3.0.tar", last modified: Thu Jun 15 18:41:10 2023, max compression
```

## Comparing `avista_digital_exchange_sdk-0.2.1.tar` & `avista_digital_exchange_sdk-0.3.0.tar`

### file list

```diff
@@ -1,115 +1,268 @@
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-02-15 19:38:30.824159 avista_digital_exchange_sdk-0.2.1/
--rw-r--r--   0 Justin     (502) staff       (20)    35148 2022-09-13 20:02:44.000000 avista_digital_exchange_sdk-0.2.1/LICENSE
--rw-r--r--   0 Justin     (502) staff       (20)    66103 2023-02-15 19:38:30.823738 avista_digital_exchange_sdk-0.2.1/PKG-INFO
--rw-r--r--   0 Justin     (502) staff       (20)    24860 2023-02-14 23:33:43.000000 avista_digital_exchange_sdk-0.2.1/README.md
--rw-r--r--   0 Justin     (502) staff       (20)      870 2023-02-15 19:38:05.000000 avista_digital_exchange_sdk-0.2.1/pyproject.toml
--rw-r--r--   0 Justin     (502) staff       (20)       38 2023-02-15 19:38:30.824279 avista_digital_exchange_sdk-0.2.1/setup.cfg
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-02-15 19:38:30.751968 avista_digital_exchange_sdk-0.2.1/src/
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-02-15 19:38:30.762015 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/
--rw-r--r--   0 Justin     (502) staff       (20)      190 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/__init__.py
--rw-r--r--   0 Justin     (502) staff       (20)     1567 2023-01-25 22:17:53.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/avista_digital_exchange.py
--rw-r--r--   0 Justin     (502) staff       (20)     2573 2022-12-03 00:28:42.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/client.py
--rw-r--r--   0 Justin     (502) staff       (20)     3384 2022-12-02 17:38:29.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/collaborativeUtil.py
--rw-r--r--   0 Justin     (502) staff       (20)     2784 2022-12-02 17:57:07.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/dataStoreUtil.py
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-02-15 19:38:30.798268 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/
--rw-r--r--   0 Justin     (502) staff       (20)        0 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/__init__.py
--rw-r--r--   0 Justin     (502) staff       (20)     1989 2022-09-29 18:39:50.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/collaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)     1630 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/collaborative_member_organization.py
--rw-r--r--   0 Justin     (502) staff       (20)      852 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/collaborative_member_user.py
--rw-r--r--   0 Justin     (502) staff       (20)     6818 2022-10-10 19:11:23.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/data_store.py
--rw-r--r--   0 Justin     (502) staff       (20)     6384 2022-12-19 18:46:23.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/data_store_directory.py
--rw-r--r--   0 Justin     (502) staff       (20)     6657 2022-12-19 18:45:32.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/data_store_file.py
--rw-r--r--   0 Justin     (502) staff       (20)     2124 2022-10-05 17:07:09.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/data_store_object.py
--rw-r--r--   0 Justin     (502) staff       (20)     1751 2023-01-24 17:50:55.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/digital_twin_model.py
--rw-r--r--   0 Justin     (502) staff       (20)     1414 2022-12-05 17:33:37.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/endpoint_last_values.py
--rw-r--r--   0 Justin     (502) staff       (20)     1214 2022-11-28 17:35:44.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/endpoint_property.py
--rw-r--r--   0 Justin     (502) staff       (20)      990 2022-11-29 01:10:28.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/endpoint_property_input.py
--rw-r--r--   0 Justin     (502) staff       (20)      681 2022-11-29 19:31:15.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/endpoint_query_filter_input.py
--rw-r--r--   0 Justin     (502) staff       (20)     1020 2022-12-02 19:07:37.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry.py
--rw-r--r--   0 Justin     (502) staff       (20)     1340 2022-12-03 00:58:02.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry_data_record.py
--rw-r--r--   0 Justin     (502) staff       (20)      924 2022-12-01 19:36:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_attribute_value.py
--rw-r--r--   0 Justin     (502) staff       (20)      403 2022-12-09 00:20:12.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_attribute_value_input.py
--rw-r--r--   0 Justin     (502) staff       (20)     1175 2022-11-22 17:09:32.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_data_record.py
--rw-r--r--   0 Justin     (502) staff       (20)      860 2022-11-22 17:17:39.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_data_record_error.py
--rw-r--r--   0 Justin     (502) staff       (20)     1816 2022-12-19 19:40:35.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_data_record_input.py
--rw-r--r--   0 Justin     (502) staff       (20)     1479 2022-11-28 18:00:38.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_data_record_with_errors.py
--rw-r--r--   0 Justin     (502) staff       (20)     1834 2022-12-03 00:56:11.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_endpoint.py
--rw-r--r--   0 Justin     (502) staff       (20)     1396 2022-11-30 19:33:37.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_endpoint_data.py
--rw-r--r--   0 Justin     (502) staff       (20)     1807 2022-12-05 17:37:27.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_endpoints_last_values_query_result.py
--rw-r--r--   0 Justin     (502) staff       (20)      726 2022-12-01 19:24:03.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_generate_query_result_export.py
--rw-r--r--   0 Justin     (502) staff       (20)     1889 2022-12-13 17:12:23.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_query_by_time_range_result.py
--rw-r--r--   0 Justin     (502) staff       (20)     2008 2022-12-13 17:11:14.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_query_export.py
--rw-r--r--   0 Justin     (502) staff       (20)     1161 2023-01-24 17:48:06.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/model_property.py
--rw-r--r--   0 Justin     (502) staff       (20)     1795 2023-01-25 00:41:35.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/model_property_input.py
--rw-r--r--   0 Justin     (502) staff       (20)     1017 2023-01-24 17:48:35.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/model_telemetry.py
--rw-r--r--   0 Justin     (502) staff       (20)      984 2023-01-25 00:48:12.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/model_telemetry_input.py
--rw-r--r--   0 Justin     (502) staff       (20)      785 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/organization.py
--rw-r--r--   0 Justin     (502) staff       (20)      732 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/presigned_url.py
--rw-r--r--   0 Justin     (502) staff       (20)     1521 2022-12-08 19:15:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/publish_iot_data_result.py
--rw-r--r--   0 Justin     (502) staff       (20)      727 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/server_response.py
--rw-r--r--   0 Justin     (502) staff       (20)     2594 2022-10-05 21:52:25.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/service.py
--rw-r--r--   0 Justin     (502) staff       (20)     1423 2022-09-29 19:12:44.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute.py
--rw-r--r--   0 Justin     (502) staff       (20)      811 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute_data.py
--rw-r--r--   0 Justin     (502) staff       (20)     1408 2022-09-30 17:03:56.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_asset_data.py
--rw-r--r--   0 Justin     (502) staff       (20)     1902 2022-09-29 19:12:59.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_assets_and_last_values_result.py
--rw-r--r--   0 Justin     (502) staff       (20)     1384 2022-10-05 16:49:01.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_db.py
--rw-r--r--   0 Justin     (502) staff       (20)      732 2022-09-29 19:13:54.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_dimension.py
--rw-r--r--   0 Justin     (502) staff       (20)      809 2022-09-29 19:11:31.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_generate_query_export_result.py
--rw-r--r--   0 Justin     (502) staff       (20)     3466 2022-09-30 16:48:18.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_input_record.py
--rw-r--r--   0 Justin     (502) staff       (20)      640 2022-09-29 19:17:22.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_measure_value.py
--rw-r--r--   0 Justin     (502) staff       (20)      911 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_publish_input.py
--rw-r--r--   0 Justin     (502) staff       (20)      837 2022-09-29 19:18:29.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_publish_response.py
--rw-r--r--   0 Justin     (502) staff       (20)     1925 2022-09-30 00:39:31.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_query_export.py
--rw-r--r--   0 Justin     (502) staff       (20)     1334 2022-09-29 19:45:45.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_query_result.py
--rw-r--r--   0 Justin     (502) staff       (20)     1602 2022-09-29 19:30:48.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/timestream_query_result.py
--rw-r--r--   0 Justin     (502) staff       (20)     1579 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/user.py
--rw-r--r--   0 Justin     (502) staff       (20)      176 2022-11-21 23:52:33.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/endpointUtil.py
--rw-r--r--   0 Justin     (502) staff       (20)     2597 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/exceptions.py
--rw-r--r--   0 Justin     (502) staff       (20)      460 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/globals.py
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-02-15 19:38:30.807361 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/
--rw-r--r--   0 Justin     (502) staff       (20)     1489 2022-09-29 19:23:24.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_addServiceToCollaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)     1469 2022-09-29 19:24:19.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_removeServiceFromCollaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)     1055 2022-12-02 17:40:14.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_cancelQuery.py
--rw-r--r--   0 Justin     (502) staff       (20)     1401 2023-02-15 19:36:31.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_createEndpoint.py
--rw-r--r--   0 Justin     (502) staff       (20)     1703 2023-02-14 23:10:32.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_createModel.py
--rw-r--r--   0 Justin     (502) staff       (20)     1333 2022-12-01 20:55:30.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_generateQueryResultExport.py
--rw-r--r--   0 Justin     (502) staff       (20)     1374 2022-11-23 17:59:59.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_publish.py
--rw-r--r--   0 Justin     (502) staff       (20)     1375 2022-11-29 01:46:34.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_updateEndpointProperties.py
--rw-r--r--   0 Justin     (502) staff       (20)     1410 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/mutation.py
--rw-r--r--   0 Justin     (502) staff       (20)     1602 2022-09-29 19:24:48.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/storage_createDataStoreFile.py
--rw-r--r--   0 Justin     (502) staff       (20)     1199 2022-09-29 19:25:14.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/storage_deleteDataStoreFile.py
--rw-r--r--   0 Justin     (502) staff       (20)     1204 2022-09-29 19:25:37.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_cancelDatabaseQuery.py
--rw-r--r--   0 Justin     (502) staff       (20)     1503 2022-09-29 19:25:41.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_generateQueryResultExportFile.py
--rw-r--r--   0 Justin     (502) staff       (20)     1825 2022-09-29 19:22:38.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_publishToDatabase.py
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-02-15 19:38:30.820677 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/
--rw-r--r--   0 Justin     (502) staff       (20)        0 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/__init__.py
--rw-r--r--   0 Justin     (502) staff       (20)     1273 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/collaborative_getCollaborative.py
--rw-r--r--   0 Justin     (502) staff       (20)     1470 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativeServices.py
--rw-r--r--   0 Justin     (502) staff       (20)     1247 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaboratives.py
--rw-r--r--   0 Justin     (502) staff       (20)     1776 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativesServiceSharedWith.py
--rw-r--r--   0 Justin     (502) staff       (20)     1205 2022-12-03 00:56:58.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/iot_getEndpoint.py
--rw-r--r--   0 Justin     (502) staff       (20)     1779 2022-11-28 19:19:16.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/iot_listEndpointLastValues.py
--rw-r--r--   0 Justin     (502) staff       (20)     2454 2022-12-01 19:24:44.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/iot_queryByTimeRange.py
--rw-r--r--   0 Justin     (502) staff       (20)     1394 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/query.py
--rw-r--r--   0 Justin     (502) staff       (20)     1189 2022-10-05 16:34:47.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStore.py
--rw-r--r--   0 Justin     (502) staff       (20)     1327 2022-10-05 21:54:09.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreDirectory.py
--rw-r--r--   0 Justin     (502) staff       (20)     1264 2022-10-05 21:53:38.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFile.py
--rw-r--r--   0 Justin     (502) staff       (20)     1417 2022-12-20 17:42:57.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFileDownloadUrl.py
--rw-r--r--   0 Justin     (502) staff       (20)     1195 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/storage_listDataStores.py
--rw-r--r--   0 Justin     (502) staff       (20)     1277 2022-09-29 18:46:04.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_getDatabase.py
--rw-r--r--   0 Justin     (502) staff       (20)     1839 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listAllAssetLastValues.py
--rw-r--r--   0 Justin     (502) staff       (20)     1216 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listDatabases.py
--rw-r--r--   0 Justin     (502) staff       (20)     3214 2022-09-30 00:23:31.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabase.py
--rw-r--r--   0 Justin     (502) staff       (20)     2085 2022-09-29 19:12:18.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabaseWithTimestreamQuery.py
--rw-r--r--   0 Justin     (502) staff       (20)     1021 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/user_getUserSession.py
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-02-15 19:38:30.822674 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_subscriptions/
--rw-r--r--   0 Justin     (502) staff       (20)     3353 2022-12-13 17:40:26.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyIotQueryExportComplete.py
--rw-r--r--   0 Justin     (502) staff       (20)     3526 2022-09-29 19:46:08.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyTimeSeriesQueryExportComplete.py
--rw-r--r--   0 Justin     (502) staff       (20)     1486 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_subscriptions/subscription.py
--rw-r--r--   0 Justin     (502) staff       (20)     8334 2023-01-25 17:05:20.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/iotUtil.py
--rw-r--r--   0 Justin     (502) staff       (20)     6848 2023-01-25 00:06:56.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/subscriptionClient.py
-drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-02-15 19:38:30.764053 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk.egg-info/
--rw-r--r--   0 Justin     (502) staff       (20)    66103 2023-02-15 19:38:30.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk.egg-info/PKG-INFO
--rw-r--r--   0 Justin     (502) staff       (20)     7154 2023-02-15 19:38:30.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 Justin     (502) staff       (20)        1 2023-02-15 19:38:30.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 Justin     (502) staff       (20)       28 2023-02-15 19:38:30.000000 avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.330997 avista_digital_exchange_sdk-0.3.0/
+-rw-r--r--   0 Justin     (502) staff       (20)    35148 2022-09-13 20:02:44.000000 avista_digital_exchange_sdk-0.3.0/LICENSE
+-rw-r--r--   0 Justin     (502) staff       (20)    74798 2023-06-15 18:41:10.330617 avista_digital_exchange_sdk-0.3.0/PKG-INFO
+-rw-r--r--   0 Justin     (502) staff       (20)    33555 2023-06-15 18:40:21.000000 avista_digital_exchange_sdk-0.3.0/README.md
+-rw-r--r--   0 Justin     (502) staff       (20)      910 2023-06-15 18:28:56.000000 avista_digital_exchange_sdk-0.3.0/pyproject.toml
+-rw-r--r--   0 Justin     (502) staff       (20)       38 2023-06-15 18:41:10.331095 avista_digital_exchange_sdk-0.3.0/setup.cfg
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.178336 avista_digital_exchange_sdk-0.3.0/src/
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.192415 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/
+-rw-r--r--   0 Justin     (502) staff       (20)     4968 2023-06-15 18:28:20.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/DxTypes.py
+-rw-r--r--   0 Justin     (502) staff       (20)      213 2023-06-14 18:10:08.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/__init__.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1628 2023-06-15 18:31:43.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/avista_digital_exchange.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3268 2023-06-15 18:28:32.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/client.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3384 2022-12-02 17:38:29.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/collaborativeUtil.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6799 2023-06-15 18:28:11.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/dataCaptureUtil.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2784 2022-12-02 17:57:07.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/dataStoreUtil.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.223612 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/
+-rw-r--r--   0 Justin     (502) staff       (20)        0 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/__init__.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1989 2022-09-29 18:39:50.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1630 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/collaborative_member_organization.py
+-rw-r--r--   0 Justin     (502) staff       (20)      852 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/collaborative_member_user.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6818 2022-10-10 19:11:23.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/data_store.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6384 2022-12-19 18:46:23.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/data_store_directory.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6657 2022-12-19 18:45:32.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/data_store_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2124 2022-10-05 17:07:09.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/data_store_object.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1751 2023-01-24 17:50:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/digital_twin_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1414 2022-12-05 17:33:37.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_last_values.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1214 2022-11-28 17:35:44.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_property.py
+-rw-r--r--   0 Justin     (502) staff       (20)      990 2022-11-29 01:10:28.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_property_input.py
+-rw-r--r--   0 Justin     (502) staff       (20)      681 2022-11-29 19:31:15.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_query_filter_input.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1020 2022-12-02 19:07:37.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1340 2022-12-03 00:58:02.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry_data_record.py
+-rw-r--r--   0 Justin     (502) staff       (20)      924 2022-12-01 19:36:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_attribute_value.py
+-rw-r--r--   0 Justin     (502) staff       (20)      403 2022-12-09 00:20:12.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_attribute_value_input.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1175 2022-11-22 17:09:32.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_data_record.py
+-rw-r--r--   0 Justin     (502) staff       (20)      860 2022-11-22 17:17:39.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_data_record_error.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1816 2022-12-19 19:40:35.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_data_record_input.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1479 2022-11-28 18:00:38.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_data_record_with_errors.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1834 2022-12-03 00:56:11.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_endpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1396 2022-11-30 19:33:37.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_endpoint_data.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1807 2022-12-05 17:37:27.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_endpoints_last_values_query_result.py
+-rw-r--r--   0 Justin     (502) staff       (20)      726 2022-12-01 19:24:03.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_generate_query_result_export.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1889 2022-12-13 17:12:23.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_query_by_time_range_result.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2008 2022-12-13 17:11:14.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_query_export.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1161 2023-01-24 17:48:06.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/model_property.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1795 2023-01-25 00:41:35.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/model_property_input.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1017 2023-01-24 17:48:35.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/model_telemetry.py
+-rw-r--r--   0 Justin     (502) staff       (20)      984 2023-01-25 00:48:12.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/model_telemetry_input.py
+-rw-r--r--   0 Justin     (502) staff       (20)      785 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/organization.py
+-rw-r--r--   0 Justin     (502) staff       (20)      732 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/presigned_url.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1521 2022-12-08 19:15:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/publish_iot_data_result.py
+-rw-r--r--   0 Justin     (502) staff       (20)      727 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/server_response.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2594 2022-10-05 21:52:25.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/service.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1423 2022-09-29 19:12:44.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute.py
+-rw-r--r--   0 Justin     (502) staff       (20)      811 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute_data.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1408 2022-09-30 17:03:56.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_asset_data.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1902 2022-09-29 19:12:59.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_assets_and_last_values_result.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1384 2022-10-05 16:49:01.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_db.py
+-rw-r--r--   0 Justin     (502) staff       (20)      732 2022-09-29 19:13:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_dimension.py
+-rw-r--r--   0 Justin     (502) staff       (20)      809 2022-09-29 19:11:31.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_generate_query_export_result.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3466 2022-09-30 16:48:18.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_input_record.py
+-rw-r--r--   0 Justin     (502) staff       (20)      640 2022-09-29 19:17:22.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_measure_value.py
+-rw-r--r--   0 Justin     (502) staff       (20)      911 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_publish_input.py
+-rw-r--r--   0 Justin     (502) staff       (20)      837 2022-09-29 19:18:29.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_publish_response.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1925 2022-09-30 00:39:31.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_query_export.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1334 2022-09-29 19:45:45.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_query_result.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1602 2022-09-29 19:30:48.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/timestream_query_result.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1579 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/user.py
+-rw-r--r--   0 Justin     (502) staff       (20)      176 2022-11-21 23:52:33.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/endpointUtil.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2597 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/exceptions.py
+-rw-r--r--   0 Justin     (502) staff       (20)      460 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/globals.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.180063 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.179651 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.308398 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/
+-rw-r--r--   0 Justin     (502) staff       (20)    94862 2023-06-08 22:03:56.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/__init__.py
+-rw-r--r--   0 Justin     (502) staff       (20)     7371 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/async_base_client.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1951 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/base_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)   200424 2023-06-08 22:03:56.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/client.py
+-rw-r--r--   0 Justin     (502) staff       (20)    10097 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_add_service_to_collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5538 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_get_collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)     7019 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_list_collaborative_member_organization_requests.py
+-rw-r--r--   0 Justin     (502) staff       (20)    10164 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_list_collaborative_services.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5658 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_list_collaboratives.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6603 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_list_collaboratives_service_shared_with.py
+-rw-r--r--   0 Justin     (502) staff       (20)    10537 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_remove_service_from_collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5561 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/collaborative_update_collaborative_member_organization.py
+-rw-r--r--   0 Justin     (502) staff       (20)      668 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_attach_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4109 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_create_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1005 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_delete_attachment.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4109 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_delete_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3969 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_get_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1222 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_get_capture_authentication_token.py
+-rw-r--r--   0 Justin     (502) staff       (20)      987 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_get_data_export_download_url.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1899 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_get_data_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)      731 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_get_data_model_export.py
+-rw-r--r--   0 Justin     (502) staff       (20)      857 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_get_file_attachment_download_url.py
+-rw-r--r--   0 Justin     (502) staff       (20)      406 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_get_python_s_d_k_sample.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4281 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_handle_completion.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1017 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_list_attachments.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4561 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_list_captures.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4528 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_notify_capture_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1833 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_publish_data.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1221 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_regenerate_authentication_token.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4063 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_start_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4009 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_stop_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4109 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_update_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2017 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_update_data_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)      760 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/data_capture_upload_data_model_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3906 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/enums.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2366 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/exceptions.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5844 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/input_types.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2516 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_add_endpoints_to_group.py
+-rw-r--r--   0 Justin     (502) staff       (20)      599 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_cancel_query.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1762 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_create_endpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2254 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_create_group.py
+-rw-r--r--   0 Justin     (502) staff       (20)      577 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_create_hub.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1616 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_create_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1866 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_create_new_model_version.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1762 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_delete_endpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2254 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_delete_group.py
+-rw-r--r--   0 Justin     (502) staff       (20)      577 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_delete_hub.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1616 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_delete_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)      761 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_generate_query_result_export.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1696 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_get_endpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1004 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_get_endpoint_token.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2128 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_get_group.py
+-rw-r--r--   0 Justin     (502) staff       (20)      547 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_get_hub.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1536 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_get_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)      383 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_get_model_in_d_t_d_l_format.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2327 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_list_endpoint_last_values.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1896 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_list_endpoints_in_hub.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2228 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_list_groups.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2544 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_list_groups_endpoints_last_values.py
+-rw-r--r--   0 Justin     (502) staff       (20)      603 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_list_hubs.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2488 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_list_hubs_endpoints_last_values.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1610 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_list_models.py
+-rw-r--r--   0 Justin     (502) staff       (20)      830 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_notify_query_export_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2275 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_publish.py
+-rw-r--r--   0 Justin     (502) staff       (20)      947 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_query_by_time_range.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1074 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_regenerate_endpoint_token.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2772 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_remove_endpoints_from_group.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1762 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_update_endpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2055 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_update_endpoint_properties.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2254 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_update_group.py
+-rw-r--r--   0 Justin     (502) staff       (20)      577 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_update_hub.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1616 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_update_model.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2139 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/iot_update_model_used_by_endpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)      835 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/notifications_notify_upload_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1776 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_capture_publish_data.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2410 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_iot_publish.py
+-rw-r--r--   0 Justin     (502) staff       (20)     4062 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_notify_capture_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)      850 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_notify_iot_query_export_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)      949 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_notify_time_series_query_export_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)      724 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_notify_upload_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3635 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_start_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3595 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_stop_capture.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1407 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/on_time_series_db_publish.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5852 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_add_collaborative_member.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5695 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_create_collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)      782 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_create_organization.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1429 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_create_user.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5695 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_delete_collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)      782 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_delete_organization.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1429 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_delete_user.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6082 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_delete_users_collaboratives.py
+-rw-r--r--   0 Justin     (502) staff       (20)     9601 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_delete_users_services.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5539 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_get_collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)      752 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_get_organization.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1381 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_get_user.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5659 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_list_collaboratives.py
+-rw-r--r--   0 Justin     (502) staff       (20)      794 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_list_organizations.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1429 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_list_users.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6603 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_migrate_users_collaboratives_ownership.py
+-rw-r--r--   0 Justin     (502) staff       (20)    10518 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_migrate_users_services_ownership.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6014 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_remove_collaborative_member.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1610 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_resend_user_invitation.py
+-rw-r--r--   0 Justin     (502) staff       (20)     5695 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_update_collaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6014 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_update_collaborative_member.py
+-rw-r--r--   0 Justin     (502) staff       (20)      782 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_update_organization.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1429 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/platform_admin_update_user.py
+-rw-r--r--   0 Justin     (502) staff       (20)      220 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/scalars.py
+-rw-r--r--   0 Justin     (502) staff       (20)      778 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_create_data_store.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3907 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_create_data_store_directory.py
+-rw-r--r--   0 Justin     (502) staff       (20)      719 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_create_data_store_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1403 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_create_data_store_file_data_view.py
+-rw-r--r--   0 Justin     (502) staff       (20)      778 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_delete_data_store.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3907 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_delete_data_store_directory.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1321 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_delete_data_store_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1403 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_delete_data_store_file_data_view.py
+-rw-r--r--   0 Justin     (502) staff       (20)      748 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_get_data_store.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3775 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_get_data_store_directory.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1291 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_get_data_store_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)      801 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_get_data_store_file_download_url.py
+-rw-r--r--   0 Justin     (502) staff       (20)      791 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_get_data_store_zip_download_url.py
+-rw-r--r--   0 Justin     (502) staff       (20)      790 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_list_data_stores.py
+-rw-r--r--   0 Justin     (502) staff       (20)      778 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_update_data_store.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3907 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_update_data_store_directory.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1321 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/storage_update_data_store_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)      772 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_cancel_database_query.py
+-rw-r--r--   0 Justin     (502) staff       (20)      866 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_create_database.py
+-rw-r--r--   0 Justin     (502) staff       (20)      866 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_delete_database.py
+-rw-r--r--   0 Justin     (502) staff       (20)      985 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_generate_query_result_export_file.py
+-rw-r--r--   0 Justin     (502) staff       (20)      836 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_get_database.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2463 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_list_all_asset_last_values.py
+-rw-r--r--   0 Justin     (502) staff       (20)      878 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_list_databases.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1052 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_notify_time_series_query_export_complete.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1695 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_publish_to_database.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1015 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_query_database.py
+-rw-r--r--   0 Justin     (502) staff       (20)      905 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_query_database_with_timestream_query.py
+-rw-r--r--   0 Justin     (502) staff       (20)      866 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/time_series_db_update_database.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1104 2023-06-08 22:03:53.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/user_create_authentication_token.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1104 2023-06-08 22:03:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/user_delete_authentication_token.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1548 2023-06-08 22:03:54.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/user_get_user_session.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1110 2023-06-08 22:03:55.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/ariadne/graphql_client/user_list_authentication_tokens.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.308881 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/gqlg/
+-rw-r--r--   0 Justin     (502) staff       (20)      507 2023-06-08 16:25:42.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_codegen/gqlg/condenseQueries.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.316975 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/
+-rw-r--r--   0 Justin     (502) staff       (20)     1489 2022-09-29 19:23:24.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_addServiceToCollaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1469 2022-09-29 19:24:19.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_removeServiceFromCollaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)      329 2023-05-17 16:29:16.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/dataCapture_publishData.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1055 2022-12-02 17:40:14.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_cancelQuery.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1401 2023-02-15 19:36:31.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_createEndpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1703 2023-02-14 23:10:32.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_createModel.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1333 2022-12-01 20:55:30.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_generateQueryResultExport.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1374 2022-11-23 17:59:59.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_publish.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1375 2022-11-29 01:46:34.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_updateEndpointProperties.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1410 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/mutation.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1602 2022-09-29 19:24:48.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/storage_createDataStoreFile.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1199 2022-09-29 19:25:14.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/storage_deleteDataStoreFile.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1204 2022-09-29 19:25:37.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_cancelDatabaseQuery.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1503 2022-09-29 19:25:41.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_generateQueryResultExportFile.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1825 2022-09-29 19:22:38.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_publishToDatabase.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.326347 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/
+-rw-r--r--   0 Justin     (502) staff       (20)        0 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/__init__.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1273 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/collaborative_getCollaborative.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1470 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativeServices.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1247 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaboratives.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1776 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativesServiceSharedWith.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1205 2022-12-03 00:56:58.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/iot_getEndpoint.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1779 2022-11-28 19:19:16.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/iot_listEndpointLastValues.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2454 2022-12-01 19:24:44.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/iot_queryByTimeRange.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1394 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/query.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1189 2022-10-05 16:34:47.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStore.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1327 2022-10-05 21:54:09.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreDirectory.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1264 2022-10-05 21:53:38.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFile.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1417 2022-12-20 17:42:57.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFileDownloadUrl.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1195 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/storage_listDataStores.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1277 2022-09-29 18:46:04.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_getDatabase.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1839 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listAllAssetLastValues.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1216 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listDatabases.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3214 2022-09-30 00:23:31.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabase.py
+-rw-r--r--   0 Justin     (502) staff       (20)     2085 2022-09-29 19:12:18.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabaseWithTimestreamQuery.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1021 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/user_getUserSession.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.328368 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_subscriptions/
+-rw-r--r--   0 Justin     (502) staff       (20)     3353 2022-12-13 17:40:26.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyIotQueryExportComplete.py
+-rw-r--r--   0 Justin     (502) staff       (20)     3526 2022-09-29 19:46:08.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyTimeSeriesQueryExportComplete.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1486 2022-09-29 18:28:05.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_subscriptions/subscription.py
+-rw-r--r--   0 Justin     (502) staff       (20)     8438 2023-06-06 23:25:52.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/iotUtil.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1000 2023-06-13 20:20:28.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/logger.py
+-rw-r--r--   0 Justin     (502) staff       (20)     6848 2023-01-25 00:06:56.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/subscriptionClient.py
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.195057 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk.egg-info/
+-rw-r--r--   0 Justin     (502) staff       (20)    74798 2023-06-15 18:41:10.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 Justin     (502) staff       (20)    22060 2023-06-15 18:41:10.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 Justin     (502) staff       (20)        1 2023-06-15 18:41:10.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 Justin     (502) staff       (20)       28 2023-06-15 18:41:10.000000 avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 Justin     (502) staff       (20)        0 2023-06-15 18:41:10.330009 avista_digital_exchange_sdk-0.3.0/tests/
+-rw-r--r--   0 Justin     (502) staff       (20)      469 2023-06-15 18:37:15.000000 avista_digital_exchange_sdk-0.3.0/tests/test.py
+-rw-r--r--   0 Justin     (502) staff       (20)      162 2023-06-15 16:15:35.000000 avista_digital_exchange_sdk-0.3.0/tests/test_dataCapture_publishData.py
+-rw-r--r--   0 Justin     (502) staff       (20)     1599 2023-06-15 18:37:22.000000 avista_digital_exchange_sdk-0.3.0/tests/test_iot_publishData.py
```

### Comparing `avista_digital_exchange_sdk-0.2.1/LICENSE` & `avista_digital_exchange_sdk-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/PKG-INFO` & `avista_digital_exchange_sdk-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avista_digital_exchange_sdk
-Version: 0.2.1
+Version: 0.3.0
 Summary: SDK to programmatically access the Avista Digital Exchange
 Author-email: Justin Whicker <jwhicker@urbanova.org>, Jon Thompson <jon.thompson@avistacorp.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -718,14 +718,18 @@
       - [getEndpoint](#getendpoint)
       - [createEndpoint](#createendpoint)
       - [createModel](#createmodel)
       - [listEndpointLastValues](#listendpointlastvalues)
       - [queryByTimeRange](#querybytimerange)
       - [publish](#publish)
       - [updateEndpointProperties](#updateendpointproperties)
+    - [dataCapture](#datacapture)
+      - [publishData](#publishdata)
+      - [startCapture](#startcapture)
+      - [stopCapture](#stopcapture)
   - [Types](#types)
     - [User](#user)
     - [Organization](#organization)
     - [DataStore](#datastore-1)
       - [Methods](#methods)
         - [cd](#cd)
         - [ls](#ls)
@@ -739,16 +743,24 @@
     - [DataStoreFile](#datastorefile)
     - [DigitalTwinModel](#digitaltwinmodel)
     - [ModelProperty](#modelproperty)
     - [ModelTelemetry](#modeltelemetry)
     - [IotEndpoint](#iotendpoint)
     - [EndpointProperty](#endpointproperty)
     - [EndpointTelemetry](#endpointtelemetry)
+    - [DxTypes.CaptureDataRecordInput](#dxtypescapturedatarecordinput)
+    - [DxTypes.PublishCaptureDataResult](#dxtypespublishcapturedataresult)
+    - [DxTypes.PublishCaptureDataSuccessfulRecord](#dxtypespublishcapturedatasuccessfulrecord)
+    - [DxTypes.PublishCaptureDataFailedRecord](#dxtypespublishcapturedatafailedrecord)
+    - [DxTypes.StartCaptureResult](#dxtypesstartcaptureresult)
+    - [DxTypes.StopCaptureResult](#dxtypesstopcaptureresult)
   - [Development](#development)
   - [Deployment](#deployment)
+  - [Generating Python types and GraphQL Client from GraphQL Schema](#generating-python-types-and-graphql-client-from-graphql-schema)
+  - [Fix for py-graphql-mapper module](#fix-for-py-graphql-mapper-module)
   - [Resources](#resources)
 
 ## Getting Started<a id="getting-started"></a>
 
 1. Install the python package.
 
 ```
@@ -1182,15 +1194,15 @@
     "iotEndpointId.1234", 
     ["SOC", "V", "V - Setpoint"], 
     "2022-09-25T20:13:04.465Z", 
     "2022-09-26T20:58:04.465Z", 
     "./")
 ```
 
-#### publish<a id="publish"></a>
+#### publish<a id="iotpublish"></a>
 
 Publish telemetry values for an endpoint.  One or more data records can be written at one time.
 
 **Parameters**
 
 ```
 iotEndpointId :  str, required
@@ -1291,19 +1303,180 @@
 
 ```
 
 properties = {
     'moving': False
 }
 
-instance.iot.updateEndpointProperties(
+digitalExchange.iot.updateEndpointProperties(
      "iotEndpointId.1234",
      properties)
 ```
 
+---
+
+### dataCapture<a id="datacapture"></a>
+
+#### publishData<a id="publishdata"></a>
+
+Publish attribute values to an active Data Capture.
+
+**Parameters**
+
+```
+captureId :  str, required
+    The id of the Data Capture.
+data :  [DxTypes.CaptureDataRecordInput], required
+    Array of data records to write.  Each dict should contain the record's timestamp, timeUnit ("MILLISECONDS"), and a dicitonary of attributeId, value pairs. Example shown below.
+```
+
+**Return Type**
+
+[DxTypes.PublishCaptureDataResult](#dxtypespublishcapturedataresult)
+
+
+**Example**
+
+```
+# captureDataPublishSample.py
+import asyncio
+import time
+from avista_digital_exchange_sdk import AvistaDigitalExchange, DxTypes
+
+# Create an instance of the AvistaDigitalExchange SDK
+# You may use a user authentication token or the authentication token of the Data Capture
+digitalExchange = AvistaDigitalExchange(AUTHENTICATION_TOKEN_VALUE)
+print("Instantiated AvistaDigitalExchange instance with authentication token")
+
+# Specify the capture you are publishing data to.
+# NOTE: The capture must be in Capturing state to accept data
+captureId = YOUR_CAPTURE_ID
+
+def getCurrentMilliseconds():
+    return int(f'{time.time() * 1000}'.split('.')[0])
+
+async def publishDataExample():
+    # Prepare the data to be published
+    # Replace ATTRIBUTE_ID and ATTRIBUTE_VALUE
+    attributeValueMap = {
+        ATTRIBUTE_ID: ATTRIBUTE_VALUE,
+        ATTRIBUTE_ID: ATTRIBUTE_VALUE,
+        ATTRIBUTE_ID: ATTRIBUTE_VALUE,
+    }
+
+    data = [DxTypes.CaptureDataRecordInput(
+            timestamp=f'{getCurrentMilliseconds()}',
+            timeUnit="MILLISECONDS",
+            attributeValues=attributeValueMap)]
+    try:
+        print("Calling dataCapture.publishData")
+        result = await digitalExchange.dataCapture.publishData(
+            captureId=captureId, data=data)
+    except:
+        print("dataCapture.publishData failed")
+
+asyncio.run(publishDataExample())
+```
+
+#### startCapture<a id="startcapture"></a>
+
+Commands a Data Capture to begin collecting data. Capture must be in 'Ready' state for startCapture to succeed.
+
+**Parameters**
+
+```
+captureId :  str, required
+    The id of the Data Capture.
+```
+
+**Return Type**
+
+[DxTypes.StartCaptureResult](#dxtypesstartcaptureresult)
+
+
+**Example**
+
+```
+# captureDataPublishSample.py
+import asyncio
+import time
+from avista_digital_exchange_sdk import AvistaDigitalExchange, DxTypes
+
+# Create an instance of the AvistaDigitalExchange SDK
+# You may use a user authentication token or the authentication token of the Data Capture
+digitalExchange = AvistaDigitalExchange(AUTHENTICATION_TOKEN_VALUE)
+print("Instantiated AvistaDigitalExchange instance with authentication token")
+
+# Specify the capture you are starting.
+# NOTE: The capture must be in 'READY' state to accept data
+captureId = YOUR_CAPTURE_ID
+
+def getCurrentMilliseconds():
+    return int(f'{time.time() * 1000}'.split('.')[0])
+
+async def startCaptureExample():
+    try:
+        print("Calling dataCapture.startCapture")
+        result = await digitalExchange.dataCapture.startCapture(
+            captureId=captureId)
+    except:
+        print("dataCapture.startCapture failed")
+
+asyncio.run(startCaptureExample())
+```
+
+
+#### stopCapture<a id="stopcapture"></a>
+
+Commands a Data Capture to stop collecting data. Capture must be in 'CAPTURING' state for stopCapture to succeed.
+
+**Parameters**
+
+```
+captureId :  str, required
+    The id of the Data Capture.
+```
+
+**Return Type**
+
+[DxTypes.StopCaptureResult](#dxtypesstopcaptureresult)
+
+
+**Example**
+
+```
+# captureDataPublishSample.py
+import asyncio
+import time
+from avista_digital_exchange_sdk import AvistaDigitalExchange, DxTypes
+
+# Create an instance of the AvistaDigitalExchange SDK
+# You may use a user authentication token or the authentication token of the Data Capture
+digitalExchange = AvistaDigitalExchange(AUTHENTICATION_TOKEN_VALUE)
+print("Instantiated AvistaDigitalExchange instance with authentication token")
+
+# Specify the capture you are stopping.
+# NOTE: The capture must be in 'CAPTURING' state to be stopped.
+captureId = YOUR_CAPTURE_ID
+
+def getCurrentMilliseconds():
+    return int(f'{time.time() * 1000}'.split('.')[0])
+
+async def stopCaptureExample():
+    try:
+        print("Calling dataCapture.stopCapture")
+        result = await digitalExchange.dataCapture.stopCapture(
+            captureId=captureId)
+    except:
+        print("dataCapture.stopCapture failed")
+
+asyncio.run(stopCaptureExample())
+```
+
+
 
 ---
 
 ## Types<a id="types"></a>
 
 ### User<a id="user"></a>
 
@@ -1617,42 +1790,162 @@
 name: str
     Name of the telemetry.
 description: str
 schemaType: str : "integer", "double", "string", "boolean", "dateTime", "duration"
     The type of the variable.
 ```
 
+### DxTypes.CaptureDataRecordInput<a id="dxtypescapturedatarecordinput"></a>
+
+A data record that is to be published to a Data Capture.
+
+**Properties**
+
+```
+timestamp: str
+    The timestamp of the data record
+timeUnit: str
+    The format of the timestamp
+attributeValues: dict
+    A dictionary containing the data to be written for the given timestmap. Key values should be attributeIds that map to the relevant attribute values. 
+```
+
+### DxTypes.PublishCaptureDataResult<a id="dxtypespublishcapturedataresult"></a>
+
+Result object for the DataCapture.publishData operation.
+
+**Properties**
+
+```
+success: bool
+    Indicates if the action was successful
+captureId: str
+    The captureId of the Data Capture published to.
+recordsWritten: [DxTypes.PublishCaptureDataSuccessfulRecord] | None
+    An array of input data records that were successfully written.
+recordsFailed: [DxTypes.PublishCaptureDataFailedRecord] | None    
+    An array of input data records that were not written.
+error: str | None
+    An error message if a problem was encountered.
+```
+
+### DxTypes.PublishCaptureDataSuccessfulRecord<a id="dxtypespublishcapturedatasuccessfulrecord"></a>
+
+A record that was published and written to a Data Capture.
+
+**Properties**
+
+```
+timestamp: str
+    The timestamp of the data record
+timeUnit: str
+    The format of the timestamp
+attributeId: str
+attributeValue: str
+```
+
+### DxTypes.PublishCaptureDataFailedRecord<a id="dxtypespublishcapturedatafailedrecord"></a>
+
+A record that was published but not written to a Data Capture.
+
+**Properties**
+
+```
+timestamp: str
+    The timestamp of the data record
+timeUnit: str
+    The format of the timestamp
+attributeId: str
+attributeValue: str
+message: str
+    Explains why the data record failed.
+```
+
+
+### DxTypes.StartCaptureResult<a id="dxtypesstartcaptureresult"></a>
+
+Result object for the DataCapture.startCapture operation.
+
+**Properties**
+
+```
+success: bool
+    Indicates if the action was successful
+captureId: str
+    The captureId of the Data Capture being started.
+startedAt: str | None
+    The timestamp at which the Data Capture was started (if successful).
+error: str | None
+    An error message if a problem was encountered.
+```
+
+
+### DxTypes.StopCaptureResult<a id="dxtypesstopcaptureresult"></a>
+
+Result object for the DataCapture.stopCapture operation.
+
+**Properties**
+
+```
+success: bool
+    Indicates if the action was successful
+captureId: str
+    The captureId of the Data Capture being stopped.
+stoppedAt: str | None
+    The timestamp at which the Data Capture was stopped (if successful).
+error: str | None
+    An error message if a problem was encountered.
+```
+
+
 ## Development<a id="development"></a>
 
 lone the repository with command `git clone https://github.com/Avista-Digital-Innovation/avista-digital-exchange-sdk.git`.
 
 Use VS Code with the Python extension to utilize formatting and code completion.
 
 Deployment related code is in the root directory and the package code is found in `src/avista_digital_exchange_sdk`.
 
 ## Deployment<a id="deployment"></a>
 
 Follow the steps below to build and push the new package version to PyPi. [(Python packaging reference used)](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
 
 **Steps**
 
-1. Update `CHANGELOG.md` with new release notes.queryTimeSeriesDatabaseWithFilters
+1. Update `CHANGELOG.md` with new release notes.
 2. Update `README.md` if necessary.
 3. PyPi deployment
    1. Update the package version in `pyproject.toml`. Follow [this versioning method](https://py-pkgs.org/07-releasing-versioning.html#version-numbering)
    2. From the root directory of the repository:
       1. Run `python3 -m build`
       2. Run `python3 -m twine upload dist/* ` to upload the new build to PyPi.
          1. Use username `__token__`
          2. Use your [PyPi authentication token](https://pypi.org/help/#apitoken) as the password. 
    3. Test that the new version is available in pip by running `pip3 install --upgrade avista-digital-exchange-sdk`.
 4. Push changes to git.
 5. Merge changes to `main`.
 6. Create a release branch from main with the name `release/YYYY_MM_DD_vXX.XX.XX` where XX.XX.XX is the new version number, and YYYY_MM_DD is the date the version was deployed.
 
+## Generating Python types and GraphQL Client from GraphQL Schema
+
+See instructions in src/avista_digital_exchange_sdk/graphql_codegen/README.md
+
+## Fix for py-graphql-mapper module
+
+The plugin was failing to assign the correct type for attributes of a schema type that were lists of other custom schema types (ie. IotEndpoint contains array of Properties and Telemetry).
+
+I edited the function _init_type(obj, fieldType, fieldName) in the file gql_init.py from commit bc0888b. There are conditions for different fieldTypes. I edited the condition if the field is a list. Changed
+'''
+    elif fieldType == list or (hasattr(fieldType, '__origin__') and fieldType.__origin__ == list):
+'''
+to
+'''
+    elif fieldType == list or (hasattr(fieldType, '__origin__') and fieldType.__origin__ == list) or "gql_types.list_" in str(fieldType):
+'''
+
 ## Resources<a id="resources"></a>
 
 1. [Avista Digital Exchange](https://energy.collaboratives.io/)
 2. [PyPi SDK project listing](https://pypi.org/project/avista-digital-exchange-sdk/)
 3. [GitHub project repository](https://github.com/Avista-Digital-Innovation/avista-digital-exchange-sdk)
 4. [Python package deployment tutorial](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
 5. [PyPi API Token](https://pypi.org/help/#apitoken)
```

### Comparing `avista_digital_exchange_sdk-0.2.1/README.md` & `avista_digital_exchange_sdk-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -29,14 +29,18 @@
       - [getEndpoint](#getendpoint)
       - [createEndpoint](#createendpoint)
       - [createModel](#createmodel)
       - [listEndpointLastValues](#listendpointlastvalues)
       - [queryByTimeRange](#querybytimerange)
       - [publish](#publish)
       - [updateEndpointProperties](#updateendpointproperties)
+    - [dataCapture](#datacapture)
+      - [publishData](#publishdata)
+      - [startCapture](#startcapture)
+      - [stopCapture](#stopcapture)
   - [Types](#types)
     - [User](#user)
     - [Organization](#organization)
     - [DataStore](#datastore-1)
       - [Methods](#methods)
         - [cd](#cd)
         - [ls](#ls)
@@ -50,16 +54,24 @@
     - [DataStoreFile](#datastorefile)
     - [DigitalTwinModel](#digitaltwinmodel)
     - [ModelProperty](#modelproperty)
     - [ModelTelemetry](#modeltelemetry)
     - [IotEndpoint](#iotendpoint)
     - [EndpointProperty](#endpointproperty)
     - [EndpointTelemetry](#endpointtelemetry)
+    - [DxTypes.CaptureDataRecordInput](#dxtypescapturedatarecordinput)
+    - [DxTypes.PublishCaptureDataResult](#dxtypespublishcapturedataresult)
+    - [DxTypes.PublishCaptureDataSuccessfulRecord](#dxtypespublishcapturedatasuccessfulrecord)
+    - [DxTypes.PublishCaptureDataFailedRecord](#dxtypespublishcapturedatafailedrecord)
+    - [DxTypes.StartCaptureResult](#dxtypesstartcaptureresult)
+    - [DxTypes.StopCaptureResult](#dxtypesstopcaptureresult)
   - [Development](#development)
   - [Deployment](#deployment)
+  - [Generating Python types and GraphQL Client from GraphQL Schema](#generating-python-types-and-graphql-client-from-graphql-schema)
+  - [Fix for py-graphql-mapper module](#fix-for-py-graphql-mapper-module)
   - [Resources](#resources)
 
 ## Getting Started<a id="getting-started"></a>
 
 1. Install the python package.
 
 ```
@@ -493,15 +505,15 @@
     "iotEndpointId.1234", 
     ["SOC", "V", "V - Setpoint"], 
     "2022-09-25T20:13:04.465Z", 
     "2022-09-26T20:58:04.465Z", 
     "./")
 ```
 
-#### publish<a id="publish"></a>
+#### publish<a id="iotpublish"></a>
 
 Publish telemetry values for an endpoint.  One or more data records can be written at one time.
 
 **Parameters**
 
 ```
 iotEndpointId :  str, required
@@ -602,19 +614,180 @@
 
 ```
 
 properties = {
     'moving': False
 }
 
-instance.iot.updateEndpointProperties(
+digitalExchange.iot.updateEndpointProperties(
      "iotEndpointId.1234",
      properties)
 ```
 
+---
+
+### dataCapture<a id="datacapture"></a>
+
+#### publishData<a id="publishdata"></a>
+
+Publish attribute values to an active Data Capture.
+
+**Parameters**
+
+```
+captureId :  str, required
+    The id of the Data Capture.
+data :  [DxTypes.CaptureDataRecordInput], required
+    Array of data records to write.  Each dict should contain the record's timestamp, timeUnit ("MILLISECONDS"), and a dicitonary of attributeId, value pairs. Example shown below.
+```
+
+**Return Type**
+
+[DxTypes.PublishCaptureDataResult](#dxtypespublishcapturedataresult)
+
+
+**Example**
+
+```
+# captureDataPublishSample.py
+import asyncio
+import time
+from avista_digital_exchange_sdk import AvistaDigitalExchange, DxTypes
+
+# Create an instance of the AvistaDigitalExchange SDK
+# You may use a user authentication token or the authentication token of the Data Capture
+digitalExchange = AvistaDigitalExchange(AUTHENTICATION_TOKEN_VALUE)
+print("Instantiated AvistaDigitalExchange instance with authentication token")
+
+# Specify the capture you are publishing data to.
+# NOTE: The capture must be in Capturing state to accept data
+captureId = YOUR_CAPTURE_ID
+
+def getCurrentMilliseconds():
+    return int(f'{time.time() * 1000}'.split('.')[0])
+
+async def publishDataExample():
+    # Prepare the data to be published
+    # Replace ATTRIBUTE_ID and ATTRIBUTE_VALUE
+    attributeValueMap = {
+        ATTRIBUTE_ID: ATTRIBUTE_VALUE,
+        ATTRIBUTE_ID: ATTRIBUTE_VALUE,
+        ATTRIBUTE_ID: ATTRIBUTE_VALUE,
+    }
+
+    data = [DxTypes.CaptureDataRecordInput(
+            timestamp=f'{getCurrentMilliseconds()}',
+            timeUnit="MILLISECONDS",
+            attributeValues=attributeValueMap)]
+    try:
+        print("Calling dataCapture.publishData")
+        result = await digitalExchange.dataCapture.publishData(
+            captureId=captureId, data=data)
+    except:
+        print("dataCapture.publishData failed")
+
+asyncio.run(publishDataExample())
+```
+
+#### startCapture<a id="startcapture"></a>
+
+Commands a Data Capture to begin collecting data. Capture must be in 'Ready' state for startCapture to succeed.
+
+**Parameters**
+
+```
+captureId :  str, required
+    The id of the Data Capture.
+```
+
+**Return Type**
+
+[DxTypes.StartCaptureResult](#dxtypesstartcaptureresult)
+
+
+**Example**
+
+```
+# captureDataPublishSample.py
+import asyncio
+import time
+from avista_digital_exchange_sdk import AvistaDigitalExchange, DxTypes
+
+# Create an instance of the AvistaDigitalExchange SDK
+# You may use a user authentication token or the authentication token of the Data Capture
+digitalExchange = AvistaDigitalExchange(AUTHENTICATION_TOKEN_VALUE)
+print("Instantiated AvistaDigitalExchange instance with authentication token")
+
+# Specify the capture you are starting.
+# NOTE: The capture must be in 'READY' state to accept data
+captureId = YOUR_CAPTURE_ID
+
+def getCurrentMilliseconds():
+    return int(f'{time.time() * 1000}'.split('.')[0])
+
+async def startCaptureExample():
+    try:
+        print("Calling dataCapture.startCapture")
+        result = await digitalExchange.dataCapture.startCapture(
+            captureId=captureId)
+    except:
+        print("dataCapture.startCapture failed")
+
+asyncio.run(startCaptureExample())
+```
+
+
+#### stopCapture<a id="stopcapture"></a>
+
+Commands a Data Capture to stop collecting data. Capture must be in 'CAPTURING' state for stopCapture to succeed.
+
+**Parameters**
+
+```
+captureId :  str, required
+    The id of the Data Capture.
+```
+
+**Return Type**
+
+[DxTypes.StopCaptureResult](#dxtypesstopcaptureresult)
+
+
+**Example**
+
+```
+# captureDataPublishSample.py
+import asyncio
+import time
+from avista_digital_exchange_sdk import AvistaDigitalExchange, DxTypes
+
+# Create an instance of the AvistaDigitalExchange SDK
+# You may use a user authentication token or the authentication token of the Data Capture
+digitalExchange = AvistaDigitalExchange(AUTHENTICATION_TOKEN_VALUE)
+print("Instantiated AvistaDigitalExchange instance with authentication token")
+
+# Specify the capture you are stopping.
+# NOTE: The capture must be in 'CAPTURING' state to be stopped.
+captureId = YOUR_CAPTURE_ID
+
+def getCurrentMilliseconds():
+    return int(f'{time.time() * 1000}'.split('.')[0])
+
+async def stopCaptureExample():
+    try:
+        print("Calling dataCapture.stopCapture")
+        result = await digitalExchange.dataCapture.stopCapture(
+            captureId=captureId)
+    except:
+        print("dataCapture.stopCapture failed")
+
+asyncio.run(stopCaptureExample())
+```
+
+
 
 ---
 
 ## Types<a id="types"></a>
 
 ### User<a id="user"></a>
 
@@ -928,42 +1101,162 @@
 name: str
     Name of the telemetry.
 description: str
 schemaType: str : "integer", "double", "string", "boolean", "dateTime", "duration"
     The type of the variable.
 ```
 
+### DxTypes.CaptureDataRecordInput<a id="dxtypescapturedatarecordinput"></a>
+
+A data record that is to be published to a Data Capture.
+
+**Properties**
+
+```
+timestamp: str
+    The timestamp of the data record
+timeUnit: str
+    The format of the timestamp
+attributeValues: dict
+    A dictionary containing the data to be written for the given timestmap. Key values should be attributeIds that map to the relevant attribute values. 
+```
+
+### DxTypes.PublishCaptureDataResult<a id="dxtypespublishcapturedataresult"></a>
+
+Result object for the DataCapture.publishData operation.
+
+**Properties**
+
+```
+success: bool
+    Indicates if the action was successful
+captureId: str
+    The captureId of the Data Capture published to.
+recordsWritten: [DxTypes.PublishCaptureDataSuccessfulRecord] | None
+    An array of input data records that were successfully written.
+recordsFailed: [DxTypes.PublishCaptureDataFailedRecord] | None    
+    An array of input data records that were not written.
+error: str | None
+    An error message if a problem was encountered.
+```
+
+### DxTypes.PublishCaptureDataSuccessfulRecord<a id="dxtypespublishcapturedatasuccessfulrecord"></a>
+
+A record that was published and written to a Data Capture.
+
+**Properties**
+
+```
+timestamp: str
+    The timestamp of the data record
+timeUnit: str
+    The format of the timestamp
+attributeId: str
+attributeValue: str
+```
+
+### DxTypes.PublishCaptureDataFailedRecord<a id="dxtypespublishcapturedatafailedrecord"></a>
+
+A record that was published but not written to a Data Capture.
+
+**Properties**
+
+```
+timestamp: str
+    The timestamp of the data record
+timeUnit: str
+    The format of the timestamp
+attributeId: str
+attributeValue: str
+message: str
+    Explains why the data record failed.
+```
+
+
+### DxTypes.StartCaptureResult<a id="dxtypesstartcaptureresult"></a>
+
+Result object for the DataCapture.startCapture operation.
+
+**Properties**
+
+```
+success: bool
+    Indicates if the action was successful
+captureId: str
+    The captureId of the Data Capture being started.
+startedAt: str | None
+    The timestamp at which the Data Capture was started (if successful).
+error: str | None
+    An error message if a problem was encountered.
+```
+
+
+### DxTypes.StopCaptureResult<a id="dxtypesstopcaptureresult"></a>
+
+Result object for the DataCapture.stopCapture operation.
+
+**Properties**
+
+```
+success: bool
+    Indicates if the action was successful
+captureId: str
+    The captureId of the Data Capture being stopped.
+stoppedAt: str | None
+    The timestamp at which the Data Capture was stopped (if successful).
+error: str | None
+    An error message if a problem was encountered.
+```
+
+
 ## Development<a id="development"></a>
 
 lone the repository with command `git clone https://github.com/Avista-Digital-Innovation/avista-digital-exchange-sdk.git`.
 
 Use VS Code with the Python extension to utilize formatting and code completion.
 
 Deployment related code is in the root directory and the package code is found in `src/avista_digital_exchange_sdk`.
 
 ## Deployment<a id="deployment"></a>
 
 Follow the steps below to build and push the new package version to PyPi. [(Python packaging reference used)](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
 
 **Steps**
 
-1. Update `CHANGELOG.md` with new release notes.queryTimeSeriesDatabaseWithFilters
+1. Update `CHANGELOG.md` with new release notes.
 2. Update `README.md` if necessary.
 3. PyPi deployment
    1. Update the package version in `pyproject.toml`. Follow [this versioning method](https://py-pkgs.org/07-releasing-versioning.html#version-numbering)
    2. From the root directory of the repository:
       1. Run `python3 -m build`
       2. Run `python3 -m twine upload dist/* ` to upload the new build to PyPi.
          1. Use username `__token__`
          2. Use your [PyPi authentication token](https://pypi.org/help/#apitoken) as the password. 
    3. Test that the new version is available in pip by running `pip3 install --upgrade avista-digital-exchange-sdk`.
 4. Push changes to git.
 5. Merge changes to `main`.
 6. Create a release branch from main with the name `release/YYYY_MM_DD_vXX.XX.XX` where XX.XX.XX is the new version number, and YYYY_MM_DD is the date the version was deployed.
 
+## Generating Python types and GraphQL Client from GraphQL Schema
+
+See instructions in src/avista_digital_exchange_sdk/graphql_codegen/README.md
+
+## Fix for py-graphql-mapper module
+
+The plugin was failing to assign the correct type for attributes of a schema type that were lists of other custom schema types (ie. IotEndpoint contains array of Properties and Telemetry).
+
+I edited the function _init_type(obj, fieldType, fieldName) in the file gql_init.py from commit bc0888b. There are conditions for different fieldTypes. I edited the condition if the field is a list. Changed
+'''
+    elif fieldType == list or (hasattr(fieldType, '__origin__') and fieldType.__origin__ == list):
+'''
+to
+'''
+    elif fieldType == list or (hasattr(fieldType, '__origin__') and fieldType.__origin__ == list) or "gql_types.list_" in str(fieldType):
+'''
+
 ## Resources<a id="resources"></a>
 
 1. [Avista Digital Exchange](https://energy.collaboratives.io/)
 2. [PyPi SDK project listing](https://pypi.org/project/avista-digital-exchange-sdk/)
 3. [GitHub project repository](https://github.com/Avista-Digital-Innovation/avista-digital-exchange-sdk)
 4. [Python package deployment tutorial](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
 5. [PyPi API Token](https://pypi.org/help/#apitoken)
```

### Comparing `avista_digital_exchange_sdk-0.2.1/pyproject.toml` & `avista_digital_exchange_sdk-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0","websocket-client","requests"] # , "pip-system-certs"
+requires = ["setuptools>=61.0","websocket-client","requests", "py-graphql-mapper", "ariadne-codegen"] # , "pip-system-certs"
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "avista_digital_exchange_sdk"
-version = "0.2.1"
+version = "0.3.0"
 authors = [
   { name="Justin Whicker", email="jwhicker@urbanova.org"},
   {  name="Jon Thompson", email="jon.thompson@avistacorp.com" }
 ]
 description = "SDK to programmatically access the Avista Digital Exchange"
 readme = "README.md"
```

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/client.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 import requests
 from . import globals
-import json
-import base64
-import websocket
 from .subscriptionClient import Subscription
+from .graphql_codegen.ariadne.graphql_client.client import Client as AriadneGraphqlClient
 
 
 class Client:
+    updatedGqlClient: AriadneGraphqlClient
 
     def __init__(self, token, stage, debug):
         APPSYNC_API_ENDPOINT_URL_dev = 'https://annsvlcb4vew7msipwjyzzvyhi.appsync-api.us-west-2.amazonaws.com/graphql'
         APPSYNC_API_ENDPOINT_URL_prod = 'https://rrfs7pb7ancybo7bom7uxcsaxq.appsync-api.us-west-2.amazonaws.com/graphql'
         self.token = token
         self._debug = debug
         self._stage = stage
         if self._stage == "PRODUCTION":
             self.APPSYNC_API_ENDPOINT_URL = APPSYNC_API_ENDPOINT_URL_prod
         else:
             self.APPSYNC_API_ENDPOINT_URL = APPSYNC_API_ENDPOINT_URL_dev
+        self.setupUpdatedGqlClient()
         return
 
+    def setupUpdatedGqlClient(self):
+        import httpx
+        headers = {'Accept': 'application/json',
+                   'Content-Type': 'application/json',
+                   'Authorization': self.token}
+        self.updatedGqlClient = AriadneGraphqlClient(url=self.APPSYNC_API_ENDPOINT_URL,
+                                                     headers=headers,
+                                                     http_client=httpx.AsyncClient(headers=headers, timeout=60))
+
     def performQuery(self, queryString):
         if self._debug:
             print(f'DEBUG - {queryString}')
         response = None
 
         try:
             with requests.Session() as session:
@@ -35,15 +44,15 @@
                              'Authorization': self.token},
                     json={'query': queryString}
                 )
         except Exception as e:
             raise e
         return response.json()
 
-    def performMutation(self, mutationString):
+    def performMutation(self, mutationString, jsonResult=True):
         if self._debug:
             print(f'DEBUG - {mutationString}')
         response = None
 
         try:
             with requests.Session() as session:
                 # Now we can simply post the request...
@@ -53,15 +62,18 @@
                     headers={'Accept': 'application/json',
                              'Content-Type': 'application/json',
                              'Authorization': self.token},
                     json={'query': mutationString}
                 )
         except Exception as error:
             raise error
-        return response.json()
+        if jsonResult:
+            return response.json()
+        else:
+            return response
 
     def getSubscriptionClient(self, subscriptionName, subscriptionQueryString, subscriptionMessageQueue, subscriptionErrorQueue):
         if self._debug:
             print(f'subscribing to {subscriptionQueryString}...')
         subscription = Subscription(
             self._debug, subscriptionName, subscriptionQueryString, self.APPSYNC_API_ENDPOINT_URL, self.token, subscriptionMessageQueue, subscriptionErrorQueue)
         return subscription
```

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/collaborativeUtil.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/collaborativeUtil.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/dataStoreUtil.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/dataStoreUtil.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/collaborative.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/collaborative.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/collaborative_member_organization.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/collaborative_member_organization.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/collaborative_member_user.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/collaborative_member_user.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/data_store.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/data_store.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/data_store_directory.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/data_store_directory.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/data_store_file.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/data_store_file.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/data_store_object.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/data_store_object.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/digital_twin_model.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/digital_twin_model.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/endpoint_last_values.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_last_values.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/endpoint_property.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_property.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/endpoint_property_input.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_property_input.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/endpoint_query_filter_input.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_query_filter_input.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry_data_record.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/endpoint_telemetry_data_record.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_attribute_value.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_attribute_value.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_data_record.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_data_record.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_data_record_error.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_data_record_error.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_data_record_input.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_data_record_input.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_data_record_with_errors.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_data_record_with_errors.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_endpoint.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_endpoint.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_endpoint_data.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_endpoint_data.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_endpoints_last_values_query_result.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_endpoints_last_values_query_result.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_generate_query_result_export.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_generate_query_result_export.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_query_by_time_range_result.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_query_by_time_range_result.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/iot_query_export.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/iot_query_export.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/model_property.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/model_property.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/model_property_input.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/model_property_input.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/model_telemetry.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/model_telemetry.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/model_telemetry_input.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/model_telemetry_input.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/organization.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/organization.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/presigned_url.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/presigned_url.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/publish_iot_data_result.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/publish_iot_data_result.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/server_response.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/server_response.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/service.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/service.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute_data.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_asset_attribute_data.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_asset_data.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_asset_data.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_assets_and_last_values_result.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_assets_and_last_values_result.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_db.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_db.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_dimension.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_dimension.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_generate_query_export_result.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_generate_query_export_result.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_input_record.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_input_record.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_measure_value.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_measure_value.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_publish_input.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_publish_input.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_publish_response.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_publish_response.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_query_export.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_query_export.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/time_series_query_result.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/time_series_query_result.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/timestream_query_result.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/timestream_query_result.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/data_types/user.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/data_types/user.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/exceptions.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_addServiceToCollaborative.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_addServiceToCollaborative.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_removeServiceFromCollaborative.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/collaborative_removeServiceFromCollaborative.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_cancelQuery.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_cancelQuery.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_createEndpoint.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_createEndpoint.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_createModel.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_createModel.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_generateQueryResultExport.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_generateQueryResultExport.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_publish.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_publish.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/iot_updateEndpointProperties.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/iot_updateEndpointProperties.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/mutation.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/mutation.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/storage_createDataStoreFile.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/storage_createDataStoreFile.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/storage_deleteDataStoreFile.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/storage_deleteDataStoreFile.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_cancelDatabaseQuery.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_cancelDatabaseQuery.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_generateQueryResultExportFile.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_generateQueryResultExportFile.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_publishToDatabase.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_mutations/timeSeriesDb_publishToDatabase.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/collaborative_getCollaborative.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/collaborative_getCollaborative.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativeServices.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativeServices.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaboratives.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaboratives.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativesServiceSharedWith.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/collaborative_listCollaborativesServiceSharedWith.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/iot_getEndpoint.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/iot_getEndpoint.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/iot_listEndpointLastValues.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/iot_listEndpointLastValues.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/iot_queryByTimeRange.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/iot_queryByTimeRange.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/query.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/query.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStore.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStore.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreDirectory.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreDirectory.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFile.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFile.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFileDownloadUrl.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/storage_getDataStoreFileDownloadUrl.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/storage_listDataStores.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/storage_listDataStores.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_getDatabase.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_getDatabase.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listAllAssetLastValues.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listAllAssetLastValues.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listDatabases.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_listDatabases.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabase.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabase.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabaseWithTimestreamQuery.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/timeSeriesDb_queryDatabaseWithTimestreamQuery.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_queries/user_getUserSession.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_queries/user_getUserSession.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyIotQueryExportComplete.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyIotQueryExportComplete.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyTimeSeriesQueryExportComplete.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_subscriptions/onNotifyTimeSeriesQueryExportComplete.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/graphql_subscriptions/subscription.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/graphql_subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/iotUtil.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/iotUtil.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,34 +84,37 @@
 
         filter = EndpointQueryFilterInput(iotEndpointId, attributeNames)
         endpointFilterInput = [filter]
         query = iot_queryByTimeRange(
             self._client, self._debug, endpointFilterInput, startTime, endTime)
         result = query.performQuery()
         queryId = result.queryId
-        print(
-            f'received query result chunk {result.resultChunkIndex}')
+        if self._debug:
+            print(
+                f'received query result chunk {result.resultChunkIndex}')
 
         def quitHandler(signum, frame):
             # Stop query
             if queryId is not None:
-                print("Cancelling query....")
+                if self._debug:
+                    print("Cancelling query....")
                 mutation = iot_cancelQuery(
                     self._client, self._debug, queryId)
                 cancelResult = mutation.performMutation()
             exit(1)
 
         signal.signal(signal.SIGINT, quitHandler)
 
         while result.nextToken is not None:
             query = iot_queryByTimeRange(
                 self._client, self._debug, endpointFilterInput, startTime, endTime, result.nextToken, result.clientToken, result.queryString, result.queryId)
             result = query.performQuery()
-            print(
-                f'received query result chunk {result.resultChunkIndex}')
+            if self._debug:
+                print(
+                    f'received query result chunk {result.resultChunkIndex}')
 
         # get onNotifyObject
         subscription = self._getSubscriptionToQueryExportFileCompletion(
             queryId)
 
         # Generate export file
         mutationResult = self._generateQueryResultFile(queryId, "CSV")
```

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk/subscriptionClient.py` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk/subscriptionClient.py`

 * *Files identical despite different names*

### Comparing `avista_digital_exchange_sdk-0.2.1/src/avista_digital_exchange_sdk.egg-info/PKG-INFO` & `avista_digital_exchange_sdk-0.3.0/src/avista_digital_exchange_sdk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avista-digital-exchange-sdk
-Version: 0.2.1
+Version: 0.3.0
 Summary: SDK to programmatically access the Avista Digital Exchange
 Author-email: Justin Whicker <jwhicker@urbanova.org>, Jon Thompson <jon.thompson@avistacorp.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -718,14 +718,18 @@
       - [getEndpoint](#getendpoint)
       - [createEndpoint](#createendpoint)
       - [createModel](#createmodel)
       - [listEndpointLastValues](#listendpointlastvalues)
       - [queryByTimeRange](#querybytimerange)
       - [publish](#publish)
       - [updateEndpointProperties](#updateendpointproperties)
+    - [dataCapture](#datacapture)
+      - [publishData](#publishdata)
+      - [startCapture](#startcapture)
+      - [stopCapture](#stopcapture)
   - [Types](#types)
     - [User](#user)
     - [Organization](#organization)
     - [DataStore](#datastore-1)
       - [Methods](#methods)
         - [cd](#cd)
         - [ls](#ls)
@@ -739,16 +743,24 @@
     - [DataStoreFile](#datastorefile)
     - [DigitalTwinModel](#digitaltwinmodel)
     - [ModelProperty](#modelproperty)
     - [ModelTelemetry](#modeltelemetry)
     - [IotEndpoint](#iotendpoint)
     - [EndpointProperty](#endpointproperty)
     - [EndpointTelemetry](#endpointtelemetry)
+    - [DxTypes.CaptureDataRecordInput](#dxtypescapturedatarecordinput)
+    - [DxTypes.PublishCaptureDataResult](#dxtypespublishcapturedataresult)
+    - [DxTypes.PublishCaptureDataSuccessfulRecord](#dxtypespublishcapturedatasuccessfulrecord)
+    - [DxTypes.PublishCaptureDataFailedRecord](#dxtypespublishcapturedatafailedrecord)
+    - [DxTypes.StartCaptureResult](#dxtypesstartcaptureresult)
+    - [DxTypes.StopCaptureResult](#dxtypesstopcaptureresult)
   - [Development](#development)
   - [Deployment](#deployment)
+  - [Generating Python types and GraphQL Client from GraphQL Schema](#generating-python-types-and-graphql-client-from-graphql-schema)
+  - [Fix for py-graphql-mapper module](#fix-for-py-graphql-mapper-module)
   - [Resources](#resources)
 
 ## Getting Started<a id="getting-started"></a>
 
 1. Install the python package.
 
 ```
@@ -1182,15 +1194,15 @@
     "iotEndpointId.1234", 
     ["SOC", "V", "V - Setpoint"], 
     "2022-09-25T20:13:04.465Z", 
     "2022-09-26T20:58:04.465Z", 
     "./")
 ```
 
-#### publish<a id="publish"></a>
+#### publish<a id="iotpublish"></a>
 
 Publish telemetry values for an endpoint.  One or more data records can be written at one time.
 
 **Parameters**
 
 ```
 iotEndpointId :  str, required
@@ -1291,19 +1303,180 @@
 
 ```
 
 properties = {
     'moving': False
 }
 
-instance.iot.updateEndpointProperties(
+digitalExchange.iot.updateEndpointProperties(
      "iotEndpointId.1234",
      properties)
 ```
 
+---
+
+### dataCapture<a id="datacapture"></a>
+
+#### publishData<a id="publishdata"></a>
+
+Publish attribute values to an active Data Capture.
+
+**Parameters**
+
+```
+captureId :  str, required
+    The id of the Data Capture.
+data :  [DxTypes.CaptureDataRecordInput], required
+    Array of data records to write.  Each dict should contain the record's timestamp, timeUnit ("MILLISECONDS"), and a dicitonary of attributeId, value pairs. Example shown below.
+```
+
+**Return Type**
+
+[DxTypes.PublishCaptureDataResult](#dxtypespublishcapturedataresult)
+
+
+**Example**
+
+```
+# captureDataPublishSample.py
+import asyncio
+import time
+from avista_digital_exchange_sdk import AvistaDigitalExchange, DxTypes
+
+# Create an instance of the AvistaDigitalExchange SDK
+# You may use a user authentication token or the authentication token of the Data Capture
+digitalExchange = AvistaDigitalExchange(AUTHENTICATION_TOKEN_VALUE)
+print("Instantiated AvistaDigitalExchange instance with authentication token")
+
+# Specify the capture you are publishing data to.
+# NOTE: The capture must be in Capturing state to accept data
+captureId = YOUR_CAPTURE_ID
+
+def getCurrentMilliseconds():
+    return int(f'{time.time() * 1000}'.split('.')[0])
+
+async def publishDataExample():
+    # Prepare the data to be published
+    # Replace ATTRIBUTE_ID and ATTRIBUTE_VALUE
+    attributeValueMap = {
+        ATTRIBUTE_ID: ATTRIBUTE_VALUE,
+        ATTRIBUTE_ID: ATTRIBUTE_VALUE,
+        ATTRIBUTE_ID: ATTRIBUTE_VALUE,
+    }
+
+    data = [DxTypes.CaptureDataRecordInput(
+            timestamp=f'{getCurrentMilliseconds()}',
+            timeUnit="MILLISECONDS",
+            attributeValues=attributeValueMap)]
+    try:
+        print("Calling dataCapture.publishData")
+        result = await digitalExchange.dataCapture.publishData(
+            captureId=captureId, data=data)
+    except:
+        print("dataCapture.publishData failed")
+
+asyncio.run(publishDataExample())
+```
+
+#### startCapture<a id="startcapture"></a>
+
+Commands a Data Capture to begin collecting data. Capture must be in 'Ready' state for startCapture to succeed.
+
+**Parameters**
+
+```
+captureId :  str, required
+    The id of the Data Capture.
+```
+
+**Return Type**
+
+[DxTypes.StartCaptureResult](#dxtypesstartcaptureresult)
+
+
+**Example**
+
+```
+# captureDataPublishSample.py
+import asyncio
+import time
+from avista_digital_exchange_sdk import AvistaDigitalExchange, DxTypes
+
+# Create an instance of the AvistaDigitalExchange SDK
+# You may use a user authentication token or the authentication token of the Data Capture
+digitalExchange = AvistaDigitalExchange(AUTHENTICATION_TOKEN_VALUE)
+print("Instantiated AvistaDigitalExchange instance with authentication token")
+
+# Specify the capture you are starting.
+# NOTE: The capture must be in 'READY' state to accept data
+captureId = YOUR_CAPTURE_ID
+
+def getCurrentMilliseconds():
+    return int(f'{time.time() * 1000}'.split('.')[0])
+
+async def startCaptureExample():
+    try:
+        print("Calling dataCapture.startCapture")
+        result = await digitalExchange.dataCapture.startCapture(
+            captureId=captureId)
+    except:
+        print("dataCapture.startCapture failed")
+
+asyncio.run(startCaptureExample())
+```
+
+
+#### stopCapture<a id="stopcapture"></a>
+
+Commands a Data Capture to stop collecting data. Capture must be in 'CAPTURING' state for stopCapture to succeed.
+
+**Parameters**
+
+```
+captureId :  str, required
+    The id of the Data Capture.
+```
+
+**Return Type**
+
+[DxTypes.StopCaptureResult](#dxtypesstopcaptureresult)
+
+
+**Example**
+
+```
+# captureDataPublishSample.py
+import asyncio
+import time
+from avista_digital_exchange_sdk import AvistaDigitalExchange, DxTypes
+
+# Create an instance of the AvistaDigitalExchange SDK
+# You may use a user authentication token or the authentication token of the Data Capture
+digitalExchange = AvistaDigitalExchange(AUTHENTICATION_TOKEN_VALUE)
+print("Instantiated AvistaDigitalExchange instance with authentication token")
+
+# Specify the capture you are stopping.
+# NOTE: The capture must be in 'CAPTURING' state to be stopped.
+captureId = YOUR_CAPTURE_ID
+
+def getCurrentMilliseconds():
+    return int(f'{time.time() * 1000}'.split('.')[0])
+
+async def stopCaptureExample():
+    try:
+        print("Calling dataCapture.stopCapture")
+        result = await digitalExchange.dataCapture.stopCapture(
+            captureId=captureId)
+    except:
+        print("dataCapture.stopCapture failed")
+
+asyncio.run(stopCaptureExample())
+```
+
+
 
 ---
 
 ## Types<a id="types"></a>
 
 ### User<a id="user"></a>
 
@@ -1617,42 +1790,162 @@
 name: str
     Name of the telemetry.
 description: str
 schemaType: str : "integer", "double", "string", "boolean", "dateTime", "duration"
     The type of the variable.
 ```
 
+### DxTypes.CaptureDataRecordInput<a id="dxtypescapturedatarecordinput"></a>
+
+A data record that is to be published to a Data Capture.
+
+**Properties**
+
+```
+timestamp: str
+    The timestamp of the data record
+timeUnit: str
+    The format of the timestamp
+attributeValues: dict
+    A dictionary containing the data to be written for the given timestmap. Key values should be attributeIds that map to the relevant attribute values. 
+```
+
+### DxTypes.PublishCaptureDataResult<a id="dxtypespublishcapturedataresult"></a>
+
+Result object for the DataCapture.publishData operation.
+
+**Properties**
+
+```
+success: bool
+    Indicates if the action was successful
+captureId: str
+    The captureId of the Data Capture published to.
+recordsWritten: [DxTypes.PublishCaptureDataSuccessfulRecord] | None
+    An array of input data records that were successfully written.
+recordsFailed: [DxTypes.PublishCaptureDataFailedRecord] | None    
+    An array of input data records that were not written.
+error: str | None
+    An error message if a problem was encountered.
+```
+
+### DxTypes.PublishCaptureDataSuccessfulRecord<a id="dxtypespublishcapturedatasuccessfulrecord"></a>
+
+A record that was published and written to a Data Capture.
+
+**Properties**
+
+```
+timestamp: str
+    The timestamp of the data record
+timeUnit: str
+    The format of the timestamp
+attributeId: str
+attributeValue: str
+```
+
+### DxTypes.PublishCaptureDataFailedRecord<a id="dxtypespublishcapturedatafailedrecord"></a>
+
+A record that was published but not written to a Data Capture.
+
+**Properties**
+
+```
+timestamp: str
+    The timestamp of the data record
+timeUnit: str
+    The format of the timestamp
+attributeId: str
+attributeValue: str
+message: str
+    Explains why the data record failed.
+```
+
+
+### DxTypes.StartCaptureResult<a id="dxtypesstartcaptureresult"></a>
+
+Result object for the DataCapture.startCapture operation.
+
+**Properties**
+
+```
+success: bool
+    Indicates if the action was successful
+captureId: str
+    The captureId of the Data Capture being started.
+startedAt: str | None
+    The timestamp at which the Data Capture was started (if successful).
+error: str | None
+    An error message if a problem was encountered.
+```
+
+
+### DxTypes.StopCaptureResult<a id="dxtypesstopcaptureresult"></a>
+
+Result object for the DataCapture.stopCapture operation.
+
+**Properties**
+
+```
+success: bool
+    Indicates if the action was successful
+captureId: str
+    The captureId of the Data Capture being stopped.
+stoppedAt: str | None
+    The timestamp at which the Data Capture was stopped (if successful).
+error: str | None
+    An error message if a problem was encountered.
+```
+
+
 ## Development<a id="development"></a>
 
 lone the repository with command `git clone https://github.com/Avista-Digital-Innovation/avista-digital-exchange-sdk.git`.
 
 Use VS Code with the Python extension to utilize formatting and code completion.
 
 Deployment related code is in the root directory and the package code is found in `src/avista_digital_exchange_sdk`.
 
 ## Deployment<a id="deployment"></a>
 
 Follow the steps below to build and push the new package version to PyPi. [(Python packaging reference used)](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
 
 **Steps**
 
-1. Update `CHANGELOG.md` with new release notes.queryTimeSeriesDatabaseWithFilters
+1. Update `CHANGELOG.md` with new release notes.
 2. Update `README.md` if necessary.
 3. PyPi deployment
    1. Update the package version in `pyproject.toml`. Follow [this versioning method](https://py-pkgs.org/07-releasing-versioning.html#version-numbering)
    2. From the root directory of the repository:
       1. Run `python3 -m build`
       2. Run `python3 -m twine upload dist/* ` to upload the new build to PyPi.
          1. Use username `__token__`
          2. Use your [PyPi authentication token](https://pypi.org/help/#apitoken) as the password. 
    3. Test that the new version is available in pip by running `pip3 install --upgrade avista-digital-exchange-sdk`.
 4. Push changes to git.
 5. Merge changes to `main`.
 6. Create a release branch from main with the name `release/YYYY_MM_DD_vXX.XX.XX` where XX.XX.XX is the new version number, and YYYY_MM_DD is the date the version was deployed.
 
+## Generating Python types and GraphQL Client from GraphQL Schema
+
+See instructions in src/avista_digital_exchange_sdk/graphql_codegen/README.md
+
+## Fix for py-graphql-mapper module
+
+The plugin was failing to assign the correct type for attributes of a schema type that were lists of other custom schema types (ie. IotEndpoint contains array of Properties and Telemetry).
+
+I edited the function _init_type(obj, fieldType, fieldName) in the file gql_init.py from commit bc0888b. There are conditions for different fieldTypes. I edited the condition if the field is a list. Changed
+'''
+    elif fieldType == list or (hasattr(fieldType, '__origin__') and fieldType.__origin__ == list):
+'''
+to
+'''
+    elif fieldType == list or (hasattr(fieldType, '__origin__') and fieldType.__origin__ == list) or "gql_types.list_" in str(fieldType):
+'''
+
 ## Resources<a id="resources"></a>
 
 1. [Avista Digital Exchange](https://energy.collaboratives.io/)
 2. [PyPi SDK project listing](https://pypi.org/project/avista-digital-exchange-sdk/)
 3. [GitHub project repository](https://github.com/Avista-Digital-Innovation/avista-digital-exchange-sdk)
 4. [Python package deployment tutorial](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
 5. [PyPi API Token](https://pypi.org/help/#apitoken)
```

