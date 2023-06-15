# Comparing `tmp/metaflow-netflixext-0.2.1.tar.gz` & `tmp/metaflow-netflixext-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow-netflixext-0.2.1.tar", last modified: Tue Jun 13 17:44:56 2023, max compression
+gzip compressed data, was "metaflow-netflixext-0.2.2.tar", last modified: Thu Jun 15 21:17:42 2023, max compression
```

## Comparing `metaflow-netflixext-0.2.1.tar` & `metaflow-netflixext-0.2.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.829685 metaflow-netflixext-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-06-13 17:44:56.829685 metaflow-netflixext-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26486 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.821685 metaflow-netflixext-0.2.1/metaflow_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.825685 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.825685 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/cmd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.825685 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/cmd/environment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/cmd/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35523 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/cmd/environment/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/cmd/mfextinit_netflixext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.825685 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/generate_vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.825685 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.825685 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   181679 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     9779 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    40641 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    50296 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py
--rw-r--r--   0 runner    (1001) docker     (123)    37869 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.825685 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg
--rw-r--r--   0 runner    (1001) docker     (123)   113678 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    20557 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20971 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/environment_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/mfextinit_netflixext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.825685 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/toplevel/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/toplevel/mfextinit_netflixext.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/toplevel/netflixext_toplevel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.821685 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.825685 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)    39124 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.829685 metaflow-netflixext-0.2.1/metaflow_netflixext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-06-13 17:44:56.000000 metaflow-netflixext-0.2.1/metaflow_netflixext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-13 17:44:56.000000 metaflow-netflixext-0.2.1/metaflow_netflixext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:44:56.000000 metaflow-netflixext-0.2.1/metaflow_netflixext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 17:44:56.000000 metaflow-netflixext-0.2.1/metaflow_netflixext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-13 17:44:56.000000 metaflow-netflixext-0.2.1/metaflow_netflixext.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 17:44:56.829685 metaflow-netflixext-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.669591 metaflow-netflixext-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-06-15 21:17:42.669591 metaflow-netflixext-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26486 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.665591 metaflow-netflixext-0.2.2/metaflow_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.665591 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.665591 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/cmd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.665591 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/cmd/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/cmd/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35592 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/cmd/environment/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/cmd/mfextinit_netflixext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.665591 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/generate_vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.669591 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.669591 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182021 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50529 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37939 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.669591 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   113678 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21000 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20971 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/environment_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/mfextinit_netflixext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.669591 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/toplevel/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/toplevel/mfextinit_netflixext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/toplevel/netflixext_toplevel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.665591 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.669591 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39124 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:17:42.669591 metaflow-netflixext-0.2.2/metaflow_netflixext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-06-15 21:17:42.000000 metaflow-netflixext-0.2.2/metaflow_netflixext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-15 21:17:42.000000 metaflow-netflixext-0.2.2/metaflow_netflixext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:17:42.000000 metaflow-netflixext-0.2.2/metaflow_netflixext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 21:17:42.000000 metaflow-netflixext-0.2.2/metaflow_netflixext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 21:17:42.000000 metaflow-netflixext-0.2.2/metaflow_netflixext.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 21:17:42.669591 metaflow-netflixext-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-15 21:17:33.000000 metaflow-netflixext-0.2.2/setup.py
```

### Comparing `metaflow-netflixext-0.2.1/LICENSE` & `metaflow-netflixext-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/PKG-INFO` & `metaflow-netflixext-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-netflixext
-Version: 0.2.1
+Version: 0.2.2
 Summary: EXPERIMENTAL Metaflow extensions from Netflix
 Author: Netflix Metaflow Developers
 Author-email: metaflow-dev@netflix.com
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow-nflx-extensions
 Project-URL: Tracker, https://github.com/Netflix/metaflow-nflx-extensions/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `metaflow-netflixext-0.2.1/README.md` & `metaflow-netflixext-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     ResolvedEnvironment,
     TStr,
 )
 from metaflow_extensions.netflix_ext.plugins.conda.envsresolver import EnvsResolver
 from metaflow_extensions.netflix_ext.plugins.conda.utils import (
     AliasType,
     arch_id,
+    conda_deps_to_pip_deps,
     resolve_env_alias,
     plural_marker,
     merge_dep_dicts,
 )
 
 from metaflow_extensions.netflix_ext.vendor.packaging.requirements import (
     InvalidRequirement,
@@ -577,15 +578,18 @@
         base_env_python = platform.python_version()
 
     # Compute the deps
     if len(new_conda_deps) == 0 and (
         not base_env or base_env.env_type == EnvType.PIP_ONLY
     ):
         # Assume a pip environment for base deps
-        pip_deps = dict(get_pinned_conda_libs(base_env_python, obj.datastore_type))
+        pip_deps = conda_deps_to_pip_deps(
+            get_pinned_conda_libs(base_env_python, obj.datastore_type)
+        )
+
         conda_deps = {}
     else:
         conda_deps = dict(get_pinned_conda_libs(base_env_python, obj.datastore_type))
         pip_deps = {}
 
     pip_deps = merge_dep_dicts(pip_deps, new_pip_deps)
     conda_deps = merge_dep_dicts(conda_deps, new_conda_deps)
```

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/cmd/environment/utils.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/cmd/environment/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/generate_vendor.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/generate_vendor.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/conda.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/conda.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,14 +375,16 @@
                             % ", ".join([d.value for d in npconda_deps])
                         )
                 if resolver_bin == "pip":
                     packages, returned_builder_env = self._resolve_env_with_pip(
                         deps, sources, extras, architecture, builder_env, base_env
                     )
                     assert returned_builder_env
+                    # packages contains only pip packages so the order between the
+                    # two does not really matter
                     packages += list(returned_builder_env.packages)
                 else:
                     # Should also never happen and be caught earlier but being clean
                     # add other pip resolvers here if needed
                     raise InvalidEnvironmentException(
                         "Resolver '%s' is not supported" % resolver_bin
                     )
@@ -3248,14 +3250,18 @@
             stat.S_IRUSR
             | stat.S_IXUSR
             | stat.S_IRGRP
             | stat.S_IXGRP
             | stat.S_IROTH
             | stat.S_IXOTH,
         )
+        # In some cases, we were seeing text file busy errors. This will hopefully
+        # force everything to be written out (including the chmod above) before we need
+        # to use it.
+        os.sync()
         self._bins = {"conda": final_path, "micromamba": final_path}
         self._conda_executable_type = "micromamba"
 
     def _validate_conda_installation(self) -> Optional[Exception]:
         # If this is installed in CONDA_LOCAL_PATH look for special marker
         if self._mode == "local" and CONDA_LOCAL_PATH is not None:
             if not os.path.isfile(
```

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py`

 * *Files 3% similar despite different names*

```diff
@@ -197,20 +197,20 @@
 
     def pylint_config(self) -> List[str]:
         config = self.base_env.pylint_config()
         # Disable (import-error) in pylint
         config.append("--disable=F0401")
         return config
 
-    def executable(self, step_name: str) -> str:
+    def executable(self, step_name: str, default: Optional[str] = None) -> str:
         # Get relevant python interpreter for step
         executable = self._get_executable(step_name)
         if executable is not None:
             return executable
-        return self.base_env.executable(step_name)
+        return self.base_env.executable(step_name, default)
 
     @classmethod
     def get_client_info(
         cls, flow_name: str, metadata: Dict[str, str]
     ) -> Dict[str, Any]:
         # TODO: FIX THIS: this doesn't work with the new format.
         if cls._filecache is None:
@@ -235,15 +235,20 @@
         resolved_env = cached_env_info.env_for(env_id[0], env_id[1])
         if resolved_env:
             new_info = {
                 "type": "conda",
                 "req_id": env_id[0],
                 "full_id": env_id[1],
                 "user_deps": "; ".join(map(str, resolved_env.deps)),
-                "all_packages": "; ".join([p.filename for p in resolved_env.packages]),
+                "all_packages": "; ".join(
+                    [
+                        p.filename
+                        for p in sorted(resolved_env.packages, key=lambda p: p.filename)
+                    ]
+                ),
             }
             return new_info
         return {"type": "conda"}
 
     def get_package_commands(self, code_package_url: str, datastore_type: str):
         return self.base_env.get_package_commands(code_package_url, datastore_type)
```

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 )
 from metaflow.plugins.env_escape import generate_trampolines
 from metaflow.unbounded_foreach import UBF_CONTROL, UBF_TASK
 from metaflow.util import get_metaflow_root
 
 from metaflow_extensions.netflix_ext.vendor.packaging.utils import canonicalize_version
 
-from .utils import arch_id, merge_dep_dicts
+from .utils import arch_id, conda_deps_to_pip_deps, merge_dep_dicts
 from .conda import Conda
 
 
 class CondaStepDecorator(StepDecorator):
     """
     Specifies the Conda environment for the step.
 
@@ -671,15 +671,15 @@
             seen.add(c)
             result.append(c)
         return result
 
     def _pip_deps(self) -> Dict[str, str]:
         deps = {}  # type: Dict[str, str]
         if self.from_env and self.from_env == EnvType.PIP_ONLY:
-            deps = dict(
+            deps = conda_deps_to_pip_deps(
                 get_pinned_conda_libs(self._python_version(), self._flow_datastore_type)
             )
 
         user_deps = dict(self._base_attributes["pip_packages"])
         user_deps.update(self.attributes["pip_packages"])
 
         return merge_dep_dicts(deps, user_deps)
@@ -989,21 +989,21 @@
     def _conda_channels(self) -> List[str]:
         return []
 
     def _pip_deps(self) -> Dict[str, str]:
         deps = {}  # type: Dict[str, str]
         if self.from_env:
             if self.from_env.env_type == EnvType.PIP_ONLY:
-                deps = dict(
+                deps = conda_deps_to_pip_deps(
                     get_pinned_conda_libs(
                         self._python_version(), self._flow_datastore_type
                     )
                 )
         else:
-            deps = dict(
+            deps = conda_deps_to_pip_deps(
                 get_pinned_conda_libs(self._python_version(), self._flow_datastore_type)
             )
 
         user_deps = dict(self._base_attributes["packages"])
         user_deps.update(self.attributes["packages"])
 
         return merge_dep_dicts(deps, user_deps)
```

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py`

 * *Files 1% similar despite different names*

```diff
@@ -678,19 +678,19 @@
         resolved_by: Optional[str] = None,
         co_resolved: Optional[List[str]] = None,
         env_type: EnvType = EnvType.MIXED,
         accurate_source: bool = True,
     ):
         self._env_type = env_type
         self._user_dependencies = list(user_dependencies)
+        # We sort the user dependencies as the order does not matter and it makes
+        # it easier for users to find their dependencies
+        self._user_dependencies.sort(key=lambda k: k.value)
         self._user_sources = list(user_sources) if user_sources else []
         self._user_extra_args = list(user_extra_args) if user_extra_args else []
-        if all_packages is not None:
-            # It should already be sorted but being very safe
-            all_packages = sorted(all_packages, key=lambda p: p.filename)
 
         self._accurate_source = accurate_source
 
         if not env_id:
             env_req_id = ResolvedEnvironment.get_req_id(
                 self._user_dependencies, self._user_sources, self._user_extra_args
             )
@@ -746,15 +746,18 @@
         envs = sorted(envs, key=lambda x: x.env_id.arch)
         to_hash = []  # type: List[str]
         archs = []  # type: List[str]
         for env in envs:
             archs.append(env.env_id.arch)
             to_hash.append(env.env_id.arch)
             to_hash.extend(
-                ["%s#%s" % (p.filename, p.pkg_hash(p.url_format)) for p in env.packages]
+                [
+                    "%s#%s" % (p.filename, p.pkg_hash(p.url_format))
+                    for p in sorted(env.packages, key=lambda p: p.filename)
+                ]
             )
         new_full_id = ResolvedEnvironment._compute_hash(to_hash)
         for env in envs:
             env.set_coresolved(archs, new_full_id)
 
     @property
     def is_info_accurate(self) -> bool:
@@ -775,27 +778,26 @@
     @property
     def extras(self) -> List[TStr]:
         return self._user_extra_args
 
     @property
     def env_id(self) -> EnvID:
         if self._env_id.full_id in ("_default", "_unresolved") and self._all_packages:
-            self._all_packages.sort(key=lambda p: p.filename)
+            all_packages = sorted(self._all_packages, key=lambda p: p.filename)
             env_full_id = self._compute_hash(
-                [p.filename for p in self._all_packages]
-                + [self._env_id.arch or arch_id()]
+                [p.filename for p in all_packages] + [self._env_id.arch or arch_id()]
             )
             self._env_id = self._env_id._replace(full_id=env_full_id)
         return self._env_id
 
     @property
     def packages(self) -> Iterable[PackageSpecification]:
-        # We always make sure it is sorted and we can do this by checking the env_id
-        # which will sort _all_packages if not sorted
-        _ = self.env_id
+        # This returns the packages in the order in which they were added which
+        # corresponds to the installation order. In some cases, the installation order
+        # matters so we make sure to preserve it.
         for p in self._all_packages:
             yield p
 
     @property
     def resolved_on(self) -> datetime:
         return self._resolved_on
 
@@ -1313,16 +1315,20 @@
 
         return me
 
 
 def read_conda_manifest(ds_root: str) -> CachedEnvironmentInfo:
     path = get_conda_manifest_path(ds_root)
     if os.path.exists(path) and os.path.getsize(path) > 0:
-        with open(path, mode="r", encoding="utf-8") as f:
-            return CachedEnvironmentInfo.from_dict(json.load(f))
+        with os.fdopen(os.open(path, os.O_RDONLY), "r", encoding="utf-8") as f:
+            try:
+                fcntl.flock(f, fcntl.LOCK_SH)
+                return CachedEnvironmentInfo.from_dict(json.load(f))
+            finally:
+                fcntl.flock(f, fcntl.LOCK_UN)
     else:
         return CachedEnvironmentInfo()
 
 
 def write_to_conda_manifest(ds_root: str, info: CachedEnvironmentInfo):
     path = get_conda_manifest_path(ds_root)
     try:
@@ -1343,12 +1349,9 @@
                 # Not a new file
                 f.seek(0)
                 current_content = CachedEnvironmentInfo.from_dict(json.load(f))
             f.seek(0)
             f.truncate(0)
             current_content.update(info)
             json.dump(current_content.to_dict(), f)
-        except IOError as e:
-            if e.errno != errno.EAGAIN:
-                raise
         finally:
             fcntl.flock(f, fcntl.LOCK_UN)
```

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -763,15 +763,17 @@
                     self._requested_envs[orig_env_id]["resolved"] = resolved_env
                     debug.conda_exec(
                         "For environment %s (%s) %s need packages %s"
                         % (
                             resolved_env_id.req_id,
                             resolved_env_id.full_id,
                             self._requested_envs[orig_env_id],
-                            ", ".join([p.filename for p in resolved_env.packages]),
+                            ", ".join(
+                                sorted([p.filename for p in resolved_env.packages])
+                            ),
                         )
                     )
 
         duration = int(time.time() - start)
         echo(" done in %d second%s." % (duration, plural_marker(duration)))
 
     @staticmethod
```

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/utils.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/conda/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -409,14 +409,28 @@
         return all_splits[0], "." + all_splits[1]
     if len(all_splits) == 1:
         return filename_with_ext, ""
     # Should never happen
     return "", ""
 
 
+def conda_deps_to_pip_deps(d: Dict[str, str]) -> Dict[str, str]:
+    # This is a hack for now -- real fix would be to specify get_pinned_pip_libs
+    # but at least for now this allows channels to be specified in the conda_libs
+    # but still work with pip
+    r = {}  # type: Dict[str, str]
+    for k, v in d.items():
+        s = k.split("::")
+        if len(s) > 1:
+            r[s[1]] = v
+        else:
+            r[k] = v
+    return r
+
+
 _UNDERSCORE_REGEX = re.compile(r"[-_.]+")
 
 
 def normalize_to_underscore(name: str) -> str:
     return _UNDERSCORE_REGEX.sub("_", name).lower()
```

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/environment_cli.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/plugins/environment_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/markers.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/tags.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/utils.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/version.py` & `metaflow-netflixext-0.2.2/metaflow_extensions/netflix_ext/vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/metaflow_netflixext.egg-info/PKG-INFO` & `metaflow-netflixext-0.2.2/metaflow_netflixext.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-netflixext
-Version: 0.2.1
+Version: 0.2.2
 Summary: EXPERIMENTAL Metaflow extensions from Netflix
 Author: Netflix Metaflow Developers
 Author-email: metaflow-dev@netflix.com
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow-nflx-extensions
 Project-URL: Tracker, https://github.com/Netflix/metaflow-nflx-extensions/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `metaflow-netflixext-0.2.1/metaflow_netflixext.egg-info/SOURCES.txt` & `metaflow-netflixext-0.2.2/metaflow_netflixext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.1/setup.py` & `metaflow-netflixext-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_namespace_packages
 
-version = "0.2.1"
+version = "0.2.2"
 
 setup(
     name="metaflow-netflixext",
     version=version,
     description="EXPERIMENTAL Metaflow extensions from Netflix",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

