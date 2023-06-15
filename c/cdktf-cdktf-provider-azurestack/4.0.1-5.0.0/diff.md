# Comparing `tmp/cdktf-cdktf-provider-azurestack-4.0.1.tar.gz` & `tmp/cdktf-cdktf-provider-azurestack-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-azurestack-4.0.1.tar", last modified: Thu Jun  1 14:17:02 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-azurestack-5.0.0.tar", last modified: Thu Jun 15 11:17:57 2023, max compression
```

## Comparing `cdktf-cdktf-provider-azurestack-4.0.1.tar` & `cdktf-cdktf-provider-azurestack-5.0.0.tar`

### file list

```diff
@@ -1,175 +1,175 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.420901 cdktf-cdktf-provider-azurestack-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:16:47.000000 cdktf-cdktf-provider-azurestack-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-01 14:17:02.416901 cdktf-cdktf-provider-azurestack-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:17:02.420901 cdktf-cdktf-provider-azurestack-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.384899 cdktf-cdktf-provider-azurestack-4.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.396899 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.396899 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1099994 2023-06-01 14:16:47.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/_jsii/provider-azurestack@4.0.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.396899 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/availability_set/
--rw-r--r--   0 runner    (1001) docker     (123)    48334 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/availability_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.396899 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_availability_set/
--rw-r--r--   0 runner    (1001) docker     (123)    30047 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_availability_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.396899 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_client_config/
--rw-r--r--   0 runner    (1001) docker     (123)    25582 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_client_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.396899 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_dns_zone/
--rw-r--r--   0 runner    (1001) docker     (123)    29560 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_dns_zone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.396899 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_image/
--rw-r--r--   0 runner    (1001) docker     (123)    53972 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.396899 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault/
--rw-r--r--   0 runner    (1001) docker     (123)    50477 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.396899 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault_access_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    27651 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault_access_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.396899 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault_key/
--rw-r--r--   0 runner    (1001) docker     (123)    29735 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault_key/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault_secret/
--rw-r--r--   0 runner    (1001) docker     (123)    29460 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault_secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_lb/
--rw-r--r--   0 runner    (1001) docker     (123)    39327 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_lb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_lb_backend_address_pool/
--rw-r--r--   0 runner    (1001) docker     (123)    39260 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_lb_backend_address_pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_lb_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    32694 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_lb_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_local_network_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)    39912 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_local_network_gateway/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_managed_disk/
--rw-r--r--   0 runner    (1001) docker     (123)    32816 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_managed_disk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_network_interface/
--rw-r--r--   0 runner    (1001) docker     (123)    42904 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_network_interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_network_security_group/
--rw-r--r--   0 runner    (1001) docker     (123)    41905 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_network_security_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_platform_image/
--rw-r--r--   0 runner    (1001) docker     (123)    34964 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_platform_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_public_ip/
--rw-r--r--   0 runner    (1001) docker     (123)    32891 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_public_ip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_public_ips/
--rw-r--r--   0 runner    (1001) docker     (123)    47077 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_public_ips/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_resource_group/
--rw-r--r--   0 runner    (1001) docker     (123)    26805 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_resource_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_resources/
--rw-r--r--   0 runner    (1001) docker     (123)    44013 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_route_table/
--rw-r--r--   0 runner    (1001) docker     (123)    38885 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_route_table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_storage_account/
--rw-r--r--   0 runner    (1001) docker     (123)    43149 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_storage_account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_storage_container/
--rw-r--r--   0 runner    (1001) docker     (123)    32560 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_storage_container/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_subnet/
--rw-r--r--   0 runner    (1001) docker     (123)    31400 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_subnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_virtual_network/
--rw-r--r--   0 runner    (1001) docker     (123)    30123 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_virtual_network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_virtual_network_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)    81790 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_virtual_network_gateway/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_virtual_network_gateway_connection/
--rw-r--r--   0 runner    (1001) docker     (123)    44316 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_virtual_network_gateway_connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_a_record/
--rw-r--r--   0 runner    (1001) docker     (123)    43251 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_a_record/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.400900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_aaaa_record/
--rw-r--r--   0 runner    (1001) docker     (123)    43846 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_aaaa_record/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.404900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_cname_record/
--rw-r--r--   0 runner    (1001) docker     (123)    43752 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_cname_record/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.404900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_mx_record/
--rw-r--r--   0 runner    (1001) docker     (123)    58233 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_mx_record/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.404900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_ns_record/
--rw-r--r--   0 runner    (1001) docker     (123)    43365 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_ns_record/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.404900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_ptr_record/
--rw-r--r--   0 runner    (1001) docker     (123)    43479 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_ptr_record/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.404900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_srv_record/
--rw-r--r--   0 runner    (1001) docker     (123)    61446 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_srv_record/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.404900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_txt_record/
--rw-r--r--   0 runner    (1001) docker     (123)    56268 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_txt_record/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.404900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_zone/
--rw-r--r--   0 runner    (1001) docker     (123)    63042 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_zone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.404900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/image/
--rw-r--r--   0 runner    (1001) docker     (123)    83075 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.404900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/key_vault/
--rw-r--r--   0 runner    (1001) docker     (123)   101815 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/key_vault/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.404900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/key_vault_access_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    51717 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/key_vault_access_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.404900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/key_vault_key/
--rw-r--r--   0 runner    (1001) docker     (123)    51599 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/key_vault_key/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.404900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/key_vault_secret/
--rw-r--r--   0 runner    (1001) docker     (123)    46838 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/key_vault_secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.404900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/lb/
--rw-r--r--   0 runner    (1001) docker     (123)    66175 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/lb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.404900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/lb_backend_address_pool/
--rw-r--r--   0 runner    (1001) docker     (123)    38510 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/lb_backend_address_pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.404900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/lb_nat_pool/
--rw-r--r--   0 runner    (1001) docker     (123)    48455 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/lb_nat_pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.404900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/lb_nat_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    52196 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/lb_nat_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.404900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/lb_probe/
--rw-r--r--   0 runner    (1001) docker     (123)    48343 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/lb_probe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.404900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/lb_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    62423 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/lb_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.404900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/linux_virtual_machine/
--rw-r--r--   0 runner    (1001) docker     (123)   214396 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/linux_virtual_machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.408900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/linux_virtual_machine_scale_set/
--rw-r--r--   0 runner    (1001) docker     (123)   374007 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/linux_virtual_machine_scale_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.408900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/local_network_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)    57799 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/local_network_gateway/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.408900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/managed_disk/
--rw-r--r--   0 runner    (1001) docker     (123)    90933 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/managed_disk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.408900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/network_interface/
--rw-r--r--   0 runner    (1001) docker     (123)    76443 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/network_interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.408900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/network_interface_backend_address_pool_association/
--rw-r--r--   0 runner    (1001) docker     (123)    41089 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/network_interface_backend_address_pool_association/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.408900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/network_security_group/
--rw-r--r--   0 runner    (1001) docker     (123)    86137 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/network_security_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.408900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/network_security_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    72226 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/network_security_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.408900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    68187 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.408900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/public_ip/
--rw-r--r--   0 runner    (1001) docker     (123)    56893 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/public_ip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.408900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/resource_group/
--rw-r--r--   0 runner    (1001) docker     (123)    36906 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/resource_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.408900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/route/
--rw-r--r--   0 runner    (1001) docker     (123)    43277 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/route/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.408900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/route_table/
--rw-r--r--   0 runner    (1001) docker     (123)    64573 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/route_table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.408900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/storage_account/
--rw-r--r--   0 runner    (1001) docker     (123)    70508 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/storage_account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.408900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/storage_blob/
--rw-r--r--   0 runner    (1001) docker     (123)    60688 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/storage_blob/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.412900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/storage_container/
--rw-r--r--   0 runner    (1001) docker     (123)    40970 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/storage_container/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.412900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/subnet/
--rw-r--r--   0 runner    (1001) docker     (123)    38636 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/subnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.412900 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/template_deployment/
--rw-r--r--   0 runner    (1001) docker     (123)    45550 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/template_deployment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.416901 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_machine/
--rw-r--r--   0 runner    (1001) docker     (123)   307052 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.416901 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_machine_data_disk_attachment/
--rw-r--r--   0 runner    (1001) docker     (123)    47208 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_machine_data_disk_attachment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.416901 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_machine_extension/
--rw-r--r--   0 runner    (1001) docker     (123)    53509 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_machine_extension/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.416901 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_machine_scale_set/
--rw-r--r--   0 runner    (1001) docker     (123)   434049 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_machine_scale_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.416901 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_machine_scale_set_extension/
--rw-r--r--   0 runner    (1001) docker     (123)    55096 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_machine_scale_set_extension/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.416901 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_network/
--rw-r--r--   0 runner    (1001) docker     (123)    66708 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.416901 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_network_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)   147132 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_network_gateway/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.416901 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_network_gateway_connection/
--rw-r--r--   0 runner    (1001) docker     (123)    95132 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_network_gateway_connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.416901 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_network_peering/
--rw-r--r--   0 runner    (1001) docker     (123)    54469 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_network_peering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.416901 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/windows_virtual_machine/
--rw-r--r--   0 runner    (1001) docker     (123)   239133 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/windows_virtual_machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.416901 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/windows_virtual_machine_scale_set/
--rw-r--r--   0 runner    (1001) docker     (123)   400073 2023-06-01 14:16:48.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/windows_virtual_machine_scale_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:17:02.396899 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-01 14:17:02.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-01 14:17:02.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:17:02.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:17:02.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 14:17:02.000000 cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.697200 cdktf-cdktf-provider-azurestack-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-15 11:17:57.697200 cdktf-cdktf-provider-azurestack-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:17:57.697200 cdktf-cdktf-provider-azurestack-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.669197 cdktf-cdktf-provider-azurestack-5.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.677198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.677198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1099923 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/_jsii/provider-azurestack@5.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.677198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/availability_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    48334 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/availability_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.677198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_availability_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    30047 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_availability_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.677198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_client_config/
+-rw-r--r--   0 runner    (1001) docker     (123)    25582 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_client_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.677198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_dns_zone/
+-rw-r--r--   0 runner    (1001) docker     (123)    29560 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_dns_zone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.681198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_image/
+-rw-r--r--   0 runner    (1001) docker     (123)    53972 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.681198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)    50477 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.681198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault_access_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    27651 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault_access_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.681198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault_key/
+-rw-r--r--   0 runner    (1001) docker     (123)    29735 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault_key/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.681198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault_secret/
+-rw-r--r--   0 runner    (1001) docker     (123)    29460 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault_secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.681198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_lb/
+-rw-r--r--   0 runner    (1001) docker     (123)    39327 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_lb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.681198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_lb_backend_address_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)    39260 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_lb_backend_address_pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.681198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_lb_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    32694 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_lb_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.681198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_local_network_gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)    39912 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_local_network_gateway/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.681198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_managed_disk/
+-rw-r--r--   0 runner    (1001) docker     (123)    32816 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_managed_disk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.681198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_network_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)    42904 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_network_interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.681198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_network_security_group/
+-rw-r--r--   0 runner    (1001) docker     (123)    41905 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_network_security_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.681198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_platform_image/
+-rw-r--r--   0 runner    (1001) docker     (123)    34964 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_platform_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.681198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_public_ip/
+-rw-r--r--   0 runner    (1001) docker     (123)    32891 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_public_ip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.681198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_public_ips/
+-rw-r--r--   0 runner    (1001) docker     (123)    47077 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_public_ips/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.681198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_resource_group/
+-rw-r--r--   0 runner    (1001) docker     (123)    26805 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_resource_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.681198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    44013 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.681198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_route_table/
+-rw-r--r--   0 runner    (1001) docker     (123)    38885 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_route_table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.681198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_storage_account/
+-rw-r--r--   0 runner    (1001) docker     (123)    43149 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_storage_account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.681198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_storage_container/
+-rw-r--r--   0 runner    (1001) docker     (123)    32560 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_storage_container/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.681198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_subnet/
+-rw-r--r--   0 runner    (1001) docker     (123)    31400 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_subnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.685199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_virtual_network/
+-rw-r--r--   0 runner    (1001) docker     (123)    30123 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_virtual_network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.685199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_virtual_network_gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)    81790 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_virtual_network_gateway/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.685199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_virtual_network_gateway_connection/
+-rw-r--r--   0 runner    (1001) docker     (123)    44316 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_virtual_network_gateway_connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.685199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_a_record/
+-rw-r--r--   0 runner    (1001) docker     (123)    43251 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_a_record/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.685199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_aaaa_record/
+-rw-r--r--   0 runner    (1001) docker     (123)    43846 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_aaaa_record/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.685199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_cname_record/
+-rw-r--r--   0 runner    (1001) docker     (123)    43752 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_cname_record/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.685199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_mx_record/
+-rw-r--r--   0 runner    (1001) docker     (123)    58233 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_mx_record/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.685199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_ns_record/
+-rw-r--r--   0 runner    (1001) docker     (123)    43365 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_ns_record/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.685199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_ptr_record/
+-rw-r--r--   0 runner    (1001) docker     (123)    43479 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_ptr_record/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.685199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_srv_record/
+-rw-r--r--   0 runner    (1001) docker     (123)    61446 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_srv_record/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.685199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_txt_record/
+-rw-r--r--   0 runner    (1001) docker     (123)    56268 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_txt_record/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.685199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_zone/
+-rw-r--r--   0 runner    (1001) docker     (123)    63042 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_zone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.685199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/image/
+-rw-r--r--   0 runner    (1001) docker     (123)    83075 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.685199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/key_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)   101815 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/key_vault/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.685199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/key_vault_access_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    51717 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/key_vault_access_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.685199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/key_vault_key/
+-rw-r--r--   0 runner    (1001) docker     (123)    51599 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/key_vault_key/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.685199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/key_vault_secret/
+-rw-r--r--   0 runner    (1001) docker     (123)    46838 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/key_vault_secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.685199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/lb/
+-rw-r--r--   0 runner    (1001) docker     (123)    66175 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/lb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.685199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/lb_backend_address_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)    38510 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/lb_backend_address_pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.685199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/lb_nat_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)    48455 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/lb_nat_pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.689199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/lb_nat_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    52196 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/lb_nat_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.689199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/lb_probe/
+-rw-r--r--   0 runner    (1001) docker     (123)    48343 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/lb_probe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.689199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/lb_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    62423 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/lb_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.689199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/linux_virtual_machine/
+-rw-r--r--   0 runner    (1001) docker     (123)   214396 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/linux_virtual_machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.689199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/linux_virtual_machine_scale_set/
+-rw-r--r--   0 runner    (1001) docker     (123)   374007 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/linux_virtual_machine_scale_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.689199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/local_network_gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)    57799 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/local_network_gateway/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.689199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/managed_disk/
+-rw-r--r--   0 runner    (1001) docker     (123)    90933 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/managed_disk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.689199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/network_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)    76443 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/network_interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.689199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/network_interface_backend_address_pool_association/
+-rw-r--r--   0 runner    (1001) docker     (123)    41089 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/network_interface_backend_address_pool_association/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.689199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/network_security_group/
+-rw-r--r--   0 runner    (1001) docker     (123)    86137 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/network_security_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.689199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/network_security_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    72226 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/network_security_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.689199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    68187 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.689199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/public_ip/
+-rw-r--r--   0 runner    (1001) docker     (123)    56893 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/public_ip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.689199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/resource_group/
+-rw-r--r--   0 runner    (1001) docker     (123)    36906 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/resource_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.689199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/route/
+-rw-r--r--   0 runner    (1001) docker     (123)    43277 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/route/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.689199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/route_table/
+-rw-r--r--   0 runner    (1001) docker     (123)    64573 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/route_table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.693199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/storage_account/
+-rw-r--r--   0 runner    (1001) docker     (123)    70508 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/storage_account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.693199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/storage_blob/
+-rw-r--r--   0 runner    (1001) docker     (123)    60688 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/storage_blob/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.693199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/storage_container/
+-rw-r--r--   0 runner    (1001) docker     (123)    40970 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/storage_container/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.693199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/subnet/
+-rw-r--r--   0 runner    (1001) docker     (123)    38636 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/subnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.693199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/template_deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)    45550 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/template_deployment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.693199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_machine/
+-rw-r--r--   0 runner    (1001) docker     (123)   307052 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.693199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_machine_data_disk_attachment/
+-rw-r--r--   0 runner    (1001) docker     (123)    47208 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_machine_data_disk_attachment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.693199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_machine_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)    53509 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_machine_extension/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.693199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_machine_scale_set/
+-rw-r--r--   0 runner    (1001) docker     (123)   434049 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_machine_scale_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.693199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_machine_scale_set_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)    55096 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_machine_scale_set_extension/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.693199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_network/
+-rw-r--r--   0 runner    (1001) docker     (123)    66708 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.693199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_network_gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)   147132 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_network_gateway/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.693199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_network_gateway_connection/
+-rw-r--r--   0 runner    (1001) docker     (123)    95132 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_network_gateway_connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.693199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_network_peering/
+-rw-r--r--   0 runner    (1001) docker     (123)    54469 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_network_peering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.693199 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/windows_virtual_machine/
+-rw-r--r--   0 runner    (1001) docker     (123)   239133 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/windows_virtual_machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.697200 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/windows_virtual_machine_scale_set/
+-rw-r--r--   0 runner    (1001) docker     (123)   400073 2023-06-15 11:17:43.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/windows_virtual_machine_scale_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:17:57.677198 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-15 11:17:57.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-15 11:17:57.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:17:57.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 11:17:57.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 11:17:57.000000 cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/LICENSE` & `cdktf-cdktf-provider-azurestack-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/PKG-INFO` & `cdktf-cdktf-provider-azurestack-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-azurestack
-Version: 4.0.1
+Version: 5.0.0
 Summary: Prebuilt azurestack Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-azurestack.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-azurestack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/README.md` & `cdktf-cdktf-provider-azurestack-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/setup.py` & `cdktf-cdktf-provider-azurestack-5.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-azurestack",
-    "version": "4.0.1",
+    "version": "5.0.0",
     "description": "Prebuilt azurestack Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-azurestack.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -99,25 +99,25 @@
         "cdktf_cdktf_provider_azurestack.virtual_network_gateway_connection",
         "cdktf_cdktf_provider_azurestack.virtual_network_peering",
         "cdktf_cdktf_provider_azurestack.windows_virtual_machine",
         "cdktf_cdktf_provider_azurestack.windows_virtual_machine_scale_set"
     ],
     "package_data": {
         "cdktf_cdktf_provider_azurestack._jsii": [
-            "provider-azurestack@4.0.1.jsii.tgz"
+            "provider-azurestack@5.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_azurestack": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdktf>=0.16.3, <0.17.0",
+        "cdktf>=0.17.0, <0.18.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.81.0, <2.0.0",
+        "jsii>=1.84.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/availability_set/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/availability_set/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_availability_set/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_availability_set/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_client_config/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_client_config/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_dns_zone/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_dns_zone/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_image/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_image/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault_access_policy/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault_access_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault_key/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault_key/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault_secret/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_lb/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_lb/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_lb_backend_address_pool/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_lb_backend_address_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_lb_rule/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_lb_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_local_network_gateway/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_local_network_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_managed_disk/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_managed_disk/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_network_interface/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_network_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_network_security_group/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_network_security_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_platform_image/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_platform_image/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_public_ip/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_public_ip/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_public_ips/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_public_ips/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_resource_group/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_resource_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_resources/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_route_table/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_route_table/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_storage_account/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_storage_account/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_storage_container/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_storage_container/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_subnet/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_subnet/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_virtual_network/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_virtual_network/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_virtual_network_gateway/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_virtual_network_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/data_azurestack_virtual_network_gateway_connection/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/data_azurestack_virtual_network_gateway_connection/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_a_record/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_a_record/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_aaaa_record/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_aaaa_record/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_cname_record/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_cname_record/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_mx_record/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_mx_record/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_ns_record/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_ns_record/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_ptr_record/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_ptr_record/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_srv_record/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_srv_record/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_txt_record/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_txt_record/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/dns_zone/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/dns_zone/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/image/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/image/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/key_vault/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/key_vault/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/key_vault_access_policy/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/key_vault_access_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/key_vault_key/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/key_vault_key/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/key_vault_secret/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/key_vault_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/lb/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/lb/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/lb_backend_address_pool/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/lb_backend_address_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/lb_nat_pool/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/lb_nat_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/lb_nat_rule/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/lb_nat_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/lb_probe/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/lb_probe/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/lb_rule/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/lb_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/linux_virtual_machine/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/linux_virtual_machine/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/linux_virtual_machine_scale_set/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/linux_virtual_machine_scale_set/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/local_network_gateway/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/local_network_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/managed_disk/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/managed_disk/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/network_interface/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/network_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/network_interface_backend_address_pool_association/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/network_interface_backend_address_pool_association/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/network_security_group/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/network_security_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/network_security_rule/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/network_security_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/provider/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/public_ip/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/public_ip/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/resource_group/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/resource_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/route/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/route/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/route_table/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/route_table/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/storage_account/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/storage_account/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/storage_blob/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/storage_blob/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/storage_container/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/storage_container/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/subnet/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/subnet/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/template_deployment/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/template_deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_machine/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_machine/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_machine_data_disk_attachment/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_machine_data_disk_attachment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_machine_extension/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_machine_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_machine_scale_set/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_machine_scale_set/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_machine_scale_set_extension/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_machine_scale_set_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_network/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_network/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_network_gateway/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_network_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_network_gateway_connection/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_network_gateway_connection/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/virtual_network_peering/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/virtual_network_peering/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/windows_virtual_machine/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/windows_virtual_machine/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack/windows_virtual_machine_scale_set/__init__.py` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack/windows_virtual_machine_scale_set/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack.egg-info/PKG-INFO` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-azurestack
-Version: 4.0.1
+Version: 5.0.0
 Summary: Prebuilt azurestack Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-azurestack.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-azurestack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-azurestack-4.0.1/src/cdktf_cdktf_provider_azurestack.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-azurestack-5.0.0/src/cdktf_cdktf_provider_azurestack.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_azurestack/py.typed
 src/cdktf_cdktf_provider_azurestack.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_azurestack.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_azurestack.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_azurestack.egg-info/requires.txt
 src/cdktf_cdktf_provider_azurestack.egg-info/top_level.txt
 src/cdktf_cdktf_provider_azurestack/_jsii/__init__.py
-src/cdktf_cdktf_provider_azurestack/_jsii/provider-azurestack@4.0.1.jsii.tgz
+src/cdktf_cdktf_provider_azurestack/_jsii/provider-azurestack@5.0.0.jsii.tgz
 src/cdktf_cdktf_provider_azurestack/availability_set/__init__.py
 src/cdktf_cdktf_provider_azurestack/data_azurestack_availability_set/__init__.py
 src/cdktf_cdktf_provider_azurestack/data_azurestack_client_config/__init__.py
 src/cdktf_cdktf_provider_azurestack/data_azurestack_dns_zone/__init__.py
 src/cdktf_cdktf_provider_azurestack/data_azurestack_image/__init__.py
 src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault/__init__.py
 src/cdktf_cdktf_provider_azurestack/data_azurestack_key_vault_access_policy/__init__.py
```

