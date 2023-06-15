# Comparing `tmp/deviceID-0.1.3.tar.gz` & `tmp/deviceID-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deviceID-0.1.3.tar", last modified: Wed Jun 14 14:31:04 2023, max compression
+gzip compressed data, was "deviceID-0.1.4.tar", last modified: Thu Jun 15 14:23:37 2023, max compression
```

## Comparing `deviceID-0.1.3.tar` & `deviceID-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:31:04.092250 deviceID-0.1.3/
--rw-r--r--   0 root         (0) root         (0)      161 2023-06-14 14:31:04.092250 deviceID-0.1.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-14 07:31:10.000000 deviceID-0.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:31:04.092250 deviceID-0.1.3/deviceID/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-14 07:31:55.000000 deviceID-0.1.3/deviceID/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5172 2023-06-14 14:27:46.000000 deviceID-0.1.3/deviceID/deviceID.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:31:04.092250 deviceID-0.1.3/deviceID.egg-info/
--rw-rw-r--   0 root         (0) root         (0)      161 2023-06-14 14:31:04.000000 deviceID-0.1.3/deviceID.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      211 2023-06-14 14:31:04.000000 deviceID-0.1.3/deviceID.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-06-14 14:31:04.000000 deviceID-0.1.3/deviceID.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)        9 2023-06-14 14:31:04.000000 deviceID-0.1.3/deviceID.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 14:31:04.092250 deviceID-0.1.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      347 2023-06-14 14:31:00.000000 deviceID-0.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:31:04.092250 deviceID-0.1.3/tests/
--rw-rw-r--   0 root         (0) root         (0)       69 2023-06-14 08:04:52.000000 deviceID-0.1.3/tests/test_deviceID.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:23:37.600656 deviceID-0.1.4/
+-rw-r--r--   0 root         (0) root         (0)      161 2023-06-15 14:23:37.600656 deviceID-0.1.4/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-14 07:31:10.000000 deviceID-0.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:23:37.600656 deviceID-0.1.4/deviceID/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-14 07:31:55.000000 deviceID-0.1.4/deviceID/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6672 2023-06-15 14:21:08.000000 deviceID-0.1.4/deviceID/deviceID.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:23:37.600656 deviceID-0.1.4/deviceID.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)      161 2023-06-15 14:23:37.000000 deviceID-0.1.4/deviceID.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      242 2023-06-15 14:23:37.000000 deviceID-0.1.4/deviceID.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-06-15 14:23:37.000000 deviceID-0.1.4/deviceID.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-15 14:23:37.000000 deviceID-0.1.4/deviceID.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)        9 2023-06-15 14:23:37.000000 deviceID-0.1.4/deviceID.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 14:23:37.600656 deviceID-0.1.4/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      367 2023-06-15 14:23:35.000000 deviceID-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:23:37.600656 deviceID-0.1.4/tests/
+-rw-rw-r--   0 root         (0) root         (0)       69 2023-06-14 08:04:52.000000 deviceID-0.1.4/tests/test_deviceID.py
```

