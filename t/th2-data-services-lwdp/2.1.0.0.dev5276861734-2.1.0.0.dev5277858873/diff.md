# Comparing `tmp/th2_data_services_lwdp-2.1.0.0.dev5276861734.tar.gz` & `tmp/th2_data_services_lwdp-2.1.0.0.dev5277858873.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services_lwdp-2.1.0.0.dev5276861734.tar", last modified: Thu Jun 15 09:04:12 2023, max compression
+gzip compressed data, was "dist/th2_data_services_lwdp-2.1.0.0.dev5277858873.tar", last modified: Thu Jun 15 10:48:57 2023, max compression
```

## Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734.tar` & `th2_data_services_lwdp-2.1.0.0.dev5277858873.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:04:12.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-15 09:04:12.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-15 09:03:56.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-15 09:04:12.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:04:12.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:04:12.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:04:12.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:04:12.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/adapters/
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/adapters/event_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/adapters/message_adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:04:12.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/commands/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    57286 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/commands/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:04:12.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/data_source/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/data_source/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/data_source/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:04:12.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:04:12.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/filters/event_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:04:12.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/interfaces/filter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/message_response_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     3894 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/page.py
--rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:04:12.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/source_api/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/source_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/source_api/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    14514 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/source_api/http.py
--rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/streams.py
--rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:04:12.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/utils/_misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/utils/_response_formats.py
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-06-15 09:03:07.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/utils/json.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 09:04:12.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services_lwdp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-15 09:04:12.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services_lwdp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-06-15 09:04:12.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services_lwdp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 09:04:12.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services_lwdp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-15 09:04:12.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services_lwdp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-15 09:04:12.000000 th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services_lwdp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:48:57.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-15 10:48:57.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-15 10:48:32.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-15 10:48:57.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:48:57.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:48:57.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:48:57.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:48:57.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/adapters/event_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/adapters/message_adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:48:57.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/commands/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57298 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/commands/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:48:57.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/data_source/
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/data_source/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/data_source/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:48:57.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:48:57.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/filters/event_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/filters/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:48:57.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/interfaces/filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/message_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3894 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/page.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:48:57.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/source_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/source_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/source_api/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14514 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/source_api/http.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/streams.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:48:57.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/utils/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/utils/_response_formats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-06-15 10:47:33.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/utils/json.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:48:57.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services_lwdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-15 10:48:56.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services_lwdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-06-15 10:48:57.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services_lwdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 10:48:56.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services_lwdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-15 10:48:56.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services_lwdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-15 10:48:56.000000 th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services_lwdp.egg-info/top_level.txt
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/PKG-INFO` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_data_services_lwdp
-Version: 2.1.0.0.dev5276861734
+Version: 2.1.0.0.dev5277858873
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/README.md` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/setup.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/adapters/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/adapters/adapter_sse.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/adapters/adapter_sse.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/adapters/basic_adapters.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/adapters/basic_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/adapters/event_adapters.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/adapters/event_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/adapters/message_adapters.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/adapters/message_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/commands/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/commands/grpc.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/commands/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/commands/http.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/commands/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -1191,29 +1191,29 @@
             get_utc_datetime_now()
             if page.end_timestamp is None
             else ProtobufTimestampConverter.to_nanoseconds(page.end_timestamp)
         )
         self._book_id = page.book
         api = data_source.source_api
         urls = api.get_download_messages(
-            start_timestamp=self._start_timestamp,
+            start_timestamp=self._start_timestamp,  
             end_timestamp=self._end_timestamp,
             book_id=self._book_id,
             groups=self._groups,
             sort=self._sort,
             response_formats=self._response_formats,
             keep_open=self._keep_open,
             max_url_length=self._max_url_length,
         )
         headers = {
             'Accept': 'application/stream+json',
             'Accept-Encoding': 'gzip, deflate'
         }
         if len(urls) == 1:
-            with open(self._filename, 'wb') as file:
+            with open(f"{self._filename}.gzip", 'wb') as file:
                 response = api.execute_request(urls[0], headers=headers, stream=True)
                 copyfileobj(response.raw, file)
         else:
             for num, url in enumerate(urls):
                 with open(f"{self._filename}.{num+1}.gzip", 'wb') as file:
                     response = api.execute_request(url, headers=headers, stream=True)
                     copyfileobj(response.raw, file)
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/data_source/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/data_source/grpc.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/data_source/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/data_source/http.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/data_source/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/event_tree/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/filters/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/filters/event_filters.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/filters/event_filters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/filters/filter.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/filters/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/interfaces/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/interfaces/command.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/interfaces/data_source.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/interfaces/filter.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/interfaces/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/interfaces/source_api.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/message_response_format.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/message_response_format.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/page.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/page.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/resolver.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/source_api/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/source_api/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/source_api/grpc.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/source_api/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/source_api/http.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/source_api/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/streams.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/streams.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/struct.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/stub_builder.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/utils/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/utils/_misc.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/utils/_response_formats.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/utils/_response_formats.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services/data_source/lwdp/utils/json.py` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services/data_source/lwdp/utils/json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services_lwdp.egg-info/PKG-INFO` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services_lwdp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-data-services-lwdp
-Version: 2.1.0.0.dev5276861734
+Version: 2.1.0.0.dev5277858873
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5276861734/th2_data_services_lwdp.egg-info/SOURCES.txt` & `th2_data_services_lwdp-2.1.0.0.dev5277858873/th2_data_services_lwdp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

