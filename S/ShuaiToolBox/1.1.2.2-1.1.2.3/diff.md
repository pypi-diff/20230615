# Comparing `tmp/ShuaiToolBox-1.1.2.2.tar.gz` & `tmp/ShuaiToolBox-1.1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ShuaiToolBox-1.1.2.2.tar", last modified: Thu Jun 15 15:22:48 2023, max compression
+gzip compressed data, was "dist\ShuaiToolBox-1.1.2.3.tar", last modified: Thu Jun 15 15:23:06 2023, max compression
```

## Comparing `ShuaiToolBox-1.1.2.2.tar` & `ShuaiToolBox-1.1.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 15:22:48.000000 ShuaiToolBox-1.1.2.2/
--rw-rw-rw-   0        0        0      223 2023-06-15 15:22:48.000000 ShuaiToolBox-1.1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-13 06:20:27.000000 ShuaiToolBox-1.1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 15:22:48.000000 ShuaiToolBox-1.1.2.2/ShuaiToolBox/
--rw-rw-rw-   0        0        0      187 2023-06-13 09:22:13.000000 ShuaiToolBox-1.1.2.2/ShuaiToolBox/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:22:48.000000 ShuaiToolBox-1.1.2.2/ShuaiToolBox.egg-info/
--rw-rw-rw-   0        0        0      223 2023-06-15 15:22:48.000000 ShuaiToolBox-1.1.2.2/ShuaiToolBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-06-15 15:22:48.000000 ShuaiToolBox-1.1.2.2/ShuaiToolBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 15:22:48.000000 ShuaiToolBox-1.1.2.2/ShuaiToolBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-06-15 15:22:48.000000 ShuaiToolBox-1.1.2.2/ShuaiToolBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-15 15:22:48.000000 ShuaiToolBox-1.1.2.2/ShuaiToolBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 15:22:48.000000 ShuaiToolBox-1.1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      413 2023-06-14 02:43:11.000000 ShuaiToolBox-1.1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:23:06.000000 ShuaiToolBox-1.1.2.3/
+-rw-rw-rw-   0        0        0      223 2023-06-15 15:23:06.000000 ShuaiToolBox-1.1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-13 06:20:27.000000 ShuaiToolBox-1.1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 15:23:06.000000 ShuaiToolBox-1.1.2.3/ShuaiToolBox/
+-rw-rw-rw-   0        0        0      187 2023-06-13 09:22:13.000000 ShuaiToolBox-1.1.2.3/ShuaiToolBox/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:23:06.000000 ShuaiToolBox-1.1.2.3/ShuaiToolBox.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-06-15 15:23:06.000000 ShuaiToolBox-1.1.2.3/ShuaiToolBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-06-15 15:23:06.000000 ShuaiToolBox-1.1.2.3/ShuaiToolBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 15:23:06.000000 ShuaiToolBox-1.1.2.3/ShuaiToolBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-06-15 15:23:06.000000 ShuaiToolBox-1.1.2.3/ShuaiToolBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-15 15:23:06.000000 ShuaiToolBox-1.1.2.3/ShuaiToolBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 15:23:06.000000 ShuaiToolBox-1.1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      413 2023-06-15 15:22:57.000000 ShuaiToolBox-1.1.2.3/setup.py
```

