# Comparing `tmp/datadog-sma-0.1.0.tar.gz` & `tmp/datadog-sma-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadog-sma-0.1.0.tar", last modified: Fri May  5 18:24:48 2023, max compression
+gzip compressed data, was "datadog-sma-0.2.0.tar", last modified: Thu Jun 15 19:08:48 2023, max compression
```

## Comparing `datadog-sma-0.1.0.tar` & `datadog-sma-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:24:48.041310 datadog-sma-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-05 18:24:48.037310 datadog-sma-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 18:24:38.000000 datadog-sma-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 18:24:48.041310 datadog-sma-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:24:48.033310 datadog-sma-0.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:24:34.000000 datadog-sma-0.1.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:24:48.033310 datadog-sma-0.1.0/src/datadog-serverless-agent-linux-amd64/
--rwxr-xr-x   0 runner    (1001) docker     (123)   968564 2023-05-05 18:24:38.000000 datadog-sma-0.1.0/src/datadog-serverless-agent-linux-amd64/datadog-serverless-trace-mini-agent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:24:48.037310 datadog-sma-0.1.0/src/datadog-serverless-agent-windows-amd64/
--rwxr-xr-x   0 runner    (1001) docker     (123)   947200 2023-05-05 18:24:38.000000 datadog-sma-0.1.0/src/datadog-serverless-agent-windows-amd64/datadog-serverless-trace-mini-agent.exe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:24:48.037310 datadog-sma-0.1.0/src/datadog_sma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-05 18:24:48.000000 datadog-sma-0.1.0/src/datadog_sma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-05 18:24:48.000000 datadog-sma-0.1.0/src/datadog_sma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:24:48.000000 datadog-sma-0.1.0/src/datadog_sma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-05 18:24:48.000000 datadog-sma-0.1.0/src/datadog_sma.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:08:48.861847 datadog-sma-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-15 19:08:48.861847 datadog-sma-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-15 19:08:41.000000 datadog-sma-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 19:08:48.861847 datadog-sma-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:08:48.857848 datadog-sma-0.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:08:32.000000 datadog-sma-0.2.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:08:48.857848 datadog-sma-0.2.0/src/datadog-serverless-agent-linux-amd64/
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1015076 2023-06-15 19:08:41.000000 datadog-sma-0.2.0/src/datadog-serverless-agent-linux-amd64/datadog-serverless-trace-mini-agent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:08:48.861847 datadog-sma-0.2.0/src/datadog-serverless-agent-windows-amd64/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   948224 2023-06-15 19:08:41.000000 datadog-sma-0.2.0/src/datadog-serverless-agent-windows-amd64/datadog-serverless-trace-mini-agent.exe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:08:48.861847 datadog-sma-0.2.0/src/datadog_sma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-15 19:08:48.000000 datadog-sma-0.2.0/src/datadog_sma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-15 19:08:48.000000 datadog-sma-0.2.0/src/datadog_sma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:08:48.000000 datadog-sma-0.2.0/src/datadog_sma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-15 19:08:48.000000 datadog-sma-0.2.0/src/datadog_sma.egg-info/top_level.txt
```

