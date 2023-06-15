# Comparing `tmp/cdktf-cdktf-provider-hcp-4.0.3.tar.gz` & `tmp/cdktf-cdktf-provider-hcp-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-hcp-4.0.3.tar", last modified: Fri Jun  2 14:05:29 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-hcp-5.0.0.tar", last modified: Thu Jun 15 11:25:39 2023, max compression
```

## Comparing `cdktf-cdktf-provider-hcp-4.0.3.tar` & `cdktf-cdktf-provider-hcp-5.0.0.tar`

### file list

```diff
@@ -1,79 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.692085 cdktf-cdktf-provider-hcp-4.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-02 14:05:29.692085 cdktf-cdktf-provider-hcp-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 14:05:29.692085 cdktf-cdktf-provider-hcp-4.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.680085 cdktf-cdktf-provider-hcp-4.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.684085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.684085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   282296 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/_jsii/provider-hcp@4.0.3.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.684085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/aws_network_peering/
--rw-r--r--   0 runner    (1001) docker     (123)    43660 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/aws_network_peering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.684085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/aws_transit_gateway_attachment/
--rw-r--r--   0 runner    (1001) docker     (123)    45014 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/aws_transit_gateway_attachment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/azure_peering_connection/
--rw-r--r--   0 runner    (1001) docker     (123)    47468 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/azure_peering_connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/boundary_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)    55834 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/boundary_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/consul_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)    84679 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/consul_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/consul_cluster_root_token/
--rw-r--r--   0 runner    (1001) docker     (123)    29804 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/consul_cluster_root_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/consul_snapshot/
--rw-r--r--   0 runner    (1001) docker     (123)    38554 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/consul_snapshot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_aws_network_peering/
--rw-r--r--   0 runner    (1001) docker     (123)    36847 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_aws_network_peering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_aws_transit_gateway_attachment/
--rw-r--r--   0 runner    (1001) docker     (123)    38197 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_aws_transit_gateway_attachment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_azure_peering_connection/
--rw-r--r--   0 runner    (1001) docker     (123)    35420 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_azure_peering_connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_boundary_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)    39571 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_boundary_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_helm_config/
--rw-r--r--   0 runner    (1001) docker     (123)    35861 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_helm_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_kubernetes_secret/
--rw-r--r--   0 runner    (1001) docker     (123)    30200 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_kubernetes_secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)    42665 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_versions/
--rw-r--r--   0 runner    (1001) docker     (123)    24777 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_hvn/
--rw-r--r--   0 runner    (1001) docker     (123)    29536 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_hvn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_peering_connection/
--rw-r--r--   0 runner    (1001) docker     (123)    34675 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_peering_connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_route/
--rw-r--r--   0 runner    (1001) docker     (123)    31726 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_route/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image/
--rw-r--r--   0 runner    (1001) docker     (123)    43006 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image_iteration/
--rw-r--r--   0 runner    (1001) docker     (123)    52859 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image_iteration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_packer_iteration/
--rw-r--r--   0 runner    (1001) docker     (123)    32920 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_packer_iteration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_vault_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)    71370 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_vault_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/hvn/
--rw-r--r--   0 runner    (1001) docker     (123)    39932 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/hvn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/hvn_peering_connection/
--rw-r--r--   0 runner    (1001) docker     (123)    36582 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/hvn_peering_connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/hvn_route/
--rw-r--r--   0 runner    (1001) docker     (123)    40310 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/hvn_route/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/packer_channel/
--rw-r--r--   0 runner    (1001) docker     (123)    52254 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/packer_channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.688085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/vault_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)   119768 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/vault_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.692085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/vault_cluster_admin_token/
--rw-r--r--   0 runner    (1001) docker     (123)    33953 2023-06-02 14:05:16.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/vault_cluster_admin_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:05:29.684085 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-02 14:05:29.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-02 14:05:29.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:05:29.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-02 14:05:29.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-02 14:05:29.000000 cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.220932 cdktf-cdktf-provider-hcp-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-15 11:25:39.220932 cdktf-cdktf-provider-hcp-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:25:39.220932 cdktf-cdktf-provider-hcp-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.212931 cdktf-cdktf-provider-hcp-5.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.212931 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.216932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   286086 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/_jsii/provider-hcp@5.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.216932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/aws_network_peering/
+-rw-r--r--   0 runner    (1001) docker     (123)    43660 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/aws_network_peering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.216932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/aws_transit_gateway_attachment/
+-rw-r--r--   0 runner    (1001) docker     (123)    45014 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/aws_transit_gateway_attachment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.216932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/azure_peering_connection/
+-rw-r--r--   0 runner    (1001) docker     (123)    47468 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/azure_peering_connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.216932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/boundary_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)    55834 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/boundary_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.216932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/consul_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)    84679 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/consul_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.216932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/consul_cluster_root_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    29804 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/consul_cluster_root_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.216932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/consul_snapshot/
+-rw-r--r--   0 runner    (1001) docker     (123)    38554 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/consul_snapshot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.216932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_aws_network_peering/
+-rw-r--r--   0 runner    (1001) docker     (123)    36847 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_aws_network_peering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.216932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_aws_transit_gateway_attachment/
+-rw-r--r--   0 runner    (1001) docker     (123)    38197 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_aws_transit_gateway_attachment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.216932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_azure_peering_connection/
+-rw-r--r--   0 runner    (1001) docker     (123)    35420 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_azure_peering_connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.216932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_boundary_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)    39571 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_boundary_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.216932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_helm_config/
+-rw-r--r--   0 runner    (1001) docker     (123)    35861 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_helm_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.216932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_kubernetes_secret/
+-rw-r--r--   0 runner    (1001) docker     (123)    30200 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_kubernetes_secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.216932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)    42665 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.216932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_versions/
+-rw-r--r--   0 runner    (1001) docker     (123)    24777 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.216932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_hvn/
+-rw-r--r--   0 runner    (1001) docker     (123)    29536 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_hvn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.216932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_peering_connection/
+-rw-r--r--   0 runner    (1001) docker     (123)    35540 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_peering_connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.216932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_route/
+-rw-r--r--   0 runner    (1001) docker     (123)    32125 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_route/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.220932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image/
+-rw-r--r--   0 runner    (1001) docker     (123)    43006 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.220932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image_iteration/
+-rw-r--r--   0 runner    (1001) docker     (123)    52859 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image_iteration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.220932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_packer_iteration/
+-rw-r--r--   0 runner    (1001) docker     (123)    32920 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_packer_iteration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.220932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_vault_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)    71370 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_vault_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.220932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_vault_secrets_app/
+-rw-r--r--   0 runner    (1001) docker     (123)    18603 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_vault_secrets_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.220932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/hvn/
+-rw-r--r--   0 runner    (1001) docker     (123)    39932 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/hvn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.220932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/hvn_peering_connection/
+-rw-r--r--   0 runner    (1001) docker     (123)    36933 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/hvn_peering_connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.220932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/hvn_route/
+-rw-r--r--   0 runner    (1001) docker     (123)    40709 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/hvn_route/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.220932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/packer_channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    52254 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/packer_channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.220932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.220932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/vault_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)   119768 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/vault_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.220932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/vault_cluster_admin_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    33953 2023-06-15 11:25:24.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/vault_cluster_admin_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:25:39.216932 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-15 11:25:39.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-15 11:25:39.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:25:39.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 11:25:39.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 11:25:39.000000 cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/LICENSE` & `cdktf-cdktf-provider-hcp-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/PKG-INFO` & `cdktf-cdktf-provider-hcp-5.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-hcp
-Version: 4.0.3
+Version: 5.0.0
 Summary: Prebuilt hcp Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-hcp.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-hcp.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/README.md` & `cdktf-cdktf-provider-hcp-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/setup.py` & `cdktf-cdktf-provider-hcp-5.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-hcp",
-    "version": "4.0.3",
+    "version": "5.0.0",
     "description": "Prebuilt hcp Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-hcp.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -41,35 +41,36 @@
         "cdktf_cdktf_provider_hcp.data_hcp_hvn",
         "cdktf_cdktf_provider_hcp.data_hcp_hvn_peering_connection",
         "cdktf_cdktf_provider_hcp.data_hcp_hvn_route",
         "cdktf_cdktf_provider_hcp.data_hcp_packer_image",
         "cdktf_cdktf_provider_hcp.data_hcp_packer_image_iteration",
         "cdktf_cdktf_provider_hcp.data_hcp_packer_iteration",
         "cdktf_cdktf_provider_hcp.data_hcp_vault_cluster",
+        "cdktf_cdktf_provider_hcp.data_hcp_vault_secrets_app",
         "cdktf_cdktf_provider_hcp.hvn",
         "cdktf_cdktf_provider_hcp.hvn_peering_connection",
         "cdktf_cdktf_provider_hcp.hvn_route",
         "cdktf_cdktf_provider_hcp.packer_channel",
         "cdktf_cdktf_provider_hcp.provider",
         "cdktf_cdktf_provider_hcp.vault_cluster",
         "cdktf_cdktf_provider_hcp.vault_cluster_admin_token"
     ],
     "package_data": {
         "cdktf_cdktf_provider_hcp._jsii": [
-            "provider-hcp@4.0.3.jsii.tgz"
+            "provider-hcp@5.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_hcp": [
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

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,15 @@
     "data_hcp_hvn",
     "data_hcp_hvn_peering_connection",
     "data_hcp_hvn_route",
     "data_hcp_packer_image",
     "data_hcp_packer_image_iteration",
     "data_hcp_packer_iteration",
     "data_hcp_vault_cluster",
+    "data_hcp_vault_secrets_app",
     "hvn",
     "hvn_peering_connection",
     "hvn_route",
     "packer_channel",
     "provider",
     "vault_cluster",
     "vault_cluster_admin_token",
@@ -159,14 +160,15 @@
 from . import data_hcp_hvn
 from . import data_hcp_hvn_peering_connection
 from . import data_hcp_hvn_route
 from . import data_hcp_packer_image
 from . import data_hcp_packer_image_iteration
 from . import data_hcp_packer_iteration
 from . import data_hcp_vault_cluster
+from . import data_hcp_vault_secrets_app
 from . import hvn
 from . import hvn_peering_connection
 from . import hvn_route
 from . import packer_channel
 from . import provider
 from . import vault_cluster
 from . import vault_cluster_admin_token
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/aws_network_peering/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/aws_network_peering/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_aws_network_peering`
 
-Refer to the Terraform Registory for docs: [`hcp_aws_network_peering`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering).
+Refer to the Terraform Registory for docs: [`hcp_aws_network_peering`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class AwsNetworkPeering(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.awsNetworkPeering.AwsNetworkPeering",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering hcp_aws_network_peering}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering hcp_aws_network_peering}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         hvn_id: builtins.str,
@@ -45,26 +45,26 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering hcp_aws_network_peering} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering hcp_aws_network_peering} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#hvn_id AwsNetworkPeering#hvn_id}
-        :param peer_account_id: The account ID of the peer VPC in AWS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#peer_account_id AwsNetworkPeering#peer_account_id}
-        :param peering_id: The ID of the network peering. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#peering_id AwsNetworkPeering#peering_id}
-        :param peer_vpc_id: The ID of the peer VPC in AWS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#peer_vpc_id AwsNetworkPeering#peer_vpc_id}
-        :param peer_vpc_region: The region of the peer VPC in AWS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#peer_vpc_region AwsNetworkPeering#peer_vpc_region}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#id AwsNetworkPeering#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the network peering is located. Always matches the HVN's project. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#project_id AwsNetworkPeering#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#timeouts AwsNetworkPeering#timeouts}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#hvn_id AwsNetworkPeering#hvn_id}
+        :param peer_account_id: The account ID of the peer VPC in AWS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#peer_account_id AwsNetworkPeering#peer_account_id}
+        :param peering_id: The ID of the network peering. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#peering_id AwsNetworkPeering#peering_id}
+        :param peer_vpc_id: The ID of the peer VPC in AWS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#peer_vpc_id AwsNetworkPeering#peer_vpc_id}
+        :param peer_vpc_region: The region of the peer VPC in AWS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#peer_vpc_region AwsNetworkPeering#peer_vpc_region}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#id AwsNetworkPeering#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the network peering is located. Always matches the HVN's project. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#project_id AwsNetworkPeering#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#timeouts AwsNetworkPeering#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -98,17 +98,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#create AwsNetworkPeering#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#default AwsNetworkPeering#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#delete AwsNetworkPeering#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#create AwsNetworkPeering#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#default AwsNetworkPeering#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#delete AwsNetworkPeering#delete}.
         '''
         value = AwsNetworkPeeringTimeouts(
             create=create, default=default, delete=delete
         )
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
@@ -340,22 +340,22 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#hvn_id AwsNetworkPeering#hvn_id}
-        :param peer_account_id: The account ID of the peer VPC in AWS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#peer_account_id AwsNetworkPeering#peer_account_id}
-        :param peering_id: The ID of the network peering. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#peering_id AwsNetworkPeering#peering_id}
-        :param peer_vpc_id: The ID of the peer VPC in AWS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#peer_vpc_id AwsNetworkPeering#peer_vpc_id}
-        :param peer_vpc_region: The region of the peer VPC in AWS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#peer_vpc_region AwsNetworkPeering#peer_vpc_region}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#id AwsNetworkPeering#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the network peering is located. Always matches the HVN's project. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#project_id AwsNetworkPeering#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#timeouts AwsNetworkPeering#timeouts}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#hvn_id AwsNetworkPeering#hvn_id}
+        :param peer_account_id: The account ID of the peer VPC in AWS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#peer_account_id AwsNetworkPeering#peer_account_id}
+        :param peering_id: The ID of the network peering. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#peering_id AwsNetworkPeering#peering_id}
+        :param peer_vpc_id: The ID of the peer VPC in AWS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#peer_vpc_id AwsNetworkPeering#peer_vpc_id}
+        :param peer_vpc_region: The region of the peer VPC in AWS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#peer_vpc_region AwsNetworkPeering#peer_vpc_region}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#id AwsNetworkPeering#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the network peering is located. Always matches the HVN's project. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#project_id AwsNetworkPeering#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#timeouts AwsNetworkPeering#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = AwsNetworkPeeringTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b9c17948df4b1bafb7d97d68e6ba1b74034b5b1e7e0ed633ac481576c3f6d8b4)
@@ -466,84 +466,84 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def hvn_id(self) -> builtins.str:
         '''The ID of the HashiCorp Virtual Network (HVN).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#hvn_id AwsNetworkPeering#hvn_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#hvn_id AwsNetworkPeering#hvn_id}
         '''
         result = self._values.get("hvn_id")
         assert result is not None, "Required property 'hvn_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peer_account_id(self) -> builtins.str:
         '''The account ID of the peer VPC in AWS.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#peer_account_id AwsNetworkPeering#peer_account_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#peer_account_id AwsNetworkPeering#peer_account_id}
         '''
         result = self._values.get("peer_account_id")
         assert result is not None, "Required property 'peer_account_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peering_id(self) -> builtins.str:
         '''The ID of the network peering.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#peering_id AwsNetworkPeering#peering_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#peering_id AwsNetworkPeering#peering_id}
         '''
         result = self._values.get("peering_id")
         assert result is not None, "Required property 'peering_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peer_vpc_id(self) -> builtins.str:
         '''The ID of the peer VPC in AWS.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#peer_vpc_id AwsNetworkPeering#peer_vpc_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#peer_vpc_id AwsNetworkPeering#peer_vpc_id}
         '''
         result = self._values.get("peer_vpc_id")
         assert result is not None, "Required property 'peer_vpc_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peer_vpc_region(self) -> builtins.str:
         '''The region of the peer VPC in AWS.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#peer_vpc_region AwsNetworkPeering#peer_vpc_region}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#peer_vpc_region AwsNetworkPeering#peer_vpc_region}
         '''
         result = self._values.get("peer_vpc_region")
         assert result is not None, "Required property 'peer_vpc_region' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#id AwsNetworkPeering#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#id AwsNetworkPeering#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the network peering is located. Always matches the HVN's project.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#project_id AwsNetworkPeering#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#project_id AwsNetworkPeering#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["AwsNetworkPeeringTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#timeouts AwsNetworkPeering#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#timeouts AwsNetworkPeering#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["AwsNetworkPeeringTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -566,17 +566,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#create AwsNetworkPeering#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#default AwsNetworkPeering#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#delete AwsNetworkPeering#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#create AwsNetworkPeering#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#default AwsNetworkPeering#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#delete AwsNetworkPeering#delete}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b0806ef2cb0a231646e95e4e369115a214ea50b4cb68f673ea8486daac15fe09)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -585,27 +585,27 @@
         if default is not None:
             self._values["default"] = default
         if delete is not None:
             self._values["delete"] = delete
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#create AwsNetworkPeering#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#create AwsNetworkPeering#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#default AwsNetworkPeering#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#default AwsNetworkPeering#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_network_peering#delete AwsNetworkPeering#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_network_peering#delete AwsNetworkPeering#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/aws_transit_gateway_attachment/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/aws_transit_gateway_attachment/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_aws_transit_gateway_attachment`
 
-Refer to the Terraform Registory for docs: [`hcp_aws_transit_gateway_attachment`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment).
+Refer to the Terraform Registory for docs: [`hcp_aws_transit_gateway_attachment`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class AwsTransitGatewayAttachment(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.awsTransitGatewayAttachment.AwsTransitGatewayAttachment",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment hcp_aws_transit_gateway_attachment}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment hcp_aws_transit_gateway_attachment}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         hvn_id: builtins.str,
@@ -44,25 +44,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment hcp_aws_transit_gateway_attachment} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment hcp_aws_transit_gateway_attachment} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#hvn_id AwsTransitGatewayAttachment#hvn_id}
-        :param resource_share_arn: The Amazon Resource Name (ARN) of the Resource Share that is needed to grant HCP access to the transit gateway in AWS. The Resource Share should be associated with the HCP AWS account principal (see `aws_ram_principal_association <https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ram_principal_association>`_) and the transit gateway resource (see `aws_ram_resource_association <https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ram_resource_association>`_) Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#resource_share_arn AwsTransitGatewayAttachment#resource_share_arn}
-        :param transit_gateway_attachment_id: The user-settable name of the transit gateway attachment in HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#transit_gateway_attachment_id AwsTransitGatewayAttachment#transit_gateway_attachment_id}
-        :param transit_gateway_id: The ID of the user-owned transit gateway in AWS. The AWS region of the transit gateway must match the HVN. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#transit_gateway_id AwsTransitGatewayAttachment#transit_gateway_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#id AwsTransitGatewayAttachment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the transit gateway attachment is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#project_id AwsTransitGatewayAttachment#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#timeouts AwsTransitGatewayAttachment#timeouts}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#hvn_id AwsTransitGatewayAttachment#hvn_id}
+        :param resource_share_arn: The Amazon Resource Name (ARN) of the Resource Share that is needed to grant HCP access to the transit gateway in AWS. The Resource Share should be associated with the HCP AWS account principal (see `aws_ram_principal_association <https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ram_principal_association>`_) and the transit gateway resource (see `aws_ram_resource_association <https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ram_resource_association>`_) Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#resource_share_arn AwsTransitGatewayAttachment#resource_share_arn}
+        :param transit_gateway_attachment_id: The user-settable name of the transit gateway attachment in HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#transit_gateway_attachment_id AwsTransitGatewayAttachment#transit_gateway_attachment_id}
+        :param transit_gateway_id: The ID of the user-owned transit gateway in AWS. The AWS region of the transit gateway must match the HVN. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#transit_gateway_id AwsTransitGatewayAttachment#transit_gateway_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#id AwsTransitGatewayAttachment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the transit gateway attachment is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#project_id AwsTransitGatewayAttachment#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#timeouts AwsTransitGatewayAttachment#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -95,17 +95,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#create AwsTransitGatewayAttachment#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#default AwsTransitGatewayAttachment#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#delete AwsTransitGatewayAttachment#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#create AwsTransitGatewayAttachment#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#default AwsTransitGatewayAttachment#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#delete AwsTransitGatewayAttachment#delete}.
         '''
         value = AwsTransitGatewayAttachmentTimeouts(
             create=create, default=default, delete=delete
         )
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
@@ -318,21 +318,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#hvn_id AwsTransitGatewayAttachment#hvn_id}
-        :param resource_share_arn: The Amazon Resource Name (ARN) of the Resource Share that is needed to grant HCP access to the transit gateway in AWS. The Resource Share should be associated with the HCP AWS account principal (see `aws_ram_principal_association <https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ram_principal_association>`_) and the transit gateway resource (see `aws_ram_resource_association <https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ram_resource_association>`_) Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#resource_share_arn AwsTransitGatewayAttachment#resource_share_arn}
-        :param transit_gateway_attachment_id: The user-settable name of the transit gateway attachment in HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#transit_gateway_attachment_id AwsTransitGatewayAttachment#transit_gateway_attachment_id}
-        :param transit_gateway_id: The ID of the user-owned transit gateway in AWS. The AWS region of the transit gateway must match the HVN. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#transit_gateway_id AwsTransitGatewayAttachment#transit_gateway_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#id AwsTransitGatewayAttachment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the transit gateway attachment is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#project_id AwsTransitGatewayAttachment#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#timeouts AwsTransitGatewayAttachment#timeouts}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#hvn_id AwsTransitGatewayAttachment#hvn_id}
+        :param resource_share_arn: The Amazon Resource Name (ARN) of the Resource Share that is needed to grant HCP access to the transit gateway in AWS. The Resource Share should be associated with the HCP AWS account principal (see `aws_ram_principal_association <https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ram_principal_association>`_) and the transit gateway resource (see `aws_ram_resource_association <https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ram_resource_association>`_) Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#resource_share_arn AwsTransitGatewayAttachment#resource_share_arn}
+        :param transit_gateway_attachment_id: The user-settable name of the transit gateway attachment in HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#transit_gateway_attachment_id AwsTransitGatewayAttachment#transit_gateway_attachment_id}
+        :param transit_gateway_id: The ID of the user-owned transit gateway in AWS. The AWS region of the transit gateway must match the HVN. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#transit_gateway_id AwsTransitGatewayAttachment#transit_gateway_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#id AwsTransitGatewayAttachment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the transit gateway attachment is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#project_id AwsTransitGatewayAttachment#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#timeouts AwsTransitGatewayAttachment#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = AwsTransitGatewayAttachmentTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e20715d2f0d81810af99b1e2ec8ab5ff9b9100521407d7dfa1313b227c18af53)
@@ -441,78 +441,78 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def hvn_id(self) -> builtins.str:
         '''The ID of the HashiCorp Virtual Network (HVN).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#hvn_id AwsTransitGatewayAttachment#hvn_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#hvn_id AwsTransitGatewayAttachment#hvn_id}
         '''
         result = self._values.get("hvn_id")
         assert result is not None, "Required property 'hvn_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def resource_share_arn(self) -> builtins.str:
         '''The Amazon Resource Name (ARN) of the Resource Share that is needed to grant HCP access to the transit gateway in AWS.
 
         The Resource Share should be associated with the HCP AWS account principal (see `aws_ram_principal_association <https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ram_principal_association>`_) and the transit gateway resource (see `aws_ram_resource_association <https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/ram_resource_association>`_)
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#resource_share_arn AwsTransitGatewayAttachment#resource_share_arn}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#resource_share_arn AwsTransitGatewayAttachment#resource_share_arn}
         '''
         result = self._values.get("resource_share_arn")
         assert result is not None, "Required property 'resource_share_arn' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def transit_gateway_attachment_id(self) -> builtins.str:
         '''The user-settable name of the transit gateway attachment in HCP.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#transit_gateway_attachment_id AwsTransitGatewayAttachment#transit_gateway_attachment_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#transit_gateway_attachment_id AwsTransitGatewayAttachment#transit_gateway_attachment_id}
         '''
         result = self._values.get("transit_gateway_attachment_id")
         assert result is not None, "Required property 'transit_gateway_attachment_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def transit_gateway_id(self) -> builtins.str:
         '''The ID of the user-owned transit gateway in AWS.
 
         The AWS region of the transit gateway must match the HVN.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#transit_gateway_id AwsTransitGatewayAttachment#transit_gateway_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#transit_gateway_id AwsTransitGatewayAttachment#transit_gateway_id}
         '''
         result = self._values.get("transit_gateway_id")
         assert result is not None, "Required property 'transit_gateway_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#id AwsTransitGatewayAttachment#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#id AwsTransitGatewayAttachment#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the transit gateway attachment is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#project_id AwsTransitGatewayAttachment#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#project_id AwsTransitGatewayAttachment#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["AwsTransitGatewayAttachmentTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#timeouts AwsTransitGatewayAttachment#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#timeouts AwsTransitGatewayAttachment#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["AwsTransitGatewayAttachmentTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -535,17 +535,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#create AwsTransitGatewayAttachment#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#default AwsTransitGatewayAttachment#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#delete AwsTransitGatewayAttachment#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#create AwsTransitGatewayAttachment#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#default AwsTransitGatewayAttachment#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#delete AwsTransitGatewayAttachment#delete}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ccdd66f27acdf06d50d9f4079bbf0ba1b927640ff31a49119b05b5c03c92f45d)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -554,27 +554,27 @@
         if default is not None:
             self._values["default"] = default
         if delete is not None:
             self._values["delete"] = delete
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#create AwsTransitGatewayAttachment#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#create AwsTransitGatewayAttachment#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#default AwsTransitGatewayAttachment#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#default AwsTransitGatewayAttachment#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/aws_transit_gateway_attachment#delete AwsTransitGatewayAttachment#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/aws_transit_gateway_attachment#delete AwsTransitGatewayAttachment#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/azure_peering_connection/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/azure_peering_connection/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_azure_peering_connection`
 
-Refer to the Terraform Registory for docs: [`hcp_azure_peering_connection`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection).
+Refer to the Terraform Registory for docs: [`hcp_azure_peering_connection`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class AzurePeeringConnection(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.azurePeeringConnection.AzurePeeringConnection",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection hcp_azure_peering_connection}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection hcp_azure_peering_connection}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         hvn_link: builtins.str,
@@ -46,27 +46,27 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection hcp_azure_peering_connection} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection hcp_azure_peering_connection} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#hvn_link AzurePeeringConnection#hvn_link}
-        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#peering_id AzurePeeringConnection#peering_id}
-        :param peer_resource_group_name: The resource group name of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#peer_resource_group_name AzurePeeringConnection#peer_resource_group_name}
-        :param peer_subscription_id: The subscription ID of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#peer_subscription_id AzurePeeringConnection#peer_subscription_id}
-        :param peer_tenant_id: The tenant ID of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#peer_tenant_id AzurePeeringConnection#peer_tenant_id}
-        :param peer_vnet_name: The name of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#peer_vnet_name AzurePeeringConnection#peer_vnet_name}
-        :param peer_vnet_region: The region of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#peer_vnet_region AzurePeeringConnection#peer_vnet_region}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#id AzurePeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#timeouts AzurePeeringConnection#timeouts}
+        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#hvn_link AzurePeeringConnection#hvn_link}
+        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#peering_id AzurePeeringConnection#peering_id}
+        :param peer_resource_group_name: The resource group name of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#peer_resource_group_name AzurePeeringConnection#peer_resource_group_name}
+        :param peer_subscription_id: The subscription ID of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#peer_subscription_id AzurePeeringConnection#peer_subscription_id}
+        :param peer_tenant_id: The tenant ID of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#peer_tenant_id AzurePeeringConnection#peer_tenant_id}
+        :param peer_vnet_name: The name of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#peer_vnet_name AzurePeeringConnection#peer_vnet_name}
+        :param peer_vnet_region: The region of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#peer_vnet_region AzurePeeringConnection#peer_vnet_region}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#id AzurePeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#timeouts AzurePeeringConnection#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -101,17 +101,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#create AzurePeeringConnection#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#default AzurePeeringConnection#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#delete AzurePeeringConnection#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#create AzurePeeringConnection#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#default AzurePeeringConnection#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#delete AzurePeeringConnection#delete}.
         '''
         value = AzurePeeringConnectionTimeouts(
             create=create, default=default, delete=delete
         )
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
@@ -368,23 +368,23 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#hvn_link AzurePeeringConnection#hvn_link}
-        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#peering_id AzurePeeringConnection#peering_id}
-        :param peer_resource_group_name: The resource group name of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#peer_resource_group_name AzurePeeringConnection#peer_resource_group_name}
-        :param peer_subscription_id: The subscription ID of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#peer_subscription_id AzurePeeringConnection#peer_subscription_id}
-        :param peer_tenant_id: The tenant ID of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#peer_tenant_id AzurePeeringConnection#peer_tenant_id}
-        :param peer_vnet_name: The name of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#peer_vnet_name AzurePeeringConnection#peer_vnet_name}
-        :param peer_vnet_region: The region of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#peer_vnet_region AzurePeeringConnection#peer_vnet_region}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#id AzurePeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#timeouts AzurePeeringConnection#timeouts}
+        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#hvn_link AzurePeeringConnection#hvn_link}
+        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#peering_id AzurePeeringConnection#peering_id}
+        :param peer_resource_group_name: The resource group name of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#peer_resource_group_name AzurePeeringConnection#peer_resource_group_name}
+        :param peer_subscription_id: The subscription ID of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#peer_subscription_id AzurePeeringConnection#peer_subscription_id}
+        :param peer_tenant_id: The tenant ID of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#peer_tenant_id AzurePeeringConnection#peer_tenant_id}
+        :param peer_vnet_name: The name of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#peer_vnet_name AzurePeeringConnection#peer_vnet_name}
+        :param peer_vnet_region: The region of the peer VNet in Azure. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#peer_vnet_region AzurePeeringConnection#peer_vnet_region}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#id AzurePeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#timeouts AzurePeeringConnection#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = AzurePeeringConnectionTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__fdeca02ceccf49e104c97dbf97368fcb5bf7c3b9bdbe2658f3fe03d7beaf4990)
@@ -496,95 +496,95 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def hvn_link(self) -> builtins.str:
         '''The ``self_link`` of the HashiCorp Virtual Network (HVN).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#hvn_link AzurePeeringConnection#hvn_link}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#hvn_link AzurePeeringConnection#hvn_link}
         '''
         result = self._values.get("hvn_link")
         assert result is not None, "Required property 'hvn_link' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peering_id(self) -> builtins.str:
         '''The ID of the peering connection.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#peering_id AzurePeeringConnection#peering_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#peering_id AzurePeeringConnection#peering_id}
         '''
         result = self._values.get("peering_id")
         assert result is not None, "Required property 'peering_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peer_resource_group_name(self) -> builtins.str:
         '''The resource group name of the peer VNet in Azure.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#peer_resource_group_name AzurePeeringConnection#peer_resource_group_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#peer_resource_group_name AzurePeeringConnection#peer_resource_group_name}
         '''
         result = self._values.get("peer_resource_group_name")
         assert result is not None, "Required property 'peer_resource_group_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peer_subscription_id(self) -> builtins.str:
         '''The subscription ID of the peer VNet in Azure.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#peer_subscription_id AzurePeeringConnection#peer_subscription_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#peer_subscription_id AzurePeeringConnection#peer_subscription_id}
         '''
         result = self._values.get("peer_subscription_id")
         assert result is not None, "Required property 'peer_subscription_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peer_tenant_id(self) -> builtins.str:
         '''The tenant ID of the peer VNet in Azure.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#peer_tenant_id AzurePeeringConnection#peer_tenant_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#peer_tenant_id AzurePeeringConnection#peer_tenant_id}
         '''
         result = self._values.get("peer_tenant_id")
         assert result is not None, "Required property 'peer_tenant_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peer_vnet_name(self) -> builtins.str:
         '''The name of the peer VNet in Azure.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#peer_vnet_name AzurePeeringConnection#peer_vnet_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#peer_vnet_name AzurePeeringConnection#peer_vnet_name}
         '''
         result = self._values.get("peer_vnet_name")
         assert result is not None, "Required property 'peer_vnet_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peer_vnet_region(self) -> builtins.str:
         '''The region of the peer VNet in Azure.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#peer_vnet_region AzurePeeringConnection#peer_vnet_region}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#peer_vnet_region AzurePeeringConnection#peer_vnet_region}
         '''
         result = self._values.get("peer_vnet_region")
         assert result is not None, "Required property 'peer_vnet_region' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#id AzurePeeringConnection#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#id AzurePeeringConnection#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["AzurePeeringConnectionTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#timeouts AzurePeeringConnection#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#timeouts AzurePeeringConnection#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["AzurePeeringConnectionTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -607,17 +607,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#create AzurePeeringConnection#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#default AzurePeeringConnection#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#delete AzurePeeringConnection#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#create AzurePeeringConnection#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#default AzurePeeringConnection#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#delete AzurePeeringConnection#delete}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__127f56bb37ab835fef1b18188f7621a124d0fb401d1e629d1300d24f99ad3d39)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -626,27 +626,27 @@
         if default is not None:
             self._values["default"] = default
         if delete is not None:
             self._values["delete"] = delete
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#create AzurePeeringConnection#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#create AzurePeeringConnection#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#default AzurePeeringConnection#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#default AzurePeeringConnection#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/azure_peering_connection#delete AzurePeeringConnection#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/azure_peering_connection#delete AzurePeeringConnection#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/boundary_cluster/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/boundary_cluster/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_boundary_cluster`
 
-Refer to the Terraform Registory for docs: [`hcp_boundary_cluster`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster).
+Refer to the Terraform Registory for docs: [`hcp_boundary_cluster`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class BoundaryCluster(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.boundaryCluster.BoundaryCluster",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster hcp_boundary_cluster}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster hcp_boundary_cluster}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_id: builtins.str,
@@ -44,25 +44,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster hcp_boundary_cluster} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster hcp_boundary_cluster} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_id: The ID of the Boundary cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#cluster_id BoundaryCluster#cluster_id}
-        :param password: The password of the initial admin user. This must be at least 8 characters in length. Note that this may show up in logs, and it will be stored in the state file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#password BoundaryCluster#password}
-        :param username: The username of the initial admin user. This must be at least 3 characters in length, alphanumeric, hyphen, or period. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#username BoundaryCluster#username}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#id BoundaryCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param maintenance_window_config: maintenance_window_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#maintenance_window_config BoundaryCluster#maintenance_window_config}
-        :param project_id: The ID of the HCP project where the Boundary cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#project_id BoundaryCluster#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#timeouts BoundaryCluster#timeouts}
+        :param cluster_id: The ID of the Boundary cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#cluster_id BoundaryCluster#cluster_id}
+        :param password: The password of the initial admin user. This must be at least 8 characters in length. Note that this may show up in logs, and it will be stored in the state file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#password BoundaryCluster#password}
+        :param username: The username of the initial admin user. This must be at least 3 characters in length, alphanumeric, hyphen, or period. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#username BoundaryCluster#username}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#id BoundaryCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param maintenance_window_config: maintenance_window_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#maintenance_window_config BoundaryCluster#maintenance_window_config}
+        :param project_id: The ID of the HCP project where the Boundary cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#project_id BoundaryCluster#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#timeouts BoundaryCluster#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -96,18 +96,18 @@
         *,
         day: typing.Optional[builtins.str] = None,
         end: typing.Optional[jsii.Number] = None,
         start: typing.Optional[jsii.Number] = None,
         upgrade_type: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param day: The maintenance day of the week for scheduled upgrades. Valid options for maintenance window day - ``MONDAY``, ``TUESDAY``, ``WEDNESDAY``, ``THURSDAY``, ``FRIDAY``, ``SATURDAY``, ``SUNDAY`` Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#day BoundaryCluster#day}
-        :param end: The end time which upgrades can be performed. Uses 24H clock and must be in UTC time zone. Valid options include - 1 to 24 (inclusive) Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#end BoundaryCluster#end}
-        :param start: The start time which upgrades can be performed. Uses 24H clock and must be in UTC time zone. Valid options include - 0 to 23 (inclusive) Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#start BoundaryCluster#start}
-        :param upgrade_type: The upgrade type for the cluster. Valid options for upgrade type - ``AUTOMATIC``, ``SCHEDULED``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#upgrade_type BoundaryCluster#upgrade_type}
+        :param day: The maintenance day of the week for scheduled upgrades. Valid options for maintenance window day - ``MONDAY``, ``TUESDAY``, ``WEDNESDAY``, ``THURSDAY``, ``FRIDAY``, ``SATURDAY``, ``SUNDAY`` Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#day BoundaryCluster#day}
+        :param end: The end time which upgrades can be performed. Uses 24H clock and must be in UTC time zone. Valid options include - 1 to 24 (inclusive) Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#end BoundaryCluster#end}
+        :param start: The start time which upgrades can be performed. Uses 24H clock and must be in UTC time zone. Valid options include - 0 to 23 (inclusive) Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#start BoundaryCluster#start}
+        :param upgrade_type: The upgrade type for the cluster. Valid options for upgrade type - ``AUTOMATIC``, ``SCHEDULED``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#upgrade_type BoundaryCluster#upgrade_type}
         '''
         value = BoundaryClusterMaintenanceWindowConfig(
             day=day, end=end, start=start, upgrade_type=upgrade_type
         )
 
         return typing.cast(None, jsii.invoke(self, "putMaintenanceWindowConfig", [value]))
 
@@ -116,17 +116,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#create BoundaryCluster#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#default BoundaryCluster#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#delete BoundaryCluster#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#create BoundaryCluster#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#default BoundaryCluster#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#delete BoundaryCluster#delete}.
         '''
         value = BoundaryClusterTimeouts(create=create, default=default, delete=delete)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -323,21 +323,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_id: The ID of the Boundary cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#cluster_id BoundaryCluster#cluster_id}
-        :param password: The password of the initial admin user. This must be at least 8 characters in length. Note that this may show up in logs, and it will be stored in the state file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#password BoundaryCluster#password}
-        :param username: The username of the initial admin user. This must be at least 3 characters in length, alphanumeric, hyphen, or period. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#username BoundaryCluster#username}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#id BoundaryCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param maintenance_window_config: maintenance_window_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#maintenance_window_config BoundaryCluster#maintenance_window_config}
-        :param project_id: The ID of the HCP project where the Boundary cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#project_id BoundaryCluster#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#timeouts BoundaryCluster#timeouts}
+        :param cluster_id: The ID of the Boundary cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#cluster_id BoundaryCluster#cluster_id}
+        :param password: The password of the initial admin user. This must be at least 8 characters in length. Note that this may show up in logs, and it will be stored in the state file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#password BoundaryCluster#password}
+        :param username: The username of the initial admin user. This must be at least 3 characters in length, alphanumeric, hyphen, or period. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#username BoundaryCluster#username}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#id BoundaryCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param maintenance_window_config: maintenance_window_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#maintenance_window_config BoundaryCluster#maintenance_window_config}
+        :param project_id: The ID of the HCP project where the Boundary cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#project_id BoundaryCluster#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#timeouts BoundaryCluster#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(maintenance_window_config, dict):
             maintenance_window_config = BoundaryClusterMaintenanceWindowConfig(**maintenance_window_config)
         if isinstance(timeouts, dict):
             timeouts = BoundaryClusterTimeouts(**timeouts)
@@ -449,79 +449,79 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cluster_id(self) -> builtins.str:
         '''The ID of the Boundary cluster.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#cluster_id BoundaryCluster#cluster_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#cluster_id BoundaryCluster#cluster_id}
         '''
         result = self._values.get("cluster_id")
         assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def password(self) -> builtins.str:
         '''The password of the initial admin user.
 
         This must be at least 8 characters in length. Note that this may show up in logs, and it will be stored in the state file.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#password BoundaryCluster#password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#password BoundaryCluster#password}
         '''
         result = self._values.get("password")
         assert result is not None, "Required property 'password' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def username(self) -> builtins.str:
         '''The username of the initial admin user.
 
         This must be at least 3 characters in length, alphanumeric, hyphen, or period.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#username BoundaryCluster#username}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#username BoundaryCluster#username}
         '''
         result = self._values.get("username")
         assert result is not None, "Required property 'username' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#id BoundaryCluster#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#id BoundaryCluster#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def maintenance_window_config(
         self,
     ) -> typing.Optional["BoundaryClusterMaintenanceWindowConfig"]:
         '''maintenance_window_config block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#maintenance_window_config BoundaryCluster#maintenance_window_config}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#maintenance_window_config BoundaryCluster#maintenance_window_config}
         '''
         result = self._values.get("maintenance_window_config")
         return typing.cast(typing.Optional["BoundaryClusterMaintenanceWindowConfig"], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the Boundary cluster is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#project_id BoundaryCluster#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#project_id BoundaryCluster#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["BoundaryClusterTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#timeouts BoundaryCluster#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#timeouts BoundaryCluster#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["BoundaryClusterTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -550,18 +550,18 @@
         *,
         day: typing.Optional[builtins.str] = None,
         end: typing.Optional[jsii.Number] = None,
         start: typing.Optional[jsii.Number] = None,
         upgrade_type: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param day: The maintenance day of the week for scheduled upgrades. Valid options for maintenance window day - ``MONDAY``, ``TUESDAY``, ``WEDNESDAY``, ``THURSDAY``, ``FRIDAY``, ``SATURDAY``, ``SUNDAY`` Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#day BoundaryCluster#day}
-        :param end: The end time which upgrades can be performed. Uses 24H clock and must be in UTC time zone. Valid options include - 1 to 24 (inclusive) Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#end BoundaryCluster#end}
-        :param start: The start time which upgrades can be performed. Uses 24H clock and must be in UTC time zone. Valid options include - 0 to 23 (inclusive) Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#start BoundaryCluster#start}
-        :param upgrade_type: The upgrade type for the cluster. Valid options for upgrade type - ``AUTOMATIC``, ``SCHEDULED``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#upgrade_type BoundaryCluster#upgrade_type}
+        :param day: The maintenance day of the week for scheduled upgrades. Valid options for maintenance window day - ``MONDAY``, ``TUESDAY``, ``WEDNESDAY``, ``THURSDAY``, ``FRIDAY``, ``SATURDAY``, ``SUNDAY`` Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#day BoundaryCluster#day}
+        :param end: The end time which upgrades can be performed. Uses 24H clock and must be in UTC time zone. Valid options include - 1 to 24 (inclusive) Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#end BoundaryCluster#end}
+        :param start: The start time which upgrades can be performed. Uses 24H clock and must be in UTC time zone. Valid options include - 0 to 23 (inclusive) Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#start BoundaryCluster#start}
+        :param upgrade_type: The upgrade type for the cluster. Valid options for upgrade type - ``AUTOMATIC``, ``SCHEDULED``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#upgrade_type BoundaryCluster#upgrade_type}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c425230c6c9dad28011618e997da80031379d340f0aa60178db1ed0b4af0b989)
             check_type(argname="argument day", value=day, expected_type=type_hints["day"])
             check_type(argname="argument end", value=end, expected_type=type_hints["end"])
             check_type(argname="argument start", value=start, expected_type=type_hints["start"])
             check_type(argname="argument upgrade_type", value=upgrade_type, expected_type=type_hints["upgrade_type"])
@@ -577,46 +577,46 @@
 
     @builtins.property
     def day(self) -> typing.Optional[builtins.str]:
         '''The maintenance day of the week for scheduled upgrades.
 
         Valid options for maintenance window day - ``MONDAY``, ``TUESDAY``, ``WEDNESDAY``, ``THURSDAY``, ``FRIDAY``, ``SATURDAY``, ``SUNDAY``
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#day BoundaryCluster#day}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#day BoundaryCluster#day}
         '''
         result = self._values.get("day")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def end(self) -> typing.Optional[jsii.Number]:
         '''The end time which upgrades can be performed.
 
         Uses 24H clock and must be in UTC time zone. Valid options include - 1 to 24 (inclusive)
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#end BoundaryCluster#end}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#end BoundaryCluster#end}
         '''
         result = self._values.get("end")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def start(self) -> typing.Optional[jsii.Number]:
         '''The start time which upgrades can be performed.
 
         Uses 24H clock and must be in UTC time zone. Valid options include - 0 to 23 (inclusive)
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#start BoundaryCluster#start}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#start BoundaryCluster#start}
         '''
         result = self._values.get("start")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def upgrade_type(self) -> typing.Optional[builtins.str]:
         '''The upgrade type for the cluster. Valid options for upgrade type - ``AUTOMATIC``, ``SCHEDULED``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#upgrade_type BoundaryCluster#upgrade_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#upgrade_type BoundaryCluster#upgrade_type}
         '''
         result = self._values.get("upgrade_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -759,17 +759,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#create BoundaryCluster#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#default BoundaryCluster#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#delete BoundaryCluster#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#create BoundaryCluster#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#default BoundaryCluster#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#delete BoundaryCluster#delete}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f1df35e6c2ce2e7de0ee92af3344b57d6ac6a21e84b62284e97df14a42ec523f)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -778,27 +778,27 @@
         if default is not None:
             self._values["default"] = default
         if delete is not None:
             self._values["delete"] = delete
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#create BoundaryCluster#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#create BoundaryCluster#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#default BoundaryCluster#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#default BoundaryCluster#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/boundary_cluster#delete BoundaryCluster#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/boundary_cluster#delete BoundaryCluster#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/consul_cluster/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/consul_cluster/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_consul_cluster`
 
-Refer to the Terraform Registory for docs: [`hcp_consul_cluster`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster).
+Refer to the Terraform Registory for docs: [`hcp_consul_cluster`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class ConsulCluster(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.consulCluster.ConsulCluster",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster hcp_consul_cluster}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster hcp_consul_cluster}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_id: builtins.str,
@@ -51,32 +51,32 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster hcp_consul_cluster} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster hcp_consul_cluster} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#cluster_id ConsulCluster#cluster_id}
-        :param hvn_id: The ID of the HVN this HCP Consul cluster is associated to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#hvn_id ConsulCluster#hvn_id}
-        :param tier: The tier that the HCP Consul cluster will be provisioned as. Only ``development``, ``standard`` and ``plus`` are available at this time. See `pricing information <https://www.hashicorp.com/products/consul/pricing>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#tier ConsulCluster#tier}
-        :param auto_hvn_to_hvn_peering: Enables automatic HVN to HVN peering when creating a secondary cluster in a federation. The alternative to using the auto-accept feature is to create an ```hcp_hvn_peering_connection`` <hvn_peering_connection.md>`_ resource that explicitly defines the HVN resources that are allowed to communicate with each other. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#auto_hvn_to_hvn_peering ConsulCluster#auto_hvn_to_hvn_peering}
-        :param connect_enabled: Denotes the Consul connect feature should be enabled for this cluster. Default to true. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#connect_enabled ConsulCluster#connect_enabled}
-        :param datacenter: The Consul data center name of the cluster. If not specified, it is defaulted to the value of ``cluster_id``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#datacenter ConsulCluster#datacenter}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#id ConsulCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param ip_allowlist: ip_allowlist block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#ip_allowlist ConsulCluster#ip_allowlist}
-        :param min_consul_version: The minimum Consul patch version of the cluster. Allows only the rightmost version component to increment (E.g: ``1.13.0`` will allow installation of ``1.13.2`` and ``1.13.3`` etc., but not ``1.14.0``). If not specified, it is defaulted to the version that is currently recommended by HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#min_consul_version ConsulCluster#min_consul_version}
-        :param primary_link: The ``self_link`` of the HCP Consul cluster which is the primary in the federation setup with this HCP Consul cluster. If not specified, it is a standalone cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#primary_link ConsulCluster#primary_link}
-        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#project_id ConsulCluster#project_id}
-        :param public_endpoint: Denotes that the cluster has a public endpoint for the Consul UI. Defaults to false. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#public_endpoint ConsulCluster#public_endpoint}
-        :param size: The t-shirt size representation of each server VM that this Consul cluster is provisioned with. Valid option for development tier - ``x_small``. Valid options for other tiers - ``small``, ``medium``, ``large``. For more details - https://cloud.hashicorp.com/pricing/consul. Upgrading the size of a cluster after creation is allowed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#size ConsulCluster#size}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#timeouts ConsulCluster#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#cluster_id ConsulCluster#cluster_id}
+        :param hvn_id: The ID of the HVN this HCP Consul cluster is associated to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#hvn_id ConsulCluster#hvn_id}
+        :param tier: The tier that the HCP Consul cluster will be provisioned as. Only ``development``, ``standard`` and ``plus`` are available at this time. See `pricing information <https://www.hashicorp.com/products/consul/pricing>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#tier ConsulCluster#tier}
+        :param auto_hvn_to_hvn_peering: Enables automatic HVN to HVN peering when creating a secondary cluster in a federation. The alternative to using the auto-accept feature is to create an ```hcp_hvn_peering_connection`` <hvn_peering_connection.md>`_ resource that explicitly defines the HVN resources that are allowed to communicate with each other. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#auto_hvn_to_hvn_peering ConsulCluster#auto_hvn_to_hvn_peering}
+        :param connect_enabled: Denotes the Consul connect feature should be enabled for this cluster. Default to true. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#connect_enabled ConsulCluster#connect_enabled}
+        :param datacenter: The Consul data center name of the cluster. If not specified, it is defaulted to the value of ``cluster_id``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#datacenter ConsulCluster#datacenter}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#id ConsulCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param ip_allowlist: ip_allowlist block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#ip_allowlist ConsulCluster#ip_allowlist}
+        :param min_consul_version: The minimum Consul patch version of the cluster. Allows only the rightmost version component to increment (E.g: ``1.13.0`` will allow installation of ``1.13.2`` and ``1.13.3`` etc., but not ``1.14.0``). If not specified, it is defaulted to the version that is currently recommended by HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#min_consul_version ConsulCluster#min_consul_version}
+        :param primary_link: The ``self_link`` of the HCP Consul cluster which is the primary in the federation setup with this HCP Consul cluster. If not specified, it is a standalone cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#primary_link ConsulCluster#primary_link}
+        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#project_id ConsulCluster#project_id}
+        :param public_endpoint: Denotes that the cluster has a public endpoint for the Consul UI. Defaults to false. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#public_endpoint ConsulCluster#public_endpoint}
+        :param size: The t-shirt size representation of each server VM that this Consul cluster is provisioned with. Valid option for development tier - ``x_small``. Valid options for other tiers - ``small``, ``medium``, ``large``. For more details - https://cloud.hashicorp.com/pricing/consul. Upgrading the size of a cluster after creation is allowed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#size ConsulCluster#size}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#timeouts ConsulCluster#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -130,18 +130,18 @@
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#create ConsulCluster#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#default ConsulCluster#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#delete ConsulCluster#delete}.
-        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#update ConsulCluster#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#create ConsulCluster#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#default ConsulCluster#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#delete ConsulCluster#delete}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#update ConsulCluster#update}.
         '''
         value = ConsulClusterTimeouts(
             create=create, default=default, delete=delete, update=update
         )
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
@@ -585,28 +585,28 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#cluster_id ConsulCluster#cluster_id}
-        :param hvn_id: The ID of the HVN this HCP Consul cluster is associated to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#hvn_id ConsulCluster#hvn_id}
-        :param tier: The tier that the HCP Consul cluster will be provisioned as. Only ``development``, ``standard`` and ``plus`` are available at this time. See `pricing information <https://www.hashicorp.com/products/consul/pricing>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#tier ConsulCluster#tier}
-        :param auto_hvn_to_hvn_peering: Enables automatic HVN to HVN peering when creating a secondary cluster in a federation. The alternative to using the auto-accept feature is to create an ```hcp_hvn_peering_connection`` <hvn_peering_connection.md>`_ resource that explicitly defines the HVN resources that are allowed to communicate with each other. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#auto_hvn_to_hvn_peering ConsulCluster#auto_hvn_to_hvn_peering}
-        :param connect_enabled: Denotes the Consul connect feature should be enabled for this cluster. Default to true. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#connect_enabled ConsulCluster#connect_enabled}
-        :param datacenter: The Consul data center name of the cluster. If not specified, it is defaulted to the value of ``cluster_id``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#datacenter ConsulCluster#datacenter}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#id ConsulCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param ip_allowlist: ip_allowlist block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#ip_allowlist ConsulCluster#ip_allowlist}
-        :param min_consul_version: The minimum Consul patch version of the cluster. Allows only the rightmost version component to increment (E.g: ``1.13.0`` will allow installation of ``1.13.2`` and ``1.13.3`` etc., but not ``1.14.0``). If not specified, it is defaulted to the version that is currently recommended by HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#min_consul_version ConsulCluster#min_consul_version}
-        :param primary_link: The ``self_link`` of the HCP Consul cluster which is the primary in the federation setup with this HCP Consul cluster. If not specified, it is a standalone cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#primary_link ConsulCluster#primary_link}
-        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#project_id ConsulCluster#project_id}
-        :param public_endpoint: Denotes that the cluster has a public endpoint for the Consul UI. Defaults to false. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#public_endpoint ConsulCluster#public_endpoint}
-        :param size: The t-shirt size representation of each server VM that this Consul cluster is provisioned with. Valid option for development tier - ``x_small``. Valid options for other tiers - ``small``, ``medium``, ``large``. For more details - https://cloud.hashicorp.com/pricing/consul. Upgrading the size of a cluster after creation is allowed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#size ConsulCluster#size}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#timeouts ConsulCluster#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#cluster_id ConsulCluster#cluster_id}
+        :param hvn_id: The ID of the HVN this HCP Consul cluster is associated to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#hvn_id ConsulCluster#hvn_id}
+        :param tier: The tier that the HCP Consul cluster will be provisioned as. Only ``development``, ``standard`` and ``plus`` are available at this time. See `pricing information <https://www.hashicorp.com/products/consul/pricing>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#tier ConsulCluster#tier}
+        :param auto_hvn_to_hvn_peering: Enables automatic HVN to HVN peering when creating a secondary cluster in a federation. The alternative to using the auto-accept feature is to create an ```hcp_hvn_peering_connection`` <hvn_peering_connection.md>`_ resource that explicitly defines the HVN resources that are allowed to communicate with each other. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#auto_hvn_to_hvn_peering ConsulCluster#auto_hvn_to_hvn_peering}
+        :param connect_enabled: Denotes the Consul connect feature should be enabled for this cluster. Default to true. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#connect_enabled ConsulCluster#connect_enabled}
+        :param datacenter: The Consul data center name of the cluster. If not specified, it is defaulted to the value of ``cluster_id``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#datacenter ConsulCluster#datacenter}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#id ConsulCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param ip_allowlist: ip_allowlist block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#ip_allowlist ConsulCluster#ip_allowlist}
+        :param min_consul_version: The minimum Consul patch version of the cluster. Allows only the rightmost version component to increment (E.g: ``1.13.0`` will allow installation of ``1.13.2`` and ``1.13.3`` etc., but not ``1.14.0``). If not specified, it is defaulted to the version that is currently recommended by HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#min_consul_version ConsulCluster#min_consul_version}
+        :param primary_link: The ``self_link`` of the HCP Consul cluster which is the primary in the federation setup with this HCP Consul cluster. If not specified, it is a standalone cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#primary_link ConsulCluster#primary_link}
+        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#project_id ConsulCluster#project_id}
+        :param public_endpoint: Denotes that the cluster has a public endpoint for the Consul UI. Defaults to false. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#public_endpoint ConsulCluster#public_endpoint}
+        :param size: The t-shirt size representation of each server VM that this Consul cluster is provisioned with. Valid option for development tier - ``x_small``. Valid options for other tiers - ``small``, ``medium``, ``large``. For more details - https://cloud.hashicorp.com/pricing/consul. Upgrading the size of a cluster after creation is allowed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#size ConsulCluster#size}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#timeouts ConsulCluster#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = ConsulClusterTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e15a4aa3c9e2c590b1a7243a86035a6b7c3197aaded71d8b2ef48bed209d4f0a)
@@ -737,154 +737,154 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cluster_id(self) -> builtins.str:
         '''The ID of the HCP Consul cluster.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#cluster_id ConsulCluster#cluster_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#cluster_id ConsulCluster#cluster_id}
         '''
         result = self._values.get("cluster_id")
         assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def hvn_id(self) -> builtins.str:
         '''The ID of the HVN this HCP Consul cluster is associated to.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#hvn_id ConsulCluster#hvn_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#hvn_id ConsulCluster#hvn_id}
         '''
         result = self._values.get("hvn_id")
         assert result is not None, "Required property 'hvn_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def tier(self) -> builtins.str:
         '''The tier that the HCP Consul cluster will be provisioned as.
 
         Only ``development``, ``standard`` and ``plus`` are available at this time. See `pricing information <https://www.hashicorp.com/products/consul/pricing>`_.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#tier ConsulCluster#tier}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#tier ConsulCluster#tier}
         '''
         result = self._values.get("tier")
         assert result is not None, "Required property 'tier' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def auto_hvn_to_hvn_peering(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Enables automatic HVN to HVN peering when creating a secondary cluster in a federation.
 
         The alternative to using the auto-accept feature is to create an ```hcp_hvn_peering_connection`` <hvn_peering_connection.md>`_ resource that explicitly defines the HVN resources that are allowed to communicate with each other.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#auto_hvn_to_hvn_peering ConsulCluster#auto_hvn_to_hvn_peering}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#auto_hvn_to_hvn_peering ConsulCluster#auto_hvn_to_hvn_peering}
         '''
         result = self._values.get("auto_hvn_to_hvn_peering")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def connect_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Denotes the Consul connect feature should be enabled for this cluster.  Default to true.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#connect_enabled ConsulCluster#connect_enabled}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#connect_enabled ConsulCluster#connect_enabled}
         '''
         result = self._values.get("connect_enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def datacenter(self) -> typing.Optional[builtins.str]:
         '''The Consul data center name of the cluster. If not specified, it is defaulted to the value of ``cluster_id``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#datacenter ConsulCluster#datacenter}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#datacenter ConsulCluster#datacenter}
         '''
         result = self._values.get("datacenter")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#id ConsulCluster#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#id ConsulCluster#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ip_allowlist(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ConsulClusterIpAllowlistStruct"]]]:
         '''ip_allowlist block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#ip_allowlist ConsulCluster#ip_allowlist}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#ip_allowlist ConsulCluster#ip_allowlist}
         '''
         result = self._values.get("ip_allowlist")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ConsulClusterIpAllowlistStruct"]]], result)
 
     @builtins.property
     def min_consul_version(self) -> typing.Optional[builtins.str]:
         '''The minimum Consul patch version of the cluster.
 
         Allows only the rightmost version component to increment (E.g: ``1.13.0`` will allow installation of ``1.13.2`` and ``1.13.3`` etc., but not ``1.14.0``). If not specified, it is defaulted to the version that is currently recommended by HCP.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#min_consul_version ConsulCluster#min_consul_version}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#min_consul_version ConsulCluster#min_consul_version}
         '''
         result = self._values.get("min_consul_version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def primary_link(self) -> typing.Optional[builtins.str]:
         '''The ``self_link`` of the HCP Consul cluster which is the primary in the federation setup with this HCP Consul cluster.
 
         If not specified, it is a standalone cluster.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#primary_link ConsulCluster#primary_link}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#primary_link ConsulCluster#primary_link}
         '''
         result = self._values.get("primary_link")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the HCP Consul cluster is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#project_id ConsulCluster#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#project_id ConsulCluster#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def public_endpoint(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Denotes that the cluster has a public endpoint for the Consul UI. Defaults to false.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#public_endpoint ConsulCluster#public_endpoint}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#public_endpoint ConsulCluster#public_endpoint}
         '''
         result = self._values.get("public_endpoint")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def size(self) -> typing.Optional[builtins.str]:
         '''The t-shirt size representation of each server VM that this Consul cluster is provisioned with.
 
         Valid option for development tier - ``x_small``. Valid options for other tiers - ``small``, ``medium``, ``large``. For more details - https://cloud.hashicorp.com/pricing/consul. Upgrading the size of a cluster after creation is allowed.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#size ConsulCluster#size}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#size ConsulCluster#size}
         '''
         result = self._values.get("size")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["ConsulClusterTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#timeouts ConsulCluster#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#timeouts ConsulCluster#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["ConsulClusterTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -906,16 +906,16 @@
     def __init__(
         self,
         *,
         address: builtins.str,
         description: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param address: IP address range in CIDR notation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#address ConsulCluster#address}
-        :param description: Description to help identify source (maximum 255 chars). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#description ConsulCluster#description}
+        :param address: IP address range in CIDR notation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#address ConsulCluster#address}
+        :param description: Description to help identify source (maximum 255 chars). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#description ConsulCluster#description}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__495bb421883917349d0c876a105aad0e63018a81a54757bca42ff15aaf04b408)
             check_type(argname="argument address", value=address, expected_type=type_hints["address"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "address": address,
@@ -923,25 +923,25 @@
         if description is not None:
             self._values["description"] = description
 
     @builtins.property
     def address(self) -> builtins.str:
         '''IP address range in CIDR notation.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#address ConsulCluster#address}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#address ConsulCluster#address}
         '''
         result = self._values.get("address")
         assert result is not None, "Required property 'address' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''Description to help identify source (maximum 255 chars).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#description ConsulCluster#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#description ConsulCluster#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1145,18 +1145,18 @@
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#create ConsulCluster#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#default ConsulCluster#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#delete ConsulCluster#delete}.
-        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#update ConsulCluster#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#create ConsulCluster#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#default ConsulCluster#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#delete ConsulCluster#delete}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#update ConsulCluster#update}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8f659835463a84e60ea15cd993c4c5de4055fb363e403183b9791dcfc6d21d85)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
             check_type(argname="argument update", value=update, expected_type=type_hints["update"])
@@ -1168,33 +1168,33 @@
         if delete is not None:
             self._values["delete"] = delete
         if update is not None:
             self._values["update"] = update
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#create ConsulCluster#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#create ConsulCluster#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#default ConsulCluster#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#default ConsulCluster#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#delete ConsulCluster#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#delete ConsulCluster#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def update(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster#update ConsulCluster#update}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster#update ConsulCluster#update}.'''
         result = self._values.get("update")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/consul_cluster_root_token/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/consul_cluster_root_token/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_consul_cluster_root_token`
 
-Refer to the Terraform Registory for docs: [`hcp_consul_cluster_root_token`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster_root_token).
+Refer to the Terraform Registory for docs: [`hcp_consul_cluster_root_token`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster_root_token).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class ConsulClusterRootToken(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.consulClusterRootToken.ConsulClusterRootToken",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster_root_token hcp_consul_cluster_root_token}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster_root_token hcp_consul_cluster_root_token}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_id: builtins.str,
@@ -41,22 +41,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster_root_token hcp_consul_cluster_root_token} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster_root_token hcp_consul_cluster_root_token} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster_root_token#cluster_id ConsulClusterRootToken#cluster_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster_root_token#id ConsulClusterRootToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster_root_token#project_id ConsulClusterRootToken#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster_root_token#timeouts ConsulClusterRootToken#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster_root_token#cluster_id ConsulClusterRootToken#cluster_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster_root_token#id ConsulClusterRootToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster_root_token#project_id ConsulClusterRootToken#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster_root_token#timeouts ConsulClusterRootToken#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -80,15 +80,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster_root_token#default ConsulClusterRootToken#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster_root_token#default ConsulClusterRootToken#default}.
         '''
         value = ConsulClusterRootTokenTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -227,18 +227,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster_root_token#cluster_id ConsulClusterRootToken#cluster_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster_root_token#id ConsulClusterRootToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster_root_token#project_id ConsulClusterRootToken#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster_root_token#timeouts ConsulClusterRootToken#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster_root_token#cluster_id ConsulClusterRootToken#cluster_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster_root_token#id ConsulClusterRootToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster_root_token#project_id ConsulClusterRootToken#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster_root_token#timeouts ConsulClusterRootToken#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = ConsulClusterRootTokenTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0926c56dc948940e26333b91643ad320e4464a38f99d953c37e4f5a86c59f395)
@@ -341,44 +341,44 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cluster_id(self) -> builtins.str:
         '''The ID of the HCP Consul cluster.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster_root_token#cluster_id ConsulClusterRootToken#cluster_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster_root_token#cluster_id ConsulClusterRootToken#cluster_id}
         '''
         result = self._values.get("cluster_id")
         assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster_root_token#id ConsulClusterRootToken#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster_root_token#id ConsulClusterRootToken#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the HCP Consul cluster is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster_root_token#project_id ConsulClusterRootToken#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster_root_token#project_id ConsulClusterRootToken#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["ConsulClusterRootTokenTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster_root_token#timeouts ConsulClusterRootToken#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster_root_token#timeouts ConsulClusterRootToken#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["ConsulClusterRootTokenTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -395,26 +395,26 @@
     jsii_type="@cdktf/provider-hcp.consulClusterRootToken.ConsulClusterRootTokenTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class ConsulClusterRootTokenTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster_root_token#default ConsulClusterRootToken#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster_root_token#default ConsulClusterRootToken#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d87a29510dda71b964e144ecd9ecd4c1a0d3c0b0f6eeacaf4c54503c6adea5cb)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_cluster_root_token#default ConsulClusterRootToken#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_cluster_root_token#default ConsulClusterRootToken#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/consul_snapshot/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/consul_snapshot/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_consul_snapshot`
 
-Refer to the Terraform Registory for docs: [`hcp_consul_snapshot`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot).
+Refer to the Terraform Registory for docs: [`hcp_consul_snapshot`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class ConsulSnapshot(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.consulSnapshot.ConsulSnapshot",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot hcp_consul_snapshot}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot hcp_consul_snapshot}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_id: builtins.str,
@@ -42,23 +42,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot hcp_consul_snapshot} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot hcp_consul_snapshot} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#cluster_id ConsulSnapshot#cluster_id}
-        :param snapshot_name: The name of the snapshot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#snapshot_name ConsulSnapshot#snapshot_name}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#id ConsulSnapshot#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#project_id ConsulSnapshot#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#timeouts ConsulSnapshot#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#cluster_id ConsulSnapshot#cluster_id}
+        :param snapshot_name: The name of the snapshot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#snapshot_name ConsulSnapshot#snapshot_name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#id ConsulSnapshot#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#project_id ConsulSnapshot#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#timeouts ConsulSnapshot#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -90,18 +90,18 @@
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#create ConsulSnapshot#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#default ConsulSnapshot#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#delete ConsulSnapshot#delete}.
-        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#update ConsulSnapshot#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#create ConsulSnapshot#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#default ConsulSnapshot#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#delete ConsulSnapshot#delete}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#update ConsulSnapshot#update}.
         '''
         value = ConsulSnapshotTimeouts(
             create=create, default=default, delete=delete, update=update
         )
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
@@ -276,19 +276,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#cluster_id ConsulSnapshot#cluster_id}
-        :param snapshot_name: The name of the snapshot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#snapshot_name ConsulSnapshot#snapshot_name}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#id ConsulSnapshot#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#project_id ConsulSnapshot#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#timeouts ConsulSnapshot#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#cluster_id ConsulSnapshot#cluster_id}
+        :param snapshot_name: The name of the snapshot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#snapshot_name ConsulSnapshot#snapshot_name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#id ConsulSnapshot#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#project_id ConsulSnapshot#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#timeouts ConsulSnapshot#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = ConsulSnapshotTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__407e2d5ef4ee09855675a8e1850926e063e9aa9defd2c3d0404764b6ddaf9375)
@@ -393,54 +393,54 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cluster_id(self) -> builtins.str:
         '''The ID of the HCP Consul cluster.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#cluster_id ConsulSnapshot#cluster_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#cluster_id ConsulSnapshot#cluster_id}
         '''
         result = self._values.get("cluster_id")
         assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def snapshot_name(self) -> builtins.str:
         '''The name of the snapshot.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#snapshot_name ConsulSnapshot#snapshot_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#snapshot_name ConsulSnapshot#snapshot_name}
         '''
         result = self._values.get("snapshot_name")
         assert result is not None, "Required property 'snapshot_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#id ConsulSnapshot#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#id ConsulSnapshot#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the HCP Consul cluster is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#project_id ConsulSnapshot#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#project_id ConsulSnapshot#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["ConsulSnapshotTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#timeouts ConsulSnapshot#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#timeouts ConsulSnapshot#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["ConsulSnapshotTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -469,18 +469,18 @@
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#create ConsulSnapshot#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#default ConsulSnapshot#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#delete ConsulSnapshot#delete}.
-        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#update ConsulSnapshot#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#create ConsulSnapshot#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#default ConsulSnapshot#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#delete ConsulSnapshot#delete}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#update ConsulSnapshot#update}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4e975142f34042561381f5a0050fa61ee7531532c88761b85e444bbe42f2fa5a)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
             check_type(argname="argument update", value=update, expected_type=type_hints["update"])
@@ -492,33 +492,33 @@
         if delete is not None:
             self._values["delete"] = delete
         if update is not None:
             self._values["update"] = update
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#create ConsulSnapshot#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#create ConsulSnapshot#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#default ConsulSnapshot#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#default ConsulSnapshot#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#delete ConsulSnapshot#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#delete ConsulSnapshot#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def update(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/consul_snapshot#update ConsulSnapshot#update}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/consul_snapshot#update ConsulSnapshot#update}.'''
         result = self._values.get("update")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_aws_network_peering/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_aws_network_peering/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_aws_network_peering`
 
-Refer to the Terraform Registory for docs: [`data_hcp_aws_network_peering`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering).
+Refer to the Terraform Registory for docs: [`data_hcp_aws_network_peering`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataHcpAwsNetworkPeering(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpAwsNetworkPeering.DataHcpAwsNetworkPeering",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering hcp_aws_network_peering}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering hcp_aws_network_peering}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         hvn_id: builtins.str,
@@ -43,24 +43,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering hcp_aws_network_peering} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering hcp_aws_network_peering} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering#hvn_id DataHcpAwsNetworkPeering#hvn_id}
-        :param peering_id: The ID of the network peering. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering#peering_id DataHcpAwsNetworkPeering#peering_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering#id DataHcpAwsNetworkPeering#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the network peering is located. Always matches the HVN's project. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering#project_id DataHcpAwsNetworkPeering#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering#timeouts DataHcpAwsNetworkPeering#timeouts}
-        :param wait_for_active_state: If ``true``, Terraform will wait for the network peering to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering#wait_for_active_state DataHcpAwsNetworkPeering#wait_for_active_state}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering#hvn_id DataHcpAwsNetworkPeering#hvn_id}
+        :param peering_id: The ID of the network peering. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering#peering_id DataHcpAwsNetworkPeering#peering_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering#id DataHcpAwsNetworkPeering#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the network peering is located. Always matches the HVN's project. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering#project_id DataHcpAwsNetworkPeering#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering#timeouts DataHcpAwsNetworkPeering#timeouts}
+        :param wait_for_active_state: If ``true``, Terraform will wait for the network peering to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering#wait_for_active_state DataHcpAwsNetworkPeering#wait_for_active_state}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -86,15 +86,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, read: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param read: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering#read DataHcpAwsNetworkPeering#read}.
+        :param read: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering#read DataHcpAwsNetworkPeering#read}.
         '''
         value = DataHcpAwsNetworkPeeringTimeouts(read=read)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -312,20 +312,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering#hvn_id DataHcpAwsNetworkPeering#hvn_id}
-        :param peering_id: The ID of the network peering. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering#peering_id DataHcpAwsNetworkPeering#peering_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering#id DataHcpAwsNetworkPeering#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the network peering is located. Always matches the HVN's project. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering#project_id DataHcpAwsNetworkPeering#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering#timeouts DataHcpAwsNetworkPeering#timeouts}
-        :param wait_for_active_state: If ``true``, Terraform will wait for the network peering to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering#wait_for_active_state DataHcpAwsNetworkPeering#wait_for_active_state}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering#hvn_id DataHcpAwsNetworkPeering#hvn_id}
+        :param peering_id: The ID of the network peering. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering#peering_id DataHcpAwsNetworkPeering#peering_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering#id DataHcpAwsNetworkPeering#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the network peering is located. Always matches the HVN's project. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering#project_id DataHcpAwsNetworkPeering#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering#timeouts DataHcpAwsNetworkPeering#timeouts}
+        :param wait_for_active_state: If ``true``, Terraform will wait for the network peering to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering#wait_for_active_state DataHcpAwsNetworkPeering#wait_for_active_state}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpAwsNetworkPeeringTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__43949da3b11b0b9444af24cc57bdefdbcb02dc379fe0bee2128f98454251c2d5)
@@ -433,65 +433,65 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def hvn_id(self) -> builtins.str:
         '''The ID of the HashiCorp Virtual Network (HVN).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering#hvn_id DataHcpAwsNetworkPeering#hvn_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering#hvn_id DataHcpAwsNetworkPeering#hvn_id}
         '''
         result = self._values.get("hvn_id")
         assert result is not None, "Required property 'hvn_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peering_id(self) -> builtins.str:
         '''The ID of the network peering.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering#peering_id DataHcpAwsNetworkPeering#peering_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering#peering_id DataHcpAwsNetworkPeering#peering_id}
         '''
         result = self._values.get("peering_id")
         assert result is not None, "Required property 'peering_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering#id DataHcpAwsNetworkPeering#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering#id DataHcpAwsNetworkPeering#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the network peering is located. Always matches the HVN's project.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering#project_id DataHcpAwsNetworkPeering#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering#project_id DataHcpAwsNetworkPeering#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpAwsNetworkPeeringTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering#timeouts DataHcpAwsNetworkPeering#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering#timeouts DataHcpAwsNetworkPeering#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpAwsNetworkPeeringTimeouts"], result)
 
     @builtins.property
     def wait_for_active_state(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If ``true``, Terraform will wait for the network peering to reach an ``ACTIVE`` state before continuing. Default ``false``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering#wait_for_active_state DataHcpAwsNetworkPeering#wait_for_active_state}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering#wait_for_active_state DataHcpAwsNetworkPeering#wait_for_active_state}
         '''
         result = self._values.get("wait_for_active_state")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -508,26 +508,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpAwsNetworkPeering.DataHcpAwsNetworkPeeringTimeouts",
     jsii_struct_bases=[],
     name_mapping={"read": "read"},
 )
 class DataHcpAwsNetworkPeeringTimeouts:
     def __init__(self, *, read: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param read: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering#read DataHcpAwsNetworkPeering#read}.
+        :param read: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering#read DataHcpAwsNetworkPeering#read}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4a4732455394dadd0b7d3991531e7ed17f2ce34ec0f53c7143fde4246e7972f2)
             check_type(argname="argument read", value=read, expected_type=type_hints["read"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if read is not None:
             self._values["read"] = read
 
     @builtins.property
     def read(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_network_peering#read DataHcpAwsNetworkPeering#read}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_network_peering#read DataHcpAwsNetworkPeering#read}.'''
         result = self._values.get("read")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_aws_transit_gateway_attachment/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_aws_transit_gateway_attachment/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_aws_transit_gateway_attachment`
 
-Refer to the Terraform Registory for docs: [`data_hcp_aws_transit_gateway_attachment`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment).
+Refer to the Terraform Registory for docs: [`data_hcp_aws_transit_gateway_attachment`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataHcpAwsTransitGatewayAttachment(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpAwsTransitGatewayAttachment.DataHcpAwsTransitGatewayAttachment",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment hcp_aws_transit_gateway_attachment}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment hcp_aws_transit_gateway_attachment}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         hvn_id: builtins.str,
@@ -43,24 +43,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment hcp_aws_transit_gateway_attachment} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment hcp_aws_transit_gateway_attachment} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment#hvn_id DataHcpAwsTransitGatewayAttachment#hvn_id}
-        :param transit_gateway_attachment_id: The user-settable name of the transit gateway attachment in HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment#transit_gateway_attachment_id DataHcpAwsTransitGatewayAttachment#transit_gateway_attachment_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment#id DataHcpAwsTransitGatewayAttachment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the transit gateway attachment is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment#project_id DataHcpAwsTransitGatewayAttachment#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment#timeouts DataHcpAwsTransitGatewayAttachment#timeouts}
-        :param wait_for_active_state: If ``true``, Terraform will wait for the transit gateway attachment to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment#wait_for_active_state DataHcpAwsTransitGatewayAttachment#wait_for_active_state}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment#hvn_id DataHcpAwsTransitGatewayAttachment#hvn_id}
+        :param transit_gateway_attachment_id: The user-settable name of the transit gateway attachment in HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment#transit_gateway_attachment_id DataHcpAwsTransitGatewayAttachment#transit_gateway_attachment_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment#id DataHcpAwsTransitGatewayAttachment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the transit gateway attachment is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment#project_id DataHcpAwsTransitGatewayAttachment#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment#timeouts DataHcpAwsTransitGatewayAttachment#timeouts}
+        :param wait_for_active_state: If ``true``, Terraform will wait for the transit gateway attachment to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment#wait_for_active_state DataHcpAwsTransitGatewayAttachment#wait_for_active_state}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -86,15 +86,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment#default DataHcpAwsTransitGatewayAttachment#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment#default DataHcpAwsTransitGatewayAttachment#default}.
         '''
         value = DataHcpAwsTransitGatewayAttachmentTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -302,20 +302,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment#hvn_id DataHcpAwsTransitGatewayAttachment#hvn_id}
-        :param transit_gateway_attachment_id: The user-settable name of the transit gateway attachment in HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment#transit_gateway_attachment_id DataHcpAwsTransitGatewayAttachment#transit_gateway_attachment_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment#id DataHcpAwsTransitGatewayAttachment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the transit gateway attachment is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment#project_id DataHcpAwsTransitGatewayAttachment#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment#timeouts DataHcpAwsTransitGatewayAttachment#timeouts}
-        :param wait_for_active_state: If ``true``, Terraform will wait for the transit gateway attachment to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment#wait_for_active_state DataHcpAwsTransitGatewayAttachment#wait_for_active_state}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment#hvn_id DataHcpAwsTransitGatewayAttachment#hvn_id}
+        :param transit_gateway_attachment_id: The user-settable name of the transit gateway attachment in HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment#transit_gateway_attachment_id DataHcpAwsTransitGatewayAttachment#transit_gateway_attachment_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment#id DataHcpAwsTransitGatewayAttachment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the transit gateway attachment is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment#project_id DataHcpAwsTransitGatewayAttachment#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment#timeouts DataHcpAwsTransitGatewayAttachment#timeouts}
+        :param wait_for_active_state: If ``true``, Terraform will wait for the transit gateway attachment to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment#wait_for_active_state DataHcpAwsTransitGatewayAttachment#wait_for_active_state}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpAwsTransitGatewayAttachmentTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__363ded0d2931637094a88761d374e1998f400853e0f9fe567af0bc1d8931a7a2)
@@ -423,65 +423,65 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def hvn_id(self) -> builtins.str:
         '''The ID of the HashiCorp Virtual Network (HVN).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment#hvn_id DataHcpAwsTransitGatewayAttachment#hvn_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment#hvn_id DataHcpAwsTransitGatewayAttachment#hvn_id}
         '''
         result = self._values.get("hvn_id")
         assert result is not None, "Required property 'hvn_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def transit_gateway_attachment_id(self) -> builtins.str:
         '''The user-settable name of the transit gateway attachment in HCP.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment#transit_gateway_attachment_id DataHcpAwsTransitGatewayAttachment#transit_gateway_attachment_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment#transit_gateway_attachment_id DataHcpAwsTransitGatewayAttachment#transit_gateway_attachment_id}
         '''
         result = self._values.get("transit_gateway_attachment_id")
         assert result is not None, "Required property 'transit_gateway_attachment_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment#id DataHcpAwsTransitGatewayAttachment#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment#id DataHcpAwsTransitGatewayAttachment#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the transit gateway attachment is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment#project_id DataHcpAwsTransitGatewayAttachment#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment#project_id DataHcpAwsTransitGatewayAttachment#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpAwsTransitGatewayAttachmentTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment#timeouts DataHcpAwsTransitGatewayAttachment#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment#timeouts DataHcpAwsTransitGatewayAttachment#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpAwsTransitGatewayAttachmentTimeouts"], result)
 
     @builtins.property
     def wait_for_active_state(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If ``true``, Terraform will wait for the transit gateway attachment to reach an ``ACTIVE`` state before continuing. Default ``false``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment#wait_for_active_state DataHcpAwsTransitGatewayAttachment#wait_for_active_state}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment#wait_for_active_state DataHcpAwsTransitGatewayAttachment#wait_for_active_state}
         '''
         result = self._values.get("wait_for_active_state")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -498,26 +498,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpAwsTransitGatewayAttachment.DataHcpAwsTransitGatewayAttachmentTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpAwsTransitGatewayAttachmentTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment#default DataHcpAwsTransitGatewayAttachment#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment#default DataHcpAwsTransitGatewayAttachment#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7f1272ea3ccd49ce428f535dea4ad39e95f9fe501d9aca38228c5aecea5b85f5)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/aws_transit_gateway_attachment#default DataHcpAwsTransitGatewayAttachment#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/aws_transit_gateway_attachment#default DataHcpAwsTransitGatewayAttachment#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_azure_peering_connection/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_azure_peering_connection/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_azure_peering_connection`
 
-Refer to the Terraform Registory for docs: [`data_hcp_azure_peering_connection`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/azure_peering_connection).
+Refer to the Terraform Registory for docs: [`data_hcp_azure_peering_connection`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/azure_peering_connection).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataHcpAzurePeeringConnection(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpAzurePeeringConnection.DataHcpAzurePeeringConnection",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/azure_peering_connection hcp_azure_peering_connection}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/azure_peering_connection hcp_azure_peering_connection}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         hvn_link: builtins.str,
@@ -42,23 +42,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/azure_peering_connection hcp_azure_peering_connection} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/azure_peering_connection hcp_azure_peering_connection} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/azure_peering_connection#hvn_link DataHcpAzurePeeringConnection#hvn_link}
-        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/azure_peering_connection#peering_id DataHcpAzurePeeringConnection#peering_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/azure_peering_connection#id DataHcpAzurePeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/azure_peering_connection#timeouts DataHcpAzurePeeringConnection#timeouts}
-        :param wait_for_active_state: If ``true``, Terraform will wait for the peering connection to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/azure_peering_connection#wait_for_active_state DataHcpAzurePeeringConnection#wait_for_active_state}
+        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/azure_peering_connection#hvn_link DataHcpAzurePeeringConnection#hvn_link}
+        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/azure_peering_connection#peering_id DataHcpAzurePeeringConnection#peering_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/azure_peering_connection#id DataHcpAzurePeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/azure_peering_connection#timeouts DataHcpAzurePeeringConnection#timeouts}
+        :param wait_for_active_state: If ``true``, Terraform will wait for the peering connection to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/azure_peering_connection#wait_for_active_state DataHcpAzurePeeringConnection#wait_for_active_state}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -83,15 +83,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, read: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param read: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/azure_peering_connection#read DataHcpAzurePeeringConnection#read}.
+        :param read: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/azure_peering_connection#read DataHcpAzurePeeringConnection#read}.
         '''
         value = DataHcpAzurePeeringConnectionTimeouts(read=read)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -306,19 +306,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/azure_peering_connection#hvn_link DataHcpAzurePeeringConnection#hvn_link}
-        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/azure_peering_connection#peering_id DataHcpAzurePeeringConnection#peering_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/azure_peering_connection#id DataHcpAzurePeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/azure_peering_connection#timeouts DataHcpAzurePeeringConnection#timeouts}
-        :param wait_for_active_state: If ``true``, Terraform will wait for the peering connection to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/azure_peering_connection#wait_for_active_state DataHcpAzurePeeringConnection#wait_for_active_state}
+        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/azure_peering_connection#hvn_link DataHcpAzurePeeringConnection#hvn_link}
+        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/azure_peering_connection#peering_id DataHcpAzurePeeringConnection#peering_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/azure_peering_connection#id DataHcpAzurePeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/azure_peering_connection#timeouts DataHcpAzurePeeringConnection#timeouts}
+        :param wait_for_active_state: If ``true``, Terraform will wait for the peering connection to reach an ``ACTIVE`` state before continuing. Default ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/azure_peering_connection#wait_for_active_state DataHcpAzurePeeringConnection#wait_for_active_state}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpAzurePeeringConnectionTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__bd4aba9c40f32574afd6b9f7bfd3bb022ad0157924dba691af2463b7fa0e49bd)
@@ -423,56 +423,56 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def hvn_link(self) -> builtins.str:
         '''The ``self_link`` of the HashiCorp Virtual Network (HVN).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/azure_peering_connection#hvn_link DataHcpAzurePeeringConnection#hvn_link}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/azure_peering_connection#hvn_link DataHcpAzurePeeringConnection#hvn_link}
         '''
         result = self._values.get("hvn_link")
         assert result is not None, "Required property 'hvn_link' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def peering_id(self) -> builtins.str:
         '''The ID of the peering connection.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/azure_peering_connection#peering_id DataHcpAzurePeeringConnection#peering_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/azure_peering_connection#peering_id DataHcpAzurePeeringConnection#peering_id}
         '''
         result = self._values.get("peering_id")
         assert result is not None, "Required property 'peering_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/azure_peering_connection#id DataHcpAzurePeeringConnection#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/azure_peering_connection#id DataHcpAzurePeeringConnection#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpAzurePeeringConnectionTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/azure_peering_connection#timeouts DataHcpAzurePeeringConnection#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/azure_peering_connection#timeouts DataHcpAzurePeeringConnection#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpAzurePeeringConnectionTimeouts"], result)
 
     @builtins.property
     def wait_for_active_state(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If ``true``, Terraform will wait for the peering connection to reach an ``ACTIVE`` state before continuing. Default ``false``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/azure_peering_connection#wait_for_active_state DataHcpAzurePeeringConnection#wait_for_active_state}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/azure_peering_connection#wait_for_active_state DataHcpAzurePeeringConnection#wait_for_active_state}
         '''
         result = self._values.get("wait_for_active_state")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -489,26 +489,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpAzurePeeringConnection.DataHcpAzurePeeringConnectionTimeouts",
     jsii_struct_bases=[],
     name_mapping={"read": "read"},
 )
 class DataHcpAzurePeeringConnectionTimeouts:
     def __init__(self, *, read: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param read: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/azure_peering_connection#read DataHcpAzurePeeringConnection#read}.
+        :param read: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/azure_peering_connection#read DataHcpAzurePeeringConnection#read}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__898b38c26d5c9a0e94ffd813a9d9bfba170550beaa5a58cee10657e5e66c4981)
             check_type(argname="argument read", value=read, expected_type=type_hints["read"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if read is not None:
             self._values["read"] = read
 
     @builtins.property
     def read(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/azure_peering_connection#read DataHcpAzurePeeringConnection#read}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/azure_peering_connection#read DataHcpAzurePeeringConnection#read}.'''
         result = self._values.get("read")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_boundary_cluster/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_boundary_cluster/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_boundary_cluster`
 
-Refer to the Terraform Registory for docs: [`data_hcp_boundary_cluster`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/boundary_cluster).
+Refer to the Terraform Registory for docs: [`data_hcp_boundary_cluster`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/boundary_cluster).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataHcpBoundaryCluster(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpBoundaryCluster.DataHcpBoundaryCluster",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/boundary_cluster hcp_boundary_cluster}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/boundary_cluster hcp_boundary_cluster}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_id: builtins.str,
@@ -41,22 +41,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/boundary_cluster hcp_boundary_cluster} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/boundary_cluster hcp_boundary_cluster} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_id: The ID of the Boundary cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/boundary_cluster#cluster_id DataHcpBoundaryCluster#cluster_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/boundary_cluster#id DataHcpBoundaryCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the Boundary cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/boundary_cluster#project_id DataHcpBoundaryCluster#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/boundary_cluster#timeouts DataHcpBoundaryCluster#timeouts}
+        :param cluster_id: The ID of the Boundary cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/boundary_cluster#cluster_id DataHcpBoundaryCluster#cluster_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/boundary_cluster#id DataHcpBoundaryCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the Boundary cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/boundary_cluster#project_id DataHcpBoundaryCluster#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/boundary_cluster#timeouts DataHcpBoundaryCluster#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -80,15 +80,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/boundary_cluster#default DataHcpBoundaryCluster#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/boundary_cluster#default DataHcpBoundaryCluster#default}.
         '''
         value = DataHcpBoundaryClusterTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -234,18 +234,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_id: The ID of the Boundary cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/boundary_cluster#cluster_id DataHcpBoundaryCluster#cluster_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/boundary_cluster#id DataHcpBoundaryCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the Boundary cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/boundary_cluster#project_id DataHcpBoundaryCluster#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/boundary_cluster#timeouts DataHcpBoundaryCluster#timeouts}
+        :param cluster_id: The ID of the Boundary cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/boundary_cluster#cluster_id DataHcpBoundaryCluster#cluster_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/boundary_cluster#id DataHcpBoundaryCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the Boundary cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/boundary_cluster#project_id DataHcpBoundaryCluster#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/boundary_cluster#timeouts DataHcpBoundaryCluster#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpBoundaryClusterTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1913eb550d7af1c0dfbcde15980d6a32f450b17c9b36190718614e6f68d1327c)
@@ -348,44 +348,44 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cluster_id(self) -> builtins.str:
         '''The ID of the Boundary cluster.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/boundary_cluster#cluster_id DataHcpBoundaryCluster#cluster_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/boundary_cluster#cluster_id DataHcpBoundaryCluster#cluster_id}
         '''
         result = self._values.get("cluster_id")
         assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/boundary_cluster#id DataHcpBoundaryCluster#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/boundary_cluster#id DataHcpBoundaryCluster#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the Boundary cluster is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/boundary_cluster#project_id DataHcpBoundaryCluster#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/boundary_cluster#project_id DataHcpBoundaryCluster#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpBoundaryClusterTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/boundary_cluster#timeouts DataHcpBoundaryCluster#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/boundary_cluster#timeouts DataHcpBoundaryCluster#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpBoundaryClusterTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -563,26 +563,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpBoundaryCluster.DataHcpBoundaryClusterTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpBoundaryClusterTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/boundary_cluster#default DataHcpBoundaryCluster#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/boundary_cluster#default DataHcpBoundaryCluster#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__fbef6012e860ebe04f146d9896c229e6efec69de6b4a4c1c99a92fcd23d124a6)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/boundary_cluster#default DataHcpBoundaryCluster#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/boundary_cluster#default DataHcpBoundaryCluster#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_helm_config/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_helm_config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_consul_agent_helm_config`
 
-Refer to the Terraform Registory for docs: [`data_hcp_consul_agent_helm_config`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config).
+Refer to the Terraform Registory for docs: [`data_hcp_consul_agent_helm_config`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataHcpConsulAgentHelmConfig(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpConsulAgentHelmConfig.DataHcpConsulAgentHelmConfig",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config hcp_consul_agent_helm_config}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config hcp_consul_agent_helm_config}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_id: builtins.str,
@@ -43,24 +43,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config hcp_consul_agent_helm_config} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config hcp_consul_agent_helm_config} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config#cluster_id DataHcpConsulAgentHelmConfig#cluster_id}
-        :param kubernetes_endpoint: The FQDN for the Kubernetes API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config#kubernetes_endpoint DataHcpConsulAgentHelmConfig#kubernetes_endpoint}
-        :param expose_gossip_ports: Denotes that the gossip ports should be exposed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config#expose_gossip_ports DataHcpConsulAgentHelmConfig#expose_gossip_ports}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config#id DataHcpConsulAgentHelmConfig#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config#project_id DataHcpConsulAgentHelmConfig#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config#timeouts DataHcpConsulAgentHelmConfig#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config#cluster_id DataHcpConsulAgentHelmConfig#cluster_id}
+        :param kubernetes_endpoint: The FQDN for the Kubernetes API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config#kubernetes_endpoint DataHcpConsulAgentHelmConfig#kubernetes_endpoint}
+        :param expose_gossip_ports: Denotes that the gossip ports should be exposed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config#expose_gossip_ports DataHcpConsulAgentHelmConfig#expose_gossip_ports}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config#id DataHcpConsulAgentHelmConfig#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config#project_id DataHcpConsulAgentHelmConfig#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config#timeouts DataHcpConsulAgentHelmConfig#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -86,15 +86,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config#default DataHcpConsulAgentHelmConfig#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config#default DataHcpConsulAgentHelmConfig#default}.
         '''
         value = DataHcpConsulAgentHelmConfigTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetExposeGossipPorts")
     def reset_expose_gossip_ports(self) -> None:
@@ -272,20 +272,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config#cluster_id DataHcpConsulAgentHelmConfig#cluster_id}
-        :param kubernetes_endpoint: The FQDN for the Kubernetes API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config#kubernetes_endpoint DataHcpConsulAgentHelmConfig#kubernetes_endpoint}
-        :param expose_gossip_ports: Denotes that the gossip ports should be exposed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config#expose_gossip_ports DataHcpConsulAgentHelmConfig#expose_gossip_ports}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config#id DataHcpConsulAgentHelmConfig#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config#project_id DataHcpConsulAgentHelmConfig#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config#timeouts DataHcpConsulAgentHelmConfig#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config#cluster_id DataHcpConsulAgentHelmConfig#cluster_id}
+        :param kubernetes_endpoint: The FQDN for the Kubernetes API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config#kubernetes_endpoint DataHcpConsulAgentHelmConfig#kubernetes_endpoint}
+        :param expose_gossip_ports: Denotes that the gossip ports should be exposed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config#expose_gossip_ports DataHcpConsulAgentHelmConfig#expose_gossip_ports}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config#id DataHcpConsulAgentHelmConfig#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config#project_id DataHcpConsulAgentHelmConfig#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config#timeouts DataHcpConsulAgentHelmConfig#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpConsulAgentHelmConfigTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__47dec92eef00aad8d588b88d58009be6faf64a357be06fe065859618bd4d3c59)
@@ -393,65 +393,65 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cluster_id(self) -> builtins.str:
         '''The ID of the HCP Consul cluster.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config#cluster_id DataHcpConsulAgentHelmConfig#cluster_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config#cluster_id DataHcpConsulAgentHelmConfig#cluster_id}
         '''
         result = self._values.get("cluster_id")
         assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def kubernetes_endpoint(self) -> builtins.str:
         '''The FQDN for the Kubernetes API.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config#kubernetes_endpoint DataHcpConsulAgentHelmConfig#kubernetes_endpoint}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config#kubernetes_endpoint DataHcpConsulAgentHelmConfig#kubernetes_endpoint}
         '''
         result = self._values.get("kubernetes_endpoint")
         assert result is not None, "Required property 'kubernetes_endpoint' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def expose_gossip_ports(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Denotes that the gossip ports should be exposed.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config#expose_gossip_ports DataHcpConsulAgentHelmConfig#expose_gossip_ports}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config#expose_gossip_ports DataHcpConsulAgentHelmConfig#expose_gossip_ports}
         '''
         result = self._values.get("expose_gossip_ports")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config#id DataHcpConsulAgentHelmConfig#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config#id DataHcpConsulAgentHelmConfig#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the HCP Consul cluster is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config#project_id DataHcpConsulAgentHelmConfig#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config#project_id DataHcpConsulAgentHelmConfig#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpConsulAgentHelmConfigTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config#timeouts DataHcpConsulAgentHelmConfig#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config#timeouts DataHcpConsulAgentHelmConfig#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpConsulAgentHelmConfigTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -468,26 +468,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpConsulAgentHelmConfig.DataHcpConsulAgentHelmConfigTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpConsulAgentHelmConfigTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config#default DataHcpConsulAgentHelmConfig#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config#default DataHcpConsulAgentHelmConfig#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5fea9574e4bcb25213a3bf7392a0f4ad548eb6e2edf296edabf437732e15d0f0)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_helm_config#default DataHcpConsulAgentHelmConfig#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_helm_config#default DataHcpConsulAgentHelmConfig#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_kubernetes_secret/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_agent_kubernetes_secret/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_consul_agent_kubernetes_secret`
 
-Refer to the Terraform Registory for docs: [`data_hcp_consul_agent_kubernetes_secret`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_kubernetes_secret).
+Refer to the Terraform Registory for docs: [`data_hcp_consul_agent_kubernetes_secret`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_kubernetes_secret).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataHcpConsulAgentKubernetesSecret(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpConsulAgentKubernetesSecret.DataHcpConsulAgentKubernetesSecret",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_kubernetes_secret hcp_consul_agent_kubernetes_secret}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_kubernetes_secret hcp_consul_agent_kubernetes_secret}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_id: builtins.str,
@@ -41,22 +41,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_kubernetes_secret hcp_consul_agent_kubernetes_secret} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_kubernetes_secret hcp_consul_agent_kubernetes_secret} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_kubernetes_secret#cluster_id DataHcpConsulAgentKubernetesSecret#cluster_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_kubernetes_secret#id DataHcpConsulAgentKubernetesSecret#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_kubernetes_secret#project_id DataHcpConsulAgentKubernetesSecret#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_kubernetes_secret#timeouts DataHcpConsulAgentKubernetesSecret#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_kubernetes_secret#cluster_id DataHcpConsulAgentKubernetesSecret#cluster_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_kubernetes_secret#id DataHcpConsulAgentKubernetesSecret#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_kubernetes_secret#project_id DataHcpConsulAgentKubernetesSecret#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_kubernetes_secret#timeouts DataHcpConsulAgentKubernetesSecret#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -80,15 +80,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_kubernetes_secret#default DataHcpConsulAgentKubernetesSecret#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_kubernetes_secret#default DataHcpConsulAgentKubernetesSecret#default}.
         '''
         value = DataHcpConsulAgentKubernetesSecretTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -217,18 +217,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_kubernetes_secret#cluster_id DataHcpConsulAgentKubernetesSecret#cluster_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_kubernetes_secret#id DataHcpConsulAgentKubernetesSecret#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_kubernetes_secret#project_id DataHcpConsulAgentKubernetesSecret#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_kubernetes_secret#timeouts DataHcpConsulAgentKubernetesSecret#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_kubernetes_secret#cluster_id DataHcpConsulAgentKubernetesSecret#cluster_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_kubernetes_secret#id DataHcpConsulAgentKubernetesSecret#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_kubernetes_secret#project_id DataHcpConsulAgentKubernetesSecret#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_kubernetes_secret#timeouts DataHcpConsulAgentKubernetesSecret#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpConsulAgentKubernetesSecretTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__be3c31d62c3a82506dcabb7d451bc380c751bf95c7a2298998776362da97a950)
@@ -331,44 +331,44 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cluster_id(self) -> builtins.str:
         '''The ID of the HCP Consul cluster.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_kubernetes_secret#cluster_id DataHcpConsulAgentKubernetesSecret#cluster_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_kubernetes_secret#cluster_id DataHcpConsulAgentKubernetesSecret#cluster_id}
         '''
         result = self._values.get("cluster_id")
         assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_kubernetes_secret#id DataHcpConsulAgentKubernetesSecret#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_kubernetes_secret#id DataHcpConsulAgentKubernetesSecret#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the HCP Consul cluster is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_kubernetes_secret#project_id DataHcpConsulAgentKubernetesSecret#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_kubernetes_secret#project_id DataHcpConsulAgentKubernetesSecret#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpConsulAgentKubernetesSecretTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_kubernetes_secret#timeouts DataHcpConsulAgentKubernetesSecret#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_kubernetes_secret#timeouts DataHcpConsulAgentKubernetesSecret#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpConsulAgentKubernetesSecretTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -385,26 +385,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpConsulAgentKubernetesSecret.DataHcpConsulAgentKubernetesSecretTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpConsulAgentKubernetesSecretTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_kubernetes_secret#default DataHcpConsulAgentKubernetesSecret#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_kubernetes_secret#default DataHcpConsulAgentKubernetesSecret#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3df70bd5a73802b3268610283263f56fafc818d7a8202339d48801ee49e63fa4)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_agent_kubernetes_secret#default DataHcpConsulAgentKubernetesSecret#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_agent_kubernetes_secret#default DataHcpConsulAgentKubernetesSecret#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_cluster/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_cluster/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_consul_cluster`
 
-Refer to the Terraform Registory for docs: [`data_hcp_consul_cluster`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_cluster).
+Refer to the Terraform Registory for docs: [`data_hcp_consul_cluster`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_cluster).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataHcpConsulCluster(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpConsulCluster.DataHcpConsulCluster",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_cluster hcp_consul_cluster}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_cluster hcp_consul_cluster}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_id: builtins.str,
@@ -41,22 +41,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_cluster hcp_consul_cluster} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_cluster hcp_consul_cluster} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_cluster#cluster_id DataHcpConsulCluster#cluster_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_cluster#id DataHcpConsulCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_cluster#project_id DataHcpConsulCluster#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_cluster#timeouts DataHcpConsulCluster#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_cluster#cluster_id DataHcpConsulCluster#cluster_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_cluster#id DataHcpConsulCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_cluster#project_id DataHcpConsulCluster#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_cluster#timeouts DataHcpConsulCluster#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -80,15 +80,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_cluster#default DataHcpConsulCluster#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_cluster#default DataHcpConsulCluster#default}.
         '''
         value = DataHcpConsulClusterTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -327,18 +327,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_cluster#cluster_id DataHcpConsulCluster#cluster_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_cluster#id DataHcpConsulCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_cluster#project_id DataHcpConsulCluster#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_cluster#timeouts DataHcpConsulCluster#timeouts}
+        :param cluster_id: The ID of the HCP Consul cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_cluster#cluster_id DataHcpConsulCluster#cluster_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_cluster#id DataHcpConsulCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HCP Consul cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_cluster#project_id DataHcpConsulCluster#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_cluster#timeouts DataHcpConsulCluster#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpConsulClusterTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__19684549a8d13e15136e636a89284757a67861c6b2b39b4bf12ae186931f5bfc)
@@ -441,44 +441,44 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cluster_id(self) -> builtins.str:
         '''The ID of the HCP Consul cluster.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_cluster#cluster_id DataHcpConsulCluster#cluster_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_cluster#cluster_id DataHcpConsulCluster#cluster_id}
         '''
         result = self._values.get("cluster_id")
         assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_cluster#id DataHcpConsulCluster#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_cluster#id DataHcpConsulCluster#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the HCP Consul cluster is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_cluster#project_id DataHcpConsulCluster#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_cluster#project_id DataHcpConsulCluster#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpConsulClusterTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_cluster#timeouts DataHcpConsulCluster#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_cluster#timeouts DataHcpConsulCluster#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpConsulClusterTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -644,26 +644,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpConsulCluster.DataHcpConsulClusterTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpConsulClusterTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_cluster#default DataHcpConsulCluster#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_cluster#default DataHcpConsulCluster#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c7161f129504bca3297102710546c4a3e54ea686e16b8260793ad0548b5feb0d)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_cluster#default DataHcpConsulCluster#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_cluster#default DataHcpConsulCluster#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_consul_versions/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_consul_versions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_consul_versions`
 
-Refer to the Terraform Registory for docs: [`data_hcp_consul_versions`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_versions).
+Refer to the Terraform Registory for docs: [`data_hcp_consul_versions`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_versions).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataHcpConsulVersions(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpConsulVersions.DataHcpConsulVersions",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_versions hcp_consul_versions}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_versions hcp_consul_versions}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: typing.Optional[builtins.str] = None,
@@ -39,20 +39,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_versions hcp_consul_versions} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_versions hcp_consul_versions} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_versions#id DataHcpConsulVersions#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_versions#timeouts DataHcpConsulVersions#timeouts}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_versions#id DataHcpConsulVersions#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_versions#timeouts DataHcpConsulVersions#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -74,15 +74,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_versions#default DataHcpConsulVersions#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_versions#default DataHcpConsulVersions#default}.
         '''
         value = DataHcpConsulVersionsTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -179,16 +179,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_versions#id DataHcpConsulVersions#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_versions#timeouts DataHcpConsulVersions#timeouts}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_versions#id DataHcpConsulVersions#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_versions#timeouts DataHcpConsulVersions#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpConsulVersionsTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ce4ec732e9d19fd84371964dd0535e9577854e1ca55940960301bcb99e1b9c2a)
@@ -283,27 +283,27 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_versions#id DataHcpConsulVersions#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_versions#id DataHcpConsulVersions#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpConsulVersionsTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_versions#timeouts DataHcpConsulVersions#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_versions#timeouts DataHcpConsulVersions#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpConsulVersionsTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -320,26 +320,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpConsulVersions.DataHcpConsulVersionsTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpConsulVersionsTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_versions#default DataHcpConsulVersions#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_versions#default DataHcpConsulVersions#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ed5af9126b62d7113ddbc82d2866619e910bd9a40ebdd4661b031b030fd73381)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/consul_versions#default DataHcpConsulVersions#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/consul_versions#default DataHcpConsulVersions#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_hvn/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_hvn/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_hvn`
 
-Refer to the Terraform Registory for docs: [`data_hcp_hvn`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn).
+Refer to the Terraform Registory for docs: [`data_hcp_hvn`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataHcpHvn(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpHvn.DataHcpHvn",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn hcp_hvn}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn hcp_hvn}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         hvn_id: builtins.str,
@@ -41,22 +41,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn hcp_hvn} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn hcp_hvn} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn#hvn_id DataHcpHvn#hvn_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn#id DataHcpHvn#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HVN is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn#project_id DataHcpHvn#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn#timeouts DataHcpHvn#timeouts}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn#hvn_id DataHcpHvn#hvn_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn#id DataHcpHvn#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HVN is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn#project_id DataHcpHvn#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn#timeouts DataHcpHvn#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -80,15 +80,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn#default DataHcpHvn#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn#default DataHcpHvn#default}.
         '''
         value = DataHcpHvnTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -252,18 +252,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn#hvn_id DataHcpHvn#hvn_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn#id DataHcpHvn#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HVN is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn#project_id DataHcpHvn#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn#timeouts DataHcpHvn#timeouts}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn#hvn_id DataHcpHvn#hvn_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn#id DataHcpHvn#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HVN is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn#project_id DataHcpHvn#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn#timeouts DataHcpHvn#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpHvnTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__453ff1b7bb2a6010c49d2b5b38f47ec9027f2eda8d8bfe47db04286175f886d2)
@@ -366,44 +366,44 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def hvn_id(self) -> builtins.str:
         '''The ID of the HashiCorp Virtual Network (HVN).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn#hvn_id DataHcpHvn#hvn_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn#hvn_id DataHcpHvn#hvn_id}
         '''
         result = self._values.get("hvn_id")
         assert result is not None, "Required property 'hvn_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn#id DataHcpHvn#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn#id DataHcpHvn#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the HVN is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn#project_id DataHcpHvn#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn#project_id DataHcpHvn#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpHvnTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn#timeouts DataHcpHvn#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn#timeouts DataHcpHvn#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpHvnTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -420,26 +420,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpHvn.DataHcpHvnTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpHvnTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn#default DataHcpHvn#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn#default DataHcpHvn#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9467b305aebd65c6d36c9d0a374293e0e94ab466fb5e32c9ca7a3f68955d8e8b)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn#default DataHcpHvn#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn#default DataHcpHvn#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_peering_connection/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_peering_connection/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_hvn_peering_connection`
 
-Refer to the Terraform Registory for docs: [`data_hcp_hvn_peering_connection`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection).
+Refer to the Terraform Registory for docs: [`data_hcp_hvn_peering_connection`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,61 +22,61 @@
 
 
 class DataHcpHvnPeeringConnection(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpHvnPeeringConnection.DataHcpHvnPeeringConnection",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection hcp_hvn_peering_connection}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection hcp_hvn_peering_connection}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         hvn1: builtins.str,
-        hvn2: builtins.str,
         peering_id: builtins.str,
+        hvn2: typing.Optional[builtins.str] = None,
         id: typing.Optional[builtins.str] = None,
         project_id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcpHvnPeeringConnectionTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection hcp_hvn_peering_connection} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection hcp_hvn_peering_connection} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param hvn1: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection#hvn_1 DataHcpHvnPeeringConnection#hvn_1}
-        :param hvn2: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection#hvn_2 DataHcpHvnPeeringConnection#hvn_2}
-        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection#peering_id DataHcpHvnPeeringConnection#peering_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection#id DataHcpHvnPeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HVN peering connection is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection#project_id DataHcpHvnPeeringConnection#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection#timeouts DataHcpHvnPeeringConnection#timeouts}
+        :param hvn1: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection#hvn_1 DataHcpHvnPeeringConnection#hvn_1}
+        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection#peering_id DataHcpHvnPeeringConnection#peering_id}
+        :param hvn2: The unique URL of one of the HVNs being peered. Setting this attribute is deprecated, but it will remain usable in read-only form. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection#hvn_2 DataHcpHvnPeeringConnection#hvn_2}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection#id DataHcpHvnPeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HVN peering connection is located. Always matches hvn_1's project ID. Setting this attribute is deprecated, but it will remain usable in read-only form. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection#project_id DataHcpHvnPeeringConnection#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection#timeouts DataHcpHvnPeeringConnection#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3daf42dbe6bf95ee2a83c236b574d35c60db016272eef0ed1296996dca9ee863)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
         config = DataHcpHvnPeeringConnectionConfig(
             hvn1=hvn1,
-            hvn2=hvn2,
             peering_id=peering_id,
+            hvn2=hvn2,
             id=id,
             project_id=project_id,
             timeouts=timeouts,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
@@ -86,20 +86,24 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection#default DataHcpHvnPeeringConnection#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection#default DataHcpHvnPeeringConnection#default}.
         '''
         value = DataHcpHvnPeeringConnectionTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
+    @jsii.member(jsii_name="resetHvn2")
+    def reset_hvn2(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetHvn2", []))
+
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetId", []))
 
     @jsii.member(jsii_name="resetProjectId")
     def reset_project_id(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetProjectId", []))
@@ -248,16 +252,16 @@
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
         "hvn1": "hvn1",
-        "hvn2": "hvn2",
         "peering_id": "peeringId",
+        "hvn2": "hvn2",
         "id": "id",
         "project_id": "projectId",
         "timeouts": "timeouts",
     },
 )
 class DataHcpHvnPeeringConnectionConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
@@ -267,34 +271,34 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         hvn1: builtins.str,
-        hvn2: builtins.str,
         peering_id: builtins.str,
+        hvn2: typing.Optional[builtins.str] = None,
         id: typing.Optional[builtins.str] = None,
         project_id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcpHvnPeeringConnectionTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param hvn1: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection#hvn_1 DataHcpHvnPeeringConnection#hvn_1}
-        :param hvn2: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection#hvn_2 DataHcpHvnPeeringConnection#hvn_2}
-        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection#peering_id DataHcpHvnPeeringConnection#peering_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection#id DataHcpHvnPeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HVN peering connection is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection#project_id DataHcpHvnPeeringConnection#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection#timeouts DataHcpHvnPeeringConnection#timeouts}
+        :param hvn1: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection#hvn_1 DataHcpHvnPeeringConnection#hvn_1}
+        :param peering_id: The ID of the peering connection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection#peering_id DataHcpHvnPeeringConnection#peering_id}
+        :param hvn2: The unique URL of one of the HVNs being peered. Setting this attribute is deprecated, but it will remain usable in read-only form. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection#hvn_2 DataHcpHvnPeeringConnection#hvn_2}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection#id DataHcpHvnPeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HVN peering connection is located. Always matches hvn_1's project ID. Setting this attribute is deprecated, but it will remain usable in read-only form. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection#project_id DataHcpHvnPeeringConnection#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection#timeouts DataHcpHvnPeeringConnection#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpHvnPeeringConnectionTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__64fce66989d09d9766300ce08a1b3a8dc5342d493a037f8bf2715a94a6016b1a)
@@ -302,22 +306,21 @@
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
             check_type(argname="argument hvn1", value=hvn1, expected_type=type_hints["hvn1"])
-            check_type(argname="argument hvn2", value=hvn2, expected_type=type_hints["hvn2"])
             check_type(argname="argument peering_id", value=peering_id, expected_type=type_hints["peering_id"])
+            check_type(argname="argument hvn2", value=hvn2, expected_type=type_hints["hvn2"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument project_id", value=project_id, expected_type=type_hints["project_id"])
             check_type(argname="argument timeouts", value=timeouts, expected_type=type_hints["timeouts"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "hvn1": hvn1,
-            "hvn2": hvn2,
             "peering_id": peering_id,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
         if depends_on is not None:
@@ -326,14 +329,16 @@
             self._values["for_each"] = for_each
         if lifecycle is not None:
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
+        if hvn2 is not None:
+            self._values["hvn2"] = hvn2
         if id is not None:
             self._values["id"] = id
         if project_id is not None:
             self._values["project_id"] = project_id
         if timeouts is not None:
             self._values["timeouts"] = timeouts
 
@@ -401,64 +406,67 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def hvn1(self) -> builtins.str:
         '''The unique URL of one of the HVNs being peered.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection#hvn_1 DataHcpHvnPeeringConnection#hvn_1}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection#hvn_1 DataHcpHvnPeeringConnection#hvn_1}
         '''
         result = self._values.get("hvn1")
         assert result is not None, "Required property 'hvn1' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def hvn2(self) -> builtins.str:
-        '''The unique URL of one of the HVNs being peered.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection#hvn_2 DataHcpHvnPeeringConnection#hvn_2}
-        '''
-        result = self._values.get("hvn2")
-        assert result is not None, "Required property 'hvn2' is missing"
-        return typing.cast(builtins.str, result)
-
-    @builtins.property
     def peering_id(self) -> builtins.str:
         '''The ID of the peering connection.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection#peering_id DataHcpHvnPeeringConnection#peering_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection#peering_id DataHcpHvnPeeringConnection#peering_id}
         '''
         result = self._values.get("peering_id")
         assert result is not None, "Required property 'peering_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
+    def hvn2(self) -> typing.Optional[builtins.str]:
+        '''The unique URL of one of the HVNs being peered.
+
+        Setting this attribute is deprecated, but it will remain usable in read-only form.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection#hvn_2 DataHcpHvnPeeringConnection#hvn_2}
+        '''
+        result = self._values.get("hvn2")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection#id DataHcpHvnPeeringConnection#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection#id DataHcpHvnPeeringConnection#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the HVN peering connection is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection#project_id DataHcpHvnPeeringConnection#project_id}
+        Always matches hvn_1's project ID. Setting this attribute is deprecated, but it will remain usable in read-only form.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection#project_id DataHcpHvnPeeringConnection#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpHvnPeeringConnectionTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection#timeouts DataHcpHvnPeeringConnection#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection#timeouts DataHcpHvnPeeringConnection#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpHvnPeeringConnectionTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -475,26 +483,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpHvnPeeringConnection.DataHcpHvnPeeringConnectionTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpHvnPeeringConnectionTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection#default DataHcpHvnPeeringConnection#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection#default DataHcpHvnPeeringConnection#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c57c224aebaac18dfcc2bfb2fab6ec74b8879a2f03b6640da399adc636b20345)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_peering_connection#default DataHcpHvnPeeringConnection#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_peering_connection#default DataHcpHvnPeeringConnection#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -575,16 +583,16 @@
 publication.publish()
 
 def _typecheckingstub__3daf42dbe6bf95ee2a83c236b574d35c60db016272eef0ed1296996dca9ee863(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     hvn1: builtins.str,
-    hvn2: builtins.str,
     peering_id: builtins.str,
+    hvn2: typing.Optional[builtins.str] = None,
     id: typing.Optional[builtins.str] = None,
     project_id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcpHvnPeeringConnectionTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
@@ -631,16 +639,16 @@
     count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     hvn1: builtins.str,
-    hvn2: builtins.str,
     peering_id: builtins.str,
+    hvn2: typing.Optional[builtins.str] = None,
     id: typing.Optional[builtins.str] = None,
     project_id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcpHvnPeeringConnectionTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_route/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_hvn_route/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_hvn_route`
 
-Refer to the Terraform Registory for docs: [`data_hcp_hvn_route`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_route).
+Refer to the Terraform Registory for docs: [`data_hcp_hvn_route`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_route).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataHcpHvnRoute(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpHvnRoute.DataHcpHvnRoute",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_route hcp_hvn_route}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_route hcp_hvn_route}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         hvn_link: builtins.str,
@@ -42,23 +42,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_route hcp_hvn_route} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_route hcp_hvn_route} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_route#hvn_link DataHcpHvnRoute#hvn_link}
-        :param hvn_route_id: The ID of the HVN route. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_route#hvn_route_id DataHcpHvnRoute#hvn_route_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_route#id DataHcpHvnRoute#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HVN route is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_route#project_id DataHcpHvnRoute#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_route#timeouts DataHcpHvnRoute#timeouts}
+        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_route#hvn_link DataHcpHvnRoute#hvn_link}
+        :param hvn_route_id: The ID of the HVN route. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_route#hvn_route_id DataHcpHvnRoute#hvn_route_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_route#id DataHcpHvnRoute#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HVN route is located. Always matches the project ID in ``hvn_link``. Setting this attribute is deprecated, but it will remain usable in read-only form. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_route#project_id DataHcpHvnRoute#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_route#timeouts DataHcpHvnRoute#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -83,15 +83,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_route#default DataHcpHvnRoute#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_route#default DataHcpHvnRoute#default}.
         '''
         value = DataHcpHvnRouteTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -259,19 +259,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_route#hvn_link DataHcpHvnRoute#hvn_link}
-        :param hvn_route_id: The ID of the HVN route. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_route#hvn_route_id DataHcpHvnRoute#hvn_route_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_route#id DataHcpHvnRoute#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HVN route is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_route#project_id DataHcpHvnRoute#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_route#timeouts DataHcpHvnRoute#timeouts}
+        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_route#hvn_link DataHcpHvnRoute#hvn_link}
+        :param hvn_route_id: The ID of the HVN route. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_route#hvn_route_id DataHcpHvnRoute#hvn_route_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_route#id DataHcpHvnRoute#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HVN route is located. Always matches the project ID in ``hvn_link``. Setting this attribute is deprecated, but it will remain usable in read-only form. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_route#project_id DataHcpHvnRoute#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_route#timeouts DataHcpHvnRoute#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpHvnRouteTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7d998d291388f4b581ac447f8245e6ae3a3b6b66449802a6f662426ff3f18163)
@@ -376,54 +376,56 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def hvn_link(self) -> builtins.str:
         '''The ``self_link`` of the HashiCorp Virtual Network (HVN).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_route#hvn_link DataHcpHvnRoute#hvn_link}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_route#hvn_link DataHcpHvnRoute#hvn_link}
         '''
         result = self._values.get("hvn_link")
         assert result is not None, "Required property 'hvn_link' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def hvn_route_id(self) -> builtins.str:
         '''The ID of the HVN route.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_route#hvn_route_id DataHcpHvnRoute#hvn_route_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_route#hvn_route_id DataHcpHvnRoute#hvn_route_id}
         '''
         result = self._values.get("hvn_route_id")
         assert result is not None, "Required property 'hvn_route_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_route#id DataHcpHvnRoute#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_route#id DataHcpHvnRoute#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the HVN route is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_route#project_id DataHcpHvnRoute#project_id}
+        Always matches the project ID in ``hvn_link``. Setting this attribute is deprecated, but it will remain usable in read-only form.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_route#project_id DataHcpHvnRoute#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpHvnRouteTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_route#timeouts DataHcpHvnRoute#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_route#timeouts DataHcpHvnRoute#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpHvnRouteTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -440,26 +442,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpHvnRoute.DataHcpHvnRouteTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpHvnRouteTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_route#default DataHcpHvnRoute#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_route#default DataHcpHvnRoute#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f0f604582e5a2eb35eace86bd6d3db0862d78e9a132e9be96ebbe04ee856c19b)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/hvn_route#default DataHcpHvnRoute#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/hvn_route#default DataHcpHvnRoute#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_packer_image`
 
-Refer to the Terraform Registory for docs: [`data_hcp_packer_image`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image).
+Refer to the Terraform Registory for docs: [`data_hcp_packer_image`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataHcpPackerImage(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpPackerImage.DataHcpPackerImage",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image hcp_packer_image}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image hcp_packer_image}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         bucket_name: builtins.str,
@@ -46,27 +46,27 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image hcp_packer_image} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image hcp_packer_image} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#bucket_name DataHcpPackerImage#bucket_name}
-        :param cloud_provider: Name of the cloud provider this image is stored-in. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#cloud_provider DataHcpPackerImage#cloud_provider}
-        :param region: Region this image is stored in, if any. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#region DataHcpPackerImage#region}
-        :param channel: The channel that points to the version of the image being retrieved. Either this or ``iteration_id`` must be specified. Note: will incur a billable request Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#channel DataHcpPackerImage#channel}
-        :param component_type: Name of the builder that built this image. Ex: ``amazon-ebs.example``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#component_type DataHcpPackerImage#component_type}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#id DataHcpPackerImage#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param iteration_id: The iteration from which to get the image. Either this or ``channel`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#iteration_id DataHcpPackerImage#iteration_id}
-        :param project_id: The ID of the HCP project where the HCP Packer Registry image is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#project_id DataHcpPackerImage#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#timeouts DataHcpPackerImage#timeouts}
+        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#bucket_name DataHcpPackerImage#bucket_name}
+        :param cloud_provider: Name of the cloud provider this image is stored-in. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#cloud_provider DataHcpPackerImage#cloud_provider}
+        :param region: Region this image is stored in, if any. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#region DataHcpPackerImage#region}
+        :param channel: The channel that points to the version of the image being retrieved. Either this or ``iteration_id`` must be specified. Note: will incur a billable request Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#channel DataHcpPackerImage#channel}
+        :param component_type: Name of the builder that built this image. Ex: ``amazon-ebs.example``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#component_type DataHcpPackerImage#component_type}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#id DataHcpPackerImage#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param iteration_id: The iteration from which to get the image. Either this or ``channel`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#iteration_id DataHcpPackerImage#iteration_id}
+        :param project_id: The ID of the HCP project where the HCP Packer Registry image is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#project_id DataHcpPackerImage#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#timeouts DataHcpPackerImage#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -95,15 +95,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#default DataHcpPackerImage#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#default DataHcpPackerImage#default}.
         '''
         value = DataHcpPackerImageTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetChannel")
     def reset_channel(self) -> None:
@@ -369,23 +369,23 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#bucket_name DataHcpPackerImage#bucket_name}
-        :param cloud_provider: Name of the cloud provider this image is stored-in. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#cloud_provider DataHcpPackerImage#cloud_provider}
-        :param region: Region this image is stored in, if any. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#region DataHcpPackerImage#region}
-        :param channel: The channel that points to the version of the image being retrieved. Either this or ``iteration_id`` must be specified. Note: will incur a billable request Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#channel DataHcpPackerImage#channel}
-        :param component_type: Name of the builder that built this image. Ex: ``amazon-ebs.example``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#component_type DataHcpPackerImage#component_type}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#id DataHcpPackerImage#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param iteration_id: The iteration from which to get the image. Either this or ``channel`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#iteration_id DataHcpPackerImage#iteration_id}
-        :param project_id: The ID of the HCP project where the HCP Packer Registry image is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#project_id DataHcpPackerImage#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#timeouts DataHcpPackerImage#timeouts}
+        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#bucket_name DataHcpPackerImage#bucket_name}
+        :param cloud_provider: Name of the cloud provider this image is stored-in. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#cloud_provider DataHcpPackerImage#cloud_provider}
+        :param region: Region this image is stored in, if any. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#region DataHcpPackerImage#region}
+        :param channel: The channel that points to the version of the image being retrieved. Either this or ``iteration_id`` must be specified. Note: will incur a billable request Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#channel DataHcpPackerImage#channel}
+        :param component_type: Name of the builder that built this image. Ex: ``amazon-ebs.example``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#component_type DataHcpPackerImage#component_type}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#id DataHcpPackerImage#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param iteration_id: The iteration from which to get the image. Either this or ``channel`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#iteration_id DataHcpPackerImage#iteration_id}
+        :param project_id: The ID of the HCP project where the HCP Packer Registry image is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#project_id DataHcpPackerImage#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#timeouts DataHcpPackerImage#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpPackerImageTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d493367e1c5b95af729f26e73812da9655a869bb22c8f88270fbf9a025718631)
@@ -501,93 +501,93 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def bucket_name(self) -> builtins.str:
         '''The slug of the HCP Packer Registry image bucket to pull from.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#bucket_name DataHcpPackerImage#bucket_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#bucket_name DataHcpPackerImage#bucket_name}
         '''
         result = self._values.get("bucket_name")
         assert result is not None, "Required property 'bucket_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def cloud_provider(self) -> builtins.str:
         '''Name of the cloud provider this image is stored-in.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#cloud_provider DataHcpPackerImage#cloud_provider}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#cloud_provider DataHcpPackerImage#cloud_provider}
         '''
         result = self._values.get("cloud_provider")
         assert result is not None, "Required property 'cloud_provider' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def region(self) -> builtins.str:
         '''Region this image is stored in, if any.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#region DataHcpPackerImage#region}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#region DataHcpPackerImage#region}
         '''
         result = self._values.get("region")
         assert result is not None, "Required property 'region' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def channel(self) -> typing.Optional[builtins.str]:
         '''The channel that points to the version of the image being retrieved.
 
         Either this or ``iteration_id`` must be specified. Note: will incur a billable request
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#channel DataHcpPackerImage#channel}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#channel DataHcpPackerImage#channel}
         '''
         result = self._values.get("channel")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def component_type(self) -> typing.Optional[builtins.str]:
         '''Name of the builder that built this image. Ex: ``amazon-ebs.example``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#component_type DataHcpPackerImage#component_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#component_type DataHcpPackerImage#component_type}
         '''
         result = self._values.get("component_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#id DataHcpPackerImage#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#id DataHcpPackerImage#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def iteration_id(self) -> typing.Optional[builtins.str]:
         '''The iteration from which to get the image. Either this or ``channel`` must be specified.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#iteration_id DataHcpPackerImage#iteration_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#iteration_id DataHcpPackerImage#iteration_id}
         '''
         result = self._values.get("iteration_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the HCP Packer Registry image is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#project_id DataHcpPackerImage#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#project_id DataHcpPackerImage#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpPackerImageTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#timeouts DataHcpPackerImage#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#timeouts DataHcpPackerImage#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpPackerImageTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -604,26 +604,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpPackerImage.DataHcpPackerImageTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpPackerImageTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#default DataHcpPackerImage#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#default DataHcpPackerImage#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4be11f84de0716029be04a7daa0df27f4151e6a0bf1e56cb08c563b3a95bdd94)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image#default DataHcpPackerImage#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image#default DataHcpPackerImage#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image_iteration/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_packer_image_iteration/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_packer_image_iteration`
 
-Refer to the Terraform Registory for docs: [`data_hcp_packer_image_iteration`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image_iteration).
+Refer to the Terraform Registory for docs: [`data_hcp_packer_image_iteration`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image_iteration).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataHcpPackerImageIteration(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpPackerImageIteration.DataHcpPackerImageIteration",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image_iteration hcp_packer_image_iteration}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image_iteration hcp_packer_image_iteration}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         bucket_name: builtins.str,
@@ -42,23 +42,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image_iteration hcp_packer_image_iteration} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image_iteration hcp_packer_image_iteration} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image_iteration#bucket_name DataHcpPackerImageIteration#bucket_name}
-        :param channel: The channel that points to the version of the image you want. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image_iteration#channel DataHcpPackerImageIteration#channel}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image_iteration#id DataHcpPackerImageIteration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HCP Packer registry is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image_iteration#project_id DataHcpPackerImageIteration#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image_iteration#timeouts DataHcpPackerImageIteration#timeouts}
+        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image_iteration#bucket_name DataHcpPackerImageIteration#bucket_name}
+        :param channel: The channel that points to the version of the image you want. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image_iteration#channel DataHcpPackerImageIteration#channel}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image_iteration#id DataHcpPackerImageIteration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HCP Packer registry is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image_iteration#project_id DataHcpPackerImageIteration#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image_iteration#timeouts DataHcpPackerImageIteration#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -83,15 +83,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image_iteration#default DataHcpPackerImageIteration#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image_iteration#default DataHcpPackerImageIteration#default}.
         '''
         value = DataHcpPackerImageIterationTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -604,19 +604,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image_iteration#bucket_name DataHcpPackerImageIteration#bucket_name}
-        :param channel: The channel that points to the version of the image you want. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image_iteration#channel DataHcpPackerImageIteration#channel}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image_iteration#id DataHcpPackerImageIteration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HCP Packer registry is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image_iteration#project_id DataHcpPackerImageIteration#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image_iteration#timeouts DataHcpPackerImageIteration#timeouts}
+        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image_iteration#bucket_name DataHcpPackerImageIteration#bucket_name}
+        :param channel: The channel that points to the version of the image you want. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image_iteration#channel DataHcpPackerImageIteration#channel}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image_iteration#id DataHcpPackerImageIteration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HCP Packer registry is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image_iteration#project_id DataHcpPackerImageIteration#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image_iteration#timeouts DataHcpPackerImageIteration#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpPackerImageIterationTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d58fea42b2c52a22d4572e002560d14dfa31818c38be7a84f5c652d433d3bf0c)
@@ -721,54 +721,54 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def bucket_name(self) -> builtins.str:
         '''The slug of the HCP Packer Registry image bucket to pull from.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image_iteration#bucket_name DataHcpPackerImageIteration#bucket_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image_iteration#bucket_name DataHcpPackerImageIteration#bucket_name}
         '''
         result = self._values.get("bucket_name")
         assert result is not None, "Required property 'bucket_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def channel(self) -> builtins.str:
         '''The channel that points to the version of the image you want.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image_iteration#channel DataHcpPackerImageIteration#channel}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image_iteration#channel DataHcpPackerImageIteration#channel}
         '''
         result = self._values.get("channel")
         assert result is not None, "Required property 'channel' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image_iteration#id DataHcpPackerImageIteration#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image_iteration#id DataHcpPackerImageIteration#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the HCP Packer registry is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image_iteration#project_id DataHcpPackerImageIteration#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image_iteration#project_id DataHcpPackerImageIteration#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpPackerImageIterationTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image_iteration#timeouts DataHcpPackerImageIteration#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image_iteration#timeouts DataHcpPackerImageIteration#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpPackerImageIterationTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -785,26 +785,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpPackerImageIteration.DataHcpPackerImageIterationTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpPackerImageIterationTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image_iteration#default DataHcpPackerImageIteration#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image_iteration#default DataHcpPackerImageIteration#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a7466533aa9f1828ae820a0ceadf3b9186cde9924c22191d7503f192b4a00a64)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_image_iteration#default DataHcpPackerImageIteration#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_image_iteration#default DataHcpPackerImageIteration#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_packer_iteration/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_packer_iteration/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_packer_iteration`
 
-Refer to the Terraform Registory for docs: [`data_hcp_packer_iteration`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_iteration).
+Refer to the Terraform Registory for docs: [`data_hcp_packer_iteration`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_iteration).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataHcpPackerIteration(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpPackerIteration.DataHcpPackerIteration",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_iteration hcp_packer_iteration}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_iteration hcp_packer_iteration}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         bucket_name: builtins.str,
@@ -42,23 +42,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_iteration hcp_packer_iteration} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_iteration hcp_packer_iteration} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_iteration#bucket_name DataHcpPackerIteration#bucket_name}
-        :param channel: The channel that points to the version of the image you want. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_iteration#channel DataHcpPackerIteration#channel}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_iteration#id DataHcpPackerIteration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HCP Packer Registry is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_iteration#project_id DataHcpPackerIteration#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_iteration#timeouts DataHcpPackerIteration#timeouts}
+        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_iteration#bucket_name DataHcpPackerIteration#bucket_name}
+        :param channel: The channel that points to the version of the image you want. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_iteration#channel DataHcpPackerIteration#channel}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_iteration#id DataHcpPackerIteration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HCP Packer Registry is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_iteration#project_id DataHcpPackerIteration#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_iteration#timeouts DataHcpPackerIteration#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -83,15 +83,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_iteration#default DataHcpPackerIteration#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_iteration#default DataHcpPackerIteration#default}.
         '''
         value = DataHcpPackerIterationTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -274,19 +274,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_iteration#bucket_name DataHcpPackerIteration#bucket_name}
-        :param channel: The channel that points to the version of the image you want. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_iteration#channel DataHcpPackerIteration#channel}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_iteration#id DataHcpPackerIteration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HCP Packer Registry is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_iteration#project_id DataHcpPackerIteration#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_iteration#timeouts DataHcpPackerIteration#timeouts}
+        :param bucket_name: The slug of the HCP Packer Registry image bucket to pull from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_iteration#bucket_name DataHcpPackerIteration#bucket_name}
+        :param channel: The channel that points to the version of the image you want. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_iteration#channel DataHcpPackerIteration#channel}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_iteration#id DataHcpPackerIteration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HCP Packer Registry is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_iteration#project_id DataHcpPackerIteration#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_iteration#timeouts DataHcpPackerIteration#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpPackerIterationTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b1907b3a3bbaf110973ff3896d69eb2ee23ee8aa755c517c2430a72823955f9f)
@@ -391,54 +391,54 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def bucket_name(self) -> builtins.str:
         '''The slug of the HCP Packer Registry image bucket to pull from.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_iteration#bucket_name DataHcpPackerIteration#bucket_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_iteration#bucket_name DataHcpPackerIteration#bucket_name}
         '''
         result = self._values.get("bucket_name")
         assert result is not None, "Required property 'bucket_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def channel(self) -> builtins.str:
         '''The channel that points to the version of the image you want.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_iteration#channel DataHcpPackerIteration#channel}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_iteration#channel DataHcpPackerIteration#channel}
         '''
         result = self._values.get("channel")
         assert result is not None, "Required property 'channel' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_iteration#id DataHcpPackerIteration#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_iteration#id DataHcpPackerIteration#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the HCP Packer Registry is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_iteration#project_id DataHcpPackerIteration#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_iteration#project_id DataHcpPackerIteration#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpPackerIterationTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_iteration#timeouts DataHcpPackerIteration#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_iteration#timeouts DataHcpPackerIteration#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpPackerIterationTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -455,26 +455,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpPackerIteration.DataHcpPackerIterationTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpPackerIterationTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_iteration#default DataHcpPackerIteration#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_iteration#default DataHcpPackerIteration#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__bc56ebde634d6984041a03ea104026e4f9ae111de199ff8f95ab8447a5a1e05a)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/packer_iteration#default DataHcpPackerIteration#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/packer_iteration#default DataHcpPackerIteration#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/data_hcp_vault_cluster/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/data_hcp_vault_cluster/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcp_vault_cluster`
 
-Refer to the Terraform Registory for docs: [`data_hcp_vault_cluster`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster).
+Refer to the Terraform Registory for docs: [`data_hcp_vault_cluster`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataHcpVaultCluster(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.dataHcpVaultCluster.DataHcpVaultCluster",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster hcp_vault_cluster}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster hcp_vault_cluster}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_id: builtins.str,
@@ -43,24 +43,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster hcp_vault_cluster} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster hcp_vault_cluster} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster#cluster_id DataHcpVaultCluster#cluster_id}
-        :param audit_log_config: audit_log_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster#audit_log_config DataHcpVaultCluster#audit_log_config}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster#id DataHcpVaultCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param metrics_config: metrics_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster#metrics_config DataHcpVaultCluster#metrics_config}
-        :param project_id: The ID of the HCP project where the Vault cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster#project_id DataHcpVaultCluster#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster#timeouts DataHcpVaultCluster#timeouts}
+        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster#cluster_id DataHcpVaultCluster#cluster_id}
+        :param audit_log_config: audit_log_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster#audit_log_config DataHcpVaultCluster#audit_log_config}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster#id DataHcpVaultCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param metrics_config: metrics_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster#metrics_config DataHcpVaultCluster#metrics_config}
+        :param project_id: The ID of the HCP project where the Vault cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster#project_id DataHcpVaultCluster#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster#timeouts DataHcpVaultCluster#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -112,15 +112,15 @@
             type_hints = typing.get_type_hints(_typecheckingstub__0f2ed9f26c2e43f2268a672c7574d1dd5434bde5b170e1e29bd79d306680414c)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast(None, jsii.invoke(self, "putMetricsConfig", [value]))
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster#default DataHcpVaultCluster#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster#default DataHcpVaultCluster#default}.
         '''
         value = DataHcpVaultClusterTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetAuditLogConfig")
     def reset_audit_log_config(self) -> None:
@@ -545,20 +545,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster#cluster_id DataHcpVaultCluster#cluster_id}
-        :param audit_log_config: audit_log_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster#audit_log_config DataHcpVaultCluster#audit_log_config}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster#id DataHcpVaultCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param metrics_config: metrics_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster#metrics_config DataHcpVaultCluster#metrics_config}
-        :param project_id: The ID of the HCP project where the Vault cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster#project_id DataHcpVaultCluster#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster#timeouts DataHcpVaultCluster#timeouts}
+        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster#cluster_id DataHcpVaultCluster#cluster_id}
+        :param audit_log_config: audit_log_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster#audit_log_config DataHcpVaultCluster#audit_log_config}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster#id DataHcpVaultCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param metrics_config: metrics_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster#metrics_config DataHcpVaultCluster#metrics_config}
+        :param project_id: The ID of the HCP project where the Vault cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster#project_id DataHcpVaultCluster#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster#timeouts DataHcpVaultCluster#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcpVaultClusterTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__da593314112c29f9ed1ae10bbea6751cfa957166b81160e91502af33eb797ec5)
@@ -667,66 +667,66 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cluster_id(self) -> builtins.str:
         '''The ID of the HCP Vault cluster.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster#cluster_id DataHcpVaultCluster#cluster_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster#cluster_id DataHcpVaultCluster#cluster_id}
         '''
         result = self._values.get("cluster_id")
         assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def audit_log_config(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataHcpVaultClusterAuditLogConfig]]]:
         '''audit_log_config block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster#audit_log_config DataHcpVaultCluster#audit_log_config}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster#audit_log_config DataHcpVaultCluster#audit_log_config}
         '''
         result = self._values.get("audit_log_config")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataHcpVaultClusterAuditLogConfig]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster#id DataHcpVaultCluster#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster#id DataHcpVaultCluster#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def metrics_config(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataHcpVaultClusterMetricsConfig"]]]:
         '''metrics_config block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster#metrics_config DataHcpVaultCluster#metrics_config}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster#metrics_config DataHcpVaultCluster#metrics_config}
         '''
         result = self._values.get("metrics_config")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataHcpVaultClusterMetricsConfig"]]], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the Vault cluster is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster#project_id DataHcpVaultCluster#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster#project_id DataHcpVaultCluster#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcpVaultClusterTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster#timeouts DataHcpVaultCluster#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster#timeouts DataHcpVaultCluster#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcpVaultClusterTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1077,26 +1077,26 @@
     jsii_type="@cdktf/provider-hcp.dataHcpVaultCluster.DataHcpVaultClusterTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcpVaultClusterTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster#default DataHcpVaultCluster#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster#default DataHcpVaultCluster#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__dc864ae2e4ef57eb0c4d269f34764f9957a907ec6662655189f9cec1dfa0b305)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/data-sources/vault_cluster#default DataHcpVaultCluster#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/data-sources/vault_cluster#default DataHcpVaultCluster#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/hvn/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/hvn/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_hvn`
 
-Refer to the Terraform Registory for docs: [`hcp_hvn`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn).
+Refer to the Terraform Registory for docs: [`hcp_hvn`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Hvn(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.hvn.Hvn",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn hcp_hvn}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn hcp_hvn}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cloud_provider: builtins.str,
@@ -44,25 +44,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn hcp_hvn} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn hcp_hvn} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cloud_provider: The provider where the HVN is located. The provider 'aws' is generally available and 'azure' is in public beta. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#cloud_provider Hvn#cloud_provider}
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#hvn_id Hvn#hvn_id}
-        :param region: The region where the HVN is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#region Hvn#region}
-        :param cidr_block: The CIDR range of the HVN. If this is not provided, the service will provide a default value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#cidr_block Hvn#cidr_block}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#id Hvn#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HVN is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#project_id Hvn#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#timeouts Hvn#timeouts}
+        :param cloud_provider: The provider where the HVN is located. The provider 'aws' is generally available and 'azure' is in public beta. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#cloud_provider Hvn#cloud_provider}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#hvn_id Hvn#hvn_id}
+        :param region: The region where the HVN is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#region Hvn#region}
+        :param cidr_block: The CIDR range of the HVN. If this is not provided, the service will provide a default value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#cidr_block Hvn#cidr_block}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#id Hvn#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HVN is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#project_id Hvn#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#timeouts Hvn#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -95,17 +95,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#create Hvn#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#default Hvn#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#delete Hvn#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#create Hvn#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#default Hvn#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#delete Hvn#delete}.
         '''
         value = HvnTimeouts(create=create, default=default, delete=delete)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetCidrBlock")
     def reset_cidr_block(self) -> None:
@@ -315,21 +315,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cloud_provider: The provider where the HVN is located. The provider 'aws' is generally available and 'azure' is in public beta. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#cloud_provider Hvn#cloud_provider}
-        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#hvn_id Hvn#hvn_id}
-        :param region: The region where the HVN is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#region Hvn#region}
-        :param cidr_block: The CIDR range of the HVN. If this is not provided, the service will provide a default value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#cidr_block Hvn#cidr_block}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#id Hvn#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HVN is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#project_id Hvn#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#timeouts Hvn#timeouts}
+        :param cloud_provider: The provider where the HVN is located. The provider 'aws' is generally available and 'azure' is in public beta. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#cloud_provider Hvn#cloud_provider}
+        :param hvn_id: The ID of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#hvn_id Hvn#hvn_id}
+        :param region: The region where the HVN is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#region Hvn#region}
+        :param cidr_block: The CIDR range of the HVN. If this is not provided, the service will provide a default value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#cidr_block Hvn#cidr_block}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#id Hvn#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HVN is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#project_id Hvn#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#timeouts Hvn#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = HvnTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d25a7fdd7ab2372e1a2e11563d24055e64416bf11f211460edfc9e4cac4b0545)
@@ -439,73 +439,73 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cloud_provider(self) -> builtins.str:
         '''The provider where the HVN is located. The provider 'aws' is generally available and 'azure' is in public beta.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#cloud_provider Hvn#cloud_provider}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#cloud_provider Hvn#cloud_provider}
         '''
         result = self._values.get("cloud_provider")
         assert result is not None, "Required property 'cloud_provider' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def hvn_id(self) -> builtins.str:
         '''The ID of the HashiCorp Virtual Network (HVN).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#hvn_id Hvn#hvn_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#hvn_id Hvn#hvn_id}
         '''
         result = self._values.get("hvn_id")
         assert result is not None, "Required property 'hvn_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def region(self) -> builtins.str:
         '''The region where the HVN is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#region Hvn#region}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#region Hvn#region}
         '''
         result = self._values.get("region")
         assert result is not None, "Required property 'region' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def cidr_block(self) -> typing.Optional[builtins.str]:
         '''The CIDR range of the HVN. If this is not provided, the service will provide a default value.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#cidr_block Hvn#cidr_block}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#cidr_block Hvn#cidr_block}
         '''
         result = self._values.get("cidr_block")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#id Hvn#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#id Hvn#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the HVN is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#project_id Hvn#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#project_id Hvn#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["HvnTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#timeouts Hvn#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#timeouts Hvn#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["HvnTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -528,17 +528,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#create Hvn#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#default Hvn#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#delete Hvn#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#create Hvn#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#default Hvn#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#delete Hvn#delete}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c6735e0b1a893f99c663fcdd555521d20556b1c3aac0d53912d420fd1bc74eaa)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -547,27 +547,27 @@
         if default is not None:
             self._values["default"] = default
         if delete is not None:
             self._values["delete"] = delete
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#create Hvn#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#create Hvn#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#default Hvn#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#default Hvn#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn#delete Hvn#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn#delete Hvn#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/hvn_peering_connection/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/hvn_peering_connection/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_hvn_peering_connection`
 
-Refer to the Terraform Registory for docs: [`hcp_hvn_peering_connection`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection).
+Refer to the Terraform Registory for docs: [`hcp_hvn_peering_connection`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class HvnPeeringConnection(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.hvnPeeringConnection.HvnPeeringConnection",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection hcp_hvn_peering_connection}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection hcp_hvn_peering_connection}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         hvn1: builtins.str,
@@ -42,23 +42,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection hcp_hvn_peering_connection} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection hcp_hvn_peering_connection} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param hvn1: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#hvn_1 HvnPeeringConnection#hvn_1}
-        :param hvn2: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#hvn_2 HvnPeeringConnection#hvn_2}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#id HvnPeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HVN peering connection is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#project_id HvnPeeringConnection#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#timeouts HvnPeeringConnection#timeouts}
+        :param hvn1: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#hvn_1 HvnPeeringConnection#hvn_1}
+        :param hvn2: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#hvn_2 HvnPeeringConnection#hvn_2}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#id HvnPeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where HVN peering connection is located. Always matches hvn_1's project ID. Setting this attribute is deprecated, but it will remain usable in read-only form. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#project_id HvnPeeringConnection#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#timeouts HvnPeeringConnection#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -89,17 +89,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#create HvnPeeringConnection#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#default HvnPeeringConnection#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#delete HvnPeeringConnection#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#create HvnPeeringConnection#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#default HvnPeeringConnection#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#delete HvnPeeringConnection#delete}.
         '''
         value = HvnPeeringConnectionTimeouts(
             create=create, default=default, delete=delete
         )
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
@@ -274,19 +274,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param hvn1: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#hvn_1 HvnPeeringConnection#hvn_1}
-        :param hvn2: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#hvn_2 HvnPeeringConnection#hvn_2}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#id HvnPeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HVN peering connection is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#project_id HvnPeeringConnection#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#timeouts HvnPeeringConnection#timeouts}
+        :param hvn1: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#hvn_1 HvnPeeringConnection#hvn_1}
+        :param hvn2: The unique URL of one of the HVNs being peered. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#hvn_2 HvnPeeringConnection#hvn_2}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#id HvnPeeringConnection#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where HVN peering connection is located. Always matches hvn_1's project ID. Setting this attribute is deprecated, but it will remain usable in read-only form. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#project_id HvnPeeringConnection#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#timeouts HvnPeeringConnection#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = HvnPeeringConnectionTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__78dd0c35c825813a5a19efd778b3a9008690809616f2a6c869b89e19d3ad99c3)
@@ -391,54 +391,56 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def hvn1(self) -> builtins.str:
         '''The unique URL of one of the HVNs being peered.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#hvn_1 HvnPeeringConnection#hvn_1}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#hvn_1 HvnPeeringConnection#hvn_1}
         '''
         result = self._values.get("hvn1")
         assert result is not None, "Required property 'hvn1' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def hvn2(self) -> builtins.str:
         '''The unique URL of one of the HVNs being peered.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#hvn_2 HvnPeeringConnection#hvn_2}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#hvn_2 HvnPeeringConnection#hvn_2}
         '''
         result = self._values.get("hvn2")
         assert result is not None, "Required property 'hvn2' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#id HvnPeeringConnection#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#id HvnPeeringConnection#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
-        '''The ID of the HCP project where the HVN peering connection is located.
+        '''The ID of the HCP project where HVN peering connection is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#project_id HvnPeeringConnection#project_id}
+        Always matches hvn_1's project ID. Setting this attribute is deprecated, but it will remain usable in read-only form.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#project_id HvnPeeringConnection#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["HvnPeeringConnectionTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#timeouts HvnPeeringConnection#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#timeouts HvnPeeringConnection#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["HvnPeeringConnectionTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -461,17 +463,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#create HvnPeeringConnection#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#default HvnPeeringConnection#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#delete HvnPeeringConnection#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#create HvnPeeringConnection#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#default HvnPeeringConnection#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#delete HvnPeeringConnection#delete}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6d89673ab7be9279ee2024c9587ecdae2ebfc5be5a751caaa32e70ba4ca3975f)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -480,27 +482,27 @@
         if default is not None:
             self._values["default"] = default
         if delete is not None:
             self._values["delete"] = delete
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#create HvnPeeringConnection#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#create HvnPeeringConnection#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#default HvnPeeringConnection#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#default HvnPeeringConnection#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_peering_connection#delete HvnPeeringConnection#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_peering_connection#delete HvnPeeringConnection#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/hvn_route/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/hvn_route/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_hvn_route`
 
-Refer to the Terraform Registory for docs: [`hcp_hvn_route`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route).
+Refer to the Terraform Registory for docs: [`hcp_hvn_route`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class HvnRoute(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.hvnRoute.HvnRoute",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route hcp_hvn_route}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route hcp_hvn_route}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         destination_cidr: builtins.str,
@@ -44,25 +44,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route hcp_hvn_route} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route hcp_hvn_route} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param destination_cidr: The destination CIDR of the HVN route. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#destination_cidr HvnRoute#destination_cidr}
-        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#hvn_link HvnRoute#hvn_link}
-        :param hvn_route_id: The ID of the HVN route. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#hvn_route_id HvnRoute#hvn_route_id}
-        :param target_link: A unique URL identifying the target of the HVN route. Examples of the target: ```aws_network_peering`` <aws_network_peering.md>`_, ```aws_transit_gateway_attachment`` <aws_transit_gateway_attachment.md>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#target_link HvnRoute#target_link}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#id HvnRoute#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HVN route is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#project_id HvnRoute#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#timeouts HvnRoute#timeouts}
+        :param destination_cidr: The destination CIDR of the HVN route. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#destination_cidr HvnRoute#destination_cidr}
+        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#hvn_link HvnRoute#hvn_link}
+        :param hvn_route_id: The ID of the HVN route. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#hvn_route_id HvnRoute#hvn_route_id}
+        :param target_link: A unique URL identifying the target of the HVN route. Examples of the target: ```aws_network_peering`` <aws_network_peering.md>`_, ```aws_transit_gateway_attachment`` <aws_transit_gateway_attachment.md>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#target_link HvnRoute#target_link}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#id HvnRoute#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HVN route is located. Always matches the project ID in ``hvn_link``. Setting this attribute is deprecated, but it will remain usable in read-only form. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#project_id HvnRoute#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#timeouts HvnRoute#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -95,17 +95,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#create HvnRoute#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#default HvnRoute#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#delete HvnRoute#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#create HvnRoute#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#default HvnRoute#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#delete HvnRoute#delete}.
         '''
         value = HvnRouteTimeouts(create=create, default=default, delete=delete)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -301,21 +301,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param destination_cidr: The destination CIDR of the HVN route. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#destination_cidr HvnRoute#destination_cidr}
-        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#hvn_link HvnRoute#hvn_link}
-        :param hvn_route_id: The ID of the HVN route. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#hvn_route_id HvnRoute#hvn_route_id}
-        :param target_link: A unique URL identifying the target of the HVN route. Examples of the target: ```aws_network_peering`` <aws_network_peering.md>`_, ```aws_transit_gateway_attachment`` <aws_transit_gateway_attachment.md>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#target_link HvnRoute#target_link}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#id HvnRoute#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HVN route is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#project_id HvnRoute#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#timeouts HvnRoute#timeouts}
+        :param destination_cidr: The destination CIDR of the HVN route. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#destination_cidr HvnRoute#destination_cidr}
+        :param hvn_link: The ``self_link`` of the HashiCorp Virtual Network (HVN). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#hvn_link HvnRoute#hvn_link}
+        :param hvn_route_id: The ID of the HVN route. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#hvn_route_id HvnRoute#hvn_route_id}
+        :param target_link: A unique URL identifying the target of the HVN route. Examples of the target: ```aws_network_peering`` <aws_network_peering.md>`_, ```aws_transit_gateway_attachment`` <aws_transit_gateway_attachment.md>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#target_link HvnRoute#target_link}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#id HvnRoute#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HVN route is located. Always matches the project ID in ``hvn_link``. Setting this attribute is deprecated, but it will remain usable in read-only form. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#project_id HvnRoute#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#timeouts HvnRoute#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = HvnRouteTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a0f8a11ad97253aa3b4db1898b778709d07fdea552ee920fe7548e933e30e5f3)
@@ -424,74 +424,76 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def destination_cidr(self) -> builtins.str:
         '''The destination CIDR of the HVN route.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#destination_cidr HvnRoute#destination_cidr}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#destination_cidr HvnRoute#destination_cidr}
         '''
         result = self._values.get("destination_cidr")
         assert result is not None, "Required property 'destination_cidr' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def hvn_link(self) -> builtins.str:
         '''The ``self_link`` of the HashiCorp Virtual Network (HVN).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#hvn_link HvnRoute#hvn_link}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#hvn_link HvnRoute#hvn_link}
         '''
         result = self._values.get("hvn_link")
         assert result is not None, "Required property 'hvn_link' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def hvn_route_id(self) -> builtins.str:
         '''The ID of the HVN route.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#hvn_route_id HvnRoute#hvn_route_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#hvn_route_id HvnRoute#hvn_route_id}
         '''
         result = self._values.get("hvn_route_id")
         assert result is not None, "Required property 'hvn_route_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def target_link(self) -> builtins.str:
         '''A unique URL identifying the target of the HVN route. Examples of the target: ```aws_network_peering`` <aws_network_peering.md>`_, ```aws_transit_gateway_attachment`` <aws_transit_gateway_attachment.md>`_.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#target_link HvnRoute#target_link}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#target_link HvnRoute#target_link}
         '''
         result = self._values.get("target_link")
         assert result is not None, "Required property 'target_link' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#id HvnRoute#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#id HvnRoute#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the HVN route is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#project_id HvnRoute#project_id}
+        Always matches the project ID in ``hvn_link``. Setting this attribute is deprecated, but it will remain usable in read-only form.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#project_id HvnRoute#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["HvnRouteTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#timeouts HvnRoute#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#timeouts HvnRoute#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["HvnRouteTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -514,17 +516,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#create HvnRoute#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#default HvnRoute#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#delete HvnRoute#delete}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#create HvnRoute#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#default HvnRoute#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#delete HvnRoute#delete}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c7530df28c80a750f79162999178fa310eed9eb7c994ca81b4125415b6563456)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -533,27 +535,27 @@
         if default is not None:
             self._values["default"] = default
         if delete is not None:
             self._values["delete"] = delete
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#create HvnRoute#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#create HvnRoute#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#default HvnRoute#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#default HvnRoute#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/hvn_route#delete HvnRoute#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/hvn_route#delete HvnRoute#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/packer_channel/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/packer_channel/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_packer_channel`
 
-Refer to the Terraform Registory for docs: [`hcp_packer_channel`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel).
+Refer to the Terraform Registory for docs: [`hcp_packer_channel`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class PackerChannel(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.packerChannel.PackerChannel",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel hcp_packer_channel}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel hcp_packer_channel}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         bucket_name: builtins.str,
@@ -43,24 +43,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel hcp_packer_channel} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel hcp_packer_channel} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param bucket_name: The slug of the HCP Packer Registry image bucket where the channel should be created in. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#bucket_name PackerChannel#bucket_name}
-        :param name: The name of the channel being managed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#name PackerChannel#name}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#id PackerChannel#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param iteration: iteration block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#iteration PackerChannel#iteration}
-        :param project_id: The ID of the HCP project where this channel is located in. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#project_id PackerChannel#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#timeouts PackerChannel#timeouts}
+        :param bucket_name: The slug of the HCP Packer Registry image bucket where the channel should be created in. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#bucket_name PackerChannel#bucket_name}
+        :param name: The name of the channel being managed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#name PackerChannel#name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#id PackerChannel#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param iteration: iteration block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#iteration PackerChannel#iteration}
+        :param project_id: The ID of the HCP project where this channel is located in. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#project_id PackerChannel#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#timeouts PackerChannel#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -92,17 +92,17 @@
         self,
         *,
         fingerprint: typing.Optional[builtins.str] = None,
         id: typing.Optional[builtins.str] = None,
         incremental_version: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
-        :param fingerprint: The fingerprint of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#fingerprint PackerChannel#fingerprint}
-        :param id: The ID of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#id PackerChannel#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param incremental_version: The incremental_version of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#incremental_version PackerChannel#incremental_version}
+        :param fingerprint: The fingerprint of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#fingerprint PackerChannel#fingerprint}
+        :param id: The ID of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#id PackerChannel#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param incremental_version: The incremental_version of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#incremental_version PackerChannel#incremental_version}
         '''
         value = PackerChannelIteration(
             fingerprint=fingerprint, id=id, incremental_version=incremental_version
         )
 
         return typing.cast(None, jsii.invoke(self, "putIteration", [value]))
 
@@ -112,18 +112,18 @@
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#create PackerChannel#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#default PackerChannel#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#delete PackerChannel#delete}.
-        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#update PackerChannel#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#create PackerChannel#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#default PackerChannel#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#delete PackerChannel#delete}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#update PackerChannel#update}.
         '''
         value = PackerChannelTimeouts(
             create=create, default=default, delete=delete, update=update
         )
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
@@ -304,20 +304,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param bucket_name: The slug of the HCP Packer Registry image bucket where the channel should be created in. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#bucket_name PackerChannel#bucket_name}
-        :param name: The name of the channel being managed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#name PackerChannel#name}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#id PackerChannel#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param iteration: iteration block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#iteration PackerChannel#iteration}
-        :param project_id: The ID of the HCP project where this channel is located in. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#project_id PackerChannel#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#timeouts PackerChannel#timeouts}
+        :param bucket_name: The slug of the HCP Packer Registry image bucket where the channel should be created in. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#bucket_name PackerChannel#bucket_name}
+        :param name: The name of the channel being managed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#name PackerChannel#name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#id PackerChannel#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param iteration: iteration block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#iteration PackerChannel#iteration}
+        :param project_id: The ID of the HCP project where this channel is located in. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#project_id PackerChannel#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#timeouts PackerChannel#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(iteration, dict):
             iteration = PackerChannelIteration(**iteration)
         if isinstance(timeouts, dict):
             timeouts = PackerChannelTimeouts(**timeouts)
@@ -427,63 +427,63 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def bucket_name(self) -> builtins.str:
         '''The slug of the HCP Packer Registry image bucket where the channel should be created in.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#bucket_name PackerChannel#bucket_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#bucket_name PackerChannel#bucket_name}
         '''
         result = self._values.get("bucket_name")
         assert result is not None, "Required property 'bucket_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the channel being managed.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#name PackerChannel#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#name PackerChannel#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#id PackerChannel#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#id PackerChannel#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def iteration(self) -> typing.Optional["PackerChannelIteration"]:
         '''iteration block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#iteration PackerChannel#iteration}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#iteration PackerChannel#iteration}
         '''
         result = self._values.get("iteration")
         return typing.cast(typing.Optional["PackerChannelIteration"], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where this channel is located in.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#project_id PackerChannel#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#project_id PackerChannel#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["PackerChannelTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#timeouts PackerChannel#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#timeouts PackerChannel#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["PackerChannelTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -510,17 +510,17 @@
         self,
         *,
         fingerprint: typing.Optional[builtins.str] = None,
         id: typing.Optional[builtins.str] = None,
         incremental_version: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
-        :param fingerprint: The fingerprint of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#fingerprint PackerChannel#fingerprint}
-        :param id: The ID of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#id PackerChannel#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param incremental_version: The incremental_version of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#incremental_version PackerChannel#incremental_version}
+        :param fingerprint: The fingerprint of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#fingerprint PackerChannel#fingerprint}
+        :param id: The ID of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#id PackerChannel#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param incremental_version: The incremental_version of the iteration assigned to the channel. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#incremental_version PackerChannel#incremental_version}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ab35d949073c20a9975f8d59dbcea56f6019586d8d17c87198ed9b73d8da416c)
             check_type(argname="argument fingerprint", value=fingerprint, expected_type=type_hints["fingerprint"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument incremental_version", value=incremental_version, expected_type=type_hints["incremental_version"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -531,36 +531,36 @@
         if incremental_version is not None:
             self._values["incremental_version"] = incremental_version
 
     @builtins.property
     def fingerprint(self) -> typing.Optional[builtins.str]:
         '''The fingerprint of the iteration assigned to the channel.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#fingerprint PackerChannel#fingerprint}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#fingerprint PackerChannel#fingerprint}
         '''
         result = self._values.get("fingerprint")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
         '''The ID of the iteration assigned to the channel.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#id PackerChannel#id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#id PackerChannel#id}
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def incremental_version(self) -> typing.Optional[jsii.Number]:
         '''The incremental_version of the iteration assigned to the channel.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#incremental_version PackerChannel#incremental_version}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#incremental_version PackerChannel#incremental_version}
         '''
         result = self._values.get("incremental_version")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -685,18 +685,18 @@
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#create PackerChannel#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#default PackerChannel#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#delete PackerChannel#delete}.
-        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#update PackerChannel#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#create PackerChannel#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#default PackerChannel#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#delete PackerChannel#delete}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#update PackerChannel#update}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__fe787a15b951abd7c6a540834a0577806e60d41fed9c893cef64fa1dabed3638)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
             check_type(argname="argument update", value=update, expected_type=type_hints["update"])
@@ -708,33 +708,33 @@
         if delete is not None:
             self._values["delete"] = delete
         if update is not None:
             self._values["update"] = update
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#create PackerChannel#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#create PackerChannel#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#default PackerChannel#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#default PackerChannel#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#delete PackerChannel#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#delete PackerChannel#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def update(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/packer_channel#update PackerChannel#update}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/packer_channel#update PackerChannel#update}.'''
         result = self._values.get("update")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/provider/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/provider/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`hcp`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs).
+Refer to the Terraform Registory for docs: [`hcp`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,34 +22,34 @@
 
 
 class HcpProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.provider.HcpProvider",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs hcp}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs hcp}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias: typing.Optional[builtins.str] = None,
         client_id: typing.Optional[builtins.str] = None,
         client_secret: typing.Optional[builtins.str] = None,
         project_id: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs hcp} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs hcp} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs#alias HcpProvider#alias}
-        :param client_id: The OAuth2 Client ID for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs#client_id HcpProvider#client_id}
-        :param client_secret: The OAuth2 Client Secret for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs#client_secret HcpProvider#client_secret}
-        :param project_id: The default project in which resources should be created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs#project_id HcpProvider#project_id}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs#alias HcpProvider#alias}
+        :param client_id: The OAuth2 Client ID for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs#client_id HcpProvider#client_id}
+        :param client_secret: The OAuth2 Client Secret for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs#client_secret HcpProvider#client_secret}
+        :param project_id: The default project in which resources should be created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs#project_id HcpProvider#project_id}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9962aa89ee76b9284f3c61b4b164aa99145fa8bddda7ed708d531d776d163687)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = HcpProviderConfig(
             alias=alias,
@@ -170,18 +170,18 @@
         *,
         alias: typing.Optional[builtins.str] = None,
         client_id: typing.Optional[builtins.str] = None,
         client_secret: typing.Optional[builtins.str] = None,
         project_id: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs#alias HcpProvider#alias}
-        :param client_id: The OAuth2 Client ID for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs#client_id HcpProvider#client_id}
-        :param client_secret: The OAuth2 Client Secret for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs#client_secret HcpProvider#client_secret}
-        :param project_id: The default project in which resources should be created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs#project_id HcpProvider#project_id}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs#alias HcpProvider#alias}
+        :param client_id: The OAuth2 Client ID for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs#client_id HcpProvider#client_id}
+        :param client_secret: The OAuth2 Client Secret for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs#client_secret HcpProvider#client_secret}
+        :param project_id: The default project in which resources should be created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs#project_id HcpProvider#project_id}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8d6d52a2ef8cb5413ad5a8ca3a6605f03df54b36c17588f9157418d93854016b)
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
             check_type(argname="argument client_id", value=client_id, expected_type=type_hints["client_id"])
             check_type(argname="argument client_secret", value=client_secret, expected_type=type_hints["client_secret"])
             check_type(argname="argument project_id", value=project_id, expected_type=type_hints["project_id"])
@@ -195,42 +195,42 @@
         if project_id is not None:
             self._values["project_id"] = project_id
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs#alias HcpProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs#alias HcpProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def client_id(self) -> typing.Optional[builtins.str]:
         '''The OAuth2 Client ID for API operations.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs#client_id HcpProvider#client_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs#client_id HcpProvider#client_id}
         '''
         result = self._values.get("client_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def client_secret(self) -> typing.Optional[builtins.str]:
         '''The OAuth2 Client Secret for API operations.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs#client_secret HcpProvider#client_secret}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs#client_secret HcpProvider#client_secret}
         '''
         result = self._values.get("client_secret")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The default project in which resources should be created.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs#project_id HcpProvider#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs#project_id HcpProvider#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/vault_cluster/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/vault_cluster/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_vault_cluster`
 
-Refer to the Terraform Registory for docs: [`hcp_vault_cluster`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster).
+Refer to the Terraform Registory for docs: [`hcp_vault_cluster`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class VaultCluster(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.vaultCluster.VaultCluster",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster hcp_vault_cluster}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster hcp_vault_cluster}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_id: builtins.str,
@@ -50,31 +50,31 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster hcp_vault_cluster} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster hcp_vault_cluster} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#cluster_id VaultCluster#cluster_id}
-        :param hvn_id: The ID of the HVN this HCP Vault cluster is associated to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#hvn_id VaultCluster#hvn_id}
-        :param audit_log_config: audit_log_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#audit_log_config VaultCluster#audit_log_config}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#id VaultCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param major_version_upgrade_config: major_version_upgrade_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#major_version_upgrade_config VaultCluster#major_version_upgrade_config}
-        :param metrics_config: metrics_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#metrics_config VaultCluster#metrics_config}
-        :param min_vault_version: The minimum Vault version to use when creating the cluster. If not specified, it is defaulted to the version that is currently recommended by HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#min_vault_version VaultCluster#min_vault_version}
-        :param paths_filter: The performance replication `paths filter <https://developer.hashicorp.com/vault/tutorials/cloud-ops/vault-replication-terraform>`_. Applies to performance replication secondaries only and operates in "deny" mode only. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#paths_filter VaultCluster#paths_filter}
-        :param primary_link: The ``self_link`` of the HCP Vault Plus tier cluster which is the primary in the performance replication setup with this HCP Vault Plus tier cluster. If not specified, it is a standalone Plus tier HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#primary_link VaultCluster#primary_link}
-        :param project_id: The ID of the HCP project where the Vault cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#project_id VaultCluster#project_id}
-        :param public_endpoint: Denotes that the cluster has a public endpoint. Defaults to false. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#public_endpoint VaultCluster#public_endpoint}
-        :param tier: Tier of the HCP Vault cluster. Valid options for tiers - ``dev``, ``starter_small``, ``standard_small``, ``standard_medium``, ``standard_large``, ``plus_small``, ``plus_medium``, ``plus_large``. See `pricing information <https://www.hashicorp.com/products/vault/pricing>`_. Changing a cluster's size or tier is only available to admins. See `Scale a cluster <https://registry.terraform.io/providers/hashicorp/hcp/latest/docs/guides/vault-scaling>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#tier VaultCluster#tier}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#timeouts VaultCluster#timeouts}
+        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#cluster_id VaultCluster#cluster_id}
+        :param hvn_id: The ID of the HVN this HCP Vault cluster is associated to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#hvn_id VaultCluster#hvn_id}
+        :param audit_log_config: audit_log_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#audit_log_config VaultCluster#audit_log_config}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#id VaultCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param major_version_upgrade_config: major_version_upgrade_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#major_version_upgrade_config VaultCluster#major_version_upgrade_config}
+        :param metrics_config: metrics_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#metrics_config VaultCluster#metrics_config}
+        :param min_vault_version: The minimum Vault version to use when creating the cluster. If not specified, it is defaulted to the version that is currently recommended by HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#min_vault_version VaultCluster#min_vault_version}
+        :param paths_filter: The performance replication `paths filter <https://developer.hashicorp.com/vault/tutorials/cloud-ops/vault-replication-terraform>`_. Applies to performance replication secondaries only and operates in "deny" mode only. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#paths_filter VaultCluster#paths_filter}
+        :param primary_link: The ``self_link`` of the HCP Vault Plus tier cluster which is the primary in the performance replication setup with this HCP Vault Plus tier cluster. If not specified, it is a standalone Plus tier HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#primary_link VaultCluster#primary_link}
+        :param project_id: The ID of the HCP project where the Vault cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#project_id VaultCluster#project_id}
+        :param public_endpoint: Denotes that the cluster has a public endpoint. Defaults to false. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#public_endpoint VaultCluster#public_endpoint}
+        :param tier: Tier of the HCP Vault cluster. Valid options for tiers - ``dev``, ``starter_small``, ``standard_small``, ``standard_medium``, ``standard_large``, ``plus_small``, ``plus_medium``, ``plus_large``. See `pricing information <https://www.hashicorp.com/products/vault/pricing>`_. Changing a cluster's size or tier is only available to admins. See `Scale a cluster <https://registry.terraform.io/providers/hashicorp/hcp/latest/docs/guides/vault-scaling>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#tier VaultCluster#tier}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#timeouts VaultCluster#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -117,21 +117,21 @@
         grafana_endpoint: typing.Optional[builtins.str] = None,
         grafana_password: typing.Optional[builtins.str] = None,
         grafana_user: typing.Optional[builtins.str] = None,
         splunk_hecendpoint: typing.Optional[builtins.str] = None,
         splunk_token: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param datadog_api_key: Datadog api key for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
-        :param datadog_region: Datadog region for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#datadog_region VaultCluster#datadog_region}
-        :param grafana_endpoint: Grafana endpoint for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
-        :param grafana_password: Grafana password for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#grafana_password VaultCluster#grafana_password}
-        :param grafana_user: Grafana user for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#grafana_user VaultCluster#grafana_user}
-        :param splunk_hecendpoint: Splunk endpoint for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
-        :param splunk_token: Splunk token for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#splunk_token VaultCluster#splunk_token}
+        :param datadog_api_key: Datadog api key for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
+        :param datadog_region: Datadog region for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#datadog_region VaultCluster#datadog_region}
+        :param grafana_endpoint: Grafana endpoint for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
+        :param grafana_password: Grafana password for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#grafana_password VaultCluster#grafana_password}
+        :param grafana_user: Grafana user for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#grafana_user VaultCluster#grafana_user}
+        :param splunk_hecendpoint: Splunk endpoint for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
+        :param splunk_token: Splunk token for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#splunk_token VaultCluster#splunk_token}
         '''
         value = VaultClusterAuditLogConfig(
             datadog_api_key=datadog_api_key,
             datadog_region=datadog_region,
             grafana_endpoint=grafana_endpoint,
             grafana_password=grafana_password,
             grafana_user=grafana_user,
@@ -146,17 +146,17 @@
         self,
         *,
         upgrade_type: builtins.str,
         maintenance_window_day: typing.Optional[builtins.str] = None,
         maintenance_window_time: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param upgrade_type: The major upgrade type for the cluster. Valid options for upgrade type - ``AUTOMATIC``, ``SCHEDULED``, ``MANUAL``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#upgrade_type VaultCluster#upgrade_type}
-        :param maintenance_window_day: The maintenance day of the week for scheduled upgrades. Valid options for maintenance window day - ``MONDAY``, ``TUESDAY``, ``WEDNESDAY``, ``THURSDAY``, ``FRIDAY``, ``SATURDAY``, ``SUNDAY`` Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#maintenance_window_day VaultCluster#maintenance_window_day}
-        :param maintenance_window_time: The maintenance time frame for scheduled upgrades. Valid options for maintenance window time - ``WINDOW_12AM_4AM``, ``WINDOW_6AM_10AM``, ``WINDOW_12PM_4PM``, ``WINDOW_6PM_10PM``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#maintenance_window_time VaultCluster#maintenance_window_time}
+        :param upgrade_type: The major upgrade type for the cluster. Valid options for upgrade type - ``AUTOMATIC``, ``SCHEDULED``, ``MANUAL``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#upgrade_type VaultCluster#upgrade_type}
+        :param maintenance_window_day: The maintenance day of the week for scheduled upgrades. Valid options for maintenance window day - ``MONDAY``, ``TUESDAY``, ``WEDNESDAY``, ``THURSDAY``, ``FRIDAY``, ``SATURDAY``, ``SUNDAY`` Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#maintenance_window_day VaultCluster#maintenance_window_day}
+        :param maintenance_window_time: The maintenance time frame for scheduled upgrades. Valid options for maintenance window time - ``WINDOW_12AM_4AM``, ``WINDOW_6AM_10AM``, ``WINDOW_12PM_4PM``, ``WINDOW_6PM_10PM``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#maintenance_window_time VaultCluster#maintenance_window_time}
         '''
         value = VaultClusterMajorVersionUpgradeConfig(
             upgrade_type=upgrade_type,
             maintenance_window_day=maintenance_window_day,
             maintenance_window_time=maintenance_window_time,
         )
 
@@ -171,21 +171,21 @@
         grafana_endpoint: typing.Optional[builtins.str] = None,
         grafana_password: typing.Optional[builtins.str] = None,
         grafana_user: typing.Optional[builtins.str] = None,
         splunk_hecendpoint: typing.Optional[builtins.str] = None,
         splunk_token: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param datadog_api_key: Datadog api key for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
-        :param datadog_region: Datadog region for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#datadog_region VaultCluster#datadog_region}
-        :param grafana_endpoint: Grafana endpoint for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
-        :param grafana_password: Grafana password for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#grafana_password VaultCluster#grafana_password}
-        :param grafana_user: Grafana user for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#grafana_user VaultCluster#grafana_user}
-        :param splunk_hecendpoint: Splunk endpoint for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
-        :param splunk_token: Splunk token for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#splunk_token VaultCluster#splunk_token}
+        :param datadog_api_key: Datadog api key for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
+        :param datadog_region: Datadog region for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#datadog_region VaultCluster#datadog_region}
+        :param grafana_endpoint: Grafana endpoint for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
+        :param grafana_password: Grafana password for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#grafana_password VaultCluster#grafana_password}
+        :param grafana_user: Grafana user for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#grafana_user VaultCluster#grafana_user}
+        :param splunk_hecendpoint: Splunk endpoint for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
+        :param splunk_token: Splunk token for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#splunk_token VaultCluster#splunk_token}
         '''
         value = VaultClusterMetricsConfig(
             datadog_api_key=datadog_api_key,
             datadog_region=datadog_region,
             grafana_endpoint=grafana_endpoint,
             grafana_password=grafana_password,
             grafana_user=grafana_user,
@@ -201,18 +201,18 @@
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#create VaultCluster#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#default VaultCluster#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#delete VaultCluster#delete}.
-        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#update VaultCluster#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#create VaultCluster#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#default VaultCluster#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#delete VaultCluster#delete}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#update VaultCluster#update}.
         '''
         value = VaultClusterTimeouts(
             create=create, default=default, delete=delete, update=update
         )
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
@@ -548,21 +548,21 @@
         grafana_endpoint: typing.Optional[builtins.str] = None,
         grafana_password: typing.Optional[builtins.str] = None,
         grafana_user: typing.Optional[builtins.str] = None,
         splunk_hecendpoint: typing.Optional[builtins.str] = None,
         splunk_token: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param datadog_api_key: Datadog api key for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
-        :param datadog_region: Datadog region for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#datadog_region VaultCluster#datadog_region}
-        :param grafana_endpoint: Grafana endpoint for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
-        :param grafana_password: Grafana password for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#grafana_password VaultCluster#grafana_password}
-        :param grafana_user: Grafana user for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#grafana_user VaultCluster#grafana_user}
-        :param splunk_hecendpoint: Splunk endpoint for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
-        :param splunk_token: Splunk token for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#splunk_token VaultCluster#splunk_token}
+        :param datadog_api_key: Datadog api key for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
+        :param datadog_region: Datadog region for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#datadog_region VaultCluster#datadog_region}
+        :param grafana_endpoint: Grafana endpoint for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
+        :param grafana_password: Grafana password for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#grafana_password VaultCluster#grafana_password}
+        :param grafana_user: Grafana user for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#grafana_user VaultCluster#grafana_user}
+        :param splunk_hecendpoint: Splunk endpoint for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
+        :param splunk_token: Splunk token for streaming audit logs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#splunk_token VaultCluster#splunk_token}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__945e965e9dab450573c42b8a5cc975ed8d0713bf41d459bead13f88051d0a34e)
             check_type(argname="argument datadog_api_key", value=datadog_api_key, expected_type=type_hints["datadog_api_key"])
             check_type(argname="argument datadog_region", value=datadog_region, expected_type=type_hints["datadog_region"])
             check_type(argname="argument grafana_endpoint", value=grafana_endpoint, expected_type=type_hints["grafana_endpoint"])
             check_type(argname="argument grafana_password", value=grafana_password, expected_type=type_hints["grafana_password"])
@@ -585,69 +585,69 @@
         if splunk_token is not None:
             self._values["splunk_token"] = splunk_token
 
     @builtins.property
     def datadog_api_key(self) -> typing.Optional[builtins.str]:
         '''Datadog api key for streaming audit logs.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
         '''
         result = self._values.get("datadog_api_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def datadog_region(self) -> typing.Optional[builtins.str]:
         '''Datadog region for streaming audit logs.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#datadog_region VaultCluster#datadog_region}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#datadog_region VaultCluster#datadog_region}
         '''
         result = self._values.get("datadog_region")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def grafana_endpoint(self) -> typing.Optional[builtins.str]:
         '''Grafana endpoint for streaming audit logs.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
         '''
         result = self._values.get("grafana_endpoint")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def grafana_password(self) -> typing.Optional[builtins.str]:
         '''Grafana password for streaming audit logs.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#grafana_password VaultCluster#grafana_password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#grafana_password VaultCluster#grafana_password}
         '''
         result = self._values.get("grafana_password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def grafana_user(self) -> typing.Optional[builtins.str]:
         '''Grafana user for streaming audit logs.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#grafana_user VaultCluster#grafana_user}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#grafana_user VaultCluster#grafana_user}
         '''
         result = self._values.get("grafana_user")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def splunk_hecendpoint(self) -> typing.Optional[builtins.str]:
         '''Splunk endpoint for streaming audit logs.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
         '''
         result = self._values.get("splunk_hecendpoint")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def splunk_token(self) -> typing.Optional[builtins.str]:
         '''Splunk token for streaming audit logs.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#splunk_token VaultCluster#splunk_token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#splunk_token VaultCluster#splunk_token}
         '''
         result = self._values.get("splunk_token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -898,27 +898,27 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#cluster_id VaultCluster#cluster_id}
-        :param hvn_id: The ID of the HVN this HCP Vault cluster is associated to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#hvn_id VaultCluster#hvn_id}
-        :param audit_log_config: audit_log_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#audit_log_config VaultCluster#audit_log_config}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#id VaultCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param major_version_upgrade_config: major_version_upgrade_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#major_version_upgrade_config VaultCluster#major_version_upgrade_config}
-        :param metrics_config: metrics_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#metrics_config VaultCluster#metrics_config}
-        :param min_vault_version: The minimum Vault version to use when creating the cluster. If not specified, it is defaulted to the version that is currently recommended by HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#min_vault_version VaultCluster#min_vault_version}
-        :param paths_filter: The performance replication `paths filter <https://developer.hashicorp.com/vault/tutorials/cloud-ops/vault-replication-terraform>`_. Applies to performance replication secondaries only and operates in "deny" mode only. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#paths_filter VaultCluster#paths_filter}
-        :param primary_link: The ``self_link`` of the HCP Vault Plus tier cluster which is the primary in the performance replication setup with this HCP Vault Plus tier cluster. If not specified, it is a standalone Plus tier HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#primary_link VaultCluster#primary_link}
-        :param project_id: The ID of the HCP project where the Vault cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#project_id VaultCluster#project_id}
-        :param public_endpoint: Denotes that the cluster has a public endpoint. Defaults to false. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#public_endpoint VaultCluster#public_endpoint}
-        :param tier: Tier of the HCP Vault cluster. Valid options for tiers - ``dev``, ``starter_small``, ``standard_small``, ``standard_medium``, ``standard_large``, ``plus_small``, ``plus_medium``, ``plus_large``. See `pricing information <https://www.hashicorp.com/products/vault/pricing>`_. Changing a cluster's size or tier is only available to admins. See `Scale a cluster <https://registry.terraform.io/providers/hashicorp/hcp/latest/docs/guides/vault-scaling>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#tier VaultCluster#tier}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#timeouts VaultCluster#timeouts}
+        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#cluster_id VaultCluster#cluster_id}
+        :param hvn_id: The ID of the HVN this HCP Vault cluster is associated to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#hvn_id VaultCluster#hvn_id}
+        :param audit_log_config: audit_log_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#audit_log_config VaultCluster#audit_log_config}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#id VaultCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param major_version_upgrade_config: major_version_upgrade_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#major_version_upgrade_config VaultCluster#major_version_upgrade_config}
+        :param metrics_config: metrics_config block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#metrics_config VaultCluster#metrics_config}
+        :param min_vault_version: The minimum Vault version to use when creating the cluster. If not specified, it is defaulted to the version that is currently recommended by HCP. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#min_vault_version VaultCluster#min_vault_version}
+        :param paths_filter: The performance replication `paths filter <https://developer.hashicorp.com/vault/tutorials/cloud-ops/vault-replication-terraform>`_. Applies to performance replication secondaries only and operates in "deny" mode only. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#paths_filter VaultCluster#paths_filter}
+        :param primary_link: The ``self_link`` of the HCP Vault Plus tier cluster which is the primary in the performance replication setup with this HCP Vault Plus tier cluster. If not specified, it is a standalone Plus tier HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#primary_link VaultCluster#primary_link}
+        :param project_id: The ID of the HCP project where the Vault cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#project_id VaultCluster#project_id}
+        :param public_endpoint: Denotes that the cluster has a public endpoint. Defaults to false. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#public_endpoint VaultCluster#public_endpoint}
+        :param tier: Tier of the HCP Vault cluster. Valid options for tiers - ``dev``, ``starter_small``, ``standard_small``, ``standard_medium``, ``standard_large``, ``plus_small``, ``plus_medium``, ``plus_large``. See `pricing information <https://www.hashicorp.com/products/vault/pricing>`_. Changing a cluster's size or tier is only available to admins. See `Scale a cluster <https://registry.terraform.io/providers/hashicorp/hcp/latest/docs/guides/vault-scaling>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#tier VaultCluster#tier}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#timeouts VaultCluster#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(audit_log_config, dict):
             audit_log_config = VaultClusterAuditLogConfig(**audit_log_config)
         if isinstance(major_version_upgrade_config, dict):
             major_version_upgrade_config = VaultClusterMajorVersionUpgradeConfig(**major_version_upgrade_config)
@@ -1053,136 +1053,136 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cluster_id(self) -> builtins.str:
         '''The ID of the HCP Vault cluster.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#cluster_id VaultCluster#cluster_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#cluster_id VaultCluster#cluster_id}
         '''
         result = self._values.get("cluster_id")
         assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def hvn_id(self) -> builtins.str:
         '''The ID of the HVN this HCP Vault cluster is associated to.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#hvn_id VaultCluster#hvn_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#hvn_id VaultCluster#hvn_id}
         '''
         result = self._values.get("hvn_id")
         assert result is not None, "Required property 'hvn_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def audit_log_config(self) -> typing.Optional[VaultClusterAuditLogConfig]:
         '''audit_log_config block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#audit_log_config VaultCluster#audit_log_config}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#audit_log_config VaultCluster#audit_log_config}
         '''
         result = self._values.get("audit_log_config")
         return typing.cast(typing.Optional[VaultClusterAuditLogConfig], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#id VaultCluster#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#id VaultCluster#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def major_version_upgrade_config(
         self,
     ) -> typing.Optional["VaultClusterMajorVersionUpgradeConfig"]:
         '''major_version_upgrade_config block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#major_version_upgrade_config VaultCluster#major_version_upgrade_config}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#major_version_upgrade_config VaultCluster#major_version_upgrade_config}
         '''
         result = self._values.get("major_version_upgrade_config")
         return typing.cast(typing.Optional["VaultClusterMajorVersionUpgradeConfig"], result)
 
     @builtins.property
     def metrics_config(self) -> typing.Optional["VaultClusterMetricsConfig"]:
         '''metrics_config block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#metrics_config VaultCluster#metrics_config}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#metrics_config VaultCluster#metrics_config}
         '''
         result = self._values.get("metrics_config")
         return typing.cast(typing.Optional["VaultClusterMetricsConfig"], result)
 
     @builtins.property
     def min_vault_version(self) -> typing.Optional[builtins.str]:
         '''The minimum Vault version to use when creating the cluster.
 
         If not specified, it is defaulted to the version that is currently recommended by HCP.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#min_vault_version VaultCluster#min_vault_version}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#min_vault_version VaultCluster#min_vault_version}
         '''
         result = self._values.get("min_vault_version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def paths_filter(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The performance replication `paths filter <https://developer.hashicorp.com/vault/tutorials/cloud-ops/vault-replication-terraform>`_. Applies to performance replication secondaries only and operates in "deny" mode only.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#paths_filter VaultCluster#paths_filter}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#paths_filter VaultCluster#paths_filter}
         '''
         result = self._values.get("paths_filter")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def primary_link(self) -> typing.Optional[builtins.str]:
         '''The ``self_link`` of the HCP Vault Plus tier cluster which is the primary in the performance replication setup with this HCP Vault Plus tier cluster.
 
         If not specified, it is a standalone Plus tier HCP Vault cluster.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#primary_link VaultCluster#primary_link}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#primary_link VaultCluster#primary_link}
         '''
         result = self._values.get("primary_link")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the Vault cluster is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#project_id VaultCluster#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#project_id VaultCluster#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def public_endpoint(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Denotes that the cluster has a public endpoint. Defaults to false.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#public_endpoint VaultCluster#public_endpoint}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#public_endpoint VaultCluster#public_endpoint}
         '''
         result = self._values.get("public_endpoint")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def tier(self) -> typing.Optional[builtins.str]:
         '''Tier of the HCP Vault cluster.
 
         Valid options for tiers - ``dev``, ``starter_small``, ``standard_small``, ``standard_medium``, ``standard_large``, ``plus_small``, ``plus_medium``, ``plus_large``. See `pricing information <https://www.hashicorp.com/products/vault/pricing>`_. Changing a cluster's size or tier is only available to admins. See `Scale a cluster <https://registry.terraform.io/providers/hashicorp/hcp/latest/docs/guides/vault-scaling>`_.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#tier VaultCluster#tier}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#tier VaultCluster#tier}
         '''
         result = self._values.get("tier")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["VaultClusterTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#timeouts VaultCluster#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#timeouts VaultCluster#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["VaultClusterTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1209,17 +1209,17 @@
         self,
         *,
         upgrade_type: builtins.str,
         maintenance_window_day: typing.Optional[builtins.str] = None,
         maintenance_window_time: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param upgrade_type: The major upgrade type for the cluster. Valid options for upgrade type - ``AUTOMATIC``, ``SCHEDULED``, ``MANUAL``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#upgrade_type VaultCluster#upgrade_type}
-        :param maintenance_window_day: The maintenance day of the week for scheduled upgrades. Valid options for maintenance window day - ``MONDAY``, ``TUESDAY``, ``WEDNESDAY``, ``THURSDAY``, ``FRIDAY``, ``SATURDAY``, ``SUNDAY`` Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#maintenance_window_day VaultCluster#maintenance_window_day}
-        :param maintenance_window_time: The maintenance time frame for scheduled upgrades. Valid options for maintenance window time - ``WINDOW_12AM_4AM``, ``WINDOW_6AM_10AM``, ``WINDOW_12PM_4PM``, ``WINDOW_6PM_10PM``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#maintenance_window_time VaultCluster#maintenance_window_time}
+        :param upgrade_type: The major upgrade type for the cluster. Valid options for upgrade type - ``AUTOMATIC``, ``SCHEDULED``, ``MANUAL``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#upgrade_type VaultCluster#upgrade_type}
+        :param maintenance_window_day: The maintenance day of the week for scheduled upgrades. Valid options for maintenance window day - ``MONDAY``, ``TUESDAY``, ``WEDNESDAY``, ``THURSDAY``, ``FRIDAY``, ``SATURDAY``, ``SUNDAY`` Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#maintenance_window_day VaultCluster#maintenance_window_day}
+        :param maintenance_window_time: The maintenance time frame for scheduled upgrades. Valid options for maintenance window time - ``WINDOW_12AM_4AM``, ``WINDOW_6AM_10AM``, ``WINDOW_12PM_4PM``, ``WINDOW_6PM_10PM``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#maintenance_window_time VaultCluster#maintenance_window_time}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f4962f49b844cabab740d8df01f3b70a715d3f1306b60fec54b6272426400d44)
             check_type(argname="argument upgrade_type", value=upgrade_type, expected_type=type_hints["upgrade_type"])
             check_type(argname="argument maintenance_window_day", value=maintenance_window_day, expected_type=type_hints["maintenance_window_day"])
             check_type(argname="argument maintenance_window_time", value=maintenance_window_time, expected_type=type_hints["maintenance_window_time"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -1230,36 +1230,36 @@
         if maintenance_window_time is not None:
             self._values["maintenance_window_time"] = maintenance_window_time
 
     @builtins.property
     def upgrade_type(self) -> builtins.str:
         '''The major upgrade type for the cluster. Valid options for upgrade type - ``AUTOMATIC``, ``SCHEDULED``, ``MANUAL``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#upgrade_type VaultCluster#upgrade_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#upgrade_type VaultCluster#upgrade_type}
         '''
         result = self._values.get("upgrade_type")
         assert result is not None, "Required property 'upgrade_type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def maintenance_window_day(self) -> typing.Optional[builtins.str]:
         '''The maintenance day of the week for scheduled upgrades.
 
         Valid options for maintenance window day - ``MONDAY``, ``TUESDAY``, ``WEDNESDAY``, ``THURSDAY``, ``FRIDAY``, ``SATURDAY``, ``SUNDAY``
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#maintenance_window_day VaultCluster#maintenance_window_day}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#maintenance_window_day VaultCluster#maintenance_window_day}
         '''
         result = self._values.get("maintenance_window_day")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def maintenance_window_time(self) -> typing.Optional[builtins.str]:
         '''The maintenance time frame for scheduled upgrades. Valid options for maintenance window time - ``WINDOW_12AM_4AM``, ``WINDOW_6AM_10AM``, ``WINDOW_12PM_4PM``, ``WINDOW_6PM_10PM``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#maintenance_window_time VaultCluster#maintenance_window_time}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#maintenance_window_time VaultCluster#maintenance_window_time}
         '''
         result = self._values.get("maintenance_window_time")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1389,21 +1389,21 @@
         grafana_endpoint: typing.Optional[builtins.str] = None,
         grafana_password: typing.Optional[builtins.str] = None,
         grafana_user: typing.Optional[builtins.str] = None,
         splunk_hecendpoint: typing.Optional[builtins.str] = None,
         splunk_token: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param datadog_api_key: Datadog api key for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
-        :param datadog_region: Datadog region for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#datadog_region VaultCluster#datadog_region}
-        :param grafana_endpoint: Grafana endpoint for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
-        :param grafana_password: Grafana password for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#grafana_password VaultCluster#grafana_password}
-        :param grafana_user: Grafana user for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#grafana_user VaultCluster#grafana_user}
-        :param splunk_hecendpoint: Splunk endpoint for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
-        :param splunk_token: Splunk token for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#splunk_token VaultCluster#splunk_token}
+        :param datadog_api_key: Datadog api key for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
+        :param datadog_region: Datadog region for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#datadog_region VaultCluster#datadog_region}
+        :param grafana_endpoint: Grafana endpoint for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
+        :param grafana_password: Grafana password for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#grafana_password VaultCluster#grafana_password}
+        :param grafana_user: Grafana user for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#grafana_user VaultCluster#grafana_user}
+        :param splunk_hecendpoint: Splunk endpoint for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
+        :param splunk_token: Splunk token for streaming metrics. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#splunk_token VaultCluster#splunk_token}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e41328d9c30b2160db3534c4e47502c0f13855650febdfb88b239dcb6d6ee814)
             check_type(argname="argument datadog_api_key", value=datadog_api_key, expected_type=type_hints["datadog_api_key"])
             check_type(argname="argument datadog_region", value=datadog_region, expected_type=type_hints["datadog_region"])
             check_type(argname="argument grafana_endpoint", value=grafana_endpoint, expected_type=type_hints["grafana_endpoint"])
             check_type(argname="argument grafana_password", value=grafana_password, expected_type=type_hints["grafana_password"])
@@ -1426,69 +1426,69 @@
         if splunk_token is not None:
             self._values["splunk_token"] = splunk_token
 
     @builtins.property
     def datadog_api_key(self) -> typing.Optional[builtins.str]:
         '''Datadog api key for streaming metrics.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#datadog_api_key VaultCluster#datadog_api_key}
         '''
         result = self._values.get("datadog_api_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def datadog_region(self) -> typing.Optional[builtins.str]:
         '''Datadog region for streaming metrics.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#datadog_region VaultCluster#datadog_region}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#datadog_region VaultCluster#datadog_region}
         '''
         result = self._values.get("datadog_region")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def grafana_endpoint(self) -> typing.Optional[builtins.str]:
         '''Grafana endpoint for streaming metrics.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#grafana_endpoint VaultCluster#grafana_endpoint}
         '''
         result = self._values.get("grafana_endpoint")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def grafana_password(self) -> typing.Optional[builtins.str]:
         '''Grafana password for streaming metrics.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#grafana_password VaultCluster#grafana_password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#grafana_password VaultCluster#grafana_password}
         '''
         result = self._values.get("grafana_password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def grafana_user(self) -> typing.Optional[builtins.str]:
         '''Grafana user for streaming metrics.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#grafana_user VaultCluster#grafana_user}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#grafana_user VaultCluster#grafana_user}
         '''
         result = self._values.get("grafana_user")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def splunk_hecendpoint(self) -> typing.Optional[builtins.str]:
         '''Splunk endpoint for streaming metrics.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#splunk_hecendpoint VaultCluster#splunk_hecendpoint}
         '''
         result = self._values.get("splunk_hecendpoint")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def splunk_token(self) -> typing.Optional[builtins.str]:
         '''Splunk token for streaming metrics.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#splunk_token VaultCluster#splunk_token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#splunk_token VaultCluster#splunk_token}
         '''
         result = self._values.get("splunk_token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1697,18 +1697,18 @@
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#create VaultCluster#create}.
-        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#default VaultCluster#default}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#delete VaultCluster#delete}.
-        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#update VaultCluster#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#create VaultCluster#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#default VaultCluster#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#delete VaultCluster#delete}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#update VaultCluster#update}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__85ee5e56e863fb68b056cf0c52c11694127fd2447b2109705c1c013124bc122b)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
             check_type(argname="argument update", value=update, expected_type=type_hints["update"])
@@ -1720,33 +1720,33 @@
         if delete is not None:
             self._values["delete"] = delete
         if update is not None:
             self._values["update"] = update
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#create VaultCluster#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#create VaultCluster#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#default VaultCluster#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#default VaultCluster#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#delete VaultCluster#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#delete VaultCluster#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def update(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster#update VaultCluster#update}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster#update VaultCluster#update}.'''
         result = self._values.get("update")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp/vault_cluster_admin_token/__init__.py` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp/vault_cluster_admin_token/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcp_vault_cluster_admin_token`
 
-Refer to the Terraform Registory for docs: [`hcp_vault_cluster_admin_token`](https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token).
+Refer to the Terraform Registory for docs: [`hcp_vault_cluster_admin_token`](https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class VaultClusterAdminToken(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcp.vaultClusterAdminToken.VaultClusterAdminToken",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token hcp_vault_cluster_admin_token}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token hcp_vault_cluster_admin_token}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_id: builtins.str,
@@ -41,22 +41,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token hcp_vault_cluster_admin_token} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token hcp_vault_cluster_admin_token} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token#cluster_id VaultClusterAdminToken#cluster_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token#id VaultClusterAdminToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HCP Vault cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token#project_id VaultClusterAdminToken#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token#timeouts VaultClusterAdminToken#timeouts}
+        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token#cluster_id VaultClusterAdminToken#cluster_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token#id VaultClusterAdminToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HCP Vault cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token#project_id VaultClusterAdminToken#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token#timeouts VaultClusterAdminToken#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -86,17 +86,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         read: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token#create VaultClusterAdminToken#create}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token#delete VaultClusterAdminToken#delete}.
-        :param read: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token#read VaultClusterAdminToken#read}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token#create VaultClusterAdminToken#create}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token#delete VaultClusterAdminToken#delete}.
+        :param read: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token#read VaultClusterAdminToken#read}.
         '''
         value = VaultClusterAdminTokenTimeouts(create=create, delete=delete, read=read)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -230,18 +230,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token#cluster_id VaultClusterAdminToken#cluster_id}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token#id VaultClusterAdminToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_id: The ID of the HCP project where the HCP Vault cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token#project_id VaultClusterAdminToken#project_id}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token#timeouts VaultClusterAdminToken#timeouts}
+        :param cluster_id: The ID of the HCP Vault cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token#cluster_id VaultClusterAdminToken#cluster_id}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token#id VaultClusterAdminToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_id: The ID of the HCP project where the HCP Vault cluster is located. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token#project_id VaultClusterAdminToken#project_id}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token#timeouts VaultClusterAdminToken#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = VaultClusterAdminTokenTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__83e679d92c18871e7ba585dbaa17bf175d7732a6c8292545e7d48798de47cf92)
@@ -344,44 +344,44 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def cluster_id(self) -> builtins.str:
         '''The ID of the HCP Vault cluster.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token#cluster_id VaultClusterAdminToken#cluster_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token#cluster_id VaultClusterAdminToken#cluster_id}
         '''
         result = self._values.get("cluster_id")
         assert result is not None, "Required property 'cluster_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token#id VaultClusterAdminToken#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token#id VaultClusterAdminToken#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def project_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the HCP project where the HCP Vault cluster is located.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token#project_id VaultClusterAdminToken#project_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token#project_id VaultClusterAdminToken#project_id}
         '''
         result = self._values.get("project_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["VaultClusterAdminTokenTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token#timeouts VaultClusterAdminToken#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token#timeouts VaultClusterAdminToken#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["VaultClusterAdminTokenTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -404,17 +404,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         read: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token#create VaultClusterAdminToken#create}.
-        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token#delete VaultClusterAdminToken#delete}.
-        :param read: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token#read VaultClusterAdminToken#read}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token#create VaultClusterAdminToken#create}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token#delete VaultClusterAdminToken#delete}.
+        :param read: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token#read VaultClusterAdminToken#read}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7b913c5a37226d68faee27ca7806a92620ab10ea5f6187e16ee77f2822bc1d2d)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
             check_type(argname="argument read", value=read, expected_type=type_hints["read"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -423,27 +423,27 @@
         if delete is not None:
             self._values["delete"] = delete
         if read is not None:
             self._values["read"] = read
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token#create VaultClusterAdminToken#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token#create VaultClusterAdminToken#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token#delete VaultClusterAdminToken#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token#delete VaultClusterAdminToken#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def read(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.59.0/docs/resources/vault_cluster_admin_token#read VaultClusterAdminToken#read}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcp/0.61.0/docs/resources/vault_cluster_admin_token#read VaultClusterAdminToken#read}.'''
         result = self._values.get("read")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp.egg-info/PKG-INFO` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-hcp
-Version: 4.0.3
+Version: 5.0.0
 Summary: Prebuilt hcp Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-hcp.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-hcp.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-hcp-4.0.3/src/cdktf_cdktf_provider_hcp.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-hcp-5.0.0/src/cdktf_cdktf_provider_hcp.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_hcp/py.typed
 src/cdktf_cdktf_provider_hcp.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_hcp.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_hcp.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_hcp.egg-info/requires.txt
 src/cdktf_cdktf_provider_hcp.egg-info/top_level.txt
 src/cdktf_cdktf_provider_hcp/_jsii/__init__.py
-src/cdktf_cdktf_provider_hcp/_jsii/provider-hcp@4.0.3.jsii.tgz
+src/cdktf_cdktf_provider_hcp/_jsii/provider-hcp@5.0.0.jsii.tgz
 src/cdktf_cdktf_provider_hcp/aws_network_peering/__init__.py
 src/cdktf_cdktf_provider_hcp/aws_transit_gateway_attachment/__init__.py
 src/cdktf_cdktf_provider_hcp/azure_peering_connection/__init__.py
 src/cdktf_cdktf_provider_hcp/boundary_cluster/__init__.py
 src/cdktf_cdktf_provider_hcp/consul_cluster/__init__.py
 src/cdktf_cdktf_provider_hcp/consul_cluster_root_token/__init__.py
 src/cdktf_cdktf_provider_hcp/consul_snapshot/__init__.py
@@ -30,14 +30,15 @@
 src/cdktf_cdktf_provider_hcp/data_hcp_hvn/__init__.py
 src/cdktf_cdktf_provider_hcp/data_hcp_hvn_peering_connection/__init__.py
 src/cdktf_cdktf_provider_hcp/data_hcp_hvn_route/__init__.py
 src/cdktf_cdktf_provider_hcp/data_hcp_packer_image/__init__.py
 src/cdktf_cdktf_provider_hcp/data_hcp_packer_image_iteration/__init__.py
 src/cdktf_cdktf_provider_hcp/data_hcp_packer_iteration/__init__.py
 src/cdktf_cdktf_provider_hcp/data_hcp_vault_cluster/__init__.py
+src/cdktf_cdktf_provider_hcp/data_hcp_vault_secrets_app/__init__.py
 src/cdktf_cdktf_provider_hcp/hvn/__init__.py
 src/cdktf_cdktf_provider_hcp/hvn_peering_connection/__init__.py
 src/cdktf_cdktf_provider_hcp/hvn_route/__init__.py
 src/cdktf_cdktf_provider_hcp/packer_channel/__init__.py
 src/cdktf_cdktf_provider_hcp/provider/__init__.py
 src/cdktf_cdktf_provider_hcp/vault_cluster/__init__.py
 src/cdktf_cdktf_provider_hcp/vault_cluster_admin_token/__init__.py
```

