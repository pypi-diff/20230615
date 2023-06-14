# Comparing `tmp/girlfriendpy-0.1.tar.gz` & `tmp/girlfriendpy-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girlfriendpy-0.1.tar", last modified: Wed Jun 14 22:52:55 2023, max compression
+gzip compressed data, was "girlfriendpy-0.2.tar", last modified: Wed Jun 14 23:05:10 2023, max compression
```

## Comparing `girlfriendpy-0.1.tar` & `girlfriendpy-0.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 22:52:55.310602 girlfriendpy-0.1/
--rw-rw-rw-   0        0        0      181 2023-06-14 22:52:55.273626 girlfriendpy-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-06-14 22:44:08.000000 girlfriendpy-0.1/gf.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:52:55.232735 girlfriendpy-0.1/girlfriendpy.egg-info/
--rw-rw-rw-   0        0        0      181 2023-06-14 22:52:54.000000 girlfriendpy-0.1/girlfriendpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-06-14 22:52:54.000000 girlfriendpy-0.1/girlfriendpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 22:52:54.000000 girlfriendpy-0.1/girlfriendpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2023-06-14 22:52:54.000000 girlfriendpy-0.1/girlfriendpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 22:52:55.310602 girlfriendpy-0.1/setup.cfg
--rw-rw-rw-   0        0        0      280 2023-06-14 22:52:21.000000 girlfriendpy-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:05:10.126281 girlfriendpy-0.2/
+-rw-rw-rw-   0        0        0      181 2023-06-14 23:05:10.108292 girlfriendpy-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      646 2023-06-14 23:02:13.000000 girlfriendpy-0.2/README.md
+-rw-rw-rw-   0        0        0        9 2023-06-14 22:44:08.000000 girlfriendpy-0.2/gf.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:05:10.105293 girlfriendpy-0.2/girlfriendpy.egg-info/
+-rw-rw-rw-   0        0        0      181 2023-06-14 23:05:09.000000 girlfriendpy-0.2/girlfriendpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-06-14 23:05:09.000000 girlfriendpy-0.2/girlfriendpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 23:05:09.000000 girlfriendpy-0.2/girlfriendpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2023-06-14 23:05:09.000000 girlfriendpy-0.2/girlfriendpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 23:05:10.127279 girlfriendpy-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      280 2023-06-14 23:03:31.000000 girlfriendpy-0.2/setup.py
```

