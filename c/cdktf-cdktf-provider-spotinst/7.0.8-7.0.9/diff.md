# Comparing `tmp/cdktf-cdktf-provider-spotinst-7.0.8.tar.gz` & `tmp/cdktf-cdktf-provider-spotinst-7.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-spotinst-7.0.8.tar", last modified: Fri Jun  2 03:17:54 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-spotinst-7.0.9.tar", last modified: Fri Jun  2 14:16:54 2023, max compression
```

## Comparing `cdktf-cdktf-provider-spotinst-7.0.8.tar` & `cdktf-cdktf-provider-spotinst-7.0.9.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.287846 cdktf-cdktf-provider-spotinst-7.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-02 03:17:54.287846 cdktf-cdktf-provider-spotinst-7.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 03:17:54.287846 cdktf-cdktf-provider-spotinst-7.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.267846 cdktf-cdktf-provider-spotinst-7.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.271846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.271846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1298803 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/_jsii/provider-spotinst@7.0.8.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.271846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/data_integration/
--rw-r--r--   0 runner    (1001) docker     (123)    29610 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/data_integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.275846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/elastigroup_aws/
--rw-r--r--   0 runner    (1001) docker     (123)  1474138 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/elastigroup_aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.275846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/elastigroup_aws_beanstalk/
--rw-r--r--   0 runner    (1001) docker     (123)   142471 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/elastigroup_aws_beanstalk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.275846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/elastigroup_aws_suspension/
--rw-r--r--   0 runner    (1001) docker     (123)    33850 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/elastigroup_aws_suspension/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.275846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/elastigroup_azure/
--rw-r--r--   0 runner    (1001) docker     (123)   416320 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/elastigroup_azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.275846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/elastigroup_azure_v3/
--rw-r--r--   0 runner    (1001) docker     (123)   218089 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/elastigroup_azure_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.275846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/elastigroup_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)   515017 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/elastigroup_gcp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.275846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/elastigroup_gke/
--rw-r--r--   0 runner    (1001) docker     (123)   461262 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/elastigroup_gke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.279846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/health_check/
--rw-r--r--   0 runner    (1001) docker     (123)    48732 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/health_check/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.279846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/managed_instance_aws/
--rw-r--r--   0 runner    (1001) docker     (123)   328023 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/managed_instance_aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.279846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/mrscaler_aws/
--rw-r--r--   0 runner    (1001) docker     (123)   590910 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/mrscaler_aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.279846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/multai_balancer/
--rw-r--r--   0 runner    (1001) docker     (123)    50263 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/multai_balancer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.279846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/multai_deployment/
--rw-r--r--   0 runner    (1001) docker     (123)    17708 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/multai_deployment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.279846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/multai_listener/
--rw-r--r--   0 runner    (1001) docker     (123)    59699 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/multai_listener/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.279846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/multai_routing_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/multai_routing_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.279846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/multai_target/
--rw-r--r--   0 runner    (1001) docker     (123)    44846 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/multai_target/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.279846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/multai_target_set/
--rw-r--r--   0 runner    (1001) docker     (123)    65888 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/multai_target_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.279846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_aks/
--rw-r--r--   0 runner    (1001) docker     (123)   317358 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_aks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.279846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_aks_np/
--rw-r--r--   0 runner    (1001) docker     (123)   190162 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_aks_np/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.279846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_aks_np_virtual_node_group/
--rw-r--r--   0 runner    (1001) docker     (123)   116045 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_aks_np_virtual_node_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.279846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_aks_virtual_node_group/
--rw-r--r--   0 runner    (1001) docker     (123)   164082 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_aks_virtual_node_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.279846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_aws/
--rw-r--r--   0 runner    (1001) docker     (123)   422088 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.283846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_aws_extended_resource_definition/
--rw-r--r--   0 runner    (1001) docker     (123)    21105 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_aws_extended_resource_definition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.283846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_aws_launch_spec/
--rw-r--r--   0 runner    (1001) docker     (123)   399606 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_aws_launch_spec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.283846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_ecs/
--rw-r--r--   0 runner    (1001) docker     (123)   393284 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_ecs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.283846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_ecs_launch_spec/
--rw-r--r--   0 runner    (1001) docker     (123)   225909 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_ecs_launch_spec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.283846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_gke_import/
--rw-r--r--   0 runner    (1001) docker     (123)   267832 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_gke_import/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.283846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_gke_launch_spec/
--rw-r--r--   0 runner    (1001) docker     (123)   301606 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_gke_launch_spec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.283846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_gke_launch_spec_import/
--rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_gke_launch_spec_import/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.283846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_spark/
--rw-r--r--   0 runner    (1001) docker     (123)   114753 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_spark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.283846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_spark_virtual_node_group/
--rw-r--r--   0 runner    (1001) docker     (123)    21156 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_spark_virtual_node_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.283846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.283846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/stateful_node_azure/
--rw-r--r--   0 runner    (1001) docker     (123)   646555 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/stateful_node_azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.283846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/subscription/
--rw-r--r--   0 runner    (1001) docker     (123)    26567 2023-06-02 03:17:42.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/subscription/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:17:54.271846 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-02 03:17:54.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-02 03:17:54.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 03:17:54.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-02 03:17:54.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-02 03:17:54.000000 cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.462041 cdktf-cdktf-provider-spotinst-7.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-02 14:16:54.462041 cdktf-cdktf-provider-spotinst-7.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 14:16:54.462041 cdktf-cdktf-provider-spotinst-7.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.442041 cdktf-cdktf-provider-spotinst-7.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.446041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.446041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1298798 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/_jsii/provider-spotinst@7.0.9.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.450041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/data_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)    29610 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/data_integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.450041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/elastigroup_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)  1474138 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/elastigroup_aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.450041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/elastigroup_aws_beanstalk/
+-rw-r--r--   0 runner    (1001) docker     (123)   142471 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/elastigroup_aws_beanstalk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.450041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/elastigroup_aws_suspension/
+-rw-r--r--   0 runner    (1001) docker     (123)    33850 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/elastigroup_aws_suspension/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.450041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/elastigroup_azure/
+-rw-r--r--   0 runner    (1001) docker     (123)   416320 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/elastigroup_azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.450041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/elastigroup_azure_v3/
+-rw-r--r--   0 runner    (1001) docker     (123)   218089 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/elastigroup_azure_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.450041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/elastigroup_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)   515017 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/elastigroup_gcp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.454041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/elastigroup_gke/
+-rw-r--r--   0 runner    (1001) docker     (123)   461262 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/elastigroup_gke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.454041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/health_check/
+-rw-r--r--   0 runner    (1001) docker     (123)    48732 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/health_check/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.454041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/managed_instance_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)   328023 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/managed_instance_aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.454041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/mrscaler_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)   590910 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/mrscaler_aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.454041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/multai_balancer/
+-rw-r--r--   0 runner    (1001) docker     (123)    50263 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/multai_balancer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.454041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/multai_deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)    17708 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/multai_deployment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.454041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/multai_listener/
+-rw-r--r--   0 runner    (1001) docker     (123)    59699 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/multai_listener/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.454041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/multai_routing_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    48826 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/multai_routing_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.454041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/multai_target/
+-rw-r--r--   0 runner    (1001) docker     (123)    44846 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/multai_target/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.454041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/multai_target_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    65888 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/multai_target_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.458041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_aks/
+-rw-r--r--   0 runner    (1001) docker     (123)   317358 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_aks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.458041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_aks_np/
+-rw-r--r--   0 runner    (1001) docker     (123)   190162 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_aks_np/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.458041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_aks_np_virtual_node_group/
+-rw-r--r--   0 runner    (1001) docker     (123)   116045 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_aks_np_virtual_node_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.458041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_aks_virtual_node_group/
+-rw-r--r--   0 runner    (1001) docker     (123)   164082 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_aks_virtual_node_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.458041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)   422088 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.458041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_aws_extended_resource_definition/
+-rw-r--r--   0 runner    (1001) docker     (123)    21105 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_aws_extended_resource_definition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.458041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_aws_launch_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)   399606 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_aws_launch_spec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.458041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)   393284 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_ecs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.458041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_ecs_launch_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)   225909 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_ecs_launch_spec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.462041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_gke_import/
+-rw-r--r--   0 runner    (1001) docker     (123)   267832 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_gke_import/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.462041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_gke_launch_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)   301606 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_gke_launch_spec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.462041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_gke_launch_spec_import/
+-rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_gke_launch_spec_import/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.462041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_spark/
+-rw-r--r--   0 runner    (1001) docker     (123)   114753 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_spark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.462041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_spark_virtual_node_group/
+-rw-r--r--   0 runner    (1001) docker     (123)    21156 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_spark_virtual_node_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.462041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.462041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/stateful_node_azure/
+-rw-r--r--   0 runner    (1001) docker     (123)   646555 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/stateful_node_azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.462041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/subscription/
+-rw-r--r--   0 runner    (1001) docker     (123)    26567 2023-06-02 14:16:41.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/subscription/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:16:54.446041 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-02 14:16:54.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-02 14:16:54.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:16:54.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-02 14:16:54.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-02 14:16:54.000000 cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/LICENSE` & `cdktf-cdktf-provider-spotinst-7.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/PKG-INFO` & `cdktf-cdktf-provider-spotinst-7.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-spotinst
-Version: 7.0.8
+Version: 7.0.9
 Summary: Prebuilt spotinst Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-spotinst.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-spotinst.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/README.md` & `cdktf-cdktf-provider-spotinst-7.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/setup.py` & `cdktf-cdktf-provider-spotinst-7.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-spotinst",
-    "version": "7.0.8",
+    "version": "7.0.9",
     "description": "Prebuilt spotinst Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-spotinst.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -56,23 +56,23 @@
         "cdktf_cdktf_provider_spotinst.ocean_spark_virtual_node_group",
         "cdktf_cdktf_provider_spotinst.provider",
         "cdktf_cdktf_provider_spotinst.stateful_node_azure",
         "cdktf_cdktf_provider_spotinst.subscription"
     ],
     "package_data": {
         "cdktf_cdktf_provider_spotinst._jsii": [
-            "provider-spotinst@7.0.8.jsii.tgz"
+            "provider-spotinst@7.0.9.jsii.tgz"
         ],
         "cdktf_cdktf_provider_spotinst": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdktf>=0.16.0, <0.17.0",
+        "cdktf>=0.16.3, <0.17.0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.81.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/data_integration/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/data_integration/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/elastigroup_aws/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/elastigroup_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/elastigroup_aws_beanstalk/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/elastigroup_aws_beanstalk/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/elastigroup_aws_suspension/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/elastigroup_aws_suspension/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/elastigroup_azure/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/elastigroup_azure/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/elastigroup_azure_v3/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/elastigroup_azure_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/elastigroup_gcp/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/elastigroup_gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/elastigroup_gke/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/elastigroup_gke/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/health_check/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/health_check/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/managed_instance_aws/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/managed_instance_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/mrscaler_aws/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/mrscaler_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/multai_balancer/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/multai_balancer/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/multai_deployment/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/multai_deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/multai_listener/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/multai_listener/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/multai_routing_rule/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/multai_routing_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/multai_target/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/multai_target/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/multai_target_set/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/multai_target_set/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_aks/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_aks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_aks_np/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_aks_np/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_aks_np_virtual_node_group/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_aks_np_virtual_node_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_aks_virtual_node_group/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_aks_virtual_node_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_aws/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_aws_extended_resource_definition/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_aws_extended_resource_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_aws_launch_spec/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_aws_launch_spec/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_ecs/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_ecs_launch_spec/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_ecs_launch_spec/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_gke_import/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_gke_import/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_gke_launch_spec/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_gke_launch_spec/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_gke_launch_spec_import/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_gke_launch_spec_import/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_spark/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_spark/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/ocean_spark_virtual_node_group/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/ocean_spark_virtual_node_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/provider/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/stateful_node_azure/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/stateful_node_azure/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst/subscription/__init__.py` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst.egg-info/PKG-INFO` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-spotinst
-Version: 7.0.8
+Version: 7.0.9
 Summary: Prebuilt spotinst Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-spotinst.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-spotinst.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-spotinst-7.0.8/src/cdktf_cdktf_provider_spotinst.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-spotinst-7.0.9/src/cdktf_cdktf_provider_spotinst.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_spotinst/py.typed
 src/cdktf_cdktf_provider_spotinst.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_spotinst.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_spotinst.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_spotinst.egg-info/requires.txt
 src/cdktf_cdktf_provider_spotinst.egg-info/top_level.txt
 src/cdktf_cdktf_provider_spotinst/_jsii/__init__.py
-src/cdktf_cdktf_provider_spotinst/_jsii/provider-spotinst@7.0.8.jsii.tgz
+src/cdktf_cdktf_provider_spotinst/_jsii/provider-spotinst@7.0.9.jsii.tgz
 src/cdktf_cdktf_provider_spotinst/data_integration/__init__.py
 src/cdktf_cdktf_provider_spotinst/elastigroup_aws/__init__.py
 src/cdktf_cdktf_provider_spotinst/elastigroup_aws_beanstalk/__init__.py
 src/cdktf_cdktf_provider_spotinst/elastigroup_aws_suspension/__init__.py
 src/cdktf_cdktf_provider_spotinst/elastigroup_azure/__init__.py
 src/cdktf_cdktf_provider_spotinst/elastigroup_azure_v3/__init__.py
 src/cdktf_cdktf_provider_spotinst/elastigroup_gcp/__init__.py
```

