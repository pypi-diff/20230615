# Comparing `tmp/otter-grader-4.3.2.tar.gz` & `tmp/otter-grader-4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otter-grader-4.3.2.tar", last modified: Sun Apr  9 02:12:47 2023, max compression
+gzip compressed data, was "otter-grader-4.3.3.tar", last modified: Thu Jun 15 18:38:12 2023, max compression
```

## Comparing `otter-grader-4.3.2.tar` & `otter-grader-4.3.3.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.571774 otter-grader-4.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-09 02:12:00.000000 otter-grader-4.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-09 02:12:00.000000 otter-grader-4.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-04-09 02:12:47.571774 otter-grader-4.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-09 02:12:00.000000 otter-grader-4.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.559774 otter-grader-4.3.2/otter/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.559774 otter-grader-4.3.2/otter/assign/
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/cell_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/feature_toggle.py
--rw-r--r--   0 runner    (1001) docker     (123)    16894 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/question_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.559774 otter-grader-4.3.2/otter/assign/r_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/r_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/r_adapter/cell_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/r_adapter/rmarkdown_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/r_adapter/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/r_adapter/tests_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/tests_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.559774 otter-grader-4.3.2/otter/assign/v0/
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/cell_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.559774 otter-grader-4.3.2/otter/assign/v0/convert/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/convert/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/convert/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/questions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.563773 otter-grader-4.3.2/otter/assign/v0/r_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/r_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/r_adapter/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.563773 otter-grader-4.3.2/otter/assign/v0/rmarkdown_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/rmarkdown_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/rmarkdown_adapter/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/rmarkdown_adapter/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/rmarkdown_adapter/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/rmarkdown_adapter/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/rmarkdown_adapter/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/rmarkdown_adapter/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/assign/v0/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.563773 otter-grader-4.3.2/otter/check/
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17923 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/check/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/check/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-04-09 02:12:44.000000 otter-grader-4.3.2/otter/check/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.563773 otter-grader-4.3.2/otter/check/validate_export/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/check/validate_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/check/validate_export/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.563773 otter-grader-4.3.2/otter/execute/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/execute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/execute/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/execute/execute_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/execute/execute_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/execute/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.563773 otter-grader-4.3.2/otter/export/
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.563773 otter-grader-4.3.2/otter/export/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/export/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/export/exporters/base_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.563773 otter-grader-4.3.2/otter/export/exporters/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.563773 otter-grader-4.3.2/otter/export/exporters/templates/via_html/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/export/exporters/templates/via_html/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/export/exporters/templates/via_html/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/export/exporters/templates/via_html.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.563773 otter-grader-4.3.2/otter/export/exporters/templates/via_latex/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/export/exporters/templates/via_latex/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/export/exporters/templates/via_latex/index.tex.j2
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/export/exporters/templates/via_latex.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.563773 otter-grader-4.3.2/otter/export/exporters/templates/via_latex_xecjk/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/export/exporters/templates/via_latex_xecjk/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/export/exporters/templates/via_latex_xecjk.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/export/exporters/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/export/exporters/via_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/export/exporters/via_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/export/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.563773 otter-grader-4.3.2/otter/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.555774 otter-grader-4.3.2/otter/generate/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.563773 otter-grader-4.3.2/otter/generate/templates/python/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/generate/templates/python/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-09 02:12:44.000000 otter-grader-4.3.2/otter/generate/templates/python/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/generate/templates/python/run_autograder
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/generate/templates/python/run_otter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/generate/templates/python/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.567774 otter-grader-4.3.2/otter/generate/templates/r/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/generate/templates/r/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/generate/templates/r/requirements.r
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-09 02:12:44.000000 otter-grader-4.3.2/otter/generate/templates/r/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/generate/templates/r/run_autograder
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/generate/templates/r/run_otter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/generate/templates/r/setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/generate/token.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/generate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.567774 otter-grader-4.3.2/otter/grade/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/grade/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/grade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/grade/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/grade/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.567774 otter-grader-4.3.2/otter/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/plugins/abstract_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.567774 otter-grader-4.3.2/otter/plugins/builtin/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/plugins/builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.567774 otter-grader-4.3.2/otter/plugins/builtin/gmail_notifications/
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/plugins/builtin/gmail_notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.567774 otter-grader-4.3.2/otter/plugins/builtin/gmail_notifications/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/plugins/builtin/gmail_notifications/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/plugins/builtin/grade_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/plugins/builtin/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.567774 otter-grader-4.3.2/otter/run/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.567774 otter-grader-4.3.2/otter/run/run_autograder/
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/run/run_autograder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/run/run_autograder/autograder_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.567774 otter-grader-4.3.2/otter/run/run_autograder/runners/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/run/run_autograder/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/run/run_autograder/runners/abstract_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/run/run_autograder/runners/python_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/run/run_autograder/runners/r_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/run/run_autograder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.567774 otter-grader-4.3.2/otter/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)    15243 2023-04-09 02:12:44.000000 otter-grader-4.3.2/otter/test_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/test_files/abstract_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/test_files/exception_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/test_files/metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/test_files/ok_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/test_files/ottr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-04-09 02:12:01.000000 otter-grader-4.3.2/otter/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-09 02:12:44.000000 otter-grader-4.3.2/otter/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.567774 otter-grader-4.3.2/otter_grader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-04-09 02:12:47.000000 otter-grader-4.3.2/otter_grader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-04-09 02:12:47.000000 otter-grader-4.3.2/otter_grader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 02:12:47.000000 otter-grader-4.3.2/otter_grader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-09 02:12:47.000000 otter-grader-4.3.2/otter_grader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-09 02:12:47.000000 otter-grader-4.3.2/otter_grader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 02:12:47.000000 otter-grader-4.3.2/otter_grader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-09 02:12:01.000000 otter-grader-4.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 02:12:47.571774 otter-grader-4.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-09 02:12:01.000000 otter-grader-4.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.571774 otter-grader-4.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-04-09 02:12:01.000000 otter-grader-4.3.2/test/test_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-09 02:12:01.000000 otter-grader-4.3.2/test/test_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-09 02:12:01.000000 otter-grader-4.3.2/test/test_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:47.571774 otter-grader-4.3.2/test/test_generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 02:12:01.000000 otter-grader-4.3.2/test/test_generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-09 02:12:01.000000 otter-grader-4.3.2/test/test_generate/test_autograder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-09 02:12:01.000000 otter-grader-4.3.2/test/test_generate/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-04-09 02:12:01.000000 otter-grader-4.3.2/test/test_grade.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-09 02:12:01.000000 otter-grader-4.3.2/test/test_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-04-09 02:12:01.000000 otter-grader-4.3.2/test/test_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)    15187 2023-04-09 02:12:01.000000 otter-grader-4.3.2/test/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-09 02:12:01.000000 otter-grader-4.3.2/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.517429 otter-grader-4.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-15 18:37:36.000000 otter-grader-4.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-15 18:37:36.000000 otter-grader-4.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-15 18:38:12.517429 otter-grader-4.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-15 18:37:36.000000 otter-grader-4.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.501429 otter-grader-4.3.3/otter/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.501429 otter-grader-4.3.3/otter/assign/
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-06-15 18:38:07.000000 otter-grader-4.3.3/otter/assign/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-06-15 18:38:07.000000 otter-grader-4.3.3/otter/assign/cell_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/feature_toggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16894 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/notebook_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/question_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.501429 otter-grader-4.3.3/otter/assign/r_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/r_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/r_adapter/cell_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/r_adapter/rmarkdown_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/r_adapter/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/r_adapter/tests_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-06-15 18:38:07.000000 otter-grader-4.3.3/otter/assign/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/tests_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.505429 otter-grader-4.3.3/otter/assign/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/cell_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.505429 otter-grader-4.3.3/otter/assign/v0/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/convert/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/convert/notebook_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/notebook_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/questions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.505429 otter-grader-4.3.3/otter/assign/v0/r_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/r_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/r_adapter/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.505429 otter-grader-4.3.3/otter/assign/v0/rmarkdown_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/rmarkdown_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/rmarkdown_adapter/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/rmarkdown_adapter/notebook_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/rmarkdown_adapter/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/rmarkdown_adapter/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/rmarkdown_adapter/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/rmarkdown_adapter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/assign/v0/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.505429 otter-grader-4.3.3/otter/check/
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17923 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/check/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18909 2023-06-15 18:38:07.000000 otter-grader-4.3.3/otter/check/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/check/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.505429 otter-grader-4.3.3/otter/check/validate_export/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/check/validate_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/check/validate_export/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.505429 otter-grader-4.3.3/otter/execute/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/execute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/execute/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/execute/execute_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/execute/execute_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/execute/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.505429 otter-grader-4.3.3/otter/export/
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.509429 otter-grader-4.3.3/otter/export/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/export/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/export/exporters/base_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.509429 otter-grader-4.3.3/otter/export/exporters/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.509429 otter-grader-4.3.3/otter/export/exporters/templates/via_html/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/export/exporters/templates/via_html/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/export/exporters/templates/via_html/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/export/exporters/templates/via_html.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.509429 otter-grader-4.3.3/otter/export/exporters/templates/via_latex/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/export/exporters/templates/via_latex/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/export/exporters/templates/via_latex/index.tex.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/export/exporters/templates/via_latex.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.509429 otter-grader-4.3.3/otter/export/exporters/templates/via_latex_xecjk/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/export/exporters/templates/via_latex_xecjk/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/export/exporters/templates/via_latex_xecjk.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/export/exporters/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/export/exporters/via_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/export/exporters/via_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/export/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.509429 otter-grader-4.3.3/otter/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.497429 otter-grader-4.3.3/otter/generate/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.509429 otter-grader-4.3.3/otter/generate/templates/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/generate/templates/python/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-15 18:38:07.000000 otter-grader-4.3.3/otter/generate/templates/python/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/generate/templates/python/run_autograder
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/generate/templates/python/run_otter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/generate/templates/python/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.509429 otter-grader-4.3.3/otter/generate/templates/r/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/generate/templates/r/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/generate/templates/r/requirements.r
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-15 18:38:07.000000 otter-grader-4.3.3/otter/generate/templates/r/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/generate/templates/r/run_autograder
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/generate/templates/r/run_otter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/generate/templates/r/setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/generate/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/generate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.509429 otter-grader-4.3.3/otter/grade/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/grade/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/grade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/grade/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/grade/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.513429 otter-grader-4.3.3/otter/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/plugins/abstract_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.513429 otter-grader-4.3.3/otter/plugins/builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/plugins/builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.513429 otter-grader-4.3.3/otter/plugins/builtin/gmail_notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/plugins/builtin/gmail_notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.513429 otter-grader-4.3.3/otter/plugins/builtin/gmail_notifications/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/plugins/builtin/gmail_notifications/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/plugins/builtin/grade_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/plugins/builtin/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.513429 otter-grader-4.3.3/otter/run/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.513429 otter-grader-4.3.3/otter/run/run_autograder/
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/run/run_autograder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/run/run_autograder/autograder_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.513429 otter-grader-4.3.3/otter/run/run_autograder/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/run/run_autograder/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/run/run_autograder/runners/abstract_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/run/run_autograder/runners/python_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/run/run_autograder/runners/r_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/run/run_autograder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.513429 otter-grader-4.3.3/otter/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)    15243 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/test_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/test_files/abstract_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/test_files/exception_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/test_files/metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/test_files/ok_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/test_files/ottr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-06-15 18:37:36.000000 otter-grader-4.3.3/otter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-15 18:38:07.000000 otter-grader-4.3.3/otter/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.513429 otter-grader-4.3.3/otter_grader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-15 18:38:12.000000 otter-grader-4.3.3/otter_grader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-15 18:38:12.000000 otter-grader-4.3.3/otter_grader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 18:38:12.000000 otter-grader-4.3.3/otter_grader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-15 18:38:12.000000 otter-grader-4.3.3/otter_grader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-15 18:38:12.000000 otter-grader-4.3.3/otter_grader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 18:38:12.000000 otter-grader-4.3.3/otter_grader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-15 18:37:36.000000 otter-grader-4.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 18:38:12.517429 otter-grader-4.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-15 18:37:36.000000 otter-grader-4.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.513429 otter-grader-4.3.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-06-15 18:37:36.000000 otter-grader-4.3.3/test/test_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-06-15 18:37:36.000000 otter-grader-4.3.3/test/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-15 18:37:36.000000 otter-grader-4.3.3/test/test_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:38:12.517429 otter-grader-4.3.3/test/test_generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:37:36.000000 otter-grader-4.3.3/test/test_generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-15 18:37:36.000000 otter-grader-4.3.3/test/test_generate/test_autograder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-15 18:37:36.000000 otter-grader-4.3.3/test/test_generate/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-06-15 18:37:36.000000 otter-grader-4.3.3/test/test_grade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-15 18:37:36.000000 otter-grader-4.3.3/test/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-06-15 18:37:36.000000 otter-grader-4.3.3/test/test_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15187 2023-06-15 18:37:36.000000 otter-grader-4.3.3/test/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 18:37:36.000000 otter-grader-4.3.3/test/test_utils.py
```

### Comparing `otter-grader-4.3.2/LICENSE` & `otter-grader-4.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/PKG-INFO` & `otter-grader-4.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-grader
-Version: 4.3.2
+Version: 4.3.3
 Summary: Python and Jupyter Notebook autograder
 Home-page: https://github.com/ucbds-infra/otter-grader
 Author: Christopher Pyles
 Author-email: otter-grader@berkeley.edu
 License: BSD-3-Clause
 Description: # Otter-Grader
```

### Comparing `otter-grader-4.3.2/README.md` & `otter-grader-4.3.3/README.md`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/api.py` & `otter-grader-4.3.3/otter/api.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/__init__.py` & `otter-grader-4.3.3/otter/assign/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/assignment.py` & `otter-grader-4.3.3/otter/assign/assignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,19 @@
         )
 
         run_tests: bool = fica.Key(
             description="whether to run student submissions against local tests during export",
             default=True,
         )
 
+        files: list = fica.Key(
+            description="a list of other files to include in the student submissions' zip file",
+            default=[],
+        )
+
     export_cell: ExportCellValue = fica.Key(
         description="whether to include an Otter export cell in the output notebooks",
         subkey_container=ExportCellValue,
     )
 
     class SeedValue(fica.Config):
```

### Comparing `otter-grader-4.3.2/otter/assign/blocks.py` & `otter-grader-4.3.3/otter/assign/blocks.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/cell_factory.py` & `otter-grader-4.3.3/otter/assign/cell_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,16 @@
             args += ["filtering=False"]
         if not self.assignment.export_cell.pdf:
             args += ["pdf=False"]
         if self.assignment.export_cell.force_save:
             args += ["force_save=True"]
         if self.assignment.export_cell.run_tests:
             args += ["run_tests=True"]
-
+        if len(self.assignment.export_cell.files) != 0:
+            args += [f"files={self.assignment.export_cell.files}"]
         source_lines.append(f"grader.export({', '.join(args)})")
         export.source = "\n".join(source_lines)
 
         lock(instructions)
         lock(export)
 
         cells = [instructions, export]
```

### Comparing `otter-grader-4.3.2/otter/assign/feature_toggle.py` & `otter-grader-4.3.3/otter/assign/feature_toggle.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/notebook_transformer.py` & `otter-grader-4.3.3/otter/assign/notebook_transformer.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/output.py` & `otter-grader-4.3.3/otter/assign/output.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/plugins.py` & `otter-grader-4.3.3/otter/assign/plugins.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/question_config.py` & `otter-grader-4.3.3/otter/assign/question_config.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/r_adapter/cell_factory.py` & `otter-grader-4.3.3/otter/assign/r_adapter/cell_factory.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/r_adapter/rmarkdown_converter.py` & `otter-grader-4.3.3/otter/assign/r_adapter/rmarkdown_converter.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/r_adapter/solutions.py` & `otter-grader-4.3.3/otter/assign/r_adapter/solutions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/r_adapter/tests_manager.py` & `otter-grader-4.3.3/otter/assign/r_adapter/tests_manager.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/solutions.py` & `otter-grader-4.3.3/otter/assign/solutions.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             match = re.match(fr"(\s*){seed_variable}\s*(=|<-)\s*", line)
             if  match:
                 source[i] = match.group(1) + f"{seed_variable} {match.group(2)} {seed}"
         cell["source"] = "\n".join(source)
     return nb
 
 
-solution_assignment_regex = re.compile(r"(\s*(?:[\w.]+(?:\[['\"].*['\"]\])*(?:,\s*)?)+\s*=).* ?# ?SOLUTION")
+solution_assignment_regex = re.compile(r"(\s*(?:[\w.]+(?=[^\w.])(?:\[['\"]?.*['\"]?\])*(?:,\s*)?)+\s*=).* ?# ?SOLUTION")
 def solution_assignment_sub(match):
     """
     Substitutes the first matching group  with `` ...``
     """
     prefix = match.group(1)
     return prefix + ' ...'
```

### Comparing `otter-grader-4.3.2/otter/assign/tests_manager.py` & `otter-grader-4.3.3/otter/assign/tests_manager.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/utils.py` & `otter-grader-4.3.3/otter/assign/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/v0/__init__.py` & `otter-grader-4.3.3/otter/assign/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/v0/assignment.py` & `otter-grader-4.3.3/otter/assign/v0/assignment.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/v0/cell_generators.py` & `otter-grader-4.3.3/otter/assign/v0/cell_generators.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/v0/constants.py` & `otter-grader-4.3.3/otter/assign/v0/constants.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/v0/convert/__main__.py` & `otter-grader-4.3.3/otter/assign/v0/convert/__main__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/v0/convert/notebook_transformer.py` & `otter-grader-4.3.3/otter/assign/v0/convert/notebook_transformer.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/v0/notebook_transformer.py` & `otter-grader-4.3.3/otter/assign/v0/notebook_transformer.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/v0/output.py` & `otter-grader-4.3.3/otter/assign/v0/output.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/v0/plugins.py` & `otter-grader-4.3.3/otter/assign/v0/plugins.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/v0/questions.py` & `otter-grader-4.3.3/otter/assign/v0/questions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/v0/r_adapter/tests.py` & `otter-grader-4.3.3/otter/assign/v0/r_adapter/tests.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/v0/rmarkdown_adapter/notebook_transformer.py` & `otter-grader-4.3.3/otter/assign/v0/rmarkdown_adapter/notebook_transformer.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/v0/rmarkdown_adapter/output.py` & `otter-grader-4.3.3/otter/assign/v0/rmarkdown_adapter/output.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/v0/rmarkdown_adapter/solutions.py` & `otter-grader-4.3.3/otter/assign/v0/rmarkdown_adapter/solutions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/v0/rmarkdown_adapter/tests.py` & `otter-grader-4.3.3/otter/assign/v0/rmarkdown_adapter/tests.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/v0/rmarkdown_adapter/utils.py` & `otter-grader-4.3.3/otter/assign/v0/rmarkdown_adapter/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/v0/solutions.py` & `otter-grader-4.3.3/otter/assign/v0/solutions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/v0/tests.py` & `otter-grader-4.3.3/otter/assign/v0/tests.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/assign/v0/utils.py` & `otter-grader-4.3.3/otter/assign/v0/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/check/__init__.py` & `otter-grader-4.3.3/otter/check/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/check/logs.py` & `otter-grader-4.3.3/otter/check/logs.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/check/notebook.py` & `otter-grader-4.3.3/otter/check/notebook.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from contextlib import contextmanager
 from glob import glob
 from IPython.display import display, HTML
 from textwrap import indent
 
 from .logs import LogEntry, EventType, Log
 from .utils import grade_zip_file, grading_mode_disabled, incompatible_with, IPythonInterpreter, \
-     list_available_tests, logs_event, resolve_test_info, save_notebook
+    list_available_tests, logs_event, resolve_test_info, save_notebook
 
 from ..execute import Checker
 from ..export import export_notebook
 from ..plugins import PluginCollection
 from ..test_files import GradingResults
 from ..utils import Loggable, loggers
 
@@ -397,15 +397,20 @@
             if len(dot_otter) != 1:
                 raise ValueError("Too many .otter files (max 1 allowed)")
             dot_otter = dot_otter[0]
             zf.write(dot_otter)
             self._logger.debug(f"Added .otter file to zip file: {dot_otter}")
 
         for file in files:
-            zf.write(file)
+            if os.path.isdir(file):
+                sub_files = glob(f"./{file}/**/*.*")
+                for sub_file in sub_files:
+                    zf.write(sub_file)
+            else:
+                zf.write(file)
             self._logger.debug(f"Added file to zip file: {file}")
 
         for file in self._addl_files:
             zf.write(file)
             self._logger.debug(f"Added plugin file to zip file: {file}")
 
         zf.close()
```

### Comparing `otter-grader-4.3.2/otter/check/utils.py` & `otter-grader-4.3.3/otter/check/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/check/validate_export/__main__.py` & `otter-grader-4.3.3/otter/check/validate_export/__main__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/cli.py` & `otter-grader-4.3.3/otter/cli.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/execute/__init__.py` & `otter-grader-4.3.3/otter/execute/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/execute/checker.py` & `otter-grader-4.3.3/otter/execute/checker.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/execute/execute_log.py` & `otter-grader-4.3.3/otter/execute/execute_log.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/execute/execute_notebook.py` & `otter-grader-4.3.3/otter/execute/execute_notebook.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/execute/transforms.py` & `otter-grader-4.3.3/otter/execute/transforms.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/export/__init__.py` & `otter-grader-4.3.3/otter/export/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/export/exporters/__init__.py` & `otter-grader-4.3.3/otter/export/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/export/exporters/base_exporter.py` & `otter-grader-4.3.3/otter/export/exporters/base_exporter.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/export/exporters/templates/via_html/index.html.j2` & `otter-grader-4.3.3/otter/export/exporters/templates/via_html/index.html.j2`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/export/exporters/templates/via_html.tpl` & `otter-grader-4.3.3/otter/export/exporters/templates/via_html.tpl`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/export/exporters/templates/via_latex/index.tex.j2` & `otter-grader-4.3.3/otter/export/exporters/templates/via_latex/index.tex.j2`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/export/exporters/templates/via_latex.tpl` & `otter-grader-4.3.3/otter/export/exporters/templates/via_latex.tpl`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2` & `otter-grader-4.3.3/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/export/exporters/templates/via_latex_xecjk.tpl` & `otter-grader-4.3.3/otter/export/exporters/templates/via_latex_xecjk.tpl`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/export/exporters/utils.py` & `otter-grader-4.3.3/otter/export/exporters/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/export/exporters/via_html.py` & `otter-grader-4.3.3/otter/export/exporters/via_html.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/export/exporters/via_latex.py` & `otter-grader-4.3.3/otter/export/exporters/via_latex.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/generate/__init__.py` & `otter-grader-4.3.3/otter/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/generate/templates/python/setup.sh` & `otter-grader-4.3.3/otter/generate/templates/python/setup.sh`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/generate/templates/r/setup.sh` & `otter-grader-4.3.3/otter/generate/templates/r/setup.sh`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/generate/token.py` & `otter-grader-4.3.3/otter/generate/token.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/generate/utils.py` & `otter-grader-4.3.3/otter/generate/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/grade/Dockerfile` & `otter-grader-4.3.3/otter/grade/Dockerfile`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/grade/__init__.py` & `otter-grader-4.3.3/otter/grade/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/grade/containers.py` & `otter-grader-4.3.3/otter/grade/containers.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/grade/utils.py` & `otter-grader-4.3.3/otter/grade/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/plugins/__init__.py` & `otter-grader-4.3.3/otter/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/plugins/abstract_plugin.py` & `otter-grader-4.3.3/otter/plugins/abstract_plugin.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/plugins/builtin/gmail_notifications/__init__.py` & `otter-grader-4.3.3/otter/plugins/builtin/gmail_notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py` & `otter-grader-4.3.3/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/plugins/builtin/grade_override.py` & `otter-grader-4.3.3/otter/plugins/builtin/grade_override.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/plugins/builtin/rate_limiting.py` & `otter-grader-4.3.3/otter/plugins/builtin/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/run/__init__.py` & `otter-grader-4.3.3/otter/run/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/run/run_autograder/__init__.py` & `otter-grader-4.3.3/otter/run/run_autograder/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/run/run_autograder/autograder_config.py` & `otter-grader-4.3.3/otter/run/run_autograder/autograder_config.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/run/run_autograder/runners/__init__.py` & `otter-grader-4.3.3/otter/run/run_autograder/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/run/run_autograder/runners/abstract_runner.py` & `otter-grader-4.3.3/otter/run/run_autograder/runners/abstract_runner.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/run/run_autograder/runners/python_runner.py` & `otter-grader-4.3.3/otter/run/run_autograder/runners/python_runner.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/run/run_autograder/runners/r_runner.py` & `otter-grader-4.3.3/otter/run/run_autograder/runners/r_runner.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/test_files/__init__.py` & `otter-grader-4.3.3/otter/test_files/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/test_files/abstract_test.py` & `otter-grader-4.3.3/otter/test_files/abstract_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/test_files/exception_test.py` & `otter-grader-4.3.3/otter/test_files/exception_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/test_files/metadata_test.py` & `otter-grader-4.3.3/otter/test_files/metadata_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/test_files/ok_test.py` & `otter-grader-4.3.3/otter/test_files/ok_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/utils.py` & `otter-grader-4.3.3/otter/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/otter/version.py` & `otter-grader-4.3.3/otter/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Version and printable logo"""
 
 import sys
 
 from textwrap import dedent
 
 
-__version__ = "4.3.2"
+__version__ = "4.3.3"
 
 
 LOGO_WITH_VERSION = fr"""
   _________        __          __               
  /  _____  \    __|  |__    __|  |__               
 |  /     \  |  |__    __|  |__    __|   _______    _  _____
 | |       | |     |  |        |  |     |  ___  |  | |/ ____|
```

### Comparing `otter-grader-4.3.2/otter_grader.egg-info/PKG-INFO` & `otter-grader-4.3.3/otter_grader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-grader
-Version: 4.3.2
+Version: 4.3.3
 Summary: Python and Jupyter Notebook autograder
 Home-page: https://github.com/ucbds-infra/otter-grader
 Author: Christopher Pyles
 Author-email: otter-grader@berkeley.edu
 License: BSD-3-Clause
 Description: # Otter-Grader
```

### Comparing `otter-grader-4.3.2/otter_grader.egg-info/SOURCES.txt` & `otter-grader-4.3.3/otter_grader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/setup.py` & `otter-grader-4.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/test/test_assign.py` & `otter-grader-4.3.3/test/test_assign.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/test/test_check.py` & `otter-grader-4.3.3/test/test_check.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/test/test_export.py` & `otter-grader-4.3.3/test/test_export.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/test/test_generate/test_autograder.py` & `otter-grader-4.3.3/test/test_generate/test_autograder.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/test/test_generate/test_token.py` & `otter-grader-4.3.3/test/test_generate/test_token.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/test/test_grade.py` & `otter-grader-4.3.3/test/test_grade.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/test/test_logs.py` & `otter-grader-4.3.3/test/test_logs.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/test/test_notebook.py` & `otter-grader-4.3.3/test/test_notebook.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.2/test/test_run.py` & `otter-grader-4.3.3/test/test_run.py`

 * *Files identical despite different names*

