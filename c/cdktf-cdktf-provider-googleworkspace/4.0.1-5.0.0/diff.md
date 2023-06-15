# Comparing `tmp/cdktf-cdktf-provider-googleworkspace-4.0.1.tar.gz` & `tmp/cdktf-cdktf-provider-googleworkspace-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-googleworkspace-4.0.1.tar", last modified: Thu Jun  1 14:22:50 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-googleworkspace-5.0.0.tar", last modified: Thu Jun 15 11:26:20 2023, max compression
```

## Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1.tar` & `cdktf-cdktf-provider-googleworkspace-5.0.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.960778 cdktf-cdktf-provider-googleworkspace-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-01 14:22:50.956778 cdktf-cdktf-provider-googleworkspace-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:22:50.960778 cdktf-cdktf-provider-googleworkspace-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.944778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.948778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.948778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   320152 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/_jsii/provider-googleworkspace@4.0.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.952778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/chrome_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    35905 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/chrome_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.952778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_chrome_policy_schema/
--rw-r--r--   0 runner    (1001) docker     (123)    69047 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_chrome_policy_schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.952778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_domain/
--rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.952778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_domain_alias/
--rw-r--r--   0 runner    (1001) docker     (123)    16316 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_domain_alias/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.952778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group/
--rw-r--r--   0 runner    (1001) docker     (123)    20143 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.952778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group_member/
--rw-r--r--   0 runner    (1001) docker     (123)    22279 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.952778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group_members/
--rw-r--r--   0 runner    (1001) docker     (123)    29663 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group_members/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.952778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group_settings/
--rw-r--r--   0 runner    (1001) docker     (123)    21522 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group_settings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.952778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_groups/
--rw-r--r--   0 runner    (1001) docker     (123)    26540 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_groups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.952778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_org_unit/
--rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_org_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.952778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_privileges/
--rw-r--r--   0 runner    (1001) docker     (123)    26133 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_privileges/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.952778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_role/
--rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.952778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_schema/
--rw-r--r--   0 runner    (1001) docker     (123)    38540 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.952778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_user/
--rw-r--r--   0 runner    (1001) docker     (123)   173381 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.952778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_users/
--rw-r--r--   0 runner    (1001) docker     (123)   181541 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_users/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.956778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/domain/
--rw-r--r--   0 runner    (1001) docker     (123)    15971 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.956778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/domain_alias/
--rw-r--r--   0 runner    (1001) docker     (123)    18927 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/domain_alias/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.956778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/gmail_send_as_alias/
--rw-r--r--   0 runner    (1001) docker     (123)    55657 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/gmail_send_as_alias/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.956778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/group/
--rw-r--r--   0 runner    (1001) docker     (123)    33875 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.956778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/group_member/
--rw-r--r--   0 runner    (1001) docker     (123)    40429 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/group_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.956778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/group_members/
--rw-r--r--   0 runner    (1001) docker     (123)    40792 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/group_members/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.956778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/group_settings/
--rw-r--r--   0 runner    (1001) docker     (123)   131945 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/group_settings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.956778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/org_unit/
--rw-r--r--   0 runner    (1001) docker     (123)    28456 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/org_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.956778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    25278 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.956778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/role/
--rw-r--r--   0 runner    (1001) docker     (123)    34927 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.956778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/role_assignment/
--rw-r--r--   0 runner    (1001) docker     (123)    23189 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/role_assignment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.956778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/schema/
--rw-r--r--   0 runner    (1001) docker     (123)    69144 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.956778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/user/
--rw-r--r--   0 runner    (1001) docker     (123)   428942 2023-06-01 14:22:36.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:22:50.948778 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-01 14:22:50.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-01 14:22:50.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:22:50.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:22:50.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-01 14:22:50.000000 cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.971926 cdktf-cdktf-provider-googleworkspace-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-15 11:26:20.971926 cdktf-cdktf-provider-googleworkspace-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:26:20.971926 cdktf-cdktf-provider-googleworkspace-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.963925 cdktf-cdktf-provider-googleworkspace-5.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.963925 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   320150 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/_jsii/provider-googleworkspace@5.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/chrome_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    35905 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/chrome_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_chrome_policy_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)    69047 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_chrome_policy_schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_domain/
+-rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_domain_alias/
+-rw-r--r--   0 runner    (1001) docker     (123)    16316 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_domain_alias/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group/
+-rw-r--r--   0 runner    (1001) docker     (123)    20143 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group_member/
+-rw-r--r--   0 runner    (1001) docker     (123)    22279 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group_members/
+-rw-r--r--   0 runner    (1001) docker     (123)    29663 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group_members/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)    21522 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group_settings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)    26540 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_groups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_org_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_org_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_privileges/
+-rw-r--r--   0 runner    (1001) docker     (123)    26133 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_privileges/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)    38540 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_user/
+-rw-r--r--   0 runner    (1001) docker     (123)   173381 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_users/
+-rw-r--r--   0 runner    (1001) docker     (123)   181541 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_users/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)    15971 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/domain_alias/
+-rw-r--r--   0 runner    (1001) docker     (123)    18927 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/domain_alias/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/gmail_send_as_alias/
+-rw-r--r--   0 runner    (1001) docker     (123)    55657 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/gmail_send_as_alias/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/group/
+-rw-r--r--   0 runner    (1001) docker     (123)    33875 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/group_member/
+-rw-r--r--   0 runner    (1001) docker     (123)    40429 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/group_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/group_members/
+-rw-r--r--   0 runner    (1001) docker     (123)    40792 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/group_members/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/group_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)   131945 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/group_settings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.971926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/org_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)    28456 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/org_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.971926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    25278 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.971926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/role/
+-rw-r--r--   0 runner    (1001) docker     (123)    34927 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.971926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/role_assignment/
+-rw-r--r--   0 runner    (1001) docker     (123)    23189 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/role_assignment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.971926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)    69144 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.971926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/user/
+-rw-r--r--   0 runner    (1001) docker     (123)   428942 2023-06-15 11:26:06.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:26:20.967926 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-15 11:26:20.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-15 11:26:20.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:26:20.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 11:26:20.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 11:26:20.000000 cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/LICENSE` & `cdktf-cdktf-provider-googleworkspace-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/PKG-INFO` & `cdktf-cdktf-provider-googleworkspace-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-googleworkspace
-Version: 4.0.1
+Version: 5.0.0
 Summary: Prebuilt googleworkspace Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-googleworkspace.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-googleworkspace.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/README.md` & `cdktf-cdktf-provider-googleworkspace-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/setup.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-googleworkspace",
-    "version": "4.0.1",
+    "version": "5.0.0",
     "description": "Prebuilt googleworkspace Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-googleworkspace.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -50,25 +50,25 @@
         "cdktf_cdktf_provider_googleworkspace.role",
         "cdktf_cdktf_provider_googleworkspace.role_assignment",
         "cdktf_cdktf_provider_googleworkspace.schema",
         "cdktf_cdktf_provider_googleworkspace.user"
     ],
     "package_data": {
         "cdktf_cdktf_provider_googleworkspace._jsii": [
-            "provider-googleworkspace@4.0.1.jsii.tgz"
+            "provider-googleworkspace@5.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_googleworkspace": [
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

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/chrome_policy/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/chrome_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_chrome_policy_schema/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_chrome_policy_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_domain/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_domain/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_domain_alias/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_domain_alias/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group_member/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group_member/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group_members/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group_members/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group_settings/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_groups/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_org_unit/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_org_unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_privileges/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_privileges/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_role/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_schema/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_user/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_users/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_users/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/domain/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/domain_alias/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/domain_alias/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/gmail_send_as_alias/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/gmail_send_as_alias/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/group/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/group_member/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/group_member/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/group_members/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/group_members/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/group_settings/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/group_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/org_unit/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/org_unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/provider/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/role/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/role_assignment/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/role_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/schema/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace/user/__init__.py` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace/user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace.egg-info/PKG-INFO` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-googleworkspace
-Version: 4.0.1
+Version: 5.0.0
 Summary: Prebuilt googleworkspace Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-googleworkspace.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-googleworkspace.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-googleworkspace-4.0.1/src/cdktf_cdktf_provider_googleworkspace.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-googleworkspace-5.0.0/src/cdktf_cdktf_provider_googleworkspace.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_googleworkspace/py.typed
 src/cdktf_cdktf_provider_googleworkspace.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_googleworkspace.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_googleworkspace.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_googleworkspace.egg-info/requires.txt
 src/cdktf_cdktf_provider_googleworkspace.egg-info/top_level.txt
 src/cdktf_cdktf_provider_googleworkspace/_jsii/__init__.py
-src/cdktf_cdktf_provider_googleworkspace/_jsii/provider-googleworkspace@4.0.1.jsii.tgz
+src/cdktf_cdktf_provider_googleworkspace/_jsii/provider-googleworkspace@5.0.0.jsii.tgz
 src/cdktf_cdktf_provider_googleworkspace/chrome_policy/__init__.py
 src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_chrome_policy_schema/__init__.py
 src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_domain/__init__.py
 src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_domain_alias/__init__.py
 src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group/__init__.py
 src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group_member/__init__.py
 src/cdktf_cdktf_provider_googleworkspace/data_googleworkspace_group_members/__init__.py
```

