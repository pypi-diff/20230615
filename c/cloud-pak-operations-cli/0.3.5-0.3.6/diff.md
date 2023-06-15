# Comparing `tmp/cloud-pak-operations-cli-0.3.5.tar.gz` & `tmp/cloud-pak-operations-cli-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-pak-operations-cli-0.3.5.tar", last modified: Wed May 24 11:28:56 2023, max compression
+gzip compressed data, was "cloud-pak-operations-cli-0.3.6.tar", last modified: Thu Jun 15 14:41:24 2023, max compression
```

## Comparing `cloud-pak-operations-cli-0.3.5.tar` & `cloud-pak-operations-cli-0.3.6.tar`

### file list

```diff
@@ -1,316 +1,319 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:56.023491 cloud-pak-operations-cli-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-05-24 11:28:56.023491 cloud-pak-operations-cli-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.951490 cloud-pak-operations-cli-0.3.5/cloud_pak_operations_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-05-24 11:28:55.000000 cloud-pak-operations-cli-0.3.5/cloud_pak_operations_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-05-24 11:28:55.000000 cloud-pak-operations-cli-0.3.5/cloud_pak_operations_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:28:55.000000 cloud-pak-operations-cli-0.3.5/cloud_pak_operations_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-24 11:28:55.000000 cloud-pak-operations-cli-0.3.5/cloud_pak_operations_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-24 11:28:55.000000 cloud-pak-operations-cli-0.3.5/cloud_pak_operations_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-24 11:28:55.000000 cloud-pak-operations-cli-0.3.5/cloud_pak_operations_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.951490 cloud-pak-operations-cli-0.3.5/cpo/
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.955490 cloud-pak-operations-cli-0.3.5/cpo/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.955490 cloud-pak-operations-cli-0.3.5/cpo/commands/adm/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/adm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.955490 cloud-pak-operations-cli-0.3.5/cpo/commands/adm/config/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/adm/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/adm/config/set.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/adm/download_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/adm/get-shell-completion-script-location.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.955490 cloud-pak-operations-cli-0.3.5/cpo/commands/adm/ibm_internal_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/adm/ibm_internal_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/adm/ibm_internal_plugin/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/adm/ibm_internal_plugin/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/adm/store_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/adm/update_dev.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.959490 cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/current.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/get_cluster_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/install_nfs_storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/install_odf_storage_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/ls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.963490 cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/pull_secret/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/pull_secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/pull_secret/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/pull_secret/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/pull_secret/set.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/use.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.963490 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.971490 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/accept_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/add_worker_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/boot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/boot_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/copy_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/create_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/disable_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/edit_inf_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/edit_master_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/edit_worker_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/enable_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/init_node_for_db2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/install_nfs_storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/reboot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/reboot_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/redeploy_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/shutdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/shutdown_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/transfer_ownership.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.971490 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/info/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/info/check_cluster_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/info/get_default_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/info/get_openshift_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/info/get_openshift_versions_all_platforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/info/get_quick_burn_max_hours.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/info/get_quick_burn_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/info/get_quota.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/info/get_request_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/info/wait_for_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/logout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.975490 cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/logout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.975490 cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/oc/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/oc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.979490 cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/oc/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/oc/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/oc/cluster/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/oc/cluster/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/oc/cluster/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/oc/cluster/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/oc/cluster/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/regenerate_api_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.979490 cloud-pak-operations-cli-0.3.5/cpo/config/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/config/binaries_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/config/cluster_credentials_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8953 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/config/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/cpo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.943490 cloud-pak-operations-cli-0.3.5/cpo/deps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.979490 cloud-pak-operations-cli-0.3.5/cpo/deps/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/deps/autocomplete/cpo-autocomplete-bash.sh
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/deps/autocomplete/cpo-autocomplete-zsh.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.979490 cloud-pak-operations-cli-0.3.5/cpo/deps/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/deps/playbooks/deploy_odf_playbook.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.979490 cloud-pak-operations-cli-0.3.5/cpo/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.979490 cloud-pak-operations-cli-0.3.5/cpo/lib/ansible/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ansible/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.983490 cloud-pak-operations-cli-0.3.5/cpo/lib/ansible/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ansible/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ansible/modules/abstract_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ansible/modules/custom_resource_event_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ansible/modules/wait_for_custom_resource_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ansible/modules/wait_for_namespaced_custom_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ansible/openshift_playbook_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ansible/playbook_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.983490 cloud-pak-operations-cli-0.3.5/cpo/lib/ansible/playbook_runners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ansible/playbook_runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ansible/playbook_runners/deploy_odf_playbook_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.983490 cloud-pak-operations-cli-0.3.5/cpo/lib/click/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/click/cpd_service_spec_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/click/lazy_loading_multi_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.983490 cloud-pak-operations-cli-0.3.5/cpo/lib/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/cluster/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/cluster/cluster_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.983490 cloud-pak-operations-cli-0.3.5/cpo/lib/dependency_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/dependency_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/dependency_manager/dependency_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/dependency_manager/dependency_manager_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.987490 cloud-pak-operations-cli-0.3.5/cpo/lib/dependency_manager/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/dependency_manager/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/dependency_manager/plugins/ibm_cloud_cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/dependency_manager/plugins/ibm_cloud_pak_cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/dependency_manager/plugins/ibm_cloud_terraform_provider_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/dependency_manager/plugins/openshift_cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/dependency_manager/plugins/terraform_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.987490 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.987490 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/cluster/ocpplus_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/cluster/ocpplus_cluster_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.991490 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/check_hostname_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/ocp_available_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/ocpplus_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/ocpplus_cluster_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/ocpplus_cluster_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/openshift_version_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/product_group_quota_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/quick_burn_max_hours_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/quick_burn_size_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/request_status_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/status_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    31273 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/ocp_plus_api_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.995490 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/check_hostname_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/json_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_accept_transfer_put_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_add_additional_nodes_put_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_available_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_cluster_action_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_default_post_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_delete_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_disable_delete_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_disk_put_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_enable_delete_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_get_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_get_manager_for_single_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_node_action_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_post_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_quick_burn_max_hours_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_quick_burn_sizes_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_resource_put_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_status_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_transfer_put_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/quota_request_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:55.999490 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/check_hostname_get_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/default_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/json_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/ocp_available_get_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/ocp_get_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/ocp_get_response_manager_for_single_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/ocp_post_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/ocp_quick_burn_max_hours_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/ocp_quick_burn_sizes_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/ocp_request_get_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/ocp_status_get_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/quota_get_response_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:56.007490 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/check_hostname_get_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/default_error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/default_success_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_add_additional_nodes_put_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_available_get_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_disk_put_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_get_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_get_response_for_single_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_post_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_post_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_quick_burn_max_hours_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_quick_burn_sizes_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_request_get_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_resource_put_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_status_get_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_transfer_put_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/quota_get_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:56.007490 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/utils/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/utils/node_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/utils/openshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/utils/request_status_progress_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:56.007490 cloud-pak-operations-cli-0.3.5/cpo/lib/ibm_internal_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ibm_internal_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ibm_internal_plugin/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ibm_internal_plugin/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:56.011490 cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:56.011490 cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/data/cluster_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/data/ingress_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    19570 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/ibm_cloud_api_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:56.011490 cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/oc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/oc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:56.011490 cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/oc/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/oc/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/oc/cluster/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/oc/cluster/roks_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/oc/cluster/roks_cluster_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/jmespath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:56.011490 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:56.015490 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/cluster/generic_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/cluster/generic_cluster_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:56.015490 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/credentials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/credentials/cluster_based_user_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/credentials/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/credentials/token_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/credentials/user_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:56.015490 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/data/global_pull_secret_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:56.015490 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/nfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/nfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/nfs/nfs_subdir_external_provisioner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/oc.py
--rw-r--r--   0 runner    (1001) docker     (123)    45780 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/openshift_api_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:56.019490 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/auths_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/catalog_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/custom_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/custom_resource_event_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/get_pod_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/kind_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/object_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/operator_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/role_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:56.019490 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/utils/click.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:56.019490 cloud-pak-operations-cli-0.3.5/cpo/lib/plugin_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/plugin_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/plugin_manager/distribution_entry_point_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/plugin_manager/package_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/lib/plugin_manager/plugin_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:56.023491 cloud-pak-operations-cli-0.3.5/cpo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/utils/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/utils/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/utils/http_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/utils/importlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/utils/operating_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/utils/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/utils/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/cpo/utils/wait.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-24 11:28:44.000000 cloud-pak-operations-cli-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-24 11:28:56.027490 cloud-pak-operations-cli-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.837862 cloud-pak-operations-cli-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-06-15 14:41:24.837862 cloud-pak-operations-cli-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.805862 cloud-pak-operations-cli-0.3.6/cloud_pak_operations_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-06-15 14:41:24.000000 cloud-pak-operations-cli-0.3.6/cloud_pak_operations_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-15 14:41:24.000000 cloud-pak-operations-cli-0.3.6/cloud_pak_operations_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:41:24.000000 cloud-pak-operations-cli-0.3.6/cloud_pak_operations_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-15 14:41:24.000000 cloud-pak-operations-cli-0.3.6/cloud_pak_operations_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-15 14:41:24.000000 cloud-pak-operations-cli-0.3.6/cloud_pak_operations_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 14:41:24.000000 cloud-pak-operations-cli-0.3.6/cloud_pak_operations_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.805862 cloud-pak-operations-cli-0.3.6/cpo/
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.805862 cloud-pak-operations-cli-0.3.6/cpo/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.805862 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.805862 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/config/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/download_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/get-shell-completion-script-location.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.809862 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/ibm_internal_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/ibm_internal_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/ibm_internal_plugin/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/ibm_internal_plugin/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/store_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/update_dev.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.809862 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/get_cluster_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/install_nfs_storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/install_odf_storage_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/ls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.809862 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/pull_secret/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/pull_secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/pull_secret/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/pull_secret/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/pull_secret/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/use.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.809862 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.813862 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/accept_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/add_worker_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/boot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/boot_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/copy_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/create_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/disable_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/edit_inf_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/edit_master_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/edit_worker_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/enable_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/init_node_for_db2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/install_nfs_storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/reboot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/reboot_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/redeploy_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/shutdown_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/transfer_ownership.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.813862 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/check_cluster_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_default_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_openshift_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_openshift_versions_all_platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_quick_burn_max_hours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_quick_burn_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_quota.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_request_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/wait_for_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/logout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.813862 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/logout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.813862 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.813862 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/regenerate_api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.813862 cloud-pak-operations-cli-0.3.6/cpo/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/config/binaries_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/config/cluster_credentials_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8953 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/config/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/cpo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.801862 cloud-pak-operations-cli-0.3.6/cpo/deps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/deps/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/deps/autocomplete/cpo-autocomplete-bash.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/deps/autocomplete/cpo-autocomplete-zsh.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/deps/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/deps/playbooks/deploy_odf_playbook.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/modules/abstract_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/modules/custom_resource_event_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/modules/wait_for_custom_resource_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/modules/wait_for_namespaced_custom_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/openshift_playbook_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/playbook_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/playbook_runners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/playbook_runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/playbook_runners/deploy_odf_playbook_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/lib/click/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/click/cpd_service_spec_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/click/lazy_loading_multi_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/lib/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/cluster/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/cluster/cluster_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/dependency_manager_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/ibm_cloud_cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/ibm_cloud_pak_cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/ibm_cloud_terraform_provider_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/openshift_cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/terraform_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.821862 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/cluster/ocpplus_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/cluster/ocpplus_cluster_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.821862 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/check_hostname_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/ocp_available_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/ocpplus_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/ocpplus_cluster_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/ocpplus_cluster_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/openshift_version_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/product_group_quota_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/quick_burn_max_hours_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/quick_burn_size_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/request_status_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/status_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31273 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/ocp_plus_api_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.825862 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/check_hostname_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/json_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_accept_transfer_put_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_add_additional_nodes_put_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_available_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_cluster_action_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_default_post_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_delete_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_disable_delete_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_disk_put_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_enable_delete_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_get_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_get_manager_for_single_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_node_action_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_post_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_quick_burn_max_hours_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_quick_burn_sizes_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_resource_put_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_status_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_transfer_put_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/quota_request_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.825862 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/check_hostname_get_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/default_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/json_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_available_get_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_get_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_get_response_manager_for_single_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_post_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_quick_burn_max_hours_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_quick_burn_sizes_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_request_get_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_status_get_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/quota_get_response_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.825862 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/check_hostname_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/default_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/default_success_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_add_additional_nodes_put_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_available_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_disk_put_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_get_response_for_single_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_post_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_post_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_quick_burn_max_hours_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_quick_burn_sizes_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_request_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_resource_put_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_status_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_transfer_put_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/quota_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/utils/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/utils/node_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/utils/openshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/utils/request_status_progress_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/ibm_internal_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibm_internal_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibm_internal_plugin/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibm_internal_plugin/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/data/cluster_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/data/ingress_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19570 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/ibm_cloud_api_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/oc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/oc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/oc/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/oc/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/oc/cluster/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/oc/cluster/roks_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/oc/cluster/roks_cluster_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/jmespath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/cluster/generic_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/cluster/generic_cluster_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/credentials/cluster_based_user_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/credentials/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/credentials/token_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/credentials/user_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/data/global_pull_secret_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/nfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/nfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/nfs/nfs_subdir_external_provisioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/oc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45780 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/openshift_api_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.833862 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/auths_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/catalog_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/custom_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/custom_resource_event_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/get_pod_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/kind_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/object_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/operator_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/role_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.833862 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/utils/click.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.833862 cloud-pak-operations-cli-0.3.6/cpo/lib/plugin_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/plugin_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/plugin_manager/distribution_entry_point_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/plugin_manager/package_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/plugin_manager/plugin_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.833862 cloud-pak-operations-cli-0.3.6/cpo/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/scripts/get_current_cluster_alias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.837862 cloud-pak-operations-cli-0.3.6/cpo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/http_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/importlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 14:41:24.837862 cloud-pak-operations-cli-0.3.6/setup.cfg
```

### Comparing `cloud-pak-operations-cli-0.3.5/LICENSE` & `cloud-pak-operations-cli-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/PKG-INFO` & `cloud-pak-operations-cli-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-pak-operations-cli
-Version: 0.3.5
+Version: 0.3.6
 Summary: IBM Cloud Pak Operations CLI
 Author-email: IBM Corporation <db2datagate@ibm.com>
 Project-URL: repository, https://github.com/IBM/cloud-pak-operations-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cloud-pak-operations-cli Version: 0.3.5 Summary:
+Metadata-Version: 2.1 Name: cloud-pak-operations-cli Version: 0.3.6 Summary:
 IBM Cloud Pak Operations CLI Author-email: IBM Corporation
 ibm.com> Project-URL: repository, https://github.com/IBM/cloud-pak-operations-
 cli Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows Classifier: Operating
 System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
```

### Comparing `cloud-pak-operations-cli-0.3.5/README.md` & `cloud-pak-operations-cli-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cloud_pak_operations_cli.egg-info/PKG-INFO` & `cloud-pak-operations-cli-0.3.6/cloud_pak_operations_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-pak-operations-cli
-Version: 0.3.5
+Version: 0.3.6
 Summary: IBM Cloud Pak Operations CLI
 Author-email: IBM Corporation <db2datagate@ibm.com>
 Project-URL: repository, https://github.com/IBM/cloud-pak-operations-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cloud-pak-operations-cli Version: 0.3.5 Summary:
+Metadata-Version: 2.1 Name: cloud-pak-operations-cli Version: 0.3.6 Summary:
 IBM Cloud Pak Operations CLI Author-email: IBM Corporation
 ibm.com> Project-URL: repository, https://github.com/IBM/cloud-pak-operations-
 cli Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows Classifier: Operating
 System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
```

### Comparing `cloud-pak-operations-cli-0.3.5/cloud_pak_operations_cli.egg-info/SOURCES.txt` & `cloud-pak-operations-cli-0.3.6/cloud_pak_operations_cli.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -245,14 +245,16 @@
 cpo/lib/openshift/types/subscription.py
 cpo/lib/openshift/utils/__init__.py
 cpo/lib/openshift/utils/click.py
 cpo/lib/plugin_manager/__init__.py
 cpo/lib/plugin_manager/distribution_entry_point_loader.py
 cpo/lib/plugin_manager/package_data.py
 cpo/lib/plugin_manager/plugin_manager.py
+cpo/scripts/__init__.py
+cpo/scripts/get_current_cluster_alias.py
 cpo/utils/__init__.py
 cpo/utils/compression.py
 cpo/utils/debugger.py
 cpo/utils/download.py
 cpo/utils/error.py
 cpo/utils/file.py
 cpo/utils/http_method.py
```

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/__init__.py` & `cloud-pak-operations-cli-0.3.6/cpo/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/adm/__init__.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/adm/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/adm/config/__init__.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/adm/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/adm/config/set.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/adm/config/set.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/adm/download_dependencies.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/adm/download_dependencies.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/adm/get-shell-completion-script-location.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/adm/get-shell-completion-script-location.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/adm/ibm_internal_plugin/__init__.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/adm/ibm_internal_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/adm/ibm_internal_plugin/install.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/adm/ibm_internal_plugin/install.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/adm/ibm_internal_plugin/ls.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/adm/ibm_internal_plugin/ls.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/adm/store_credentials.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/adm/store_credentials.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/adm/update_dev.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/adm/update_dev.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/__init__.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/add.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/add.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/current.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/current.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,22 +8,33 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+from typing import Optional
+
 import click
 
 import cpo.config.cluster_credentials_manager
 
 from cpo.utils.logging import loglevel_command
 
 
 @loglevel_command()
-def current():
+@click.option(
+    "--print-alias", help="Print the alias used to reference a cluster instead of its server URL", is_flag=True
+)
+def current(print_alias: Optional[bool]):
     """Get the current registered OpenShift cluster"""
 
     current_cluster = cpo.config.cluster_credentials_manager.cluster_credentials_manager.get_current_cluster()
 
     if current_cluster is not None:
-        click.echo(current_cluster.get_server())
+        if not print_alias:
+            click.echo(current_cluster.get_server())
+        else:
+            cluster_data = current_cluster.get_cluster_data()
+
+            if "alias" in cluster_data:
+                click.echo(cluster_data["alias"])
```

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/edit.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/edit.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/get_cluster_access_token.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/get_cluster_access_token.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/install_nfs_storage_class.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/install_nfs_storage_class.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/install_odf_storage_classes.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/install_odf_storage_classes.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/login.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/login.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/ls.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/ls.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/pull_secret/__init__.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/pull_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/pull_secret/ls.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/pull_secret/ls.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/pull_secret/rm.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/pull_secret/rm.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/pull_secret/set.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/pull_secret/set.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/rm.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/rm.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/cluster/use.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/use.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/__init__.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/__init__.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/accept_transfer.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/accept_transfer.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/add.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/add.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/add_worker_node.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/add_worker_node.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/boot.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/boot.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/boot_node.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/boot_node.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/copy_ssh_key.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/copy_ssh_key.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/create.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/create.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/create_default.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/create_default.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/details.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/details.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/disable_delete.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/disable_delete.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/edit_inf_node.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/edit_inf_node.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/edit_master_node.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/edit_master_node.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/edit_worker_node.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/edit_worker_node.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/enable_delete.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/enable_delete.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/init_node_for_db2.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/init_node_for_db2.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/install_nfs_storage_class.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/install_nfs_storage_class.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/ls.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/ls.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/reboot.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/reboot.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/reboot_node.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/reboot_node.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/redeploy_node.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/redeploy_node.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/rm.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/rm.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/shutdown.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/shutdown.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/shutdown_node.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/shutdown_node.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/ssh.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/status.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/status.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/cluster/transfer_ownership.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/transfer_ownership.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/info/__init__.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/info/check_cluster_name.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/check_cluster_name.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/info/get_default_sizes.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_default_sizes.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/info/get_openshift_versions.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_openshift_versions.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/info/get_openshift_versions_all_platforms.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_openshift_versions_all_platforms.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/info/get_quick_burn_max_hours.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_quick_burn_max_hours.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/info/get_quick_burn_sizes.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_quick_burn_sizes.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/info/get_quota.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_quota.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/info/get_request_status.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_request_status.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/info/wait_for_request.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/wait_for_request.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/login.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/login.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/fyre/logout.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/logout.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/__init__.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/login.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/login.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/logout.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/logout.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/oc/__init__.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/oc/cluster/__init__.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/oc/cluster/add.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/add.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/oc/cluster/login.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/login.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/oc/cluster/ls.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/ls.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/oc/cluster/rm.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/rm.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/oc/cluster/status.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/status.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/commands/ibmcloud/regenerate_api_key.py` & `cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/regenerate_api_key.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/config/__init__.py` & `cloud-pak-operations-cli-0.3.6/cpo/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/config/binaries_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/config/binaries_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/config/cluster_credentials_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/config/cluster_credentials_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/config/configuration_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/config/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/cpo.py` & `cloud-pak-operations-cli-0.3.6/cpo/cpo.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/deps/autocomplete/cpo-autocomplete-bash.sh` & `cloud-pak-operations-cli-0.3.6/cpo/deps/autocomplete/cpo-autocomplete-bash.sh`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/deps/autocomplete/cpo-autocomplete-zsh.sh` & `cloud-pak-operations-cli-0.3.6/cpo/deps/autocomplete/cpo-autocomplete-zsh.sh`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/deps/playbooks/deploy_odf_playbook.yaml` & `cloud-pak-operations-cli-0.3.6/cpo/deps/playbooks/deploy_odf_playbook.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         resource_definition:
           apiVersion: operators.coreos.com/v1alpha1
           kind: Subscription
           metadata:
             name: local-storage-operator
             namespace: openshift-local-storage
           spec:
-            channel: "{{ openshift_server_version | string }}"
+            channel: stable
             installPlanApproval: Automatic
             name: local-storage-operator
             source: redhat-operators
             sourceNamespace: openshift-marketplace
         state: present
 
     - name: "Waiting for creation of custom resource definitions"
```

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/ansible/modules/abstract_module.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/modules/abstract_module.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/ansible/modules/custom_resource_event_result.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/modules/custom_resource_event_result.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/ansible/modules/wait_for_custom_resource_definitions.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/modules/wait_for_custom_resource_definitions.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/ansible/modules/wait_for_namespaced_custom_resource.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/modules/wait_for_namespaced_custom_resource.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/ansible/openshift_playbook_runner.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/openshift_playbook_runner.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/ansible/playbook_runner.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/playbook_runner.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/ansible/playbook_runners/deploy_odf_playbook_runner.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/playbook_runners/deploy_odf_playbook_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,18 +8,23 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+import pathlib
+
 from cpo.lib.ansible.openshift_playbook_runner import OpenShiftPlaybookRunner
 from cpo.lib.openshift.credentials.credentials import AbstractCredentials
 
 
 class DeployODFPlaybookRunner(OpenShiftPlaybookRunner):
     def __init__(self, credentials: AbstractCredentials):
         super().__init__(self._get_playbook_name_from_class_name(), credentials)
 
         version = self._openshift_api_manager.get_version()
 
         self.openshift_server_version = f"{version.major}.{version.minor}"
+
+    def get_private_data_dir(self) -> pathlib.Path:
+        return super().get_private_data_dir()
```

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/click/cpd_service_spec_param_type.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/click/cpd_service_spec_param_type.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/click/lazy_loading_multi_command.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/click/lazy_loading_multi_command.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/click/utils.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/click/utils.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/cluster/__init__.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/cluster/cluster.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/cluster/cluster_factory.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/cluster/cluster_factory.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/dependency_manager/__init__.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/dependency_manager/dependency_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/dependency_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/dependency_manager/dependency_manager_plugin.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/dependency_manager_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/dependency_manager/plugins/ibm_cloud_cli_plugin.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/ibm_cloud_cli_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/dependency_manager/plugins/ibm_cloud_pak_cli_plugin.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/ibm_cloud_pak_cli_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/dependency_manager/plugins/ibm_cloud_terraform_provider_plugin.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/ibm_cloud_terraform_provider_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/dependency_manager/plugins/openshift_cli_plugin.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/openshift_cli_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/dependency_manager/plugins/terraform_plugin.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/terraform_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/cluster/__init__.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/cluster/ocpplus_cluster.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/cluster/ocpplus_cluster.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/cluster/ocpplus_cluster_factory.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/cluster/ocpplus_cluster_factory.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/check_hostname_data.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/check_hostname_data.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/ocp_available_data.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/ocp_available_data.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/ocpplus_cluster.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/ocpplus_cluster.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/ocpplus_cluster_data.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/ocpplus_cluster_data.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/ocpplus_cluster_specification.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/ocpplus_cluster_specification.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/openshift_version_data.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/openshift_version_data.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/product_group_quota_data.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/product_group_quota_data.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/quick_burn_max_hours_data.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/quick_burn_max_hours_data.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/quick_burn_size_data.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/quick_burn_size_data.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/request_status_data.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/request_status_data.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/data/status_data.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/status_data.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/ocp_plus_api_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/ocp_plus_api_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/check_hostname_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/check_hostname_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/json_request_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/json_request_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_accept_transfer_put_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_accept_transfer_put_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_add_additional_nodes_put_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_add_additional_nodes_put_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_available_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_available_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_cluster_action_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_cluster_action_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_default_post_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_default_post_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_delete_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_delete_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_disable_delete_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_disable_delete_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_disk_put_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_disk_put_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_enable_delete_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_enable_delete_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_get_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_get_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_get_manager_for_single_cluster.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_get_manager_for_single_cluster.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_node_action_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_node_action_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_post_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_post_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_quick_burn_max_hours_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_quick_burn_max_hours_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_quick_burn_sizes_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_quick_burn_sizes_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_resource_put_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_resource_put_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_status_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_status_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/ocp_transfer_put_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_transfer_put_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/request_managers/quota_request_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/quota_request_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/check_hostname_get_response_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/check_hostname_get_response_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/default_response_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/default_response_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/json_response_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/json_response_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/ocp_available_get_response_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_available_get_response_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/ocp_get_response_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_get_response_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/ocp_get_response_manager_for_single_cluster.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_get_response_manager_for_single_cluster.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/ocp_post_response_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_post_response_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/ocp_quick_burn_max_hours_response_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_quick_burn_max_hours_response_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/ocp_quick_burn_sizes_response_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_quick_burn_sizes_response_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/ocp_request_get_response_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_request_get_response_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/ocp_status_get_response_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_status_get_response_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/response_managers/quota_get_response_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/quota_get_response_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/check_hostname_get_response.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/check_hostname_get_response.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/default_error_response.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/default_error_response.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/default_success_response.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/default_success_response.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_add_additional_nodes_put_request.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_add_additional_nodes_put_request.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_available_get_response.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_available_get_response.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_disk_put_request.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_disk_put_request.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_get_response.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_get_response.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_get_response_for_single_cluster.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_get_response_for_single_cluster.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_post_request.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_post_request.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_post_response.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_post_response.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_quick_burn_max_hours_response.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_quick_burn_max_hours_response.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_quick_burn_sizes_response.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_quick_burn_sizes_response.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_request_get_response.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_request_get_response.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_resource_put_request.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_resource_put_request.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_status_get_response.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_status_get_response.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/ocp_transfer_put_request.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_transfer_put_request.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/quota_get_response.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/quota_get_response.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/types/shared.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/shared.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/utils/click.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/utils/click.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/utils/network.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/utils/network.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/utils/node_name.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/utils/node_name.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/utils/openshift.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/utils/openshift.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/fyre/utils/request_status_progress_bar.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/utils/request_status_progress_bar.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/ibm_internal_plugin/install.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/ibm_internal_plugin/install.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/ibm_internal_plugin/list.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/ibm_internal_plugin/list.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/__init__.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/data/cluster_status.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/data/cluster_status.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/data/ingress_status.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/data/ingress_status.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/ibm_cloud_api_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/ibm_cloud_api_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/oc/cluster/__init__.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/oc/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/oc/cluster/ls.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/oc/cluster/ls.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/oc/cluster/roks_cluster.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/oc/cluster/roks_cluster.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/ibmcloud/oc/cluster/roks_cluster_factory.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/oc/cluster/roks_cluster_factory.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/jmespath.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/jmespath.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/cluster/__init__.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/cluster/generic_cluster.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/cluster/generic_cluster.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/cluster/generic_cluster_factory.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/cluster/generic_cluster_factory.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/credentials/cluster_based_user_credentials.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/credentials/cluster_based_user_credentials.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/credentials/credentials.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/credentials/token_credentials.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/credentials/token_credentials.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/credentials/user_credentials.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/credentials/user_credentials.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/data/global_pull_secret_data.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/data/global_pull_secret_data.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/nfs/nfs_subdir_external_provisioner.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/nfs/nfs_subdir_external_provisioner.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/oc.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/oc.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/openshift_api_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/openshift_api_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/auths_dict.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/auths_dict.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/catalog_source.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/catalog_source.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/credentials.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/credentials.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/custom_resource.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/custom_resource.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/custom_resource_event_result.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/custom_resource_event_result.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/get_pod_entry.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/get_pod_entry.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/kind_metadata.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/kind_metadata.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/object_meta.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/object_meta.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/operator_group.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/operator_group.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/role.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/role.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/role_binding.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/role_binding.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/role_rule.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/role_rule.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/service_account.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/service_account.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/types/subscription.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/subscription.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/openshift/utils/click.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/utils/click.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/plugin_manager/distribution_entry_point_loader.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/plugin_manager/distribution_entry_point_loader.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/plugin_manager/package_data.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/plugin_manager/package_data.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/lib/plugin_manager/plugin_manager.py` & `cloud-pak-operations-cli-0.3.6/cpo/lib/plugin_manager/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/utils/compression.py` & `cloud-pak-operations-cli-0.3.6/cpo/utils/compression.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/utils/debugger.py` & `cloud-pak-operations-cli-0.3.6/cpo/utils/debugger.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/utils/download.py` & `cloud-pak-operations-cli-0.3.6/cpo/utils/download.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/utils/error.py` & `cloud-pak-operations-cli-0.3.6/cpo/utils/error.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/utils/file.py` & `cloud-pak-operations-cli-0.3.6/cpo/utils/file.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/utils/http_method.py` & `cloud-pak-operations-cli-0.3.6/cpo/utils/http_method.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/utils/importlib.py` & `cloud-pak-operations-cli-0.3.6/cpo/utils/importlib.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/utils/logging.py` & `cloud-pak-operations-cli-0.3.6/cpo/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/utils/network.py` & `cloud-pak-operations-cli-0.3.6/cpo/utils/network.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/utils/operating_system.py` & `cloud-pak-operations-cli-0.3.6/cpo/utils/operating_system.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/utils/path.py` & `cloud-pak-operations-cli-0.3.6/cpo/utils/path.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/utils/process.py` & `cloud-pak-operations-cli-0.3.6/cpo/utils/process.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/utils/ssh.py` & `cloud-pak-operations-cli-0.3.6/cpo/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/utils/string.py` & `cloud-pak-operations-cli-0.3.6/cpo/utils/string.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/cpo/utils/wait.py` & `cloud-pak-operations-cli-0.3.6/cpo/utils/wait.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.5/pyproject.toml` & `cloud-pak-operations-cli-0.3.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 dynamic = ["version"]
 name = "cloud-pak-operations-cli"
 readme = "README.md"
 requires-python = ">=3.8"
 
 [project.scripts]
 cpo = "cpo.cpo:cli"
+cpo-get-current-cluster-alias = "cpo.scripts.get_current_cluster_alias:get_current_cluster_alias"
 
 [project.urls]
 repository = "https://github.com/IBM/cloud-pak-operations-cli"
 
 [tool.pytest.ini_options]
 filterwarnings = [
 	# https://setuptools.pypa.io/en/latest/history.html#v67-3-2
```

