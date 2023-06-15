# Comparing `tmp/flake8_no_pep420-2.4.0.tar.gz` & `tmp/flake8_no_pep420-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_no_pep420-2.4.0.tar", last modified: Thu Apr 27 15:42:54 2023, max compression
+gzip compressed data, was "flake8_no_pep420-2.5.0.tar", last modified: Thu Jun 15 14:06:02 2023, max compression
```

## Comparing `flake8_no_pep420-2.4.0.tar` & `flake8_no_pep420-2.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-27 15:42:54.841275 flake8_no_pep420-2.4.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1203 2023-04-27 15:42:49.000000 flake8_no_pep420-2.4.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:25.000000 flake8_no_pep420-2.4.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-20 12:10:00.000000 flake8_no_pep420-2.4.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4473 2023-04-27 15:42:54.841331 flake8_no_pep420-2.4.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3314 2022-12-26 15:11:06.000000 flake8_no_pep420-2.4.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-02-28 09:05:59.000000 flake8_no_pep420-2.4.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1442 2023-04-27 15:42:54.841601 flake8_no_pep420-2.4.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-27 15:42:54.839185 flake8_no_pep420-2.4.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-27 15:42:54.840253 flake8_no_pep420-2.4.0/src/flake8_no_pep420/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1062 2023-04-27 15:37:02.000000 flake8_no_pep420-2.4.0/src/flake8_no_pep420/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:25.000000 flake8_no_pep420-2.4.0/src/flake8_no_pep420/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-27 15:42:54.841052 flake8_no_pep420-2.4.0/src/flake8_no_pep420.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4473 2023-04-27 15:42:54.000000 flake8_no_pep420-2.4.0/src/flake8_no_pep420.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      472 2023-04-27 15:42:54.000000 flake8_no_pep420-2.4.0/src/flake8_no_pep420.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-04-27 15:42:54.000000 flake8_no_pep420-2.4.0/src/flake8_no_pep420.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       58 2023-04-27 15:42:54.000000 flake8_no_pep420-2.4.0/src/flake8_no_pep420.egg-info/entry_points.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-04-27 15:42:54.000000 flake8_no_pep420-2.4.0/src/flake8_no_pep420.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       66 2023-04-27 15:42:54.000000 flake8_no_pep420-2.4.0/src/flake8_no_pep420.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       17 2023-04-27 15:42:54.000000 flake8_no_pep420-2.4.0/src/flake8_no_pep420.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-04-27 15:42:54.841172 flake8_no_pep420-2.4.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2580 2023-04-27 15:37:02.000000 flake8_no_pep420-2.4.0/tests/test_flake8_no_pep420.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-15 14:06:02.203341 flake8_no_pep420-2.5.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1242 2023-06-15 14:05:59.000000 flake8_no_pep420-2.5.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:59:25.000000 flake8_no_pep420-2.5.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-20 12:10:00.000000 flake8_no_pep420-2.5.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4473 2023-06-15 14:06:02.203396 flake8_no_pep420-2.5.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3314 2023-06-15 14:05:57.000000 flake8_no_pep420-2.5.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-02-28 09:05:59.000000 flake8_no_pep420-2.5.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1443 2023-06-15 14:06:02.203643 flake8_no_pep420-2.5.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-15 14:06:02.200739 flake8_no_pep420-2.5.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-15 14:06:02.202106 flake8_no_pep420-2.5.0/src/flake8_no_pep420/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1062 2023-04-27 15:37:02.000000 flake8_no_pep420-2.5.0/src/flake8_no_pep420/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:59:25.000000 flake8_no_pep420-2.5.0/src/flake8_no_pep420/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-15 14:06:02.203003 flake8_no_pep420-2.5.0/src/flake8_no_pep420.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4473 2023-06-15 14:06:02.000000 flake8_no_pep420-2.5.0/src/flake8_no_pep420.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      472 2023-06-15 14:06:02.000000 flake8_no_pep420-2.5.0/src/flake8_no_pep420.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-15 14:06:02.000000 flake8_no_pep420-2.5.0/src/flake8_no_pep420.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       58 2023-06-15 14:06:02.000000 flake8_no_pep420-2.5.0/src/flake8_no_pep420.egg-info/entry_points.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-15 14:06:02.000000 flake8_no_pep420-2.5.0/src/flake8_no_pep420.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       66 2023-06-15 14:06:02.000000 flake8_no_pep420-2.5.0/src/flake8_no_pep420.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       17 2023-06-15 14:06:02.000000 flake8_no_pep420-2.5.0/src/flake8_no_pep420.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-15 14:06:02.203120 flake8_no_pep420-2.5.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2580 2023-04-27 15:37:02.000000 flake8_no_pep420-2.5.0/tests/test_flake8_no_pep420.py
```

### Comparing `flake8_no_pep420-2.4.0/CHANGELOG.rst` & `flake8_no_pep420-2.5.0/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 =========
 Changelog
 =========
 
+2.5.0 (2023-06-15)
+------------------
+
 2.4.0 (2023-04-27)
 ------------------
 
 * Support ``.pyi`` files.
 
 2.3.0 (2022-05-11)
 ------------------
```

### Comparing `flake8_no_pep420-2.4.0/LICENSE` & `flake8_no_pep420-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_no_pep420-2.4.0/PKG-INFO` & `flake8_no_pep420-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8_no_pep420
-Version: 2.4.0
+Version: 2.5.0
 Summary: A flake8 plugin to ban PEP-420 implicit namespace packages.
 Home-page: https://github.com/adamchainz/flake8-no-pep420
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/flake8-no-pep420/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
```

### Comparing `flake8_no_pep420-2.4.0/README.rst` & `flake8_no_pep420-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `flake8_no_pep420-2.4.0/setup.cfg` & `flake8_no_pep420-2.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = flake8_no_pep420
-version = 2.4.0
+version = 2.5.0
 description = A flake8 plugin to ban PEP-420 implicit namespace packages.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/flake8-no-pep420
 author = Adam Johnson
 author_email = me@adamj.eu
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Flake8
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Programming Language :: Python :: 3
```

### Comparing `flake8_no_pep420-2.4.0/src/flake8_no_pep420/__init__.py` & `flake8_no_pep420-2.5.0/src/flake8_no_pep420/__init__.py`

 * *Files identical despite different names*

### Comparing `flake8_no_pep420-2.4.0/src/flake8_no_pep420.egg-info/PKG-INFO` & `flake8_no_pep420-2.5.0/src/flake8_no_pep420.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-no-pep420
-Version: 2.4.0
+Version: 2.5.0
 Summary: A flake8 plugin to ban PEP-420 implicit namespace packages.
 Home-page: https://github.com/adamchainz/flake8-no-pep420
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/flake8-no-pep420/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
```

### Comparing `flake8_no_pep420-2.4.0/tests/test_flake8_no_pep420.py` & `flake8_no_pep420-2.5.0/tests/test_flake8_no_pep420.py`

 * *Files identical despite different names*

