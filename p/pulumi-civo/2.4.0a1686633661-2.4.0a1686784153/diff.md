# Comparing `tmp/pulumi_civo-2.4.0a1686633661.tar.gz` & `tmp/pulumi_civo-2.4.0a1686784153.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_civo-2.4.0a1686633661.tar", last modified: Tue Jun 13 05:28:18 2023, max compression
+gzip compressed data, was "pulumi_civo-2.4.0a1686784153.tar", last modified: Wed Jun 14 23:13:21 2023, max compression
```

## Comparing `pulumi_civo-2.4.0a1686633661.tar` & `pulumi_civo-2.4.0a1686784153.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:28:18.680394 pulumi_civo-2.4.0a1686633661/
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-13 05:28:18.680394 pulumi_civo-2.4.0a1686633661/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:28:18.680394 pulumi_civo-2.4.0a1686633661/pulumi_civo/
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39145 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:28:18.680394 pulumi_civo-2.4.0a1686633661/pulumi_civo/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    17497 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/dns_domain_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/dns_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    22605 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    24236 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/firewall_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/get_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/get_disk_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/get_dns_domain_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/get_dns_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/get_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/get_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/get_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/get_instances_size.py
--rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/get_kubernetes_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/get_kubernetes_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/get_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/get_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/get_object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/get_object_store_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/get_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/get_reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/get_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/get_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    47045 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/instance_reserved_ip_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    42980 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/kubernetes_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    22159 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/kubernetes_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/object_store_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    47516 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo/volume_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:28:18.680394 pulumi_civo-2.4.0a1686633661/pulumi_civo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/pulumi_civo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 05:28:18.680394 pulumi_civo-2.4.0a1686633661/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-13 05:28:18.000000 pulumi_civo-2.4.0a1686633661/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 23:13:21.893622 pulumi_civo-2.4.0a1686784153/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-14 23:13:21.893622 pulumi_civo-2.4.0a1686784153/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 23:13:21.889622 pulumi_civo-2.4.0a1686784153/pulumi_civo/
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39031 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 23:13:21.889622 pulumi_civo-2.4.0a1686784153/pulumi_civo/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20882 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/dns_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/dns_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22605 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24236 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/firewall_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/get_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/get_database_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/get_disk_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/get_dns_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/get_dns_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/get_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/get_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/get_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/get_kubernetes_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/get_kubernetes_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/get_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/get_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/get_object_store_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/get_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/get_reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/get_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/get_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/get_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47045 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/instance_reserved_ip_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42980 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/kubernetes_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22159 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/kubernetes_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/object_store_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46709 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo/volume_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 23:13:21.889622 pulumi_civo-2.4.0a1686784153/pulumi_civo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/pulumi_civo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 23:13:21.893622 pulumi_civo-2.4.0a1686784153/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-14 23:13:21.000000 pulumi_civo-2.4.0a1686784153/setup.py
```

### Comparing `pulumi_civo-2.4.0a1686633661/PKG-INFO` & `pulumi_civo-2.4.0a1686784153/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_civo
-Version: 2.4.0a1686633661
+Version: 2.4.0a1686784153
 Summary: A Pulumi package for creating and managing Civo cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-civo
 Keywords: pulumi civo
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_civo-2.4.0a1686633661/README.md` & `pulumi_civo-2.4.0a1686784153/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/__init__.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 # Export this package's modules as members:
 from .database import *
 from .dns_domain_name import *
 from .dns_domain_record import *
 from .firewall import *
 from .firewall_rule import *
 from .get_database import *
+from .get_database_version import *
 from .get_disk_image import *
 from .get_dns_domain_name import *
 from .get_dns_domain_record import *
 from .get_firewall import *
 from .get_instance import *
 from .get_instances import *
-from .get_instances_size import *
 from .get_kubernetes_cluster import *
 from .get_kubernetes_version import *
 from .get_load_balancer import *
 from .get_network import *
 from .get_object_store import *
 from .get_object_store_credential import *
 from .get_region import *
```

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/_inputs.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 from . import _utilities
 
 __all__ = [
     'FirewallEgressRuleArgs',
     'FirewallIngressRuleArgs',
     'KubernetesClusterInstalledApplicationArgs',
     'KubernetesClusterPoolsArgs',
+    'GetDatabaseVersionFilterArgs',
+    'GetDatabaseVersionSortArgs',
     'GetDiskImageFilterArgs',
     'GetDiskImageSortArgs',
     'GetInstancesFilterArgs',
-    'GetInstancesSizeFilterArgs',
-    'GetInstancesSizeSortArgs',
     'GetInstancesSortArgs',
     'GetKubernetesVersionFilterArgs',
     'GetKubernetesVersionSortArgs',
     'GetRegionFilterArgs',
     'GetRegionSortArgs',
     'GetSizeFilterArgs',
     'GetSizeSortArgs',
@@ -349,50 +349,50 @@
 
     @label.setter
     def label(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "label", value)
 
 
 @pulumi.input_type
-class GetDiskImageFilterArgs:
+class GetDatabaseVersionFilterArgs:
     def __init__(__self__, *,
                  key: str,
                  values: Sequence[str],
                  all: Optional[bool] = None,
                  match_by: Optional[str] = None):
         """
-        :param str key: Filter diskimages by this key. This may be one of `id`, `label`, `name`, `version`.
-        :param Sequence[str] values: Only retrieves `diskimages` which keys has value that matches one of the values provided here
+        :param str key: Filter versions by this key. This may be one of `default`, `engine`, `version`.
+        :param Sequence[str] values: Only retrieves `versions` which keys has value that matches one of the values provided here
         :param bool all: Set to `true` to require that a field match all of the `values` instead of just one or more of them. This is useful when matching against multi-valued fields such as lists or sets where you want to ensure that all of the `values` are present in the list or set.
         :param str match_by: One of `exact` (default), `re`, or `substring`. For string-typed fields, specify `re` to match by using the `values` as regular expressions, or specify `substring` to match by treating the `values` as substrings to find within the string field.
         """
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "values", values)
         if all is not None:
             pulumi.set(__self__, "all", all)
         if match_by is not None:
             pulumi.set(__self__, "match_by", match_by)
 
     @property
     @pulumi.getter
     def key(self) -> str:
         """
-        Filter diskimages by this key. This may be one of `id`, `label`, `name`, `version`.
+        Filter versions by this key. This may be one of `default`, `engine`, `version`.
         """
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: str):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def values(self) -> Sequence[str]:
         """
-        Only retrieves `diskimages` which keys has value that matches one of the values provided here
+        Only retrieves `versions` which keys has value that matches one of the values provided here
         """
         return pulumi.get(self, "values")
 
     @values.setter
     def values(self, value: Sequence[str]):
         pulumi.set(self, "values", value)
 
@@ -418,31 +418,31 @@
 
     @match_by.setter
     def match_by(self, value: Optional[str]):
         pulumi.set(self, "match_by", value)
 
 
 @pulumi.input_type
-class GetDiskImageSortArgs:
+class GetDatabaseVersionSortArgs:
     def __init__(__self__, *,
                  key: str,
                  direction: Optional[str] = None):
         """
-        :param str key: Sort diskimages by this key. This may be one of `id`, `label`, `name`, `version`.
+        :param str key: Sort versions by this key. This may be one of `default`, `engine`, `version`.
         :param str direction: The sort direction. This may be either `asc` or `desc`.
         """
         pulumi.set(__self__, "key", key)
         if direction is not None:
             pulumi.set(__self__, "direction", direction)
 
     @property
     @pulumi.getter
     def key(self) -> str:
         """
-        Sort diskimages by this key. This may be one of `id`, `label`, `name`, `version`.
+        Sort versions by this key. This may be one of `default`, `engine`, `version`.
         """
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: str):
         pulumi.set(self, "key", value)
 
@@ -456,50 +456,50 @@
 
     @direction.setter
     def direction(self, value: Optional[str]):
         pulumi.set(self, "direction", value)
 
 
 @pulumi.input_type
-class GetInstancesFilterArgs:
+class GetDiskImageFilterArgs:
     def __init__(__self__, *,
                  key: str,
                  values: Sequence[str],
                  all: Optional[bool] = None,
                  match_by: Optional[str] = None):
         """
-        :param str key: Filter instances by this key. This may be one of `cpu_cores`, `created_at`, `disk_gb`, `firewall_id`, `hostname`, `id`, `initial_password`, `initial_user`, `network_id`, `notes`, `private_ip`, `pseudo_ip`, `public_ip`, `ram_mb`, `region`, `reverse_dns`, `script`, `size`, `sshkey_id`, `status`, `tags`, `template`.
-        :param Sequence[str] values: Only retrieves `instances` which keys has value that matches one of the values provided here
+        :param str key: Filter diskimages by this key. This may be one of `id`, `label`, `name`, `version`.
+        :param Sequence[str] values: Only retrieves `diskimages` which keys has value that matches one of the values provided here
         :param bool all: Set to `true` to require that a field match all of the `values` instead of just one or more of them. This is useful when matching against multi-valued fields such as lists or sets where you want to ensure that all of the `values` are present in the list or set.
         :param str match_by: One of `exact` (default), `re`, or `substring`. For string-typed fields, specify `re` to match by using the `values` as regular expressions, or specify `substring` to match by treating the `values` as substrings to find within the string field.
         """
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "values", values)
         if all is not None:
             pulumi.set(__self__, "all", all)
         if match_by is not None:
             pulumi.set(__self__, "match_by", match_by)
 
     @property
     @pulumi.getter
     def key(self) -> str:
         """
-        Filter instances by this key. This may be one of `cpu_cores`, `created_at`, `disk_gb`, `firewall_id`, `hostname`, `id`, `initial_password`, `initial_user`, `network_id`, `notes`, `private_ip`, `pseudo_ip`, `public_ip`, `ram_mb`, `region`, `reverse_dns`, `script`, `size`, `sshkey_id`, `status`, `tags`, `template`.
+        Filter diskimages by this key. This may be one of `id`, `label`, `name`, `version`.
         """
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: str):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def values(self) -> Sequence[str]:
         """
-        Only retrieves `instances` which keys has value that matches one of the values provided here
+        Only retrieves `diskimages` which keys has value that matches one of the values provided here
         """
         return pulumi.get(self, "values")
 
     @values.setter
     def values(self, value: Sequence[str]):
         pulumi.set(self, "values", value)
 
@@ -525,50 +525,88 @@
 
     @match_by.setter
     def match_by(self, value: Optional[str]):
         pulumi.set(self, "match_by", value)
 
 
 @pulumi.input_type
-class GetInstancesSizeFilterArgs:
+class GetDiskImageSortArgs:
+    def __init__(__self__, *,
+                 key: str,
+                 direction: Optional[str] = None):
+        """
+        :param str key: Sort diskimages by this key. This may be one of `id`, `label`, `name`, `version`.
+        :param str direction: The sort direction. This may be either `asc` or `desc`.
+        """
+        pulumi.set(__self__, "key", key)
+        if direction is not None:
+            pulumi.set(__self__, "direction", direction)
+
+    @property
+    @pulumi.getter
+    def key(self) -> str:
+        """
+        Sort diskimages by this key. This may be one of `id`, `label`, `name`, `version`.
+        """
+        return pulumi.get(self, "key")
+
+    @key.setter
+    def key(self, value: str):
+        pulumi.set(self, "key", value)
+
+    @property
+    @pulumi.getter
+    def direction(self) -> Optional[str]:
+        """
+        The sort direction. This may be either `asc` or `desc`.
+        """
+        return pulumi.get(self, "direction")
+
+    @direction.setter
+    def direction(self, value: Optional[str]):
+        pulumi.set(self, "direction", value)
+
+
+@pulumi.input_type
+class GetInstancesFilterArgs:
     def __init__(__self__, *,
                  key: str,
                  values: Sequence[str],
                  all: Optional[bool] = None,
                  match_by: Optional[str] = None):
         """
-        :param str key: Filter sizes by this key. This may be one of `cpu`, `description`, `disk`, `name`, `ram`, `selectable`, `type`.
-        :param Sequence[str] values: Only retrieves `sizes` which keys has value that matches one of the values provided here
+        :param str key: Filter instances by this key. This may be one of `cpu_cores`, `created_at`, `disk_gb`, `firewall_id`, `hostname`, `id`, `initial_password`, `initial_user`, `network_id`, `notes`, `private_ip`, `pseudo_ip`, `public_ip`, `ram_mb`, `region`, `reverse_dns`, `script`, `size`, `sshkey_id`, `status`, `tags`, `template`.
+        :param Sequence[str] values: Only retrieves `instances` which keys has value that matches one of the values provided here
         :param bool all: Set to `true` to require that a field match all of the `values` instead of just one or more of them. This is useful when matching against multi-valued fields such as lists or sets where you want to ensure that all of the `values` are present in the list or set.
         :param str match_by: One of `exact` (default), `re`, or `substring`. For string-typed fields, specify `re` to match by using the `values` as regular expressions, or specify `substring` to match by treating the `values` as substrings to find within the string field.
         """
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "values", values)
         if all is not None:
             pulumi.set(__self__, "all", all)
         if match_by is not None:
             pulumi.set(__self__, "match_by", match_by)
 
     @property
     @pulumi.getter
     def key(self) -> str:
         """
-        Filter sizes by this key. This may be one of `cpu`, `description`, `disk`, `name`, `ram`, `selectable`, `type`.
+        Filter instances by this key. This may be one of `cpu_cores`, `created_at`, `disk_gb`, `firewall_id`, `hostname`, `id`, `initial_password`, `initial_user`, `network_id`, `notes`, `private_ip`, `pseudo_ip`, `public_ip`, `ram_mb`, `region`, `reverse_dns`, `script`, `size`, `sshkey_id`, `status`, `tags`, `template`.
         """
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: str):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def values(self) -> Sequence[str]:
         """
-        Only retrieves `sizes` which keys has value that matches one of the values provided here
+        Only retrieves `instances` which keys has value that matches one of the values provided here
         """
         return pulumi.get(self, "values")
 
     @values.setter
     def values(self, value: Sequence[str]):
         pulumi.set(self, "values", value)
 
@@ -594,52 +632,14 @@
 
     @match_by.setter
     def match_by(self, value: Optional[str]):
         pulumi.set(self, "match_by", value)
 
 
 @pulumi.input_type
-class GetInstancesSizeSortArgs:
-    def __init__(__self__, *,
-                 key: str,
-                 direction: Optional[str] = None):
-        """
-        :param str key: Sort sizes by this key. This may be one of `cpu`, `description`, `disk`, `name`, `ram`, `selectable`, `type`.
-        :param str direction: The sort direction. This may be either `asc` or `desc`.
-        """
-        pulumi.set(__self__, "key", key)
-        if direction is not None:
-            pulumi.set(__self__, "direction", direction)
-
-    @property
-    @pulumi.getter
-    def key(self) -> str:
-        """
-        Sort sizes by this key. This may be one of `cpu`, `description`, `disk`, `name`, `ram`, `selectable`, `type`.
-        """
-        return pulumi.get(self, "key")
-
-    @key.setter
-    def key(self, value: str):
-        pulumi.set(self, "key", value)
-
-    @property
-    @pulumi.getter
-    def direction(self) -> Optional[str]:
-        """
-        The sort direction. This may be either `asc` or `desc`.
-        """
-        return pulumi.get(self, "direction")
-
-    @direction.setter
-    def direction(self, value: Optional[str]):
-        pulumi.set(self, "direction", value)
-
-
-@pulumi.input_type
 class GetInstancesSortArgs:
     def __init__(__self__, *,
                  key: str,
                  direction: Optional[str] = None):
         """
         :param str key: Sort instances by this key. This may be one of `cpu_cores`, `created_at`, `disk_gb`, `firewall_id`, `hostname`, `id`, `initial_password`, `initial_user`, `network_id`, `notes`, `private_ip`, `pseudo_ip`, `public_ip`, `ram_mb`, `region`, `reverse_dns`, `script`, `size`, `sshkey_id`, `status`, `template`.
         :param str direction: The sort direction. This may be either `asc` or `desc`.
```

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/_utilities.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/config/vars.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/database.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/database.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,42 +10,60 @@
 from . import _utilities
 
 __all__ = ['DatabaseArgs', 'Database']
 
 @pulumi.input_type
 class DatabaseArgs:
     def __init__(__self__, *,
+                 engine: pulumi.Input[str],
                  nodes: pulumi.Input[int],
                  size: pulumi.Input[str],
+                 version: pulumi.Input[str],
                  firewall_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  network_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Database resource.
+        :param pulumi.Input[str] engine: The engine of the database
         :param pulumi.Input[int] nodes: Count of nodes
         :param pulumi.Input[str] size: Size of the database
+        :param pulumi.Input[str] version: The version of the database
         :param pulumi.Input[str] firewall_id: The ID of the firewall to use, from the current list. If left blank or not sent, the default firewall will be used (open to all)
         :param pulumi.Input[str] name: Name of the database
         :param pulumi.Input[str] network_id: The id of the associated network
         :param pulumi.Input[str] region: The region where the database will be created.
         """
+        pulumi.set(__self__, "engine", engine)
         pulumi.set(__self__, "nodes", nodes)
         pulumi.set(__self__, "size", size)
+        pulumi.set(__self__, "version", version)
         if firewall_id is not None:
             pulumi.set(__self__, "firewall_id", firewall_id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if network_id is not None:
             pulumi.set(__self__, "network_id", network_id)
         if region is not None:
             pulumi.set(__self__, "region", region)
 
     @property
     @pulumi.getter
+    def engine(self) -> pulumi.Input[str]:
+        """
+        The engine of the database
+        """
+        return pulumi.get(self, "engine")
+
+    @engine.setter
+    def engine(self, value: pulumi.Input[str]):
+        pulumi.set(self, "engine", value)
+
+    @property
+    @pulumi.getter
     def nodes(self) -> pulumi.Input[int]:
         """
         Count of nodes
         """
         return pulumi.get(self, "nodes")
 
     @nodes.setter
@@ -61,14 +79,26 @@
         return pulumi.get(self, "size")
 
     @size.setter
     def size(self, value: pulumi.Input[str]):
         pulumi.set(self, "size", value)
 
     @property
+    @pulumi.getter
+    def version(self) -> pulumi.Input[str]:
+        """
+        The version of the database
+        """
+        return pulumi.get(self, "version")
+
+    @version.setter
+    def version(self, value: pulumi.Input[str]):
+        pulumi.set(self, "version", value)
+
+    @property
     @pulumi.getter(name="firewallId")
     def firewall_id(self) -> Optional[pulumi.Input[str]]:
         """
         The ID of the firewall to use, from the current list. If left blank or not sent, the default firewall will be used (open to all)
         """
         return pulumi.get(self, "firewall_id")
 
@@ -112,35 +142,41 @@
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
 
 @pulumi.input_type
 class _DatabaseState:
     def __init__(__self__, *,
+                 engine: Optional[pulumi.Input[str]] = None,
                  firewall_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  network_id: Optional[pulumi.Input[str]] = None,
                  nodes: Optional[pulumi.Input[int]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None,
-                 username: Optional[pulumi.Input[str]] = None):
+                 username: Optional[pulumi.Input[str]] = None,
+                 version: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Database resources.
+        :param pulumi.Input[str] engine: The engine of the database
         :param pulumi.Input[str] firewall_id: The ID of the firewall to use, from the current list. If left blank or not sent, the default firewall will be used (open to all)
         :param pulumi.Input[str] name: Name of the database
         :param pulumi.Input[str] network_id: The id of the associated network
         :param pulumi.Input[int] nodes: Count of nodes
         :param pulumi.Input[str] password: The password of the database
         :param pulumi.Input[str] region: The region where the database will be created.
         :param pulumi.Input[str] size: Size of the database
         :param pulumi.Input[str] status: The status of the database
         :param pulumi.Input[str] username: The username of the database
+        :param pulumi.Input[str] version: The version of the database
         """
+        if engine is not None:
+            pulumi.set(__self__, "engine", engine)
         if firewall_id is not None:
             pulumi.set(__self__, "firewall_id", firewall_id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if network_id is not None:
             pulumi.set(__self__, "network_id", network_id)
         if nodes is not None:
@@ -151,14 +187,28 @@
             pulumi.set(__self__, "region", region)
         if size is not None:
             pulumi.set(__self__, "size", size)
         if status is not None:
             pulumi.set(__self__, "status", status)
         if username is not None:
             pulumi.set(__self__, "username", username)
+        if version is not None:
+            pulumi.set(__self__, "version", version)
+
+    @property
+    @pulumi.getter
+    def engine(self) -> Optional[pulumi.Input[str]]:
+        """
+        The engine of the database
+        """
+        return pulumi.get(self, "engine")
+
+    @engine.setter
+    def engine(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "engine", value)
 
     @property
     @pulumi.getter(name="firewallId")
     def firewall_id(self) -> Optional[pulumi.Input[str]]:
         """
         The ID of the firewall to use, from the current list. If left blank or not sent, the default firewall will be used (open to all)
         """
@@ -260,44 +310,60 @@
         """
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username", value)
 
+    @property
+    @pulumi.getter
+    def version(self) -> Optional[pulumi.Input[str]]:
+        """
+        The version of the database
+        """
+        return pulumi.get(self, "version")
+
+    @version.setter
+    def version(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "version", value)
+
 
 class Database(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 engine: Optional[pulumi.Input[str]] = None,
                  firewall_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  network_id: Optional[pulumi.Input[str]] = None,
                  nodes: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None,
+                 version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Import
 
         using ID
 
         ```sh
          $ pulumi import civo:index/database:Database mydb 29fcd1c4-fb61-44c7-b49c-dc7b98e9927e
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] engine: The engine of the database
         :param pulumi.Input[str] firewall_id: The ID of the firewall to use, from the current list. If left blank or not sent, the default firewall will be used (open to all)
         :param pulumi.Input[str] name: Name of the database
         :param pulumi.Input[str] network_id: The id of the associated network
         :param pulumi.Input[int] nodes: Count of nodes
         :param pulumi.Input[str] region: The region where the database will be created.
         :param pulumi.Input[str] size: Size of the database
+        :param pulumi.Input[str] version: The version of the database
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: DatabaseArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -321,94 +387,116 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 engine: Optional[pulumi.Input[str]] = None,
                  firewall_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  network_id: Optional[pulumi.Input[str]] = None,
                  nodes: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None,
+                 version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DatabaseArgs.__new__(DatabaseArgs)
 
+            if engine is None and not opts.urn:
+                raise TypeError("Missing required property 'engine'")
+            __props__.__dict__["engine"] = engine
             __props__.__dict__["firewall_id"] = firewall_id
             __props__.__dict__["name"] = name
             __props__.__dict__["network_id"] = network_id
             if nodes is None and not opts.urn:
                 raise TypeError("Missing required property 'nodes'")
             __props__.__dict__["nodes"] = nodes
             __props__.__dict__["region"] = region
             if size is None and not opts.urn:
                 raise TypeError("Missing required property 'size'")
             __props__.__dict__["size"] = size
+            if version is None and not opts.urn:
+                raise TypeError("Missing required property 'version'")
+            __props__.__dict__["version"] = version
             __props__.__dict__["password"] = None
             __props__.__dict__["status"] = None
             __props__.__dict__["username"] = None
         super(Database, __self__).__init__(
             'civo:index/database:Database',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            engine: Optional[pulumi.Input[str]] = None,
             firewall_id: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             network_id: Optional[pulumi.Input[str]] = None,
             nodes: Optional[pulumi.Input[int]] = None,
             password: Optional[pulumi.Input[str]] = None,
             region: Optional[pulumi.Input[str]] = None,
             size: Optional[pulumi.Input[str]] = None,
             status: Optional[pulumi.Input[str]] = None,
-            username: Optional[pulumi.Input[str]] = None) -> 'Database':
+            username: Optional[pulumi.Input[str]] = None,
+            version: Optional[pulumi.Input[str]] = None) -> 'Database':
         """
         Get an existing Database resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] engine: The engine of the database
         :param pulumi.Input[str] firewall_id: The ID of the firewall to use, from the current list. If left blank or not sent, the default firewall will be used (open to all)
         :param pulumi.Input[str] name: Name of the database
         :param pulumi.Input[str] network_id: The id of the associated network
         :param pulumi.Input[int] nodes: Count of nodes
         :param pulumi.Input[str] password: The password of the database
         :param pulumi.Input[str] region: The region where the database will be created.
         :param pulumi.Input[str] size: Size of the database
         :param pulumi.Input[str] status: The status of the database
         :param pulumi.Input[str] username: The username of the database
+        :param pulumi.Input[str] version: The version of the database
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _DatabaseState.__new__(_DatabaseState)
 
+        __props__.__dict__["engine"] = engine
         __props__.__dict__["firewall_id"] = firewall_id
         __props__.__dict__["name"] = name
         __props__.__dict__["network_id"] = network_id
         __props__.__dict__["nodes"] = nodes
         __props__.__dict__["password"] = password
         __props__.__dict__["region"] = region
         __props__.__dict__["size"] = size
         __props__.__dict__["status"] = status
         __props__.__dict__["username"] = username
+        __props__.__dict__["version"] = version
         return Database(resource_name, opts=opts, __props__=__props__)
 
     @property
+    @pulumi.getter
+    def engine(self) -> pulumi.Output[str]:
+        """
+        The engine of the database
+        """
+        return pulumi.get(self, "engine")
+
+    @property
     @pulumi.getter(name="firewallId")
     def firewall_id(self) -> pulumi.Output[str]:
         """
         The ID of the firewall to use, from the current list. If left blank or not sent, the default firewall will be used (open to all)
         """
         return pulumi.get(self, "firewall_id")
 
@@ -472,7 +560,15 @@
     @pulumi.getter
     def username(self) -> pulumi.Output[str]:
         """
         The username of the database
         """
         return pulumi.get(self, "username")
 
+    @property
+    @pulumi.getter
+    def version(self) -> pulumi.Output[str]:
+        """
+        The version of the database
+        """
+        return pulumi.get(self, "version")
+
```

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/dns_domain_name.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/dns_domain_name.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/dns_domain_record.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/dns_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/firewall.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/firewall_rule.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/firewall_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/get_database.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/get_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 ]
 
 @pulumi.output_type
 class GetDatabaseResult:
     """
     A collection of values returned by getDatabase.
     """
-    def __init__(__self__, firewall_id=None, id=None, name=None, network_id=None, nodes=None, password=None, region=None, size=None, status=None, username=None):
+    def __init__(__self__, engine=None, firewall_id=None, id=None, name=None, network_id=None, nodes=None, password=None, region=None, size=None, status=None, username=None, version=None):
+        if engine and not isinstance(engine, str):
+            raise TypeError("Expected argument 'engine' to be a str")
+        pulumi.set(__self__, "engine", engine)
         if firewall_id and not isinstance(firewall_id, str):
             raise TypeError("Expected argument 'firewall_id' to be a str")
         pulumi.set(__self__, "firewall_id", firewall_id)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if name and not isinstance(name, str):
@@ -48,14 +51,25 @@
         pulumi.set(__self__, "size", size)
         if status and not isinstance(status, str):
             raise TypeError("Expected argument 'status' to be a str")
         pulumi.set(__self__, "status", status)
         if username and not isinstance(username, str):
             raise TypeError("Expected argument 'username' to be a str")
         pulumi.set(__self__, "username", username)
+        if version and not isinstance(version, str):
+            raise TypeError("Expected argument 'version' to be a str")
+        pulumi.set(__self__, "version", version)
+
+    @property
+    @pulumi.getter
+    def engine(self) -> str:
+        """
+        The engine of the database
+        """
+        return pulumi.get(self, "engine")
 
     @property
     @pulumi.getter(name="firewallId")
     def firewall_id(self) -> str:
         """
         The firewall id of the Database
         """
@@ -129,31 +143,41 @@
     @pulumi.getter
     def username(self) -> str:
         """
         The username of the database
         """
         return pulumi.get(self, "username")
 
+    @property
+    @pulumi.getter
+    def version(self) -> str:
+        """
+        The version of the database
+        """
+        return pulumi.get(self, "version")
+
 
 class AwaitableGetDatabaseResult(GetDatabaseResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetDatabaseResult(
+            engine=self.engine,
             firewall_id=self.firewall_id,
             id=self.id,
             name=self.name,
             network_id=self.network_id,
             nodes=self.nodes,
             password=self.password,
             region=self.region,
             size=self.size,
             status=self.status,
-            username=self.username)
+            username=self.username,
+            version=self.version)
 
 
 def get_database(id: Optional[str] = None,
                  name: Optional[str] = None,
                  region: Optional[str] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatabaseResult:
     """
@@ -180,24 +204,26 @@
     __args__['id'] = id
     __args__['name'] = name
     __args__['region'] = region
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('civo:index/getDatabase:getDatabase', __args__, opts=opts, typ=GetDatabaseResult).value
 
     return AwaitableGetDatabaseResult(
+        engine=__ret__.engine,
         firewall_id=__ret__.firewall_id,
         id=__ret__.id,
         name=__ret__.name,
         network_id=__ret__.network_id,
         nodes=__ret__.nodes,
         password=__ret__.password,
         region=__ret__.region,
         size=__ret__.size,
         status=__ret__.status,
-        username=__ret__.username)
+        username=__ret__.username,
+        version=__ret__.version)
 
 
 @_utilities.lift_output_func(get_database)
 def get_database_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                         name: Optional[pulumi.Input[Optional[str]]] = None,
                         region: Optional[pulumi.Input[Optional[str]]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatabaseResult]:
```

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/get_disk_image.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/get_disk_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/get_dns_domain_name.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/get_dns_domain_name.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/get_dns_domain_record.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/get_dns_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/get_firewall.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/get_firewall.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                  region: Optional[str] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetFirewallResult:
     """
     Retrieve information about a firewall for use in other resources.
 
     This data source provides all of the firewall's properties as configured on your Civo account.
 
-    Firewalls may be looked up by id or name, and you can optionally pass region if you want to make a lookup for an expecific firewall inside that region.
+    Firewalls may be looked up by id or name, and you can optionally pass region if you want to make a lookup for a specific firewall inside that region.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_civo as civo
 
@@ -126,15 +126,15 @@
                         region: Optional[pulumi.Input[Optional[str]]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetFirewallResult]:
     """
     Retrieve information about a firewall for use in other resources.
 
     This data source provides all of the firewall's properties as configured on your Civo account.
 
-    Firewalls may be looked up by id or name, and you can optionally pass region if you want to make a lookup for an expecific firewall inside that region.
+    Firewalls may be looked up by id or name, and you can optionally pass region if you want to make a lookup for a specific firewall inside that region.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_civo as civo
```

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/get_instance.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/get_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             raise TypeError("Expected argument 'template' to be a str")
         pulumi.set(__self__, "template", template)
 
     @property
     @pulumi.getter(name="cpuCores")
     def cpu_cores(self) -> int:
         """
-        Total cpu of the inatance
+        Total cpu of the instance
         """
         return pulumi.get(self, "cpu_cores")
 
     @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> str:
         """
```

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/get_instances.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/get_instances.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/get_instances_size.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/get_size.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
 
 __all__ = [
-    'GetInstancesSizeResult',
-    'AwaitableGetInstancesSizeResult',
-    'get_instances_size',
-    'get_instances_size_output',
+    'GetSizeResult',
+    'AwaitableGetSizeResult',
+    'get_size',
+    'get_size_output',
 ]
 
 @pulumi.output_type
-class GetInstancesSizeResult:
+class GetSizeResult:
     """
-    A collection of values returned by getInstancesSize.
+    A collection of values returned by getSize.
     """
     def __init__(__self__, filters=None, id=None, sizes=None, sorts=None):
         if filters and not isinstance(filters, list):
             raise TypeError("Expected argument 'filters' to be a list")
         pulumi.set(__self__, "filters", filters)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
@@ -35,15 +35,15 @@
         pulumi.set(__self__, "sizes", sizes)
         if sorts and not isinstance(sorts, list):
             raise TypeError("Expected argument 'sorts' to be a list")
         pulumi.set(__self__, "sorts", sorts)
 
     @property
     @pulumi.getter
-    def filters(self) -> Optional[Sequence['outputs.GetInstancesSizeFilterResult']]:
+    def filters(self) -> Optional[Sequence['outputs.GetSizeFilterResult']]:
         """
         One or more key/value pairs on which to filter results
         """
         return pulumi.get(self, "filters")
 
     @property
     @pulumi.getter
@@ -51,66 +51,66 @@
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def sizes(self) -> Sequence['outputs.GetInstancesSizeSizeResult']:
+    def sizes(self) -> Sequence['outputs.GetSizeSizeResult']:
         return pulumi.get(self, "sizes")
 
     @property
     @pulumi.getter
-    def sorts(self) -> Optional[Sequence['outputs.GetInstancesSizeSortResult']]:
+    def sorts(self) -> Optional[Sequence['outputs.GetSizeSortResult']]:
         """
         One or more key/direction pairs on which to sort results
         """
         return pulumi.get(self, "sorts")
 
 
-class AwaitableGetInstancesSizeResult(GetInstancesSizeResult):
+class AwaitableGetSizeResult(GetSizeResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetInstancesSizeResult(
+        return GetSizeResult(
             filters=self.filters,
             id=self.id,
             sizes=self.sizes,
             sorts=self.sorts)
 
 
-def get_instances_size(filters: Optional[Sequence[pulumi.InputType['GetInstancesSizeFilterArgs']]] = None,
-                       sorts: Optional[Sequence[pulumi.InputType['GetInstancesSizeSortArgs']]] = None,
-                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInstancesSizeResult:
+def get_size(filters: Optional[Sequence[pulumi.InputType['GetSizeFilterArgs']]] = None,
+             sorts: Optional[Sequence[pulumi.InputType['GetSizeSortArgs']]] = None,
+             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSizeResult:
     """
-    Retrieves information about the instance sizes that Civo supports, with the ability to filter the results.
+    Retrieves information about the sizes that Civo supports, with the ability to filter the results.
 
 
-    :param Sequence[pulumi.InputType['GetInstancesSizeFilterArgs']] filters: One or more key/value pairs on which to filter results
-    :param Sequence[pulumi.InputType['GetInstancesSizeSortArgs']] sorts: One or more key/direction pairs on which to sort results
+    :param Sequence[pulumi.InputType['GetSizeFilterArgs']] filters: One or more key/value pairs on which to filter results
+    :param Sequence[pulumi.InputType['GetSizeSortArgs']] sorts: One or more key/direction pairs on which to sort results
     """
     __args__ = dict()
     __args__['filters'] = filters
     __args__['sorts'] = sorts
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('civo:index/getInstancesSize:getInstancesSize', __args__, opts=opts, typ=GetInstancesSizeResult).value
+    __ret__ = pulumi.runtime.invoke('civo:index/getSize:getSize', __args__, opts=opts, typ=GetSizeResult).value
 
-    return AwaitableGetInstancesSizeResult(
+    return AwaitableGetSizeResult(
         filters=__ret__.filters,
         id=__ret__.id,
         sizes=__ret__.sizes,
         sorts=__ret__.sorts)
 
 
-@_utilities.lift_output_func(get_instances_size)
-def get_instances_size_output(filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetInstancesSizeFilterArgs']]]]] = None,
-                              sorts: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetInstancesSizeSortArgs']]]]] = None,
-                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInstancesSizeResult]:
+@_utilities.lift_output_func(get_size)
+def get_size_output(filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetSizeFilterArgs']]]]] = None,
+                    sorts: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetSizeSortArgs']]]]] = None,
+                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSizeResult]:
     """
-    Retrieves information about the instance sizes that Civo supports, with the ability to filter the results.
+    Retrieves information about the sizes that Civo supports, with the ability to filter the results.
 
 
-    :param Sequence[pulumi.InputType['GetInstancesSizeFilterArgs']] filters: One or more key/value pairs on which to filter results
-    :param Sequence[pulumi.InputType['GetInstancesSizeSortArgs']] sorts: One or more key/direction pairs on which to sort results
+    :param Sequence[pulumi.InputType['GetSizeFilterArgs']] filters: One or more key/value pairs on which to filter results
+    :param Sequence[pulumi.InputType['GetSizeSortArgs']] sorts: One or more key/direction pairs on which to sort results
     """
     ...
```

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/get_kubernetes_cluster.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/get_kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/get_kubernetes_version.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/get_kubernetes_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/get_load_balancer.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/get_load_balancer.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         """
         return pulumi.get(self, "public_ip")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
         """
-        The region of the load balancer, if you delcare this field, the datasource will use this value instead of the one defined in the provider
+        The region of the load balancer, if you declare this field, the datasource will use this value instead of the one defined in the provider
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="sessionAffinity")
     def session_affinity(self) -> str:
         """
@@ -217,15 +217,15 @@
         region="LON1")
     pulumi.export("civoLoadbalancerOutput", my_lb.public_ip)
     ```
 
 
     :param str id: The id of the load balancer to retrieve (You can find this id from service annotations 'kubernetes.civo.com/loadbalancer-id')
     :param str name: The name of the load balancer (You can find this name from service annotations 'kubernetes.civo.com/loadbalancer-name')
-    :param str region: The region of the load balancer, if you delcare this field, the datasource will use this value instead of the one defined in the provider
+    :param str region: The region of the load balancer, if you declare this field, the datasource will use this value instead of the one defined in the provider
     """
     __args__ = dict()
     __args__['id'] = id
     __args__['name'] = name
     __args__['region'] = region
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('civo:index/getLoadBalancer:getLoadBalancer', __args__, opts=opts, typ=GetLoadBalancerResult).value
@@ -267,10 +267,10 @@
         region="LON1")
     pulumi.export("civoLoadbalancerOutput", my_lb.public_ip)
     ```
 
 
     :param str id: The id of the load balancer to retrieve (You can find this id from service annotations 'kubernetes.civo.com/loadbalancer-id')
     :param str name: The name of the load balancer (You can find this name from service annotations 'kubernetes.civo.com/loadbalancer-name')
-    :param str region: The region of the load balancer, if you delcare this field, the datasource will use this value instead of the one defined in the provider
+    :param str region: The region of the load balancer, if you declare this field, the datasource will use this value instead of the one defined in the provider
     """
     ...
```

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/get_network.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/get_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                 region: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetNetworkResult:
     """
     Retrieve information about a network for use in other resources.
 
     This data source provides all of the network's properties as configured on your Civo account.
 
-    Networks may be looked up by id or label, and you can optionally pass region if you want to make a lookup for an expecific network inside that region.
+    Networks may be looked up by id or label, and you can optionally pass region if you want to make a lookup for a specific network inside that region.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_civo as civo
 
@@ -139,15 +139,15 @@
                        region: Optional[pulumi.Input[Optional[str]]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNetworkResult]:
     """
     Retrieve information about a network for use in other resources.
 
     This data source provides all of the network's properties as configured on your Civo account.
 
-    Networks may be looked up by id or label, and you can optionally pass region if you want to make a lookup for an expecific network inside that region.
+    Networks may be looked up by id or label, and you can optionally pass region if you want to make a lookup for a specific network inside that region.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_civo as civo
```

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/get_object_store.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/get_object_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/get_object_store_credential.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/get_object_store_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/get_region.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/get_region.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/get_reserved_ip.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/get_reserved_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/get_size.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/get_database_version.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,42 +8,42 @@
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
 
 __all__ = [
-    'GetSizeResult',
-    'AwaitableGetSizeResult',
-    'get_size',
-    'get_size_output',
+    'GetDatabaseVersionResult',
+    'AwaitableGetDatabaseVersionResult',
+    'get_database_version',
+    'get_database_version_output',
 ]
 
 @pulumi.output_type
-class GetSizeResult:
+class GetDatabaseVersionResult:
     """
-    A collection of values returned by getSize.
+    A collection of values returned by getDatabaseVersion.
     """
-    def __init__(__self__, filters=None, id=None, sizes=None, sorts=None):
+    def __init__(__self__, filters=None, id=None, sorts=None, versions=None):
         if filters and not isinstance(filters, list):
             raise TypeError("Expected argument 'filters' to be a list")
         pulumi.set(__self__, "filters", filters)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if sizes and not isinstance(sizes, list):
-            raise TypeError("Expected argument 'sizes' to be a list")
-        pulumi.set(__self__, "sizes", sizes)
         if sorts and not isinstance(sorts, list):
             raise TypeError("Expected argument 'sorts' to be a list")
         pulumi.set(__self__, "sorts", sorts)
+        if versions and not isinstance(versions, list):
+            raise TypeError("Expected argument 'versions' to be a list")
+        pulumi.set(__self__, "versions", versions)
 
     @property
     @pulumi.getter
-    def filters(self) -> Optional[Sequence['outputs.GetSizeFilterResult']]:
+    def filters(self) -> Optional[Sequence['outputs.GetDatabaseVersionFilterResult']]:
         """
         One or more key/value pairs on which to filter results
         """
         return pulumi.get(self, "filters")
 
     @property
     @pulumi.getter
@@ -51,66 +51,66 @@
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def sizes(self) -> Sequence['outputs.GetSizeSizeResult']:
-        return pulumi.get(self, "sizes")
-
-    @property
-    @pulumi.getter
-    def sorts(self) -> Optional[Sequence['outputs.GetSizeSortResult']]:
+    def sorts(self) -> Optional[Sequence['outputs.GetDatabaseVersionSortResult']]:
         """
         One or more key/direction pairs on which to sort results
         """
         return pulumi.get(self, "sorts")
 
+    @property
+    @pulumi.getter
+    def versions(self) -> Sequence['outputs.GetDatabaseVersionVersionResult']:
+        return pulumi.get(self, "versions")
+
 
-class AwaitableGetSizeResult(GetSizeResult):
+class AwaitableGetDatabaseVersionResult(GetDatabaseVersionResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetSizeResult(
+        return GetDatabaseVersionResult(
             filters=self.filters,
             id=self.id,
-            sizes=self.sizes,
-            sorts=self.sorts)
+            sorts=self.sorts,
+            versions=self.versions)
 
 
-def get_size(filters: Optional[Sequence[pulumi.InputType['GetSizeFilterArgs']]] = None,
-             sorts: Optional[Sequence[pulumi.InputType['GetSizeSortArgs']]] = None,
-             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSizeResult:
+def get_database_version(filters: Optional[Sequence[pulumi.InputType['GetDatabaseVersionFilterArgs']]] = None,
+                         sorts: Optional[Sequence[pulumi.InputType['GetDatabaseVersionSortArgs']]] = None,
+                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatabaseVersionResult:
     """
-    Retrieves information about the sizes that Civo supports, with the ability to filter the results.
+    Retrieves information about the database versions that Civo supports, with the ability to filter the results.
 
 
-    :param Sequence[pulumi.InputType['GetSizeFilterArgs']] filters: One or more key/value pairs on which to filter results
-    :param Sequence[pulumi.InputType['GetSizeSortArgs']] sorts: One or more key/direction pairs on which to sort results
+    :param Sequence[pulumi.InputType['GetDatabaseVersionFilterArgs']] filters: One or more key/value pairs on which to filter results
+    :param Sequence[pulumi.InputType['GetDatabaseVersionSortArgs']] sorts: One or more key/direction pairs on which to sort results
     """
     __args__ = dict()
     __args__['filters'] = filters
     __args__['sorts'] = sorts
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('civo:index/getSize:getSize', __args__, opts=opts, typ=GetSizeResult).value
+    __ret__ = pulumi.runtime.invoke('civo:index/getDatabaseVersion:getDatabaseVersion', __args__, opts=opts, typ=GetDatabaseVersionResult).value
 
-    return AwaitableGetSizeResult(
+    return AwaitableGetDatabaseVersionResult(
         filters=__ret__.filters,
         id=__ret__.id,
-        sizes=__ret__.sizes,
-        sorts=__ret__.sorts)
+        sorts=__ret__.sorts,
+        versions=__ret__.versions)
 
 
-@_utilities.lift_output_func(get_size)
-def get_size_output(filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetSizeFilterArgs']]]]] = None,
-                    sorts: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetSizeSortArgs']]]]] = None,
-                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSizeResult]:
+@_utilities.lift_output_func(get_database_version)
+def get_database_version_output(filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetDatabaseVersionFilterArgs']]]]] = None,
+                                sorts: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetDatabaseVersionSortArgs']]]]] = None,
+                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatabaseVersionResult]:
     """
-    Retrieves information about the sizes that Civo supports, with the ability to filter the results.
+    Retrieves information about the database versions that Civo supports, with the ability to filter the results.
 
 
-    :param Sequence[pulumi.InputType['GetSizeFilterArgs']] filters: One or more key/value pairs on which to filter results
-    :param Sequence[pulumi.InputType['GetSizeSortArgs']] sorts: One or more key/direction pairs on which to sort results
+    :param Sequence[pulumi.InputType['GetDatabaseVersionFilterArgs']] filters: One or more key/value pairs on which to filter results
+    :param Sequence[pulumi.InputType['GetDatabaseVersionSortArgs']] sorts: One or more key/direction pairs on which to sort results
     """
     ...
```

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/get_ssh_key.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/get_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/get_volume.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/get_volume.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,15 +115,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_civo as civo
 
-    mysql = civo.get_volume(name="database-mysql")
+    myvolume = civo.get_volume(name="test-volume-name")
+    pulumi.export("volumeOutput", myvolume)
     ```
 
 
     :param str id: The ID of this resource.
     :param str name: The name of the volume
     :param str region: The region where volume is running
     """
@@ -155,15 +156,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_civo as civo
 
-    mysql = civo.get_volume(name="database-mysql")
+    myvolume = civo.get_volume(name="test-volume-name")
+    pulumi.export("volumeOutput", myvolume)
     ```
 
 
     :param str id: The ID of this resource.
     :param str name: The name of the volume
     :param str region: The region where volume is running
     """
```

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/instance.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/instance_reserved_ip_assignment.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/instance_reserved_ip_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/kubernetes_cluster.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/kubernetes_node_pool.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/kubernetes_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/network.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/network.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/object_store.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/object_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/object_store_credential.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/object_store_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/outputs.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 from . import _utilities
 
 __all__ = [
     'FirewallEgressRule',
     'FirewallIngressRule',
     'KubernetesClusterInstalledApplication',
     'KubernetesClusterPools',
+    'GetDatabaseVersionFilterResult',
+    'GetDatabaseVersionSortResult',
+    'GetDatabaseVersionVersionResult',
     'GetDiskImageDiskimageResult',
     'GetDiskImageFilterResult',
     'GetDiskImageSortResult',
     'GetInstancesFilterResult',
     'GetInstancesInstanceResult',
-    'GetInstancesSizeFilterResult',
-    'GetInstancesSizeSizeResult',
-    'GetInstancesSizeSortResult',
     'GetInstancesSortResult',
     'GetKubernetesClusterInstalledApplicationResult',
     'GetKubernetesClusterPoolResult',
     'GetKubernetesVersionFilterResult',
     'GetKubernetesVersionSortResult',
     'GetKubernetesVersionVersionResult',
     'GetLoadBalancerBackendResult',
@@ -331,14 +331,123 @@
         """
         Node pool label, if you don't provide one, we will generate one for you
         """
         return pulumi.get(self, "label")
 
 
 @pulumi.output_type
+class GetDatabaseVersionFilterResult(dict):
+    def __init__(__self__, *,
+                 key: str,
+                 values: Sequence[str],
+                 all: Optional[bool] = None,
+                 match_by: Optional[str] = None):
+        """
+        :param str key: Filter versions by this key. This may be one of `default`, `engine`, `version`.
+        :param Sequence[str] values: Only retrieves `versions` which keys has value that matches one of the values provided here
+        :param bool all: Set to `true` to require that a field match all of the `values` instead of just one or more of them. This is useful when matching against multi-valued fields such as lists or sets where you want to ensure that all of the `values` are present in the list or set.
+        :param str match_by: One of `exact` (default), `re`, or `substring`. For string-typed fields, specify `re` to match by using the `values` as regular expressions, or specify `substring` to match by treating the `values` as substrings to find within the string field.
+        """
+        pulumi.set(__self__, "key", key)
+        pulumi.set(__self__, "values", values)
+        if all is not None:
+            pulumi.set(__self__, "all", all)
+        if match_by is not None:
+            pulumi.set(__self__, "match_by", match_by)
+
+    @property
+    @pulumi.getter
+    def key(self) -> str:
+        """
+        Filter versions by this key. This may be one of `default`, `engine`, `version`.
+        """
+        return pulumi.get(self, "key")
+
+    @property
+    @pulumi.getter
+    def values(self) -> Sequence[str]:
+        """
+        Only retrieves `versions` which keys has value that matches one of the values provided here
+        """
+        return pulumi.get(self, "values")
+
+    @property
+    @pulumi.getter
+    def all(self) -> Optional[bool]:
+        """
+        Set to `true` to require that a field match all of the `values` instead of just one or more of them. This is useful when matching against multi-valued fields such as lists or sets where you want to ensure that all of the `values` are present in the list or set.
+        """
+        return pulumi.get(self, "all")
+
+    @property
+    @pulumi.getter(name="matchBy")
+    def match_by(self) -> Optional[str]:
+        """
+        One of `exact` (default), `re`, or `substring`. For string-typed fields, specify `re` to match by using the `values` as regular expressions, or specify `substring` to match by treating the `values` as substrings to find within the string field.
+        """
+        return pulumi.get(self, "match_by")
+
+
+@pulumi.output_type
+class GetDatabaseVersionSortResult(dict):
+    def __init__(__self__, *,
+                 key: str,
+                 direction: Optional[str] = None):
+        """
+        :param str key: Sort versions by this key. This may be one of `default`, `engine`, `version`.
+        :param str direction: The sort direction. This may be either `asc` or `desc`.
+        """
+        pulumi.set(__self__, "key", key)
+        if direction is not None:
+            pulumi.set(__self__, "direction", direction)
+
+    @property
+    @pulumi.getter
+    def key(self) -> str:
+        """
+        Sort versions by this key. This may be one of `default`, `engine`, `version`.
+        """
+        return pulumi.get(self, "key")
+
+    @property
+    @pulumi.getter
+    def direction(self) -> Optional[str]:
+        """
+        The sort direction. This may be either `asc` or `desc`.
+        """
+        return pulumi.get(self, "direction")
+
+
+@pulumi.output_type
+class GetDatabaseVersionVersionResult(dict):
+    def __init__(__self__, *,
+                 default: bool,
+                 engine: str,
+                 version: str):
+        pulumi.set(__self__, "default", default)
+        pulumi.set(__self__, "engine", engine)
+        pulumi.set(__self__, "version", version)
+
+    @property
+    @pulumi.getter
+    def default(self) -> bool:
+        return pulumi.get(self, "default")
+
+    @property
+    @pulumi.getter
+    def engine(self) -> str:
+        return pulumi.get(self, "engine")
+
+    @property
+    @pulumi.getter
+    def version(self) -> str:
+        return pulumi.get(self, "version")
+
+
+@pulumi.output_type
 class GetDiskImageDiskimageResult(dict):
     def __init__(__self__, *,
                  id: str,
                  label: str,
                  name: str,
                  version: str):
         """
@@ -675,151 +784,14 @@
     @property
     @pulumi.getter
     def template(self) -> str:
         return pulumi.get(self, "template")
 
 
 @pulumi.output_type
-class GetInstancesSizeFilterResult(dict):
-    def __init__(__self__, *,
-                 key: str,
-                 values: Sequence[str],
-                 all: Optional[bool] = None,
-                 match_by: Optional[str] = None):
-        """
-        :param str key: Filter sizes by this key. This may be one of `cpu`, `description`, `disk`, `name`, `ram`, `selectable`, `type`.
-        :param Sequence[str] values: Only retrieves `sizes` which keys has value that matches one of the values provided here
-        :param bool all: Set to `true` to require that a field match all of the `values` instead of just one or more of them. This is useful when matching against multi-valued fields such as lists or sets where you want to ensure that all of the `values` are present in the list or set.
-        :param str match_by: One of `exact` (default), `re`, or `substring`. For string-typed fields, specify `re` to match by using the `values` as regular expressions, or specify `substring` to match by treating the `values` as substrings to find within the string field.
-        """
-        pulumi.set(__self__, "key", key)
-        pulumi.set(__self__, "values", values)
-        if all is not None:
-            pulumi.set(__self__, "all", all)
-        if match_by is not None:
-            pulumi.set(__self__, "match_by", match_by)
-
-    @property
-    @pulumi.getter
-    def key(self) -> str:
-        """
-        Filter sizes by this key. This may be one of `cpu`, `description`, `disk`, `name`, `ram`, `selectable`, `type`.
-        """
-        return pulumi.get(self, "key")
-
-    @property
-    @pulumi.getter
-    def values(self) -> Sequence[str]:
-        """
-        Only retrieves `sizes` which keys has value that matches one of the values provided here
-        """
-        return pulumi.get(self, "values")
-
-    @property
-    @pulumi.getter
-    def all(self) -> Optional[bool]:
-        """
-        Set to `true` to require that a field match all of the `values` instead of just one or more of them. This is useful when matching against multi-valued fields such as lists or sets where you want to ensure that all of the `values` are present in the list or set.
-        """
-        return pulumi.get(self, "all")
-
-    @property
-    @pulumi.getter(name="matchBy")
-    def match_by(self) -> Optional[str]:
-        """
-        One of `exact` (default), `re`, or `substring`. For string-typed fields, specify `re` to match by using the `values` as regular expressions, or specify `substring` to match by treating the `values` as substrings to find within the string field.
-        """
-        return pulumi.get(self, "match_by")
-
-
-@pulumi.output_type
-class GetInstancesSizeSizeResult(dict):
-    def __init__(__self__, *,
-                 cpu: int,
-                 description: str,
-                 disk: int,
-                 name: str,
-                 ram: int,
-                 selectable: bool,
-                 type: str):
-        pulumi.set(__self__, "cpu", cpu)
-        pulumi.set(__self__, "description", description)
-        pulumi.set(__self__, "disk", disk)
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "ram", ram)
-        pulumi.set(__self__, "selectable", selectable)
-        pulumi.set(__self__, "type", type)
-
-    @property
-    @pulumi.getter
-    def cpu(self) -> int:
-        return pulumi.get(self, "cpu")
-
-    @property
-    @pulumi.getter
-    def description(self) -> str:
-        return pulumi.get(self, "description")
-
-    @property
-    @pulumi.getter
-    def disk(self) -> int:
-        return pulumi.get(self, "disk")
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        return pulumi.get(self, "name")
-
-    @property
-    @pulumi.getter
-    def ram(self) -> int:
-        return pulumi.get(self, "ram")
-
-    @property
-    @pulumi.getter
-    def selectable(self) -> bool:
-        return pulumi.get(self, "selectable")
-
-    @property
-    @pulumi.getter
-    def type(self) -> str:
-        return pulumi.get(self, "type")
-
-
-@pulumi.output_type
-class GetInstancesSizeSortResult(dict):
-    def __init__(__self__, *,
-                 key: str,
-                 direction: Optional[str] = None):
-        """
-        :param str key: Sort sizes by this key. This may be one of `cpu`, `description`, `disk`, `name`, `ram`, `selectable`, `type`.
-        :param str direction: The sort direction. This may be either `asc` or `desc`.
-        """
-        pulumi.set(__self__, "key", key)
-        if direction is not None:
-            pulumi.set(__self__, "direction", direction)
-
-    @property
-    @pulumi.getter
-    def key(self) -> str:
-        """
-        Sort sizes by this key. This may be one of `cpu`, `description`, `disk`, `name`, `ram`, `selectable`, `type`.
-        """
-        return pulumi.get(self, "key")
-
-    @property
-    @pulumi.getter
-    def direction(self) -> Optional[str]:
-        """
-        The sort direction. This may be either `asc` or `desc`.
-        """
-        return pulumi.get(self, "direction")
-
-
-@pulumi.output_type
 class GetInstancesSortResult(dict):
     def __init__(__self__, *,
                  key: str,
                  direction: Optional[str] = None):
         """
         :param str key: Sort instances by this key. This may be one of `cpu_cores`, `created_at`, `disk_gb`, `firewall_id`, `hostname`, `id`, `initial_password`, `initial_user`, `network_id`, `notes`, `private_ip`, `pseudo_ip`, `public_ip`, `ram_mb`, `region`, `reverse_dns`, `script`, `size`, `sshkey_id`, `status`, `template`.
         :param str direction: The sort direction. This may be either `asc` or `desc`.
```

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/provider.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/reserved_ip.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/reserved_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/ssh_key.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/volume.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo/volume_attachment.py` & `pulumi_civo-2.4.0a1686784153/pulumi_civo/volume_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo.egg-info/PKG-INFO` & `pulumi_civo-2.4.0a1686784153/pulumi_civo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-civo
-Version: 2.4.0a1686633661
+Version: 2.4.0a1686784153
 Summary: A Pulumi package for creating and managing Civo cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-civo
 Keywords: pulumi civo
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_civo-2.4.0a1686633661/pulumi_civo.egg-info/SOURCES.txt` & `pulumi_civo-2.4.0a1686784153/pulumi_civo.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 pulumi_civo/_utilities.py
 pulumi_civo/database.py
 pulumi_civo/dns_domain_name.py
 pulumi_civo/dns_domain_record.py
 pulumi_civo/firewall.py
 pulumi_civo/firewall_rule.py
 pulumi_civo/get_database.py
+pulumi_civo/get_database_version.py
 pulumi_civo/get_disk_image.py
 pulumi_civo/get_dns_domain_name.py
 pulumi_civo/get_dns_domain_record.py
 pulumi_civo/get_firewall.py
 pulumi_civo/get_instance.py
 pulumi_civo/get_instances.py
-pulumi_civo/get_instances_size.py
 pulumi_civo/get_kubernetes_cluster.py
 pulumi_civo/get_kubernetes_version.py
 pulumi_civo/get_load_balancer.py
 pulumi_civo/get_network.py
 pulumi_civo/get_object_store.py
 pulumi_civo/get_object_store_credential.py
 pulumi_civo/get_region.py
```

### Comparing `pulumi_civo-2.4.0a1686633661/setup.py` & `pulumi_civo-2.4.0a1686784153/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "2.4.0a1686633661"
-PLUGIN_VERSION = "2.4.0-alpha.1686633661+567dd156"
+VERSION = "2.4.0a1686784153"
+PLUGIN_VERSION = "2.4.0-alpha.1686784153+7275ee29"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'civo', PLUGIN_VERSION])
         except OSError as error:
```

