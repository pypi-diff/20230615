# Comparing `tmp/cdktf-cdktf-provider-databricks-7.0.7.tar.gz` & `tmp/cdktf-cdktf-provider-databricks-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-databricks-7.0.7.tar", last modified: Thu Jun 15 03:18:41 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-databricks-8.0.0.tar", last modified: Thu Jun 15 11:24:59 2023, max compression
```

## Comparing `cdktf-cdktf-provider-databricks-7.0.7.tar` & `cdktf-cdktf-provider-databricks-8.0.0.tar`

### file list

```diff
@@ -1,237 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.513399 cdktf-cdktf-provider-databricks-7.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-06-15 03:18:41.513399 cdktf-cdktf-provider-databricks-7.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 03:18:41.513399 cdktf-cdktf-provider-databricks-7.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.461399 cdktf-cdktf-provider-databricks-7.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.477399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/
--rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.477399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1486573 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/_jsii/provider-databricks@7.0.7.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.481399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/aws_s3_mount/
--rw-r--r--   0 runner    (1001) docker     (123)    25103 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/aws_s3_mount/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.481399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/azure_adls_gen1_mount/
--rw-r--r--   0 runner    (1001) docker     (123)    37192 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/azure_adls_gen1_mount/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.481399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/azure_adls_gen2_mount/
--rw-r--r--   0 runner    (1001) docker     (123)    39923 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/azure_adls_gen2_mount/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.481399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/azure_blob_mount/
--rw-r--r--   0 runner    (1001) docker     (123)    34286 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/azure_blob_mount/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.481399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)    39684 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.481399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)   374730 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.481399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/cluster_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    31179 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/cluster_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.481399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_aws_assume_role_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_aws_assume_role_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.481399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_aws_bucket_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    26627 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_aws_bucket_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.481399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_aws_crossaccount_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    18946 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_aws_crossaccount_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.481399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)    18139 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_catalogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.485399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)   405001 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.485399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_cluster_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    34768 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_cluster_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.485399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_clusters/
--rw-r--r--   0 runner    (1001) docker     (123)    18782 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_clusters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.485399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_current_user/
--rw-r--r--   0 runner    (1001) docker     (123)    16942 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_current_user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.485399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file/
--rw-r--r--   0 runner    (1001) docker     (123)    21011 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.485399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file_paths/
--rw-r--r--   0 runner    (1001) docker     (123)    30164 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file_paths/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.485399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_directory/
--rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_directory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.485399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_group/
--rw-r--r--   0 runner    (1001) docker     (123)    52152 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.485399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_instance_pool/
--rw-r--r--   0 runner    (1001) docker     (123)   214292 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_instance_pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.485399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_job/
--rw-r--r--   0 runner    (1001) docker     (123)  1628066 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_job/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.489399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_jobs/
--rw-r--r--   0 runner    (1001) docker     (123)    18211 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_jobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.489399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_mws_credentials/
--rw-r--r--   0 runner    (1001) docker     (123)    18514 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_mws_credentials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.489399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_mws_workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_mws_workspaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.489399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_node_type/
--rw-r--r--   0 runner    (1001) docker     (123)    52603 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_node_type/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.489399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_notebook/
--rw-r--r--   0 runner    (1001) docker     (123)    27043 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_notebook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.489399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_notebook_paths/
--rw-r--r--   0 runner    (1001) docker     (123)    30333 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_notebook_paths/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.489399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.489399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    20311 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.489399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_service_principal/
--rw-r--r--   0 runner    (1001) docker     (123)    33251 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_service_principal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.489399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_service_principals/
--rw-r--r--   0 runner    (1001) docker     (123)    21674 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_service_principals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.489399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_share/
--rw-r--r--   0 runner    (1001) docker     (123)    91706 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_share/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.489399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_shares/
--rw-r--r--   0 runner    (1001) docker     (123)    18189 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_shares/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.489399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_spark_version/
--rw-r--r--   0 runner    (1001) docker     (123)    43822 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_spark_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.493399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouse/
--rw-r--r--   0 runner    (1001) docker     (123)    98211 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.493399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouses/
--rw-r--r--   0 runner    (1001) docker     (123)    21182 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.493399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_tables/
--rw-r--r--   0 runner    (1001) docker     (123)    22429 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.493399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_user/
--rw-r--r--   0 runner    (1001) docker     (123)    21375 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.493399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_views/
--rw-r--r--   0 runner    (1001) docker     (123)    22388 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.493399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_zones/
--rw-r--r--   0 runner    (1001) docker     (123)    16121 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_zones/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.493399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/dbfs_file/
--rw-r--r--   0 runner    (1001) docker     (123)    24655 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/dbfs_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.493399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/directory/
--rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/directory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.493399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/entitlements/
--rw-r--r--   0 runner    (1001) docker     (123)    36323 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/entitlements/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.493399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/external_location/
--rw-r--r--   0 runner    (1001) docker     (123)    38113 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/external_location/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.493399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/git_credential/
--rw-r--r--   0 runner    (1001) docker     (123)    25909 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/git_credential/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.493399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/global_init_script/
--rw-r--r--   0 runner    (1001) docker     (123)    35510 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/global_init_script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.493399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/grants/
--rw-r--r--   0 runner    (1001) docker     (123)    55461 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/grants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.493399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/group/
--rw-r--r--   0 runner    (1001) docker     (123)    38035 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.493399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/group_instance_profile/
--rw-r--r--   0 runner    (1001) docker     (123)    20452 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/group_instance_profile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.493399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/group_member/
--rw-r--r--   0 runner    (1001) docker     (123)    19797 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/group_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.493399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/group_role/
--rw-r--r--   0 runner    (1001) docker     (123)    19568 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/group_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.493399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/instance_pool/
--rw-r--r--   0 runner    (1001) docker     (123)   171446 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/instance_pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.497399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/instance_profile/
--rw-r--r--   0 runner    (1001) docker     (123)    27316 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/instance_profile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.497399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/ip_access_list/
--rw-r--r--   0 runner    (1001) docker     (123)    24956 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/ip_access_list/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.497399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/job/
--rw-r--r--   0 runner    (1001) docker     (123)  1504922 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/job/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.497399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/library/
--rw-r--r--   0 runner    (1001) docker     (123)    54504 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.497399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/metastore/
--rw-r--r--   0 runner    (1001) docker     (123)    53817 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/metastore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.497399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/metastore_assignment/
--rw-r--r--   0 runner    (1001) docker     (123)    23058 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/metastore_assignment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.501399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/metastore_data_access/
--rw-r--r--   0 runner    (1001) docker     (123)    79505 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/metastore_data_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.501399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mlflow_experiment/
--rw-r--r--   0 runner    (1001) docker     (123)    38578 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mlflow_experiment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.501399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mlflow_model/
--rw-r--r--   0 runner    (1001) docker     (123)    47009 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mlflow_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.501399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mlflow_webhook/
--rw-r--r--   0 runner    (1001) docker     (123)    53025 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mlflow_webhook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.501399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/model_serving/
--rw-r--r--   0 runner    (1001) docker     (123)    81786 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/model_serving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.501399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mount/
--rw-r--r--   0 runner    (1001) docker     (123)   121729 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mount/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.501399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_credentials/
--rw-r--r--   0 runner    (1001) docker     (123)    22803 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_credentials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.501399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_customer_managed_keys/
--rw-r--r--   0 runner    (1001) docker     (123)    46981 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_customer_managed_keys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.501399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_log_delivery/
--rw-r--r--   0 runner    (1001) docker     (123)    42349 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_log_delivery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.501399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_networks/
--rw-r--r--   0 runner    (1001) docker     (123)    85166 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.501399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_permission_assignment/
--rw-r--r--   0 runner    (1001) docker     (123)    22828 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_permission_assignment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.501399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_private_access_settings/
--rw-r--r--   0 runner    (1001) docker     (123)    37950 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_private_access_settings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.501399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_storage_configurations/
--rw-r--r--   0 runner    (1001) docker     (123)    23504 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_storage_configurations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.501399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_vpc_endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)    56430 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_vpc_endpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.501399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)   148773 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_workspaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.505399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)    33598 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/notebook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.505399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/obo_token/
--rw-r--r--   0 runner    (1001) docker     (123)    22810 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/obo_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.505399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/permission_assignment/
--rw-r--r--   0 runner    (1001) docker     (123)    20476 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/permission_assignment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.505399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/permissions/
--rw-r--r--   0 runner    (1001) docker     (123)    92218 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/permissions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.505399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)   340923 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.505399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    75645 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.505399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/provider_resource/
--rw-r--r--   0 runner    (1001) docker     (123)    24759 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/provider_resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.505399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/recipient/
--rw-r--r--   0 runner    (1001) docker     (123)    64516 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/recipient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.505399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/repo/
--rw-r--r--   0 runner    (1001) docker     (123)    36402 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/repo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.505399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/schema/
--rw-r--r--   0 runner    (1001) docker     (123)    34497 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.505399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/secret/
--rw-r--r--   0 runner    (1001) docker     (123)    21865 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.505399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/secret_acl/
--rw-r--r--   0 runner    (1001) docker     (123)    21743 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/secret_acl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.505399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/secret_scope/
--rw-r--r--   0 runner    (1001) docker     (123)    33202 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/secret_scope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.505399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/service_principal/
--rw-r--r--   0 runner    (1001) docker     (123)    53372 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/service_principal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.505399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/service_principal_role/
--rw-r--r--   0 runner    (1001) docker     (123)    20359 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/service_principal_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.509399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/service_principal_secret/
--rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/service_principal_secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.509399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/share/
--rw-r--r--   0 runner    (1001) docker     (123)    89048 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/share/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.509399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_alert/
--rw-r--r--   0 runner    (1001) docker     (123)    42260 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_alert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.509399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)    22195 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.509399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)   105173 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_endpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.509399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_global_config/
--rw-r--r--   0 runner    (1001) docker     (123)    30740 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_global_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.509399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_permissions/
--rw-r--r--   0 runner    (1001) docker     (123)    52298 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_permissions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.509399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_query/
--rw-r--r--   0 runner    (1001) docker     (123)   223497 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_query/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.509399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_table/
--rw-r--r--   0 runner    (1001) docker     (123)    62781 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.509399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_visualization/
--rw-r--r--   0 runner    (1001) docker     (123)    31228 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.509399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_widget/
--rw-r--r--   0 runner    (1001) docker     (123)    70645 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_widget/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.509399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/storage_credential/
--rw-r--r--   0 runner    (1001) docker     (123)    80952 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/storage_credential/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.509399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/table/
--rw-r--r--   0 runner    (1001) docker     (123)    75587 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.509399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/token/
--rw-r--r--   0 runner    (1001) docker     (123)    27481 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.513399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/user/
--rw-r--r--   0 runner    (1001) docker     (123)    51683 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.513399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/user_instance_profile/
--rw-r--r--   0 runner    (1001) docker     (123)    20384 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/user_instance_profile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.513399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/user_role/
--rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/user_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.513399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/volume/
--rw-r--r--   0 runner    (1001) docker     (123)    30714 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/volume/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.513399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/workspace_conf/
--rw-r--r--   0 runner    (1001) docker     (123)    18601 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/workspace_conf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.513399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/workspace_file/
--rw-r--r--   0 runner    (1001) docker     (123)    27029 2023-06-15 03:18:27.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/workspace_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:18:41.477399 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-06-15 03:18:41.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-06-15 03:18:41.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 03:18:41.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 03:18:41.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 03:18:41.000000 cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.734825 cdktf-cdktf-provider-databricks-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-06-15 11:24:59.734825 cdktf-cdktf-provider-databricks-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:24:59.734825 cdktf-cdktf-provider-databricks-8.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.682825 cdktf-cdktf-provider-databricks-8.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.698825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.698825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1486562 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/_jsii/provider-databricks@8.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.702825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/aws_s3_mount/
+-rw-r--r--   0 runner    (1001) docker     (123)    25103 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/aws_s3_mount/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.702825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/azure_adls_gen1_mount/
+-rw-r--r--   0 runner    (1001) docker     (123)    37192 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/azure_adls_gen1_mount/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.702825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/azure_adls_gen2_mount/
+-rw-r--r--   0 runner    (1001) docker     (123)    39923 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/azure_adls_gen2_mount/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.702825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/azure_blob_mount/
+-rw-r--r--   0 runner    (1001) docker     (123)    34286 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/azure_blob_mount/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.702825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    39684 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.702825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)   374730 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.702825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/cluster_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    31179 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/cluster_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.702825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_aws_assume_role_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_aws_assume_role_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.706825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_aws_bucket_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    26627 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_aws_bucket_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.706825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_aws_crossaccount_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    18946 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_aws_crossaccount_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.706825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)    18139 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_catalogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.706825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)   405001 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.706825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_cluster_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    34768 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_cluster_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.706825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_clusters/
+-rw-r--r--   0 runner    (1001) docker     (123)    18782 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_clusters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.706825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_current_user/
+-rw-r--r--   0 runner    (1001) docker     (123)    16942 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_current_user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.706825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file/
+-rw-r--r--   0 runner    (1001) docker     (123)    21011 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.706825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file_paths/
+-rw-r--r--   0 runner    (1001) docker     (123)    30164 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file_paths/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.706825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_directory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.706825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_group/
+-rw-r--r--   0 runner    (1001) docker     (123)    52152 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.706825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_instance_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)   214292 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_instance_pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.710825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_job/
+-rw-r--r--   0 runner    (1001) docker     (123)  1628066 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_job/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.710825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)    18211 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_jobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.710825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_mws_credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)    18514 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_mws_credentials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.710825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_mws_workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_mws_workspaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.710825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_node_type/
+-rw-r--r--   0 runner    (1001) docker     (123)    52603 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_node_type/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.710825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)    27043 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_notebook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.710825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_notebook_paths/
+-rw-r--r--   0 runner    (1001) docker     (123)    30333 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_notebook_paths/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.710825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.714825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    20311 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.714825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_service_principal/
+-rw-r--r--   0 runner    (1001) docker     (123)    33251 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_service_principal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.714825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_service_principals/
+-rw-r--r--   0 runner    (1001) docker     (123)    21674 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_service_principals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.714825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_share/
+-rw-r--r--   0 runner    (1001) docker     (123)    91706 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_share/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.714825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_shares/
+-rw-r--r--   0 runner    (1001) docker     (123)    18189 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_shares/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.714825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_spark_version/
+-rw-r--r--   0 runner    (1001) docker     (123)    43822 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_spark_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.714825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouse/
+-rw-r--r--   0 runner    (1001) docker     (123)    98211 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.714825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouses/
+-rw-r--r--   0 runner    (1001) docker     (123)    21182 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.714825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)    22429 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.714825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_user/
+-rw-r--r--   0 runner    (1001) docker     (123)    21375 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.714825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_views/
+-rw-r--r--   0 runner    (1001) docker     (123)    22388 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.714825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_zones/
+-rw-r--r--   0 runner    (1001) docker     (123)    16121 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_zones/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.714825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/dbfs_file/
+-rw-r--r--   0 runner    (1001) docker     (123)    24655 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/dbfs_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.714825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/directory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.714825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/entitlements/
+-rw-r--r--   0 runner    (1001) docker     (123)    36323 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/entitlements/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.714825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/external_location/
+-rw-r--r--   0 runner    (1001) docker     (123)    38113 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/external_location/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.714825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/git_credential/
+-rw-r--r--   0 runner    (1001) docker     (123)    25909 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/git_credential/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.718825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/global_init_script/
+-rw-r--r--   0 runner    (1001) docker     (123)    35510 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/global_init_script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.718825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/grants/
+-rw-r--r--   0 runner    (1001) docker     (123)    55461 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/grants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.718825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/group/
+-rw-r--r--   0 runner    (1001) docker     (123)    38035 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.718825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/group_instance_profile/
+-rw-r--r--   0 runner    (1001) docker     (123)    20452 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/group_instance_profile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.718825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/group_member/
+-rw-r--r--   0 runner    (1001) docker     (123)    19797 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/group_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.718825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/group_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    19568 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/group_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.718825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/instance_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)   171446 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/instance_pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.718825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/instance_profile/
+-rw-r--r--   0 runner    (1001) docker     (123)    27316 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/instance_profile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.718825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/ip_access_list/
+-rw-r--r--   0 runner    (1001) docker     (123)    24956 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/ip_access_list/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.718825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/job/
+-rw-r--r--   0 runner    (1001) docker     (123)  1504922 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/job/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.722825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/library/
+-rw-r--r--   0 runner    (1001) docker     (123)    54504 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.722825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/metastore/
+-rw-r--r--   0 runner    (1001) docker     (123)    53817 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/metastore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.722825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/metastore_assignment/
+-rw-r--r--   0 runner    (1001) docker     (123)    23058 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/metastore_assignment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.722825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/metastore_data_access/
+-rw-r--r--   0 runner    (1001) docker     (123)    79505 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/metastore_data_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.722825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mlflow_experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)    38578 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mlflow_experiment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.722825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mlflow_model/
+-rw-r--r--   0 runner    (1001) docker     (123)    47009 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mlflow_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.722825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mlflow_webhook/
+-rw-r--r--   0 runner    (1001) docker     (123)    53025 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mlflow_webhook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.722825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/model_serving/
+-rw-r--r--   0 runner    (1001) docker     (123)    81786 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/model_serving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.722825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mount/
+-rw-r--r--   0 runner    (1001) docker     (123)   121729 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mount/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.722825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)    22803 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_credentials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.722825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_customer_managed_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)    46981 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_customer_managed_keys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.722825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_log_delivery/
+-rw-r--r--   0 runner    (1001) docker     (123)    42349 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_log_delivery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.722825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_networks/
+-rw-r--r--   0 runner    (1001) docker     (123)    85166 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.722825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_permission_assignment/
+-rw-r--r--   0 runner    (1001) docker     (123)    22828 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_permission_assignment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.726825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_private_access_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)    37950 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_private_access_settings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.726825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_storage_configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)    23504 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_storage_configurations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.726825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_vpc_endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)    56430 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_vpc_endpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.726825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)   148773 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_workspaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.726825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)    33598 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/notebook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.726825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/obo_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    22810 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/obo_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.726825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/permission_assignment/
+-rw-r--r--   0 runner    (1001) docker     (123)    20476 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/permission_assignment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.726825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)    92218 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/permissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.726825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)   340923 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.726825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    75645 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.726825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/provider_resource/
+-rw-r--r--   0 runner    (1001) docker     (123)    24759 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/provider_resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.726825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/recipient/
+-rw-r--r--   0 runner    (1001) docker     (123)    64516 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/recipient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.726825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)    36402 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/repo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.726825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)    34497 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.730825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)    21865 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.730825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/secret_acl/
+-rw-r--r--   0 runner    (1001) docker     (123)    21743 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/secret_acl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.730825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/secret_scope/
+-rw-r--r--   0 runner    (1001) docker     (123)    33202 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/secret_scope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.730825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/service_principal/
+-rw-r--r--   0 runner    (1001) docker     (123)    53372 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/service_principal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.730825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/service_principal_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    20359 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/service_principal_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.730825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/service_principal_secret/
+-rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/service_principal_secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.730825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/share/
+-rw-r--r--   0 runner    (1001) docker     (123)    89048 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/share/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.730825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_alert/
+-rw-r--r--   0 runner    (1001) docker     (123)    42260 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_alert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.730825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)    22195 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.730825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)   105173 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_endpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.730825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_global_config/
+-rw-r--r--   0 runner    (1001) docker     (123)    30740 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_global_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.730825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)    52298 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_permissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.730825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_query/
+-rw-r--r--   0 runner    (1001) docker     (123)   223497 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_query/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.734825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_table/
+-rw-r--r--   0 runner    (1001) docker     (123)    62781 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.734825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)    31228 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.734825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_widget/
+-rw-r--r--   0 runner    (1001) docker     (123)    70645 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_widget/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.734825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/storage_credential/
+-rw-r--r--   0 runner    (1001) docker     (123)    80952 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/storage_credential/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.734825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/table/
+-rw-r--r--   0 runner    (1001) docker     (123)    75587 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.734825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/token/
+-rw-r--r--   0 runner    (1001) docker     (123)    27481 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.734825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    51683 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.734825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/user_instance_profile/
+-rw-r--r--   0 runner    (1001) docker     (123)    20384 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/user_instance_profile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.734825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/user_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/user_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.734825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/volume/
+-rw-r--r--   0 runner    (1001) docker     (123)    30714 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/volume/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.734825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/workspace_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)    18601 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/workspace_conf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.734825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/workspace_file/
+-rw-r--r--   0 runner    (1001) docker     (123)    27029 2023-06-15 11:24:43.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/workspace_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:24:59.698825 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-06-15 11:24:59.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-06-15 11:24:59.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:24:59.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 11:24:59.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 11:24:59.000000 cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/LICENSE` & `cdktf-cdktf-provider-databricks-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/PKG-INFO` & `cdktf-cdktf-provider-databricks-8.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-databricks
-Version: 7.0.7
+Version: 8.0.0
 Summary: Prebuilt databricks Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-databricks.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-databricks.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/README.md` & `cdktf-cdktf-provider-databricks-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/setup.py` & `cdktf-cdktf-provider-databricks-8.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-databricks",
-    "version": "7.0.7",
+    "version": "8.0.0",
     "description": "Prebuilt databricks Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-databricks.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -130,23 +130,23 @@
         "cdktf_cdktf_provider_databricks.user_role",
         "cdktf_cdktf_provider_databricks.volume",
         "cdktf_cdktf_provider_databricks.workspace_conf",
         "cdktf_cdktf_provider_databricks.workspace_file"
     ],
     "package_data": {
         "cdktf_cdktf_provider_databricks._jsii": [
-            "provider-databricks@7.0.7.jsii.tgz"
+            "provider-databricks@8.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_databricks": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdktf>=0.16.3, <0.17.0",
+        "cdktf>=0.17.0, <0.18.0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.84.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/aws_s3_mount/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/aws_s3_mount/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/azure_adls_gen1_mount/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/azure_adls_gen1_mount/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/azure_adls_gen2_mount/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/azure_adls_gen2_mount/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/azure_blob_mount/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/azure_blob_mount/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/catalog/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/cluster/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/cluster_policy/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/cluster_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_aws_assume_role_policy/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_aws_assume_role_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_aws_bucket_policy/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_aws_bucket_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_aws_crossaccount_policy/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_aws_crossaccount_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_catalogs/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_catalogs/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_cluster/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_cluster_policy/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_cluster_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_clusters/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_clusters/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_current_user/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_current_user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file_paths/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_dbfs_file_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_directory/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_directory/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_group/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_instance_pool/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_instance_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_job/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_job/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_jobs/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_mws_credentials/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_mws_credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_mws_workspaces/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_mws_workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_node_type/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_node_type/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_notebook/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_notebook_paths/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_notebook_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_pipelines/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_schemas/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_service_principal/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_service_principal/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_service_principals/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_service_principals/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_share/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_share/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_shares/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_shares/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_spark_version/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_spark_version/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouse/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouse/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouses/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_sql_warehouses/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_tables/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_user/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_views/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_views/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/data_databricks_zones/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/data_databricks_zones/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/dbfs_file/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/dbfs_file/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/directory/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/entitlements/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/entitlements/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/external_location/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/external_location/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/git_credential/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/git_credential/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/global_init_script/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/global_init_script/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/grants/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/grants/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/group/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/group_instance_profile/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/group_instance_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/group_member/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/group_member/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/group_role/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/group_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/instance_pool/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/instance_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/instance_profile/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/instance_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/ip_access_list/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/ip_access_list/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/job/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/job/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/library/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/library/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/metastore/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/metastore/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/metastore_assignment/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/metastore_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/metastore_data_access/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/metastore_data_access/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mlflow_experiment/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mlflow_experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mlflow_model/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mlflow_model/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mlflow_webhook/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mlflow_webhook/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/model_serving/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/model_serving/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mount/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mount/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_credentials/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_customer_managed_keys/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_customer_managed_keys/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_log_delivery/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_log_delivery/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_networks/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_networks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_permission_assignment/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_permission_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_private_access_settings/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_private_access_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_storage_configurations/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_storage_configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_vpc_endpoint/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_vpc_endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/mws_workspaces/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/mws_workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/notebook/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/obo_token/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/obo_token/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/permission_assignment/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/permission_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/permissions/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/pipeline/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/provider/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/provider_resource/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/provider_resource/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/recipient/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/recipient/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/repo/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/schema/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/secret/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/secret_acl/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/secret_acl/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/secret_scope/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/secret_scope/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/service_principal/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/service_principal/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/service_principal_role/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/service_principal_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/service_principal_secret/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/service_principal_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/share/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/share/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_alert/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_alert/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_dashboard/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_endpoint/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_global_config/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_global_config/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_permissions/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_query/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_query/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_table/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_table/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_visualization/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/sql_widget/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/sql_widget/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/storage_credential/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/storage_credential/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/table/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/table/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/token/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/token/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/user/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/user_instance_profile/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/user_instance_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/user_role/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/user_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/volume/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/workspace_conf/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/workspace_conf/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks/workspace_file/__init__.py` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks/workspace_file/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks.egg-info/PKG-INFO` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-databricks
-Version: 7.0.7
+Version: 8.0.0
 Summary: Prebuilt databricks Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-databricks.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-databricks.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-databricks-7.0.7/src/cdktf_cdktf_provider_databricks.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-databricks-8.0.0/src/cdktf_cdktf_provider_databricks.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_databricks/py.typed
 src/cdktf_cdktf_provider_databricks.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_databricks.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_databricks.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_databricks.egg-info/requires.txt
 src/cdktf_cdktf_provider_databricks.egg-info/top_level.txt
 src/cdktf_cdktf_provider_databricks/_jsii/__init__.py
-src/cdktf_cdktf_provider_databricks/_jsii/provider-databricks@7.0.7.jsii.tgz
+src/cdktf_cdktf_provider_databricks/_jsii/provider-databricks@8.0.0.jsii.tgz
 src/cdktf_cdktf_provider_databricks/aws_s3_mount/__init__.py
 src/cdktf_cdktf_provider_databricks/azure_adls_gen1_mount/__init__.py
 src/cdktf_cdktf_provider_databricks/azure_adls_gen2_mount/__init__.py
 src/cdktf_cdktf_provider_databricks/azure_blob_mount/__init__.py
 src/cdktf_cdktf_provider_databricks/catalog/__init__.py
 src/cdktf_cdktf_provider_databricks/cluster/__init__.py
 src/cdktf_cdktf_provider_databricks/cluster_policy/__init__.py
```

