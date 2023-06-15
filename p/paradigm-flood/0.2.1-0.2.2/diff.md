# Comparing `tmp/paradigm-flood-0.2.1.tar.gz` & `tmp/paradigm-flood-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paradigm-flood-0.2.1.tar", last modified: Tue Jun  6 15:07:48 2023, max compression
+gzip compressed data, was "paradigm-flood-0.2.2.tar", last modified: Thu Jun 15 06:39:52 2023, max compression
```

## Comparing `paradigm-flood-0.2.1.tar` & `paradigm-flood-0.2.2.tar`

### file list

```diff
@@ -1,62 +1,71 @@
--rw-r--r--   0        0        0      225 2023-05-06 04:56:40.389625 paradigm-flood-0.2.1/.gitignore
--rw-r--r--   0        0        0    10332 2023-06-04 20:22:19.525565 paradigm-flood-0.2.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      832 2023-06-02 00:45:29.473078 paradigm-flood-0.2.1/Dockerfile
--rw-r--r--   0        0        0    10839 2023-06-04 20:13:59.817606 paradigm-flood-0.2.1/LICENSE-APACHE
--rw-r--r--   0        0        0     1085 2023-06-04 20:13:48.830823 paradigm-flood-0.2.1/LICENSE-MIT
--rw-r--r--   0        0        0     2434 2023-06-06 01:32:05.739668 paradigm-flood-0.2.1/README.md
--rw-r--r--   0        0        0      625 2023-06-06 15:07:21.901429 paradigm-flood-0.2.1/flood/__init__.py
--rw-r--r--   0        0        0      117 2023-06-04 23:14:01.291195 paradigm-flood-0.2.1/flood/__main__.py
--rw-r--r--   0        0        0     1509 2023-06-04 23:14:01.296616 paradigm-flood-0.2.1/flood/cli/cli_run.py
--rw-r--r--   0        0        0      877 2023-06-04 23:14:01.298637 paradigm-flood-0.2.1/flood/cli/ls_command.py
--rw-r--r--   0        0        0     1221 2023-06-04 23:14:01.302153 paradigm-flood-0.2.1/flood/cli/report_command.py
--rw-r--r--   0        0        0     5701 2023-06-04 23:14:01.321565 paradigm-flood-0.2.1/flood/cli/root_command.py
--rw-r--r--   0        0        0     1315 2023-06-04 23:14:01.307482 paradigm-flood-0.2.1/flood/cli/samples_collect_command.py
--rw-r--r--   0        0        0     1673 2023-06-04 23:14:01.307524 paradigm-flood-0.2.1/flood/cli/samples_download_command.py
--rw-r--r--   0        0        0     1860 2023-06-04 23:14:01.318783 paradigm-flood-0.2.1/flood/cli/samples_ls_command.py
--rw-r--r--   0        0        0      121 2023-06-03 19:54:58.405209 paradigm-flood-0.2.1/flood/generators/__init__.py
--rw-r--r--   0        0        0      199 2023-06-03 19:54:39.491471 paradigm-flood-0.2.1/flood/generators/object_generators/__init__.py
--rw-r--r--   0        0        0      603 2023-06-04 23:14:01.311234 paradigm-flood-0.2.1/flood/generators/object_generators/address_generators.py
--rw-r--r--   0        0        0     4815 2023-06-04 23:14:01.335388 paradigm-flood-0.2.1/flood/generators/object_generators/block_generators.py
--rw-r--r--   0        0        0    17228 2023-06-04 23:14:01.443043 paradigm-flood-0.2.1/flood/generators/object_generators/call_generators.py
--rw-r--r--   0        0        0      337 2023-06-04 23:14:01.306215 paradigm-flood-0.2.1/flood/generators/object_generators/slot_generators.py
--rw-r--r--   0        0        0     4128 2023-06-04 23:14:01.342234 paradigm-flood-0.2.1/flood/generators/object_generators/timing_generators.py
--rw-r--r--   0        0        0      346 2023-06-04 23:14:01.315806 paradigm-flood-0.2.1/flood/generators/object_generators/transaction_generators.py
--rw-r--r--   0        0        0      129 2023-06-02 06:40:02.759112 paradigm-flood-0.2.1/flood/generators/raw_data_sources/__init__.py
--rw-r--r--   0        0        0      465 2023-06-04 23:14:01.312615 paradigm-flood-0.2.1/flood/generators/raw_data_sources/raw_data_spec.py
--rw-r--r--   0        0        0     1935 2023-06-04 23:14:01.327302 paradigm-flood-0.2.1/flood/generators/raw_data_sources/raw_download_utils.py
--rw-r--r--   0        0        0     5688 2023-06-04 23:14:01.364193 paradigm-flood-0.2.1/flood/generators/raw_data_sources/raw_gather_utils.py
--rw-r--r--   0        0        0     4662 2023-06-04 23:14:01.352117 paradigm-flood-0.2.1/flood/generators/raw_data_sources/raw_sample_loading.py
--rw-r--r--   0        0        0      530 2023-06-04 23:14:01.322799 paradigm-flood-0.2.1/flood/generators/rng_utils.py
--rw-r--r--   0        0        0      270 2023-06-02 21:54:22.919273 paradigm-flood-0.2.1/flood/generators/test_generators/__init__.py
--rw-r--r--   0        0        0     1507 2023-06-04 23:14:01.337667 paradigm-flood-0.2.1/flood/generators/test_generators/address_test_generators.py
--rw-r--r--   0        0        0     1559 2023-06-04 23:14:01.331116 paradigm-flood-0.2.1/flood/generators/test_generators/block_test_generators.py
--rw-r--r--   0        0        0     2150 2023-06-04 23:14:01.346034 paradigm-flood-0.2.1/flood/generators/test_generators/contract_test_generators.py
--rw-r--r--   0        0        0     3713 2023-06-04 23:14:01.359661 paradigm-flood-0.2.1/flood/generators/test_generators/generic_test_generators.py
--rw-r--r--   0        0        0     3870 2023-06-04 23:14:01.341234 paradigm-flood-0.2.1/flood/generators/test_generators/log_test_generators.py
--rw-r--r--   0        0        0     5897 2023-06-04 23:14:01.413684 paradigm-flood-0.2.1/flood/generators/test_generators/trace_test_generators.py
--rw-r--r--   0        0        0     1512 2023-06-04 23:14:01.354881 paradigm-flood-0.2.1/flood/generators/test_generators/transaction_test_generators.py
--rw-r--r--   0        0        0     5060 2023-06-04 23:14:01.380065 paradigm-flood-0.2.1/flood/spec.py
--rw-r--r--   0        0        0       78 2023-06-04 23:14:01.343121 paradigm-flood-0.2.1/flood/tests/__init__.py
--rw-r--r--   0        0        0       34 2023-06-04 23:14:01.345292 paradigm-flood-0.2.1/flood/tests/equality_tests/__init__.py
--rw-r--r--   0        0        0     8677 2023-06-04 23:14:01.423939 paradigm-flood-0.2.1/flood/tests/equality_tests/equality_test_runs.py
--rw-r--r--   0        0        0     8375 2023-06-04 23:14:01.401754 paradigm-flood-0.2.1/flood/tests/equality_tests/equality_test_sets.py
--rw-r--r--   0        0        0      154 2023-06-02 00:45:29.480806 paradigm-flood-0.2.1/flood/tests/load_tests/__init__.py
--rw-r--r--   0        0        0     2682 2023-06-04 23:14:01.379714 paradigm-flood-0.2.1/flood/tests/load_tests/load_test_construction.py
--rw-r--r--   0        0        0     5741 2023-06-04 23:14:01.398331 paradigm-flood-0.2.1/flood/tests/load_tests/load_test_plots.py
--rw-r--r--   0        0        0    10208 2023-06-06 15:07:11.584179 paradigm-flood-0.2.1/flood/tests/load_tests/load_test_reports.py
--rw-r--r--   0        0        0    10751 2023-06-04 23:14:01.455828 paradigm-flood-0.2.1/flood/tests/load_tests/load_test_runs.py
--rw-r--r--   0        0        0     4916 2023-06-04 23:14:01.417311 paradigm-flood-0.2.1/flood/tests/load_tests/vegeta.py
--rw-r--r--   0        0        0    12506 2023-06-04 23:14:01.459741 paradigm-flood-0.2.1/flood/tests/runner.py
--rw-r--r--   0        0        0       68 2023-06-02 00:45:29.482030 paradigm-flood-0.2.1/flood/user_io/__init__.py
--rw-r--r--   0        0        0     3265 2023-06-04 23:14:01.401591 paradigm-flood-0.2.1/flood/user_io/file_io.py
--rw-r--r--   0        0        0     5886 2023-06-04 23:14:01.446135 paradigm-flood-0.2.1/flood/user_io/inputs.py
--rw-r--r--   0        0        0     4285 2023-06-04 23:14:01.438468 paradigm-flood-0.2.1/flood/user_io/notebook_io.py
--rw-r--r--   0        0        0     5851 2023-06-04 23:14:01.447395 paradigm-flood-0.2.1/flood/user_io/outputs.py
--rw-r--r--   0        0        0     1842 2023-06-06 00:35:48.011034 paradigm-flood-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      381 2023-06-04 20:35:57.569281 paradigm-flood-0.2.1/tests/README.md
--rw-r--r--   0        0        0      582 2023-06-04 20:33:44.674285 paradigm-flood-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0      593 2023-06-04 20:53:58.379044 paradigm-flood-0.2.1/tests/test_env_vars.py
--rw-r--r--   0        0        0      270 2023-06-04 21:22:03.070619 paradigm-flood-0.2.1/tests/test_equality_tests.py
--rw-r--r--   0        0        0     1072 2023-06-04 21:21:55.766285 paradigm-flood-0.2.1/tests/test_load_tests.py
--rw-r--r--   0        0        0     1736 2023-06-04 16:00:15.996050 paradigm-flood-0.2.1/tests/test_node_parsing.py
--rw-r--r--   0        0        0     4058 1970-01-01 00:00:00.000000 paradigm-flood-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-06-06 19:32:53.475871 paradigm-flood-0.2.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      607 2023-06-06 19:32:53.476113 paradigm-flood-0.2.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      193 2023-06-06 19:32:53.476353 paradigm-flood-0.2.2/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0      781 2023-06-06 19:32:53.476534 paradigm-flood-0.2.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      165 2023-06-06 19:32:53.476751 paradigm-flood-0.2.2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      513 2023-06-06 21:16:25.551820 paradigm-flood-0.2.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      225 2023-05-06 04:56:40.389625 paradigm-flood-0.2.2/.gitignore
+-rw-r--r--   0        0        0    10332 2023-06-04 20:22:19.525565 paradigm-flood-0.2.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      832 2023-06-02 00:45:29.473078 paradigm-flood-0.2.2/Dockerfile
+-rw-r--r--   0        0        0    10839 2023-06-04 20:13:59.817606 paradigm-flood-0.2.2/LICENSE-APACHE
+-rw-r--r--   0        0        0     1085 2023-06-04 20:13:48.830823 paradigm-flood-0.2.2/LICENSE-MIT
+-rw-r--r--   0        0        0     2865 2023-06-06 19:32:53.477627 paradigm-flood-0.2.2/README.md
+-rw-r--r--   0        0        0  3038209 2023-06-06 19:32:53.483637 paradigm-flood-0.2.2/assets/cover.png
+-rw-r--r--   0        0        0      124 2023-06-06 21:20:36.150174 paradigm-flood-0.2.2/examples/equality_test.sh
+-rwxr-xr-x   0        0        0     1905 2023-06-06 21:26:28.863576 paradigm-flood-0.2.2/examples/report.sh
+-rw-r--r--   0        0        0      625 2023-06-15 06:39:10.965720 paradigm-flood-0.2.2/flood/__init__.py
+-rw-r--r--   0        0        0      117 2023-06-04 23:14:01.291195 paradigm-flood-0.2.2/flood/__main__.py
+-rw-r--r--   0        0        0     1509 2023-06-04 23:14:01.296616 paradigm-flood-0.2.2/flood/cli/cli_run.py
+-rw-r--r--   0        0        0      877 2023-06-04 23:14:01.298637 paradigm-flood-0.2.2/flood/cli/ls_command.py
+-rw-r--r--   0        0        0     1221 2023-06-04 23:14:01.302153 paradigm-flood-0.2.2/flood/cli/report_command.py
+-rw-r--r--   0        0        0     5729 2023-06-06 20:38:56.286320 paradigm-flood-0.2.2/flood/cli/root_command.py
+-rw-r--r--   0        0        0     1315 2023-06-04 23:14:01.307482 paradigm-flood-0.2.2/flood/cli/samples_collect_command.py
+-rw-r--r--   0        0        0     1687 2023-06-06 20:39:09.158213 paradigm-flood-0.2.2/flood/cli/samples_download_command.py
+-rw-r--r--   0        0        0     1874 2023-06-06 20:39:23.569867 paradigm-flood-0.2.2/flood/cli/samples_ls_command.py
+-rw-r--r--   0        0        0      121 2023-06-03 19:54:58.405209 paradigm-flood-0.2.2/flood/generators/__init__.py
+-rw-r--r--   0        0        0      199 2023-06-03 19:54:39.491471 paradigm-flood-0.2.2/flood/generators/object_generators/__init__.py
+-rw-r--r--   0        0        0      603 2023-06-04 23:14:01.311234 paradigm-flood-0.2.2/flood/generators/object_generators/address_generators.py
+-rw-r--r--   0        0        0     4815 2023-06-04 23:14:01.335388 paradigm-flood-0.2.2/flood/generators/object_generators/block_generators.py
+-rw-r--r--   0        0        0    17256 2023-06-06 20:39:37.317485 paradigm-flood-0.2.2/flood/generators/object_generators/call_generators.py
+-rw-r--r--   0        0        0      337 2023-06-04 23:14:01.306215 paradigm-flood-0.2.2/flood/generators/object_generators/slot_generators.py
+-rw-r--r--   0        0        0     4156 2023-06-06 20:41:05.406418 paradigm-flood-0.2.2/flood/generators/object_generators/timing_generators.py
+-rw-r--r--   0        0        0      346 2023-06-04 23:14:01.315806 paradigm-flood-0.2.2/flood/generators/object_generators/transaction_generators.py
+-rw-r--r--   0        0        0      129 2023-06-02 06:40:02.759112 paradigm-flood-0.2.2/flood/generators/raw_data_sources/__init__.py
+-rw-r--r--   0        0        0      465 2023-06-04 23:14:01.312615 paradigm-flood-0.2.2/flood/generators/raw_data_sources/raw_data_spec.py
+-rw-r--r--   0        0        0     1935 2023-06-04 23:14:01.327302 paradigm-flood-0.2.2/flood/generators/raw_data_sources/raw_download_utils.py
+-rw-r--r--   0        0        0     5688 2023-06-04 23:14:01.364193 paradigm-flood-0.2.2/flood/generators/raw_data_sources/raw_gather_utils.py
+-rw-r--r--   0        0        0     4662 2023-06-04 23:14:01.352117 paradigm-flood-0.2.2/flood/generators/raw_data_sources/raw_sample_loading.py
+-rw-r--r--   0        0        0      530 2023-06-04 23:14:01.322799 paradigm-flood-0.2.2/flood/generators/rng_utils.py
+-rw-r--r--   0        0        0      270 2023-06-02 21:54:22.919273 paradigm-flood-0.2.2/flood/generators/test_generators/__init__.py
+-rw-r--r--   0        0        0     1507 2023-06-04 23:14:01.337667 paradigm-flood-0.2.2/flood/generators/test_generators/address_test_generators.py
+-rw-r--r--   0        0        0     1559 2023-06-04 23:14:01.331116 paradigm-flood-0.2.2/flood/generators/test_generators/block_test_generators.py
+-rw-r--r--   0        0        0     2150 2023-06-04 23:14:01.346034 paradigm-flood-0.2.2/flood/generators/test_generators/contract_test_generators.py
+-rw-r--r--   0        0        0     3713 2023-06-04 23:14:01.359661 paradigm-flood-0.2.2/flood/generators/test_generators/generic_test_generators.py
+-rw-r--r--   0        0        0     3870 2023-06-04 23:14:01.341234 paradigm-flood-0.2.2/flood/generators/test_generators/log_test_generators.py
+-rw-r--r--   0        0        0     5897 2023-06-04 23:14:01.413684 paradigm-flood-0.2.2/flood/generators/test_generators/trace_test_generators.py
+-rw-r--r--   0        0        0     1512 2023-06-04 23:14:01.354881 paradigm-flood-0.2.2/flood/generators/test_generators/transaction_test_generators.py
+-rw-r--r--   0        0        0     5060 2023-06-04 23:14:01.380065 paradigm-flood-0.2.2/flood/spec.py
+-rw-r--r--   0        0        0       78 2023-06-04 23:14:01.343121 paradigm-flood-0.2.2/flood/tests/__init__.py
+-rw-r--r--   0        0        0       34 2023-06-04 23:14:01.345292 paradigm-flood-0.2.2/flood/tests/equality_tests/__init__.py
+-rw-r--r--   0        0        0     6029 2023-06-15 06:20:28.831486 paradigm-flood-0.2.2/flood/tests/equality_tests/equality_test_runs.py
+-rw-r--r--   0        0        0     8501 2023-06-06 20:41:24.278488 paradigm-flood-0.2.2/flood/tests/equality_tests/equality_test_sets.py
+-rw-r--r--   0        0        0      154 2023-06-02 00:45:29.480806 paradigm-flood-0.2.2/flood/tests/load_tests/__init__.py
+-rw-r--r--   0        0        0     2682 2023-06-04 23:14:01.379714 paradigm-flood-0.2.2/flood/tests/load_tests/load_test_construction.py
+-rw-r--r--   0        0        0     5741 2023-06-04 23:14:01.398331 paradigm-flood-0.2.2/flood/tests/load_tests/load_test_plots.py
+-rw-r--r--   0        0        0    10264 2023-06-06 20:42:07.952278 paradigm-flood-0.2.2/flood/tests/load_tests/load_test_reports.py
+-rw-r--r--   0        0        0    10809 2023-06-06 20:43:29.736775 paradigm-flood-0.2.2/flood/tests/load_tests/load_test_runs.py
+-rw-r--r--   0        0        0     4916 2023-06-04 23:14:01.417311 paradigm-flood-0.2.2/flood/tests/load_tests/vegeta.py
+-rw-r--r--   0        0        0    12506 2023-06-04 23:14:01.459741 paradigm-flood-0.2.2/flood/tests/runner.py
+-rw-r--r--   0        0        0       68 2023-06-02 00:45:29.482030 paradigm-flood-0.2.2/flood/user_io/__init__.py
+-rw-r--r--   0        0        0     3265 2023-06-04 23:14:01.401591 paradigm-flood-0.2.2/flood/user_io/file_io.py
+-rw-r--r--   0        0        0     5903 2023-06-15 06:32:18.240729 paradigm-flood-0.2.2/flood/user_io/inputs.py
+-rw-r--r--   0        0        0     4285 2023-06-04 23:14:01.438468 paradigm-flood-0.2.2/flood/user_io/notebook_io.py
+-rw-r--r--   0        0        0     5864 2023-06-06 20:35:25.703304 paradigm-flood-0.2.2/flood/user_io/outputs.py
+-rw-r--r--   0        0        0     1890 2023-06-15 06:36:29.930748 paradigm-flood-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      381 2023-06-04 20:35:57.569281 paradigm-flood-0.2.2/tests/README.md
+-rw-r--r--   0        0        0      993 2023-06-06 21:03:30.304627 paradigm-flood-0.2.2/tests/conftest.py
+-rw-r--r--   0        0        0      593 2023-06-04 20:53:58.379044 paradigm-flood-0.2.2/tests/test_env_vars.py
+-rw-r--r--   0        0        0      269 2023-06-06 21:04:00.022725 paradigm-flood-0.2.2/tests/test_equality_tests.py
+-rw-r--r--   0        0        0     1128 2023-06-06 21:03:47.012574 paradigm-flood-0.2.2/tests/test_load_tests.py
+-rw-r--r--   0        0        0     1736 2023-06-04 16:00:15.996050 paradigm-flood-0.2.2/tests/test_node_parsing.py
+-rw-r--r--   0        0        0     4489 1970-01-01 00:00:00.000000 paradigm-flood-0.2.2/PKG-INFO
```

### Comparing `paradigm-flood-0.2.1/CONTRIBUTING.md` & `paradigm-flood-0.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/Dockerfile` & `paradigm-flood-0.2.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/LICENSE-APACHE` & `paradigm-flood-0.2.2/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/LICENSE-MIT` & `paradigm-flood-0.2.2/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/README.md` & `paradigm-flood-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 
-# 🌊🌊 flood 🌊🌊
+# <h1 align="center"> 🌊🌊 flood 🌊🌊 </h1>
 
-`flood` is a load testing tool for benchmarking EVM nodes over RPC
+**`flood` is a load testing tool for benchmarking EVM nodes over RPC**
+
+![](./assets/cover.png)
+
+[![CI status](https://github.com/paradigmxyz/flood/workflows/Pytest/badge.svg)][gh-ci]
+[![Telegram Chat][tg-badge]][tg-url]
+
+[gh-ci]: https://github.com/paradigmxyz/flood/actions/workflows/ci.yml
+[tg-badge]: https://img.shields.io/endpoint?color=neon&logo=telegram&label=chat&url=https%3A%2F%2Ftg.sumanjay.workers.dev%2Fparadigm%5Fflood
+[tg-url]: https://t.me/paradigm_flood
 
 For each RPC method, `flood` measures how load affects metrics such as:
 1. throughput
 2. latency (mean, P50, P90, P95, P99, max)
 3. error rate
 
 `flood` makes it easy to compare the performance of:
```

### Comparing `paradigm-flood-0.2.1/flood/__init__.py` & `paradigm-flood-0.2.2/flood/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from .generators import *
 from .spec import *
 from .tests import *
 from .user_io import *
 
 
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 
 
 def _clean_package_imports() -> None:
     """remove deep nested modules from flood namespace"""
 
     import sys
```

### Comparing `paradigm-flood-0.2.1/flood/cli/cli_run.py` & `paradigm-flood-0.2.2/flood/cli/cli_run.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/cli/ls_command.py` & `paradigm-flood-0.2.2/flood/cli/ls_command.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/cli/report_command.py` & `paradigm-flood-0.2.2/flood/cli/report_command.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/cli/root_command.py` & `paradigm-flood-0.2.2/flood/cli/root_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,25 @@
 - Use node syntax [metavar]user@remote:node_url[/metavar] or [metavar]name=user@remote:node_url[/metavar]
 - Can omit the [metavar]user@[/metavar] prefix if ssh config has username specified
 - [metavar]flood[/metavar] must already be installed on each remote machine
 
 [bold][title]Parameter Randomization[/bold][/title]
 - [metavar]flood[/metavar] can call each RPC method multiple times using [metavar]-n <N>[/metavar]
 - For each call, parameters are randomized to minimize caching effects
-- Specify random seed [metavar]-s <seed>[/metavar] for repeatable set of randomized calls"""
+- Specify random seed [metavar]-s <seed>[/metavar] for repeatable set of randomized calls"""  # noqa: E501
 
 
 def get_command_spec() -> toolcli.CommandSpec:
     return {
         'f': root_command,
         'help': help_message,
         'args': [
             {
                 'name': 'test',
-                'help': 'test to run (use [metavar]flood ls[/metavar] for list)',
+                'help': 'test to run (use [metavar]flood ls[/metavar] for list)',  # noqa: E501
             },
             {
                 'name': 'nodes',
                 'nargs': '*',
                 'help': 'nodes to test, see syntax above',
             },
             {
```

### Comparing `paradigm-flood-0.2.1/flood/cli/samples_collect_command.py` & `paradigm-flood-0.2.2/flood/cli/samples_collect_command.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/cli/samples_download_command.py` & `paradigm-flood-0.2.2/flood/cli/samples_download_command.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         'args': [
             {
                 'name': ('-n', '--network'),
                 'help': 'network, default ethereum',
             },
             {
                 'name': ('-s', '--sizes'),
-                'help': 'sample sizes, one of {XS, S, M, L, XL, all}, default L',
+                'help': 'sample sizes, one of {XS, S, M, L, XL, all}, default L',  # noqa: E501
                 'nargs': '+',
             },
             {
                 'name': ('-o', '--output-dir'),
                 'help': 'download location, default FLOOD_SAMPLES_DIR or cwd',
             },
             {
```

### Comparing `paradigm-flood-0.2.1/flood/cli/samples_ls_command.py` & `paradigm-flood-0.2.2/flood/cli/samples_ls_command.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import flood
 
 
 def get_command_spec() -> toolcli.CommandSpec:
     return {
         'f': samples_ls_command,
-        'help': 'list raw EVM data samples that are downloaded and downloadable',
+        'help': 'list raw EVM data samples that are downloaded and downloadable',  # noqa: E501
         'args': [],
     }
 
 
 def samples_ls_command() -> None:
     version = 'v1_0_0'
```

### Comparing `paradigm-flood-0.2.1/flood/generators/object_generators/address_generators.py` & `paradigm-flood-0.2.2/flood/generators/object_generators/address_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/generators/object_generators/block_generators.py` & `paradigm-flood-0.2.2/flood/generators/object_generators/block_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/generators/object_generators/call_generators.py` & `paradigm-flood-0.2.2/flood/generators/object_generators/call_generators.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,16 +204,16 @@
 _default_contracts = {
     'USDC': '0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48',
     'DAI': '0x6b175474e89094c44da98b954eedeac495271d0f',
     'LUSD': '0x5f98805a4e8be255a32880fdec7f6728c6568ba0',
 }
 
 _default_event_hashes = {
-    'Transfer': '0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef',
-    'Approval': '0x8c5be1e5ebec7d5bd14f71427d1e84f3dd0314c0f7b2291e5b200ac8c7c3b925',
+    'Transfer': '0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef',  # noqa: E501
+    'Approval': '0x8c5be1e5ebec7d5bd14f71427d1e84f3dd0314c0f7b2291e5b200ac8c7c3b925',  # noqa: E501
 }
 
 
 def generate_calls_eth_get_logs(
     n_calls: int | None = None,
     *,
     contract_address: str | None = None,
```

### Comparing `paradigm-flood-0.2.1/flood/generators/object_generators/timing_generators.py` & `paradigm-flood-0.2.2/flood/generators/object_generators/timing_generators.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                 rates[0],
                 default_spike_rates['after'],
             ]
         elif len(rates) == 3:
             pass
         else:
             raise Exception(
-                'must specify eith a single spike rate or a [before, during, after] triplet of rates'
+                'must specify eith a single spike rate or a [before, during, after] triplet of rates'  # noqa: E501
             )
 
     if duration is not None:
         durations = [
             default_spike_durations['before'],
             duration,
             default_spike_durations['after'],
@@ -106,15 +106,15 @@
                 durations[0],
                 default_spike_durations['after'],
             ]
         elif len(durations) == 3:
             pass
         else:
             raise Exception(
-                'must specify eith a single spike duration or a [before, during, after] triplet of rates'
+                'must specify eith a single spike duration or a [before, during, after] triplet of rates'  # noqa: E501
             )
     else:
         durations = [
             default_spike_durations['before'],
             default_spike_durations['during'],
             default_spike_durations['after'],
         ]
```

### Comparing `paradigm-flood-0.2.1/flood/generators/raw_data_sources/raw_download_utils.py` & `paradigm-flood-0.2.2/flood/generators/raw_data_sources/raw_download_utils.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/generators/raw_data_sources/raw_gather_utils.py` & `paradigm-flood-0.2.2/flood/generators/raw_data_sources/raw_gather_utils.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/generators/raw_data_sources/raw_sample_loading.py` & `paradigm-flood-0.2.2/flood/generators/raw_data_sources/raw_sample_loading.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/generators/rng_utils.py` & `paradigm-flood-0.2.2/flood/generators/rng_utils.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/generators/test_generators/address_test_generators.py` & `paradigm-flood-0.2.2/flood/generators/test_generators/address_test_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/generators/test_generators/block_test_generators.py` & `paradigm-flood-0.2.2/flood/generators/test_generators/block_test_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/generators/test_generators/contract_test_generators.py` & `paradigm-flood-0.2.2/flood/generators/test_generators/contract_test_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/generators/test_generators/generic_test_generators.py` & `paradigm-flood-0.2.2/flood/generators/test_generators/generic_test_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/generators/test_generators/log_test_generators.py` & `paradigm-flood-0.2.2/flood/generators/test_generators/log_test_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/generators/test_generators/trace_test_generators.py` & `paradigm-flood-0.2.2/flood/generators/test_generators/trace_test_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/generators/test_generators/transaction_test_generators.py` & `paradigm-flood-0.2.2/flood/generators/test_generators/transaction_test_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/spec.py` & `paradigm-flood-0.2.2/flood/spec.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/tests/equality_tests/equality_test_runs.py` & `paradigm-flood-0.2.2/flood/tests/equality_tests/equality_test_runs.py`

 * *Files 24% similar despite different names*

```diff
@@ -128,32 +128,26 @@
             flood.print_bullet(key=name, value='', colon_str='')
     print()
     toolstr.print(
         'summary saved to: ' + file_path, style=flood.styles['comment']
     )
 
 
-def _json_equal(lhs: typing.Any, rhs: typing.Any) -> bool:
-    import json
-
-    return json.dumps(lhs, sort_keys=True) == json.dumps(rhs, sort_keys=True)
-
-
 def _summarize_result(
     responses: typing.Sequence[typing.Any],
     results: typing.Sequence[typing.Any],
     nodes: flood.Nodes,
     test: flood.EqualityTest,
     call: typing.Mapping[str, typing.Any],
 ) -> bool:
     import toolstr
 
     test_name, constructor, args, kwargs = test
 
-    if not _json_equal(results[0], results[1]):
+    if not toolstr.nested_equal(results[0], results[1]):
         print()
         flood.print_text_box('Discrepancies in ' + test_name)
         print()
         flood.print_header('args')
         if len(args) > 0:
             for arg in args:
                 flood.print_bullet(key=arg, value='', colon_str='')
@@ -167,110 +161,37 @@
         if any(result is None for result in results):
             print()
         for node, result, response in zip(nodes.values(), results, responses):
             if result is None:
                 toolstr.print(
                     node['name'] + ' failed', style=flood.styles['title']
                 )
-                if response.status_code == 200:
+                if response is None:
+                    print('response: no response')
+                elif response.status_code == 200:
                     print('response:', response.json())
                 else:
                     print('response: status code ', response.status_code)
 
         if results[0] is None or results[1] is None:
             return False
 
-        _print_result_diff(results=results, nodes=list(nodes.values()))
-
-        return False
-
-    else:
-        return True
-
-
-def _print_result_diff(
-    results: typing.Sequence[typing.Any],
-    nodes: typing.Sequence[flood.Node],
-) -> None:
-    import toolstr
-
-    result0 = results[0]
-    result1 = results[1]
-
-    if type(result0) is not type(result1):
-        for node, result in zip(nodes, results):
-            print(node['name'], 'type:', type(result))
-        return
-
-    if isinstance(result0, dict):
-        keys0 = set(result0.keys())
-        keys1 = set(result1.keys())
-        if keys0 != keys1:
-            only_in_0 = keys0 - keys1
-            only_in_1 = keys1 - keys0
-            print()
-            flood.print_header('different fields in results')
-            if len(only_in_0) > 0:
-                print(
-                    '- present only in',
-                    nodes[0]['name'] + ':',
-                    ', '.join(only_in_0),
-                )
-            if len(only_in_1) > 0:
-                print(
-                    '- present only in',
-                    nodes[1]['name'] + ':',
-                    ', '.join(only_in_1),
-                )
-
-        rows = []
-        for key in keys0 & keys1:
-            if not _json_equal(result0[key], result1[key]):
-                row = [key, result0[key], result1[key]]
-                rows.append(row)
-        if len(rows) > 0:
+        if len(results) == 2:
+            node0, node1 = list(nodes.values())
             print()
-            flood.print_header('differences in values')
-            flood.print_table(
-                rows,
-                labels=['field', nodes[0]['name'], nodes[1]['name']],
-                compact=3,
-                max_column_widths=[20, 30, 30],
+            flood.print_header('differences in response')
+            toolstr.print_nested_diff(
+                lhs=results[0],
+                rhs=results[1],
+                lhs_name=node0['name'],
+                rhs_name=node1['name'],
+                styles=flood.styles,
                 indent=4,
             )
-
-    elif isinstance(result0, list):
-        if len(result1) != len(result0):
-            print()
-            flood.print_header('different number of results')
-            for node, result in zip(nodes, results):
-                flood.print_bullet(
-                    key=node['name'], value=str(len(result)) + ' results'
-                )
         else:
-            import json
-
-            print('differences:')
-            n_printed = 0
-            for i, (item0, item1) in enumerate(zip(result0, result1)):
-                if not _json_equal(item0, item1):
-                    if n_printed >= 10:
-                        print('...')
-                        break
-
-                    item0_str = json.dumps(item0)
-                    if len(item0_str) > 20:
-                        item0_str = item0_str[:17] + '...'
-                    item1_str = json.dumps(item1)
-                    if len(item1_str) > 20:
-                        item1_str = item1_str[:17] + '...'
-                    print('- item at index', i)
-                    print('    -', nodes[0]['name'] + ':', item0_str)
-                    print('    -', nodes[1]['name'] + ':', item1_str)
+            print('omitting details when >2 nodes tested')
 
-                    n_printed += 1
+        return False
 
     else:
-        if result1 != result0:
-            flood.print_header('differences in values')
-            for node, result in zip(nodes, results):
-                flood.print_bullet(key=node['name'], value=result)
+        return True
+
```

### Comparing `paradigm-flood-0.2.1/flood/tests/equality_tests/equality_test_sets.py` & `paradigm-flood-0.2.2/flood/tests/equality_tests/equality_test_sets.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         ),
         (
             'eth_getStorageAt',
             ctc.rpc.construct_eth_get_storage_at,
             [],
             {
                 'address': '0x4d9079bb4165aeb4084c526a32695dcfd2f77381',
-                'position': '0x0000000000000000000000000000000000000000000000000000000000000002',
+                'position': '0x0000000000000000000000000000000000000000000000000000000000000002',  # noqa: E501
                 'block_number': start_block,
             },
         ),
         (
             'eth_getCode',
             ctc.rpc.construct_eth_get_code,
             ['0x4d9079bb4165aeb4084c526a32695dcfd2f77381'],
@@ -106,31 +106,31 @@
             [start_block],
             {},
         ),
         (
             'eth_getBlockByHash',
             ctc.rpc.construct_eth_get_block_by_hash,
             [
-                '0x3dc4ef568ae2635db1419c5fec55c4a9322c05302ae527cd40bff380c1d465dd'
+                '0x3dc4ef568ae2635db1419c5fec55c4a9322c05302ae527cd40bff380c1d465dd'  # noqa: E501
             ],
             {},
         ),
         (
             'eth_getTransactionByHash',
             ctc.rpc.construct_eth_get_transaction_by_hash,
             [
-                '0xd01212e8ab48d2fd2ea9c4f33f8670fd1cf0cfb09d2e3c6ceddfaf54152386e5'
+                '0xd01212e8ab48d2fd2ea9c4f33f8670fd1cf0cfb09d2e3c6ceddfaf54152386e5'  # noqa: E501
             ],
             {},
         ),
         (
             'eth_getTransactionReceipt',
             ctc.rpc.construct_eth_get_transaction_receipt,
             [
-                '0xd01212e8ab48d2fd2ea9c4f33f8670fd1cf0cfb09d2e3c6ceddfaf54152386e5'
+                '0xd01212e8ab48d2fd2ea9c4f33f8670fd1cf0cfb09d2e3c6ceddfaf54152386e5'  # noqa: E501
             ],
             {},
         ),
         (
             'eth_call',
             ctc.rpc.construct_eth_call,
             [],
@@ -214,15 +214,15 @@
         (
             'trace_call_many',
             ctc.rpc.construct_trace_call_many,
             [],
             {
                 'calls': [
                     {
-                        'to_address': '0x6b175474e89094c44da98b954eedeac495271d0f',
+                        'to_address': '0x6b175474e89094c44da98b954eedeac495271d0f',  # noqa: E501
                         'function_abi': function_abi,
                         'function_parameters': [
                             '0x5d3a536e4d6dbd6114cc1ead35777bab948e3643'
                         ],
                         'trace_type': ['trace'],
                     },
                 ],
@@ -230,30 +230,30 @@
             },
         ),
         #     (
         #         'trace_filter',
         #         ctc.rpc.construct_trace_filter,
         #         [],
         #         {
-        #             'to_addresses': ['0x6b175474e89094c44da98b954eedeac495271d0f'],
+        #             'to_addresses': ['0x6b175474e89094c44da98b954eedeac495271d0f'],  # noqa: E501
         #             'start_block': 10_000_000,
         #             'end_block': 10_000_001,
         #             'count': 10,
         #         }
         #     ),
         #     (
         #         'trace_get',
         #         ctc.rpc.construct_trace_get,
         #         [],
         #         {}
         #     ),
         #     (
         #         'trace_raw_transaction',
         #         ctc.rpc.construct_trace_raw_transaction,
-        #         ['0xd01212e8ab48d2fd2ea9c4f33f8670fd1cf0cfb09d2e3c6ceddfaf54152386e5'],
+        #         ['0xd01212e8ab48d2fd2ea9c4f33f8670fd1cf0cfb09d2e3c6ceddfaf54152386e5'],  # noqa: E501
         #         {'trace_type': ['trace']},
         #     ),
         (
             'trace_replay_block_transactions',
             ctc.rpc.construct_trace_replay_block_transactions,
             [],
             {
@@ -261,20 +261,20 @@
                 'trace_type': ['trace'],
             },
         ),
         (
             'trace_replay_transaction',
             ctc.rpc.construct_trace_replay_transaction,
             [
-                '0xd01212e8ab48d2fd2ea9c4f33f8670fd1cf0cfb09d2e3c6ceddfaf54152386e5'
+                '0xd01212e8ab48d2fd2ea9c4f33f8670fd1cf0cfb09d2e3c6ceddfaf54152386e5'  # noqa: E501
             ],
             {'trace_type': ['trace']},
         ),
         (
             'trace_transaction',
             ctc.rpc.construct_trace_transaction,
             [
-                '0xd01212e8ab48d2fd2ea9c4f33f8670fd1cf0cfb09d2e3c6ceddfaf54152386e5'
+                '0xd01212e8ab48d2fd2ea9c4f33f8670fd1cf0cfb09d2e3c6ceddfaf54152386e5'  # noqa: E501
             ],
             {},
         ),
     ]
```

### Comparing `paradigm-flood-0.2.1/flood/tests/load_tests/load_test_construction.py` & `paradigm-flood-0.2.2/flood/tests/load_tests/load_test_construction.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/tests/load_tests/load_test_plots.py` & `paradigm-flood-0.2.2/flood/tests/load_tests/load_test_plots.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/tests/load_tests/load_test_reports.py` & `paradigm-flood-0.2.2/flood/tests/load_tests/load_test_reports.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 _header_template = """# `flood` Load Test Report
 
 
 {toc}
 
 ### Report Generation
 
-*This report was generated by `flood`. See the `flood report --help` command for report generation options. This report can be executed as a Python notebook using the `.ipynb` version of this file.*"""
+*This report was generated by `flood`. See the `flood report --help` command for report generation options. This report can be executed as a Python notebook using the `.ipynb` version of this file.*"""  # noqa: E501
 
 
 _toc_template = """### Contents
 1. [Test Summary](#Test-Summary)
 2. [Tests](#Tests)
 {toc_lines}"""
 
@@ -197,15 +197,15 @@
                 for test_name, test_path in test_paths.items()
             }}
 
             results_payloads = {{
                 test_name: flood.load_single_run_results_payload(output_dir=test_path)
                 for test_name, test_path in test_paths.items()
             }}
-        """,
+        """,  # noqa: E501
         'inputs': [],
     },
     {
         # Test summary header
         'type': 'markdown',
         'content': '# Test Summary',
         'inputs': [],
@@ -249,15 +249,15 @@
             toolstr.print_text_box('Total time per test')
             rows = list(time_per_test.items())
             toolstr.print_table(rows, labels=['test', 'time (s)'])
 
             toolstr.print_text_box('Total time per condition')
             rows = list(time_per_condition.items())
             toolstr.print_table(rows, labels=['condition', 'time (s)'])
-        """,
+        """,  # noqa: E501
         'inputs': [],
     },
     {
         # Tests header
         'type': 'markdown',
         'content': '# Tests',
         'inputs': [],
@@ -344,15 +344,15 @@
                     error for error_list in results[name]['errors'] for error in error_list
                 }}
                 print(name)
                 for error in unique_errors[name]:
                     print('-', error)
                 if n != len(results) - 1:
                     print()
-        """,
+        """,  # noqa: E501
         'inputs': [],
     },
     {
         # show complete results
         'type': 'code',
         'content': """
             # show complete results
```

### Comparing `paradigm-flood-0.2.1/flood/tests/load_tests/load_test_runs.py` & `paradigm-flood-0.2.2/flood/tests/load_tests/load_test_runs.py`

 * *Files 3% similar despite different names*

```diff
@@ -226,15 +226,15 @@
         )
         results.append(result)
         if verbose >= 2:
             print()
 
     # format output
     keys = results[0].keys()
-    return {key: [result[key] for result in results] for key in keys}  # type: ignore
+    return {key: [result[key] for result in results] for key in keys}  # type: ignore # noqa: E501
 
 
 def _run_load_test_remotely(
     *,
     node: spec.Node,
     test: spec.LoadTest,
     verbose: bool | int = False,
@@ -305,15 +305,16 @@
             toolstr.add_style('\[', flood.styles['content'])
             + toolstr.add_style(str(dt), flood.styles['metavar'])
             + toolstr.add_style(']', flood.styles['content'])
         )
         toolstr.print(
             timestamp + ' ' + node_name + ' Executing test on remote node'
         )
-    cmd = "ssh {host} bash -c 'source ~/.profile; python3 -m flood {test} {name}={url} --output {output} --no-figures'".format(
+    cmd_template = "ssh {host} bash -c 'source ~/.profile; python3 -m flood {test} {name}={url} --output {output} --no-figures'" # noqa: E501
+    cmd = cmd_template.format(
         host=remote,
         name=node['name'],
         url=node['url'],
         test=tempdir,
         output=tempdir,
     )
     subprocess.check_output(cmd.split(' '), stderr=subprocess.DEVNULL)
```

### Comparing `paradigm-flood-0.2.1/flood/tests/load_tests/vegeta.py` & `paradigm-flood-0.2.2/flood/tests/load_tests/vegeta.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/tests/runner.py` & `paradigm-flood-0.2.2/flood/tests/runner.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/user_io/file_io.py` & `paradigm-flood-0.2.2/flood/user_io/file_io.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/user_io/inputs.py` & `paradigm-flood-0.2.2/flood/user_io/inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     prefixes = ['http', 'https', 'ws', 'wss']
 
     if isinstance(node, dict):
         return node
     elif isinstance(node, str):
         # parse name
         if '=' in node:
-            name, url = node.split('=')
+            name, url = node.split('=', 1)
         else:
             name = node
             url = node
 
         # check if node is in ctc aliases
         alias_url = get_ctc_alias_url(url)
         if alias_url is not None:
@@ -164,15 +164,15 @@
         else:
             import json
             import subprocess
 
             cmd = [
                 """ssh""",
                 remote,
-                """curl -X POST -H 'Content-Type: application/json' -d '{\"jsonrpc\": \"2.0\", \"method\": \"web3_clientVersion\", \"params\": [], \"id\": 1}' """
+                """curl -X POST -H 'Content-Type: application/json' -d '{\"jsonrpc\": \"2.0\", \"method\": \"web3_clientVersion\", \"params\": [], \"id\": 1}' """  # noqa: E501
                 + url,
             ]
             output = subprocess.check_output(cmd, stderr=subprocess.DEVNULL)
             response = json.loads(output)
             info = response['result']
             return info
     except Exception:
```

### Comparing `paradigm-flood-0.2.1/flood/user_io/notebook_io.py` & `paradigm-flood-0.2.2/flood/user_io/notebook_io.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/flood/user_io/outputs.py` & `paradigm-flood-0.2.2/flood/user_io/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 
 def _get_tqdm() -> types.ModuleType:
     import sys
 
     if 'jupyter_client' in sys.modules:
         try:
-            import ipywidgets  # type: ignore
+            import ipywidgets  # type: ignore # noqa: F401
             import tqdm.notebook as tqdm
 
             return tqdm
         except ImportError:
             pass
 
     import tqdm  # type: ignore
```

### Comparing `paradigm-flood-0.2.1/pyproject.toml` & `paradigm-flood-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Typing :: Typed",
 ]
 dependencies = [
     'typing-extensions >=4.2.0, <5',
     'toolcli >=0.6.14, <0.7',
-    'toolstr >=0.9.5, <0.10',
+    'toolstr >=0.9.6, <0.10',
     'requests >=2.20.0, <3',
     'tqdm >=4.65.0, <5',
     'numpy >=1.19.0, <1.25',
     'nbformat >= 5.8.0, <6',
     'toolplot >= 0.3.4, <0.4',
     'matplotlib >= 3.7.1, <4',
     'paradigm-data-portal >= 0.2.2, <0.3',
@@ -68,7 +68,11 @@
 asyncio_mode = 'auto'
 
 [tool.black]
 line-length = 80
 skip-string-normalization = true
 target-version = ['py37']
 
+[tool.ruff]
+line-length = 80
+ignore = ["F403"]
+
```

### Comparing `paradigm-flood-0.2.1/tests/test_env_vars.py` & `paradigm-flood-0.2.2/tests/test_env_vars.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/tests/test_load_tests.py` & `paradigm-flood-0.2.2/tests/test_load_tests.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import pytest
 
 import flood
 
 
 cmd_templates = {
-    'local_bare': 'flood {test_name} {local_node_1} {local_node_2} -d 1 -r 1 2 4',
-    # 'local_alias': 'flood {test_name} node1={local_node_1} node2={local_node_2} -d 1 -r 1 2 4',
-    'remote_bare': 'flood {test_name} {remote_node_1} {remote_node_2} -d 1 -r 20 40 60',
-    # 'remote_alias': 'flood {test_name} node1={remote_node_1} node2={remote_node_2} -d 1 -r 1 2 4',
+    'local_bare': 'flood {test_name} {local_node_1} {local_node_2} -d 1 -r 1 2 4',  # noqa: E501
+    # 'local_alias': 'flood {test_name} node1={local_node_1} node2={local_node_2} -d 1 -r 1 2 4',  # noqa: E501
+    'remote_bare': 'flood {test_name} {remote_node_1} {remote_node_2} -d 1 -r 20 40 60',  # noqa: E501
+    # 'remote_alias': 'flood {test_name} node1={remote_node_1} node2={remote_node_2} -d 1 -r 1 2 4',  # noqa: E501
 }
 
 
 @pytest.mark.parametrize('test_name', flood.get_single_test_generators().keys())
 @pytest.mark.parametrize('cmd_template', cmd_templates.keys())
 def test_load_test(
     test_name,
```

### Comparing `paradigm-flood-0.2.1/tests/test_node_parsing.py` & `paradigm-flood-0.2.2/tests/test_node_parsing.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.1/PKG-INFO` & `paradigm-flood-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradigm-flood
-Version: 0.2.1
+Version: 0.2.2
 Summary: tool for benchmarking RPC endpoints
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: typing-extensions >=4.2.0, <5
 Requires-Dist: toolcli >=0.6.14, <0.7
-Requires-Dist: toolstr >=0.9.5, <0.10
+Requires-Dist: toolstr >=0.9.6, <0.10
 Requires-Dist: requests >=2.20.0, <3
 Requires-Dist: tqdm >=4.65.0, <5
 Requires-Dist: numpy >=1.19.0, <1.25
 Requires-Dist: nbformat >= 5.8.0, <6
 Requires-Dist: toolplot >= 0.3.4, <0.4
 Requires-Dist: matplotlib >= 3.7.1, <4
 Requires-Dist: paradigm-data-portal >= 0.2.2, <0.3
@@ -34,17 +34,26 @@
 Requires-Dist: mypy ==1.2.0 ; extra == "test"
 Requires-Dist: mypy_extensions >= 1.0.0, <1.1.0 ; extra == "test"
 Requires-Dist: pytest >=6, <7 ; extra == "test"
 Requires-Dist: types-tqdm >= 4.65.0.1, <5 ; extra == "test"
 Provides-Extra: test
 
 
-# 🌊🌊 flood 🌊🌊
+# <h1 align="center"> 🌊🌊 flood 🌊🌊 </h1>
 
-`flood` is a load testing tool for benchmarking EVM nodes over RPC
+**`flood` is a load testing tool for benchmarking EVM nodes over RPC**
+
+![](./assets/cover.png)
+
+[![CI status](https://github.com/paradigmxyz/flood/workflows/Pytest/badge.svg)][gh-ci]
+[![Telegram Chat][tg-badge]][tg-url]
+
+[gh-ci]: https://github.com/paradigmxyz/flood/actions/workflows/ci.yml
+[tg-badge]: https://img.shields.io/endpoint?color=neon&logo=telegram&label=chat&url=https%3A%2F%2Ftg.sumanjay.workers.dev%2Fparadigm%5Fflood
+[tg-url]: https://t.me/paradigm_flood
 
 For each RPC method, `flood` measures how load affects metrics such as:
 1. throughput
 2. latency (mean, P50, P90, P95, P99, max)
 3. error rate
 
 `flood` makes it easy to compare the performance of:
```

