# Comparing `tmp/pulumi_proxmoxve-5.5.0.tar.gz` & `tmp/pulumi_proxmoxve-5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_proxmoxve-5.5.0.tar", last modified: Thu Jun  8 07:57:40 2023, max compression
+gzip compressed data, was "pulumi_proxmoxve-5.6.0.tar", last modified: Thu Jun 15 14:21:32 2023, max compression
```

## Comparing `pulumi_proxmoxve-5.5.0.tar` & `pulumi_proxmoxve-5.6.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:57:40.519412 pulumi_proxmoxve-5.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-06-08 07:57:40.519412 pulumi_proxmoxve-5.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:57:40.515412 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10392 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/certifi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:57:40.515412 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/cluster/get_nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:57:40.515412 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:57:40.515412 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/ct/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/ct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/ct/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37407 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/ct/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    15863 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/ct/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/get_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/get_hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/get_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/get_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/hosts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:57:40.515412 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/network/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/network/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/network/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/network/firewall_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/network/firewall_ip_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    29546 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/network/firewall_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/network/firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    15125 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/network/firewall_security_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/network/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:57:40.519412 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/get_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    22997 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:57:40.519412 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/storage/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17318 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/storage/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/storage/get_datastores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/storage/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:57:40.519412 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/vm/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34450 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/vm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/vm/get_virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/vm/get_virtual_machines.py
--rw-r--r--   0 runner    (1001) docker     (123)    28465 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/vm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    83149 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/vm/virtual_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:57:40.515412 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/pulumi_proxmoxve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 07:57:40.519412 pulumi_proxmoxve-5.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-08 07:57:40.000000 pulumi_proxmoxve-5.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:32.185571 pulumi_proxmoxve-5.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-15 14:21:32.185571 pulumi_proxmoxve-5.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:32.181571 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10392 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/certifi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:32.181571 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/cluster/get_nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:32.181571 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:32.181571 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/ct/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/ct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/ct/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37407 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/ct/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15863 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/ct/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/get_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/get_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/get_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/get_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/hosts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:32.181571 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall_ip_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29546 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15125 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:32.185571 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22997 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:32.185571 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/storage/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17318 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/storage/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/storage/get_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/storage/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:32.185571 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34450 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/get_virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/get_virtual_machines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28465 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83149 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/virtual_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:32.181571 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-15 14:21:32.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-15 14:21:32.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:21:32.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:21:32.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 14:21:32.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 14:21:32.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 14:21:32.185571 pulumi_proxmoxve-5.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/setup.py
```

### Comparing `pulumi_proxmoxve-5.5.0/PKG-INFO` & `pulumi_proxmoxve-5.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_proxmoxve
-Version: 5.5.0
+Version: 5.6.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -120,14 +120,15 @@
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://muehlbachler.io/"><img src="https://avatars.githubusercontent.com/u/653739?v=4?s=100" width="100px;" alt="Daniel Mühlbachler-Pietrzykowski"/><br /><sub><b>Daniel Mühlbachler-Pietrzykowski</b></sub></a><br /><a href="#maintenance-muhlba91" title="Maintenance">🚧</a> <a href="https://github.com/muhlba91/pulumi-proxmoxve/commits?author=muhlba91" title="Code">💻</a> <a href="https://github.com/muhlba91/pulumi-proxmoxve/commits?author=muhlba91" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/NCMartins"><img src="https://avatars.githubusercontent.com/u/11583533?v=4?s=100" width="100px;" alt="Nelson Costa Martins"/><br /><sub><b>Nelson Costa Martins</b></sub></a><br /><a href="#example-NCMartins" title="Examples">💡</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/guineveresaenger"><img src="https://avatars.githubusercontent.com/u/13116240?v=4?s=100" width="100px;" alt="Guinevere Saenger"/><br /><sub><b>Guinevere Saenger</b></sub></a><br /><a href="https://github.com/muhlba91/pulumi-proxmoxve/commits?author=guineveresaenger" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/susanev"><img src="https://avatars.githubusercontent.com/u/5489125?v=4?s=100" width="100px;" alt="Susan Evans"/><br /><sub><b>Susan Evans</b></sub></a><br /><a href="https://github.com/muhlba91/pulumi-proxmoxve/commits?author=susanev" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `pulumi_proxmoxve-5.5.0/README.md` & `pulumi_proxmoxve-5.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://muehlbachler.io/"><img src="https://avatars.githubusercontent.com/u/653739?v=4?s=100" width="100px;" alt="Daniel Mühlbachler-Pietrzykowski"/><br /><sub><b>Daniel Mühlbachler-Pietrzykowski</b></sub></a><br /><a href="#maintenance-muhlba91" title="Maintenance">🚧</a> <a href="https://github.com/muhlba91/pulumi-proxmoxve/commits?author=muhlba91" title="Code">💻</a> <a href="https://github.com/muhlba91/pulumi-proxmoxve/commits?author=muhlba91" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/NCMartins"><img src="https://avatars.githubusercontent.com/u/11583533?v=4?s=100" width="100px;" alt="Nelson Costa Martins"/><br /><sub><b>Nelson Costa Martins</b></sub></a><br /><a href="#example-NCMartins" title="Examples">💡</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/guineveresaenger"><img src="https://avatars.githubusercontent.com/u/13116240?v=4?s=100" width="100px;" alt="Guinevere Saenger"/><br /><sub><b>Guinevere Saenger</b></sub></a><br /><a href="https://github.com/muhlba91/pulumi-proxmoxve/commits?author=guineveresaenger" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/susanev"><img src="https://avatars.githubusercontent.com/u/5489125?v=4?s=100" width="100px;" alt="Susan Evans"/><br /><sub><b>Susan Evans</b></sub></a><br /><a href="https://github.com/muhlba91/pulumi-proxmoxve/commits?author=susanev" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/__init__.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/_inputs.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/_utilities.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/certifi.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/certifi.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/cluster/get_nodes.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/cluster/get_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/config/outputs.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/config/vars.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/ct/_inputs.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/ct/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/ct/container.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/ct/container.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/ct/outputs.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/ct/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/dns.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/get_dns.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/get_dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/get_hosts.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/get_hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/get_time.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/get_time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/get_version.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/get_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/hosts.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/network/_inputs.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/network/firewall.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/network/firewall_alias.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/network/firewall_ip_set.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall_ip_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/network/firewall_options.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall_options.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/network/firewall_rules.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/network/firewall_security_group.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall_security_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/network/outputs.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/outputs.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/__init__.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/_inputs.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/get_group.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/get_groups.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/get_pool.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/get_pools.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/get_role.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/get_roles.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/get_user.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/get_users.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/group.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/outputs.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/pool.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/role.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/permission/user.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/provider.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/storage/_inputs.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/storage/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/storage/file.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/storage/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/storage/get_datastores.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/storage/get_datastores.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/storage/outputs.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/storage/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/time.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/vm/_inputs.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/vm/get_virtual_machine.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/get_virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/vm/get_virtual_machines.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/get_virtual_machines.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/vm/outputs.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve/vm/virtual_machine.py` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve.egg-info/PKG-INFO` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-proxmoxve
-Version: 5.5.0
+Version: 5.6.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -120,14 +120,15 @@
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://muehlbachler.io/"><img src="https://avatars.githubusercontent.com/u/653739?v=4?s=100" width="100px;" alt="Daniel Mühlbachler-Pietrzykowski"/><br /><sub><b>Daniel Mühlbachler-Pietrzykowski</b></sub></a><br /><a href="#maintenance-muhlba91" title="Maintenance">🚧</a> <a href="https://github.com/muhlba91/pulumi-proxmoxve/commits?author=muhlba91" title="Code">💻</a> <a href="https://github.com/muhlba91/pulumi-proxmoxve/commits?author=muhlba91" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/NCMartins"><img src="https://avatars.githubusercontent.com/u/11583533?v=4?s=100" width="100px;" alt="Nelson Costa Martins"/><br /><sub><b>Nelson Costa Martins</b></sub></a><br /><a href="#example-NCMartins" title="Examples">💡</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/guineveresaenger"><img src="https://avatars.githubusercontent.com/u/13116240?v=4?s=100" width="100px;" alt="Guinevere Saenger"/><br /><sub><b>Guinevere Saenger</b></sub></a><br /><a href="https://github.com/muhlba91/pulumi-proxmoxve/commits?author=guineveresaenger" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/susanev"><img src="https://avatars.githubusercontent.com/u/5489125?v=4?s=100" width="100px;" alt="Susan Evans"/><br /><sub><b>Susan Evans</b></sub></a><br /><a href="https://github.com/muhlba91/pulumi-proxmoxve/commits?author=susanev" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `pulumi_proxmoxve-5.5.0/pulumi_proxmoxve.egg-info/SOURCES.txt` & `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.5.0/setup.py` & `pulumi_proxmoxve-5.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.5.0"
-PLUGIN_VERSION = "5.5.0"
+VERSION = "5.6.0"
+PLUGIN_VERSION = "5.6.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'proxmoxve', PLUGIN_VERSION, '--server', 'github://api.github.com/muhlba91/pulumi-proxmoxve'])
         except OSError as error:
```

