# Comparing `tmp/cdktf-cdktf-provider-azuread-7.0.4.tar.gz` & `tmp/cdktf-cdktf-provider-azuread-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-azuread-7.0.4.tar", last modified: Thu Jun  1 14:11:42 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-azuread-8.0.0.tar", last modified: Thu Jun 15 11:20:36 2023, max compression
```

## Comparing `cdktf-cdktf-provider-azuread-7.0.4.tar` & `cdktf-cdktf-provider-azuread-8.0.0.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.762685 cdktf-cdktf-provider-azuread-7.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-01 14:11:42.762685 cdktf-cdktf-provider-azuread-7.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:11:42.762685 cdktf-cdktf-provider-azuread-7.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.742685 cdktf-cdktf-provider-azuread-7.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.750685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/
--rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.750685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   665771 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/_jsii/provider-azuread@7.0.4.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.750685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/access_package/
--rw-r--r--   0 runner    (1001) docker     (123)    40228 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/access_package/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.750685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/access_package_assignment_policy/
--rw-r--r--   0 runner    (1001) docker     (123)   318206 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/access_package_assignment_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.750685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/access_package_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)    42414 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/access_package_catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.750685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/access_package_catalog_role_assignment/
--rw-r--r--   0 runner    (1001) docker     (123)    39434 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/access_package_catalog_role_assignment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.750685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/access_package_resource_catalog_association/
--rw-r--r--   0 runner    (1001) docker     (123)    38467 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/access_package_resource_catalog_association/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.750685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/access_package_resource_package_association/
--rw-r--r--   0 runner    (1001) docker     (123)    38823 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/access_package_resource_package_association/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.750685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/administrative_unit/
--rw-r--r--   0 runner    (1001) docker     (123)    46305 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/administrative_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.750685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/administrative_unit_member/
--rw-r--r--   0 runner    (1001) docker     (123)    37211 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/administrative_unit_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.750685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/administrative_unit_role_member/
--rw-r--r--   0 runner    (1001) docker     (123)    39472 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/administrative_unit_role_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.750685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/app_role_assignment/
--rw-r--r--   0 runner    (1001) docker     (123)    36629 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/app_role_assignment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.750685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/application/
--rw-r--r--   0 runner    (1001) docker     (123)   346736 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.754685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/application_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    52745 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/application_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.754685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/application_federated_identity_credential/
--rw-r--r--   0 runner    (1001) docker     (123)    48984 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/application_federated_identity_credential/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.754685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/application_password/
--rw-r--r--   0 runner    (1001) docker     (123)    48631 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/application_password/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.754685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/application_pre_authorized/
--rw-r--r--   0 runner    (1001) docker     (123)    39349 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/application_pre_authorized/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.754685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/claims_mapping_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    20784 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/claims_mapping_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.754685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/conditional_access_policy/
--rw-r--r--   0 runner    (1001) docker     (123)   163936 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/conditional_access_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.754685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/custom_directory_role/
--rw-r--r--   0 runner    (1001) docker     (123)    60177 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/custom_directory_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.754685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_access_package/
--rw-r--r--   0 runner    (1001) docker     (123)    32321 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_access_package/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.754685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_access_package_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)    30568 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_access_package_catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.754685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_access_package_catalog_role/
--rw-r--r--   0 runner    (1001) docker     (123)    30595 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_access_package_catalog_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.754685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_administrative_unit/
--rw-r--r--   0 runner    (1001) docker     (123)    37150 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_administrative_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.754685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_application/
--rw-r--r--   0 runner    (1001) docker     (123)   172398 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.754685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_application_published_app_ids/
--rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_application_published_app_ids/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.754685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_application_template/
--rw-r--r--   0 runner    (1001) docker     (123)    31144 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_application_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.754685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_client_config/
--rw-r--r--   0 runner    (1001) docker     (123)    24750 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_client_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.754685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_directory_object/
--rw-r--r--   0 runner    (1001) docker     (123)    26814 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_directory_object/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.754685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_directory_roles/
--rw-r--r--   0 runner    (1001) docker     (123)    34425 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_directory_roles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.754685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_domains/
--rw-r--r--   0 runner    (1001) docker     (123)    53864 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_domains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.754685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_group/
--rw-r--r--   0 runner    (1001) docker     (123)    49604 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_groups/
--rw-r--r--   0 runner    (1001) docker     (123)    45029 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_groups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_service_principal/
--rw-r--r--   0 runner    (1001) docker     (123)    86938 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_service_principal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_service_principals/
--rw-r--r--   0 runner    (1001) docker     (123)    52122 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_service_principals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_user/
--rw-r--r--   0 runner    (1001) docker     (123)    41338 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_users/
--rw-r--r--   0 runner    (1001) docker     (123)    49680 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_users/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/directory_role/
--rw-r--r--   0 runner    (1001) docker     (123)    35881 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/directory_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/directory_role_assignment/
--rw-r--r--   0 runner    (1001) docker     (123)    47879 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/directory_role_assignment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/directory_role_member/
--rw-r--r--   0 runner    (1001) docker     (123)    36214 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/directory_role_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/group/
--rw-r--r--   0 runner    (1001) docker     (123)   107807 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/group_member/
--rw-r--r--   0 runner    (1001) docker     (123)    35352 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/group_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/invitation/
--rw-r--r--   0 runner    (1001) docker     (123)    53926 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/invitation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/named_location/
--rw-r--r--   0 runner    (1001) docker     (123)    54830 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/named_location/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    59133 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/service_principal/
--rw-r--r--   0 runner    (1001) docker     (123)   151087 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/service_principal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/service_principal_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    53133 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/service_principal_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/service_principal_claims_mapping_policy_assignment/
--rw-r--r--   0 runner    (1001) docker     (123)    22225 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/service_principal_claims_mapping_policy_assignment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/service_principal_delegated_permission_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    44961 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/service_principal_delegated_permission_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/service_principal_password/
--rw-r--r--   0 runner    (1001) docker     (123)    49229 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/service_principal_password/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/service_principal_token_signing_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    41707 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/service_principal_token_signing_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/synchronization_job/
--rw-r--r--   0 runner    (1001) docker     (123)    48267 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/synchronization_job/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/synchronization_secret/
--rw-r--r--   0 runner    (1001) docker     (123)    51470 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/synchronization_secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.758685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/user/
--rw-r--r--   0 runner    (1001) docker     (123)   128509 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.762685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/user_flow_attribute/
--rw-r--r--   0 runner    (1001) docker     (123)    37925 2023-06-01 14:11:30.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/user_flow_attribute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:11:42.750685 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-01 14:11:42.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-01 14:11:42.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:11:42.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:11:42.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 14:11:42.000000 cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:36.000445 cdktf-cdktf-provider-azuread-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-15 11:20:36.000445 cdktf-cdktf-provider-azuread-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:20:36.000445 cdktf-cdktf-provider-azuread-8.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.984445 cdktf-cdktf-provider-azuread-8.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.988445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/
+-rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.988445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   665765 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/_jsii/provider-azuread@8.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.992445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/access_package/
+-rw-r--r--   0 runner    (1001) docker     (123)    40228 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/access_package/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.992445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/access_package_assignment_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)   318206 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/access_package_assignment_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.992445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/access_package_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    42414 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/access_package_catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.992445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/access_package_catalog_role_assignment/
+-rw-r--r--   0 runner    (1001) docker     (123)    39434 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/access_package_catalog_role_assignment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.992445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/access_package_resource_catalog_association/
+-rw-r--r--   0 runner    (1001) docker     (123)    38467 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/access_package_resource_catalog_association/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.992445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/access_package_resource_package_association/
+-rw-r--r--   0 runner    (1001) docker     (123)    38823 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/access_package_resource_package_association/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.992445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)    46305 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.992445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit_member/
+-rw-r--r--   0 runner    (1001) docker     (123)    37211 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.992445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit_role_member/
+-rw-r--r--   0 runner    (1001) docker     (123)    39472 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit_role_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.992445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/app_role_assignment/
+-rw-r--r--   0 runner    (1001) docker     (123)    36629 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/app_role_assignment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.992445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/application/
+-rw-r--r--   0 runner    (1001) docker     (123)   346736 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.992445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/application_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    52745 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/application_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.992445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/application_federated_identity_credential/
+-rw-r--r--   0 runner    (1001) docker     (123)    48984 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/application_federated_identity_credential/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.992445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/application_password/
+-rw-r--r--   0 runner    (1001) docker     (123)    48631 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/application_password/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.992445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/application_pre_authorized/
+-rw-r--r--   0 runner    (1001) docker     (123)    39349 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/application_pre_authorized/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.992445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/claims_mapping_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    20784 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/claims_mapping_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.992445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/conditional_access_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)   163936 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/conditional_access_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.992445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/custom_directory_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    60177 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/custom_directory_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.992445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_access_package/
+-rw-r--r--   0 runner    (1001) docker     (123)    32321 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_access_package/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_access_package_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    30568 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_access_package_catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_access_package_catalog_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    30595 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_access_package_catalog_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_administrative_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)    37150 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_administrative_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application/
+-rw-r--r--   0 runner    (1001) docker     (123)   172398 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application_published_app_ids/
+-rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application_published_app_ids/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application_template/
+-rw-r--r--   0 runner    (1001) docker     (123)    31144 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_client_config/
+-rw-r--r--   0 runner    (1001) docker     (123)    24750 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_client_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_directory_object/
+-rw-r--r--   0 runner    (1001) docker     (123)    26814 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_directory_object/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_directory_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)    34425 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_directory_roles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_domains/
+-rw-r--r--   0 runner    (1001) docker     (123)    53864 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_domains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_group/
+-rw-r--r--   0 runner    (1001) docker     (123)    49604 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)    45029 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_groups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_service_principal/
+-rw-r--r--   0 runner    (1001) docker     (123)    86938 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_service_principal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_service_principals/
+-rw-r--r--   0 runner    (1001) docker     (123)    52122 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_service_principals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_user/
+-rw-r--r--   0 runner    (1001) docker     (123)    41338 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_users/
+-rw-r--r--   0 runner    (1001) docker     (123)    49680 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_users/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/directory_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    35881 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/directory_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/directory_role_assignment/
+-rw-r--r--   0 runner    (1001) docker     (123)    47879 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/directory_role_assignment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/directory_role_member/
+-rw-r--r--   0 runner    (1001) docker     (123)    36214 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/directory_role_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/group/
+-rw-r--r--   0 runner    (1001) docker     (123)   107807 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/group_member/
+-rw-r--r--   0 runner    (1001) docker     (123)    35352 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/group_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/invitation/
+-rw-r--r--   0 runner    (1001) docker     (123)    53926 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/invitation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/named_location/
+-rw-r--r--   0 runner    (1001) docker     (123)    54830 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/named_location/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    59133 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.996445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/service_principal/
+-rw-r--r--   0 runner    (1001) docker     (123)   151087 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/service_principal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:36.000445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/service_principal_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    53133 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/service_principal_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:36.000445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/service_principal_claims_mapping_policy_assignment/
+-rw-r--r--   0 runner    (1001) docker     (123)    22225 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/service_principal_claims_mapping_policy_assignment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:36.000445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/service_principal_delegated_permission_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    44961 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/service_principal_delegated_permission_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:36.000445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/service_principal_password/
+-rw-r--r--   0 runner    (1001) docker     (123)    49229 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/service_principal_password/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:36.000445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/service_principal_token_signing_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    41707 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/service_principal_token_signing_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:36.000445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/synchronization_job/
+-rw-r--r--   0 runner    (1001) docker     (123)    48267 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/synchronization_job/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:36.000445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/synchronization_secret/
+-rw-r--r--   0 runner    (1001) docker     (123)    51470 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/synchronization_secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:36.000445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/user/
+-rw-r--r--   0 runner    (1001) docker     (123)   128509 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:36.000445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/user_flow_attribute/
+-rw-r--r--   0 runner    (1001) docker     (123)    37925 2023-06-15 11:20:23.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/user_flow_attribute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:20:35.988445 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-15 11:20:35.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-15 11:20:35.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:20:35.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 11:20:35.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 11:20:35.000000 cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/LICENSE` & `cdktf-cdktf-provider-azuread-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/PKG-INFO` & `cdktf-cdktf-provider-azuread-8.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-azuread
-Version: 7.0.4
+Version: 8.0.0
 Summary: Prebuilt azuread Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-azuread.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-azuread.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/README.md` & `cdktf-cdktf-provider-azuread-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/setup.py` & `cdktf-cdktf-provider-azuread-8.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-azuread",
-    "version": "7.0.4",
+    "version": "8.0.0",
     "description": "Prebuilt azuread Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-azuread.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -75,25 +75,25 @@
         "cdktf_cdktf_provider_azuread.synchronization_job",
         "cdktf_cdktf_provider_azuread.synchronization_secret",
         "cdktf_cdktf_provider_azuread.user",
         "cdktf_cdktf_provider_azuread.user_flow_attribute"
     ],
     "package_data": {
         "cdktf_cdktf_provider_azuread._jsii": [
-            "provider-azuread@7.0.4.jsii.tgz"
+            "provider-azuread@8.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_azuread": [
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

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/access_package/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/access_package/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/access_package_assignment_policy/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/access_package_assignment_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/access_package_catalog/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/access_package_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/access_package_catalog_role_assignment/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/access_package_catalog_role_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/access_package_resource_catalog_association/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/access_package_resource_catalog_association/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/access_package_resource_package_association/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/access_package_resource_package_association/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/administrative_unit/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/administrative_unit_member/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit_member/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/administrative_unit_role_member/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/administrative_unit_role_member/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/app_role_assignment/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/app_role_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/application/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/application/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/application_certificate/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/application_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/application_federated_identity_credential/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/application_federated_identity_credential/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/application_password/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/application_password/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/application_pre_authorized/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/application_pre_authorized/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/claims_mapping_policy/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/claims_mapping_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/conditional_access_policy/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/conditional_access_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/custom_directory_role/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/custom_directory_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_access_package/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_access_package/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_access_package_catalog/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_access_package_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_access_package_catalog_role/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_access_package_catalog_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_administrative_unit/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_administrative_unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_application/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_application_published_app_ids/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application_published_app_ids/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_application_template/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_application_template/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_client_config/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_client_config/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_directory_object/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_directory_object/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_directory_roles/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_directory_roles/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_domains/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_domains/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_group/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_groups/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_service_principal/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_service_principal/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_service_principals/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_service_principals/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_user/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/data_azuread_users/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/data_azuread_users/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/directory_role/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/directory_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/directory_role_assignment/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/directory_role_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/directory_role_member/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/directory_role_member/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/group/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/group_member/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/group_member/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/invitation/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/invitation/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/named_location/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/named_location/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/provider/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/service_principal/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/service_principal/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/service_principal_certificate/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/service_principal_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/service_principal_claims_mapping_policy_assignment/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/service_principal_claims_mapping_policy_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/service_principal_delegated_permission_grant/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/service_principal_delegated_permission_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/service_principal_password/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/service_principal_password/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/service_principal_token_signing_certificate/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/service_principal_token_signing_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/synchronization_job/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/synchronization_job/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/synchronization_secret/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/synchronization_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/user/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread/user_flow_attribute/__init__.py` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread/user_flow_attribute/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread.egg-info/PKG-INFO` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-azuread
-Version: 7.0.4
+Version: 8.0.0
 Summary: Prebuilt azuread Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-azuread.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-azuread.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-azuread-7.0.4/src/cdktf_cdktf_provider_azuread.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-azuread-8.0.0/src/cdktf_cdktf_provider_azuread.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_azuread/py.typed
 src/cdktf_cdktf_provider_azuread.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_azuread.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_azuread.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_azuread.egg-info/requires.txt
 src/cdktf_cdktf_provider_azuread.egg-info/top_level.txt
 src/cdktf_cdktf_provider_azuread/_jsii/__init__.py
-src/cdktf_cdktf_provider_azuread/_jsii/provider-azuread@7.0.4.jsii.tgz
+src/cdktf_cdktf_provider_azuread/_jsii/provider-azuread@8.0.0.jsii.tgz
 src/cdktf_cdktf_provider_azuread/access_package/__init__.py
 src/cdktf_cdktf_provider_azuread/access_package_assignment_policy/__init__.py
 src/cdktf_cdktf_provider_azuread/access_package_catalog/__init__.py
 src/cdktf_cdktf_provider_azuread/access_package_catalog_role_assignment/__init__.py
 src/cdktf_cdktf_provider_azuread/access_package_resource_catalog_association/__init__.py
 src/cdktf_cdktf_provider_azuread/access_package_resource_package_association/__init__.py
 src/cdktf_cdktf_provider_azuread/administrative_unit/__init__.py
```

