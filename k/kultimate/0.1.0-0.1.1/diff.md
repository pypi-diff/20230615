# Comparing `tmp/kultimate-0.1.0.tar.gz` & `tmp/kultimate-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kultimate-0.1.0.tar", max compression
+gzip compressed data, was "kultimate-0.1.1.tar", max compression
```

## Comparing `kultimate-0.1.0.tar` & `kultimate-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,19 @@
--rw-r--r--   0        0        0        0 2023-06-01 23:06:52.117595 kultimate-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-01 23:06:52.117595 kultimate-0.1.0/kultimate/__init__.py
--rw-r--r--   0        0        0      408 2023-06-01 23:29:42.327625 kultimate-0.1.0/kultimate/app.py
--rw-r--r--   0        0        0       23 2023-06-01 23:29:28.820958 kultimate-0.1.0/kultimate/screens/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 23:21:10.614281 kultimate-0.1.0/kultimate/screens/file_select.py
--rw-r--r--   0        0        0      439 2023-06-01 23:31:06.960960 kultimate-0.1.0/kultimate/screens/main.py
--rw-r--r--   0        0        0      396 2023-06-01 23:11:01.307601 kultimate-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      410 1970-01-01 00:00:00.000000 kultimate-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1820 2023-06-14 22:51:45.896608 kultimate-0.1.1/README.md
+-rw-r--r--   0        0        0       22 2023-06-05 20:11:41.877983 kultimate-0.1.1/kultimate/__init__.py
+-rw-r--r--   0        0        0     1405 2023-06-14 18:50:13.597219 kultimate-0.1.1/kultimate/app.css
+-rw-r--r--   0        0        0    18118 2023-06-14 21:37:13.313178 kultimate-0.1.1/kultimate/app.py
+-rw-r--r--   0        0        0       64 2023-06-14 18:50:13.597219 kultimate-0.1.1/kultimate/screens/__init__.py
+-rw-r--r--   0        0        0      896 2023-06-14 18:50:13.597219 kultimate-0.1.1/kultimate/screens/addTask.py
+-rw-r--r--   0        0        0      988 2023-06-14 16:24:13.233698 kultimate-0.1.1/kultimate/screens/deleteTask.py
+-rw-r--r--   0        0        0      125 2023-06-09 21:48:51.262790 kultimate-0.1.1/kultimate/utils/__init__.py
+-rw-r--r--   0        0        0     2068 2023-06-12 23:04:04.110731 kultimate-0.1.1/kultimate/utils/app_config.py
+-rw-r--r--   0        0        0     2043 2023-06-14 21:37:13.313178 kultimate-0.1.1/kultimate/utils/html_to_markdown.py
+-rw-r--r--   0        0        0     2417 2023-06-14 21:37:13.313178 kultimate-0.1.1/kultimate/utils/parser_html.py
+-rw-r--r--   0        0        0     1084 2023-06-02 22:13:35.823860 kultimate-0.1.1/kultimate/utils/process_yaml.py
+-rw-r--r--   0        0        0      127 2023-06-07 23:20:48.314373 kultimate-0.1.1/kultimate/widgets/__init__.py
+-rw-r--r--   0        0        0      620 2023-06-09 21:48:51.266124 kultimate-0.1.1/kultimate/widgets/directory.py
+-rw-r--r--   0        0        0      426 2023-06-07 21:05:08.384197 kultimate-0.1.1/kultimate/widgets/stages.py
+-rw-r--r--   0        0        0      122 2023-06-07 21:03:56.964196 kultimate-0.1.1/kultimate/widgets/stagesContainer.py
+-rw-r--r--   0        0        0      136 2023-06-09 19:45:57.286316 kultimate-0.1.1/kultimate/widgets/task.py
+-rw-r--r--   0        0        0      606 2023-06-14 22:55:37.839947 kultimate-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2447 1970-01-01 00:00:00.000000 kultimate-0.1.1/PKG-INFO
```

