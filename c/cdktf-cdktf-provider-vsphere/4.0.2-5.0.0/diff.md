# Comparing `tmp/cdktf-cdktf-provider-vsphere-4.0.2.tar.gz` & `tmp/cdktf-cdktf-provider-vsphere-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-vsphere-4.0.2.tar", last modified: Fri Jun  2 14:22:44 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-vsphere-5.0.0.tar", last modified: Thu Jun 15 11:39:33 2023, max compression
```

## Comparing `cdktf-cdktf-provider-vsphere-4.0.2.tar` & `cdktf-cdktf-provider-vsphere-5.0.0.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.257267 cdktf-cdktf-provider-vsphere-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-02 14:22:29.000000 cdktf-cdktf-provider-vsphere-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-02 14:22:44.257267 cdktf-cdktf-provider-vsphere-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 14:22:44.257267 cdktf-cdktf-provider-vsphere-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.229267 cdktf-cdktf-provider-vsphere-4.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.237266 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.237266 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   600174 2023-06-02 14:22:29.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/_jsii/provider-vsphere@4.0.2.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.241267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/compute_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)   258599 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/compute_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.241267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/compute_cluster_host_group/
--rw-r--r--   0 runner    (1001) docker     (123)    23525 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/compute_cluster_host_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.241267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_affinity_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    30050 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_affinity_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.241267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_anti_affinity_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    30314 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_anti_affinity_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.241267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_dependency_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    33343 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_dependency_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.241267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_group/
--rw-r--r--   0 runner    (1001) docker     (123)    23656 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.241267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_host_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    36225 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_host_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.241267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/content_library/
--rw-r--r--   0 runner    (1001) docker     (123)    60618 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/content_library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.241267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/content_library_item/
--rw-r--r--   0 runner    (1001) docker     (123)    30182 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/content_library_item/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.245267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/custom_attribute/
--rw-r--r--   0 runner    (1001) docker     (123)    20879 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/custom_attribute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.245267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_compute_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)    21028 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_compute_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.245267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_compute_cluster_host_group/
--rw-r--r--   0 runner    (1001) docker     (123)    21105 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_compute_cluster_host_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.245267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_content_library/
--rw-r--r--   0 runner    (1001) docker     (123)    17958 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_content_library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.245267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_content_library_item/
--rw-r--r--   0 runner    (1001) docker     (123)    22507 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_content_library_item/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.245267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_custom_attribute/
--rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_custom_attribute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.245267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_datacenter/
--rw-r--r--   0 runner    (1001) docker     (123)    18340 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_datacenter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.245267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_datastore/
--rw-r--r--   0 runner    (1001) docker     (123)    20813 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_datastore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.245267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_datastore_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)    20936 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_datastore_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.245267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_distributed_virtual_switch/
--rw-r--r--   0 runner    (1001) docker     (123)    21775 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_distributed_virtual_switch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.245267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_dynamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.245267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_folder/
--rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_folder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.245267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_host/
--rw-r--r--   0 runner    (1001) docker     (123)    20664 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_host/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.245267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_host_pci_device/
--rw-r--r--   0 runner    (1001) docker     (123)    25854 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_host_pci_device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.245267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_host_thumbprint/
--rw-r--r--   0 runner    (1001) docker     (123)    23621 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_host_thumbprint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.245267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_license/
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_license/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.245267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_network/
--rw-r--r--   0 runner    (1001) docker     (123)    24350 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.249266 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_ovf_vm_template/
--rw-r--r--   0 runner    (1001) docker     (123)    59374 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_ovf_vm_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.249266 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_resource_pool/
--rw-r--r--   0 runner    (1001) docker     (123)    21193 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_resource_pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.249266 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_role/
--rw-r--r--   0 runner    (1001) docker     (123)    25205 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.249266 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_storage_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    17950 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_storage_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.249266 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_tag/
--rw-r--r--   0 runner    (1001) docker     (123)    20098 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_tag/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.249266 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_tag_category/
--rw-r--r--   0 runner    (1001) docker     (123)    18456 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_tag_category/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.249266 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_vapp_container/
--rw-r--r--   0 runner    (1001) docker     (123)    20304 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_vapp_container/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.249266 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_virtual_machine/
--rw-r--r--   0 runner    (1001) docker     (123)   213606 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_virtual_machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.249266 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_vmfs_disks/
--rw-r--r--   0 runner    (1001) docker     (123)    24133 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_vmfs_disks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.249266 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/datacenter/
--rw-r--r--   0 runner    (1001) docker     (123)    25482 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/datacenter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.249266 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/datastore_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)    98575 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/datastore_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.249266 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/datastore_cluster_vm_anti_affinity_rule/
--rw-r--r--   0 runner    (1001) docker     (123)    30531 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/datastore_cluster_vm_anti_affinity_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.249266 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/distributed_port_group/
--rw-r--r--   0 runner    (1001) docker     (123)   183875 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/distributed_port_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.249266 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/distributed_virtual_switch/
--rw-r--r--   0 runner    (1001) docker     (123)   358617 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/distributed_virtual_switch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.249266 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/dpm_host_override/
--rw-r--r--   0 runner    (1001) docker     (123)    26705 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/dpm_host_override/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.253267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/drs_vm_override/
--rw-r--r--   0 runner    (1001) docker     (123)    26905 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/drs_vm_override/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.253267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/entity_permissions/
--rw-r--r--   0 runner    (1001) docker     (123)    42876 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/entity_permissions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.253267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/file/
--rw-r--r--   0 runner    (1001) docker     (123)    32371 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.253267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/folder/
--rw-r--r--   0 runner    (1001) docker     (123)    27933 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/folder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.253267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/ha_vm_override/
--rw-r--r--   0 runner    (1001) docker     (123)    65637 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/ha_vm_override/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.253267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/host/
--rw-r--r--   0 runner    (1001) docker     (123)    52455 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/host/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.253267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/host_port_group/
--rw-r--r--   0 runner    (1001) docker     (123)    76884 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/host_port_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.253267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/host_virtual_switch/
--rw-r--r--   0 runner    (1001) docker     (123)    78981 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/host_virtual_switch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.253267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/license_resource/
--rw-r--r--   0 runner    (1001) docker     (123)    21004 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/license_resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.253267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/nas_datastore/
--rw-r--r--   0 runner    (1001) docker     (123)    45501 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/nas_datastore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.253267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    41115 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.253267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/resource_pool/
--rw-r--r--   0 runner    (1001) docker     (123)    59676 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/resource_pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.253267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/role/
--rw-r--r--   0 runner    (1001) docker     (123)    20395 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.253267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/storage_drs_vm_override/
--rw-r--r--   0 runner    (1001) docker     (123)    29813 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/storage_drs_vm_override/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.253267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/tag/
--rw-r--r--   0 runner    (1001) docker     (123)    22294 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/tag/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.253267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/tag_category/
--rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/tag_category/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.253267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/vapp_container/
--rw-r--r--   0 runner    (1001) docker     (123)    59255 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/vapp_container/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.257267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/vapp_entity/
--rw-r--r--   0 runner    (1001) docker     (123)    43070 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/vapp_entity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.257267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/virtual_disk/
--rw-r--r--   0 runner    (1001) docker     (123)    31785 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/virtual_disk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.257267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/virtual_machine/
--rw-r--r--   0 runner    (1001) docker     (123)   518258 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/virtual_machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.257267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/virtual_machine_snapshot/
--rw-r--r--   0 runner    (1001) docker     (123)    34295 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/virtual_machine_snapshot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.257267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/vm_storage_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    41018 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/vm_storage_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.257267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/vmfs_datastore/
--rw-r--r--   0 runner    (1001) docker     (123)    34708 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/vmfs_datastore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.257267 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/vnic/
--rw-r--r--   0 runner    (1001) docker     (123)    65457 2023-06-02 14:22:30.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/vnic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:22:44.237266 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-02 14:22:44.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-02 14:22:44.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:22:44.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-02 14:22:44.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 14:22:44.000000 cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.721512 cdktf-cdktf-provider-vsphere-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-15 11:39:33.721512 cdktf-cdktf-provider-vsphere-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:39:33.721512 cdktf-cdktf-provider-vsphere-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.705512 cdktf-cdktf-provider-vsphere-5.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.709513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.709513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   600182 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/_jsii/provider-vsphere@5.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.709513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/compute_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)   258599 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/compute_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/compute_cluster_host_group/
+-rw-r--r--   0 runner    (1001) docker     (123)    23525 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/compute_cluster_host_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_affinity_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    30050 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_affinity_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_anti_affinity_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    30314 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_anti_affinity_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_dependency_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    33343 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_dependency_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_group/
+-rw-r--r--   0 runner    (1001) docker     (123)    23656 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_host_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    36225 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_host_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/content_library/
+-rw-r--r--   0 runner    (1001) docker     (123)    60618 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/content_library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/content_library_item/
+-rw-r--r--   0 runner    (1001) docker     (123)    30182 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/content_library_item/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/custom_attribute/
+-rw-r--r--   0 runner    (1001) docker     (123)    20879 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/custom_attribute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_compute_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)    21028 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_compute_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_compute_cluster_host_group/
+-rw-r--r--   0 runner    (1001) docker     (123)    21105 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_compute_cluster_host_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_content_library/
+-rw-r--r--   0 runner    (1001) docker     (123)    17958 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_content_library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_content_library_item/
+-rw-r--r--   0 runner    (1001) docker     (123)    22507 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_content_library_item/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_custom_attribute/
+-rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_custom_attribute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_datacenter/
+-rw-r--r--   0 runner    (1001) docker     (123)    18340 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_datacenter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)    20813 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_datastore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_datastore_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)    20936 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_datastore_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_distributed_virtual_switch/
+-rw-r--r--   0 runner    (1001) docker     (123)    21775 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_distributed_virtual_switch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_dynamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_folder/
+-rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_folder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_host/
+-rw-r--r--   0 runner    (1001) docker     (123)    20664 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_host/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_host_pci_device/
+-rw-r--r--   0 runner    (1001) docker     (123)    25854 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_host_pci_device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_host_thumbprint/
+-rw-r--r--   0 runner    (1001) docker     (123)    23621 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_host_thumbprint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_license/
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_license/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_network/
+-rw-r--r--   0 runner    (1001) docker     (123)    24350 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_ovf_vm_template/
+-rw-r--r--   0 runner    (1001) docker     (123)    59374 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_ovf_vm_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_resource_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)    21193 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_resource_pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.713513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    25205 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_storage_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    17950 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_storage_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_tag/
+-rw-r--r--   0 runner    (1001) docker     (123)    20098 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_tag/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_tag_category/
+-rw-r--r--   0 runner    (1001) docker     (123)    18456 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_tag_category/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_vapp_container/
+-rw-r--r--   0 runner    (1001) docker     (123)    20304 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_vapp_container/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_virtual_machine/
+-rw-r--r--   0 runner    (1001) docker     (123)   213606 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_virtual_machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_vmfs_disks/
+-rw-r--r--   0 runner    (1001) docker     (123)    24133 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_vmfs_disks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/datacenter/
+-rw-r--r--   0 runner    (1001) docker     (123)    25482 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/datacenter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/datastore_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)    98575 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/datastore_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/datastore_cluster_vm_anti_affinity_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)    30531 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/datastore_cluster_vm_anti_affinity_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/distributed_port_group/
+-rw-r--r--   0 runner    (1001) docker     (123)   183875 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/distributed_port_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/distributed_virtual_switch/
+-rw-r--r--   0 runner    (1001) docker     (123)   358617 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/distributed_virtual_switch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/dpm_host_override/
+-rw-r--r--   0 runner    (1001) docker     (123)    26705 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/dpm_host_override/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/drs_vm_override/
+-rw-r--r--   0 runner    (1001) docker     (123)    26905 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/drs_vm_override/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/entity_permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)    42876 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/entity_permissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/file/
+-rw-r--r--   0 runner    (1001) docker     (123)    32371 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/folder/
+-rw-r--r--   0 runner    (1001) docker     (123)    27933 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/folder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/ha_vm_override/
+-rw-r--r--   0 runner    (1001) docker     (123)    65637 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/ha_vm_override/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/host/
+-rw-r--r--   0 runner    (1001) docker     (123)    52455 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/host/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/host_port_group/
+-rw-r--r--   0 runner    (1001) docker     (123)    76884 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/host_port_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/host_virtual_switch/
+-rw-r--r--   0 runner    (1001) docker     (123)    78981 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/host_virtual_switch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/license_resource/
+-rw-r--r--   0 runner    (1001) docker     (123)    21004 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/license_resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/nas_datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)    45501 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/nas_datastore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.717512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    41115 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.721512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/resource_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)    59676 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/resource_pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.721512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/role/
+-rw-r--r--   0 runner    (1001) docker     (123)    20395 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.721512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/storage_drs_vm_override/
+-rw-r--r--   0 runner    (1001) docker     (123)    29813 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/storage_drs_vm_override/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.721512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/tag/
+-rw-r--r--   0 runner    (1001) docker     (123)    22294 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/tag/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.721512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/tag_category/
+-rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/tag_category/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.721512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/vapp_container/
+-rw-r--r--   0 runner    (1001) docker     (123)    59255 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/vapp_container/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.721512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/vapp_entity/
+-rw-r--r--   0 runner    (1001) docker     (123)    43070 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/vapp_entity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.721512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/virtual_disk/
+-rw-r--r--   0 runner    (1001) docker     (123)    31785 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/virtual_disk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.721512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/virtual_machine/
+-rw-r--r--   0 runner    (1001) docker     (123)   518258 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/virtual_machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.721512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/virtual_machine_snapshot/
+-rw-r--r--   0 runner    (1001) docker     (123)    34295 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/virtual_machine_snapshot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.721512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/vm_storage_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    41018 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/vm_storage_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.721512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/vmfs_datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)    34708 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/vmfs_datastore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.721512 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/vnic/
+-rw-r--r--   0 runner    (1001) docker     (123)    65457 2023-06-15 11:39:19.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/vnic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:39:33.709513 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-15 11:39:33.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-15 11:39:33.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:39:33.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 11:39:33.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 11:39:33.000000 cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/LICENSE` & `cdktf-cdktf-provider-vsphere-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/PKG-INFO` & `cdktf-cdktf-provider-vsphere-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-vsphere
-Version: 4.0.2
+Version: 5.0.0
 Summary: Prebuilt vsphere Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-vsphere.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-vsphere.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/README.md` & `cdktf-cdktf-provider-vsphere-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/setup.py` & `cdktf-cdktf-provider-vsphere-5.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-vsphere",
-    "version": "4.0.2",
+    "version": "5.0.0",
     "description": "Prebuilt vsphere Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-vsphere.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -87,25 +87,25 @@
         "cdktf_cdktf_provider_vsphere.virtual_machine_snapshot",
         "cdktf_cdktf_provider_vsphere.vm_storage_policy",
         "cdktf_cdktf_provider_vsphere.vmfs_datastore",
         "cdktf_cdktf_provider_vsphere.vnic"
     ],
     "package_data": {
         "cdktf_cdktf_provider_vsphere._jsii": [
-            "provider-vsphere@4.0.2.jsii.tgz"
+            "provider-vsphere@5.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_vsphere": [
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

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/compute_cluster/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/compute_cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/compute_cluster_host_group/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/compute_cluster_host_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_affinity_rule/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_affinity_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_anti_affinity_rule/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_anti_affinity_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_dependency_rule/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_dependency_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_group/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_host_rule/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_host_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/content_library/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/content_library/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/content_library_item/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/content_library_item/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/custom_attribute/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/custom_attribute/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_compute_cluster/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_compute_cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_compute_cluster_host_group/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_compute_cluster_host_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_content_library/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_content_library/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_content_library_item/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_content_library_item/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_custom_attribute/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_custom_attribute/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_datacenter/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_datacenter/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_datastore/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_datastore_cluster/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_datastore_cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_distributed_virtual_switch/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_distributed_virtual_switch/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_dynamic/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_dynamic/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_folder/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_folder/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_host/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_host/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_host_pci_device/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_host_pci_device/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_host_thumbprint/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_host_thumbprint/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_license/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_license/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_network/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_network/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_ovf_vm_template/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_ovf_vm_template/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_resource_pool/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_resource_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_role/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_storage_policy/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_storage_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_tag/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_tag/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_tag_category/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_tag_category/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_vapp_container/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_vapp_container/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_virtual_machine/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_virtual_machine/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/data_vsphere_vmfs_disks/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/data_vsphere_vmfs_disks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/datacenter/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/datacenter/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/datastore_cluster/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/datastore_cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/datastore_cluster_vm_anti_affinity_rule/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/datastore_cluster_vm_anti_affinity_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/distributed_port_group/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/distributed_port_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/distributed_virtual_switch/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/distributed_virtual_switch/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/dpm_host_override/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/dpm_host_override/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/drs_vm_override/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/drs_vm_override/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/entity_permissions/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/entity_permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/file/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/file/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/folder/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/folder/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/ha_vm_override/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/ha_vm_override/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/host/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/host/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/host_port_group/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/host_port_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/host_virtual_switch/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/host_virtual_switch/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/license_resource/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/license_resource/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/nas_datastore/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/nas_datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/provider/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/resource_pool/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/resource_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/role/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/storage_drs_vm_override/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/storage_drs_vm_override/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/tag/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/tag/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/tag_category/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/tag_category/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/vapp_container/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/vapp_container/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/vapp_entity/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/vapp_entity/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/virtual_disk/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/virtual_disk/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/virtual_machine/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/virtual_machine/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/virtual_machine_snapshot/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/virtual_machine_snapshot/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/vm_storage_policy/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/vm_storage_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/vmfs_datastore/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/vmfs_datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere/vnic/__init__.py` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere/vnic/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere.egg-info/PKG-INFO` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-vsphere
-Version: 4.0.2
+Version: 5.0.0
 Summary: Prebuilt vsphere Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-vsphere.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-vsphere.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-vsphere-4.0.2/src/cdktf_cdktf_provider_vsphere.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-vsphere-5.0.0/src/cdktf_cdktf_provider_vsphere.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_vsphere/py.typed
 src/cdktf_cdktf_provider_vsphere.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_vsphere.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_vsphere.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_vsphere.egg-info/requires.txt
 src/cdktf_cdktf_provider_vsphere.egg-info/top_level.txt
 src/cdktf_cdktf_provider_vsphere/_jsii/__init__.py
-src/cdktf_cdktf_provider_vsphere/_jsii/provider-vsphere@4.0.2.jsii.tgz
+src/cdktf_cdktf_provider_vsphere/_jsii/provider-vsphere@5.0.0.jsii.tgz
 src/cdktf_cdktf_provider_vsphere/compute_cluster/__init__.py
 src/cdktf_cdktf_provider_vsphere/compute_cluster_host_group/__init__.py
 src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_affinity_rule/__init__.py
 src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_anti_affinity_rule/__init__.py
 src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_dependency_rule/__init__.py
 src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_group/__init__.py
 src/cdktf_cdktf_provider_vsphere/compute_cluster_vm_host_rule/__init__.py
```

