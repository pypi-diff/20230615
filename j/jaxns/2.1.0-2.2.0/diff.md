# Comparing `tmp/jaxns-2.1.0.tar.gz` & `tmp/jaxns-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxns-2.1.0.tar", last modified: Sat Apr 15 13:41:40 2023, max compression
+gzip compressed data, was "jaxns-2.2.0.tar", last modified: Thu Jun 15 14:57:59 2023, max compression
```

## Comparing `jaxns-2.1.0.tar` & `jaxns-2.2.0.tar`

### file list

```diff
@@ -1,58 +1,61 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-04-15 13:41:40.401876 jaxns-2.1.0/
--rw-rw-r--   0 albert    (1000) albert    (1000)    20138 2022-10-13 02:52:05.000000 jaxns-2.1.0/LICENSE
--rw-rw-r--   0 albert    (1000) albert    (1000)     3692 2023-04-15 13:41:40.401876 jaxns-2.1.0/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)     3253 2023-04-15 05:01:38.000000 jaxns-2.1.0/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-04-15 13:41:40.397876 jaxns-2.1.0/jaxns/
--rw-rw-r--   0 albert    (1000) albert    (1000)      344 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    10208 2023-04-14 22:54:16.000000 jaxns-2.1.0/jaxns/adaptive_refinement.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5281 2023-04-15 05:17:24.000000 jaxns-2.1.0/jaxns/initial_state.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-04-15 13:41:40.397876 jaxns-2.1.0/jaxns/internals/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.1.0/jaxns/internals/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      849 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/internals/linalg.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    12443 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/internals/log_semiring.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     4824 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/internals/maps.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1899 2022-10-13 02:52:05.000000 jaxns-2.1.0/jaxns/internals/shapes.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1853 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/internals/stats.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-04-15 13:41:40.401876 jaxns-2.1.0/jaxns/internals/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.1.0/jaxns/internals/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      277 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/internals/tests/test_linalg.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5490 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/internals/tests/test_log_semiring.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2842 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/internals/tests/test_maps.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1110 2022-12-29 07:48:31.000000 jaxns-2.1.0/jaxns/internals/tests/test_shapes.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1186 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/internals/tests/test_stats.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-04-15 13:41:40.401876 jaxns-2.1.0/jaxns/likelihood_samplers/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.1.0/jaxns/likelihood_samplers/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    21852 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/likelihood_samplers/multi_ellipsoid_utils.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-04-15 13:41:40.401876 jaxns-2.1.0/jaxns/likelihood_samplers/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.1.0/jaxns/likelihood_samplers/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1753 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/likelihood_samplers/tests/test_multi_ellipsoid.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3103 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/model.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    18710 2023-04-15 01:00:38.000000 jaxns-2.1.0/jaxns/nested_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    16040 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/plotting.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    11830 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/prior.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2716 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/random.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    26123 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/slice_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     9157 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/special_priors.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     8748 2023-04-15 04:48:14.000000 jaxns-2.1.0/jaxns/static_slice.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3878 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/static_uniform.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    17405 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/statistics.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5697 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/termination.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-04-15 13:41:40.401876 jaxns-2.1.0/jaxns/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3561 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/tests/test_initial_state.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    14429 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/tests/test_nested_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     8024 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/tests/test_prior.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      976 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/tests/test_random.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    13733 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/tests/test_statistics.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      477 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/tests/test_utils.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5040 2023-03-08 22:42:25.000000 jaxns-2.1.0/jaxns/types.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1899 2023-01-03 05:33:37.000000 jaxns-2.1.0/jaxns/uniform_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    15180 2023-04-15 00:09:56.000000 jaxns-2.1.0/jaxns/utils.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-04-15 13:41:40.397876 jaxns-2.1.0/jaxns.egg-info/
--rw-rw-r--   0 albert    (1000) albert    (1000)     3692 2023-04-15 13:41:40.000000 jaxns-2.1.0/jaxns.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)     1367 2023-04-15 13:41:40.000000 jaxns-2.1.0/jaxns.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-04-15 13:41:40.000000 jaxns-2.1.0/jaxns.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        6 2023-04-15 13:41:40.000000 jaxns-2.1.0/jaxns.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)      103 2022-10-13 02:52:05.000000 jaxns-2.1.0/pyproject.toml
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-04-15 13:41:40.401876 jaxns-2.1.0/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)      949 2023-04-15 04:58:33.000000 jaxns-2.1.0/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 14:57:59.366724 jaxns-2.2.0/
+-rw-rw-r--   0 albert    (1000) albert    (1000)    20138 2022-10-13 02:52:05.000000 jaxns-2.2.0/LICENSE
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4810 2023-06-15 14:57:59.366724 jaxns-2.2.0/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4371 2023-06-15 14:34:45.000000 jaxns-2.2.0/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 14:57:59.362723 jaxns-2.2.0/jaxns/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      386 2023-04-20 22:44:04.000000 jaxns-2.2.0/jaxns/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    13247 2023-05-18 21:09:50.000000 jaxns-2.2.0/jaxns/adaptive_refinement.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     6940 2023-04-21 01:26:04.000000 jaxns-2.2.0/jaxns/initial_state.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 14:57:59.362723 jaxns-2.2.0/jaxns/internals/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.2.0/jaxns/internals/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      849 2023-01-03 05:33:37.000000 jaxns-2.2.0/jaxns/internals/linalg.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    12651 2023-06-15 13:49:53.000000 jaxns-2.2.0/jaxns/internals/log_semiring.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4919 2023-04-21 14:08:43.000000 jaxns-2.2.0/jaxns/internals/maps.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1899 2022-10-13 02:52:05.000000 jaxns-2.2.0/jaxns/internals/shapes.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1853 2023-01-03 05:33:37.000000 jaxns-2.2.0/jaxns/internals/stats.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 14:57:59.362723 jaxns-2.2.0/jaxns/internals/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.2.0/jaxns/internals/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      277 2023-01-03 05:33:37.000000 jaxns-2.2.0/jaxns/internals/tests/test_linalg.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5490 2023-01-03 05:33:37.000000 jaxns-2.2.0/jaxns/internals/tests/test_log_semiring.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2898 2023-06-14 16:43:12.000000 jaxns-2.2.0/jaxns/internals/tests/test_maps.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1110 2022-12-29 07:48:31.000000 jaxns-2.2.0/jaxns/internals/tests/test_shapes.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1186 2023-01-03 05:33:37.000000 jaxns-2.2.0/jaxns/internals/tests/test_stats.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 14:57:59.362723 jaxns-2.2.0/jaxns/likelihood_samplers/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.2.0/jaxns/likelihood_samplers/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3269 2023-06-15 13:57:48.000000 jaxns-2.2.0/jaxns/likelihood_samplers/em_gmm.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    20604 2023-06-15 10:22:16.000000 jaxns-2.2.0/jaxns/likelihood_samplers/multi_ellipsoid_utils.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 14:57:59.362723 jaxns-2.2.0/jaxns/likelihood_samplers/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.2.0/jaxns/likelihood_samplers/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1304 2023-06-14 20:46:20.000000 jaxns-2.2.0/jaxns/likelihood_samplers/tests/test_em_gmm.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4836 2023-06-14 21:03:21.000000 jaxns-2.2.0/jaxns/likelihood_samplers/tests/test_multi_ellipsoid.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3103 2023-05-18 20:19:33.000000 jaxns-2.2.0/jaxns/model.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    18103 2023-06-15 13:59:36.000000 jaxns-2.2.0/jaxns/nested_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    16040 2023-01-03 05:33:37.000000 jaxns-2.2.0/jaxns/plotting.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    12554 2023-06-14 10:16:12.000000 jaxns-2.2.0/jaxns/prior.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2787 2023-04-20 15:27:03.000000 jaxns-2.2.0/jaxns/random.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    10153 2023-05-18 20:55:58.000000 jaxns-2.2.0/jaxns/special_priors.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    16184 2023-05-15 09:26:33.000000 jaxns-2.2.0/jaxns/static_nested_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    26201 2023-04-25 10:29:16.000000 jaxns-2.2.0/jaxns/static_slice.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5072 2023-05-12 12:36:05.000000 jaxns-2.2.0/jaxns/static_uniform.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    16841 2023-06-15 13:57:48.000000 jaxns-2.2.0/jaxns/statistics.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     6607 2023-05-12 13:17:17.000000 jaxns-2.2.0/jaxns/termination.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 14:57:59.362723 jaxns-2.2.0/jaxns/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-01-03 05:33:37.000000 jaxns-2.2.0/jaxns/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2821 2023-06-15 14:57:56.000000 jaxns-2.2.0/jaxns/tests/test_adaptive_refinement.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3882 2023-06-15 10:22:16.000000 jaxns-2.2.0/jaxns/tests/test_initial_state.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    16392 2023-05-15 05:52:12.000000 jaxns-2.2.0/jaxns/tests/test_nested_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     9019 2023-05-18 20:50:55.000000 jaxns-2.2.0/jaxns/tests/test_prior.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1306 2023-04-15 16:37:14.000000 jaxns-2.2.0/jaxns/tests/test_random.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    24209 2023-06-15 13:59:36.000000 jaxns-2.2.0/jaxns/tests/test_statistics.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      477 2023-01-03 05:33:37.000000 jaxns-2.2.0/jaxns/tests/test_utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5118 2023-05-12 12:43:32.000000 jaxns-2.2.0/jaxns/types.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    17668 2023-05-15 05:41:18.000000 jaxns-2.2.0/jaxns/utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      716 2023-05-07 18:38:45.000000 jaxns-2.2.0/jaxns/warnings.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 14:57:59.362723 jaxns-2.2.0/jaxns.egg-info/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4810 2023-06-15 14:57:59.000000 jaxns-2.2.0/jaxns.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1497 2023-06-15 14:57:59.000000 jaxns-2.2.0/jaxns.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-06-15 14:57:59.000000 jaxns-2.2.0/jaxns.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        6 2023-06-15 14:57:59.000000 jaxns-2.2.0/jaxns.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)      103 2022-10-13 02:52:05.000000 jaxns-2.2.0/pyproject.toml
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-06-15 14:57:59.366724 jaxns-2.2.0/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)      949 2023-06-15 14:09:56.000000 jaxns-2.2.0/setup.py
```

### Comparing `jaxns-2.1.0/LICENSE` & `jaxns-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxns-2.1.0/PKG-INFO` & `jaxns-2.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,125 @@
-Metadata-Version: 2.1
-Name: jaxns
-Version: 2.1.0
-Summary: Nested Sampling in JAX
-Home-page: https://github.com/joshuaalbert/jaxns
-Author: Joshua G. Albert
-Author-email: albert@strw.leidenuniv.nl
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
+[![Python](https://img.shields.io/pypi/pyversions/jaxns.svg)](https://badge.fury.io/py/jaxns)
+[![PyPI](https://badge.fury.io/py/jaxns.svg)](https://badge.fury.io/py/jaxns)
 
-![https://pypi.org/project/jaxns/](https://img.shields.io/pypi/v/jaxns.svg)
+Main
+Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=main)
+
+Develop
+Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=develop)
 
 ![JAXNS](https://github.com/Joshuaalbert/jaxns/raw/main/jaxns_logo.png)
 
+## Mission: _To make nested sampling **faster, easier, and more powerful**_
 
 # What is it?
-Provides a probabilistic programming framework based on nested sampling. It's coded in JAX in a manner that allows lowering the entire inference algorithm to XLA primitives, which are JIT-compiled for high performance. You can read about it here: (https://arxiv.org/abs/2012.15286)
 
-JAXNS uses a unique adaptive algorithm that enables arbitrary precision computing of evidence. Stay tuned for the paper that explains it.
+JAXNS is:
+
+1) a probabilistic programming framework using nested sampling as the engine;
+2) coded in JAX in a manner that allows lowering the entire inference algorithm to XLA primitives, which are
+   JIT-compiled for high performance;
+3) continuously improving on its mission of making nested sampling faster, easier, and more powerful; and
+4) citable, and you can read an (old) pre-print here: (https://arxiv.org/abs/2012.15286).
 
 # Documentation
 
-You can check out the docs [here](https://jaxns.readthedocs.io/en/latest/#).
+You can read the documentation [here](https://jaxns.readthedocs.io/en/latest/#).
 
 # Install
 
-Note: JAXNS requires >= Python 3.8, and is tested on 3.8, 3.9, 3.10, and 3.11.
+**Notes:**
+
+1. JAXNS requires >= Python 3.8.
+2. It is always highly recommended to use a unique virtual environment for each project.
+   To use `miniconda`, have it installed, and run
+
+```bash
+# To create a new env, if necessary
+conda create -n jaxns_py python=3.11
+conda activate jaxns_py
+```
+
+## For end users
+
+Install directly from PyPi,
+
+```bash
+pip install jaxns
+```
 
-Make sure you have JAX and the usual suspects with `pip install jax jaxlib numpy matplotlib scipy`, optionally also `scikit-learn` and `haiku-dm` for some examples. 
-Install with `pip install jaxns` or `pip install git+http://github.com/Joshuaalbert/jaxns.git` for the (no promises) bleeding-edge.
+## For development
+
+Clone repo `git clone https://www.github.com/JoshuaAlbert/jaxns.git`, and install:
+
+```bash
+cd jaxns
+pip install -r requirements.txt
+pip install -r requirements-tests.txt
+pip install -r requirements-examples.txt
+pip install .
+```
 
 # Getting help and contributing examples
 
-I'm really encourage anyone in the scientific community to get involved and join the discussion forum.
-Please use the [github discussion forum](https://github.com/Joshuaalbert/jaxns/discussions) for getting help, or contributing examples/neat use cases.
+Do you have a neat Bayesian problem, and want to solve it with JAXNS?
+I'm really encourage anyone in either the scientific community or industry to get involved and join the discussion
+forum.
+Please use the [github discussion forum](https://github.com/Joshuaalbert/jaxns/discussions) for getting help, or
+contributing examples/neat use cases.
 
 # Quick start
 
-JAXNS is really fast because it uses JAX. 
-The caveat is that you need to be able to define your likelihood function with JAX. This is usually no big deal because JAX is just a replacement for numpy and many likelihoods can be expressed such. 
+Checkout the examples [here](https://jaxns.readthedocs.io/en/latest/#).
+
+## Caveats
+
+The caveat is that you need to be able to define your likelihood function with JAX. This is usually no big deal because
+JAX is just a replacement for NumPy and many likelihoods can be expressed such.
 If you're unfamiliar, take a quick tour of JAX (https://jax.readthedocs.io/en/latest/notebooks/quickstart.html).
-Check out the examples for a starter.
 
 # Speed test comparison with other nested sampling packages
 
-JAXNS is much faster than PolyChord, MultiNEST, and dynesty, typically achieving two to three orders of magnitude improvement in speed on cheap likelihood evaluations.
-This is shown in (https://arxiv.org/abs/2012.15286). With regards to how efficiently JAXNS used likeihood evaluations, JAXNS prizes exactness over efficiency, however since it employs an adaptive strategy, users can control efficiency by controlling some precision parameters.
+JAXNS is really fast because it uses JAX.
+JAXNS is much faster than PolyChord, MultiNEST, and dynesty, typically achieving two to three orders of magnitude
+improvement in speed on cheap likelihood evaluations.
+This is shown in (https://arxiv.org/abs/2012.15286). With regards to how efficiently JAXNS used likelihood evaluations,
+JAXNS prizes exactness over efficiency, however since it employs an adaptive strategy, users can control efficiency by
+controlling some precision parameters.
 
 # Change Log
 
+15 June, 2023 -- JAXNS 2.2.0 released. Added support to allow TFP bijectors to defined transformed distributions. Other
+minor improvements.
+
+15 April, 2023 -- JAXNS 2.1.0 released. pmap used on outer-most loops allowing efficient device-device communication
+during parallel runs.
+
 8 March, 2023 -- JAXNS 2.0.1 released. Changed how we're doing annotations to support python 3.8 again.
 
 3 January, 2023 -- JAXNS 2.0 released. Complete overhaul of components. New way to build models.
 
 5 August, 2022 -- JAXNS 1.1.1 released. Pytree shaped priors.
 
-2 June, 2022 -- JAXNS 1.1.0 released. Dynamic sampling takes advantage of adaptive refinement. Parallelisation. Bayesian opt and global opt modules.
+2 June, 2022 -- JAXNS 1.1.0 released. Dynamic sampling takes advantage of adaptive refinement. Parallelisation. Bayesian
+opt and global opt modules.
 
 30 May, 2022 -- JAXNS 1.0.1 released. Improvements to speed, parallelisation, and structure of code.
 
-9 April, 2022 -- JAXNS 1.0.0 released. Parallel sampling, dynamic search, and adaptive refinement. Global optimiser released.
+9 April, 2022 -- JAXNS 1.0.0 released. Parallel sampling, dynamic search, and adaptive refinement. Global optimiser
+released.
 
 2 Jun, 2021 -- JAXNS 0.0.7 released.
 
 13 May, 2021 -- JAXNS 0.0.6 released.
 
 8 Mar, 2021 -- JAXNS 0.0.5 released.
 
 8 Mar, 2021 -- JAXNS 0.0.4 released.
 
-7 Mar, 2021 -- JAXNS 0.0.3 released. 
+7 Mar, 2021 -- JAXNS 0.0.3 released.
 
-28 Feb, 2021 -- JAXNS 0.0.2 released. 
+28 Feb, 2021 -- JAXNS 0.0.2 released.
 
-28 Feb, 2021 -- JAXNS 0.0.1 released. 
+28 Feb, 2021 -- JAXNS 0.0.1 released.
 
 1 January, 2021 -- Paper submitted
```

### Comparing `jaxns-2.1.0/jaxns/adaptive_refinement.py` & `jaxns-2.2.0/jaxns/adaptive_refinement.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,83 @@
-from functools import partial
-from typing import Tuple, Optional, NamedTuple
+import logging
+from typing import Tuple, NamedTuple
 
 from etils.array_types import PRNGKey, FloatArray, IntArray, BoolArray
-from jax import core, numpy as jnp, tree_map, random, jit
-from jax._src.lax.control_flow import while_loop
+from jax import core, numpy as jnp, tree_map, random, pmap
+from jax._src.lax.control_flow import while_loop, scan
+from jax._src.lax.parallel import all_gather
 
-from jaxns.internals.maps import chunked_pmap
 from jaxns.internals.stats import linear_to_log_stats
 from jaxns.model import Model
-from jaxns.slice_sampler import UniDimSliceSampler, SeedPoint, PreprocessType, AbstractSliceSampler
+from jaxns.static_nested_sampler import PreProcessType, add_chunk_dim, remove_chunk_dim, SeedPoint
+from jaxns.static_slice import UniDimSliceSampler
 from jaxns.statistics import analyse_sample_collection
 from jaxns.types import NestedSamplerState, Reservoir, int_type, float_type
 from jaxns.utils import sort_samples
 
 __all__ = ['AdaptiveRefinement']
 
+logger = logging.getLogger('jaxns')
+
 
 class AdaptiveRefinement:
-    def __init__(self, model: Model, uncert_improvement_patience: int, num_slices: int, num_parallel_samplers: int = 1,
-                 slice_sampler: Optional[AbstractSliceSampler] = None):
-        if uncert_improvement_patience <= 0:
-            raise ValueError(f"uncert_improvement_patient should be > 0, got {uncert_improvement_patience}.")
-        self.uncert_improvement_patience = uncert_improvement_patience
+    """
+    Class for adaptive refinement.
+    """
+
+    def __init__(self, model: Model, patience: int = 1, num_parallel_samplers: int = 1):
+        """
+        Initialised adaptive refinement.
+
+        Args:
+            model: Model
+            patience: how many steps with stopping condition met before stopping
+            num_parallel_samplers: how many parallel samplers to use.
+        """
+        if patience < 1:
+            raise ValueError(f"patience should be >= 1, got {patience}.")
+        self.patience = patience
         self.num_parallel_samplers = num_parallel_samplers
-        if slice_sampler is None:
-            slice_sampler = UniDimSliceSampler(
-                model=model,
-                midpoint_shrink=True,
-                multi_ellipse_bound=False
-            )
-        self.slice_sampler = slice_sampler
-        self.num_slices = num_slices
+        self.sampler = UniDimSliceSampler(model=model, num_slices=model.U_ndims, midpoint_shrink=True, perfect=True)
 
-    def split_state(self, state: NestedSamplerState) -> Tuple[NestedSamplerState, Reservoir]:
+    def _split_state(self, state: NestedSamplerState) -> Tuple[NestedSamplerState, Reservoir]:
         """
         Splice a state into iid samples and non-iid samples.
 
         Note: must not be run in a JIT-context, as the nonzero operation non-static.
 
         Args:
             state: state to split
 
         Returns:
             a state of iid samples, and reservoir of non-iid samples
         """
         if isinstance(state.sample_collection.reservoir.iid, core.Tracer):
             raise RuntimeError("Tracer detected, but expected imperative context.")
         num_samples = state.sample_collection.reservoir.log_L.size
+
         (update_indicies,) = jnp.nonzero(
-            jnp.bitwise_not(state.sample_collection.reservoir.iid) & (
-                    jnp.arange(num_samples) < state.sample_collection.sample_idx
-            )
+            (jnp.bitwise_not(state.sample_collection.reservoir.iid) &
+             (jnp.arange(num_samples) < state.sample_collection.sample_idx)
+             )
         )
 
         (keep_indicies,) = jnp.nonzero(state.sample_collection.reservoir.iid)
 
         update_reservoir = tree_map(lambda x: x[update_indicies], state.sample_collection.reservoir)
         keep_reservoir = tree_map(lambda x: x[keep_indicies], state.sample_collection.reservoir)
         state = state._replace(
             sample_collection=state.sample_collection._replace(
                 sample_idx=keep_indicies.size,
                 reservoir=keep_reservoir
             )
         )
         return state, update_reservoir
 
-    def combine_state(self, state: NestedSamplerState, update_reservoir: Reservoir) -> NestedSamplerState:
+    def _combine_state(self, state: NestedSamplerState, update_reservoir: Reservoir) -> NestedSamplerState:
         """
         Concatenates a state and reservoir and sorts the state.
 
         Args:
             state: state
             update_reservoir: reservoir
 
@@ -86,95 +94,132 @@
         )
         # Sort
         sample_collection = sort_samples(sample_collection)
         state = state._replace(sample_collection=sample_collection)
         return state
 
     def _single_improvement(self, key: PRNGKey, seed_point: SeedPoint, log_L_constraint: FloatArray,
-                            preprocess_data: PreprocessType) -> Reservoir:
+                            preprocess_data: PreProcessType) -> Reservoir:
         """
         Perform perfect slice sampling, thereby improving the sample.
 
         Args:
             key: PRNGKey
             seed_point: seed point to sample from
             log_L_constraint: the constraint to sample inside
             preprocess_data: preprocessing data
 
         Returns:
             a sample from the seed point sampled within the given constraint
         """
-        sample = self.slice_sampler.get_sample(key=key,
-                                               seed_point=seed_point,
-                                               log_L_constraint=log_L_constraint,
-                                               num_slices=self.num_slices,
-                                               preprocess_data=preprocess_data)
+        sample = self.sampler.get_sample_from_seed(key=key,
+                                                   seed_point=seed_point,
+                                                   log_L_constraint=log_L_constraint,
+                                                   preprocess_data=preprocess_data)
         return Reservoir(*sample)
 
-    @partial(jit, static_argnums=0)
-    def improve(self, state: NestedSamplerState, iid_state: NestedSamplerState, non_iid_reservoir: Reservoir):
+    def _single_improvement_batch(self,
+                                  key: PRNGKey,
+                                  non_iid_reservoir: Reservoir,
+                                  preprocess_data: PreProcessType) -> Reservoir:
+        """
+        Run nested sampling to replace an entire live point reservoir via shrinkage.
+
+        Args:
+            key: PRNGKey
+            non_iid_reservoir: reservoir to improve
+            preprocess_data: any data needed to shrink the replace the live point reservoir with i.i.d. samples.
+
+        Returns:
+            improved reservoir
+        """
+
+        class CarryType(NamedTuple):
+            key: PRNGKey
+
+        class XsType(NamedTuple):
+            reservoir_point: Reservoir
+
+        ResultType = Reservoir
+
+        def body(carry: CarryType, X: XsType) -> Tuple[CarryType, ResultType]:
+            key, improve_key = random.split(carry.key, 2)
+            seed_point = SeedPoint(U0=X.reservoir_point.point_U, log_L0=X.reservoir_point.log_L)
+            improved_point = self._single_improvement(
+                key=improve_key,
+                seed_point=seed_point,
+                log_L_constraint=X.reservoir_point.log_L_constraint,
+                preprocess_data=preprocess_data
+            )
+            # Update stats
+            improved_point = improved_point._replace(
+                num_slices=improved_point.num_slices + X.reservoir_point.num_slices,
+                num_likelihood_evaluations=(improved_point.num_likelihood_evaluations
+                                            + X.reservoir_point.num_likelihood_evaluations)
+            )
+
+            return CarryType(key=key), improved_point
+
+        _, improved_reservoir = scan(body,
+                                     CarryType(key),
+                                     XsType(reservoir_point=non_iid_reservoir))
+        return improved_reservoir
+
+    def _single_improve_thread(self, key: PRNGKey, iid_state: NestedSamplerState,
+                               non_iid_reservoir: Reservoir) -> [NestedSamplerState, Reservoir]:
         """
         Performs perfect slice sampling on the set of samples that are not considered i.i.d. sampled within their
         respective likelihood constraint.
 
         Args:
-            state: state to improve
+            key: PRNGKey
             iid_state: state with only the i.i.d. samples
             non_iid_reservoir: samples that are not deemed i.i.d.
 
         Returns:
-            state where all samples are considered i.i.d. sampled within their respective likelihood constraints
+            reservoir where all samples are considered i.i.d. sampled within their respective likelihood constraints
         """
 
+        iid_state = iid_state._replace(key=key)
+
         # update each sample one slice at a time until the stopping condition
 
         class CarryType(NamedTuple):
             key: PRNGKey
-            reservoir: Reservoir
+            non_iid_reservoir: Reservoir
             last_log_Z_mean: FloatArray
             last_diff_log_Z_mean: FloatArray
-            patience: IntArray
-            preprocess_data: PreprocessType
+            converged_step_count: IntArray
+            state: NestedSamplerState
+            output_log_Z: FloatArray
+            iter_j: IntArray
 
         def cond(body_state: CarryType) -> BoolArray:
-            (_, _, _, _, patience, _) = body_state
-            done = jnp.greater_equal(patience, self.uncert_improvement_patience)
+            done = jnp.greater_equal(body_state.converged_step_count, self.patience)
+            done = body_state.iter_j >= 0  # TODO: remove
             return jnp.bitwise_not(done)
 
         def body(body_state: CarryType) -> CarryType:
-            batch_size = body_state.reservoir.iid.size
+            key, improve_key = random.split(body_state.state.key, 2)
+            state = body_state.state._replace(key=key)
 
-            key, combine_key, improve_key = random.split(body_state.key, 3)
+            preprocess_data = self.sampler.preprocess(state)
 
-            parallel_improvement = chunked_pmap(
-                lambda key, seed_point, log_L_constraint: self._single_improvement(
-                    key=key,
-                    seed_point=seed_point,
-                    log_L_constraint=log_L_constraint,
-                    preprocess_data=body_state.preprocess_data
-                ),
-                chunksize=self.num_parallel_samplers,
-                batch_size=batch_size)
-            seed_points = SeedPoint(
-                U0=body_state.reservoir.point_U,
-                log_L0=body_state.reservoir.log_L
-            )
-            update_reservoir = parallel_improvement(random.split(improve_key, batch_size),
-                                                    seed_points,
-                                                    body_state.reservoir.log_L_constraint)
-
-            update_reservoir = update_reservoir._replace(
-                num_slices=update_reservoir.num_slices + body_state.reservoir.num_slices,
-                num_likelihood_evaluations=(update_reservoir.num_likelihood_evaluations
-                                            + body_state.reservoir.num_likelihood_evaluations)
+            update_reservoir = self._single_improvement_batch(
+                key=improve_key,
+                non_iid_reservoir=body_state.non_iid_reservoir,
+                preprocess_data=preprocess_data
             )
 
-            updated_state = self.combine_state(state=iid_state, update_reservoir=update_reservoir)
+            all_update_reservoir: Reservoir = remove_chunk_dim(all_gather(update_reservoir, 'i'))
+
+            all_state = self._combine_state(state=iid_state, update_reservoir=all_update_reservoir)
+
             evidence_calculation, sample_stats = analyse_sample_collection(
-                sample_collection=updated_state.sample_collection,
+                sample_collection=all_state.sample_collection,
                 sorted_collection=True
             )
             log_Z_mean, log_Z_var = linear_to_log_stats(
                 log_f_mean=evidence_calculation.log_Z_mean,
                 log_f2_mean=evidence_calculation.log_Z2_mean
             )
             nan_last_log_Z_mean = jnp.isnan(body_state.last_log_Z_mean)
@@ -182,44 +227,82 @@
             nan_log_Z_mean = jnp.isnan(log_Z_mean)
 
             diff_log_Z_mean = jnp.abs(body_state.last_log_Z_mean - log_Z_mean)
             small_change = jnp.square(2. * diff_log_Z_mean) < log_Z_var
             decreasing_change = diff_log_Z_mean < body_state.last_diff_log_Z_mean
             stable = decreasing_change | small_change
             reset_patience = jnp.bitwise_not(stable) | (nan_log_Z_mean | nan_last_log_Z_mean | nan_log_Z_var)
-            patience = jnp.where(reset_patience, jnp.zeros_like(body_state.patience),
-                                 body_state.patience + jnp.ones_like(body_state.patience))
-            preprocess_data = self.slice_sampler.preprocess(updated_state)
-            return CarryType(key, update_reservoir, log_Z_mean, diff_log_Z_mean, patience, preprocess_data)
+            converged_step_count = jnp.where(reset_patience, jnp.asarray(0, int_type),
+                                             body_state.converged_step_count + jnp.asarray(1, int_type))
 
-        preprocess_data = self.slice_sampler.preprocess(state)
+            # output_log_Z = body_state.output_log_Z.at[body_state.iter_j].set(jnp.sum(sample_stats.num_live_points))
+            output_log_Z = body_state.output_log_Z.at[body_state.iter_j].set(log_Z_mean)  # TODO: remove
+            return CarryType(key=key, non_iid_reservoir=update_reservoir, last_log_Z_mean=log_Z_mean,
+                             last_diff_log_Z_mean=diff_log_Z_mean, converged_step_count=converged_step_count,
+                             state=all_state,
+                             output_log_Z=output_log_Z, iter_j=body_state.iter_j + 1)
 
-        key, improve_key = random.split(state.key, 2)
+        key, improve_key = random.split(iid_state.key, 2)
+        init_state = self._combine_state(state=iid_state, update_reservoir=non_iid_reservoir)
         init_evidence_calculation, _ = analyse_sample_collection(
-            sample_collection=state.sample_collection,
+            sample_collection=init_state.sample_collection,
             sorted_collection=True
         )
         init_log_Z_mean, _ = linear_to_log_stats(
             log_f_mean=init_evidence_calculation.log_Z_mean,
             log_f2_mean=init_evidence_calculation.log_Z2_mean
         )
-
+        output_log_Z = jnp.full((20,), jnp.nan, float_type)
+        output_log_Z = output_log_Z.at[0].set(init_log_Z_mean)
         init_body_state: CarryType = CarryType(
-            improve_key, non_iid_reservoir, init_log_Z_mean, jnp.asarray(0., float_type), jnp.asarray(0, int_type),
-            preprocess_data)
+            key=improve_key, non_iid_reservoir=non_iid_reservoir, last_log_Z_mean=init_log_Z_mean,
+            last_diff_log_Z_mean=jnp.asarray(0., float_type), converged_step_count=jnp.asarray(0, int_type),
+            state=init_state, output_log_Z=output_log_Z, iter_j=jnp.asarray(1, int_type))
         output_state = while_loop(cond,
                                   body,
                                   init_body_state)
 
-        # mark as iid now <==> the evidence stopped changing
-        update_reservoir = output_state.reservoir._replace(iid=jnp.ones_like(output_state.reservoir.iid))
+        return output_state.state, output_state.output_log_Z
+
+    def __call__(self, state: NestedSamplerState) -> NestedSamplerState:
+        """
+        Adaptively refines the state until all samples are i.i.d. (according to a given stopping condition).
+
+        Args:
+            state: nested sampler state
 
-        updated_state = self.combine_state(state=iid_state, update_reservoir=update_reservoir)
+        Returns:
+            state after refinement
+        """
+        # Split state will give an error if this is a tracer context so don't JIT compile.
+        iid_state, non_iid_reservoir = self._split_state(state)
 
-        updated_state = updated_state._replace(key=key)
-        return updated_state
+        keys = random.split(state.key, self.num_parallel_samplers)
 
-    def __call__(self, state: NestedSamplerState) -> NestedSamplerState:
-        if isinstance(state.sample_collection.reservoir.iid, core.Tracer):
-            raise RuntimeError("Tracer detected, but expected imperative context.")
-        iid_state, non_iid_reservoir = self.split_state(state)
-        return self.improve(state=state, iid_state=iid_state, non_iid_reservoir=non_iid_reservoir)
+        non_iid_count = non_iid_reservoir.log_L.size
+        remainder = int(non_iid_count) % self.num_parallel_samplers
+        extra = (self.num_parallel_samplers - remainder) % self.num_parallel_samplers
+        if extra > 0:
+            logger.warning(
+                f"Increasing non_iid_reservoir ({non_iid_count}) by {extra} to closest multiple of num_parallel_samplers.")
+            non_iid_reservoir = tree_map(lambda x: jnp.concatenate([x] + [x[0:1]] * extra, axis=0), non_iid_reservoir)
+
+        chunked_non_iid_reservoir = add_chunk_dim(non_iid_reservoir, self.num_parallel_samplers)
+
+        parallel_ar = pmap(
+            lambda key, non_iid_reservoir: self._single_improve_thread(
+                key=key,
+                iid_state=iid_state,
+                non_iid_reservoir=non_iid_reservoir
+            ),
+            axis_name='i')
+
+        chunked_updated_state, chunked_output_log_Z = parallel_ar(keys, chunked_non_iid_reservoir)
+
+        # Is there a better way to get only one out, since they are identical on each device?
+        (updated_state, output_log_Z) = tree_map(lambda x: x[0], (chunked_updated_state, chunked_output_log_Z))
+
+        # import pylab as plt
+        # plt.plot(output_log_Z)
+        # plt.show()
+
+        return updated_state
```

### Comparing `jaxns-2.1.0/jaxns/internals/linalg.py` & `jaxns-2.2.0/jaxns/internals/linalg.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.1.0/jaxns/internals/log_semiring.py` & `jaxns-2.2.0/jaxns/internals/log_semiring.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from typing import Union
+
 from jax import numpy as jnp
 from jax.lax import scan
 from jax.scipy.special import logsumexp
 
-from jaxns.types import SignedLog
+from jaxns.types import SignedLog, float_type
 
 
 def logaddexp(x1, x2):
     """
     Equivalent to logaddexp but supporting complex arguments.
 
     see np.logaddexp
@@ -86,21 +88,21 @@
         v = result
         if axis != 0:
             v = jnp.swapaxes(v, axis, 0)
         return v
 
 
 class LogSpace(object):
-    def __init__(self, log_abs_val: jnp.ndarray, sign=None):
-        self._log_abs_val = log_abs_val
+    def __init__(self, log_abs_val: Union[jnp.ndarray, float], sign: Union[jnp.ndarray, float] = None):
+        self._log_abs_val = jnp.asarray(log_abs_val, float_type)
         if sign is None:
-            self._sign = 1.
+            self._sign = jnp.asarray(1., float_type)
             self._naked = True
         else:
-            self._sign = sign
+            self._sign = jnp.asarray(sign, float_type)
             self._naked = False
 
     @property
     def dtype(self):
         return self.log_abs_val.dtype
 
     @property
@@ -311,16 +313,17 @@
 
         Args:
             other: ndarray or LogSpace, if ndarray assumed to be log(B)
 
         Returns:
              LogSpace
         """
-        if not isinstance(n, (int, float)):
+        if not isinstance(n, (int, float, jnp.ndarray)):
             raise NotImplementedError("Not implemented for non-int powers.")
+        n = jnp.asarray(n, float_type)
         if self._naked:
             return LogSpace(n * self.log_abs_val)
         # complex values can occur if n is not even
         return LogSpace(n * self.log_abs_val, sign=self.sign ** n)
         # for _ in range(n-1):
         #     output = output * self
         # return output
```

### Comparing `jaxns-2.1.0/jaxns/internals/maps.py` & `jaxns-2.2.0/jaxns/internals/maps.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,7 +131,10 @@
         arg = jnp.concatenate([arg] + [arg[0:1]] * extra, axis=0)
         N = N + extra
     else:
         extra = 0
     T = N // chunksize
     arg = jnp.reshape(arg, (chunksize, N // chunksize) + arg.shape[1:])
     return arg
+
+def prepad(a, chunksize: int):
+    return tree_map(lambda arg: _pad_extra(arg, chunksize), a)
```

### Comparing `jaxns-2.1.0/jaxns/internals/shapes.py` & `jaxns-2.2.0/jaxns/internals/shapes.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.1.0/jaxns/internals/stats.py` & `jaxns-2.2.0/jaxns/internals/stats.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.1.0/jaxns/internals/tests/test_log_semiring.py` & `jaxns-2.2.0/jaxns/internals/tests/test_log_semiring.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.1.0/jaxns/internals/tests/test_maps.py` & `jaxns-2.2.0/jaxns/internals/tests/test_maps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import jax
 from jax import numpy as jnp
 
 from jaxns.internals.maps import replace_index, chunked_pmap, prepare_func_args, get_index
 
 
 def test_replace_index():
     operand = jnp.asarray([0, 1, 2, 3, 4])
@@ -34,16 +35,17 @@
         return x * y
 
     chunked_f = chunked_pmap(f, 1)
     x = jnp.arange(3)
     assert chunked_f(x, y=x).shape == x.shape
     assert jnp.all(chunked_f(x, y=x) == x ** 2)
 
-    chunked_f = chunked_pmap(f, 2)
-    x = jnp.arange(2)
+    num_dev = len(jax.devices())
+    chunked_f = chunked_pmap(f, num_dev)
+    x = jnp.arange(num_dev)
     assert chunked_f(x, y=x).shape == x.shape
     assert jnp.all(chunked_f(x, y=x) == x ** 2)
 
     x = jnp.arange(3)
     assert chunked_f(x, y=x).shape == x.shape
     assert jnp.all(chunked_f(x, y=x) == x ** 2)
```

### Comparing `jaxns-2.1.0/jaxns/internals/tests/test_shapes.py` & `jaxns-2.2.0/jaxns/internals/tests/test_shapes.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.1.0/jaxns/internals/tests/test_stats.py` & `jaxns-2.2.0/jaxns/internals/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.1.0/jaxns/likelihood_samplers/multi_ellipsoid_utils.py` & `jaxns-2.2.0/jaxns/likelihood_samplers/multi_ellipsoid_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from typing import NamedTuple, Tuple
 
+import numpy as np
+import pylab as plt
 from etils.array_types import IntArray, FloatArray, PRNGKey, BoolArray
 from jax import numpy as jnp, vmap, random, tree_map
 from jax._src.lax.control_flow import while_loop
 from jax._src.scipy.special import gammaln
 
 from jaxns.internals.log_semiring import LogSpace
+from jaxns.likelihood_samplers.em_gmm import em_gmm
 from jaxns.types import UType, int_type, float_type
 
 __all__ = ['ellipsoid_clustering',
            'sample_multi_ellipsoid',
            'MultEllipsoidState']
 
 
@@ -36,31 +39,46 @@
     Args:
         points: [N, D] points to fit ellipsoids to
         mask: [N] mask of which points to consider
 
     Returns:
         mu, cov
     """
-
     mu = jnp.average(points, weights=mask, axis=0)
     dx = points - mu
     cov = jnp.average(dx[:, :, None] * dx[:, None, :], weights=mask, axis=0)
     return mu, cov
 
 
-def test_ellipsoid_params():
-    n = 1000
-    X = random.multivariate_normal(random.PRNGKey(42), mean=jnp.asarray([0., 0.]),
-                                   cov=jnp.asarray([[1., 0.4], [0.4, 1.]]), shape=(n,))
-    mu, radii, rotation = ellipsoid_params(points=X, mask=jnp.ones(n, jnp.bool_))
-    import pylab as plt
-    plt.scatter(X[:,0], X[:,1])
-    plot_ellipses(tree_map(lambda x: x[None], MultiEllipsoidParams(mu, radii, rotation)))
-    assert jnp.all(vmap(lambda x: point_in_ellipsoid(x, mu, radii, rotation))(X))
+def covariance_to_rotational(cov: jnp.ndarray) -> Tuple[jnp.ndarray, jnp.ndarray]:
+    """
+    (x - mu)^T inv(cov) (x - mu) = (x - mu)^T J @ J.T (x - mu)
+
+    where J.T is composed of un-rotation and un-scaling:
+
+    J.T = diag(1/radii) @ rotation.T <==> J = rotation @ diag(1/radii)
+
+    Now since, cov = U @ diag(s) @ V.H we have
+
+    J @ J.T = inv(U @ diag(s) @ V.H) = V @ diag(1/s) @ U.H
+
+    ==> J.T = diag(1/sqrt(s)) @ U.H
+    ==> radii = sqrt(s), rotation = U
+
+    Args:
+        cov:
 
+    Returns:
+        radii, rotation
+    """
+    u, s, vh = jnp.linalg.svd(cov)
+    radii_min = jnp.finfo(s.dtype).eps
+    radii = jnp.maximum(jnp.sqrt(s), radii_min)
+    rotation = u
+    return radii, rotation
 
 
 def ellipsoid_params(points: UType, mask: FloatArray) -> Tuple[FloatArray, FloatArray, FloatArray]:
     """
     If the ellipsoid is defined by
 
     (x - mu)^T cov (x - mu) = 1
@@ -73,92 +91,41 @@
         points: [N, D] points to fit ellipsoids to
         mask: [N] mask of which points to consider
 
     Returns:
         mu [D], radii [D] rotation [D,D]
     """
     # get ellipsoid mean and covariance
-    mu, cov = bounding_ellipsoid(points=points, mask=mask)
-    # compute factorisation
-    u, s, vh = jnp.linalg.svd(cov)
-    W, Q, Vh = vh.T, jnp.where(s > 1e-15, jnp.reciprocal(s), jnp.zeros_like(s)), u.T
-    C = (W * Q) @ Vh
-
-    print(jnp.linalg.inv(C))
-    radii = jnp.sqrt(Q)
-    print(radii, s)
-    rotation = u # Vh.conj().T
+    mu, Sigma = bounding_ellipsoid(points=points, mask=mask)
+    radii, rotation = covariance_to_rotational(Sigma)
 
     # Compute scale factor for radii to enclose all points.
-    # for all i (points[i] - f) @ inv(scale * cov) @ (points[i] - f) <= 1
-    # for all i (points[i] - f) @ inv(cov) @ (points[i] - f) <= scale
-    # -> choose scale = max_i (points[i] - f) @ inv(cov) @ (points[i] - f)
-    dx = points - mu
-    maha = vmap(lambda dx: dx @ C @ dx)(dx)
-    scale = jnp.max(jnp.where(mask, maha, 0.))
-    radii /= scale
+    # for all i (points[i] - mu) @ inv(Sigma) / scale**2 @ (points[i] - mu) <= 1
+    # for all i (points[i] - mu) @ (L @ L.T) @ (points[i] - mu) <= scale**2
+    rho = vmap(lambda x: maha_ellipsoid(x=x, mu=mu, radii=radii, rotation=rotation))(points)
 
-    return mu, radii, rotation
+    rho_max = jnp.max(jnp.where(mask, rho, 0.))
+    radii *= jnp.sqrt(rho_max)
 
-
-###
-# clustering
-
-def kmeans(key, points, mask, K=2):
-    """
-    Perform kmeans clustering with Euclidean metric.
-
-    Args:
-        key:
-        points: [N, D]
-        mask: [N] bool
-        K: int
-
-    Returns: cluster_id [N], centers [K, D]
-
-    """
-    N, D = points.shape
-
-    def body(state):
-        (i, done, old_cluster_id, centers) = state
-        new_centers = vmap(lambda k: jnp.average(points, weights=(old_cluster_id == k) & mask, axis=0))(jnp.arange(K))
-        dx = points - new_centers[:, None, :]  # K, N, D
-        squared_norm = jnp.sum(jnp.square(dx), axis=-1)  # K, N
-        new_cluster_id = jnp.argmin(squared_norm, axis=0)  # N
-        done = jnp.all(new_cluster_id == old_cluster_id)
-        # print("kmeans reassigns", jnp.sum(old_cluster_id!=new_cluster_k))
-        return i + 1, done, new_cluster_id, new_centers
-
-    do_kmeans = jnp.sum(mask) > K
-    i, _, cluster_id, centers = while_loop(lambda state: ~state[1],
-                                           body,
-                                           (jnp.array(0), ~do_kmeans,
-                                            random.randint(key, shape=(N,), minval=jnp.asarray(0),
-                                                           maxval=jnp.asarray(2)),
-                                            jnp.zeros((K, D))))
-    return cluster_id, centers
-
-
-###
-# Sampling
+    return mu, radii, rotation
 
 
 def ellipsoid_to_circle(point: FloatArray, mu: FloatArray, radii: FloatArray, rotation: FloatArray) -> FloatArray:
     """
     Apply a linear map that would turn an ellipsoid into a sphere.
     Args:
         point: [D] point to transform
         mu: [D] center of ellipse
         radii: [D] radii of ellipse
         rotation: [D,D] rotation matrix of ellipse
 
     Returns:
         a transformed point of shape [D]
     """
-    return (rotation.T / radii[:, None]) @ (point - mu)
+    return jnp.diag(jnp.reciprocal(radii)) @ rotation.T @ (point - mu)
 
 
 def circle_to_ellipsoid(point: FloatArray, mu: FloatArray, radii: FloatArray, rotation: FloatArray) -> FloatArray:
     """
     Apple a linear map that would turn a sphere into an ellipsoid
 
     Args:
@@ -166,15 +133,15 @@
         mu: [D] center of ellipse
         radii: [D] radii of ellipse
         rotation: [D,D] rotation matrix of ellipse
 
     Returns:
         a transformed point of shape [D]
     """
-    return (rotation * radii[None, :]) @ point + mu
+    return mu + (rotation @ jnp.diag(radii) @ point)
 
 
 def maha_ellipsoid(x: FloatArray, mu: FloatArray, radii: FloatArray, rotation: FloatArray) -> FloatArray:
     """
     Compute the Mahalanobis distance.
 
     Args:
@@ -356,15 +323,16 @@
     N, D = points.shape
     n_S = jnp.sum(mask)
     # calculate bounding ellipsoid
     ###
     # input is essentially log_VS
     if kmeans_init:
         # do Euclidean kmean clustering
-        cluster_id, centers = kmeans(init_key, points, mask, K=2)
+        cluster_id, (centers, covariances, log_weight), total_iters = em_gmm(key=init_key, data=points, mask=mask,
+                                                                             n_components=2, n_iters=100)
     else:
         # assign to random clusters: child0 or child1
         cluster_id = random.randint(init_key, shape=(N,), minval=0, maxval=2)
 
     def body(state):
         (i, done, old_cluster_id, _, _, _, _, _, _, _, _, min_loss, delay) = state
         mask1 = mask & (old_cluster_id == 0)
@@ -460,20 +428,19 @@
 
     params2 = MultiEllipsoidParams(mu=mu2, radii=radii2, rotation=rotation2)
 
     return cluster_id, log_VS1, params1, log_VS2, params2, do_split
 
 
 def plot_ellipses(params: MultiEllipsoidParams):
-    import pylab as plt
     theta = jnp.linspace(0., 2 * jnp.pi, 100)
     circle = jnp.stack([jnp.cos(theta), jnp.sin(theta)], axis=1)
     for mu, radii, rotation in zip(params.mu, params.radii, params.rotation):
         ellipse = vmap(lambda point: circle_to_ellipsoid(point, mu, radii, rotation))(circle)
-        plt.plot(ellipse[:, 0], ellipse[:, 1])
+        plt.plot(ellipse[:, 0], ellipse[:, 1], c=np.random.uniform(size=3))
     plt.show()
 
 
 def ellipsoid_clustering(key: PRNGKey, points: FloatArray, log_VS: FloatArray,
                          max_num_ellipsoids: int) -> MultEllipsoidState:
     """
     Partition live_points into 2^depth ellipsoids in depth-first order.
@@ -504,17 +471,14 @@
     mu, radii, rotation = ellipsoid_params(points=points, mask=jnp.ones(N, jnp.bool_))
 
     params = params._replace(
         mu=params.mu.at[0].set(mu),
         radii=params.radii.at[0].set(radii),
         rotation=params.rotation.at[0].set(rotation)
     )
-    import pylab as plt
-    plt.scatter(points[:, 0], points[:, 1])
-    plot_ellipses(params)
 
     state = MultEllipsoidState(cluster_id=cluster_id,
                                params=params)
 
     log_VS_subclusters = jnp.array([log_VS] + [-jnp.inf] * (K - 1))
     done_splitting = jnp.asarray([False] + [True] * (K - 1), jnp.bool_)
     split_depth = jnp.zeros([K], int_type)
```

### Comparing `jaxns-2.1.0/jaxns/model.py` & `jaxns-2.2.0/jaxns/model.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.1.0/jaxns/nested_sampler.py` & `jaxns-2.2.0/jaxns/nested_sampler.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,54 +3,60 @@
 from typing import Optional, Tuple, Union, List
 
 import tensorflow_probability.substrates.jax as tfp
 from etils.array_types import PRNGKey, IntArray
 from jax import random, numpy as jnp, core, tree_map, vmap, jit
 
 from jaxns.adaptive_refinement import AdaptiveRefinement
-from jaxns.initial_state import init_sample_collection, get_uniform_init_live_points, get_live_points_from_samples
+from jaxns.initial_state import init_sample_collection, get_uniform_init_live_points
 from jaxns.internals.log_semiring import LogSpace, normalise_log_space
 from jaxns.internals.stats import linear_to_log_stats, effective_sample_size
 from jaxns.model import Model
 from jaxns.plotting import plot_cornerplot, plot_diagnostics
-from jaxns.slice_sampler import UniDimSliceSampler, AbstractSliceSampler
-from jaxns.static_slice import StaticSlice
-from jaxns.static_uniform import StaticUniform
+from jaxns.static_nested_sampler import StaticNestedSampler, AbstractSampler
+from jaxns.static_slice import UniDimSliceSampler
+from jaxns.static_uniform import UniformSampler
 from jaxns.statistics import analyse_sample_collection
 from jaxns.types import TerminationCondition, NestedSamplerState, NestedSamplerResults, LivePoints
 from jaxns.utils import collect_samples
 from jaxns.utils import summary, save_results, load_results
 
 tfpd = tfp.distributions
 
 logger = logging.getLogger('jaxns')
 
-__all__ = ['NestedSampler',
+__all__ = ['BaseNestedSampler',
            'ApproximateNestedSampler',
            'ExactNestedSampler']
 
 
-class NestedSampler:
-    def __init__(self, model: Model, num_live_points: Union[int, float], num_parallel_samplers: int,
-                 max_samples: Union[int, float]):
-        remainder = int(num_live_points) % num_parallel_samplers
-        extra = (num_parallel_samplers - remainder) % num_parallel_samplers
-        if extra > 0:
-            logger.warning(
-                f"Increasing num_live_points ({num_live_points}) by {extra} to closest multiple of num_parallel_samplers.")
-        self.num_live_points = int(num_live_points + extra)
-        self.num_parallel_samplers = int(num_parallel_samplers)
+class BaseNestedSampler:
+    def __init__(self, model: Model, max_samples: Union[int, float]):
         self.model = model
+        self.max_samples = int(max_samples)
 
-        remainder = int(max_samples) % num_parallel_samplers
-        extra = (num_parallel_samplers - remainder) % num_parallel_samplers
-        if extra > 0:
-            logger.warning(
-                f"Increasing max_samples ({max_samples}) by {extra} to closest multiple of num_parallel_samplers.")
-        self.max_samples = int(max_samples + extra)
+    def initialise(self, key: PRNGKey, num_live_points: int) -> Tuple[NestedSamplerState, LivePoints]:
+        """
+        Creates initial live points from -inf contour and state.
+
+        Args:
+            key: PRNGKey
+
+        Returns:
+            initial state, and live points
+        """
+        state_key, live_points_key = random.split(key, 2)
+        init_state = NestedSamplerState(
+            key=state_key,
+            sample_collection=init_sample_collection(size=self.max_samples, model=self.model)
+        )
+        live_points = get_uniform_init_live_points(live_points_key,
+                                                   num_live_points=num_live_points,
+                                                   model=self.model)
+        return init_state, live_points
 
     def resize_state(self, state: NestedSamplerState, max_num_samples: int) -> NestedSamplerState:
         """
         Grow the state to the size of max_num_samples.
 
         Args:
             state: state to enlarge
@@ -164,58 +170,82 @@
             total_num_slices=total_num_slices,
             log_efficiency=efficiency.log_abs_val,
             # total_num_samples / total_num_likelihood_evaluations
             termination_reason=termination_reason,  # termination condition as bit mask
             num_slices=sample_collection.reservoir.num_slices,
             samples=samples)
 
+    def __call__(self, key: PRNGKey, term_cond: TerminationCondition, *,
+                 init_state: Optional[NestedSamplerState] = None) -> Tuple[IntArray, NestedSamplerState]:
+        """
+        Performs approximate nested sampling followed by adaptive refinement.
 
-class ApproximateNestedSampler(NestedSampler):
+        Args:
+            key: PRNGKey
+            term_cond: termination condition
+            init_state: optional initial state
+
+        Returns:
+            termination reason, and exact state
+        """
+        raise NotImplementedError()
+
+
+class ApproximateNestedSampler(BaseNestedSampler):
     """
-    Performs nested sampling, producing only weakly i.i.d. samples during the shrinkage process.
+    Performs nested sampling, using a chain of nested samplers, producing only weakly i.i.d. samples during the
+    shrinkage process.
     """
+
     def __init__(self, model: Model, num_live_points: Union[int, float], num_parallel_samplers: int,
                  max_samples: Union[int, float],
-                 slice_sampler: Optional[AbstractSliceSampler] = None):
-        super(ApproximateNestedSampler, self).__init__(model=model, num_live_points=num_live_points,
-                                                       num_parallel_samplers=num_parallel_samplers,
-                                                       max_samples=max_samples)
-
-        self.static_uniform = StaticUniform(model=self.model,
-                                            num_live_points=self.num_live_points,
-                                            efficiency_threshold=0.1)
-        if slice_sampler is None:
-            slice_sampler = UniDimSliceSampler(model=model,
-                                               midpoint_shrink=True,
-                                               multi_ellipse_bound=False)
-        self.static_slice = StaticSlice(model=self.model,
-                                        num_live_points=self.num_live_points,
-                                        num_parallel_samplers=self.num_parallel_samplers,
-                                        slice_sampler=slice_sampler,
-                                        num_slices=1)
+                 sampler_chain: Optional[List[AbstractSampler]] = None):
+        super().__init__(model=model, max_samples=max_samples)
 
-    def initialise(self, key: PRNGKey) -> Tuple[NestedSamplerState, LivePoints]:
-        """
-        Creates initial live points from -inf contour and state.
+        if sampler_chain is None:
+            sampler_chain = [
+                UniformSampler(model=model, efficiency_threshold=0.1),
+                UniDimSliceSampler(model=model, num_slices=model.U_ndims * 3, midpoint_shrink=True, perfect=True)
+            ]
+
+        if sampler_chain[-1].efficiency_threshold is not None:
+            if sampler_chain[-1].efficiency_threshold > 0.:
+                logger.warning(
+                    f"Your sampler chain will stop prematurely at an efficiency of "
+                    f"{sampler_chain[-1].efficiency_threshold}. "
+                    f"To change this behaviour, you should ensure the last sampler in your sampler_chain has no "
+                    f"efficiency_threshold set."
+                )
 
-        Args:
-            key: PRNGKey
+        remainder = int(num_live_points) % num_parallel_samplers
+        extra = (num_parallel_samplers - remainder) % num_parallel_samplers
+        if extra > 0:
+            logger.warning(
+                f"Increasing num_live_points ({num_live_points}) by {extra} to closest multiple of num_parallel_samplers.")
+        num_live_points = int(num_live_points + extra)
+        num_parallel_samplers = int(num_parallel_samplers)
 
-        Returns:
-            initial state, and live points
-        """
-        state_key, live_points_key = random.split(key, 2)
-        init_state = NestedSamplerState(
-            key=state_key,
-            sample_collection=init_sample_collection(size=self.max_samples, model=self.model)
-        )
-        live_points = get_uniform_init_live_points(live_points_key,
-                                                   num_live_points=self.num_live_points,
-                                                   model=self.model)
-        return init_state, live_points
+        self._nested_sampler = StaticNestedSampler(samplers=sampler_chain,
+                                                   num_live_points=num_live_points,
+                                                   num_parallel_samplers=num_parallel_samplers)
+
+    @property
+    def num_live_points(self) -> int:
+        return self._nested_sampler.num_live_points
+
+    @property
+    def nested_sampler(self) -> StaticNestedSampler:
+        return self._nested_sampler
+
+    def _run_chain(self, state: NestedSamplerState, live_points: LivePoints, term_cond: TerminationCondition) -> Tuple[
+        IntArray, NestedSamplerState, LivePoints]:
+
+        termination_reason, state, live_points = self._nested_sampler(
+            state=state, live_points=live_points, termination_cond=term_cond)
+        return termination_reason, state, live_points
 
     def approximate_shrinkage(self, state: NestedSamplerState, live_points: LivePoints,
                               term_cond: TerminationCondition) -> Tuple[IntArray, NestedSamplerState]:
         """
         Performs approximate shrinkage using a fast but inaccurate static nested sampler.
 
         Note: samples are not sure to be i.i.d. from within the likelihood constraint.
@@ -224,20 +254,16 @@
             state: initial state
             live_points: initial live points
             term_cond: termination condition
 
         Returns:
             termination reason, and state
         """
-        # Perform uniform "perfect" sampling down to a given efficiency <==> Up to a given X(L)
-        state, live_points = self.static_uniform(state=state, live_points=live_points)
-        # Low accuracy sampling
-        termination_reason, state, live_points = self.static_slice(state=state,
-                                                                   live_points=live_points,
-                                                                   termination_cond=term_cond)
+        termination_reason, state, live_points = self._nested_sampler(
+            state=state, live_points=live_points, termination_cond=term_cond)
         state = collect_samples(state=state, new_reservoir=live_points.reservoir)
         return termination_reason, state
 
     @partial(jit, static_argnums=0)
     def fresh_run(self, key: PRNGKey, term_cond: TerminationCondition) -> Tuple[IntArray, NestedSamplerState]:
         """
         Creates a new initial state and live points from -inf contour and samples until termination.
@@ -245,34 +271,37 @@
         Args:
             key: PRNGKey
             term_cond: termination condition
 
         Returns:
             termination reason, and state
         """
-        state, live_points = self.initialise(key=key)
+        state, live_points = self.initialise(key=key, num_live_points=self.num_live_points)
         return self.approximate_shrinkage(state=state, live_points=live_points, term_cond=term_cond)
 
     @partial(jit, static_argnums=0)
     def concat_run(self, state: NestedSamplerState, live_points: LivePoints,
-                   term_cond: TerminationCondition) -> Tuple[IntArray, NestedSamplerState]:
+                   term_cond: TerminationCondition) -> Tuple[IntArray, NestedSamplerState, LivePoints]:
         """
         Uses a given live points reservoir and performs approximate sampling until termination with a given initial
         state.
 
         Args:
             state: state to augment onto
+            live_points: live points to use
             term_cond: termination condition
 
         Returns:
-            termination reason, and state
+            termination reason, state, and live points
         """
-        return self.approximate_shrinkage(state=state, live_points=live_points, term_cond=term_cond)
+        termination_reason, state, live_points = self._nested_sampler(
+            state=state, live_points=live_points, termination_cond=term_cond)
+        return termination_reason, state, live_points
 
-    @jit
+    @partial(jit, static_argnums=0)
     def augment_run(self, state: NestedSamplerState, term_cond: TerminationCondition) -> Tuple[
         IntArray, NestedSamplerState]:
         """
         Creates a new live points reservoir from -inf contour and performs approximate sampling until termination with
         a given initial state.
 
         Args:
@@ -286,119 +315,92 @@
         state = state._replace(key=key)
         live_points = get_uniform_init_live_points(live_points_key,
                                                    num_live_points=self.num_live_points,
                                                    model=self.model)
         return self.approximate_shrinkage(state=state, live_points=live_points, term_cond=term_cond)
 
     def __call__(self, key: PRNGKey, term_cond: TerminationCondition, *,
-                 init_state: Optional[NestedSamplerState] = None,
-                 live_points: Optional[LivePoints] = None) -> Tuple[IntArray, NestedSamplerState]:
+                 init_state: Optional[NestedSamplerState] = None) -> Tuple[IntArray, NestedSamplerState]:
         """
         Performs approximate nested sampling.
 
         Args:
             key: PRNGKey
             term_cond: termination conditions
             init_state: optional initial state, resume from here if provided
-            live_points: optional initial live points, use if provided otherwise create one
 
         Returns:
             termination reason, state
         """
         if term_cond.max_samples is None:  # add a convenience termination condition for user
             term_cond = term_cond._replace(max_samples=self.max_samples)
-        else:
+        else:  # truncate for sanity
             term_cond = term_cond._replace(max_samples=jnp.minimum(self.max_samples, term_cond.max_samples))
         if init_state is None:
             # We create fresh live points and state
             termination_reason, state = self.fresh_run(key=key, term_cond=term_cond)
         else:
-            if live_points is None:
-                # We create a fresh set of live points from -inf contour and run on top of init_state
-                init_state = self.resize_state(init_state, max_num_samples=self.max_samples)
-                termination_reason, state = self.augment_run(state=init_state, term_cond=term_cond)
-            else:
-                # We use the input live points and run on top of init_state
-                init_state = self.resize_state(init_state, max_num_samples=self.max_samples)
-                termination_reason, state = self.concat_run(state=init_state, live_points=live_points,
-                                                            term_cond=term_cond)
+            # We use the input live points and run on top of init_state
+            init_state = self.resize_state(init_state, max_num_samples=self.max_samples)
+            termination_reason, state = self.augment_run(state=init_state, term_cond=term_cond)
         return termination_reason, state
 
 
-class ExactNestedSampler(NestedSampler):
+class ExactNestedSampler(BaseNestedSampler):
+    """
+    A two stage nested sampler, where the first stage produces sample that are only weakly i.i.d., and the second stage
+    adaptively refines these samples until they are strongly i.i.d. (according to a stopping criterion).
+    """
+
     def __init__(self, model: Model, num_live_points: Union[int, float],
                  max_samples: Union[int, float],
                  num_parallel_samplers: int = 1,
-                 uncert_improvement_patience: int = 2,
-                 shrinkage_slice_sampler: Optional[AbstractSliceSampler] = None,
-                 refinement_slice_sampler: Optional[AbstractSliceSampler] = None):
-        super(ExactNestedSampler, self).__init__(model=model, num_live_points=num_live_points,
-                                                 num_parallel_samplers=num_parallel_samplers,
-                                                 max_samples=max_samples)
+                 patience: int = 1):
+        """
+        A two stage nested sampler, where the first stage produces sample that are only weakly i.i.d., and the
+        second stage adaptively refines these samples until they are strongly i.i.d. (according to a stopping
+        criterion).
+
+        Args:
+            model: model
+            num_live_points: the number of static live points
+            max_samples: maximum number of (non equally weighted) samples to allocate space for.
+                Note: to control stopping criterion related to a maximum number of samples, use TerminationCondition.
+            num_parallel_samplers: the number of parallel instances to run. This must be <= len(jax.devices())
+            patience: how many rounds of converged refinement to wait before stopping.
+                Values > 1 mean refinement will continue until `patience` consecutive rounds of convergence are
+                observed. Similar to famous patience parameter of early stopping in deep learning community.
+        """
+        super(ExactNestedSampler, self).__init__(model=model, max_samples=max_samples)
 
         self.approximate_sampler = ApproximateNestedSampler(
             model=model,
             num_live_points=num_live_points,
             num_parallel_samplers=num_parallel_samplers,
-            max_samples=max_samples,
-            slice_sampler=shrinkage_slice_sampler
+            max_samples=max_samples
         )
 
         self.adaptive_refinement = AdaptiveRefinement(
             model=self.model,
-            uncert_improvement_patience=uncert_improvement_patience,
-            num_slices=model.U_ndims,
-            num_parallel_samplers=self.num_parallel_samplers,
-            slice_sampler=refinement_slice_sampler
+            patience=patience
         )
 
-    def improvement(self, state: NestedSamplerState) -> NestedSamplerState:
-        """
-        Run adaptive refinement until evidence converges.
-
-        Args:
-            state: state (may be approximate, i.e. non-iid samples.)
-
-        Returns:
-            state with samples considered iid sampled from the likelihood constraint
-        """
-        return self.adaptive_refinement(state)
-
-    def prepare_new_iteration(self, state: NestedSamplerState, log_L_constraint: float,
-                              sorted_collection: bool = True) -> Tuple[NestedSamplerState, LivePoints]:
-        """
-        Extract live points from the samples already collected.
-
-        Args:
-            state: the current state
-            log_L_constraint: the contour to sample above
-            sorted_collection: whether the sample collection is already sorted
-
-        Returns:
-            a new state, and live points
-        """
-        return get_live_points_from_samples(state=state, log_L_constraint=log_L_constraint,
-                                            num_live_points=self.num_live_points, sorted_collection=sorted_collection)
-
     def __call__(self, key: PRNGKey, term_cond: TerminationCondition, *,
-                 init_state: Optional[NestedSamplerState] = None,
-                 live_points: Optional[LivePoints] = None) -> Tuple[IntArray, NestedSamplerState]:
+                 init_state: Optional[NestedSamplerState] = None) -> Tuple[IntArray, NestedSamplerState]:
         """
         Performs approximate nested sampling followed by adaptive refinement.
 
         Args:
             key: PRNGKey
             term_cond: termination condition
             init_state: optional initial state
-            live_points: optional initial live points
 
         Returns:
             termination reason, and exact state
         """
         if isinstance(key, core.Tracer):
             raise RuntimeError("Tracer detected, but expected imperative context.")
 
-        termination_reason, state = self.approximate_sampler(key=key, term_cond=term_cond, init_state=init_state,
-                                                             live_points=live_points)
-        state = self.improvement(state=state)
+        termination_reason, state = self.approximate_sampler(key=key, term_cond=term_cond, init_state=init_state)
+        state = self.adaptive_refinement(state=state)
 
         return termination_reason, state
```

### Comparing `jaxns-2.1.0/jaxns/plotting.py` & `jaxns-2.2.0/jaxns/plotting.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.1.0/jaxns/prior.py` & `jaxns-2.2.0/jaxns/prior.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 
 class InvalidPriorName(Exception):
     def __init__(self, name: Optional[str] = None):
         super(InvalidPriorName, self).__init__(f'Prior name {name} already taken by another prior.')
 
 
 def distribution_chain(dist: tfpd.Distribution) -> List[Union[tfpd.TransformedDistribution,
-                                                              tfpd.Sample,
-                                                              tfpd.Distribution]]:
+tfpd.Sample,
+tfpd.Distribution]]:
     chain = []
     while True:
         chain.append(dist)
         if isinstance(dist, tfpd.TransformedDistribution):
             dist = dist.distribution
             continue
         break
@@ -58,14 +58,18 @@
         ...
 
     @abstractmethod
     def _forward(self, U):
         ...
 
     @abstractmethod
+    def _inverse(self, X):
+        ...
+
+    @abstractmethod
     def _log_prob(self, X):
         ...
 
     @property
     def dtype(self):
         return self._dtype()
 
@@ -76,14 +80,17 @@
     @property
     def shape(self) -> Tuple[int, ...]:
         return self._shape()
 
     def forward(self, U):
         return self._forward(U)
 
+    def inverse(self, X):
+        return self._inverse(X)
+
     def log_prob(self, X):
         return self._log_prob(X)
 
 
 class Distribution(AbstractDistribution):
     def __init__(self, dist: tfpd.Distribution):
         self.dist_chain = distribution_chain(dist)
@@ -104,23 +111,32 @@
 
     def _base_shape(self) -> Tuple[int, ...]:
         return tuple(self.dist_chain[0].batch_shape_tensor()) + tuple(self.dist_chain[0].event_shape_tensor())
 
     def _shape(self) -> Tuple[int, ...]:
         return tuple(self.dist_chain[-1].batch_shape_tensor()) + tuple(self.dist_chain[-1].event_shape_tensor())
 
-    def _forward(self, U):
+    def _forward(self, U) -> Union[FloatArray, IntArray, BoolArray]:
         dist = self.dist_chain[0]
         if isinstance(dist, tfpd.Sample):
             dist = dist.distribution
         X = dist.quantile(U)
         for dist in self.dist_chain[1:]:
             X = dist.bijector.forward(X)
         return X
 
+    def _inverse(self, X) -> FloatArray:
+        for dist in reversed(self.dist_chain[1:]):
+            X = dist.bijector.inverse(X)
+        dist = self.dist_chain[0]
+        if isinstance(dist, tfpd.Sample):
+            dist = dist.distribution
+        X = dist.cdf(X)
+        return X
+
     def _log_prob(self, X):
         return self.dist_chain[-1].log_prob(X)
 
 
 class AbstractPrior(ABC):
     def __init__(self, name: Optional[str] = None):
         self.name = name
@@ -141,14 +157,18 @@
         ...
 
     @abstractmethod
     def _forward(self, U) -> Union[FloatArray, IntArray, BoolArray]:
         ...
 
     @abstractmethod
+    def _inverse(self, X) -> FloatArray:
+        ...
+
+    @abstractmethod
     def _log_prob(self, X) -> FloatArray:
         ...
 
     @property
     def dtype(self):
         return self._dtype()
 
@@ -163,33 +183,36 @@
     @property
     def shape(self) -> Tuple[int, ...]:
         return self._shape()
 
     def forward(self, U) -> Union[FloatArray, IntArray, BoolArray]:
         return self._forward(U)
 
+    def inverse(self, X) -> FloatArray:
+        return self._inverse(X)
+
     def log_prob(self, X) -> FloatArray:
         log_prob = self._log_prob(X)
         if log_prob.size > 1:
             log_prob = jnp.sum(log_prob)
         if log_prob.shape != ():
             log_prob = log_prob.reshape(())
         return log_prob
 
 
 class Prior(AbstractPrior):
     def __init__(self, dist_or_value: Union[tfpd.Distribution, jnp.ndarray], name: Optional[str] = None):
         super(Prior, self).__init__(name=name)
         if isinstance(dist_or_value, tfpd.Distribution):
-            self._dist = Distribution(dist_or_value)
             self._type = 'dist'
+            self._dist = Distribution(dist_or_value)
 
         elif isinstance(dist_or_value, (jnp.ndarray, np.ndarray)):
-            self._value = jnp.asarray(dist_or_value)
             self._type = 'value'
+            self._value = jnp.asarray(dist_or_value)
         self.name = name
 
     @property
     def dist(self) -> Distribution:
         if self._type != 'dist':
             raise ValueError(f"Wrong type, got {self._type}")
         return self._dist
@@ -228,14 +251,22 @@
         if self._type == 'value':
             return self.value
         elif self._type == 'dist':
             return self.dist.forward(U)
         else:
             raise NotImplementedError()
 
+    def _inverse(self, X) -> FloatArray:
+        if self._type == 'value':
+            return jnp.asarray([], float_type)
+        elif self._type == 'dist':
+            return self.dist.inverse(X)
+        else:
+            raise NotImplementedError()
+
     def _log_prob(self, X: jnp.ndarray) -> FloatArray:
         if self._type == 'value':
             return jnp.asarray(0., float_type)
         elif self._type == 'dist':
             return self.dist.log_prob(X=X)
         else:
             raise NotImplementedError()
```

### Comparing `jaxns-2.1.0/jaxns/random.py` & `jaxns-2.2.0/jaxns/random.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 
 from jaxns.internals.log_semiring import cumulative_logsumexp
 
 __all__ = ['random_ortho_matrix',
            'resample_indicies']
 
 
-def random_ortho_matrix(key, n):
+def random_ortho_matrix(key, n, special_orthogonal: bool = False):
     """
-    Samples a random orthonormal num_parent,num_parent matrix from Stiefels manifold.
+    Samples a random orthonormal n by n matrix from Stiefels manifold.
     From https://stackoverflow.com/a/38430739
 
     Args:
         key: PRNG seed
         n: Size of matrix, draws from O(num_options) group.
 
     Returns: random [num_options,num_options] matrix with determinant = +-1
     """
     H = random.normal(key, shape=(n, n))
     Q, R = jnp.linalg.qr(H)
+    if special_orthogonal:
+        R *= jnp.sign(R)
     Q = Q @ jnp.diag(jnp.sign(jnp.diag(R)))
     return Q
 
 
 def resample_indicies(key: PRNGKey, log_weights: Optional[FloatArray] = None, S: Optional[int] = None,
                       replace: bool = False, num_total: Optional[int] = None) -> IntArray:
     """
```

### Comparing `jaxns-2.1.0/jaxns/slice_sampler.py` & `jaxns-2.2.0/jaxns/static_slice.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from abc import ABC, abstractmethod
-from typing import NamedTuple, Optional, Tuple, Any
+import logging
+from typing import TypeVar, NamedTuple, Tuple, Optional
 
-from etils.array_types import FloatArray, IntArray, PRNGKey, BoolArray
-from jax import random, numpy as jnp, tree_map
+from etils.array_types import PRNGKey, FloatArray, BoolArray
+from jax import numpy as jnp, random, tree_map
 from jax._src.lax.control_flow import while_loop
 
 from jaxns.model import Model
-from jaxns.types import NestedSamplerState, LivePoints, Sample, int_type, float_type
+from jaxns.static_nested_sampler import MarkovSampler, PreProcessType, SeedPoint
+from jaxns.types import Sample, NestedSamplerState
+from jaxns.types import float_type, int_type
 
-__all__ = ['UniDimSliceSampler']
+logger = logging.getLogger('jaxns')
 
+__all__ = ['UniDimSliceSampler', 'MultiDimSliceSampler']
 
-class SeedPoint(NamedTuple):
-    U0: FloatArray
-    log_L0: FloatArray
+T = TypeVar('T')
 
 
 class UniDimProposalState(NamedTuple):
     key: jnp.ndarray  # PRNG key
     process_step: jnp.ndarray  # what stage of the sampling each independent point is at
     proposal_count: jnp.ndarray  # how many successful proposals have happened for each independent point
     num_likelihood_evaluations: jnp.ndarray  # how many  likelihood evaluations have been made for each independent point
@@ -27,73 +28,47 @@
     left: jnp.ndarray  # the left bound of slice
     right: jnp.ndarray  # the right bound of slice
     point_U: jnp.ndarray  # the point up for likelihood computation
     t: jnp.ndarray  # the parameter measuring between left and right bounds.
     log_L_constraint: jnp.ndarray  # the constraint to sample within
 
 
-PreprocessType = Optional[Any]
+class UniDimSliceSampler(MarkovSampler):
+    """
+    Slice sampler for a single dimension. Produces correlated (non-i.i.d.) samples.
+    """
 
-
-class AbstractSliceSampler(ABC):
-
-    def get_seed_point(self, key: PRNGKey, live_points: LivePoints, log_L_constraint: FloatArray) -> SeedPoint:
-        sample_idx = random.randint(key, (), minval=0, maxval=live_points.reservoir.log_L.size)
-        return SeedPoint(
-            U0=live_points.reservoir.point_U[sample_idx],
-            log_L0=live_points.reservoir.log_L[sample_idx]
-        )
-
-    @abstractmethod
-    def get_sample(self, key: PRNGKey, seed_point: SeedPoint, log_L_constraint: FloatArray, num_slices: IntArray,
-                   preprocess_data: PreprocessType) -> Sample:
+    def __init__(self, model: Model, num_slices: int, midpoint_shrink: bool, perfect: bool,
+                 efficiency_threshold: Optional[float] = None):
         """
-        Get a sample from a given seed point that already satisfied the likelihood constraint.
+        Unidimensional slice sampler.
 
         Args:
-            key: PRNGKey
-            seed_point: the seed point
-            log_L_constraint: likelihood constraint
-            num_slices: how many slices to take per sample
-            preprocess_data: auxilary data specific to the slice sampler that is needed to perform the op.
-
-        Returns:
-            a new sample
-        """
-        ...
-
-    @abstractmethod
-    def preprocess(self, state: NestedSamplerState) -> PreprocessType:
-        """
-        Compute an auxillary object that is needed to perform the slice sampling.
-
-        Args:
-            state: state
-
-        Returns:
-            an object specfic to this sampler's needs
-        """
-        ...
-
-
-class UniDimSliceSampler(AbstractSliceSampler):
-    def __init__(self, model: Model, midpoint_shrink: bool, multi_ellipse_bound: bool = False):
-        self.model = model
+            model: Model
+            num_slices: number of slices between acceptance, in units of 1, unlike other software which does it in units of prior dimension.
+            midpoint_shrink: if true then contract to the midpoint of interval on rejection. Otherwise, contract to
+                rejection point.
+            perfect: if true then perform exponential shrinkage from maximal bounds, requiring no step-out procedure.
+                Otherwise, uses a doubling procedure (exponentially finding bracket).
+                Note: Perfect is a misnomer, as perfection also depends on the number of slices between acceptance.
+        """
+        super().__init__(model=model, efficiency_threshold=efficiency_threshold)
+        if num_slices < 1:
+            raise ValueError(f"num_slices should be > 0, got {num_slices}.")
+        self.num_slices = num_slices
         self.midpoint_shrink = midpoint_shrink
-        self.multi_ellipse_bound = multi_ellipse_bound
-
-    def compute_multi_ellipse_bound(self, state: NestedSamplerState) -> Any:
-        raise NotImplementedError()
+        self.perfect = perfect
 
-    def preprocess(self, state: NestedSamplerState) -> PreprocessType:
-        if self.multi_ellipse_bound:
-            return self.compute_multi_ellipse_bound(state=state)
-        return None
+    def preprocess(self, state: NestedSamplerState) -> PreProcessType:
+        if self.perfect: # nothing needed
+            return ()
+        # else: # step out with doubling
+        #     return multi_ellipsoidal_params()
 
-    def sample_direction(self, n_key: PRNGKey, ndim: int) -> FloatArray:
+    def _sample_direction(self, n_key: PRNGKey, ndim: int) -> FloatArray:
         """
         Choose a direction randomly from S^(D-1).
 
         Args:
             n_key: PRNG key
             ndim: int, number of dimentions
 
@@ -102,15 +77,15 @@
         """
         if ndim == 1:
             return jnp.ones(())
         direction = random.normal(n_key, shape=(ndim,), dtype=float_type)
         direction /= jnp.linalg.norm(direction)
         return direction
 
-    def slice_bounds(self, point_U0: FloatArray, direction: FloatArray) -> Tuple[FloatArray, FloatArray]:
+    def _slice_bounds(self, point_U0: FloatArray, direction: FloatArray) -> Tuple[FloatArray, FloatArray]:
         """
         Compute the slice bounds, t, where point_U0 + direction * t intersects uit cube boundary.
 
         Args:
             point_U0: [D]
             direction: [D]
 
@@ -124,16 +99,16 @@
         t0 = -point_U0 / direction
         t0_right = jnp.min(jnp.where(t0 >= 0., t0, jnp.inf))
         t0_left = jnp.max(jnp.where(t0 <= 0., t0, -jnp.inf))
         right_bound = jnp.minimum(t0_right, t1_right)
         left_bound = jnp.maximum(t0_left, t1_left)
         return left_bound, right_bound
 
-    def pick_point_in_interval(self, t_key: PRNGKey, point_U0: FloatArray, direction: FloatArray, left: FloatArray,
-                               right: FloatArray) -> Tuple[FloatArray, FloatArray]:
+    def _pick_point_in_interval(self, t_key: PRNGKey, point_U0: FloatArray, direction: FloatArray, left: FloatArray,
+                                right: FloatArray) -> Tuple[FloatArray, FloatArray]:
         """
         Select a point along slice in [point_U0 + direction * left, point_U0 + direction * right]
 
         Args:
             t_key: PRNG key
             point_U0: [D]
             direction: [D]
@@ -147,47 +122,47 @@
         t = random.uniform(t_key, minval=left, maxval=right, dtype=float_type)
         point_U = point_U0 + t * direction
         # close_to_zero = (left >= -10*jnp.finfo(left.dtype).eps) & (right <= 10*jnp.finfo(right.dtype).eps)
         # point_U = jnp.where(close_to_zero, point_U0, point_U)
         # t = jnp.where(close_to_zero, jnp.zeros_like(t), t)
         return point_U, t
 
-    def change_direction(self, from_proposal_state: UniDimProposalState,
-                         log_L_proposal: jnp.ndarray) -> UniDimProposalState:
+    def _change_direction(self, from_proposal_state: UniDimProposalState,
+                          log_L_proposal: jnp.ndarray) -> UniDimProposalState:
         """
         Successful proposal, but not enough proposals to de-correlate.
         Pick a new direction and propose from current point.
         """
         proposal_key, n_key, t_key = random.split(from_proposal_state.key, 3)
         point_U0 = from_proposal_state.point_U
         log_L0 = log_L_proposal
-        direction = self.sample_direction(n_key, point_U0.size)
+        direction = self._sample_direction(n_key, point_U0.size)
         # project out the previous direction to sample in orthogonal slice
         if point_U0.size > 1:
             _direction = direction
             direction = direction - direction * (direction @ from_proposal_state.direction)
             direction = jnp.where(jnp.all(direction == jnp.zeros_like(direction)), _direction, direction)
             direction /= jnp.linalg.norm(direction)
 
-        (left, right) = self.slice_bounds(point_U0, direction)
-        point_U, t = self.pick_point_in_interval(t_key, point_U0, direction, left, right)
+        (left, right) = self._slice_bounds(point_U0, direction)
+        point_U, t = self._pick_point_in_interval(t_key, point_U0, direction, left, right)
 
         return from_proposal_state._replace(key=proposal_key,
                                             process_step=jnp.full((), 3, int_type),
                                             point_U0=point_U0,
                                             log_L0=log_L0,
                                             direction=direction,
                                             left=left,
                                             right=right,
                                             point_U=point_U,
                                             t=t)
 
-    def shrink_interval(self, from_proposal_state: UniDimProposalState, log_L_proposal: jnp.ndarray,
-                        log_L_contour: jnp.ndarray,
-                        midpoint_shrink: bool, destructive_shrink: bool) -> UniDimProposalState:
+    def _shrink_interval(self, from_proposal_state: UniDimProposalState, log_L_proposal: jnp.ndarray,
+                         log_L_contour: jnp.ndarray,
+                         midpoint_shrink: bool, destructive_shrink: bool) -> UniDimProposalState:
         """
         Not successful proposal, so shrink, optionally apply exponential shrinkage.
         """
         # witout exponential shrinkage, we shrink to failed proposal point, which is 100% correct.
         left = jnp.where(from_proposal_state.t < 0., from_proposal_state.t, from_proposal_state.left)
         right = jnp.where(from_proposal_state.t > 0., from_proposal_state.t, from_proposal_state.right)
         key, t_key, midpoint_key = random.split(from_proposal_state.key, 3)
@@ -220,32 +195,31 @@
             alpha = random.uniform(alpha_key)
             beta = random.uniform(beta_key)
             logL_alpha = from_proposal_state.log_L0 + alpha * (log_L_proposal - from_proposal_state.log_L0)
             logL_beta = log_L_proposal + beta * (log_L_contour - log_L_proposal)
             do_mid_point_shrink = logL_alpha < logL_beta
             left = jnp.where((from_proposal_state.t < 0.) & do_mid_point_shrink, alpha * left, left)
             right = jnp.where((from_proposal_state.t > 0.) & do_mid_point_shrink, alpha * right, right)
-        point_U, t = self.pick_point_in_interval(t_key, from_proposal_state.point_U0, from_proposal_state.direction,
-                                                 left, right)
+        point_U, t = self._pick_point_in_interval(t_key, from_proposal_state.point_U0, from_proposal_state.direction,
+                                                  left, right)
         return from_proposal_state._replace(key=key,
                                             process_step=jnp.full((), 3, int_type),
                                             left=left,
                                             right=right,
                                             point_U=point_U,
                                             t=t)
 
-    def get_sample(self, key: PRNGKey, seed_point: SeedPoint, log_L_constraint: FloatArray, num_slices: IntArray,
-                   preprocess_data: PreprocessType) -> Sample:
-
+    def get_sample_from_seed(self, key: PRNGKey, seed_point: SeedPoint, log_L_constraint: FloatArray,
+                             preprocess_data: PreProcessType) -> Sample:
         slice_sampler_key, select_key, proposal_key, n_key, t_key = random.split(key, 5)
 
-        direction = self.sample_direction(n_key, seed_point.U0.size)
+        direction = self._sample_direction(n_key, seed_point.U0.size)
         num_likelihood_evaluations = jnp.full((), 0, int_type)
-        (left, right) = self.slice_bounds(seed_point.U0, direction)
-        point_U, t = self.pick_point_in_interval(t_key, seed_point.U0, direction, left, right)
+        (left, right) = self._slice_bounds(seed_point.U0, direction)
+        point_U, t = self._pick_point_in_interval(t_key, seed_point.U0, direction, left, right)
         init_proposal_state = UniDimProposalState(key=proposal_key,
                                                   process_step=jnp.full((), 3, int_type),
                                                   proposal_count=jnp.zeros((), int_type),
                                                   num_likelihood_evaluations=num_likelihood_evaluations,
                                                   point_U0=seed_point.U0,
                                                   log_L0=seed_point.log_L0,
                                                   direction=direction,
@@ -279,15 +253,15 @@
             proposal_state = proposal_state._replace(log_L_constraint=safe_log_L_constraint)
             good_proposal = good_proposal | potential_instability
 
             proposal_count = jnp.where(good_proposal,
                                        proposal_state.proposal_count + jnp.ones_like(proposal_state.proposal_count),
                                        proposal_state.proposal_count)
 
-            enough_proposals = proposal_count >= num_slices
+            enough_proposals = proposal_count >= self.num_slices
 
             # 0: successful proposal & enough proposals -> done
             # 1: successful proposal & not enough proposals -> change direction
             # 2: unsuccessful proposal -> shrink interval
 
             process_step = jnp.where(enough_proposals,
                                      jnp.full(good_proposal.shape, 0, int_type),
@@ -296,19 +270,19 @@
                                                jnp.full(good_proposal.shape, 2, int_type)
                                                )
                                      )
 
             def _map_where(cond, a_tree, b_tree):
                 return tree_map(lambda a, b: jnp.where(cond, a, b), a_tree, b_tree)
 
-            proposal_state_from_1 = self.change_direction(proposal_state, log_L_point_U)
-            proposal_state_from_2 = self.shrink_interval(proposal_state, log_L_point_U,
-                                                         log_L_contour=proposal_state.log_L_constraint,
-                                                         midpoint_shrink=self.midpoint_shrink,
-                                                         destructive_shrink=False)
+            proposal_state_from_1 = self._change_direction(proposal_state, log_L_point_U)
+            proposal_state_from_2 = self._shrink_interval(proposal_state, log_L_point_U,
+                                                          log_L_contour=proposal_state.log_L_constraint,
+                                                          midpoint_shrink=self.midpoint_shrink,
+                                                          destructive_shrink=False)
 
             # replace with the proposal state as appropriate
 
             proposal_state = _map_where(process_step == 1,
                                         proposal_state_from_1, proposal_state)
             proposal_state = _map_where(process_step == 2,
                                         proposal_state_from_2, proposal_state)
@@ -319,28 +293,28 @@
             return (proposal_state, log_L_point_U)
 
         def slice_sampler_cond(body_state: CarryType) -> BoolArray:
             """
             Stops when there have been enough proposals.
             """
             (proposal_state, _) = body_state
-            return jnp.less(proposal_state.proposal_count, num_slices)
+            return jnp.less(proposal_state.proposal_count, self.num_slices)
 
         (proposal_state, log_L) = while_loop(slice_sampler_cond,
                                              slice_sampler_body,
                                              (init_proposal_state, -jnp.inf))
-        # passthrough when num_slices==0
-        pass_through = num_slices == jnp.zeros_like(num_slices)
+        # when num_slices==0, that means we don't want to run this
+        pass_through = self.num_slices == jnp.zeros_like(self.num_slices)
         log_L = jnp.where(pass_through, seed_point.log_L0, log_L)
         point_U = jnp.where(pass_through, seed_point.U0, proposal_state.point_U)
         sample = Sample(point_U=point_U,
                         log_L_constraint=proposal_state.log_L_constraint,
                         log_L=log_L,
                         num_likelihood_evaluations=proposal_state.num_likelihood_evaluations,
-                        num_slices=num_slices,
+                        num_slices=self.num_slices,
                         iid=jnp.asarray(False, jnp.bool_))
         return sample
 
 
 class MultiDimProposalState(NamedTuple):
     key: jnp.ndarray  # PRNG key
     process_step: jnp.ndarray  # what stage of the sampling each independent point is at
@@ -349,28 +323,43 @@
     point_U0: jnp.ndarray  # the origin of current slice of each independent point
     log_L0: jnp.ndarray  # the value of log-likelihood at each indpendent point origin
     left: jnp.ndarray  # the left bound of slice
     right: jnp.ndarray  # the right bound of slice
     point_U: jnp.ndarray  # the point up for likelihood computation
 
 
-class MultiDimSliceSampler(AbstractSliceSampler):
-    def __init__(self, model: Model, num_restrict_dims: Optional[int] = None):
-        self.model = model
+class MultiDimSliceSampler(MarkovSampler):
+    def __init__(self, model: Model, num_slices: int, num_restrict_dims: Optional[int] = None,
+                 efficiency_threshold: Optional[float] = None):
+        """
+        Multi-dimensional slice sampler, with exponential shrinkage. Produces correlated (non-i.i.d.) samples.
+
+        Notes: Not very efficient.
+
+        Args:
+            model: Model
+            num_slices: number of slices between acceptance, in units of 1, unlike other software which does it in units of prior dimension.
+            num_restrict_dims: size of subspace to slice along. Setting to 1 would be like UniDimSliceSampler,
+                but far less efficient.
+        """
+        super().__init__(model=model, efficiency_threshold=efficiency_threshold)
+        if num_slices < 1:
+            raise ValueError(f"num_slices must be > 0.")
+        self.num_slices = num_slices
         if num_restrict_dims is not None:
             if num_restrict_dims == 1:
                 raise ValueError(f"If restricting to 1 dimension, then you should use UniDimSliceSampler.")
             if not (1 < num_restrict_dims <= model.U_ndims):
                 raise ValueError(f"Expected num_restriction dim in (1, {model.U_ndims}], got {num_restrict_dims}.")
         self.num_restrict_dims = num_restrict_dims
 
-    def preprocess(self, state: NestedSamplerState) -> PreprocessType:
-        return None
+    def preprocess(self, state: NestedSamplerState) -> PreProcessType:
+        return ()
 
-    def slice_bounds(self, key: PRNGKey, point_U0: FloatArray) -> Tuple[FloatArray, FloatArray]:
+    def _slice_bounds(self, key: PRNGKey, point_U0: FloatArray) -> Tuple[FloatArray, FloatArray]:
         """
         Get the slice bounds, randomly selecting which dimensions to slice in.
 
         Args:
             key: PRNGKey
             point_U0: the seed point
 
@@ -382,18 +371,18 @@
             left = point_U0.at[slice_dims].set(jnp.zeros(self.num_restrict_dims, point_U0.dtype))
             right = point_U0.at[slice_dims].set(jnp.ones(self.num_restrict_dims, point_U0.dtype))
         else:
             left = jnp.zeros_like(point_U0)
             right = jnp.ones_like(point_U0)
         return left, right
 
-    def new_slice(self, proposal_state: MultiDimProposalState, log_L_U: FloatArray) -> MultiDimProposalState:
+    def _new_slice(self, proposal_state: MultiDimProposalState, log_L_U: FloatArray) -> MultiDimProposalState:
         key, slice_key, sample_key = random.split(proposal_state.key, 3)
 
-        left, right = self.slice_bounds(key=slice_key, point_U0=proposal_state.point_U0)
+        left, right = self._slice_bounds(key=slice_key, point_U0=proposal_state.point_U0)
 
         point_U = random.uniform(key=sample_key, shape=left.shape, dtype=left.dtype, minval=left, maxval=right)
 
         next_proposal_state = MultiDimProposalState(
             key=key,
             process_step=jnp.full((), 3, int_type),
             proposal_count=proposal_state.proposal_count,
@@ -402,15 +391,15 @@
             log_L0=log_L_U,
             left=left,
             right=right,
             point_U=point_U
         )
         return next_proposal_state
 
-    def shrink_region(self, proposal_state: MultiDimProposalState) -> MultiDimProposalState:
+    def _shrink_region(self, proposal_state: MultiDimProposalState) -> MultiDimProposalState:
         # if point_U is on the 'right' side then we shrink the 'right' side to it.
         # same of 'left'
         left = jnp.where(proposal_state.point_U < proposal_state.point_U0,
                          jnp.maximum(proposal_state.left, proposal_state.point_U),
                          proposal_state.left)
         right = jnp.where(proposal_state.point_U > proposal_state.point_U0,
                           jnp.minimum(proposal_state.right, proposal_state.point_U),
@@ -426,21 +415,21 @@
             left=left,
             right=right,
             point_U=point_U
         )
 
         return next_proposal_state
 
-    def get_sample(self, key: PRNGKey, seed_point: SeedPoint, log_L_constraint: FloatArray, num_slices: IntArray,
-                   preprocess_data: PreprocessType) -> Sample:
+    def get_sample_from_seed(self, key: PRNGKey, seed_point: SeedPoint, log_L_constraint: FloatArray,
+                             preprocess_data: PreProcessType) -> Sample:
         slice_key, sample_key, proposal_key = random.split(key, 3)
 
         num_likelihood_evaluations = jnp.full((), 0, int_type)
 
-        left, right = self.slice_bounds(key=slice_key, point_U0=seed_point.U0)
+        left, right = self._slice_bounds(key=slice_key, point_U0=seed_point.U0)
 
         point_U = random.uniform(key=sample_key, shape=left.shape, dtype=left.dtype, minval=left, maxval=right)
 
         init_proposal_state = MultiDimProposalState(key=proposal_key,
                                                     process_step=jnp.full((), 3, int_type),
                                                     proposal_count=jnp.zeros((), int_type),
                                                     num_likelihood_evaluations=num_likelihood_evaluations,
@@ -463,15 +452,15 @@
                 proposal_state.num_likelihood_evaluations)
             # assumes that log_L0 > log_L_constraint
             good_proposal = jnp.greater(log_L_point_U, log_L_constraint)
             proposal_count = jnp.where(good_proposal,
                                        proposal_state.proposal_count + jnp.ones_like(proposal_state.proposal_count),
                                        proposal_state.proposal_count)
 
-            enough_proposals = proposal_count >= num_slices
+            enough_proposals = proposal_count >= self.num_slices
 
             # 0: successful proposal & enough proposals -> done
             # 1: successful proposal & not enough proposals -> change direction
             # 2: unsuccessful proposal -> shrink interval
 
             process_step = jnp.where(good_proposal & enough_proposals,
                                      jnp.full(good_proposal.shape, 0, int_type),
@@ -480,16 +469,16 @@
                                                jnp.full(good_proposal.shape, 2, int_type)
                                                )
                                      )
 
             def _map_where(cond, a_tree, b_tree):
                 return tree_map(lambda a, b: jnp.where(cond, a, b), a_tree, b_tree)
 
-            proposal_state_from_1 = self.new_slice(proposal_state, log_L_point_U)
-            proposal_state_from_2 = self.shrink_region(proposal_state)
+            proposal_state_from_1 = self._new_slice(proposal_state, log_L_point_U)
+            proposal_state_from_2 = self._shrink_region(proposal_state)
 
             # replace with the proposal state as appropriate
 
             proposal_state = _map_where(process_step == 1, proposal_state_from_1, proposal_state)
             proposal_state = _map_where(process_step == 2, proposal_state_from_2, proposal_state)
 
             proposal_state = proposal_state._replace(process_step=process_step,
@@ -498,24 +487,19 @@
             return (proposal_state, log_L_point_U)
 
         def slice_sampler_cond(body_state: CarryType) -> BoolArray:
             """
             Stops when there have been enough proposals.
             """
             (proposal_state, _) = body_state
-            return jnp.bitwise_not(proposal_state.proposal_count >= num_slices)
+            return jnp.bitwise_not(proposal_state.proposal_count >= self.num_slices)
 
         (proposal_state, log_L) = while_loop(slice_sampler_cond,
                                              slice_sampler_body,
                                              (init_proposal_state, -jnp.inf))
-        # TODO(Joshuaalbert): consider removing pass_through as there is no case where num_slices is ever 0 now.
-        # passthrough when num_slices==0
-        pass_through = num_slices == jnp.zeros_like(num_slices)
-        log_L = jnp.where(pass_through, seed_point.log_L0, log_L)
-        point_U = jnp.where(pass_through, seed_point.U0, proposal_state.point_U)
         sample = Sample(point_U=point_U,
                         log_L_constraint=log_L_constraint,
                         log_L=log_L,
                         num_likelihood_evaluations=proposal_state.num_likelihood_evaluations,
-                        num_slices=num_slices,
+                        num_slices=self.num_slices,
                         iid=jnp.asarray(False, jnp.bool_))
         return sample
```

### Comparing `jaxns-2.1.0/jaxns/special_priors.py` & `jaxns-2.2.0/jaxns/special_priors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
 from typing import Tuple, Union, Optional, Literal
 
 import tensorflow_probability.substrates.jax as tfp
 from etils.array_types import FloatArray, IntArray, BoolArray
-from jax import numpy as jnp
+from jax import numpy as jnp, vmap
 from jax._src.lax.control_flow import while_loop, scan
-from jax._src.scipy.special import logsumexp, gammaln
+from jax._src.scipy.special import gammaln
 from tensorflow_probability.substrates.jax.math import lbeta, betaincinv
 
+from jaxns.internals.log_semiring import cumulative_logsumexp
 from jaxns.prior import AbstractPrior
 from jaxns.types import float_type
 
 logger = logging.getLogger('jaxns')
 tfpd = tfp.distributions
 
 __all__ = [
@@ -36,14 +37,17 @@
 
     def _shape(self) -> Tuple[int, ...]:
         return tuple(self.dist.batch_shape_tensor()) + tuple(self.dist.event_shape_tensor())
 
     def _forward(self, U) -> Union[FloatArray, IntArray, BoolArray]:
         return self._quantile(U)
 
+    def _inverse(self, X) -> FloatArray:
+        return self.dist.cdf(X)
+
     def _log_prob(self, X) -> FloatArray:
         return self.dist.log_prob(X)
 
     def _quantile(self, U):
         probs = self.dist._probs_parameter_no_checks()
         sample = jnp.less(U, probs)
         return sample.astype(self.dtype)
@@ -62,14 +66,17 @@
 
     def _shape(self) -> Tuple[int, ...]:
         return tuple(self.dist.batch_shape_tensor()) + tuple(self.dist.event_shape_tensor())
 
     def _forward(self, U) -> Union[FloatArray, IntArray, BoolArray]:
         return self._quantile(U)
 
+    def _inverse(self, X) -> FloatArray:
+        return self.dist.cdf(X)
+
     def _log_prob(self, X) -> FloatArray:
         return self.dist.log_prob(X)
 
     def _quantile(self, U):
         alpha = self.dist.concentration0
         beta = self.dist.concentration1
         # cdf(x, a, b) = I(x,a,b) = B(x,a,b)/B(a,b)
@@ -79,14 +86,24 @@
         X = betaincinv(alpha, beta, Y)
         return X.astype(self.dtype)
 
 
 class Categorical(AbstractPrior):
     def __init__(self, parametrisation: Literal['gumbel_max', 'cdf'], *, logits=None, probs=None,
                  name: Optional[str] = None):
+        """
+        Initialised Categorical special prior.
+
+        Args:
+            parametrisation: 'cdf' is good for discrete params with correlation between neighbouring categories,
+                otherwise gumbel is better.
+            logits: log-prob of each category
+            probs: prob of each category
+            name: optional name
+        """
         super(Categorical, self).__init__(name=name)
         self.dist = tfpd.Categorical(logits=logits, probs=probs)
         self._parametrisation = parametrisation
 
     def _dtype(self):
         return self.dist.dtype
 
@@ -101,49 +118,47 @@
 
     def _forward(self, U) -> Union[FloatArray, IntArray, BoolArray]:
         if self._parametrisation == 'gumbel_max':
             return self._quantile_gumbelmax(U)
         elif self._parametrisation == 'cdf':
             return self._quantile_cdf(U)
 
+    def _inverse(self, X) -> FloatArray:
+        return self.dist.cdf(X)
+
     def _log_prob(self, X) -> FloatArray:
         return self.dist.log_prob(X)
 
     def _quantile_gumbelmax(self, U):
         logits = self.dist._logits_parameter_no_checks()
         sample_dtype = self.dtype
         z = -jnp.log(-jnp.log(U))  # gumbel
         draws = jnp.argmax(logits + z, axis=-1).astype(sample_dtype)
         return draws
 
     def _quantile_cdf(self, U):
+        """
+        The quantile for CDF parametrisation.
+
+        Args:
+            U: [...]
+
+        Returns:
+            [...]
+        """
         logits = self.dist._logits_parameter_no_checks()  # [..., N]
-        logits = jnp.swapaxes(logits, axis1=0, axis2=-1)  # [N, ...]
-        # normalise logits
-        logits -= logsumexp(logits, axis=0, keepdims=True)
-        log_u = jnp.log(U)
-
-        # parallel CDF sampling, imputing the done ones
-        def body(state):
-            (_, accumulant, i, output) = state
-            new_accumulant = jnp.logaddexp(accumulant, logits[i])
-            done = log_u < new_accumulant
-            output = jnp.where(done, output, i + 1)
-            return (done, new_accumulant, i + 1, output)
-
-        loop_vars = (
-            jnp.zeros(self.base_shape, dtype=jnp.bool_),
-            -jnp.inf * jnp.ones(self.base_shape, dtype=U.dtype),
-            jnp.asarray(0, self.dtype),
-            jnp.zeros(self.base_shape, dtype=self.dtype)
-        )
-        (_, _, _, output) = while_loop(lambda state: ~jnp.all(state[0]),
-                                       body,
-                                       loop_vars)
-        return output
+        cum_logits = cumulative_logsumexp(logits, axis=-1)  # [..., N]
+        cum_logits -= cum_logits[..., -1:]
+        N = cum_logits.shape[-1]
+        cum_logits_flat = jnp.reshape(cum_logits, (-1, N))
+        log_U_flat = jnp.reshape(jnp.log(U), (-1,))
+
+        category_flat = vmap(lambda a, v: jnp.searchsorted(a, v, side='left'))(cum_logits_flat, log_U_flat)
+        category = jnp.reshape(category_flat, U.shape)
+        return category
 
 
 class ForcedIdentifiability(AbstractPrior):
     """
     Prior for a sequence of `n` random variables uniformly distributed on U[low, high] such that U[i,...] <= U[i+1,...].
     For broadcasting the resulting random variable is sorted on the first dimension elementwise.
 
@@ -168,32 +183,50 @@
 
     def _shape(self) -> Tuple[int, ...]:
         return (self.n,) + jnp.shape(self.low)
 
     def _forward(self, U) -> Union[FloatArray, IntArray, BoolArray]:
         return self._quantile(U)
 
+    def _inverse(self, X) -> FloatArray:
+        return self._cdf(X)
+
     def _log_prob(self, X) -> FloatArray:
         log_n_fac = gammaln(self.n + 1)
         diff = self.high - self.low
         log_prob = - log_n_fac - self.n * jnp.log(diff)
         # no check that X is inside high and low
         return log_prob
 
+    def _cdf(self, X):
+        log_theta = jnp.log((X - self.low) / (self.high - self.low))  # [n, ...]
+
+        def inv_body(state, X):
+            (log_theta_prev,) = state
+            (log_theta, i) = X
+            log_x = i * (log_theta - log_theta_prev)
+            return (log_theta,), (log_x,)
+
+        # Initial log_x value
+        log_init_x = jnp.zeros(self.shape[1:], self.dtype)  # [...]
+        _, (log_x,) = scan(inv_body, (log_init_x,), (log_theta, jnp.arange(1, self.n + 1)), reverse=True)
+        U = jnp.exp(log_x)
+        return U.astype(self.dtype)
+
     def _quantile(self, U):
         log_x = jnp.log(U)  # [n, ...]
 
         # theta[i] = theta[i-1] * (1 - x[i]) + theta_max * x[i]
         def body(state, X):
             (log_theta,) = state
             (log_x, i) = X
-            log_theta = log_x / i + log_theta
+            log_theta = log_x / i + log_theta  # shrinkage
             return (log_theta,), (log_theta,)
 
-        log_init_theta = jnp.zeros(self.shape[1:], self.dtype)  # [...]
+        log_init_theta = jnp.zeros(self.shape[1:], self.dtype)  # [...] -- log(1)
         _, (log_theta,) = scan(body, (log_init_theta,), (log_x, jnp.arange(1, self.n + 1)), reverse=True)
         theta = self.low + (self.high - self.low) * jnp.exp(log_theta)
         return theta.astype(self.dtype)
 
 
 class Poisson(AbstractPrior):
     def __init__(self, *, rate=None, log_rate=None, name: Optional[str] = None):
@@ -208,14 +241,17 @@
 
     def _shape(self) -> Tuple[int, ...]:
         return tuple(self.dist.batch_shape_tensor()) + tuple(self.dist.event_shape_tensor())
 
     def _forward(self, U) -> Union[FloatArray, IntArray, BoolArray]:
         return self._quantile(U)
 
+    def _inverse(self, X) -> FloatArray:
+        return self.dist.cdf(X)
+
     def _log_prob(self, X) -> FloatArray:
         return self.dist.log_prob(X)
 
     def _quantile(self, U):
         """
         Algorithmic Poisson generator based upon the inversion by sequential search
```

### Comparing `jaxns-2.1.0/jaxns/statistics.py` & `jaxns-2.2.0/jaxns/statistics.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-from typing import Tuple, Union
+from typing import Tuple, Union, List
 
 from etils.array_types import FloatArray, IntArray
-from jax import numpy as jnp, tree_map, random
+from jax import numpy as jnp, tree_map
 from jax._src.lax.control_flow import while_loop
 from jax._src.lax.slicing import dynamic_update_slice
 
-from jaxns.internals.log_semiring import LogSpace, normalise_log_space
-from jaxns.internals.maps import replace_index
-from jaxns.internals.stats import linear_to_log_stats
-from jaxns.types import EvidenceCalculation, SampleCollection, SampleStatistics, float_type, int_type
-from jaxns.types import NestedSamplerState
+from jaxns.internals.log_semiring import LogSpace
+from jaxns.types import EvidenceCalculation, SampleCollection, SampleStatistics, float_type, int_type, Reservoir
 
 __all__ = ['compute_evidence',
            'analyse_sample_collection',
            'compute_num_live_points_from_unit_threads']
 
 
 def _init_evidence_calculation() -> EvidenceCalculation:
@@ -193,14 +190,101 @@
         sample_collection=sample_collection,
         num_live_points=num_live_points
     )
 
     return evidence_calculation, sample_stats
 
 
+def perfect_live_point_computation_jax(log_L_constraints: jnp.ndarray, log_L_samples: jnp.ndarray,
+                                       num_samples: Union[jnp.ndarray, None] = None):
+    # log_L_constraints has shape [N]
+    # log_L_samples has shape [N]
+    sort_idx = jnp.lexsort((log_L_constraints, log_L_samples))
+    log_L_samples = log_L_samples[sort_idx]
+    log_L_constraints = log_L_constraints[sort_idx]
+    log_L_contour = log_L_constraints[0]
+
+    def outer_cond(state):
+        (i, log_L_contour, log_L_samples, log_L_constraints, num_live_points) = state
+        return i < log_L_samples.size
+
+    def outer_loop_body(state):
+        (i, log_L_contour, log_L_samples, log_L_constraints, num_live_points) = state
+        log_L_dead = log_L_samples[i]
+
+        def inner_cond(state):
+            (i, log_L_samples, log_L_constraints, num_live_points) = state
+            return jnp.bitwise_and(log_L_samples[i] == log_L_dead, i < log_L_constraints.size)
+
+        def inner_loop_body(state):
+            (i, log_L_samples, log_L_constraints, num_live_points) = state
+            count = jnp.sum(jnp.bitwise_and(log_L_contour < log_L_samples, log_L_constraints <= log_L_contour))
+            log_L_samples = log_L_samples.at[i].set(-jnp.inf)
+            log_L_constraints = log_L_constraints.at[i].set(jnp.inf)
+            num_live_points = num_live_points.at[i].set(count.astype(log_L_samples.dtype))
+            return (i + 1, log_L_samples, log_L_constraints, num_live_points)
+
+        (i, log_L_samples, log_L_constraints, num_live_points) = while_loop(
+            inner_cond,
+            inner_loop_body,
+            (i, log_L_samples, log_L_constraints, num_live_points)
+        )
+        log_L_contour = log_L_dead
+        return (i, log_L_contour, log_L_samples, log_L_constraints, num_live_points)
+
+    (i, log_L_contour, log_L_samples, log_L_constraints, num_live_points) = while_loop(
+        outer_cond,
+        outer_loop_body,
+        (jnp.asarray(0, int_type), log_L_contour, log_L_samples, log_L_constraints, jnp.zeros_like(log_L_samples))
+    )
+    if num_samples is not None:
+        empty_mask = jnp.greater_equal(jnp.arange(log_L_samples.size), num_samples)
+        num_live_points = jnp.where(empty_mask, 0, num_live_points)
+    return num_live_points, sort_idx
+
+
+def fast_triu_rowsum(a, b):
+    """
+    Computes a fast row sum of the upper triangular part of the outer product of a and b.
+
+    Args:
+        a: [N] array
+        b: [N] array
+
+    Returns:
+        [N] of the row sum of upper trianguarl part of outer product of a and b.
+    """
+    b_cumsum_rev = jnp.cumsum(b[::-1])[::-1]
+    return a * b_cumsum_rev
+
+
+def fast_perfect_live_point_computation_jax(log_L_constraints: jnp.ndarray, log_L_samples: jnp.ndarray,
+                                            num_samples: Union[jnp.ndarray, None] = None):
+    # log_L_constraints has shape [N]
+    # log_L_samples has shape [N]
+    sort_idx = jnp.lexsort((log_L_constraints, log_L_samples))
+    log_L_samples = log_L_samples[sort_idx]
+    log_L_constraints = log_L_constraints[sort_idx]
+    log_L_contour = log_L_constraints[0]
+    search_contours = jnp.concatenate([log_L_contour[None], log_L_samples], axis=0)
+
+    contour_map_idx = jnp.searchsorted(search_contours, log_L_samples, side='left') - 1
+    log_L_contours = search_contours[contour_map_idx]
+    diag_i = jnp.arange(log_L_samples.size)
+    right_most_idx = jnp.searchsorted(jnp.sort(log_L_constraints), log_L_contours, side='right') - 1
+    left_most_idx = jnp.maximum(diag_i, jnp.searchsorted(log_L_samples, log_L_contours, side='right') - 1)
+    num_live_points = jnp.maximum(0, right_most_idx - left_most_idx + 1)
+
+    if num_samples is not None:
+        empty_mask = jnp.greater_equal(jnp.arange(log_L_samples.size), num_samples)
+        num_live_points = jnp.where(empty_mask, jnp.asarray(0., log_L_samples.dtype), num_live_points)
+
+    return num_live_points, sort_idx
+
+
 def compute_num_live_points_from_unit_threads(log_L_constraints: FloatArray, log_L_samples: FloatArray,
                                               num_samples: IntArray = None, sorted_collection: bool = True) \
         -> Union[FloatArray, Tuple[FloatArray, IntArray]]:
     """
     Compute the number of live points of shrinkage distribution, from an arbitrary list of samples with
     corresponding sampling constraints.
 
@@ -211,77 +295,22 @@
 
     Returns:
         if sorted_collection is true:
             num_live_points for shrinkage distribution
         otherwise:
             num_live_points for shrinkage distribution, and sort indicies
     """
-    # mask the samples that are not yet taken
-
-    if num_samples is None:
-        num_samples = log_L_samples.size
-    empty_mask = jnp.greater_equal(jnp.arange(log_L_samples.size), num_samples)
-
-    # masking samples is already done, since they are inf by default.
-    # log_L_samples = jnp.where(empty_mask, jnp.inf, log_L_samples)
-    # log_L_constraints = jnp.where(empty_mask, jnp.inf, log_L_constraints)
-    # sort log_L_samples, breaking degeneracies on log_L_constraints
+    num_live_points, sort_idx = fast_perfect_live_point_computation_jax(log_L_constraints=log_L_constraints,
+                                                                        log_L_samples=log_L_samples,
+                                                                        num_samples=num_samples)
 
     if not sorted_collection:
-        idx_sort = jnp.lexsort((log_L_constraints, log_L_samples))
-        log_L_samples = log_L_samples[idx_sort]
-        log_L_constraints = log_L_constraints[idx_sort]
-        empty_mask = empty_mask[idx_sort]
-
-    # n = jnp.sum(available & (log_L_samples >= contour) & (log_L_constraints <= contour))
-    # n = jnp.sum(available & (log_L_constraints <= contour))
-    # n = available.size - jnp.sum(jnp.bitwise_not(available) | jnp.bitwise_not(log_L_constraints <= contour))
-    # n = available.size - jnp.sum(jnp.bitwise_not(available)) - jnp.sum(jnp.bitwise_not(log_L_constraints <= contour)) + jnp.sum(jnp.bitwise_not(available) & jnp.bitwise_not(log_L_constraints <= contour))
-    # n = jnp.sum(available) - jnp.sum(log_L_constraints > contour) + jnp.sum(jnp.bitwise_not(available) & (log_L_constraints > contour))
-    # Since jnp.sum(jnp.bitwise_not(available) & (log_L_constraints > contour)) can be shown to be zero
-    # n = jnp.sum(available) - jnp.sum(log_L_constraints > contour)
-
-    _log_L_samples = jnp.concatenate([log_L_constraints[0:1], log_L_samples])
-    n_base = jnp.arange(1, log_L_samples.size + 1)[::-1]
-
-    # jnp.sum(log_L_samples[idx-1] < log_L_constraints)
-
-    u = jnp.searchsorted(_log_L_samples, log_L_constraints, side='left')
-    b = u.size - jnp.cumsum(jnp.bincount(u, length=u.size))
-    n = n_base - b
-    n = jnp.where(empty_mask, 0, n)
-    n = jnp.asarray(n, log_L_samples.dtype)
-    if not sorted_collection:
-        return (n, idx_sort)
-    return n
+        return num_live_points, sort_idx
 
-
-def sample_goal_distribution(key, log_goal_weights, S: int, *, replace: bool = True):
-    """
-    Sample indices that match unnormalised log_probabilities.
-
-    Args:
-        key: PRNG key
-        log_goal_weights: unnormalised log probabilities
-        S: number of samples
-        replace: bool, whether to sample with replacement
-
-    Returns:
-        indices that draw from target density
-    """
-    if replace:
-        p_cuml = LogSpace(log_goal_weights).cumsum()
-        # 1 - U in (0,1] instead of [0,1)
-        r = p_cuml[-1] * LogSpace(jnp.log(1 - random.uniform(key, (S,))))
-        idx = jnp.searchsorted(p_cuml.log_abs_val, r.log_abs_val)
-    else:
-        assert S <= log_goal_weights.size
-        g = -random.gumbel(key, shape=log_goal_weights.shape) - log_goal_weights
-        idx = jnp.argsort(g)[:S]
-    return idx
+    return num_live_points
 
 
 def compute_remaining_evidence(sample_idx, log_dZ_mean):
     # Z_remaining = dZ_mean.cumsum(reverse=True)
 
     def logsumexp_cumsum_body(_state):
         (log_abs_val, idx) = _state
@@ -295,90 +324,54 @@
     (log_Z_remaining, _) = while_loop(lambda _state: _state[1] > 0,
                                       logsumexp_cumsum_body,
                                       (log_dZ_mean,
                                        sample_idx - jnp.ones_like(sample_idx)))
     return log_Z_remaining
 
 
-def evidence_goal(state: NestedSamplerState):
+def combine_reservoirs(*reservoirs: Reservoir) -> Tuple[Reservoir, jnp.ndarray]:
     """
-    Estimates the impact of adding a sample at a certain likelihood contour by computing the impact of removing a point.
+    Combine two reservoirs sorting, and updating the number of live points properly.
 
     Args:
-        state:
+        *reservoirs: Reservoirs to combine.
 
     Returns:
-
-    """
-    # evidence uncertainty minimising goal.
-    # remove points and see what increases uncertainty the most.
-
-    _, log_Z_var0 = linear_to_log_stats(log_f_mean=state.evidence_calculation.log_Z_mean,
-                                        log_f2_mean=state.evidence_calculation.log_Z2_mean)
-    num_shrinkages = -state.evidence_calculation.log_X_mean
-    delta_idx = state.sample_idx / (2. * num_shrinkages)
-
-    def body(body_state):
-        (remove_idx, inf_max_dvar, inf_max_dvar_idx, sup_max_dvar, sup_max_dvar_idx) = body_state
-        # removing a sample is equivalent to setting that n=inf at that point
-        perturbed_num_live_points = replace_index(state.sample_collection.num_live_points, jnp.inf,
-                                                  remove_idx.astype(int_type))
-        perturbed_sample_collection = state.sample_collection._replace(num_live_points=perturbed_num_live_points)
-        (evidence_calculation, _, _, _, _) = \
-            compute_evidence(num_samples=state.sample_idx, sample_collection=perturbed_sample_collection)
-        _, log_Z_var = linear_to_log_stats(log_f_mean=evidence_calculation.log_Z_mean,
-                                           log_f2_mean=evidence_calculation.log_Z2_mean)
-        dvar = log_Z_var - log_Z_var0
-
-        return remove_idx + delta_idx, dvar
-
-
-def _get_dynamic_goal(state: NestedSamplerState, G: jnp.ndarray):
-    """
-    Get contiguous contours that we'd like to reinforce.
-
-    We have two objectives, which can be mixed by setting `G`.
-    G=0: choose contours that decrease evidence uncertainty the most.
-    G=1: choose contours that increase ESS the most.
-
-    Note: This slightly departs from the Dynamic Nested Sampling paper.
-    """
-
-    n_i = state.sample_collection.num_live_points
-    dZ_mean = LogSpace(state.sample_collection.log_dZ_mean)
-    # Calculate remaining evidence, doing only the amount of work necessary.
-    Z_remaining = LogSpace(compute_remaining_evidence(state.sample_idx, state.sample_collection.log_dZ_mean))
-    # TODO: numerically compute goal using custome norm
-    I_evidence = ((LogSpace(jnp.log(n_i + 1.)) * Z_remaining + LogSpace(jnp.log(n_i)) * dZ_mean) / (
-            LogSpace(jnp.log(n_i + 1.)).sqrt() * LogSpace(jnp.log(n_i + 2.)) ** (1.5)))
-    I_evidence = normalise_log_space(I_evidence)
-
-    I_posterior = dZ_mean
-    I_posterior = normalise_log_space(I_posterior)
-
-    I_goal = LogSpace(jnp.log(1. - G)) * I_evidence + LogSpace(jnp.log(G)) * I_posterior
-    # I_goal = normalise_log_space(I_goal) # unnecessary for sampling
-
-    mask = jnp.arange(I_goal.size) >= state.sample_idx
-    I_goal = LogSpace(jnp.where(mask, -jnp.inf, I_goal.log_abs_val))
-
-    return I_goal.log_abs_val
-
-
-def get_dynamic_goal(key, state: NestedSamplerState, num_samples: int, G: jnp.ndarray) -> Tuple[
-    jnp.ndarray, jnp.ndarray]:
-    """
-    Determines what seed points to sample above.
+        a sorted, updated reservoir
     """
-    contours = jnp.concatenate([state.sample_collection.log_L_constraint[0:1],
-                                state.sample_collection.log_L_samples])
-    if G is None:
-        raise ValueError(f"G should be a float in [0,1].")
-    log_goal_weights = _get_dynamic_goal(state, G)
-    # Probabilistically sample the contours according to goal distribution
-    indices_constraint_reinforce = sample_goal_distribution(key, log_goal_weights, num_samples, replace=True)
-    start_idx = indices_constraint_reinforce.min()
-    end_idx = indices_constraint_reinforce.max()
-    log_L_constraint_start = contours[start_idx]
-    log_L_constraint_end = contours[end_idx]
+    if len(reservoirs) == 0:
+        raise ValueError(f"Need at least one reservoir to combine.")
+    if len(reservoirs) == 1:
+        return reservoirs[0]
+
+    def sort_reservoir(reservoir: Reservoir) -> Reservoir:
+        sort_idx = jnp.lexsort((reservoir.log_L_constraint, reservoir.log_L))
+        return tree_map(lambda x: x[sort_idx], reservoir)
+
+    reservoirs: List[Reservoir] = list(map(sort_reservoir, reservoirs))
+
+    # point_U -> concatenate and sort
+    # log_L_constraint -> concatenate and sort
+    # log_L -> concatenate and sort
+    # num_likelihood_evaluations -> concatenate and sort
+    # num_live_points -> concatenate, sort, and sum
+    # num_slices -> concatenate and sort
+    # iid -> concatenate and sort
+
+    output_reservoir: Reservoir = tree_map(lambda *x: jnp.concatenate(x, axis=0), *reservoirs)
+    sort_idx = jnp.lexsort((output_reservoir.log_L_constraint, output_reservoir.log_L))
+    output_reservoir: Reservoir = tree_map(lambda x: x[sort_idx], output_reservoir)
+
+    # combine each reservoir iteratively
+    combined_num_live_points = jnp.zeros_like(output_reservoir.log_L)
+
+    for r in reservoirs:
+        num_live_points = compute_num_live_points_from_unit_threads(r.log_L_constraint, r.log_L,
+                                                                    sorted_collection=True)
+        print(num_live_points)
+        j = 0
+        for i, log_L in enumerate(r.log_L):
+            while log_L > output_reservoir.log_L[j]:
+                j += 1
+            combined_num_live_points = combined_num_live_points.at[j].add(num_live_points[i])
 
-    return log_L_constraint_start, log_L_constraint_end
+    return output_reservoir, combined_num_live_points
```

### Comparing `jaxns-2.1.0/jaxns/termination.py` & `jaxns-2.2.0/jaxns/termination.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,28 +15,28 @@
                           evidence_calculation: Optional[EvidenceCalculation] = None,
                           live_points: Optional[LivePoints] = None
                           ):
     """
     Determine if termination should happen.
 
     Args:
-        evidence_calculation: evidence calculation
-        sample_stats: sample statistics
         term_cond: termination condition
 
     Returns:
         boolean done signal, and termination reason
 
     Termination Flags are bits:
         0-bit -> 1: used maximum allowed number of samples
         1-bit -> 2: evidence uncert below threshold
         2-bit -> 4: live points evidence below threshold
         3-bit -> 8: effective sample size big enough
         4-bit -> 16: used maxmimum allowed number of likelihood evaluations
         5-bit -> 32: maximum log-likelihood contour reached
+        6-bit -> 64: sampler efficiency too low
+        7-bit -> 128: entire live-points set is a single plateau
 
     Multiple flags are summed together
     """
     termination_condition = jnp.asarray(0, int_type)
     done = jnp.asarray(False)
 
     def _set_done_bit(bit, bit_reason, done, termination_condition):
@@ -96,17 +96,29 @@
         done, termination_condition = _set_done_bit(too_max_likelihood_evaluations, 4,
                                                     done=done, termination_condition=termination_condition)
 
     if term_cond.log_L_contour is not None:
         if sample_collection is None:
             raise ValueError("sample_collections must not be None.")
         log_L_max = jnp.max(
-            jnp.where(jnp.isinf(sample_collection.reservoir.log_L),
-                      -jnp.inf,
-                      sample_collection.reservoir.log_L
+            jnp.where(jnp.arange(sample_collection.reservoir.log_L.size) < sample_collection.sample_idx,
+                      sample_collection.reservoir.log_L,
+                      -jnp.inf
                       )
         )
         likeihood_contour_reached = log_L_max >= term_cond.log_L_contour
         done, termination_condition = _set_done_bit(likeihood_contour_reached, 5,
                                                     done=done, termination_condition=termination_condition)
 
+    if term_cond.efficiency_threshold is not None:
+        if live_points is None:
+            raise ValueError("live_points must be provided.")
+        efficiency = jnp.reciprocal(jnp.mean(live_points.reservoir.num_likelihood_evaluations))
+        efficiency_too_low = efficiency <= term_cond.efficiency_threshold
+        done, termination_condition = _set_done_bit(efficiency_too_low, 6,
+                                                    done=done, termination_condition=termination_condition)
+    if (live_points is not None) and (live_points.reservoir.log_L.size > 1):
+        all_plateau = jnp.min(live_points.reservoir.log_L) == jnp.max(live_points.reservoir.log_L)
+        done, termination_condition = _set_done_bit(all_plateau, 7,
+                                                    done=done, termination_condition=termination_condition)
+
     return done, termination_condition
```

### Comparing `jaxns-2.1.0/jaxns/tests/test_initial_state.py` & `jaxns-2.2.0/jaxns/tests/test_initial_state.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import numpy as np
 import tensorflow_probability.substrates.jax as tfp
 from jax import numpy as jnp, vmap, random
 
+from jaxns import StaticNestedSampler, collect_samples
 from jaxns.initial_state import init_sample_collection, get_uniform_init_live_points, \
     get_live_points_from_samples
 from jaxns.model import Model
 from jaxns.prior import PriorModelGen, Prior
-from jaxns.static_uniform import StaticUniform
-from jaxns.types import NestedSamplerState, SampleCollection
+from jaxns.static_uniform import UniformSampler
+from jaxns.types import NestedSamplerState, SampleCollection, TerminationCondition
 
 tfpd = tfp.distributions
 
 
 def test_init_sample_collection():
     def prior_model() -> PriorModelGen:
         x = yield Prior(tfpd.Uniform(low=0, high=2))
@@ -85,11 +86,15 @@
     state = NestedSamplerState(key=random.PRNGKey(42), sample_collection=sample_collection)
 
     n = 100
     live_points = get_uniform_init_live_points(random.PRNGKey(43),
                                                num_live_points=n,
                                                model=model)
     efficiency_threshold = 0.1
-    ns = StaticUniform(model=model, num_live_points=n, efficiency_threshold=efficiency_threshold)
-    state, live_points = ns(state=state, live_points=live_points)
+    ns = StaticNestedSampler(
+        samplers=[UniformSampler(model=model, efficiency_threshold=efficiency_threshold)],
+        num_live_points=n, num_parallel_samplers=1)
+    _, state, live_points = ns(state=state, live_points=live_points,
+                               termination_cond=TerminationCondition(max_samples=0))
+    state = collect_samples(state=state, new_reservoir=live_points.reservoir)
     assert state.sample_collection.sample_idx > 0
-    assert jnp.mean(1./live_points.reservoir.num_likelihood_evaluations) > efficiency_threshold
+    assert jnp.mean(1. / live_points.reservoir.num_likelihood_evaluations) > efficiency_threshold
```

### Comparing `jaxns-2.1.0/jaxns/tests/test_nested_sampler.py` & `jaxns-2.2.0/jaxns/tests/test_nested_sampler.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from time import monotonic_ns
 
+import pylab as plt
 import tensorflow_probability.substrates.jax as tfp
 from jax import random, numpy as jnp
+from jax._src.lax.control_flow import scan
 from jax._src.scipy.linalg import solve_triangular
 
+from jaxns.internals.log_semiring import LogSpace
 from jaxns.model import Model
 from jaxns.nested_sampler import ApproximateNestedSampler, ExactNestedSampler
 from jaxns.prior import PriorModelGen, Prior
-from jaxns.slice_sampler import MultiDimSliceSampler, UniDimSliceSampler
-from jaxns.types import TerminationCondition
-from jaxns.utils import evidence_posterior_samples, analytic_log_evidence
+from jaxns.static_uniform import BadUniformSampler
+from jaxns.types import TerminationCondition, float_type
+from jaxns.utils import sample_evidence, bruteforce_evidence
 
 tfpd = tfp.distributions
 
 
 class Timer:
     def __enter__(self):
         self.t0 = monotonic_ns()
@@ -33,20 +36,20 @@
         return -jnp.sum(z ** 2)
 
     model = Model(prior_model=prior_model,
                   log_likelihood=log_likelihood)
     approx_ns = ApproximateNestedSampler(model=model, num_live_points=50, num_parallel_samplers=1,
                                          max_samples=1000)
     # print(termination_reason)
-    # print(state)
     with Timer():
         termination_reason, state = approx_ns(random.PRNGKey(42),
                                               term_cond=TerminationCondition(live_evidence_frac=1e-4))
         results = approx_ns.to_results(state, termination_reason)
         results.log_Z_mean.block_until_ready()
+    approx_ns.summary(approx_ns.to_results(state, termination_reason))
 
     with Timer():
         termination_reason, state = approx_ns(random.PRNGKey(42),
                                               term_cond=TerminationCondition(live_evidence_frac=1e-4))
         results = approx_ns.to_results(state, termination_reason)
         results.log_Z_mean.block_until_ready()
 
@@ -61,61 +64,30 @@
     def log_likelihood(z):
         return -z ** 2
 
     model = Model(prior_model=prior_model, log_likelihood=log_likelihood)
     model.sanity_check(random.PRNGKey(0), S=100)
 
     exact_ns = ExactNestedSampler(model=model, num_live_points=50, num_parallel_samplers=1, max_samples=1000,
-                                  uncert_improvement_patience=1)
+                                  patience=1)
     # print(termination_reason)
     # print(state)
     with Timer():
         termination_reason, state = exact_ns(random.PRNGKey(42),
                                              term_cond=TerminationCondition(live_evidence_frac=1e-4))
         results = exact_ns.to_results(state, termination_reason)
         exact_ns.summary(results)
         exact_ns.plot_diagnostics(results)
 
-
     with Timer():
         termination_reason, state = exact_ns(random.PRNGKey(42),
                                              term_cond=TerminationCondition(live_evidence_frac=1e-4))
         results = exact_ns.to_results(state, termination_reason)
 
 
-def test_exact_nested_sampler_multidim_slice_sampler():
-    def prior_model() -> PriorModelGen:
-        x = yield Prior(tfpd.Uniform(low=0, high=2))
-        y = yield Prior(tfpd.Normal(loc=2, scale=x))
-        z = x + y
-        return z
-
-    def log_likelihood(z):
-        return -z ** 2
-
-    model = Model(prior_model=prior_model,
-                  log_likelihood=log_likelihood)
-    slice_sampler = MultiDimSliceSampler(model=model, num_restrict_dims=model.U_ndims)
-    exact_ns = ExactNestedSampler(model=model, num_live_points=50, num_parallel_samplers=1,
-                                  max_samples=1000, refinement_slice_sampler=slice_sampler)
-    # print(termination_reason)
-    # print(state)
-    with Timer():
-        termination_reason, state = exact_ns(random.PRNGKey(42),
-                                             term_cond=TerminationCondition(live_evidence_frac=1e-4))
-        results = exact_ns.to_results(state, termination_reason)
-        results.log_Z_mean.block_until_ready()
-
-    with Timer():
-        termination_reason, state = exact_ns(random.PRNGKey(42),
-                                             term_cond=TerminationCondition(live_evidence_frac=1e-4))
-        results = exact_ns.to_results(state, termination_reason)
-        results.log_Z_mean.block_until_ready()
-
-
 def test_nested_sampling_basic():
     def prior_model() -> PriorModelGen:
         x = yield Prior(tfpd.Uniform(low=0, high=1), name='x')
         return x
 
     def log_likelihood(x):
         return - jnp.sum(x ** 2)
@@ -129,19 +101,19 @@
                                              term_cond=TerminationCondition(live_evidence_frac=1e-4))
         results = exact_ns.to_results(state, termination_reason)
 
         # exact_ns.plot_diagnostics(results)
         exact_ns.summary(results)
         # exact_ns.plot_cornerplot(results)
 
-    log_Z_true = analytic_log_evidence(model=model, S=200)
+    log_Z_true = bruteforce_evidence(model=model, S=200)
 
-    log_Z_samples = evidence_posterior_samples(random.PRNGKey(42),
-                                               results.num_live_points_per_sample,
-                                               results.log_L_samples, S=1000)
+    log_Z_samples = sample_evidence(random.PRNGKey(42),
+                                    results.num_live_points_per_sample,
+                                    results.log_L_samples, S=1000)
 
     assert jnp.isclose(results.log_Z_mean, jnp.mean(log_Z_samples), atol=1e-3)
     assert jnp.isclose(results.log_Z_uncert, jnp.std(log_Z_samples), atol=1e-2)
 
     assert jnp.bitwise_not(jnp.isnan(results.log_Z_mean))
     assert jnp.isclose(results.log_Z_mean, log_Z_true, atol=1.75 * results.log_Z_uncert)
 
@@ -164,17 +136,17 @@
 #                                          term_cond=TerminationCondition(live_evidence_frac=1e-4))
 #     results = exact_ns.to_results(state, termination_reason)
 #
 #     exact_ns.plot_diagnostics(results)
 #     exact_ns.summary(results)
 #     exact_ns.plot_cornerplot(results)
 #
-#     log_Z_true = analytic_log_evidence(model=model, S=200)
+#     log_Z_true = bruteforce_evidence(model=model, S=200)
 #
-#     log_Z_samples = evidence_posterior_samples(random.PRNGKey(42),
+#     log_Z_samples = sample_evidence(random.PRNGKey(42),
 #                                                results.num_live_points_per_sample,
 #                                                results.log_L_samples, S=1000)
 #
 #     assert jnp.isclose(results.log_Z_mean, jnp.mean(log_Z_samples), atol=1e-3)
 #     assert jnp.isclose(results.log_Z_uncert, jnp.std(log_Z_samples), atol=1e-3)
 #
 #     assert jnp.bitwise_not(jnp.isnan(results.log_Z_mean))
@@ -183,23 +155,23 @@
 
 def test_nested_sampling_mvn_static():
     def log_normal(x, mean, cov):
         L = jnp.linalg.cholesky(cov)
         dx = x - mean
         dx = solve_triangular(L, dx, lower=True)
         return -0.5 * x.size * jnp.log(2. * jnp.pi) - jnp.sum(jnp.log(jnp.diag(L))) \
-               - 0.5 * dx @ dx
+            - 0.5 * dx @ dx
 
-    ndims = 4
-    prior_mu = 2 * jnp.ones(ndims)
+    ndims = 8
+    prior_mu = 15 * jnp.ones(ndims)
     prior_cov = jnp.diag(jnp.ones(ndims)) ** 2
 
     data_mu = jnp.zeros(ndims)
     data_cov = jnp.diag(jnp.ones(ndims)) ** 2
-    data_cov = jnp.where(data_cov == 0., 0.95, data_cov)
+    data_cov = jnp.where(data_cov == 0., 0.99, data_cov)
 
     true_logZ = log_normal(data_mu, prior_mu, prior_cov + data_cov)
     # not super happy with this being 1.58 and being off by like 0.1. Probably related to the ESS.
     post_mu = prior_cov @ jnp.linalg.inv(prior_cov + data_cov) @ data_mu + data_cov @ jnp.linalg.inv(
         prior_cov + data_cov) @ prior_mu
 
     print(f"True post mu:{post_mu}")
@@ -212,92 +184,99 @@
         return x
 
     def log_likelihood(x):
         return log_normal(x, data_mu, data_cov)
 
     model = Model(prior_model=prior_model, log_likelihood=log_likelihood)
 
-    model.sanity_check(random.PRNGKey(52), S=100)
-    exact_ns = ExactNestedSampler(model=model, num_live_points=200, num_parallel_samplers=1,
-                                  max_samples=3000)
+    # model.sanity_check(random.PRNGKey(42), S=100)
+    exact_ns = ExactNestedSampler(model=model, num_live_points=100, num_parallel_samplers=1,
+                                  max_samples=40000, patience=20)
     with Timer():
-        termination_reason, state = exact_ns(random.PRNGKey(42),
-                                             term_cond=TerminationCondition(live_evidence_frac=1e-4))
+        termination_reason, state = exact_ns(random.PRNGKey(41),
+                                             term_cond=TerminationCondition(live_evidence_frac=1e-5))
         results = exact_ns.to_results(state, termination_reason)
         exact_ns.summary(results)
-    # exact_ns.plot_diagnostics(results)
-    assert jnp.isclose(results.log_Z_mean, true_logZ, atol=1.75 * results.log_Z_uncert)
-
-
-def test_multi_needs_fewer_slices():
+    exact_ns.plot_diagnostics(results)
+    actual_log_Z_mean = results.log_Z_mean
+    expected_log_Z_mean = true_logZ
+    tol = 1.75 * results.log_Z_uncert
+    assert jnp.isclose(actual_log_Z_mean, expected_log_Z_mean, atol=tol)
 
-    def log_normal(x, mean, cov):
-        L = jnp.linalg.cholesky(cov)
-        dx = x - mean
-        dx = solve_triangular(L, dx, lower=True)
-        return -0.5 * x.size * jnp.log(2. * jnp.pi) - jnp.sum(jnp.log(jnp.diag(L))) - 0.5 * dx @ dx
 
-    ndims = 4
-    prior_mu = 2 * jnp.ones(ndims)
-    prior_cov = jnp.diag(jnp.ones(ndims)) ** 2
-
-    data_mu = jnp.zeros(ndims)
-    data_cov = jnp.diag(jnp.ones(ndims)) ** 2
-    data_cov = jnp.where(data_cov == 0., 0.95, data_cov)
-
-    true_logZ = log_normal(data_mu, prior_mu, prior_cov + data_cov)
-    # not super happy with this being 1.58 and being off by like 0.1. Probably related to the ESS.
-    post_mu = prior_cov @ jnp.linalg.inv(prior_cov + data_cov) @ data_mu + data_cov @ jnp.linalg.inv(
-        prior_cov + data_cov) @ prior_mu
-
-    print(f"True post mu:{post_mu}")
-    print(f"True log Z: {true_logZ}")
-
-    def prior_model() -> PriorModelGen:
-        x = yield Prior(
-            tfpd.MultivariateNormalTriL(loc=prior_mu, scale_tril=jnp.linalg.cholesky(prior_cov)),
-            name='x')
-        return x
-
-    def log_likelihood(x):
-        return log_normal(x, data_mu, data_cov)
-
-    model = Model(prior_model=prior_model, log_likelihood=log_likelihood)
-
-    model.sanity_check(random.PRNGKey(52), S=100)
-    slice_sampler = MultiDimSliceSampler(model=model, num_restrict_dims=model.U_ndims)
-    exact_ns = ExactNestedSampler(model=model, num_live_points=200, num_parallel_samplers=1,
-                                  max_samples=1e4, refinement_slice_sampler=slice_sampler)
-    with Timer():
-        print("Using Multi Dimensional Slice Sampling")
-        termination_reason, state = exact_ns(random.PRNGKey(42),
-                                             term_cond=TerminationCondition(live_evidence_frac=1e-4))
-        results = exact_ns.to_results(state, termination_reason)
-        exact_ns.summary(results)
-        num_slices_multi = results.total_num_slices
-    assert jnp.isclose(results.log_Z_mean, true_logZ, atol=1.75 * results.log_Z_uncert)
-
-    slice_sampler = UniDimSliceSampler(model=model, midpoint_shrink=True)
-    exact_ns = ExactNestedSampler(model=model, num_live_points=200, num_parallel_samplers=1,
-                                  max_samples=1e4, refinement_slice_sampler=slice_sampler)
-    with Timer():
-        print("Using Uni Dimensional Slice Sampling")
-        termination_reason, state = exact_ns(random.PRNGKey(42),
-                                             term_cond=TerminationCondition(live_evidence_frac=1e-4))
-        results = exact_ns.to_results(state, termination_reason)
-        exact_ns.summary(results)
-        num_slices_uni = results.total_num_slices
-    assert jnp.isclose(results.log_Z_mean, true_logZ, atol=1.75 * results.log_Z_uncert)
-    # TODO(Joshuaalbert): broken test, probably means multidim slice sampling is not robust to structure.
-    # assert num_slices_multi < num_slices_uni
+# def test_multi_needs_fewer_slices():
+#     def log_normal(x, mean, cov):
+#         L = jnp.linalg.cholesky(cov)
+#         dx = x - mean
+#         dx = solve_triangular(L, dx, lower=True)
+#         return -0.5 * x.size * jnp.log(2. * jnp.pi) - jnp.sum(jnp.log(jnp.diag(L))) - 0.5 * dx @ dx
+#
+#     ndims = 4
+#     prior_mu = 2 * jnp.ones(ndims)
+#     prior_cov = jnp.diag(jnp.ones(ndims)) ** 2
+#
+#     data_mu = jnp.zeros(ndims)
+#     data_cov = jnp.diag(jnp.ones(ndims)) ** 2
+#     data_cov = jnp.where(data_cov == 0., 0.95, data_cov)
+#
+#     true_logZ = log_normal(data_mu, prior_mu, prior_cov + data_cov)
+#     # not super happy with this being 1.58 and being off by like 0.1. Probably related to the ESS.
+#     post_mu = prior_cov @ jnp.linalg.inv(prior_cov + data_cov) @ data_mu + data_cov @ jnp.linalg.inv(
+#         prior_cov + data_cov) @ prior_mu
+#
+#     print(f"True post mu:{post_mu}")
+#     print(f"True log Z: {true_logZ}")
+#
+#     def prior_model() -> PriorModelGen:
+#         x = yield Prior(
+#             tfpd.MultivariateNormalTriL(loc=prior_mu, scale_tril=jnp.linalg.cholesky(prior_cov)),
+#             name='x')
+#         return x
+#
+#     def log_likelihood(x):
+#         return log_normal(x, data_mu, data_cov)
+#
+#     model = Model(prior_model=prior_model, log_likelihood=log_likelihood)
+#
+#     model.sanity_check(random.PRNGKey(52), S=100)
+#     exact_ns = ExactNestedSampler(model=model, num_live_points=200, num_parallel_samplers=1,
+#                                   max_samples=1e4)
+#     with Timer():
+#         print("Using Multi Dimensional Slice Sampling")
+#         termination_reason, state = exact_ns(random.PRNGKey(42),
+#                                              term_cond=TerminationCondition(live_evidence_frac=1e-4))
+#         results = exact_ns.to_results(state, termination_reason)
+#         exact_ns.summary(results)
+#         num_slices_multi = results.total_num_slices
+#     assert jnp.isclose(results.log_Z_mean, true_logZ, atol=1.75 * results.log_Z_uncert)
+#
+#     slice_sampler = UniDimSliceSampler(model=model, midpoint_shrink=True)
+#     exact_ns = ExactNestedSampler(model=model, num_live_points=200, num_parallel_samplers=1,
+#                                   max_samples=1e4, refinement_slice_sampler=slice_sampler)
+#     with Timer():
+#         print("Using Uni Dimensional Slice Sampling")
+#         termination_reason, state = exact_ns(random.PRNGKey(42),
+#                                              term_cond=TerminationCondition(live_evidence_frac=1e-4))
+#         results = exact_ns.to_results(state, termination_reason)
+#         exact_ns.summary(results)
+#         num_slices_uni = results.total_num_slices
+#     assert jnp.isclose(results.log_Z_mean, true_logZ, atol=1.75 * results.log_Z_uncert)
+#     # TODO(Joshuaalbert): broken test, probably means multidim slice sampling is not robust to structure.
+#     # assert num_slices_multi < num_slices_uni
 
 
 def test_shrinkage():
     n = 2
 
+    # Prior is uniform in U[0,1]
+    # Likelihood is 1 - x**n
+    # Z = 1 - 1/n+1
+
+    log_Z_true = jnp.log(1. - 1. / (n + 1))
+
     def prior_model() -> PriorModelGen:
         x = yield Prior(tfpd.Uniform(low=0, high=1))
         return x
 
     def log_likelihood(x):
         return jnp.log(1. - x ** n)
 
@@ -316,36 +295,125 @@
     # print(list(results.log_X_mean[:results.total_num_samples]))
     # print(list(results.log_L_samples[:results.total_num_samples]))
     # print(list(jnp.log(exact_X(jnp.exp(results.log_L_samples[:results.total_num_samples])))))
     diff = results.log_X_mean - jnp.log(exact_X(jnp.exp(results.log_L_samples)))
     diff = jnp.where(jnp.isfinite(diff), diff, jnp.nan)
     # print(jnp.nanstd(diff))
     assert jnp.nanstd(diff) < 0.26
+    assert jnp.isclose(results.log_Z_mean, log_Z_true, atol=results.log_Z_uncert * 1.75)
+
+
+def compute_shrinkage_stats(num_live_points):
+    def _update_stats(state, num_live_points):
+        X_mean = LogSpace(state['log_X_mean'])
+        X2_mean = LogSpace(state['log_X2_mean'])
+
+        T_mean = LogSpace(- jnp.logaddexp(0., -jnp.log(num_live_points)))
+        T2_mean = LogSpace(- jnp.logaddexp((0.), jnp.log(2.) - jnp.log(num_live_points)))
+
+        next_X_mean = X_mean * T_mean
+        next_X2_mean = X2_mean * T2_mean
+
+        return dict(log_X_mean=next_X_mean.log_abs_val, log_X2_mean=next_X2_mean.log_abs_val), dict(
+            log_X_mean=next_X_mean.log_abs_val, log_X2_mean=next_X2_mean.log_abs_val)
+
+    state = dict(
+        log_X_mean=jnp.asarray(0., float_type),
+        log_X2_mean=jnp.asarray(0., float_type),
+    )
+    _, stats = scan(_update_stats,
+                    state,
+                    num_live_points)
+    log_X_uncert = (LogSpace(stats['log_X2_mean']) - LogSpace(stats['log_X_mean']).square()).sqrt().log_abs_val
+    return stats['log_X_mean'], log_X_uncert
+
+
+def test_adaptive_refinement():
+    n = 2
+
+    # Prior is uniform in U[0,1]
+    # Likelihood is 1 - x**n
+    # Z = 1 - 1/n+1
+
+    log_Z_true = jnp.log(1. - 1. / (n + 1))
+    print(f"True log(Z): {log_Z_true}")
+
+    def prior_model() -> PriorModelGen:
+        x = yield Prior(tfpd.Uniform(low=0, high=1))
+        return x
+
+    def log_likelihood(x):
+        return (LogSpace(0.) - LogSpace(n * jnp.log(x))).log_abs_val
+
+    def exact_X(L):
+        return (1. - L) ** (1. / n)
+
+    model = Model(prior_model=prior_model,
+                  log_likelihood=log_likelihood)
+    ns = ApproximateNestedSampler(
+        model=model,
+        num_live_points=50,
+        num_parallel_samplers=1,
+        max_samples=1e4,
+        sampler_chain=[
+            BadUniformSampler(mis_fraction=0., model=model)
+        ]
+    )
+
+    termination_reason, state = ns(random.PRNGKey(42),
+                                   term_cond=TerminationCondition(live_evidence_frac=1e-4))
+    results = ns.to_results(state, termination_reason)
+    ns.summary(results)
+    ns.plot_diagnostics(results)
+
+    # ensure there is no bug in control flow. X should be same to controlled evaluation
+    log_X_mean, log_X_std = compute_shrinkage_stats(results.num_live_points_per_sample)
+    assert jnp.allclose(results.log_X_mean, log_X_mean)
+
+    # ensure the deviation from the exact shrinkage is correct
+    X_exact = exact_X(jnp.exp(results.log_L_samples))
+
+    rel_diff = jnp.abs(jnp.exp(log_X_mean) - X_exact) / jnp.exp(log_X_std)
+
+    # ensure log_Z is close to truth
+    assert jnp.isclose(results.log_Z_mean, log_Z_true, atol=results.log_Z_uncert * 1.75)
+
+    print("Relative shrinkage errors", jnp.percentile(rel_diff, jnp.asarray([50, 75, 90, 95])))
+    assert jnp.all(jnp.percentile(rel_diff, jnp.asarray([50, 75, 90, 95])) < jnp.asarray([0.9, 1.1, 1.4, 1.5]))
 
 
 def test_nested_sampling_plateau():
     def log_likelihood(x):
         return 0.
 
     def prior_model() -> PriorModelGen:
         x = yield Prior(tfpd.Uniform(low=0, high=1))
         return x
 
     model = Model(prior_model=prior_model,
                   log_likelihood=log_likelihood)
-    exact_ns = ExactNestedSampler(model=model, num_live_points=50,
-                                  max_samples=1000)
+    exact_ns = ExactNestedSampler(
+        model=model,
+        num_live_points=50,
+        max_samples=1000
+    )
+
+    termination_reason, state = exact_ns(
+        random.PRNGKey(42),
+        term_cond=TerminationCondition(live_evidence_frac=1e-4)
+    )
 
-    termination_reason, state = exact_ns(random.PRNGKey(42),
-                                         term_cond=TerminationCondition(live_evidence_frac=1e-4))
     results = exact_ns.to_results(state, termination_reason)
     exact_ns.summary(results)
+    exact_ns.plot_diagnostics(results)
 
-    log_Z_samples = evidence_posterior_samples(random.PRNGKey(42),
-                                               results.num_live_points_per_sample,
-                                               results.log_L_samples, S=1000)
+    log_Z_samples = sample_evidence(random.PRNGKey(42),
+                                    results.num_live_points_per_sample,
+                                    results.log_L_samples, S=1000)
+    plt.hist(log_Z_samples, bins='auto')
+    plt.show()
 
     true_log_Z_uncert = jnp.std(log_Z_samples)
     print(f"true logZ uncert: {true_log_Z_uncert}")
 
     assert jnp.bitwise_not(jnp.isnan(results.log_Z_mean))
     assert jnp.isclose(results.log_Z_mean, 0., atol=1.75 * true_log_Z_uncert)
```

### Comparing `jaxns-2.1.0/jaxns/tests/test_prior.py` & `jaxns-2.2.0/jaxns/tests/test_prior.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 
 import tensorflow_probability.substrates.jax as tfp
-from jax import random, numpy as jnp
+from jax import random, numpy as jnp, vmap
 
 from jaxns.prior import PriorModelGen, Prior, parse_prior, compute_log_likelihood, InvalidDistribution, \
     InvalidPriorName, prepare_input, distribution_chain
 from jaxns.special_priors import Bernoulli, Categorical, Poisson, Beta, ForcedIdentifiability
 from jaxns.types import float_type
 
 logger = logging.getLogger('jaxns')
@@ -100,15 +100,14 @@
     d = Prior(jnp.zeros(5))
     print(d)
     assert d.forward(jnp.ones(d.base_shape, float_type)).shape == d.shape
     assert d.forward(jnp.zeros(d.base_shape, float_type)).shape == d.shape
     assert d.base_shape == ()
     assert d.shape == (5,)
 
-
     d = Prior(tfpd.Uniform(low=jnp.zeros(5), high=jnp.ones(5)))
     print(d)
     assert d.forward(jnp.ones(d.base_shape, float_type)).shape == d.shape
     assert d.forward(jnp.zeros(d.base_shape, float_type)).shape == d.shape
     assert d.base_shape == (5,)
     assert d.shape == (5,)
 
@@ -186,27 +185,46 @@
     d = Bernoulli(probs=jnp.ones(5), name='x')
     print(d)
     assert d.forward(jnp.ones(d.base_shape, float_type)).shape == d.shape
     assert d.forward(jnp.zeros(d.base_shape, float_type)).shape == d.shape
     assert d.base_shape == (5,)
     assert d.shape == (5,)
 
-    d = Categorical(parametrisation='gumbel_max', probs=jnp.ones(5), name='x')
+    probs = jnp.asarray([1, 2, 3, 2, 1], float_type)
+    d = Categorical(parametrisation='gumbel_max', probs=probs, name='x')
     print(d)
     assert d.forward(jnp.ones(d.base_shape, float_type)).shape == d.shape
     assert d.forward(jnp.zeros(d.base_shape, float_type)).shape == d.shape
     assert d.base_shape == (5,)
     assert d.shape == ()
+    x = vmap(lambda key: d.forward(random.uniform(key, shape=d.base_shape)))(random.split(random.PRNGKey(42), 10000))
+    assert jnp.all(x >= 0)
+    assert jnp.all(x < 5)
+    assert jnp.any(x == 0)
+    assert jnp.any(x == 4)
+    count = jnp.bincount(x)
+    count /= jnp.sum(count)
+    assert jnp.allclose(count, probs / jnp.sum(probs), atol=1e-2)
 
-    d = Categorical(parametrisation='cdf', probs=jnp.ones(5), name='x')
+    probs = jnp.asarray([1, 2, 3, 2, 1], float_type)
+    d = Categorical(parametrisation='cdf', probs=probs, name='x')
     print(d)
     assert d.forward(jnp.ones(d.base_shape, float_type)).shape == d.shape
     assert d.forward(jnp.zeros(d.base_shape, float_type)).shape == d.shape
     assert d.base_shape == ()
     assert d.shape == ()
+    u_array = jnp.linspace(0., 1., 10000)
+    x = vmap(lambda u: d.forward(u))(u_array)
+    assert jnp.all(x >= 0)
+    assert jnp.all(x < 5)
+    assert jnp.any(x == 0)
+    assert jnp.any(x == 4)
+    count = jnp.bincount(x)
+    count /= jnp.sum(count)
+    assert jnp.allclose(count, probs / jnp.sum(probs), atol=1e-2)
 
     d = Poisson(rate=jnp.ones(5), name='x')
     print(d)
     assert d.forward(jnp.ones(d.base_shape, float_type)).shape == d.shape
     assert d.forward(jnp.zeros(d.base_shape, float_type)).shape == d.shape
     assert d.base_shape == (5,)
     assert d.shape == (5,)
@@ -220,7 +238,12 @@
 
     d = ForcedIdentifiability(n=10, low=jnp.zeros(5), high=jnp.ones(5), name='x')
     print(d)
     assert d.forward(jnp.ones(d.base_shape, float_type)).shape == d.shape
     assert d.forward(jnp.zeros(d.base_shape, float_type)).shape == d.shape
     assert d.base_shape == (10, 5)
     assert d.shape == (10, 5)
+
+    u_input = vmap(lambda key: random.uniform(key, shape=d.base_shape))(random.split(random.PRNGKey(42), 1))
+    x = vmap(lambda u: d.forward(u))(u_input)
+    u = vmap(lambda x: d.inverse(x))(x)
+    assert jnp.allclose(u, u_input)
```

### Comparing `jaxns-2.1.0/jaxns/tests/test_random.py` & `jaxns-2.2.0/jaxns/tests/test_random.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,14 +7,22 @@
 def test_random_ortho_matrix():
     M = random_ortho_matrix(random.PRNGKey(42), 5)
     assert jnp.isclose(jnp.linalg.det(M), 1.)
     assert jnp.allclose(M.T @ M, M @ M.T, atol=1e-6)
     assert jnp.allclose(M.T @ M, jnp.eye(5), atol=1e-6)
     assert jnp.allclose(jnp.linalg.norm(M, axis=0), jnp.linalg.norm(M, axis=1))
 
+    for i in range(100):
+        M = random_ortho_matrix(random.PRNGKey(i), 5)
+        np.testing.assert_allclose(jnp.abs(jnp.linalg.det(M)), 1, atol=1e-6)
+
+    for i in range(100):
+        M = random_ortho_matrix(random.PRNGKey(i), 5, special_orthogonal=True)
+        np.testing.assert_allclose(jnp.linalg.det(M), 1, atol=1e-6)
+
 
 def test_random_ortho_normal_matrix():
     for i in range(100):
         H = random_ortho_matrix(random.PRNGKey(0), 3)
         assert jnp.all(jnp.isclose(H @ H.conj().T, jnp.eye(3), atol=1e-6))
```

### Comparing `jaxns-2.1.0/jaxns/types.py` & `jaxns-2.2.0/jaxns/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 class TerminationCondition(NamedTuple):
     ess: Optional[FloatArray] = jnp.inf
     evidence_uncert: Optional[FloatArray] = jnp.asarray(0., float_type)
     live_evidence_frac: Optional[FloatArray] = jnp.asarray(1e-4, float_type)
     max_samples: Optional[IntArray] = jnp.iinfo(int_type).max
     max_num_likelihood_evaluations: Optional[IntArray] = jnp.iinfo(int_type).max
     log_L_contour: Optional[FloatArray] = jnp.inf
+    efficiency_threshold: Optional[FloatArray] = jnp.asarray(0., float_type)
 
 
 class NestedSamplerResults(NamedTuple):
     log_Z_mean: FloatArray  # estimate of E[log(Z)]
     log_Z_uncert: FloatArray  # estimate of StdDev[log(Z)]
     ESS: FloatArray  # estimate of Kish's effective sample size
     H_mean: FloatArray  # estimate of E[int log(L) L dp/Z]
@@ -104,15 +105,15 @@
     log_dp_mean: FloatArray  # log(E[dZ]) of each sample, where dZ is how much it contributes to the total evidence.
     log_X_mean: FloatArray  # log(E[U]) of each sample
     log_posterior_density: FloatArray  # log(P( theta | D )) log posteriori density
     num_live_points_per_sample: IntArray  # how many live points were taken for the samples.
     num_likelihood_evaluations_per_sample: IntArray  # how many likelihood evaluations were made per sample.
     num_slices: IntArray  # how many slices were taken for slice sampled points
     total_num_samples: IntArray  # int, the total number of samples collected.
-    total_num_slices: IntArray # int, how many slices in total were taken
+    total_num_slices: IntArray  # int, how many slices in total were taken
     total_num_likelihood_evaluations: IntArray  # how many likelihood evaluations were made in total
     log_efficiency: FloatArray  # log(total_num_samples / total_num_likelihood_evaluations)
     termination_reason: IntArray  # this will be an int reflecting the reason for termination
 
 
 class SignedLog(NamedTuple):
     """
```

### Comparing `jaxns-2.1.0/jaxns/utils.py` & `jaxns-2.2.0/jaxns/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 import io
 import logging
-from typing import NamedTuple, TextIO, Union, Optional
+from typing import NamedTuple, TextIO, Union, Optional, Tuple, TypeVar, Callable
 
 import numpy as np
+from etils.array_types import PRNGKey
 from jax import numpy as jnp, tree_map, vmap, random, jit
 from jax._src.lax.control_flow import while_loop
 
 from jaxns.internals.log_semiring import LogSpace
 from jaxns.internals.maps import replace_index, prepare_func_args
 from jaxns.model import Model
 from jaxns.random import resample_indicies
 from jaxns.types import SampleCollection, NestedSamplerState, Reservoir, NestedSamplerResults, \
-    float_type
+    float_type, XType
+from jaxns.warnings import deprecated
 
 logger = logging.getLogger('jaxns')
 
 __all__ = ['sort_samples',
            'collect_samples',
            'resample',
            'marginalise_static',
            'marginalise_dynamic',
            'maximum_a_posteriori_point',
            'summary',
-           'evidence_posterior_samples',
            'analytic_posterior_samples',
-           'analytic_log_evidence',
+           'sample_evidence',
+           'bruteforce_posterior_samples',
+           'bruteforce_evidence',
            'save_pytree',
            'save_results',
            'load_pytree',
            'load_results']
 
+
 def sort_samples(sample_collection: SampleCollection):
     """
     Sorts a sample collection lexigraphically, first on log_L then on log_L_constraint.
 
     Args:
         sample_collection: sample collection to sort
 
@@ -70,52 +74,69 @@
     )
     # Sort
     sample_collection = sort_samples(sample_collection)
     state = state._replace(sample_collection=sample_collection)
     return state
 
 
-def resample(key, samples, log_weights, S=None, replace=False):
+def resample(key: PRNGKey, samples: XType, log_weights: jnp.ndarray, S: int = None, replace: bool = False) -> XType:
+    """
+    Resample the weighted samples into uniformly weighted samples.
+
+    Args:
+        key: PRNGKey
+        samples: samples from nested sampled results
+        log_weights: log-posterior weight
+        S: number of samples to generate. Will use Kish's estimate of ESS if None.
+        replace: whether to sample with replacement
+
+    Returns:
+        equally weighted samples
+    """
     idx = resample_indicies(key, log_weights, S=S, replace=replace)
     return tree_map(lambda s: s[idx, ...], samples)
 
 
-def marginalise_static(key, samples, log_weights, ESS, fun):
+_V = TypeVar('_V')
+
+
+def marginalise_static(key: PRNGKey, samples: XType, log_weights: jnp.ndarray, ESS: int, fun: Callable[..., _V]) -> _V:
     """
     Marginalises function over posterior samples, where ESS is static.
 
     Args:
         key: PRNG key
         samples (dict): dict of batched array of nested sampling samples
         log_weights: log weights from nested sampling
         ESS: static effective sample size
         fun (:code:`callable(**kwargs)`): function to marginalise
 
     Returns:
-        expectation over resampled samples.
+        expectation over resampled samples
     """
     fun = prepare_func_args(fun)
     samples = resample(key, samples, log_weights, S=ESS, replace=True)
     marginalised = tree_map(lambda marg: jnp.nanmean(marg, axis=0), vmap(fun)(**samples))
     return marginalised
 
 
-def marginalise_dynamic(key, samples, log_weights, ESS, fun):
+def marginalise_dynamic(key: PRNGKey, samples: XType, log_weights: jnp.ndarray, ESS: jnp.ndarray,
+                        fun: Callable[..., _V]) -> _V:
     """
     Marginalises function over posterior samples, where ESS can be dynamic.
 
     Args:
         key: PRNG key
         samples (dict): dict of batched array of nested sampling samples
         log_weights: log weights from nested sampling
         ESS: dynamic effective sample size
         fun (:code:`callable(**kwargs)`): function to marginalise
 
     Returns:
-        expectation over resampled samples.
+        expectation of `func` over resampled samples.
     """
     fun = prepare_func_args(fun)
     ESS = jnp.asarray(ESS)
 
     def body(state):
         (key, i, count, marginalised) = state
         key, resample_key = random.split(key, 2)
@@ -134,15 +155,15 @@
     (_, _, count, marginalised) = while_loop(lambda state: state[1] < ESS,
                                              body,
                                              (key, jnp.array(0, ESS.dtype), count, init_marginalised))
     marginalised = tree_map(lambda x, c: x / c, marginalised, count)
     return marginalised
 
 
-def maximum_a_posteriori_point(results: NestedSamplerResults):
+def maximum_a_posteriori_point(results: NestedSamplerResults) -> XType:
     """
     Get the MAP point of a nested sampling result.
     Does this by choosing the point with largest L(x) p(x).
 
     Args:
         results (NestedSamplerResult): Nested sampler result
 
@@ -192,22 +213,24 @@
         try:
             sig_figs = -int("{:e}".format(uncert_v).split('e')[1]) + 1
             return round(float(v), sig_figs)
         except:
             return float(v)
 
     _print("--------")
-    termination_bit_mask = _bit_mask(results.termination_reason, width=6)
+    termination_bit_mask = _bit_mask(results.termination_reason, width=8)
     _print("Termination Conditions:")
     for bit, condition in zip(termination_bit_mask, ['Reached max samples',
                                                      'Evidence uncertainty low enough',
                                                      'Small remaining evidence',
                                                      'Reached ESS',
                                                      "Used max num likelihood evaluations",
-                                                     'likelihood contour reached']):
+                                                     'Likelihood contour reached',
+                                                     'Sampler efficiency too low',
+                                                     'All live-points are on a single plateau (potential numerical errors, consider 64-bit)']):
         if bit == 1:
             _print(condition)
     _print("--------")
     _print("# likelihood evals: {}".format(results.total_num_likelihood_evaluations))
     _print("# samples: {}".format(results.total_num_samples))
     _print("# slices: {:.1f}".format(results.total_num_slices))
     _print(
@@ -268,15 +291,31 @@
                 f.write(out)
         elif isinstance(f_obj, io.TextIOBase):
             f_obj.write(out)
         else:
             raise TypeError(f"Invalid f_obj: {type(f_obj)}")
 
 
-def evidence_posterior_samples(key, num_live_points_per_sample, log_L_samples, S: int = 100):
+def sample_evidence(key, num_live_points_per_sample, log_L_samples, S: int = 100) -> jnp.ndarray:
+    """
+    Sample the evidence distribution, but stochastically simulating the shrinkage distribution.
+
+    Note: this produces approximate samples, since there is also an uncertainty in the placement of the contours during
+    shrinkage. Incorporating this stochasticity into the simulation would require running an entire
+    nested sampling many times.
+
+    Args:
+        key: PRNGKey
+        num_live_points_per_sample: the number of live points for each sample
+        log_L_samples: the log-L of samples
+        S: The number of samples to produce
+
+    Returns:
+        samples of log(Z)
+    """
     n_i = num_live_points_per_sample
     L = LogSpace(jnp.asarray([-jnp.inf], log_L_samples.dtype)).concatenate(
         LogSpace(log_L_samples))
     L_mid = (L[:-1] + L[1:]) * LogSpace(jnp.log(0.5))
 
     def evidence_chain(key):
         # T ~ Beta(n[i],1) <==> T ~ Kumaraswamy(n[i],1)
@@ -294,15 +333,36 @@
         return Z.log_abs_val
 
     log_Z_chains = vmap(evidence_chain)(random.split(key, S))
     Z_chains = LogSpace(log_Z_chains)
     return Z_chains.log_abs_val
 
 
-def analytic_log_evidence(model: Model, S: int = 60):
+def bruteforce_posterior_samples(model: Model, S: int = 60) -> Tuple[XType, jnp.ndarray]:
+    """
+    Compute the posterior with brute-force over a regular grid.
+
+    Args:
+        prior_chain (jaxns.PriorChain): PriorChain of model
+        log_likelihood (:code:`callable(**samples)`): log-likelihood function
+        S (int): resolution of grid
+
+    Returns:
+        samples, and log-weight
+    """
+    u_vec = jnp.linspace(jnp.finfo(float_type).eps, 1. - jnp.finfo(float_type).eps, S)
+    du = u_vec[1] - u_vec[0]
+    args = jnp.stack([x.flatten() for x in jnp.meshgrid(*[u_vec] * model.U_ndims, indexing='ij')], axis=-1)
+    samples = jit(vmap(model.transform))(args)
+    log_L = jit(vmap(model.forward))(args)
+    dZ = LogSpace(log_L) * LogSpace(jnp.log(du)) ** model.U_ndims
+    return samples, dZ.log_abs_val
+
+
+def bruteforce_evidence(model: Model, S: int = 60):
     """
     Compute the evidence with brute-force over a regular grid.
 
     Args:
         prior_chain: PriorChain of model
         log_likelihood (:code:`callable(**samples)`): log-likelihood function
         S (int): resolution of grid
@@ -315,26 +375,28 @@
     du = u_vec[1] - u_vec[0]
     args = jnp.stack([x.flatten() for x in jnp.meshgrid(*[u_vec] * model.U_ndims, indexing='ij')], axis=-1)
     Z_true = (LogSpace(jit(vmap(model.forward))(args)).nansum() * LogSpace(
         jnp.log(du)) ** model.U_ndims)
     return Z_true.log_abs_val
 
 
+@deprecated(bruteforce_posterior_samples)
 def analytic_posterior_samples(model: Model, S: int = 60):
     """
     Compute the evidence with brute-force over a regular grid.
 
     Args:
         prior_chain (jaxns.PriorChain): PriorChain of model
         log_likelihood (:code:`callable(**samples)`): log-likelihood function
         S (int): resolution of grid
 
     Returns:
         log(Z)
     """
+    logger.warning(f"")
 
     u_vec = jnp.linspace(jnp.finfo(float_type).eps, 1. - jnp.finfo(float_type).eps, S)
     du = u_vec[1] - u_vec[0]
     args = jnp.stack([x.flatten() for x in jnp.meshgrid(*[u_vec] * model.U_ndims, indexing='ij')], axis=-1)
     samples = jit(vmap(model.transform))(args)
     log_L = jit(vmap(model.forward))(args)
     dZ = LogSpace(log_L) * LogSpace(jnp.log(du)) ** model.U_ndims
```

### Comparing `jaxns-2.1.0/jaxns.egg-info/PKG-INFO` & `jaxns-2.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,139 @@
 Metadata-Version: 2.1
 Name: jaxns
-Version: 2.1.0
+Version: 2.2.0
 Summary: Nested Sampling in JAX
 Home-page: https://github.com/joshuaalbert/jaxns
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![https://pypi.org/project/jaxns/](https://img.shields.io/pypi/v/jaxns.svg)
+[![Python](https://img.shields.io/pypi/pyversions/jaxns.svg)](https://badge.fury.io/py/jaxns)
+[![PyPI](https://badge.fury.io/py/jaxns.svg)](https://badge.fury.io/py/jaxns)
+
+Main
+Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=main)
+
+Develop
+Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=develop)
 
 ![JAXNS](https://github.com/Joshuaalbert/jaxns/raw/main/jaxns_logo.png)
 
+## Mission: _To make nested sampling **faster, easier, and more powerful**_
 
 # What is it?
-Provides a probabilistic programming framework based on nested sampling. It's coded in JAX in a manner that allows lowering the entire inference algorithm to XLA primitives, which are JIT-compiled for high performance. You can read about it here: (https://arxiv.org/abs/2012.15286)
 
-JAXNS uses a unique adaptive algorithm that enables arbitrary precision computing of evidence. Stay tuned for the paper that explains it.
+JAXNS is:
+
+1) a probabilistic programming framework using nested sampling as the engine;
+2) coded in JAX in a manner that allows lowering the entire inference algorithm to XLA primitives, which are
+   JIT-compiled for high performance;
+3) continuously improving on its mission of making nested sampling faster, easier, and more powerful; and
+4) citable, and you can read an (old) pre-print here: (https://arxiv.org/abs/2012.15286).
 
 # Documentation
 
-You can check out the docs [here](https://jaxns.readthedocs.io/en/latest/#).
+You can read the documentation [here](https://jaxns.readthedocs.io/en/latest/#).
 
 # Install
 
-Note: JAXNS requires >= Python 3.8, and is tested on 3.8, 3.9, 3.10, and 3.11.
+**Notes:**
+
+1. JAXNS requires >= Python 3.8.
+2. It is always highly recommended to use a unique virtual environment for each project.
+   To use `miniconda`, have it installed, and run
+
+```bash
+# To create a new env, if necessary
+conda create -n jaxns_py python=3.11
+conda activate jaxns_py
+```
+
+## For end users
+
+Install directly from PyPi,
 
-Make sure you have JAX and the usual suspects with `pip install jax jaxlib numpy matplotlib scipy`, optionally also `scikit-learn` and `haiku-dm` for some examples. 
-Install with `pip install jaxns` or `pip install git+http://github.com/Joshuaalbert/jaxns.git` for the (no promises) bleeding-edge.
+```bash
+pip install jaxns
+```
+
+## For development
+
+Clone repo `git clone https://www.github.com/JoshuaAlbert/jaxns.git`, and install:
+
+```bash
+cd jaxns
+pip install -r requirements.txt
+pip install -r requirements-tests.txt
+pip install -r requirements-examples.txt
+pip install .
+```
 
 # Getting help and contributing examples
 
-I'm really encourage anyone in the scientific community to get involved and join the discussion forum.
-Please use the [github discussion forum](https://github.com/Joshuaalbert/jaxns/discussions) for getting help, or contributing examples/neat use cases.
+Do you have a neat Bayesian problem, and want to solve it with JAXNS?
+I'm really encourage anyone in either the scientific community or industry to get involved and join the discussion
+forum.
+Please use the [github discussion forum](https://github.com/Joshuaalbert/jaxns/discussions) for getting help, or
+contributing examples/neat use cases.
 
 # Quick start
 
-JAXNS is really fast because it uses JAX. 
-The caveat is that you need to be able to define your likelihood function with JAX. This is usually no big deal because JAX is just a replacement for numpy and many likelihoods can be expressed such. 
+Checkout the examples [here](https://jaxns.readthedocs.io/en/latest/#).
+
+## Caveats
+
+The caveat is that you need to be able to define your likelihood function with JAX. This is usually no big deal because
+JAX is just a replacement for NumPy and many likelihoods can be expressed such.
 If you're unfamiliar, take a quick tour of JAX (https://jax.readthedocs.io/en/latest/notebooks/quickstart.html).
-Check out the examples for a starter.
 
 # Speed test comparison with other nested sampling packages
 
-JAXNS is much faster than PolyChord, MultiNEST, and dynesty, typically achieving two to three orders of magnitude improvement in speed on cheap likelihood evaluations.
-This is shown in (https://arxiv.org/abs/2012.15286). With regards to how efficiently JAXNS used likeihood evaluations, JAXNS prizes exactness over efficiency, however since it employs an adaptive strategy, users can control efficiency by controlling some precision parameters.
+JAXNS is really fast because it uses JAX.
+JAXNS is much faster than PolyChord, MultiNEST, and dynesty, typically achieving two to three orders of magnitude
+improvement in speed on cheap likelihood evaluations.
+This is shown in (https://arxiv.org/abs/2012.15286). With regards to how efficiently JAXNS used likelihood evaluations,
+JAXNS prizes exactness over efficiency, however since it employs an adaptive strategy, users can control efficiency by
+controlling some precision parameters.
 
 # Change Log
 
+15 June, 2023 -- JAXNS 2.2.0 released. Added support to allow TFP bijectors to defined transformed distributions. Other
+minor improvements.
+
+15 April, 2023 -- JAXNS 2.1.0 released. pmap used on outer-most loops allowing efficient device-device communication
+during parallel runs.
+
 8 March, 2023 -- JAXNS 2.0.1 released. Changed how we're doing annotations to support python 3.8 again.
 
 3 January, 2023 -- JAXNS 2.0 released. Complete overhaul of components. New way to build models.
 
 5 August, 2022 -- JAXNS 1.1.1 released. Pytree shaped priors.
 
-2 June, 2022 -- JAXNS 1.1.0 released. Dynamic sampling takes advantage of adaptive refinement. Parallelisation. Bayesian opt and global opt modules.
+2 June, 2022 -- JAXNS 1.1.0 released. Dynamic sampling takes advantage of adaptive refinement. Parallelisation. Bayesian
+opt and global opt modules.
 
 30 May, 2022 -- JAXNS 1.0.1 released. Improvements to speed, parallelisation, and structure of code.
 
-9 April, 2022 -- JAXNS 1.0.0 released. Parallel sampling, dynamic search, and adaptive refinement. Global optimiser released.
+9 April, 2022 -- JAXNS 1.0.0 released. Parallel sampling, dynamic search, and adaptive refinement. Global optimiser
+released.
 
 2 Jun, 2021 -- JAXNS 0.0.7 released.
 
 13 May, 2021 -- JAXNS 0.0.6 released.
 
 8 Mar, 2021 -- JAXNS 0.0.5 released.
 
 8 Mar, 2021 -- JAXNS 0.0.4 released.
 
-7 Mar, 2021 -- JAXNS 0.0.3 released. 
+7 Mar, 2021 -- JAXNS 0.0.3 released.
 
-28 Feb, 2021 -- JAXNS 0.0.2 released. 
+28 Feb, 2021 -- JAXNS 0.0.2 released.
 
-28 Feb, 2021 -- JAXNS 0.0.1 released. 
+28 Feb, 2021 -- JAXNS 0.0.1 released.
 
 1 January, 2021 -- Paper submitted
```

### Comparing `jaxns-2.1.0/jaxns.egg-info/SOURCES.txt` & `jaxns-2.2.0/jaxns.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 ./jaxns/adaptive_refinement.py
 ./jaxns/initial_state.py
 ./jaxns/model.py
 ./jaxns/nested_sampler.py
 ./jaxns/plotting.py
 ./jaxns/prior.py
 ./jaxns/random.py
-./jaxns/slice_sampler.py
 ./jaxns/special_priors.py
+./jaxns/static_nested_sampler.py
 ./jaxns/static_slice.py
 ./jaxns/static_uniform.py
 ./jaxns/statistics.py
 ./jaxns/termination.py
 ./jaxns/types.py
-./jaxns/uniform_sampler.py
 ./jaxns/utils.py
+./jaxns/warnings.py
 ./jaxns.egg-info/PKG-INFO
 ./jaxns.egg-info/SOURCES.txt
 ./jaxns.egg-info/dependency_links.txt
 ./jaxns.egg-info/top_level.txt
 ./jaxns/internals/__init__.py
 ./jaxns/internals/linalg.py
 ./jaxns/internals/log_semiring.py
@@ -32,17 +32,20 @@
 ./jaxns/internals/tests/__init__.py
 ./jaxns/internals/tests/test_linalg.py
 ./jaxns/internals/tests/test_log_semiring.py
 ./jaxns/internals/tests/test_maps.py
 ./jaxns/internals/tests/test_shapes.py
 ./jaxns/internals/tests/test_stats.py
 ./jaxns/likelihood_samplers/__init__.py
+./jaxns/likelihood_samplers/em_gmm.py
 ./jaxns/likelihood_samplers/multi_ellipsoid_utils.py
 ./jaxns/likelihood_samplers/tests/__init__.py
+./jaxns/likelihood_samplers/tests/test_em_gmm.py
 ./jaxns/likelihood_samplers/tests/test_multi_ellipsoid.py
 ./jaxns/tests/__init__.py
+./jaxns/tests/test_adaptive_refinement.py
 ./jaxns/tests/test_initial_state.py
 ./jaxns/tests/test_nested_sampler.py
 ./jaxns/tests/test_prior.py
 ./jaxns/tests/test_random.py
 ./jaxns/tests/test_statistics.py
 ./jaxns/tests/test_utils.py
```

### Comparing `jaxns-2.1.0/setup.py` & `jaxns-2.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 setup_requires = ['jax>=' + __minimum_jax_version__]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='jaxns',
-      version='2.1.0',
+      version='2.2.0',
       description='Nested Sampling in JAX',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/joshuaalbert/jaxns",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       setup_requires=setup_requires,
```

