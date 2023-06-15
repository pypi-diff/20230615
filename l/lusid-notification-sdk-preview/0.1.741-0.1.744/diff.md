# Comparing `tmp/lusid-notification-sdk-preview-0.1.741.tar.gz` & `tmp/lusid-notification-sdk-preview-0.1.744.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.741.tar", last modified: Tue Jun 13 10:34:59 2023, max compression
+gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.744.tar", last modified: Thu Jun 15 15:28:47 2023, max compression
```

## Comparing `lusid-notification-sdk-preview-0.1.741.tar` & `lusid-notification-sdk-preview-0.1.744.tar`

### file list

```diff
@@ -1,68 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      379 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8040 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/
--rw-r--r--   0 root         (0) root         (0)     4452 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/api/
--rw-r--r--   0 root         (0) root         (0)      506 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6847 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    10519 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/api/deliveries_api.py
--rw-r--r--   0 root         (0) root         (0)    13984 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/api/event_types_api.py
--rw-r--r--   0 root         (0) root         (0)     7820 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/api/manual_event_api.py
--rw-r--r--   0 root         (0) root         (0)    52797 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/api/notifications_api.py
--rw-r--r--   0 root         (0) root         (0)    47803 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/api/subscriptions_api.py
--rw-r--r--   0 root         (0) root         (0)    27431 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16631 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/
--rw-r--r--   0 root         (0) root         (0)     3100 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7254 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     9017 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7231 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)    10957 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/amazon_sqs_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     9234 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/api_request_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     6508 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/attempt.py
--rw-r--r--   0 root         (0) root         (0)     5556 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/attempt_status.py
--rw-r--r--   0 root         (0) root         (0)    11191 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/create_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    12413 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/create_subscription.py
--rw-r--r--   0 root         (0) root         (0)    12390 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/delivery.py
--rw-r--r--   0 root         (0) root         (0)    14935 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/email_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    11110 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     8021 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9510 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     6425 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9539 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10704 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     5086 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/manual_event.py
--rw-r--r--   0 root         (0) root         (0)     7863 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/manual_event_body.py
--rw-r--r--   0 root         (0) root         (0)     6827 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/manual_event_header.py
--rw-r--r--   0 root         (0) root         (0)     4162 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/manual_event_request.py
--rw-r--r--   0 root         (0) root         (0)     7436 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    16373 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/notification.py
--rw-r--r--   0 root         (0) root         (0)     5154 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/notification_status.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7768 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7320 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_list_of_delivery.py
--rw-r--r--   0 root         (0) root         (0)     7516 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_list_of_event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     7432 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_list_of_notification.py
--rw-r--r--   0 root         (0) root         (0)     7432 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_list_of_subscription.py
--rw-r--r--   0 root         (0) root         (0)     8012 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/sms_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    15856 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)     9020 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/update_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    11551 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/update_subscription.py
--rw-r--r--   0 root         (0) root         (0)    15803 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/models/webhook_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    13560 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/utilities/
--rw-r--r--   0 root         (0) root         (0)       64 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      379 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2734 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/lusid_notification_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 10:34:59.000000 lusid-notification-sdk-preview-0.1.741/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2327 2023-06-13 10:32:53.000000 lusid-notification-sdk-preview-0.1.741/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 15:28:47.000000 lusid-notification-sdk-preview-0.1.744/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      379 2023-06-15 15:28:47.000000 lusid-notification-sdk-preview-0.1.744/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7722 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 15:28:47.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 15:28:47.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/api/
+-rw-r--r--   0 root         (0) root         (0)      442 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6847 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    13984 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/api/event_types_api.py
+-rw-r--r--   0 root         (0) root         (0)     7820 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/api/manual_event_api.py
+-rw-r--r--   0 root         (0) root         (0)    52797 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/api/notifications_api.py
+-rw-r--r--   0 root         (0) root         (0)    47803 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/api/subscriptions_api.py
+-rw-r--r--   0 root         (0) root         (0)    27431 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16631 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 15:28:47.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7254 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     9017 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7231 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)    10957 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/amazon_sqs_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     9234 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/api_request_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    11191 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/create_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    12413 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/create_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    14935 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/email_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    11110 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     8021 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9510 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6425 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9539 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10704 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     5086 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/manual_event.py
+-rw-r--r--   0 root         (0) root         (0)     7863 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/manual_event_body.py
+-rw-r--r--   0 root         (0) root         (0)     6827 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/manual_event_header.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/manual_event_request.py
+-rw-r--r--   0 root         (0) root         (0)     7436 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    16373 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)     5154 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/notification_status.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7768 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7516 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/resource_list_of_event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     7432 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/resource_list_of_notification.py
+-rw-r--r--   0 root         (0) root         (0)     7432 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/resource_list_of_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8012 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/sms_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    15856 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     9020 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/update_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    11551 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/update_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    15803 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/models/webhook_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    13560 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 15:28:47.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/utilities/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 15:28:47.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      379 2023-06-15 15:28:47.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-06-15 15:28:47.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 15:28:47.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-06-15 15:28:47.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-15 15:28:47.000000 lusid-notification-sdk-preview-0.1.744/lusid_notification_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 15:28:47.000000 lusid-notification-sdk-preview-0.1.744/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-06-15 15:28:04.000000 lusid-notification-sdk-preview-0.1.744/setup.py
```

### Comparing `lusid-notification-sdk-preview-0.1.741/README.md` & `lusid-notification-sdk-preview-0.1.744/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-notification-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.741
-- Package version: 0.1.741
+- API version: 0.1.744
+- Package version: 0.1.744
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -88,15 +88,14 @@
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://www.lusid.com/notification*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
-*DeliveriesApi* | [**list_deliveries**](docs/DeliveriesApi.md#list_deliveries) | **GET** /api/deliveries | [EXPERIMENTAL] ListDeliveries: List Deliveries
 *EventTypesApi* | [**get_event_type**](docs/EventTypesApi.md#get_event_type) | **GET** /api/eventtypes/{eventType} | [EXPERIMENTAL] GetEventType: Gets the specified event type schema.
 *EventTypesApi* | [**list_event_types**](docs/EventTypesApi.md#list_event_types) | **GET** /api/eventtypes | [EXPERIMENTAL] ListEventTypes: Lists all of the available event types.
 *ManualEventApi* | [**trigger_manual_event**](docs/ManualEventApi.md#trigger_manual_event) | **POST** /api/manualevent | [EXPERIMENTAL] TriggerManualEvent: Trigger a manual event.
 *NotificationsApi* | [**create_notification**](docs/NotificationsApi.md#create_notification) | **POST** /api/subscriptions/{scope}/{code}/notifications | [EXPERIMENTAL] CreateNotification: Add a Notification to a Subscription.
 *NotificationsApi* | [**delete_notification**](docs/NotificationsApi.md#delete_notification) | **DELETE** /api/subscriptions/{scope}/{code}/notifications/{id} | [EXPERIMENTAL] DeleteNotification: Delete a notification for a given subscription.
 *NotificationsApi* | [**get_notification**](docs/NotificationsApi.md#get_notification) | **GET** /api/subscriptions/{scope}/{code}/notifications/{id} | [EXPERIMENTAL] GetNotification: Get a notification on a subscription.
 *NotificationsApi* | [**list_notifications**](docs/NotificationsApi.md#list_notifications) | **GET** /api/subscriptions/{scope}/{code}/notifications | [EXPERIMENTAL] ListNotifications: List all notifications on a subscription.
@@ -111,19 +110,16 @@
 ## Documentation For Models
 
  - [AccessControlledAction](docs/AccessControlledAction.md)
  - [AccessControlledResource](docs/AccessControlledResource.md)
  - [ActionId](docs/ActionId.md)
  - [AmazonSqsNotificationType](docs/AmazonSqsNotificationType.md)
  - [ApiRequestNotificationType](docs/ApiRequestNotificationType.md)
- - [Attempt](docs/Attempt.md)
- - [AttemptStatus](docs/AttemptStatus.md)
  - [CreateNotificationRequest](docs/CreateNotificationRequest.md)
  - [CreateSubscription](docs/CreateSubscription.md)
- - [Delivery](docs/Delivery.md)
  - [EmailNotificationType](docs/EmailNotificationType.md)
  - [EventTypeSchema](docs/EventTypeSchema.md)
  - [IdSelectorDefinition](docs/IdSelectorDefinition.md)
  - [IdentifierPartSchema](docs/IdentifierPartSchema.md)
  - [Link](docs/Link.md)
  - [LusidProblemDetails](docs/LusidProblemDetails.md)
  - [LusidValidationProblemDetails](docs/LusidValidationProblemDetails.md)
@@ -132,15 +128,14 @@
  - [ManualEventHeader](docs/ManualEventHeader.md)
  - [ManualEventRequest](docs/ManualEventRequest.md)
  - [MatchingPattern](docs/MatchingPattern.md)
  - [Notification](docs/Notification.md)
  - [NotificationStatus](docs/NotificationStatus.md)
  - [ResourceId](docs/ResourceId.md)
  - [ResourceListOfAccessControlledResource](docs/ResourceListOfAccessControlledResource.md)
- - [ResourceListOfDelivery](docs/ResourceListOfDelivery.md)
  - [ResourceListOfEventTypeSchema](docs/ResourceListOfEventTypeSchema.md)
  - [ResourceListOfNotification](docs/ResourceListOfNotification.md)
  - [ResourceListOfSubscription](docs/ResourceListOfSubscription.md)
  - [SmsNotificationType](docs/SmsNotificationType.md)
  - [Subscription](docs/Subscription.md)
  - [UpdateNotificationRequest](docs/UpdateNotificationRequest.md)
  - [UpdateSubscription](docs/UpdateSubscription.md)
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/__init__.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 # flake8: noqa
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.741"
+__version__ = "0.1.744"
 
 # import apis into sdk package
 from lusid_notification.api.application_metadata_api import ApplicationMetadataApi
-from lusid_notification.api.deliveries_api import DeliveriesApi
 from lusid_notification.api.event_types_api import EventTypesApi
 from lusid_notification.api.manual_event_api import ManualEventApi
 from lusid_notification.api.notifications_api import NotificationsApi
 from lusid_notification.api.subscriptions_api import SubscriptionsApi
 
 # import ApiClient
 from lusid_notification.api_client import ApiClient
@@ -35,19 +34,16 @@
 from lusid_notification.exceptions import ApiException
 # import models into sdk package
 from lusid_notification.models.access_controlled_action import AccessControlledAction
 from lusid_notification.models.access_controlled_resource import AccessControlledResource
 from lusid_notification.models.action_id import ActionId
 from lusid_notification.models.amazon_sqs_notification_type import AmazonSqsNotificationType
 from lusid_notification.models.api_request_notification_type import ApiRequestNotificationType
-from lusid_notification.models.attempt import Attempt
-from lusid_notification.models.attempt_status import AttemptStatus
 from lusid_notification.models.create_notification_request import CreateNotificationRequest
 from lusid_notification.models.create_subscription import CreateSubscription
-from lusid_notification.models.delivery import Delivery
 from lusid_notification.models.email_notification_type import EmailNotificationType
 from lusid_notification.models.event_type_schema import EventTypeSchema
 from lusid_notification.models.id_selector_definition import IdSelectorDefinition
 from lusid_notification.models.identifier_part_schema import IdentifierPartSchema
 from lusid_notification.models.link import Link
 from lusid_notification.models.lusid_problem_details import LusidProblemDetails
 from lusid_notification.models.lusid_validation_problem_details import LusidValidationProblemDetails
@@ -56,15 +52,14 @@
 from lusid_notification.models.manual_event_header import ManualEventHeader
 from lusid_notification.models.manual_event_request import ManualEventRequest
 from lusid_notification.models.matching_pattern import MatchingPattern
 from lusid_notification.models.notification import Notification
 from lusid_notification.models.notification_status import NotificationStatus
 from lusid_notification.models.resource_id import ResourceId
 from lusid_notification.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
-from lusid_notification.models.resource_list_of_delivery import ResourceListOfDelivery
 from lusid_notification.models.resource_list_of_event_type_schema import ResourceListOfEventTypeSchema
 from lusid_notification.models.resource_list_of_notification import ResourceListOfNotification
 from lusid_notification.models.resource_list_of_subscription import ResourceListOfSubscription
 from lusid_notification.models.sms_notification_type import SmsNotificationType
 from lusid_notification.models.subscription import Subscription
 from lusid_notification.models.update_notification_request import UpdateNotificationRequest
 from lusid_notification.models.update_subscription import UpdateSubscription
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/api/application_metadata_api.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/api/application_metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.741'
+        header_params['X-LUSID-SDK-Version'] = '0.1.744'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/api/event_types_api.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/api/event_types_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -160,15 +160,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.741'
+        header_params['X-LUSID-SDK-Version'] = '0.1.744'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "EventTypeSchema",
             400: "LusidValidationProblemDetails",
@@ -292,15 +292,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.741'
+        header_params['X-LUSID-SDK-Version'] = '0.1.744'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfEventTypeSchema",
             404: "str",
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/api/manual_event_api.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/api/manual_event_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -155,15 +155,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.741'
+        header_params['X-LUSID-SDK-Version'] = '0.1.744'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "ManualEvent",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/api/notifications_api.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/api/notifications_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -195,15 +195,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.741'
+        header_params['X-LUSID-SDK-Version'] = '0.1.744'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -375,15 +375,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.741'
+        header_params['X-LUSID-SDK-Version'] = '0.1.744'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -552,15 +552,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.741'
+        header_params['X-LUSID-SDK-Version'] = '0.1.744'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -722,15 +722,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.741'
+        header_params['X-LUSID-SDK-Version'] = '0.1.744'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfNotification",
             400: "LusidValidationProblemDetails",
@@ -925,15 +925,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.741'
+        header_params['X-LUSID-SDK-Version'] = '0.1.744'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/api/subscriptions_api.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/api/subscriptions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -157,15 +157,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.741'
+        header_params['X-LUSID-SDK-Version'] = '0.1.744'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -326,15 +326,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.741'
+        header_params['X-LUSID-SDK-Version'] = '0.1.744'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -492,15 +492,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.741'
+        header_params['X-LUSID-SDK-Version'] = '0.1.744'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -680,15 +680,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.741'
+        header_params['X-LUSID-SDK-Version'] = '0.1.744'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfSubscription",
             400: "LusidValidationProblemDetails",
@@ -863,15 +863,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.741'
+        header_params['X-LUSID-SDK-Version'] = '0.1.744'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/api_client.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.741/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.744/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/configuration.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.741\n"\
-               "SDK Package Version: 0.1.741".\
+               "Version of the API: 0.1.744\n"\
+               "SDK Package Version: 0.1.744".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/exceptions.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/__init__.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,33 +2,30 @@
 
 # flake8: noqa
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
 from lusid_notification.models.access_controlled_action import AccessControlledAction
 from lusid_notification.models.access_controlled_resource import AccessControlledResource
 from lusid_notification.models.action_id import ActionId
 from lusid_notification.models.amazon_sqs_notification_type import AmazonSqsNotificationType
 from lusid_notification.models.api_request_notification_type import ApiRequestNotificationType
-from lusid_notification.models.attempt import Attempt
-from lusid_notification.models.attempt_status import AttemptStatus
 from lusid_notification.models.create_notification_request import CreateNotificationRequest
 from lusid_notification.models.create_subscription import CreateSubscription
-from lusid_notification.models.delivery import Delivery
 from lusid_notification.models.email_notification_type import EmailNotificationType
 from lusid_notification.models.event_type_schema import EventTypeSchema
 from lusid_notification.models.id_selector_definition import IdSelectorDefinition
 from lusid_notification.models.identifier_part_schema import IdentifierPartSchema
 from lusid_notification.models.link import Link
 from lusid_notification.models.lusid_problem_details import LusidProblemDetails
 from lusid_notification.models.lusid_validation_problem_details import LusidValidationProblemDetails
@@ -37,15 +34,14 @@
 from lusid_notification.models.manual_event_header import ManualEventHeader
 from lusid_notification.models.manual_event_request import ManualEventRequest
 from lusid_notification.models.matching_pattern import MatchingPattern
 from lusid_notification.models.notification import Notification
 from lusid_notification.models.notification_status import NotificationStatus
 from lusid_notification.models.resource_id import ResourceId
 from lusid_notification.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
-from lusid_notification.models.resource_list_of_delivery import ResourceListOfDelivery
 from lusid_notification.models.resource_list_of_event_type_schema import ResourceListOfEventTypeSchema
 from lusid_notification.models.resource_list_of_notification import ResourceListOfNotification
 from lusid_notification.models.resource_list_of_subscription import ResourceListOfSubscription
 from lusid_notification.models.sms_notification_type import SmsNotificationType
 from lusid_notification.models.subscription import Subscription
 from lusid_notification.models.update_notification_request import UpdateNotificationRequest
 from lusid_notification.models.update_subscription import UpdateSubscription
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/access_controlled_action.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/access_controlled_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/action_id.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/action_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/amazon_sqs_notification_type.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/amazon_sqs_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/api_request_notification_type.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/api_request_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/attempt_status.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/link.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_notification.configuration import Configuration
 
 
-class AttemptStatus(object):
+class Link(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,98 +35,151 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'result': 'str',
-        'detailed_message': 'str'
+        'relation': 'str',
+        'href': 'str',
+        'description': 'str',
+        'method': 'str'
     }
 
     attribute_map = {
-        'result': 'result',
-        'detailed_message': 'detailedMessage'
+        'relation': 'relation',
+        'href': 'href',
+        'description': 'description',
+        'method': 'method'
     }
 
     required_map = {
-        'result': 'required',
-        'detailed_message': 'optional'
+        'relation': 'required',
+        'href': 'required',
+        'description': 'optional',
+        'method': 'required'
     }
 
-    def __init__(self, result=None, detailed_message=None, local_vars_configuration=None):  # noqa: E501
-        """AttemptStatus - a model defined in OpenAPI"
+    def __init__(self, relation=None, href=None, description=None, method=None, local_vars_configuration=None):  # noqa: E501
+        """Link - a model defined in OpenAPI"
         
-        :param result:  Result of the delivery. (required)
-        :type result: str
-        :param detailed_message:  The detailed message from attempting to deliver the message.
-        :type detailed_message: str
+        :param relation:  (required)
+        :type relation: str
+        :param href:  (required)
+        :type href: str
+        :param description: 
+        :type description: str
+        :param method:  (required)
+        :type method: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._result = None
-        self._detailed_message = None
+        self._relation = None
+        self._href = None
+        self._description = None
+        self._method = None
         self.discriminator = None
 
-        self.result = result
-        self.detailed_message = detailed_message
+        self.relation = relation
+        self.href = href
+        self.description = description
+        self.method = method
 
     @property
-    def result(self):
-        """Gets the result of this AttemptStatus.  # noqa: E501
+    def relation(self):
+        """Gets the relation of this Link.  # noqa: E501
 
-        Result of the delivery.  # noqa: E501
 
-        :return: The result of this AttemptStatus.  # noqa: E501
+        :return: The relation of this Link.  # noqa: E501
         :rtype: str
         """
-        return self._result
+        return self._relation
 
-    @result.setter
-    def result(self, result):
-        """Sets the result of this AttemptStatus.
+    @relation.setter
+    def relation(self, relation):
+        """Sets the relation of this Link.
 
-        Result of the delivery.  # noqa: E501
 
-        :param result: The result of this AttemptStatus.  # noqa: E501
-        :type result: str
+        :param relation: The relation of this Link.  # noqa: E501
+        :type relation: str
         """
-        if self.local_vars_configuration.client_side_validation and result is None:  # noqa: E501
-            raise ValueError("Invalid value for `result`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                result is not None and len(result) < 1):
-            raise ValueError("Invalid value for `result`, length must be greater than or equal to `1`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and relation is None:  # noqa: E501
+            raise ValueError("Invalid value for `relation`, must not be `None`")  # noqa: E501
 
-        self._result = result
+        self._relation = relation
 
     @property
-    def detailed_message(self):
-        """Gets the detailed_message of this AttemptStatus.  # noqa: E501
+    def href(self):
+        """Gets the href of this Link.  # noqa: E501
 
-        The detailed message from attempting to deliver the message.  # noqa: E501
 
-        :return: The detailed_message of this AttemptStatus.  # noqa: E501
+        :return: The href of this Link.  # noqa: E501
         :rtype: str
         """
-        return self._detailed_message
+        return self._href
 
-    @detailed_message.setter
-    def detailed_message(self, detailed_message):
-        """Sets the detailed_message of this AttemptStatus.
+    @href.setter
+    def href(self, href):
+        """Sets the href of this Link.
 
-        The detailed message from attempting to deliver the message.  # noqa: E501
 
-        :param detailed_message: The detailed_message of this AttemptStatus.  # noqa: E501
-        :type detailed_message: str
+        :param href: The href of this Link.  # noqa: E501
+        :type href: str
         """
+        if self.local_vars_configuration.client_side_validation and href is None:  # noqa: E501
+            raise ValueError("Invalid value for `href`, must not be `None`")  # noqa: E501
 
-        self._detailed_message = detailed_message
+        self._href = href
+
+    @property
+    def description(self):
+        """Gets the description of this Link.  # noqa: E501
+
+
+        :return: The description of this Link.  # noqa: E501
+        :rtype: str
+        """
+        return self._description
+
+    @description.setter
+    def description(self, description):
+        """Sets the description of this Link.
+
+
+        :param description: The description of this Link.  # noqa: E501
+        :type description: str
+        """
+
+        self._description = description
+
+    @property
+    def method(self):
+        """Gets the method of this Link.  # noqa: E501
+
+
+        :return: The method of this Link.  # noqa: E501
+        :rtype: str
+        """
+        return self._method
+
+    @method.setter
+    def method(self, method):
+        """Sets the method of this Link.
+
+
+        :param method: The method of this Link.  # noqa: E501
+        :type method: str
+        """
+        if self.local_vars_configuration.client_side_validation and method is None:  # noqa: E501
+            raise ValueError("Invalid value for `method`, must not be `None`")  # noqa: E501
+
+        self._method = method
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -162,18 +215,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, AttemptStatus):
+        if not isinstance(other, Link):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, AttemptStatus):
+        if not isinstance(other, Link):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/create_notification_request.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/create_notification_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/create_subscription.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/create_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/email_notification_type.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/email_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/event_type_schema.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/id_selector_definition.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/id_selector_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/identifier_part_schema.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/identifier_part_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/lusid_problem_details.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/lusid_validation_problem_details.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/lusid_validation_problem_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/manual_event.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/manual_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/manual_event_body.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/manual_event_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/manual_event_header.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/manual_event_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/manual_event_request.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/manual_event_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/matching_pattern.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/matching_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/notification.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/notification_status.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/notification_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_id.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/resource_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_list_of_access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/resource_list_of_access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_list_of_delivery.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/resource_list_of_event_type_schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_notification.configuration import Configuration
 
 
-class ResourceListOfDelivery(object):
+class ResourceListOfEventTypeSchema(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,15 +35,15 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'values': 'list[Delivery]',
+        'values': 'list[EventTypeSchema]',
         'href': 'str',
         'links': 'list[Link]',
         'next_page': 'str',
         'previous_page': 'str'
     }
 
     attribute_map = {
@@ -59,18 +59,18 @@
         'href': 'optional',
         'links': 'optional',
         'next_page': 'optional',
         'previous_page': 'optional'
     }
 
     def __init__(self, values=None, href=None, links=None, next_page=None, previous_page=None, local_vars_configuration=None):  # noqa: E501
-        """ResourceListOfDelivery - a model defined in OpenAPI"
+        """ResourceListOfEventTypeSchema - a model defined in OpenAPI"
         
         :param values:  (required)
-        :type values: list[lusid_notification.Delivery]
+        :type values: list[lusid_notification.EventTypeSchema]
         :param href: 
         :type href: str
         :param links: 
         :type links: list[lusid_notification.Link]
         :param next_page: 
         :type next_page: str
         :param previous_page: 
@@ -92,114 +92,114 @@
         self.href = href
         self.links = links
         self.next_page = next_page
         self.previous_page = previous_page
 
     @property
     def values(self):
-        """Gets the values of this ResourceListOfDelivery.  # noqa: E501
+        """Gets the values of this ResourceListOfEventTypeSchema.  # noqa: E501
 
 
-        :return: The values of this ResourceListOfDelivery.  # noqa: E501
-        :rtype: list[lusid_notification.Delivery]
+        :return: The values of this ResourceListOfEventTypeSchema.  # noqa: E501
+        :rtype: list[lusid_notification.EventTypeSchema]
         """
         return self._values
 
     @values.setter
     def values(self, values):
-        """Sets the values of this ResourceListOfDelivery.
+        """Sets the values of this ResourceListOfEventTypeSchema.
 
 
-        :param values: The values of this ResourceListOfDelivery.  # noqa: E501
-        :type values: list[lusid_notification.Delivery]
+        :param values: The values of this ResourceListOfEventTypeSchema.  # noqa: E501
+        :type values: list[lusid_notification.EventTypeSchema]
         """
         if self.local_vars_configuration.client_side_validation and values is None:  # noqa: E501
             raise ValueError("Invalid value for `values`, must not be `None`")  # noqa: E501
 
         self._values = values
 
     @property
     def href(self):
-        """Gets the href of this ResourceListOfDelivery.  # noqa: E501
+        """Gets the href of this ResourceListOfEventTypeSchema.  # noqa: E501
 
 
-        :return: The href of this ResourceListOfDelivery.  # noqa: E501
+        :return: The href of this ResourceListOfEventTypeSchema.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
-        """Sets the href of this ResourceListOfDelivery.
+        """Sets the href of this ResourceListOfEventTypeSchema.
 
 
-        :param href: The href of this ResourceListOfDelivery.  # noqa: E501
+        :param href: The href of this ResourceListOfEventTypeSchema.  # noqa: E501
         :type href: str
         """
 
         self._href = href
 
     @property
     def links(self):
-        """Gets the links of this ResourceListOfDelivery.  # noqa: E501
+        """Gets the links of this ResourceListOfEventTypeSchema.  # noqa: E501
 
 
-        :return: The links of this ResourceListOfDelivery.  # noqa: E501
+        :return: The links of this ResourceListOfEventTypeSchema.  # noqa: E501
         :rtype: list[lusid_notification.Link]
         """
         return self._links
 
     @links.setter
     def links(self, links):
-        """Sets the links of this ResourceListOfDelivery.
+        """Sets the links of this ResourceListOfEventTypeSchema.
 
 
-        :param links: The links of this ResourceListOfDelivery.  # noqa: E501
+        :param links: The links of this ResourceListOfEventTypeSchema.  # noqa: E501
         :type links: list[lusid_notification.Link]
         """
 
         self._links = links
 
     @property
     def next_page(self):
-        """Gets the next_page of this ResourceListOfDelivery.  # noqa: E501
+        """Gets the next_page of this ResourceListOfEventTypeSchema.  # noqa: E501
 
 
-        :return: The next_page of this ResourceListOfDelivery.  # noqa: E501
+        :return: The next_page of this ResourceListOfEventTypeSchema.  # noqa: E501
         :rtype: str
         """
         return self._next_page
 
     @next_page.setter
     def next_page(self, next_page):
-        """Sets the next_page of this ResourceListOfDelivery.
+        """Sets the next_page of this ResourceListOfEventTypeSchema.
 
 
-        :param next_page: The next_page of this ResourceListOfDelivery.  # noqa: E501
+        :param next_page: The next_page of this ResourceListOfEventTypeSchema.  # noqa: E501
         :type next_page: str
         """
 
         self._next_page = next_page
 
     @property
     def previous_page(self):
-        """Gets the previous_page of this ResourceListOfDelivery.  # noqa: E501
+        """Gets the previous_page of this ResourceListOfEventTypeSchema.  # noqa: E501
 
 
-        :return: The previous_page of this ResourceListOfDelivery.  # noqa: E501
+        :return: The previous_page of this ResourceListOfEventTypeSchema.  # noqa: E501
         :rtype: str
         """
         return self._previous_page
 
     @previous_page.setter
     def previous_page(self, previous_page):
-        """Sets the previous_page of this ResourceListOfDelivery.
+        """Sets the previous_page of this ResourceListOfEventTypeSchema.
 
 
-        :param previous_page: The previous_page of this ResourceListOfDelivery.  # noqa: E501
+        :param previous_page: The previous_page of this ResourceListOfEventTypeSchema.  # noqa: E501
         :type previous_page: str
         """
 
         self._previous_page = previous_page
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
@@ -239,18 +239,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResourceListOfDelivery):
+        if not isinstance(other, ResourceListOfEventTypeSchema):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ResourceListOfDelivery):
+        if not isinstance(other, ResourceListOfEventTypeSchema):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_list_of_notification.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/resource_list_of_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/resource_list_of_subscription.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/resource_list_of_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/sms_notification_type.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/sms_notification_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/subscription.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/update_notification_request.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/update_notification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/update_subscription.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/update_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/models/webhook_notification_type.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/models/webhook_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/rest.py` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.741
+    The version of the OpenAPI document: 0.1.744
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification/utilities/config_keys.json` & `lusid-notification-sdk-preview-0.1.744/lusid_notification/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-notification-sdk-preview-0.1.741/lusid_notification_sdk_preview.egg-info/SOURCES.txt` & `lusid-notification-sdk-preview-0.1.744/lusid_notification_sdk_preview.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,30 +5,26 @@
 lusid_notification/__version__.py
 lusid_notification/api_client.py
 lusid_notification/configuration.py
 lusid_notification/exceptions.py
 lusid_notification/rest.py
 lusid_notification/api/__init__.py
 lusid_notification/api/application_metadata_api.py
-lusid_notification/api/deliveries_api.py
 lusid_notification/api/event_types_api.py
 lusid_notification/api/manual_event_api.py
 lusid_notification/api/notifications_api.py
 lusid_notification/api/subscriptions_api.py
 lusid_notification/models/__init__.py
 lusid_notification/models/access_controlled_action.py
 lusid_notification/models/access_controlled_resource.py
 lusid_notification/models/action_id.py
 lusid_notification/models/amazon_sqs_notification_type.py
 lusid_notification/models/api_request_notification_type.py
-lusid_notification/models/attempt.py
-lusid_notification/models/attempt_status.py
 lusid_notification/models/create_notification_request.py
 lusid_notification/models/create_subscription.py
-lusid_notification/models/delivery.py
 lusid_notification/models/email_notification_type.py
 lusid_notification/models/event_type_schema.py
 lusid_notification/models/id_selector_definition.py
 lusid_notification/models/identifier_part_schema.py
 lusid_notification/models/link.py
 lusid_notification/models/lusid_problem_details.py
 lusid_notification/models/lusid_validation_problem_details.py
@@ -37,15 +33,14 @@
 lusid_notification/models/manual_event_header.py
 lusid_notification/models/manual_event_request.py
 lusid_notification/models/matching_pattern.py
 lusid_notification/models/notification.py
 lusid_notification/models/notification_status.py
 lusid_notification/models/resource_id.py
 lusid_notification/models/resource_list_of_access_controlled_resource.py
-lusid_notification/models/resource_list_of_delivery.py
 lusid_notification/models/resource_list_of_event_type_schema.py
 lusid_notification/models/resource_list_of_notification.py
 lusid_notification/models/resource_list_of_subscription.py
 lusid_notification/models/sms_notification_type.py
 lusid_notification/models/subscription.py
 lusid_notification/models/update_notification_request.py
 lusid_notification/models/update_subscription.py
```

### Comparing `lusid-notification-sdk-preview-0.1.741/setup.py` & `lusid-notification-sdk-preview-0.1.744/setup.py`

 * *Files identical despite different names*

