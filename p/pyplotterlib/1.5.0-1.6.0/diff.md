# Comparing `tmp/pyplotterlib-1.5.0.tar.gz` & `tmp/pyplotterlib-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplotterlib-1.5.0.tar", last modified: Thu Apr 20 09:31:28 2023, max compression
+gzip compressed data, was "pyplotterlib-1.6.0.tar", last modified: Thu Jun 15 19:21:22 2023, max compression
```

## Comparing `pyplotterlib-1.5.0.tar` & `pyplotterlib-1.6.0.tar`

### file list

```diff
@@ -1,77 +1,79 @@
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/
--rw-rw-r--   0 richard   (1000) richard   (1000)     1066 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/LICENSE
--rw-rw-r--   0 richard   (1000) richard   (1000)     2054 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/PKG-INFO
--rw-rw-r--   0 richard   (1000) richard   (1000)      151 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/README.md
--rw-rw-r--   0 richard   (1000) richard   (1000)     1124 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/pyproject.toml
--rw-rw-r--   0 richard   (1000) richard   (1000)       38 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/setup.cfg
--rw-rw-r--   0 richard   (1000) richard   (1000)       50 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/setup.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.532442 pyplotterlib-1.5.0/src/
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/__init__.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/core/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      570 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/json_transform.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1088 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/plot_command.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    11890 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/plot_options.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     5558 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/plotters.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/core/serialization/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/serialization/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      510 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/serialization/json_io.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      175 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/serialization/register.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2617 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/serialization/registration_funct.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/core/serialization/unit_tests/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/serialization/unit_tests/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2222 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/serialization/unit_tests/utest_create_from_json.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/core/unit_tests/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/unit_tests/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    17393 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/unit_tests/utest_plot_options.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     5031 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/core/unit_tests/utest_plotters.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/__init__.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/read_serialization_test/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/read_serialization_test/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1276 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/read_serialization_test/helpers.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      570 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/shared.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/viz_diff/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/viz_diff/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1693 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/viz_diff/helpers.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/standard/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    37511 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/plot_commands.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    27328 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/plot_options.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      911 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/plotters.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    10931 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/bar_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    16170 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/box_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    15587 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/disc_heat_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     8516 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/histogram_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     4673 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/image_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     4129 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/line_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    23966 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/rect_multi_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2686 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/shared.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     5300 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/shared_axis_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    18443 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/split_axis_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    23588 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/split_axis_plotter_creator.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/unit_tests/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/unit_tests/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2079 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/private/unit_tests/utests_histogram_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1937 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/serialization.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/__init__.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1119 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_bar_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      888 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_histogram_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      951 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_image_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1269 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_line_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1049 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_rect_multi_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1093 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_shared_axis_plotter.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1289 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_creator.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1059 2023-04-20 09:31:13.000000 pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_plotter.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:28.536442 pyplotterlib-1.5.0/src/pyplotterlib.egg-info/
--rw-rw-r--   0 richard   (1000) richard   (1000)     2054 2023-04-20 09:31:28.000000 pyplotterlib-1.5.0/src/pyplotterlib.egg-info/PKG-INFO
--rw-rw-r--   0 richard   (1000) richard   (1000)     2945 2023-04-20 09:31:28.000000 pyplotterlib-1.5.0/src/pyplotterlib.egg-info/SOURCES.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)        1 2023-04-20 09:31:28.000000 pyplotterlib-1.5.0/src/pyplotterlib.egg-info/dependency_links.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)      110 2023-04-20 09:31:28.000000 pyplotterlib-1.5.0/src/pyplotterlib.egg-info/requires.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)       13 2023-04-20 09:31:28.000000 pyplotterlib-1.5.0/src/pyplotterlib.egg-info/top_level.txt
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.692657 pyplotterlib-1.6.0/
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1066 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/LICENSE
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2054 2023-06-15 19:21:22.692657 pyplotterlib-1.6.0/PKG-INFO
+-rw-rw-r--   0 richard   (1000) richard   (1000)      151 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/README.md
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1199 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/pyproject.toml
+-rw-rw-r--   0 richard   (1000) richard   (1000)       38 2023-06-15 19:21:22.692657 pyplotterlib-1.6.0/setup.cfg
+-rw-rw-r--   0 richard   (1000) richard   (1000)       50 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/setup.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/__init__.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib/core/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      570 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/json_transform.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1088 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/plot_command.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    11955 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/plot_options.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     5558 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/plotters.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib/core/serialization/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/serialization/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      510 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/serialization/json_io.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      175 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/serialization/register.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2617 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/serialization/registration_funct.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib/core/serialization/unit_tests/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/serialization/unit_tests/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2222 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/serialization/unit_tests/utest_create_from_json.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib/core/unit_tests/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/unit_tests/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    17393 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/unit_tests/utest_plot_options.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     5031 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/core/unit_tests/utest_plotters.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/__init__.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/read_serialization_test/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/read_serialization_test/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1276 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/read_serialization_test/helpers.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      570 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/shared.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/viz_diff/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/viz_diff/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1693 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/viz_diff/helpers.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib/standard/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     5823 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/annotations.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    40317 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/plot_commands.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    28022 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/plot_options.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      952 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/plotters.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    17613 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/bar_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    16907 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/box_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    15676 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/disc_heat_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     8696 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/histogram_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     4762 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/image_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     4309 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/line_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    23966 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/rect_multi_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     3002 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/shared.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     5339 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/shared_axis_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    18443 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/split_axis_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    23588 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/split_axis_plotter_creator.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.692657 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/unit_tests/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/unit_tests/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2079 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/private/unit_tests/utests_histogram_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1937 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/serialization.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.692657 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/__init__.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.692657 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1119 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_bar_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      888 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_histogram_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      951 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_image_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1269 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_line_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1049 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_rect_multi_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1093 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_shared_axis_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1289 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_creator.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1059 2023-04-20 09:31:13.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_plotter.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1140 2023-06-15 19:20:07.000000 pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/utests_plot_commands.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2023-06-15 19:21:22.688657 pyplotterlib-1.6.0/src/pyplotterlib.egg-info/
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2054 2023-06-15 19:21:22.000000 pyplotterlib-1.6.0/src/pyplotterlib.egg-info/PKG-INFO
+-rw-rw-r--   0 richard   (1000) richard   (1000)     3047 2023-06-15 19:21:22.000000 pyplotterlib-1.6.0/src/pyplotterlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)        1 2023-06-15 19:21:22.000000 pyplotterlib-1.6.0/src/pyplotterlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)      180 2023-06-15 19:21:22.000000 pyplotterlib-1.6.0/src/pyplotterlib.egg-info/requires.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)       13 2023-06-15 19:21:22.000000 pyplotterlib-1.6.0/src/pyplotterlib.egg-info/top_level.txt
```

### Comparing `pyplotterlib-1.5.0/LICENSE` & `pyplotterlib-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/PKG-INFO` & `pyplotterlib-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplotterlib
-Version: 1.5.0
+Version: 1.6.0
 Summary: A package used to create plots in python
 Author-email: Richard Fogarty <richard.m.fogarty@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 RFogarty1
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyplotterlib-1.5.0/pyproject.toml` & `pyplotterlib-1.6.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=60.9.3", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyplotterlib"
-version = "1.5.0"
+version = "1.6.0"
 description = "A package used to create plots in python"
 readme = "README.md"
 authors = [{ name = "Richard Fogarty", email = "richard.m.fogarty@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Framework :: Matplotlib",
     "License :: OSI Approved :: MIT License",
@@ -24,16 +24,16 @@
     "matplotlib",
 ]
 
 #requires-python = ">=3.9"
 
 #Note: Initially created with python 3.10.4; but not sure if i can specify that anywhere
 [project.optional-dependencies]
-pinned = ["numpy ==1.22.2", "matplotlib==3.5.1"]
-dev = ["numpy", "matplotlib", "ipyplot", "pydataset","notebook"]
+pinned = ["numpy==1.22.2", "matplotlib==3.5.1"]
+dev = ["numpy==1.22.2", "matplotlib==3.5.1", "matplotlib-inline==0.1.3", "ipython==8.4.0", "ipyplot==1.1.1", "pydataset","notebook==6.4.12"]
 
 [project.urls]
 Documentation = "https://pyplotterlib.readthedocs.io/en/latest/index.html"
 Github = "https://github.com/RFogarty1/pyplotterlib"
 
 #[project.scripts]
 #something = "pyplotlib.__main__:main"
```

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/core/json_transform.py` & `pyplotterlib-1.6.0/src/pyplotterlib/core/json_transform.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/core/plot_command.py` & `pyplotterlib-1.6.0/src/pyplotterlib/core/plot_command.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/core/plot_options.py` & `pyplotterlib-1.6.0/src/pyplotterlib/core/plot_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,17 @@
 
 
 #Registered for Serialization mainly for purposes of test code
 @regHelp.registerForSerialization()
 class BooleanPlotOption(SinglePlotOptionInter):
 	pass
 
+class BooleanOrBoolIterPlotOption(SinglePlotOptionInter):
+	pass
+
 @regHelp.registerForSerialization()
 class StringPlotOption(SinglePlotOptionInter):
 	pass
 
 
 @regHelp.registerForSerialization()
 class StringIterPlotOption(SinglePlotOptionInter):
```

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/core/plotters.py` & `pyplotterlib-1.6.0/src/pyplotterlib/core/plotters.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/core/serialization/registration_funct.py` & `pyplotterlib-1.6.0/src/pyplotterlib/core/serialization/registration_funct.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/core/serialization/unit_tests/utest_create_from_json.py` & `pyplotterlib-1.6.0/src/pyplotterlib/core/serialization/unit_tests/utest_create_from_json.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/core/unit_tests/utest_plot_options.py` & `pyplotterlib-1.6.0/src/pyplotterlib/core/unit_tests/utest_plot_options.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/core/unit_tests/utest_plotters.py` & `pyplotterlib-1.6.0/src/pyplotterlib/core/unit_tests/utest_plotters.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/read_serialization_test/helpers.py` & `pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/read_serialization_test/helpers.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/shared.py` & `pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/shared.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/reg_testing/viz_diff/helpers.py` & `pyplotterlib-1.6.0/src/pyplotterlib/reg_testing/viz_diff/helpers.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/plot_commands.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/plot_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,14 +102,101 @@
 		except AttributeError:
 			figSize = None
 
 		currFigHandle = plt.figure(figsize=figSize)
 		currFigHandle.add_subplot(111)
 		plotterInstance._scratchSpace["axHandle"] = plt.gca()
 
+@serializationReg.registerForSerialization()
+class DrawShadedAnnotationsGeneric(plotCommCoreHelp.PlotCommand):
+
+	def __init__(self):
+		self._name = "drawGenericShadedAnnotations"
+		self._description = "Adds shaded area annotations to the plot"
+		self._optName = "annotationsShadedGeneric"
+
+	def execute(self, plotterInstance):
+		vals = _getValueFromOptName(plotterInstance, self._optName)
+		if vals is None:
+			return None
+
+		for annotation in vals:
+			self._addSingleAnnotation(plotterInstance, annotation)
+
+
+	def _addSingleAnnotation(self, plotterInstance, annotation):
+		#Figure out the command to use
+		useComm = self._getUseComm(annotation)		
+
+		#Figure out the keyword arguments
+		kwargDict = {"alpha":annotation.opacity}
+
+		if annotation.color is not None:
+			kwargDict["color"] = annotation.color
+
+		if annotation.polygonHooks is not None:
+			kwargDict.update(annotation.polygonHooks)
+
+		useComm(*annotation.shadeRange, **kwargDict)
+
+
+
+	def _getUseComm(self, annotation):
+		if annotation.direction.lower() == "vertical":
+			return plt.axvspan
+		elif annotation.direction.lower() == "horizontal":
+			return plt.axhspan
+		else:
+			raise ValueError("{} is an invalid value for annotation.direction".format(annotation.direction))
+
+
+@serializationReg.registerForSerialization()
+class DrawTextAnnotationsGeneric(plotCommCoreHelp.PlotCommand):
+
+	def __init__(self):
+		self._name = "drawGenericAnnotations"
+		self._description = "Adds Text annotations to the plot"
+		self._optName = "annotationsTextGeneric"
+
+	def execute(self, plotterInstance):
+		vals = _getValueFromOptName(plotterInstance, self._optName)
+		if vals is None:
+			return None
+
+		for annotation in vals:
+			self._addSingleAnnotation(plotterInstance, annotation)
+
+	def _addSingleAnnotation(self, plotterInstance, annotation):
+		annotatePos = annotation.arrowPos if annotation.arrowPos is not None else annotation.textPos
+		posArgs = [annotation.textVal, annotatePos]
+		useDict = {"xytext":annotation.textPos}
+
+		#Deal with fontsize; Note this can still be overwritten with "annotateMplHooks"
+		fontSize = _getValueFromOptName(plotterInstance, "fontSizeDefault")
+		fontSize = fontSize if annotation.fontSize is None else annotation.fontSize
+		useDict["fontsize"] = fontSize
+
+		#Update various fields
+		if annotation.arrowPos is not None:
+			useDict["arrowprops"] = dict()
+			if annotation.arrowPropHooks is not None:
+				useDict.update({"arrowprops":annotation.arrowPropHooks})
+
+		if annotation.annotateMplHooks is not None:
+			useDict.update(annotation.annotateMplHooks)
+
+		if annotation.arrowCoordSys is not None:
+			useDict.update({"xycoords":annotation.arrowCoordSys})
+
+		if annotation.textCoordSys is not None:
+			useDict.update({"textcoords":annotation.textCoordSys})
+
+		#Actually add the annotation
+		plt.annotate(*posArgs, **useDict)
+
 
 @serializationReg.registerForSerialization()
 class GridLinesCreate(plotCommCoreHelp.PlotCommand):
 
 	def __init__(self):
 		self._name = "create-grid-lines"
 		self._description = "Creates grid lines if required"
```

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/plot_options.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/plot_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,35 @@
 import types
 
 import numpy as np
 
 from ..core import plot_options as plotOptCore
 from ..core.serialization import register as serializationReg
 
+
+@serializationReg.registerForSerialization()
+class AnnotationsTextGeneric(plotOptCore.ObjectIterPlotOption):
+	""" Options containing details of various text annotations
+
+	Values should be iter of TextAnnotation objects (found in .annotations module)
+	"""
+	def __init__(self,name=None, value=None):
+		self.name = "annotationsTextGeneric"
+		self.value = value
+
+@serializationReg.registerForSerialization()
+class AnnotationsShadedGeneric(plotOptCore.ObjectIterPlotOption):
+	""" Options containing details of areas of the axis to shade
+
+	Values should be ShadedSliceAnnotation objects
+	"""
+	def __init__(self, name=None, value=None):
+		self.name = "annotationsShadedGeneric"
+		self.value = value
+
 @serializationReg.registerForSerialization()
 class AspectString(plotOptCore.StringPlotOption):
 	""" String controlling how the image aspect works
 
 	equal: Pixels kept square; aspect ratio is maintained but axes may not fill the space
 	auto: Aspect ratio is altered such that the image fits the axes; may be useful when creating grids of images
```

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/plotters.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/plotters.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,13 +9,15 @@
 from .private.split_axis_plotter import SplitAxisPlotter as SplitAxisPlotter
 from .private.split_axis_plotter_creator import SplitAxisPlotterCreator as SplitAxisPlotterCreator
 from .private import shared_axis_plotter
 
 #Code for serialization
 from .serialization import writePlotterToFile, readPlotterFromFile
 
+#Other objects
+from . import annotations
 
 
 #Define them like this to keep the file easier to read + plotters easy as possible to access
 #LinePlotter = line_plotter.LinePlotter
 DoubleAxisPlotter = shared_axis_plotter.DoubleAxisPlotter
```

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/bar_plotter.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/bar_plotter.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 
 from ...core import plotters as plotterCoreHelp
 from ...core import plot_command as plotCommCoreHelp
 from ...core import plot_options as plotOptCoreHelp
 
 from ...core.serialization import register as serializationReg
 
+from .. import annotations as annotateHelp
 from .. import plot_options as plotOptStdHelp
 from .. import plot_commands as plotCmdStdHelp
 
+
 @serializationReg.registerForSerialization()
 class BarPlotter(shared.FromJsonMixin, shared.FromPlotterMixin, plotterCoreHelp.SingleGraphPlotter):
 
 	def __init__(self, **kwargs):
 		""" Initializer
 		
 		Args:
@@ -42,14 +44,15 @@
 
 
 def _createCommandsList():
 	outList = [
 	plotCmdStdHelp.AddPlotterToOutput(),
 	plotCmdStdHelp.CreateFigureIfNoAxHandle(),
 	CalculateCentreVals(),
+	CalculateBottomVals(),
 	PlotOneDimDataAsBars(),
 	SetTickValsToGroupCentres(),
 	SetTickLabelsToGroupLabels(),
 	SetTickMinorValsOnOrOff(),
 	plotCmdStdHelp.GridLinesCreate(),
 	SetBarDataLabels(),
 	plotCmdStdHelp.SetBarColors(),
@@ -67,20 +70,27 @@
 	plotCmdStdHelp.SetAxisTickAndLabelVisibilitiesEachSide(),
 	plotCmdStdHelp.SetLegendLocStr(),
 	plotCmdStdHelp.SetLegendFontSize(),
 	plotCmdStdHelp.SetLegendFractPosStart(),
 	plotCmdStdHelp.SetLegendNumberColumns(),
 	plotCmdStdHelp.SetTitleStr(),
 	plotCmdStdHelp.PlotHozAndVertLines(),
-	plotCmdStdHelp.TurnLegendOnIfRequested()
+	plotCmdStdHelp.TurnLegendOnIfRequested(),
+	plotCmdStdHelp.DrawShadedAnnotationsGeneric(),
+	plotCmdStdHelp.DrawTextAnnotationsGeneric(),
+	AddBarLabels(),
 	]
 	return outList
 
 def _createOptionsList():
 	outList = [
+	AddBarLabelsByDefault(value=False),
+	BarLabels(),
+	plotOptStdHelp.AnnotationsShadedGeneric(),
+	plotOptStdHelp.AnnotationsTextGeneric(),
 	plotOptStdHelp.AxisBorderMakeInvisible(),
 	plotOptStdHelp.AxisColorX(),
 	plotOptStdHelp.AxisColorX_exclSpines(),
 	plotOptStdHelp.AxisColorY(),
 	plotOptStdHelp.AxisColorY_exclSpines(),
 	plotOptStdHelp.BarColors(),
 	plotOptStdHelp.BarOpacities(),
@@ -108,28 +118,51 @@
 	ShowMinorTickMarkers(),
 	ReverseIntraBarOrdering(),
 	WidthBars(value=1.0),
 	WidthInterSpacing(),
 	WidthIntraSpacing(value=0.0),
 	plotOptStdHelp.SetFigsizeOnCreation(),
 	plotOptStdHelp.ShowTicksAndLabelsOnSides( value=types.SimpleNamespace(top=None,bottom=None,left=None, right=None) ),
+	StackBars(),
 	plotOptStdHelp.TitleStr(),
 	plotOptStdHelp.XLabelFractPos(),
 	plotOptStdHelp.XLabelStr(),
 	plotOptStdHelp.YLabelFractPos(),
 	plotOptStdHelp.YLabelStr(),
 	plotOptStdHelp.XLimit(),
 	plotOptStdHelp.YLimit()
 	
 	]
 	return outList
 
 
 #Options
 @serializationReg.registerForSerialization()
+class AddBarLabelsByDefault(plotOptCoreHelp.BooleanPlotOption):
+	""" Boolean.
+
+	If True, then default bar labels will be added *iff* they are not specified in a more specific option
+
+	"""
+	def __init__(self, name=None, value=None):
+		self.name = "addBarLabelsByDefault" if name is None else name
+		self.value = value
+
+@serializationReg.registerForSerialization()
+class BarLabels(plotOptCoreHelp.ObjectIterPlotOption):
+	""" Iter of "BarLabelAnnotation" objects (found in the .annotations module)
+
+	These each refer to options to use for bar labels for a single data series. MUST pass an iterable, but will cycle over whatevers passed (meaning you can pass a single object for N data series)
+	"""
+	def __init__(self, name=None, value=None):
+		self.name = "barLabels" if name is None else name
+		self.value = value
+
+
+@serializationReg.registerForSerialization()
 class GroupLabels(plotOptStdHelp.GroupLabels):
 
 	"""String iter. Each is a label for a group of bars; if your only plotting one data series then this means 1 label per value input. 
 
 	E.g. If plotting years vs population this might be ["1970", "1980", "1990"]
 
 	"""
@@ -167,14 +200,29 @@
 
 	"""
 	def __init__(self, name=None, value=None):
 		self.name = "showMinorTickMarkers"
 		self.value = value
 
 @serializationReg.registerForSerialization()
+class StackBars(plotOptCoreHelp.BooleanOrBoolIterPlotOption):
+	""" Boolean or iter of Boolean. If set to True, means bars from different series are plotted on top of each other.
+
+	Examples:
+		1) value=False. Bars from different series are plotted adjacent to each other (for vertical plots)
+		2) value=True. Bars from different series are plotted on top of each other (for vertical plots)
+		3) value = [True,False]. Bars are stacked in pairs. If three data series are present then the first two are stacked, the next is adjacent.
+
+	"""
+	def __init__(self, name=None, value=None):
+		self.name = "stackBars" if name is None else name
+		self.value = value
+
+
+@serializationReg.registerForSerialization()
 class WidthBars(plotOptCoreHelp.FloatPlotOption):
 	""" Width value for each bar in the bar chart. The default is generally 1.0
 
 	"""
 	def __init__(self, name=None, value=None):
 		self.name = "widthBars"
 		self.value = value
@@ -198,43 +246,174 @@
 		self.value = value
 
 
 
 
 #Commands
 @serializationReg.registerForSerialization()
-class CalculateCentreVals(plotCommCoreHelp.PlotCommand):
+class AddBarLabels(plotCommCoreHelp.PlotCommand):
+
+	def __init__(self):
+		self._name = "add-labels-to-bars"
+		self._description = "Adds labels to bars; generally showing the value for each"
+
+	def execute(self, plotterInstance):
+		#Get relevant values
+		labelByDefault = plotCmdStdHelp._getValueFromOptName(plotterInstance, "addBarLabelsByDefault")
+		nonDefaultLabels = plotCmdStdHelp._getValueFromOptName(plotterInstance, "barLabels", retIfNone=list())
+
+		if (labelByDefault is not True) and (len(nonDefaultLabels)==0):
+			return None
+
+		#Populate default labels if required; exit if no plot data to populate them with
+		plotData = plotCmdStdHelp._getValueFromOptName(plotterInstance, "plotData1D", retIfNone=list())
+		if len(nonDefaultLabels)==0:
+			if len(plotData)==0:
+				return None
+			nonDefaultLabels = [annotateHelp.BarLabelAnnotation() for x in plotData]
+
+		#
+		bars = plotterInstance._scratchSpace["barHandles"]
+		cycledLabels = it.cycle(nonDefaultLabels)
+		for data, bar,annotation in zip(plotData, bars,cycledLabels):
+			self._addAnnotation(data, bar, annotation, plotterInstance)
+
+	#TODO: Probably need to check for None with the format
+	def _addAnnotation(self, data, inpBar, annotation, plotterInstance):
+		labels = [annotation.fmt.format(x) for x in data]
+
+		#Set standard kwargs
+		defaultFontsize = plotCmdStdHelp._getDefaultFontSizeFromPlotter(plotterInstance)
+		kwargs = {"labels":labels, "padding":annotation.paddingVal, "fontsize":defaultFontsize}
+
+		if annotation.fontSize is not None:
+			kwargs["fontsize"] = annotation.fontSize
+
+		if annotation.fontRotation is not None:
+			kwargs["rotation"] = annotation.fontRotation
+
+		#Add overides; this can likely include the "labels" as a keyword
+		if annotation.mplBarLabelHooks is not None:
+			kwargs.update(annotation.mplBarLabelHooks)
+
+		plt.bar_label(inpBar, **kwargs)
+
+
+class _CalcValsMixin():
+
+	#List is actually 1 element longer than needed i think but...
+	def _getSkipSeriesList(self,plotterInstance, plotData):
+		stackVals = plotCmdStdHelp._getValueFromOptName(plotterInstance, "stackBars")
+		if stackVals is not None:
+			try:
+				iter(stackVals)
+			except TypeError:
+				stackVals = [stackVals for unused in plotData]
+			else:
+				stackVals = [val for val,unused in zip( it.cycle(stackVals), plotData)]
+		return stackVals 
+
+
+@serializationReg.registerForSerialization()
+class CalculateBottomVals(plotCommCoreHelp.PlotCommand, _CalcValsMixin):
+
+	def __init__(self):
+		self._name = "calculate-bar-bottom-vals"
+		self._description = "Calculates the bottom value of each bar (i.e. where to draw from) and saves to the scratch space"
+
+	def execute(self, plotterInstance):
+		#Get the data, exit if none present
+		plotData = plotCmdStdHelp._getValueFromOptName(plotterInstance, "plotData1D")
+		if plotData is None:
+			return None
+		elif len(plotData)==0:
+			return None
+
+		reverseIntraBarOrdering = plotCmdStdHelp._getValueFromOptName(plotterInstance, "reverseIntraBarOrdering", retIfNone=False)
+
+		#Figure out which (if any) series should be stacked
+		skipVals = self._getSkipSeriesList(plotterInstance, plotData)
+		barBotVals = _getBarBottomVals(plotData, skipVals, reverseIntraOrdering=reverseIntraBarOrdering)
+		plotterInstance._scratchSpace["bottom_vals"] = barBotVals
+
+
+def _getBarBottomVals(inpPlotData, skipVals, reverseIntraOrdering=False):
+
+
+	#Initialize output
+	nSeries = len(inpPlotData)
+	nGroups = max( [len(x) for x in inpPlotData] )
+	outVals = [ list() for x in range(nSeries) ]
+
+	#
+	if skipVals is None:
+		skipVals = [False for x in range(nSeries)]
+
+	#Best to NOT reverse stack order i think.
+	if reverseIntraOrdering:
+#		skipVals = [val for val in reversed(skipVals)]
+		plotData = list()
+		for currSeries in reversed(inpPlotData):
+			plotData.append(currSeries)
+	else:
+		plotData = inpPlotData 
+
+
+	defStartPos = 0.0
+
+	#Set the first series to zero for each group
+	outVals[0] = [defStartPos for x in range(nGroups)]
+
+	#Now we apply the relevant shift to each series
+	for skipShift,sIdx in zip(skipVals,range(1,nSeries)):
+		for gIdx in range(nGroups):
+			if skipShift is True:
+				prevBottom = outVals[sIdx-1][gIdx]
+				prevVal = plotData[sIdx-1][gIdx]
+				outVals[sIdx].append( prevBottom + prevVal )
+			else:
+				outVals[sIdx].append(defStartPos)
+
+
+	return outVals
+
+@serializationReg.registerForSerialization()
+class CalculateCentreVals(plotCommCoreHelp.PlotCommand, _CalcValsMixin):
 
 	def __init__(self):
 		self._name = "calculate-bar-centre-vals"
 		self._description = "Calculates the central position of each bar in the bar plot and saves to the scratch space"
 
 	def execute(self, plotterInstance):
 		#Get the data, exit if none present
 		plotData = getattr(plotterInstance.opts, "plotData1D").value
 		if plotData is None:
 			return None
 		elif len(plotData)==0:
 			return None
 
+		#Figure out which (if any) series should be stacked
+		skipVals = self._getSkipSeriesList(plotterInstance, plotData)
+
 		#Get the relevant widths
 		widthBars = plotterInstance.opts.widthBars.value
 		widthInterSpacing = plotterInstance.opts.widthInterSpacing.value
 		widthIntraSpacing = plotterInstance.opts.widthIntraSpacing.value
 
 		widthBars = 1 if widthBars is None else widthBars
 		widthInterSpacing = 1 if widthInterSpacing is None else widthInterSpacing
 		widthIntraSpacing = 0.0 if widthIntraSpacing is None else widthIntraSpacing
 
 		#Calculate the centre values
 		nGroups = max( [len(x) for x in plotData] )
 		nSeries = len(plotData)
 
 		_currArgs = [nGroups, nSeries, widthBars, widthIntraSpacing, widthInterSpacing]
-		barCentres, groupCentres = shared._getIndividAndGroupCentresBarLikePlot(*_currArgs, startPos=0)
+		_currKwargs = {"startPos":0, "skipSeries":skipVals}
+		barCentres, groupCentres = shared._getIndividAndGroupCentresBarLikePlot(*_currArgs, **_currKwargs)
 
 		plotterInstance._scratchSpace["centres"] = barCentres
 		plotterInstance._scratchSpace["groupCentres"] = groupCentres
 
 
 #This will get A LOT more complicated later (when dealing with widths etc)
 @serializationReg.registerForSerialization()
@@ -248,17 +427,18 @@
 	def execute(self, plotterInstance):
 		#Get the data; exit if none present
 		targVal = getattr(plotterInstance.opts, self._optName).value
 
 		if not( _doesPlotterInstanceHaveData(plotterInstance) ):
 			return None
 
-		#Check if we plot vertically or horizontally
+		#Check if we plot vertically or horizontally + get the bar centres/bottoms
 		plotHoz = plotterInstance.opts.plotHorizontally.value
 		allCentres = plotterInstance._scratchSpace["centres"]
+		allBottoms = plotterInstance._scratchSpace["bottom_vals"]
 
 		#Figure out the bar widths
 		barWidth = plotterInstance.opts.widthBars.value
 		barWidth = 1.0 if barWidth is None else barWidth
 
 
 		#Optionally reverse the order the bars are plotted in
@@ -266,25 +446,27 @@
 
 		#Plot the data; may want to return handles to scratch space later
 		outBars = list()
 		for idx,currData in enumerate(targVal):
 			#We need centres for idx from the other end is all
 			if reverseIntraOrdering:
 				centres = allCentres[len(targVal)-1-idx]
-
+				bottoms = allBottoms[len(targVal)-1-idx]
 			else:
 				centres = allCentres[idx]
+				bottoms = allBottoms[idx]
 
 			useCentres = [centre for centre,val in zip(centres,currData) if val is not None]
+			useBottoms = [bottom for bottom,val in zip(bottoms,currData) if val is not None]
 			useData = [val for val in currData if val is not None]
 
 			if plotHoz:
-				currBars = plt.barh( np.array(useCentres), np.array(useData), height=barWidth )
+				currBars = plt.barh( np.array(useCentres), np.array(useData), height=barWidth, left=np.array(useBottoms) )
 			else:
-				currBars = plt.bar( np.array(useCentres), np.array(useData), width=barWidth )
+				currBars = plt.bar( np.array(useCentres), np.array(useData), width=barWidth, bottom=np.array(useBottoms) )
 
 			outBars.append(currBars)
 
 		plotterInstance._scratchSpace["barHandles"] = outBars
 		return
 
 @serializationReg.registerForSerialization()
```

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/box_plotter.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/box_plotter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 
 
 import copy
 import itertools as it
+import types
 import matplotlib.pyplot as plt
 
 import numpy as np
 
 from . import shared
 
 from .. import plot_options as plotOptStdHelp
@@ -58,37 +59,49 @@
 	AddNotchesOnOrOffToScratch(),
 	AddOutlierOptsToScratch(),
 	AddWhiskerOnOrOffToScratch(),
 	PlotBoxData(),
 	plotCmdStdHelp.SetTickValsToGroupCentres(),
 	plotCmdStdHelp.SetTickLabelsToGroupLabels(),
 	plotCmdStdHelp.SetTickLabelFontSize(),
+	plotCmdStdHelp.SetAxisTickAndLabelVisibilitiesEachSide(),
+	plotCmdStdHelp.SetTickMinorMarkersOn(),
 	plotCmdStdHelp.GridLinesCreate(),
 	plotCmdStdHelp.SetTitleStr(),
 	plotCmdStdHelp.SetXLabelStr(),
 	plotCmdStdHelp.SetXLabelFractPos(),
 	plotCmdStdHelp.SetYLabelStr(),
 	plotCmdStdHelp.SetYLabelFractPos(),
 	plotCmdStdHelp.SetXLimit(),
 	plotCmdStdHelp.SetYLimit(),
+	plotCmdStdHelp.SetAxisColorX(), #Best if done after labels etc. set
+	plotCmdStdHelp.SetAxisColorY(),
 
 	plotCmdStdHelp.PlotHozAndVertLines(),
 
 	plotCmdStdHelp.SetLegendFontSize(),
 	plotCmdStdHelp.SetLegendNumberColumns(),
 	plotCmdStdHelp.SetLegendLocStr(),
 	plotCmdStdHelp.SetLegendFractPosStart(),
 	SetLegendDataHandlesAndLabels(),
 	plotCmdStdHelp.TurnLegendOnIfRequested(),
+	plotCmdStdHelp.DrawShadedAnnotationsGeneric(),
+	plotCmdStdHelp.DrawTextAnnotationsGeneric(),
 	]
 	return outList
 
 
 def _createOptionsList():
 	outList = [
+	plotOptStdHelp.AnnotationsShadedGeneric(),
+	plotOptStdHelp.AnnotationsTextGeneric(),
+	plotOptStdHelp.AxisColorX(),
+	plotOptStdHelp.AxisColorX_exclSpines(),
+	plotOptStdHelp.AxisColorY(),
+	plotOptStdHelp.AxisColorY_exclSpines(),
 	BoxColorsOn(),
 	BoxColorStrsInterSeries(),
 	BoxNotchOn(),
 	plotOptStdHelp.DataLabels(),
 	plotOptStdHelp.FontSizeDefault(),
 	plotOptStdHelp.GridLinesShow(),
 	plotOptStdHelp.GridLinesShowX(),
@@ -107,14 +120,17 @@
 	plotOptStdHelp.PlotHozLinesColorStrs(),
 	plotOptStdHelp.PlotHozLinesPositions(),
 	plotOptStdHelp.PlotHozLinesStyleStrs(),
 	plotOptStdHelp.PlotVertLinesColorStrs(),
 	plotOptStdHelp.PlotVertLinesPositions(),
 	plotOptStdHelp.PlotVertLinesStyleStrs(),
 	plotOptStdHelp.SetFigsizeOnCreation(),
+	plotOptStdHelp.ShowMinorTickMarkersX(),
+	plotOptStdHelp.ShowMinorTickMarkersY(),
+	plotOptStdHelp.ShowTicksAndLabelsOnSides( value=types.SimpleNamespace(top=None,bottom=None,left=None, right=None) ),
 	plotOptStdHelp.TitleFractPosX(),
 	plotOptStdHelp.TitleFractPosY(),
 	plotOptStdHelp.TitleStr(),
 	plotOptStdHelp.XLabelStr(),
 	plotOptStdHelp.XLabelFractPos(),
 	plotOptStdHelp.YLabelStr(),
 	plotOptStdHelp.YLabelFractPos(),
```

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/disc_heat_plotter.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/disc_heat_plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,25 +60,27 @@
 	plotCmdStdHelp.SetXLabelStr(),
 	plotCmdStdHelp.SetYLabelStr(),
 	SetTicksToDataCentres(),
 	SetTickLabelsToGroupLabels(),
 	AddDataAnnotations(),
 	plotCmdStdHelp.SetTickLabelFontSize(),
 	plotCmdStdHelp.GridLinesCreate(),
-	plotCmdStdHelp.SetTitleStr()
+	plotCmdStdHelp.SetTitleStr(),
+	plotCmdStdHelp.DrawTextAnnotationsGeneric(),
 	]
 	return outList
 
 def _createOptionsList():
 	outList = [
 	AnnotateVals(),
 	AnnotateValsFontSize(),
 	AnnotateValsRotation(),
 	AnnotateValsStrFmt(value="{:.2f}"),
 	AnnotateValsTextColor(),
+	plotOptStdHelp.AnnotationsTextGeneric(),
 	plotOptStdHelp.AspectString(value="auto"),
 	plotOptStdHelp.ColorBarFontSize(),
 	plotOptStdHelp.ColorBarLabelFontSize(),
 	plotOptStdHelp.ColorBarTickLabelFontSize(),
 	plotOptStdHelp.ColorBarLabel(),
 	plotOptStdHelp.ColorBarLocation(),
 	plotOptStdHelp.ColorBarShow(),
```

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/histogram_plotter.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/histogram_plotter.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,24 +64,28 @@
 	plotCmdStdHelp.SetTitleStr(),
 	plotCmdStdHelp.SetLegendLocStr(),
 	plotCmdStdHelp.SetLegendFontSize(),
 	plotCmdStdHelp.SetLegendFractPosStart(),
 	plotCmdStdHelp.SetLegendNumberColumns(),
 	plotCmdStdHelp.PlotHozAndVertLines(),
 	plotCmdStdHelp.TurnLegendOnIfRequested(),
-	plotCmdStdHelp.AddPlotterToOutput()
+	plotCmdStdHelp.AddPlotterToOutput(),
+	plotCmdStdHelp.DrawShadedAnnotationsGeneric(),
+	plotCmdStdHelp.DrawTextAnnotationsGeneric()
 	]
 
 	return outList
 
 #Write in alphabetical order
 #Largely taken from Line_Plotter
 #TODO: Various forms of plotData
 def _createOptionsList():
 	outList = [
+	plotOptStdHelp.AnnotationsShadedGeneric(),
+	plotOptStdHelp.AnnotationsTextGeneric(),
 	plotOptStdHelp.AxisBorderMakeInvisible(),
 	plotOptStdHelp.AxisColorX(),
 	plotOptStdHelp.AxisColorX_exclSpines(),
 	plotOptStdHelp.AxisColorY(),
 	plotOptStdHelp.AxisColorY_exclSpines(),
 	plotOptStdHelp.BarColors(),
 	plotOptStdHelp.BarOpacities(),
```

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/image_plotter.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/image_plotter.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,23 +54,25 @@
 	plotCmdStdHelp.GridLinesCreate(),
 	plotCmdStdHelp.SetXLabelFractPos(),
 	plotCmdStdHelp.SetYLabelFractPos(),
 	plotCmdStdHelp.SetXLimit(),
 	plotCmdStdHelp.SetYLimit(),
 	plotCmdStdHelp.SetAxisColorX(), #Best if done after labels etc. set
 	plotCmdStdHelp.SetAxisColorY(),
-	plotCmdStdHelp.SetTitleStr()
+	plotCmdStdHelp.SetTitleStr(),
+	plotCmdStdHelp.DrawTextAnnotationsGeneric(),
 	]
 
 	return outList
 
 
 #Write in alphabetical order
 def _createOptionsList():
 	outList = [
+	plotOptStdHelp.AnnotationsTextGeneric(),
 	AspectString(),
 	plotOptStdHelp.AxisColorX(),
 	plotOptStdHelp.AxisColorX_exclSpines(),
 	plotOptStdHelp.AxisColorY(),
 	plotOptStdHelp.AxisColorY_exclSpines(),
 	plotOptStdHelp.ColorBarFontSize(),
 	plotOptStdHelp.ColorBarLabelFontSize(),
```

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/line_plotter.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/line_plotter.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,22 +66,26 @@
 	plotCmdStdHelp.SetAxisBorderInvisible(),
 	plotCmdStdHelp.SetTitleStr(),
 	plotCmdStdHelp.SetLegendLocStr(),
 	plotCmdStdHelp.SetLegendFontSize(),
 	plotCmdStdHelp.SetLegendFractPosStart(),
 	plotCmdStdHelp.SetLegendNumberColumns(),
 	plotCmdStdHelp.PlotHozAndVertLines(),
-	plotCmdStdHelp.TurnLegendOnIfRequested()
+	plotCmdStdHelp.TurnLegendOnIfRequested(),
+	plotCmdStdHelp.DrawShadedAnnotationsGeneric(),
+	plotCmdStdHelp.DrawTextAnnotationsGeneric()
 	]
 
 	return outList
 
 #Write in alphabetical order
 def _createOptionsList():
 	outList = [
+	plotOptStdHelp.AnnotationsShadedGeneric(),
+	plotOptStdHelp.AnnotationsTextGeneric(),
 	plotOptStdHelp.AxisBorderMakeInvisible(),
 	plotOptStdHelp.AxisColorX(),
 	plotOptStdHelp.AxisColorX_exclSpines(),
 	plotOptStdHelp.AxisColorY(),
 	plotOptStdHelp.AxisColorY_exclSpines(),
 	plotOptStdHelp.AxisScaleX(),
 	plotOptStdHelp.AxisScaleY(),
```

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/rect_multi_plotter.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/rect_multi_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/shared.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/shared.py`

 * *Files 17% similar despite different names*

```diff
@@ -54,25 +54,35 @@
 	startX, startY, xLength, yLength = inpAx.get_position().bounds
 	endX, endY = startX+xLength, startY+yLength
 	return startX, startY, endX, endY
 
 
 
 #Refactored/Extracted from bar_plotter; also usable in boxPlotter (and likely other similar plotters in the future)
-def _getIndividAndGroupCentresBarLikePlot(nGroups, nSeries, widthBar, widthIntraSpacing, widthInterSpacing, startPos=0):
+def _getIndividAndGroupCentresBarLikePlot(nGroups, nSeries, widthBar, widthIntraSpacing,
+                                          widthInterSpacing, startPos=0, skipSeries=None):
 	outCentres = [ list() for x in range(nSeries) ]
 	currPos = startPos
 
+	if skipSeries is None:
+		skipSeries = [False for x in range(nSeries)]
+
 	#Figure out where to plot the individual bars/similar
 	for gIdx in range(nGroups):
-		for sIdx in range(nSeries):
+		for skipShift,sIdx in zip(skipSeries, range(nSeries)):
 			outCentres[sIdx].append(currPos)
-			currPos += widthBar
-			currPos += widthIntraSpacing
-		currPos += widthInterSpacing
+			if skipShift is False:
+				currPos += widthIntraSpacing
+				currPos += widthBar
+
+		#Not 100% sure why this if statement had to be added
+		if any(skipSeries):
+			currPos += widthInterSpacing + widthBar
+		else:
+			currPos += widthInterSpacing
 
 
 	#Figure out the centre of each group
 	groupCentres = list()
 	for idx in range(nGroups):
 		currCentres = [ x[idx] for x in outCentres ]
 		currAverage = sum(currCentres)/len(currCentres)
```

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/shared_axis_plotter.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/shared_axis_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,16 @@
 
 def _createOptionsList():
 	outList = [
 
 	AllowTwoIndependentAxes(),
 	plotOptStdHelp.PlotterIter(),
 	IndependentXAxis(),
-	IndependentYAxis()
-
+	IndependentYAxis(),
+	plotOptStdHelp.SetFigsizeOnCreation()
 	]
 	return outList
 
 
 #These commands/options are only really EVER needed here
 
 @serializationReg.registerForSerialization()
```

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/split_axis_plotter.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/split_axis_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/split_axis_plotter_creator.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/split_axis_plotter_creator.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/private/unit_tests/utests_histogram_plotter.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/private/unit_tests/utests_histogram_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/serialization.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/serialization.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_bar_plotter.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_bar_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_histogram_plotter.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_histogram_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_image_plotter.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_image_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_line_plotter.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_line_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_rect_multi_plotter.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_rect_multi_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_shared_axis_plotter.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_shared_axis_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_creator.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_creator.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_plotter.py` & `pyplotterlib-1.6.0/src/pyplotterlib/standard/unit_tests/serialization/utests_split_axis_plotter.py`

 * *Files identical despite different names*

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib.egg-info/PKG-INFO` & `pyplotterlib-1.6.0/src/pyplotterlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplotterlib
-Version: 1.5.0
+Version: 1.6.0
 Summary: A package used to create plots in python
 Author-email: Richard Fogarty <richard.m.fogarty@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 RFogarty1
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyplotterlib-1.5.0/src/pyplotterlib.egg-info/SOURCES.txt` & `pyplotterlib-1.6.0/src/pyplotterlib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 src/pyplotterlib/reg_testing/__init__.py
 src/pyplotterlib/reg_testing/shared.py
 src/pyplotterlib/reg_testing/read_serialization_test/__init__.py
 src/pyplotterlib/reg_testing/read_serialization_test/helpers.py
 src/pyplotterlib/reg_testing/viz_diff/__init__.py
 src/pyplotterlib/reg_testing/viz_diff/helpers.py
 src/pyplotterlib/standard/__init__.py
+src/pyplotterlib/standard/annotations.py
 src/pyplotterlib/standard/plot_commands.py
 src/pyplotterlib/standard/plot_options.py
 src/pyplotterlib/standard/plotters.py
 src/pyplotterlib/standard/serialization.py
 src/pyplotterlib/standard/private/__init__.py
 src/pyplotterlib/standard/private/bar_plotter.py
 src/pyplotterlib/standard/private/box_plotter.py
@@ -44,14 +45,15 @@
 src/pyplotterlib/standard/private/shared.py
 src/pyplotterlib/standard/private/shared_axis_plotter.py
 src/pyplotterlib/standard/private/split_axis_plotter.py
 src/pyplotterlib/standard/private/split_axis_plotter_creator.py
 src/pyplotterlib/standard/private/unit_tests/__init__.py
 src/pyplotterlib/standard/private/unit_tests/utests_histogram_plotter.py
 src/pyplotterlib/standard/unit_tests/__init__.py
+src/pyplotterlib/standard/unit_tests/utests_plot_commands.py
 src/pyplotterlib/standard/unit_tests/serialization/__init__.py
 src/pyplotterlib/standard/unit_tests/serialization/utests_bar_plotter.py
 src/pyplotterlib/standard/unit_tests/serialization/utests_histogram_plotter.py
 src/pyplotterlib/standard/unit_tests/serialization/utests_image_plotter.py
 src/pyplotterlib/standard/unit_tests/serialization/utests_line_plotter.py
 src/pyplotterlib/standard/unit_tests/serialization/utests_rect_multi_plotter.py
 src/pyplotterlib/standard/unit_tests/serialization/utests_shared_axis_plotter.py
```

