# Comparing `tmp/klaviyo-api-2.0.2.tar.gz` & `tmp/klaviyo-api-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klaviyo-api-2.0.2.tar", last modified: Fri Jun  9 19:11:08 2023, max compression
+gzip compressed data, was "/home/jenkins/build/workspace/dev-team/DevX/generateSDKs/pip/dist/tmpk6guwiwm/klaviyo-api-3.0.0.tar", last modified: Thu Jun 15 15:53:59 2023, max compression
```

## Comparing `klaviyo-api-2.0.2.tar` & `klaviyo-api-3.0.0.tar`

### file list

```diff
@@ -1,252 +1,246 @@
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-06-09 19:11:08.222437 klaviyo-api-2.0.2/
--rw-r--r--   0 local      (503) staff       (20)     1063 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/LICENSE
--rw-r--r--   0 local      (503) staff       (20)    55411 2023-06-09 19:11:08.223169 klaviyo-api-2.0.2/PKG-INFO
--rw-r--r--   0 local      (503) staff       (20)    54894 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/README.md
--rw-r--r--   0 local      (503) staff       (20)      103 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/pyproject.toml
--rw-r--r--   0 local      (503) staff       (20)      801 2023-06-09 19:11:08.224583 klaviyo-api-2.0.2/setup.cfg
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-06-09 19:11:07.979222 klaviyo-api-2.0.2/src/
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-06-09 19:11:07.984390 klaviyo-api-2.0.2/src/klaviyo_api/
--rw-r--r--   0 local      (503) staff       (20)      130 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/klaviyo_api/__init__.py
--rw-r--r--   0 local      (503) staff       (20)      501 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/klaviyo_api/custom_retry.py
--rw-r--r--   0 local      (503) staff       (20)    25983 2023-06-09 19:10:52.000000 klaviyo-api-2.0.2/src/klaviyo_api/wrapper.py
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-06-09 19:11:07.988615 klaviyo-api-2.0.2/src/klaviyo_api.egg-info/
--rw-r--r--   0 local      (503) staff       (20)    55411 2023-06-09 19:11:07.000000 klaviyo-api-2.0.2/src/klaviyo_api.egg-info/PKG-INFO
--rw-r--r--   0 local      (503) staff       (20)    15129 2023-06-09 19:11:07.000000 klaviyo-api-2.0.2/src/klaviyo_api.egg-info/SOURCES.txt
--rw-r--r--   0 local      (503) staff       (20)        1 2023-06-09 19:11:07.000000 klaviyo-api-2.0.2/src/klaviyo_api.egg-info/dependency_links.txt
--rw-r--r--   0 local      (503) staff       (20)      119 2023-06-09 19:11:07.000000 klaviyo-api-2.0.2/src/klaviyo_api.egg-info/requires.txt
--rw-r--r--   0 local      (503) staff       (20)       27 2023-06-09 19:11:07.000000 klaviyo-api-2.0.2/src/klaviyo_api.egg-info/top_level.txt
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-06-09 19:11:07.994296 klaviyo-api-2.0.2/src/openapi_client/
--rw-r--r--   0 local      (503) staff       (20)      788 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/openapi_client/__init__.py
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-06-09 19:11:08.008558 klaviyo-api-2.0.2/src/openapi_client/api/
--rw-r--r--   0 local      (503) staff       (20)      220 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/openapi_client/api/__init__.py
--rw-r--r--   0 local      (503) staff       (20)   108410 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/campaigns_api.py
--rw-r--r--   0 local      (503) staff       (20)   351426 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/catalogs_api.py
--rw-r--r--   0 local      (503) staff       (20)    19728 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/client_api.py
--rw-r--r--   0 local      (503) staff       (20)     7236 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/data_privacy_api.py
--rw-r--r--   0 local      (503) staff       (20)    58131 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/events_api.py
--rw-r--r--   0 local      (503) staff       (20)   108931 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/flows_api.py
--rw-r--r--   0 local      (503) staff       (20)    70516 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/lists_api.py
--rw-r--r--   0 local      (503) staff       (20)    21844 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/metrics_api.py
--rw-r--r--   0 local      (503) staff       (20)    86332 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/profiles_api.py
--rw-r--r--   0 local      (503) staff       (20)    48324 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/segments_api.py
--rw-r--r--   0 local      (503) staff       (20)   147862 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/tags_api.py
--rw-r--r--   0 local      (503) staff       (20)    42670 2023-06-09 19:10:51.000000 klaviyo-api-2.0.2/src/openapi_client/api/templates_api.py
--rw-r--r--   0 local      (503) staff       (20)    39451 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/openapi_client/api_client.py
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-06-09 19:11:08.009513 klaviyo-api-2.0.2/src/openapi_client/apis/
--rw-r--r--   0 local      (503) staff       (20)     1084 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/openapi_client/apis/__init__.py
--rw-r--r--   0 local      (503) staff       (20)    17158 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/openapi_client/configuration.py
--rw-r--r--   0 local      (503) staff       (20)     5120 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/openapi_client/exceptions.py
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-06-09 19:11:08.220023 klaviyo-api-2.0.2/src/openapi_client/model/
--rw-r--r--   0 local      (503) staff       (20)      348 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/openapi_client/model/__init__.py
--rw-r--r--   0 local      (503) staff       (20)    11834 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/audiences_sub_object.py
--rw-r--r--   0 local      (503) staff       (20)    11849 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_clone_query.py
--rw-r--r--   0 local      (503) staff       (20)    12354 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_clone_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11954 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_clone_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11859 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12364 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    13914 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11633 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12011 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_assign_template_query.py
--rw-r--r--   0 local      (503) staff       (20)    12566 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_assign_template_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12055 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_assign_template_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11750 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12001 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_partial_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12786 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_partial_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12109 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_partial_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11930 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_partial_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12667 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_partial_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    13373 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_partial_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12082 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_recipient_estimation_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12744 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11768 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11999 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_recipient_estimation_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11931 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12487 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11675 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11762 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12002 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_partial_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12848 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11850 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11981 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_bulk_create_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11981 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_bulk_delete_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11981 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_bulk_update_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12022 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12671 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12179 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11930 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    13136 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    13243 2023-06-09 19:10:48.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12022 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_delete_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12671 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12179 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12422 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_delete_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11750 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12114 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_item_op.py
--rw-r--r--   0 local      (503) staff       (20)    12022 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12671 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12179 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11930 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    13736 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11663 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12102 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query_resource_object_relationships.py
--rw-r--r--   0 local      (503) staff       (20)    12225 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items.py
--rw-r--r--   0 local      (503) staff       (20)    12137 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11921 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_bulk_create_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11921 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_bulk_delete_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11921 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_bulk_update_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12121 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_category_op.py
--rw-r--r--   0 local      (503) staff       (20)    11982 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12603 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12074 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11890 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    13040 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    17029 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12122 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query_resource_object_relationships.py
--rw-r--r--   0 local      (503) staff       (20)    12235 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories.py
--rw-r--r--   0 local      (503) staff       (20)    12172 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11982 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_delete_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12603 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12074 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12374 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_delete_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11690 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11982 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12603 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12074 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11890 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    13632 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    15281 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11966 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_bulk_create_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11966 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_bulk_delete_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11966 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_bulk_update_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12012 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12654 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12143 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11920 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    13119 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    19026 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12012 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_delete_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12654 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12143 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12410 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_delete_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11735 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12012 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12654 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12143 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11920 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    13066 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    17148 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    13057 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/content_sub_object.py
--rw-r--r--   0 local      (503) staff       (20)    12002 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/data_privacy_create_deletion_job_query.py
--rw-r--r--   0 local      (503) staff       (20)    12608 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12449 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11879 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/data_privacy_deletion_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11829 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/event_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12313 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/event_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    17076 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/event_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11588 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/event_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11573 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/flow_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11819 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/flow_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12538 2023-06-09 19:10:49.000000 klaviyo-api-2.0.2/src/openapi_client/model/flow_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11764 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/flow_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11999 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/get_create_variants_jobs5_xx_response.py
--rw-r--r--   0 local      (503) staff       (20)    12816 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11775 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner_source.py
--rw-r--r--   0 local      (503) staff       (20)    11819 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/list_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12296 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/list_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11668 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/list_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11573 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/list_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11831 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/list_members_add_query.py
--rw-r--r--   0 local      (503) staff       (20)    11980 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/list_members_add_query_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11840 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/list_members_delete_query.py
--rw-r--r--   0 local      (503) staff       (20)    11890 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/list_partial_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12625 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/list_partial_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11750 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/metric_aggregate_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11869 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/metric_aggregate_query.py
--rw-r--r--   0 local      (503) staff       (20)    12424 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/metric_aggregate_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    21013 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/metric_aggregate_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11996 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/metric_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    11910 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/onsite_profile_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12408 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/onsite_profile_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    15425 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/onsite_profile_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11960 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/onsite_subscription_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12493 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/onsite_subscription_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    13508 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/onsite_subscription_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11849 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12347 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    15156 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11618 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_enum.py
--rw-r--r--   0 local      (503) staff       (20)    13961 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_location.py
--rw-r--r--   0 local      (503) staff       (20)    11301 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_location_latitude.py
--rw-r--r--   0 local      (503) staff       (20)    11304 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_location_longitude.py
--rw-r--r--   0 local      (503) staff       (20)    11920 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_partial_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12725 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_partial_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12041 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_subscription_bulk_create_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12026 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_suppression_bulk_create_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12071 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_unsubscription_bulk_create_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12056 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/profile_unsuppression_bulk_create_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11618 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/segment_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11920 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/segment_partial_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12586 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/segment_partial_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11632 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/segment_partial_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11612 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/send_options_sub_object.py
--rw-r--r--   0 local      (503) staff       (20)    13115 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/send_strategy_sub_object.py
--rw-r--r--   0 local      (503) staff       (20)    12702 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/static_schedule_options.py
--rw-r--r--   0 local      (503) staff       (20)    11547 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/sto_schedule_options.py
--rw-r--r--   0 local      (503) staff       (20)    12979 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/subscription.py
--rw-r--r--   0 local      (503) staff       (20)    12200 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/subscription_channels.py
--rw-r--r--   0 local      (503) staff       (20)    11991 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/subscription_create_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12668 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/subscription_create_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12750 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/subscription_create_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11693 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/subscription_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11598 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/suppression.py
--rw-r--r--   0 local      (503) staff       (20)    11981 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/suppression_create_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12651 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/suppression_create_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11983 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/suppression_create_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11770 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_campaign_op.py
--rw-r--r--   0 local      (503) staff       (20)    11970 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_campaign_op_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11809 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12279 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12174 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11558 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11730 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_flow_op.py
--rw-r--r--   0 local      (503) staff       (20)    11926 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_flow_op_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11860 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_group_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12366 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_group_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11858 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_group_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11645 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_group_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11860 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_group_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12568 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_group_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11881 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_group_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11730 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_list_op.py
--rw-r--r--   0 local      (503) staff       (20)    11926 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_list_op_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11760 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_segment_op.py
--rw-r--r--   0 local      (503) staff       (20)    11959 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_segment_op_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11809 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12469 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11625 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tag_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11849 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_clone_query.py
--rw-r--r--   0 local      (503) staff       (20)    12354 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_clone_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12223 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_clone_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11859 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12364 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12887 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11633 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11859 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_render_query.py
--rw-r--r--   0 local      (503) staff       (20)    12364 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_render_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12898 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_render_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11859 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12570 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12475 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/template_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12184 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/throttled_schedule_options.py
--rw-r--r--   0 local      (503) staff       (20)    13204 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/tracking_options_sub_object.py
--rw-r--r--   0 local      (503) staff       (20)    12011 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/unsubscription_create_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12702 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/unsubscription_create_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12305 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/unsubscription_create_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12001 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/unsuppression_create_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12685 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/unsuppression_create_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11989 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/unsuppression_create_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11845 2023-06-09 19:10:50.000000 klaviyo-api-2.0.2/src/openapi_client/model/utm_params_sub_object.py
--rw-r--r--   0 local      (503) staff       (20)    82630 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/openapi_client/model_utils.py
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-06-09 19:11:08.221569 klaviyo-api-2.0.2/src/openapi_client/models/
--rw-r--r--   0 local      (503) staff       (20)    22673 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/openapi_client/models/__init__.py
--rw-r--r--   0 local      (503) staff       (20)    14324 2023-06-09 19:10:53.000000 klaviyo-api-2.0.2/src/openapi_client/rest.py
+drwxrwxr-x   0 jenkins    (500) jenkins    (500)        0 2023-06-15 15:53:59.000000 klaviyo-api-3.0.0/
+-rw-r--r--   0 jenkins    (500) jenkins    (500)     1063 2023-06-15 15:53:54.000000 klaviyo-api-3.0.0/LICENSE
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)      801 2023-06-15 15:53:59.000000 klaviyo-api-3.0.0/setup.cfg
+drwxrwxr-x   0 jenkins    (500) jenkins    (500)        0 2023-06-15 15:53:59.000000 klaviyo-api-3.0.0/src/
+drwxrwxr-x   0 jenkins    (500) jenkins    (500)        0 2023-06-15 15:53:59.000000 klaviyo-api-3.0.0/src/klaviyo_api/
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    25839 2023-06-15 15:53:53.000000 klaviyo-api-3.0.0/src/klaviyo_api/wrapper.py
+-rw-r--r--   0 jenkins    (500) jenkins    (500)      501 2023-06-15 15:53:54.000000 klaviyo-api-3.0.0/src/klaviyo_api/custom_retry.py
+-rw-r--r--   0 jenkins    (500) jenkins    (500)      130 2023-06-15 15:53:54.000000 klaviyo-api-3.0.0/src/klaviyo_api/__init__.py
+drwxrwxr-x   0 jenkins    (500) jenkins    (500)        0 2023-06-15 15:53:59.000000 klaviyo-api-3.0.0/src/klaviyo_api.egg-info/
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)      119 2023-06-15 15:53:59.000000 klaviyo-api-3.0.0/src/klaviyo_api.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)        1 2023-06-15 15:53:59.000000 klaviyo-api-3.0.0/src/klaviyo_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)       27 2023-06-15 15:53:59.000000 klaviyo-api-3.0.0/src/klaviyo_api.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    14690 2023-06-15 15:53:59.000000 klaviyo-api-3.0.0/src/klaviyo_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    54926 2023-06-15 15:53:59.000000 klaviyo-api-3.0.0/src/klaviyo_api.egg-info/PKG-INFO
+drwxrwxr-x   0 jenkins    (500) jenkins    (500)        0 2023-06-15 15:53:59.000000 klaviyo-api-3.0.0/src/openapi_client/
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)     5120 2023-06-15 15:53:54.000000 klaviyo-api-3.0.0/src/openapi_client/exceptions.py
+drwxrwxr-x   0 jenkins    (500) jenkins    (500)        0 2023-06-15 15:53:59.000000 klaviyo-api-3.0.0/src/openapi_client/api/
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    15356 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/api/accounts_api.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)   108547 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/api/flows_api.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)   350561 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/api/catalogs_api.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    70258 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/api/lists_api.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    86140 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/api/profiles_api.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)   147836 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/api/tags_api.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    48132 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/api/segments_api.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)     7236 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/api/data_privacy_api.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    58101 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/api/events_api.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    21844 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/api/metrics_api.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)      219 2023-06-15 15:53:54.000000 klaviyo-api-3.0.0/src/openapi_client/api/__init__.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    42670 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/api/templates_api.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)   108302 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/api/campaigns_api.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    39434 2023-06-15 15:53:54.000000 klaviyo-api-3.0.0/src/openapi_client/api_client.py
+drwxrwxr-x   0 jenkins    (500) jenkins    (500)        0 2023-06-15 15:53:59.000000 klaviyo-api-3.0.0/src/openapi_client/models/
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    21956 2023-06-15 15:53:54.000000 klaviyo-api-3.0.0/src/openapi_client/models/__init__.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    82630 2023-06-15 15:53:54.000000 klaviyo-api-3.0.0/src/openapi_client/model_utils.py
+drwxrwxr-x   0 jenkins    (500) jenkins    (500)        0 2023-06-15 15:53:59.000000 klaviyo-api-3.0.0/src/openapi_client/model/
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11890 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12022 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_delete_job_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12816 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12074 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_update_job_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11982 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_create_job_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12026 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/profile_suppression_bulk_create_job_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11980 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/list_members_add_query_data_inner.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12422 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_delete_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    13115 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/send_strategy_sub_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11989 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/unsuppression_create_job_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12744 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12538 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/flow_update_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11966 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_bulk_delete_job_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12305 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/unsubscription_create_job_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11829 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/event_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12603 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_create_job_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11690 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12671 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_create_job_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    21013 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/metric_aggregate_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12041 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/profile_subscription_bulk_create_job_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12654 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12022 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_create_job_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12174 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11859 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11920 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/segment_partial_update_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12671 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11735 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12887 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/template_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12625 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/list_partial_update_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12074 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12179 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_update_job_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11859 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/template_render_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11926 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_flow_op_data_inner.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11304 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/profile_location_longitude.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11859 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/template_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12449 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11663 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_update_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11930 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12410 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_delete_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11618 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/segment_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12074 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_create_job_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12122 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_create_query_resource_object_relationships.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12184 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/throttled_schedule_options.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11573 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/flow_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    13736 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_update_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11859 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/template_update_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12586 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/segment_partial_update_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11890 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/list_partial_update_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11926 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_list_op_data_inner.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12011 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_message_assign_template_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12475 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/template_update_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12347 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/profile_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11981 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/suppression_create_job_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12001 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_message_partial_update_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11301 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/profile_location_latitude.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12114 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_item_op.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11858 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_group_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11920 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_update_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12011 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/unsubscription_create_job_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12058 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_category_op_data_inner.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11840 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/list_members_delete_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12685 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/unsuppression_create_job_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11633 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11750 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12109 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_message_partial_update_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12179 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_create_job_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11981 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_bulk_update_job_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12608 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12143 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12001 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/unsuppression_create_job_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12143 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12848 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11819 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/flow_update_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12424 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/metric_aggregate_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12200 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/subscription_channels.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12012 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_create_job_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12603 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_update_job_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    19026 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11819 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/list_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12487 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_send_job_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11618 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/profile_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12671 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_update_job_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    13243 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11982 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_delete_job_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11625 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_update_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    13040 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11981 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_bulk_delete_job_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11645 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_group_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11965 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11675 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_send_job_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    13066 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_update_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12082 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_recipient_estimation_job_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11764 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/flow_update_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11920 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/profile_partial_update_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12702 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/static_schedule_options.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12143 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11834 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/audiences_sub_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11890 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_update_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    13373 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_partial_update_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12279 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12651 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/suppression_create_job_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11869 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/metric_aggregate_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    17076 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/event_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12022 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_update_job_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11983 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/suppression_create_job_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    13204 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tracking_options_sub_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11588 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/event_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12354 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_clone_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11996 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/metric_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12469 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_update_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11668 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/list_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11959 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_segment_op_data_inner.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    13057 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/content_sub_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    13914 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    13961 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/profile_location.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11845 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/utm_params_sub_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11849 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_clone_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11921 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_bulk_create_job_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12296 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/list_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11750 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_message_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    15156 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/profile_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12568 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_group_update_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12898 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/template_render_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    13136 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11730 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_list_op.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12179 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11750 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/metric_aggregate_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11598 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/suppression.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11849 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/profile_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12786 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_message_partial_update_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    13119 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12012 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_update_job_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11860 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_group_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11921 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_bulk_update_job_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12223 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/template_clone_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12654 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12354 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/template_clone_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12668 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/subscription_create_job_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11612 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/send_options_sub_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11632 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/segment_partial_update_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12364 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    17029 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11851 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_category_op.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11966 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_bulk_update_job_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12364 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/template_render_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    13632 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_update_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11921 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_bulk_delete_job_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11860 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_group_update_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12002 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/data_privacy_create_deletion_job_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11881 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_group_update_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11966 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_bulk_create_job_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12366 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_group_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    17148 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_update_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11770 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_campaign_op.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11991 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/subscription_create_job_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11850 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11768 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11981 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_bulk_create_job_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11762 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_send_job_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)      348 2023-06-15 15:53:54.000000 klaviyo-api-3.0.0/src/openapi_client/model/__init__.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12002 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_send_job_partial_update_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11879 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/data_privacy_deletion_job_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12313 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/event_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11809 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11760 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_segment_op.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11831 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/list_members_add_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12654 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12979 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/subscription.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11930 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_partial_update_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11999 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_recipient_estimation_job_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12364 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/template_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11730 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_flow_op.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    15281 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_update_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11982 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_update_job_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11954 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_clone_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12137 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items_data_inner.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12566 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_message_assign_template_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11999 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/get_create_variants_jobs5_xx_response.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12750 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/subscription_create_job_create_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11547 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/sto_schedule_options.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11931 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_send_job_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11930 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_update_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11573 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/list_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12374 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_delete_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11775 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner_source.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12732 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/profile_partial_update_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12056 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/profile_unsuppression_bulk_create_job_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12603 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12702 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/unsubscription_create_job_create_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12225 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11849 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/template_clone_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11633 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/template_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11558 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12071 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/profile_unsubscription_bulk_create_job_enum.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11920 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11809 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_update_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12667 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_partial_update_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    11970 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/tag_campaign_op_data_inner.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12102 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_update_query_resource_object_relationships.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12012 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_delete_job_create_query.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12570 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/template_update_query_resource_object.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    15428 2023-06-15 15:53:51.000000 klaviyo-api-3.0.0/src/openapi_client/model/profile_partial_update_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    12055 2023-06-15 15:53:50.000000 klaviyo-api-3.0.0/src/openapi_client/model/campaign_message_assign_template_query_resource_object_attributes.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    14324 2023-06-15 15:53:54.000000 klaviyo-api-3.0.0/src/openapi_client/rest.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)      788 2023-06-15 15:53:54.000000 klaviyo-api-3.0.0/src/openapi_client/__init__.py
+drwxrwxr-x   0 jenkins    (500) jenkins    (500)        0 2023-06-15 15:53:59.000000 klaviyo-api-3.0.0/src/openapi_client/apis/
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)     1086 2023-06-15 15:53:54.000000 klaviyo-api-3.0.0/src/openapi_client/apis/__init__.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    17158 2023-06-15 15:53:54.000000 klaviyo-api-3.0.0/src/openapi_client/configuration.py
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    54373 2023-06-15 15:53:54.000000 klaviyo-api-3.0.0/README.md
+-rw-r--r--   0 jenkins    (500) jenkins    (500)      103 2023-06-15 15:53:54.000000 klaviyo-api-3.0.0/pyproject.toml
+-rw-rw-r--   0 jenkins    (500) jenkins    (500)    54926 2023-06-15 15:53:59.000000 klaviyo-api-3.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `klaviyo-api-2.0.2/LICENSE` & `klaviyo-api-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.2/PKG-INFO` & `klaviyo-api-3.0.0/src/klaviyo_api.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: klaviyo-api
-Version: 2.0.2
+Version: 3.0.0
 Summary: Klaviyo Python SDK
 Home-page: https://github.com/klaviyo/klaviyo-api-python
 Author: Klaviyo Developers
 Author-email: developers@klaviyo.com
+License: UNKNOWN
 Project-URL: API Docs, https://developers.klaviyo.com/en/reference/api_overview
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Klaviyo Python SDK
 
-- SDK version: 2.0.2
-- API revision: 2023-02-22
+- SDK version: 3.0.0
+- API revision: 2023-06-15
 
 ## Helpful Resources
 
-- [API Reference](https://developers.klaviyo.com/en/v2023-02-22/reference)
-- [API Guides](https://developers.klaviyo.com/en/v2023-02-22/docs)
+- [API Reference](https://developers.klaviyo.com/en/v2023-06-15/reference)
+- [API Guides](https://developers.klaviyo.com/en/v2023-06-15/docs)
 - [Postman Workspace](https://www.postman.com/klaviyo/workspace/klaviyo-developers)
 - [Interactive Guide (Jupyter Notebook)](https://github.com/klaviyo-labs/klaviyo-api-guides)
 
 ## Design & Approach
 
 This SDK is a thin wrapper around our API. See our API Reference for full documentation on behavior.
 
@@ -33,23 +35,23 @@
 
 ## Organization
 
 This SDK is organized into the following resources:
 
 
 
-- Campaigns
+- Accounts
 
 
 
-- Catalogs
+- Campaigns
 
 
 
-- Client
+- Catalogs
 
 
 
 - Data_Privacy
 
 
 
@@ -132,16 +134,14 @@
 klaviyo.Events.get_events(
     fields_event=['event_properties'], 
     filter="equals(metric_id,\"aBc123\")", 
     sort='-datetime'
     )
 ```
 
-NOTE: the filter param values need to be url-encoded
-
 #### How to filter based on datetime
 
 **Use Case**: Get profiles that have been updated between two datetimes.
 
 ```python
 klaviyo.Profiles.get_profiles(
     filter='less-than(updated,2023-04-26T00:00:00Z),greater-than(updated,2023-04-19T00:00:00Z)'
@@ -215,107 +215,142 @@
             keys = YOUR_EXCEPTION.headers.keys()
             values = YOUR_EXCEPTION.headers.values()
             ```
 
 ## Important Notes
 
 - The main difference between this SDK and the language-agnostic API Docs that the below endpoints link to is that this SDK automatically adds the `revision` header corresponding to the SDK version.
-- Organization: Resource groups and operation_ids are listed below in alphabetical order, first by Resource name, then by **OpenAPI Summary**. Operation summaries are those listed in the right side bar of the [API Reference](https://developers.klaviyo.com/en/v2023-02-22/reference/get_events).
+- Organization: Resource groups and operation_ids are listed below in alphabetical order, first by Resource name, then by **OpenAPI Summary**. Operation summaries are those listed in the right side bar of the [API Reference](https://developers.klaviyo.com/en/v2023-06-15/reference/get_events).
 - For example values / data types, as well as whether parameters are required/optional, please reference the corresponding API Reference link.
 - Some keyword args may potentially be required for the API call to succeed, the linked API docs are the source of truth regarding which keyword params are required.
 - JSON payloads should be passed in as native python dictionaries.
 - You can override the client private key by passing in an optional `api_key` keyword arg to any API call that takes a private key. As a reminder: do NOT do this client-side/onsite.
 
 # Comprehensive list of Operations & Parameters
 
 
 
 
 
+## Accounts
+
+#### [Get Account](https://developers.klaviyo.com/en/v2023-06-15/reference/get_account)
+
+```python
+## Positional Arguments
+
+# id | str
+
+## Keyword Arguments
+
+# fields_account | [str]
+
+klaviyo.Accounts.get_account(id, fields_account=fields_account)
+```
+
+
+
+
+#### [Get Accounts](https://developers.klaviyo.com/en/v2023-06-15/reference/get_accounts)
+
+```python
+
+## Keyword Arguments
+
+# fields_account | [str]
+
+klaviyo.Accounts.get_accounts(fields_account=fields_account)
+```
+
+
+
+
+
+
 ## Campaigns
 
-#### [Create Campaign](https://developers.klaviyo.com/en/v2023-02-22/reference/create_campaign)
+#### [Create Campaign](https://developers.klaviyo.com/en/v2023-06-15/reference/create_campaign)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Campaigns.create_campaign(body)
 ```
 
 
 
 
-#### [Create Campaign Clone](https://developers.klaviyo.com/en/v2023-02-22/reference/create_campaign_clone)
+#### [Create Campaign Clone](https://developers.klaviyo.com/en/v2023-06-15/reference/create_campaign_clone)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Campaigns.create_campaign_clone(body)
 ```
 
 
 
 
-#### [Assign Campaign Message Template](https://developers.klaviyo.com/en/v2023-02-22/reference/create_campaign_message_assign_template)
+#### [Assign Campaign Message Template](https://developers.klaviyo.com/en/v2023-06-15/reference/create_campaign_message_assign_template)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Campaigns.create_campaign_message_assign_template(body)
 ```
 
 
 
 
-#### [Create Campaign Recipient Estimation Job](https://developers.klaviyo.com/en/v2023-02-22/reference/create_campaign_recipient_estimation_job)
+#### [Create Campaign Recipient Estimation Job](https://developers.klaviyo.com/en/v2023-06-15/reference/create_campaign_recipient_estimation_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Campaigns.create_campaign_recipient_estimation_job(body)
 ```
 
 
 
 
-#### [Create Campaign Send Job](https://developers.klaviyo.com/en/v2023-02-22/reference/create_campaign_send_job)
+#### [Create Campaign Send Job](https://developers.klaviyo.com/en/v2023-06-15/reference/create_campaign_send_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Campaigns.create_campaign_send_job(body)
 ```
 
 
 
 
-#### [Delete Campaign](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_campaign)
+#### [Delete Campaign](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_campaign)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Campaigns.delete_campaign(id)
 ```
 
 
 
 
-#### [Get Campaign](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaign)
+#### [Get Campaign](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaign)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -326,15 +361,15 @@
 
 klaviyo.Campaigns.get_campaign(id, fields_campaign=fields_campaign, fields_tag=fields_tag, include=include)
 ```
 
 
 
 
-#### [Get Campaign Message](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaign_message)
+#### [Get Campaign Message](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaign_message)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -343,15 +378,15 @@
 
 klaviyo.Campaigns.get_campaign_message(id, fields_campaign_message=fields_campaign_message)
 ```
 
 
 
 
-#### [Get Campaign Recipient Estimation](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaign_recipient_estimation)
+#### [Get Campaign Recipient Estimation](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaign_recipient_estimation)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -360,15 +395,15 @@
 
 klaviyo.Campaigns.get_campaign_recipient_estimation(id, fields_campaign_recipient_estimation=fields_campaign_recipient_estimation)
 ```
 
 
 
 
-#### [Get Campaign Recipient Estimation Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaign_recipient_estimation_job)
+#### [Get Campaign Recipient Estimation Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaign_recipient_estimation_job)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -377,28 +412,28 @@
 
 klaviyo.Campaigns.get_campaign_recipient_estimation_job(id, fields_campaign_recipient_estimation_job=fields_campaign_recipient_estimation_job)
 ```
 
 
 
 
-#### [Get Campaign Relationships Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaign_relationships_tags)
+#### [Get Campaign Relationships Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaign_relationships_tags)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Campaigns.get_campaign_relationships_tags(id)
 ```
 
 
 
 
-#### [Get Campaign Send Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaign_send_job)
+#### [Get Campaign Send Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaign_send_job)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -407,32 +442,32 @@
 
 klaviyo.Campaigns.get_campaign_send_job(id, fields_campaign_send_job=fields_campaign_send_job)
 ```
 
 
 
 
-#### [Get Campaign Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaign_tags)
+#### [Get Campaign Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaign_tags)
 
 ```python
 ## Positional Arguments
 
-# campaign_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_tag | [str]
 
-klaviyo.Campaigns.get_campaign_tags(campaign_id, fields_tag=fields_tag)
+klaviyo.Campaigns.get_campaign_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
-#### [Get Campaigns](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaigns)
+#### [Get Campaigns](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaigns)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_campaign | [str]
 # fields_tag | [str]
@@ -443,43 +478,43 @@
 
 klaviyo.Campaigns.get_campaigns(fields_campaign=fields_campaign, fields_tag=fields_tag, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Update Campaign](https://developers.klaviyo.com/en/v2023-02-22/reference/update_campaign)
+#### [Update Campaign](https://developers.klaviyo.com/en/v2023-06-15/reference/update_campaign)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Campaigns.update_campaign(id, body)
 ```
 
 
 
 
-#### [Update Campaign Message](https://developers.klaviyo.com/en/v2023-02-22/reference/update_campaign_message)
+#### [Update Campaign Message](https://developers.klaviyo.com/en/v2023-06-15/reference/update_campaign_message)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Campaigns.update_campaign_message(id, body)
 ```
 
 
 
 
-#### [Update Campaign Send Job](https://developers.klaviyo.com/en/v2023-02-22/reference/update_campaign_send_job)
+#### [Update Campaign Send Job](https://developers.klaviyo.com/en/v2023-06-15/reference/update_campaign_send_job)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -489,149 +524,149 @@
 
 
 
 
 
 ## Catalogs
 
-#### [Create Catalog Category](https://developers.klaviyo.com/en/v2023-02-22/reference/create_catalog_category)
+#### [Create Catalog Category](https://developers.klaviyo.com/en/v2023-06-15/reference/create_catalog_category)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.create_catalog_category(body)
 ```
 
 
 
 
-#### [Create Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-02-22/reference/create_catalog_category_relationships_items)
+#### [Create Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-06-15/reference/create_catalog_category_relationships_items)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.create_catalog_category_relationships_items(id, body)
 ```
 
 
 
 
-#### [Create Catalog Item](https://developers.klaviyo.com/en/v2023-02-22/reference/create_catalog_item)
+#### [Create Catalog Item](https://developers.klaviyo.com/en/v2023-06-15/reference/create_catalog_item)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.create_catalog_item(body)
 ```
 
 
 
 
-#### [Create Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-02-22/reference/create_catalog_item_relationships_categories)
+#### [Create Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-06-15/reference/create_catalog_item_relationships_categories)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.create_catalog_item_relationships_categories(id, body)
 ```
 
 
 
 
-#### [Create Catalog Variant](https://developers.klaviyo.com/en/v2023-02-22/reference/create_catalog_variant)
+#### [Create Catalog Variant](https://developers.klaviyo.com/en/v2023-06-15/reference/create_catalog_variant)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.create_catalog_variant(body)
 ```
 
 
 
 
-#### [Delete Catalog Category](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_catalog_category)
+#### [Delete Catalog Category](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_catalog_category)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Catalogs.delete_catalog_category(id)
 ```
 
 
 
 
-#### [Delete Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_catalog_category_relationships_items)
+#### [Delete Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_catalog_category_relationships_items)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.delete_catalog_category_relationships_items(id, body)
 ```
 
 
 
 
-#### [Delete Catalog Item](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_catalog_item)
+#### [Delete Catalog Item](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_catalog_item)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Catalogs.delete_catalog_item(id)
 ```
 
 
 
 
-#### [Delete Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_catalog_item_relationships_categories)
+#### [Delete Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_catalog_item_relationships_categories)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.delete_catalog_item_relationships_categories(id, body)
 ```
 
 
 
 
-#### [Delete Catalog Variant](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_catalog_variant)
+#### [Delete Catalog Variant](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_catalog_variant)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Catalogs.delete_catalog_variant(id)
 ```
 
 
 
 
-#### [Get Catalog Categories](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_categories)
+#### [Get Catalog Categories](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_categories)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_category | [str]
 # filter | str
@@ -640,15 +675,15 @@
 
 klaviyo.Catalogs.get_catalog_categories(fields_catalog_category=fields_catalog_category, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Get Catalog Category](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_category)
+#### [Get Catalog Category](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_category)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -657,37 +692,37 @@
 
 klaviyo.Catalogs.get_catalog_category(id, fields_catalog_category=fields_catalog_category)
 ```
 
 
 
 
-#### [Get Catalog Category Items](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_category_items)
+#### [Get Catalog Category Items](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_category_items)
 
 ```python
 ## Positional Arguments
 
-# category_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_catalog_item | [str]
 # fields_catalog_variant | [str]
 # filter | str
 # include | [str]
 # page_cursor | str
 # sort | str
 
-klaviyo.Catalogs.get_catalog_category_items(category_id, fields_catalog_item=fields_catalog_item, fields_catalog_variant=fields_catalog_variant, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
+klaviyo.Catalogs.get_catalog_category_items(id, fields_catalog_item=fields_catalog_item, fields_catalog_variant=fields_catalog_variant, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Get Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_category_relationships_items)
+#### [Get Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_category_relationships_items)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -696,15 +731,15 @@
 
 klaviyo.Catalogs.get_catalog_category_relationships_items(id, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Catalog Item](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_item)
+#### [Get Catalog Item](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_item)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -715,35 +750,35 @@
 
 klaviyo.Catalogs.get_catalog_item(id, fields_catalog_item=fields_catalog_item, fields_catalog_variant=fields_catalog_variant, include=include)
 ```
 
 
 
 
-#### [Get Catalog Item Categories](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_item_categories)
+#### [Get Catalog Item Categories](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_item_categories)
 
 ```python
 ## Positional Arguments
 
-# item_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_catalog_category | [str]
 # filter | str
 # page_cursor | str
 # sort | str
 
-klaviyo.Catalogs.get_catalog_item_categories(item_id, fields_catalog_category=fields_catalog_category, filter=filter, page_cursor=page_cursor, sort=sort)
+klaviyo.Catalogs.get_catalog_item_categories(id, fields_catalog_category=fields_catalog_category, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Get Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_item_relationships_categories)
+#### [Get Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_item_relationships_categories)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -752,35 +787,35 @@
 
 klaviyo.Catalogs.get_catalog_item_relationships_categories(id, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Catalog Item Variants](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_item_variants)
+#### [Get Catalog Item Variants](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_item_variants)
 
 ```python
 ## Positional Arguments
 
-# item_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_catalog_variant | [str]
 # filter | str
 # page_cursor | str
 # sort | str
 
-klaviyo.Catalogs.get_catalog_item_variants(item_id, fields_catalog_variant=fields_catalog_variant, filter=filter, page_cursor=page_cursor, sort=sort)
+klaviyo.Catalogs.get_catalog_item_variants(id, fields_catalog_variant=fields_catalog_variant, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Get Catalog Items](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_items)
+#### [Get Catalog Items](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_items)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_item | [str]
 # fields_catalog_variant | [str]
@@ -791,15 +826,15 @@
 
 klaviyo.Catalogs.get_catalog_items(fields_catalog_item=fields_catalog_item, fields_catalog_variant=fields_catalog_variant, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Get Catalog Variant](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_variant)
+#### [Get Catalog Variant](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_variant)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -808,15 +843,15 @@
 
 klaviyo.Catalogs.get_catalog_variant(id, fields_catalog_variant=fields_catalog_variant)
 ```
 
 
 
 
-#### [Get Catalog Variants](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_variants)
+#### [Get Catalog Variants](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_variants)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_variant | [str]
 # filter | str
@@ -825,15 +860,15 @@
 
 klaviyo.Catalogs.get_catalog_variants(fields_catalog_variant=fields_catalog_variant, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Get Create Categories Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_create_categories_job)
+#### [Get Create Categories Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_create_categories_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -844,15 +879,15 @@
 
 klaviyo.Catalogs.get_create_categories_job(job_id, fields_catalog_category_bulk_create_job=fields_catalog_category_bulk_create_job, fields_catalog_category=fields_catalog_category, include=include)
 ```
 
 
 
 
-#### [Get Create Categories Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_create_categories_jobs)
+#### [Get Create Categories Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_create_categories_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_category_bulk_create_job | [str]
 # filter | str
@@ -860,15 +895,15 @@
 
 klaviyo.Catalogs.get_create_categories_jobs(fields_catalog_category_bulk_create_job=fields_catalog_category_bulk_create_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Create Items Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_create_items_job)
+#### [Get Create Items Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_create_items_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -879,15 +914,15 @@
 
 klaviyo.Catalogs.get_create_items_job(job_id, fields_catalog_item_bulk_create_job=fields_catalog_item_bulk_create_job, fields_catalog_item=fields_catalog_item, include=include)
 ```
 
 
 
 
-#### [Get Create Items Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_create_items_jobs)
+#### [Get Create Items Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_create_items_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_item_bulk_create_job | [str]
 # filter | str
@@ -895,15 +930,15 @@
 
 klaviyo.Catalogs.get_create_items_jobs(fields_catalog_item_bulk_create_job=fields_catalog_item_bulk_create_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Create Variants Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_create_variants_job)
+#### [Get Create Variants Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_create_variants_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -914,15 +949,15 @@
 
 klaviyo.Catalogs.get_create_variants_job(job_id, fields_catalog_variant_bulk_create_job=fields_catalog_variant_bulk_create_job, fields_catalog_variant=fields_catalog_variant, include=include)
 ```
 
 
 
 
-#### [Get Create Variants Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_create_variants_jobs)
+#### [Get Create Variants Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_create_variants_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_variant_bulk_create_job | [str]
 # filter | str
@@ -930,15 +965,15 @@
 
 klaviyo.Catalogs.get_create_variants_jobs(fields_catalog_variant_bulk_create_job=fields_catalog_variant_bulk_create_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Delete Categories Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_delete_categories_job)
+#### [Get Delete Categories Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_delete_categories_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -947,15 +982,15 @@
 
 klaviyo.Catalogs.get_delete_categories_job(job_id, fields_catalog_category_bulk_delete_job=fields_catalog_category_bulk_delete_job)
 ```
 
 
 
 
-#### [Get Delete Categories Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_delete_categories_jobs)
+#### [Get Delete Categories Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_delete_categories_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_category_bulk_delete_job | [str]
 # filter | str
@@ -963,15 +998,15 @@
 
 klaviyo.Catalogs.get_delete_categories_jobs(fields_catalog_category_bulk_delete_job=fields_catalog_category_bulk_delete_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Delete Items Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_delete_items_job)
+#### [Get Delete Items Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_delete_items_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -980,15 +1015,15 @@
 
 klaviyo.Catalogs.get_delete_items_job(job_id, fields_catalog_item_bulk_delete_job=fields_catalog_item_bulk_delete_job)
 ```
 
 
 
 
-#### [Get Delete Items Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_delete_items_jobs)
+#### [Get Delete Items Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_delete_items_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_item_bulk_delete_job | [str]
 # filter | str
@@ -996,15 +1031,15 @@
 
 klaviyo.Catalogs.get_delete_items_jobs(fields_catalog_item_bulk_delete_job=fields_catalog_item_bulk_delete_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Delete Variants Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_delete_variants_job)
+#### [Get Delete Variants Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_delete_variants_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -1013,15 +1048,15 @@
 
 klaviyo.Catalogs.get_delete_variants_job(job_id, fields_catalog_variant_bulk_delete_job=fields_catalog_variant_bulk_delete_job)
 ```
 
 
 
 
-#### [Get Delete Variants Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_delete_variants_jobs)
+#### [Get Delete Variants Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_delete_variants_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_variant_bulk_delete_job | [str]
 # filter | str
@@ -1029,15 +1064,15 @@
 
 klaviyo.Catalogs.get_delete_variants_jobs(fields_catalog_variant_bulk_delete_job=fields_catalog_variant_bulk_delete_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Update Categories Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_update_categories_job)
+#### [Get Update Categories Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_update_categories_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -1048,15 +1083,15 @@
 
 klaviyo.Catalogs.get_update_categories_job(job_id, fields_catalog_category_bulk_update_job=fields_catalog_category_bulk_update_job, fields_catalog_category=fields_catalog_category, include=include)
 ```
 
 
 
 
-#### [Get Update Categories Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_update_categories_jobs)
+#### [Get Update Categories Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_update_categories_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_category_bulk_update_job | [str]
 # filter | str
@@ -1064,15 +1099,15 @@
 
 klaviyo.Catalogs.get_update_categories_jobs(fields_catalog_category_bulk_update_job=fields_catalog_category_bulk_update_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Update Items Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_update_items_job)
+#### [Get Update Items Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_update_items_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -1083,15 +1118,15 @@
 
 klaviyo.Catalogs.get_update_items_job(job_id, fields_catalog_item_bulk_update_job=fields_catalog_item_bulk_update_job, fields_catalog_item=fields_catalog_item, include=include)
 ```
 
 
 
 
-#### [Get Update Items Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_update_items_jobs)
+#### [Get Update Items Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_update_items_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_item_bulk_update_job | [str]
 # filter | str
@@ -1099,15 +1134,15 @@
 
 klaviyo.Catalogs.get_update_items_jobs(fields_catalog_item_bulk_update_job=fields_catalog_item_bulk_update_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Update Variants Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_update_variants_job)
+#### [Get Update Variants Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_update_variants_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -1118,15 +1153,15 @@
 
 klaviyo.Catalogs.get_update_variants_job(job_id, fields_catalog_variant_bulk_update_job=fields_catalog_variant_bulk_update_job, fields_catalog_variant=fields_catalog_variant, include=include)
 ```
 
 
 
 
-#### [Get Update Variants Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_update_variants_jobs)
+#### [Get Update Variants Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_update_variants_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_variant_bulk_update_job | [str]
 # filter | str
@@ -1134,188 +1169,188 @@
 
 klaviyo.Catalogs.get_update_variants_jobs(fields_catalog_variant_bulk_update_job=fields_catalog_variant_bulk_update_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Spawn Create Categories Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_create_categories_job)
+#### [Spawn Create Categories Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_create_categories_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_create_categories_job(body)
 ```
 
 
 
 
-#### [Spawn Create Items Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_create_items_job)
+#### [Spawn Create Items Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_create_items_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_create_items_job(body)
 ```
 
 
 
 
-#### [Spawn Create Variants Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_create_variants_job)
+#### [Spawn Create Variants Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_create_variants_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_create_variants_job(body)
 ```
 
 
 
 
-#### [Spawn Delete Categories Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_delete_categories_job)
+#### [Spawn Delete Categories Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_delete_categories_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_delete_categories_job(body)
 ```
 
 
 
 
-#### [Spawn Delete Items Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_delete_items_job)
+#### [Spawn Delete Items Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_delete_items_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_delete_items_job(body)
 ```
 
 
 
 
-#### [Spawn Delete Variants Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_delete_variants_job)
+#### [Spawn Delete Variants Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_delete_variants_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_delete_variants_job(body)
 ```
 
 
 
 
-#### [Spawn Update Categories Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_update_categories_job)
+#### [Spawn Update Categories Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_update_categories_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_update_categories_job(body)
 ```
 
 
 
 
-#### [Spawn Update Items Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_update_items_job)
+#### [Spawn Update Items Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_update_items_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_update_items_job(body)
 ```
 
 
 
 
-#### [Spawn Update Variants Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_update_variants_job)
+#### [Spawn Update Variants Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_update_variants_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_update_variants_job(body)
 ```
 
 
 
 
-#### [Update Catalog Category](https://developers.klaviyo.com/en/v2023-02-22/reference/update_catalog_category)
+#### [Update Catalog Category](https://developers.klaviyo.com/en/v2023-06-15/reference/update_catalog_category)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.update_catalog_category(id, body)
 ```
 
 
 
 
-#### [Update Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-02-22/reference/update_catalog_category_relationships_items)
+#### [Update Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-06-15/reference/update_catalog_category_relationships_items)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.update_catalog_category_relationships_items(id, body)
 ```
 
 
 
 
-#### [Update Catalog Item](https://developers.klaviyo.com/en/v2023-02-22/reference/update_catalog_item)
+#### [Update Catalog Item](https://developers.klaviyo.com/en/v2023-06-15/reference/update_catalog_item)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.update_catalog_item(id, body)
 ```
 
 
 
 
-#### [Update Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-02-22/reference/update_catalog_item_relationships_categories)
+#### [Update Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-06-15/reference/update_catalog_item_relationships_categories)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.update_catalog_item_relationships_categories(id, body)
 ```
 
 
 
 
-#### [Update Catalog Variant](https://developers.klaviyo.com/en/v2023-02-22/reference/update_catalog_variant)
+#### [Update Catalog Variant](https://developers.klaviyo.com/en/v2023-06-15/reference/update_catalog_variant)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -1323,63 +1358,17 @@
 ```
 
 
 
 
 
 
-## Client
-
-#### [Create Client Event](https://developers.klaviyo.com/en/v2023-02-22/reference/create_client_event)
-
-```python
-## Positional Arguments
-
-# company_id | str
-# body | dict
-
-klaviyo.Client.create_client_event(company_id, body)
-```
-
-
-
-
-#### [Create or Update Client Profile](https://developers.klaviyo.com/en/v2023-02-22/reference/create_client_profile)
-
-```python
-## Positional Arguments
-
-# company_id | str
-# body | dict
-
-klaviyo.Client.create_client_profile(company_id, body)
-```
-
-
-
-
-#### [Create Client Subscription](https://developers.klaviyo.com/en/v2023-02-22/reference/create_client_subscription)
-
-```python
-## Positional Arguments
-
-# company_id | str
-# body | dict
-
-klaviyo.Client.create_client_subscription(company_id, body)
-```
-
-
-
-
-
-
 ## Data_Privacy
 
-#### [Request Profile Deletion](https://developers.klaviyo.com/en/v2023-02-22/reference/request_profile_deletion)
+#### [Request Profile Deletion](https://developers.klaviyo.com/en/v2023-06-15/reference/request_profile_deletion)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Data_Privacy.request_profile_deletion(body)
@@ -1388,28 +1377,28 @@
 
 
 
 
 
 ## Events
 
-#### [Create Event](https://developers.klaviyo.com/en/v2023-02-22/reference/create_event)
+#### [Create Event](https://developers.klaviyo.com/en/v2023-06-15/reference/create_event)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Events.create_event(body)
 ```
 
 
 
 
-#### [Get Event](https://developers.klaviyo.com/en/v2023-02-22/reference/get_event)
+#### [Get Event](https://developers.klaviyo.com/en/v2023-06-15/reference/get_event)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1421,15 +1410,15 @@
 
 klaviyo.Events.get_event(id, fields_event=fields_event, fields_metric=fields_metric, fields_profile=fields_profile, include=include)
 ```
 
 
 
 
-#### [Get Event Metrics](https://developers.klaviyo.com/en/v2023-02-22/reference/get_event_metrics)
+#### [Get Event Metrics](https://developers.klaviyo.com/en/v2023-06-15/reference/get_event_metrics)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1438,15 +1427,15 @@
 
 klaviyo.Events.get_event_metrics(id, fields_metric=fields_metric)
 ```
 
 
 
 
-#### [Get Event Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/get_event_profiles)
+#### [Get Event Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/get_event_profiles)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1456,41 +1445,41 @@
 
 klaviyo.Events.get_event_profiles(id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile)
 ```
 
 
 
 
-#### [Get Event Relationships Metrics](https://developers.klaviyo.com/en/v2023-02-22/reference/get_event_relationships_metrics)
+#### [Get Event Relationships Metrics](https://developers.klaviyo.com/en/v2023-06-15/reference/get_event_relationships_metrics)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Events.get_event_relationships_metrics(id)
 ```
 
 
 
 
-#### [Get Event Relationships Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/get_event_relationships_profiles)
+#### [Get Event Relationships Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/get_event_relationships_profiles)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Events.get_event_relationships_profiles(id)
 ```
 
 
 
 
-#### [Get Events](https://developers.klaviyo.com/en/v2023-02-22/reference/get_events)
+#### [Get Events](https://developers.klaviyo.com/en/v2023-06-15/reference/get_events)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_event | [str]
 # fields_metric | [str]
@@ -1506,15 +1495,15 @@
 
 
 
 
 
 ## Flows
 
-#### [Get Flow](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow)
+#### [Get Flow](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1525,15 +1514,15 @@
 
 klaviyo.Flows.get_flow(id, fields_flow_action=fields_flow_action, fields_flow=fields_flow, include=include)
 ```
 
 
 
 
-#### [Get Flow Action](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_action)
+#### [Get Flow Action](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_action)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1545,66 +1534,66 @@
 
 klaviyo.Flows.get_flow_action(id, fields_flow_action=fields_flow_action, fields_flow_message=fields_flow_message, fields_flow=fields_flow, include=include)
 ```
 
 
 
 
-#### [Get Flow For Flow Action](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_action_flow)
+#### [Get Flow For Flow Action](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_action_flow)
 
 ```python
 ## Positional Arguments
 
-# action_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_flow | [str]
 
-klaviyo.Flows.get_flow_action_flow(action_id, fields_flow=fields_flow)
+klaviyo.Flows.get_flow_action_flow(id, fields_flow=fields_flow)
 ```
 
 
 
 
-#### [Get Messages For Flow Action](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_action_messages)
+#### [Get Messages For Flow Action](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_action_messages)
 
 ```python
 ## Positional Arguments
 
-# action_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_flow_message | [str]
 # filter | str
 # page_cursor | str
 # page_size | int
 # sort | str
 
-klaviyo.Flows.get_flow_action_messages(action_id, fields_flow_message=fields_flow_message, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
+klaviyo.Flows.get_flow_action_messages(id, fields_flow_message=fields_flow_message, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
-#### [Get Flow Action Relationships Flow](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_action_relationships_flow)
+#### [Get Flow Action Relationships Flow](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_action_relationships_flow)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Flows.get_flow_action_relationships_flow(id)
 ```
 
 
 
 
-#### [Get Flow Action Relationships Messages](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_action_relationships_messages)
+#### [Get Flow Action Relationships Messages](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_action_relationships_messages)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1616,36 +1605,36 @@
 
 klaviyo.Flows.get_flow_action_relationships_messages(id, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
-#### [Get Flow Actions For Flow](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_flow_actions)
+#### [Get Flow Actions For Flow](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_flow_actions)
 
 ```python
 ## Positional Arguments
 
-# flow_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_flow_action | [str]
 # filter | str
 # page_cursor | str
 # page_size | int
 # sort | str
 
-klaviyo.Flows.get_flow_flow_actions(flow_id, fields_flow_action=fields_flow_action, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
+klaviyo.Flows.get_flow_flow_actions(id, fields_flow_action=fields_flow_action, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
-#### [Get Flow Message](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_message)
+#### [Get Flow Message](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_message)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1656,45 +1645,45 @@
 
 klaviyo.Flows.get_flow_message(id, fields_flow_action=fields_flow_action, fields_flow_message=fields_flow_message, include=include)
 ```
 
 
 
 
-#### [Get Flow Action For Message](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_message_action)
+#### [Get Flow Action For Message](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_message_action)
 
 ```python
 ## Positional Arguments
 
-# message_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_flow_action | [str]
 
-klaviyo.Flows.get_flow_message_action(message_id, fields_flow_action=fields_flow_action)
+klaviyo.Flows.get_flow_message_action(id, fields_flow_action=fields_flow_action)
 ```
 
 
 
 
-#### [Get Flow Message Relationships Action](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_message_relationships_action)
+#### [Get Flow Message Relationships Action](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_message_relationships_action)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Flows.get_flow_message_relationships_action(id)
 ```
 
 
 
 
-#### [Get Flow Relationships Flow Actions](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_relationships_flow_actions)
+#### [Get Flow Relationships Flow Actions](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_relationships_flow_actions)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1705,45 +1694,45 @@
 
 klaviyo.Flows.get_flow_relationships_flow_actions(id, filter=filter, page_size=page_size, sort=sort)
 ```
 
 
 
 
-#### [Get Flow Relationships Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_relationships_tags)
+#### [Get Flow Relationships Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_relationships_tags)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Flows.get_flow_relationships_tags(id)
 ```
 
 
 
 
-#### [Get Flow Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_tags)
+#### [Get Flow Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_tags)
 
 ```python
 ## Positional Arguments
 
-# flow_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_tag | [str]
 
-klaviyo.Flows.get_flow_tags(flow_id, fields_tag=fields_tag)
+klaviyo.Flows.get_flow_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
-#### [Get Flows](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flows)
+#### [Get Flows](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flows)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_flow_action | [str]
 # fields_flow | [str]
@@ -1755,15 +1744,15 @@
 
 klaviyo.Flows.get_flows(fields_flow_action=fields_flow_action, fields_flow=fields_flow, filter=filter, include=include, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
-#### [Update Flow Status](https://developers.klaviyo.com/en/v2023-02-22/reference/update_flow)
+#### [Update Flow Status](https://developers.klaviyo.com/en/v2023-06-15/reference/update_flow)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -1773,69 +1762,69 @@
 
 
 
 
 
 ## Lists
 
-#### [Create List](https://developers.klaviyo.com/en/v2023-02-22/reference/create_list)
+#### [Create List](https://developers.klaviyo.com/en/v2023-06-15/reference/create_list)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Lists.create_list(body)
 ```
 
 
 
 
-#### [Add Profile To List](https://developers.klaviyo.com/en/v2023-02-22/reference/create_list_relationships)
+#### [Add Profile To List](https://developers.klaviyo.com/en/v2023-06-15/reference/create_list_relationships)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Lists.create_list_relationships(id, body)
 ```
 
 
 
 
-#### [Delete List](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_list)
+#### [Delete List](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_list)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Lists.delete_list(id)
 ```
 
 
 
 
-#### [Remove Profile From List](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_list_relationships)
+#### [Remove Profile From List](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_list_relationships)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Lists.delete_list_relationships(id, body)
 ```
 
 
 
 
-#### [Get List](https://developers.klaviyo.com/en/v2023-02-22/reference/get_list)
+#### [Get List](https://developers.klaviyo.com/en/v2023-06-15/reference/get_list)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1844,36 +1833,36 @@
 
 klaviyo.Lists.get_list(id, fields_list=fields_list)
 ```
 
 
 
 
-#### [Get List Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/get_list_profiles)
+#### [Get List Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/get_list_profiles)
 
 ```python
 ## Positional Arguments
 
-# list_id | str
+# id | str
 
 ## Keyword Arguments
 
 # additional_fields_profile | [str]
 # fields_profile | [str]
 # filter | str
 # page_cursor | str
 # page_size | int
 
-klaviyo.Lists.get_list_profiles(list_id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size)
+klaviyo.Lists.get_list_profiles(id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size)
 ```
 
 
 
 
-#### [Get List Relationships Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/get_list_relationships_profiles)
+#### [Get List Relationships Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/get_list_relationships_profiles)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1882,45 +1871,45 @@
 
 klaviyo.Lists.get_list_relationships_profiles(id, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get List Relationships Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_list_relationships_tags)
+#### [Get List Relationships Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_list_relationships_tags)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Lists.get_list_relationships_tags(id)
 ```
 
 
 
 
-#### [Get List Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_list_tags)
+#### [Get List Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_list_tags)
 
 ```python
 ## Positional Arguments
 
-# list_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_tag | [str]
 
-klaviyo.Lists.get_list_tags(list_id, fields_tag=fields_tag)
+klaviyo.Lists.get_list_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
-#### [Get Lists](https://developers.klaviyo.com/en/v2023-02-22/reference/get_lists)
+#### [Get Lists](https://developers.klaviyo.com/en/v2023-06-15/reference/get_lists)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_list | [str]
 # filter | str
@@ -1928,15 +1917,15 @@
 
 klaviyo.Lists.get_lists(fields_list=fields_list, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Update List](https://developers.klaviyo.com/en/v2023-02-22/reference/update_list)
+#### [Update List](https://developers.klaviyo.com/en/v2023-06-15/reference/update_list)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -1946,15 +1935,15 @@
 
 
 
 
 
 ## Metrics
 
-#### [Get Metric](https://developers.klaviyo.com/en/v2023-02-22/reference/get_metric)
+#### [Get Metric](https://developers.klaviyo.com/en/v2023-06-15/reference/get_metric)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1963,15 +1952,15 @@
 
 klaviyo.Metrics.get_metric(id, fields_metric=fields_metric)
 ```
 
 
 
 
-#### [Get Metrics](https://developers.klaviyo.com/en/v2023-02-22/reference/get_metrics)
+#### [Get Metrics](https://developers.klaviyo.com/en/v2023-06-15/reference/get_metrics)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_metric | [str]
 # filter | str
@@ -1979,15 +1968,15 @@
 
 klaviyo.Metrics.get_metrics(fields_metric=fields_metric, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Query Metric Aggregates](https://developers.klaviyo.com/en/v2023-02-22/reference/query_metric_aggregates)
+#### [Query Metric Aggregates](https://developers.klaviyo.com/en/v2023-06-15/reference/query_metric_aggregates)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Metrics.query_metric_aggregates(body)
@@ -1996,28 +1985,28 @@
 
 
 
 
 
 ## Profiles
 
-#### [Create Profile](https://developers.klaviyo.com/en/v2023-02-22/reference/create_profile)
+#### [Create Profile](https://developers.klaviyo.com/en/v2023-06-15/reference/create_profile)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Profiles.create_profile(body)
 ```
 
 
 
 
-#### [Get Profile](https://developers.klaviyo.com/en/v2023-02-22/reference/get_profile)
+#### [Get Profile](https://developers.klaviyo.com/en/v2023-06-15/reference/get_profile)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2030,75 +2019,75 @@
 
 klaviyo.Profiles.get_profile(id, additional_fields_profile=additional_fields_profile, fields_list=fields_list, fields_profile=fields_profile, fields_segment=fields_segment, include=include)
 ```
 
 
 
 
-#### [Get Profile Lists](https://developers.klaviyo.com/en/v2023-02-22/reference/get_profile_lists)
+#### [Get Profile Lists](https://developers.klaviyo.com/en/v2023-06-15/reference/get_profile_lists)
 
 ```python
 ## Positional Arguments
 
-# profile_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_list | [str]
 
-klaviyo.Profiles.get_profile_lists(profile_id, fields_list=fields_list)
+klaviyo.Profiles.get_profile_lists(id, fields_list=fields_list)
 ```
 
 
 
 
-#### [Get Profile Relationships Lists](https://developers.klaviyo.com/en/v2023-02-22/reference/get_profile_relationships_lists)
+#### [Get Profile Relationships Lists](https://developers.klaviyo.com/en/v2023-06-15/reference/get_profile_relationships_lists)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Profiles.get_profile_relationships_lists(id)
 ```
 
 
 
 
-#### [Get Profile Relationships Segments](https://developers.klaviyo.com/en/v2023-02-22/reference/get_profile_relationships_segments)
+#### [Get Profile Relationships Segments](https://developers.klaviyo.com/en/v2023-06-15/reference/get_profile_relationships_segments)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Profiles.get_profile_relationships_segments(id)
 ```
 
 
 
 
-#### [Get Profile Segments](https://developers.klaviyo.com/en/v2023-02-22/reference/get_profile_segments)
+#### [Get Profile Segments](https://developers.klaviyo.com/en/v2023-06-15/reference/get_profile_segments)
 
 ```python
 ## Positional Arguments
 
-# profile_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_segment | [str]
 
-klaviyo.Profiles.get_profile_segments(profile_id, fields_segment=fields_segment)
+klaviyo.Profiles.get_profile_segments(id, fields_segment=fields_segment)
 ```
 
 
 
 
-#### [Get Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/get_profiles)
+#### [Get Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/get_profiles)
 
 ```python
 
 ## Keyword Arguments
 
 # additional_fields_profile | [str]
 # fields_profile | [str]
@@ -2109,67 +2098,67 @@
 
 klaviyo.Profiles.get_profiles(additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
-#### [Subscribe Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/subscribe_profiles)
+#### [Subscribe Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/subscribe_profiles)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Profiles.subscribe_profiles(body)
 ```
 
 
 
 
-#### [Suppress Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/suppress_profiles)
+#### [Suppress Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/suppress_profiles)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Profiles.suppress_profiles(body)
 ```
 
 
 
 
-#### [Unsubscribe Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/unsubscribe_profiles)
+#### [Unsubscribe Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/unsubscribe_profiles)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Profiles.unsubscribe_profiles(body)
 ```
 
 
 
 
-#### [Unsuppress Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/unsuppress_profiles)
+#### [Unsuppress Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/unsuppress_profiles)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Profiles.unsuppress_profiles(body)
 ```
 
 
 
 
-#### [Update Profile](https://developers.klaviyo.com/en/v2023-02-22/reference/update_profile)
+#### [Update Profile](https://developers.klaviyo.com/en/v2023-06-15/reference/update_profile)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -2179,15 +2168,15 @@
 
 
 
 
 
 ## Segments
 
-#### [Get Segment](https://developers.klaviyo.com/en/v2023-02-22/reference/get_segment)
+#### [Get Segment](https://developers.klaviyo.com/en/v2023-06-15/reference/get_segment)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2196,36 +2185,36 @@
 
 klaviyo.Segments.get_segment(id, fields_segment=fields_segment)
 ```
 
 
 
 
-#### [Get Segment Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/get_segment_profiles)
+#### [Get Segment Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/get_segment_profiles)
 
 ```python
 ## Positional Arguments
 
-# segment_id | str
+# id | str
 
 ## Keyword Arguments
 
 # additional_fields_profile | [str]
 # fields_profile | [str]
 # filter | str
 # page_cursor | str
 # page_size | int
 
-klaviyo.Segments.get_segment_profiles(segment_id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size)
+klaviyo.Segments.get_segment_profiles(id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size)
 ```
 
 
 
 
-#### [Get Segment Relationships Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/get_segment_relationships_profiles)
+#### [Get Segment Relationships Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/get_segment_relationships_profiles)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2234,45 +2223,45 @@
 
 klaviyo.Segments.get_segment_relationships_profiles(id, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Segment Relationships Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_segment_relationships_tags)
+#### [Get Segment Relationships Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_segment_relationships_tags)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Segments.get_segment_relationships_tags(id)
 ```
 
 
 
 
-#### [Get Segment Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_segment_tags)
+#### [Get Segment Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_segment_tags)
 
 ```python
 ## Positional Arguments
 
-# segment_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_tag | [str]
 
-klaviyo.Segments.get_segment_tags(segment_id, fields_tag=fields_tag)
+klaviyo.Segments.get_segment_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
-#### [Get Segments](https://developers.klaviyo.com/en/v2023-02-22/reference/get_segments)
+#### [Get Segments](https://developers.klaviyo.com/en/v2023-06-15/reference/get_segments)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_segment | [str]
 # filter | str
@@ -2280,15 +2269,15 @@
 
 klaviyo.Segments.get_segments(fields_segment=fields_segment, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Update Segment](https://developers.klaviyo.com/en/v2023-02-22/reference/update_segment)
+#### [Update Segment](https://developers.klaviyo.com/en/v2023-06-15/reference/update_segment)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -2298,179 +2287,179 @@
 
 
 
 
 
 ## Tags
 
-#### [Create Tag](https://developers.klaviyo.com/en/v2023-02-22/reference/create_tag)
+#### [Create Tag](https://developers.klaviyo.com/en/v2023-06-15/reference/create_tag)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Tags.create_tag(body)
 ```
 
 
 
 
-#### [Create Tag Group](https://developers.klaviyo.com/en/v2023-02-22/reference/create_tag_group)
+#### [Create Tag Group](https://developers.klaviyo.com/en/v2023-06-15/reference/create_tag_group)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Tags.create_tag_group(body)
 ```
 
 
 
 
-#### [Create Tag Relationships Campaigns](https://developers.klaviyo.com/en/v2023-02-22/reference/create_tag_relationships_campaigns)
+#### [Create Tag Relationships Campaigns](https://developers.klaviyo.com/en/v2023-06-15/reference/create_tag_relationships_campaigns)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.create_tag_relationships_campaigns(id, body)
 ```
 
 
 
 
-#### [Create Tag Relationships Flows](https://developers.klaviyo.com/en/v2023-02-22/reference/create_tag_relationships_flows)
+#### [Create Tag Relationships Flows](https://developers.klaviyo.com/en/v2023-06-15/reference/create_tag_relationships_flows)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.create_tag_relationships_flows(id, body)
 ```
 
 
 
 
-#### [Create Tag Relationships Lists](https://developers.klaviyo.com/en/v2023-02-22/reference/create_tag_relationships_lists)
+#### [Create Tag Relationships Lists](https://developers.klaviyo.com/en/v2023-06-15/reference/create_tag_relationships_lists)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.create_tag_relationships_lists(id, body)
 ```
 
 
 
 
-#### [Create Tag Relationships Segments](https://developers.klaviyo.com/en/v2023-02-22/reference/create_tag_relationships_segments)
+#### [Create Tag Relationships Segments](https://developers.klaviyo.com/en/v2023-06-15/reference/create_tag_relationships_segments)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.create_tag_relationships_segments(id, body)
 ```
 
 
 
 
-#### [Delete Tag](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_tag)
+#### [Delete Tag](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_tag)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.delete_tag(id)
 ```
 
 
 
 
-#### [Delete Tag Group](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_tag_group)
+#### [Delete Tag Group](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_tag_group)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.delete_tag_group(id)
 ```
 
 
 
 
-#### [Delete Tag Relationships Campaigns](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_tag_relationships_campaigns)
+#### [Delete Tag Relationships Campaigns](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_tag_relationships_campaigns)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.delete_tag_relationships_campaigns(id, body)
 ```
 
 
 
 
-#### [Delete Tag Relationships Flows](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_tag_relationships_flows)
+#### [Delete Tag Relationships Flows](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_tag_relationships_flows)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.delete_tag_relationships_flows(id, body)
 ```
 
 
 
 
-#### [Delete Tag Relationships Lists](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_tag_relationships_lists)
+#### [Delete Tag Relationships Lists](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_tag_relationships_lists)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.delete_tag_relationships_lists(id, body)
 ```
 
 
 
 
-#### [Delete Tag Relationships Segments](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_tag_relationships_segments)
+#### [Delete Tag Relationships Segments](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_tag_relationships_segments)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.delete_tag_relationships_segments(id, body)
 ```
 
 
 
 
-#### [Get Tag](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag)
+#### [Get Tag](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2479,15 +2468,15 @@
 
 klaviyo.Tags.get_tag(id, fields_tag=fields_tag)
 ```
 
 
 
 
-#### [Get Tag Group](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_group)
+#### [Get Tag Group](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_group)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2496,28 +2485,28 @@
 
 klaviyo.Tags.get_tag_group(id, fields_tag_group=fields_tag_group)
 ```
 
 
 
 
-#### [Get Tag Group Relationships Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_group_relationships_tags)
+#### [Get Tag Group Relationships Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_group_relationships_tags)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.get_tag_group_relationships_tags(id)
 ```
 
 
 
 
-#### [Get Tag Group Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_group_tags)
+#### [Get Tag Group Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_group_tags)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2526,15 +2515,15 @@
 
 klaviyo.Tags.get_tag_group_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
-#### [Get Tag Groups](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_groups)
+#### [Get Tag Groups](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_groups)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_tag_group | [str]
 # filter | str
@@ -2543,80 +2532,80 @@
 
 klaviyo.Tags.get_tag_groups(fields_tag_group=fields_tag_group, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Get Tag Relationships Campaigns](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_relationships_campaigns)
+#### [Get Tag Relationships Campaigns](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_relationships_campaigns)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.get_tag_relationships_campaigns(id)
 ```
 
 
 
 
-#### [Get Tag Relationships Flows](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_relationships_flows)
+#### [Get Tag Relationships Flows](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_relationships_flows)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.get_tag_relationships_flows(id)
 ```
 
 
 
 
-#### [Get Tag Relationships Lists](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_relationships_lists)
+#### [Get Tag Relationships Lists](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_relationships_lists)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.get_tag_relationships_lists(id)
 ```
 
 
 
 
-#### [Get Tag Relationships Segments](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_relationships_segments)
+#### [Get Tag Relationships Segments](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_relationships_segments)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.get_tag_relationships_segments(id)
 ```
 
 
 
 
-#### [Get Tag Relationships Tag Group](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_relationships_tag_group)
+#### [Get Tag Relationships Tag Group](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_relationships_tag_group)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.get_tag_relationships_tag_group(id)
 ```
 
 
 
 
-#### [Get Tag Tag Group](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_tag_group)
+#### [Get Tag Tag Group](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_tag_group)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2625,15 +2614,15 @@
 
 klaviyo.Tags.get_tag_tag_group(id, fields_tag_group=fields_tag_group)
 ```
 
 
 
 
-#### [Get Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tags)
+#### [Get Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tags)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_tag | [str]
 # filter | str
@@ -2642,29 +2631,29 @@
 
 klaviyo.Tags.get_tags(fields_tag=fields_tag, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Update Tag](https://developers.klaviyo.com/en/v2023-02-22/reference/update_tag)
+#### [Update Tag](https://developers.klaviyo.com/en/v2023-06-15/reference/update_tag)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.update_tag(id, body)
 ```
 
 
 
 
-#### [Update Tag Group](https://developers.klaviyo.com/en/v2023-02-22/reference/update_tag_group)
+#### [Update Tag Group](https://developers.klaviyo.com/en/v2023-06-15/reference/update_tag_group)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -2674,67 +2663,67 @@
 
 
 
 
 
 ## Templates
 
-#### [Create Template](https://developers.klaviyo.com/en/v2023-02-22/reference/create_template)
+#### [Create Template](https://developers.klaviyo.com/en/v2023-06-15/reference/create_template)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Templates.create_template(body)
 ```
 
 
 
 
-#### [Create Template Clone](https://developers.klaviyo.com/en/v2023-02-22/reference/create_template_clone)
+#### [Create Template Clone](https://developers.klaviyo.com/en/v2023-06-15/reference/create_template_clone)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Templates.create_template_clone(body)
 ```
 
 
 
 
-#### [Create Template Render](https://developers.klaviyo.com/en/v2023-02-22/reference/create_template_render)
+#### [Create Template Render](https://developers.klaviyo.com/en/v2023-06-15/reference/create_template_render)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Templates.create_template_render(body)
 ```
 
 
 
 
-#### [Delete Template](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_template)
+#### [Delete Template](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_template)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Templates.delete_template(id)
 ```
 
 
 
 
-#### [Get Template](https://developers.klaviyo.com/en/v2023-02-22/reference/get_template)
+#### [Get Template](https://developers.klaviyo.com/en/v2023-06-15/reference/get_template)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2743,15 +2732,15 @@
 
 klaviyo.Templates.get_template(id, fields_template=fields_template)
 ```
 
 
 
 
-#### [Get Templates](https://developers.klaviyo.com/en/v2023-02-22/reference/get_templates)
+#### [Get Templates](https://developers.klaviyo.com/en/v2023-06-15/reference/get_templates)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_template | [str]
 # filter | str
@@ -2760,15 +2749,15 @@
 
 klaviyo.Templates.get_templates(fields_template=fields_template, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Update Template](https://developers.klaviyo.com/en/v2023-02-22/reference/update_template)
+#### [Update Template](https://developers.klaviyo.com/en/v2023-06-15/reference/update_template)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -2813,7 +2802,8 @@
 
 ## Namespace
 
 In the interest of making the SDK Pythonic, we made the following namespace changes *relative* to the language agnostic resources up top (API Docs, Guides, etc).
 
 - Resource names use Title + Snake Casing, (e.g. `Data_Privacy`)
 - function names and parameter names use snake case (e.g. `get_metrics`, and `profile_id`)
+
```

### Comparing `klaviyo-api-2.0.2/README.md` & `klaviyo-api-3.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Klaviyo Python SDK
 
-- SDK version: 2.0.2
-- API revision: 2023-02-22
+- SDK version: 3.0.0
+- API revision: 2023-06-15
 
 ## Helpful Resources
 
-- [API Reference](https://developers.klaviyo.com/en/v2023-02-22/reference)
-- [API Guides](https://developers.klaviyo.com/en/v2023-02-22/docs)
+- [API Reference](https://developers.klaviyo.com/en/v2023-06-15/reference)
+- [API Guides](https://developers.klaviyo.com/en/v2023-06-15/docs)
 - [Postman Workspace](https://www.postman.com/klaviyo/workspace/klaviyo-developers)
 - [Interactive Guide (Jupyter Notebook)](https://github.com/klaviyo-labs/klaviyo-api-guides)
 
 ## Design & Approach
 
 This SDK is a thin wrapper around our API. See our API Reference for full documentation on behavior.
 
@@ -18,23 +18,23 @@
 
 ## Organization
 
 This SDK is organized into the following resources:
 
 
 
-- Campaigns
+- Accounts
 
 
 
-- Catalogs
+- Campaigns
 
 
 
-- Client
+- Catalogs
 
 
 
 - Data_Privacy
 
 
 
@@ -117,16 +117,14 @@
 klaviyo.Events.get_events(
     fields_event=['event_properties'], 
     filter="equals(metric_id,\"aBc123\")", 
     sort='-datetime'
     )
 ```
 
-NOTE: the filter param values need to be url-encoded
-
 #### How to filter based on datetime
 
 **Use Case**: Get profiles that have been updated between two datetimes.
 
 ```python
 klaviyo.Profiles.get_profiles(
     filter='less-than(updated,2023-04-26T00:00:00Z),greater-than(updated,2023-04-19T00:00:00Z)'
@@ -200,107 +198,142 @@
             keys = YOUR_EXCEPTION.headers.keys()
             values = YOUR_EXCEPTION.headers.values()
             ```
 
 ## Important Notes
 
 - The main difference between this SDK and the language-agnostic API Docs that the below endpoints link to is that this SDK automatically adds the `revision` header corresponding to the SDK version.
-- Organization: Resource groups and operation_ids are listed below in alphabetical order, first by Resource name, then by **OpenAPI Summary**. Operation summaries are those listed in the right side bar of the [API Reference](https://developers.klaviyo.com/en/v2023-02-22/reference/get_events).
+- Organization: Resource groups and operation_ids are listed below in alphabetical order, first by Resource name, then by **OpenAPI Summary**. Operation summaries are those listed in the right side bar of the [API Reference](https://developers.klaviyo.com/en/v2023-06-15/reference/get_events).
 - For example values / data types, as well as whether parameters are required/optional, please reference the corresponding API Reference link.
 - Some keyword args may potentially be required for the API call to succeed, the linked API docs are the source of truth regarding which keyword params are required.
 - JSON payloads should be passed in as native python dictionaries.
 - You can override the client private key by passing in an optional `api_key` keyword arg to any API call that takes a private key. As a reminder: do NOT do this client-side/onsite.
 
 # Comprehensive list of Operations & Parameters
 
 
 
 
 
+## Accounts
+
+#### [Get Account](https://developers.klaviyo.com/en/v2023-06-15/reference/get_account)
+
+```python
+## Positional Arguments
+
+# id | str
+
+## Keyword Arguments
+
+# fields_account | [str]
+
+klaviyo.Accounts.get_account(id, fields_account=fields_account)
+```
+
+
+
+
+#### [Get Accounts](https://developers.klaviyo.com/en/v2023-06-15/reference/get_accounts)
+
+```python
+
+## Keyword Arguments
+
+# fields_account | [str]
+
+klaviyo.Accounts.get_accounts(fields_account=fields_account)
+```
+
+
+
+
+
+
 ## Campaigns
 
-#### [Create Campaign](https://developers.klaviyo.com/en/v2023-02-22/reference/create_campaign)
+#### [Create Campaign](https://developers.klaviyo.com/en/v2023-06-15/reference/create_campaign)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Campaigns.create_campaign(body)
 ```
 
 
 
 
-#### [Create Campaign Clone](https://developers.klaviyo.com/en/v2023-02-22/reference/create_campaign_clone)
+#### [Create Campaign Clone](https://developers.klaviyo.com/en/v2023-06-15/reference/create_campaign_clone)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Campaigns.create_campaign_clone(body)
 ```
 
 
 
 
-#### [Assign Campaign Message Template](https://developers.klaviyo.com/en/v2023-02-22/reference/create_campaign_message_assign_template)
+#### [Assign Campaign Message Template](https://developers.klaviyo.com/en/v2023-06-15/reference/create_campaign_message_assign_template)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Campaigns.create_campaign_message_assign_template(body)
 ```
 
 
 
 
-#### [Create Campaign Recipient Estimation Job](https://developers.klaviyo.com/en/v2023-02-22/reference/create_campaign_recipient_estimation_job)
+#### [Create Campaign Recipient Estimation Job](https://developers.klaviyo.com/en/v2023-06-15/reference/create_campaign_recipient_estimation_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Campaigns.create_campaign_recipient_estimation_job(body)
 ```
 
 
 
 
-#### [Create Campaign Send Job](https://developers.klaviyo.com/en/v2023-02-22/reference/create_campaign_send_job)
+#### [Create Campaign Send Job](https://developers.klaviyo.com/en/v2023-06-15/reference/create_campaign_send_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Campaigns.create_campaign_send_job(body)
 ```
 
 
 
 
-#### [Delete Campaign](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_campaign)
+#### [Delete Campaign](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_campaign)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Campaigns.delete_campaign(id)
 ```
 
 
 
 
-#### [Get Campaign](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaign)
+#### [Get Campaign](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaign)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -311,15 +344,15 @@
 
 klaviyo.Campaigns.get_campaign(id, fields_campaign=fields_campaign, fields_tag=fields_tag, include=include)
 ```
 
 
 
 
-#### [Get Campaign Message](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaign_message)
+#### [Get Campaign Message](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaign_message)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -328,15 +361,15 @@
 
 klaviyo.Campaigns.get_campaign_message(id, fields_campaign_message=fields_campaign_message)
 ```
 
 
 
 
-#### [Get Campaign Recipient Estimation](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaign_recipient_estimation)
+#### [Get Campaign Recipient Estimation](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaign_recipient_estimation)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -345,15 +378,15 @@
 
 klaviyo.Campaigns.get_campaign_recipient_estimation(id, fields_campaign_recipient_estimation=fields_campaign_recipient_estimation)
 ```
 
 
 
 
-#### [Get Campaign Recipient Estimation Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaign_recipient_estimation_job)
+#### [Get Campaign Recipient Estimation Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaign_recipient_estimation_job)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -362,28 +395,28 @@
 
 klaviyo.Campaigns.get_campaign_recipient_estimation_job(id, fields_campaign_recipient_estimation_job=fields_campaign_recipient_estimation_job)
 ```
 
 
 
 
-#### [Get Campaign Relationships Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaign_relationships_tags)
+#### [Get Campaign Relationships Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaign_relationships_tags)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Campaigns.get_campaign_relationships_tags(id)
 ```
 
 
 
 
-#### [Get Campaign Send Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaign_send_job)
+#### [Get Campaign Send Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaign_send_job)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -392,32 +425,32 @@
 
 klaviyo.Campaigns.get_campaign_send_job(id, fields_campaign_send_job=fields_campaign_send_job)
 ```
 
 
 
 
-#### [Get Campaign Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaign_tags)
+#### [Get Campaign Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaign_tags)
 
 ```python
 ## Positional Arguments
 
-# campaign_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_tag | [str]
 
-klaviyo.Campaigns.get_campaign_tags(campaign_id, fields_tag=fields_tag)
+klaviyo.Campaigns.get_campaign_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
-#### [Get Campaigns](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaigns)
+#### [Get Campaigns](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaigns)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_campaign | [str]
 # fields_tag | [str]
@@ -428,43 +461,43 @@
 
 klaviyo.Campaigns.get_campaigns(fields_campaign=fields_campaign, fields_tag=fields_tag, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Update Campaign](https://developers.klaviyo.com/en/v2023-02-22/reference/update_campaign)
+#### [Update Campaign](https://developers.klaviyo.com/en/v2023-06-15/reference/update_campaign)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Campaigns.update_campaign(id, body)
 ```
 
 
 
 
-#### [Update Campaign Message](https://developers.klaviyo.com/en/v2023-02-22/reference/update_campaign_message)
+#### [Update Campaign Message](https://developers.klaviyo.com/en/v2023-06-15/reference/update_campaign_message)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Campaigns.update_campaign_message(id, body)
 ```
 
 
 
 
-#### [Update Campaign Send Job](https://developers.klaviyo.com/en/v2023-02-22/reference/update_campaign_send_job)
+#### [Update Campaign Send Job](https://developers.klaviyo.com/en/v2023-06-15/reference/update_campaign_send_job)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -474,149 +507,149 @@
 
 
 
 
 
 ## Catalogs
 
-#### [Create Catalog Category](https://developers.klaviyo.com/en/v2023-02-22/reference/create_catalog_category)
+#### [Create Catalog Category](https://developers.klaviyo.com/en/v2023-06-15/reference/create_catalog_category)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.create_catalog_category(body)
 ```
 
 
 
 
-#### [Create Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-02-22/reference/create_catalog_category_relationships_items)
+#### [Create Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-06-15/reference/create_catalog_category_relationships_items)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.create_catalog_category_relationships_items(id, body)
 ```
 
 
 
 
-#### [Create Catalog Item](https://developers.klaviyo.com/en/v2023-02-22/reference/create_catalog_item)
+#### [Create Catalog Item](https://developers.klaviyo.com/en/v2023-06-15/reference/create_catalog_item)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.create_catalog_item(body)
 ```
 
 
 
 
-#### [Create Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-02-22/reference/create_catalog_item_relationships_categories)
+#### [Create Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-06-15/reference/create_catalog_item_relationships_categories)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.create_catalog_item_relationships_categories(id, body)
 ```
 
 
 
 
-#### [Create Catalog Variant](https://developers.klaviyo.com/en/v2023-02-22/reference/create_catalog_variant)
+#### [Create Catalog Variant](https://developers.klaviyo.com/en/v2023-06-15/reference/create_catalog_variant)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.create_catalog_variant(body)
 ```
 
 
 
 
-#### [Delete Catalog Category](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_catalog_category)
+#### [Delete Catalog Category](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_catalog_category)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Catalogs.delete_catalog_category(id)
 ```
 
 
 
 
-#### [Delete Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_catalog_category_relationships_items)
+#### [Delete Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_catalog_category_relationships_items)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.delete_catalog_category_relationships_items(id, body)
 ```
 
 
 
 
-#### [Delete Catalog Item](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_catalog_item)
+#### [Delete Catalog Item](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_catalog_item)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Catalogs.delete_catalog_item(id)
 ```
 
 
 
 
-#### [Delete Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_catalog_item_relationships_categories)
+#### [Delete Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_catalog_item_relationships_categories)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.delete_catalog_item_relationships_categories(id, body)
 ```
 
 
 
 
-#### [Delete Catalog Variant](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_catalog_variant)
+#### [Delete Catalog Variant](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_catalog_variant)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Catalogs.delete_catalog_variant(id)
 ```
 
 
 
 
-#### [Get Catalog Categories](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_categories)
+#### [Get Catalog Categories](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_categories)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_category | [str]
 # filter | str
@@ -625,15 +658,15 @@
 
 klaviyo.Catalogs.get_catalog_categories(fields_catalog_category=fields_catalog_category, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Get Catalog Category](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_category)
+#### [Get Catalog Category](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_category)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -642,37 +675,37 @@
 
 klaviyo.Catalogs.get_catalog_category(id, fields_catalog_category=fields_catalog_category)
 ```
 
 
 
 
-#### [Get Catalog Category Items](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_category_items)
+#### [Get Catalog Category Items](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_category_items)
 
 ```python
 ## Positional Arguments
 
-# category_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_catalog_item | [str]
 # fields_catalog_variant | [str]
 # filter | str
 # include | [str]
 # page_cursor | str
 # sort | str
 
-klaviyo.Catalogs.get_catalog_category_items(category_id, fields_catalog_item=fields_catalog_item, fields_catalog_variant=fields_catalog_variant, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
+klaviyo.Catalogs.get_catalog_category_items(id, fields_catalog_item=fields_catalog_item, fields_catalog_variant=fields_catalog_variant, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Get Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_category_relationships_items)
+#### [Get Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_category_relationships_items)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -681,15 +714,15 @@
 
 klaviyo.Catalogs.get_catalog_category_relationships_items(id, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Catalog Item](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_item)
+#### [Get Catalog Item](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_item)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -700,35 +733,35 @@
 
 klaviyo.Catalogs.get_catalog_item(id, fields_catalog_item=fields_catalog_item, fields_catalog_variant=fields_catalog_variant, include=include)
 ```
 
 
 
 
-#### [Get Catalog Item Categories](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_item_categories)
+#### [Get Catalog Item Categories](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_item_categories)
 
 ```python
 ## Positional Arguments
 
-# item_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_catalog_category | [str]
 # filter | str
 # page_cursor | str
 # sort | str
 
-klaviyo.Catalogs.get_catalog_item_categories(item_id, fields_catalog_category=fields_catalog_category, filter=filter, page_cursor=page_cursor, sort=sort)
+klaviyo.Catalogs.get_catalog_item_categories(id, fields_catalog_category=fields_catalog_category, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Get Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_item_relationships_categories)
+#### [Get Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_item_relationships_categories)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -737,35 +770,35 @@
 
 klaviyo.Catalogs.get_catalog_item_relationships_categories(id, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Catalog Item Variants](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_item_variants)
+#### [Get Catalog Item Variants](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_item_variants)
 
 ```python
 ## Positional Arguments
 
-# item_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_catalog_variant | [str]
 # filter | str
 # page_cursor | str
 # sort | str
 
-klaviyo.Catalogs.get_catalog_item_variants(item_id, fields_catalog_variant=fields_catalog_variant, filter=filter, page_cursor=page_cursor, sort=sort)
+klaviyo.Catalogs.get_catalog_item_variants(id, fields_catalog_variant=fields_catalog_variant, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Get Catalog Items](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_items)
+#### [Get Catalog Items](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_items)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_item | [str]
 # fields_catalog_variant | [str]
@@ -776,15 +809,15 @@
 
 klaviyo.Catalogs.get_catalog_items(fields_catalog_item=fields_catalog_item, fields_catalog_variant=fields_catalog_variant, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Get Catalog Variant](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_variant)
+#### [Get Catalog Variant](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_variant)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -793,15 +826,15 @@
 
 klaviyo.Catalogs.get_catalog_variant(id, fields_catalog_variant=fields_catalog_variant)
 ```
 
 
 
 
-#### [Get Catalog Variants](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_variants)
+#### [Get Catalog Variants](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_variants)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_variant | [str]
 # filter | str
@@ -810,15 +843,15 @@
 
 klaviyo.Catalogs.get_catalog_variants(fields_catalog_variant=fields_catalog_variant, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Get Create Categories Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_create_categories_job)
+#### [Get Create Categories Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_create_categories_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -829,15 +862,15 @@
 
 klaviyo.Catalogs.get_create_categories_job(job_id, fields_catalog_category_bulk_create_job=fields_catalog_category_bulk_create_job, fields_catalog_category=fields_catalog_category, include=include)
 ```
 
 
 
 
-#### [Get Create Categories Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_create_categories_jobs)
+#### [Get Create Categories Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_create_categories_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_category_bulk_create_job | [str]
 # filter | str
@@ -845,15 +878,15 @@
 
 klaviyo.Catalogs.get_create_categories_jobs(fields_catalog_category_bulk_create_job=fields_catalog_category_bulk_create_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Create Items Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_create_items_job)
+#### [Get Create Items Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_create_items_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -864,15 +897,15 @@
 
 klaviyo.Catalogs.get_create_items_job(job_id, fields_catalog_item_bulk_create_job=fields_catalog_item_bulk_create_job, fields_catalog_item=fields_catalog_item, include=include)
 ```
 
 
 
 
-#### [Get Create Items Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_create_items_jobs)
+#### [Get Create Items Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_create_items_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_item_bulk_create_job | [str]
 # filter | str
@@ -880,15 +913,15 @@
 
 klaviyo.Catalogs.get_create_items_jobs(fields_catalog_item_bulk_create_job=fields_catalog_item_bulk_create_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Create Variants Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_create_variants_job)
+#### [Get Create Variants Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_create_variants_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -899,15 +932,15 @@
 
 klaviyo.Catalogs.get_create_variants_job(job_id, fields_catalog_variant_bulk_create_job=fields_catalog_variant_bulk_create_job, fields_catalog_variant=fields_catalog_variant, include=include)
 ```
 
 
 
 
-#### [Get Create Variants Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_create_variants_jobs)
+#### [Get Create Variants Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_create_variants_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_variant_bulk_create_job | [str]
 # filter | str
@@ -915,15 +948,15 @@
 
 klaviyo.Catalogs.get_create_variants_jobs(fields_catalog_variant_bulk_create_job=fields_catalog_variant_bulk_create_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Delete Categories Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_delete_categories_job)
+#### [Get Delete Categories Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_delete_categories_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -932,15 +965,15 @@
 
 klaviyo.Catalogs.get_delete_categories_job(job_id, fields_catalog_category_bulk_delete_job=fields_catalog_category_bulk_delete_job)
 ```
 
 
 
 
-#### [Get Delete Categories Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_delete_categories_jobs)
+#### [Get Delete Categories Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_delete_categories_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_category_bulk_delete_job | [str]
 # filter | str
@@ -948,15 +981,15 @@
 
 klaviyo.Catalogs.get_delete_categories_jobs(fields_catalog_category_bulk_delete_job=fields_catalog_category_bulk_delete_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Delete Items Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_delete_items_job)
+#### [Get Delete Items Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_delete_items_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -965,15 +998,15 @@
 
 klaviyo.Catalogs.get_delete_items_job(job_id, fields_catalog_item_bulk_delete_job=fields_catalog_item_bulk_delete_job)
 ```
 
 
 
 
-#### [Get Delete Items Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_delete_items_jobs)
+#### [Get Delete Items Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_delete_items_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_item_bulk_delete_job | [str]
 # filter | str
@@ -981,15 +1014,15 @@
 
 klaviyo.Catalogs.get_delete_items_jobs(fields_catalog_item_bulk_delete_job=fields_catalog_item_bulk_delete_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Delete Variants Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_delete_variants_job)
+#### [Get Delete Variants Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_delete_variants_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -998,15 +1031,15 @@
 
 klaviyo.Catalogs.get_delete_variants_job(job_id, fields_catalog_variant_bulk_delete_job=fields_catalog_variant_bulk_delete_job)
 ```
 
 
 
 
-#### [Get Delete Variants Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_delete_variants_jobs)
+#### [Get Delete Variants Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_delete_variants_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_variant_bulk_delete_job | [str]
 # filter | str
@@ -1014,15 +1047,15 @@
 
 klaviyo.Catalogs.get_delete_variants_jobs(fields_catalog_variant_bulk_delete_job=fields_catalog_variant_bulk_delete_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Update Categories Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_update_categories_job)
+#### [Get Update Categories Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_update_categories_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -1033,15 +1066,15 @@
 
 klaviyo.Catalogs.get_update_categories_job(job_id, fields_catalog_category_bulk_update_job=fields_catalog_category_bulk_update_job, fields_catalog_category=fields_catalog_category, include=include)
 ```
 
 
 
 
-#### [Get Update Categories Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_update_categories_jobs)
+#### [Get Update Categories Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_update_categories_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_category_bulk_update_job | [str]
 # filter | str
@@ -1049,15 +1082,15 @@
 
 klaviyo.Catalogs.get_update_categories_jobs(fields_catalog_category_bulk_update_job=fields_catalog_category_bulk_update_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Update Items Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_update_items_job)
+#### [Get Update Items Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_update_items_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -1068,15 +1101,15 @@
 
 klaviyo.Catalogs.get_update_items_job(job_id, fields_catalog_item_bulk_update_job=fields_catalog_item_bulk_update_job, fields_catalog_item=fields_catalog_item, include=include)
 ```
 
 
 
 
-#### [Get Update Items Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_update_items_jobs)
+#### [Get Update Items Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_update_items_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_item_bulk_update_job | [str]
 # filter | str
@@ -1084,15 +1117,15 @@
 
 klaviyo.Catalogs.get_update_items_jobs(fields_catalog_item_bulk_update_job=fields_catalog_item_bulk_update_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Update Variants Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_update_variants_job)
+#### [Get Update Variants Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_update_variants_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -1103,15 +1136,15 @@
 
 klaviyo.Catalogs.get_update_variants_job(job_id, fields_catalog_variant_bulk_update_job=fields_catalog_variant_bulk_update_job, fields_catalog_variant=fields_catalog_variant, include=include)
 ```
 
 
 
 
-#### [Get Update Variants Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_update_variants_jobs)
+#### [Get Update Variants Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_update_variants_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_variant_bulk_update_job | [str]
 # filter | str
@@ -1119,188 +1152,188 @@
 
 klaviyo.Catalogs.get_update_variants_jobs(fields_catalog_variant_bulk_update_job=fields_catalog_variant_bulk_update_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Spawn Create Categories Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_create_categories_job)
+#### [Spawn Create Categories Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_create_categories_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_create_categories_job(body)
 ```
 
 
 
 
-#### [Spawn Create Items Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_create_items_job)
+#### [Spawn Create Items Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_create_items_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_create_items_job(body)
 ```
 
 
 
 
-#### [Spawn Create Variants Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_create_variants_job)
+#### [Spawn Create Variants Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_create_variants_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_create_variants_job(body)
 ```
 
 
 
 
-#### [Spawn Delete Categories Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_delete_categories_job)
+#### [Spawn Delete Categories Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_delete_categories_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_delete_categories_job(body)
 ```
 
 
 
 
-#### [Spawn Delete Items Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_delete_items_job)
+#### [Spawn Delete Items Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_delete_items_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_delete_items_job(body)
 ```
 
 
 
 
-#### [Spawn Delete Variants Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_delete_variants_job)
+#### [Spawn Delete Variants Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_delete_variants_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_delete_variants_job(body)
 ```
 
 
 
 
-#### [Spawn Update Categories Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_update_categories_job)
+#### [Spawn Update Categories Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_update_categories_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_update_categories_job(body)
 ```
 
 
 
 
-#### [Spawn Update Items Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_update_items_job)
+#### [Spawn Update Items Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_update_items_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_update_items_job(body)
 ```
 
 
 
 
-#### [Spawn Update Variants Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_update_variants_job)
+#### [Spawn Update Variants Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_update_variants_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_update_variants_job(body)
 ```
 
 
 
 
-#### [Update Catalog Category](https://developers.klaviyo.com/en/v2023-02-22/reference/update_catalog_category)
+#### [Update Catalog Category](https://developers.klaviyo.com/en/v2023-06-15/reference/update_catalog_category)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.update_catalog_category(id, body)
 ```
 
 
 
 
-#### [Update Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-02-22/reference/update_catalog_category_relationships_items)
+#### [Update Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-06-15/reference/update_catalog_category_relationships_items)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.update_catalog_category_relationships_items(id, body)
 ```
 
 
 
 
-#### [Update Catalog Item](https://developers.klaviyo.com/en/v2023-02-22/reference/update_catalog_item)
+#### [Update Catalog Item](https://developers.klaviyo.com/en/v2023-06-15/reference/update_catalog_item)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.update_catalog_item(id, body)
 ```
 
 
 
 
-#### [Update Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-02-22/reference/update_catalog_item_relationships_categories)
+#### [Update Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-06-15/reference/update_catalog_item_relationships_categories)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.update_catalog_item_relationships_categories(id, body)
 ```
 
 
 
 
-#### [Update Catalog Variant](https://developers.klaviyo.com/en/v2023-02-22/reference/update_catalog_variant)
+#### [Update Catalog Variant](https://developers.klaviyo.com/en/v2023-06-15/reference/update_catalog_variant)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -1308,63 +1341,17 @@
 ```
 
 
 
 
 
 
-## Client
-
-#### [Create Client Event](https://developers.klaviyo.com/en/v2023-02-22/reference/create_client_event)
-
-```python
-## Positional Arguments
-
-# company_id | str
-# body | dict
-
-klaviyo.Client.create_client_event(company_id, body)
-```
-
-
-
-
-#### [Create or Update Client Profile](https://developers.klaviyo.com/en/v2023-02-22/reference/create_client_profile)
-
-```python
-## Positional Arguments
-
-# company_id | str
-# body | dict
-
-klaviyo.Client.create_client_profile(company_id, body)
-```
-
-
-
-
-#### [Create Client Subscription](https://developers.klaviyo.com/en/v2023-02-22/reference/create_client_subscription)
-
-```python
-## Positional Arguments
-
-# company_id | str
-# body | dict
-
-klaviyo.Client.create_client_subscription(company_id, body)
-```
-
-
-
-
-
-
 ## Data_Privacy
 
-#### [Request Profile Deletion](https://developers.klaviyo.com/en/v2023-02-22/reference/request_profile_deletion)
+#### [Request Profile Deletion](https://developers.klaviyo.com/en/v2023-06-15/reference/request_profile_deletion)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Data_Privacy.request_profile_deletion(body)
@@ -1373,28 +1360,28 @@
 
 
 
 
 
 ## Events
 
-#### [Create Event](https://developers.klaviyo.com/en/v2023-02-22/reference/create_event)
+#### [Create Event](https://developers.klaviyo.com/en/v2023-06-15/reference/create_event)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Events.create_event(body)
 ```
 
 
 
 
-#### [Get Event](https://developers.klaviyo.com/en/v2023-02-22/reference/get_event)
+#### [Get Event](https://developers.klaviyo.com/en/v2023-06-15/reference/get_event)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1406,15 +1393,15 @@
 
 klaviyo.Events.get_event(id, fields_event=fields_event, fields_metric=fields_metric, fields_profile=fields_profile, include=include)
 ```
 
 
 
 
-#### [Get Event Metrics](https://developers.klaviyo.com/en/v2023-02-22/reference/get_event_metrics)
+#### [Get Event Metrics](https://developers.klaviyo.com/en/v2023-06-15/reference/get_event_metrics)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1423,15 +1410,15 @@
 
 klaviyo.Events.get_event_metrics(id, fields_metric=fields_metric)
 ```
 
 
 
 
-#### [Get Event Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/get_event_profiles)
+#### [Get Event Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/get_event_profiles)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1441,41 +1428,41 @@
 
 klaviyo.Events.get_event_profiles(id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile)
 ```
 
 
 
 
-#### [Get Event Relationships Metrics](https://developers.klaviyo.com/en/v2023-02-22/reference/get_event_relationships_metrics)
+#### [Get Event Relationships Metrics](https://developers.klaviyo.com/en/v2023-06-15/reference/get_event_relationships_metrics)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Events.get_event_relationships_metrics(id)
 ```
 
 
 
 
-#### [Get Event Relationships Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/get_event_relationships_profiles)
+#### [Get Event Relationships Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/get_event_relationships_profiles)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Events.get_event_relationships_profiles(id)
 ```
 
 
 
 
-#### [Get Events](https://developers.klaviyo.com/en/v2023-02-22/reference/get_events)
+#### [Get Events](https://developers.klaviyo.com/en/v2023-06-15/reference/get_events)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_event | [str]
 # fields_metric | [str]
@@ -1491,15 +1478,15 @@
 
 
 
 
 
 ## Flows
 
-#### [Get Flow](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow)
+#### [Get Flow](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1510,15 +1497,15 @@
 
 klaviyo.Flows.get_flow(id, fields_flow_action=fields_flow_action, fields_flow=fields_flow, include=include)
 ```
 
 
 
 
-#### [Get Flow Action](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_action)
+#### [Get Flow Action](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_action)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1530,66 +1517,66 @@
 
 klaviyo.Flows.get_flow_action(id, fields_flow_action=fields_flow_action, fields_flow_message=fields_flow_message, fields_flow=fields_flow, include=include)
 ```
 
 
 
 
-#### [Get Flow For Flow Action](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_action_flow)
+#### [Get Flow For Flow Action](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_action_flow)
 
 ```python
 ## Positional Arguments
 
-# action_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_flow | [str]
 
-klaviyo.Flows.get_flow_action_flow(action_id, fields_flow=fields_flow)
+klaviyo.Flows.get_flow_action_flow(id, fields_flow=fields_flow)
 ```
 
 
 
 
-#### [Get Messages For Flow Action](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_action_messages)
+#### [Get Messages For Flow Action](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_action_messages)
 
 ```python
 ## Positional Arguments
 
-# action_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_flow_message | [str]
 # filter | str
 # page_cursor | str
 # page_size | int
 # sort | str
 
-klaviyo.Flows.get_flow_action_messages(action_id, fields_flow_message=fields_flow_message, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
+klaviyo.Flows.get_flow_action_messages(id, fields_flow_message=fields_flow_message, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
-#### [Get Flow Action Relationships Flow](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_action_relationships_flow)
+#### [Get Flow Action Relationships Flow](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_action_relationships_flow)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Flows.get_flow_action_relationships_flow(id)
 ```
 
 
 
 
-#### [Get Flow Action Relationships Messages](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_action_relationships_messages)
+#### [Get Flow Action Relationships Messages](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_action_relationships_messages)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1601,36 +1588,36 @@
 
 klaviyo.Flows.get_flow_action_relationships_messages(id, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
-#### [Get Flow Actions For Flow](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_flow_actions)
+#### [Get Flow Actions For Flow](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_flow_actions)
 
 ```python
 ## Positional Arguments
 
-# flow_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_flow_action | [str]
 # filter | str
 # page_cursor | str
 # page_size | int
 # sort | str
 
-klaviyo.Flows.get_flow_flow_actions(flow_id, fields_flow_action=fields_flow_action, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
+klaviyo.Flows.get_flow_flow_actions(id, fields_flow_action=fields_flow_action, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
-#### [Get Flow Message](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_message)
+#### [Get Flow Message](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_message)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1641,45 +1628,45 @@
 
 klaviyo.Flows.get_flow_message(id, fields_flow_action=fields_flow_action, fields_flow_message=fields_flow_message, include=include)
 ```
 
 
 
 
-#### [Get Flow Action For Message](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_message_action)
+#### [Get Flow Action For Message](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_message_action)
 
 ```python
 ## Positional Arguments
 
-# message_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_flow_action | [str]
 
-klaviyo.Flows.get_flow_message_action(message_id, fields_flow_action=fields_flow_action)
+klaviyo.Flows.get_flow_message_action(id, fields_flow_action=fields_flow_action)
 ```
 
 
 
 
-#### [Get Flow Message Relationships Action](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_message_relationships_action)
+#### [Get Flow Message Relationships Action](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_message_relationships_action)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Flows.get_flow_message_relationships_action(id)
 ```
 
 
 
 
-#### [Get Flow Relationships Flow Actions](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_relationships_flow_actions)
+#### [Get Flow Relationships Flow Actions](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_relationships_flow_actions)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1690,45 +1677,45 @@
 
 klaviyo.Flows.get_flow_relationships_flow_actions(id, filter=filter, page_size=page_size, sort=sort)
 ```
 
 
 
 
-#### [Get Flow Relationships Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_relationships_tags)
+#### [Get Flow Relationships Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_relationships_tags)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Flows.get_flow_relationships_tags(id)
 ```
 
 
 
 
-#### [Get Flow Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_tags)
+#### [Get Flow Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_tags)
 
 ```python
 ## Positional Arguments
 
-# flow_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_tag | [str]
 
-klaviyo.Flows.get_flow_tags(flow_id, fields_tag=fields_tag)
+klaviyo.Flows.get_flow_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
-#### [Get Flows](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flows)
+#### [Get Flows](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flows)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_flow_action | [str]
 # fields_flow | [str]
@@ -1740,15 +1727,15 @@
 
 klaviyo.Flows.get_flows(fields_flow_action=fields_flow_action, fields_flow=fields_flow, filter=filter, include=include, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
-#### [Update Flow Status](https://developers.klaviyo.com/en/v2023-02-22/reference/update_flow)
+#### [Update Flow Status](https://developers.klaviyo.com/en/v2023-06-15/reference/update_flow)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -1758,69 +1745,69 @@
 
 
 
 
 
 ## Lists
 
-#### [Create List](https://developers.klaviyo.com/en/v2023-02-22/reference/create_list)
+#### [Create List](https://developers.klaviyo.com/en/v2023-06-15/reference/create_list)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Lists.create_list(body)
 ```
 
 
 
 
-#### [Add Profile To List](https://developers.klaviyo.com/en/v2023-02-22/reference/create_list_relationships)
+#### [Add Profile To List](https://developers.klaviyo.com/en/v2023-06-15/reference/create_list_relationships)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Lists.create_list_relationships(id, body)
 ```
 
 
 
 
-#### [Delete List](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_list)
+#### [Delete List](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_list)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Lists.delete_list(id)
 ```
 
 
 
 
-#### [Remove Profile From List](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_list_relationships)
+#### [Remove Profile From List](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_list_relationships)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Lists.delete_list_relationships(id, body)
 ```
 
 
 
 
-#### [Get List](https://developers.klaviyo.com/en/v2023-02-22/reference/get_list)
+#### [Get List](https://developers.klaviyo.com/en/v2023-06-15/reference/get_list)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1829,36 +1816,36 @@
 
 klaviyo.Lists.get_list(id, fields_list=fields_list)
 ```
 
 
 
 
-#### [Get List Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/get_list_profiles)
+#### [Get List Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/get_list_profiles)
 
 ```python
 ## Positional Arguments
 
-# list_id | str
+# id | str
 
 ## Keyword Arguments
 
 # additional_fields_profile | [str]
 # fields_profile | [str]
 # filter | str
 # page_cursor | str
 # page_size | int
 
-klaviyo.Lists.get_list_profiles(list_id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size)
+klaviyo.Lists.get_list_profiles(id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size)
 ```
 
 
 
 
-#### [Get List Relationships Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/get_list_relationships_profiles)
+#### [Get List Relationships Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/get_list_relationships_profiles)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1867,45 +1854,45 @@
 
 klaviyo.Lists.get_list_relationships_profiles(id, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get List Relationships Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_list_relationships_tags)
+#### [Get List Relationships Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_list_relationships_tags)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Lists.get_list_relationships_tags(id)
 ```
 
 
 
 
-#### [Get List Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_list_tags)
+#### [Get List Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_list_tags)
 
 ```python
 ## Positional Arguments
 
-# list_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_tag | [str]
 
-klaviyo.Lists.get_list_tags(list_id, fields_tag=fields_tag)
+klaviyo.Lists.get_list_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
-#### [Get Lists](https://developers.klaviyo.com/en/v2023-02-22/reference/get_lists)
+#### [Get Lists](https://developers.klaviyo.com/en/v2023-06-15/reference/get_lists)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_list | [str]
 # filter | str
@@ -1913,15 +1900,15 @@
 
 klaviyo.Lists.get_lists(fields_list=fields_list, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Update List](https://developers.klaviyo.com/en/v2023-02-22/reference/update_list)
+#### [Update List](https://developers.klaviyo.com/en/v2023-06-15/reference/update_list)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -1931,15 +1918,15 @@
 
 
 
 
 
 ## Metrics
 
-#### [Get Metric](https://developers.klaviyo.com/en/v2023-02-22/reference/get_metric)
+#### [Get Metric](https://developers.klaviyo.com/en/v2023-06-15/reference/get_metric)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1948,15 +1935,15 @@
 
 klaviyo.Metrics.get_metric(id, fields_metric=fields_metric)
 ```
 
 
 
 
-#### [Get Metrics](https://developers.klaviyo.com/en/v2023-02-22/reference/get_metrics)
+#### [Get Metrics](https://developers.klaviyo.com/en/v2023-06-15/reference/get_metrics)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_metric | [str]
 # filter | str
@@ -1964,15 +1951,15 @@
 
 klaviyo.Metrics.get_metrics(fields_metric=fields_metric, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Query Metric Aggregates](https://developers.klaviyo.com/en/v2023-02-22/reference/query_metric_aggregates)
+#### [Query Metric Aggregates](https://developers.klaviyo.com/en/v2023-06-15/reference/query_metric_aggregates)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Metrics.query_metric_aggregates(body)
@@ -1981,28 +1968,28 @@
 
 
 
 
 
 ## Profiles
 
-#### [Create Profile](https://developers.klaviyo.com/en/v2023-02-22/reference/create_profile)
+#### [Create Profile](https://developers.klaviyo.com/en/v2023-06-15/reference/create_profile)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Profiles.create_profile(body)
 ```
 
 
 
 
-#### [Get Profile](https://developers.klaviyo.com/en/v2023-02-22/reference/get_profile)
+#### [Get Profile](https://developers.klaviyo.com/en/v2023-06-15/reference/get_profile)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2015,75 +2002,75 @@
 
 klaviyo.Profiles.get_profile(id, additional_fields_profile=additional_fields_profile, fields_list=fields_list, fields_profile=fields_profile, fields_segment=fields_segment, include=include)
 ```
 
 
 
 
-#### [Get Profile Lists](https://developers.klaviyo.com/en/v2023-02-22/reference/get_profile_lists)
+#### [Get Profile Lists](https://developers.klaviyo.com/en/v2023-06-15/reference/get_profile_lists)
 
 ```python
 ## Positional Arguments
 
-# profile_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_list | [str]
 
-klaviyo.Profiles.get_profile_lists(profile_id, fields_list=fields_list)
+klaviyo.Profiles.get_profile_lists(id, fields_list=fields_list)
 ```
 
 
 
 
-#### [Get Profile Relationships Lists](https://developers.klaviyo.com/en/v2023-02-22/reference/get_profile_relationships_lists)
+#### [Get Profile Relationships Lists](https://developers.klaviyo.com/en/v2023-06-15/reference/get_profile_relationships_lists)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Profiles.get_profile_relationships_lists(id)
 ```
 
 
 
 
-#### [Get Profile Relationships Segments](https://developers.klaviyo.com/en/v2023-02-22/reference/get_profile_relationships_segments)
+#### [Get Profile Relationships Segments](https://developers.klaviyo.com/en/v2023-06-15/reference/get_profile_relationships_segments)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Profiles.get_profile_relationships_segments(id)
 ```
 
 
 
 
-#### [Get Profile Segments](https://developers.klaviyo.com/en/v2023-02-22/reference/get_profile_segments)
+#### [Get Profile Segments](https://developers.klaviyo.com/en/v2023-06-15/reference/get_profile_segments)
 
 ```python
 ## Positional Arguments
 
-# profile_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_segment | [str]
 
-klaviyo.Profiles.get_profile_segments(profile_id, fields_segment=fields_segment)
+klaviyo.Profiles.get_profile_segments(id, fields_segment=fields_segment)
 ```
 
 
 
 
-#### [Get Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/get_profiles)
+#### [Get Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/get_profiles)
 
 ```python
 
 ## Keyword Arguments
 
 # additional_fields_profile | [str]
 # fields_profile | [str]
@@ -2094,67 +2081,67 @@
 
 klaviyo.Profiles.get_profiles(additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
-#### [Subscribe Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/subscribe_profiles)
+#### [Subscribe Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/subscribe_profiles)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Profiles.subscribe_profiles(body)
 ```
 
 
 
 
-#### [Suppress Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/suppress_profiles)
+#### [Suppress Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/suppress_profiles)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Profiles.suppress_profiles(body)
 ```
 
 
 
 
-#### [Unsubscribe Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/unsubscribe_profiles)
+#### [Unsubscribe Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/unsubscribe_profiles)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Profiles.unsubscribe_profiles(body)
 ```
 
 
 
 
-#### [Unsuppress Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/unsuppress_profiles)
+#### [Unsuppress Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/unsuppress_profiles)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Profiles.unsuppress_profiles(body)
 ```
 
 
 
 
-#### [Update Profile](https://developers.klaviyo.com/en/v2023-02-22/reference/update_profile)
+#### [Update Profile](https://developers.klaviyo.com/en/v2023-06-15/reference/update_profile)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -2164,15 +2151,15 @@
 
 
 
 
 
 ## Segments
 
-#### [Get Segment](https://developers.klaviyo.com/en/v2023-02-22/reference/get_segment)
+#### [Get Segment](https://developers.klaviyo.com/en/v2023-06-15/reference/get_segment)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2181,36 +2168,36 @@
 
 klaviyo.Segments.get_segment(id, fields_segment=fields_segment)
 ```
 
 
 
 
-#### [Get Segment Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/get_segment_profiles)
+#### [Get Segment Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/get_segment_profiles)
 
 ```python
 ## Positional Arguments
 
-# segment_id | str
+# id | str
 
 ## Keyword Arguments
 
 # additional_fields_profile | [str]
 # fields_profile | [str]
 # filter | str
 # page_cursor | str
 # page_size | int
 
-klaviyo.Segments.get_segment_profiles(segment_id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size)
+klaviyo.Segments.get_segment_profiles(id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size)
 ```
 
 
 
 
-#### [Get Segment Relationships Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/get_segment_relationships_profiles)
+#### [Get Segment Relationships Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/get_segment_relationships_profiles)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2219,45 +2206,45 @@
 
 klaviyo.Segments.get_segment_relationships_profiles(id, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Segment Relationships Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_segment_relationships_tags)
+#### [Get Segment Relationships Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_segment_relationships_tags)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Segments.get_segment_relationships_tags(id)
 ```
 
 
 
 
-#### [Get Segment Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_segment_tags)
+#### [Get Segment Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_segment_tags)
 
 ```python
 ## Positional Arguments
 
-# segment_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_tag | [str]
 
-klaviyo.Segments.get_segment_tags(segment_id, fields_tag=fields_tag)
+klaviyo.Segments.get_segment_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
-#### [Get Segments](https://developers.klaviyo.com/en/v2023-02-22/reference/get_segments)
+#### [Get Segments](https://developers.klaviyo.com/en/v2023-06-15/reference/get_segments)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_segment | [str]
 # filter | str
@@ -2265,15 +2252,15 @@
 
 klaviyo.Segments.get_segments(fields_segment=fields_segment, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Update Segment](https://developers.klaviyo.com/en/v2023-02-22/reference/update_segment)
+#### [Update Segment](https://developers.klaviyo.com/en/v2023-06-15/reference/update_segment)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -2283,179 +2270,179 @@
 
 
 
 
 
 ## Tags
 
-#### [Create Tag](https://developers.klaviyo.com/en/v2023-02-22/reference/create_tag)
+#### [Create Tag](https://developers.klaviyo.com/en/v2023-06-15/reference/create_tag)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Tags.create_tag(body)
 ```
 
 
 
 
-#### [Create Tag Group](https://developers.klaviyo.com/en/v2023-02-22/reference/create_tag_group)
+#### [Create Tag Group](https://developers.klaviyo.com/en/v2023-06-15/reference/create_tag_group)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Tags.create_tag_group(body)
 ```
 
 
 
 
-#### [Create Tag Relationships Campaigns](https://developers.klaviyo.com/en/v2023-02-22/reference/create_tag_relationships_campaigns)
+#### [Create Tag Relationships Campaigns](https://developers.klaviyo.com/en/v2023-06-15/reference/create_tag_relationships_campaigns)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.create_tag_relationships_campaigns(id, body)
 ```
 
 
 
 
-#### [Create Tag Relationships Flows](https://developers.klaviyo.com/en/v2023-02-22/reference/create_tag_relationships_flows)
+#### [Create Tag Relationships Flows](https://developers.klaviyo.com/en/v2023-06-15/reference/create_tag_relationships_flows)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.create_tag_relationships_flows(id, body)
 ```
 
 
 
 
-#### [Create Tag Relationships Lists](https://developers.klaviyo.com/en/v2023-02-22/reference/create_tag_relationships_lists)
+#### [Create Tag Relationships Lists](https://developers.klaviyo.com/en/v2023-06-15/reference/create_tag_relationships_lists)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.create_tag_relationships_lists(id, body)
 ```
 
 
 
 
-#### [Create Tag Relationships Segments](https://developers.klaviyo.com/en/v2023-02-22/reference/create_tag_relationships_segments)
+#### [Create Tag Relationships Segments](https://developers.klaviyo.com/en/v2023-06-15/reference/create_tag_relationships_segments)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.create_tag_relationships_segments(id, body)
 ```
 
 
 
 
-#### [Delete Tag](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_tag)
+#### [Delete Tag](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_tag)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.delete_tag(id)
 ```
 
 
 
 
-#### [Delete Tag Group](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_tag_group)
+#### [Delete Tag Group](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_tag_group)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.delete_tag_group(id)
 ```
 
 
 
 
-#### [Delete Tag Relationships Campaigns](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_tag_relationships_campaigns)
+#### [Delete Tag Relationships Campaigns](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_tag_relationships_campaigns)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.delete_tag_relationships_campaigns(id, body)
 ```
 
 
 
 
-#### [Delete Tag Relationships Flows](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_tag_relationships_flows)
+#### [Delete Tag Relationships Flows](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_tag_relationships_flows)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.delete_tag_relationships_flows(id, body)
 ```
 
 
 
 
-#### [Delete Tag Relationships Lists](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_tag_relationships_lists)
+#### [Delete Tag Relationships Lists](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_tag_relationships_lists)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.delete_tag_relationships_lists(id, body)
 ```
 
 
 
 
-#### [Delete Tag Relationships Segments](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_tag_relationships_segments)
+#### [Delete Tag Relationships Segments](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_tag_relationships_segments)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.delete_tag_relationships_segments(id, body)
 ```
 
 
 
 
-#### [Get Tag](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag)
+#### [Get Tag](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2464,15 +2451,15 @@
 
 klaviyo.Tags.get_tag(id, fields_tag=fields_tag)
 ```
 
 
 
 
-#### [Get Tag Group](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_group)
+#### [Get Tag Group](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_group)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2481,28 +2468,28 @@
 
 klaviyo.Tags.get_tag_group(id, fields_tag_group=fields_tag_group)
 ```
 
 
 
 
-#### [Get Tag Group Relationships Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_group_relationships_tags)
+#### [Get Tag Group Relationships Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_group_relationships_tags)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.get_tag_group_relationships_tags(id)
 ```
 
 
 
 
-#### [Get Tag Group Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_group_tags)
+#### [Get Tag Group Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_group_tags)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2511,15 +2498,15 @@
 
 klaviyo.Tags.get_tag_group_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
-#### [Get Tag Groups](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_groups)
+#### [Get Tag Groups](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_groups)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_tag_group | [str]
 # filter | str
@@ -2528,80 +2515,80 @@
 
 klaviyo.Tags.get_tag_groups(fields_tag_group=fields_tag_group, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Get Tag Relationships Campaigns](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_relationships_campaigns)
+#### [Get Tag Relationships Campaigns](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_relationships_campaigns)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.get_tag_relationships_campaigns(id)
 ```
 
 
 
 
-#### [Get Tag Relationships Flows](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_relationships_flows)
+#### [Get Tag Relationships Flows](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_relationships_flows)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.get_tag_relationships_flows(id)
 ```
 
 
 
 
-#### [Get Tag Relationships Lists](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_relationships_lists)
+#### [Get Tag Relationships Lists](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_relationships_lists)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.get_tag_relationships_lists(id)
 ```
 
 
 
 
-#### [Get Tag Relationships Segments](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_relationships_segments)
+#### [Get Tag Relationships Segments](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_relationships_segments)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.get_tag_relationships_segments(id)
 ```
 
 
 
 
-#### [Get Tag Relationships Tag Group](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_relationships_tag_group)
+#### [Get Tag Relationships Tag Group](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_relationships_tag_group)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.get_tag_relationships_tag_group(id)
 ```
 
 
 
 
-#### [Get Tag Tag Group](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_tag_group)
+#### [Get Tag Tag Group](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_tag_group)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2610,15 +2597,15 @@
 
 klaviyo.Tags.get_tag_tag_group(id, fields_tag_group=fields_tag_group)
 ```
 
 
 
 
-#### [Get Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tags)
+#### [Get Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tags)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_tag | [str]
 # filter | str
@@ -2627,29 +2614,29 @@
 
 klaviyo.Tags.get_tags(fields_tag=fields_tag, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Update Tag](https://developers.klaviyo.com/en/v2023-02-22/reference/update_tag)
+#### [Update Tag](https://developers.klaviyo.com/en/v2023-06-15/reference/update_tag)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.update_tag(id, body)
 ```
 
 
 
 
-#### [Update Tag Group](https://developers.klaviyo.com/en/v2023-02-22/reference/update_tag_group)
+#### [Update Tag Group](https://developers.klaviyo.com/en/v2023-06-15/reference/update_tag_group)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -2659,67 +2646,67 @@
 
 
 
 
 
 ## Templates
 
-#### [Create Template](https://developers.klaviyo.com/en/v2023-02-22/reference/create_template)
+#### [Create Template](https://developers.klaviyo.com/en/v2023-06-15/reference/create_template)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Templates.create_template(body)
 ```
 
 
 
 
-#### [Create Template Clone](https://developers.klaviyo.com/en/v2023-02-22/reference/create_template_clone)
+#### [Create Template Clone](https://developers.klaviyo.com/en/v2023-06-15/reference/create_template_clone)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Templates.create_template_clone(body)
 ```
 
 
 
 
-#### [Create Template Render](https://developers.klaviyo.com/en/v2023-02-22/reference/create_template_render)
+#### [Create Template Render](https://developers.klaviyo.com/en/v2023-06-15/reference/create_template_render)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Templates.create_template_render(body)
 ```
 
 
 
 
-#### [Delete Template](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_template)
+#### [Delete Template](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_template)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Templates.delete_template(id)
 ```
 
 
 
 
-#### [Get Template](https://developers.klaviyo.com/en/v2023-02-22/reference/get_template)
+#### [Get Template](https://developers.klaviyo.com/en/v2023-06-15/reference/get_template)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2728,15 +2715,15 @@
 
 klaviyo.Templates.get_template(id, fields_template=fields_template)
 ```
 
 
 
 
-#### [Get Templates](https://developers.klaviyo.com/en/v2023-02-22/reference/get_templates)
+#### [Get Templates](https://developers.klaviyo.com/en/v2023-06-15/reference/get_templates)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_template | [str]
 # filter | str
@@ -2745,15 +2732,15 @@
 
 klaviyo.Templates.get_templates(fields_template=fields_template, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Update Template](https://developers.klaviyo.com/en/v2023-02-22/reference/update_template)
+#### [Update Template](https://developers.klaviyo.com/en/v2023-06-15/reference/update_template)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
```

### Comparing `klaviyo-api-2.0.2/setup.cfg` & `klaviyo-api-3.0.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = klaviyo-api
-version = 2.0.2
+version = 3.0.0
 author = Klaviyo Developers
 author_email = developers@klaviyo.com
 description = Klaviyo Python SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/klaviyo/klaviyo-api-python
 project_urls =
```

### Comparing `klaviyo-api-2.0.2/src/klaviyo_api/wrapper.py` & `klaviyo-api-3.0.0/src/klaviyo_api/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import tenacity
 from urllib.parse import quote, unquote
 
 import openapi_client
 import klaviyo_api.custom_retry as custom_retry
 from dataclasses import dataclass
 from typing import Callable, ClassVar
+from openapi_client.api import accounts_api
 from openapi_client.api import campaigns_api
 from openapi_client.api import catalogs_api
-from openapi_client.api import client_api
 from openapi_client.api import data_privacy_api
 from openapi_client.api import events_api
 from openapi_client.api import flows_api
 from openapi_client.api import lists_api
 from openapi_client.api import metrics_api
 from openapi_client.api import profiles_api
 from openapi_client.api import segments_api
@@ -26,15 +26,15 @@
 class KlaviyoAPI:
 
     api_key: str
     max_delay: int = 60
     max_retries: int = 3
     test_host: str = ''
 
-    _REVISION = "2023-02-22"
+    _REVISION = "2023-06-15"
 
     _STATUS_CODE_CONNECTION_RESET_BY_PEER = 104
     _STATUS_CODE_TOO_MANY_REQUESTS = 429
     _STATUS_CODE_SERVICE_UNAVAILABLE = 503
     _STATUS_CODE_GATEWAY_TIMEOUT = 504
     _STATUS_CODE_A_TIMEOUT_OCCURED = 524
 
@@ -71,14 +71,22 @@
             reraise=True,
             retry=custom_retry.retry_if_qualifies(self._RETRY_CODES),
             wait=tenacity.wait.wait_random_exponential(multiplier = 1, max = self.max_wait),
             stop=tenacity.stop.stop_after_attempt(self.max_retries)
         )
 
         
+        ## Adding Accounts to Client
+        self.Accounts=accounts_api.AccountsApi(self.api_client)
+        
+        ## Applying tenacity retry decorator to each endpoint in Accounts
+        self.Accounts.get_account=self._page_cursor_update(self.retry_logic(self.Accounts.get_account))
+        self.Accounts.get_accounts=self._page_cursor_update(self.retry_logic(self.Accounts.get_accounts))
+        
+        
         ## Adding Campaigns to Client
         self.Campaigns=campaigns_api.CampaignsApi(self.api_client)
         
         ## Applying tenacity retry decorator to each endpoint in Campaigns
         self.Campaigns.create_campaign=self._page_cursor_update(self.retry_logic(self.Campaigns.create_campaign))
         self.Campaigns.create_campaign_clone=self._page_cursor_update(self.retry_logic(self.Campaigns.create_campaign_clone))
         self.Campaigns.create_campaign_message_assign_template=self._page_cursor_update(self.retry_logic(self.Campaigns.create_campaign_message_assign_template))
@@ -153,23 +161,14 @@
         self.Catalogs.update_catalog_category=self._page_cursor_update(self.retry_logic(self.Catalogs.update_catalog_category))
         self.Catalogs.update_catalog_category_relationships_items=self._page_cursor_update(self.retry_logic(self.Catalogs.update_catalog_category_relationships_items))
         self.Catalogs.update_catalog_item=self._page_cursor_update(self.retry_logic(self.Catalogs.update_catalog_item))
         self.Catalogs.update_catalog_item_relationships_categories=self._page_cursor_update(self.retry_logic(self.Catalogs.update_catalog_item_relationships_categories))
         self.Catalogs.update_catalog_variant=self._page_cursor_update(self.retry_logic(self.Catalogs.update_catalog_variant))
         
         
-        ## Adding Client to Client
-        self.Client=client_api.ClientApi(self.api_client)
-        
-        ## Applying tenacity retry decorator to each endpoint in Client
-        self.Client.create_client_event=self._page_cursor_update(self.retry_logic(self.Client.create_client_event))
-        self.Client.create_client_profile=self._page_cursor_update(self.retry_logic(self.Client.create_client_profile))
-        self.Client.create_client_subscription=self._page_cursor_update(self.retry_logic(self.Client.create_client_subscription))
-        
-        
         ## Adding Data_Privacy to Client
         self.Data_Privacy=data_privacy_api.DataPrivacyApi(self.api_client)
         
         ## Applying tenacity retry decorator to each endpoint in Data_Privacy
         self.Data_Privacy.request_profile_deletion=self._page_cursor_update(self.retry_logic(self.Data_Privacy.request_profile_deletion))
```

### Comparing `klaviyo-api-2.0.2/src/klaviyo_api.egg-info/PKG-INFO` & `klaviyo-api-3.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: klaviyo-api
-Version: 2.0.2
+Version: 3.0.0
 Summary: Klaviyo Python SDK
 Home-page: https://github.com/klaviyo/klaviyo-api-python
 Author: Klaviyo Developers
 Author-email: developers@klaviyo.com
+License: UNKNOWN
 Project-URL: API Docs, https://developers.klaviyo.com/en/reference/api_overview
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Klaviyo Python SDK
 
-- SDK version: 2.0.2
-- API revision: 2023-02-22
+- SDK version: 3.0.0
+- API revision: 2023-06-15
 
 ## Helpful Resources
 
-- [API Reference](https://developers.klaviyo.com/en/v2023-02-22/reference)
-- [API Guides](https://developers.klaviyo.com/en/v2023-02-22/docs)
+- [API Reference](https://developers.klaviyo.com/en/v2023-06-15/reference)
+- [API Guides](https://developers.klaviyo.com/en/v2023-06-15/docs)
 - [Postman Workspace](https://www.postman.com/klaviyo/workspace/klaviyo-developers)
 - [Interactive Guide (Jupyter Notebook)](https://github.com/klaviyo-labs/klaviyo-api-guides)
 
 ## Design & Approach
 
 This SDK is a thin wrapper around our API. See our API Reference for full documentation on behavior.
 
@@ -33,23 +35,23 @@
 
 ## Organization
 
 This SDK is organized into the following resources:
 
 
 
-- Campaigns
+- Accounts
 
 
 
-- Catalogs
+- Campaigns
 
 
 
-- Client
+- Catalogs
 
 
 
 - Data_Privacy
 
 
 
@@ -132,16 +134,14 @@
 klaviyo.Events.get_events(
     fields_event=['event_properties'], 
     filter="equals(metric_id,\"aBc123\")", 
     sort='-datetime'
     )
 ```
 
-NOTE: the filter param values need to be url-encoded
-
 #### How to filter based on datetime
 
 **Use Case**: Get profiles that have been updated between two datetimes.
 
 ```python
 klaviyo.Profiles.get_profiles(
     filter='less-than(updated,2023-04-26T00:00:00Z),greater-than(updated,2023-04-19T00:00:00Z)'
@@ -215,107 +215,142 @@
             keys = YOUR_EXCEPTION.headers.keys()
             values = YOUR_EXCEPTION.headers.values()
             ```
 
 ## Important Notes
 
 - The main difference between this SDK and the language-agnostic API Docs that the below endpoints link to is that this SDK automatically adds the `revision` header corresponding to the SDK version.
-- Organization: Resource groups and operation_ids are listed below in alphabetical order, first by Resource name, then by **OpenAPI Summary**. Operation summaries are those listed in the right side bar of the [API Reference](https://developers.klaviyo.com/en/v2023-02-22/reference/get_events).
+- Organization: Resource groups and operation_ids are listed below in alphabetical order, first by Resource name, then by **OpenAPI Summary**. Operation summaries are those listed in the right side bar of the [API Reference](https://developers.klaviyo.com/en/v2023-06-15/reference/get_events).
 - For example values / data types, as well as whether parameters are required/optional, please reference the corresponding API Reference link.
 - Some keyword args may potentially be required for the API call to succeed, the linked API docs are the source of truth regarding which keyword params are required.
 - JSON payloads should be passed in as native python dictionaries.
 - You can override the client private key by passing in an optional `api_key` keyword arg to any API call that takes a private key. As a reminder: do NOT do this client-side/onsite.
 
 # Comprehensive list of Operations & Parameters
 
 
 
 
 
+## Accounts
+
+#### [Get Account](https://developers.klaviyo.com/en/v2023-06-15/reference/get_account)
+
+```python
+## Positional Arguments
+
+# id | str
+
+## Keyword Arguments
+
+# fields_account | [str]
+
+klaviyo.Accounts.get_account(id, fields_account=fields_account)
+```
+
+
+
+
+#### [Get Accounts](https://developers.klaviyo.com/en/v2023-06-15/reference/get_accounts)
+
+```python
+
+## Keyword Arguments
+
+# fields_account | [str]
+
+klaviyo.Accounts.get_accounts(fields_account=fields_account)
+```
+
+
+
+
+
+
 ## Campaigns
 
-#### [Create Campaign](https://developers.klaviyo.com/en/v2023-02-22/reference/create_campaign)
+#### [Create Campaign](https://developers.klaviyo.com/en/v2023-06-15/reference/create_campaign)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Campaigns.create_campaign(body)
 ```
 
 
 
 
-#### [Create Campaign Clone](https://developers.klaviyo.com/en/v2023-02-22/reference/create_campaign_clone)
+#### [Create Campaign Clone](https://developers.klaviyo.com/en/v2023-06-15/reference/create_campaign_clone)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Campaigns.create_campaign_clone(body)
 ```
 
 
 
 
-#### [Assign Campaign Message Template](https://developers.klaviyo.com/en/v2023-02-22/reference/create_campaign_message_assign_template)
+#### [Assign Campaign Message Template](https://developers.klaviyo.com/en/v2023-06-15/reference/create_campaign_message_assign_template)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Campaigns.create_campaign_message_assign_template(body)
 ```
 
 
 
 
-#### [Create Campaign Recipient Estimation Job](https://developers.klaviyo.com/en/v2023-02-22/reference/create_campaign_recipient_estimation_job)
+#### [Create Campaign Recipient Estimation Job](https://developers.klaviyo.com/en/v2023-06-15/reference/create_campaign_recipient_estimation_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Campaigns.create_campaign_recipient_estimation_job(body)
 ```
 
 
 
 
-#### [Create Campaign Send Job](https://developers.klaviyo.com/en/v2023-02-22/reference/create_campaign_send_job)
+#### [Create Campaign Send Job](https://developers.klaviyo.com/en/v2023-06-15/reference/create_campaign_send_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Campaigns.create_campaign_send_job(body)
 ```
 
 
 
 
-#### [Delete Campaign](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_campaign)
+#### [Delete Campaign](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_campaign)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Campaigns.delete_campaign(id)
 ```
 
 
 
 
-#### [Get Campaign](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaign)
+#### [Get Campaign](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaign)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -326,15 +361,15 @@
 
 klaviyo.Campaigns.get_campaign(id, fields_campaign=fields_campaign, fields_tag=fields_tag, include=include)
 ```
 
 
 
 
-#### [Get Campaign Message](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaign_message)
+#### [Get Campaign Message](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaign_message)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -343,15 +378,15 @@
 
 klaviyo.Campaigns.get_campaign_message(id, fields_campaign_message=fields_campaign_message)
 ```
 
 
 
 
-#### [Get Campaign Recipient Estimation](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaign_recipient_estimation)
+#### [Get Campaign Recipient Estimation](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaign_recipient_estimation)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -360,15 +395,15 @@
 
 klaviyo.Campaigns.get_campaign_recipient_estimation(id, fields_campaign_recipient_estimation=fields_campaign_recipient_estimation)
 ```
 
 
 
 
-#### [Get Campaign Recipient Estimation Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaign_recipient_estimation_job)
+#### [Get Campaign Recipient Estimation Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaign_recipient_estimation_job)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -377,28 +412,28 @@
 
 klaviyo.Campaigns.get_campaign_recipient_estimation_job(id, fields_campaign_recipient_estimation_job=fields_campaign_recipient_estimation_job)
 ```
 
 
 
 
-#### [Get Campaign Relationships Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaign_relationships_tags)
+#### [Get Campaign Relationships Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaign_relationships_tags)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Campaigns.get_campaign_relationships_tags(id)
 ```
 
 
 
 
-#### [Get Campaign Send Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaign_send_job)
+#### [Get Campaign Send Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaign_send_job)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -407,32 +442,32 @@
 
 klaviyo.Campaigns.get_campaign_send_job(id, fields_campaign_send_job=fields_campaign_send_job)
 ```
 
 
 
 
-#### [Get Campaign Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaign_tags)
+#### [Get Campaign Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaign_tags)
 
 ```python
 ## Positional Arguments
 
-# campaign_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_tag | [str]
 
-klaviyo.Campaigns.get_campaign_tags(campaign_id, fields_tag=fields_tag)
+klaviyo.Campaigns.get_campaign_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
-#### [Get Campaigns](https://developers.klaviyo.com/en/v2023-02-22/reference/get_campaigns)
+#### [Get Campaigns](https://developers.klaviyo.com/en/v2023-06-15/reference/get_campaigns)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_campaign | [str]
 # fields_tag | [str]
@@ -443,43 +478,43 @@
 
 klaviyo.Campaigns.get_campaigns(fields_campaign=fields_campaign, fields_tag=fields_tag, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Update Campaign](https://developers.klaviyo.com/en/v2023-02-22/reference/update_campaign)
+#### [Update Campaign](https://developers.klaviyo.com/en/v2023-06-15/reference/update_campaign)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Campaigns.update_campaign(id, body)
 ```
 
 
 
 
-#### [Update Campaign Message](https://developers.klaviyo.com/en/v2023-02-22/reference/update_campaign_message)
+#### [Update Campaign Message](https://developers.klaviyo.com/en/v2023-06-15/reference/update_campaign_message)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Campaigns.update_campaign_message(id, body)
 ```
 
 
 
 
-#### [Update Campaign Send Job](https://developers.klaviyo.com/en/v2023-02-22/reference/update_campaign_send_job)
+#### [Update Campaign Send Job](https://developers.klaviyo.com/en/v2023-06-15/reference/update_campaign_send_job)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -489,149 +524,149 @@
 
 
 
 
 
 ## Catalogs
 
-#### [Create Catalog Category](https://developers.klaviyo.com/en/v2023-02-22/reference/create_catalog_category)
+#### [Create Catalog Category](https://developers.klaviyo.com/en/v2023-06-15/reference/create_catalog_category)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.create_catalog_category(body)
 ```
 
 
 
 
-#### [Create Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-02-22/reference/create_catalog_category_relationships_items)
+#### [Create Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-06-15/reference/create_catalog_category_relationships_items)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.create_catalog_category_relationships_items(id, body)
 ```
 
 
 
 
-#### [Create Catalog Item](https://developers.klaviyo.com/en/v2023-02-22/reference/create_catalog_item)
+#### [Create Catalog Item](https://developers.klaviyo.com/en/v2023-06-15/reference/create_catalog_item)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.create_catalog_item(body)
 ```
 
 
 
 
-#### [Create Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-02-22/reference/create_catalog_item_relationships_categories)
+#### [Create Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-06-15/reference/create_catalog_item_relationships_categories)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.create_catalog_item_relationships_categories(id, body)
 ```
 
 
 
 
-#### [Create Catalog Variant](https://developers.klaviyo.com/en/v2023-02-22/reference/create_catalog_variant)
+#### [Create Catalog Variant](https://developers.klaviyo.com/en/v2023-06-15/reference/create_catalog_variant)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.create_catalog_variant(body)
 ```
 
 
 
 
-#### [Delete Catalog Category](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_catalog_category)
+#### [Delete Catalog Category](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_catalog_category)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Catalogs.delete_catalog_category(id)
 ```
 
 
 
 
-#### [Delete Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_catalog_category_relationships_items)
+#### [Delete Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_catalog_category_relationships_items)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.delete_catalog_category_relationships_items(id, body)
 ```
 
 
 
 
-#### [Delete Catalog Item](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_catalog_item)
+#### [Delete Catalog Item](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_catalog_item)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Catalogs.delete_catalog_item(id)
 ```
 
 
 
 
-#### [Delete Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_catalog_item_relationships_categories)
+#### [Delete Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_catalog_item_relationships_categories)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.delete_catalog_item_relationships_categories(id, body)
 ```
 
 
 
 
-#### [Delete Catalog Variant](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_catalog_variant)
+#### [Delete Catalog Variant](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_catalog_variant)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Catalogs.delete_catalog_variant(id)
 ```
 
 
 
 
-#### [Get Catalog Categories](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_categories)
+#### [Get Catalog Categories](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_categories)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_category | [str]
 # filter | str
@@ -640,15 +675,15 @@
 
 klaviyo.Catalogs.get_catalog_categories(fields_catalog_category=fields_catalog_category, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Get Catalog Category](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_category)
+#### [Get Catalog Category](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_category)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -657,37 +692,37 @@
 
 klaviyo.Catalogs.get_catalog_category(id, fields_catalog_category=fields_catalog_category)
 ```
 
 
 
 
-#### [Get Catalog Category Items](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_category_items)
+#### [Get Catalog Category Items](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_category_items)
 
 ```python
 ## Positional Arguments
 
-# category_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_catalog_item | [str]
 # fields_catalog_variant | [str]
 # filter | str
 # include | [str]
 # page_cursor | str
 # sort | str
 
-klaviyo.Catalogs.get_catalog_category_items(category_id, fields_catalog_item=fields_catalog_item, fields_catalog_variant=fields_catalog_variant, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
+klaviyo.Catalogs.get_catalog_category_items(id, fields_catalog_item=fields_catalog_item, fields_catalog_variant=fields_catalog_variant, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Get Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_category_relationships_items)
+#### [Get Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_category_relationships_items)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -696,15 +731,15 @@
 
 klaviyo.Catalogs.get_catalog_category_relationships_items(id, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Catalog Item](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_item)
+#### [Get Catalog Item](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_item)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -715,35 +750,35 @@
 
 klaviyo.Catalogs.get_catalog_item(id, fields_catalog_item=fields_catalog_item, fields_catalog_variant=fields_catalog_variant, include=include)
 ```
 
 
 
 
-#### [Get Catalog Item Categories](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_item_categories)
+#### [Get Catalog Item Categories](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_item_categories)
 
 ```python
 ## Positional Arguments
 
-# item_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_catalog_category | [str]
 # filter | str
 # page_cursor | str
 # sort | str
 
-klaviyo.Catalogs.get_catalog_item_categories(item_id, fields_catalog_category=fields_catalog_category, filter=filter, page_cursor=page_cursor, sort=sort)
+klaviyo.Catalogs.get_catalog_item_categories(id, fields_catalog_category=fields_catalog_category, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Get Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_item_relationships_categories)
+#### [Get Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_item_relationships_categories)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -752,35 +787,35 @@
 
 klaviyo.Catalogs.get_catalog_item_relationships_categories(id, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Catalog Item Variants](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_item_variants)
+#### [Get Catalog Item Variants](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_item_variants)
 
 ```python
 ## Positional Arguments
 
-# item_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_catalog_variant | [str]
 # filter | str
 # page_cursor | str
 # sort | str
 
-klaviyo.Catalogs.get_catalog_item_variants(item_id, fields_catalog_variant=fields_catalog_variant, filter=filter, page_cursor=page_cursor, sort=sort)
+klaviyo.Catalogs.get_catalog_item_variants(id, fields_catalog_variant=fields_catalog_variant, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Get Catalog Items](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_items)
+#### [Get Catalog Items](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_items)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_item | [str]
 # fields_catalog_variant | [str]
@@ -791,15 +826,15 @@
 
 klaviyo.Catalogs.get_catalog_items(fields_catalog_item=fields_catalog_item, fields_catalog_variant=fields_catalog_variant, filter=filter, include=include, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Get Catalog Variant](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_variant)
+#### [Get Catalog Variant](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_variant)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -808,15 +843,15 @@
 
 klaviyo.Catalogs.get_catalog_variant(id, fields_catalog_variant=fields_catalog_variant)
 ```
 
 
 
 
-#### [Get Catalog Variants](https://developers.klaviyo.com/en/v2023-02-22/reference/get_catalog_variants)
+#### [Get Catalog Variants](https://developers.klaviyo.com/en/v2023-06-15/reference/get_catalog_variants)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_variant | [str]
 # filter | str
@@ -825,15 +860,15 @@
 
 klaviyo.Catalogs.get_catalog_variants(fields_catalog_variant=fields_catalog_variant, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Get Create Categories Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_create_categories_job)
+#### [Get Create Categories Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_create_categories_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -844,15 +879,15 @@
 
 klaviyo.Catalogs.get_create_categories_job(job_id, fields_catalog_category_bulk_create_job=fields_catalog_category_bulk_create_job, fields_catalog_category=fields_catalog_category, include=include)
 ```
 
 
 
 
-#### [Get Create Categories Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_create_categories_jobs)
+#### [Get Create Categories Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_create_categories_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_category_bulk_create_job | [str]
 # filter | str
@@ -860,15 +895,15 @@
 
 klaviyo.Catalogs.get_create_categories_jobs(fields_catalog_category_bulk_create_job=fields_catalog_category_bulk_create_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Create Items Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_create_items_job)
+#### [Get Create Items Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_create_items_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -879,15 +914,15 @@
 
 klaviyo.Catalogs.get_create_items_job(job_id, fields_catalog_item_bulk_create_job=fields_catalog_item_bulk_create_job, fields_catalog_item=fields_catalog_item, include=include)
 ```
 
 
 
 
-#### [Get Create Items Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_create_items_jobs)
+#### [Get Create Items Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_create_items_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_item_bulk_create_job | [str]
 # filter | str
@@ -895,15 +930,15 @@
 
 klaviyo.Catalogs.get_create_items_jobs(fields_catalog_item_bulk_create_job=fields_catalog_item_bulk_create_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Create Variants Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_create_variants_job)
+#### [Get Create Variants Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_create_variants_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -914,15 +949,15 @@
 
 klaviyo.Catalogs.get_create_variants_job(job_id, fields_catalog_variant_bulk_create_job=fields_catalog_variant_bulk_create_job, fields_catalog_variant=fields_catalog_variant, include=include)
 ```
 
 
 
 
-#### [Get Create Variants Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_create_variants_jobs)
+#### [Get Create Variants Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_create_variants_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_variant_bulk_create_job | [str]
 # filter | str
@@ -930,15 +965,15 @@
 
 klaviyo.Catalogs.get_create_variants_jobs(fields_catalog_variant_bulk_create_job=fields_catalog_variant_bulk_create_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Delete Categories Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_delete_categories_job)
+#### [Get Delete Categories Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_delete_categories_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -947,15 +982,15 @@
 
 klaviyo.Catalogs.get_delete_categories_job(job_id, fields_catalog_category_bulk_delete_job=fields_catalog_category_bulk_delete_job)
 ```
 
 
 
 
-#### [Get Delete Categories Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_delete_categories_jobs)
+#### [Get Delete Categories Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_delete_categories_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_category_bulk_delete_job | [str]
 # filter | str
@@ -963,15 +998,15 @@
 
 klaviyo.Catalogs.get_delete_categories_jobs(fields_catalog_category_bulk_delete_job=fields_catalog_category_bulk_delete_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Delete Items Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_delete_items_job)
+#### [Get Delete Items Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_delete_items_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -980,15 +1015,15 @@
 
 klaviyo.Catalogs.get_delete_items_job(job_id, fields_catalog_item_bulk_delete_job=fields_catalog_item_bulk_delete_job)
 ```
 
 
 
 
-#### [Get Delete Items Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_delete_items_jobs)
+#### [Get Delete Items Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_delete_items_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_item_bulk_delete_job | [str]
 # filter | str
@@ -996,15 +1031,15 @@
 
 klaviyo.Catalogs.get_delete_items_jobs(fields_catalog_item_bulk_delete_job=fields_catalog_item_bulk_delete_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Delete Variants Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_delete_variants_job)
+#### [Get Delete Variants Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_delete_variants_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -1013,15 +1048,15 @@
 
 klaviyo.Catalogs.get_delete_variants_job(job_id, fields_catalog_variant_bulk_delete_job=fields_catalog_variant_bulk_delete_job)
 ```
 
 
 
 
-#### [Get Delete Variants Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_delete_variants_jobs)
+#### [Get Delete Variants Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_delete_variants_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_variant_bulk_delete_job | [str]
 # filter | str
@@ -1029,15 +1064,15 @@
 
 klaviyo.Catalogs.get_delete_variants_jobs(fields_catalog_variant_bulk_delete_job=fields_catalog_variant_bulk_delete_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Update Categories Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_update_categories_job)
+#### [Get Update Categories Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_update_categories_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -1048,15 +1083,15 @@
 
 klaviyo.Catalogs.get_update_categories_job(job_id, fields_catalog_category_bulk_update_job=fields_catalog_category_bulk_update_job, fields_catalog_category=fields_catalog_category, include=include)
 ```
 
 
 
 
-#### [Get Update Categories Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_update_categories_jobs)
+#### [Get Update Categories Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_update_categories_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_category_bulk_update_job | [str]
 # filter | str
@@ -1064,15 +1099,15 @@
 
 klaviyo.Catalogs.get_update_categories_jobs(fields_catalog_category_bulk_update_job=fields_catalog_category_bulk_update_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Update Items Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_update_items_job)
+#### [Get Update Items Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_update_items_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -1083,15 +1118,15 @@
 
 klaviyo.Catalogs.get_update_items_job(job_id, fields_catalog_item_bulk_update_job=fields_catalog_item_bulk_update_job, fields_catalog_item=fields_catalog_item, include=include)
 ```
 
 
 
 
-#### [Get Update Items Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_update_items_jobs)
+#### [Get Update Items Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_update_items_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_item_bulk_update_job | [str]
 # filter | str
@@ -1099,15 +1134,15 @@
 
 klaviyo.Catalogs.get_update_items_jobs(fields_catalog_item_bulk_update_job=fields_catalog_item_bulk_update_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Update Variants Job](https://developers.klaviyo.com/en/v2023-02-22/reference/get_update_variants_job)
+#### [Get Update Variants Job](https://developers.klaviyo.com/en/v2023-06-15/reference/get_update_variants_job)
 
 ```python
 ## Positional Arguments
 
 # job_id | str
 
 ## Keyword Arguments
@@ -1118,15 +1153,15 @@
 
 klaviyo.Catalogs.get_update_variants_job(job_id, fields_catalog_variant_bulk_update_job=fields_catalog_variant_bulk_update_job, fields_catalog_variant=fields_catalog_variant, include=include)
 ```
 
 
 
 
-#### [Get Update Variants Jobs](https://developers.klaviyo.com/en/v2023-02-22/reference/get_update_variants_jobs)
+#### [Get Update Variants Jobs](https://developers.klaviyo.com/en/v2023-06-15/reference/get_update_variants_jobs)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_catalog_variant_bulk_update_job | [str]
 # filter | str
@@ -1134,188 +1169,188 @@
 
 klaviyo.Catalogs.get_update_variants_jobs(fields_catalog_variant_bulk_update_job=fields_catalog_variant_bulk_update_job, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Spawn Create Categories Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_create_categories_job)
+#### [Spawn Create Categories Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_create_categories_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_create_categories_job(body)
 ```
 
 
 
 
-#### [Spawn Create Items Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_create_items_job)
+#### [Spawn Create Items Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_create_items_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_create_items_job(body)
 ```
 
 
 
 
-#### [Spawn Create Variants Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_create_variants_job)
+#### [Spawn Create Variants Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_create_variants_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_create_variants_job(body)
 ```
 
 
 
 
-#### [Spawn Delete Categories Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_delete_categories_job)
+#### [Spawn Delete Categories Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_delete_categories_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_delete_categories_job(body)
 ```
 
 
 
 
-#### [Spawn Delete Items Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_delete_items_job)
+#### [Spawn Delete Items Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_delete_items_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_delete_items_job(body)
 ```
 
 
 
 
-#### [Spawn Delete Variants Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_delete_variants_job)
+#### [Spawn Delete Variants Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_delete_variants_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_delete_variants_job(body)
 ```
 
 
 
 
-#### [Spawn Update Categories Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_update_categories_job)
+#### [Spawn Update Categories Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_update_categories_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_update_categories_job(body)
 ```
 
 
 
 
-#### [Spawn Update Items Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_update_items_job)
+#### [Spawn Update Items Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_update_items_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_update_items_job(body)
 ```
 
 
 
 
-#### [Spawn Update Variants Job](https://developers.klaviyo.com/en/v2023-02-22/reference/spawn_update_variants_job)
+#### [Spawn Update Variants Job](https://developers.klaviyo.com/en/v2023-06-15/reference/spawn_update_variants_job)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Catalogs.spawn_update_variants_job(body)
 ```
 
 
 
 
-#### [Update Catalog Category](https://developers.klaviyo.com/en/v2023-02-22/reference/update_catalog_category)
+#### [Update Catalog Category](https://developers.klaviyo.com/en/v2023-06-15/reference/update_catalog_category)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.update_catalog_category(id, body)
 ```
 
 
 
 
-#### [Update Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-02-22/reference/update_catalog_category_relationships_items)
+#### [Update Catalog Category Relationships Items](https://developers.klaviyo.com/en/v2023-06-15/reference/update_catalog_category_relationships_items)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.update_catalog_category_relationships_items(id, body)
 ```
 
 
 
 
-#### [Update Catalog Item](https://developers.klaviyo.com/en/v2023-02-22/reference/update_catalog_item)
+#### [Update Catalog Item](https://developers.klaviyo.com/en/v2023-06-15/reference/update_catalog_item)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.update_catalog_item(id, body)
 ```
 
 
 
 
-#### [Update Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-02-22/reference/update_catalog_item_relationships_categories)
+#### [Update Catalog Item Relationships Categories](https://developers.klaviyo.com/en/v2023-06-15/reference/update_catalog_item_relationships_categories)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Catalogs.update_catalog_item_relationships_categories(id, body)
 ```
 
 
 
 
-#### [Update Catalog Variant](https://developers.klaviyo.com/en/v2023-02-22/reference/update_catalog_variant)
+#### [Update Catalog Variant](https://developers.klaviyo.com/en/v2023-06-15/reference/update_catalog_variant)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -1323,63 +1358,17 @@
 ```
 
 
 
 
 
 
-## Client
-
-#### [Create Client Event](https://developers.klaviyo.com/en/v2023-02-22/reference/create_client_event)
-
-```python
-## Positional Arguments
-
-# company_id | str
-# body | dict
-
-klaviyo.Client.create_client_event(company_id, body)
-```
-
-
-
-
-#### [Create or Update Client Profile](https://developers.klaviyo.com/en/v2023-02-22/reference/create_client_profile)
-
-```python
-## Positional Arguments
-
-# company_id | str
-# body | dict
-
-klaviyo.Client.create_client_profile(company_id, body)
-```
-
-
-
-
-#### [Create Client Subscription](https://developers.klaviyo.com/en/v2023-02-22/reference/create_client_subscription)
-
-```python
-## Positional Arguments
-
-# company_id | str
-# body | dict
-
-klaviyo.Client.create_client_subscription(company_id, body)
-```
-
-
-
-
-
-
 ## Data_Privacy
 
-#### [Request Profile Deletion](https://developers.klaviyo.com/en/v2023-02-22/reference/request_profile_deletion)
+#### [Request Profile Deletion](https://developers.klaviyo.com/en/v2023-06-15/reference/request_profile_deletion)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Data_Privacy.request_profile_deletion(body)
@@ -1388,28 +1377,28 @@
 
 
 
 
 
 ## Events
 
-#### [Create Event](https://developers.klaviyo.com/en/v2023-02-22/reference/create_event)
+#### [Create Event](https://developers.klaviyo.com/en/v2023-06-15/reference/create_event)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Events.create_event(body)
 ```
 
 
 
 
-#### [Get Event](https://developers.klaviyo.com/en/v2023-02-22/reference/get_event)
+#### [Get Event](https://developers.klaviyo.com/en/v2023-06-15/reference/get_event)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1421,15 +1410,15 @@
 
 klaviyo.Events.get_event(id, fields_event=fields_event, fields_metric=fields_metric, fields_profile=fields_profile, include=include)
 ```
 
 
 
 
-#### [Get Event Metrics](https://developers.klaviyo.com/en/v2023-02-22/reference/get_event_metrics)
+#### [Get Event Metrics](https://developers.klaviyo.com/en/v2023-06-15/reference/get_event_metrics)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1438,15 +1427,15 @@
 
 klaviyo.Events.get_event_metrics(id, fields_metric=fields_metric)
 ```
 
 
 
 
-#### [Get Event Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/get_event_profiles)
+#### [Get Event Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/get_event_profiles)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1456,41 +1445,41 @@
 
 klaviyo.Events.get_event_profiles(id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile)
 ```
 
 
 
 
-#### [Get Event Relationships Metrics](https://developers.klaviyo.com/en/v2023-02-22/reference/get_event_relationships_metrics)
+#### [Get Event Relationships Metrics](https://developers.klaviyo.com/en/v2023-06-15/reference/get_event_relationships_metrics)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Events.get_event_relationships_metrics(id)
 ```
 
 
 
 
-#### [Get Event Relationships Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/get_event_relationships_profiles)
+#### [Get Event Relationships Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/get_event_relationships_profiles)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Events.get_event_relationships_profiles(id)
 ```
 
 
 
 
-#### [Get Events](https://developers.klaviyo.com/en/v2023-02-22/reference/get_events)
+#### [Get Events](https://developers.klaviyo.com/en/v2023-06-15/reference/get_events)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_event | [str]
 # fields_metric | [str]
@@ -1506,15 +1495,15 @@
 
 
 
 
 
 ## Flows
 
-#### [Get Flow](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow)
+#### [Get Flow](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1525,15 +1514,15 @@
 
 klaviyo.Flows.get_flow(id, fields_flow_action=fields_flow_action, fields_flow=fields_flow, include=include)
 ```
 
 
 
 
-#### [Get Flow Action](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_action)
+#### [Get Flow Action](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_action)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1545,66 +1534,66 @@
 
 klaviyo.Flows.get_flow_action(id, fields_flow_action=fields_flow_action, fields_flow_message=fields_flow_message, fields_flow=fields_flow, include=include)
 ```
 
 
 
 
-#### [Get Flow For Flow Action](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_action_flow)
+#### [Get Flow For Flow Action](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_action_flow)
 
 ```python
 ## Positional Arguments
 
-# action_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_flow | [str]
 
-klaviyo.Flows.get_flow_action_flow(action_id, fields_flow=fields_flow)
+klaviyo.Flows.get_flow_action_flow(id, fields_flow=fields_flow)
 ```
 
 
 
 
-#### [Get Messages For Flow Action](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_action_messages)
+#### [Get Messages For Flow Action](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_action_messages)
 
 ```python
 ## Positional Arguments
 
-# action_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_flow_message | [str]
 # filter | str
 # page_cursor | str
 # page_size | int
 # sort | str
 
-klaviyo.Flows.get_flow_action_messages(action_id, fields_flow_message=fields_flow_message, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
+klaviyo.Flows.get_flow_action_messages(id, fields_flow_message=fields_flow_message, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
-#### [Get Flow Action Relationships Flow](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_action_relationships_flow)
+#### [Get Flow Action Relationships Flow](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_action_relationships_flow)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Flows.get_flow_action_relationships_flow(id)
 ```
 
 
 
 
-#### [Get Flow Action Relationships Messages](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_action_relationships_messages)
+#### [Get Flow Action Relationships Messages](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_action_relationships_messages)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1616,36 +1605,36 @@
 
 klaviyo.Flows.get_flow_action_relationships_messages(id, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
-#### [Get Flow Actions For Flow](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_flow_actions)
+#### [Get Flow Actions For Flow](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_flow_actions)
 
 ```python
 ## Positional Arguments
 
-# flow_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_flow_action | [str]
 # filter | str
 # page_cursor | str
 # page_size | int
 # sort | str
 
-klaviyo.Flows.get_flow_flow_actions(flow_id, fields_flow_action=fields_flow_action, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
+klaviyo.Flows.get_flow_flow_actions(id, fields_flow_action=fields_flow_action, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
-#### [Get Flow Message](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_message)
+#### [Get Flow Message](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_message)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1656,45 +1645,45 @@
 
 klaviyo.Flows.get_flow_message(id, fields_flow_action=fields_flow_action, fields_flow_message=fields_flow_message, include=include)
 ```
 
 
 
 
-#### [Get Flow Action For Message](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_message_action)
+#### [Get Flow Action For Message](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_message_action)
 
 ```python
 ## Positional Arguments
 
-# message_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_flow_action | [str]
 
-klaviyo.Flows.get_flow_message_action(message_id, fields_flow_action=fields_flow_action)
+klaviyo.Flows.get_flow_message_action(id, fields_flow_action=fields_flow_action)
 ```
 
 
 
 
-#### [Get Flow Message Relationships Action](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_message_relationships_action)
+#### [Get Flow Message Relationships Action](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_message_relationships_action)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Flows.get_flow_message_relationships_action(id)
 ```
 
 
 
 
-#### [Get Flow Relationships Flow Actions](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_relationships_flow_actions)
+#### [Get Flow Relationships Flow Actions](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_relationships_flow_actions)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1705,45 +1694,45 @@
 
 klaviyo.Flows.get_flow_relationships_flow_actions(id, filter=filter, page_size=page_size, sort=sort)
 ```
 
 
 
 
-#### [Get Flow Relationships Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_relationships_tags)
+#### [Get Flow Relationships Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_relationships_tags)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Flows.get_flow_relationships_tags(id)
 ```
 
 
 
 
-#### [Get Flow Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flow_tags)
+#### [Get Flow Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flow_tags)
 
 ```python
 ## Positional Arguments
 
-# flow_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_tag | [str]
 
-klaviyo.Flows.get_flow_tags(flow_id, fields_tag=fields_tag)
+klaviyo.Flows.get_flow_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
-#### [Get Flows](https://developers.klaviyo.com/en/v2023-02-22/reference/get_flows)
+#### [Get Flows](https://developers.klaviyo.com/en/v2023-06-15/reference/get_flows)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_flow_action | [str]
 # fields_flow | [str]
@@ -1755,15 +1744,15 @@
 
 klaviyo.Flows.get_flows(fields_flow_action=fields_flow_action, fields_flow=fields_flow, filter=filter, include=include, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
-#### [Update Flow Status](https://developers.klaviyo.com/en/v2023-02-22/reference/update_flow)
+#### [Update Flow Status](https://developers.klaviyo.com/en/v2023-06-15/reference/update_flow)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -1773,69 +1762,69 @@
 
 
 
 
 
 ## Lists
 
-#### [Create List](https://developers.klaviyo.com/en/v2023-02-22/reference/create_list)
+#### [Create List](https://developers.klaviyo.com/en/v2023-06-15/reference/create_list)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Lists.create_list(body)
 ```
 
 
 
 
-#### [Add Profile To List](https://developers.klaviyo.com/en/v2023-02-22/reference/create_list_relationships)
+#### [Add Profile To List](https://developers.klaviyo.com/en/v2023-06-15/reference/create_list_relationships)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Lists.create_list_relationships(id, body)
 ```
 
 
 
 
-#### [Delete List](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_list)
+#### [Delete List](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_list)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Lists.delete_list(id)
 ```
 
 
 
 
-#### [Remove Profile From List](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_list_relationships)
+#### [Remove Profile From List](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_list_relationships)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Lists.delete_list_relationships(id, body)
 ```
 
 
 
 
-#### [Get List](https://developers.klaviyo.com/en/v2023-02-22/reference/get_list)
+#### [Get List](https://developers.klaviyo.com/en/v2023-06-15/reference/get_list)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1844,36 +1833,36 @@
 
 klaviyo.Lists.get_list(id, fields_list=fields_list)
 ```
 
 
 
 
-#### [Get List Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/get_list_profiles)
+#### [Get List Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/get_list_profiles)
 
 ```python
 ## Positional Arguments
 
-# list_id | str
+# id | str
 
 ## Keyword Arguments
 
 # additional_fields_profile | [str]
 # fields_profile | [str]
 # filter | str
 # page_cursor | str
 # page_size | int
 
-klaviyo.Lists.get_list_profiles(list_id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size)
+klaviyo.Lists.get_list_profiles(id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size)
 ```
 
 
 
 
-#### [Get List Relationships Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/get_list_relationships_profiles)
+#### [Get List Relationships Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/get_list_relationships_profiles)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1882,45 +1871,45 @@
 
 klaviyo.Lists.get_list_relationships_profiles(id, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get List Relationships Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_list_relationships_tags)
+#### [Get List Relationships Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_list_relationships_tags)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Lists.get_list_relationships_tags(id)
 ```
 
 
 
 
-#### [Get List Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_list_tags)
+#### [Get List Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_list_tags)
 
 ```python
 ## Positional Arguments
 
-# list_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_tag | [str]
 
-klaviyo.Lists.get_list_tags(list_id, fields_tag=fields_tag)
+klaviyo.Lists.get_list_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
-#### [Get Lists](https://developers.klaviyo.com/en/v2023-02-22/reference/get_lists)
+#### [Get Lists](https://developers.klaviyo.com/en/v2023-06-15/reference/get_lists)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_list | [str]
 # filter | str
@@ -1928,15 +1917,15 @@
 
 klaviyo.Lists.get_lists(fields_list=fields_list, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Update List](https://developers.klaviyo.com/en/v2023-02-22/reference/update_list)
+#### [Update List](https://developers.klaviyo.com/en/v2023-06-15/reference/update_list)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -1946,15 +1935,15 @@
 
 
 
 
 
 ## Metrics
 
-#### [Get Metric](https://developers.klaviyo.com/en/v2023-02-22/reference/get_metric)
+#### [Get Metric](https://developers.klaviyo.com/en/v2023-06-15/reference/get_metric)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -1963,15 +1952,15 @@
 
 klaviyo.Metrics.get_metric(id, fields_metric=fields_metric)
 ```
 
 
 
 
-#### [Get Metrics](https://developers.klaviyo.com/en/v2023-02-22/reference/get_metrics)
+#### [Get Metrics](https://developers.klaviyo.com/en/v2023-06-15/reference/get_metrics)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_metric | [str]
 # filter | str
@@ -1979,15 +1968,15 @@
 
 klaviyo.Metrics.get_metrics(fields_metric=fields_metric, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Query Metric Aggregates](https://developers.klaviyo.com/en/v2023-02-22/reference/query_metric_aggregates)
+#### [Query Metric Aggregates](https://developers.klaviyo.com/en/v2023-06-15/reference/query_metric_aggregates)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Metrics.query_metric_aggregates(body)
@@ -1996,28 +1985,28 @@
 
 
 
 
 
 ## Profiles
 
-#### [Create Profile](https://developers.klaviyo.com/en/v2023-02-22/reference/create_profile)
+#### [Create Profile](https://developers.klaviyo.com/en/v2023-06-15/reference/create_profile)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Profiles.create_profile(body)
 ```
 
 
 
 
-#### [Get Profile](https://developers.klaviyo.com/en/v2023-02-22/reference/get_profile)
+#### [Get Profile](https://developers.klaviyo.com/en/v2023-06-15/reference/get_profile)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2030,75 +2019,75 @@
 
 klaviyo.Profiles.get_profile(id, additional_fields_profile=additional_fields_profile, fields_list=fields_list, fields_profile=fields_profile, fields_segment=fields_segment, include=include)
 ```
 
 
 
 
-#### [Get Profile Lists](https://developers.klaviyo.com/en/v2023-02-22/reference/get_profile_lists)
+#### [Get Profile Lists](https://developers.klaviyo.com/en/v2023-06-15/reference/get_profile_lists)
 
 ```python
 ## Positional Arguments
 
-# profile_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_list | [str]
 
-klaviyo.Profiles.get_profile_lists(profile_id, fields_list=fields_list)
+klaviyo.Profiles.get_profile_lists(id, fields_list=fields_list)
 ```
 
 
 
 
-#### [Get Profile Relationships Lists](https://developers.klaviyo.com/en/v2023-02-22/reference/get_profile_relationships_lists)
+#### [Get Profile Relationships Lists](https://developers.klaviyo.com/en/v2023-06-15/reference/get_profile_relationships_lists)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Profiles.get_profile_relationships_lists(id)
 ```
 
 
 
 
-#### [Get Profile Relationships Segments](https://developers.klaviyo.com/en/v2023-02-22/reference/get_profile_relationships_segments)
+#### [Get Profile Relationships Segments](https://developers.klaviyo.com/en/v2023-06-15/reference/get_profile_relationships_segments)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Profiles.get_profile_relationships_segments(id)
 ```
 
 
 
 
-#### [Get Profile Segments](https://developers.klaviyo.com/en/v2023-02-22/reference/get_profile_segments)
+#### [Get Profile Segments](https://developers.klaviyo.com/en/v2023-06-15/reference/get_profile_segments)
 
 ```python
 ## Positional Arguments
 
-# profile_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_segment | [str]
 
-klaviyo.Profiles.get_profile_segments(profile_id, fields_segment=fields_segment)
+klaviyo.Profiles.get_profile_segments(id, fields_segment=fields_segment)
 ```
 
 
 
 
-#### [Get Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/get_profiles)
+#### [Get Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/get_profiles)
 
 ```python
 
 ## Keyword Arguments
 
 # additional_fields_profile | [str]
 # fields_profile | [str]
@@ -2109,67 +2098,67 @@
 
 klaviyo.Profiles.get_profiles(additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size, sort=sort)
 ```
 
 
 
 
-#### [Subscribe Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/subscribe_profiles)
+#### [Subscribe Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/subscribe_profiles)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Profiles.subscribe_profiles(body)
 ```
 
 
 
 
-#### [Suppress Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/suppress_profiles)
+#### [Suppress Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/suppress_profiles)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Profiles.suppress_profiles(body)
 ```
 
 
 
 
-#### [Unsubscribe Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/unsubscribe_profiles)
+#### [Unsubscribe Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/unsubscribe_profiles)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Profiles.unsubscribe_profiles(body)
 ```
 
 
 
 
-#### [Unsuppress Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/unsuppress_profiles)
+#### [Unsuppress Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/unsuppress_profiles)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Profiles.unsuppress_profiles(body)
 ```
 
 
 
 
-#### [Update Profile](https://developers.klaviyo.com/en/v2023-02-22/reference/update_profile)
+#### [Update Profile](https://developers.klaviyo.com/en/v2023-06-15/reference/update_profile)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -2179,15 +2168,15 @@
 
 
 
 
 
 ## Segments
 
-#### [Get Segment](https://developers.klaviyo.com/en/v2023-02-22/reference/get_segment)
+#### [Get Segment](https://developers.klaviyo.com/en/v2023-06-15/reference/get_segment)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2196,36 +2185,36 @@
 
 klaviyo.Segments.get_segment(id, fields_segment=fields_segment)
 ```
 
 
 
 
-#### [Get Segment Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/get_segment_profiles)
+#### [Get Segment Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/get_segment_profiles)
 
 ```python
 ## Positional Arguments
 
-# segment_id | str
+# id | str
 
 ## Keyword Arguments
 
 # additional_fields_profile | [str]
 # fields_profile | [str]
 # filter | str
 # page_cursor | str
 # page_size | int
 
-klaviyo.Segments.get_segment_profiles(segment_id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size)
+klaviyo.Segments.get_segment_profiles(id, additional_fields_profile=additional_fields_profile, fields_profile=fields_profile, filter=filter, page_cursor=page_cursor, page_size=page_size)
 ```
 
 
 
 
-#### [Get Segment Relationships Profiles](https://developers.klaviyo.com/en/v2023-02-22/reference/get_segment_relationships_profiles)
+#### [Get Segment Relationships Profiles](https://developers.klaviyo.com/en/v2023-06-15/reference/get_segment_relationships_profiles)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2234,45 +2223,45 @@
 
 klaviyo.Segments.get_segment_relationships_profiles(id, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Get Segment Relationships Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_segment_relationships_tags)
+#### [Get Segment Relationships Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_segment_relationships_tags)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Segments.get_segment_relationships_tags(id)
 ```
 
 
 
 
-#### [Get Segment Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_segment_tags)
+#### [Get Segment Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_segment_tags)
 
 ```python
 ## Positional Arguments
 
-# segment_id | str
+# id | str
 
 ## Keyword Arguments
 
 # fields_tag | [str]
 
-klaviyo.Segments.get_segment_tags(segment_id, fields_tag=fields_tag)
+klaviyo.Segments.get_segment_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
-#### [Get Segments](https://developers.klaviyo.com/en/v2023-02-22/reference/get_segments)
+#### [Get Segments](https://developers.klaviyo.com/en/v2023-06-15/reference/get_segments)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_segment | [str]
 # filter | str
@@ -2280,15 +2269,15 @@
 
 klaviyo.Segments.get_segments(fields_segment=fields_segment, filter=filter, page_cursor=page_cursor)
 ```
 
 
 
 
-#### [Update Segment](https://developers.klaviyo.com/en/v2023-02-22/reference/update_segment)
+#### [Update Segment](https://developers.klaviyo.com/en/v2023-06-15/reference/update_segment)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -2298,179 +2287,179 @@
 
 
 
 
 
 ## Tags
 
-#### [Create Tag](https://developers.klaviyo.com/en/v2023-02-22/reference/create_tag)
+#### [Create Tag](https://developers.klaviyo.com/en/v2023-06-15/reference/create_tag)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Tags.create_tag(body)
 ```
 
 
 
 
-#### [Create Tag Group](https://developers.klaviyo.com/en/v2023-02-22/reference/create_tag_group)
+#### [Create Tag Group](https://developers.klaviyo.com/en/v2023-06-15/reference/create_tag_group)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Tags.create_tag_group(body)
 ```
 
 
 
 
-#### [Create Tag Relationships Campaigns](https://developers.klaviyo.com/en/v2023-02-22/reference/create_tag_relationships_campaigns)
+#### [Create Tag Relationships Campaigns](https://developers.klaviyo.com/en/v2023-06-15/reference/create_tag_relationships_campaigns)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.create_tag_relationships_campaigns(id, body)
 ```
 
 
 
 
-#### [Create Tag Relationships Flows](https://developers.klaviyo.com/en/v2023-02-22/reference/create_tag_relationships_flows)
+#### [Create Tag Relationships Flows](https://developers.klaviyo.com/en/v2023-06-15/reference/create_tag_relationships_flows)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.create_tag_relationships_flows(id, body)
 ```
 
 
 
 
-#### [Create Tag Relationships Lists](https://developers.klaviyo.com/en/v2023-02-22/reference/create_tag_relationships_lists)
+#### [Create Tag Relationships Lists](https://developers.klaviyo.com/en/v2023-06-15/reference/create_tag_relationships_lists)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.create_tag_relationships_lists(id, body)
 ```
 
 
 
 
-#### [Create Tag Relationships Segments](https://developers.klaviyo.com/en/v2023-02-22/reference/create_tag_relationships_segments)
+#### [Create Tag Relationships Segments](https://developers.klaviyo.com/en/v2023-06-15/reference/create_tag_relationships_segments)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.create_tag_relationships_segments(id, body)
 ```
 
 
 
 
-#### [Delete Tag](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_tag)
+#### [Delete Tag](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_tag)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.delete_tag(id)
 ```
 
 
 
 
-#### [Delete Tag Group](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_tag_group)
+#### [Delete Tag Group](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_tag_group)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.delete_tag_group(id)
 ```
 
 
 
 
-#### [Delete Tag Relationships Campaigns](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_tag_relationships_campaigns)
+#### [Delete Tag Relationships Campaigns](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_tag_relationships_campaigns)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.delete_tag_relationships_campaigns(id, body)
 ```
 
 
 
 
-#### [Delete Tag Relationships Flows](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_tag_relationships_flows)
+#### [Delete Tag Relationships Flows](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_tag_relationships_flows)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.delete_tag_relationships_flows(id, body)
 ```
 
 
 
 
-#### [Delete Tag Relationships Lists](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_tag_relationships_lists)
+#### [Delete Tag Relationships Lists](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_tag_relationships_lists)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.delete_tag_relationships_lists(id, body)
 ```
 
 
 
 
-#### [Delete Tag Relationships Segments](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_tag_relationships_segments)
+#### [Delete Tag Relationships Segments](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_tag_relationships_segments)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.delete_tag_relationships_segments(id, body)
 ```
 
 
 
 
-#### [Get Tag](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag)
+#### [Get Tag](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2479,15 +2468,15 @@
 
 klaviyo.Tags.get_tag(id, fields_tag=fields_tag)
 ```
 
 
 
 
-#### [Get Tag Group](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_group)
+#### [Get Tag Group](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_group)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2496,28 +2485,28 @@
 
 klaviyo.Tags.get_tag_group(id, fields_tag_group=fields_tag_group)
 ```
 
 
 
 
-#### [Get Tag Group Relationships Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_group_relationships_tags)
+#### [Get Tag Group Relationships Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_group_relationships_tags)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.get_tag_group_relationships_tags(id)
 ```
 
 
 
 
-#### [Get Tag Group Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_group_tags)
+#### [Get Tag Group Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_group_tags)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2526,15 +2515,15 @@
 
 klaviyo.Tags.get_tag_group_tags(id, fields_tag=fields_tag)
 ```
 
 
 
 
-#### [Get Tag Groups](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_groups)
+#### [Get Tag Groups](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_groups)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_tag_group | [str]
 # filter | str
@@ -2543,80 +2532,80 @@
 
 klaviyo.Tags.get_tag_groups(fields_tag_group=fields_tag_group, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Get Tag Relationships Campaigns](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_relationships_campaigns)
+#### [Get Tag Relationships Campaigns](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_relationships_campaigns)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.get_tag_relationships_campaigns(id)
 ```
 
 
 
 
-#### [Get Tag Relationships Flows](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_relationships_flows)
+#### [Get Tag Relationships Flows](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_relationships_flows)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.get_tag_relationships_flows(id)
 ```
 
 
 
 
-#### [Get Tag Relationships Lists](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_relationships_lists)
+#### [Get Tag Relationships Lists](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_relationships_lists)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.get_tag_relationships_lists(id)
 ```
 
 
 
 
-#### [Get Tag Relationships Segments](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_relationships_segments)
+#### [Get Tag Relationships Segments](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_relationships_segments)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.get_tag_relationships_segments(id)
 ```
 
 
 
 
-#### [Get Tag Relationships Tag Group](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_relationships_tag_group)
+#### [Get Tag Relationships Tag Group](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_relationships_tag_group)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Tags.get_tag_relationships_tag_group(id)
 ```
 
 
 
 
-#### [Get Tag Tag Group](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tag_tag_group)
+#### [Get Tag Tag Group](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tag_tag_group)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2625,15 +2614,15 @@
 
 klaviyo.Tags.get_tag_tag_group(id, fields_tag_group=fields_tag_group)
 ```
 
 
 
 
-#### [Get Tags](https://developers.klaviyo.com/en/v2023-02-22/reference/get_tags)
+#### [Get Tags](https://developers.klaviyo.com/en/v2023-06-15/reference/get_tags)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_tag | [str]
 # filter | str
@@ -2642,29 +2631,29 @@
 
 klaviyo.Tags.get_tags(fields_tag=fields_tag, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Update Tag](https://developers.klaviyo.com/en/v2023-02-22/reference/update_tag)
+#### [Update Tag](https://developers.klaviyo.com/en/v2023-06-15/reference/update_tag)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
 klaviyo.Tags.update_tag(id, body)
 ```
 
 
 
 
-#### [Update Tag Group](https://developers.klaviyo.com/en/v2023-02-22/reference/update_tag_group)
+#### [Update Tag Group](https://developers.klaviyo.com/en/v2023-06-15/reference/update_tag_group)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -2674,67 +2663,67 @@
 
 
 
 
 
 ## Templates
 
-#### [Create Template](https://developers.klaviyo.com/en/v2023-02-22/reference/create_template)
+#### [Create Template](https://developers.klaviyo.com/en/v2023-06-15/reference/create_template)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Templates.create_template(body)
 ```
 
 
 
 
-#### [Create Template Clone](https://developers.klaviyo.com/en/v2023-02-22/reference/create_template_clone)
+#### [Create Template Clone](https://developers.klaviyo.com/en/v2023-06-15/reference/create_template_clone)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Templates.create_template_clone(body)
 ```
 
 
 
 
-#### [Create Template Render](https://developers.klaviyo.com/en/v2023-02-22/reference/create_template_render)
+#### [Create Template Render](https://developers.klaviyo.com/en/v2023-06-15/reference/create_template_render)
 
 ```python
 ## Positional Arguments
 
 # body | dict
 
 klaviyo.Templates.create_template_render(body)
 ```
 
 
 
 
-#### [Delete Template](https://developers.klaviyo.com/en/v2023-02-22/reference/delete_template)
+#### [Delete Template](https://developers.klaviyo.com/en/v2023-06-15/reference/delete_template)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 klaviyo.Templates.delete_template(id)
 ```
 
 
 
 
-#### [Get Template](https://developers.klaviyo.com/en/v2023-02-22/reference/get_template)
+#### [Get Template](https://developers.klaviyo.com/en/v2023-06-15/reference/get_template)
 
 ```python
 ## Positional Arguments
 
 # id | str
 
 ## Keyword Arguments
@@ -2743,15 +2732,15 @@
 
 klaviyo.Templates.get_template(id, fields_template=fields_template)
 ```
 
 
 
 
-#### [Get Templates](https://developers.klaviyo.com/en/v2023-02-22/reference/get_templates)
+#### [Get Templates](https://developers.klaviyo.com/en/v2023-06-15/reference/get_templates)
 
 ```python
 
 ## Keyword Arguments
 
 # fields_template | [str]
 # filter | str
@@ -2760,15 +2749,15 @@
 
 klaviyo.Templates.get_templates(fields_template=fields_template, filter=filter, page_cursor=page_cursor, sort=sort)
 ```
 
 
 
 
-#### [Update Template](https://developers.klaviyo.com/en/v2023-02-22/reference/update_template)
+#### [Update Template](https://developers.klaviyo.com/en/v2023-06-15/reference/update_template)
 
 ```python
 ## Positional Arguments
 
 # id | str
 # body | dict
 
@@ -2813,7 +2802,8 @@
 
 ## Namespace
 
 In the interest of making the SDK Pythonic, we made the following namespace changes *relative* to the language agnostic resources up top (API Docs, Guides, etc).
 
 - Resource names use Title + Snake Casing, (e.g. `Data_Privacy`)
 - function names and parameter names use snake case (e.g. `get_metrics`, and `profile_id`)
+
```

### Comparing `klaviyo-api-2.0.2/src/klaviyo_api.egg-info/SOURCES.txt` & `klaviyo-api-3.0.0/src/klaviyo_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 src/openapi_client/__init__.py
 src/openapi_client/api_client.py
 src/openapi_client/configuration.py
 src/openapi_client/exceptions.py
 src/openapi_client/model_utils.py
 src/openapi_client/rest.py
 src/openapi_client/api/__init__.py
+src/openapi_client/api/accounts_api.py
 src/openapi_client/api/campaigns_api.py
 src/openapi_client/api/catalogs_api.py
-src/openapi_client/api/client_api.py
 src/openapi_client/api/data_privacy_api.py
 src/openapi_client/api/events_api.py
 src/openapi_client/api/flows_api.py
 src/openapi_client/api/lists_api.py
 src/openapi_client/api/metrics_api.py
 src/openapi_client/api/profiles_api.py
 src/openapi_client/api/segments_api.py
@@ -84,23 +84,23 @@
 src/openapi_client/model/catalog_category_update_query_resource_object_relationships.py
 src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items.py
 src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items_data_inner.py
 src/openapi_client/model/catalog_item_bulk_create_job_enum.py
 src/openapi_client/model/catalog_item_bulk_delete_job_enum.py
 src/openapi_client/model/catalog_item_bulk_update_job_enum.py
 src/openapi_client/model/catalog_item_category_op.py
+src/openapi_client/model/catalog_item_category_op_data_inner.py
 src/openapi_client/model/catalog_item_create_job_create_query.py
 src/openapi_client/model/catalog_item_create_job_create_query_resource_object.py
 src/openapi_client/model/catalog_item_create_job_create_query_resource_object_attributes.py
 src/openapi_client/model/catalog_item_create_query.py
 src/openapi_client/model/catalog_item_create_query_resource_object.py
 src/openapi_client/model/catalog_item_create_query_resource_object_attributes.py
 src/openapi_client/model/catalog_item_create_query_resource_object_relationships.py
 src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories.py
-src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories_data_inner.py
 src/openapi_client/model/catalog_item_delete_job_create_query.py
 src/openapi_client/model/catalog_item_delete_job_create_query_resource_object.py
 src/openapi_client/model/catalog_item_delete_job_create_query_resource_object_attributes.py
 src/openapi_client/model/catalog_item_delete_query_resource_object.py
 src/openapi_client/model/catalog_item_enum.py
 src/openapi_client/model/catalog_item_update_job_create_query.py
 src/openapi_client/model/catalog_item_update_job_create_query_resource_object.py
@@ -154,29 +154,24 @@
 src/openapi_client/model/list_partial_update_query.py
 src/openapi_client/model/list_partial_update_query_resource_object.py
 src/openapi_client/model/metric_aggregate_enum.py
 src/openapi_client/model/metric_aggregate_query.py
 src/openapi_client/model/metric_aggregate_query_resource_object.py
 src/openapi_client/model/metric_aggregate_query_resource_object_attributes.py
 src/openapi_client/model/metric_create_query.py
-src/openapi_client/model/onsite_profile_create_query.py
-src/openapi_client/model/onsite_profile_create_query_resource_object.py
-src/openapi_client/model/onsite_profile_create_query_resource_object_attributes.py
-src/openapi_client/model/onsite_subscription_create_query.py
-src/openapi_client/model/onsite_subscription_create_query_resource_object.py
-src/openapi_client/model/onsite_subscription_create_query_resource_object_attributes.py
 src/openapi_client/model/profile_create_query.py
 src/openapi_client/model/profile_create_query_resource_object.py
 src/openapi_client/model/profile_create_query_resource_object_attributes.py
 src/openapi_client/model/profile_enum.py
 src/openapi_client/model/profile_location.py
 src/openapi_client/model/profile_location_latitude.py
 src/openapi_client/model/profile_location_longitude.py
 src/openapi_client/model/profile_partial_update_query.py
 src/openapi_client/model/profile_partial_update_query_resource_object.py
+src/openapi_client/model/profile_partial_update_query_resource_object_attributes.py
 src/openapi_client/model/profile_subscription_bulk_create_job_enum.py
 src/openapi_client/model/profile_suppression_bulk_create_job_enum.py
 src/openapi_client/model/profile_unsubscription_bulk_create_job_enum.py
 src/openapi_client/model/profile_unsuppression_bulk_create_job_enum.py
 src/openapi_client/model/segment_enum.py
 src/openapi_client/model/segment_partial_update_query.py
 src/openapi_client/model/segment_partial_update_query_resource_object.py
@@ -186,15 +181,14 @@
 src/openapi_client/model/static_schedule_options.py
 src/openapi_client/model/sto_schedule_options.py
 src/openapi_client/model/subscription.py
 src/openapi_client/model/subscription_channels.py
 src/openapi_client/model/subscription_create_job_create_query.py
 src/openapi_client/model/subscription_create_job_create_query_resource_object.py
 src/openapi_client/model/subscription_create_job_create_query_resource_object_attributes.py
-src/openapi_client/model/subscription_enum.py
 src/openapi_client/model/suppression.py
 src/openapi_client/model/suppression_create_job_create_query.py
 src/openapi_client/model/suppression_create_job_create_query_resource_object.py
 src/openapi_client/model/suppression_create_job_create_query_resource_object_attributes.py
 src/openapi_client/model/tag_campaign_op.py
 src/openapi_client/model/tag_campaign_op_data_inner.py
 src/openapi_client/model/tag_create_query.py
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/__init__.py` & `klaviyo-api-3.0.0/src/openapi_client/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # flake8: noqa
 
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "2.0.2"
+__version__ = "3.0.0"
 
 # import ApiClient
 from openapi_client.api_client import ApiClient
 
 # import Configuration
 from openapi_client.configuration import Configuration
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/api/campaigns_api.py` & `klaviyo-api-3.0.0/src/openapi_client/api/campaigns_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -781,26 +781,26 @@
         )
         self.get_campaign_tags_endpoint = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'Klaviyo-API-Key'
                 ],
-                'endpoint_path': '/api/campaigns/{campaign_id}/tags/',
+                'endpoint_path': '/api/campaigns/{id}/tags/',
                 'operation_id': 'get_campaign_tags',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'campaign_id',
+                    'id',
                     'fields_tag',
                 ],
                 'required': [
-                    'campaign_id',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'fields_tag',
                 ],
                 'validation': [
@@ -812,25 +812,25 @@
                 'allowed_values': {
                     ('fields_tag',): {
 
                         "NAME": "name"
                     },
                 },
                 'openapi_types': {
-                    'campaign_id':
+                    'id':
                         (str,),
                     'fields_tag':
                         ([str],),
                 },
                 'attribute_map': {
-                    'campaign_id': 'campaign_id',
+                    'id': 'id',
                     'fields_tag': 'fields[tag]',
                 },
                 'location_map': {
-                    'campaign_id': 'path',
+                    'id': 'path',
                     'fields_tag': 'query',
                 },
                 'collection_format_map': {
                     'fields_tag': 'csv',
                 }
             },
             headers_map={
@@ -1663,17 +1663,17 @@
         >>> thread = api.get_campaign(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): The campaign ID to be retrieved
 
         Keyword Args:
-            fields_campaign ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_tag ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#relationships. [optional]
+            fields_campaign ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_tag ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#relationships. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1749,15 +1749,15 @@
         >>> thread = api.get_campaign_message(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): The message ID to be retrieved
 
         Keyword Args:
-            fields_campaign_message ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_campaign_message ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1833,15 +1833,15 @@
         >>> thread = api.get_campaign_recipient_estimation(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): The ID of the campaign for which to get the estimated number of recipients
 
         Keyword Args:
-            fields_campaign_recipient_estimation ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_campaign_recipient_estimation ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1917,15 +1917,15 @@
         >>> thread = api.get_campaign_recipient_estimation_job(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): The ID of the campaign to get recipient estimation status
 
         Keyword Args:
-            fields_campaign_recipient_estimation_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_campaign_recipient_estimation_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2084,15 +2084,15 @@
         >>> thread = api.get_campaign_send_job(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): The ID of the campaign to send
 
         Keyword Args:
-            fields_campaign_send_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_campaign_send_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2152,31 +2152,31 @@
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.get_campaign_send_job_endpoint.call_with_http_info(**kwargs)
 
     def get_campaign_tags(
         self,
-        campaign_id,
+        id,
         **kwargs
     ):
         """Get Campaign Tags  # noqa: E501
 
         Return all tags that belong to the given campaign.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `campaigns:read` `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_campaign_tags(campaign_id, async_req=True)
+        >>> thread = api.get_campaign_tags(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            campaign_id (str): 
+            id (str): 
 
         Keyword Args:
-            fields_tag ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_tag ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2230,16 +2230,16 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['campaign_id'] = \
-            campaign_id
+        kwargs['id'] = \
+            id
         return self.get_campaign_tags_endpoint.call_with_http_info(**kwargs)
 
     def get_campaigns(
         self,
         **kwargs
     ):
         """Get Campaigns  # noqa: E501
@@ -2249,20 +2249,20 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_campaigns(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            fields_campaign ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_tag ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`name`: `contains`<br>`status`: `any`, `equals`<br>`archived`: `equals`<br>`created_at`: `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`scheduled_at`: `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`updated_at`: `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`. [optional]
-            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#relationships. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
-            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
+            fields_campaign ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_tag ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`name`: `contains`<br>`status`: `any`, `equals`<br>`archived`: `equals`<br>`created_at`: `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`scheduled_at`: `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`updated_at`: `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`. [optional]
+            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#relationships. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
+            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/api/catalogs_api.py` & `klaviyo-api-3.0.0/src/openapi_client/api/catalogs_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -738,31 +738,31 @@
         )
         self.get_catalog_category_items_endpoint = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'Klaviyo-API-Key'
                 ],
-                'endpoint_path': '/api/catalog-categories/{category_id}/items/',
+                'endpoint_path': '/api/catalog-categories/{id}/items/',
                 'operation_id': 'get_catalog_category_items',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'category_id',
+                    'id',
                     'fields_catalog_item',
                     'fields_catalog_variant',
                     'filter',
                     'include',
                     'page_cursor',
                     'sort',
                 ],
                 'required': [
-                    'category_id',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'fields_catalog_item',
                     'fields_catalog_variant',
                     'include',
@@ -815,15 +815,15 @@
                     ('sort',): {
 
                         "CREATED": "created",
                         "-CREATED": "-created"
                     },
                 },
                 'openapi_types': {
-                    'category_id':
+                    'id':
                         (str,),
                     'fields_catalog_item':
                         ([str],),
                     'fields_catalog_variant':
                         ([str],),
                     'filter':
                         (str,),
@@ -831,24 +831,24 @@
                         ([str],),
                     'page_cursor':
                         (str,),
                     'sort':
                         (str,),
                 },
                 'attribute_map': {
-                    'category_id': 'category_id',
+                    'id': 'id',
                     'fields_catalog_item': 'fields[catalog-item]',
                     'fields_catalog_variant': 'fields[catalog-variant]',
                     'filter': 'filter',
                     'include': 'include',
                     'page_cursor': 'page[cursor]',
                     'sort': 'sort',
                 },
                 'location_map': {
-                    'category_id': 'path',
+                    'id': 'path',
                     'fields_catalog_item': 'query',
                     'fields_catalog_variant': 'query',
                     'filter': 'query',
                     'include': 'query',
                     'page_cursor': 'query',
                     'sort': 'query',
                 },
@@ -1033,29 +1033,29 @@
         )
         self.get_catalog_item_categories_endpoint = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'Klaviyo-API-Key'
                 ],
-                'endpoint_path': '/api/catalog-items/{item_id}/categories/',
+                'endpoint_path': '/api/catalog-items/{id}/categories/',
                 'operation_id': 'get_catalog_item_categories',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'item_id',
+                    'id',
                     'fields_catalog_category',
                     'filter',
                     'page_cursor',
                     'sort',
                 ],
                 'required': [
-                    'item_id',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'fields_catalog_category',
                     'sort',
                 ],
@@ -1075,34 +1075,34 @@
                     ('sort',): {
 
                         "CREATED": "created",
                         "-CREATED": "-created"
                     },
                 },
                 'openapi_types': {
-                    'item_id':
+                    'id':
                         (str,),
                     'fields_catalog_category':
                         ([str],),
                     'filter':
                         (str,),
                     'page_cursor':
                         (str,),
                     'sort':
                         (str,),
                 },
                 'attribute_map': {
-                    'item_id': 'item_id',
+                    'id': 'id',
                     'fields_catalog_category': 'fields[catalog-category]',
                     'filter': 'filter',
                     'page_cursor': 'page[cursor]',
                     'sort': 'sort',
                 },
                 'location_map': {
-                    'item_id': 'path',
+                    'id': 'path',
                     'fields_catalog_category': 'query',
                     'filter': 'query',
                     'page_cursor': 'query',
                     'sort': 'query',
                 },
                 'collection_format_map': {
                     'fields_catalog_category': 'csv',
@@ -1174,29 +1174,29 @@
         )
         self.get_catalog_item_variants_endpoint = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'Klaviyo-API-Key'
                 ],
-                'endpoint_path': '/api/catalog-items/{item_id}/variants/',
+                'endpoint_path': '/api/catalog-items/{id}/variants/',
                 'operation_id': 'get_catalog_item_variants',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'item_id',
+                    'id',
                     'fields_catalog_variant',
                     'filter',
                     'page_cursor',
                     'sort',
                 ],
                 'required': [
-                    'item_id',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'fields_catalog_variant',
                     'sort',
                 ],
@@ -1228,34 +1228,34 @@
                     ('sort',): {
 
                         "CREATED": "created",
                         "-CREATED": "-created"
                     },
                 },
                 'openapi_types': {
-                    'item_id':
+                    'id':
                         (str,),
                     'fields_catalog_variant':
                         ([str],),
                     'filter':
                         (str,),
                     'page_cursor':
                         (str,),
                     'sort':
                         (str,),
                 },
                 'attribute_map': {
-                    'item_id': 'item_id',
+                    'id': 'id',
                     'fields_catalog_variant': 'fields[catalog-variant]',
                     'filter': 'filter',
                     'page_cursor': 'page[cursor]',
                     'sort': 'sort',
                 },
                 'location_map': {
-                    'item_id': 'path',
+                    'id': 'path',
                     'fields_catalog_variant': 'query',
                     'filter': 'query',
                     'page_cursor': 'query',
                     'sort': 'query',
                 },
                 'collection_format_map': {
                     'fields_catalog_variant': 'csv',
@@ -4647,18 +4647,18 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_catalog_categories(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            fields_catalog_category ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`ids`: `any`<br>`item`: `equals`<br>`name`: `contains`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
-            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
+            fields_catalog_category ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`ids`: `any`<br>`item`: `equals`<br>`name`: `contains`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
+            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -4732,15 +4732,15 @@
         >>> thread = api.get_catalog_category(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): The catalog category ID is a compound ID (string), with format: `{integration}:::{catalog}:::{external_id}`. Currently, the only supported integration type is `$custom`, and the only supported catalog is `$default`.
 
         Keyword Args:
-            fields_catalog_category ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_catalog_category ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -4800,36 +4800,36 @@
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.get_catalog_category_endpoint.call_with_http_info(**kwargs)
 
     def get_catalog_category_items(
         self,
-        category_id,
+        id,
         **kwargs
     ):
         """Get Catalog Category Items  # noqa: E501
 
         Get all items in a category with the given category ID. Items can be sorted by the following fields, in ascending and descending order: `created` Include parameters can be provided to get the following related resource data: `variants` Returns a maximum of 100 items per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_catalog_category_items(category_id, async_req=True)
+        >>> thread = api.get_catalog_category_items(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            category_id (str): The catalog category ID is a compound ID (string), with format: `{integration}:::{catalog}:::{external_id}`. Currently, the only supported integration type is `$custom`, and the only supported catalog is `$default`.
+            id (str): 
 
         Keyword Args:
-            fields_catalog_item ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_catalog_variant ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`ids`: `any`<br>`category`: `equals`<br>`title`: `contains`<br>`published`: `equals`. [optional]
-            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#relationships. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
-            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
+            fields_catalog_item ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_catalog_variant ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`ids`: `any`<br>`category`: `equals`<br>`title`: `contains`<br>`published`: `equals`. [optional]
+            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#relationships. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
+            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -4883,16 +4883,16 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['category_id'] = \
-            category_id
+        kwargs['id'] = \
+            id
         return self.get_catalog_category_items_endpoint.call_with_http_info(**kwargs)
 
     def get_catalog_category_relationships_items(
         self,
         id,
         **kwargs
     ):
@@ -4905,15 +4905,15 @@
         >>> thread = api.get_catalog_category_relationships_items(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): 
 
         Keyword Args:
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -4989,17 +4989,17 @@
         >>> thread = api.get_catalog_item(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): The catalog item ID is a compound ID (string), with format: `{integration}:::{catalog}:::{external_id}`. Currently, the only supported integration type is `$custom`, and the only supported catalog is `$default`.
 
         Keyword Args:
-            fields_catalog_item ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_catalog_variant ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#relationships. [optional]
+            fields_catalog_item ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_catalog_variant ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#relationships. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -5059,34 +5059,34 @@
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.get_catalog_item_endpoint.call_with_http_info(**kwargs)
 
     def get_catalog_item_categories(
         self,
-        item_id,
+        id,
         **kwargs
     ):
         """Get Catalog Item Categories  # noqa: E501
 
         Get all catalog categories that an item with the given item ID is in. Catalog categories can be sorted by the following fields, in ascending and descending order: `created` Returns a maximum of 100 categories per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_catalog_item_categories(item_id, async_req=True)
+        >>> thread = api.get_catalog_item_categories(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            item_id (str): The catalog item ID is a compound ID (string), with format: `{integration}:::{catalog}:::{external_id}`. Currently, the only supported integration type is `$custom`, and the only supported catalog is `$default`.
+            id (str): 
 
         Keyword Args:
-            fields_catalog_category ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`ids`: `any`<br>`item`: `equals`<br>`name`: `contains`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
-            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
+            fields_catalog_category ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`ids`: `any`<br>`item`: `equals`<br>`name`: `contains`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
+            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -5140,16 +5140,16 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['item_id'] = \
-            item_id
+        kwargs['id'] = \
+            id
         return self.get_catalog_item_categories_endpoint.call_with_http_info(**kwargs)
 
     def get_catalog_item_relationships_categories(
         self,
         id,
         **kwargs
     ):
@@ -5162,15 +5162,15 @@
         >>> thread = api.get_catalog_item_relationships_categories(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): 
 
         Keyword Args:
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -5230,34 +5230,34 @@
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.get_catalog_item_relationships_categories_endpoint.call_with_http_info(**kwargs)
 
     def get_catalog_item_variants(
         self,
-        item_id,
+        id,
         **kwargs
     ):
         """Get Catalog Item Variants  # noqa: E501
 
         Get all variants related to the given item ID. Variants can be sorted by the following fields, in ascending and descending order: `created` Returns a maximum of 100 variants per request.<br><br>*Rate limits*:<br>Burst: `350/s`<br>Steady: `3500/m`  **Scopes:** `catalogs:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_catalog_item_variants(item_id, async_req=True)
+        >>> thread = api.get_catalog_item_variants(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            item_id (str): The catalog item ID is a compound ID (string), with format: `{integration}:::{catalog}:::{external_id}`. Currently, the only supported integration type is `$custom`, and the only supported catalog is `$default`.
+            id (str): 
 
         Keyword Args:
-            fields_catalog_variant ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`ids`: `any`<br>`item`: `equals`<br>`sku`: `equals`<br>`title`: `contains`<br>`published`: `equals`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
-            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
+            fields_catalog_variant ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`ids`: `any`<br>`item`: `equals`<br>`sku`: `equals`<br>`title`: `contains`<br>`published`: `equals`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
+            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -5311,16 +5311,16 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['item_id'] = \
-            item_id
+        kwargs['id'] = \
+            id
         return self.get_catalog_item_variants_endpoint.call_with_http_info(**kwargs)
 
     def get_catalog_items(
         self,
         **kwargs
     ):
         """Get Catalog Items  # noqa: E501
@@ -5330,20 +5330,20 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_catalog_items(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            fields_catalog_item ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_catalog_variant ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`ids`: `any`<br>`category`: `equals`<br>`title`: `contains`<br>`published`: `equals`. [optional]
-            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#relationships. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
-            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
+            fields_catalog_item ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_catalog_variant ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`ids`: `any`<br>`category`: `equals`<br>`title`: `contains`<br>`published`: `equals`. [optional]
+            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#relationships. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
+            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -5417,15 +5417,15 @@
         >>> thread = api.get_catalog_variant(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): The catalog variant ID is a compound ID (string), with format: `{integration}:::{catalog}:::{external_id}`. Currently, the only supported integration type is `$custom`, and the only supported catalog is `$default`.
 
         Keyword Args:
-            fields_catalog_variant ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_catalog_variant ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -5498,18 +5498,18 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_catalog_variants(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            fields_catalog_variant ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`ids`: `any`<br>`item`: `equals`<br>`sku`: `equals`<br>`title`: `contains`<br>`published`: `equals`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
-            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
+            fields_catalog_variant ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`ids`: `any`<br>`item`: `equals`<br>`sku`: `equals`<br>`title`: `contains`<br>`published`: `equals`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
+            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -5583,17 +5583,17 @@
         >>> thread = api.get_create_categories_job(job_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             job_id (str): ID of the job to retrieve.
 
         Keyword Args:
-            fields_catalog_category_bulk_create_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_catalog_category ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#relationships. [optional]
+            fields_catalog_category_bulk_create_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_catalog_category ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#relationships. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -5666,17 +5666,17 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_create_categories_jobs(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            fields_catalog_category_bulk_create_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`status`: `equals`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            fields_catalog_category_bulk_create_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`status`: `equals`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -5750,17 +5750,17 @@
         >>> thread = api.get_create_items_job(job_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             job_id (str): ID of the job to retrieve.
 
         Keyword Args:
-            fields_catalog_item_bulk_create_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_catalog_item ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#relationships. [optional]
+            fields_catalog_item_bulk_create_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_catalog_item ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#relationships. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -5833,17 +5833,17 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_create_items_jobs(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            fields_catalog_item_bulk_create_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`status`: `equals`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            fields_catalog_item_bulk_create_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`status`: `equals`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -5917,17 +5917,17 @@
         >>> thread = api.get_create_variants_job(job_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             job_id (str): ID of the job to retrieve.
 
         Keyword Args:
-            fields_catalog_variant_bulk_create_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_catalog_variant ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#relationships. [optional]
+            fields_catalog_variant_bulk_create_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_catalog_variant ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#relationships. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -6000,17 +6000,17 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_create_variants_jobs(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            fields_catalog_variant_bulk_create_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`status`: `equals`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            fields_catalog_variant_bulk_create_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`status`: `equals`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -6084,15 +6084,15 @@
         >>> thread = api.get_delete_categories_job(job_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             job_id (str): ID of the job to retrieve.
 
         Keyword Args:
-            fields_catalog_category_bulk_delete_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_catalog_category_bulk_delete_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -6165,17 +6165,17 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_delete_categories_jobs(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            fields_catalog_category_bulk_delete_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`status`: `equals`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            fields_catalog_category_bulk_delete_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`status`: `equals`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -6249,15 +6249,15 @@
         >>> thread = api.get_delete_items_job(job_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             job_id (str): ID of the job to retrieve.
 
         Keyword Args:
-            fields_catalog_item_bulk_delete_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_catalog_item_bulk_delete_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -6330,17 +6330,17 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_delete_items_jobs(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            fields_catalog_item_bulk_delete_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`status`: `equals`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            fields_catalog_item_bulk_delete_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`status`: `equals`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -6414,15 +6414,15 @@
         >>> thread = api.get_delete_variants_job(job_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             job_id (str): ID of the job to retrieve.
 
         Keyword Args:
-            fields_catalog_variant_bulk_delete_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_catalog_variant_bulk_delete_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -6495,17 +6495,17 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_delete_variants_jobs(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            fields_catalog_variant_bulk_delete_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`status`: `equals`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            fields_catalog_variant_bulk_delete_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`status`: `equals`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -6579,17 +6579,17 @@
         >>> thread = api.get_update_categories_job(job_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             job_id (str): ID of the job to retrieve.
 
         Keyword Args:
-            fields_catalog_category_bulk_update_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_catalog_category ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#relationships. [optional]
+            fields_catalog_category_bulk_update_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_catalog_category ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#relationships. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -6662,17 +6662,17 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_update_categories_jobs(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            fields_catalog_category_bulk_update_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`status`: `equals`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            fields_catalog_category_bulk_update_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`status`: `equals`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -6746,17 +6746,17 @@
         >>> thread = api.get_update_items_job(job_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             job_id (str): ID of the job to retrieve.
 
         Keyword Args:
-            fields_catalog_item_bulk_update_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_catalog_item ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#relationships. [optional]
+            fields_catalog_item_bulk_update_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_catalog_item ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#relationships. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -6829,17 +6829,17 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_update_items_jobs(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            fields_catalog_item_bulk_update_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`status`: `equals`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            fields_catalog_item_bulk_update_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`status`: `equals`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -6913,17 +6913,17 @@
         >>> thread = api.get_update_variants_job(job_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             job_id (str): ID of the job to retrieve.
 
         Keyword Args:
-            fields_catalog_variant_bulk_update_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_catalog_variant ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#relationships. [optional]
+            fields_catalog_variant_bulk_update_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_catalog_variant ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#relationships. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -6996,17 +6996,17 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_update_variants_jobs(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            fields_catalog_variant_bulk_update_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`status`: `equals`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            fields_catalog_variant_bulk_update_job ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`status`: `equals`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/api/data_privacy_api.py` & `klaviyo-api-3.0.0/src/openapi_client/api/data_privacy_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/api/events_api.py` & `klaviyo-api-3.0.0/src/openapi_client/api/events_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -790,18 +790,18 @@
         >>> thread = api.get_event(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): ID of the event
 
         Keyword Args:
-            fields_event ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_metric ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_profile ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#relationships. [optional]
+            fields_event ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_metric ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_profile ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#relationships. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -874,18 +874,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_event_metrics(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): ID of the event
+            id (str): 
 
         Keyword Args:
-            fields_metric ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_metric ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -958,19 +958,19 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_event_profiles(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): ID of the event
+            id (str): 
 
         Keyword Args:
             additional_fields_profile ([str]): Request additional fields not included by default in the response. Supported values: 'predictive_analytics'. [optional]
-            fields_profile ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_profile ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1209,21 +1209,21 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_events(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            fields_event ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_metric ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_profile ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`metric_id`: `equals`<br>`profile_id`: `equals`<br>`datetime`: `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`timestamp`: `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`. [optional]
-            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#relationships. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
-            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
+            fields_event ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_metric ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_profile ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`metric_id`: `equals`<br>`profile_id`: `equals`<br>`datetime`: `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`timestamp`: `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`. [optional]
+            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#relationships. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
+            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/api/flows_api.py` & `klaviyo-api-3.0.0/src/openapi_client/api/flows_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -259,26 +259,26 @@
         )
         self.get_flow_action_flow_endpoint = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'Klaviyo-API-Key'
                 ],
-                'endpoint_path': '/api/flow-actions/{action_id}/flow/',
+                'endpoint_path': '/api/flow-actions/{id}/flow/',
                 'operation_id': 'get_flow_action_flow',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'action_id',
+                    'id',
                     'fields_flow',
                 ],
                 'required': [
-                    'action_id',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'fields_flow',
                 ],
                 'validation': [
@@ -295,25 +295,25 @@
                         "ARCHIVED": "archived",
                         "CREATED": "created",
                         "UPDATED": "updated",
                         "TRIGGER_TYPE": "trigger_type"
                     },
                 },
                 'openapi_types': {
-                    'action_id':
+                    'id':
                         (str,),
                     'fields_flow':
                         ([str],),
                 },
                 'attribute_map': {
-                    'action_id': 'action_id',
+                    'id': 'id',
                     'fields_flow': 'fields[flow]',
                 },
                 'location_map': {
-                    'action_id': 'path',
+                    'id': 'path',
                     'fields_flow': 'query',
                 },
                 'collection_format_map': {
                     'fields_flow': 'csv',
                 }
             },
             headers_map={
@@ -326,30 +326,30 @@
         )
         self.get_flow_action_messages_endpoint = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'Klaviyo-API-Key'
                 ],
-                'endpoint_path': '/api/flow-actions/{action_id}/flow-messages/',
+                'endpoint_path': '/api/flow-actions/{id}/flow-messages/',
                 'operation_id': 'get_flow_action_messages',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'action_id',
+                    'id',
                     'fields_flow_message',
                     'filter',
                     'page_cursor',
                     'page_size',
                     'sort',
                 ],
                 'required': [
-                    'action_id',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'fields_flow_message',
                     'sort',
                 ],
@@ -383,37 +383,37 @@
                         "NAME": "name",
                         "-NAME": "-name",
                         "UPDATED": "updated",
                         "-UPDATED": "-updated"
                     },
                 },
                 'openapi_types': {
-                    'action_id':
+                    'id':
                         (str,),
                     'fields_flow_message':
                         ([str],),
                     'filter':
                         (str,),
                     'page_cursor':
                         (str,),
                     'page_size':
                         (int,),
                     'sort':
                         (str,),
                 },
                 'attribute_map': {
-                    'action_id': 'action_id',
+                    'id': 'id',
                     'fields_flow_message': 'fields[flow-message]',
                     'filter': 'filter',
                     'page_cursor': 'page[cursor]',
                     'page_size': 'page[size]',
                     'sort': 'sort',
                 },
                 'location_map': {
-                    'action_id': 'path',
+                    'id': 'path',
                     'fields_flow_message': 'query',
                     'filter': 'query',
                     'page_cursor': 'query',
                     'page_size': 'query',
                     'sort': 'query',
                 },
                 'collection_format_map': {
@@ -570,30 +570,30 @@
         )
         self.get_flow_flow_actions_endpoint = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'Klaviyo-API-Key'
                 ],
-                'endpoint_path': '/api/flows/{flow_id}/flow-actions/',
+                'endpoint_path': '/api/flows/{id}/flow-actions/',
                 'operation_id': 'get_flow_flow_actions',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'flow_id',
+                    'id',
                     'fields_flow_action',
                     'filter',
                     'page_cursor',
                     'page_size',
                     'sort',
                 ],
                 'required': [
-                    'flow_id',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'fields_flow_action',
                     'sort',
                 ],
@@ -638,37 +638,37 @@
                         "STATUS": "status",
                         "-STATUS": "-status",
                         "UPDATED": "updated",
                         "-UPDATED": "-updated"
                     },
                 },
                 'openapi_types': {
-                    'flow_id':
+                    'id':
                         (str,),
                     'fields_flow_action':
                         ([str],),
                     'filter':
                         (str,),
                     'page_cursor':
                         (str,),
                     'page_size':
                         (int,),
                     'sort':
                         (str,),
                 },
                 'attribute_map': {
-                    'flow_id': 'flow_id',
+                    'id': 'id',
                     'fields_flow_action': 'fields[flow-action]',
                     'filter': 'filter',
                     'page_cursor': 'page[cursor]',
                     'page_size': 'page[size]',
                     'sort': 'sort',
                 },
                 'location_map': {
-                    'flow_id': 'path',
+                    'id': 'path',
                     'fields_flow_action': 'query',
                     'filter': 'query',
                     'page_cursor': 'query',
                     'page_size': 'query',
                     'sort': 'query',
                 },
                 'collection_format_map': {
@@ -786,26 +786,26 @@
         )
         self.get_flow_message_action_endpoint = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'Klaviyo-API-Key'
                 ],
-                'endpoint_path': '/api/flow-messages/{message_id}/flow-action/',
+                'endpoint_path': '/api/flow-messages/{id}/flow-action/',
                 'operation_id': 'get_flow_message_action',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'message_id',
+                    'id',
                     'fields_flow_action',
                 ],
                 'required': [
-                    'message_id',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'fields_flow_action',
                 ],
                 'validation': [
@@ -830,25 +830,25 @@
                         "RENDER_OPTIONS.SHORTEN_LINKS": "render_options.shorten_links",
                         "RENDER_OPTIONS.ADD_ORG_PREFIX": "render_options.add_org_prefix",
                         "RENDER_OPTIONS.ADD_INFO_LINK": "render_options.add_info_link",
                         "RENDER_OPTIONS.ADD_OPT_OUT_LANGUAGE": "render_options.add_opt_out_language"
                     },
                 },
                 'openapi_types': {
-                    'message_id':
+                    'id':
                         (str,),
                     'fields_flow_action':
                         ([str],),
                 },
                 'attribute_map': {
-                    'message_id': 'message_id',
+                    'id': 'id',
                     'fields_flow_action': 'fields[flow-action]',
                 },
                 'location_map': {
-                    'message_id': 'path',
+                    'id': 'path',
                     'fields_flow_action': 'query',
                 },
                 'collection_format_map': {
                     'fields_flow_action': 'csv',
                 }
             },
             headers_map={
@@ -1047,26 +1047,26 @@
         )
         self.get_flow_tags_endpoint = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'Klaviyo-API-Key'
                 ],
-                'endpoint_path': '/api/flows/{flow_id}/tags/',
+                'endpoint_path': '/api/flows/{id}/tags/',
                 'operation_id': 'get_flow_tags',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'flow_id',
+                    'id',
                     'fields_tag',
                 ],
                 'required': [
-                    'flow_id',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'fields_tag',
                 ],
                 'validation': [
@@ -1078,25 +1078,25 @@
                 'allowed_values': {
                     ('fields_tag',): {
 
                         "NAME": "name"
                     },
                 },
                 'openapi_types': {
-                    'flow_id':
+                    'id':
                         (str,),
                     'fields_tag':
                         ([str],),
                 },
                 'attribute_map': {
-                    'flow_id': 'flow_id',
+                    'id': 'id',
                     'fields_tag': 'fields[tag]',
                 },
                 'location_map': {
-                    'flow_id': 'path',
+                    'id': 'path',
                     'fields_tag': 'query',
                 },
                 'collection_format_map': {
                     'fields_tag': 'csv',
                 }
             },
             headers_map={
@@ -1317,17 +1317,17 @@
         >>> thread = api.get_flow(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): 
 
         Keyword Args:
-            fields_flow_action ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_flow ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#relationships. [optional]
+            fields_flow_action ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_flow ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#relationships. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1403,18 +1403,18 @@
         >>> thread = api.get_flow_action(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): 
 
         Keyword Args:
-            fields_flow_action ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_flow_message ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_flow ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#relationships. [optional]
+            fields_flow_action ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_flow_message ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_flow ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#relationships. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1474,31 +1474,31 @@
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.get_flow_action_endpoint.call_with_http_info(**kwargs)
 
     def get_flow_action_flow(
         self,
-        action_id,
+        id,
         **kwargs
     ):
         """Get Flow For Flow Action  # noqa: E501
 
         Get the flow associated with the given action ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_flow_action_flow(action_id, async_req=True)
+        >>> thread = api.get_flow_action_flow(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            action_id (str): 
+            id (str): 
 
         Keyword Args:
-            fields_flow ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_flow ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1552,41 +1552,41 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['action_id'] = \
-            action_id
+        kwargs['id'] = \
+            id
         return self.get_flow_action_flow_endpoint.call_with_http_info(**kwargs)
 
     def get_flow_action_messages(
         self,
-        action_id,
+        id,
         **kwargs
     ):
         """Get Messages For Flow Action  # noqa: E501
 
         Get all flow messages associated with the given flow action ID.  Returns a maximum of 50 flow message relationships per request, which can be paginated with cursor-based pagination.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_flow_action_messages(action_id, async_req=True)
+        >>> thread = api.get_flow_action_messages(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            action_id (str): 
+            id (str): 
 
         Keyword Args:
-            fields_flow_message ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`id`: `any`<br>`name`: `contains`, `ends-with`, `equals`, `starts-with`<br>`created`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`updated`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            fields_flow_message ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`id`: `any`<br>`name`: `contains`, `ends-with`, `equals`, `starts-with`<br>`created`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`updated`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             page_size (int): Default: 50. Min: 1. Max: 50.. [optional] if omitted the server will use the default value of 50
-            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
+            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1640,16 +1640,16 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['action_id'] = \
-            action_id
+        kwargs['id'] = \
+            id
         return self.get_flow_action_messages_endpoint.call_with_http_info(**kwargs)
 
     def get_flow_action_relationships_flow(
         self,
         id,
         **kwargs
     ):
@@ -1745,18 +1745,18 @@
         >>> thread = api.get_flow_action_relationships_messages(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): 
 
         Keyword Args:
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`name`: `contains`, `ends-with`, `equals`, `starts-with`<br>`created`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`updated`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`name`: `contains`, `ends-with`, `equals`, `starts-with`<br>`created`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`updated`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             page_size (int): Default: 50. Min: 1. Max: 50.. [optional] if omitted the server will use the default value of 50
-            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
+            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1816,35 +1816,35 @@
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.get_flow_action_relationships_messages_endpoint.call_with_http_info(**kwargs)
 
     def get_flow_flow_actions(
         self,
-        flow_id,
+        id,
         **kwargs
     ):
         """Get Flow Actions For Flow  # noqa: E501
 
         Get all flow actions associated with the given flow ID.  Returns a maximum of 50 flows per request, which can be paginated with cursor-based pagination.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_flow_flow_actions(flow_id, async_req=True)
+        >>> thread = api.get_flow_flow_actions(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            flow_id (str): 
+            id (str): 
 
         Keyword Args:
-            fields_flow_action ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`id`: `any`<br>`action_type`: `any`, `equals`<br>`status`: `equals`<br>`created`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`updated`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            fields_flow_action ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`id`: `any`<br>`action_type`: `any`, `equals`<br>`status`: `equals`<br>`created`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`updated`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             page_size (int): Default: 50. Min: 1. Max: 50.. [optional] if omitted the server will use the default value of 50
-            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
+            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1898,16 +1898,16 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['flow_id'] = \
-            flow_id
+        kwargs['id'] = \
+            id
         return self.get_flow_flow_actions_endpoint.call_with_http_info(**kwargs)
 
     def get_flow_message(
         self,
         id,
         **kwargs
     ):
@@ -1920,17 +1920,17 @@
         >>> thread = api.get_flow_message(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): 
 
         Keyword Args:
-            fields_flow_action ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_flow_message ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#relationships. [optional]
+            fields_flow_action ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_flow_message ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#relationships. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1990,31 +1990,31 @@
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.get_flow_message_endpoint.call_with_http_info(**kwargs)
 
     def get_flow_message_action(
         self,
-        message_id,
+        id,
         **kwargs
     ):
         """Get Flow Action For Message  # noqa: E501
 
         Get the flow action for a flow message with the given message ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_flow_message_action(message_id, async_req=True)
+        >>> thread = api.get_flow_message_action(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            message_id (str): 
+            id (str): 
 
         Keyword Args:
-            fields_flow_action ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_flow_action ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2068,16 +2068,16 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['message_id'] = \
-            message_id
+        kwargs['id'] = \
+            id
         return self.get_flow_message_action_endpoint.call_with_http_info(**kwargs)
 
     def get_flow_message_relationships_action(
         self,
         id,
         **kwargs
     ):
@@ -2173,17 +2173,17 @@
         >>> thread = api.get_flow_relationships_flow_actions(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): 
 
         Keyword Args:
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`action_type`: `equals`<br>`status`: `equals`<br>`created`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`updated`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`action_type`: `equals`<br>`status`: `equals`<br>`created`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`updated`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`. [optional]
             page_size (int): Default: 50. Min: 1. Max: 100.. [optional] if omitted the server will use the default value of 50
-            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
+            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2326,31 +2326,31 @@
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.get_flow_relationships_tags_endpoint.call_with_http_info(**kwargs)
 
     def get_flow_tags(
         self,
-        flow_id,
+        id,
         **kwargs
     ):
         """Get Flow Tags  # noqa: E501
 
         Return all tags associated with the given flow ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `flows:read` `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_flow_tags(flow_id, async_req=True)
+        >>> thread = api.get_flow_tags(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            flow_id (str): 
+            id (str): 
 
         Keyword Args:
-            fields_tag ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_tag ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2404,16 +2404,16 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['flow_id'] = \
-            flow_id
+        kwargs['id'] = \
+            id
         return self.get_flow_tags_endpoint.call_with_http_info(**kwargs)
 
     def get_flows(
         self,
         **kwargs
     ):
         """Get Flows  # noqa: E501
@@ -2423,21 +2423,21 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_flows(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            fields_flow_action ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_flow ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`id`: `any`<br>`name`: `contains`, `ends-with`, `equals`, `starts-with`<br>`status`: `equals`<br>`archived`: `equals`<br>`created`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`updated`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`trigger_type`: `equals`. [optional]
-            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#relationships. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            fields_flow_action ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_flow ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`id`: `any`<br>`name`: `contains`, `ends-with`, `equals`, `starts-with`<br>`status`: `equals`<br>`archived`: `equals`<br>`created`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`updated`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`trigger_type`: `equals`. [optional]
+            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#relationships. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             page_size (int): Default: 50. Min: 1. Max: 50.. [optional] if omitted the server will use the default value of 50
-            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
+            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/api/lists_api.py` & `klaviyo-api-3.0.0/src/openapi_client/api/lists_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -325,30 +325,30 @@
         )
         self.get_list_profiles_endpoint = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'Klaviyo-API-Key'
                 ],
-                'endpoint_path': '/api/lists/{list_id}/profiles/',
+                'endpoint_path': '/api/lists/{id}/profiles/',
                 'operation_id': 'get_list_profiles',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'list_id',
+                    'id',
                     'additional_fields_profile',
                     'fields_profile',
                     'filter',
                     'page_cursor',
                     'page_size',
                 ],
                 'required': [
-                    'list_id',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'additional_fields_profile',
                     'fields_profile',
                 ],
@@ -424,37 +424,37 @@
                         "PREDICTIVE_ANALYTICS.AVERAGE_DAYS_BETWEEN_ORDERS": "predictive_analytics.average_days_between_orders",
                         "PREDICTIVE_ANALYTICS.AVERAGE_ORDER_VALUE": "predictive_analytics.average_order_value",
                         "PREDICTIVE_ANALYTICS.CHURN_PROBABILITY": "predictive_analytics.churn_probability",
                         "PREDICTIVE_ANALYTICS.EXPECTED_DATE_OF_NEXT_ORDER": "predictive_analytics.expected_date_of_next_order"
                     },
                 },
                 'openapi_types': {
-                    'list_id':
+                    'id':
                         (str,),
                     'additional_fields_profile':
                         ([str],),
                     'fields_profile':
                         ([str],),
                     'filter':
                         (str,),
                     'page_cursor':
                         (str,),
                     'page_size':
                         (int,),
                 },
                 'attribute_map': {
-                    'list_id': 'list_id',
+                    'id': 'id',
                     'additional_fields_profile': 'additional-fields[profile]',
                     'fields_profile': 'fields[profile]',
                     'filter': 'filter',
                     'page_cursor': 'page[cursor]',
                     'page_size': 'page[size]',
                 },
                 'location_map': {
-                    'list_id': 'path',
+                    'id': 'path',
                     'additional_fields_profile': 'query',
                     'fields_profile': 'query',
                     'filter': 'query',
                     'page_cursor': 'query',
                     'page_size': 'query',
                 },
                 'collection_format_map': {
@@ -579,26 +579,26 @@
         )
         self.get_list_tags_endpoint = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'Klaviyo-API-Key'
                 ],
-                'endpoint_path': '/api/lists/{list_id}/tags/',
+                'endpoint_path': '/api/lists/{id}/tags/',
                 'operation_id': 'get_list_tags',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'list_id',
+                    'id',
                     'fields_tag',
                 ],
                 'required': [
-                    'list_id',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'fields_tag',
                 ],
                 'validation': [
@@ -610,25 +610,25 @@
                 'allowed_values': {
                     ('fields_tag',): {
 
                         "NAME": "name"
                     },
                 },
                 'openapi_types': {
-                    'list_id':
+                    'id':
                         (str,),
                     'fields_tag':
                         ([str],),
                 },
                 'attribute_map': {
-                    'list_id': 'list_id',
+                    'id': 'id',
                     'fields_tag': 'fields[tag]',
                 },
                 'location_map': {
-                    'list_id': 'path',
+                    'id': 'path',
                     'fields_tag': 'query',
                 },
                 'collection_format_map': {
                     'fields_tag': 'csv',
                 }
             },
             headers_map={
@@ -1119,15 +1119,15 @@
         >>> thread = api.get_list(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): Primary key that uniquely identifies this list. Generated by Klaviyo.
 
         Keyword Args:
-            fields_list ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_list ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1187,34 +1187,34 @@
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.get_list_endpoint.call_with_http_info(**kwargs)
 
     def get_list_profiles(
         self,
-        list_id,
+        id,
         **kwargs
     ):
         """Get List Profiles  # noqa: E501
 
         Get all profiles within a list with the given list ID. Filter to request a subset of all profiles. Profiles can be filtered by `email`, `phone_number`, and `push_token` fields.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `list:read` `profiles:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_list_profiles(list_id, async_req=True)
+        >>> thread = api.get_list_profiles(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            list_id (str): Primary key that uniquely identifies this list. Generated by Klaviyo.
+            id (str): 
 
         Keyword Args:
             additional_fields_profile ([str]): Request additional fields not included by default in the response. Supported values: 'predictive_analytics'. [optional]
-            fields_profile ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`email`: `any`<br>`phone_number`: `any`<br>`push_token`: `any`<br>`_kx`: `equals`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            fields_profile ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`email`: `any`<br>`phone_number`: `any`<br>`push_token`: `any`<br>`_kx`: `equals`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             page_size (int): Default: 20. Min: 1. Max: 100.. [optional] if omitted the server will use the default value of 20
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -1269,16 +1269,16 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['list_id'] = \
-            list_id
+        kwargs['id'] = \
+            id
         return self.get_list_profiles_endpoint.call_with_http_info(**kwargs)
 
     def get_list_relationships_profiles(
         self,
         id,
         **kwargs
     ):
@@ -1291,15 +1291,15 @@
         >>> thread = api.get_list_relationships_profiles(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): 
 
         Keyword Args:
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1442,31 +1442,31 @@
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.get_list_relationships_tags_endpoint.call_with_http_info(**kwargs)
 
     def get_list_tags(
         self,
-        list_id,
+        id,
         **kwargs
     ):
         """Get List Tags  # noqa: E501
 
         Return all tags associated with the given list ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `list:read` `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_list_tags(list_id, async_req=True)
+        >>> thread = api.get_list_tags(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            list_id (str): Primary key that uniquely identifies this list. Generated by Klaviyo.
+            id (str): 
 
         Keyword Args:
-            fields_tag ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_tag ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1520,16 +1520,16 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['list_id'] = \
-            list_id
+        kwargs['id'] = \
+            id
         return self.get_list_tags_endpoint.call_with_http_info(**kwargs)
 
     def get_lists(
         self,
         **kwargs
     ):
         """Get Lists  # noqa: E501
@@ -1539,17 +1539,17 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_lists(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            fields_list ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`name`: `any`, `equals`<br>`id`: `any`, `equals`<br>`created`: `greater-than`<br>`updated`: `greater-than`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            fields_list ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`name`: `any`, `equals`<br>`id`: `any`, `equals`<br>`created`: `greater-than`<br>`updated`: `greater-than`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/api/metrics_api.py` & `klaviyo-api-3.0.0/src/openapi_client/api/metrics_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -237,15 +237,15 @@
         >>> thread = api.get_metric(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): Metric ID
 
         Keyword Args:
-            fields_metric ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_metric ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -318,17 +318,17 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_metrics(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            fields_metric ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`integration.name`: `equals`<br>`integration.category`: `equals`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            fields_metric ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`integration.name`: `equals`<br>`integration.category`: `equals`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/api/profiles_api.py` & `klaviyo-api-3.0.0/src/openapi_client/api/profiles_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -260,26 +260,26 @@
         )
         self.get_profile_lists_endpoint = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'Klaviyo-API-Key'
                 ],
-                'endpoint_path': '/api/profiles/{profile_id}/lists/',
+                'endpoint_path': '/api/profiles/{id}/lists/',
                 'operation_id': 'get_profile_lists',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'profile_id',
+                    'id',
                     'fields_list',
                 ],
                 'required': [
-                    'profile_id',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'fields_list',
                 ],
                 'validation': [
@@ -293,25 +293,25 @@
 
                         "NAME": "name",
                         "CREATED": "created",
                         "UPDATED": "updated"
                     },
                 },
                 'openapi_types': {
-                    'profile_id':
+                    'id':
                         (str,),
                     'fields_list':
                         ([str],),
                 },
                 'attribute_map': {
-                    'profile_id': 'profile_id',
+                    'id': 'id',
                     'fields_list': 'fields[list]',
                 },
                 'location_map': {
-                    'profile_id': 'path',
+                    'id': 'path',
                     'fields_list': 'query',
                 },
                 'collection_format_map': {
                     'fields_list': 'csv',
                 }
             },
             headers_map={
@@ -426,26 +426,26 @@
         )
         self.get_profile_segments_endpoint = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'Klaviyo-API-Key'
                 ],
-                'endpoint_path': '/api/profiles/{profile_id}/segments/',
+                'endpoint_path': '/api/profiles/{id}/segments/',
                 'operation_id': 'get_profile_segments',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'profile_id',
+                    'id',
                     'fields_segment',
                 ],
                 'required': [
-                    'profile_id',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'fields_segment',
                 ],
                 'validation': [
@@ -459,25 +459,25 @@
 
                         "NAME": "name",
                         "CREATED": "created",
                         "UPDATED": "updated"
                     },
                 },
                 'openapi_types': {
-                    'profile_id':
+                    'id':
                         (str,),
                     'fields_segment':
                         ([str],),
                 },
                 'attribute_map': {
-                    'profile_id': 'profile_id',
+                    'id': 'id',
                     'fields_segment': 'fields[segment]',
                 },
                 'location_map': {
-                    'profile_id': 'path',
+                    'id': 'path',
                     'fields_segment': 'query',
                 },
                 'collection_format_map': {
                     'fields_segment': 'csv',
                 }
             },
             headers_map={
@@ -1010,18 +1010,18 @@
         >>> result = thread.get()
 
         Args:
             id (str): 
 
         Keyword Args:
             additional_fields_profile ([str]): Request additional fields not included by default in the response. Supported values: 'predictive_analytics'. [optional]
-            fields_list ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_profile ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            fields_segment ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#relationships. [optional]
+            fields_list ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_profile ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            fields_segment ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            include ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#relationships. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1081,31 +1081,31 @@
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.get_profile_endpoint.call_with_http_info(**kwargs)
 
     def get_profile_lists(
         self,
-        profile_id,
+        id,
         **kwargs
     ):
         """Get Profile Lists  # noqa: E501
 
         Get list memberships for a profile with the given profile ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `list:read` `profiles:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_profile_lists(profile_id, async_req=True)
+        >>> thread = api.get_profile_lists(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            profile_id (str): 
+            id (str): 
 
         Keyword Args:
-            fields_list ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_list ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1159,16 +1159,16 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['profile_id'] = \
-            profile_id
+        kwargs['id'] = \
+            id
         return self.get_profile_lists_endpoint.call_with_http_info(**kwargs)
 
     def get_profile_relationships_lists(
         self,
         id,
         **kwargs
     ):
@@ -1331,31 +1331,31 @@
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.get_profile_relationships_segments_endpoint.call_with_http_info(**kwargs)
 
     def get_profile_segments(
         self,
-        profile_id,
+        id,
         **kwargs
     ):
         """Get Profile Segments  # noqa: E501
 
         Get segment memberships for a profile with the given profile ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `profiles:read` `segments:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_profile_segments(profile_id, async_req=True)
+        >>> thread = api.get_profile_segments(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            profile_id (str): 
+            id (str): 
 
         Keyword Args:
-            fields_segment ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_segment ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1409,16 +1409,16 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['profile_id'] = \
-            profile_id
+        kwargs['id'] = \
+            id
         return self.get_profile_segments_endpoint.call_with_http_info(**kwargs)
 
     def get_profiles(
         self,
         **kwargs
     ):
         """Get Profiles  # noqa: E501
@@ -1429,19 +1429,19 @@
 
         >>> thread = api.get_profiles(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
             additional_fields_profile ([str]): Request additional fields not included by default in the response. Supported values: 'predictive_analytics'. [optional]
-            fields_profile ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`id`: `any`, `equals`<br>`email`: `any`, `equals`<br>`phone_number`: `any`, `equals`<br>`external_id`: `any`, `equals`<br>`_kx`: `equals`<br>`created`: `greater-than`, `less-than`<br>`updated`: `greater-than`, `less-than`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            fields_profile ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`id`: `any`, `equals`<br>`email`: `any`, `equals`<br>`phone_number`: `any`, `equals`<br>`external_id`: `any`, `equals`<br>`_kx`: `equals`<br>`created`: `greater-than`, `less-than`<br>`updated`: `greater-than`, `less-than`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             page_size (int): Default: 20. Min: 1. Max: 100.. [optional] if omitted the server will use the default value of 20
-            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
+            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/api/segments_api.py` & `klaviyo-api-3.0.0/src/openapi_client/api/segments_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -103,30 +103,30 @@
         )
         self.get_segment_profiles_endpoint = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'Klaviyo-API-Key'
                 ],
-                'endpoint_path': '/api/segments/{segment_id}/profiles/',
+                'endpoint_path': '/api/segments/{id}/profiles/',
                 'operation_id': 'get_segment_profiles',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'segment_id',
+                    'id',
                     'additional_fields_profile',
                     'fields_profile',
                     'filter',
                     'page_cursor',
                     'page_size',
                 ],
                 'required': [
-                    'segment_id',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'additional_fields_profile',
                     'fields_profile',
                 ],
@@ -202,37 +202,37 @@
                         "PREDICTIVE_ANALYTICS.AVERAGE_DAYS_BETWEEN_ORDERS": "predictive_analytics.average_days_between_orders",
                         "PREDICTIVE_ANALYTICS.AVERAGE_ORDER_VALUE": "predictive_analytics.average_order_value",
                         "PREDICTIVE_ANALYTICS.CHURN_PROBABILITY": "predictive_analytics.churn_probability",
                         "PREDICTIVE_ANALYTICS.EXPECTED_DATE_OF_NEXT_ORDER": "predictive_analytics.expected_date_of_next_order"
                     },
                 },
                 'openapi_types': {
-                    'segment_id':
+                    'id':
                         (str,),
                     'additional_fields_profile':
                         ([str],),
                     'fields_profile':
                         ([str],),
                     'filter':
                         (str,),
                     'page_cursor':
                         (str,),
                     'page_size':
                         (int,),
                 },
                 'attribute_map': {
-                    'segment_id': 'segment_id',
+                    'id': 'id',
                     'additional_fields_profile': 'additional-fields[profile]',
                     'fields_profile': 'fields[profile]',
                     'filter': 'filter',
                     'page_cursor': 'page[cursor]',
                     'page_size': 'page[size]',
                 },
                 'location_map': {
-                    'segment_id': 'path',
+                    'id': 'path',
                     'additional_fields_profile': 'query',
                     'fields_profile': 'query',
                     'filter': 'query',
                     'page_cursor': 'query',
                     'page_size': 'query',
                 },
                 'collection_format_map': {
@@ -357,26 +357,26 @@
         )
         self.get_segment_tags_endpoint = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'Klaviyo-API-Key'
                 ],
-                'endpoint_path': '/api/segments/{segment_id}/tags/',
+                'endpoint_path': '/api/segments/{id}/tags/',
                 'operation_id': 'get_segment_tags',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'segment_id',
+                    'id',
                     'fields_tag',
                 ],
                 'required': [
-                    'segment_id',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'fields_tag',
                 ],
                 'validation': [
@@ -388,25 +388,25 @@
                 'allowed_values': {
                     ('fields_tag',): {
 
                         "NAME": "name"
                     },
                 },
                 'openapi_types': {
-                    'segment_id':
+                    'id':
                         (str,),
                     'fields_tag':
                         ([str],),
                 },
                 'attribute_map': {
-                    'segment_id': 'segment_id',
+                    'id': 'id',
                     'fields_tag': 'fields[tag]',
                 },
                 'location_map': {
-                    'segment_id': 'path',
+                    'id': 'path',
                     'fields_tag': 'query',
                 },
                 'collection_format_map': {
                     'fields_tag': 'csv',
                 }
             },
             headers_map={
@@ -557,15 +557,15 @@
         >>> thread = api.get_segment(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): 
 
         Keyword Args:
-            fields_segment ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_segment ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -625,34 +625,34 @@
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.get_segment_endpoint.call_with_http_info(**kwargs)
 
     def get_segment_profiles(
         self,
-        segment_id,
+        id,
         **kwargs
     ):
         """Get Segment Profiles  # noqa: E501
 
         Get all profiles within the given segment ID. Filter to request a subset of all profiles. Profiles can be filtered by `email`, `phone_number`, and `push_token` fields.<br><br>*Rate limits*:<br>Burst: `10/s`<br>Steady: `150/m`  **Scopes:** `profiles:read` `segments:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_segment_profiles(segment_id, async_req=True)
+        >>> thread = api.get_segment_profiles(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            segment_id (str): 
+            id (str): 
 
         Keyword Args:
             additional_fields_profile ([str]): Request additional fields not included by default in the response. Supported values: 'predictive_analytics'. [optional]
-            fields_profile ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`email`: `any`<br>`phone_number`: `any`<br>`push_token`: `any`<br>`_kx`: `equals`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            fields_profile ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`email`: `any`<br>`phone_number`: `any`<br>`push_token`: `any`<br>`_kx`: `equals`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             page_size (int): Default: 20. Min: 1. Max: 100.. [optional] if omitted the server will use the default value of 20
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -707,16 +707,16 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['segment_id'] = \
-            segment_id
+        kwargs['id'] = \
+            id
         return self.get_segment_profiles_endpoint.call_with_http_info(**kwargs)
 
     def get_segment_relationships_profiles(
         self,
         id,
         **kwargs
     ):
@@ -729,15 +729,15 @@
         >>> thread = api.get_segment_relationships_profiles(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): 
 
         Keyword Args:
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -880,31 +880,31 @@
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
         return self.get_segment_relationships_tags_endpoint.call_with_http_info(**kwargs)
 
     def get_segment_tags(
         self,
-        segment_id,
+        id,
         **kwargs
     ):
         """Get Segment Tags  # noqa: E501
 
         Return all tags associated with the given segment ID.<br><br>*Rate limits*:<br>Burst: `3/s`<br>Steady: `60/m`  **Scopes:** `segments:read` `tags:read`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_segment_tags(segment_id, async_req=True)
+        >>> thread = api.get_segment_tags(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            segment_id (str): 
+            id (str): 
 
         Keyword Args:
-            fields_tag ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_tag ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -958,16 +958,16 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['segment_id'] = \
-            segment_id
+        kwargs['id'] = \
+            id
         return self.get_segment_tags_endpoint.call_with_http_info(**kwargs)
 
     def get_segments(
         self,
         **kwargs
     ):
         """Get Segments  # noqa: E501
@@ -977,17 +977,17 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_segments(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            fields_segment ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`name`: `any`, `equals`<br>`id`: `any`, `equals`<br>`created`: `greater-than`<br>`updated`: `greater-than`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
+            fields_segment ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`name`: `any`, `equals`<br>`id`: `any`, `equals`<br>`created`: `greater-than`<br>`updated`: `greater-than`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/api/tags_api.py` & `klaviyo-api-3.0.0/src/openapi_client/api/tags_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -2589,15 +2589,15 @@
         >>> thread = api.get_tag(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): The Tag ID
 
         Keyword Args:
-            fields_tag ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_tag ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2673,15 +2673,15 @@
         >>> thread = api.get_tag_group(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): The Tag Group ID
 
         Keyword Args:
-            fields_tag_group ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_tag_group ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2837,18 +2837,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_tag_group_tags(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): The Tag Group ID
+            id (str): 
 
         Keyword Args:
-            fields_tag ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_tag ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2921,18 +2921,18 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_tag_groups(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            fields_tag_group ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`name`: `contains`, `ends-with`, `equals`, `starts-with`<br>`exclusive`: `equals`<br>`default`: `equals`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
-            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
+            fields_tag_group ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`name`: `contains`, `ends-with`, `equals`, `starts-with`<br>`exclusive`: `equals`<br>`default`: `equals`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
+            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -3418,18 +3418,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_tag_tag_group(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str): The Tag ID
+            id (str): 
 
         Keyword Args:
-            fields_tag_group ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_tag_group ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -3502,18 +3502,18 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_tags(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            fields_tag ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`name`: `contains`, `ends-with`, `equals`, `starts-with`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
-            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
+            fields_tag ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`name`: `contains`, `ends-with`, `equals`, `starts-with`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
+            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/api/templates_api.py` & `klaviyo-api-3.0.0/src/openapi_client/api/templates_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -808,15 +808,15 @@
         >>> thread = api.get_template(id, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (str): The ID of template
 
         Keyword Args:
-            fields_template ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
+            fields_template ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -889,18 +889,18 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_templates(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            fields_template ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sparse-fieldsets. [optional]
-            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`id`: `any`, `equals`<br>`name`: `any`, `equals`<br>`created`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`updated`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`. [optional]
-            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#pagination. [optional]
-            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-02-22/reference/api-overview#sorting. [optional]
+            fields_template ([str]): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sparse-fieldsets. [optional]
+            filter (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#filtering<br>Allowed field(s)/operator(s):<br>`id`: `any`, `equals`<br>`name`: `any`, `equals`<br>`created`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`<br>`updated`: `equals`, `greater-or-equal`, `greater-than`, `less-or-equal`, `less-than`. [optional]
+            page_cursor (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#pagination. [optional]
+            sort (str): For more information please visit https://developers.klaviyo.com/en/v2023-06-15/reference/api-overview#sorting. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/api_client.py` & `klaviyo-api-3.0.0/src/openapi_client/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'klaviyo-api-python/2.0.2'
+        self.user_agent = 'klaviyo-api-python/3.0.0'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
@@ -798,19 +798,19 @@
 
         return params
 
     def __call__(self, *args, **kwargs):
         """ This method is invoked when endpoints are called
         Example:
 
-        api_instance = CampaignsApi()
-        api_instance.create_campaign  # this is an instance of the class Endpoint
-        api_instance.create_campaign()  # this invokes api_instance.create_campaign.__call__()
+        api_instance = AccountsApi()
+        api_instance.get_account  # this is an instance of the class Endpoint
+        api_instance.get_account()  # this invokes api_instance.get_account.__call__()
         which then invokes the callable functions stored in that endpoint at
-        api_instance.create_campaign.callable or self.callable in this class
+        api_instance.get_account.callable or self.callable in this class
 
         """
         return self.callable(self, *args, **kwargs)
 
     def call_with_http_info(self, **kwargs):
 
         if 'api_key' in kwargs:
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/apis/__init__.py` & `klaviyo-api-3.0.0/src/openapi_client/apis/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 # flake8: noqa
 
 # Import all APIs into this package.
 # If you have many APIs here with many many models used in each API this may
 # raise a `RecursionError`.
 # In order to avoid this, import only the API that you directly need like:
 #
-#   from openapi_client.api.campaigns_api import CampaignsApi
+#   from openapi_client.api.accounts_api import AccountsApi
 #
 # or import this package, but before doing it, use:
 #
 #   import sys
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
+from openapi_client.api.accounts_api import AccountsApi
 from openapi_client.api.campaigns_api import CampaignsApi
 from openapi_client.api.catalogs_api import CatalogsApi
-from openapi_client.api.client_api import ClientApi
 from openapi_client.api.data_privacy_api import DataPrivacyApi
 from openapi_client.api.events_api import EventsApi
 from openapi_client.api.flows_api import FlowsApi
 from openapi_client.api.lists_api import ListsApi
 from openapi_client.api.metrics_api import MetricsApi
 from openapi_client.api.profiles_api import ProfilesApi
 from openapi_client.api.segments_api import SegmentsApi
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/configuration.py` & `klaviyo-api-3.0.0/src/openapi_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
@@ -405,16 +405,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2023-02-22\n"\
-               "SDK Package Version: 2.0.2".\
+               "Version of the API: 2023-06-15\n"\
+               "SDK Package Version: 3.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/exceptions.py` & `klaviyo-api-3.0.0/src/openapi_client/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/audiences_sub_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/audiences_sub_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_clone_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_clone_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_clone_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_clone_query_resource_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_clone_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_clone_query_resource_object_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_create_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_create_query_resource_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_create_query_resource_object_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_assign_template_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_message_assign_template_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_assign_template_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_message_assign_template_query_resource_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_assign_template_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_message_assign_template_query_resource_object_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_message_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_partial_update_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_message_partial_update_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_partial_update_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_message_partial_update_query_resource_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_message_partial_update_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_message_partial_update_query_resource_object_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_partial_update_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_partial_update_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_partial_update_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_partial_update_query_resource_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_partial_update_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_partial_update_query_resource_object_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_recipient_estimation_job_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_recipient_estimation_job_create_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_recipient_estimation_job_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_recipient_estimation_job_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_send_job_create_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_send_job_create_query_resource_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_send_job_create_query_resource_object_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_send_job_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_partial_update_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_send_job_partial_update_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_bulk_create_job_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_bulk_create_job_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_bulk_delete_job_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_bulk_delete_job_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_bulk_update_job_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_bulk_update_job_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_job_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_create_job_create_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_job_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_create_job_create_query_resource_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_job_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_create_job_create_query_resource_object_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_create_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_create_query_resource_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_create_query_resource_object_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_delete_job_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_delete_job_create_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_delete_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_delete_query_resource_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_item_op.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_item_op.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_job_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_update_job_create_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_job_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_update_job_create_query_resource_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_job_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_update_job_create_query_resource_object_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_update_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_update_query_resource_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_update_query_resource_object_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query_resource_object_relationships.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_update_query_resource_object_relationships.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items_data_inner.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items_data_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_bulk_create_job_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_bulk_create_job_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_bulk_delete_job_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_bulk_delete_job_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_bulk_update_job_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_bulk_update_job_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_category_op.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_create_query_resource_object_relationships.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.catalog_item_create_query_resource_object_relationships_categories_data_inner import CatalogItemCreateQueryResourceObjectRelationshipsCategoriesDataInner
-    globals()['CatalogItemCreateQueryResourceObjectRelationshipsCategoriesDataInner'] = CatalogItemCreateQueryResourceObjectRelationshipsCategoriesDataInner
+    from openapi_client.model.catalog_item_create_query_resource_object_relationships_categories import CatalogItemCreateQueryResourceObjectRelationshipsCategories
+    globals()['CatalogItemCreateQueryResourceObjectRelationshipsCategories'] = CatalogItemCreateQueryResourceObjectRelationshipsCategories
 
 
-class CatalogItemCategoryOp(ModelNormal):
+class CatalogItemCreateQueryResourceObjectRelationships(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,38 +84,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([CatalogItemCreateQueryResourceObjectRelationshipsCategoriesDataInner],),  # noqa: E501
+            'categories': (CatalogItemCreateQueryResourceObjectRelationshipsCategories,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'categories': 'categories',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """CatalogItemCategoryOp - a model defined in OpenAPI
-
-        Args:
-            data ([CatalogItemCreateQueryResourceObjectRelationshipsCategoriesDataInner]):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """CatalogItemCreateQueryResourceObjectRelationships - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,14 +137,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            categories (CatalogItemCreateQueryResourceObjectRelationshipsCategories): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -171,15 +169,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,19 +189,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """CatalogItemCategoryOp - a model defined in OpenAPI
-
-        Args:
-            data ([CatalogItemCreateQueryResourceObjectRelationshipsCategoriesDataInner]):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """CatalogItemCreateQueryResourceObjectRelationships - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -229,14 +223,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            categories (CatalogItemCreateQueryResourceObjectRelationshipsCategories): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -258,15 +253,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_job_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_create_job_create_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_job_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_create_job_create_query_resource_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_job_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_create_job_create_query_resource_object_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_create_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_create_query_resource_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_create_query_resource_object_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query_resource_object_relationships.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.catalog_item_create_query_resource_object_relationships_categories import CatalogItemCreateQueryResourceObjectRelationshipsCategories
-    globals()['CatalogItemCreateQueryResourceObjectRelationshipsCategories'] = CatalogItemCreateQueryResourceObjectRelationshipsCategories
+    from openapi_client.model.catalog_item_category_op_data_inner import CatalogItemCategoryOpDataInner
+    globals()['CatalogItemCategoryOpDataInner'] = CatalogItemCategoryOpDataInner
 
 
-class CatalogItemCreateQueryResourceObjectRelationships(ModelNormal):
+class CatalogItemCreateQueryResourceObjectRelationshipsCategories(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,35 +84,38 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'categories': (CatalogItemCreateQueryResourceObjectRelationshipsCategories,),  # noqa: E501
+            'data': ([CatalogItemCategoryOpDataInner],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'categories': 'categories',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CatalogItemCreateQueryResourceObjectRelationships - a model defined in OpenAPI
+    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
+        """CatalogItemCreateQueryResourceObjectRelationshipsCategories - a model defined in OpenAPI
+
+        Args:
+            data ([CatalogItemCategoryOpDataInner]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,15 +140,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            categories (CatalogItemCreateQueryResourceObjectRelationshipsCategories): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -169,14 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -189,16 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """CatalogItemCreateQueryResourceObjectRelationships - a model defined in OpenAPI
+    def __init__(self, data, *args, **kwargs):  # noqa: E501
+        """CatalogItemCreateQueryResourceObjectRelationshipsCategories - a model defined in OpenAPI
+
+        Args:
+            data ([CatalogItemCategoryOpDataInner]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -223,15 +229,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            categories (CatalogItemCreateQueryResourceObjectRelationshipsCategories): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -253,14 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_delete_job_create_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.catalog_item_create_query_resource_object_relationships_categories_data_inner import CatalogItemCreateQueryResourceObjectRelationshipsCategoriesDataInner
-    globals()['CatalogItemCreateQueryResourceObjectRelationshipsCategoriesDataInner'] = CatalogItemCreateQueryResourceObjectRelationshipsCategoriesDataInner
+    from openapi_client.model.catalog_item_delete_job_create_query_resource_object import CatalogItemDeleteJobCreateQueryResourceObject
+    globals()['CatalogItemDeleteJobCreateQueryResourceObject'] = CatalogItemDeleteJobCreateQueryResourceObject
 
 
-class CatalogItemCreateQueryResourceObjectRelationshipsCategories(ModelNormal):
+class CatalogItemDeleteJobCreateQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,15 +84,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([CatalogItemCreateQueryResourceObjectRelationshipsCategoriesDataInner],),  # noqa: E501
+            'data': (CatalogItemDeleteJobCreateQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -104,18 +104,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """CatalogItemCreateQueryResourceObjectRelationshipsCategories - a model defined in OpenAPI
+        """CatalogItemDeleteJobCreateQuery - a model defined in OpenAPI
 
         Args:
-            data ([CatalogItemCreateQueryResourceObjectRelationshipsCategoriesDataInner]):
+            data (CatalogItemDeleteJobCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -193,18 +193,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """CatalogItemCreateQueryResourceObjectRelationshipsCategories - a model defined in OpenAPI
+        """CatalogItemDeleteJobCreateQuery - a model defined in OpenAPI
 
         Args:
-            data ([CatalogItemCreateQueryResourceObjectRelationshipsCategoriesDataInner]):
+            data (CatalogItemDeleteJobCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories_data_inner.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_category_op_data_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class CatalogItemCreateQueryResourceObjectRelationshipsCategoriesDataInner(ModelNormal):
+class CatalogItemCategoryOpDataInner(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -103,15 +103,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, id, *args, **kwargs):  # noqa: E501
-        """CatalogItemCreateQueryResourceObjectRelationshipsCategoriesDataInner - a model defined in OpenAPI
+        """CatalogItemCategoryOpDataInner - a model defined in OpenAPI
 
         Args:
             id (str):
 
         Keyword Args:
             type (str): defaults to "catalog-category", must be one of ["catalog-category", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
@@ -195,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, id, *args, **kwargs):  # noqa: E501
-        """CatalogItemCreateQueryResourceObjectRelationshipsCategoriesDataInner - a model defined in OpenAPI
+        """CatalogItemCategoryOpDataInner - a model defined in OpenAPI
 
         Args:
             id (str):
 
         Keyword Args:
             type (str): defaults to "catalog-category", must be one of ["catalog-category", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_delete_job_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_update_job_create_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.catalog_item_delete_job_create_query_resource_object import CatalogItemDeleteJobCreateQueryResourceObject
-    globals()['CatalogItemDeleteJobCreateQueryResourceObject'] = CatalogItemDeleteJobCreateQueryResourceObject
+    from openapi_client.model.catalog_item_update_job_create_query_resource_object import CatalogItemUpdateJobCreateQueryResourceObject
+    globals()['CatalogItemUpdateJobCreateQueryResourceObject'] = CatalogItemUpdateJobCreateQueryResourceObject
 
 
-class CatalogItemDeleteJobCreateQuery(ModelNormal):
+class CatalogItemUpdateJobCreateQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,15 +84,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (CatalogItemDeleteJobCreateQueryResourceObject,),  # noqa: E501
+            'data': (CatalogItemUpdateJobCreateQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -104,18 +104,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """CatalogItemDeleteJobCreateQuery - a model defined in OpenAPI
+        """CatalogItemUpdateJobCreateQuery - a model defined in OpenAPI
 
         Args:
-            data (CatalogItemDeleteJobCreateQueryResourceObject):
+            data (CatalogItemUpdateJobCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -193,18 +193,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """CatalogItemDeleteJobCreateQuery - a model defined in OpenAPI
+        """CatalogItemUpdateJobCreateQuery - a model defined in OpenAPI
 
         Args:
-            data (CatalogItemDeleteJobCreateQueryResourceObject):
+            data (CatalogItemUpdateJobCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_delete_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_delete_query_resource_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_job_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_update_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.catalog_item_update_job_create_query_resource_object import CatalogItemUpdateJobCreateQueryResourceObject
-    globals()['CatalogItemUpdateJobCreateQueryResourceObject'] = CatalogItemUpdateJobCreateQueryResourceObject
+    from openapi_client.model.catalog_item_update_query_resource_object import CatalogItemUpdateQueryResourceObject
+    globals()['CatalogItemUpdateQueryResourceObject'] = CatalogItemUpdateQueryResourceObject
 
 
-class CatalogItemUpdateJobCreateQuery(ModelNormal):
+class CatalogItemUpdateQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,15 +84,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (CatalogItemUpdateJobCreateQueryResourceObject,),  # noqa: E501
+            'data': (CatalogItemUpdateQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -104,18 +104,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """CatalogItemUpdateJobCreateQuery - a model defined in OpenAPI
+        """CatalogItemUpdateQuery - a model defined in OpenAPI
 
         Args:
-            data (CatalogItemUpdateJobCreateQueryResourceObject):
+            data (CatalogItemUpdateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -193,18 +193,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """CatalogItemUpdateJobCreateQuery - a model defined in OpenAPI
+        """CatalogItemUpdateQuery - a model defined in OpenAPI
 
         Args:
-            data (CatalogItemUpdateJobCreateQueryResourceObject):
+            data (CatalogItemUpdateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_job_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_update_job_create_query_resource_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_job_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_update_job_create_query_resource_object_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_update_query.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.catalog_item_update_query_resource_object import CatalogItemUpdateQueryResourceObject
-    globals()['CatalogItemUpdateQueryResourceObject'] = CatalogItemUpdateQueryResourceObject
+    from openapi_client.model.tag_update_query_resource_object import TagUpdateQueryResourceObject
+    globals()['TagUpdateQueryResourceObject'] = TagUpdateQueryResourceObject
 
 
-class CatalogItemUpdateQuery(ModelNormal):
+class TagUpdateQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,15 +84,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (CatalogItemUpdateQueryResourceObject,),  # noqa: E501
+            'data': (TagUpdateQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -104,18 +104,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """CatalogItemUpdateQuery - a model defined in OpenAPI
+        """TagUpdateQuery - a model defined in OpenAPI
 
         Args:
-            data (CatalogItemUpdateQueryResourceObject):
+            data (TagUpdateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -193,18 +193,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """CatalogItemUpdateQuery - a model defined in OpenAPI
+        """TagUpdateQuery - a model defined in OpenAPI
 
         Args:
-            data (CatalogItemUpdateQueryResourceObject):
+            data (TagUpdateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_update_query_resource_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_item_update_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_update_query_resource_object_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_bulk_create_job_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_bulk_create_job_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_bulk_delete_job_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_bulk_delete_job_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_bulk_update_job_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_bulk_update_job_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_job_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_create_job_create_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_create_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_create_query_resource_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_create_query_resource_object_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_delete_job_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_delete_job_create_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_delete_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_delete_query_resource_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_job_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_update_job_create_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_update_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_update_query_resource_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/catalog_variant_update_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_variant_update_query_resource_object_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/content_sub_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/content_sub_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/data_privacy_create_deletion_job_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/data_privacy_create_deletion_job_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/data_privacy_deletion_job_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/data_privacy_deletion_job_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/event_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/event_create_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/event_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/event_create_query_resource_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/event_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/event_create_query_resource_object_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/event_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/event_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/flow_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/flow_enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/flow_update_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/flow_update_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/flow_update_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/flow_update_query_resource_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/flow_update_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/flow_update_query_resource_object_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/get_create_variants_jobs5_xx_response.py` & `klaviyo-api-3.0.0/src/openapi_client/model/get_create_variants_jobs5_xx_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner.py` & `klaviyo-api-3.0.0/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner_source.py` & `klaviyo-api-3.0.0/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/list_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/list_create_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/list_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/list_create_query_resource_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/list_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/list_create_query_resource_object_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/list_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/list_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/list_members_add_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/list_members_add_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/list_members_add_query_data_inner.py` & `klaviyo-api-3.0.0/src/openapi_client/model/list_members_add_query_data_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/list_members_delete_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/list_members_delete_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/list_partial_update_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/list_partial_update_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/list_partial_update_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/list_partial_update_query_resource_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/metric_aggregate_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/metric_aggregate_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/metric_aggregate_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/metric_aggregate_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/metric_aggregate_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/metric_aggregate_query_resource_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/metric_aggregate_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/metric_aggregate_query_resource_object_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/metric_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/metric_create_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/onsite_profile_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/profile_create_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.onsite_profile_create_query_resource_object import OnsiteProfileCreateQueryResourceObject
-    globals()['OnsiteProfileCreateQueryResourceObject'] = OnsiteProfileCreateQueryResourceObject
+    from openapi_client.model.profile_create_query_resource_object import ProfileCreateQueryResourceObject
+    globals()['ProfileCreateQueryResourceObject'] = ProfileCreateQueryResourceObject
 
 
-class OnsiteProfileCreateQuery(ModelNormal):
+class ProfileCreateQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,15 +84,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (OnsiteProfileCreateQueryResourceObject,),  # noqa: E501
+            'data': (ProfileCreateQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -104,18 +104,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """OnsiteProfileCreateQuery - a model defined in OpenAPI
+        """ProfileCreateQuery - a model defined in OpenAPI
 
         Args:
-            data (OnsiteProfileCreateQueryResourceObject):
+            data (ProfileCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -193,18 +193,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """OnsiteProfileCreateQuery - a model defined in OpenAPI
+        """ProfileCreateQuery - a model defined in OpenAPI
 
         Args:
-            data (OnsiteProfileCreateQueryResourceObject):
+            data (ProfileCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/onsite_profile_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/profile_create_query_resource_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,21 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.onsite_profile_create_query_resource_object_attributes import OnsiteProfileCreateQueryResourceObjectAttributes
+    from openapi_client.model.profile_create_query_resource_object_attributes import ProfileCreateQueryResourceObjectAttributes
     from openapi_client.model.profile_enum import ProfileEnum
-    globals()['OnsiteProfileCreateQueryResourceObjectAttributes'] = OnsiteProfileCreateQueryResourceObjectAttributes
+    globals()['ProfileCreateQueryResourceObjectAttributes'] = ProfileCreateQueryResourceObjectAttributes
     globals()['ProfileEnum'] = ProfileEnum
 
 
-class OnsiteProfileCreateQueryResourceObject(ModelNormal):
+class ProfileCreateQueryResourceObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,15 +86,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (OnsiteProfileCreateQueryResourceObjectAttributes,),  # noqa: E501
+            'attributes': (ProfileCreateQueryResourceObjectAttributes,),  # noqa: E501
             'type': (ProfileEnum,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -108,18 +108,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, attributes, type, *args, **kwargs):  # noqa: E501
-        """OnsiteProfileCreateQueryResourceObject - a model defined in OpenAPI
+        """ProfileCreateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (OnsiteProfileCreateQueryResourceObjectAttributes):
+            attributes (ProfileCreateQueryResourceObjectAttributes):
             type (ProfileEnum):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -199,18 +199,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, attributes, type, *args, **kwargs):  # noqa: E501
-        """OnsiteProfileCreateQueryResourceObject - a model defined in OpenAPI
+        """ProfileCreateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (OnsiteProfileCreateQueryResourceObjectAttributes):
+            attributes (ProfileCreateQueryResourceObjectAttributes):
             type (ProfileEnum):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/onsite_profile_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/profile_partial_update_query_resource_object_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -31,15 +31,15 @@
 
 
 def lazy_import():
     from openapi_client.model.profile_location import ProfileLocation
     globals()['ProfileLocation'] = ProfileLocation
 
 
-class OnsiteProfileCreateQueryResourceObjectAttributes(ModelNormal):
+class ProfilePartialUpdateQueryResourceObjectAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -124,15 +124,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """OnsiteProfileCreateQueryResourceObjectAttributes - a model defined in OpenAPI
+        """ProfilePartialUpdateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -220,15 +220,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """OnsiteProfileCreateQueryResourceObjectAttributes - a model defined in OpenAPI
+        """ProfilePartialUpdateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/onsite_subscription_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/subscription_create_job_create_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.onsite_subscription_create_query_resource_object import OnsiteSubscriptionCreateQueryResourceObject
-    globals()['OnsiteSubscriptionCreateQueryResourceObject'] = OnsiteSubscriptionCreateQueryResourceObject
+    from openapi_client.model.subscription_create_job_create_query_resource_object import SubscriptionCreateJobCreateQueryResourceObject
+    globals()['SubscriptionCreateJobCreateQueryResourceObject'] = SubscriptionCreateJobCreateQueryResourceObject
 
 
-class OnsiteSubscriptionCreateQuery(ModelNormal):
+class SubscriptionCreateJobCreateQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,15 +84,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (OnsiteSubscriptionCreateQueryResourceObject,),  # noqa: E501
+            'data': (SubscriptionCreateJobCreateQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -104,18 +104,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """OnsiteSubscriptionCreateQuery - a model defined in OpenAPI
+        """SubscriptionCreateJobCreateQuery - a model defined in OpenAPI
 
         Args:
-            data (OnsiteSubscriptionCreateQueryResourceObject):
+            data (SubscriptionCreateJobCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -193,18 +193,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """OnsiteSubscriptionCreateQuery - a model defined in OpenAPI
+        """SubscriptionCreateJobCreateQuery - a model defined in OpenAPI
 
         Args:
-            data (OnsiteSubscriptionCreateQueryResourceObject):
+            data (SubscriptionCreateJobCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/onsite_subscription_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/suppression_create_job_create_query_resource_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,21 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.onsite_subscription_create_query_resource_object_attributes import OnsiteSubscriptionCreateQueryResourceObjectAttributes
-    from openapi_client.model.subscription_enum import SubscriptionEnum
-    globals()['OnsiteSubscriptionCreateQueryResourceObjectAttributes'] = OnsiteSubscriptionCreateQueryResourceObjectAttributes
-    globals()['SubscriptionEnum'] = SubscriptionEnum
+    from openapi_client.model.profile_suppression_bulk_create_job_enum import ProfileSuppressionBulkCreateJobEnum
+    from openapi_client.model.suppression_create_job_create_query_resource_object_attributes import SuppressionCreateJobCreateQueryResourceObjectAttributes
+    globals()['ProfileSuppressionBulkCreateJobEnum'] = ProfileSuppressionBulkCreateJobEnum
+    globals()['SuppressionCreateJobCreateQueryResourceObjectAttributes'] = SuppressionCreateJobCreateQueryResourceObjectAttributes
 
 
-class OnsiteSubscriptionCreateQueryResourceObject(ModelNormal):
+class SuppressionCreateJobCreateQueryResourceObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,16 +86,16 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (OnsiteSubscriptionCreateQueryResourceObjectAttributes,),  # noqa: E501
-            'type': (SubscriptionEnum,),  # noqa: E501
+            'attributes': (SuppressionCreateJobCreateQueryResourceObjectAttributes,),  # noqa: E501
+            'type': (ProfileSuppressionBulkCreateJobEnum,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -108,19 +108,19 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, attributes, type, *args, **kwargs):  # noqa: E501
-        """OnsiteSubscriptionCreateQueryResourceObject - a model defined in OpenAPI
+        """SuppressionCreateJobCreateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (OnsiteSubscriptionCreateQueryResourceObjectAttributes):
-            type (SubscriptionEnum):
+            attributes (SuppressionCreateJobCreateQueryResourceObjectAttributes):
+            type (ProfileSuppressionBulkCreateJobEnum):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -199,19 +199,19 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, attributes, type, *args, **kwargs):  # noqa: E501
-        """OnsiteSubscriptionCreateQueryResourceObject - a model defined in OpenAPI
+        """SuppressionCreateJobCreateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (OnsiteSubscriptionCreateQueryResourceObjectAttributes):
-            type (SubscriptionEnum):
+            attributes (SuppressionCreateJobCreateQueryResourceObjectAttributes):
+            type (ProfileSuppressionBulkCreateJobEnum):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/onsite_subscription_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/template_update_query_resource_object_attributes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class OnsiteSubscriptionCreateQueryResourceObjectAttributes(ModelNormal):
+class TemplateUpdateQueryResourceObjectAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,46 +78,41 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'list_id': (str, none_type,),  # noqa: E501
-            'phone_number': (str, none_type,),  # noqa: E501
-            'properties': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'email': (str, none_type,),  # noqa: E501
-            'custom_source': (str, none_type,),  # noqa: E501
+            'text': (str, none_type,),  # noqa: E501
+            'html': (str, none_type,),  # noqa: E501
+            'name': (str, none_type,),  # noqa: E501
+            'return_fields': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'list_id': 'list_id',  # noqa: E501
-        'phone_number': 'phone_number',  # noqa: E501
-        'properties': 'properties',  # noqa: E501
-        'email': 'email',  # noqa: E501
-        'custom_source': 'custom_source',  # noqa: E501
+        'text': 'text',  # noqa: E501
+        'html': 'html',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'return_fields': 'return_fields',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, list_id, *args, **kwargs):  # noqa: E501
-        """OnsiteSubscriptionCreateQueryResourceObjectAttributes - a model defined in OpenAPI
-
-        Args:
-            list_id (str, none_type): The list ID to add the newly subscribed profile to.
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """TemplateUpdateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,18 +137,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            phone_number (str, none_type): Phone number to create subscription and SMS consent record for, in E.164 format.. [optional]  # noqa: E501
-            properties ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Profile properties to set on the newly subscribed profile.. [optional]  # noqa: E501
-            email (str, none_type): Email address to create subscription and email consent record for.. [optional]  # noqa: E501
-            custom_source (str, none_type): A custom method detail or source to store on the consent records for this subscription.. [optional]  # noqa: E501
+            text (str, none_type): The plaintext of the template. [optional]  # noqa: E501
+            html (str, none_type): The HTML of the template. [optional]  # noqa: E501
+            name (str, none_type): The name of the template. [optional]  # noqa: E501
+            return_fields ([str]): Provide fields to limit the returned data. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -177,15 +172,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.list_id = list_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -198,19 +192,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, list_id, *args, **kwargs):  # noqa: E501
-        """OnsiteSubscriptionCreateQueryResourceObjectAttributes - a model defined in OpenAPI
-
-        Args:
-            list_id (str, none_type): The list ID to add the newly subscribed profile to.
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """TemplateUpdateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -235,18 +226,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            phone_number (str, none_type): Phone number to create subscription and SMS consent record for, in E.164 format.. [optional]  # noqa: E501
-            properties ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Profile properties to set on the newly subscribed profile.. [optional]  # noqa: E501
-            email (str, none_type): Email address to create subscription and email consent record for.. [optional]  # noqa: E501
-            custom_source (str, none_type): A custom method detail or source to store on the consent records for this subscription.. [optional]  # noqa: E501
+            text (str, none_type): The plaintext of the template. [optional]  # noqa: E501
+            html (str, none_type): The HTML of the template. [optional]  # noqa: E501
+            name (str, none_type): The name of the template. [optional]  # noqa: E501
+            return_fields ([str]): Provide fields to limit the returned data. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -268,15 +259,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.list_id = list_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/profile_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/suppression_create_job_create_query.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.profile_create_query_resource_object import ProfileCreateQueryResourceObject
-    globals()['ProfileCreateQueryResourceObject'] = ProfileCreateQueryResourceObject
+    from openapi_client.model.suppression_create_job_create_query_resource_object import SuppressionCreateJobCreateQueryResourceObject
+    globals()['SuppressionCreateJobCreateQueryResourceObject'] = SuppressionCreateJobCreateQueryResourceObject
 
 
-class ProfileCreateQuery(ModelNormal):
+class SuppressionCreateJobCreateQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,15 +84,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (ProfileCreateQueryResourceObject,),  # noqa: E501
+            'data': (SuppressionCreateJobCreateQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -104,18 +104,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """ProfileCreateQuery - a model defined in OpenAPI
+        """SuppressionCreateJobCreateQuery - a model defined in OpenAPI
 
         Args:
-            data (ProfileCreateQueryResourceObject):
+            data (SuppressionCreateJobCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -193,18 +193,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """ProfileCreateQuery - a model defined in OpenAPI
+        """SuppressionCreateJobCreateQuery - a model defined in OpenAPI
 
         Args:
-            data (ProfileCreateQueryResourceObject):
+            data (SuppressionCreateJobCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/profile_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_group_create_query_resource_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,21 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.profile_create_query_resource_object_attributes import ProfileCreateQueryResourceObjectAttributes
-    from openapi_client.model.profile_enum import ProfileEnum
-    globals()['ProfileCreateQueryResourceObjectAttributes'] = ProfileCreateQueryResourceObjectAttributes
-    globals()['ProfileEnum'] = ProfileEnum
+    from openapi_client.model.tag_group_create_query_resource_object_attributes import TagGroupCreateQueryResourceObjectAttributes
+    from openapi_client.model.tag_group_enum import TagGroupEnum
+    globals()['TagGroupCreateQueryResourceObjectAttributes'] = TagGroupCreateQueryResourceObjectAttributes
+    globals()['TagGroupEnum'] = TagGroupEnum
 
 
-class ProfileCreateQueryResourceObject(ModelNormal):
+class TagGroupCreateQueryResourceObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,16 +86,16 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (ProfileCreateQueryResourceObjectAttributes,),  # noqa: E501
-            'type': (ProfileEnum,),  # noqa: E501
+            'attributes': (TagGroupCreateQueryResourceObjectAttributes,),  # noqa: E501
+            'type': (TagGroupEnum,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -108,19 +108,19 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, attributes, type, *args, **kwargs):  # noqa: E501
-        """ProfileCreateQueryResourceObject - a model defined in OpenAPI
+        """TagGroupCreateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (ProfileCreateQueryResourceObjectAttributes):
-            type (ProfileEnum):
+            attributes (TagGroupCreateQueryResourceObjectAttributes):
+            type (TagGroupEnum):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -199,19 +199,19 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, attributes, type, *args, **kwargs):  # noqa: E501
-        """ProfileCreateQueryResourceObject - a model defined in OpenAPI
+        """TagGroupCreateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (ProfileCreateQueryResourceObjectAttributes):
-            type (ProfileEnum):
+            attributes (TagGroupCreateQueryResourceObjectAttributes):
+            type (TagGroupEnum):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/profile_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/profile_create_query_resource_object_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/profile_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/profile_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/profile_location.py` & `klaviyo-api-3.0.0/src/openapi_client/model/profile_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/profile_location_latitude.py` & `klaviyo-api-3.0.0/src/openapi_client/model/profile_location_latitude.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/profile_location_longitude.py` & `klaviyo-api-3.0.0/src/openapi_client/model/profile_location_longitude.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/profile_partial_update_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/profile_partial_update_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/profile_partial_update_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_group_update_query_resource_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,21 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.onsite_profile_create_query_resource_object_attributes import OnsiteProfileCreateQueryResourceObjectAttributes
-    from openapi_client.model.profile_enum import ProfileEnum
-    globals()['OnsiteProfileCreateQueryResourceObjectAttributes'] = OnsiteProfileCreateQueryResourceObjectAttributes
-    globals()['ProfileEnum'] = ProfileEnum
+    from openapi_client.model.tag_group_enum import TagGroupEnum
+    from openapi_client.model.tag_group_update_query_resource_object_attributes import TagGroupUpdateQueryResourceObjectAttributes
+    globals()['TagGroupEnum'] = TagGroupEnum
+    globals()['TagGroupUpdateQueryResourceObjectAttributes'] = TagGroupUpdateQueryResourceObjectAttributes
 
 
-class ProfilePartialUpdateQueryResourceObject(ModelNormal):
+class TagGroupUpdateQueryResourceObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,16 +86,16 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (OnsiteProfileCreateQueryResourceObjectAttributes,),  # noqa: E501
-            'type': (ProfileEnum,),  # noqa: E501
+            'attributes': (TagGroupUpdateQueryResourceObjectAttributes,),  # noqa: E501
+            'type': (TagGroupEnum,),  # noqa: E501
             'id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -110,20 +110,20 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, attributes, type, id, *args, **kwargs):  # noqa: E501
-        """ProfilePartialUpdateQueryResourceObject - a model defined in OpenAPI
+        """TagGroupUpdateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (OnsiteProfileCreateQueryResourceObjectAttributes):
-            type (ProfileEnum):
-            id (str): Primary key that uniquely identifies this profile. Generated by Klaviyo.
+            attributes (TagGroupUpdateQueryResourceObjectAttributes):
+            type (TagGroupEnum):
+            id (str): The Tag Group ID
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -203,20 +203,20 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, attributes, type, id, *args, **kwargs):  # noqa: E501
-        """ProfilePartialUpdateQueryResourceObject - a model defined in OpenAPI
+        """TagGroupUpdateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (OnsiteProfileCreateQueryResourceObjectAttributes):
-            type (ProfileEnum):
-            id (str): Primary key that uniquely identifies this profile. Generated by Klaviyo.
+            attributes (TagGroupUpdateQueryResourceObjectAttributes):
+            type (TagGroupEnum):
+            id (str): The Tag Group ID
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/profile_subscription_bulk_create_job_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/profile_subscription_bulk_create_job_enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/profile_suppression_bulk_create_job_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/profile_suppression_bulk_create_job_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/profile_unsubscription_bulk_create_job_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/profile_unsubscription_bulk_create_job_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/profile_unsuppression_bulk_create_job_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/profile_unsuppression_bulk_create_job_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/segment_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/segment_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/segment_partial_update_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/segment_partial_update_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/segment_partial_update_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/segment_partial_update_query_resource_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/segment_partial_update_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/segment_partial_update_query_resource_object_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/send_options_sub_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/send_options_sub_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/send_strategy_sub_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/send_strategy_sub_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/static_schedule_options.py` & `klaviyo-api-3.0.0/src/openapi_client/model/static_schedule_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/sto_schedule_options.py` & `klaviyo-api-3.0.0/src/openapi_client/model/sto_schedule_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/subscription.py` & `klaviyo-api-3.0.0/src/openapi_client/model/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/subscription_channels.py` & `klaviyo-api-3.0.0/src/openapi_client/model/subscription_channels.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/subscription_create_job_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/unsubscription_create_job_create_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.subscription_create_job_create_query_resource_object import SubscriptionCreateJobCreateQueryResourceObject
-    globals()['SubscriptionCreateJobCreateQueryResourceObject'] = SubscriptionCreateJobCreateQueryResourceObject
+    from openapi_client.model.unsubscription_create_job_create_query_resource_object import UnsubscriptionCreateJobCreateQueryResourceObject
+    globals()['UnsubscriptionCreateJobCreateQueryResourceObject'] = UnsubscriptionCreateJobCreateQueryResourceObject
 
 
-class SubscriptionCreateJobCreateQuery(ModelNormal):
+class UnsubscriptionCreateJobCreateQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,15 +84,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (SubscriptionCreateJobCreateQueryResourceObject,),  # noqa: E501
+            'data': (UnsubscriptionCreateJobCreateQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -104,18 +104,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """SubscriptionCreateJobCreateQuery - a model defined in OpenAPI
+        """UnsubscriptionCreateJobCreateQuery - a model defined in OpenAPI
 
         Args:
-            data (SubscriptionCreateJobCreateQueryResourceObject):
+            data (UnsubscriptionCreateJobCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -193,18 +193,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """SubscriptionCreateJobCreateQuery - a model defined in OpenAPI
+        """UnsubscriptionCreateJobCreateQuery - a model defined in OpenAPI
 
         Args:
-            data (SubscriptionCreateJobCreateQueryResourceObject):
+            data (UnsubscriptionCreateJobCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/subscription_create_job_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/subscription_create_job_create_query_resource_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/subscription_create_job_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/subscription_create_job_create_query_resource_object_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/subscription_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_enum.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class SubscriptionEnum(ModelSimple):
+class TagEnum(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,15 +49,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'SUBSCRIPTION': "subscription",
+            'TAG': "tag",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -96,23 +96,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """SubscriptionEnum - a model defined in OpenAPI
+        """TagEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "subscription", must be one of ["subscription", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "tag", must be one of ["tag", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "subscription", must be one of ["subscription", ]  # noqa: E501
+            value (str): if omitted defaults to "tag", must be one of ["tag", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -145,15 +145,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "subscription"
+            value = "tag"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -186,23 +186,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """SubscriptionEnum - a model defined in OpenAPI
+        """TagEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "subscription", must be one of ["subscription", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "tag", must be one of ["tag", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "subscription", must be one of ["subscription", ]  # noqa: E501
+            value (str): if omitted defaults to "tag", must be one of ["tag", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -237,15 +237,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "subscription"
+            value = "tag"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/suppression.py` & `klaviyo-api-3.0.0/src/openapi_client/model/suppression.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/suppression_create_job_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/unsuppression_create_job_create_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.suppression_create_job_create_query_resource_object import SuppressionCreateJobCreateQueryResourceObject
-    globals()['SuppressionCreateJobCreateQueryResourceObject'] = SuppressionCreateJobCreateQueryResourceObject
+    from openapi_client.model.unsuppression_create_job_create_query_resource_object import UnsuppressionCreateJobCreateQueryResourceObject
+    globals()['UnsuppressionCreateJobCreateQueryResourceObject'] = UnsuppressionCreateJobCreateQueryResourceObject
 
 
-class SuppressionCreateJobCreateQuery(ModelNormal):
+class UnsuppressionCreateJobCreateQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,15 +84,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (SuppressionCreateJobCreateQueryResourceObject,),  # noqa: E501
+            'data': (UnsuppressionCreateJobCreateQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -104,18 +104,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """SuppressionCreateJobCreateQuery - a model defined in OpenAPI
+        """UnsuppressionCreateJobCreateQuery - a model defined in OpenAPI
 
         Args:
-            data (SuppressionCreateJobCreateQueryResourceObject):
+            data (UnsuppressionCreateJobCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -193,18 +193,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """SuppressionCreateJobCreateQuery - a model defined in OpenAPI
+        """UnsuppressionCreateJobCreateQuery - a model defined in OpenAPI
 
         Args:
-            data (SuppressionCreateJobCreateQueryResourceObject):
+            data (UnsuppressionCreateJobCreateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/suppression_create_job_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/unsuppression_create_job_create_query_resource_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,21 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.profile_suppression_bulk_create_job_enum import ProfileSuppressionBulkCreateJobEnum
-    from openapi_client.model.suppression_create_job_create_query_resource_object_attributes import SuppressionCreateJobCreateQueryResourceObjectAttributes
-    globals()['ProfileSuppressionBulkCreateJobEnum'] = ProfileSuppressionBulkCreateJobEnum
-    globals()['SuppressionCreateJobCreateQueryResourceObjectAttributes'] = SuppressionCreateJobCreateQueryResourceObjectAttributes
+    from openapi_client.model.profile_unsuppression_bulk_create_job_enum import ProfileUnsuppressionBulkCreateJobEnum
+    from openapi_client.model.unsuppression_create_job_create_query_resource_object_attributes import UnsuppressionCreateJobCreateQueryResourceObjectAttributes
+    globals()['ProfileUnsuppressionBulkCreateJobEnum'] = ProfileUnsuppressionBulkCreateJobEnum
+    globals()['UnsuppressionCreateJobCreateQueryResourceObjectAttributes'] = UnsuppressionCreateJobCreateQueryResourceObjectAttributes
 
 
-class SuppressionCreateJobCreateQueryResourceObject(ModelNormal):
+class UnsuppressionCreateJobCreateQueryResourceObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,16 +86,16 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (SuppressionCreateJobCreateQueryResourceObjectAttributes,),  # noqa: E501
-            'type': (ProfileSuppressionBulkCreateJobEnum,),  # noqa: E501
+            'attributes': (UnsuppressionCreateJobCreateQueryResourceObjectAttributes,),  # noqa: E501
+            'type': (ProfileUnsuppressionBulkCreateJobEnum,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -108,19 +108,19 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, attributes, type, *args, **kwargs):  # noqa: E501
-        """SuppressionCreateJobCreateQueryResourceObject - a model defined in OpenAPI
+        """UnsuppressionCreateJobCreateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (SuppressionCreateJobCreateQueryResourceObjectAttributes):
-            type (ProfileSuppressionBulkCreateJobEnum):
+            attributes (UnsuppressionCreateJobCreateQueryResourceObjectAttributes):
+            type (ProfileUnsuppressionBulkCreateJobEnum):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -199,19 +199,19 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, attributes, type, *args, **kwargs):  # noqa: E501
-        """SuppressionCreateJobCreateQueryResourceObject - a model defined in OpenAPI
+        """UnsuppressionCreateJobCreateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (SuppressionCreateJobCreateQueryResourceObjectAttributes):
-            type (ProfileSuppressionBulkCreateJobEnum):
+            attributes (UnsuppressionCreateJobCreateQueryResourceObjectAttributes):
+            type (ProfileUnsuppressionBulkCreateJobEnum):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/suppression_create_job_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/suppression_create_job_create_query_resource_object_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_campaign_op.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_campaign_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_campaign_op_data_inner.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_campaign_op_data_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_create_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_create_query_resource_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_create_query_resource_object_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_group_enum.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class TagEnum(ModelSimple):
+class TagGroupEnum(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,15 +49,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'TAG': "tag",
+            'TAG-GROUP': "tag-group",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -96,23 +96,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """TagEnum - a model defined in OpenAPI
+        """TagGroupEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "tag", must be one of ["tag", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "tag-group", must be one of ["tag-group", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "tag", must be one of ["tag", ]  # noqa: E501
+            value (str): if omitted defaults to "tag-group", must be one of ["tag-group", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -145,15 +145,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "tag"
+            value = "tag-group"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -186,23 +186,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """TagEnum - a model defined in OpenAPI
+        """TagGroupEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "tag", must be one of ["tag", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "tag-group", must be one of ["tag-group", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "tag", must be one of ["tag", ]  # noqa: E501
+            value (str): if omitted defaults to "tag-group", must be one of ["tag-group", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -237,15 +237,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "tag"
+            value = "tag-group"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_flow_op.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_flow_op.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_flow_op_data_inner.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_flow_op_data_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_group_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_group_create_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_group_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_update_query_resource_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,21 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.tag_group_create_query_resource_object_attributes import TagGroupCreateQueryResourceObjectAttributes
-    from openapi_client.model.tag_group_enum import TagGroupEnum
-    globals()['TagGroupCreateQueryResourceObjectAttributes'] = TagGroupCreateQueryResourceObjectAttributes
-    globals()['TagGroupEnum'] = TagGroupEnum
+    from openapi_client.model.tag_enum import TagEnum
+    from openapi_client.model.tag_update_query_resource_object_attributes import TagUpdateQueryResourceObjectAttributes
+    globals()['TagEnum'] = TagEnum
+    globals()['TagUpdateQueryResourceObjectAttributes'] = TagUpdateQueryResourceObjectAttributes
 
 
-class TagGroupCreateQueryResourceObject(ModelNormal):
+class TagUpdateQueryResourceObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,41 +86,44 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (TagGroupCreateQueryResourceObjectAttributes,),  # noqa: E501
-            'type': (TagGroupEnum,),  # noqa: E501
+            'attributes': (TagUpdateQueryResourceObjectAttributes,),  # noqa: E501
+            'type': (TagEnum,),  # noqa: E501
+            'id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'attributes': 'attributes',  # noqa: E501
         'type': 'type',  # noqa: E501
+        'id': 'id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, attributes, type, *args, **kwargs):  # noqa: E501
-        """TagGroupCreateQueryResourceObject - a model defined in OpenAPI
+    def _from_openapi_data(cls, attributes, type, id, *args, **kwargs):  # noqa: E501
+        """TagUpdateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (TagGroupCreateQueryResourceObjectAttributes):
-            type (TagGroupEnum):
+            attributes (TagUpdateQueryResourceObjectAttributes):
+            type (TagEnum):
+            id (str): The Tag ID
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -178,14 +181,15 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.attributes = attributes
         self.type = type
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -198,20 +202,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, attributes, type, *args, **kwargs):  # noqa: E501
-        """TagGroupCreateQueryResourceObject - a model defined in OpenAPI
+    def __init__(self, attributes, type, id, *args, **kwargs):  # noqa: E501
+        """TagUpdateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (TagGroupCreateQueryResourceObjectAttributes):
-            type (TagGroupEnum):
+            attributes (TagUpdateQueryResourceObjectAttributes):
+            type (TagEnum):
+            id (str): The Tag ID
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -267,14 +272,15 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.attributes = attributes
         self.type = type
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_group_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_group_create_query_resource_object_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_group_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/template_enum.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class TagGroupEnum(ModelSimple):
+class TemplateEnum(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,15 +49,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'TAG-GROUP': "tag-group",
+            'TEMPLATE': "template",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -96,23 +96,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """TagGroupEnum - a model defined in OpenAPI
+        """TemplateEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "tag-group", must be one of ["tag-group", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "template", must be one of ["template", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "tag-group", must be one of ["tag-group", ]  # noqa: E501
+            value (str): if omitted defaults to "template", must be one of ["template", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -145,15 +145,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "tag-group"
+            value = "template"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -186,23 +186,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """TagGroupEnum - a model defined in OpenAPI
+        """TemplateEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "tag-group", must be one of ["tag-group", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "template", must be one of ["template", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "tag-group", must be one of ["tag-group", ]  # noqa: E501
+            value (str): if omitted defaults to "template", must be one of ["template", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -237,15 +237,15 @@
 
         if 'value' in kwargs:
             value = kwargs.pop('value')
         elif args:
             args = list(args)
             value = args.pop(0)
         else:
-            value = "tag-group"
+            value = "template"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_group_update_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_group_update_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_group_update_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/template_clone_query_resource_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,21 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.tag_group_enum import TagGroupEnum
-    from openapi_client.model.tag_group_update_query_resource_object_attributes import TagGroupUpdateQueryResourceObjectAttributes
-    globals()['TagGroupEnum'] = TagGroupEnum
-    globals()['TagGroupUpdateQueryResourceObjectAttributes'] = TagGroupUpdateQueryResourceObjectAttributes
+    from openapi_client.model.template_clone_query_resource_object_attributes import TemplateCloneQueryResourceObjectAttributes
+    from openapi_client.model.template_enum import TemplateEnum
+    globals()['TemplateCloneQueryResourceObjectAttributes'] = TemplateCloneQueryResourceObjectAttributes
+    globals()['TemplateEnum'] = TemplateEnum
 
 
-class TagGroupUpdateQueryResourceObject(ModelNormal):
+class TemplateCloneQueryResourceObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,44 +86,41 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (TagGroupUpdateQueryResourceObjectAttributes,),  # noqa: E501
-            'type': (TagGroupEnum,),  # noqa: E501
-            'id': (str,),  # noqa: E501
+            'attributes': (TemplateCloneQueryResourceObjectAttributes,),  # noqa: E501
+            'type': (TemplateEnum,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'attributes': 'attributes',  # noqa: E501
         'type': 'type',  # noqa: E501
-        'id': 'id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, attributes, type, id, *args, **kwargs):  # noqa: E501
-        """TagGroupUpdateQueryResourceObject - a model defined in OpenAPI
+    def _from_openapi_data(cls, attributes, type, *args, **kwargs):  # noqa: E501
+        """TemplateCloneQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (TagGroupUpdateQueryResourceObjectAttributes):
-            type (TagGroupEnum):
-            id (str): The Tag Group ID
+            attributes (TemplateCloneQueryResourceObjectAttributes):
+            type (TemplateEnum):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -181,15 +178,14 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.attributes = attributes
         self.type = type
-        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -202,21 +198,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, attributes, type, id, *args, **kwargs):  # noqa: E501
-        """TagGroupUpdateQueryResourceObject - a model defined in OpenAPI
+    def __init__(self, attributes, type, *args, **kwargs):  # noqa: E501
+        """TemplateCloneQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (TagGroupUpdateQueryResourceObjectAttributes):
-            type (TagGroupEnum):
-            id (str): The Tag Group ID
+            attributes (TemplateCloneQueryResourceObjectAttributes):
+            type (TemplateEnum):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -272,15 +267,14 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.attributes = attributes
         self.type = type
-        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_group_update_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_group_update_query_resource_object_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_list_op.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_list_op.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_list_op_data_inner.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_list_op_data_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_segment_op.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_segment_op.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_segment_op_data_inner.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_segment_op_data_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_update_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/template_clone_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.tag_update_query_resource_object import TagUpdateQueryResourceObject
-    globals()['TagUpdateQueryResourceObject'] = TagUpdateQueryResourceObject
+    from openapi_client.model.template_clone_query_resource_object import TemplateCloneQueryResourceObject
+    globals()['TemplateCloneQueryResourceObject'] = TemplateCloneQueryResourceObject
 
 
-class TagUpdateQuery(ModelNormal):
+class TemplateCloneQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,15 +84,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (TagUpdateQueryResourceObject,),  # noqa: E501
+            'data': (TemplateCloneQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -104,18 +104,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """TagUpdateQuery - a model defined in OpenAPI
+        """TemplateCloneQuery - a model defined in OpenAPI
 
         Args:
-            data (TagUpdateQueryResourceObject):
+            data (TemplateCloneQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -193,18 +193,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """TagUpdateQuery - a model defined in OpenAPI
+        """TemplateCloneQuery - a model defined in OpenAPI
 
         Args:
-            data (TagUpdateQueryResourceObject):
+            data (TemplateCloneQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_update_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/template_create_query_resource_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,21 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.tag_enum import TagEnum
-    from openapi_client.model.tag_update_query_resource_object_attributes import TagUpdateQueryResourceObjectAttributes
-    globals()['TagEnum'] = TagEnum
-    globals()['TagUpdateQueryResourceObjectAttributes'] = TagUpdateQueryResourceObjectAttributes
+    from openapi_client.model.template_create_query_resource_object_attributes import TemplateCreateQueryResourceObjectAttributes
+    from openapi_client.model.template_enum import TemplateEnum
+    globals()['TemplateCreateQueryResourceObjectAttributes'] = TemplateCreateQueryResourceObjectAttributes
+    globals()['TemplateEnum'] = TemplateEnum
 
 
-class TagUpdateQueryResourceObject(ModelNormal):
+class TemplateCreateQueryResourceObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,44 +86,41 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (TagUpdateQueryResourceObjectAttributes,),  # noqa: E501
-            'type': (TagEnum,),  # noqa: E501
-            'id': (str,),  # noqa: E501
+            'attributes': (TemplateCreateQueryResourceObjectAttributes,),  # noqa: E501
+            'type': (TemplateEnum,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'attributes': 'attributes',  # noqa: E501
         'type': 'type',  # noqa: E501
-        'id': 'id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, attributes, type, id, *args, **kwargs):  # noqa: E501
-        """TagUpdateQueryResourceObject - a model defined in OpenAPI
+    def _from_openapi_data(cls, attributes, type, *args, **kwargs):  # noqa: E501
+        """TemplateCreateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (TagUpdateQueryResourceObjectAttributes):
-            type (TagEnum):
-            id (str): The Tag ID
+            attributes (TemplateCreateQueryResourceObjectAttributes):
+            type (TemplateEnum):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -181,15 +178,14 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.attributes = attributes
         self.type = type
-        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -202,21 +198,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, attributes, type, id, *args, **kwargs):  # noqa: E501
-        """TagUpdateQueryResourceObject - a model defined in OpenAPI
+    def __init__(self, attributes, type, *args, **kwargs):  # noqa: E501
+        """TemplateCreateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (TagUpdateQueryResourceObjectAttributes):
-            type (TagEnum):
-            id (str): The Tag ID
+            attributes (TemplateCreateQueryResourceObjectAttributes):
+            type (TemplateEnum):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -272,15 +267,14 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.attributes = attributes
         self.type = type
-        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tag_update_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tag_update_query_resource_object_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/template_clone_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/template_update_query.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.template_clone_query_resource_object import TemplateCloneQueryResourceObject
-    globals()['TemplateCloneQueryResourceObject'] = TemplateCloneQueryResourceObject
+    from openapi_client.model.template_update_query_resource_object import TemplateUpdateQueryResourceObject
+    globals()['TemplateUpdateQueryResourceObject'] = TemplateUpdateQueryResourceObject
 
 
-class TemplateCloneQuery(ModelNormal):
+class TemplateUpdateQuery(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,15 +84,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (TemplateCloneQueryResourceObject,),  # noqa: E501
+            'data': (TemplateUpdateQueryResourceObject,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -104,18 +104,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """TemplateCloneQuery - a model defined in OpenAPI
+        """TemplateUpdateQuery - a model defined in OpenAPI
 
         Args:
-            data (TemplateCloneQueryResourceObject):
+            data (TemplateUpdateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -193,18 +193,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """TemplateCloneQuery - a model defined in OpenAPI
+        """TemplateUpdateQuery - a model defined in OpenAPI
 
         Args:
-            data (TemplateCloneQueryResourceObject):
+            data (TemplateUpdateQueryResourceObject):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/template_clone_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/template_update_query_resource_object.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,21 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.template_clone_query_resource_object_attributes import TemplateCloneQueryResourceObjectAttributes
     from openapi_client.model.template_enum import TemplateEnum
-    globals()['TemplateCloneQueryResourceObjectAttributes'] = TemplateCloneQueryResourceObjectAttributes
+    from openapi_client.model.template_update_query_resource_object_attributes import TemplateUpdateQueryResourceObjectAttributes
     globals()['TemplateEnum'] = TemplateEnum
+    globals()['TemplateUpdateQueryResourceObjectAttributes'] = TemplateUpdateQueryResourceObjectAttributes
 
 
-class TemplateCloneQueryResourceObject(ModelNormal):
+class TemplateUpdateQueryResourceObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,41 +86,44 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (TemplateCloneQueryResourceObjectAttributes,),  # noqa: E501
+            'attributes': (TemplateUpdateQueryResourceObjectAttributes,),  # noqa: E501
             'type': (TemplateEnum,),  # noqa: E501
+            'id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'attributes': 'attributes',  # noqa: E501
         'type': 'type',  # noqa: E501
+        'id': 'id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, attributes, type, *args, **kwargs):  # noqa: E501
-        """TemplateCloneQueryResourceObject - a model defined in OpenAPI
+    def _from_openapi_data(cls, attributes, type, id, *args, **kwargs):  # noqa: E501
+        """TemplateUpdateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (TemplateCloneQueryResourceObjectAttributes):
+            attributes (TemplateUpdateQueryResourceObjectAttributes):
             type (TemplateEnum):
+            id (str): The ID of template
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -178,14 +181,15 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.attributes = attributes
         self.type = type
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -198,20 +202,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, attributes, type, *args, **kwargs):  # noqa: E501
-        """TemplateCloneQueryResourceObject - a model defined in OpenAPI
+    def __init__(self, attributes, type, id, *args, **kwargs):  # noqa: E501
+        """TemplateUpdateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (TemplateCloneQueryResourceObjectAttributes):
+            attributes (TemplateUpdateQueryResourceObjectAttributes):
             type (TemplateEnum):
+            id (str): The ID of template
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -267,14 +272,15 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.attributes = attributes
         self.type = type
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/template_clone_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/template_clone_query_resource_object_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/template_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/template_create_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/template_create_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/template_render_query_resource_object_attributes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -26,22 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from openapi_client.model.template_create_query_resource_object_attributes import TemplateCreateQueryResourceObjectAttributes
-    from openapi_client.model.template_enum import TemplateEnum
-    globals()['TemplateCreateQueryResourceObjectAttributes'] = TemplateCreateQueryResourceObjectAttributes
-    globals()['TemplateEnum'] = TemplateEnum
 
-
-class TemplateCreateQueryResourceObject(ModelNormal):
+class TemplateRenderQueryResourceObjectAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -69,58 +63,58 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'attributes': (TemplateCreateQueryResourceObjectAttributes,),  # noqa: E501
-            'type': (TemplateEnum,),  # noqa: E501
+            'id': (str, none_type,),  # noqa: E501
+            'context': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'return_fields': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'attributes': 'attributes',  # noqa: E501
-        'type': 'type',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'context': 'context',  # noqa: E501
+        'return_fields': 'return_fields',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, attributes, type, *args, **kwargs):  # noqa: E501
-        """TemplateCreateQueryResourceObject - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, context, *args, **kwargs):  # noqa: E501
+        """TemplateRenderQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            attributes (TemplateCreateQueryResourceObjectAttributes):
-            type (TemplateEnum):
+            id (str, none_type): The ID of template
+            context ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): The context for the template render. This must be a JSON object which has values for any tags used in the template. See [this doc](https://help.klaviyo.com/hc/en-us/articles/115005084927-Template-tags-and-variable-syntax-reference-classic-editor-) for more details.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -145,14 +139,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            return_fields ([str]): Provide fields to limit the returned data. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -176,16 +171,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.attributes = attributes
-        self.type = type
+        self.id = id
+        self.context = context
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -198,20 +193,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, attributes, type, *args, **kwargs):  # noqa: E501
-        """TemplateCreateQueryResourceObject - a model defined in OpenAPI
+    def __init__(self, id, context, *args, **kwargs):  # noqa: E501
+        """TemplateRenderQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            attributes (TemplateCreateQueryResourceObjectAttributes):
-            type (TemplateEnum):
+            id (str, none_type): The ID of template
+            context ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): The context for the template render. This must be a JSON object which has values for any tags used in the template. See [this doc](https://help.klaviyo.com/hc/en-us/articles/115005084927-Template-tags-and-variable-syntax-reference-classic-editor-) for more details.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -236,14 +231,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            return_fields ([str]): Provide fields to limit the returned data. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -265,16 +261,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.attributes = attributes
-        self.type = type
+        self.id = id
+        self.context = context
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/template_create_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/template_create_query_resource_object_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/template_enum.py` & `klaviyo-api-3.0.0/src/openapi_client/model/catalog_item_category_op.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -26,93 +26,98 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from openapi_client.model.catalog_item_category_op_data_inner import CatalogItemCategoryOpDataInner
+    globals()['CatalogItemCategoryOpDataInner'] = CatalogItemCategoryOpDataInner
 
-class TemplateEnum(ModelSimple):
+
+class CatalogItemCategoryOp(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
       validations (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('value',): {
-            'TEMPLATE': "template",
-        },
     }
 
     validations = {
     }
 
-    additional_properties_type = None
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        lazy_import()
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'value': (str,),
+            'data': ([CatalogItemCategoryOpDataInner],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
-    attribute_map = {}
-
-    read_only_vars = set()
+    attribute_map = {
+        'data': 'data',  # noqa: E501
+    }
 
-    _composed_schemas = None
+    read_only_vars = {
+    }
 
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
+    _composed_schemas = {}
 
+    @classmethod
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):
-        """TemplateEnum - a model defined in OpenAPI
-
-        Note that value can be passed either in args or in kwargs, but not in both.
+    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
+        """CatalogItemCategoryOp - a model defined in OpenAPI
 
         Args:
-            args[0] (str): if omitted defaults to "template", must be one of ["template", ]  # noqa: E501
+            data ([CatalogItemCategoryOpDataInner]):
 
         Keyword Args:
-            value (str): if omitted defaults to "template", must be one of ["template", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -136,30 +141,23 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            value = "template"
 
         _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
+        self = super(OpenApiModel, cls).__new__(cls)
+
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
                 else:
                     raise ApiTypeError(
                         "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
@@ -172,37 +170,43 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):
-        """TemplateEnum - a model defined in OpenAPI
+        self.data = data
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
 
-        Note that value can be passed either in args or in kwargs, but not in both.
+    @convert_js_args_to_python_args
+    def __init__(self, data, *args, **kwargs):  # noqa: E501
+        """CatalogItemCategoryOp - a model defined in OpenAPI
 
         Args:
-            args[0] (str): if omitted defaults to "template", must be one of ["template", ]  # noqa: E501
+            data ([CatalogItemCategoryOpDataInner]):
 
         Keyword Args:
-            value (str): if omitted defaults to "template", must be one of ["template", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -226,29 +230,18 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
-        # required up here when default value is not given
-        _path_to_item = kwargs.pop('_path_to_item', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if 'value' in kwargs:
-            value = kwargs.pop('value')
-        elif args:
-            args = list(args)
-            value = args.pop(0)
-        else:
-            value = "template"
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
@@ -264,19 +257,20 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-        self.value = value
-        if kwargs:
-            raise ApiTypeError(
-                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
-                    kwargs,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
 
-        return self
+        self.data = data
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/template_render_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/template_render_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/template_render_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/template_render_query_resource_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/template_render_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/unsubscription_create_job_create_query_resource_object.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -26,16 +26,22 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from openapi_client.model.profile_unsubscription_bulk_create_job_enum import ProfileUnsubscriptionBulkCreateJobEnum
+    from openapi_client.model.unsubscription_create_job_create_query_resource_object_attributes import UnsubscriptionCreateJobCreateQueryResourceObjectAttributes
+    globals()['ProfileUnsubscriptionBulkCreateJobEnum'] = ProfileUnsubscriptionBulkCreateJobEnum
+    globals()['UnsubscriptionCreateJobCreateQueryResourceObjectAttributes'] = UnsubscriptionCreateJobCreateQueryResourceObjectAttributes
 
-class TemplateRenderQueryResourceObjectAttributes(ModelNormal):
+
+class UnsubscriptionCreateJobCreateQueryResourceObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,58 +69,58 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'id': (str, none_type,),  # noqa: E501
-            'context': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'return_fields': ([str],),  # noqa: E501
+            'attributes': (UnsubscriptionCreateJobCreateQueryResourceObjectAttributes,),  # noqa: E501
+            'type': (ProfileUnsubscriptionBulkCreateJobEnum,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'context': 'context',  # noqa: E501
-        'return_fields': 'return_fields',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
+        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, context, *args, **kwargs):  # noqa: E501
-        """TemplateRenderQueryResourceObjectAttributes - a model defined in OpenAPI
+    def _from_openapi_data(cls, attributes, type, *args, **kwargs):  # noqa: E501
+        """UnsubscriptionCreateJobCreateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            id (str, none_type): The ID of template
-            context ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): The context for the template render. This must be a JSON object which has values for any tags used in the template. See [this doc](https://help.klaviyo.com/hc/en-us/articles/115005084927-Template-tags-and-variable-syntax-reference-classic-editor-) for more details.
+            attributes (UnsubscriptionCreateJobCreateQueryResourceObjectAttributes):
+            type (ProfileUnsubscriptionBulkCreateJobEnum):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,15 +145,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            return_fields ([str]): Provide fields to limit the returned data. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -171,16 +176,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.context = context
+        self.attributes = attributes
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -193,20 +198,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, context, *args, **kwargs):  # noqa: E501
-        """TemplateRenderQueryResourceObjectAttributes - a model defined in OpenAPI
+    def __init__(self, attributes, type, *args, **kwargs):  # noqa: E501
+        """UnsubscriptionCreateJobCreateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            id (str, none_type): The ID of template
-            context ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): The context for the template render. This must be a JSON object which has values for any tags used in the template. See [this doc](https://help.klaviyo.com/hc/en-us/articles/115005084927-Template-tags-and-variable-syntax-reference-classic-editor-) for more details.
+            attributes (UnsubscriptionCreateJobCreateQueryResourceObjectAttributes):
+            type (ProfileUnsubscriptionBulkCreateJobEnum):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -231,15 +236,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            return_fields ([str]): Provide fields to limit the returned data. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -261,16 +265,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.context = context
+        self.attributes = attributes
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/template_update_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/unsuppression_create_job_create_query_resource_object_attributes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.template_update_query_resource_object import TemplateUpdateQueryResourceObject
-    globals()['TemplateUpdateQueryResourceObject'] = TemplateUpdateQueryResourceObject
+    from openapi_client.model.suppression import Suppression
+    globals()['Suppression'] = Suppression
 
 
-class TemplateUpdateQuery(ModelNormal):
+class UnsuppressionCreateJobCreateQueryResourceObjectAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,38 +84,38 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (TemplateUpdateQueryResourceObject,),  # noqa: E501
+            'suppressions': ([Suppression],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'suppressions': 'suppressions',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """TemplateUpdateQuery - a model defined in OpenAPI
+    def _from_openapi_data(cls, suppressions, *args, **kwargs):  # noqa: E501
+        """UnsuppressionCreateJobCreateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            data (TemplateUpdateQueryResourceObject):
+            suppressions ([Suppression]): One or more suppressions to be removed.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -171,15 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
+        self.suppressions = suppressions
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,19 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """TemplateUpdateQuery - a model defined in OpenAPI
+    def __init__(self, suppressions, *args, **kwargs):  # noqa: E501
+        """UnsuppressionCreateJobCreateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Args:
-            data (TemplateUpdateQueryResourceObject):
+            suppressions ([Suppression]): One or more suppressions to be removed.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -258,15 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
+        self.suppressions = suppressions
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/template_update_query_resource_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/profile_partial_update_query_resource_object.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,21 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from openapi_client.model.template_enum import TemplateEnum
-    from openapi_client.model.template_update_query_resource_object_attributes import TemplateUpdateQueryResourceObjectAttributes
-    globals()['TemplateEnum'] = TemplateEnum
-    globals()['TemplateUpdateQueryResourceObjectAttributes'] = TemplateUpdateQueryResourceObjectAttributes
+    from openapi_client.model.profile_enum import ProfileEnum
+    from openapi_client.model.profile_partial_update_query_resource_object_attributes import ProfilePartialUpdateQueryResourceObjectAttributes
+    globals()['ProfileEnum'] = ProfileEnum
+    globals()['ProfilePartialUpdateQueryResourceObjectAttributes'] = ProfilePartialUpdateQueryResourceObjectAttributes
 
 
-class TemplateUpdateQueryResourceObject(ModelNormal):
+class ProfilePartialUpdateQueryResourceObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,16 +86,16 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (TemplateUpdateQueryResourceObjectAttributes,),  # noqa: E501
-            'type': (TemplateEnum,),  # noqa: E501
+            'attributes': (ProfilePartialUpdateQueryResourceObjectAttributes,),  # noqa: E501
+            'type': (ProfileEnum,),  # noqa: E501
             'id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -110,20 +110,20 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, attributes, type, id, *args, **kwargs):  # noqa: E501
-        """TemplateUpdateQueryResourceObject - a model defined in OpenAPI
+        """ProfilePartialUpdateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (TemplateUpdateQueryResourceObjectAttributes):
-            type (TemplateEnum):
-            id (str): The ID of template
+            attributes (ProfilePartialUpdateQueryResourceObjectAttributes):
+            type (ProfileEnum):
+            id (str): Primary key that uniquely identifies this profile. Generated by Klaviyo.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -203,20 +203,20 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, attributes, type, id, *args, **kwargs):  # noqa: E501
-        """TemplateUpdateQueryResourceObject - a model defined in OpenAPI
+        """ProfilePartialUpdateQueryResourceObject - a model defined in OpenAPI
 
         Args:
-            attributes (TemplateUpdateQueryResourceObjectAttributes):
-            type (TemplateEnum):
-            id (str): The ID of template
+            attributes (ProfilePartialUpdateQueryResourceObjectAttributes):
+            type (ProfileEnum):
+            id (str): Primary key that uniquely identifies this profile. Generated by Klaviyo.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/template_update_query_resource_object_attributes.py` & `klaviyo-api-3.0.0/src/openapi_client/model/throttled_schedule_options.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class TemplateUpdateQueryResourceObjectAttributes(ModelNormal):
+class ThrottledScheduleOptions(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,41 +78,41 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'text': (str, none_type,),  # noqa: E501
-            'html': (str, none_type,),  # noqa: E501
-            'name': (str, none_type,),  # noqa: E501
-            'return_fields': ([str],),  # noqa: E501
+            'throttle_percentage': (int,),  # noqa: E501
+            'datetime': (datetime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'text': 'text',  # noqa: E501
-        'html': 'html',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'return_fields': 'return_fields',  # noqa: E501
+        'throttle_percentage': 'throttle_percentage',  # noqa: E501
+        'datetime': 'datetime',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TemplateUpdateQueryResourceObjectAttributes - a model defined in OpenAPI
+    def _from_openapi_data(cls, throttle_percentage, datetime, *args, **kwargs):  # noqa: E501
+        """ThrottledScheduleOptions - a model defined in OpenAPI
+
+        Args:
+            throttle_percentage (int): The percentage of recipients per hour to send to. Allowed values: [10, 11, 13, 14, 17, 20, 25, 33, 50]
+            datetime (datetime): The time to send at
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,18 +137,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            text (str, none_type): The plaintext of the template. [optional]  # noqa: E501
-            html (str, none_type): The HTML of the template. [optional]  # noqa: E501
-            name (str, none_type): The name of the template. [optional]  # noqa: E501
-            return_fields ([str]): Provide fields to limit the returned data. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -172,14 +168,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.throttle_percentage = throttle_percentage
+        self.datetime = datetime
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,16 +190,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """TemplateUpdateQueryResourceObjectAttributes - a model defined in OpenAPI
+    def __init__(self, throttle_percentage, datetime, *args, **kwargs):  # noqa: E501
+        """ThrottledScheduleOptions - a model defined in OpenAPI
+
+        Args:
+            throttle_percentage (int): The percentage of recipients per hour to send to. Allowed values: [10, 11, 13, 14, 17, 20, 25, 33, 50]
+            datetime (datetime): The time to send at
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,18 +228,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            text (str, none_type): The plaintext of the template. [optional]  # noqa: E501
-            html (str, none_type): The HTML of the template. [optional]  # noqa: E501
-            name (str, none_type): The name of the template. [optional]  # noqa: E501
-            return_fields ([str]): Provide fields to limit the returned data. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -259,14 +257,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.throttle_percentage = throttle_percentage
+        self.datetime = datetime
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/throttled_schedule_options.py` & `klaviyo-api-3.0.0/src/openapi_client/model/unsubscription_create_job_create_query_resource_object_attributes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
 
-class ThrottledScheduleOptions(ModelNormal):
+class UnsubscriptionCreateJobCreateQueryResourceObjectAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,41 +78,39 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'throttle_percentage': (int,),  # noqa: E501
-            'datetime': (datetime,),  # noqa: E501
+            'phone_numbers': ([str],),  # noqa: E501
+            'emails': ([str],),  # noqa: E501
+            'list_id': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'throttle_percentage': 'throttle_percentage',  # noqa: E501
-        'datetime': 'datetime',  # noqa: E501
+        'phone_numbers': 'phone_numbers',  # noqa: E501
+        'emails': 'emails',  # noqa: E501
+        'list_id': 'list_id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, throttle_percentage, datetime, *args, **kwargs):  # noqa: E501
-        """ThrottledScheduleOptions - a model defined in OpenAPI
-
-        Args:
-            throttle_percentage (int): The percentage of recipients per hour to send to. Allowed values: [10, 11, 13, 14, 17, 20, 25, 33, 50]
-            datetime (datetime): The time to send at
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """UnsubscriptionCreateJobCreateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,14 +135,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            phone_numbers ([str]): The phone numbers to unsubscribe if any.. [optional]  # noqa: E501
+            emails ([str]): The emails to unsubscribe if any.. [optional]  # noqa: E501
+            list_id (str, none_type): Optional, the list to remove the profiles from. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -168,16 +169,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.throttle_percentage = throttle_percentage
-        self.datetime = datetime
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -190,20 +189,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, throttle_percentage, datetime, *args, **kwargs):  # noqa: E501
-        """ThrottledScheduleOptions - a model defined in OpenAPI
-
-        Args:
-            throttle_percentage (int): The percentage of recipients per hour to send to. Allowed values: [10, 11, 13, 14, 17, 20, 25, 33, 50]
-            datetime (datetime): The time to send at
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """UnsubscriptionCreateJobCreateQueryResourceObjectAttributes - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,14 +223,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            phone_numbers ([str]): The phone numbers to unsubscribe if any.. [optional]  # noqa: E501
+            emails ([str]): The emails to unsubscribe if any.. [optional]  # noqa: E501
+            list_id (str, none_type): Optional, the list to remove the profiles from. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -257,16 +255,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.throttle_percentage = throttle_percentage
-        self.datetime = datetime
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/tracking_options_sub_object.py` & `klaviyo-api-3.0.0/src/openapi_client/model/tracking_options_sub_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model/unsubscription_create_job_create_query.py` & `klaviyo-api-3.0.0/src/openapi_client/model/utm_params_sub_object.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from openapi_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from openapi_client.model.unsubscription_create_job_create_query_resource_object import UnsubscriptionCreateJobCreateQueryResourceObject
-    globals()['UnsubscriptionCreateJobCreateQueryResourceObject'] = UnsubscriptionCreateJobCreateQueryResourceObject
 
-
-class UnsubscriptionCreateJobCreateQuery(ModelNormal):
+class UTMParamsSubObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,55 +63,56 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'data': (UnsubscriptionCreateJobCreateQueryResourceObject,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'value': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """UnsubscriptionCreateJobCreateQuery - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, value, *args, **kwargs):  # noqa: E501
+        """UTMParamsSubObject - a model defined in OpenAPI
 
         Args:
-            data (UnsubscriptionCreateJobCreateQueryResourceObject):
+            name (str): Name of the UTM param
+            value (str): Value of the UTM param. Can be templated data.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -171,15 +168,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
+        self.name = name
+        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,19 +190,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """UnsubscriptionCreateJobCreateQuery - a model defined in OpenAPI
+    def __init__(self, name, value, *args, **kwargs):  # noqa: E501
+        """UTMParamsSubObject - a model defined in OpenAPI
 
         Args:
-            data (UnsubscriptionCreateJobCreateQueryResourceObject):
+            name (str): Name of the UTM param
+            value (str): Value of the UTM param. Can be templated data.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -258,15 +257,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
+        self.name = name
+        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/model_utils.py` & `klaviyo-api-3.0.0/src/openapi_client/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/models/__init__.py` & `klaviyo-api-3.0.0/src/openapi_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,23 +62,23 @@
 from openapi_client.model.catalog_category_update_query_resource_object_relationships import CatalogCategoryUpdateQueryResourceObjectRelationships
 from openapi_client.model.catalog_category_update_query_resource_object_relationships_items import CatalogCategoryUpdateQueryResourceObjectRelationshipsItems
 from openapi_client.model.catalog_category_update_query_resource_object_relationships_items_data_inner import CatalogCategoryUpdateQueryResourceObjectRelationshipsItemsDataInner
 from openapi_client.model.catalog_item_bulk_create_job_enum import CatalogItemBulkCreateJobEnum
 from openapi_client.model.catalog_item_bulk_delete_job_enum import CatalogItemBulkDeleteJobEnum
 from openapi_client.model.catalog_item_bulk_update_job_enum import CatalogItemBulkUpdateJobEnum
 from openapi_client.model.catalog_item_category_op import CatalogItemCategoryOp
+from openapi_client.model.catalog_item_category_op_data_inner import CatalogItemCategoryOpDataInner
 from openapi_client.model.catalog_item_create_job_create_query import CatalogItemCreateJobCreateQuery
 from openapi_client.model.catalog_item_create_job_create_query_resource_object import CatalogItemCreateJobCreateQueryResourceObject
 from openapi_client.model.catalog_item_create_job_create_query_resource_object_attributes import CatalogItemCreateJobCreateQueryResourceObjectAttributes
 from openapi_client.model.catalog_item_create_query import CatalogItemCreateQuery
 from openapi_client.model.catalog_item_create_query_resource_object import CatalogItemCreateQueryResourceObject
 from openapi_client.model.catalog_item_create_query_resource_object_attributes import CatalogItemCreateQueryResourceObjectAttributes
 from openapi_client.model.catalog_item_create_query_resource_object_relationships import CatalogItemCreateQueryResourceObjectRelationships
 from openapi_client.model.catalog_item_create_query_resource_object_relationships_categories import CatalogItemCreateQueryResourceObjectRelationshipsCategories
-from openapi_client.model.catalog_item_create_query_resource_object_relationships_categories_data_inner import CatalogItemCreateQueryResourceObjectRelationshipsCategoriesDataInner
 from openapi_client.model.catalog_item_delete_job_create_query import CatalogItemDeleteJobCreateQuery
 from openapi_client.model.catalog_item_delete_job_create_query_resource_object import CatalogItemDeleteJobCreateQueryResourceObject
 from openapi_client.model.catalog_item_delete_job_create_query_resource_object_attributes import CatalogItemDeleteJobCreateQueryResourceObjectAttributes
 from openapi_client.model.catalog_item_delete_query_resource_object import CatalogItemDeleteQueryResourceObject
 from openapi_client.model.catalog_item_enum import CatalogItemEnum
 from openapi_client.model.catalog_item_update_job_create_query import CatalogItemUpdateJobCreateQuery
 from openapi_client.model.catalog_item_update_job_create_query_resource_object import CatalogItemUpdateJobCreateQueryResourceObject
@@ -132,29 +132,24 @@
 from openapi_client.model.list_partial_update_query import ListPartialUpdateQuery
 from openapi_client.model.list_partial_update_query_resource_object import ListPartialUpdateQueryResourceObject
 from openapi_client.model.metric_aggregate_enum import MetricAggregateEnum
 from openapi_client.model.metric_aggregate_query import MetricAggregateQuery
 from openapi_client.model.metric_aggregate_query_resource_object import MetricAggregateQueryResourceObject
 from openapi_client.model.metric_aggregate_query_resource_object_attributes import MetricAggregateQueryResourceObjectAttributes
 from openapi_client.model.metric_create_query import MetricCreateQuery
-from openapi_client.model.onsite_profile_create_query import OnsiteProfileCreateQuery
-from openapi_client.model.onsite_profile_create_query_resource_object import OnsiteProfileCreateQueryResourceObject
-from openapi_client.model.onsite_profile_create_query_resource_object_attributes import OnsiteProfileCreateQueryResourceObjectAttributes
-from openapi_client.model.onsite_subscription_create_query import OnsiteSubscriptionCreateQuery
-from openapi_client.model.onsite_subscription_create_query_resource_object import OnsiteSubscriptionCreateQueryResourceObject
-from openapi_client.model.onsite_subscription_create_query_resource_object_attributes import OnsiteSubscriptionCreateQueryResourceObjectAttributes
 from openapi_client.model.profile_create_query import ProfileCreateQuery
 from openapi_client.model.profile_create_query_resource_object import ProfileCreateQueryResourceObject
 from openapi_client.model.profile_create_query_resource_object_attributes import ProfileCreateQueryResourceObjectAttributes
 from openapi_client.model.profile_enum import ProfileEnum
 from openapi_client.model.profile_location import ProfileLocation
 from openapi_client.model.profile_location_latitude import ProfileLocationLatitude
 from openapi_client.model.profile_location_longitude import ProfileLocationLongitude
 from openapi_client.model.profile_partial_update_query import ProfilePartialUpdateQuery
 from openapi_client.model.profile_partial_update_query_resource_object import ProfilePartialUpdateQueryResourceObject
+from openapi_client.model.profile_partial_update_query_resource_object_attributes import ProfilePartialUpdateQueryResourceObjectAttributes
 from openapi_client.model.profile_subscription_bulk_create_job_enum import ProfileSubscriptionBulkCreateJobEnum
 from openapi_client.model.profile_suppression_bulk_create_job_enum import ProfileSuppressionBulkCreateJobEnum
 from openapi_client.model.profile_unsubscription_bulk_create_job_enum import ProfileUnsubscriptionBulkCreateJobEnum
 from openapi_client.model.profile_unsuppression_bulk_create_job_enum import ProfileUnsuppressionBulkCreateJobEnum
 from openapi_client.model.sto_schedule_options import STOScheduleOptions
 from openapi_client.model.segment_enum import SegmentEnum
 from openapi_client.model.segment_partial_update_query import SegmentPartialUpdateQuery
@@ -164,15 +159,14 @@
 from openapi_client.model.send_strategy_sub_object import SendStrategySubObject
 from openapi_client.model.static_schedule_options import StaticScheduleOptions
 from openapi_client.model.subscription import Subscription
 from openapi_client.model.subscription_channels import SubscriptionChannels
 from openapi_client.model.subscription_create_job_create_query import SubscriptionCreateJobCreateQuery
 from openapi_client.model.subscription_create_job_create_query_resource_object import SubscriptionCreateJobCreateQueryResourceObject
 from openapi_client.model.subscription_create_job_create_query_resource_object_attributes import SubscriptionCreateJobCreateQueryResourceObjectAttributes
-from openapi_client.model.subscription_enum import SubscriptionEnum
 from openapi_client.model.suppression import Suppression
 from openapi_client.model.suppression_create_job_create_query import SuppressionCreateJobCreateQuery
 from openapi_client.model.suppression_create_job_create_query_resource_object import SuppressionCreateJobCreateQueryResourceObject
 from openapi_client.model.suppression_create_job_create_query_resource_object_attributes import SuppressionCreateJobCreateQueryResourceObjectAttributes
 from openapi_client.model.tag_campaign_op import TagCampaignOp
 from openapi_client.model.tag_campaign_op_data_inner import TagCampaignOpDataInner
 from openapi_client.model.tag_create_query import TagCreateQuery
```

### Comparing `klaviyo-api-2.0.2/src/openapi_client/rest.py` & `klaviyo-api-3.0.0/src/openapi_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Klaviyo API
 
     The Klaviyo REST API. Please visit https://developers.klaviyo.com for more details.  # noqa: E501
 
-    The version of the OpenAPI document: 2023-02-22
+    The version of the OpenAPI document: 2023-06-15
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
```

