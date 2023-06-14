# Comparing `tmp/pysamosa-0.2.12.tar.gz` & `tmp/pysamosa-0.2.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysamosa-0.2.12.tar", last modified: Tue Jun 13 05:09:42 2023, max compression
+gzip compressed data, was "pysamosa-0.2.13.tar", last modified: Wed Jun 14 23:07:28 2023, max compression
```

## Comparing `pysamosa-0.2.12.tar` & `pysamosa-0.2.13.tar`

### file list

```diff
@@ -1,83 +1,79 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-13 05:09:42.584864 pysamosa-0.2.12/
--rw-rw-r--   0 travis    (2000) travis    (2000)      214 2023-06-13 05:03:34.000000 pysamosa-0.2.12/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3525 2023-06-13 05:03:34.000000 pysamosa-0.2.12/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       89 2023-06-13 05:03:34.000000 pysamosa-0.2.12/HISTORY.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1829 2023-06-13 05:03:34.000000 pysamosa-0.2.12/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      306 2023-06-13 05:03:34.000000 pysamosa-0.2.12/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    13570 2023-06-13 05:09:42.584864 pysamosa-0.2.12/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    12366 2023-06-13 05:03:34.000000 pysamosa-0.2.12/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-13 05:09:42.540860 pysamosa-0.2.12/notebooks/
--rw-rw-r--   0 travis    (2000) travis    (2000)   423031 2023-06-13 05:03:34.000000 pysamosa-0.2.12/notebooks/retracking_example.ipynb
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-13 05:09:42.560862 pysamosa-0.2.12/pysamosa/
--rw-rw-r--   0 travis    (2000) travis    (2000)      184 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      387 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12897 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/common_types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      334 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/conf_params.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26149 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/data_access.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3162 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/dist2coast.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      463 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/download_aux_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5205 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/l1b_simulator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3086 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/leading_edge_detector.py
--rw-rw-r--   0 travis    (2000) travis    (2000)  9928947 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/luts_samosa.pickle
--rw-rw-r--   0 travis    (2000) travis    (2000)     6199 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/main_coastalffsar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6399 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/main_coral_paper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2002 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/main_cs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1709 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/main_s3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1914 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/main_s6.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2868 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/main_s6jtex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3128 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/main_s6jtex_raw_vs_rmc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18453 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1612 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/model_helpers.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)     7278 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/montecarlo_simulator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/pysamosa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1622 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/qual_flag_estimator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25442 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/retracker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12295 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/retracker_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21157 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/retracker_processor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6888 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/rip.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      233 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/settings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5900 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/settings_manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1684 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/simple_logger.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9196 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-13 05:09:42.564862 pysamosa-0.2.12/pysamosa.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13570 2023-06-13 05:09:42.000000 pysamosa-0.2.12/pysamosa.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1912 2023-06-13 05:09:42.000000 pysamosa-0.2.12/pysamosa.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-13 05:09:42.000000 pysamosa-0.2.12/pysamosa.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-13 05:09:42.000000 pysamosa-0.2.12/pysamosa.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2023-06-13 05:09:42.000000 pysamosa-0.2.12/pysamosa.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2023-06-13 05:09:42.000000 pysamosa-0.2.12/pysamosa.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      284 2023-06-13 05:03:34.000000 pysamosa-0.2.12/requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-13 05:09:42.564862 pysamosa-0.2.12/scripts/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1670 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/cs_l2_conversion.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-13 05:09:42.580864 pysamosa-0.2.12/scripts/luts/
--rw-rw-r--   0 travis    (2000) travis    (2000)   217134 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/luts/AUX_RLUT_S6A_002.nc
--rw-rw-r--   0 travis    (2000) travis    (2000)   214215 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/luts/AUX_RLUT_S6A_003.nc
--rwxrwxr-x   0 travis    (2000) travis    (2000)  4818008 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/luts/F0.txt
--rwxrwxr-x   0 travis    (2000) travis    (2000)  4827430 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/luts/F1.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    30520 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/luts/LUT_Alpha_P_CS-2.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)   993604 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/luts/S6A_TEST_AUX_FLUT___00000000T000000_99999999T999999_0001.NC
--rw-rw-r--   0 travis    (2000) travis    (2000)    30520 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/luts/alphap_table_SEN3_09_Nov_2017.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3215 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/luts/convert_luts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9703 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/thesis_plots.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6110 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/track_browser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9809 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/track_browser_footprint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      437 2023-06-13 05:09:42.584864 pysamosa-0.2.12/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2400 2023-06-13 05:03:34.000000 pysamosa-0.2.12/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-13 05:09:42.584864 pysamosa-0.2.12/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10801 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2432 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/settings_dumper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_common_types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3314 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_dist2coast.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5903 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_dynamic_fg_epoch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5007 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_l1b_sim_retracker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2235 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_l1b_simulator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1897 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_leading_edge_detector.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9238 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9916 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_montecarlo_sim.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8931 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_retrack_multi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9651 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_retrack_single.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4892 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_samplusplus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1110 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 23:07:28.264827 pysamosa-0.2.13/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1829 2023-06-14 23:00:41.000000 pysamosa-0.2.13/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      306 2023-06-14 23:00:41.000000 pysamosa-0.2.13/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13837 2023-06-14 23:07:28.264827 pysamosa-0.2.13/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12659 2023-06-14 23:00:41.000000 pysamosa-0.2.13/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 23:07:28.216824 pysamosa-0.2.13/notebooks/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   423031 2023-06-14 23:00:41.000000 pysamosa-0.2.13/notebooks/retracking_example.ipynb
+-rw-rw-r--   0 travis    (2000) travis    (2000)      132 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 23:07:28.240826 pysamosa-0.2.13/pysamosa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      184 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12896 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/common_types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      334 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/conf_params.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26159 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/data_access.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3162 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/dist2coast.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      462 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/download_aux_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5188 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/l1b_simulator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3086 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/leading_edge_detector.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)  9928947 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/luts_samosa.pickle
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6199 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/main_coastalffsar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6399 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/main_coral_paper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2001 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/main_cs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1708 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/main_s3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1913 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/main_s6.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2869 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/main_s6jtex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3128 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/main_s6jtex_raw_vs_rmc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18453 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1614 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/model_helpers.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7278 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/montecarlo_simulator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/pysamosa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1622 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/qual_flag_estimator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25417 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/retracker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12275 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/retracker_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21157 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/retracker_processor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6887 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/rip.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      232 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/settings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5900 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/settings_manager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1684 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/simple_logger.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9195 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       48 2023-06-14 23:00:41.000000 pysamosa-0.2.13/pysamosa/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 23:07:28.244826 pysamosa-0.2.13/pysamosa.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13837 2023-06-14 23:07:28.000000 pysamosa-0.2.13/pysamosa.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1855 2023-06-14 23:07:28.000000 pysamosa-0.2.13/pysamosa.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-14 23:07:28.000000 pysamosa-0.2.13/pysamosa.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-14 23:07:28.000000 pysamosa-0.2.13/pysamosa.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      165 2023-06-14 23:07:28.000000 pysamosa-0.2.13/pysamosa.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2023-06-14 23:07:28.000000 pysamosa-0.2.13/pysamosa.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      308 2023-06-14 23:00:41.000000 pysamosa-0.2.13/requirements.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 23:07:28.244826 pysamosa-0.2.13/scripts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1671 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/cs_l2_conversion.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 23:07:28.260827 pysamosa-0.2.13/scripts/luts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   217134 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/luts/AUX_RLUT_S6A_002.nc
+-rw-rw-r--   0 travis    (2000) travis    (2000)   214215 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/luts/AUX_RLUT_S6A_003.nc
+-rwxrwxr-x   0 travis    (2000) travis    (2000)  4818008 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/luts/F0.txt
+-rwxrwxr-x   0 travis    (2000) travis    (2000)  4827430 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/luts/F1.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30520 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/luts/LUT_Alpha_P_CS-2.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)   993604 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/luts/S6A_TEST_AUX_FLUT___00000000T000000_99999999T999999_0001.NC
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30520 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/luts/alphap_table_SEN3_09_Nov_2017.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3215 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/luts/convert_luts.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9704 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/thesis_plots.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6110 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/track_browser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9809 2023-06-14 23:00:41.000000 pysamosa-0.2.13/scripts/track_browser_footprint.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      437 2023-06-14 23:07:28.268828 pysamosa-0.2.13/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2362 2023-06-14 23:00:41.000000 pysamosa-0.2.13/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-14 23:07:28.264827 pysamosa-0.2.13/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10800 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2431 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/settings_dumper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_common_types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3305 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_dist2coast.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5903 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_dynamic_fg_epoch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4987 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_l1b_sim_retracker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2235 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_l1b_simulator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1897 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_leading_edge_detector.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9238 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9915 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_montecarlo_sim.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8931 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_retrack_multi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9630 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_retrack_single.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4892 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_samplusplus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1111 2023-06-14 23:00:41.000000 pysamosa-0.2.13/tests/test_utils.py
```

### Comparing `pysamosa-0.2.12/LICENSE` & `pysamosa-0.2.13/LICENSE`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.12/PKG-INFO` & `pysamosa-0.2.13/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysamosa
-Version: 0.2.12
+Version: 0.2.13
 Summary: PySAMOSA is a software framework for processing open ocean and coastal waveforms from SAR satellite altimetry to measure sea surface heights, wave heights, and wind speed for the oceans and inland water bodies. Satellite altimetry is a space-borne remote sensing technique used for Earth observation.
 Home-page: https://github.com/floschl/pysamosa
 Author: Florian Schlembach
 Author-email: florian.schlembach@tum.de
 License: GNU General Public License v3
 Keywords: satellite altimetry retracking samosa+ samosa coastal open ocean sentinel esasar altimetry ff-sar fully focused
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: AUTHORS.rst
 
 [//]: # (![pysamosa logo]&#40;./resources/logo.jpg&#41;)
 
 ![]() <div align="center"><img src="https://github.com/floschl/pysamosa/blob/main/resources/logo_name.png?raw=true"
 width="500"></div>
 
 [![Build Status](https://app.travis-ci.com/floschl/pysamosa.svg?branch=main)](https://app.travis-ci.com/floschl/pysamosa)
@@ -144,15 +143,15 @@
 
 or via pyenv/pipenv/venv.
 
 Activate pysamosa conda environment
 
     $ conda activate pysamosa
 
-Install dependencies
+Install dependencies into your conda env/virtualenv
 
     $ pip install -r requirements.txt
 
 Compile the .pyx files (e.g. model_helpers.pyx) by running cython to build the extensions
 For Windows users: An installed C/C++ compiler may be required for installation, e.g. MSCV, which comes with
 the free [Visual Studio Community](https://visualstudio.microsoft.com/vs/community/)
 
@@ -227,14 +226,23 @@
 ## Contributions
 
 This software is intended to be a community-based project. Contributions to this project are very welcome.
 In this case:
 - Fork this repository
 - Submit a pull request to be merged back into this repository.
 
+Before submitting changes, please check that your changes pass flake8, black, isort and the
+   tests, including testing other Python versions with tox:
+
+    $ flake8 pysamosa tests scripts
+    $ black . --check --diff
+    $ isort . --check-only --diff
+    $ pytest
+    $ tox
+
 If your pull request is accepted, you will be included in the next official release and will be listed as a
 co-author for the DOI link created by Zenodo.
 
 ## Future work
 
 Possible developments of this project are:
 
@@ -243,22 +251,22 @@
 [SAMpy](https://github.com/cls-obsnadir-dev/SAMPy) developed as part of the [ESA Cryo-TEMPO project](https://earth.esa.int/eogateway/documents/20142/37627/Cryo-TEMPO-ATBD-Coastal-Oceans.pdf)
 - Implement numerical retracking planned for Q3/2023 in the EUMETSAT's baseline processing chain [6]
 
 Software-related
 - Create notebook for a coastal retracking demo
 - Create richer documentation (readthedocs)
 
-## Credits and code reuse
+## Credits
 
 If you use this code, please cite this DOI:
 
 Florian Schlembach; Marcello Passaro. PySAMOSA: An Open-source Software Framework for Retracking SAMOSA-based, Open
 Ocean and Coastal Waveforms of SAR Satellite Altimetry. Zenodo. https://zenodo.org/badge/latestdoi/646028227.
 
-Salvatore Dinardo for his support in implementing the SAMOSA-based and SAMOSA+ [3] retracking algorithm.
+Salvatore Dinardo for his support in implementing the SAMOSA-based and SAMOSA+ [3] retracking algorithms.
 
 This software is licenced under [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html). In short, you are allowed to use
 this software in your projects, if you change parts of the code you are required to also publish it. For more
 frequently asked questions about GPL, please see [here](https://www.gnu.org/licenses/gpl-faq.html).
 
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage) project template.
```

### Comparing `pysamosa-0.2.12/README.md` & `pysamosa-0.2.13/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
 or via pyenv/pipenv/venv.
 
 Activate pysamosa conda environment
 
     $ conda activate pysamosa
 
-Install dependencies
+Install dependencies into your conda env/virtualenv
 
     $ pip install -r requirements.txt
 
 Compile the .pyx files (e.g. model_helpers.pyx) by running cython to build the extensions
 For Windows users: An installed C/C++ compiler may be required for installation, e.g. MSCV, which comes with
 the free [Visual Studio Community](https://visualstudio.microsoft.com/vs/community/)
 
@@ -204,14 +204,23 @@
 ## Contributions
 
 This software is intended to be a community-based project. Contributions to this project are very welcome.
 In this case:
 - Fork this repository
 - Submit a pull request to be merged back into this repository.
 
+Before submitting changes, please check that your changes pass flake8, black, isort and the
+   tests, including testing other Python versions with tox:
+
+    $ flake8 pysamosa tests scripts
+    $ black . --check --diff
+    $ isort . --check-only --diff
+    $ pytest
+    $ tox
+
 If your pull request is accepted, you will be included in the next official release and will be listed as a
 co-author for the DOI link created by Zenodo.
 
 ## Future work
 
 Possible developments of this project are:
 
@@ -220,22 +229,22 @@
 [SAMpy](https://github.com/cls-obsnadir-dev/SAMPy) developed as part of the [ESA Cryo-TEMPO project](https://earth.esa.int/eogateway/documents/20142/37627/Cryo-TEMPO-ATBD-Coastal-Oceans.pdf)
 - Implement numerical retracking planned for Q3/2023 in the EUMETSAT's baseline processing chain [6]
 
 Software-related
 - Create notebook for a coastal retracking demo
 - Create richer documentation (readthedocs)
 
-## Credits and code reuse
+## Credits
 
 If you use this code, please cite this DOI:
 
 Florian Schlembach; Marcello Passaro. PySAMOSA: An Open-source Software Framework for Retracking SAMOSA-based, Open
 Ocean and Coastal Waveforms of SAR Satellite Altimetry. Zenodo. https://zenodo.org/badge/latestdoi/646028227.
 
-Salvatore Dinardo for his support in implementing the SAMOSA-based and SAMOSA+ [3] retracking algorithm.
+Salvatore Dinardo for his support in implementing the SAMOSA-based and SAMOSA+ [3] retracking algorithms.
 
 This software is licenced under [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html). In short, you are allowed to use
 this software in your projects, if you change parts of the code you are required to also publish it. For more
 frequently asked questions about GPL, please see [here](https://www.gnu.org/licenses/gpl-faq.html).
 
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage) project template.
```

### Comparing `pysamosa-0.2.12/notebooks/retracking_example.ipynb` & `pysamosa-0.2.13/notebooks/retracking_example.ipynb`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.12/pysamosa/common_types.py` & `pysamosa-0.2.13/pysamosa/common_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import logging
 from enum import Enum
 from pathlib import Path
+from typing import Optional
 
 import numpy as np
 from pydantic import BaseModel, root_validator, validator
 
-from typing import Optional
-
 
 class SensorType(Enum):
     S3 = "s3"
     CS = "cs"
     S6_F04 = "s6_f04"
     S6_F06 = "s6_f06"
     S6_F04_FF = "s6_f04_ff"
```

### Comparing `pysamosa-0.2.12/pysamosa/data_access.py` & `pysamosa-0.2.13/pysamosa/data_access.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
+import os
 import tempfile
+from datetime import datetime
 from pathlib import Path
-import os
 
 import numpy as np
-import xarray as xr
 import pandas as pd
-from datetime import datetime
+import xarray as xr
+
 from pysamosa.dist2coast import get_dist_pacioos
 
 from .common_types import ModelParameter
 from .conf_params import CONST_C
 
-
 data_vars_s3 = {
     "l1b": {
         "wf": "i2q2_meas_ku_l1b_echo_sar_ku",
         "time": "time_l1b_echo_sar_ku",
         "lat_rad": "lat_l1b_echo_sar_ku",
         "lon_rad": "lon_l1b_echo_sar_ku",
         "alt_m": "alt_l1b_echo_sar_ku",
@@ -278,15 +278,15 @@
     n_inds=0,
     do_interp_dist2coast=False,
     group=None,
 ):
     # hack required because some nc files have issues with decoding of times
     try:
         ds = xr.open_dataset(nc_filename, group=group)
-    except:
+    except Exception:
         ds = xr.open_dataset(nc_filename, group=group, decode_times=False)
 
     last_ind = get_last_ind(
         n_offset=n_offset,
         n_inds=n_inds,
         n_total_length=ds[data_var_names["time"]].shape[0],
     )
```

### Comparing `pysamosa-0.2.12/pysamosa/dist2coast.py` & `pysamosa-0.2.13/pysamosa/dist2coast.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.12/pysamosa/l1b_simulator.py` & `pysamosa-0.2.13/pysamosa/l1b_simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import numpy as np
 from numpy.random import default_rng
 
 from pysamosa import simple_logger
-from pysamosa.common_types import (
-    ModelSettings,
-    SensorSettings,
-    RetrackerBaseType,
-)
+from pysamosa.common_types import ModelSettings, RetrackerBaseType, SensorSettings
 from pysamosa.conf_params import CONST_C
 from pysamosa.data_access import get_model_param_obj_from_l1b_data
 from pysamosa.model import SamosaModel
 
 # fixed values taken from ind 42660, file
 # RES_S3A_SR_1_SRA_A__20200108T101712_20200108T110742_20200202T201001_3029_053_279_GPOD_SAR_O_NT_003
 l1b_data_single_template = {
```

### Comparing `pysamosa-0.2.12/pysamosa/leading_edge_detector.py` & `pysamosa-0.2.13/pysamosa/leading_edge_detector.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.12/pysamosa/luts_samosa.pickle` & `pysamosa-0.2.13/pysamosa/luts_samosa.pickle`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.12/pysamosa/main_coastalffsar.py` & `pysamosa-0.2.13/pysamosa/main_coastalffsar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import numpy as np
-from datetime import datetime
 import logging
-from pathlib import Path
 import re
+from datetime import datetime
+from pathlib import Path
+
+import numpy as np
 import pandas as pd
 
-from pysamosa.common_types import RetrackerBaseType, L1bSourceType, ProcMode
+from pysamosa import simple_logger
+from pysamosa.common_types import L1bSourceType, ProcMode, RetrackerBaseType
 from pysamosa.data_access import data_vars_dart
 from pysamosa.retracker_processor import RetrackerProcessor
-from pysamosa.settings_manager import get_default_base_settings, SettingsPreset
-
-from pysamosa import simple_logger
+from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
 
 simple_logger.set_root_logger(log_level=logging.INFO)
 
 
 def convert_dt(dt_str):
     return np.datetime64(datetime.strptime(dt_str, "%Y%m%dT%H%M%S"))
```

### Comparing `pysamosa-0.2.12/pysamosa/main_coral_paper.py` & `pysamosa-0.2.13/pysamosa/main_coral_paper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 import os
 import re
 from pathlib import Path
 from sys import platform
 
-from pysamosa.common_types import RetrackerBaseType, L1bSourceType
+from pysamosa.common_types import L1bSourceType, RetrackerBaseType
 from pysamosa.data_access import data_vars_s3
 from pysamosa.retracker_processor import RetrackerProcessor
-from pysamosa.settings_manager import get_default_base_settings, SettingsPreset
+from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
 
 is_linux = "linux" in platform
 is_slurm = "SLURM_JOB_ID" in os.environ
 slurm_abs_procid, slurm_n_total_processes = None, None
 if is_slurm:
     if "SLURM_ARRAY_TASK_COUNT" in os.environ:
         slurm_n_array_jobs = int(os.environ["SLURM_ARRAY_TASK_COUNT"])
```

### Comparing `pysamosa-0.2.12/pysamosa/main_cs.py` & `pysamosa-0.2.13/pysamosa/main_cs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 from pathlib import Path
 
-from pysamosa.common_types import RetrackerBaseType, L1bSourceType
+from pysamosa.common_types import L1bSourceType, RetrackerBaseType
 from pysamosa.data_access import data_vars_cs
 from pysamosa.retracker_processor import RetrackerProcessor
-from pysamosa.settings_manager import get_default_base_settings, SettingsPreset
-
+from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
 
 if __name__ == "__main__":
     nc_src_base_path = Path(
         "/nfs/DGFI145/C/work_flo/cs2_files_samplus_test/CS2_open_ocean/"
     )
     nc_dest_path = Path("/nfs/DGFI145/C/work_flo/cs2_files_samplus_test/")
     run_name = "samplus_cs_test"
```

### Comparing `pysamosa-0.2.12/pysamosa/main_s3.py` & `pysamosa-0.2.13/pysamosa/main_s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 
-from pysamosa.common_types import RetrackerBaseType, L1bSourceType
+from pysamosa.common_types import L1bSourceType, RetrackerBaseType
 from pysamosa.data_access import data_vars_s3
 from pysamosa.retracker_processor import RetrackerProcessor
-from pysamosa.settings_manager import get_default_base_settings, SettingsPreset
 from pysamosa.settings import TEST_DATA_DIR
-
+from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
 
 if __name__ == "__main__":
     nc_src_base_path = TEST_DATA_DIR / "s3" / "l1b"
     run_name = "s3_retrack_open_ocean"
     nc_dest_path = nc_src_base_path.parent
 
     # select files
```

### Comparing `pysamosa-0.2.12/pysamosa/main_s6.py` & `pysamosa-0.2.13/pysamosa/main_s6.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 from pathlib import Path
 
-from pysamosa.common_types import RetrackerBaseType, L1bSourceType
+from pysamosa.common_types import L1bSourceType, RetrackerBaseType
 from pysamosa.data_access import data_vars_s6
 from pysamosa.retracker_processor import RetrackerProcessor
-from pysamosa.settings_manager import get_default_base_settings, SettingsPreset
-
+from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
 
 if __name__ == "__main__":
     nc_src_base_path = Path(
         "/nfs/DGFI145/A/original_data/sentinel6a/JASON_CS_S6A_L1B_ALT_HR_NTC_F_V2/"
     )
     # nc_dest_path = Path('/nfs/DGFI145/C/work_flo/s6jtex_coral/')
     run_name = "coral_retrack"
```

### Comparing `pysamosa-0.2.12/pysamosa/main_s6jtex.py` & `pysamosa-0.2.13/pysamosa/main_s6jtex.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
-from pathlib import Path
 import re
 from datetime import datetime
+from pathlib import Path
+
 import numpy as np
 import pandas as pd
 
-from pysamosa.common_types import RetrackerBaseType, L1bSourceType
+from pysamosa.common_types import L1bSourceType, RetrackerBaseType
 from pysamosa.data_access import data_vars_s6
 from pysamosa.retracker_processor import RetrackerProcessor
-from pysamosa.settings_manager import get_default_base_settings, SettingsPreset
+from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
 
 
 def convert_dt(dt_str):
     return np.datetime64(datetime.strptime(dt_str, "%Y%m%dT%H%M%S"))
 
 
 if __name__ == "__main__":
```

### Comparing `pysamosa-0.2.12/pysamosa/main_s6jtex_raw_vs_rmc.py` & `pysamosa-0.2.13/pysamosa/main_s6jtex_raw_vs_rmc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
-from pathlib import Path
 import re
+from pathlib import Path
+
 import pandas as pd
 
-from pysamosa.common_types import RetrackerBaseType, L1bSourceType
+from pysamosa.common_types import L1bSourceType, RetrackerBaseType
 from pysamosa.data_access import data_vars_s6
 from pysamosa.retracker_processor import RetrackerProcessor
-from pysamosa.settings_manager import get_default_base_settings, SettingsPreset
-
+from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
 
 if __name__ == "__main__":
     nc_dest_path = Path("/lfs/DGFI24/bigdata/s6jtex_raw2rmc/retracked/")
 
     run_name_basepath = [
         ("coral_raw", Path("/lfs/DGFI24/bigdata/s6jtex_raw2rmc/HR_RAW/1B/")),
         ("coral_rmc", Path("/lfs/DGFI24/bigdata/s6jtex_raw2rmc/HR_RMC/1B/")),
```

### Comparing `pysamosa-0.2.12/pysamosa/model.py` & `pysamosa-0.2.13/pysamosa/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from bisect import bisect_left
 from itertools import chain
 
 import numpy as np
 
 from pysamosa.common_types import (
-    ModelSettings,
     ModelParameter,
+    ModelSettings,
     RetrackerBaseType,
-    WaveformSettings,
     SensorSettings,
+    WaveformSettings,
 )
 from pysamosa.conf_params import CONST_A, CONST_B, CONST_C, CONST_F
-from pysamosa.model_helpers import load_samosa_luts, get_f_from_lut
+from pysamosa.model_helpers import get_f_from_lut, load_samosa_luts
 from pysamosa.rip import RipAnalyser
 
 
 def get_region_max(wf, region_center, n_before_after):
     return np.max(wf[region_center - n_before_after : region_center + n_before_after])
```

### Comparing `pysamosa-0.2.12/pysamosa/model_helpers.pyx` & `pysamosa-0.2.13/pysamosa/model_helpers.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import os
 import pickle
-import numpy as np
+
 import cython
+import numpy as np
 
 
 def load_samosa_luts():
     with open(os.path.dirname(__file__) + f'/luts_samosa.pickle', 'rb') as handle:
         return pickle.load(handle)
 
-from libc.math cimport sqrt, M_PI
+from libc.math cimport M_PI, sqrt
+
 
 @cython.cdivision(True)
 @cython.boundscheck(False)
 cpdef get_f_from_lut(double[:] xi, double[:,:] f_lut, int degree):
     ''' Reads the F0/F1 values from the LUT as described in DPM doc v2.5.2 4.2.3 SL7
 
     :param xi: the value to look up
```

### Comparing `pysamosa-0.2.12/pysamosa/montecarlo_simulator.py` & `pysamosa-0.2.13/pysamosa/montecarlo_simulator.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
 from pysamosa import retracker
 from pysamosa.common_types import (
+    SENSOR_SETS_DEFAULT_S3,
+    FittingSettings,
     ModelSettings,
     RetrackerBaseType,
     RetrackerSettings,
-    FittingSettings,
     WaveformSettings,
-    SENSOR_SETS_DEFAULT_S3,
 )
 from pysamosa.data_access import get_model_param_obj_from_l1b_data
 from pysamosa.l1b_simulator import L1bSimulator
 
 
 class CostFunctionType(Enum):
     RMSE = "rmse"
```

### Comparing `pysamosa-0.2.12/pysamosa/qual_flag_estimator.py` & `pysamosa-0.2.13/pysamosa/qual_flag_estimator.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.12/pysamosa/retracker.py` & `pysamosa-0.2.13/pysamosa/retracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import logging
 
 import numpy as np
 from scipy.interpolate import Akima1DInterpolator
 from scipy.optimize import least_squares
 
 from pysamosa.common_types import (
-    ModelSettings,
+    FittingParameters,
+    FittingSettings,
     ModelParameter,
+    ModelSettings,
+    RetrackerBaseType,
     RetrackerSettings,
-    FittingSettings,
+    SensorSettings,
     WaveformSettings,
-    FittingParameters,
 )
-from pysamosa.common_types import RetrackerBaseType, SensorSettings
 from pysamosa.leading_edge_detector import detect_leading_edge
-from pysamosa.model import SamosaModel, get_region_max, get_region_argmax
+from pysamosa.model import SamosaModel, get_region_argmax, get_region_max
 
 
 def calc_misfit(wf1, wf2, inds_only=None, exclude_inds=None):
     if inds_only is not None and exclude_inds is not None:
         raise RuntimeError("Error calculating misfit. ")
 
     inds_only = np.asarray(inds_only) if inds_only is not None else None
```

### Comparing `pysamosa-0.2.12/pysamosa/retracker_helpers.py` & `pysamosa-0.2.13/pysamosa/retracker_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from collections import deque
-from itertools import islice
 from concurrent import futures
-from itertools import repeat
+from itertools import islice, repeat
+
 import numpy as np
 
+from pysamosa.conf_params import CONST_C
 from pysamosa.data_access import (
     _read_dataset_vars_from_ds,
-    get_subset_dataset,
     get_model_param_obj_from_l1b_data,
+    get_subset_dataset,
 )
 from pysamosa.retracker import SamosaRetracker
-from pysamosa.conf_params import CONST_C
 
 
 def get_tracker_shift_n_samps(
     tracker_range_m: np.ndarray, alt_m: np.ndarray, t0_sampling_gate_ns: float
 ) -> np.ndarray:
     """
     Calulates the number of samples to shift for range-aligning multiple waveforms.
```

### Comparing `pysamosa-0.2.12/pysamosa/retracker_processor.py` & `pysamosa-0.2.13/pysamosa/retracker_processor.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import logging
 import os
 from concurrent import futures
 from itertools import repeat
 
+import netCDF4
 import numpy as np
 import xarray as xr
-import netCDF4
 
 from pysamosa import simple_logger
 from pysamosa.common_types import (
-    RetrackerProcessorSettings,
-    RetrackerSettings,
-    FittingSettings,
-    WaveformSettings,
     ExportSettings,
+    FittingSettings,
     L1bSourceType,
+    RetrackerProcessorSettings,
+    RetrackerSettings,
     SensorSettings,
+    WaveformSettings,
 )
 from pysamosa.conf_params import CONST_C
 from pysamosa.data_access import (
     _read_dataset_vars_from_ds,
-    get_subset_dataset,
+    gen_model_param_obj_from_l1b_data,
+    gen_subset_dataset,
     get_model_param_obj_from_l1b_data,
     get_nc_src_dest_file_list,
-    gen_subset_dataset,
-    gen_model_param_obj_from_l1b_data,
+    get_subset_dataset,
 )
 from pysamosa.retracker import SamosaRetracker
 from pysamosa.retracker_helpers import get_dynamic_first_guess_epochs
 from pysamosa.version import __version__
 
 
 def haversine_np(lat1, lon1, lat2, lon2):
```

### Comparing `pysamosa-0.2.12/pysamosa/rip.py` & `pysamosa-0.2.13/pysamosa/rip.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-import numpy as np
-from scipy.signal import argrelextrema
-from scipy.interpolate import interp1d
-from pydantic import BaseModel
 import copy
 
-from pysamosa.conf_params import CONST_C
-from pysamosa.common_types import ModelParameter, SensorSettings
-
+import numpy as np
 from astropy import modeling
 from astropy.modeling import models
+from pydantic import BaseModel
+from scipy.interpolate import interp1d
+from scipy.signal import argrelextrema
 
+from pysamosa.common_types import ModelParameter, SensorSettings
+from pysamosa.conf_params import CONST_C
 
 # class RipAnalyserSettings(BaseModel):
 #     model_params: ModelParameter
 #     sensor_sets: SensorSettings
 
 
 class RIPParameters(BaseModel):
```

### Comparing `pysamosa-0.2.12/pysamosa/settings_manager.py` & `pysamosa-0.2.13/pysamosa/settings_manager.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from enum import Enum
 
 from pysamosa.common_types import (
-    RetrackerProcessorSettings,
-    RetrackerSettings,
     FittingSettings,
+    L1bSourceType,
     RetrackerBaseType,
-    WaveformSettings,
-    SensorType,
+    RetrackerProcessorSettings,
+    RetrackerSettings,
     SensorSettings,
-    L1bSourceType,
+    SensorType,
+    WaveformSettings,
 )
 
 
 class SettingsPreset(Enum):
     NONE = "none"  # take default preset for RetrackerBaseType
     SAM_FLO = "samflo"
     CORALv1 = "coralv1"
```

### Comparing `pysamosa-0.2.12/pysamosa/simple_logger.py` & `pysamosa-0.2.13/pysamosa/simple_logger.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import os
-import logging
 import datetime
+import logging
+import os
 
 
 class DeltaTimeFormatter(logging.Formatter):
     def format(self, record):
         now = datetime.datetime.now()
         self.last_timestamp = (
             now if "last_timestamp" not in dir(self) else self.last_timestamp
```

### Comparing `pysamosa-0.2.12/pysamosa/utils.py` & `pysamosa-0.2.13/pysamosa/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-import os
-from pathlib import Path
 import logging
-import numpy as np
-from tqdm import tqdm
-import requests
+import os
 import tarfile
+from pathlib import Path
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
+import numpy as np
+import requests
 from matplotlib.backends.backend_pdf import PdfPages
 from matplotlib.backends.backend_pgf import FigureCanvasPgf
-
 from scipy import signal
+from tqdm import tqdm
 
 default_width_in = 5.79  # in inches
 default_ratio = 0.5 + np.sqrt(5) / 2  # 1.618, golden ratio
 default_figsize_in = [default_width_in, default_width_in / default_ratio]
 
 
 def gen_first_true():
```

### Comparing `pysamosa-0.2.12/pysamosa.egg-info/PKG-INFO` & `pysamosa-0.2.13/pysamosa.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysamosa
-Version: 0.2.12
+Version: 0.2.13
 Summary: PySAMOSA is a software framework for processing open ocean and coastal waveforms from SAR satellite altimetry to measure sea surface heights, wave heights, and wind speed for the oceans and inland water bodies. Satellite altimetry is a space-borne remote sensing technique used for Earth observation.
 Home-page: https://github.com/floschl/pysamosa
 Author: Florian Schlembach
 Author-email: florian.schlembach@tum.de
 License: GNU General Public License v3
 Keywords: satellite altimetry retracking samosa+ samosa coastal open ocean sentinel esasar altimetry ff-sar fully focused
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: AUTHORS.rst
 
 [//]: # (![pysamosa logo]&#40;./resources/logo.jpg&#41;)
 
 ![]() <div align="center"><img src="https://github.com/floschl/pysamosa/blob/main/resources/logo_name.png?raw=true"
 width="500"></div>
 
 [![Build Status](https://app.travis-ci.com/floschl/pysamosa.svg?branch=main)](https://app.travis-ci.com/floschl/pysamosa)
@@ -144,15 +143,15 @@
 
 or via pyenv/pipenv/venv.
 
 Activate pysamosa conda environment
 
     $ conda activate pysamosa
 
-Install dependencies
+Install dependencies into your conda env/virtualenv
 
     $ pip install -r requirements.txt
 
 Compile the .pyx files (e.g. model_helpers.pyx) by running cython to build the extensions
 For Windows users: An installed C/C++ compiler may be required for installation, e.g. MSCV, which comes with
 the free [Visual Studio Community](https://visualstudio.microsoft.com/vs/community/)
 
@@ -227,14 +226,23 @@
 ## Contributions
 
 This software is intended to be a community-based project. Contributions to this project are very welcome.
 In this case:
 - Fork this repository
 - Submit a pull request to be merged back into this repository.
 
+Before submitting changes, please check that your changes pass flake8, black, isort and the
+   tests, including testing other Python versions with tox:
+
+    $ flake8 pysamosa tests scripts
+    $ black . --check --diff
+    $ isort . --check-only --diff
+    $ pytest
+    $ tox
+
 If your pull request is accepted, you will be included in the next official release and will be listed as a
 co-author for the DOI link created by Zenodo.
 
 ## Future work
 
 Possible developments of this project are:
 
@@ -243,22 +251,22 @@
 [SAMpy](https://github.com/cls-obsnadir-dev/SAMPy) developed as part of the [ESA Cryo-TEMPO project](https://earth.esa.int/eogateway/documents/20142/37627/Cryo-TEMPO-ATBD-Coastal-Oceans.pdf)
 - Implement numerical retracking planned for Q3/2023 in the EUMETSAT's baseline processing chain [6]
 
 Software-related
 - Create notebook for a coastal retracking demo
 - Create richer documentation (readthedocs)
 
-## Credits and code reuse
+## Credits
 
 If you use this code, please cite this DOI:
 
 Florian Schlembach; Marcello Passaro. PySAMOSA: An Open-source Software Framework for Retracking SAMOSA-based, Open
 Ocean and Coastal Waveforms of SAR Satellite Altimetry. Zenodo. https://zenodo.org/badge/latestdoi/646028227.
 
-Salvatore Dinardo for his support in implementing the SAMOSA-based and SAMOSA+ [3] retracking algorithm.
+Salvatore Dinardo for his support in implementing the SAMOSA-based and SAMOSA+ [3] retracking algorithms.
 
 This software is licenced under [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html). In short, you are allowed to use
 this software in your projects, if you change parts of the code you are required to also publish it. For more
 frequently asked questions about GPL, please see [here](https://www.gnu.org/licenses/gpl-faq.html).
 
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage) project template.
```

### Comparing `pysamosa-0.2.12/pysamosa.egg-info/SOURCES.txt` & `pysamosa-0.2.13/pysamosa.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-AUTHORS.rst
-CONTRIBUTING.rst
-HISTORY.rst
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 notebooks/retracking_example.ipynb
 pysamosa/__init__.py
-pysamosa/cli.py
 pysamosa/common_types.py
 pysamosa/conf_params.py
 pysamosa/data_access.py
 pysamosa/dist2coast.py
 pysamosa/download_aux_data.py
 pysamosa/l1b_simulator.py
 pysamosa/leading_edge_detector.py
```

### Comparing `pysamosa-0.2.12/scripts/cs_l2_conversion.py` & `pysamosa-0.2.13/scripts/cs_l2_conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from pathlib import Path
+
 import numpy as np
 import xarray as xr
-from pathlib import Path
 
 ncfile_l1b = Path(
     "/nfs/DGFI145/C/work_flo/cs2_files_samplus_test/CS2_open_ocean/CS_LTA__SIR_SAR_1B_20150503T160800_20150503T161329_D001.nc"
 )
 ncfile_l2gop = Path(
     "/nfs/DGFI145/C/work_flo/cs2_files_samplus_test/CS2_open_ocean/CS_LTA__SIR_GOP_2__20150503T155002_20150503T163939_C001_0269.nc"
 )
```

### Comparing `pysamosa-0.2.12/scripts/luts/AUX_RLUT_S6A_002.nc` & `pysamosa-0.2.13/scripts/luts/AUX_RLUT_S6A_002.nc`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.12/scripts/luts/AUX_RLUT_S6A_003.nc` & `pysamosa-0.2.13/scripts/luts/AUX_RLUT_S6A_003.nc`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.12/scripts/luts/F0.txt` & `pysamosa-0.2.13/scripts/luts/F0.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.12/scripts/luts/F1.txt` & `pysamosa-0.2.13/scripts/luts/F1.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.12/scripts/luts/LUT_Alpha_P_CS-2.txt` & `pysamosa-0.2.13/scripts/luts/LUT_Alpha_P_CS-2.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.12/scripts/luts/S6A_TEST_AUX_FLUT___00000000T000000_99999999T999999_0001.NC` & `pysamosa-0.2.13/scripts/luts/S6A_TEST_AUX_FLUT___00000000T000000_99999999T999999_0001.NC`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.12/scripts/luts/alphap_table_SEN3_09_Nov_2017.txt` & `pysamosa-0.2.13/scripts/luts/alphap_table_SEN3_09_Nov_2017.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.12/scripts/luts/convert_luts.py` & `pysamosa-0.2.13/scripts/luts/convert_luts.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from pathlib import Path
 import pickle
-import numpy as np
-import xarray as xr
+from pathlib import Path
 
 import matplotlib.pyplot as plt
+import numpy as np
+import xarray as xr
 
 from pysamosa.common_types import SensorType
 
 
 def read_f(name):
     LUT_X = []
     LUT_Y = []
```

### Comparing `pysamosa-0.2.12/scripts/thesis_plots.py` & `pysamosa-0.2.13/scripts/thesis_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,30 @@
+import string
+from pathlib import Path
+
 import matplotlib.pyplot as plt
 import numpy as np
-from pathlib import Path
-import string
 
+from pysamosa import retracker
 from pysamosa.common_types import (
+    L1bSourceType,
     RetrackerBaseType,
-    WaveformSettings,
     SensorSettings,
-    L1bSourceType,
     SensorType,
+    WaveformSettings,
 )
-from pysamosa.model import SamosaModel, ModelParameter, ModelSettings
 from pysamosa.data_access import (
     _read_dataset_vars_from_ds,
-    get_subset_dataset,
-    get_model_param_obj_from_l1b_data,
     data_vars_s6,
+    get_model_param_obj_from_l1b_data,
+    get_subset_dataset,
 )
-from pysamosa.settings_manager import get_default_base_settings, SettingsPreset
+from pysamosa.model import ModelParameter, ModelSettings, SamosaModel
+from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
 from pysamosa.utils import gen_first_true
-from pysamosa import retracker
 
 default_width_in = 5.79  # in inches
 default_ratio = 0.5 + np.sqrt(5) / 2  # 1.618, golden ratio
 default_figsize_in = [default_width_in, default_width_in / default_ratio]
 
 # set_pgf_mode()
```

### Comparing `pysamosa-0.2.12/scripts/track_browser.py` & `pysamosa-0.2.13/scripts/track_browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from pathlib import Path
-import netCDF4
 
+import netCDF4
 import numpy as np
 import pandas as pd
 from bokeh.io import show
 from bokeh.models import HoverTool
 from bokeh.models.glyphs import Circle
-from bokeh.plotting import figure, ColumnDataSource
-from bokeh.tile_providers import get_provider, Vendors
+from bokeh.plotting import ColumnDataSource, figure
+from bokeh.tile_providers import Vendors, get_provider
 
 from pysamosa.data_access import _read_dataset_vars_from_ds
 
 data_vars_eumetsat_s6 = {
     "time": "time",
     "lat_rad": "latitude",
     "lon_rad": "longitude",
```

### Comparing `pysamosa-0.2.12/scripts/track_browser_footprint.py` & `pysamosa-0.2.13/scripts/track_browser_footprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import xarray as xr
-import cftime
-from pathlib import Path
 import tempfile
-import netCDF4
+from pathlib import Path
 
+import cftime
+import netCDF4
 import numpy as np
 import pandas as pd
-from bokeh.io import show, output_file
+import xarray as xr
+from bokeh.io import output_file, show
 from bokeh.models import HoverTool
 from bokeh.models.glyphs import Patches
-from bokeh.plotting import figure, ColumnDataSource
+from bokeh.plotting import ColumnDataSource, figure
 from bokeh.tile_providers import Vendors
 
 from pysamosa.data_access import _read_dataset_vars_from_ds
 from pysamosa.settings import TEST_DATA_DIR
 
 # data preparation
 ncfile_list = sorted((TEST_DATA_DIR / "l1bs").rglob("*.nc"))
```

### Comparing `pysamosa-0.2.12/setup.py` & `pysamosa-0.2.13/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
-import sys
-from setuptools import setup, find_packages, Extension
 import re
+import sys
+
+from setuptools import Extension, find_packages, setup
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
-# with open("HISTORY.rst") as history_file:
-#     history = history_file.read()
-
 requirements = []
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
     requirements = [
         r
         for r in requirements
         if re.split("[^a-zA-Z0-9]", r)[0]
         not in [
             "python",
             "watchdog",
             "pip",
             "bump2version",
             "tox",
             "flake8",
+            "black",
+            "isort",
             "imageio",
             "pytest",
             "wheel",
             "coverage",
             "twine",
         ]
     ]
@@ -65,11 +65,11 @@
     "sar altimetry ff-sar fully focused",
     name="pysamosa",
     packages=find_packages(include=["pysamosa", "pysamosa.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     ext_modules=extensions,
     url="https://github.com/floschl/pysamosa",
-    version="0.2.12",
+    version="0.2.13",
     zip_safe=False,
     setup_requires=[],
 )
```

### Comparing `pysamosa-0.2.12/tests/helpers.py` & `pysamosa-0.2.13/tests/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import numbers
 from textwrap import wrap
 
 import matplotlib.pyplot as plt
 import numpy as np
 
-from pysamosa.utils import consecutive_regions_from_ind_list
-
 from pysamosa.common_types import (
-    RetrackerProcessorSettings,
-    WaveformSettings,
+    SENSOR_SETS_DEFAULT_S3,
+    L1bSourceType,
     ModelSettings,
+    RetrackerProcessorSettings,
     RetrackerSettings,
     SensorSettings,
-    L1bSourceType,
-    SENSOR_SETS_DEFAULT_S3,
+    WaveformSettings,
 )
 from pysamosa.conf_params import CONST_C
 from pysamosa.data_access import get_model_param_obj_from_l1b_data, get_subset_dataset
 from pysamosa.model import SamosaModel
-from pysamosa.retracker import calc_misfit, SamosaRetracker
+from pysamosa.retracker import SamosaRetracker, calc_misfit
 from pysamosa.retracker_helpers import get_dynamic_first_guess_epochs
 from pysamosa.rip import RipAnalyser, RIPParameters
+from pysamosa.utils import consecutive_regions_from_ind_list
 
 
 def plot_retrack_result(
     l1b_data,
     l2_data,
     res_fit,
     model_params,
```

### Comparing `pysamosa-0.2.12/tests/settings_dumper.py` & `pysamosa-0.2.13/tests/settings_dumper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import numpy as np
 import logging
 
 # import imageio.v3 as iio
 import imageio.v2 as iio
-
+import numpy as np
 from scipy.io import savemat
 
 
 def dict_remove_None(d):
     return dict(filter(lambda item: item[1] is not None, dict(d).items()))
```

### Comparing `pysamosa-0.2.12/tests/test_common_types.py` & `pysamosa-0.2.13/tests/test_common_types.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pysamosa.common_types import (
-    RetrackerBaseType,
     FittingSettings,
-    WaveformSettings,
-    SensorType,
     L1bSourceType,
     ModelSettings,
+    RetrackerBaseType,
+    SensorType,
+    WaveformSettings,
 )
 
 
 def test_fitting_sets():
     fit_sets = FittingSettings(retracker_basetype=RetrackerBaseType.SAM)
     assert fit_sets.Fit_Var_2_Init_Hs == 2.0
```

### Comparing `pysamosa-0.2.12/tests/test_dist2coast.py` & `pysamosa-0.2.13/tests/test_dist2coast.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import numpy as np
-from pysamosa.dist2coast import (
-    get_dist_pacioos,
-)
 
+from pysamosa.dist2coast import get_dist_pacioos
 
 # def test_dist2coast_interp_on():
 #     """Test for cross-checking the results and performance of different dist2coast sources. """
 #
 #     n_repl = 1
 #     coords = {
 #             'lat': np.array([54.6177, 42.40, 54.0886, 54.7985, 36.0579, 48.1411] * n_repl),
```

### Comparing `pysamosa-0.2.12/tests/test_dynamic_fg_epoch.py` & `pysamosa-0.2.13/tests/test_dynamic_fg_epoch.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import numpy as np
 import pytest
 
 from pysamosa.common_types import SENSOR_SETS_DEFAULT_S3
 from pysamosa.retracker_helpers import (
-    get_tracker_shift_n_samps,
-    get_pointwise_product,
-    shift_waveform_by_n,
+    gen_sliding_window_from_seq,
     get_dynamic_first_guess_epochs,
     get_inds_sliding_window,
-    gen_sliding_window_from_seq,
+    get_pointwise_product,
+    get_tracker_shift_n_samps,
+    shift_waveform_by_n,
 )
 
 
 @pytest.mark.parametrize(
     "n_offset, n_inds",
     [
         (25800, 100),
```

### Comparing `pysamosa-0.2.12/tests/test_l1b_sim_retracker.py` & `pysamosa-0.2.13/tests/test_l1b_sim_retracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import matplotlib.pyplot as plt
 
-from pysamosa import retracker
-from pysamosa import simple_logger
+from pysamosa import retracker, simple_logger
 from pysamosa.common_types import (
-    RetrackerBaseType,
-    ModelSettings,
-    WaveformSettings,
+    SENSOR_SETS_DEFAULT_S3,
     L1bSourceType,
+    ModelSettings,
+    RetrackerBaseType,
     SensorSettings,
-    SENSOR_SETS_DEFAULT_S3,
+    WaveformSettings,
 )
 from pysamosa.data_access import get_model_param_obj_from_l1b_data
 from pysamosa.l1b_simulator import L1bSimulator
 from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
 from tests.helpers import plot_retrack_result
 
 l1b_src_type, retracker_basetype, settings_preset = (
```

### Comparing `pysamosa-0.2.12/tests/test_l1b_simulator.py` & `pysamosa-0.2.13/tests/test_l1b_simulator.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import pytest
 import matplotlib.pyplot as plt
+import pytest
 
 from pysamosa.common_types import (
+    L1bSourceType,
     ModelSettings,
     RetrackerBaseType,
-    WaveformSettings,
-    L1bSourceType,
     SensorSettings,
     SensorType,
+    WaveformSettings,
 )
 from pysamosa.l1b_simulator import L1bSimulator
 
 
 @pytest.mark.parametrize(
     "swh",
     # np.arange(1, 10, 2),
```

### Comparing `pysamosa-0.2.12/tests/test_leading_edge_detector.py` & `pysamosa-0.2.13/tests/test_leading_edge_detector.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import matplotlib.pyplot as plt
 
-from pysamosa.common_types import RetrackerBaseType, L1bSourceType
-from pysamosa.settings_manager import get_default_base_settings, SettingsPreset
+from pysamosa.common_types import L1bSourceType, RetrackerBaseType
+from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
 
 test_inds_gpod = [
     # coast
     # 12327,
     # 12330,
     # 12330,
     # 12330,
```

### Comparing `pysamosa-0.2.12/tests/test_model.py` & `pysamosa-0.2.13/tests/test_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from pysamosa.retracker import oversample_wf
 import matplotlib.pyplot as plt
 import numpy as np
 
 from pysamosa.common_types import (
+    L1bSourceType,
     RetrackerBaseType,
-    WaveformSettings,
     SensorSettings,
-    L1bSourceType,
     SensorType,
+    WaveformSettings,
 )
-from pysamosa.model import SamosaModel, ModelParameter, ModelSettings
+from pysamosa.model import ModelParameter, ModelSettings, SamosaModel
+from pysamosa.retracker import oversample_wf
 
 
 def test_setting_model_parameter_obj():
     mp = ModelParameter(ascending=True)
     print(mp)
     assert mp
```

### Comparing `pysamosa-0.2.12/tests/test_montecarlo_sim.py` & `pysamosa-0.2.13/tests/test_montecarlo_sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pytest
 
 from pysamosa.common_types import (
-    RetrackerBaseType,
+    L1bSourceType,
     ModelSettings,
+    RetrackerBaseType,
     WaveformSettings,
-    L1bSourceType,
 )
 from pysamosa.montecarlo_simulator import (
+    CostFunctionType,
     MonteCarloSimulator,
+    cost_functions,
+    default_cost_functions,
     plot_cost_func_vs_swh,
     plot_swh_epoch_scatter,
-    CostFunctionType,
-    default_cost_functions,
-    cost_functions,
 )
-from pysamosa.settings_manager import get_default_base_settings, SettingsPreset
-
+from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
 
 retracker_basetype, settings_preset = (
     # RetrackerBaseType.SAM, SettingsPreset.NONE,
     RetrackerBaseType.SAM,
     SettingsPreset.CORALv1,
     # RetrackerBaseType.SAMPLUS, SettingsPreset.NONE,
     # RetrackerBaseType.SAM, SettingsPreset.SAM_FLO,
```

### Comparing `pysamosa-0.2.12/tests/test_retrack_multi.py` & `pysamosa-0.2.13/tests/test_retrack_multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import logging
-
 from pathlib import Path
+
 import numpy as np
 
-from pysamosa.common_types import RetrackerBaseType, L1bSourceType, ProcMode
+from pysamosa.common_types import L1bSourceType, ProcMode, RetrackerBaseType
 from pysamosa.data_access import (
-    data_vars_s3,
-    data_vars_s6,
     data_vars_cs,
     data_vars_dart,
     data_vars_retracker,
+    data_vars_s3,
+    data_vars_s6,
 )
 from pysamosa.retracker_processor import RetrackerProcessor
-from pysamosa.settings_manager import get_default_base_settings, SettingsPreset
 from pysamosa.settings import S6_DATA_DIR
+from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
 from pysamosa.utils import plot_l2_results_vs_ref
 
 
 def raise_wrong_sensor_type(st, st_correct):
     if st.value is not st_correct.value:
         raise RuntimeError("choose correct SensorType")
```

### Comparing `pysamosa-0.2.12/tests/test_retrack_single.py` & `pysamosa-0.2.13/tests/test_retrack_single.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 import logging
 import tempfile
 from pathlib import Path
 from textwrap import wrap
-import xarray as xr
 
-import numpy as np
 import matplotlib.pyplot as plt
+import numpy as np
 import pytest
+import xarray as xr
 
-from pysamosa import retracker
-from pysamosa import simple_logger
+from pysamosa import retracker, simple_logger
 from pysamosa.common_types import (
     L1bSourceType,
-    RetrackerBaseType,
     ModelSettings,
     ProcMode,
+    RetrackerBaseType,
 )
 from pysamosa.data_access import (
-    get_subset_dataset,
-    get_model_param_obj_from_l1b_data,
     data_vars_dart,
     data_vars_retracker,
     data_vars_s6,
+    get_model_param_obj_from_l1b_data,
+    get_subset_dataset,
 )
 from pysamosa.retracker_helpers import get_dynamic_first_guess_epochs
-from pysamosa.settings_manager import get_default_base_settings, SettingsPreset
+from pysamosa.settings_manager import SettingsPreset, get_default_base_settings
 from tests.helpers import plot_retrack_result
 from tests.settings_dumper import SettingsDumper
 
-
 rel_inds, file_id = (
     # list(range(46403, 46403+60)), 's3_0',  # nice coastal retracking
     # scenario from CORAL paper
     [25480],
     "s3_0",  # nice coastal retracking scenario from CORAL paper
     # [1000], 'cs_0',
     # [3503], 'cs_1',
```

### Comparing `pysamosa-0.2.12/tests/test_samplusplus.py` & `pysamosa-0.2.13/tests/test_samplusplus.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.12/tests/test_utils.py` & `pysamosa-0.2.13/tests/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+
 from pysamosa.utils import consecutive_regions_from_ind_list
 
 
 def test_consecutive_regions_from_ind_list():
     a = [
         53,
         54,
```

