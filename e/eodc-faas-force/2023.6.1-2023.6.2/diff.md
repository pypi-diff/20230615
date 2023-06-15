# Comparing `tmp/eodc_faas_force-2023.6.1.tar.gz` & `tmp/eodc_faas_force-2023.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc_faas_force-2023.6.1.tar", max compression
+gzip compressed data, was "eodc_faas_force-2023.6.2.tar", max compression
```

## Comparing `eodc_faas_force-2023.6.1.tar` & `eodc_faas_force-2023.6.2.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0       24 2023-05-04 07:19:47.659253 eodc_faas_force-2023.6.1/README.md
--rw-r--r--   0        0        0       93 2023-06-02 12:10:30.023253 eodc_faas_force-2023.6.1/force_processor_bindings/__init__.py
--rw-r--r--   0        0        0     1907 2023-05-30 18:55:22.703253 eodc_faas_force-2023.6.1/force_processor_bindings/model.py
--rw-r--r--   0        0        0     4754 2023-05-23 08:18:00.179253 eodc_faas_force-2023.6.1/force_processor_bindings/workflows.py
--rw-r--r--   0        0        0      692 2023-06-02 12:10:30.023253 eodc_faas_force-2023.6.1/pyproject.toml
--rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 eodc_faas_force-2023.6.1/PKG-INFO
+-rw-r--r--   0        0        0       24 2023-05-04 07:19:47.663253 eodc_faas_force-2023.6.2/README.md
+-rw-r--r--   0        0        0       93 2023-06-15 09:56:41.391253 eodc_faas_force-2023.6.2/force_processor_bindings/__init__.py
+-rw-r--r--   0        0        0     2952 2023-06-15 09:39:13.387253 eodc_faas_force-2023.6.2/force_processor_bindings/model.py
+-rw-r--r--   0        0        0      610 2023-06-15 09:56:41.391253 eodc_faas_force-2023.6.2/pyproject.toml
+-rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 eodc_faas_force-2023.6.2/PKG-INFO
```

