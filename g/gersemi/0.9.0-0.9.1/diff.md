# Comparing `tmp/gersemi-0.9.0.tar.gz` & `tmp/gersemi-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gersemi-0.9.0.tar", last modified: Tue May  2 16:46:29 2023, max compression
+gzip compressed data, was "gersemi-0.9.1.tar", last modified: Thu Jun 15 20:33:49 2023, max compression
```

## Comparing `gersemi-0.9.0.tar` & `gersemi-0.9.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:29.064202 gersemi-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-05-02 16:46:17.000000 gersemi-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-05-02 16:46:29.064202 gersemi-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15532 2023-05-02 16:46:17.000000 gersemi-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:29.048202 gersemi-0.9.0/gersemi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/ast_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/base_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/base_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/builtin_commands
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/cmake.lark
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:29.056202 gersemi-0.9.0/gersemi/command_invocation_dumpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/argument_aware_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/condition_syntax_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/ctest_command_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    24395 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/module_command_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/multiple_signature_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/preserving_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)    17819 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/project_command_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    33017 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/scripting_command_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/section_aware_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/specialized_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/target_link_libraries_command_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/two_word_keyword_isolator.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_line_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/custom_command_definition_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/formatted_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/keyword_with_pairs_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/parsing_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/result.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/return_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/sanity_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/task_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:29.060202 gersemi-0.9.0/gersemi/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/tasks/check_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/tasks/format_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/tasks/forward_to_stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/tasks/rewrite_in_place.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/tasks/show_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:29.048202 gersemi-0.9.0/gersemi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-05-02 16:46:29.000000 gersemi-0.9.0/gersemi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-02 16:46:29.000000 gersemi-0.9.0/gersemi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:46:29.000000 gersemi-0.9.0/gersemi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-02 16:46:29.000000 gersemi-0.9.0/gersemi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 16:46:29.000000 gersemi-0.9.0/gersemi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 16:46:29.000000 gersemi-0.9.0/gersemi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:46:29.064202 gersemi-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-02 16:46:17.000000 gersemi-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:29.064202 gersemi-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-02 16:46:17.000000 gersemi-0.9.0/tests/test_custom_command_dumper_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-02 16:46:17.000000 gersemi-0.9.0/tests/test_custom_command_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    28369 2023-05-02 16:46:17.000000 gersemi-0.9.0/tests/test_executable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-02 16:46:17.000000 gersemi-0.9.0/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-02 16:46:17.000000 gersemi-0.9.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-02 16:46:17.000000 gersemi-0.9.0/tests/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-02 16:46:17.000000 gersemi-0.9.0/tests/tests_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:33:49.729003 gersemi-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-06-15 20:33:41.000000 gersemi-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-06-15 20:33:49.729003 gersemi-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15532 2023-06-15 20:33:41.000000 gersemi-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:33:49.725003 gersemi-0.9.1/gersemi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/ast_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/base_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/base_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/builtin_commands
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/cmake.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:33:49.729003 gersemi-0.9.1/gersemi/command_invocation_dumpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/argument_aware_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/condition_syntax_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/ctest_command_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24458 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/module_command_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/multiple_signature_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/preserving_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/project_command_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33017 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/scripting_command_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/section_aware_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/specialized_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/target_link_libraries_command_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/two_word_keyword_isolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_line_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/custom_command_definition_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/formatted_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/keyword_with_pairs_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/parsing_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/return_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/sanity_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/task_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:33:49.729003 gersemi-0.9.1/gersemi/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/tasks/check_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/tasks/format_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/tasks/forward_to_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/tasks/rewrite_in_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/tasks/show_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:33:49.725003 gersemi-0.9.1/gersemi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-06-15 20:33:49.000000 gersemi-0.9.1/gersemi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-15 20:33:49.000000 gersemi-0.9.1/gersemi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 20:33:49.000000 gersemi-0.9.1/gersemi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 20:33:49.000000 gersemi-0.9.1/gersemi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 20:33:49.000000 gersemi-0.9.1/gersemi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 20:33:49.000000 gersemi-0.9.1/gersemi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 20:33:49.729003 gersemi-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-15 20:33:41.000000 gersemi-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:33:49.729003 gersemi-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-15 20:33:41.000000 gersemi-0.9.1/tests/test_custom_command_dumper_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-06-15 20:33:41.000000 gersemi-0.9.1/tests/test_custom_command_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28369 2023-06-15 20:33:41.000000 gersemi-0.9.1/tests/test_executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-15 20:33:41.000000 gersemi-0.9.1/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-15 20:33:41.000000 gersemi-0.9.1/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-15 20:33:41.000000 gersemi-0.9.1/tests/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-06-15 20:33:41.000000 gersemi-0.9.1/tests/tests_generator.py
```

### Comparing `gersemi-0.9.0/LICENSE` & `gersemi-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/PKG-INFO` & `gersemi-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gersemi
-Version: 0.9.0
+Version: 0.9.1
 Summary: A formatter to make your CMake code the real treasure
 Home-page: https://github.com/BlankSpruce/gersemi
 Author: Blank Spruce
 Author-email: blankspruce@protonmail.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `gersemi-0.9.0/README.md` & `gersemi-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/__main__.py` & `gersemi-0.9.1/gersemi/__main__.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/ast_helpers.py` & `gersemi-0.9.1/gersemi/ast_helpers.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/base_command_invocation_dumper.py` & `gersemi-0.9.1/gersemi/base_command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/base_dumper.py` & `gersemi-0.9.1/gersemi/base_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/builtin_commands` & `gersemi-0.9.1/gersemi/builtin_commands`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 add_executable
 add_library
 add_link_options
 add_subdirectory
 add_test
 aux_source_directory
 build_command
+cmake_file_api
 create_test_sourcelist
 define_property
 enable_language
 enable_testing
 export
 fltk_wrap_ui
 get_source_file_property
```

### Comparing `gersemi-0.9.0/gersemi/cache.py` & `gersemi-0.9.1/gersemi/cache.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/cmake.lark` & `gersemi-0.9.1/gersemi/cmake.lark`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/command_invocation_dumper.py` & `gersemi-0.9.1/gersemi/command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/command_invocation_dumpers/argument_aware_command_invocation_dumper.py` & `gersemi-0.9.1/gersemi/command_invocation_dumpers/argument_aware_command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/command_invocation_dumpers/condition_syntax_command_invocation_dumper.py` & `gersemi-0.9.1/gersemi/command_invocation_dumpers/condition_syntax_command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/command_invocation_dumpers/ctest_command_dumpers.py` & `gersemi-0.9.1/gersemi/command_invocation_dumpers/ctest_command_dumpers.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/command_invocation_dumpers/module_command_dumpers.py` & `gersemi-0.9.1/gersemi/command_invocation_dumpers/module_command_dumpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -640,16 +640,17 @@
 
 
 class BisonTarget(ArgumentAwareCommandInvocationDumper):
     one_value_keywords = ["COMPILE_FLAGS", "DEFINES_FILES", "VERBOSE", "REPORT_FILE"]
 
 
 class DoxygenAddDocs(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["targetName"]
     options = ["ALL", "USE_STAMP_FILE"]
-    one_value_keywords = ["WORKING_DIRECTORY", "COMMENT"]
+    one_value_keywords = ["WORKING_DIRECTORY", "COMMENT", "CONFIG_FILE"]
 
 
 class EnvModule(CommandLineFormatter, ArgumentAwareCommandInvocationDumper):
     one_value_keywords = ["OUTPUT_VARIABLE", "RESULT_VARIABLE"]
     multi_value_keywords = ["COMMAND"]
     keyword_formatters = {"COMMAND": "_format_command_line"}
```

### Comparing `gersemi-0.9.0/gersemi/command_invocation_dumpers/multiple_signature_command_invocation_dumper.py` & `gersemi-0.9.1/gersemi/command_invocation_dumpers/multiple_signature_command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/command_invocation_dumpers/preserving_command_invocation_dumper.py` & `gersemi-0.9.1/gersemi/command_invocation_dumpers/preserving_command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/command_invocation_dumpers/project_command_dumpers.py` & `gersemi-0.9.1/gersemi/command_invocation_dumpers/project_command_dumpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 from .target_link_libraries_command_dumper import TargetLinkLibraries
 from .two_word_keyword_isolator import TwoWordKeywordIsolator
 
 
 class AddCustomCommand(CommandLineFormatter, MultipleSignatureCommandInvocationDumper):
     customized_signatures = {
         "OUTPUT": dict(
-            options=["VERBATIM", "APPEND", "USES_TERMINAL", "COMMAND_EXPAND_LISTS"],
+            options=[
+                "VERBATIM",
+                "APPEND",
+                "USES_TERMINAL",
+                "COMMAND_EXPAND_LISTS",
+                "DEPENDS_EXPLICIT_ONLY",
+            ],
             one_value_keywords=[
                 "MAIN_DEPENDENCY",
                 "WORKING_DIRECTORY",
                 "COMMENT",
                 "DEPFILE",
                 "JOB_POOL",
             ],
@@ -114,14 +120,24 @@
 
 
 class BuildCommand(ArgumentAwareCommandInvocationDumper):
     front_positional_arguments = ["<variable>"]
     one_value_keywords = ["CONFIGURATION", "TARGET", "PROJECT_NAME", "PARALLEL_LEVEL"]
 
 
+class CMakeFileApi(MultipleSignatureCommandInvocationDumper):
+    customized_signatures = {
+        "QUERY": dict(
+            options=["QUERY"],
+            one_value_keywords=["API_VERSION"],
+            multi_value_keywords=["CODEMODEL", "CACHE", "CMAKEFILES", "TOOLCHAINS"],
+        ),
+    }
+
+
 class CreateTestSourcelist(ArgumentAwareCommandInvocationDumper):
     front_positional_arguments = ["sourceListName", "driverName"]
     one_value_keywords = ["EXTRA_INCLUDE", "FUNCTION"]
 
 
 class DefineProperty(ArgumentAwareCommandInvocationDumper):
     options = [
@@ -506,14 +522,15 @@
     "add_custom_target": AddCustomTarget,
     "add_dependencies": AddDependencies,
     "add_executable": AddExecutable,
     "add_library": AddLibrary,
     "add_subdirectory": AddSubdirectory,
     "add_test": AddTest,
     "build_command": BuildCommand,
+    "cmake_file_api": CMakeFileApi,
     "create_test_sourcelist": CreateTestSourcelist,
     "define_property": DefineProperty,
     "export": Export,
     "fltk_wrap_ui": FtlkWrapUi,
     "get_source_file_property": GetSourceFileProperty,
     "get_target_property": GetTargetProperty,
     "get_test_property": GetTestProperty,
```

### Comparing `gersemi-0.9.0/gersemi/command_invocation_dumpers/scripting_command_dumpers.py` & `gersemi-0.9.1/gersemi/command_invocation_dumpers/scripting_command_dumpers.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/command_invocation_dumpers/section_aware_command_invocation_dumper.py` & `gersemi-0.9.1/gersemi/command_invocation_dumpers/section_aware_command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/command_invocation_dumpers/specialized_dumpers.py` & `gersemi-0.9.1/gersemi/command_invocation_dumpers/specialized_dumpers.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/command_invocation_dumpers/target_link_libraries_command_dumper.py` & `gersemi-0.9.1/gersemi/command_invocation_dumpers/target_link_libraries_command_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/command_invocation_dumpers/two_word_keyword_isolator.py` & `gersemi-0.9.1/gersemi/command_invocation_dumpers/two_word_keyword_isolator.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/command_line_formatter.py` & `gersemi-0.9.1/gersemi/command_line_formatter.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/configuration.py` & `gersemi-0.9.1/gersemi/configuration.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/custom_command_definition_finder.py` & `gersemi-0.9.1/gersemi/custom_command_definition_finder.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/dumper.py` & `gersemi-0.9.1/gersemi/dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/exceptions.py` & `gersemi-0.9.1/gersemi/exceptions.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/formatter.py` & `gersemi-0.9.1/gersemi/formatter.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/keyword_with_pairs_formatter.py` & `gersemi-0.9.1/gersemi/keyword_with_pairs_formatter.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/parser.py` & `gersemi-0.9.1/gersemi/parser.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/parsing_transformer.py` & `gersemi-0.9.1/gersemi/parsing_transformer.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/postprocessor.py` & `gersemi-0.9.1/gersemi/postprocessor.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/result.py` & `gersemi-0.9.1/gersemi/result.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/runner.py` & `gersemi-0.9.1/gersemi/runner.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/sanity_checker.py` & `gersemi-0.9.1/gersemi/sanity_checker.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/tasks/check_formatting.py` & `gersemi-0.9.1/gersemi/tasks/check_formatting.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/tasks/format_file.py` & `gersemi-0.9.1/gersemi/tasks/format_file.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/tasks/rewrite_in_place.py` & `gersemi-0.9.1/gersemi/tasks/rewrite_in_place.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/tasks/show_diff.py` & `gersemi-0.9.1/gersemi/tasks/show_diff.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi/utils.py` & `gersemi-0.9.1/gersemi/utils.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/gersemi.egg-info/PKG-INFO` & `gersemi-0.9.1/gersemi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gersemi
-Version: 0.9.0
+Version: 0.9.1
 Summary: A formatter to make your CMake code the real treasure
 Home-page: https://github.com/BlankSpruce/gersemi
 Author: Blank Spruce
 Author-email: blankspruce@protonmail.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `gersemi-0.9.0/gersemi.egg-info/SOURCES.txt` & `gersemi-0.9.1/gersemi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/setup.py` & `gersemi-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/tests/test_custom_command_dumper_generation.py` & `gersemi-0.9.1/tests/test_custom_command_dumper_generation.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/tests/test_custom_command_formatting.py` & `gersemi-0.9.1/tests/test_custom_command_formatting.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/tests/test_executable.py` & `gersemi-0.9.1/tests/test_executable.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/tests/test_formatter.py` & `gersemi-0.9.1/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/tests/test_parser.py` & `gersemi-0.9.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.0/tests/tests_generator.py` & `gersemi-0.9.1/tests/tests_generator.py`

 * *Files identical despite different names*

