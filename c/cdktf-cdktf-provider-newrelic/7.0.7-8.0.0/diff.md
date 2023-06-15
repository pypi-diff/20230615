# Comparing `tmp/cdktf-cdktf-provider-newrelic-7.0.7.tar.gz` & `tmp/cdktf-cdktf-provider-newrelic-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-newrelic-7.0.7.tar", last modified: Tue Jun 13 03:16:25 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-newrelic-8.0.0.tar", last modified: Thu Jun 15 11:31:17 2023, max compression
```

## Comparing `cdktf-cdktf-provider-newrelic-7.0.7.tar` & `cdktf-cdktf-provider-newrelic-8.0.0.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.662413 cdktf-cdktf-provider-newrelic-7.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-13 03:16:25.662413 cdktf-cdktf-provider-newrelic-7.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 03:16:25.662413 cdktf-cdktf-provider-newrelic-7.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.642413 cdktf-cdktf-provider-newrelic-7.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.646413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.646413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   990919 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/_jsii/provider-newrelic@7.0.7.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.650413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/account_management/
--rw-r--r--   0 runner    (1001) docker     (123)    28308 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/account_management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.650413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/alert_channel/
--rw-r--r--   0 runner    (1001) docker     (123)    83067 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/alert_channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.650413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/alert_condition/
--rw-r--r--   0 runner    (1001) docker     (123)    70943 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/alert_condition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.650413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/alert_muting_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    76696 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/alert_muting_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.650413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/alert_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    26576 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/alert_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.650413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/alert_policy_channel/
--rw-r--r--   0 runner    (1001) docker     (123)    31710 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/alert_policy_channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.650413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/api_access_key/
--rw-r--r--   0 runner    (1001) docker     (123)    28938 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/api_access_key/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.650413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/application_settings/
--rw-r--r--   0 runner    (1001) docker     (123)    26062 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/application_settings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.650413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/browser_application/
--rw-r--r--   0 runner    (1001) docker     (123)    30313 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/browser_application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.650413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_integrations/
--rw-r--r--   0 runner    (1001) docker     (123)   396373 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.650413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_link_account/
--rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_link_account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.650413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_aws_integrations/
--rw-r--r--   0 runner    (1001) docker     (123)   832474 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_aws_integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.650413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_aws_link_account/
--rw-r--r--   0 runner    (1001) docker     (123)    33917 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_aws_link_account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.650413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_azure_integrations/
--rw-r--r--   0 runner    (1001) docker     (123)   424446 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_azure_integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.650413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_azure_link_account/
--rw-r--r--   0 runner    (1001) docker     (123)    30071 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_azure_link_account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.650413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_gcp_integrations/
--rw-r--r--   0 runner    (1001) docker     (123)   267462 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_gcp_integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_gcp_link_account/
--rw-r--r--   0 runner    (1001) docker     (123)    22663 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_gcp_link_account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_account/
--rw-r--r--   0 runner    (1001) docker     (123)    23043 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_channel/
--rw-r--r--   0 runner    (1001) docker     (123)    33433 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    23992 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_application/
--rw-r--r--   0 runner    (1001) docker     (123)    18316 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_cloud_account/
--rw-r--r--   0 runner    (1001) docker     (123)    22887 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_cloud_account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_entity/
--rw-r--r--   0 runner    (1001) docker     (123)    43903 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_entity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_key_transaction/
--rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_key_transaction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_notification_destination/
--rw-r--r--   0 runner    (1001) docker     (123)    29183 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_notification_destination/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_obfuscation_expression/
--rw-r--r--   0 runner    (1001) docker     (123)    20788 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_obfuscation_expression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_service_level_alert_helper/
--rw-r--r--   0 runner    (1001) docker     (123)    31959 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_service_level_alert_helper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_private_location/
--rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_private_location/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_secure_credential/
--rw-r--r--   0 runner    (1001) docker     (123)    21727 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_secure_credential/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_test_grok_pattern/
--rw-r--r--   0 runner    (1001) docker     (123)    42037 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_test_grok_pattern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_partition_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    39813 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_partition_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/entity_tags/
--rw-r--r--   0 runner    (1001) docker     (123)    42218 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/entity_tags/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/events_to_metrics_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    28631 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/events_to_metrics_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/infra_alert_condition/
--rw-r--r--   0 runner    (1001) docker     (123)    77306 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/infra_alert_condition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/insights_event/
--rw-r--r--   0 runner    (1001) docker     (123)    51813 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/insights_event/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/log_parsing_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    35191 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/log_parsing_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/notification_channel/
--rw-r--r--   0 runner    (1001) docker     (123)    52371 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/notification_channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/notification_destination/
--rw-r--r--   0 runner    (1001) docker     (123)    68718 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/notification_destination/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/nrql_alert_condition/
--rw-r--r--   0 runner    (1001) docker     (123)   175881 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/nrql_alert_condition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/nrql_drop_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    25248 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/nrql_drop_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/obfuscation_expression/
--rw-r--r--   0 runner    (1001) docker     (123)    25128 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/obfuscation_expression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.654413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/obfuscation_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    47114 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/obfuscation_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.658413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/one_dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)  2263309 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/one_dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.658413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/one_dashboard_json/
--rw-r--r--   0 runner    (1001) docker     (123)    31382 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/one_dashboard_json/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.658413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/one_dashboard_raw/
--rw-r--r--   0 runner    (1001) docker     (123)    72306 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/one_dashboard_raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.658413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    38739 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.658413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/service_level/
--rw-r--r--   0 runner    (1001) docker     (123)   123714 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/service_level/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.658413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_alert_condition/
--rw-r--r--   0 runner    (1001) docker     (123)    28663 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_alert_condition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.658413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_broken_links_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)    52018 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_broken_links_monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.658413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_cert_check_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)    54105 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_cert_check_monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.658413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)    96311 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.658413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_multilocation_alert_condition/
--rw-r--r--   0 runner    (1001) docker     (123)    50382 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_multilocation_alert_condition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.658413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_private_location/
--rw-r--r--   0 runner    (1001) docker     (123)    27421 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_private_location/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.658413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_script_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)    88113 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_script_monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.658413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_secure_credential/
--rw-r--r--   0 runner    (1001) docker     (123)    37082 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_secure_credential/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.662413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_step_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)    88580 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_step_monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.662413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)   117351 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.662413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/workload/
--rw-r--r--   0 runner    (1001) docker     (123)   140236 2023-06-13 03:16:11.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/workload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:16:25.646413 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-13 03:16:25.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-06-13 03:16:25.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:16:25.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-13 03:16:25.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-13 03:16:25.000000 cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.120872 cdktf-cdktf-provider-newrelic-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-15 11:31:17.120872 cdktf-cdktf-provider-newrelic-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:31:17.120872 cdktf-cdktf-provider-newrelic-8.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.100872 cdktf-cdktf-provider-newrelic-8.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.108872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.108872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   990910 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/_jsii/provider-newrelic@8.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.108872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/account_management/
+-rw-r--r--   0 runner    (1001) docker     (123)    28308 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/account_management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.108872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/alert_channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    83067 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/alert_channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.108872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/alert_condition/
+-rw-r--r--   0 runner    (1001) docker     (123)    70943 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/alert_condition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.108872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/alert_muting_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    76696 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/alert_muting_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.108872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/alert_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    26576 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/alert_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.108872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/alert_policy_channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    31710 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/alert_policy_channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.108872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/api_access_key/
+-rw-r--r--   0 runner    (1001) docker     (123)    28938 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/api_access_key/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.108872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/application_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)    26062 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/application_settings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.108872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/browser_application/
+-rw-r--r--   0 runner    (1001) docker     (123)    30313 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/browser_application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.108872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)   396373 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.108872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_link_account/
+-rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_link_account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.112872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_aws_integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)   832474 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_aws_integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.112872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_aws_link_account/
+-rw-r--r--   0 runner    (1001) docker     (123)    33917 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_aws_link_account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.112872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_azure_integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)   424446 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_azure_integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.112872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_azure_link_account/
+-rw-r--r--   0 runner    (1001) docker     (123)    30071 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_azure_link_account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.112872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_gcp_integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)   267462 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_gcp_integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.112872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_gcp_link_account/
+-rw-r--r--   0 runner    (1001) docker     (123)    22663 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_gcp_link_account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.112872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_account/
+-rw-r--r--   0 runner    (1001) docker     (123)    23043 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.112872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    33433 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.112872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    23992 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.112872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_application/
+-rw-r--r--   0 runner    (1001) docker     (123)    18316 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.112872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_cloud_account/
+-rw-r--r--   0 runner    (1001) docker     (123)    22887 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_cloud_account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.112872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_entity/
+-rw-r--r--   0 runner    (1001) docker     (123)    43903 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_entity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.112872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_key_transaction/
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_key_transaction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.112872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_notification_destination/
+-rw-r--r--   0 runner    (1001) docker     (123)    29183 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_notification_destination/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.112872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_obfuscation_expression/
+-rw-r--r--   0 runner    (1001) docker     (123)    20788 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_obfuscation_expression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.112872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_service_level_alert_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)    31959 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_service_level_alert_helper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.112872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_private_location/
+-rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_private_location/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.112872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_secure_credential/
+-rw-r--r--   0 runner    (1001) docker     (123)    21727 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_secure_credential/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.112872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_test_grok_pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)    42037 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_test_grok_pattern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.116872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_partition_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    39813 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_partition_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.116872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/entity_tags/
+-rw-r--r--   0 runner    (1001) docker     (123)    42218 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/entity_tags/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.116872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/events_to_metrics_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    28631 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/events_to_metrics_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.116872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/infra_alert_condition/
+-rw-r--r--   0 runner    (1001) docker     (123)    77306 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/infra_alert_condition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.116872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/insights_event/
+-rw-r--r--   0 runner    (1001) docker     (123)    51813 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/insights_event/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.116872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/log_parsing_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    35191 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/log_parsing_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.116872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/notification_channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    52371 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/notification_channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.116872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/notification_destination/
+-rw-r--r--   0 runner    (1001) docker     (123)    68718 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/notification_destination/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.116872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/nrql_alert_condition/
+-rw-r--r--   0 runner    (1001) docker     (123)   175881 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/nrql_alert_condition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.116872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/nrql_drop_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    25248 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/nrql_drop_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.116872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/obfuscation_expression/
+-rw-r--r--   0 runner    (1001) docker     (123)    25128 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/obfuscation_expression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.116872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/obfuscation_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    47114 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/obfuscation_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.116872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/one_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)  2263309 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/one_dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.120872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/one_dashboard_json/
+-rw-r--r--   0 runner    (1001) docker     (123)    31382 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/one_dashboard_json/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.120872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/one_dashboard_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)    72306 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/one_dashboard_raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.120872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    38739 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.120872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/service_level/
+-rw-r--r--   0 runner    (1001) docker     (123)   123714 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/service_level/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.120872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_alert_condition/
+-rw-r--r--   0 runner    (1001) docker     (123)    28663 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_alert_condition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.120872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_broken_links_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)    52018 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_broken_links_monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.120872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_cert_check_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)    54105 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_cert_check_monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.120872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)    96311 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.120872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_multilocation_alert_condition/
+-rw-r--r--   0 runner    (1001) docker     (123)    50382 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_multilocation_alert_condition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.120872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_private_location/
+-rw-r--r--   0 runner    (1001) docker     (123)    27421 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_private_location/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.120872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_script_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)    88113 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_script_monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.120872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_secure_credential/
+-rw-r--r--   0 runner    (1001) docker     (123)    37082 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_secure_credential/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.120872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_step_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)    88580 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_step_monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.120872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)   117351 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.120872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/workload/
+-rw-r--r--   0 runner    (1001) docker     (123)   140236 2023-06-15 11:31:03.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/workload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:31:17.108872 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-15 11:31:17.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-06-15 11:31:17.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:31:17.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 11:31:17.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 11:31:17.000000 cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/LICENSE` & `cdktf-cdktf-provider-newrelic-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/PKG-INFO` & `cdktf-cdktf-provider-newrelic-8.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-newrelic
-Version: 7.0.7
+Version: 8.0.0
 Summary: Prebuilt newrelic Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-newrelic.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-newrelic.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/README.md` & `cdktf-cdktf-provider-newrelic-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/setup.py` & `cdktf-cdktf-provider-newrelic-8.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-newrelic",
-    "version": "7.0.7",
+    "version": "8.0.0",
     "description": "Prebuilt newrelic Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-newrelic.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -80,25 +80,25 @@
         "cdktf_cdktf_provider_newrelic.synthetics_secure_credential",
         "cdktf_cdktf_provider_newrelic.synthetics_step_monitor",
         "cdktf_cdktf_provider_newrelic.workflow",
         "cdktf_cdktf_provider_newrelic.workload"
     ],
     "package_data": {
         "cdktf_cdktf_provider_newrelic._jsii": [
-            "provider-newrelic@7.0.7.jsii.tgz"
+            "provider-newrelic@8.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_newrelic": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdktf>=0.16.3, <0.17.0",
+        "cdktf>=0.17.0, <0.18.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.83.0, <2.0.0",
+        "jsii>=1.84.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/account_management/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/account_management/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/alert_channel/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/alert_channel/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
         '''Create a new {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_channel newrelic_alert_channel} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
         :param name: (Required) The name of the channel. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_channel#name AlertChannel#name}
-        :param type: (Required) The type of channel. One of: (slack, user, victorops, webhook, email, opsgenie, pagerduty). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_channel#type AlertChannel#type}
+        :param type: (Required) The type of channel. One of: (pagerduty, slack, user, victorops, webhook, email, opsgenie). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_channel#type AlertChannel#type}
         :param account_id: The New Relic account ID where you want to create alert channels. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_channel#account_id AlertChannel#account_id}
         :param config: config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_channel#config AlertChannel#config}
         :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_channel#id AlertChannel#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
@@ -299,15 +299,15 @@
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         :param name: (Required) The name of the channel. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_channel#name AlertChannel#name}
-        :param type: (Required) The type of channel. One of: (slack, user, victorops, webhook, email, opsgenie, pagerduty). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_channel#type AlertChannel#type}
+        :param type: (Required) The type of channel. One of: (pagerduty, slack, user, victorops, webhook, email, opsgenie). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_channel#type AlertChannel#type}
         :param account_id: The New Relic account ID where you want to create alert channels. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_channel#account_id AlertChannel#account_id}
         :param config: config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_channel#config AlertChannel#config}
         :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_channel#id AlertChannel#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(config, dict):
@@ -423,15 +423,15 @@
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> builtins.str:
-        '''(Required) The type of channel. One of: (slack, user, victorops, webhook, email, opsgenie, pagerduty).
+        '''(Required) The type of channel. One of: (pagerduty, slack, user, victorops, webhook, email, opsgenie).
 
         Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_channel#type AlertChannel#type}
         '''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
```

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/alert_condition/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/alert_condition/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
         :param entities: The instance IDs associated with this condition. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#entities AlertCondition#entities}
         :param metric: The metric field accepts parameters based on the type set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#metric AlertCondition#metric}
         :param name: The title of the condition. Must be between 1 and 128 characters, inclusive. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#name AlertCondition#name}
         :param policy_id: The ID of the policy where this condition should be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#policy_id AlertCondition#policy_id}
         :param term: term block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#term AlertCondition#term}
-        :param type: The type of condition. One of: (apm_app_metric, apm_jvm_metric, apm_kt_metric, browser_metric, mobile_metric, servers_metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#type AlertCondition#type}
+        :param type: The type of condition. One of: (mobile_metric, servers_metric, apm_app_metric, apm_jvm_metric, apm_kt_metric, browser_metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#type AlertCondition#type}
         :param condition_scope: One of (application, instance). Choose application for most scenarios. If you are using the JVM plugin in New Relic, the instance setting allows your condition to trigger for specific app instances. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#condition_scope AlertCondition#condition_scope}
         :param enabled: Whether the condition is enabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#enabled AlertCondition#enabled}
         :param gc_metric: A valid Garbage Collection metric e.g. GC/G1 Young Generation. This is required if you are using apm_jvm_metric with gc_cpu_time condition type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#gc_metric AlertCondition#gc_metric}
         :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#id AlertCondition#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param runbook_url: Runbook URL to display in notifications. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#runbook_url AlertCondition#runbook_url}
         :param user_defined_metric: A custom metric to be evaluated. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#user_defined_metric AlertCondition#user_defined_metric}
         :param user_defined_value_function: One of: (average, min, max, total, sample_size, percent, rate). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#user_defined_value_function AlertCondition#user_defined_value_function}
@@ -471,15 +471,15 @@
         :param provider: 
         :param provisioners: 
         :param entities: The instance IDs associated with this condition. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#entities AlertCondition#entities}
         :param metric: The metric field accepts parameters based on the type set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#metric AlertCondition#metric}
         :param name: The title of the condition. Must be between 1 and 128 characters, inclusive. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#name AlertCondition#name}
         :param policy_id: The ID of the policy where this condition should be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#policy_id AlertCondition#policy_id}
         :param term: term block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#term AlertCondition#term}
-        :param type: The type of condition. One of: (apm_app_metric, apm_jvm_metric, apm_kt_metric, browser_metric, mobile_metric, servers_metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#type AlertCondition#type}
+        :param type: The type of condition. One of: (mobile_metric, servers_metric, apm_app_metric, apm_jvm_metric, apm_kt_metric, browser_metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#type AlertCondition#type}
         :param condition_scope: One of (application, instance). Choose application for most scenarios. If you are using the JVM plugin in New Relic, the instance setting allows your condition to trigger for specific app instances. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#condition_scope AlertCondition#condition_scope}
         :param enabled: Whether the condition is enabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#enabled AlertCondition#enabled}
         :param gc_metric: A valid Garbage Collection metric e.g. GC/G1 Young Generation. This is required if you are using apm_jvm_metric with gc_cpu_time condition type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#gc_metric AlertCondition#gc_metric}
         :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#id AlertCondition#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param runbook_url: Runbook URL to display in notifications. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#runbook_url AlertCondition#runbook_url}
         :param user_defined_metric: A custom metric to be evaluated. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#user_defined_metric AlertCondition#user_defined_metric}
         :param user_defined_value_function: One of: (average, min, max, total, sample_size, percent, rate). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#user_defined_value_function AlertCondition#user_defined_value_function}
@@ -663,15 +663,15 @@
         '''
         result = self._values.get("term")
         assert result is not None, "Required property 'term' is missing"
         return typing.cast(typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["AlertConditionTerm"]], result)
 
     @builtins.property
     def type(self) -> builtins.str:
-        '''The type of condition. One of: (apm_app_metric, apm_jvm_metric, apm_kt_metric, browser_metric, mobile_metric, servers_metric).
+        '''The type of condition. One of: (mobile_metric, servers_metric, apm_app_metric, apm_jvm_metric, apm_kt_metric, browser_metric).
 
         Docs at Terraform Registry: {@link https://registry.terraform.io/providers/newrelic/newrelic/3.24.2/docs/resources/alert_condition#type AlertCondition#type}
         '''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
```

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/alert_muting_rule/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/alert_muting_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/alert_policy/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/alert_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/alert_policy_channel/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/alert_policy_channel/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/api_access_key/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/api_access_key/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/application_settings/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/application_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/browser_application/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/browser_application/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_integrations/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_link_account/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_aws_govcloud_link_account/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_aws_integrations/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_aws_integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_aws_link_account/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_aws_link_account/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_azure_integrations/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_azure_integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_azure_link_account/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_azure_link_account/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_gcp_integrations/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_gcp_integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/cloud_gcp_link_account/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/cloud_gcp_link_account/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_account/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_account/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_channel/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_channel/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_policy/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_alert_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_application/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_application/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_cloud_account/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_cloud_account/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_entity/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_entity/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_key_transaction/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_key_transaction/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_notification_destination/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_notification_destination/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_obfuscation_expression/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_obfuscation_expression/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_service_level_alert_helper/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_service_level_alert_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_private_location/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_private_location/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_secure_credential/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_synthetics_secure_credential/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_newrelic_test_grok_pattern/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_newrelic_test_grok_pattern/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/data_partition_rule/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/data_partition_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/entity_tags/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/entity_tags/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/events_to_metrics_rule/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/events_to_metrics_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/infra_alert_condition/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/infra_alert_condition/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/insights_event/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/insights_event/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/log_parsing_rule/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/log_parsing_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/notification_channel/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/notification_channel/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/notification_destination/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/notification_destination/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/nrql_alert_condition/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/nrql_alert_condition/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/nrql_drop_rule/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/nrql_drop_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/obfuscation_expression/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/obfuscation_expression/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/obfuscation_rule/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/obfuscation_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/one_dashboard/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/one_dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/one_dashboard_json/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/one_dashboard_json/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/one_dashboard_raw/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/one_dashboard_raw/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/provider/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/service_level/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/service_level/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_alert_condition/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_alert_condition/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_broken_links_monitor/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_broken_links_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_cert_check_monitor/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_cert_check_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_monitor/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_multilocation_alert_condition/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_multilocation_alert_condition/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_private_location/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_private_location/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_script_monitor/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_script_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_secure_credential/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_secure_credential/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/synthetics_step_monitor/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/synthetics_step_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/workflow/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic/workload/__init__.py` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic/workload/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic.egg-info/PKG-INFO` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-newrelic
-Version: 7.0.7
+Version: 8.0.0
 Summary: Prebuilt newrelic Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-newrelic.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-newrelic.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-newrelic-7.0.7/src/cdktf_cdktf_provider_newrelic.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-newrelic-8.0.0/src/cdktf_cdktf_provider_newrelic.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_newrelic/py.typed
 src/cdktf_cdktf_provider_newrelic.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_newrelic.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_newrelic.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_newrelic.egg-info/requires.txt
 src/cdktf_cdktf_provider_newrelic.egg-info/top_level.txt
 src/cdktf_cdktf_provider_newrelic/_jsii/__init__.py
-src/cdktf_cdktf_provider_newrelic/_jsii/provider-newrelic@7.0.7.jsii.tgz
+src/cdktf_cdktf_provider_newrelic/_jsii/provider-newrelic@8.0.0.jsii.tgz
 src/cdktf_cdktf_provider_newrelic/account_management/__init__.py
 src/cdktf_cdktf_provider_newrelic/alert_channel/__init__.py
 src/cdktf_cdktf_provider_newrelic/alert_condition/__init__.py
 src/cdktf_cdktf_provider_newrelic/alert_muting_rule/__init__.py
 src/cdktf_cdktf_provider_newrelic/alert_policy/__init__.py
 src/cdktf_cdktf_provider_newrelic/alert_policy_channel/__init__.py
 src/cdktf_cdktf_provider_newrelic/api_access_key/__init__.py
```

