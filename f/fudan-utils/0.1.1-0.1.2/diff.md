# Comparing `tmp/fudan_utils-0.1.1.tar.gz` & `tmp/fudan_utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fudan_utils-0.1.1.tar", max compression
+gzip compressed data, was "fudan_utils-0.1.2.tar", max compression
```

## Comparing `fudan_utils-0.1.1.tar` & `fudan_utils-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-15 05:20:31.973091 fudan_utils-0.1.1/README.md
--rw-r--r--   0        0        0       21 2023-06-15 05:23:23.015942 fudan_utils-0.1.1/fudan_utils/__init__.py
--rw-r--r--   0        0        0      649 2023-06-15 05:23:23.014507 fudan_utils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 fudan_utils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-15 05:20:31.973091 fudan_utils-0.1.2/README.md
+-rw-r--r--   0        0        0       21 2023-06-15 06:27:07.665899 fudan_utils-0.1.2/fudan_utils/__init__.py
+-rw-r--r--   0        0        0       77 2023-06-15 06:07:40.832259 fudan_utils-0.1.2/fudan_utils/config.py
+-rw-r--r--   0        0        0     7703 2023-06-15 06:26:16.496167 fudan_utils-0.1.2/fudan_utils/fudan.py
+-rwxr-xr-x   0        0        0     1122 2023-06-15 06:26:37.079823 fudan_utils-0.1.2/fudan_utils/fudan_grades.py
+-rw-r--r--   0        0        0      963 2023-06-15 06:27:07.664055 fudan_utils-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 fudan_utils-0.1.2/PKG-INFO
```

