# Comparing `tmp/articlesumm-0.0.1.tar.gz` & `tmp/articlesumm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "articlesumm-0.0.1.tar", last modified: Tue Jun  6 14:59:00 2023, max compression
+gzip compressed data, was "articlesumm-0.0.2.tar", last modified: Thu Jun 15 01:05:50 2023, max compression
```

## Comparing `articlesumm-0.0.1.tar` & `articlesumm-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 14:58:59.999498 articlesumm-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-06 14:58:59.308444 articlesumm-0.0.1/ArticleSumm/
--rw-rw-rw-   0        0        0     2228 2023-06-06 12:39:30.000000 articlesumm-0.0.1/ArticleSumm/__init__.py
--rw-rw-rw-   0        0        0       89 2023-06-06 12:55:07.000000 articlesumm-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2023-06-06 13:05:43.000000 articlesumm-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-06 12:56:52.000000 articlesumm-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1234 2023-06-06 14:58:59.966535 articlesumm-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      545 2023-06-06 12:54:40.000000 articlesumm-0.0.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-06 14:58:59.963534 articlesumm-0.0.1/articlesumm.egg-info/
--rw-rw-rw-   0        0        0     1234 2023-06-06 14:58:56.000000 articlesumm-0.0.1/articlesumm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-06-06 14:58:57.000000 articlesumm-0.0.1/articlesumm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 14:58:56.000000 articlesumm-0.0.1/articlesumm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-06-06 14:58:56.000000 articlesumm-0.0.1/articlesumm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-06 14:58:56.000000 articlesumm-0.0.1/articlesumm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 14:59:00.000497 articlesumm-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      841 2023-06-06 14:37:09.000000 articlesumm-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:05:50.181300 articlesumm-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-15 01:05:49.723185 articlesumm-0.0.2/ArticleSumm/
+-rw-rw-rw-   0        0        0     2228 2023-06-14 21:38:04.000000 articlesumm-0.0.2/ArticleSumm/__init__.py
+-rw-rw-rw-   0        0        0      188 2023-06-14 20:03:15.000000 articlesumm-0.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2023-06-06 13:05:43.000000 articlesumm-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       54 2023-06-15 01:00:01.000000 articlesumm-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2619 2023-06-15 01:05:50.150200 articlesumm-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1982 2023-06-15 00:35:06.000000 articlesumm-0.0.2/README.md
+-rw-rw-rw-   0        0        0      545 2023-06-15 00:35:39.000000 articlesumm-0.0.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 01:05:50.121256 articlesumm-0.0.2/articlesumm.egg-info/
+-rw-rw-rw-   0        0        0     2619 2023-06-15 01:05:46.000000 articlesumm-0.0.2/articlesumm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-06-15 01:05:47.000000 articlesumm-0.0.2/articlesumm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 01:05:46.000000 articlesumm-0.0.2/articlesumm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-06-15 01:05:46.000000 articlesumm-0.0.2/articlesumm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-15 01:05:46.000000 articlesumm-0.0.2/articlesumm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 01:05:50.195171 articlesumm-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1092 2023-06-15 00:49:35.000000 articlesumm-0.0.2/setup.py
```

### Comparing `articlesumm-0.0.1/ArticleSumm/__init__.py` & `articlesumm-0.0.2/ArticleSumm/__init__.py`

 * *Files identical despite different names*

### Comparing `articlesumm-0.0.1/LICENSE.txt` & `articlesumm-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `articlesumm-0.0.1/README.txt` & `articlesumm-0.0.2/README.txt`

 * *Files identical despite different names*

