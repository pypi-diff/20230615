# Comparing `tmp/cdktf-cdktf-provider-docker-7.0.1.tar.gz` & `tmp/cdktf-cdktf-provider-docker-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-docker-7.0.1.tar", last modified: Thu Jun  1 14:14:21 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-docker-8.0.0.tar", last modified: Thu Jun 15 11:21:25 2023, max compression
```

## Comparing `cdktf-cdktf-provider-docker-7.0.1.tar` & `cdktf-cdktf-provider-docker-8.0.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:21.265517 cdktf-cdktf-provider-docker-7.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-01 14:14:21.261517 cdktf-cdktf-provider-docker-7.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:14:21.265517 cdktf-cdktf-provider-docker-7.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:21.257517 cdktf-cdktf-provider-docker-7.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:21.257517 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:21.261517 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   306535 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/_jsii/provider-docker@7.0.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:21.261517 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/config/
--rw-r--r--   0 runner    (1001) docker     (123)    19489 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:21.261517 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/container/
--rw-r--r--   0 runner    (1001) docker     (123)   436603 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/container/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:21.261517 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/data_docker_image/
--rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/data_docker_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:21.261517 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/data_docker_logs/
--rw-r--r--   0 runner    (1001) docker     (123)    45717 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/data_docker_logs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:21.261517 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/data_docker_network/
--rw-r--r--   0 runner    (1001) docker     (123)    25165 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/data_docker_network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:21.261517 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/data_docker_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)    19415 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/data_docker_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:21.261517 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/data_docker_registry_image/
--rw-r--r--   0 runner    (1001) docker     (123)    21915 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/data_docker_registry_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:21.261517 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/image/
--rw-r--r--   0 runner    (1001) docker     (123)   169468 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:21.261517 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/network/
--rw-r--r--   0 runner    (1001) docker     (123)    83412 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:21.261517 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)    55351 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:21.261517 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    32727 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:21.261517 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/registry_image/
--rw-r--r--   0 runner    (1001) docker     (123)    28322 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/registry_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:21.261517 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/secret/
--rw-r--r--   0 runner    (1001) docker     (123)    36158 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:21.261517 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/service/
--rw-r--r--   0 runner    (1001) docker     (123)   541834 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:21.261517 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/tag/
--rw-r--r--   0 runner    (1001) docker     (123)    20035 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/tag/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:21.261517 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/volume/
--rw-r--r--   0 runner    (1001) docker     (123)    39885 2023-06-01 14:14:09.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/volume/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:21.257517 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-01 14:14:21.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-01 14:14:21.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:14:21.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:14:21.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-01 14:14:21.000000 cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:21:25.202300 cdktf-cdktf-provider-docker-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-15 11:21:25.202300 cdktf-cdktf-provider-docker-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:21:25.202300 cdktf-cdktf-provider-docker-8.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:21:25.194300 cdktf-cdktf-provider-docker-8.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:21:25.198300 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:21:25.198300 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   306536 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/_jsii/provider-docker@8.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:21:25.198300 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    19489 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:21:25.198300 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/container/
+-rw-r--r--   0 runner    (1001) docker     (123)   436603 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/container/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:21:25.198300 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/data_docker_image/
+-rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/data_docker_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:21:25.198300 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/data_docker_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)    45717 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/data_docker_logs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:21:25.198300 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/data_docker_network/
+-rw-r--r--   0 runner    (1001) docker     (123)    25165 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/data_docker_network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:21:25.198300 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/data_docker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)    19415 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/data_docker_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:21:25.198300 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/data_docker_registry_image/
+-rw-r--r--   0 runner    (1001) docker     (123)    21915 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/data_docker_registry_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:21:25.202300 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/image/
+-rw-r--r--   0 runner    (1001) docker     (123)   169468 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:21:25.202300 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/network/
+-rw-r--r--   0 runner    (1001) docker     (123)    83412 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:21:25.202300 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)    55351 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:21:25.202300 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    32727 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:21:25.202300 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/registry_image/
+-rw-r--r--   0 runner    (1001) docker     (123)    28322 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/registry_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:21:25.202300 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)    36158 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:21:25.202300 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/service/
+-rw-r--r--   0 runner    (1001) docker     (123)   541834 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:21:25.202300 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/tag/
+-rw-r--r--   0 runner    (1001) docker     (123)    20035 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/tag/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:21:25.202300 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/volume/
+-rw-r--r--   0 runner    (1001) docker     (123)    39885 2023-06-15 11:20:59.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/volume/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:21:25.198300 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-15 11:21:25.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-15 11:21:25.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:21:25.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 11:21:25.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 11:21:25.000000 cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-docker-7.0.1/LICENSE` & `cdktf-cdktf-provider-docker-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-docker-7.0.1/PKG-INFO` & `cdktf-cdktf-provider-docker-8.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-docker
-Version: 7.0.1
+Version: 8.0.0
 Summary: Prebuilt docker Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-docker.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-docker.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-docker-7.0.1/README.md` & `cdktf-cdktf-provider-docker-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-docker-7.0.1/setup.py` & `cdktf-cdktf-provider-docker-8.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-docker",
-    "version": "7.0.1",
+    "version": "8.0.0",
     "description": "Prebuilt docker Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-docker.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -38,25 +38,25 @@
         "cdktf_cdktf_provider_docker.secret",
         "cdktf_cdktf_provider_docker.service",
         "cdktf_cdktf_provider_docker.tag",
         "cdktf_cdktf_provider_docker.volume"
     ],
     "package_data": {
         "cdktf_cdktf_provider_docker._jsii": [
-            "provider-docker@7.0.1.jsii.tgz"
+            "provider-docker@8.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_docker": [
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

### Comparing `cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/__init__.py` & `cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/config/__init__.py` & `cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/container/__init__.py` & `cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/container/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/data_docker_image/__init__.py` & `cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/data_docker_image/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/data_docker_logs/__init__.py` & `cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/data_docker_logs/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/data_docker_network/__init__.py` & `cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/data_docker_network/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/data_docker_plugin/__init__.py` & `cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/data_docker_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/data_docker_registry_image/__init__.py` & `cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/data_docker_registry_image/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/image/__init__.py` & `cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/image/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/network/__init__.py` & `cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/network/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/plugin/__init__.py` & `cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/provider/__init__.py` & `cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/registry_image/__init__.py` & `cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/registry_image/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/secret/__init__.py` & `cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/service/__init__.py` & `cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/service/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/tag/__init__.py` & `cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/tag/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker/volume/__init__.py` & `cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker.egg-info/PKG-INFO` & `cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-docker
-Version: 7.0.1
+Version: 8.0.0
 Summary: Prebuilt docker Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-docker.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-docker.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-docker-7.0.1/src/cdktf_cdktf_provider_docker.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-docker-8.0.0/src/cdktf_cdktf_provider_docker.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_docker/py.typed
 src/cdktf_cdktf_provider_docker.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_docker.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_docker.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_docker.egg-info/requires.txt
 src/cdktf_cdktf_provider_docker.egg-info/top_level.txt
 src/cdktf_cdktf_provider_docker/_jsii/__init__.py
-src/cdktf_cdktf_provider_docker/_jsii/provider-docker@7.0.1.jsii.tgz
+src/cdktf_cdktf_provider_docker/_jsii/provider-docker@8.0.0.jsii.tgz
 src/cdktf_cdktf_provider_docker/config/__init__.py
 src/cdktf_cdktf_provider_docker/container/__init__.py
 src/cdktf_cdktf_provider_docker/data_docker_image/__init__.py
 src/cdktf_cdktf_provider_docker/data_docker_logs/__init__.py
 src/cdktf_cdktf_provider_docker/data_docker_network/__init__.py
 src/cdktf_cdktf_provider_docker/data_docker_plugin/__init__.py
 src/cdktf_cdktf_provider_docker/data_docker_registry_image/__init__.py
```

