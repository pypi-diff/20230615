# Comparing `tmp/pulumi_fastly-8.1.0a1686634705.tar.gz` & `tmp/pulumi_fastly-8.1.0a1686825094.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_fastly-8.1.0a1686634705.tar", last modified: Tue Jun 13 05:49:41 2023, max compression
+gzip compressed data, was "pulumi_fastly-8.1.0a1686825094.tar", last modified: Thu Jun 15 10:36:53 2023, max compression
```

## Comparing `pulumi_fastly-8.1.0a1686634705.tar` & `pulumi_fastly-8.1.0a1686825094.tar`

### file list

```diff
@@ -1,56 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:49:41.891144 pulumi_fastly-8.1.0a1686634705/
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-13 05:49:41.891144 pulumi_fastly-8.1.0a1686634705/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:49:41.891144 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   506544 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:49:41.891144 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_fastly_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_package_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_activation_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_configuration_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_platform_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_private_key_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_subscription_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_waf_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)   451028 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13944 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/service_acl_entries.py
--rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/service_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)    93253 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/service_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/service_dictionary_items.py
--rw-r--r--   0 runner    (1001) docker     (123)    14198 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/service_dynamic_snippet_content.py
--rw-r--r--   0 runner    (1001) docker     (123)   124679 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/service_vcl.py
--rw-r--r--   0 runner    (1001) docker     (123)    81770 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/service_waf_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    26052 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    34762 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/tls_subscription_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:49:41.891144 pulumi_fastly-8.1.0a1686634705/pulumi_fastly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/pulumi_fastly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 05:49:41.891144 pulumi_fastly-8.1.0a1686634705/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-13 05:49:41.000000 pulumi_fastly-8.1.0a1686634705/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:36:53.851963 pulumi_fastly-8.1.0a1686825094/
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-15 10:36:53.851963 pulumi_fastly-8.1.0a1686825094/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:36:53.851963 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   508272 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:36:53.851963 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/configstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/configstore_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_fastly_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_package_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_activation_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_configuration_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_platform_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_private_key_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_subscription_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_waf_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)   452937 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13944 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/service_acl_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/service_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96684 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/service_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/service_dictionary_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14198 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/service_dynamic_snippet_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124679 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/service_vcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81770 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/service_waf_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17758 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/tls_mutual_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26052 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34762 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/tls_subscription_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:36:53.851963 pulumi_fastly-8.1.0a1686825094/pulumi_fastly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/pulumi_fastly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 10:36:53.851963 pulumi_fastly-8.1.0a1686825094/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-15 10:36:53.000000 pulumi_fastly-8.1.0a1686825094/setup.py
```

### Comparing `pulumi_fastly-8.1.0a1686634705/PKG-INFO` & `pulumi_fastly-8.1.0a1686825094/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 8.1.0a1686634705
+Version: 8.1.0a1686825094
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi fastly
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_fastly-8.1.0a1686634705/README.md` & `pulumi_fastly-8.1.0a1686825094/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/__init__.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
+from .configstore import *
+from .configstore_entries import *
 from .get_datacenters import *
 from .get_dictionaries import *
 from .get_fastly_ip_ranges import *
 from .get_package_hash import *
 from .get_services import *
 from .get_tls_activation import *
 from .get_tls_activation_ids import *
@@ -20,24 +22,26 @@
 from .get_tls_platform_certificate import *
 from .get_tls_platform_certificate_ids import *
 from .get_tls_private_key import *
 from .get_tls_private_key_ids import *
 from .get_tls_subscription import *
 from .get_tls_subscription_ids import *
 from .get_waf_rules import *
+from .kvstore import *
 from .provider import *
 from .service_acl_entries import *
 from .service_authorization import *
 from .service_compute import *
 from .service_dictionary_items import *
 from .service_dynamic_snippet_content import *
 from .service_vcl import *
 from .service_waf_configuration import *
 from .tls_activation import *
 from .tls_certificate import *
+from .tls_mutual_authentication import *
 from .tls_platform_certificate import *
 from .tls_private_key import *
 from .tls_subscription import *
 from .tls_subscription_validation import *
 from .user import *
 from ._inputs import *
 from . import outputs
@@ -50,14 +54,38 @@
     config = _utilities.lazy_import('pulumi_fastly.config')
 
 _utilities.register(
     resource_modules="""
 [
  {
   "pkg": "fastly",
+  "mod": "index/configstore",
+  "fqn": "pulumi_fastly",
+  "classes": {
+   "fastly:index/configstore:Configstore": "Configstore"
+  }
+ },
+ {
+  "pkg": "fastly",
+  "mod": "index/configstoreEntries",
+  "fqn": "pulumi_fastly",
+  "classes": {
+   "fastly:index/configstoreEntries:ConfigstoreEntries": "ConfigstoreEntries"
+  }
+ },
+ {
+  "pkg": "fastly",
+  "mod": "index/kvstore",
+  "fqn": "pulumi_fastly",
+  "classes": {
+   "fastly:index/kvstore:Kvstore": "Kvstore"
+  }
+ },
+ {
+  "pkg": "fastly",
   "mod": "index/serviceACLEntries",
   "fqn": "pulumi_fastly",
   "classes": {
    "fastly:index/serviceACLEntries:ServiceACLEntries": "ServiceACLEntries"
   }
  },
  {
@@ -122,14 +150,22 @@
   "fqn": "pulumi_fastly",
   "classes": {
    "fastly:index/tlsCertificate:TlsCertificate": "TlsCertificate"
   }
  },
  {
   "pkg": "fastly",
+  "mod": "index/tlsMutualAuthentication",
+  "fqn": "pulumi_fastly",
+  "classes": {
+   "fastly:index/tlsMutualAuthentication:TlsMutualAuthentication": "TlsMutualAuthentication"
+  }
+ },
+ {
+  "pkg": "fastly",
   "mod": "index/tlsPlatformCertificate",
   "fqn": "pulumi_fastly",
   "classes": {
    "fastly:index/tlsPlatformCertificate:TlsPlatformCertificate": "TlsPlatformCertificate"
   }
  },
  {
```

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/_inputs.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     'ServiceComputeLoggingScalyrArgs',
     'ServiceComputeLoggingSftpArgs',
     'ServiceComputeLoggingSplunkArgs',
     'ServiceComputeLoggingSumologicArgs',
     'ServiceComputeLoggingSyslogArgs',
     'ServiceComputePackageArgs',
     'ServiceComputeProductEnablementArgs',
+    'ServiceComputeResourceLinkArgs',
     'ServiceVclAclArgs',
     'ServiceVclBackendArgs',
     'ServiceVclCacheSettingArgs',
     'ServiceVclConditionArgs',
     'ServiceVclDictionaryArgs',
     'ServiceVclDirectorArgs',
     'ServiceVclDomainArgs',
@@ -4256,14 +4257,67 @@
 
     @websockets.setter
     def websockets(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "websockets", value)
 
 
 @pulumi.input_type
+class ServiceComputeResourceLinkArgs:
+    def __init__(__self__, *,
+                 name: pulumi.Input[str],
+                 resource_id: pulumi.Input[str],
+                 link_id: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] name: The name of the resource link.
+        :param pulumi.Input[str] resource_id: The ID of the underlying linked resource.
+        :param pulumi.Input[str] link_id: An alphanumeric string identifying the resource link.
+        """
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "resource_id", resource_id)
+        if link_id is not None:
+            pulumi.set(__self__, "link_id", link_id)
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        The name of the resource link.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter(name="resourceId")
+    def resource_id(self) -> pulumi.Input[str]:
+        """
+        The ID of the underlying linked resource.
+        """
+        return pulumi.get(self, "resource_id")
+
+    @resource_id.setter
+    def resource_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "resource_id", value)
+
+    @property
+    @pulumi.getter(name="linkId")
+    def link_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        An alphanumeric string identifying the resource link.
+        """
+        return pulumi.get(self, "link_id")
+
+    @link_id.setter
+    def link_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "link_id", value)
+
+
+@pulumi.input_type
 class ServiceVclAclArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  acl_id: Optional[pulumi.Input[str]] = None,
                  force_destroy: Optional[pulumi.Input[bool]] = None):
         """
         :param pulumi.Input[str] name: A unique name to identify this ACL. It is important to note that changing this attribute will delete and recreate the ACL, and discard the current items in the ACL
@@ -10896,15 +10950,15 @@
                  feature_revision: Optional[pulumi.Input[int]] = None,
                  logger_type: Optional[pulumi.Input[str]] = None,
                  ratelimiter_id: Optional[pulumi.Input[str]] = None,
                  response: Optional[pulumi.Input['ServiceVclRateLimiterResponseArgs']] = None,
                  response_object_name: Optional[pulumi.Input[str]] = None,
                  uri_dictionary_name: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] action: The action to take when a rate limiter violation is detected (one of: log*only, log*only, response_object)
+        :param pulumi.Input[str] action: The action to take when a rate limiter violation is detected (one of: log*only, response, response*object)
         :param pulumi.Input[str] client_key: Comma-separated list of VCL variables used to generate a counter key to identify a client
         :param pulumi.Input[str] http_methods: Comma-separated list of HTTP methods to apply rate limiting to
         :param pulumi.Input[str] name: A unique human readable name for the rate limiting rule
         :param pulumi.Input[int] penalty_box_duration: Length of time in minutes that the rate limiter is in effect after the initial violation is detected
         :param pulumi.Input[int] rps_limit: Upper limit of requests per second allowed by the rate limiter
         :param pulumi.Input[int] window_size: Number of seconds during which the RPS limit must be exceeded in order to trigger a violation (one of: 1, 10, 60)
         :param pulumi.Input[int] feature_revision: Revision number of the rate limiting feature implementation
@@ -10934,15 +10988,15 @@
         if uri_dictionary_name is not None:
             pulumi.set(__self__, "uri_dictionary_name", uri_dictionary_name)
 
     @property
     @pulumi.getter
     def action(self) -> pulumi.Input[str]:
         """
-        The action to take when a rate limiter violation is detected (one of: log*only, log*only, response_object)
+        The action to take when a rate limiter violation is detected (one of: log*only, response, response*object)
         """
         return pulumi.get(self, "action")
 
     @action.setter
     def action(self, value: pulumi.Input[str]):
         pulumi.set(self, "action", value)
```

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/_utilities.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/config/vars.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_datacenters.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_dictionaries.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_dictionaries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_fastly_ip_ranges.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_fastly_ip_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_package_hash.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_package_hash.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_services.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_activation.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_activation_ids.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_activation_ids.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
-    example_tls_activation_ids = fastly.get_tls_activation_ids(certificate_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    example_tls_activation_ids = fastly.get_tls_activation_ids(certificate_id=fastly_tls_certificate["example"]["id"])
     example_tls_activation = [fastly.get_tls_activation(id=__value) for __key, __value in example_tls_activation_ids.ids]
     pulumi.export("activationDomains", [a.domain for a in example_tls_activation])
     ```
 
 
     :param str certificate_id: ID of TLS certificate used to filter activations
     """
@@ -106,15 +106,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
-    example_tls_activation_ids = fastly.get_tls_activation_ids(certificate_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    example_tls_activation_ids = fastly.get_tls_activation_ids(certificate_id=fastly_tls_certificate["example"]["id"])
     example_tls_activation = [fastly.get_tls_activation(id=__value) for __key, __value in example_tls_activation_ids.ids]
     pulumi.export("activationDomains", [a.domain for a in example_tls_activation])
     ```
 
 
     :param str certificate_id: ID of TLS certificate used to filter activations
     """
```

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_certificate.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_certificate_ids.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_configuration.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_configuration_ids.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_configuration_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_domain.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_platform_certificate.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_platform_certificate_ids.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_platform_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_private_key.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_private_key_ids.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_private_key_ids.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     demo = fastly.get_tls_private_key_ids()
-    example = fastly.get_tls_private_key(id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    example = fastly.get_tls_private_key(id=fastly_tls_private_key_ids["demo"]["ids"])
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsPrivateKeyIds:getTlsPrivateKeyIds', __args__, opts=opts, typ=GetTlsPrivateKeyIdsResult).value
 
     return AwaitableGetTlsPrivateKeyIdsResult(
```

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_subscription.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_tls_subscription_ids.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_tls_subscription_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/get_waf_rules.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/get_waf_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/outputs.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     'ServiceComputeLoggingScalyr',
     'ServiceComputeLoggingSftp',
     'ServiceComputeLoggingSplunk',
     'ServiceComputeLoggingSumologic',
     'ServiceComputeLoggingSyslog',
     'ServiceComputePackage',
     'ServiceComputeProductEnablement',
+    'ServiceComputeResourceLink',
     'ServiceVclAcl',
     'ServiceVclBackend',
     'ServiceVclCacheSetting',
     'ServiceVclCondition',
     'ServiceVclDictionary',
     'ServiceVclDirector',
     'ServiceVclDomain',
@@ -3831,14 +3832,74 @@
         """
         Enable WebSockets support
         """
         return pulumi.get(self, "websockets")
 
 
 @pulumi.output_type
+class ServiceComputeResourceLink(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "resourceId":
+            suggest = "resource_id"
+        elif key == "linkId":
+            suggest = "link_id"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ServiceComputeResourceLink. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ServiceComputeResourceLink.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ServiceComputeResourceLink.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 name: str,
+                 resource_id: str,
+                 link_id: Optional[str] = None):
+        """
+        :param str name: The name of the resource link.
+        :param str resource_id: The ID of the underlying linked resource.
+        :param str link_id: An alphanumeric string identifying the resource link.
+        """
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "resource_id", resource_id)
+        if link_id is not None:
+            pulumi.set(__self__, "link_id", link_id)
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        The name of the resource link.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="resourceId")
+    def resource_id(self) -> str:
+        """
+        The ID of the underlying linked resource.
+        """
+        return pulumi.get(self, "resource_id")
+
+    @property
+    @pulumi.getter(name="linkId")
+    def link_id(self) -> Optional[str]:
+        """
+        An alphanumeric string identifying the resource link.
+        """
+        return pulumi.get(self, "link_id")
+
+
+@pulumi.output_type
 class ServiceVclAcl(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "aclId":
             suggest = "acl_id"
         elif key == "forceDestroy":
@@ -9817,15 +9878,15 @@
                  feature_revision: Optional[int] = None,
                  logger_type: Optional[str] = None,
                  ratelimiter_id: Optional[str] = None,
                  response: Optional['outputs.ServiceVclRateLimiterResponse'] = None,
                  response_object_name: Optional[str] = None,
                  uri_dictionary_name: Optional[str] = None):
         """
-        :param str action: The action to take when a rate limiter violation is detected (one of: log*only, log*only, response_object)
+        :param str action: The action to take when a rate limiter violation is detected (one of: log*only, response, response*object)
         :param str client_key: Comma-separated list of VCL variables used to generate a counter key to identify a client
         :param str http_methods: Comma-separated list of HTTP methods to apply rate limiting to
         :param str name: A unique human readable name for the rate limiting rule
         :param int penalty_box_duration: Length of time in minutes that the rate limiter is in effect after the initial violation is detected
         :param int rps_limit: Upper limit of requests per second allowed by the rate limiter
         :param int window_size: Number of seconds during which the RPS limit must be exceeded in order to trigger a violation (one of: 1, 10, 60)
         :param int feature_revision: Revision number of the rate limiting feature implementation
@@ -9855,15 +9916,15 @@
         if uri_dictionary_name is not None:
             pulumi.set(__self__, "uri_dictionary_name", uri_dictionary_name)
 
     @property
     @pulumi.getter
     def action(self) -> str:
         """
-        The action to take when a rate limiter violation is detected (one of: log*only, log*only, response_object)
+        The action to take when a rate limiter violation is detected (one of: log*only, response, response*object)
         """
         return pulumi.get(self, "action")
 
     @property
     @pulumi.getter(name="clientKey")
     def client_key(self) -> str:
         """
```

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/provider.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/service_acl_entries.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/service_acl_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/service_authorization.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/service_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/service_compute.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/service_compute.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,24 +47,26 @@
                  logging_scalyrs: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingScalyrArgs']]]] = None,
                  logging_sftps: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingSftpArgs']]]] = None,
                  logging_splunks: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingSplunkArgs']]]] = None,
                  logging_sumologics: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingSumologicArgs']]]] = None,
                  logging_syslogs: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingSyslogArgs']]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  product_enablement: Optional[pulumi.Input['ServiceComputeProductEnablementArgs']] = None,
+                 resource_links: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeResourceLinkArgs']]]] = None,
                  reuse: Optional[pulumi.Input[bool]] = None,
                  version_comment: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ServiceCompute resource.
         :param pulumi.Input[Sequence[pulumi.Input['ServiceComputeDomainArgs']]] domains: A set of Domain names to serve as entry points for your Service
         :param pulumi.Input['ServiceComputePackageArgs'] package: The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute@Edge service. See Fastly's documentation on [Compute@Edge](https://developer.fastly.com/learning/compute/)
         :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
         :param pulumi.Input[str] comment: Description field for the service. Default `Managed by Terraform`
         :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         :param pulumi.Input[str] name: The unique name for the Service to create
+        :param pulumi.Input[Sequence[pulumi.Input['ServiceComputeResourceLinkArgs']]] resource_links: A resource link represents a link between a shared resource (such as an KV Store or Config Store) and a service version.
         :param pulumi.Input[bool] reuse: Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
                deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
                an active service will cause an error. Default `false`
         :param pulumi.Input[str] version_comment: Description field for the version
         """
         pulumi.set(__self__, "domains", domains)
         pulumi.set(__self__, "package", package)
@@ -130,14 +132,16 @@
             pulumi.set(__self__, "logging_sumologics", logging_sumologics)
         if logging_syslogs is not None:
             pulumi.set(__self__, "logging_syslogs", logging_syslogs)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if product_enablement is not None:
             pulumi.set(__self__, "product_enablement", product_enablement)
+        if resource_links is not None:
+            pulumi.set(__self__, "resource_links", resource_links)
         if reuse is not None:
             pulumi.set(__self__, "reuse", reuse)
         if version_comment is not None:
             pulumi.set(__self__, "version_comment", version_comment)
 
     @property
     @pulumi.getter
@@ -469,14 +473,26 @@
         return pulumi.get(self, "product_enablement")
 
     @product_enablement.setter
     def product_enablement(self, value: Optional[pulumi.Input['ServiceComputeProductEnablementArgs']]):
         pulumi.set(self, "product_enablement", value)
 
     @property
+    @pulumi.getter(name="resourceLinks")
+    def resource_links(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeResourceLinkArgs']]]]:
+        """
+        A resource link represents a link between a shared resource (such as an KV Store or Config Store) and a service version.
+        """
+        return pulumi.get(self, "resource_links")
+
+    @resource_links.setter
+    def resource_links(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeResourceLinkArgs']]]]):
+        pulumi.set(self, "resource_links", value)
+
+    @property
     @pulumi.getter
     def reuse(self) -> Optional[pulumi.Input[bool]]:
         """
         Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
         deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
         an active service will cause an error. Default `false`
         """
@@ -537,14 +553,15 @@
                  logging_sftps: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingSftpArgs']]]] = None,
                  logging_splunks: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingSplunkArgs']]]] = None,
                  logging_sumologics: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingSumologicArgs']]]] = None,
                  logging_syslogs: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeLoggingSyslogArgs']]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  package: Optional[pulumi.Input['ServiceComputePackageArgs']] = None,
                  product_enablement: Optional[pulumi.Input['ServiceComputeProductEnablementArgs']] = None,
+                 resource_links: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeResourceLinkArgs']]]] = None,
                  reuse: Optional[pulumi.Input[bool]] = None,
                  version_comment: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ServiceCompute resources.
         :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
         :param pulumi.Input[int] active_version: The currently active version of your Fastly Service
         :param pulumi.Input[int] cloned_version: The latest cloned version by the provider
@@ -553,14 +570,15 @@
         :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         :param pulumi.Input[bool] force_refresh: Used internally by the provider to temporarily indicate if all resources should call their associated API to update the
                local state. This is for scenarios where the service version has been reverted outside of Terraform (e.g. via the Fastly
                UI) and the provider needs to resync the state for a different active version (this is only if `activate` is `true`).
         :param pulumi.Input[bool] imported: Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the import is finished
         :param pulumi.Input[str] name: The unique name for the Service to create
         :param pulumi.Input['ServiceComputePackageArgs'] package: The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute@Edge service. See Fastly's documentation on [Compute@Edge](https://developer.fastly.com/learning/compute/)
+        :param pulumi.Input[Sequence[pulumi.Input['ServiceComputeResourceLinkArgs']]] resource_links: A resource link represents a link between a shared resource (such as an KV Store or Config Store) and a service version.
         :param pulumi.Input[bool] reuse: Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
                deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
                an active service will cause an error. Default `false`
         :param pulumi.Input[str] version_comment: Description field for the version
         """
         if activate is not None:
             pulumi.set(__self__, "activate", activate)
@@ -636,14 +654,16 @@
             pulumi.set(__self__, "logging_syslogs", logging_syslogs)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if package is not None:
             pulumi.set(__self__, "package", package)
         if product_enablement is not None:
             pulumi.set(__self__, "product_enablement", product_enablement)
+        if resource_links is not None:
+            pulumi.set(__self__, "resource_links", resource_links)
         if reuse is not None:
             pulumi.set(__self__, "reuse", reuse)
         if version_comment is not None:
             pulumi.set(__self__, "version_comment", version_comment)
 
     @property
     @pulumi.getter
@@ -1025,14 +1045,26 @@
         return pulumi.get(self, "product_enablement")
 
     @product_enablement.setter
     def product_enablement(self, value: Optional[pulumi.Input['ServiceComputeProductEnablementArgs']]):
         pulumi.set(self, "product_enablement", value)
 
     @property
+    @pulumi.getter(name="resourceLinks")
+    def resource_links(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeResourceLinkArgs']]]]:
+        """
+        A resource link represents a link between a shared resource (such as an KV Store or Config Store) and a service version.
+        """
+        return pulumi.get(self, "resource_links")
+
+    @resource_links.setter
+    def resource_links(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceComputeResourceLinkArgs']]]]):
+        pulumi.set(self, "resource_links", value)
+
+    @property
     @pulumi.getter
     def reuse(self) -> Optional[pulumi.Input[bool]]:
         """
         Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
         deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
         an active service will cause an error. Default `false`
         """
@@ -1091,14 +1123,15 @@
                  logging_sftps: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingSftpArgs']]]]] = None,
                  logging_splunks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingSplunkArgs']]]]] = None,
                  logging_sumologics: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingSumologicArgs']]]]] = None,
                  logging_syslogs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingSyslogArgs']]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  package: Optional[pulumi.Input[pulumi.InputType['ServiceComputePackageArgs']]] = None,
                  product_enablement: Optional[pulumi.Input[pulumi.InputType['ServiceComputeProductEnablementArgs']]] = None,
+                 resource_links: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeResourceLinkArgs']]]]] = None,
                  reuse: Optional[pulumi.Input[bool]] = None,
                  version_comment: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Import
 
         Fastly Services can be imported using their service ID, e.g.
@@ -1117,14 +1150,15 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] activate: Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to `false`. Default `true`
         :param pulumi.Input[str] comment: Description field for the service. Default `Managed by Terraform`
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeDomainArgs']]]] domains: A set of Domain names to serve as entry points for your Service
         :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         :param pulumi.Input[str] name: The unique name for the Service to create
         :param pulumi.Input[pulumi.InputType['ServiceComputePackageArgs']] package: The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute@Edge service. See Fastly's documentation on [Compute@Edge](https://developer.fastly.com/learning/compute/)
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeResourceLinkArgs']]]] resource_links: A resource link represents a link between a shared resource (such as an KV Store or Config Store) and a service version.
         :param pulumi.Input[bool] reuse: Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
                deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
                an active service will cause an error. Default `false`
         :param pulumi.Input[str] version_comment: Description field for the version
         """
         ...
     @overload
@@ -1193,14 +1227,15 @@
                  logging_sftps: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingSftpArgs']]]]] = None,
                  logging_splunks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingSplunkArgs']]]]] = None,
                  logging_sumologics: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingSumologicArgs']]]]] = None,
                  logging_syslogs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingSyslogArgs']]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  package: Optional[pulumi.Input[pulumi.InputType['ServiceComputePackageArgs']]] = None,
                  product_enablement: Optional[pulumi.Input[pulumi.InputType['ServiceComputeProductEnablementArgs']]] = None,
+                 resource_links: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeResourceLinkArgs']]]]] = None,
                  reuse: Optional[pulumi.Input[bool]] = None,
                  version_comment: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
@@ -1243,14 +1278,15 @@
             __props__.__dict__["logging_sumologics"] = logging_sumologics
             __props__.__dict__["logging_syslogs"] = logging_syslogs
             __props__.__dict__["name"] = name
             if package is None and not opts.urn:
                 raise TypeError("Missing required property 'package'")
             __props__.__dict__["package"] = package
             __props__.__dict__["product_enablement"] = product_enablement
+            __props__.__dict__["resource_links"] = resource_links
             __props__.__dict__["reuse"] = reuse
             __props__.__dict__["version_comment"] = version_comment
             __props__.__dict__["active_version"] = None
             __props__.__dict__["cloned_version"] = None
             __props__.__dict__["force_refresh"] = None
             __props__.__dict__["imported"] = None
         super(ServiceCompute, __self__).__init__(
@@ -1298,14 +1334,15 @@
             logging_sftps: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingSftpArgs']]]]] = None,
             logging_splunks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingSplunkArgs']]]]] = None,
             logging_sumologics: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingSumologicArgs']]]]] = None,
             logging_syslogs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeLoggingSyslogArgs']]]]] = None,
             name: Optional[pulumi.Input[str]] = None,
             package: Optional[pulumi.Input[pulumi.InputType['ServiceComputePackageArgs']]] = None,
             product_enablement: Optional[pulumi.Input[pulumi.InputType['ServiceComputeProductEnablementArgs']]] = None,
+            resource_links: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeResourceLinkArgs']]]]] = None,
             reuse: Optional[pulumi.Input[bool]] = None,
             version_comment: Optional[pulumi.Input[str]] = None) -> 'ServiceCompute':
         """
         Get an existing ServiceCompute resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
@@ -1319,14 +1356,15 @@
         :param pulumi.Input[bool] force_destroy: Services that are active cannot be destroyed. In order to destroy the Service, set `force_destroy` to `true`. Default `false`
         :param pulumi.Input[bool] force_refresh: Used internally by the provider to temporarily indicate if all resources should call their associated API to update the
                local state. This is for scenarios where the service version has been reverted outside of Terraform (e.g. via the Fastly
                UI) and the provider needs to resync the state for a different active version (this is only if `activate` is `true`).
         :param pulumi.Input[bool] imported: Used internally by the provider to temporarily indicate if the service is being imported, and is reset to false once the import is finished
         :param pulumi.Input[str] name: The unique name for the Service to create
         :param pulumi.Input[pulumi.InputType['ServiceComputePackageArgs']] package: The `package` block supports uploading or modifying Wasm packages for use in a Fastly Compute@Edge service. See Fastly's documentation on [Compute@Edge](https://developer.fastly.com/learning/compute/)
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceComputeResourceLinkArgs']]]] resource_links: A resource link represents a link between a shared resource (such as an KV Store or Config Store) and a service version.
         :param pulumi.Input[bool] reuse: Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
                deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
                an active service will cause an error. Default `false`
         :param pulumi.Input[str] version_comment: Description field for the version
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -1367,14 +1405,15 @@
         __props__.__dict__["logging_sftps"] = logging_sftps
         __props__.__dict__["logging_splunks"] = logging_splunks
         __props__.__dict__["logging_sumologics"] = logging_sumologics
         __props__.__dict__["logging_syslogs"] = logging_syslogs
         __props__.__dict__["name"] = name
         __props__.__dict__["package"] = package
         __props__.__dict__["product_enablement"] = product_enablement
+        __props__.__dict__["resource_links"] = resource_links
         __props__.__dict__["reuse"] = reuse
         __props__.__dict__["version_comment"] = version_comment
         return ServiceCompute(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def activate(self) -> pulumi.Output[Optional[bool]]:
@@ -1599,14 +1638,22 @@
 
     @property
     @pulumi.getter(name="productEnablement")
     def product_enablement(self) -> pulumi.Output[Optional['outputs.ServiceComputeProductEnablement']]:
         return pulumi.get(self, "product_enablement")
 
     @property
+    @pulumi.getter(name="resourceLinks")
+    def resource_links(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceComputeResourceLink']]]:
+        """
+        A resource link represents a link between a shared resource (such as an KV Store or Config Store) and a service version.
+        """
+        return pulumi.get(self, "resource_links")
+
+    @property
     @pulumi.getter
     def reuse(self) -> pulumi.Output[Optional[bool]]:
         """
         Services that are active cannot be destroyed. If set to `true` a service Terraform intends to destroy will instead be
         deactivated (allowing it to be reused by importing it into another Terraform project). If `false`, attempting to destroy
         an active service will cause an error. Default `false`
         """
```

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/service_dictionary_items.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/service_dictionary_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/service_dynamic_snippet_content.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/service_dynamic_snippet_content.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/service_vcl.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/service_vcl.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/service_waf_configuration.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/service_waf_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/tls_activation.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/tls_activation.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,25 +12,29 @@
 __all__ = ['TlsActivationArgs', 'TlsActivation']
 
 @pulumi.input_type
 class TlsActivationArgs:
     def __init__(__self__, *,
                  certificate_id: pulumi.Input[str],
                  domain: pulumi.Input[str],
-                 configuration_id: Optional[pulumi.Input[str]] = None):
+                 configuration_id: Optional[pulumi.Input[str]] = None,
+                 mutual_authentication_id: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a TlsActivation resource.
         :param pulumi.Input[str] certificate_id: ID of certificate to use. Must have the `domain` specified in the certificate's Subject Alternative Names.
         :param pulumi.Input[str] domain: Domain to enable TLS on. Must be assigned to an existing Fastly Service.
         :param pulumi.Input[str] configuration_id: ID of TLS configuration to be used to terminate TLS traffic, or use the default one if missing.
+        :param pulumi.Input[str] mutual_authentication_id: An alphanumeric string identifying a mutual authentication.
         """
         pulumi.set(__self__, "certificate_id", certificate_id)
         pulumi.set(__self__, "domain", domain)
         if configuration_id is not None:
             pulumi.set(__self__, "configuration_id", configuration_id)
+        if mutual_authentication_id is not None:
+            pulumi.set(__self__, "mutual_authentication_id", mutual_authentication_id)
 
     @property
     @pulumi.getter(name="certificateId")
     def certificate_id(self) -> pulumi.Input[str]:
         """
         ID of certificate to use. Must have the `domain` specified in the certificate's Subject Alternative Names.
         """
@@ -60,37 +64,53 @@
         """
         return pulumi.get(self, "configuration_id")
 
     @configuration_id.setter
     def configuration_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "configuration_id", value)
 
+    @property
+    @pulumi.getter(name="mutualAuthenticationId")
+    def mutual_authentication_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        An alphanumeric string identifying a mutual authentication.
+        """
+        return pulumi.get(self, "mutual_authentication_id")
+
+    @mutual_authentication_id.setter
+    def mutual_authentication_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "mutual_authentication_id", value)
+
 
 @pulumi.input_type
 class _TlsActivationState:
     def __init__(__self__, *,
                  certificate_id: Optional[pulumi.Input[str]] = None,
                  configuration_id: Optional[pulumi.Input[str]] = None,
                  created_at: Optional[pulumi.Input[str]] = None,
-                 domain: Optional[pulumi.Input[str]] = None):
+                 domain: Optional[pulumi.Input[str]] = None,
+                 mutual_authentication_id: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering TlsActivation resources.
         :param pulumi.Input[str] certificate_id: ID of certificate to use. Must have the `domain` specified in the certificate's Subject Alternative Names.
         :param pulumi.Input[str] configuration_id: ID of TLS configuration to be used to terminate TLS traffic, or use the default one if missing.
         :param pulumi.Input[str] created_at: Time-stamp (GMT) when TLS was enabled.
         :param pulumi.Input[str] domain: Domain to enable TLS on. Must be assigned to an existing Fastly Service.
+        :param pulumi.Input[str] mutual_authentication_id: An alphanumeric string identifying a mutual authentication.
         """
         if certificate_id is not None:
             pulumi.set(__self__, "certificate_id", certificate_id)
         if configuration_id is not None:
             pulumi.set(__self__, "configuration_id", configuration_id)
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
+        if mutual_authentication_id is not None:
+            pulumi.set(__self__, "mutual_authentication_id", mutual_authentication_id)
 
     @property
     @pulumi.getter(name="certificateId")
     def certificate_id(self) -> Optional[pulumi.Input[str]]:
         """
         ID of certificate to use. Must have the `domain` specified in the certificate's Subject Alternative Names.
         """
@@ -132,23 +152,36 @@
         """
         return pulumi.get(self, "domain")
 
     @domain.setter
     def domain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "domain", value)
 
+    @property
+    @pulumi.getter(name="mutualAuthenticationId")
+    def mutual_authentication_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        An alphanumeric string identifying a mutual authentication.
+        """
+        return pulumi.get(self, "mutual_authentication_id")
+
+    @mutual_authentication_id.setter
+    def mutual_authentication_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "mutual_authentication_id", value)
+
 
 class TlsActivation(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  certificate_id: Optional[pulumi.Input[str]] = None,
                  configuration_id: Optional[pulumi.Input[str]] = None,
                  domain: Optional[pulumi.Input[str]] = None,
+                 mutual_authentication_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Enables TLS on a domain using a specified custom TLS certificate.
 
         > **Note:** The Fastly service must be provisioned _prior_ to enabling TLS on it.
 
         ## Example Usage
@@ -188,14 +221,15 @@
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] certificate_id: ID of certificate to use. Must have the `domain` specified in the certificate's Subject Alternative Names.
         :param pulumi.Input[str] configuration_id: ID of TLS configuration to be used to terminate TLS traffic, or use the default one if missing.
         :param pulumi.Input[str] domain: Domain to enable TLS on. Must be assigned to an existing Fastly Service.
+        :param pulumi.Input[str] mutual_authentication_id: An alphanumeric string identifying a mutual authentication.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: TlsActivationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -254,14 +288,15 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  certificate_id: Optional[pulumi.Input[str]] = None,
                  configuration_id: Optional[pulumi.Input[str]] = None,
                  domain: Optional[pulumi.Input[str]] = None,
+                 mutual_authentication_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
@@ -270,49 +305,53 @@
             if certificate_id is None and not opts.urn:
                 raise TypeError("Missing required property 'certificate_id'")
             __props__.__dict__["certificate_id"] = certificate_id
             __props__.__dict__["configuration_id"] = configuration_id
             if domain is None and not opts.urn:
                 raise TypeError("Missing required property 'domain'")
             __props__.__dict__["domain"] = domain
+            __props__.__dict__["mutual_authentication_id"] = mutual_authentication_id
             __props__.__dict__["created_at"] = None
         super(TlsActivation, __self__).__init__(
             'fastly:index/tlsActivation:TlsActivation',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             certificate_id: Optional[pulumi.Input[str]] = None,
             configuration_id: Optional[pulumi.Input[str]] = None,
             created_at: Optional[pulumi.Input[str]] = None,
-            domain: Optional[pulumi.Input[str]] = None) -> 'TlsActivation':
+            domain: Optional[pulumi.Input[str]] = None,
+            mutual_authentication_id: Optional[pulumi.Input[str]] = None) -> 'TlsActivation':
         """
         Get an existing TlsActivation resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] certificate_id: ID of certificate to use. Must have the `domain` specified in the certificate's Subject Alternative Names.
         :param pulumi.Input[str] configuration_id: ID of TLS configuration to be used to terminate TLS traffic, or use the default one if missing.
         :param pulumi.Input[str] created_at: Time-stamp (GMT) when TLS was enabled.
         :param pulumi.Input[str] domain: Domain to enable TLS on. Must be assigned to an existing Fastly Service.
+        :param pulumi.Input[str] mutual_authentication_id: An alphanumeric string identifying a mutual authentication.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _TlsActivationState.__new__(_TlsActivationState)
 
         __props__.__dict__["certificate_id"] = certificate_id
         __props__.__dict__["configuration_id"] = configuration_id
         __props__.__dict__["created_at"] = created_at
         __props__.__dict__["domain"] = domain
+        __props__.__dict__["mutual_authentication_id"] = mutual_authentication_id
         return TlsActivation(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="certificateId")
     def certificate_id(self) -> pulumi.Output[str]:
         """
         ID of certificate to use. Must have the `domain` specified in the certificate's Subject Alternative Names.
@@ -339,7 +378,15 @@
     @pulumi.getter
     def domain(self) -> pulumi.Output[str]:
         """
         Domain to enable TLS on. Must be assigned to an existing Fastly Service.
         """
         return pulumi.get(self, "domain")
 
+    @property
+    @pulumi.getter(name="mutualAuthenticationId")
+    def mutual_authentication_id(self) -> pulumi.Output[Optional[str]]:
+        """
+        An alphanumeric string identifying a mutual authentication.
+        """
+        return pulumi.get(self, "mutual_authentication_id")
+
```

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/tls_certificate.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/tls_platform_certificate.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/tls_private_key.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/tls_subscription.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/tls_subscription_validation.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/tls_subscription_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly/user.py` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly.egg-info/PKG-INFO` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-fastly
-Version: 8.1.0a1686634705
+Version: 8.1.0a1686825094
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi fastly
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_fastly-8.1.0a1686634705/pulumi_fastly.egg-info/SOURCES.txt` & `pulumi_fastly-8.1.0a1686825094/pulumi_fastly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 README.md
 setup.py
 pulumi_fastly/__init__.py
 pulumi_fastly/_inputs.py
 pulumi_fastly/_utilities.py
+pulumi_fastly/configstore.py
+pulumi_fastly/configstore_entries.py
 pulumi_fastly/get_datacenters.py
 pulumi_fastly/get_dictionaries.py
 pulumi_fastly/get_fastly_ip_ranges.py
 pulumi_fastly/get_package_hash.py
 pulumi_fastly/get_services.py
 pulumi_fastly/get_tls_activation.py
 pulumi_fastly/get_tls_activation_ids.py
@@ -18,27 +20,29 @@
 pulumi_fastly/get_tls_platform_certificate.py
 pulumi_fastly/get_tls_platform_certificate_ids.py
 pulumi_fastly/get_tls_private_key.py
 pulumi_fastly/get_tls_private_key_ids.py
 pulumi_fastly/get_tls_subscription.py
 pulumi_fastly/get_tls_subscription_ids.py
 pulumi_fastly/get_waf_rules.py
+pulumi_fastly/kvstore.py
 pulumi_fastly/outputs.py
 pulumi_fastly/provider.py
 pulumi_fastly/pulumi-plugin.json
 pulumi_fastly/py.typed
 pulumi_fastly/service_acl_entries.py
 pulumi_fastly/service_authorization.py
 pulumi_fastly/service_compute.py
 pulumi_fastly/service_dictionary_items.py
 pulumi_fastly/service_dynamic_snippet_content.py
 pulumi_fastly/service_vcl.py
 pulumi_fastly/service_waf_configuration.py
 pulumi_fastly/tls_activation.py
 pulumi_fastly/tls_certificate.py
+pulumi_fastly/tls_mutual_authentication.py
 pulumi_fastly/tls_platform_certificate.py
 pulumi_fastly/tls_private_key.py
 pulumi_fastly/tls_subscription.py
 pulumi_fastly/tls_subscription_validation.py
 pulumi_fastly/user.py
 pulumi_fastly.egg-info/PKG-INFO
 pulumi_fastly.egg-info/SOURCES.txt
```

### Comparing `pulumi_fastly-8.1.0a1686634705/setup.py` & `pulumi_fastly-8.1.0a1686825094/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "8.1.0a1686634705"
-PLUGIN_VERSION = "8.1.0-alpha.1686634705+71c7be02"
+VERSION = "8.1.0a1686825094"
+PLUGIN_VERSION = "8.1.0-alpha.1686825094+338b7fea"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'fastly', PLUGIN_VERSION])
         except OSError as error:
```

