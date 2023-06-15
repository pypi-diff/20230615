# Comparing `tmp/finops-0.0.2.tar.gz` & `tmp/finops-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finops-0.0.2.tar", last modified: Thu Jun 15 16:25:59 2023, max compression
+gzip compressed data, was "finops-0.0.3.tar", last modified: Thu Jun 15 19:32:18 2023, max compression
```

## Comparing `finops-0.0.2.tar` & `finops-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:25:59.005511 finops-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-15 16:25:46.000000 finops-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-15 16:25:59.005511 finops-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 16:25:46.000000 finops-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-15 16:25:46.000000 finops-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:25:59.005511 finops-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:25:59.001511 finops-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:25:59.001511 finops-0.0.2/src/finops/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:25:46.000000 finops-0.0.2/src/finops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 16:25:46.000000 finops-0.0.2/src/finops/shareholders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:25:59.005511 finops-0.0.2/src/finops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-15 16:25:58.000000 finops-0.0.2/src/finops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-15 16:25:58.000000 finops-0.0.2/src/finops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:25:58.000000 finops-0.0.2/src/finops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 16:25:58.000000 finops-0.0.2/src/finops.egg-info/top_level.txt
+drwxrwxr-x   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 19:32:18.519399 finops-0.0.3/
+-rw-rw-r--   0 nixuri    (1000) nixuri    (1000)     1544 2023-06-15 19:06:45.000000 finops-0.0.3/LICENSE
+-rw-rw-r--   0 nixuri    (1000) nixuri    (1000)      637 2023-06-15 19:32:18.519399 finops-0.0.3/PKG-INFO
+-rw-rw-r--   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 19:08:19.000000 finops-0.0.3/README.md
+drwxrwxr-x   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 19:32:18.519399 finops-0.0.3/finops/
+-rw-rw-r--   0 nixuri    (1000) nixuri    (1000)        0 2023-06-05 14:53:44.000000 finops-0.0.3/finops/__init__.py
+drwxrwxr-x   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 19:32:18.519399 finops-0.0.3/finops/data/
+-rw-rw-r--   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 17:23:36.000000 finops-0.0.3/finops/data/__init__.py
+-rw-rw-r--   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 17:23:22.000000 finops-0.0.3/finops/data/shareholders.py
+drwxrwxr-x   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 19:32:18.519399 finops-0.0.3/finops.egg-info/
+-rw-rw-r--   0 nixuri    (1000) nixuri    (1000)      637 2023-06-15 19:32:18.000000 finops-0.0.3/finops.egg-info/PKG-INFO
+-rw-rw-r--   0 nixuri    (1000) nixuri    (1000)      291 2023-06-15 19:32:18.000000 finops-0.0.3/finops.egg-info/SOURCES.txt
+-rw-rw-r--   0 nixuri    (1000) nixuri    (1000)        1 2023-06-15 19:32:18.000000 finops-0.0.3/finops.egg-info/dependency_links.txt
+-rw-rw-r--   0 nixuri    (1000) nixuri    (1000)       13 2023-06-15 19:32:18.000000 finops-0.0.3/finops.egg-info/requires.txt
+-rw-rw-r--   0 nixuri    (1000) nixuri    (1000)       13 2023-06-15 19:32:18.000000 finops-0.0.3/finops.egg-info/top_level.txt
+-rw-rw-r--   0 nixuri    (1000) nixuri    (1000)       38 2023-06-15 19:32:18.519399 finops-0.0.3/setup.cfg
+-rw-rw-r--   0 nixuri    (1000) nixuri    (1000)      798 2023-06-15 19:27:54.000000 finops-0.0.3/setup.py
+drwxrwxr-x   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 19:32:18.519399 finops-0.0.3/tests/
+-rw-rw-r--   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 17:23:45.000000 finops-0.0.3/tests/__init__.py
+-rw-rw-r--   0 nixuri    (1000) nixuri    (1000)        0 2023-06-15 17:24:10.000000 finops-0.0.3/tests/test_shareholders.py
```

