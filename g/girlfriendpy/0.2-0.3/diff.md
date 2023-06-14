# Comparing `tmp/girlfriendpy-0.2.tar.gz` & `tmp/girlfriendpy-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girlfriendpy-0.2.tar", last modified: Wed Jun 14 23:05:10 2023, max compression
+gzip compressed data, was "girlfriendpy-0.3.tar", last modified: Wed Jun 14 23:12:55 2023, max compression
```

## Comparing `girlfriendpy-0.2.tar` & `girlfriendpy-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 23:05:10.126281 girlfriendpy-0.2/
--rw-rw-rw-   0        0        0      181 2023-06-14 23:05:10.108292 girlfriendpy-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      646 2023-06-14 23:02:13.000000 girlfriendpy-0.2/README.md
--rw-rw-rw-   0        0        0        9 2023-06-14 22:44:08.000000 girlfriendpy-0.2/gf.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:05:10.105293 girlfriendpy-0.2/girlfriendpy.egg-info/
--rw-rw-rw-   0        0        0      181 2023-06-14 23:05:09.000000 girlfriendpy-0.2/girlfriendpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-06-14 23:05:09.000000 girlfriendpy-0.2/girlfriendpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 23:05:09.000000 girlfriendpy-0.2/girlfriendpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2023-06-14 23:05:09.000000 girlfriendpy-0.2/girlfriendpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 23:05:10.127279 girlfriendpy-0.2/setup.cfg
--rw-rw-rw-   0        0        0      280 2023-06-14 23:03:31.000000 girlfriendpy-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:12:55.532972 girlfriendpy-0.3/
+-rw-rw-rw-   0        0        0      872 2023-06-14 23:12:55.508986 girlfriendpy-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      646 2023-06-14 23:02:13.000000 girlfriendpy-0.3/README.md
+-rw-rw-rw-   0        0        0        9 2023-06-14 22:44:08.000000 girlfriendpy-0.3/gf.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:12:55.505475 girlfriendpy-0.3/girlfriendpy.egg-info/
+-rw-rw-rw-   0        0        0      872 2023-06-14 23:12:54.000000 girlfriendpy-0.3/girlfriendpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-06-14 23:12:55.000000 girlfriendpy-0.3/girlfriendpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 23:12:54.000000 girlfriendpy-0.3/girlfriendpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2023-06-14 23:12:54.000000 girlfriendpy-0.3/girlfriendpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 23:12:55.532972 girlfriendpy-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      463 2023-06-14 23:12:49.000000 girlfriendpy-0.3/setup.py
```

### Comparing `girlfriendpy-0.2/README.md` & `girlfriendpy-0.3/README.md`

 * *Files identical despite different names*

