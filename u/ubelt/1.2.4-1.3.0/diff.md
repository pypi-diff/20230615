# Comparing `tmp/ubelt-1.2.4.tar.gz` & `tmp/ubelt-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubelt-1.2.4.tar", last modified: Tue Feb 28 21:45:23 2023, max compression
+gzip compressed data, was "ubelt-1.3.0.tar", last modified: Thu Jun 15 02:32:50 2023, max compression
```

## Comparing `ubelt-1.2.4.tar` & `ubelt-1.3.0.tar`

### file list

```diff
@@ -1,76 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:45:23.521800 ubelt-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-02-28 21:45:17.000000 ubelt-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    58100 2023-02-28 21:45:23.521800 ubelt-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    56762 2023-02-28 21:45:17.000000 ubelt-1.2.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-02-28 21:45:17.000000 ubelt-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 21:45:23.521800 ubelt-1.2.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     7952 2023-02-28 21:45:17.000000 ubelt-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:45:23.517799 ubelt-1.2.4/ubelt/
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/__main__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/_win32_links.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/_win32_links.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16069 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/orderedset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/orderedset.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    36626 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/progiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/progiter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_arg.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_arg.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    52100 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_cache.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    28175 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_cmd.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_colors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_const.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_const.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_deprecate.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_deprecate.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    67505 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_dict.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18494 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_download.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_download_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_download_manager.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    44312 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_format.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_func.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18831 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_futures.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    49678 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_hash.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    36987 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_import.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18992 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_indexable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_indexable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10328 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_io.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_links.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_links.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    32834 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_list.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_memoize.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_mixins.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    59845 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_path.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14734 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_platform.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_str.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_stream.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22494 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_time.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14905 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-02-28 21:45:17.000000 ubelt-1.2.4/ubelt/util_zip.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:45:23.521800 ubelt-1.2.4/ubelt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    58100 2023-02-28 21:45:23.000000 ubelt-1.2.4/ubelt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-02-28 21:45:23.000000 ubelt-1.2.4/ubelt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 21:45:23.000000 ubelt-1.2.4/ubelt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-02-28 21:45:23.000000 ubelt-1.2.4/ubelt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-28 21:45:23.000000 ubelt-1.2.4/ubelt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:32:50.173372 ubelt-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-15 02:32:40.000000 ubelt-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    59674 2023-06-15 02:32:50.173372 ubelt-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    58336 2023-06-15 02:32:40.000000 ubelt-1.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-15 02:32:40.000000 ubelt-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 02:32:50.173372 ubelt-1.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7952 2023-06-15 02:32:40.000000 ubelt-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:32:50.173372 ubelt-1.3.0/ubelt/
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/__main__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/_win32_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/_win32_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16069 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/orderedset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/orderedset.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    36626 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/progiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/progiter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_arg.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    52100 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    31964 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_cmd.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_colors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_const.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_deprecate.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    74794 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_dict.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_download.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_download_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_download_manager.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_func.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19328 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_futures.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    49678 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_hash.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    38221 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_import.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_indexable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_indexable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10328 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_io.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13011 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    32834 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_memoize.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    59178 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_path.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14734 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_platform.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    42633 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_repr.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_str.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_stream.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22494 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_time.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14905 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_zip.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:32:50.173372 ubelt-1.3.0/ubelt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    59674 2023-06-15 02:32:50.000000 ubelt-1.3.0/ubelt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-15 02:32:50.000000 ubelt-1.3.0/ubelt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 02:32:50.000000 ubelt-1.3.0/ubelt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-06-15 02:32:50.000000 ubelt-1.3.0/ubelt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 02:32:50.000000 ubelt-1.3.0/ubelt.egg-info/top_level.txt
```

### Comparing `ubelt-1.2.4/LICENSE` & `ubelt-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/PKG-INFO` & `ubelt-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubelt
-Version: 1.2.4
+Version: 1.3.0
 Summary: A Python utility belt containing simple tools, a stdlib like feel, and extra batteries.
 Home-page: https://github.com/Erotemic/ubelt
 Author: Jon Crall
 Author-email: erotemic@gmail.com
 License: Apache 2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -31,42 +31,59 @@
 Provides-Extra: optional
 Provides-Extra: optional-strict
 Provides-Extra: runtime-strict
 Provides-Extra: tests
 Provides-Extra: tests-strict
 License-File: LICENSE
 
-|GithubActions| |ReadTheDocs| |Pypi| |Downloads| |Codecov| |CircleCI| |Appveyor| 
+|GithubActions| |ReadTheDocs| |Pypi| |Downloads| |Codecov| |CircleCI| |Appveyor|
 
 .. .. |CodeQuality| |TwitterFollow|
 
 
 .. The large version wont work because github strips rst image rescaling. https://i.imgur.com/AcWVroL.png
 .. image:: https://i.imgur.com/PoYIsWE.png
    :height: 100px
    :align: left
 
 
 ..   .. raw:: html
 ..       <img src="https://i.imgur.com/AcWVroL.png" height="100px">
 
-Ubelt is a small library of robust, tested, documented, and simple functions
+
+Ubelt is a utility library for Python with a stdlib like feel.
+
+
+Elevator Pitch:
+===============
+
+Is the Python standard library good?  Yes.  Could it's conciseness be improved?  Yes.  Ubelt aims to provide a quicker way to express things you can do in the standard library.  Progress?  `ub.ProgIter <https://ubelt.readthedocs.io/en/latest/ubelt.progiter.html#ubelt.progiter.ProgIter>`_.  Hashing?  `ub.hash_data <https://ubelt.readthedocs.io/en/latest/ubelt.util_hash.html#ubelt.util_hash.hash_data>`_ / `ub.hash_file <https://ubelt.readthedocs.io/en/latest/ubelt.util_hash.html#ubelt.util_hash.hash_file>`_.  Caching?  `ub.Cacher <https://ubelt.readthedocs.io/en/latest/ubelt.util_cache.html#ubelt.util_cache.Cacher>`_ / `ub.CacheStamp <https://ubelt.readthedocs.io/en/latest/ubelt.util_cache.html#ubelt.util_cache.CacheStamp>`_.  Shell commands?  `ub.cmd <https://ubelt.readthedocs.io/en/latest/ubelt.util_cmd.html#ubelt.util_cmd.cmd>`_. There are similar functions for downloading data, futures-based parallel (or serial) job execution, pretty reprs, path management, iteration, and one of my favorites: set operation enriched dictionaries: `ub.udict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.UDict>`_.
+
+There are 120ish functions and classes to help make your code shorter and easier to express concisely.  The library is fast to install and import, all dependencies are optional.  As of 2023 it is 6 years old, regularly maintained, and mature.  It is well tested and has moderate usage.
+
+To learn more, the function usefulness chart is a good place to start.  This shows how often I use particular functions, and while some of the less used ones are candidates for removal, some of them still worth checking out. For a slightly slower start, read the introduction:
+
+
+Introduction:
+=============
+
+Ubelt is a lightweight library of robust, tested, documented, and simple functions
 that extend the Python standard library. It has a flat API that all behaves
 similarly on Windows, Mac, and Linux (up to some small unavoidable
 differences).  Almost every function in ``ubelt`` was written with a doctest.
 This provides helpful documentation and example usage as well as helping
-achieve 100% test coverage (with minor exceptions on Windows). 
+achieve 100% test coverage (with minor exceptions on Windows).
 
 * Goal: provide simple functions that accomplish common tasks not yet addressed by the python standard library.
 
 * Constraints: Must be low-impact pure python; it should be easy to install and use.
 
 * Method: All functions are written with docstrings and doctests to ensure that a baseline level of documentation and testing always exists (even if functions are copy/pasted into other libraries)
 
-* Motto: Good utilities lift all codes. 
+* Motto: Good utilities lift all codes.
 
 
 Read the docs here: http://ubelt.readthedocs.io/en/latest/
 
 These are some of the tasks that ubelt's API enables:
 
   - extended pathlib with expand, ensuredir, endswith, augment, delete (ub.Path)
@@ -87,17 +104,17 @@
 
   - show loop progress with less overhead than tqdm (ProgIter)
 
   - download a file with optional caching and hash verification (download, grabdata)
 
   - run shell commands (cmd)
 
-  - find a file or directory in candidate locations (find_path, find_exe) 
+  - find a file or directory in candidate locations (find_path, find_exe)
 
-  - string-format nested data structures (urepr)
+  - string-repr for nested data structures (urepr)
 
   - color text with ANSI tags (color_text)
 
   - horizontally concatenate multiline strings (hzcat)
 
   - create cross platform symlinks (symlink)
 
@@ -105,15 +122,15 @@
 
   - check if a particular flag or value is on the command line (argflag, argval)
 
   - memoize functions (memoize, memoize_method, memoize_property)
 
   - build ordered sets (oset)
 
-  - argmax/min/sort on lists and dictionaries (argmin, argsort,) 
+  - argmax/min/sort on lists and dictionaries (argmin, argsort,)
 
   - get a histogram of items or find duplicates in a list (dict_hist, find_duplicates)
 
   - group a sequence of items by some criterion (group_items)
 
 Ubelt is small. Its top-level API is defined using roughly 40 lines:
 
@@ -130,15 +147,15 @@
                                  invert_dict, map_keys, map_vals, map_values,
                                  named_product, odict, sdict, sorted_keys,
                                  sorted_vals, sorted_values, udict, varied_values,)
     from ubelt.util_deprecate import (schedule_deprecation,)
     from ubelt.util_download import (download, grabdata,)
     from ubelt.util_download_manager import (DownloadManager,)
     from ubelt.util_func import (compatible, identity, inject_method,)
-    from ubelt.util_format import (FormatterExtensions, repr2, urepr,)
+    from ubelt.util_repr import (ReprExtensions, urepr,)
     from ubelt.util_futures import (Executor, JobPool,)
     from ubelt.util_io import (delete, touch,)
     from ubelt.util_links import (symlink,)
     from ubelt.util_list import (allsame, argmax, argmin, argsort, argunique,
                                  boolmask, chunks, compress, flatten, iter_window,
                                  iterable, peek, take, unique, unique_flags,)
     from ubelt.util_hash import (hash_data, hash_file,)
@@ -172,15 +189,15 @@
 
     pip install ubelt
 
 Note that our distributions on pypi are signed with GPG. The signing public key
 is ``D297D757``; this should agree with the value in `dev/public_gpg_key`.
 
 
-Function Usefulness 
+Function Usefulness
 ===================
 
 When I had to hand pick a set of functions that I thought were the most useful
 I chose these and provided some comment on why:
 
 .. code:: python
 
@@ -196,98 +213,97 @@
     ub.JobPool   # easy multi-threading / multi-procesing / or single-threaded processing
     ub.ProgIter  # a minimal progress iterator. It's single threaded, informative, and faster than tqdm.
     ub.memoize  # like ``functools.cache``, but uses ub.hash_data if the args are not hashable.
     ub.urepr  # readable representations of nested data structures
 
 
 But a better way might to objectively measure the frequency of usage and built
-a histogram of usefulness. I generated this histogram using ``python dev/maintain/gen_api_for_docs.py``, 
+a histogram of usefulness. I generated this histogram using ``python dev/maintain/gen_api_for_docs.py``,
 which roughly counts the number of times I've used a ubelt function in another
 project. Note: this measure is biased towards older functions.
 
 ================================================================================================================================================ ================
  Function name                                                                                                                                         Usefulness
 ================================================================================================================================================ ================
-`ubelt.repr2 <https://ubelt.readthedocs.io/en/latest/ubelt.util_format.html#ubelt.util_format.repr2>`__                                                      2621
-`ubelt.Path <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.Path>`__                                                             903
-`ubelt.ProgIter <https://ubelt.readthedocs.io/en/latest/ubelt.progiter.html#ubelt.progiter.ProgIter>`__                                                       540
-`ubelt.paragraph <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.paragraph>`__                                                     392
-`ubelt.take <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.take>`__                                                             385
-`ubelt.codeblock <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.codeblock>`__                                                     330
-`ubelt.expandpath <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.expandpath>`__                                                 330
-`ubelt.cmd <https://ubelt.readthedocs.io/en/latest/ubelt.util_cmd.html#ubelt.util_cmd.cmd>`__                                                                 279
-`ubelt.ensuredir <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.ensuredir>`__                                                   258
-`ubelt.odict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.odict>`__                                                           255
-`ubelt.iterable <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.iterable>`__                                                     245
-`ubelt.udict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.udict>`__                                                           238
-`ubelt.ddict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.ddict>`__                                                           234
-`ubelt.NoParam <https://ubelt.readthedocs.io/en/latest/ubelt.util_const.html#ubelt.util_const.NoParam>`__                                                     220
-`ubelt.NiceRepr <https://ubelt.readthedocs.io/en/latest/ubelt.util_mixins.html#ubelt.util_mixins.NiceRepr>`__                                                 219
-`ubelt.map_vals <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.map_vals>`__                                                     216
-`ubelt.flatten <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.flatten>`__                                                       208
-`ubelt.dzip <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dzip>`__                                                             201
-`ubelt.peek <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.peek>`__                                                             197
-`ubelt.oset <https://ubelt.readthedocs.io/en/latest/ubelt.orderedset.html#ubelt.orderedset.oset>`__                                                           191
-`ubelt.argflag <https://ubelt.readthedocs.io/en/latest/ubelt.util_arg.html#ubelt.util_arg.argflag>`__                                                         178
-`ubelt.group_items <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.group_items>`__                                               169
-`ubelt.urepr <https://ubelt.readthedocs.io/en/latest/ubelt.util_format.html#ubelt.util_format.urepr>`__                                                       162
-`ubelt.hash_data <https://ubelt.readthedocs.io/en/latest/ubelt.util_hash.html#ubelt.util_hash.hash_data>`__                                                   154
+`ubelt.urepr <https://ubelt.readthedocs.io/en/latest/ubelt.util_repr.html#ubelt.util_repr.urepr>`__                                                          2893
+`ubelt.Path <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.Path>`__                                                             992
+`ubelt.ProgIter <https://ubelt.readthedocs.io/en/latest/ubelt.progiter.html#ubelt.progiter.ProgIter>`__                                                       544
+`ubelt.paragraph <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.paragraph>`__                                                     482
+`ubelt.take <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.take>`__                                                             387
+`ubelt.codeblock <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.codeblock>`__                                                     358
+`ubelt.expandpath <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.expandpath>`__                                                 331
+`ubelt.cmd <https://ubelt.readthedocs.io/en/latest/ubelt.util_cmd.html#ubelt.util_cmd.cmd>`__                                                                 302
+`ubelt.udict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.udict>`__                                                           271
+`ubelt.ensuredir <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.ensuredir>`__                                                   256
+`ubelt.odict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.odict>`__                                                           253
+`ubelt.iterable <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.iterable>`__                                                     252
+`ubelt.ddict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.ddict>`__                                                           238
+`ubelt.NiceRepr <https://ubelt.readthedocs.io/en/latest/ubelt.util_mixins.html#ubelt.util_mixins.NiceRepr>`__                                                 221
+`ubelt.NoParam <https://ubelt.readthedocs.io/en/latest/ubelt.util_const.html#ubelt.util_const.NoParam>`__                                                     216
+`ubelt.map_vals <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.map_vals>`__                                                     215
+`ubelt.flatten <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.flatten>`__                                                       214
+`ubelt.dzip <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dzip>`__                                                             200
+`ubelt.oset <https://ubelt.readthedocs.io/en/latest/ubelt.orderedset.html#ubelt.orderedset.oset>`__                                                           198
+`ubelt.peek <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.peek>`__                                                             196
+`ubelt.argflag <https://ubelt.readthedocs.io/en/latest/ubelt.util_arg.html#ubelt.util_arg.argflag>`__                                                         177
+`ubelt.group_items <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.group_items>`__                                               171
+`ubelt.hash_data <https://ubelt.readthedocs.io/en/latest/ubelt.util_hash.html#ubelt.util_hash.hash_data>`__                                                   165
 `ubelt.grabdata <https://ubelt.readthedocs.io/en/latest/ubelt.util_download.html#ubelt.util_download.grabdata>`__                                             131
+`ubelt.argval <https://ubelt.readthedocs.io/en/latest/ubelt.util_arg.html#ubelt.util_arg.argval>`__                                                           125
 `ubelt.Timer <https://ubelt.readthedocs.io/en/latest/ubelt.util_time.html#ubelt.util_time.Timer>`__                                                           120
 `ubelt.dict_isect <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dict_isect>`__                                                 113
-`ubelt.dict_hist <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dict_hist>`__                                                   112
-`ubelt.argval <https://ubelt.readthedocs.io/en/latest/ubelt.util_arg.html#ubelt.util_arg.argval>`__                                                           110
+`ubelt.dict_hist <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dict_hist>`__                                                   111
 `ubelt.augpath <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.augpath>`__                                                       106
-`ubelt.identity <https://ubelt.readthedocs.io/en/latest/ubelt.util_func.html#ubelt.util_func.identity>`__                                                     105
+`ubelt.identity <https://ubelt.readthedocs.io/en/latest/ubelt.util_func.html#ubelt.util_func.identity>`__                                                     106
 `ubelt.ensure_app_cache_dir <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.ensure_app_cache_dir>`__                     105
-`ubelt.allsame <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.allsame>`__                                                        98
-`ubelt.memoize <https://ubelt.readthedocs.io/en/latest/ubelt.util_memoize.html#ubelt.util_memoize.memoize>`__                                                  97
-`ubelt.color_text <https://ubelt.readthedocs.io/en/latest/ubelt.util_colors.html#ubelt.util_colors.color_text>`__                                              96
+`ubelt.allsame <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.allsame>`__                                                       102
+`ubelt.memoize <https://ubelt.readthedocs.io/en/latest/ubelt.util_memoize.html#ubelt.util_memoize.memoize>`__                                                  99
+`ubelt.color_text <https://ubelt.readthedocs.io/en/latest/ubelt.util_colors.html#ubelt.util_colors.color_text>`__                                              98
 `ubelt.dict_diff <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dict_diff>`__                                                    95
 `ubelt.delete <https://ubelt.readthedocs.io/en/latest/ubelt.util_io.html#ubelt.util_io.delete>`__                                                              89
+`ubelt.hzcat <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.hzcat>`__                                                              88
+`ubelt.schedule_deprecation <https://ubelt.readthedocs.io/en/latest/ubelt.util_deprecate.html#ubelt.util_deprecate.schedule_deprecation>`__                    87
 `ubelt.named_product <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.named_product>`__                                            85
-`ubelt.compress <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.compress>`__                                                      83
-`ubelt.schedule_deprecation <https://ubelt.readthedocs.io/en/latest/ubelt.util_deprecate.html#ubelt.util_deprecate.schedule_deprecation>`__                    77
-`ubelt.IndexableWalker <https://ubelt.readthedocs.io/en/latest/ubelt.util_indexable.html#ubelt.util_indexable.IndexableWalker>`__                              72
-`ubelt.hzcat <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.hzcat>`__                                                              68
+`ubelt.compress <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.compress>`__                                                      85
+`ubelt.IndexableWalker <https://ubelt.readthedocs.io/en/latest/ubelt.util_indexable.html#ubelt.util_indexable.IndexableWalker>`__                              74
 `ubelt.indent <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.indent>`__                                                            68
-`ubelt.JobPool <https://ubelt.readthedocs.io/en/latest/ubelt.util_futures.html#ubelt.util_futures.JobPool>`__                                                  65
+`ubelt.JobPool <https://ubelt.readthedocs.io/en/latest/ubelt.util_futures.html#ubelt.util_futures.JobPool>`__                                                  67
 `ubelt.unique <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.unique>`__                                                          63
 `ubelt.dict_union <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dict_union>`__                                                  57
 `ubelt.map_keys <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.map_keys>`__                                                      49
 `ubelt.invert_dict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.invert_dict>`__                                                48
+`ubelt.iter_window <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.iter_window>`__                                                46
 `ubelt.timestamp <https://ubelt.readthedocs.io/en/latest/ubelt.util_time.html#ubelt.util_time.timestamp>`__                                                    46
-`ubelt.iter_window <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.iter_window>`__                                                44
 `ubelt.argsort <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.argsort>`__                                                        44
 `ubelt.Cacher <https://ubelt.readthedocs.io/en/latest/ubelt.util_cache.html#ubelt.util_cache.Cacher>`__                                                        43
 `ubelt.find_exe <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.find_exe>`__                                              41
 `ubelt.symlink <https://ubelt.readthedocs.io/en/latest/ubelt.util_links.html#ubelt.util_links.symlink>`__                                                      41
 `ubelt.dict_subset <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dict_subset>`__                                                41
 `ubelt.writeto <https://ubelt.readthedocs.io/en/latest/ubelt.util_io.html#ubelt.util_io.writeto>`__                                                            40
-`ubelt.chunks <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.chunks>`__                                                          39
+`ubelt.find_duplicates <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.find_duplicates>`__                                        39
+`ubelt.chunks <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.chunks>`__                                                          38
 `ubelt.hash_file <https://ubelt.readthedocs.io/en/latest/ubelt.util_hash.html#ubelt.util_hash.hash_file>`__                                                    37
 `ubelt.modname_to_modpath <https://ubelt.readthedocs.io/en/latest/ubelt.util_import.html#ubelt.util_import.modname_to_modpath>`__                              37
 `ubelt.ensure_unicode <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.ensure_unicode>`__                                            33
-`ubelt.sorted_vals <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.sorted_vals>`__                                                33
 `ubelt.memoize_property <https://ubelt.readthedocs.io/en/latest/ubelt.util_memoize.html#ubelt.util_memoize.memoize_property>`__                                33
-`ubelt.CacheStamp <https://ubelt.readthedocs.io/en/latest/ubelt.util_cache.html#ubelt.util_cache.CacheStamp>`__                                                32
-`ubelt.find_duplicates <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.find_duplicates>`__                                        32
-`ubelt.highlight_code <https://ubelt.readthedocs.io/en/latest/ubelt.util_colors.html#ubelt.util_colors.highlight_code>`__                                      31
+`ubelt.highlight_code <https://ubelt.readthedocs.io/en/latest/ubelt.util_colors.html#ubelt.util_colors.highlight_code>`__                                      33
+`ubelt.sorted_vals <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.sorted_vals>`__                                                32
+`ubelt.CacheStamp <https://ubelt.readthedocs.io/en/latest/ubelt.util_cache.html#ubelt.util_cache.CacheStamp>`__                                                30
 `ubelt.WIN32 <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.WIN32>`__                                                    28
 `ubelt.import_module_from_name <https://ubelt.readthedocs.io/en/latest/ubelt.util_import.html#ubelt.util_import.import_module_from_name>`__                    27
-`ubelt.argmax <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.argmax>`__                                                          26
-`ubelt.readfrom <https://ubelt.readthedocs.io/en/latest/ubelt.util_io.html#ubelt.util_io.readfrom>`__                                                          24
-`ubelt.import_module_from_path <https://ubelt.readthedocs.io/en/latest/ubelt.util_import.html#ubelt.util_import.import_module_from_path>`__                    21
+`ubelt.argmax <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.argmax>`__                                                          27
+`ubelt.readfrom <https://ubelt.readthedocs.io/en/latest/ubelt.util_io.html#ubelt.util_io.readfrom>`__                                                          23
+`ubelt.import_module_from_path <https://ubelt.readthedocs.io/en/latest/ubelt.util_import.html#ubelt.util_import.import_module_from_path>`__                    22
+`ubelt.compatible <https://ubelt.readthedocs.io/en/latest/ubelt.util_func.html#ubelt.util_func.compatible>`__                                                  17
 `ubelt.touch <https://ubelt.readthedocs.io/en/latest/ubelt.util_io.html#ubelt.util_io.touch>`__                                                                17
+`ubelt.Executor <https://ubelt.readthedocs.io/en/latest/ubelt.util_futures.html#ubelt.util_futures.Executor>`__                                                16
 `ubelt.memoize_method <https://ubelt.readthedocs.io/en/latest/ubelt.util_memoize.html#ubelt.util_memoize.memoize_method>`__                                    16
-`ubelt.Executor <https://ubelt.readthedocs.io/en/latest/ubelt.util_futures.html#ubelt.util_futures.Executor>`__                                                15
-`ubelt.compatible <https://ubelt.readthedocs.io/en/latest/ubelt.util_func.html#ubelt.util_func.compatible>`__                                                  15
 `ubelt.sorted_keys <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.sorted_keys>`__                                                14
+`ubelt.AutoDict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.AutoDict>`__                                                      11
 `ubelt.shrinkuser <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.shrinkuser>`__                                                  11
-`ubelt.AutoDict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.AutoDict>`__                                                      10
 `ubelt.inject_method <https://ubelt.readthedocs.io/en/latest/ubelt.util_func.html#ubelt.util_func.inject_method>`__                                            10
 `ubelt.varied_values <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.varied_values>`__                                             9
 `ubelt.split_modpath <https://ubelt.readthedocs.io/en/latest/ubelt.util_import.html#ubelt.util_import.split_modpath>`__                                         8
 `ubelt.modpath_to_modname <https://ubelt.readthedocs.io/en/latest/ubelt.util_import.html#ubelt.util_import.modpath_to_modname>`__                               8
 `ubelt.get_app_cache_dir <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.get_app_cache_dir>`__                             8
 `ubelt.zopen <https://ubelt.readthedocs.io/en/latest/ubelt.util_zip.html#ubelt.util_zip.zopen>`__                                                               7
 `ubelt.LINUX <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.LINUX>`__                                                     7
@@ -315,26 +331,26 @@
 `ubelt.get_app_data_dir <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.get_app_data_dir>`__                               0
 `ubelt.get_app_config_dir <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.get_app_config_dir>`__                           0
 `ubelt.ensure_app_data_dir <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.ensure_app_data_dir>`__                         0
 `ubelt.ensure_app_config_dir <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.ensure_app_config_dir>`__                     0
 `ubelt.TempDir <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.TempDir>`__                                                         0
 `ubelt.TeeStringIO <https://ubelt.readthedocs.io/en/latest/ubelt.util_stream.html#ubelt.util_stream.TeeStringIO>`__                                             0
 `ubelt.SetDict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.SetDict>`__                                                         0
+`ubelt.ReprExtensions <https://ubelt.readthedocs.io/en/latest/ubelt.util_repr.html#ubelt.util_repr.ReprExtensions>`__                                           0
 `ubelt.POSIX <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.POSIX>`__                                                     0
 `ubelt.OrderedSet <https://ubelt.readthedocs.io/en/latest/ubelt.orderedset.html#ubelt.orderedset.OrderedSet>`__                                                 0
-`ubelt.FormatterExtensions <https://ubelt.readthedocs.io/en/latest/ubelt.util_format.html#ubelt.util_format.FormatterExtensions>`__                             0
 `ubelt.DownloadManager <https://ubelt.readthedocs.io/en/latest/ubelt.util_download_manager.html#ubelt.util_download_manager.DownloadManager>`__                 0
 `ubelt.CaptureStream <https://ubelt.readthedocs.io/en/latest/ubelt.util_stream.html#ubelt.util_stream.CaptureStream>`__                                         0
 ================================================================================================================================================ ================
 
 
 Examples
 ========
 
-The most up to date examples are the doctests. 
+The most up to date examples are the doctests.
 We also have a Jupyter notebook: https://github.com/Erotemic/ubelt/blob/main/docs/notebooks/Ubelt%20Demo.ipynb
 
 Here are some examples of some features inside ``ubelt``
 
 Paths
 -----
 
@@ -386,15 +402,15 @@
 usable and will become better integrated in the future. See
 ``ubelt/util_hash.py`` for details.
 
 Caching
 -------
 
 Cache intermediate results from blocks of code inside a script with minimal
-boilerplate or modification to the original code.  
+boilerplate or modification to the original code.
 
 For direct caching of data, use the ``Cacher`` class.  By default results will
 be written to the ubelt's appdir cache, but the exact location can be specified
 via ``dpath`` or the ``appname`` arguments.  Additionally, process dependencies
 can be specified via the ``depends`` argument, which allows for implicit cache
 invalidation.  As far as I can tell, this is the most concise way (4 lines of
 boilerplate) to cache a block of code with existing Python syntax (as of
@@ -430,61 +446,61 @@
     >>> params = {'params1': 1, 'param2': 2}
     >>> expected_fpath = dpath / 'file.txt'
     >>> stamp = ub.CacheStamp('name', dpath=dpath, depends=params,
     >>>                      hasher='sha256', product=expected_fpath,
     >>>                      expires='2101-01-01T000000Z', verbose=3)
     >>> # Start fresh
     >>> stamp.clear()
-    >>>     
+    >>>
     >>> for _ in range(2):
     >>>     if stamp.expired():
     >>>         expected_fpath.write_text('expensive process')
     >>>         stamp.renew()
 
 See `<https://ubelt.readthedocs.io/en/latest/ubelt.util_cache.html>`_ for more
 details about ``Cacher`` and ``CacheStamp``.
 
 Loop Progress
 -------------
 
 ``ProgIter`` is a no-threads attached Progress meter that writes to stdout.  It
 is a mostly drop-in alternative to `tqdm
-<https://pypi.python.org/pypi/tqdm>`__. 
+<https://pypi.python.org/pypi/tqdm>`__.
 *The advantage of ``ProgIter`` is that it does not use any python threading*,
 and therefore can be safer with code that makes heavy use of multiprocessing.
 
 Note: ``ProgIter`` is also defined in a standalone module: ``pip install progiter``)
 
 .. code:: python
 
     >>> import ubelt as ub
     >>> def is_prime(n):
     ...     return n >= 2 and not any(n % i == 0 for i in range(2, n))
     >>> for n in ub.ProgIter(range(1000), verbose=2):
     >>>     # do some work
     >>>     is_prime(n)
-        0/1000... rate=0.00 Hz, eta=?, total=0:00:00, wall=14:05 EST 
-        1/1000... rate=82241.25 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST 
-      257/1000... rate=177204.69 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST 
-      642/1000... rate=94099.22 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST 
-     1000/1000... rate=71886.74 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST 
+        0/1000... rate=0.00 Hz, eta=?, total=0:00:00, wall=14:05 EST
+        1/1000... rate=82241.25 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST
+      257/1000... rate=177204.69 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST
+      642/1000... rate=94099.22 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST
+     1000/1000... rate=71886.74 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST
 
 
 Command Line Interaction
 ------------------------
 
 The builtin Python ``subprocess.Popen`` module is great, but it can be a
 bit clunky at times. The ``os.system`` command is easy to use, but it
 doesn't have much flexibility. The ``ub.cmd`` function aims to fix this.
 It is as simple to run as ``os.system``, but it returns a dictionary
 containing the return code, standard out, standard error, and the
 ``Popen`` object used under the hood.
 
 This utility is designed to provide as consistent as possible behavior across
-different platforms.  We aim to support Windows, Linux, and OSX. 
+different platforms.  We aim to support Windows, Linux, and OSX.
 
 .. code:: python
 
     >>> import ubelt as ub
     >>> info = ub.cmd('gcc --version')
     >>> print(ub.urepr(info))
     {
@@ -522,15 +538,15 @@
 
 This allows you to easily run a command line executable as part of a
 python process, see what it is doing, and then do something based on its
 output, just as you would if you were interacting with the command line
 itself.
 
 The idea is that ``ub.cmd`` removes the need to think about if you need to pass
-a list of args, or a string. Both will work. 
+a list of args, or a string. Both will work.
 
 New in ``1.0.0``, a third variant with different consequences for executing
 shell commands. Using the ``system=True`` kwarg will directly use ``os.system``
 instead of ``Popen`` entirely. In this mode it is not possible to ``tee`` the
 output because the program is executing directly in the foreground. This is
 useful for doing things like spawning a vim session and returning if the user
 manages to quit vim.
@@ -568,25 +584,25 @@
 provided value. The ``hasher`` keyword argument can be used to change which
 hashing algorithm is used (it defaults to ``"sha512"``).
 
 Dictionary Set Operations
 -------------------------
 
 
-Dictionary operations that are analogous to set operations. 
+Dictionary operations that are analogous to set operations.
 See each funtions documentation for more details on the behavior of the values.
 Typically the last seen value is given priority.
 
-I hope Python decides to add these to the stdlib someday. 
+I hope Python decides to add these to the stdlib someday.
 
 * ``ubelt.dict_union`` corresponds to ``set.union``.
 * ``ubelt.dict_isect`` corresponds to ``set.intersection``.
 * ``ubelt.dict_diff`` corresponds to ``set.difference``.
 
-.. code:: python 
+.. code:: python
 
    >>> d1 = {'a': 1, 'b': 2, 'c': 3}
    >>> d2 = {'c': 10, 'e': 20, 'f': 30}
    >>> d3 = {'e': 10, 'f': 20, 'g': 30, 'a': 40}
    >>> ub.dict_union(d1, d2, d3)
    {'a': 40, 'b': 2, 'c': 10, 'e': 10, 'f': 20, 'g': 30}
 
@@ -594,19 +610,19 @@
    {'c': 3}
 
    >>> ub.dict_diff(d1, d2)
    {'a': 1, 'b': 2}
 
 
 New in Version 1.2.0: Ubelt now contains a dictionary subclass with set
-operations that can be invoked as ``ubelt.SetDict`` or ``ub.sdict``. 
+operations that can be invoked as ``ubelt.SetDict`` or ``ub.sdict``.
 Note that n-ary operations are supported.
 
 
-.. code:: python 
+.. code:: python
 
    >>> d1 = ub.sdict({'a': 1, 'b': 2, 'c': 3})
    >>> d2 = {'c': 10, 'e': 20, 'f': 30}
    >>> d3 = {'e': 10, 'f': 20, 'g': 30, 'a': 40}
    >>> d1 | d2 | d3
    {'a': 40, 'b': 2, 'c': 10, 'e': 10, 'f': 20, 'g': 30}
 
@@ -629,15 +645,15 @@
 id to a list of its corresponding items.  In other words, group a sequence of
 items of type ``VT`` and corresponding keys of type ``KT`` given by a function
 or corresponding list, group them into a ``Dict[KT, List[VT]`` such that each
 key maps to a list of the values associated with the key.  This is similar to
 `pandas.DataFrame.groupby <https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.groupby.html>`_.
 
 Group ids can be specified by a second list containing the id for
-each corresponding item. 
+each corresponding item.
 
 .. code:: python
 
     >>> import ubelt as ub
     >>> # Group via a corresonding list
     >>> item_list    = ['ham',     'jam',   'spam',     'eggs',    'cheese', 'bannana']
     >>> groupid_list = ['protein', 'fruit', 'protein',  'protein', 'dairy',  'fruit']
@@ -657,26 +673,26 @@
     ...     return item.count('a')
     >>> dict(ub.group_items(item_list, grouper))
     {1: ['ham', 'jam', 'spam'], 0: ['eggs', 'cheese'], 3: ['bannana']}
 
 Dictionary Histogram
 --------------------
 
-Find the frequency of items in a sequence. 
+Find the frequency of items in a sequence.
 Given a list or sequence of items, this returns a dictionary mapping each
 unique value in the sequence to the number of times it appeared.
 This is similar to `pandas.DataFrame.value_counts <https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.value_counts.html>`_.
 
 .. code:: python
 
     >>> import ubelt as ub
     >>> item_list = [1, 2, 39, 900, 1232, 900, 1232, 2, 2, 2, 900]
     >>> ub.dict_hist(item_list)
     {1232: 2, 1: 1, 2: 4, 900: 3, 39: 1}
-    
+
 
 Each item can also be given a weight
 
 .. code:: python
 
     >>> import ubelt as ub
     >>> item_list = [1, 2, 39, 900, 1232, 900, 1232, 2, 2, 2, 900]
@@ -752,15 +768,15 @@
     {0: {'A', 'a'}, 1: {'b'}, 2: {'C', 'c'}, 3: {'d'}}
 
 
 New in Version 1.2.0: Ubelt now contains a dictionary subclass ``ubelt.UDict``
 with these quality of life operations (and also inherits from
 ``ubelt.SetDict``). The alias ``ubelt.udict`` can be used for quicker access.
 
-.. code:: python 
+.. code:: python
 
    >>> import ubelt as ub
    >>> d1 = ub.udict({'a': 1, 'b': 2, 'c': 3})
    >>> d1 & {'a', 'c'}
    {'a': 1, 'c': 3}
 
    >>> d1.map_keys(ord)
@@ -778,49 +794,49 @@
 
 Next time you have a default configuration dictionary like and you allow the
 developer to pass keyword arguments to modify these behaviors, consider using
 dictionary intersection (&) to separate out only the relevant parts and
 dictionary union (|) to update those relevant parts.  You can also use
 dictionary differences (-) if you need to check for unused arguments.
 
-.. code:: python 
+.. code:: python
 
     import ubelt as ub
-    
+
     def run_multiple_algos(**kwargs):
         algo1_defaults = {'opt1': 10, 'opt2': 11}
         algo2_defaults = {'src': './here/', 'dst': './there'}
-    
+
         kwargs = ub.udict(kwargs)
-    
+
         algo1_specified = kwargs & algo1_defaults
         algo2_specified = kwargs & algo2_defaults
-    
+
         algo1_config = algo1_defaults | algo1_specified
         algo2_config = algo2_defaults | algo2_specified
-    
+
         unused_kwargs = kwargs - (algo1_defaults | algo2_defaults)
-    
+
         print('algo1_specified = {}'.format(ub.urepr(algo1_specified, nl=1)))
         print('algo2_specified = {}'.format(ub.urepr(algo2_specified, nl=1)))
         print(f'algo1_config={algo1_config}')
         print(f'algo2_config={algo2_config}')
         print(f'The following kwargs were unused {unused_kwargs}')
-    
+
     print(chr(10))
     print('-- Run with some specified --')
     run_multiple_algos(src='box', opt2='fox')
     print(chr(10))
     print('-- Run with extra unspecified --')
     run_multiple_algos(a=1, b=2)
 
 
-Produces: 
+Produces:
 
-.. code:: 
+.. code::
 
     -- Run with some specified --
     algo1_specified = {
         'opt2': 'fox',
     }
     algo2_specified = {
         'src': 'box',
@@ -832,15 +848,15 @@
 
     -- Run with extra unspecified --
     algo1_specified = {}
     algo2_specified = {}
     algo1_config={'opt1': 10, 'opt2': 11}
     algo2_config={'src': './here/', 'dst': './there'}
     The following kwargs were unused {'a': 1, 'b': 2}
-        
+
 
 
 Find Duplicates
 ---------------
 
 Find all duplicate items in a list. More specifically,
 ``ub.find_duplicates`` searches for items that appear more than ``k``
@@ -862,19 +878,19 @@
 the standard place to dump those files differs depending if you are on
 Windows, Linux, or Mac. Ubelt offers a unified functions for determining
 what these paths are.
 
 New in version 1.0.0: the ``ub.Path.appdir`` classmethod provides a way to
 achieve the above with a chainable object oriented interface.
 
-The ``ub.Path.appdir(..., type='cache')``, 
-``ub.Path.appdir(..., type='config')``, and 
+The ``ub.Path.appdir(..., type='cache')``,
+``ub.Path.appdir(..., type='config')``, and
 ``ub.Path.appdir(..., type='data')``
 functions find the correct platform-specific location for these files and
-calling ``ensuredir`` ensures that the directories exist. 
+calling ``ensuredir`` ensures that the directories exist.
 
 The config root directory is ``~/AppData/Roaming`` on Windows,
 ``~/.config`` on Linux and ``~/Library/Application Support`` on Mac. The
 cache root directory is ``~/AppData/Local`` on Windows, ``~/.config`` on
 Linux and ``~/Library/Caches`` on Mac.
 
 Example usage on Linux might look like this:
@@ -930,28 +946,28 @@
 
 Ubelt contains functions to import modules dynamically without using the
 python ``import`` statement. While ``importlib`` exists, the ``ubelt``
 implementation is simpler to user and does not have the disadvantage of
 breaking ``pytest``.
 
 Note ``ubelt`` simply provides an interface to this functionality, the
-core implementation is in ``xdoctest`` (over as of version ``0.7.0``, 
+core implementation is in ``xdoctest`` (over as of version ``0.7.0``,
 the code is statically copied into an autogenerated file such that ``ubelt``
 does not actually depend on ``xdoctest`` during runtime).
 
 .. code:: python
 
     >>> import ubelt as ub
     >>> try:
     >>>     # This is where I keep ubelt on my machine, so it is not expected to work elsewhere.
     >>>     module = ub.import_module_from_path(ub.expandpath('~/code/ubelt/ubelt'))
     >>>     print('module = {!r}'.format(module))
     >>> except OSError:
     >>>     pass
-    >>>         
+    >>>
     >>> module = ub.import_module_from_name('ubelt')
     >>> print('module = {!r}'.format(module))
     >>> #
     >>> try:
     >>>     module = ub.import_module_from_name('does-not-exist')
     >>>     raise AssertionError
     >>> except ModuleNotFoundError:
@@ -1016,16 +1032,16 @@
 
 
 External tools
 --------------
 
 Some of the tools in ``ubelt`` also exist as standalone modules. I haven't
 decided if its best to statically copy them into ubelt or require on pypi to
-satisfy the dependency. There are some tools that are not used by default 
-unless you explicitly allow for them. 
+satisfy the dependency. There are some tools that are not used by default
+unless you explicitly allow for them.
 
 Code that is currently statically included (vendored):
 
 -  ProgIter - https://github.com/Erotemic/progiter
 -  OrderedSet - https://github.com/LuminosoInsight/ordered-set
 
 Code that is completely optional, and only used in specific cases:
@@ -1061,15 +1077,15 @@
 
 * Benedict: dictionary tools - https://pypi.org/project/python-benedict/
 * tqdm: progress bars - https://pypi.org/project/tqdm/
 * pooch: data downloading - https://pypi.org/project/pooch/
 * timerit: snippet timing for benchmarks - https://github.com/Erotemic/timerit
 
 
-Ubelt is included in the the [bestof-python list](https://github.com/ml-tooling/best-of-python), 
+Ubelt is included in the the [bestof-python list](https://github.com/ml-tooling/best-of-python),
 which contains many other tools that you should check out.
 
 
 History:
 ========
 
 Ubelt is a migration of the most useful parts of
@@ -1078,29 +1094,29 @@
 
 The ``utool`` library contains a number of useful utility functions, but it
 also contained non-useful functions, as well as the kitchen sink. A number of
 the functions were too specific or not well documented. The ``ubelt`` is a port
 of the simplest and most useful parts of ``utool``.
 
 Note that there are other cool things in ``utool`` that are not in ``ubelt``.
-Notably, the doctest harness ultimately became `xdoctest <https://github.com/Erotemic/xdoctest>`__. 
+Notably, the doctest harness ultimately became `xdoctest <https://github.com/Erotemic/xdoctest>`__.
 Code introspection and dynamic analysis tools were ported to `xinspect <https://github.com/Erotemic/xinspect>`__.
 The more IPython-y tools were ported to `xdev <https://github.com/Erotemic/xdev>`__.
 Parts of it made their way into `scriptconfig <https://gitlab.kitware.com/utils/scriptconfig>`__.
 The init-file generation was moved to `mkinit <https://github.com/Erotemic/mkinit>`__.
 Some vim and system-y things can be found in `vimtk <https://github.com/Erotemic/vimtk>`__.
 
 Development on ubelt started 2017-01-30 and development of utool mostly stopped
 on utool was stopped later that year, but received patches until about 2020.
 Ubelt achieved 1.0.0 and removed support for Python 2.7 and 3.5 on 2022-01-07.
 
 
 Notes.
 ------
-PRs are welcome. 
+PRs are welcome.
 
 Also check out my other projects which are powered by ubelt:
 
 -  xinspect https://github.com/Erotemic/xinspect
 -  xdev https://github.com/Erotemic/xdev
 -  vimtk https://github.com/Erotemic/vimtk
 -  graphid https://github.com/Erotemic/graphid
@@ -1112,15 +1128,15 @@
 And my projects related to ubelt:
 
 -  ProgIter https://github.com/Erotemic/progiter
 -  Timerit https://github.com/Erotemic/timerit
 -  mkinit https://github.com/Erotemic/mkinit
 -  xdoctest https://github.com/Erotemic/xdoctest
 
-  
+
 
 .. |CircleCI| image:: https://circleci.com/gh/Erotemic/ubelt.svg?style=svg
     :target: https://circleci.com/gh/Erotemic/ubelt
 .. |Travis| image:: https://img.shields.io/travis/Erotemic/ubelt/main.svg?label=Travis%20CI
    :target: https://travis-ci.org/Erotemic/ubelt?branch=main
 .. |Appveyor| image:: https://ci.appveyor.com/api/projects/status/github/Erotemic/ubelt?branch=main&svg=True
    :target: https://ci.appveyor.com/project/Erotemic/ubelt/branch/main
@@ -1128,15 +1144,15 @@
    :target: https://codecov.io/github/Erotemic/ubelt?branch=main
 .. |Pypi| image:: https://img.shields.io/pypi/v/ubelt.svg
    :target: https://pypi.python.org/pypi/ubelt
 .. |Downloads| image:: https://img.shields.io/pypi/dm/ubelt.svg
    :target: https://pypistats.org/packages/ubelt
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/ubelt/badge/?version=latest
     :target: http://ubelt.readthedocs.io/en/latest/
-.. |CodeQuality| image:: https://api.codacy.com/project/badge/Grade/4d815305fc014202ba7dea09c4676343   
+.. |CodeQuality| image:: https://api.codacy.com/project/badge/Grade/4d815305fc014202ba7dea09c4676343
     :target: https://www.codacy.com/manual/Erotemic/ubelt?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Erotemic/ubelt&amp;utm_campaign=Badge_Grade
 .. |GithubActions| image:: https://github.com/Erotemic/ubelt/actions/workflows/tests.yml/badge.svg?branch=main
     :target: https://github.com/Erotemic/ubelt/actions?query=branch%3Amain
 .. |TwitterFollow| image:: https://img.shields.io/twitter/follow/Erotemic.svg?style=social
     :target: https://twitter.com/Erotemic
```

### Comparing `ubelt-1.2.4/README.rst` & `ubelt-1.3.0/ubelt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,89 @@
-|GithubActions| |ReadTheDocs| |Pypi| |Downloads| |Codecov| |CircleCI| |Appveyor| 
+Metadata-Version: 2.1
+Name: ubelt
+Version: 1.3.0
+Summary: A Python utility belt containing simple tools, a stdlib like feel, and extra batteries.
+Home-page: https://github.com/Erotemic/ubelt
+Author: Jon Crall
+Author-email: erotemic@gmail.com
+License: Apache 2
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Typing :: Stubs Only
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
+Provides-Extra: all
+Provides-Extra: all-strict
+Provides-Extra: docs
+Provides-Extra: docs-strict
+Provides-Extra: optional
+Provides-Extra: optional-strict
+Provides-Extra: runtime-strict
+Provides-Extra: tests
+Provides-Extra: tests-strict
+License-File: LICENSE
+
+|GithubActions| |ReadTheDocs| |Pypi| |Downloads| |Codecov| |CircleCI| |Appveyor|
 
 .. .. |CodeQuality| |TwitterFollow|
 
 
 .. The large version wont work because github strips rst image rescaling. https://i.imgur.com/AcWVroL.png
 .. image:: https://i.imgur.com/PoYIsWE.png
    :height: 100px
    :align: left
 
 
 ..   .. raw:: html
 ..       <img src="https://i.imgur.com/AcWVroL.png" height="100px">
 
-Ubelt is a small library of robust, tested, documented, and simple functions
+
+Ubelt is a utility library for Python with a stdlib like feel.
+
+
+Elevator Pitch:
+===============
+
+Is the Python standard library good?  Yes.  Could it's conciseness be improved?  Yes.  Ubelt aims to provide a quicker way to express things you can do in the standard library.  Progress?  `ub.ProgIter <https://ubelt.readthedocs.io/en/latest/ubelt.progiter.html#ubelt.progiter.ProgIter>`_.  Hashing?  `ub.hash_data <https://ubelt.readthedocs.io/en/latest/ubelt.util_hash.html#ubelt.util_hash.hash_data>`_ / `ub.hash_file <https://ubelt.readthedocs.io/en/latest/ubelt.util_hash.html#ubelt.util_hash.hash_file>`_.  Caching?  `ub.Cacher <https://ubelt.readthedocs.io/en/latest/ubelt.util_cache.html#ubelt.util_cache.Cacher>`_ / `ub.CacheStamp <https://ubelt.readthedocs.io/en/latest/ubelt.util_cache.html#ubelt.util_cache.CacheStamp>`_.  Shell commands?  `ub.cmd <https://ubelt.readthedocs.io/en/latest/ubelt.util_cmd.html#ubelt.util_cmd.cmd>`_. There are similar functions for downloading data, futures-based parallel (or serial) job execution, pretty reprs, path management, iteration, and one of my favorites: set operation enriched dictionaries: `ub.udict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.UDict>`_.
+
+There are 120ish functions and classes to help make your code shorter and easier to express concisely.  The library is fast to install and import, all dependencies are optional.  As of 2023 it is 6 years old, regularly maintained, and mature.  It is well tested and has moderate usage.
+
+To learn more, the function usefulness chart is a good place to start.  This shows how often I use particular functions, and while some of the less used ones are candidates for removal, some of them still worth checking out. For a slightly slower start, read the introduction:
+
+
+Introduction:
+=============
+
+Ubelt is a lightweight library of robust, tested, documented, and simple functions
 that extend the Python standard library. It has a flat API that all behaves
 similarly on Windows, Mac, and Linux (up to some small unavoidable
 differences).  Almost every function in ``ubelt`` was written with a doctest.
 This provides helpful documentation and example usage as well as helping
-achieve 100% test coverage (with minor exceptions on Windows). 
+achieve 100% test coverage (with minor exceptions on Windows).
 
 * Goal: provide simple functions that accomplish common tasks not yet addressed by the python standard library.
 
 * Constraints: Must be low-impact pure python; it should be easy to install and use.
 
 * Method: All functions are written with docstrings and doctests to ensure that a baseline level of documentation and testing always exists (even if functions are copy/pasted into other libraries)
 
-* Motto: Good utilities lift all codes. 
+* Motto: Good utilities lift all codes.
 
 
 Read the docs here: http://ubelt.readthedocs.io/en/latest/
 
 These are some of the tasks that ubelt's API enables:
 
   - extended pathlib with expand, ensuredir, endswith, augment, delete (ub.Path)
@@ -50,17 +104,17 @@
 
   - show loop progress with less overhead than tqdm (ProgIter)
 
   - download a file with optional caching and hash verification (download, grabdata)
 
   - run shell commands (cmd)
 
-  - find a file or directory in candidate locations (find_path, find_exe) 
+  - find a file or directory in candidate locations (find_path, find_exe)
 
-  - string-format nested data structures (urepr)
+  - string-repr for nested data structures (urepr)
 
   - color text with ANSI tags (color_text)
 
   - horizontally concatenate multiline strings (hzcat)
 
   - create cross platform symlinks (symlink)
 
@@ -68,15 +122,15 @@
 
   - check if a particular flag or value is on the command line (argflag, argval)
 
   - memoize functions (memoize, memoize_method, memoize_property)
 
   - build ordered sets (oset)
 
-  - argmax/min/sort on lists and dictionaries (argmin, argsort,) 
+  - argmax/min/sort on lists and dictionaries (argmin, argsort,)
 
   - get a histogram of items or find duplicates in a list (dict_hist, find_duplicates)
 
   - group a sequence of items by some criterion (group_items)
 
 Ubelt is small. Its top-level API is defined using roughly 40 lines:
 
@@ -93,15 +147,15 @@
                                  invert_dict, map_keys, map_vals, map_values,
                                  named_product, odict, sdict, sorted_keys,
                                  sorted_vals, sorted_values, udict, varied_values,)
     from ubelt.util_deprecate import (schedule_deprecation,)
     from ubelt.util_download import (download, grabdata,)
     from ubelt.util_download_manager import (DownloadManager,)
     from ubelt.util_func import (compatible, identity, inject_method,)
-    from ubelt.util_format import (FormatterExtensions, repr2, urepr,)
+    from ubelt.util_repr import (ReprExtensions, urepr,)
     from ubelt.util_futures import (Executor, JobPool,)
     from ubelt.util_io import (delete, touch,)
     from ubelt.util_links import (symlink,)
     from ubelt.util_list import (allsame, argmax, argmin, argsort, argunique,
                                  boolmask, chunks, compress, flatten, iter_window,
                                  iterable, peek, take, unique, unique_flags,)
     from ubelt.util_hash import (hash_data, hash_file,)
@@ -135,15 +189,15 @@
 
     pip install ubelt
 
 Note that our distributions on pypi are signed with GPG. The signing public key
 is ``D297D757``; this should agree with the value in `dev/public_gpg_key`.
 
 
-Function Usefulness 
+Function Usefulness
 ===================
 
 When I had to hand pick a set of functions that I thought were the most useful
 I chose these and provided some comment on why:
 
 .. code:: python
 
@@ -159,98 +213,97 @@
     ub.JobPool   # easy multi-threading / multi-procesing / or single-threaded processing
     ub.ProgIter  # a minimal progress iterator. It's single threaded, informative, and faster than tqdm.
     ub.memoize  # like ``functools.cache``, but uses ub.hash_data if the args are not hashable.
     ub.urepr  # readable representations of nested data structures
 
 
 But a better way might to objectively measure the frequency of usage and built
-a histogram of usefulness. I generated this histogram using ``python dev/maintain/gen_api_for_docs.py``, 
+a histogram of usefulness. I generated this histogram using ``python dev/maintain/gen_api_for_docs.py``,
 which roughly counts the number of times I've used a ubelt function in another
 project. Note: this measure is biased towards older functions.
 
 ================================================================================================================================================ ================
  Function name                                                                                                                                         Usefulness
 ================================================================================================================================================ ================
-`ubelt.repr2 <https://ubelt.readthedocs.io/en/latest/ubelt.util_format.html#ubelt.util_format.repr2>`__                                                      2621
-`ubelt.Path <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.Path>`__                                                             903
-`ubelt.ProgIter <https://ubelt.readthedocs.io/en/latest/ubelt.progiter.html#ubelt.progiter.ProgIter>`__                                                       540
-`ubelt.paragraph <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.paragraph>`__                                                     392
-`ubelt.take <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.take>`__                                                             385
-`ubelt.codeblock <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.codeblock>`__                                                     330
-`ubelt.expandpath <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.expandpath>`__                                                 330
-`ubelt.cmd <https://ubelt.readthedocs.io/en/latest/ubelt.util_cmd.html#ubelt.util_cmd.cmd>`__                                                                 279
-`ubelt.ensuredir <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.ensuredir>`__                                                   258
-`ubelt.odict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.odict>`__                                                           255
-`ubelt.iterable <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.iterable>`__                                                     245
-`ubelt.udict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.udict>`__                                                           238
-`ubelt.ddict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.ddict>`__                                                           234
-`ubelt.NoParam <https://ubelt.readthedocs.io/en/latest/ubelt.util_const.html#ubelt.util_const.NoParam>`__                                                     220
-`ubelt.NiceRepr <https://ubelt.readthedocs.io/en/latest/ubelt.util_mixins.html#ubelt.util_mixins.NiceRepr>`__                                                 219
-`ubelt.map_vals <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.map_vals>`__                                                     216
-`ubelt.flatten <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.flatten>`__                                                       208
-`ubelt.dzip <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dzip>`__                                                             201
-`ubelt.peek <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.peek>`__                                                             197
-`ubelt.oset <https://ubelt.readthedocs.io/en/latest/ubelt.orderedset.html#ubelt.orderedset.oset>`__                                                           191
-`ubelt.argflag <https://ubelt.readthedocs.io/en/latest/ubelt.util_arg.html#ubelt.util_arg.argflag>`__                                                         178
-`ubelt.group_items <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.group_items>`__                                               169
-`ubelt.urepr <https://ubelt.readthedocs.io/en/latest/ubelt.util_format.html#ubelt.util_format.urepr>`__                                                       162
-`ubelt.hash_data <https://ubelt.readthedocs.io/en/latest/ubelt.util_hash.html#ubelt.util_hash.hash_data>`__                                                   154
+`ubelt.urepr <https://ubelt.readthedocs.io/en/latest/ubelt.util_repr.html#ubelt.util_repr.urepr>`__                                                          2893
+`ubelt.Path <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.Path>`__                                                             992
+`ubelt.ProgIter <https://ubelt.readthedocs.io/en/latest/ubelt.progiter.html#ubelt.progiter.ProgIter>`__                                                       544
+`ubelt.paragraph <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.paragraph>`__                                                     482
+`ubelt.take <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.take>`__                                                             387
+`ubelt.codeblock <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.codeblock>`__                                                     358
+`ubelt.expandpath <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.expandpath>`__                                                 331
+`ubelt.cmd <https://ubelt.readthedocs.io/en/latest/ubelt.util_cmd.html#ubelt.util_cmd.cmd>`__                                                                 302
+`ubelt.udict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.udict>`__                                                           271
+`ubelt.ensuredir <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.ensuredir>`__                                                   256
+`ubelt.odict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.odict>`__                                                           253
+`ubelt.iterable <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.iterable>`__                                                     252
+`ubelt.ddict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.ddict>`__                                                           238
+`ubelt.NiceRepr <https://ubelt.readthedocs.io/en/latest/ubelt.util_mixins.html#ubelt.util_mixins.NiceRepr>`__                                                 221
+`ubelt.NoParam <https://ubelt.readthedocs.io/en/latest/ubelt.util_const.html#ubelt.util_const.NoParam>`__                                                     216
+`ubelt.map_vals <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.map_vals>`__                                                     215
+`ubelt.flatten <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.flatten>`__                                                       214
+`ubelt.dzip <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dzip>`__                                                             200
+`ubelt.oset <https://ubelt.readthedocs.io/en/latest/ubelt.orderedset.html#ubelt.orderedset.oset>`__                                                           198
+`ubelt.peek <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.peek>`__                                                             196
+`ubelt.argflag <https://ubelt.readthedocs.io/en/latest/ubelt.util_arg.html#ubelt.util_arg.argflag>`__                                                         177
+`ubelt.group_items <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.group_items>`__                                               171
+`ubelt.hash_data <https://ubelt.readthedocs.io/en/latest/ubelt.util_hash.html#ubelt.util_hash.hash_data>`__                                                   165
 `ubelt.grabdata <https://ubelt.readthedocs.io/en/latest/ubelt.util_download.html#ubelt.util_download.grabdata>`__                                             131
+`ubelt.argval <https://ubelt.readthedocs.io/en/latest/ubelt.util_arg.html#ubelt.util_arg.argval>`__                                                           125
 `ubelt.Timer <https://ubelt.readthedocs.io/en/latest/ubelt.util_time.html#ubelt.util_time.Timer>`__                                                           120
 `ubelt.dict_isect <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dict_isect>`__                                                 113
-`ubelt.dict_hist <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dict_hist>`__                                                   112
-`ubelt.argval <https://ubelt.readthedocs.io/en/latest/ubelt.util_arg.html#ubelt.util_arg.argval>`__                                                           110
+`ubelt.dict_hist <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dict_hist>`__                                                   111
 `ubelt.augpath <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.augpath>`__                                                       106
-`ubelt.identity <https://ubelt.readthedocs.io/en/latest/ubelt.util_func.html#ubelt.util_func.identity>`__                                                     105
+`ubelt.identity <https://ubelt.readthedocs.io/en/latest/ubelt.util_func.html#ubelt.util_func.identity>`__                                                     106
 `ubelt.ensure_app_cache_dir <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.ensure_app_cache_dir>`__                     105
-`ubelt.allsame <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.allsame>`__                                                        98
-`ubelt.memoize <https://ubelt.readthedocs.io/en/latest/ubelt.util_memoize.html#ubelt.util_memoize.memoize>`__                                                  97
-`ubelt.color_text <https://ubelt.readthedocs.io/en/latest/ubelt.util_colors.html#ubelt.util_colors.color_text>`__                                              96
+`ubelt.allsame <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.allsame>`__                                                       102
+`ubelt.memoize <https://ubelt.readthedocs.io/en/latest/ubelt.util_memoize.html#ubelt.util_memoize.memoize>`__                                                  99
+`ubelt.color_text <https://ubelt.readthedocs.io/en/latest/ubelt.util_colors.html#ubelt.util_colors.color_text>`__                                              98
 `ubelt.dict_diff <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dict_diff>`__                                                    95
 `ubelt.delete <https://ubelt.readthedocs.io/en/latest/ubelt.util_io.html#ubelt.util_io.delete>`__                                                              89
+`ubelt.hzcat <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.hzcat>`__                                                              88
+`ubelt.schedule_deprecation <https://ubelt.readthedocs.io/en/latest/ubelt.util_deprecate.html#ubelt.util_deprecate.schedule_deprecation>`__                    87
 `ubelt.named_product <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.named_product>`__                                            85
-`ubelt.compress <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.compress>`__                                                      83
-`ubelt.schedule_deprecation <https://ubelt.readthedocs.io/en/latest/ubelt.util_deprecate.html#ubelt.util_deprecate.schedule_deprecation>`__                    77
-`ubelt.IndexableWalker <https://ubelt.readthedocs.io/en/latest/ubelt.util_indexable.html#ubelt.util_indexable.IndexableWalker>`__                              72
-`ubelt.hzcat <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.hzcat>`__                                                              68
+`ubelt.compress <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.compress>`__                                                      85
+`ubelt.IndexableWalker <https://ubelt.readthedocs.io/en/latest/ubelt.util_indexable.html#ubelt.util_indexable.IndexableWalker>`__                              74
 `ubelt.indent <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.indent>`__                                                            68
-`ubelt.JobPool <https://ubelt.readthedocs.io/en/latest/ubelt.util_futures.html#ubelt.util_futures.JobPool>`__                                                  65
+`ubelt.JobPool <https://ubelt.readthedocs.io/en/latest/ubelt.util_futures.html#ubelt.util_futures.JobPool>`__                                                  67
 `ubelt.unique <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.unique>`__                                                          63
 `ubelt.dict_union <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dict_union>`__                                                  57
 `ubelt.map_keys <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.map_keys>`__                                                      49
 `ubelt.invert_dict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.invert_dict>`__                                                48
+`ubelt.iter_window <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.iter_window>`__                                                46
 `ubelt.timestamp <https://ubelt.readthedocs.io/en/latest/ubelt.util_time.html#ubelt.util_time.timestamp>`__                                                    46
-`ubelt.iter_window <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.iter_window>`__                                                44
 `ubelt.argsort <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.argsort>`__                                                        44
 `ubelt.Cacher <https://ubelt.readthedocs.io/en/latest/ubelt.util_cache.html#ubelt.util_cache.Cacher>`__                                                        43
 `ubelt.find_exe <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.find_exe>`__                                              41
 `ubelt.symlink <https://ubelt.readthedocs.io/en/latest/ubelt.util_links.html#ubelt.util_links.symlink>`__                                                      41
 `ubelt.dict_subset <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dict_subset>`__                                                41
 `ubelt.writeto <https://ubelt.readthedocs.io/en/latest/ubelt.util_io.html#ubelt.util_io.writeto>`__                                                            40
-`ubelt.chunks <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.chunks>`__                                                          39
+`ubelt.find_duplicates <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.find_duplicates>`__                                        39
+`ubelt.chunks <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.chunks>`__                                                          38
 `ubelt.hash_file <https://ubelt.readthedocs.io/en/latest/ubelt.util_hash.html#ubelt.util_hash.hash_file>`__                                                    37
 `ubelt.modname_to_modpath <https://ubelt.readthedocs.io/en/latest/ubelt.util_import.html#ubelt.util_import.modname_to_modpath>`__                              37
 `ubelt.ensure_unicode <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.ensure_unicode>`__                                            33
-`ubelt.sorted_vals <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.sorted_vals>`__                                                33
 `ubelt.memoize_property <https://ubelt.readthedocs.io/en/latest/ubelt.util_memoize.html#ubelt.util_memoize.memoize_property>`__                                33
-`ubelt.CacheStamp <https://ubelt.readthedocs.io/en/latest/ubelt.util_cache.html#ubelt.util_cache.CacheStamp>`__                                                32
-`ubelt.find_duplicates <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.find_duplicates>`__                                        32
-`ubelt.highlight_code <https://ubelt.readthedocs.io/en/latest/ubelt.util_colors.html#ubelt.util_colors.highlight_code>`__                                      31
+`ubelt.highlight_code <https://ubelt.readthedocs.io/en/latest/ubelt.util_colors.html#ubelt.util_colors.highlight_code>`__                                      33
+`ubelt.sorted_vals <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.sorted_vals>`__                                                32
+`ubelt.CacheStamp <https://ubelt.readthedocs.io/en/latest/ubelt.util_cache.html#ubelt.util_cache.CacheStamp>`__                                                30
 `ubelt.WIN32 <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.WIN32>`__                                                    28
 `ubelt.import_module_from_name <https://ubelt.readthedocs.io/en/latest/ubelt.util_import.html#ubelt.util_import.import_module_from_name>`__                    27
-`ubelt.argmax <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.argmax>`__                                                          26
-`ubelt.readfrom <https://ubelt.readthedocs.io/en/latest/ubelt.util_io.html#ubelt.util_io.readfrom>`__                                                          24
-`ubelt.import_module_from_path <https://ubelt.readthedocs.io/en/latest/ubelt.util_import.html#ubelt.util_import.import_module_from_path>`__                    21
+`ubelt.argmax <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.argmax>`__                                                          27
+`ubelt.readfrom <https://ubelt.readthedocs.io/en/latest/ubelt.util_io.html#ubelt.util_io.readfrom>`__                                                          23
+`ubelt.import_module_from_path <https://ubelt.readthedocs.io/en/latest/ubelt.util_import.html#ubelt.util_import.import_module_from_path>`__                    22
+`ubelt.compatible <https://ubelt.readthedocs.io/en/latest/ubelt.util_func.html#ubelt.util_func.compatible>`__                                                  17
 `ubelt.touch <https://ubelt.readthedocs.io/en/latest/ubelt.util_io.html#ubelt.util_io.touch>`__                                                                17
+`ubelt.Executor <https://ubelt.readthedocs.io/en/latest/ubelt.util_futures.html#ubelt.util_futures.Executor>`__                                                16
 `ubelt.memoize_method <https://ubelt.readthedocs.io/en/latest/ubelt.util_memoize.html#ubelt.util_memoize.memoize_method>`__                                    16
-`ubelt.Executor <https://ubelt.readthedocs.io/en/latest/ubelt.util_futures.html#ubelt.util_futures.Executor>`__                                                15
-`ubelt.compatible <https://ubelt.readthedocs.io/en/latest/ubelt.util_func.html#ubelt.util_func.compatible>`__                                                  15
 `ubelt.sorted_keys <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.sorted_keys>`__                                                14
+`ubelt.AutoDict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.AutoDict>`__                                                      11
 `ubelt.shrinkuser <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.shrinkuser>`__                                                  11
-`ubelt.AutoDict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.AutoDict>`__                                                      10
 `ubelt.inject_method <https://ubelt.readthedocs.io/en/latest/ubelt.util_func.html#ubelt.util_func.inject_method>`__                                            10
 `ubelt.varied_values <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.varied_values>`__                                             9
 `ubelt.split_modpath <https://ubelt.readthedocs.io/en/latest/ubelt.util_import.html#ubelt.util_import.split_modpath>`__                                         8
 `ubelt.modpath_to_modname <https://ubelt.readthedocs.io/en/latest/ubelt.util_import.html#ubelt.util_import.modpath_to_modname>`__                               8
 `ubelt.get_app_cache_dir <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.get_app_cache_dir>`__                             8
 `ubelt.zopen <https://ubelt.readthedocs.io/en/latest/ubelt.util_zip.html#ubelt.util_zip.zopen>`__                                                               7
 `ubelt.LINUX <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.LINUX>`__                                                     7
@@ -278,26 +331,26 @@
 `ubelt.get_app_data_dir <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.get_app_data_dir>`__                               0
 `ubelt.get_app_config_dir <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.get_app_config_dir>`__                           0
 `ubelt.ensure_app_data_dir <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.ensure_app_data_dir>`__                         0
 `ubelt.ensure_app_config_dir <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.ensure_app_config_dir>`__                     0
 `ubelt.TempDir <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.TempDir>`__                                                         0
 `ubelt.TeeStringIO <https://ubelt.readthedocs.io/en/latest/ubelt.util_stream.html#ubelt.util_stream.TeeStringIO>`__                                             0
 `ubelt.SetDict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.SetDict>`__                                                         0
+`ubelt.ReprExtensions <https://ubelt.readthedocs.io/en/latest/ubelt.util_repr.html#ubelt.util_repr.ReprExtensions>`__                                           0
 `ubelt.POSIX <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.POSIX>`__                                                     0
 `ubelt.OrderedSet <https://ubelt.readthedocs.io/en/latest/ubelt.orderedset.html#ubelt.orderedset.OrderedSet>`__                                                 0
-`ubelt.FormatterExtensions <https://ubelt.readthedocs.io/en/latest/ubelt.util_format.html#ubelt.util_format.FormatterExtensions>`__                             0
 `ubelt.DownloadManager <https://ubelt.readthedocs.io/en/latest/ubelt.util_download_manager.html#ubelt.util_download_manager.DownloadManager>`__                 0
 `ubelt.CaptureStream <https://ubelt.readthedocs.io/en/latest/ubelt.util_stream.html#ubelt.util_stream.CaptureStream>`__                                         0
 ================================================================================================================================================ ================
 
 
 Examples
 ========
 
-The most up to date examples are the doctests. 
+The most up to date examples are the doctests.
 We also have a Jupyter notebook: https://github.com/Erotemic/ubelt/blob/main/docs/notebooks/Ubelt%20Demo.ipynb
 
 Here are some examples of some features inside ``ubelt``
 
 Paths
 -----
 
@@ -349,15 +402,15 @@
 usable and will become better integrated in the future. See
 ``ubelt/util_hash.py`` for details.
 
 Caching
 -------
 
 Cache intermediate results from blocks of code inside a script with minimal
-boilerplate or modification to the original code.  
+boilerplate or modification to the original code.
 
 For direct caching of data, use the ``Cacher`` class.  By default results will
 be written to the ubelt's appdir cache, but the exact location can be specified
 via ``dpath`` or the ``appname`` arguments.  Additionally, process dependencies
 can be specified via the ``depends`` argument, which allows for implicit cache
 invalidation.  As far as I can tell, this is the most concise way (4 lines of
 boilerplate) to cache a block of code with existing Python syntax (as of
@@ -393,61 +446,61 @@
     >>> params = {'params1': 1, 'param2': 2}
     >>> expected_fpath = dpath / 'file.txt'
     >>> stamp = ub.CacheStamp('name', dpath=dpath, depends=params,
     >>>                      hasher='sha256', product=expected_fpath,
     >>>                      expires='2101-01-01T000000Z', verbose=3)
     >>> # Start fresh
     >>> stamp.clear()
-    >>>     
+    >>>
     >>> for _ in range(2):
     >>>     if stamp.expired():
     >>>         expected_fpath.write_text('expensive process')
     >>>         stamp.renew()
 
 See `<https://ubelt.readthedocs.io/en/latest/ubelt.util_cache.html>`_ for more
 details about ``Cacher`` and ``CacheStamp``.
 
 Loop Progress
 -------------
 
 ``ProgIter`` is a no-threads attached Progress meter that writes to stdout.  It
 is a mostly drop-in alternative to `tqdm
-<https://pypi.python.org/pypi/tqdm>`__. 
+<https://pypi.python.org/pypi/tqdm>`__.
 *The advantage of ``ProgIter`` is that it does not use any python threading*,
 and therefore can be safer with code that makes heavy use of multiprocessing.
 
 Note: ``ProgIter`` is also defined in a standalone module: ``pip install progiter``)
 
 .. code:: python
 
     >>> import ubelt as ub
     >>> def is_prime(n):
     ...     return n >= 2 and not any(n % i == 0 for i in range(2, n))
     >>> for n in ub.ProgIter(range(1000), verbose=2):
     >>>     # do some work
     >>>     is_prime(n)
-        0/1000... rate=0.00 Hz, eta=?, total=0:00:00, wall=14:05 EST 
-        1/1000... rate=82241.25 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST 
-      257/1000... rate=177204.69 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST 
-      642/1000... rate=94099.22 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST 
-     1000/1000... rate=71886.74 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST 
+        0/1000... rate=0.00 Hz, eta=?, total=0:00:00, wall=14:05 EST
+        1/1000... rate=82241.25 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST
+      257/1000... rate=177204.69 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST
+      642/1000... rate=94099.22 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST
+     1000/1000... rate=71886.74 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST
 
 
 Command Line Interaction
 ------------------------
 
 The builtin Python ``subprocess.Popen`` module is great, but it can be a
 bit clunky at times. The ``os.system`` command is easy to use, but it
 doesn't have much flexibility. The ``ub.cmd`` function aims to fix this.
 It is as simple to run as ``os.system``, but it returns a dictionary
 containing the return code, standard out, standard error, and the
 ``Popen`` object used under the hood.
 
 This utility is designed to provide as consistent as possible behavior across
-different platforms.  We aim to support Windows, Linux, and OSX. 
+different platforms.  We aim to support Windows, Linux, and OSX.
 
 .. code:: python
 
     >>> import ubelt as ub
     >>> info = ub.cmd('gcc --version')
     >>> print(ub.urepr(info))
     {
@@ -485,15 +538,15 @@
 
 This allows you to easily run a command line executable as part of a
 python process, see what it is doing, and then do something based on its
 output, just as you would if you were interacting with the command line
 itself.
 
 The idea is that ``ub.cmd`` removes the need to think about if you need to pass
-a list of args, or a string. Both will work. 
+a list of args, or a string. Both will work.
 
 New in ``1.0.0``, a third variant with different consequences for executing
 shell commands. Using the ``system=True`` kwarg will directly use ``os.system``
 instead of ``Popen`` entirely. In this mode it is not possible to ``tee`` the
 output because the program is executing directly in the foreground. This is
 useful for doing things like spawning a vim session and returning if the user
 manages to quit vim.
@@ -531,25 +584,25 @@
 provided value. The ``hasher`` keyword argument can be used to change which
 hashing algorithm is used (it defaults to ``"sha512"``).
 
 Dictionary Set Operations
 -------------------------
 
 
-Dictionary operations that are analogous to set operations. 
+Dictionary operations that are analogous to set operations.
 See each funtions documentation for more details on the behavior of the values.
 Typically the last seen value is given priority.
 
-I hope Python decides to add these to the stdlib someday. 
+I hope Python decides to add these to the stdlib someday.
 
 * ``ubelt.dict_union`` corresponds to ``set.union``.
 * ``ubelt.dict_isect`` corresponds to ``set.intersection``.
 * ``ubelt.dict_diff`` corresponds to ``set.difference``.
 
-.. code:: python 
+.. code:: python
 
    >>> d1 = {'a': 1, 'b': 2, 'c': 3}
    >>> d2 = {'c': 10, 'e': 20, 'f': 30}
    >>> d3 = {'e': 10, 'f': 20, 'g': 30, 'a': 40}
    >>> ub.dict_union(d1, d2, d3)
    {'a': 40, 'b': 2, 'c': 10, 'e': 10, 'f': 20, 'g': 30}
 
@@ -557,19 +610,19 @@
    {'c': 3}
 
    >>> ub.dict_diff(d1, d2)
    {'a': 1, 'b': 2}
 
 
 New in Version 1.2.0: Ubelt now contains a dictionary subclass with set
-operations that can be invoked as ``ubelt.SetDict`` or ``ub.sdict``. 
+operations that can be invoked as ``ubelt.SetDict`` or ``ub.sdict``.
 Note that n-ary operations are supported.
 
 
-.. code:: python 
+.. code:: python
 
    >>> d1 = ub.sdict({'a': 1, 'b': 2, 'c': 3})
    >>> d2 = {'c': 10, 'e': 20, 'f': 30}
    >>> d3 = {'e': 10, 'f': 20, 'g': 30, 'a': 40}
    >>> d1 | d2 | d3
    {'a': 40, 'b': 2, 'c': 10, 'e': 10, 'f': 20, 'g': 30}
 
@@ -592,15 +645,15 @@
 id to a list of its corresponding items.  In other words, group a sequence of
 items of type ``VT`` and corresponding keys of type ``KT`` given by a function
 or corresponding list, group them into a ``Dict[KT, List[VT]`` such that each
 key maps to a list of the values associated with the key.  This is similar to
 `pandas.DataFrame.groupby <https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.groupby.html>`_.
 
 Group ids can be specified by a second list containing the id for
-each corresponding item. 
+each corresponding item.
 
 .. code:: python
 
     >>> import ubelt as ub
     >>> # Group via a corresonding list
     >>> item_list    = ['ham',     'jam',   'spam',     'eggs',    'cheese', 'bannana']
     >>> groupid_list = ['protein', 'fruit', 'protein',  'protein', 'dairy',  'fruit']
@@ -620,26 +673,26 @@
     ...     return item.count('a')
     >>> dict(ub.group_items(item_list, grouper))
     {1: ['ham', 'jam', 'spam'], 0: ['eggs', 'cheese'], 3: ['bannana']}
 
 Dictionary Histogram
 --------------------
 
-Find the frequency of items in a sequence. 
+Find the frequency of items in a sequence.
 Given a list or sequence of items, this returns a dictionary mapping each
 unique value in the sequence to the number of times it appeared.
 This is similar to `pandas.DataFrame.value_counts <https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.value_counts.html>`_.
 
 .. code:: python
 
     >>> import ubelt as ub
     >>> item_list = [1, 2, 39, 900, 1232, 900, 1232, 2, 2, 2, 900]
     >>> ub.dict_hist(item_list)
     {1232: 2, 1: 1, 2: 4, 900: 3, 39: 1}
-    
+
 
 Each item can also be given a weight
 
 .. code:: python
 
     >>> import ubelt as ub
     >>> item_list = [1, 2, 39, 900, 1232, 900, 1232, 2, 2, 2, 900]
@@ -715,15 +768,15 @@
     {0: {'A', 'a'}, 1: {'b'}, 2: {'C', 'c'}, 3: {'d'}}
 
 
 New in Version 1.2.0: Ubelt now contains a dictionary subclass ``ubelt.UDict``
 with these quality of life operations (and also inherits from
 ``ubelt.SetDict``). The alias ``ubelt.udict`` can be used for quicker access.
 
-.. code:: python 
+.. code:: python
 
    >>> import ubelt as ub
    >>> d1 = ub.udict({'a': 1, 'b': 2, 'c': 3})
    >>> d1 & {'a', 'c'}
    {'a': 1, 'c': 3}
 
    >>> d1.map_keys(ord)
@@ -741,49 +794,49 @@
 
 Next time you have a default configuration dictionary like and you allow the
 developer to pass keyword arguments to modify these behaviors, consider using
 dictionary intersection (&) to separate out only the relevant parts and
 dictionary union (|) to update those relevant parts.  You can also use
 dictionary differences (-) if you need to check for unused arguments.
 
-.. code:: python 
+.. code:: python
 
     import ubelt as ub
-    
+
     def run_multiple_algos(**kwargs):
         algo1_defaults = {'opt1': 10, 'opt2': 11}
         algo2_defaults = {'src': './here/', 'dst': './there'}
-    
+
         kwargs = ub.udict(kwargs)
-    
+
         algo1_specified = kwargs & algo1_defaults
         algo2_specified = kwargs & algo2_defaults
-    
+
         algo1_config = algo1_defaults | algo1_specified
         algo2_config = algo2_defaults | algo2_specified
-    
+
         unused_kwargs = kwargs - (algo1_defaults | algo2_defaults)
-    
+
         print('algo1_specified = {}'.format(ub.urepr(algo1_specified, nl=1)))
         print('algo2_specified = {}'.format(ub.urepr(algo2_specified, nl=1)))
         print(f'algo1_config={algo1_config}')
         print(f'algo2_config={algo2_config}')
         print(f'The following kwargs were unused {unused_kwargs}')
-    
+
     print(chr(10))
     print('-- Run with some specified --')
     run_multiple_algos(src='box', opt2='fox')
     print(chr(10))
     print('-- Run with extra unspecified --')
     run_multiple_algos(a=1, b=2)
 
 
-Produces: 
+Produces:
 
-.. code:: 
+.. code::
 
     -- Run with some specified --
     algo1_specified = {
         'opt2': 'fox',
     }
     algo2_specified = {
         'src': 'box',
@@ -795,15 +848,15 @@
 
     -- Run with extra unspecified --
     algo1_specified = {}
     algo2_specified = {}
     algo1_config={'opt1': 10, 'opt2': 11}
     algo2_config={'src': './here/', 'dst': './there'}
     The following kwargs were unused {'a': 1, 'b': 2}
-        
+
 
 
 Find Duplicates
 ---------------
 
 Find all duplicate items in a list. More specifically,
 ``ub.find_duplicates`` searches for items that appear more than ``k``
@@ -825,19 +878,19 @@
 the standard place to dump those files differs depending if you are on
 Windows, Linux, or Mac. Ubelt offers a unified functions for determining
 what these paths are.
 
 New in version 1.0.0: the ``ub.Path.appdir`` classmethod provides a way to
 achieve the above with a chainable object oriented interface.
 
-The ``ub.Path.appdir(..., type='cache')``, 
-``ub.Path.appdir(..., type='config')``, and 
+The ``ub.Path.appdir(..., type='cache')``,
+``ub.Path.appdir(..., type='config')``, and
 ``ub.Path.appdir(..., type='data')``
 functions find the correct platform-specific location for these files and
-calling ``ensuredir`` ensures that the directories exist. 
+calling ``ensuredir`` ensures that the directories exist.
 
 The config root directory is ``~/AppData/Roaming`` on Windows,
 ``~/.config`` on Linux and ``~/Library/Application Support`` on Mac. The
 cache root directory is ``~/AppData/Local`` on Windows, ``~/.config`` on
 Linux and ``~/Library/Caches`` on Mac.
 
 Example usage on Linux might look like this:
@@ -893,28 +946,28 @@
 
 Ubelt contains functions to import modules dynamically without using the
 python ``import`` statement. While ``importlib`` exists, the ``ubelt``
 implementation is simpler to user and does not have the disadvantage of
 breaking ``pytest``.
 
 Note ``ubelt`` simply provides an interface to this functionality, the
-core implementation is in ``xdoctest`` (over as of version ``0.7.0``, 
+core implementation is in ``xdoctest`` (over as of version ``0.7.0``,
 the code is statically copied into an autogenerated file such that ``ubelt``
 does not actually depend on ``xdoctest`` during runtime).
 
 .. code:: python
 
     >>> import ubelt as ub
     >>> try:
     >>>     # This is where I keep ubelt on my machine, so it is not expected to work elsewhere.
     >>>     module = ub.import_module_from_path(ub.expandpath('~/code/ubelt/ubelt'))
     >>>     print('module = {!r}'.format(module))
     >>> except OSError:
     >>>     pass
-    >>>         
+    >>>
     >>> module = ub.import_module_from_name('ubelt')
     >>> print('module = {!r}'.format(module))
     >>> #
     >>> try:
     >>>     module = ub.import_module_from_name('does-not-exist')
     >>>     raise AssertionError
     >>> except ModuleNotFoundError:
@@ -979,16 +1032,16 @@
 
 
 External tools
 --------------
 
 Some of the tools in ``ubelt`` also exist as standalone modules. I haven't
 decided if its best to statically copy them into ubelt or require on pypi to
-satisfy the dependency. There are some tools that are not used by default 
-unless you explicitly allow for them. 
+satisfy the dependency. There are some tools that are not used by default
+unless you explicitly allow for them.
 
 Code that is currently statically included (vendored):
 
 -  ProgIter - https://github.com/Erotemic/progiter
 -  OrderedSet - https://github.com/LuminosoInsight/ordered-set
 
 Code that is completely optional, and only used in specific cases:
@@ -1024,15 +1077,15 @@
 
 * Benedict: dictionary tools - https://pypi.org/project/python-benedict/
 * tqdm: progress bars - https://pypi.org/project/tqdm/
 * pooch: data downloading - https://pypi.org/project/pooch/
 * timerit: snippet timing for benchmarks - https://github.com/Erotemic/timerit
 
 
-Ubelt is included in the the [bestof-python list](https://github.com/ml-tooling/best-of-python), 
+Ubelt is included in the the [bestof-python list](https://github.com/ml-tooling/best-of-python),
 which contains many other tools that you should check out.
 
 
 History:
 ========
 
 Ubelt is a migration of the most useful parts of
@@ -1041,29 +1094,29 @@
 
 The ``utool`` library contains a number of useful utility functions, but it
 also contained non-useful functions, as well as the kitchen sink. A number of
 the functions were too specific or not well documented. The ``ubelt`` is a port
 of the simplest and most useful parts of ``utool``.
 
 Note that there are other cool things in ``utool`` that are not in ``ubelt``.
-Notably, the doctest harness ultimately became `xdoctest <https://github.com/Erotemic/xdoctest>`__. 
+Notably, the doctest harness ultimately became `xdoctest <https://github.com/Erotemic/xdoctest>`__.
 Code introspection and dynamic analysis tools were ported to `xinspect <https://github.com/Erotemic/xinspect>`__.
 The more IPython-y tools were ported to `xdev <https://github.com/Erotemic/xdev>`__.
 Parts of it made their way into `scriptconfig <https://gitlab.kitware.com/utils/scriptconfig>`__.
 The init-file generation was moved to `mkinit <https://github.com/Erotemic/mkinit>`__.
 Some vim and system-y things can be found in `vimtk <https://github.com/Erotemic/vimtk>`__.
 
 Development on ubelt started 2017-01-30 and development of utool mostly stopped
 on utool was stopped later that year, but received patches until about 2020.
 Ubelt achieved 1.0.0 and removed support for Python 2.7 and 3.5 on 2022-01-07.
 
 
 Notes.
 ------
-PRs are welcome. 
+PRs are welcome.
 
 Also check out my other projects which are powered by ubelt:
 
 -  xinspect https://github.com/Erotemic/xinspect
 -  xdev https://github.com/Erotemic/xdev
 -  vimtk https://github.com/Erotemic/vimtk
 -  graphid https://github.com/Erotemic/graphid
@@ -1075,15 +1128,15 @@
 And my projects related to ubelt:
 
 -  ProgIter https://github.com/Erotemic/progiter
 -  Timerit https://github.com/Erotemic/timerit
 -  mkinit https://github.com/Erotemic/mkinit
 -  xdoctest https://github.com/Erotemic/xdoctest
 
-  
+
 
 .. |CircleCI| image:: https://circleci.com/gh/Erotemic/ubelt.svg?style=svg
     :target: https://circleci.com/gh/Erotemic/ubelt
 .. |Travis| image:: https://img.shields.io/travis/Erotemic/ubelt/main.svg?label=Travis%20CI
    :target: https://travis-ci.org/Erotemic/ubelt?branch=main
 .. |Appveyor| image:: https://ci.appveyor.com/api/projects/status/github/Erotemic/ubelt?branch=main&svg=True
    :target: https://ci.appveyor.com/project/Erotemic/ubelt/branch/main
@@ -1091,13 +1144,15 @@
    :target: https://codecov.io/github/Erotemic/ubelt?branch=main
 .. |Pypi| image:: https://img.shields.io/pypi/v/ubelt.svg
    :target: https://pypi.python.org/pypi/ubelt
 .. |Downloads| image:: https://img.shields.io/pypi/dm/ubelt.svg
    :target: https://pypistats.org/packages/ubelt
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/ubelt/badge/?version=latest
     :target: http://ubelt.readthedocs.io/en/latest/
-.. |CodeQuality| image:: https://api.codacy.com/project/badge/Grade/4d815305fc014202ba7dea09c4676343   
+.. |CodeQuality| image:: https://api.codacy.com/project/badge/Grade/4d815305fc014202ba7dea09c4676343
     :target: https://www.codacy.com/manual/Erotemic/ubelt?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Erotemic/ubelt&amp;utm_campaign=Badge_Grade
 .. |GithubActions| image:: https://github.com/Erotemic/ubelt/actions/workflows/tests.yml/badge.svg?branch=main
     :target: https://github.com/Erotemic/ubelt/actions?query=branch%3Amain
 .. |TwitterFollow| image:: https://img.shields.io/twitter/follow/Erotemic.svg?style=social
     :target: https://twitter.com/Erotemic
+
+
```

### Comparing `ubelt-1.2.4/pyproject.toml` & `ubelt-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/setup.py` & `ubelt-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt/__init__.py` & `ubelt-1.3.0/ubelt/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,25 +20,27 @@
     mkinit ubelt -w  # todo: get sphinx to ignore this
     # TODO: Lazy imports with mkinit (requires python 3.7)
 
 Testing:
     xdoctest ubelt
 """
 
-__version__ = '1.2.4'
+__version__ = '1.3.0'
 
 # Deprecated functions
 from ubelt.util_platform import (
     ensure_app_cache_dir, ensure_app_config_dir,
     ensure_app_data_dir, get_app_cache_dir, get_app_config_dir,
     get_app_data_dir,
 )
 
 from ubelt.util_io import (readfrom, writeto,)
 from ubelt.util_str import (ensure_unicode,)
+from ubelt import util_format
+from ubelt.util_format import FormatterExtensions, repr2
 
 
 __ignore__ = [
     'ensure_app_cache_dir',
     'ensure_app_config_dir',
     'ensure_app_data_dir',
     'get_app_cache_dir',
@@ -55,29 +57,32 @@
     'ensure_app_data_dir',
     'get_app_cache_dir',
     'get_app_config_dir',
     'get_app_data_dir',
     'readfrom',
     'writeto',
     'ensure_unicode',
+    'util_format',
+    'repr2',
+    'FormatterExtensions',
 ]
 
 
 __submodules__ = {
     'util_arg': None,
     'util_cache': None,
     'util_colors': None,
     'util_const': None,
     'util_cmd': None,
     'util_dict': None,
     'util_deprecate': None,
     'util_download': None,
     'util_download_manager': None,
     'util_func': None,
-    'util_format': None,
+    'util_repr': None,
     'util_futures': None,
     'util_io': None,
     'util_links': None,
     'util_list': None,
     'util_hash': None,
     'util_import': None,
     'util_indexable': None,
@@ -100,27 +105,27 @@
 from ubelt import util_cmd
 from ubelt import util_colors
 from ubelt import util_const
 from ubelt import util_deprecate
 from ubelt import util_dict
 from ubelt import util_download
 from ubelt import util_download_manager
-from ubelt import util_format
 from ubelt import util_func
 from ubelt import util_futures
 from ubelt import util_hash
 from ubelt import util_import
 from ubelt import util_indexable
 from ubelt import util_io
 from ubelt import util_links
 from ubelt import util_list
 from ubelt import util_memoize
 from ubelt import util_mixins
 from ubelt import util_path
 from ubelt import util_platform
+from ubelt import util_repr
 from ubelt import util_str
 from ubelt import util_stream
 from ubelt import util_time
 from ubelt import util_zip
 
 from ubelt.util_arg import (argflag, argval,)
 from ubelt.util_cache import (CacheStamp, Cacher,)
@@ -133,15 +138,15 @@
                              invert_dict, map_keys, map_vals, map_values,
                              named_product, odict, sdict, sorted_keys,
                              sorted_vals, sorted_values, udict, varied_values,)
 from ubelt.util_deprecate import (schedule_deprecation,)
 from ubelt.util_download import (download, grabdata,)
 from ubelt.util_download_manager import (DownloadManager,)
 from ubelt.util_func import (compatible, identity, inject_method,)
-from ubelt.util_format import (FormatterExtensions, repr2, urepr,)
+from ubelt.util_repr import (ReprExtensions, urepr,)
 from ubelt.util_futures import (Executor, JobPool,)
 from ubelt.util_io import (delete, touch,)
 from ubelt.util_links import (symlink,)
 from ubelt.util_list import (allsame, argmax, argmin, argsort, argunique,
                              boolmask, chunks, compress, flatten, iter_window,
                              iterable, peek, take, unique, unique_flags,)
 from ubelt.util_hash import (hash_data, hash_file,)
@@ -163,36 +168,37 @@
 from ubelt.orderedset import (OrderedSet, oset,)
 from ubelt.progiter import (ProgIter,)
 
 __all__ = ['AutoDict', 'AutoOrderedDict', 'CacheStamp', 'Cacher',
            'CaptureStdout', 'CaptureStream', 'DARWIN', 'DownloadManager',
            'Executor', 'FormatterExtensions', 'IndexableWalker', 'JobPool',
            'LINUX', 'NO_COLOR', 'NiceRepr', 'NoParam', 'OrderedSet', 'POSIX',
-           'Path', 'ProgIter', 'SetDict', 'TeeStringIO', 'TempDir', 'Timer',
-           'UDict', 'WIN32', 'allsame', 'argflag', 'argmax', 'argmin',
-           'argsort', 'argunique', 'argval', 'augpath', 'boolmask', 'chunks',
-           'cmd', 'codeblock', 'color_text', 'compatible', 'compress', 'ddict',
-           'delete', 'dict_diff', 'dict_hist', 'dict_isect', 'dict_subset',
-           'dict_union', 'download', 'dzip', 'ensure_app_cache_dir',
-           'ensure_app_config_dir', 'ensure_app_data_dir', 'ensure_unicode',
-           'ensuredir', 'expandpath', 'find_duplicates', 'find_exe',
-           'find_path', 'flatten', 'get_app_cache_dir', 'get_app_config_dir',
-           'get_app_data_dir', 'grabdata', 'group_items', 'hash_data',
-           'hash_file', 'highlight_code', 'hzcat', 'identity',
-           'import_module_from_name', 'import_module_from_path', 'indent',
-           'indexable_allclose', 'inject_method', 'invert_dict', 'iter_window',
-           'iterable', 'map_keys', 'map_vals', 'map_values', 'memoize',
-           'memoize_method', 'memoize_property', 'modname_to_modpath',
-           'modpath_to_modname', 'named_product', 'odict', 'orderedset',
-           'oset', 'paragraph', 'peek', 'platform_cache_dir',
-           'platform_config_dir', 'platform_data_dir', 'progiter', 'readfrom',
-           'repr2', 'schedule_deprecation', 'sdict', 'shrinkuser',
-           'sorted_keys', 'sorted_vals', 'sorted_values', 'split_archive',
-           'split_modpath', 'symlink', 'take', 'timeparse', 'timestamp',
-           'touch', 'udict', 'unique', 'unique_flags', 'userhome', 'urepr',
-           'util_arg', 'util_cache', 'util_cmd', 'util_colors', 'util_const',
-           'util_deprecate', 'util_dict', 'util_download',
+           'Path', 'ProgIter', 'ReprExtensions', 'SetDict', 'TeeStringIO',
+           'TempDir', 'Timer', 'UDict', 'WIN32', 'allsame', 'argflag',
+           'argmax', 'argmin', 'argsort', 'argunique', 'argval', 'augpath',
+           'boolmask', 'chunks', 'cmd', 'codeblock', 'color_text',
+           'compatible', 'compress', 'ddict', 'delete', 'dict_diff',
+           'dict_hist', 'dict_isect', 'dict_subset', 'dict_union', 'download',
+           'dzip', 'ensure_app_cache_dir', 'ensure_app_config_dir',
+           'ensure_app_data_dir', 'ensure_unicode', 'ensuredir', 'expandpath',
+           'find_duplicates', 'find_exe', 'find_path', 'flatten',
+           'get_app_cache_dir', 'get_app_config_dir', 'get_app_data_dir',
+           'grabdata', 'group_items', 'hash_data', 'hash_file',
+           'highlight_code', 'hzcat', 'identity', 'import_module_from_name',
+           'import_module_from_path', 'indent', 'indexable_allclose',
+           'inject_method', 'invert_dict', 'iter_window', 'iterable',
+           'map_keys', 'map_vals', 'map_values', 'memoize', 'memoize_method',
+           'memoize_property', 'modname_to_modpath', 'modpath_to_modname',
+           'named_product', 'odict', 'orderedset', 'oset', 'paragraph', 'peek',
+           'platform_cache_dir', 'platform_config_dir', 'platform_data_dir',
+           'progiter', 'readfrom', 'repr2', 'schedule_deprecation', 'sdict',
+           'shrinkuser', 'sorted_keys', 'sorted_vals', 'sorted_values',
+           'split_archive', 'split_modpath', 'symlink', 'take', 'timeparse',
+           'timestamp', 'touch', 'udict', 'unique', 'unique_flags', 'urepr',
+           'userhome', 'util_arg', 'util_cache', 'util_cmd', 'util_colors',
+           'util_const', 'util_deprecate', 'util_dict', 'util_download',
            'util_download_manager', 'util_format', 'util_func', 'util_futures',
            'util_hash', 'util_import', 'util_indexable', 'util_io',
            'util_links', 'util_list', 'util_memoize', 'util_mixins',
-           'util_path', 'util_platform', 'util_str', 'util_stream',
-           'util_time', 'util_zip', 'varied_values', 'writeto', 'zopen']
+           'util_path', 'util_platform', 'util_repr', 'util_str',
+           'util_stream', 'util_time', 'util_zip', 'varied_values', 'writeto',
+           'zopen']
```

### Comparing `ubelt-1.2.4/ubelt/_win32_links.py` & `ubelt-1.3.0/ubelt/_win32_links.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt/orderedset.py` & `ubelt-1.3.0/ubelt/orderedset.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt/orderedset.pyi` & `ubelt-1.3.0/ubelt/orderedset.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -26,24 +26,24 @@
 
     def __contains__(self, key):
         ...
 
     def add(self, key):
         ...
 
-    append: Incomplete
+    append = add
 
     def update(self, sequence):
         ...
 
     def index(self, key):
         ...
 
-    get_loc: Incomplete
-    get_indexer: Incomplete
+    get_loc = index
+    get_indexer = index
 
     def pop(self):
         ...
 
     def discard(self, key) -> None:
         ...
```

### Comparing `ubelt-1.2.4/ubelt/progiter.py` & `ubelt-1.3.0/ubelt/progiter.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt/progiter.pyi` & `ubelt-1.3.0/ubelt/util_futures.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,163 +1,105 @@
-from typing import Union
-from typing import Iterable
+import concurrent
+import concurrent.futures
+from typing import Callable
+from typing import Any
 from typing import List
-import typing
+import concurrent.futures
 from _typeshed import Incomplete
+from collections.abc import Generator
+from typing import Any
 
-default_timer: Incomplete
-CLEAR_BEFORE: str
-AT_END: str
 
+class SerialFuture(concurrent.futures.Future):
+    func: Incomplete
+    args: Incomplete
+    kw: Incomplete
 
-class _TQDMCompat:
-
-    @classmethod
-    def write(cls,
-              s,
-              file: Incomplete | None = ...,
-              end: str = ...,
-              nolock: bool = ...) -> None:
-        ...
-
-    desc: Incomplete
-
-    def set_description(self,
-                        desc: Incomplete | None = ...,
-                        refresh: bool = ...) -> None:
-        ...
-
-    def set_description_str(self,
-                            desc: Incomplete | None = ...,
-                            refresh: bool = ...) -> None:
+    def __init__(self, func, *args, **kw) -> None:
         ...
 
-    def update(self, n: int = ...) -> None:
+    def set_result(self, result) -> None:
         ...
 
-    def close(self) -> None:
-        ...
 
-    def unpause(self) -> None:
-        ...
+class SerialExecutor:
+    max_workers: int
 
-    def moveto(self, n) -> None:
+    def __enter__(self):
         ...
 
-    def clear(self, nolock: bool = ...) -> None:
+    def __exit__(self, ex_type, ex_value, tb) -> None:
         ...
 
-    def refresh(self, nolock: bool = ...) -> None:
+    def submit(self, func, *args, **kw) -> concurrent.futures.Future:
         ...
 
-    @property
-    def pos(self):
+    def shutdown(self) -> None:
         ...
 
-    @classmethod
-    def set_lock(cls, lock) -> None:
+    def map(self, fn: Callable[..., Any], *iterables,
+            **kwargs) -> Generator[Any, None, None]:
         ...
 
-    @classmethod
-    def get_lock(cls) -> None:
-        ...
 
-    def set_postfix(self,
-                    ordered_dict: Incomplete | None = ...,
-                    refresh: bool = ...,
-                    **kwargs) -> None:
-        ...
+class Executor:
+    backend: Incomplete
 
-    def set_postfix_str(self, s: str = ..., refresh: bool = ...) -> None:
+    def __init__(self, mode: str = 'thread', max_workers: int = 0) -> None:
         ...
 
-
-class _BackwardsCompat:
-
-    @property
-    def length(self):
+    def __enter__(self):
         ...
 
-    @property
-    def label(self):
+    def __exit__(self, ex_type, ex_value, tb):
         ...
 
-
-class ProgIter(_TQDMCompat, _BackwardsCompat):
-    iterable: Union[List, Iterable]
-    desc: str
-    total: int
-    freq: int
-    adjust: bool
-    eta_window: int
-    clearline: bool
-    time_thresh: float
-    show_times: bool
-    show_wall: bool
-    initial: int
-    stream: typing.IO
-    enabled: bool
-    chunksize: Union[int, None]
-    rel_adjust_limit: float
-    verbose: int
-    extra: str
-    started: bool
-    finished: bool
-
-    def __init__(self,
-                 iterable: Incomplete | None = ...,
-                 desc: Incomplete | None = ...,
-                 total: Incomplete | None = ...,
-                 freq: int = ...,
-                 initial: int = ...,
-                 eta_window: int = ...,
-                 clearline: bool = ...,
-                 adjust: bool = ...,
-                 time_thresh: float = ...,
-                 show_times: bool = ...,
-                 show_wall: bool = ...,
-                 enabled: bool = ...,
-                 verbose: Incomplete | None = ...,
-                 stream: Incomplete | None = ...,
-                 chunksize: Incomplete | None = ...,
-                 rel_adjust_limit: float = ...,
-                 **kwargs) -> None:
+    def submit(self, func, *args, **kw) -> concurrent.futures.Future:
         ...
 
-    def __call__(self, iterable):
+    def shutdown(self):
         ...
 
-    def __enter__(self):
+    def map(self, fn, *iterables, **kwargs):
         ...
 
-    def __exit__(self, type_, value, trace):
-        ...
 
-    def __iter__(self):
-        ...
+class JobPool:
+    executor: Incomplete
+    transient: Incomplete
+    jobs: Incomplete
 
-    def set_extra(self, extra) -> None:
+    def __init__(self,
+                 mode: str = ...,
+                 max_workers: int = ...,
+                 transient: bool = ...) -> None:
         ...
 
-    def step(self, inc: int = 1, force: bool = False) -> None:
+    def __len__(self):
         ...
 
-    def start(self):
+    def submit(self, func: Callable[..., Any], *args,
+               **kwargs) -> concurrent.futures.Future:
         ...
 
-    def begin(self) -> ProgIter:
+    def shutdown(self):
         ...
 
-    def end(self) -> None:
+    def __enter__(self):
         ...
 
-    def format_message(self):
+    def __exit__(self, a, b, c) -> None:
         ...
 
-    def format_message_parts(self):
+    def as_completed(
+        self,
+        timeout: float | None = None,
+        desc: str | None = None,
+        progkw: dict | None = None
+    ) -> Generator[concurrent.futures.Future, None, None]:
         ...
 
-    def ensure_newline(self) -> None:
+    def join(self, **kwargs) -> List[Any]:
         ...
 
-    def display_message(self) -> None:
+    def __iter__(self):
         ...
```

### Comparing `ubelt-1.2.4/ubelt/util_arg.py` & `ubelt-1.3.0/ubelt/util_arg.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt/util_cache.py` & `ubelt-1.3.0/ubelt/util_cache.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt/util_cmd.py` & `ubelt-1.3.0/ubelt/util_cmd.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,14 +27,62 @@
         'command': 'echo "write your command naturally"',
         'cwd': None,
         'err': '',
         'out': 'write your command naturally\n',
         'proc': <...Popen...>,
         'ret': 0,
     }
+
+
+The cmd is able to handle common uses cases of the subprocess module with a
+simpler interface.
+
+.. code:: python
+
+    import subprocess
+    import ubelt as ub
+
+Run without capturing output and without printing to the screen
+
+.. code:: python
+
+    # stdlib
+    subprocess.run(['ls', '-l'], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL, universal_newlines=True)
+
+    # ubelt equivalent
+    ub.cmd(['ls', '-l'], capture=False)
+
+Print output to the screen, but no programmatic access to the data
+
+.. code:: python
+
+    # stdlib
+    subprocess.check_call(['ls', '-l'])
+
+    # ubelt equivalent
+    ub.cmd(['ls', '-l'], verbose=1, capture=False)
+
+Get programmatic access to the data but don't show it on screen
+
+.. code:: python
+
+    # stdlib
+    subprocess.check_output(['ls', '-l'], universal_newlines=True)
+
+    # ubelt equivalent
+    ub.cmd(['ls', '-l'])['out']
+
+Get programatic access AND show it on screen
+
+.. code:: python
+
+    # stdlib has no easy way to to this
+
+    # ubelt has "tee" functionality
+    ub.cmd(['ls', '-l'], verbose=1)
 """
 import sys
 import os
 
 
 __pitch__ = """
 The ubelt.cmd command is probably the easiest way to execute a command line program from Python. Unlike os.system, subprocess.check_output, and subprocess.call, The syntax for what you want to call is exactly the same no matter what type of configuration you are using.
@@ -56,16 +104,47 @@
 
 __all__ = ['cmd']
 
 POSIX = 'posix' in sys.builtin_module_names
 WIN32 = sys.platform == 'win32'
 
 
+class CmdOutput(dict):
+    """
+    An container that holds the output of :func:`ubelt.cmd`.
+
+    This inherits from dictionary to be backwards compatible with older
+    versions of ubelt, but also includes methods that ducktype the stdlib
+    :class:`subprocess.CompletedProcess`, which makes it easier for existing
+    code that uses :func:`subprocess.run` to switch to :func:`ubelt.cmd`.
+    """
+
+    @property
+    def stdout(self):
+        return self['out']
+
+    @property
+    def stderr(self):
+        return self['err']
+
+    @property
+    def returncode(self):
+        return self['ret']
+
+    def check_returncode(self):
+        """Raise CalledProcessError if the exit code is non-zero."""
+        import subprocess
+        if self.returncode:
+            raise subprocess.CalledProcessError(
+                self.returncode, self.args, self.stdout, self.stderr)
+
+
 def cmd(command, shell=False, detach=False, verbose=0, tee=None, cwd=None,
-        env=None, tee_backend='auto', check=False, system=False, timeout=None):
+        env=None, tee_backend='auto', check=False, system=False, timeout=None,
+        capture=True):
     """
     Executes a command in a subprocess.
 
     The advantage of this wrapper around subprocess is that
     (1) you control if the subprocess prints to stdout,
     (2) the text written to stdout and stderr is returned for parsing,
     (3) cross platform behavior that lets you specify the command as a string
@@ -109,21 +188,20 @@
         system (bool, default=False):
             if True, most other considerations are dropped, and
             :func:`os.system` is used to execute the command in a platform
             dependant way. Other arguments such as env, tee, timeout, and shell
             are all ignored.  (new in version 1.1.0)
 
         timeout (float | None):
-            If the process does not complete in `timeout` seconds, raises a
-            :class:`subprocess.TimeoutExpired`. (new in version 1.1.0)
-            Currently unhandled when tee is True.
-
-        log (Callable | None):
-            If specified, verbose output is written using this function,
-            otherwise the builtin print function is used.
+            If the process does not complete in ``timeout`` seconds, raise a
+            :class:`subprocess.TimeoutExpired`. (new in version 1.1.0).
+
+        capture (bool):
+            if True, the stdout/stderr are captured and returned in the
+            information dictionary. Ignored if detatch or system is True.
 
     Returns:
         dict:
             info - information about command status.
             if detach is False ``info`` contains captured standard out,
             standard error, and the return code
             if detach is True ``info`` contains a reference to the process.
@@ -225,38 +303,42 @@
         >>> info = ub.cmd('echo hi', check=True, system=True)
         >>> with pytest.raises(subprocess.CalledProcessError):
         >>>     ub.cmd('exit 1', check=True, shell=True)
     """
     # In the future we might allow the user to pass a custom log function
     # But this has weird interactions with how the tee process works
     # because of the assumption stdout.write does not emit a newline
+    # TODO:
+    # log (Callable | None):
+    #     If specified, verbose output is written using this function,
+    #     otherwise the builtin print function is used.
     log = print
 
     import subprocess
     # TODO: stdout, stderr - experimental - custom file to pipe stdout/stderr to
     # Determine if command is specified as text or a tuple
     if isinstance(command, str):
         command_text = command
         command_tup = None
     else:
-        import pipes
+        import shlex
         command_parts = []
         # Allow the user to specify paths as part of the command
         for part in command:
             if isinstance(part, os.PathLike):
                 part = os.fspath(part)
             command_parts.append(part)
-        command_tup = tuple(command_parts)
-        command_text = ' '.join(list(map(pipes.quote, command_tup)))
+        command_tup = list(command_parts)
+        command_text = ' '.join(list(map(shlex.quote, command_tup)))
 
     # Inputs can either be text or tuple based. On UNIX we ensure conversion
     # to text if shell is True, and to tuple if shell is False. On windows,
     # the input is text if shell is True, but can be either if shell is
     # False as noted in [SO_33560364]_.
-    if shell:
+    if shell or system:
         # When shell=True, args is sent to the shell (e.g. bin/sh) as text
         args = command_text
     else:
         # When shell=False, args is a list of executable and arguments
         if command_tup is None:
             if sys.platform.startswith('win32'):  # nocover
                 # On windows when shell=False, args can be a str | List[str]
@@ -271,14 +353,25 @@
 
     if tee is None:
         tee = verbose > 0
 
     if tee and tee_backend not in {'auto', 'thread', 'select'}:
         raise ValueError('tee_backend must be select, thread, or auto')
 
+    # note: we use ``tee`` as a proxy for "show"
+    # we may upgrade show to an actual argument
+    show = tee
+
+    if show and not capture:
+        # even though tee was probably true, semantically it should be
+        # considered false unless we are doing both.
+        # when show becomes an arguments we should do error handling for
+        # inconsistency here
+        tee = False
+
     if verbose > 1:
         import platform
         import getpass
         from ubelt import shrinkuser
         if verbose > 2:
             try:
                 log('┌─── START CMD ───')
@@ -290,75 +383,111 @@
         cwd_ = shrinkuser(cwd_)
         ps1 = '[ubelt.cmd] {}@{}:{}$ '.format(username, compname, cwd_)
         log(ps1 + command_text)
 
     # Create a new process to execute the command
     def make_proc():
         # delay the creation of the process until we validate all args
-        proc = subprocess.Popen(args, stdout=subprocess.PIPE,
-                                stderr=subprocess.PIPE, shell=shell,
-                                universal_newlines=True, cwd=cwd, env=env)
+        popen_kwargs = {'cwd': cwd, 'env': env, 'shell': shell}
+        popen_kwargs['universal_newlines'] = True
+
+        if capture:
+            popen_kwargs['stdout'] = subprocess.PIPE
+            popen_kwargs['stderr'] = subprocess.PIPE
+        elif not show:
+            # The only way to suppress printing to the screen is by
+            # piping to devnull
+            popen_kwargs['stdout'] = subprocess.DEVNULL
+            popen_kwargs['stderr'] = subprocess.DEVNULL
+        proc = subprocess.Popen(args, **popen_kwargs)
         return proc
 
     if system:
-        info = {
-            'command': command_text,
-            'out': None,
-            'err': None,
-        }
         from ubelt.util_path import ChDir
         with ChDir(cwd):
             ret = os.system(command_text)
-        info['ret'] = ret
+        info = CmdOutput(**{
+            'out': None,
+            'err': None,
+            'ret': ret,
+            'cwd': cwd,
+            'command': command_text,
+        })
     elif detach:
-        info = {'proc': make_proc(), 'command': command_text}
-        if verbose > 0:  # nocover
+        info = CmdOutput(**{
+            # Not including out/err/ret because the user could still compute
+            # them via proc. I'm open to reconsidering this design decision.
+            'proc': make_proc(),
+            'cwd': cwd,
+            'command': command_text
+        })
+        if verbose > 1:  # nocover
             log('...detaching')
     else:
         if tee:
+            # tee means both capture and show are true.
             # We logging stdout and stderr, while simultaneously piping it to
             # another stream.
             stdout = sys.stdout
             stderr = sys.stderr
             proc = make_proc()
             with proc:
                 out, err = _tee_output(
                     proc=proc, stdout=stdout, stderr=stderr,
                     backend=tee_backend, timeout=timeout,
                     command_text=command_text)
                 (out_, err_) = proc.communicate(timeout=timeout)
-        else:
+        elif capture:
             proc = make_proc()
+            # Follow the error handling in the stdlib implementation of
+            # subprocess.run
             with proc:
                 try:
                     (out, err) = proc.communicate(timeout=timeout)
                 except subprocess.TimeoutExpired as exc:
-                    # Follow the error handling in the stdlib implementation of
-                    # subprocess.run
                     proc.kill()
                     if WIN32:  # nocover
                         # Win32 needs a communicate after the kill to get the
                         # output. See stdlib for details.
                         exc.stdout, exc.stderr = proc.communicate()
                     else:
                         # Posix implementations already handle the populate.
                         proc.wait()
                     raise
+        else:
+            # Not capturing output, but it might print to the screen
+            # i.e. capture is False, but show might be True or False
+            proc = make_proc()
+            out = None
+            err = None
+            # Follow the error handling in the stdlib implementation of
+            # subprocess.call
+            with proc:
+                try:
+                    proc.wait(timeout=timeout)
+                except:  # NOQA  # Including KeyboardInterrupt, wait handled that.
+                    proc.kill()
+                    # We don't call p.wait() again as p.__exit__ does that for us.
+                    raise
+
         # We used the popen context manager, which means that wait was called,
         # the process has existed, so it is safe to return a reference to the
         # process object.
         ret = proc.poll()
-        info = {
+        info = CmdOutput(**{
             'out': out,
             'err': err,
             'ret': ret,
             'proc': proc,
             'cwd': cwd,
-            'command': command_text
-        }
+            'command': command_text,
+        })
+
+    # For subprocess compatability
+    info.args = args
 
     if not detach:
         if verbose > 2:
             # https://en.wikipedia.org/wiki/Box-drawing_character
             try:
                 log('└─── END CMD ───')
             except Exception:  # nocover
@@ -671,15 +800,14 @@
         _proc_iteroutput = _proc_iteroutput_thread
     else:  # nocover
         # The value of "backend" should be checked before we create the
         # processes, otherwise we will have a dangling process
         raise AssertionError(
             'Invalid backend, but the check should have already a happened')
 
-    # TODO: handle timeout
     output_gen = _proc_iteroutput(proc, timeout=timeout)
     # logger.debug("Start waiting for buffered output")
     for oline, eline in output_gen:
         if timeout is not None:
             if oline is subprocess.TimeoutExpired or eline is subprocess.TimeoutExpired:
                 # logger.error("Timeout error triggered!")
                 try:
```

### Comparing `ubelt-1.2.4/ubelt/util_colors.py` & `ubelt-1.3.0/ubelt/util_colors.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt/util_const.py` & `ubelt-1.3.0/ubelt/util_const.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 :data:`NoParam` is robust to reloading, pickling, and copying (i.e. ``var is
 ub.NoParam`` will return ``True`` after these operations).
 
 Use cases that demonstrate the value of :data:`NoParam` can be found in
 :mod:`ubelt.util_dict`, where it simplifies the implementation of methods that
 behave like :meth:`dict.get`.
 
+The value of :data:`NoParam` is robust to reloading, pickling, and copying. See
+[SO_41048643]_ for more details.
+
+References:
+    .. [SO_41048643]: http://stackoverflow.com/questions/41048643/a-second-none
+
 Example:
     >>> import ubelt as ub
     >>> def func(a=ub.NoParam):
     >>>     if a is ub.NoParam:
     >>>         print('no param specified')
     >>>     else:
     >>>         print('a = {}'.format(a))
```

### Comparing `ubelt-1.2.4/ubelt/util_deprecate.py` & `ubelt-1.3.0/ubelt/util_deprecate.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt/util_dict.py` & `ubelt-1.3.0/ubelt/util_dict.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     .. [GHDictMap] https://github.com/ulisesojeda/dictionary_map
 """
 import sys
 import operator as op
 import itertools as it
 from collections import OrderedDict
 from collections import defaultdict
-# from ubelt import util_const
 from ubelt.util_const import NoParam
 
 __all__ = [
     'AutoDict',
     'AutoOrderedDict',
     'dzip',
     'ddict',
@@ -110,15 +109,15 @@
     Args:
         items1 (Iterable[KT]): full sequence
 
         items2 (Iterable[VT]):
             can either be a sequence of one item or a sequence of equal length
             to ``items1``
 
-        cls (Type[dict], default=dict): dictionary type to use.
+        cls (Type[dict]): dictionary type to use. Defaults to ``dict``.
 
     Returns:
         Dict[KT, VT]: similar to ``dict(zip(items1, items2))``.
 
     Example:
         >>> import ubelt as ub
         >>> assert ub.dzip([1, 2, 3], [4]) == {1: 4, 2: 4, 3: 4}
@@ -190,24 +189,27 @@
     Builds a histogram of items, counting the number of time each item appears
     in the input.
 
     Args:
         items (Iterable[T]):
             hashable items (usually containing duplicates)
 
-        weights (Iterable[float] | None, default=None):
+        weights (Iterable[float] | None):
             Corresponding weights for each item, defaults to 1 if unspecified.
+            Defaults to None.
 
-        ordered (bool, default=False):
+        ordered (bool):
             If True the result is ordered by frequency.
+            Defaults to False.
 
-        labels (Iterable[T] | None, default=None):
+        labels (Iterable[T] | None):
             Expected labels.  Allows this function to pre-initialize the
             histogram.  If specified the frequency of each label is initialized
             to zero and ``items`` can only contain items specified in labels.
+            Defaults to None.
 
     Returns:
         dict[T, int] :
             dictionary where the keys are unique elements from ``items``, and
             the values are the number of times the item appears in ``items``.
 
     SeeAlso:
@@ -269,26 +271,27 @@
     Find all duplicate items in a list.
 
     Search for all items that appear more than ``k`` times and return a mapping
     from each (k)-duplicate item to the positions it appeared in.
 
     Args:
         items (Iterable[T]):
-            hashable items possibly containing duplicates
+            Hashable items possibly containing duplicates
 
-        k (int, default=2):
-            only return items that appear at least ``k`` times.
+        k (int):
+            Only return items that appear at least ``k`` times.
+            Defaults to 2.
 
-        key (Callable[[T], Any] | None, default=None):
+        key (Callable[[T], Any] | None):
             Returns indices where `key(items[i])` maps to a particular value at
-            least k times.
+            least k times. Default to None.
 
     Returns:
         dict[T, List[int]] :
-            maps each duplicate item to the indices at which it appears
+            Maps each duplicate item to the indices at which it appears
 
     Notes:
         Similar to :func:`more_itertools.duplicates_everseen`,
         :func:`more_itertools.duplicates_justseen`.
 
     Example:
         >>> import ubelt as ub
@@ -340,15 +343,16 @@
         dict_ (Dict[KT, VT]): superset dictionary
 
         keys (Iterable[KT]): keys to take from ``dict_``
 
         default (Optional[object] | NoParamType):
             if specified uses default if keys are missing.
 
-        cls (Type[Dict], default=OrderedDict): type of the returned dictionary.
+        cls (Type[Dict]): type of the returned dictionary.
+            Defaults to ``OrderedDict``.
 
     Returns:
         Dict[KT, VT]: subset dictionary
 
     SeeAlso:
         :func:`dict_isect` - similar functionality, but ignores missing keys
         ::py:meth:`UDict.subdict` - object oriented version of this function
@@ -610,18 +614,18 @@
         dict_ (Dict[KT, VT]):
             dictionary to sort. The values must be of comparable types.
 
         key (Callable[[VT], Any] | None):
             If given as a callable, customizes the sorting by ordering using
             transformed values.
 
-        reverse (bool, default=False):
-            if True returns in descending order
+        reverse (bool, default):
+            If True returns in descending order. Defaults to False.
 
-        cls (type): specifies the dict return type
+        cls (type): Specifies the dict return type. Default to OrderedDict.
 
     SeeAlso:
         ::py:meth:`UDict.sorted_values` - object oriented version of this function
 
     Returns:
         OrderedDict[KT, VT]: new dictionary where the values are ordered
 
@@ -652,22 +656,22 @@
 
 def sorted_keys(dict_, key=None, reverse=False, cls=OrderedDict):
     """
     Return an ordered dictionary sorted by its keys
 
     Args:
         dict_ (Dict[KT, VT]):
-            dictionary to sort. The keys must be of comparable types.
+            Dictionary to sort. The keys must be of comparable types.
 
         key (Callable[[KT], Any] | None):
             If given as a callable, customizes the sorting by ordering using
             transformed keys.
 
-        reverse (bool, default=False):
-            if True returns in descending order
+        reverse (bool):
+            If True returns in descending order. Default to False.
 
         cls (type): specifies the dict return type
 
     SeeAlso:
         ::py:meth:`UDict.sorted_keys` - object oriented version of this function
 
     Returns:
@@ -698,16 +702,16 @@
 def invert_dict(dict_, unique_vals=True, cls=None):
     """
     Swaps the keys and values in a dictionary.
 
     Args:
         dict_ (Dict[KT, VT]): dictionary to invert
 
-        unique_vals (bool, default=True): if False, the values of the new
-            dictionary are sets of the original keys.
+        unique_vals (bool): if False, the values of the new
+            dictionary are sets of the original keys. Defaults to True.
 
         cls (type | None): specifies the dict subclassof the result.
             if unspecified will be dict or OrderedDict. This behavior may
             change.
 
     SeeAlso:
         ::py:meth:`UDict.invert` - object oriented version of this function
@@ -766,17 +770,17 @@
 
     In other words, given a dictionary that maps each "axes" (i.e. some
     variable) to its "basis" (i.e. the possible values that it can take),
     generate all possible points in that grid (i.e. unique assignments of
     variables to values).
 
     Args:
-        _ (Dict[str, List[VT]] | None, default=None):
+        _ (Dict[str, List[VT]] | None):
             Use of this positional argument is not recommend. Instead specify
-            all arguments as keyword args.
+            all arguments as keyword args. Defaults to None.
 
             If specified, this should be a dictionary is unioned with the
             keyword args.  This exists to support ordered dictionaries before
             Python 3.6, and may eventually be removed.
 
         basis (Dict[str, List[VT]]):
             A dictionary where the keys correspond to "columns" and the values
@@ -869,17 +873,17 @@
             list of dictionaries.
 
             Each item in the list - or row - is a dictionary and can be thought
             of as an observation. The keys in each dictionary are the columns.
             The values of the dictionary must be hashable. Lists will be
             converted into tuples.
 
-        min_variations (int, default=0):
+        min_variations (int):
             "columns" with fewer than ``min_variations`` unique values are
-            removed from the result.
+            removed from the result. Defaults to 0.
 
         default (VT | NoParamType):
             if specified, unspecified columns are given this value.
             Defaults to NoParam.
 
     Returns:
         Dict[KT, List[VT]] :
@@ -1002,21 +1006,119 @@
 
 
 class SetDict(dict):
     """
     A dictionary subclass where all set operations are defined.
 
     All of the set operations are defined in a key-wise fashion, that is it is
-    like performing the operation on sets of keys.
+    like performing the operation on sets of keys. Value conflicts are handled
+    with left-most priority (default for ``intersection`` and ``difference``),
+    right-most priority (default for ``union`` and ``symmetric_difference``),
+    or via a custom ``merge`` callable similar to [RubyMerge]_.
+
+    The set operations are:
+
+        * union (or the ``|`` operator) combines multiple dicttionaries into
+            one. This is nearly identical to the update operation. Rightmost
+            values take priority.
+
+        * intersection (or the ``&`` operator). Takes the items from the
+            first dictionary that share keys with the following dictionaries
+            (or lists or sets of keys).  Leftmost values take priority.
+
+        * difference (or the ``-`` operator). Takes only items from the first
+            dictionary that do not share keys with following dictionaries.
+            Leftmost values take priority.
+
+        * symmetric_difference (or the ``^`` operator). Takes the items
+            from all dictionaries where the key appears an odd number of times.
+            Rightmost values take priority.
+
+    Note:
+        The reason righmost values take priority in union /
+        symmetric_difference and left-most values take priority in intersection
+        / difference is:
+
+            1. intersection / difference is for removing keys --- i.e. is used
+            to find values in the first (main) dictionary that are also in some
+            other dictionary (or set or list of keys), whereas
+
+            2. union is for adding keys --- i.e. it is basically just an alias
+            for dict.update, so the new (rightmost) keys clobber the old.
+
+            3. symmetric_difference is somewhat strange. I'm don't have a great
+            argument for it, but it seemed easier to implement this way and it
+            does seem closer to a union than it is to a difference. Perhaps
+            unpaired union might have been a better name for this, but take
+            that up with the set theorists.
+
+        Also, union / symmetric_difference does not make sense if arguments on
+        the rights are lists/sets, whereas difference / intersection does.
 
     Note:
         The SetDict class only defines key-wise set operations.  Value-wise or
         item-wise operations are in general not hashable and therefore not
         supported. A heavier extension would be needed for that.
 
+    TODO:
+        - [ ] implement merge callables so the user can specify how to resolve
+              value conflicts / combine values.
+
+    References:
+        .. [RubyMerge] https://ruby-doc.org/core-2.7.0/Hash.html#method-i-merge
+
+    CommandLine:
+        xdoctest -m ubelt.util_dict SetDict
+
+    Example:
+        >>> import ubelt as ub
+        >>> a = ub.SetDict({'A': 'Aa', 'B': 'Ba',            'D': 'Da'})
+        >>> b = ub.SetDict({'A': 'Ab', 'B': 'Bb', 'C': 'Cb',          })
+        >>> print(a.union(b))
+        >>> print(a.intersection(b))
+        >>> print(a.difference(b))
+        >>> print(a.symmetric_difference(b))
+        {'A': 'Ab', 'B': 'Bb', 'D': 'Da', 'C': 'Cb'}
+        {'A': 'Aa', 'B': 'Ba'}
+        {'D': 'Da'}
+        {'D': 'Da', 'C': 'Cb'}
+        >>> print(a | b)  # union
+        >>> print(a & b)  # intersection
+        >>> print(a - b)  # difference
+        >>> print(a ^ b)  # symmetric_difference
+        {'A': 'Ab', 'B': 'Bb', 'D': 'Da', 'C': 'Cb'}
+        {'A': 'Aa', 'B': 'Ba'}
+        {'D': 'Da'}
+        {'D': 'Da', 'C': 'Cb'}
+
+    Example:
+        >>> import ubelt as ub
+        >>> a = ub.SetDict({'A': 'Aa', 'B': 'Ba',            'D': 'Da'})
+        >>> b = ub.SetDict({'A': 'Ab', 'B': 'Bb', 'C': 'Cb',          })
+        >>> c = ub.SetDict({'A': 'Ac', 'B': 'Bc',                       'E': 'Ec'})
+        >>> d = ub.SetDict({'A': 'Ad',            'C': 'Cd', 'D': 'Dd'})
+        >>> # 3-ary operations
+        >>> print(a.union(b, c))
+        >>> print(a.intersection(b, c))
+        >>> print(a.difference(b, c))
+        >>> print(a.symmetric_difference(b, c))
+        {'A': 'Ac', 'B': 'Bc', 'D': 'Da', 'C': 'Cb', 'E': 'Ec'}
+        {'A': 'Aa', 'B': 'Ba'}
+        {'D': 'Da'}
+        {'D': 'Da', 'C': 'Cb', 'A': 'Ac', 'B': 'Bc', 'E': 'Ec'}
+        >>> # 4-ary operations
+        >>> print(ub.UDict.union(a, b, c, c))
+        >>> print(ub.UDict.intersection(a, b, c, c))
+        >>> print(ub.UDict.difference(a, b, c, d))
+        >>> print(ub.UDict.symmetric_difference(a, b, c, d))
+        {'A': 'Ac', 'B': 'Bc', 'D': 'Da', 'C': 'Cb', 'E': 'Ec'}
+        {'A': 'Aa', 'B': 'Ba'}
+        {}
+        {'B': 'Bc', 'E': 'Ec'}
+
     Example:
         >>> import ubelt as ub
         >>> primes = ub.sdict({v: f'prime_{v}' for v in [2, 3, 5, 7, 11]})
         >>> evens = ub.sdict({v: f'even_{v}' for v in [0, 2, 4, 6, 8, 10]})
         >>> odds = ub.sdict({v: f'odd_{v}' for v in [1, 3, 5, 7, 9, 11]})
         >>> squares = ub.sdict({v: f'square_{v}' for v in [0, 1, 4, 9]})
         >>> div3 = ub.sdict({v: f'div3_{v}' for v in [0, 3, 6, 9]})
@@ -1316,34 +1418,43 @@
         result = self.symmetric_difference(other)
         self.clear()
         self.update(result)
         return self
 
     ### Main set operations
 
-    def union(self, *others, cls=None):
+    def union(self, *others, cls=None, merge=None):
         """
         Return the key-wise union of two or more dictionaries.
 
-        For items with intersecting keys, dictionaries towards the end of the
-        sequence are given precedence.
+        Values chosen with *right-most* priority. I.e. for items with
+        intersecting keys, dictionaries towards the end of the sequence are
+        given precedence.
 
         Args:
             self (SetDict | dict):
                 if called as a static method this must be provided.
 
             *others : other dictionary like objects that have an ``items``
                 method. (i.e. it must return an iterable of 2-tuples where the
                 first item is hashable.)
 
             cls (type | None):
                 the desired return dictionary type.
 
+            merge (None | Callable):
+                if specified this function must accept an iterable of values
+                and return a new value to use (which typically is derived from
+                input values). NotImplemented, help wanted.
+
         Returns:
-            dict : whatever the dictionary type of the first argument is
+            dict : items from all input dictionaries. Conflicts are resolved
+                with right-most priority unless ``merge`` is specified.
+                Specific return type is specified by ``cls`` or defaults to the
+                leftmost input.
 
         Example:
             >>> import ubelt as ub
             >>> a = ub.SetDict({k: 'A_' + chr(97 + k) for k in [2, 3, 5, 7]})
             >>> b = ub.SetDict({k: 'B_' + chr(97 + k) for k in [2, 4, 0, 7]})
             >>> c = ub.SetDict({k: 'C_' + chr(97 + k) for k in [2, 8, 3]})
             >>> d = ub.SetDict({k: 'D_' + chr(97 + k) for k in [9, 10, 11]})
@@ -1353,36 +1464,57 @@
             >>> a | b | c
             >>> res = ub.SetDict.union(a, b, c, d, e)
             >>> print(ub.repr2(res, sort=1, nl=0, si=1))
             {0: B_a, 2: C_c, 3: C_d, 4: B_e, 5: A_f, 7: B_h, 8: C_i, 9: D_j, 10: D_k, 11: D_l}
         """
         cls = cls or self.__class__
         args = it.chain([self], others)
-        new = cls(it.chain.from_iterable(d.items() for d in args))
+        if merge is None:
+            new = cls(it.chain.from_iterable(d.items() for d in args))
+        else:
+            raise NotImplementedError('merge function is not yet implemented')
         return new
 
-    def intersection(self, *others, cls=None):
+    def intersection(self, *others, cls=None, merge=None):
         """
         Return the key-wise intersection of two or more dictionaries.
 
-        All items returned will be from the first dictionary for keys that
-        exist in all other dictionaries / sets provided.
+        Values returned with *left-most* priority. I.e. all items returned will
+        be from the first dictionary for keys that exist in all other
+        dictionaries / sets provided.
 
         Args:
             self (SetDict | dict):
                 if called as a static method this must be provided.
 
             *others : other dictionary or set like objects that can
                 be coerced into a set of keys.
 
             cls (type | None):
                 the desired return dictionary type.
 
+            merge (None | Callable):
+                if specified this function must accept an iterable of values
+                and return a new value to use (which typically is derived from
+                input values). NotImplemented, help wanted.
+
         Returns:
-            dict : whatever the dictionary type of the first argument is
+            dict : items with keys shared by all the inputs. Values take
+                left-most priority unless ``merge`` is specified. Specific
+                return type is specified by ``cls`` or defaults to the leftmost
+                input.
+
+        Example:
+            >>> import ubelt as ub
+            >>> a = ub.SetDict({'a': 1, 'b': 2, 'd': 4})
+            >>> b = ub.SetDict({'a': 10, 'b': 20, 'c': 30})
+            >>> a.intersection(b)
+            {'a': 1, 'b': 2}
+            >>> a & b
+            {'a': 1, 'b': 2}
 
         Example:
             >>> import ubelt as ub
             >>> a = ub.SetDict({k: 'A_' + chr(97 + k) for k in [2, 3, 5, 7]})
             >>> b = ub.SetDict({k: 'B_' + chr(97 + k) for k in [2, 4, 0, 7]})
             >>> c = ub.SetDict({k: 'C_' + chr(97 + k) for k in [2, 8, 3]})
             >>> d = ub.SetDict({k: 'D_' + chr(97 + k) for k in [9, 10, 11]})
@@ -1394,38 +1526,49 @@
             >>> print(ub.repr2(res, sort=1, nl=0, si=1))
             {}
         """
         cls = cls or self.__class__
         isect_keys = set(self.keys())
         for v in others:
             isect_keys.intersection_update(v)
-        new = cls((k, self[k]) for k in self if k in isect_keys)
+        if merge is None:
+            new = cls((k, self[k]) for k in self if k in isect_keys)
+        else:
+            raise NotImplementedError('merge function is not yet implemented')
         return new
 
-    def difference(self, *others, cls=None):
+    def difference(self, *others, cls=None, merge=None):
         """
         Return the key-wise difference between this dictionary and one or
         more other dictionary / keys.
 
-        The returned items will be from the first dictionary, and will only
-        contain keys that do not appear in any of the other dictionaries /
-        sets.
+        Values returned with *left-most* priority. I.e. the returned items will
+        be from the first dictionary, and will only contain keys that do not
+        appear in any of the other dictionaries / sets.
 
         Args:
             self (SetDict | dict):
                 if called as a static method this must be provided.
 
             *others : other dictionary or set like objects that can
                 be coerced into a set of keys.
 
             cls (type | None):
                 the desired return dictionary type.
 
+            merge (None | Callable):
+                if specified this function must accept an iterable of values
+                and return a new value to use (which typically is derived from
+                input values). NotImplemented, help wanted.
+
         Returns:
-            dict : whatever the dictionary type of the first argument is
+            dict : items from the first dictionary with keys not in any of the
+                following inputs. Values take left-most priority unless
+                ``merge`` is specified. Specific return type is specified by
+                ``cls`` or defaults to the leftmost input.
 
         Example:
             >>> import ubelt as ub
             >>> a = ub.SetDict({k: 'A_' + chr(97 + k) for k in [2, 3, 5, 7]})
             >>> b = ub.SetDict({k: 'B_' + chr(97 + k) for k in [2, 4, 0, 7]})
             >>> c = ub.SetDict({k: 'C_' + chr(97 + k) for k in [2, 8, 3]})
             >>> d = ub.SetDict({k: 'D_' + chr(97 + k) for k in [9, 10, 11]})
@@ -1437,40 +1580,51 @@
             >>> print(ub.repr2(res, sort=1, nl=0, si=1))
             {5: A_f}
         """
         cls = cls or self.__class__
         other_keys = set()
         for v in others:
             other_keys.update(v)
-        # Looping over original keys is important to maintain partial order.
-        new = cls((k, self[k]) for k in self.keys() if k not in other_keys)
+        if merge is None:
+            # Looping over original keys is important to maintain partial order.
+            new = cls((k, self[k]) for k in self.keys() if k not in other_keys)
+        else:
+            raise NotImplementedError('merge function is not yet implemented')
         return new
 
-    def symmetric_difference(self, *others, cls=None):
+    def symmetric_difference(self, *others, cls=None, merge=None):
         """
         Return the key-wise symmetric difference between this dictionary and
         one or more other dictionaries.
 
-        Returns items that are (key-wise) in an odd number of the given
-        dictionaries. This is consistent with the standard n-ary definition of
-        symmetric difference [WikiSymDiff]_ and corresponds with the xor
-        operation.
+        Values chosen with *right-most* priority. Returns items that are
+        (key-wise) in an odd number of the given dictionaries. This is
+        consistent with the standard n-ary definition of symmetric difference
+        [WikiSymDiff]_ and corresponds with the xor operation.
 
         Args:
             self (SetDict | dict):
                 if called as a static method this must be provided.
 
             *others : other dictionary or set like objects that can
                 be coerced into a set of keys.
 
             cls (type | None):
                 the desired return dictionary type.
 
+            merge (None | Callable):
+                if specified this function must accept an iterable of values
+                and return a new value to use (which typically is derived from
+                input values). NotImplemented, help wanted.
+
         Returns:
-            dict : whatever the dictionary type of the first argument is
+            dict : items from input dictionaries where the key appears an odd
+                number of times. Values take right-most priority unless
+                ``merge`` is specified. Specific return type is specified by
+                ``cls`` or defaults to the leftmost input.
 
         References:
             .. [WikiSymDiff] https://en.wikipedia.org/wiki/Symmetric_difference
 
         Example:
             >>> import ubelt as ub
             >>> a = ub.SetDict({k: 'A_' + chr(97 + k) for k in [2, 3, 5, 7]})
@@ -1484,20 +1638,23 @@
             >>> a - b - c
             >>> res = ub.SetDict.symmetric_difference(a, b, c, d, e)
             >>> print(ub.repr2(res, sort=1, nl=0, si=1))
             {0: B_a, 2: C_c, 4: B_e, 5: A_f, 8: C_i, 9: D_j, 10: D_k, 11: D_l}
         """
         cls = cls or self.__class__
         new = cls(self)  # shallow copy
-        for d in others:
-            for k, v in d.items():
-                if k in new:
-                    new.pop(k)
-                else:
-                    new[k] = v
+        if merge is None:
+            for d in others:
+                for k, v in d.items():
+                    if k in new:
+                        new.pop(k)
+                    else:
+                        new[k] = v
+        else:
+            raise NotImplementedError('merge function is not yet implemented')
         return new
 
 
 sdict = SetDict
 
 
 # Might need to make these mixins for 3.6
```

### Comparing `ubelt-1.2.4/ubelt/util_dict.pyi` & `ubelt-1.3.0/ubelt/util_dict.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import sys
 from typing import Iterable
 from typing import Type
 from typing import Dict
-from typing import Union
 from typing import Callable
 from typing import List
 from typing import Any
 from typing import Optional
 from ubelt.util_const import NoParam
 from ubelt.util_const import NoParamType
 from collections import OrderedDict
@@ -26,106 +25,103 @@
 
 def dzip(items1: Iterable[KT],
          items2: Iterable[VT],
          cls: Type[dict] = dict) -> Dict[KT, VT]:
     ...
 
 
-def group_items(
-        items: Iterable[VT],
-        key: Union[Iterable[KT], Callable[[VT], KT]]) -> dict[KT, List[VT]]:
+def group_items(items: Iterable[VT],
+                key: Iterable[KT] | Callable[[VT], KT]) -> dict[KT, List[VT]]:
     ...
 
 
 def dict_hist(items: Iterable[T],
-              weights: Union[Iterable[float], None] = None,
+              weights: Iterable[float] | None = None,
               ordered: bool = False,
-              labels: Union[Iterable[T], None] = None) -> dict[T, int]:
+              labels: Iterable[T] | None = None) -> dict[T, int]:
     ...
 
 
 def find_duplicates(
         items: Iterable[T],
         k: int = 2,
-        key: Union[Callable[[T], Any], None] = None) -> dict[T, List[int]]:
+        key: Callable[[T], Any] | None = None) -> dict[T, List[int]]:
     ...
 
 
 def dict_subset(dict_: Dict[KT, VT],
                 keys: Iterable[KT],
-                default: Union[Optional[object], NoParamType] = NoParam,
+                default: Optional[object] | NoParamType = NoParam,
                 cls: Type[Dict] = OrderedDict) -> Dict[KT, VT]:
     ...
 
 
 def dict_union(*args: List[Dict]) -> Dict | OrderedDict:
     ...
 
 
 def dict_diff(
-    *args: List[Union[Dict[KT, VT], Iterable[KT]]]
+    *args: List[Dict[KT, VT] | Iterable[KT]]
 ) -> Dict[KT, VT] | OrderedDict[KT, VT]:
     ...
 
 
 def dict_isect(
-    *args: List[Union[Dict[KT, VT], Iterable[KT]]]
+    *args: List[Dict[KT, VT] | Iterable[KT]]
 ) -> Dict[KT, VT] | OrderedDict[KT, VT]:
     ...
 
 
-def map_values(func: Union[Callable[[VT], T], Mapping[VT, T]],
+def map_values(func: Callable[[VT], T] | Mapping[VT, T],
                dict_: Dict[KT, VT],
-               cls: Union[type, None] = None) -> Dict[KT, T]:
+               cls: type | None = None) -> Dict[KT, T]:
     ...
 
 
 map_vals = map_values
 
 
-def map_keys(func: Union[Callable[[KT], T], Mapping[KT, T]],
+def map_keys(func: Callable[[KT], T] | Mapping[KT, T],
              dict_: Dict[KT, VT],
-             cls: Union[type, None] = None) -> Dict[T, VT]:
+             cls: type | None = None) -> Dict[T, VT]:
     ...
 
 
 def sorted_values(dict_: Dict[KT, VT],
-                  key: Union[Callable[[VT], Any], None] = None,
+                  key: Callable[[VT], Any] | None = None,
                   reverse: bool = False,
                   cls: type = OrderedDict) -> OrderedDict[KT, VT]:
     ...
 
 
 sorted_vals = sorted_values
 
 
 def sorted_keys(dict_: Dict[KT, VT],
-                key: Union[Callable[[KT], Any], None] = None,
+                key: Callable[[KT], Any] | None = None,
                 reverse: bool = False,
                 cls: type = OrderedDict) -> OrderedDict[KT, VT]:
     ...
 
 
-def invert_dict(
-        dict_: Dict[KT, VT],
-        unique_vals: bool = True,
-        cls: Union[type, None] = None) -> Dict[VT, KT] | Dict[VT, Set[KT]]:
+def invert_dict(dict_: Dict[KT, VT],
+                unique_vals: bool = True,
+                cls: type | None = None) -> Dict[VT, KT] | Dict[VT, Set[KT]]:
     ...
 
 
 def named_product(
-        _: Union[Dict[str, List[VT]], None] = None,
+        _: Dict[str, List[VT]] | None = None,
         **basis: Dict[str, List[VT]]) -> Generator[Dict[str, VT], None, None]:
     ...
 
 
-def varied_values(
-        longform: List[Dict[KT, VT]],
-        min_variations: int = 0,
-        default: Union[VT, NoParamType] = NoParam) -> Dict[KT, List[VT]]:
+def varied_values(longform: List[Dict[KT, VT]],
+                  min_variations: int = 0,
+                  default: VT | NoParamType = NoParam) -> Dict[KT, List[VT]]:
     ...
 
 
 class SetDict(dict):
 
     def copy(self):
         ...
@@ -162,74 +158,82 @@
 
     def __isub__(self, other):
         ...
 
     def __ixor__(self, other):
         ...
 
-    def union(self, *others, cls: Union[type, None] = None) -> dict:
-        ...
-
-    def intersection(self, *others, cls: Union[type, None] = None) -> dict:
-        ...
-
-    def difference(self, *others, cls: Union[type, None] = None) -> dict:
+    def union(self,
+              *others,
+              cls: type | None = None,
+              merge: None | Callable = None) -> dict:
+        ...
+
+    def intersection(self,
+                     *others,
+                     cls: type | None = None,
+                     merge: None | Callable = None) -> dict:
+        ...
+
+    def difference(self,
+                   *others,
+                   cls: type | None = None,
+                   merge: None | Callable = None) -> dict:
         ...
 
     def symmetric_difference(self,
                              *others,
-                             cls: Union[type, None] = None) -> dict:
+                             cls: type | None = None,
+                             merge: None | Callable = None) -> dict:
         ...
 
 
 sdict = SetDict
 
 
 class UDict(SetDict):
 
     def subdict(self,
                 keys: Iterable[KT],
-                default: Union[Optional[object], NoParamType] = NoParam):
+                default: Optional[object] | NoParamType = NoParam):
         ...
 
     def take(
         self,
         keys: Iterable[KT],
-        default: Union[Optional[object], NoParamType] = NoParam
+        default: Optional[object] | NoParamType = NoParam
     ) -> Generator[VT, None, None]:
         ...
 
     def invert(self,
                unique_vals: bool = True) -> Dict[VT, KT] | Dict[VT, Set[KT]]:
         ...
 
-    def map_keys(
-            self, func: Union[Callable[[VT], T], Mapping[VT,
-                                                         T]]) -> Dict[KT, T]:
+    def map_keys(self,
+                 func: Callable[[VT], T] | Mapping[VT, T]) -> Dict[KT, T]:
         ...
 
-    def map_values(
-            self, func: Union[Callable[[VT], T], Mapping[VT,
-                                                         T]]) -> Dict[KT, T]:
+    def map_values(self,
+                   func: Callable[[VT], T] | Mapping[VT, T]) -> Dict[KT, T]:
         ...
 
     def sorted_keys(self,
-                    key: Union[Callable[[KT], Any], None] = None,
+                    key: Callable[[KT], Any] | None = None,
                     reverse: bool = False) -> OrderedDict[KT, VT]:
         ...
 
     def sorted_values(self,
-                      key: Union[Callable[[VT], Any], None] = None,
+                      key: Callable[[VT], Any] | None = None,
                       reverse: bool = False) -> OrderedDict[KT, VT]:
         ...
 
-    def peek_key(self, default: Union[KT, NoParamType] = NoParam) -> KT:
+    def peek_key(self, default: KT | NoParamType = NoParam) -> KT:
         ...
 
-    def peek_value(self, default: Union[VT, NoParamType] = NoParam) -> VT:
+    def peek_value(self, default: VT | NoParamType = NoParam) -> VT:
         ...
 
 
 class AutoDict(UDict):
 
     def __getitem__(self, key):
         ...
```

### Comparing `ubelt-1.2.4/ubelt/util_download.py` & `ubelt-1.3.0/ubelt/util_download.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,15 +417,15 @@
             fname = basename(url)
         fpath = join(dpath, fname)
 
     if dpath is None or fname is None:
         dpath, fname = split(fpath)
 
     if hasher is not None:
-        if not isinstance(hasher, str):
+        if not isinstance(hasher, str):   # nocover
             from ubelt import schedule_deprecation
             schedule_deprecation(
                 modname='ubelt',
                 migration='Pass hasher as a string, otherwise unexpected behavior can occur',
                 name='hasher', type='grabdata arg',
                 deprecate='1.1.0', error='1.3.0', remove='1.4.0')
             hasher_name = hasher.name
```

### Comparing `ubelt-1.2.4/ubelt/util_download_manager.py` & `ubelt-1.3.0/ubelt/util_download_manager.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt/util_format.py` & `ubelt-1.3.0/ubelt/util_repr.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 
 >>> print(ub.urepr({1: float('nan'), 2: float('inf'), 3: 3.0}, nl=0))
 {1: float('nan'), 2: float('inf'), 3: 3.0}
 
 
 You can also define or overwrite how representations for different types are
 created. You can either create your own extension object, or you can
-monkey-patch `ub.util_format._FORMATTER_EXTENSIONS` without specifying the
+monkey-patch `ub.util_repr._REPR_EXTENSIONS` without specifying the
 extensions keyword argument (although this will be a global change).
 
->>> extensions = ub.util_format.FormatterExtensions()
+>>> extensions = ub.util_repr.ReprExtensions()
 >>> @extensions.register(float)
 >>> def my_float_formater(data, **kw):
 >>>     return "monkey({})".format(data)
 >>> print(ub.urepr({1: float('nan'), 2: float('inf'), 3: 3.0}, nl=0, extensions=extensions))
 {1: monkey(nan), 2: monkey(inf), 3: monkey(3.0)}
 
 As of ubelt 1.1.0 you can now access and update the default extensions via the
@@ -48,15 +48,15 @@
 >>>     return "monkey2({})".format(data)
 >>> print(ub.urepr({1: float('nan'), 2: float('inf'), 3: 3.0}, nl=0))
 """
 import collections
 from ubelt import util_str
 from ubelt import util_list
 
-__all__ = ['repr2', 'urepr', 'FormatterExtensions']
+__all__ = ['urepr', 'ReprExtensions']
 
 
 def urepr(data, **kwargs):
     """
     Makes a pretty string representation of ``data``.
 
     Makes a pretty and easy-to-doctest string representation. Has nice handling
@@ -148,16 +148,16 @@
         with_dtype (bool):
             only relevant to numpy.ndarrays. if True includes the dtype.
             Defaults to `not strvals`.
 
         align (bool | str, default=False):
             if True, will align multi-line dictionaries by the kvsep
 
-        extensions (FormatterExtensions):
-            a custom :class:`FormatterExtensions` instance that can overwrite
+        extensions (ReprExtensions):
+            a custom :class:`ReprExtensions` instance that can overwrite
             or define how different types of objects are formatted.
 
     Returns:
         str: outstr - output string
 
     Note:
         There are also internal kwargs, which should not be used:
@@ -271,64 +271,27 @@
         if isinstance(data, dict):
             outstr, _leaf_info = _format_dict(data, **kwargs)
         elif isinstance(data, (list, tuple, set, frozenset)):
             outstr, _leaf_info = _format_list(data, **kwargs)
 
     if outstr is None:
         # check any globally registered functions for special formatters
-        func = _FORMATTER_EXTENSIONS.lookup(data)
+        func = _REPR_EXTENSIONS.lookup(data)
         if func is not None:
             outstr = func(data, **kwargs)
         else:
             outstr = _format_object(data, **kwargs)
 
     if _return_info:
         _leaf_info = _rectify_leaf_info(_leaf_info)
         return outstr, _leaf_info
     else:
         return outstr
 
 
-def repr2(data, **kwargs):
-    """
-    Deprecated for urepr
-
-    Example:
-        >>> # Test that repr2 remains backwards compatible
-        >>> import ubelt as ub
-        >>> dict_ = {
-        ...     'custom_types': [slice(0, 1, None), 1/3],
-        ...     'nest_dict': {'k1': [1, 2, {3: {4, 5}}],
-        ...                   'key2': [1, 2, {3: {4, 5}}],
-        ...                   'key3': [1, 2, {3: {4, 5}}],
-        ...                   },
-        ...     'nest_dict2': {'k': [1, 2, {3: {4, 5}}]},
-        ...     'nested_tuples': [tuple([1]), tuple([2, 3]), frozenset([4, 5, 6])],
-        ...     'one_tup': tuple([1]),
-        ...     'simple_dict': {'spam': 'eggs', 'ham': 'jam'},
-        ...     'simple_list': [1, 2, 'red', 'blue'],
-        ...     'odict': ub.odict([(2, '1'), (1, '2')]),
-        ... }
-        >>> result = ub.repr2(dict_, nl=1, precision=2)
-        >>> print(result)
-        {
-            'custom_types': [slice(0, 1, None), 0.33],
-            'nest_dict': {'k1': [1, 2, {3: {4, 5}}], 'key2': [1, 2, {3: {4, 5}}], 'key3': [1, 2, {3: {4, 5}}]},
-            'nest_dict2': {'k': [1, 2, {3: {4, 5}}]},
-            'nested_tuples': [(1,), (2, 3), {4, 5, 6}],
-            'odict': {2: '1', 1: '2'},
-            'one_tup': (1,),
-            'simple_dict': {'ham': 'jam', 'spam': 'eggs'},
-            'simple_list': [1, 2, 'red', 'blue'],
-        }
-    """
-    kwargs['_dict_sort_behavior'] = kwargs.get('_dict_sort_behavior', 'old')
-    return urepr(data, **kwargs)
-
-
 def _rectify_root_info(_root_info):
     if _root_info is None:
         _root_info = {
             'depth': 0,
         }
     return _root_info
 
@@ -338,30 +301,30 @@
         _leaf_info = {
             'max_height': 0,
             'min_height': 0,
         }
     return _leaf_info
 
 
-class FormatterExtensions(object):
+class ReprExtensions(object):
     """
     Helper class for managing non-builtin (e.g. numpy) format types.
 
-    This module (:mod:`ubelt.util_format`) maintains a global set of basic
+    This module (:mod:`ubelt.util_repr`) maintains a global set of basic
     extensions, but it is also possible to create a locally scoped set of
     extensions and explicitly pass it to urepr. The following example
     demonstrates this.
 
     Example:
         >>> import ubelt as ub
         >>> class MyObject(object):
         >>>     pass
         >>> data = {'a': [1, 2.2222, MyObject()], 'b': MyObject()}
         >>> # Create a custom set of extensions
-        >>> extensions = ub.FormatterExtensions()
+        >>> extensions = ub.ReprExtensions()
         >>> # Register a function to format your specific type
         >>> @extensions.register(MyObject)
         >>> def format_myobject(data, **kwargs):
         >>>     return 'I can do anything here'
         >>> # Repr2 will now respect the passed custom extensions
         >>> # Note that the global extensions will still be respected
         >>> # unless they are overloaded.
@@ -448,15 +411,15 @@
             >>> # xdoctest: +REQUIRES(module:pandas)
             >>> # xdoctest: +IGNORE_WHITESPACE
             >>> import pandas as pd
             >>> import numpy as np
             >>> import ubelt as ub
             >>> rng = np.random.RandomState(0)
             >>> data = pd.DataFrame(rng.rand(3, 3))
-            >>> print(ub.repr2(data))
+            >>> print(ub.urepr(data))
             >>> print(ub.urepr(data, precision=2))
             >>> print(ub.urepr({'akeyfdfj': data}, precision=2))
         """
         @self.register('DataFrame')
         def format_pandas(data, **kwargs):  # nocover
             precision = kwargs.get('precision', None)
             float_format = (None if precision is None
@@ -619,34 +582,34 @@
         @self.register(slice)
         def format_slice(data, **kwargs):
             if kwargs.get('itemsep', ' ') == '':
                 return 'slice(%r,%r,%r)' % (data.start, data.stop, data.step)
             else:
                 return _format_object(data, **kwargs)
 
-_FORMATTER_EXTENSIONS = FormatterExtensions()
-_FORMATTER_EXTENSIONS._register_builtin_extensions()
+_REPR_EXTENSIONS = ReprExtensions()
+_REPR_EXTENSIONS._register_builtin_extensions()
 
 
 def _lazy_init():
     """
     Only called in the case where we encounter an unknown type that a commonly
     used external library might have. For now this is just numpy. Numpy is
     ubiquitous.
     """
     try:
         # TODO: can we use lazy loading to prevent trying to import numpy until
-        # some attribute of _FORMATTER_EXTENSIONS is used?
-        _FORMATTER_EXTENSIONS._register_numpy_extensions()
-        _FORMATTER_EXTENSIONS._register_pandas_extensions()
-        # _FORMATTER_EXTENSIONS._register_torch_extensions()
+        # some attribute of _REPR_EXTENSIONS is used?
+        _REPR_EXTENSIONS._register_numpy_extensions()
+        _REPR_EXTENSIONS._register_pandas_extensions()
+        # _REPR_EXTENSIONS._register_torch_extensions()
     except ImportError:  # nocover
         pass
 
-_FORMATTER_EXTENSIONS._lazy_queue.append(_lazy_init)
+_REPR_EXTENSIONS._lazy_queue.append(_lazy_init)
 
 
 def _format_object(val, **kwargs):
     stritems = kwargs.get('si', kwargs.get('stritems', False))
     strvals = stritems or kwargs.get('sv', kwargs.get('strvals', False))
     base_valfunc = str if strvals else repr
     itemstr = base_valfunc(val)
@@ -747,15 +710,15 @@
 
         nobr (bool, default=False): removes outer braces
 
     Returns:
         Tuple[str, Dict] : retstr, _leaf_info
 
     Example:
-        >>> from ubelt.util_format import *  # NOQA
+        >>> from ubelt.util_repr import *  # NOQA
         >>> dict_ = {'a': 'edf', 'bc': 'ghi'}
         >>> print(_format_dict(dict_)[0])
         {
             'a': 'edf',
             'bc': 'ghi',
         }
         >>> print(_format_dict(dict_, align=True)[0])
@@ -878,20 +841,20 @@
 
     Args:
         dict_ (dict): the dict
         **kwargs: explicit, precision, kvsep, strkeys, _return_info, cbr,
             compact_brace, sort
 
     Ignore:
-        from ubelt.util_format import _dict_itemstrs
+        from ubelt.util_repr import _dict_itemstrs
         import xinspect
         print(', '.join(xinspect.get_kwargs(_dict_itemstrs, max_depth=0).keys()))
 
     Example:
-        >>> from ubelt.util_format import *
+        >>> from ubelt.util_repr import *
         >>> dict_ =  {'b': .1, 'l': 'st', 'g': 1.0, 's': 10, 'm': 0.9, 'w': .5}
         >>> kwargs = {'strkeys': True, 'sort': True}
         >>> itemstrs, _ = _dict_itemstrs(dict_, **kwargs)
         >>> char_order = [p[0] for p in itemstrs]
         >>> assert char_order == ['b', 'g', 'l', 'm', 's', 'w']
     """
     import ubelt as ub
@@ -1033,15 +996,15 @@
         count_or_bool (bool | int): if positive and an integer, it will count
             down, otherwise it will remain the same.
 
     Returns:
         int or bool: count_or_bool_
 
     Example:
-        >>> from ubelt.util_format import _rectify_countdown_or_bool  # NOQA
+        >>> from ubelt.util_repr import _rectify_countdown_or_bool  # NOQA
         >>> count_or_bool = True
         >>> a1 = (_rectify_countdown_or_bool(2))
         >>> a2 = (_rectify_countdown_or_bool(1))
         >>> a3 = (_rectify_countdown_or_bool(0))
         >>> a4 = (_rectify_countdown_or_bool(-1))
         >>> a5 = (_rectify_countdown_or_bool(-2))
         >>> a6 = (_rectify_countdown_or_bool(True))
@@ -1215,12 +1178,9 @@
         else:
             new_lines.append(replchar.join(tup))
     return new_lines
 
 
 # Give the urepr function itself a reference to the default extensions
 # register method so the user can modify them without accessing this module
-urepr.extensions = _FORMATTER_EXTENSIONS
-urepr.register = _FORMATTER_EXTENSIONS.register
-
-repr2.extensions = urepr.extensions
-repr2.register = urepr.register
+urepr.extensions = _REPR_EXTENSIONS
+urepr.register = _REPR_EXTENSIONS.register
```

### Comparing `ubelt-1.2.4/ubelt/util_func.py` & `ubelt-1.3.0/ubelt/util_func.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt/util_futures.py` & `ubelt-1.3.0/ubelt/util_futures.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,16 +141,16 @@
         >>>     for i, f in enumerate(futures):
         >>>         assert i + 1 == f.result()
     """
     def __enter__(self):
         self.max_workers = 0
         return self
 
-    def __exit__(self, ex_type, ex_value, tb):
-        pass
+    def __exit__(self, ex_type, ex_value, ex_traceback):
+        return False
 
     def submit(self, func, *args, **kw):
         """
         Submit a job to be executed later
 
         Returns:
             concurrent.futures.Future:
@@ -226,16 +226,16 @@
 #             self.loop = asyncio.get_event_loop()
 #         except RuntimeError:
 #             loop = asyncio.new_event_loop()
 #             asyncio.set_event_loop(loop)
 #             self.loop = asyncio.get_event_loop()
 #     def __enter__(self):
 #         return self
-#     def __exit__(self, ex_type, ex_value, tb):
-#         pass
+#     def __exit__(self, ex_type, ex_value, ex_traceback):
+#         ...
 #     def submit(self, func, *args, **kw):
 #         ...
 #     def shutdown(self):
 #         ...
 #     def map(self, fn, *iterables, **kwargs):
 #         ...
 
@@ -294,16 +294,17 @@
             raise KeyError(mode)
         self.backend = backend
 
     def __enter__(self):
         self.backend.__enter__()
         return self
 
-    def __exit__(self, ex_type, ex_value, tb):
-        return self.backend.__exit__(ex_type, ex_value, tb)
+    def __exit__(self, ex_type, ex_value, ex_traceback):
+        # Note: the following call will block
+        return self.backend.__exit__(ex_type, ex_value, ex_traceback)
 
     def submit(self, func, *args, **kw):
         """
         Calls the submit function of the underlying backend.
 
         Returns:
             concurrent.futures.Future:
@@ -417,16 +418,16 @@
         self.jobs = None
         return self.executor.shutdown()
 
     def __enter__(self):
         self.executor.__enter__()
         return self
 
-    def __exit__(self, a, b, c):
-        self.executor.__exit__(a, b, c)
+    def __exit__(self, ex_type, ex_value, ex_traceback):
+        return self.executor.__exit__(ex_type, ex_value, ex_traceback)
 
     def _clear_completed(self):
         active_jobs = [job for job in self.jobs if job.running()]
         self.jobs = active_jobs
 
     def as_completed(self, timeout=None, desc=None, progkw=None):
         """
@@ -476,14 +477,17 @@
             if progkw is None:
                 progkw = {}
             job_iter = ub.ProgIter(
                 job_iter, desc=desc, total=len(self.jobs), **progkw)
             self._prog = job_iter
         for job in job_iter:
             if self.transient:
+                # Maybe keep a reference to the job index and then null it out
+                # in our job list? Should probably think about a good
+                # implementation. See kwcoco.CocoDataset._load_multiple
                 self.jobs.remove(job)
             yield job
 
     def join(self, **kwargs):
         """
         Like :func:`JobPool.as_completed`, but executes the `result` method
         of each future and returns only after all processes are complete.
@@ -516,15 +520,19 @@
         for job in self.as_completed(**kwargs):
             result = job.result()
             results.append(result)
         return results
 
     def __iter__(self):
         """
-        An alternative to as completed
+        An alternative to as completed.
+
+        NOTE:
+            The order of iteration may be changed in the future to be the
+            submission order instead.
 
         Example:
             >>> import ubelt as ub
             >>> pool = ub.JobPool('serial')
             >>> assert len(list(iter(pool))) == 0
             >>> pool.submit(print, 'hi')
             >>> assert len(list(iter(pool))) == 1
```

### Comparing `ubelt-1.2.4/ubelt/util_futures.pyi` & `ubelt-1.3.0/ubelt/util_indexable.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,102 +1,56 @@
-import concurrent
-import concurrent.futures
-from typing import Callable
-from typing import Any
-from typing import Union
+from typing import Tuple
 from typing import List
-import concurrent.futures
+from typing import Any
+from typing import Dict
 from _typeshed import Incomplete
 from collections.abc import Generator
 from typing import Any
 
 
-class SerialFuture(concurrent.futures.Future):
-    func: Incomplete
-    args: Incomplete
-    kw: Incomplete
-
-    def __init__(self, func, *args, **kw) -> None:
-        ...
-
-    def set_result(self, result) -> None:
-        ...
-
-
-class SerialExecutor:
-    max_workers: int
-
-    def __enter__(self):
-        ...
-
-    def __exit__(self, ex_type, ex_value, tb) -> None:
-        ...
-
-    def submit(self, func, *args, **kw) -> concurrent.futures.Future:
-        ...
-
-    def shutdown(self) -> None:
-        ...
-
-    def map(self, fn: Callable[..., Any], *iterables,
-            **kwargs) -> Generator[Any, None, None]:
-        ...
-
-
-class Executor:
-    backend: Incomplete
-
-    def __init__(self, mode: str = ..., max_workers: int = ...) -> None:
-        ...
-
-    def __enter__(self):
-        ...
-
-    def __exit__(self, ex_type, ex_value, tb):
-        ...
-
-    def submit(self, func, *args, **kw) -> concurrent.futures.Future:
-        ...
+class IndexableWalker(Generator):
+    data: dict | list | tuple
+    dict_cls: Tuple[type]
+    list_cls: Tuple[type]
+    indexable_cls: Incomplete
 
-    def shutdown(self):
+    def __init__(self, data, dict_cls=..., list_cls=...) -> None:
         ...
 
-    def map(self, fn, *iterables, **kwargs):
+    def __iter__(self) -> Generator[Tuple[List, Any], Any, Any]:
         ...
 
-
-class JobPool:
-    executor: Incomplete
-    jobs: Incomplete
-
-    def __init__(self, mode: str = ..., max_workers: int = ...) -> None:
+    def __next__(self) -> Any:
         ...
 
-    def __len__(self):
+    def send(self, arg) -> None:
         ...
 
-    def submit(self, func: Callable[..., Any], *args,
-               **kwargs) -> concurrent.futures.Future:
+    def throw(self,
+              type: Incomplete | None = ...,
+              value: Incomplete | None = ...,
+              traceback: Incomplete | None = ...) -> None:
         ...
 
-    def shutdown(self):
+    def __setitem__(self, path: List, value: Any) -> None:
         ...
 
-    def __enter__(self):
+    def __getitem__(self, path: List) -> Any:
         ...
 
-    def __exit__(self, a, b, c) -> None:
+    def __delitem__(self, path: List) -> None:
         ...
 
-    def as_completed(
-        self,
-        timeout: Union[float, None] = None,
-        desc: Union[str, None] = None,
-        progkw: Union[dict, None] = None
-    ) -> Generator[concurrent.futures.Future, None, None]:
+    def allclose(self,
+                 other: IndexableWalker | List | Dict,
+                 rel_tol: float = 1e-09,
+                 abs_tol: float = 0.0,
+                 return_info: bool = False) -> bool | Tuple[bool, Dict]:
         ...
 
-    def join(self, **kwargs) -> List[Any]:
-        ...
 
-    def __iter__(self):
-        ...
+def indexable_allclose(items1: dict | list | tuple,
+                       items2: dict | list | tuple,
+                       rel_tol: float = 1e-09,
+                       abs_tol: float = 0.0,
+                       return_info: bool = False) -> bool | Tuple[bool, Dict]:
+    ...
```

### Comparing `ubelt-1.2.4/ubelt/util_hash.py` & `ubelt-1.3.0/ubelt/util_hash.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt/util_hash.pyi` & `ubelt-1.3.0/ubelt/util_hash.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Union
 from typing import Tuple
 from typing import Callable
 from ubelt.util_const import NoParam
 from ubelt.util_const import NoParamType
 from typing import List
 from os import PathLike
 from _typeshed import Incomplete
@@ -40,15 +39,15 @@
 class HashableExtensions:
     keyed_extensions: Incomplete
     iterable_checks: Incomplete
 
     def __init__(self) -> None:
         ...
 
-    def register(self, hash_types: Union[type, Tuple[type]]) -> Callable:
+    def register(self, hash_types: type | Tuple[type]) -> Callable:
         ...
 
     def lookup(self, data):
         ...
 
     def add_iterable_check(self, func):
         ...
@@ -64,22 +63,22 @@
         ...
 
     def hexdigest(self):
         ...
 
 
 def hash_data(data: object,
-              hasher: Union[str, Hasher, NoParamType] = NoParam,
-              base: Union[List[str], str, NoParamType] = NoParam,
+              hasher: str | Hasher | NoParamType = NoParam,
+              base: List[str] | str | NoParamType = NoParam,
               types: bool = False,
               convert: bool = False,
-              extensions: Union[HashableExtensions, None] = None) -> str:
+              extensions: HashableExtensions | None = None) -> str:
     ...
 
 
 def hash_file(fpath: PathLike,
               blocksize: int = 1048576,
               stride: int = 1,
-              maxbytes: Union[int, None] = None,
-              hasher: Union[str, Hasher, NoParamType] = NoParam,
-              base: Union[List[str], str, NoParamType] = NoParam):
+              maxbytes: int | None = None,
+              hasher: str | Hasher | NoParamType = NoParam,
+              base: List[str] | int | str | NoParamType = NoParam):
     ...
```

### Comparing `ubelt-1.2.4/ubelt/util_import.py` & `ubelt-1.3.0/ubelt/util_import.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,33 +41,39 @@
         to detect it and warn.
 
     Args:
         dpath (str | PathLike): directory to insert into the PYTHONPATH
         index (int): position to add to. Typically either -1 or 0.
 
     Example:
+        >>> from ubelt.util_import import PythonPathContext
+        >>> import sys
         >>> with PythonPathContext('foo', -1):
         >>>     assert sys.path[-1] == 'foo'
         >>> assert sys.path[-1] != 'foo'
         >>> with PythonPathContext('bar', 0):
         >>>     assert sys.path[0] == 'bar'
         >>> assert sys.path[0] != 'bar'
 
     Example:
         >>> # xdoctest: +REQUIRES(module:pytest)
         >>> # Mangle the path inside the context
+        >>> from ubelt.util_import import PythonPathContext
+        >>> import sys
         >>> self = PythonPathContext('foo', 0)
         >>> self.__enter__()
         >>> sys.path.insert(0, 'mangled')
         >>> import pytest
         >>> with pytest.warns(UserWarning):
         >>>     self.__exit__(None, None, None)
 
     Example:
         >>> # xdoctest: +REQUIRES(module:pytest)
+        >>> from ubelt.util_import import PythonPathContext
+        >>> import sys
         >>> self = PythonPathContext('foo', 0)
         >>> self.__enter__()
         >>> sys.path.remove('foo')
         >>> import pytest
         >>> with pytest.raises(RuntimeError):
         >>>     self.__exit__(None, None, None)
     """
@@ -177,32 +183,35 @@
             - foo/
               +- bar/
                  +- pkg/
                     +  __init__.py
                     |- mod.py
                     |- helper.py
 
-       If there exists another module named ``pkg`` already in sys.modules
-       and mod.py does something like ``from . import helper``, Python will
-       assume helper belongs to the ``pkg`` module already in sys.modules.
-       This can cause a NameError or worse --- a incorrect helper module.
+       If there exists another module named ``pkg`` already in ``sys.modules``
+       and mod.py contains the code ``from . import helper``, Python will
+       assume helper belongs to the ``pkg`` module already in ``sys.modules``.
+       This can cause a NameError or worse --- an incorrect helper module.
 
     SeeAlso:
         :func:`import_module_from_name`
 
     Example:
+        >>> import ubelt as ub
         >>> import xdoctest
         >>> modpath = xdoctest.__file__
-        >>> module = import_module_from_path(modpath)
+        >>> module = ub.import_module_from_path(modpath)
         >>> assert module is xdoctest
 
     Example:
         >>> # Test importing a module from within a zipfile
+        >>> import ubelt as ub
         >>> import zipfile
         >>> from xdoctest import utils
+        >>> import os
         >>> from os.path import join, expanduser, normpath
         >>> dpath = expanduser('~/.cache/xdoctest')
         >>> dpath = utils.ensuredir(dpath)
         >>> #dpath = utils.TempDir().ensure()
         >>> # Write to an external module named bar
         >>> external_modpath = join(dpath, 'bar.py')
         >>> # For pypy support we have to write this using with
@@ -212,24 +221,25 @@
         >>> # Move the external bar module into a zipfile
         >>> zippath = join(dpath, 'myzip.zip')
         >>> with zipfile.ZipFile(zippath, 'w') as myzip:
         >>>     myzip.write(external_modpath, internal)
         >>> # Import the bar module from within the zipfile
         >>> modpath = zippath + ':' + internal
         >>> modpath = zippath + os.path.sep + internal
-        >>> module = import_module_from_path(modpath)
+        >>> module = ub.import_module_from_path(modpath)
         >>> assert normpath(module.__name__) == normpath('folder/bar')
         >>> assert module.testvar == 1
 
     Example:
         >>> import pytest
+        >>> import ubelt as ub
         >>> with pytest.raises(IOError):
-        >>>     import_module_from_path('does-not-exist')
+        >>>     ub.import_module_from_path('does-not-exist')
         >>> with pytest.raises(IOError):
-        >>>     import_module_from_path('does-not-exist.zip/')
+        >>>     ub.import_module_from_path('does-not-exist.zip/')
     """
     if not os.path.exists(modpath):
         import re
         import zipimport
         # We allow (if not prefer or force) the colon to be a path.sep in order
         # to agree with the mod.__name__ attribute that will be produced
         # TODO: we could codify this by using `util_zip.split_archive`
@@ -294,20 +304,22 @@
 
     SeeAlso:
         :func:`import_module_from_path`
 
     Example:
         >>> # test with modules that won't be imported in normal circumstances
         >>> # todo write a test where we guarantee this
+        >>> import ubelt as ub
+        >>> import sys
         >>> modname_list = [
         >>>     'pickletools',
         >>>     'lib2to3.fixes.fix_apply',
         >>> ]
         >>> #assert not any(m in sys.modules for m in modname_list)
-        >>> modules = [import_module_from_name(modname) for modname in modname_list]
+        >>> modules = [ub.import_module_from_name(modname) for modname in modname_list]
         >>> assert [m.__name__ for m in modules] == modname_list
         >>> assert all(m in sys.modules for m in modname_list)
     """
     if True:
         # See if this fixes the Docker issue we saw but were unable to
         # reproduce on another environment. Either way its better to use the
         # standard importlib implementation than the one I wrote a long time
@@ -388,14 +400,16 @@
         https://github.com/pypa/setuptools/issues/3548
         Trying to find more docs about it.
 
         TODO: add a test where we make an editable install, regular install,
         standalone install, and check that we always find the right path.
 
     Example:
+        >>> from ubelt.util_import import *  # NOQA
+        >>> from ubelt.util_import import _syspath_modname_to_modpath
         >>> print(_syspath_modname_to_modpath('xdoctest.static_analysis'))
         ...static_analysis.py
         >>> print(_syspath_modname_to_modpath('xdoctest'))
         ...xdoctest
         >>> # xdoctest: +REQUIRES(CPython)
         >>> print(_syspath_modname_to_modpath('_ctypes'))
         ..._ctypes...
@@ -615,14 +629,15 @@
     mechanisms, but unfortunately it doesn't play nice with pytest.
 
     Args:
         modname (str): the module name.
 
     Example:
         >>> # xdoctest: +SKIP
+        >>> from ubelt.util_import import _pkgutil_modname_to_modpath
         >>> modname = 'xdoctest.static_analysis'
         >>> _pkgutil_modname_to_modpath(modname)
         ...static_analysis.py
         >>> # xdoctest: +REQUIRES(CPython)
         >>> _pkgutil_modname_to_modpath('_ctypes')
         ..._ctypes...
 
@@ -653,25 +668,26 @@
 
         hide_init (bool):
             if False, __init__.py will be returned for packages.
             Defaults to True.
 
         hide_main (bool):
             if False, and ``hide_init`` is True, __main__.py will be returned
-            for packages, if it exists. Defautls to False.
+            for packages, if it exists. Defaults to False.
 
         sys_path (None | List[str | PathLike]):
             The paths to search for the module.
             If unspecified, defaults to ``sys.path``.
 
     Returns:
         str | None:
             modpath - path to the module, or None if it doesn't exist
 
     Example:
+        >>> from ubelt.util_import import modname_to_modpath
         >>> modname = 'xdoctest.__main__'
         >>> modpath = modname_to_modpath(modname, hide_main=False)
         >>> assert modpath.endswith('__main__.py')
         >>> modname = 'xdoctest'
         >>> modpath = modname_to_modpath(modname, hide_init=False)
         >>> assert modpath.endswith('__init__.py')
         >>> # xdoctest: +REQUIRES(CPython)
@@ -706,14 +722,15 @@
     Returns:
         str | PathLike: a normalized path to the module
 
     Note:
         Adds __init__ if reasonable, but only removes __main__ by default
 
     Example:
+        >>> from ubelt.util_import import normalize_modpath
         >>> from xdoctest import static_analysis as module
         >>> modpath = module.__file__
         >>> assert normalize_modpath(modpath) == modpath.replace('.pyc', '.py')
         >>> dpath = dirname(modpath)
         >>> res0 = normalize_modpath(dpath, hide_init=0, hide_main=0)
         >>> res1 = normalize_modpath(dpath, hide_init=0, hide_main=1)
         >>> res2 = normalize_modpath(dpath, hide_init=1, hide_main=0)
@@ -770,32 +787,37 @@
     Returns:
         str: modname
 
     Raises:
         ValueError: if check is True and the path does not exist
 
     Example:
+        >>> from ubelt.util_import import modpath_to_modname
         >>> from xdoctest import static_analysis
         >>> modpath = static_analysis.__file__.replace('.pyc', '.py')
         >>> modpath = modpath.replace('.pyc', '.py')
         >>> modname = modpath_to_modname(modpath)
         >>> assert modname == 'xdoctest.static_analysis'
 
     Example:
+        >>> from ubelt.util_import import modpath_to_modname
         >>> import xdoctest
         >>> assert modpath_to_modname(xdoctest.__file__.replace('.pyc', '.py')) == 'xdoctest'
         >>> assert modpath_to_modname(dirname(xdoctest.__file__.replace('.pyc', '.py'))) == 'xdoctest'
 
     Example:
         >>> # xdoctest: +REQUIRES(CPython)
+        >>> from ubelt.util_import import modpath_to_modname
+        >>> from ubelt.util_import import modname_to_modpath
         >>> modpath = modname_to_modpath('_ctypes')
         >>> modname = modpath_to_modname(modpath)
         >>> assert modname == '_ctypes'
 
     Example:
+        >>> from ubelt.util_import import modpath_to_modname
         >>> modpath = '/foo/libfoobar.linux-x86_64-3.6.so'
         >>> modname = modpath_to_modname(modpath, check=False)
         >>> assert modname == 'libfoobar'
     """
     if check and relativeto is None:
         if not exists(modpath):
             raise ValueError('modpath={} does not exist'.format(modpath))
@@ -831,14 +853,15 @@
         Tuple[str, str]: (directory, rel_modpath)
 
     Raises:
         ValueError: if modpath does not exist or is not a package
 
     Example:
         >>> from xdoctest import static_analysis
+        >>> from ubelt.util_import import split_modpath
         >>> modpath = static_analysis.__file__.replace('.pyc', '.py')
         >>> modpath = abspath(modpath)
         >>> dpath, rel_modpath = split_modpath(modpath)
         >>> recon = join(dpath, rel_modpath)
         >>> assert recon == modpath
         >>> assert rel_modpath == join('xdoctest', 'static_analysis.py')
     """
@@ -873,14 +896,15 @@
         exclude (list | None): list of directory paths. if specified prevents these
             directories from being searched.
 
     Returns:
         bool: True if the module can be imported
 
     Example:
+        >>> from ubelt.util_import import is_modname_importable
         >>> is_modname_importable('xdoctest')
         True
         >>> is_modname_importable('not_a_real_module')
         False
         >>> is_modname_importable('xdoctest', sys_path=[])
         False
     """
@@ -892,14 +916,15 @@
 
 def _static_parse(varname, fpath):
     """
     Statically parse the a constant variable from a python file
 
     Example:
         >>> import ubelt as ub
+        >>> from ubelt.util_import import _static_parse
         >>> dpath = ub.Path.appdir('tests/import/staticparse').ensuredir()
         >>> fpath = (dpath / 'foo.py')
         >>> fpath.write_text('a = {1: 2}')
         >>> assert _static_parse('a', fpath) == {1: 2}
         >>> fpath.write_text('a = 2')
         >>> assert _static_parse('a', fpath) == 2
         >>> fpath.write_text('a = "3"')
```

### Comparing `ubelt-1.2.4/ubelt/util_import.pyi` & `ubelt-1.3.0/ubelt/util_import.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Union
 from os import PathLike
 from types import ModuleType
 from typing import List
 from typing import Tuple
 from _typeshed import Incomplete
 
 
@@ -16,47 +15,46 @@
     def __enter__(self) -> None:
         ...
 
     def __exit__(self, type, value, trace) -> None:
         ...
 
 
-def import_module_from_path(modpath: Union[str, PathLike],
+def import_module_from_path(modpath: str | PathLike,
                             index: int = ...) -> ModuleType:
     ...
 
 
 def import_module_from_name(modname: str) -> ModuleType:
     ...
 
 
 def modname_to_modpath(
         modname: str,
         hide_init: bool = True,
         hide_main: bool = False,
-        sys_path: Union[None, List[Union[str,
-                                         PathLike]]] = None) -> str | None:
+        sys_path: None | List[str | PathLike] = None) -> str | None:
     ...
 
 
-def normalize_modpath(modpath: Union[str, PathLike],
+def normalize_modpath(modpath: str | PathLike,
                       hide_init: bool = True,
                       hide_main: bool = False) -> str | PathLike:
     ...
 
 
 def modpath_to_modname(modpath: str,
                        hide_init: bool = True,
                        hide_main: bool = False,
                        check: bool = True,
-                       relativeto: Union[str, None] = None) -> str:
+                       relativeto: str | None = None) -> str:
     ...
 
 
 def split_modpath(modpath: str, check: bool = True) -> Tuple[str, str]:
     ...
 
 
 def is_modname_importable(modname: str,
-                          sys_path: Union[list, None] = None,
-                          exclude: Union[list, None] = None) -> bool:
+                          sys_path: list | None = None,
+                          exclude: list | None = None) -> bool:
     ...
```

### Comparing `ubelt-1.2.4/ubelt/util_indexable.py` & `ubelt-1.3.0/ubelt/util_indexable.py`

 * *Files 6% similar despite different names*

```diff
@@ -204,18 +204,23 @@
         """
         Set nested value by path
 
         Args:
             path (List): list of indexes into the nested structure
             value (Any): new value
         """
+        import itertools as it
         d = self.data
         # note: slice unpack seems faster in 3.9 at least, dont change
         # ~/misc/tests/python/bench_unpack.py
-        prefix, key = path[:-1], path[-1]
+        # Using islice allows path to be a list or deque
+        key_index = len(path) - 1
+        prefix = it.islice(path, 0, key_index)
+        key = path[key_index]
+        # prefix, key = path[:-1], path[-1]
         # *prefix, key = path
         for k in prefix:
             d = d[k]
         d[key] = value
 
     def __getitem__(self, path):
         """
@@ -223,16 +228,21 @@
 
         Args:
             path (List): list of indexes into the nested structure
 
         Returns:
             Any: value
         """
+        import itertools as it
         d = self.data
-        prefix, key = path[:-1], path[-1]
+        # Using islice allows path to be a list or deque
+        key_index = len(path) - 1
+        prefix = it.islice(path, 0, key_index)
+        key = path[key_index]
+        # prefix, key = path[:-1], path[-1]
         # *prefix, key = path
         for k in prefix:
             d = d[k]
         return d[key]
 
     def __delitem__(self, path):
         """
```

### Comparing `ubelt-1.2.4/ubelt/util_io.py` & `ubelt-1.3.0/ubelt/util_io.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt/util_io.pyi` & `ubelt-1.3.0/ubelt/util_io.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-from typing import Union
 from os import PathLike
 import io
 
 
-def writeto(fpath: Union[str, PathLike],
+def writeto(fpath: str | PathLike,
             to_write: str,
             aslines: bool = False,
-            verbose: Union[int, None] = None) -> None:
+            verbose: int | None = None) -> None:
     ...
 
 
-def readfrom(fpath: Union[str, PathLike],
+def readfrom(fpath: str | PathLike,
              aslines: bool = False,
              errors: str = 'replace',
-             verbose: Union[int, None] = None) -> str:
+             verbose: int | None = None) -> str:
     ...
 
 
-def touch(fpath: Union[str, PathLike],
+def touch(fpath: str | PathLike,
           mode: int = 438,
-          dir_fd: Union[io.IOBase, None] = None,
+          dir_fd: io.IOBase | None = None,
           verbose: int = 0,
           **kwargs) -> str:
     ...
 
 
-def delete(path: Union[str, PathLike], verbose: bool = False) -> None:
+def delete(path: str | PathLike, verbose: bool = False) -> None:
     ...
```

### Comparing `ubelt-1.2.4/ubelt/util_links.py` & `ubelt-1.3.0/ubelt/util_links.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,14 +67,17 @@
         works in the sense that (1) ``link_path`` will mirror the data from
         ``real_path``, (2) updates to one will effect the other, and (3) no
         extra space will be used.
 
         More details can be found in :mod:`ubelt._win32_links`. On systems that
         support symlinks (e.g. Linux), none of the above applies.
 
+    Note:
+        This function may contain a bug when creating a relative link
+
     References:
         .. [WikiSymLink] https://en.wikipedia.org/wiki/Symbolic_link
         .. [WikiHardLink] https://en.wikipedia.org/wiki/Hard_link
         .. [WikiNTFSLinks] https://en.wikipedia.org/wiki/NTFS_links
 
     Example:
         >>> import ubelt as ub
@@ -134,19 +137,22 @@
         raise ValueError('The link_path argument cannot be empty')
 
     path = normpath(real_path)
     link = normpath(link_path)
 
     if not os.path.isabs(path):
         # if path is not absolute it must be specified relative to link
-        if _can_symlink():
-            path = os.path.relpath(path, os.path.dirname(link))
-        else:  # nocover
+        if not _can_symlink():  # nocover
             # On windows, we need to use absolute paths
             path = os.path.abspath(path)
+        else:
+            # FIXME: This behavior seems like it might be wrong.
+            path = os.path.relpath(path, os.path.dirname(link))
+            # abs_path = join(os.path.dirname(link), path)
+            ...
 
     if verbose:
         print('Symlink: {link} -> {path}'.format(path=path, link=link))
     if islink(link):
         if verbose:
             print('... already exists')
         pointed = _readlink(link)
@@ -154,14 +160,23 @@
             if verbose > 1:
                 print('... and points to the right place')
             return link
         if verbose > 1:
             if not exists(link):
                 print('... but it is broken and points somewhere else: {}'.format(pointed))
             else:
+                # TODO: if we fix the relative symlink bug, this text might be better
+                # import pathlib
+                # abs_path = join(os.path.dirname(link), path)
+                # resolved_path = pathlib.Path(abs_path).resolve()
+                # resolved_pointed = (pathlib.Path(link).parent / pointed).resolve()
+                # if  resolved_path == resolved_pointed:
+                #     print('... and it resolves to the right location')
+                #     print('... but the pointer is different: {}'.format(pointed))
+                # else:
                 print('... but it points somewhere else: {}'.format(pointed))
         if overwrite:
             util_io.delete(link, verbose=verbose > 1)
     elif exists(link):
         if _win32_links is None:
             if verbose:
                 print('... already exists, but its a file. This will error.')
```

### Comparing `ubelt-1.2.4/ubelt/util_list.py` & `ubelt-1.3.0/ubelt/util_list.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt/util_list.pyi` & `ubelt-1.3.0/ubelt/util_list.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Union
 from typing import Mapping
 from typing import Sequence
 from typing import Iterable
 from typing import Any
 from typing import Callable
 from typing import Iterator
 from typing import List
@@ -52,101 +51,98 @@
         ...
 
 
 def iterable(obj: object, strok: bool = False) -> bool:
     ...
 
 
-def take(items: Union[Sequence[VT], Mapping[KT, VT]],
-         indices: Iterable[Union[int, KT]],
+def take(items: Sequence[VT] | Mapping[KT, VT],
+         indices: Iterable[int | KT],
          default: Any = ...) -> Generator[VT, None, None]:
     ...
 
 
 def compress(items: Iterable[Any], flags: Iterable[bool]) -> Iterable[Any]:
     ...
 
 
 def flatten(nested: Iterable[Iterable[Any]]) -> Iterable[Any]:
     ...
 
 
-def unique(
-        items: Iterable[T],
-        key: Union[Callable[[T], Any],
-                   None] = None) -> Generator[T, None, None]:
+def unique(items: Iterable[T],
+           key: Callable[[T], Any] | None = None) -> Generator[T, None, None]:
     ...
 
 
 def argunique(items: Sequence[VT],
-              key: Union[Callable[[VT], Any], None] = None) -> Iterator[int]:
+              key: Callable[[VT], Any] | None = None) -> Iterator[int]:
     ...
 
 
 def unique_flags(items: Sequence[VT],
-                 key: Union[Callable[[VT], Any], None] = None) -> List[bool]:
+                 key: Callable[[VT], Any] | None = None) -> List[bool]:
     ...
 
 
-def boolmask(indices: List[int],
-             maxval: Union[int, None] = None) -> List[bool]:
+def boolmask(indices: List[int], maxval: int | None = None) -> List[bool]:
     ...
 
 
 def iter_window(iterable: Iterable[T],
                 size: int = 2,
                 step: int = 1,
                 wrap: bool = False) -> Iterable[T]:
     ...
 
 
 def allsame(iterable: Iterable[T], eq: Callable[[T, T], bool] = ...) -> bool:
     ...
 
 
-def argsort(indexable: Union[Iterable[VT], Mapping[KT, VT]],
-            key: Union[Callable[[VT], VT], None] = None,
+def argsort(indexable: Iterable[VT] | Mapping[KT, VT],
+            key: Callable[[VT], VT] | None = None,
             reverse: bool = False) -> List[int] | List[KT]:
     ...
 
 
-def argmax(indexable: Union[Iterable[VT], Mapping[KT, VT]],
-           key: Union[Callable[[VT], Any], None] = None) -> int | KT:
+def argmax(indexable: Iterable[VT] | Mapping[KT, VT],
+           key: Callable[[VT], Any] | None = None) -> int | KT:
     ...
 
 
-def argmin(indexable: Union[Iterable[VT], Mapping[KT, VT]],
-           key: Union[Callable[[VT], VT], None] = None) -> int | KT:
+def argmin(indexable: Iterable[VT] | Mapping[KT, VT],
+           key: Callable[[VT], VT] | None = None) -> int | KT:
     ...
 
 
 def peek(iterable: Iterable[T], default: T = ...) -> T:
     ...
 
 
 class IterableMixin:
-    unique: Incomplete
+    unique = unique
     histogram: Incomplete
     duplicates: Incomplete
     group: Incomplete
 
     def chunks(self,
                size: Incomplete | None = ...,
                num: Incomplete | None = ...,
                bordermode: str = ...):
         ...
 
 
 class OrderedIterableMixin(IterableMixin):
-    compress: Incomplete
-    argunique: Incomplete
-    window: Incomplete
+    compress = compress
+    argunique = argunique
+    window = iter_window
 
 
 class UList(list, OrderedIterableMixin):
-    peek: Incomplete
-    take: Incomplete
-    flatten: Incomplete
-    allsame: Incomplete
-    argsort: Incomplete
-    argmax: Incomplete
-    argmin: Incomplete
+    peek = peek
+    take = take
+    flatten = flatten
+    allsame = allsame
+    argsort = argsort
+    argmax = argmax
+    argmin = argmin
```

### Comparing `ubelt-1.2.4/ubelt/util_memoize.py` & `ubelt-1.3.0/ubelt/util_memoize.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt/util_mixins.py` & `ubelt-1.3.0/ubelt/util_mixins.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt/util_path.py` & `ubelt-1.3.0/ubelt/util_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from ubelt import util_io
 import pathlib
 import warnings
 
 
 __all__ = [
     'Path', 'TempDir', 'augpath', 'shrinkuser', 'userhome', 'ensuredir',
-    'expandpath',
+    'expandpath', 'ChDir',
 ]
 
 
 def augpath(path, suffix='', prefix='', ext=None, tail='', base=None,
             dpath=None, relative=None, multidot=False):
     """
     Create a new path with a different extension, basename, directory, prefix,
@@ -162,32 +162,32 @@
 
 def userhome(username=None):
     """
     Returns the path to some user's home directory.
 
     Args:
         username (str | None):
-            name of a user on the system. If not specified, the current user is
+            name of a user on the system. If unspecified, the current user is
             inferred.
 
     Returns:
-        str: userhome_dpath - path to the specified home directory
+        str: path to the specified home directory
 
     Raises:
         KeyError: if the specified user does not exist on the system
 
         OSError: if username is unspecified and the current user cannot be
             inferred
 
     Example:
-        >>> from ubelt.util_path import *  # NOQA
         >>> import ubelt as ub
+        >>> import os
         >>> import getpass
         >>> username = getpass.getuser()
-        >>> userhome_target = expanduser('~')
+        >>> userhome_target = os.path.expanduser('~')
         >>> userhome_got1 = ub.userhome()
         >>> userhome_got2 = ub.userhome(username)
         >>> print(f'username={username}')
         >>> print(f'userhome_got1={userhome_got1}')
         >>> print(f'userhome_got2={userhome_got2}')
         >>> print(f'userhome_target={userhome_target}')
         >>> assert userhome_got1 == userhome_target
@@ -236,15 +236,15 @@
     Args:
         path (str | PathLike): path in system file structure
         home (str): symbol used to replace the home path.
             Defaults to '~', but you might want to use '$HOME' or
             '%USERPROFILE%' instead.
 
     Returns:
-        str: path - shortened path replacing the home directory with a symbol
+        str: shortened path replacing the home directory with a symbol
 
     Example:
         >>> from ubelt.util_path import *  # NOQA
         >>> path = expanduser('~')
         >>> assert path != '~'
         >>> assert shrinkuser(path) == '~'
         >>> assert shrinkuser(path + '1') == path + '1'
@@ -266,15 +266,15 @@
     """
     Shell-like environment variable and tilde path expansion.
 
     Args:
         path (str | PathLike): string representation of a path
 
     Returns:
-        str : expanded path
+        str: expanded path
 
     Example:
         >>> from ubelt.util_path import *  # NOQA
         >>> import ubelt as ub
         >>> assert normpath(ub.expandpath('~/foo')) == join(ub.userhome(), 'foo')
         >>> assert ub.expandpath('foo') == 'foo'
     """
@@ -285,49 +285,49 @@
 
 def ensuredir(dpath, mode=0o1777, verbose=0, recreate=False):
     r"""
     Ensures that directory will exist. Creates new dir with sticky bits by
     default
 
     Args:
-        dpath (str | PathLike | Tuple[str | PathLike]): dir to ensure. Can also
-            be a tuple to send to join
+        dpath (str | PathLike | Tuple[str | PathLike]): dir to ensure.
         mode (int): octal mode of directory
         verbose (int): verbosity
+
         recreate (bool): if True removes the directory and
-            all of its contents and creates a fresh new directory.
-            USE CAREFULLY.
+            all of its contents and creates a new empty directory.
+            DEPRECATED: Use ``ub.Path(dpath).delete().ensuredir()`` instead.
 
     Returns:
-        str: path - the ensured directory
+        str: the ensured directory
 
     SeeAlso:
         :func:`ubelt.Path.ensuredir`
 
-    Note:
-        This function is not thread-safe in Python2
-
     Example:
-        >>> from ubelt.util_path import *  # NOQA
         >>> import ubelt as ub
-        >>> cache_dpath = ub.Path.appdir('ubelt').ensuredir()
-        >>> dpath = join(cache_dpath, 'ensuredir')
-        >>> if exists(dpath):
-        ...     os.rmdir(dpath)
-        >>> assert not exists(dpath)
+        >>> dpath = ub.Path.appdir('ubelt', 'ensuredir')
+        >>> dpath.delete()
+        >>> assert not dpath.exists()
         >>> ub.ensuredir(dpath)
-        >>> assert exists(dpath)
-        >>> os.rmdir(dpath)
+        >>> assert dpath.exists()
+        >>> dpath.delete()
     """
     if isinstance(dpath, (list, tuple)):
         dpath = join(*dpath)
 
     if recreate:
         import ubelt as ub
-        ub.delete(dpath, verbose=verbose)
+        ub.schedule_deprecation(
+            modname='ubelt',
+            migration='Use ``ub.Path(dpath).delete().ensuredir()`` instead', name='recreate',
+            type='argument of ensuredir', deprecate='1.3.0', error='2.0.0',
+            remove='2.1.0',
+        )
+        util_io.delete(dpath, verbose=verbose)
 
     if not exists(dpath):
         if verbose:
             print('Ensuring directory (creating {!r})'.format(dpath))
         os.makedirs(normpath(dpath), mode=mode, exist_ok=True)
     else:
         if verbose:
@@ -348,15 +348,15 @@
     Example:
         >>> import ubelt as ub
         >>> dpath = ub.Path.appdir('ubelt/tests/chdir').ensuredir()
         >>> dir1 = (dpath / 'dir1').ensuredir()
         >>> dir2 = (dpath / 'dir2').ensuredir()
         >>> with ChDir(dpath):
         >>>     assert ub.Path.cwd() == dpath
-        >>>     # changes to the given directory, and then returns back
+        >>>     # change to the given directory, and then returns back
         >>>     with ChDir(dir1):
         >>>         assert ub.Path.cwd() == dir1
         >>>         with ChDir(dir2):
         >>>             assert ub.Path.cwd() == dir2
         >>>             # changes inside the context manager will be reset
         >>>             os.chdir(dpath)
         >>>         assert ub.Path.cwd() == dir1
@@ -390,23 +390,24 @@
             os.chdir(self.orig_dpath)
 
 
 class TempDir:
     """
     Context for creating and cleaning up temporary directories.
 
-    Note:
-        This class will be DEPRECATED. The exact deprecation version and
-        mitigation plan has not yet been developed.
+    DEPRECATED. Use `tempfile` instead.
 
     Note:
         This exists because :class:`tempfile.TemporaryDirectory` was
         introduced in Python 3.2. Thus once ubelt no longer supports
         python 2.7, this class will be deprecated.
 
+    Note:
+        # WE MAY WANT TO KEEP THIS FOR WINDOWS.
+
     Example:
         >>> from ubelt.util_path import *  # NOQA
         >>> with TempDir() as self:
         >>>     dpath = self.dpath
         >>>     assert exists(dpath)
         >>> assert not exists(dpath)
 
@@ -700,23 +701,22 @@
         See :func:`augpath` for more details.
 
         Args:
             prefix (str):
                 Text placed in front of the stem. Defaults to ''.
 
             stemsuffix (str):
-                Text placed between the stem and extension. Default to ''.
-                Note: this is just called suffix in :func:`ub.augpath`.
+                Text placed between the stem and extension. Defaults to ''.
 
             ext (str | None):
                 If specified, replaces the extension
 
             stem (str | None):
                 If specified, replaces the stem (i.e. basename without
-                extension). Note: named base in :func:`augpath`.
+                extension).
 
             dpath (str | PathLike | None):
                 If specified, replaces the specified "relative" directory,
                 which by default is the parent directory.
 
             tail (str | None):
                 If specified, appends this text the very end of the path -
@@ -745,31 +745,26 @@
             NOTICE OF BACKWARDS INCOMPATABILITY.
 
             THE INITIAL RELEASE OF Path.augment suffered from an unfortunate
             variable naming decision that conflicts with pathlib.Path
 
             .. code:: python
 
-            p = ub.Path('the.entire.fname.or.dname.is.the.name.exe')
-            print(f'p     ={p}')
-            print(f'p.name={p.name}')
-            p = ub.Path('the.stem.ends.here.ext')
-            print(f'p     ={p}')
-            print(f'p.stem={p.stem}')
-            p = ub.Path('only.the.last.dot.is.the.suffix')
-            print(f'p       ={p}')
-            print(f'p.suffix={p.suffix}')
-            p = ub.Path('but.all.suffixes.can.be.recovered')
-            print(f'p         ={p}')
-            print(f'p.suffixes={p.suffixes}')
-
-            p.name
-            p.stem
-            p.suffixes
-            p.parts
+                p = ub.Path('the.entire.fname.or.dname.is.the.name.exe')
+                print(f'p     ={p}')
+                print(f'p.name={p.name}')
+                p = ub.Path('the.stem.ends.here.ext')
+                print(f'p     ={p}')
+                print(f'p.stem={p.stem}')
+                p = ub.Path('only.the.last.dot.is.the.suffix')
+                print(f'p       ={p}')
+                print(f'p.suffix={p.suffix}')
+                p = ub.Path('but.all.suffixes.can.be.recovered')
+                print(f'p         ={p}')
+                print(f'p.suffixes={p.suffixes}')
 
         Example:
             >>> import ubelt as ub
             >>> path = ub.Path('foo.bar')
             >>> suffix = '_suff'
             >>> prefix = 'pref_'
             >>> ext = '.baz'
@@ -819,15 +814,14 @@
             schedule_deprecation(
                 'ubelt', 'suffix', 'arg',
                 deprecate='1.1.3', remove='1.4.0',
                 migration='Use stemsuffix instead',
             )
             if not stemsuffix:
                 stemsuffix = suffix
-            import warnings
             warnings.warn(
                 'DEVELOPER NOTICE: The ubelt.Path.augment function may '
                 'experience a BACKWARDS INCOMPATIBLE update in the future '
                 'having to do with the suffix argument to ub.Path.augment '
                 'To avoid any issue use the ``stemsuffix` argument or use the '
                 '``ubelt.augpath`` function instead. '
                 'If you see this warning, please make an '
@@ -899,15 +893,15 @@
         """
         Create a new directory at this given path.
 
         Note:
             The ubelt variant is the same, except it returns the path as well.
 
         Args:
-            mode (int) : perms
+            mode (int) : permission bits
             parents (bool) : create parents
             exist_ok (bool) : fail if exists
 
         Returns:
             Path: returns itself
         """
         super().mkdir(mode=mode, parents=parents, exist_ok=exist_ok)
@@ -920,22 +914,19 @@
         Concise alias of ``Path(os.path.expandvars(self.expanduser()))``
 
         Returns:
             Path: path with expanded environment variables and tildes
 
         Example:
             >>> import ubelt as ub
-            >>> #home_v1 = ub.Path('$HOME').expand()
-            >>> home_v2 = ub.Path('~/').expand()
-            >>> assert isinstance(home_v2, ub.Path)
-            >>> home_v3 = ub.Path.home()
-            >>> #print('home_v1 = {!r}'.format(home_v1))
+            >>> home_v1 = ub.Path('~/').expand()
+            >>> home_v2 = ub.Path.home()
+            >>> print('home_v1 = {!r}'.format(home_v1))
             >>> print('home_v2 = {!r}'.format(home_v2))
-            >>> print('home_v3 = {!r}'.format(home_v3))
-            >>> assert home_v3 == home_v2 # == home_v1
+            >>> assert home_v1 == home_v2
         """
         return self.expandvars().expanduser()
 
     def expandvars(self):
         """
         As discussed in [CPythonIssue21301]_, CPython won't be adding
         expandvars to pathlib. I think this is a mistake, so I added it in this
@@ -949,25 +940,25 @@
         """
         return self.__class__(os.path.expandvars(self))
 
     def ls(self, pattern=None):
         """
         A convenience function to list all paths in a directory.
 
-        This is simply a wraper around iterdir that returns the results as a
-        list instead of a generator. This is mainly for faster navigation in
+        This is a wrapper around iterdir that returns the results as a list
+        instead of a generator. This is mainly for faster navigation in
         IPython. In production code ``iterdir`` or ``glob`` should be used
         instead.
 
         Args:
             pattern (None | str):
                 if specified, performs a glob instead of an iterdir.
 
         Returns:
-            List[Path]: an eagerly evaluated list of paths
+            List['Path']: an eagerly evaluated list of paths
 
         Note:
             When pattern is specified only paths matching the pattern are
             returned, not the paths inside matched directories.  This is
             different than bash semantics where the pattern is first expanded
             and then ls is performed on all matching paths.
 
@@ -998,27 +989,36 @@
             ]
         """
         if pattern is None:
             return list(self.iterdir())
         else:
             return list(self.glob(pattern))
 
+    # TODO:
+    # def _glob(self):
+    #     """
+    #     I would like some way of globbing using patterns contained in the path
+    #     itself. Perhaps this goes into expand?
+    #     """
+    #     import glob
+    #     yield from map(self.__class__, glob.glob(self))
+
     def shrinkuser(self, home='~'):
         """
-        Shrinks your home dir by replacing it with a tilde.
+        Shrinks your home directory by replacing it with a tilde.
 
         This is the inverse of :func:`os.path.expanduser`.
 
         Args:
             home (str): symbol used to replace the home path.
                 Defaults to '~', but you might want to use '$HOME' or
                 '%USERPROFILE%' instead.
 
         Returns:
-            Path: path - shortened path replacing the home directory with a symbol
+            Path: shortened path replacing the home directory with a symbol
 
         Example:
             >>> import ubelt as ub
             >>> path = ub.Path('~').expand()
             >>> assert str(path.shrinkuser()) == '~'
             >>> assert str(ub.Path((str(path) + '1')).shrinkuser()) == str(path) + '1'
             >>> assert str((path / '1').shrinkuser()) == join('~', '1')
@@ -1149,29 +1149,29 @@
             >>> assert 'foo' + base_ == 'foobase'
             >>> assert 'foo' + base2 == str(base2.augment(dpath='foobase'))
         """
         return other + os.fspath(self)
 
     def endswith(self, suffix, *args):
         """
-        Test if the fspath representation endswith a particular string
+        Test if the fspath representation ends with ``suffix``.
 
         Allows ubelt.Path to be a better drop-in replacement when working with
         string-based paths.
 
         Args:
             suffix (str | Tuple[str, ...]):
                 One or more suffixes to test for
 
             *args:
                 start (int): if specified begin testing at this position.
                 end (int): if specified stop testing at this position.
 
         Returns:
-            bool: True if any of the suffixes are matched.
+            bool: True if any of the suffixes match.
 
         Example:
             >>> import ubelt as ub
             >>> base = ub.Path('base')
             >>> assert base.endswith('se')
             >>> assert not base.endswith('be')
             >>> # test start / stop cases
@@ -1184,29 +1184,29 @@
             >>> assert ub.Path('foo').endswith(('foo', 'cdd'))
             >>> assert not ub.Path('bar').endswith(('foo', 'cdd'))
         """
         return os.fspath(self).endswith(suffix, *args)
 
     def startswith(self, prefix, *args):
         """
-        Test if the fspath representation startswith a particular string
+        Test if the fspath representation starts with ``prefix``.
 
         Allows ubelt.Path to be a better drop-in replacement when working with
         string-based paths.
 
         Args:
             prefix (str | Tuple[str, ...]):
                 One or more prefixes to test for
 
             *args:
                 start (int): if specified begin testing at this position.
                 end (int): if specified stop testing at this position.
 
         Returns:
-            bool: True if any of the prefixes are matched.
+            bool: True if any of the prefixes match.
 
         Example:
             >>> import ubelt as ub
             >>> base = ub.Path('base')
             >>> assert base.startswith('base')
             >>> assert not base.startswith('all your')
             >>> # test start / stop cases
@@ -1244,33 +1244,32 @@
     def copy(self, dst, follow_file_symlinks=False, follow_dir_symlinks=False,
              meta='stats', overwrite=False):
         """
         Copy this file or directory to dst.
 
         By default files are never overwritten and symlinks are copied as-is.
 
-
         At a basic level (i.e. ignoring symlinks) for each path argument
         (``src`` and ``dst``) these can either be files, directories, or not
         exist. Given these three states, the following table summarizes how
         this function copies this path to its destination.
 
         TextArt:
 
-            +----------+------------------------+------------------------+------------+
-            | dst      | dir                    | file                   | no-exist   |
-            +----------+                        |                        |            |
-            | src      |                        |                        |            |
-            +==========+========================+========================+============+
-            | dir      | error-or-overwrite-dst | error                  | dst        |
-            +----------+------------------------+------------------------+------------+
-            | file     | dst / src.name         | error-or-overwrite-dst | dst        |
-            +----------+------------------------+------------------------+------------+
-            | no-exist | error                  | error                  | error      |
-            +----------+------------------------+------------------------+------------+
+            +----------+------------------------+------------------------+----------+
+            | dst      | dir                    | file                   | no-exist |
+            +----------+                        |                        |          |
+            | src      |                        |                        |          |
+            +==========+========================+========================+==========+
+            | dir      | error-or-overwrite-dst | error                  | dst      |
+            +----------+------------------------+------------------------+----------+
+            | file     | dst / src.name         | error-or-overwrite-dst | dst      |
+            +----------+------------------------+------------------------+----------+
+            | no-exist | error                  | error                  | error    |
+            +----------+------------------------+------------------------+----------+
 
         In general, the contents of src will be the contents of dst, except for
         the one case where a file is copied into an existing directory. In this
         case the name is used to construct a fully qualified destination.
 
         Ignore:
             # Enumerate cases
@@ -1286,26 +1285,26 @@
                 {'src': 'dir', 'dst': 'no-exist', 'result': 'dst'},
                 {'src': 'dir', 'dst': 'dir',      'result': 'error-or-overwrite-dst'},
                 {'src': 'dir', 'dst': 'file',     'result': 'error'},
             ]
             import pandas as pd
             df = pd.DataFrame(rows)
             piv = df.pivot(['src'], ['dst'], 'result')
-            print(piv.to_markdown(tablefmt="presto"))
-            print(piv.to_markdown(tablefmt="pretty", index=True))
             print(piv.to_markdown(tablefmt="grid", index=True))
 
+            See: ~/code/ubelt/tests/test_path.py for test cases
+
         Args:
             dst (str | PathLike):
-                if `src` is a file and `dst` does not exist, copies this to `dst`
-                if `src` is a file and `dst` is a directory, copies this to `dst / src.name`
+                if ``src`` is a file and ``dst`` does not exist, copies this to ``dst``
+                if ``src`` is a file and ``dst`` is a directory, copies this to ``dst / src.name``
 
-                if `src` is a directory and `dst` does not exist, copies this to `dst`
-                if `src` is a directory and `dst` is a directory, errors unless
-                overwrite is True, in which case, copies this to `dst` and
+                if ``src`` is a directory and ``dst`` does not exist, copies this to ``dst``
+                if ``src`` is a directory and ``dst`` is a directory, errors unless
+                overwrite is True, in which case, copies this to ``dst`` and
                 overwrites anything conflicting path.
 
             follow_file_symlinks (bool):
                 If True and src is a link, the link will be resolved before
                 it is copied (i.e. the data is duplicated), otherwise just
                 the link itself will be copied.
 
@@ -1323,21 +1322,30 @@
                 (i.e.  like :py:func:`shutil.copyfile`).
 
             overwrite (bool):
                 if False, and target file exists, this will raise an error,
                 otherwise the file will be overwritten.
 
         Returns:
-            Path: where the path was actually copied to
+            Path: where the path was copied to
 
         Note:
             This is implemented with a combination of :func:`shutil.copy`,
-            :func:`shutil.copy2`, and :func:`shutil.copytree`, but the The
-            defaults and behavior here are noticably different (and hopefully
-            safer and more intuitive).
+            :func:`shutil.copy2`, and :func:`shutil.copytree`, but the defaults
+            and behavior here are different (and ideally safer and more
+            intuitive).
+
+        Note:
+            Unlike cp on Linux, copying a src directory into a dst directory
+            will not implicitly add the src directory name to the dst
+            directory. This means we cannot copy directory ``<parent>/<dname>``
+            to ``<dst>`` and expect the result to be ``<dst>/<dname>``.
+
+            Conceptually you can expect ``<parent>/<dname>/<contents>``
+            to exist in ``<dst>/<contents>``.
 
         Example:
             >>> import ubelt as ub
             >>> root = ub.Path.appdir('ubelt', 'tests', 'path', 'copy').delete().ensuredir()
             >>> paths = {}
             >>> dpath = (root / 'orig').ensuredir()
             >>> clone0 = (root / 'dst_is_explicit').ensuredir()
@@ -1352,23 +1360,15 @@
             >>> assert all(p.exists() for p in paths.values())
             >>> paths['fpath'].copy(clone0 / 'file0.txt')
             >>> paths['fpath'].copy(clone1)
             >>> paths['empty_dpath'].copy(clone0 / 'empty_dpath')
             >>> paths['empty_dpath'].copy((clone1 / 'empty_dpath_alt').ensuredir(), overwrite=True)
             >>> paths['nested_dpath'].copy(clone0 / 'nested_dpath')
             >>> paths['nested_dpath'].copy((clone1 / 'nested_dpath_alt').ensuredir(), overwrite=True)
-
-        Ignore:
-            import xdev
-            xdev.tree_repr(dpath)
-            xdev.tree_repr(clone0, max_files=10)
-            xdev.tree_repr(clone1, max_files=10)
         """
-        warnings.warn('The ub.Path.copy function is experimental and may change, '
-                      'in corner cases. Primary cases seem stable.')
         import shutil
         copy_function = self._request_copy_function(
             follow_file_symlinks=follow_file_symlinks,
             follow_dir_symlinks=follow_dir_symlinks, meta=meta)
         if self.is_dir():
             if sys.version_info[0:2] < (3, 8):  # nocover
                 copytree = _compat_copytree
@@ -1384,15 +1384,15 @@
                     real_dst = dst / self.name
                 else:
                     real_dst = dst
                 if real_dst.exists():
                     raise FileExistsError('Cannot overwrite existing file unless overwrite=True')
             dst = copy_function(self, dst)
         else:
-            raise Exception
+            raise FileExistsError('The source path does not exist')
         return Path(dst)
 
     def move(self, dst, follow_file_symlinks=False, follow_dir_symlinks=False,
              meta='stats'):
         """
         Move a file from one location to another, or recursively move a
         directory from one location to another.
@@ -1424,56 +1424,40 @@
                 shutil.copyfile).
 
         Note:
             This method will refuse to overwrite anything.
 
             This is implemented via :func:`shutil.move`, which depends heavily
             on :func:`os.rename` semantics. For this reason, this function
-            error if it would overwrite any data. If you want an overwriting
-            variant of move we recommend you either either copy the data, and
-            then delete the original (potentially inefficient), or use
-            :func:`shutil.move` directly if you know how :func:`os.rename`
+            will error if it would overwrite any data. If you want an
+            overwriting variant of move we recommend you either either copy the
+            data, and then delete the original (potentially inefficient), or
+            use :func:`shutil.move` directly if you know how :func:`os.rename`
             works on your system.
 
         Returns:
-            Path: where the path was actually moved to
+            Path: where the path was moved to
 
         Example:
             >>> import ubelt as ub
             >>> dpath = ub.Path.appdir('ubelt', 'tests', 'path', 'move').delete().ensuredir()
             >>> paths = {}
             >>> paths['dpath0'] = (dpath / 'dpath0').ensuredir()
             >>> paths['dpath00'] = (dpath / 'dpath0' / 'sub0').ensuredir()
             >>> paths['fpath000'] = (dpath / 'dpath0' / 'sub0' / 'f0.txt').touch()
             >>> paths['fpath001'] = (dpath / 'dpath0' / 'sub0' / 'f1.txt').touch()
             >>> paths['dpath01'] = (dpath / 'dpath0' / 'sub1').ensuredir()
             >>> print('paths = {}'.format(ub.repr2(paths, nl=1)))
             >>> assert all(p.exists() for p in paths.values())
-            >>> # xdev.tree_repr(dpath, max_files=10)
             >>> paths['dpath0'].move(dpath / 'dpath1')
-            >>> # xdev.tree_repr(dpath, max_files=10)
-
-        Ignore:
-            import xdev
-            xdev.tree_repr(dpath)
         """
-        warnings.warn('The ub.Path.move function is experimental and may change! '
-                      'Do not rely on this behavior yet!')
-
         # Behave more like POSIX move to avoid potential confusing behavior
         if exists(dst):
             raise FileExistsError(
                 'Moves are only allowed to locations that dont exist')
-        # if os.path.isdir(dst):
-        #     with os.scandir(dst) as itr:
-        #         is_empty = next(itr, None) is None
-        #     if not is_empty:
-        #         raise IOError(f'Cannot move {self!r} to {dst!r}. '
-        #                       'Directory not empty')
-
         import shutil
         copy_function = self._request_copy_function(
             follow_file_symlinks=follow_file_symlinks,
             follow_dir_symlinks=follow_dir_symlinks, meta=meta)
         real_dst = shutil.move(self, dst, copy_function=copy_function)
         return Path(real_dst)
 
@@ -1483,15 +1467,14 @@
     def _compat_copytree(src, dst, symlinks=False, ignore=None,
                          copy_function=None, ignore_dangling_symlinks=False,
                          dirs_exist_ok=False):
         """
         A vendored shutil.copytree for older pythons based on the 3.10
         implementation
         """
-        # import stat
         from shutil import Error, copystat, copy2, copy
         with os.scandir(src) as itr:
             entries = list(itr)
 
         if ignore is not None:
             ignored_names = ignore(os.fspath(src), [x.name for x in entries])
         else:
```

### Comparing `ubelt-1.2.4/ubelt/util_platform.py` & `ubelt-1.3.0/ubelt/util_platform.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt/util_str.py` & `ubelt-1.3.0/ubelt/util_str.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt/util_stream.py` & `ubelt-1.3.0/ubelt/util_stream.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt/util_stream.pyi` & `ubelt-1.3.0/ubelt/util_stream.pyi`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt/util_time.py` & `ubelt-1.3.0/ubelt/util_time.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt/util_time.pyi` & `ubelt-1.3.0/ubelt/util_time.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Union
 import datetime
 from _typeshed import Incomplete
 
 
-def timestamp(datetime: Union[datetime.datetime, datetime.date, None] = None,
+def timestamp(datetime: datetime.datetime | datetime.date | None = None,
               precision: int = 0,
-              default_timezone: Union[str, datetime.timezone] = 'local',
+              default_timezone: str | datetime.timezone = 'local',
               allow_dateutil: bool = True) -> str:
     ...
 
 
 def timeparse(stamp: str,
               default_timezone: str = 'local',
               allow_dateutil: bool = True) -> datetime.datetime:
```

### Comparing `ubelt-1.2.4/ubelt/util_zip.py` & `ubelt-1.3.0/ubelt/util_zip.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt/util_zip.pyi` & `ubelt-1.3.0/ubelt/util_zip.pyi`

 * *Files identical despite different names*

### Comparing `ubelt-1.2.4/ubelt.egg-info/PKG-INFO` & `ubelt-1.3.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,72 +1,52 @@
-Metadata-Version: 2.1
-Name: ubelt
-Version: 1.2.4
-Summary: A Python utility belt containing simple tools, a stdlib like feel, and extra batteries.
-Home-page: https://github.com/Erotemic/ubelt
-Author: Jon Crall
-Author-email: erotemic@gmail.com
-License: Apache 2
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Typing :: Stubs Only
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-Provides-Extra: all
-Provides-Extra: all-strict
-Provides-Extra: docs
-Provides-Extra: docs-strict
-Provides-Extra: optional
-Provides-Extra: optional-strict
-Provides-Extra: runtime-strict
-Provides-Extra: tests
-Provides-Extra: tests-strict
-License-File: LICENSE
-
-|GithubActions| |ReadTheDocs| |Pypi| |Downloads| |Codecov| |CircleCI| |Appveyor| 
+|GithubActions| |ReadTheDocs| |Pypi| |Downloads| |Codecov| |CircleCI| |Appveyor|
 
 .. .. |CodeQuality| |TwitterFollow|
 
 
 .. The large version wont work because github strips rst image rescaling. https://i.imgur.com/AcWVroL.png
 .. image:: https://i.imgur.com/PoYIsWE.png
    :height: 100px
    :align: left
 
 
 ..   .. raw:: html
 ..       <img src="https://i.imgur.com/AcWVroL.png" height="100px">
 
-Ubelt is a small library of robust, tested, documented, and simple functions
+
+Ubelt is a utility library for Python with a stdlib like feel.
+
+
+Elevator Pitch:
+===============
+
+Is the Python standard library good?  Yes.  Could it's conciseness be improved?  Yes.  Ubelt aims to provide a quicker way to express things you can do in the standard library.  Progress?  `ub.ProgIter <https://ubelt.readthedocs.io/en/latest/ubelt.progiter.html#ubelt.progiter.ProgIter>`_.  Hashing?  `ub.hash_data <https://ubelt.readthedocs.io/en/latest/ubelt.util_hash.html#ubelt.util_hash.hash_data>`_ / `ub.hash_file <https://ubelt.readthedocs.io/en/latest/ubelt.util_hash.html#ubelt.util_hash.hash_file>`_.  Caching?  `ub.Cacher <https://ubelt.readthedocs.io/en/latest/ubelt.util_cache.html#ubelt.util_cache.Cacher>`_ / `ub.CacheStamp <https://ubelt.readthedocs.io/en/latest/ubelt.util_cache.html#ubelt.util_cache.CacheStamp>`_.  Shell commands?  `ub.cmd <https://ubelt.readthedocs.io/en/latest/ubelt.util_cmd.html#ubelt.util_cmd.cmd>`_. There are similar functions for downloading data, futures-based parallel (or serial) job execution, pretty reprs, path management, iteration, and one of my favorites: set operation enriched dictionaries: `ub.udict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.UDict>`_.
+
+There are 120ish functions and classes to help make your code shorter and easier to express concisely.  The library is fast to install and import, all dependencies are optional.  As of 2023 it is 6 years old, regularly maintained, and mature.  It is well tested and has moderate usage.
+
+To learn more, the function usefulness chart is a good place to start.  This shows how often I use particular functions, and while some of the less used ones are candidates for removal, some of them still worth checking out. For a slightly slower start, read the introduction:
+
+
+Introduction:
+=============
+
+Ubelt is a lightweight library of robust, tested, documented, and simple functions
 that extend the Python standard library. It has a flat API that all behaves
 similarly on Windows, Mac, and Linux (up to some small unavoidable
 differences).  Almost every function in ``ubelt`` was written with a doctest.
 This provides helpful documentation and example usage as well as helping
-achieve 100% test coverage (with minor exceptions on Windows). 
+achieve 100% test coverage (with minor exceptions on Windows).
 
 * Goal: provide simple functions that accomplish common tasks not yet addressed by the python standard library.
 
 * Constraints: Must be low-impact pure python; it should be easy to install and use.
 
 * Method: All functions are written with docstrings and doctests to ensure that a baseline level of documentation and testing always exists (even if functions are copy/pasted into other libraries)
 
-* Motto: Good utilities lift all codes. 
+* Motto: Good utilities lift all codes.
 
 
 Read the docs here: http://ubelt.readthedocs.io/en/latest/
 
 These are some of the tasks that ubelt's API enables:
 
   - extended pathlib with expand, ensuredir, endswith, augment, delete (ub.Path)
@@ -87,17 +67,17 @@
 
   - show loop progress with less overhead than tqdm (ProgIter)
 
   - download a file with optional caching and hash verification (download, grabdata)
 
   - run shell commands (cmd)
 
-  - find a file or directory in candidate locations (find_path, find_exe) 
+  - find a file or directory in candidate locations (find_path, find_exe)
 
-  - string-format nested data structures (urepr)
+  - string-repr for nested data structures (urepr)
 
   - color text with ANSI tags (color_text)
 
   - horizontally concatenate multiline strings (hzcat)
 
   - create cross platform symlinks (symlink)
 
@@ -105,15 +85,15 @@
 
   - check if a particular flag or value is on the command line (argflag, argval)
 
   - memoize functions (memoize, memoize_method, memoize_property)
 
   - build ordered sets (oset)
 
-  - argmax/min/sort on lists and dictionaries (argmin, argsort,) 
+  - argmax/min/sort on lists and dictionaries (argmin, argsort,)
 
   - get a histogram of items or find duplicates in a list (dict_hist, find_duplicates)
 
   - group a sequence of items by some criterion (group_items)
 
 Ubelt is small. Its top-level API is defined using roughly 40 lines:
 
@@ -130,15 +110,15 @@
                                  invert_dict, map_keys, map_vals, map_values,
                                  named_product, odict, sdict, sorted_keys,
                                  sorted_vals, sorted_values, udict, varied_values,)
     from ubelt.util_deprecate import (schedule_deprecation,)
     from ubelt.util_download import (download, grabdata,)
     from ubelt.util_download_manager import (DownloadManager,)
     from ubelt.util_func import (compatible, identity, inject_method,)
-    from ubelt.util_format import (FormatterExtensions, repr2, urepr,)
+    from ubelt.util_repr import (ReprExtensions, urepr,)
     from ubelt.util_futures import (Executor, JobPool,)
     from ubelt.util_io import (delete, touch,)
     from ubelt.util_links import (symlink,)
     from ubelt.util_list import (allsame, argmax, argmin, argsort, argunique,
                                  boolmask, chunks, compress, flatten, iter_window,
                                  iterable, peek, take, unique, unique_flags,)
     from ubelt.util_hash import (hash_data, hash_file,)
@@ -172,15 +152,15 @@
 
     pip install ubelt
 
 Note that our distributions on pypi are signed with GPG. The signing public key
 is ``D297D757``; this should agree with the value in `dev/public_gpg_key`.
 
 
-Function Usefulness 
+Function Usefulness
 ===================
 
 When I had to hand pick a set of functions that I thought were the most useful
 I chose these and provided some comment on why:
 
 .. code:: python
 
@@ -196,98 +176,97 @@
     ub.JobPool   # easy multi-threading / multi-procesing / or single-threaded processing
     ub.ProgIter  # a minimal progress iterator. It's single threaded, informative, and faster than tqdm.
     ub.memoize  # like ``functools.cache``, but uses ub.hash_data if the args are not hashable.
     ub.urepr  # readable representations of nested data structures
 
 
 But a better way might to objectively measure the frequency of usage and built
-a histogram of usefulness. I generated this histogram using ``python dev/maintain/gen_api_for_docs.py``, 
+a histogram of usefulness. I generated this histogram using ``python dev/maintain/gen_api_for_docs.py``,
 which roughly counts the number of times I've used a ubelt function in another
 project. Note: this measure is biased towards older functions.
 
 ================================================================================================================================================ ================
  Function name                                                                                                                                         Usefulness
 ================================================================================================================================================ ================
-`ubelt.repr2 <https://ubelt.readthedocs.io/en/latest/ubelt.util_format.html#ubelt.util_format.repr2>`__                                                      2621
-`ubelt.Path <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.Path>`__                                                             903
-`ubelt.ProgIter <https://ubelt.readthedocs.io/en/latest/ubelt.progiter.html#ubelt.progiter.ProgIter>`__                                                       540
-`ubelt.paragraph <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.paragraph>`__                                                     392
-`ubelt.take <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.take>`__                                                             385
-`ubelt.codeblock <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.codeblock>`__                                                     330
-`ubelt.expandpath <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.expandpath>`__                                                 330
-`ubelt.cmd <https://ubelt.readthedocs.io/en/latest/ubelt.util_cmd.html#ubelt.util_cmd.cmd>`__                                                                 279
-`ubelt.ensuredir <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.ensuredir>`__                                                   258
-`ubelt.odict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.odict>`__                                                           255
-`ubelt.iterable <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.iterable>`__                                                     245
-`ubelt.udict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.udict>`__                                                           238
-`ubelt.ddict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.ddict>`__                                                           234
-`ubelt.NoParam <https://ubelt.readthedocs.io/en/latest/ubelt.util_const.html#ubelt.util_const.NoParam>`__                                                     220
-`ubelt.NiceRepr <https://ubelt.readthedocs.io/en/latest/ubelt.util_mixins.html#ubelt.util_mixins.NiceRepr>`__                                                 219
-`ubelt.map_vals <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.map_vals>`__                                                     216
-`ubelt.flatten <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.flatten>`__                                                       208
-`ubelt.dzip <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dzip>`__                                                             201
-`ubelt.peek <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.peek>`__                                                             197
-`ubelt.oset <https://ubelt.readthedocs.io/en/latest/ubelt.orderedset.html#ubelt.orderedset.oset>`__                                                           191
-`ubelt.argflag <https://ubelt.readthedocs.io/en/latest/ubelt.util_arg.html#ubelt.util_arg.argflag>`__                                                         178
-`ubelt.group_items <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.group_items>`__                                               169
-`ubelt.urepr <https://ubelt.readthedocs.io/en/latest/ubelt.util_format.html#ubelt.util_format.urepr>`__                                                       162
-`ubelt.hash_data <https://ubelt.readthedocs.io/en/latest/ubelt.util_hash.html#ubelt.util_hash.hash_data>`__                                                   154
+`ubelt.urepr <https://ubelt.readthedocs.io/en/latest/ubelt.util_repr.html#ubelt.util_repr.urepr>`__                                                          2893
+`ubelt.Path <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.Path>`__                                                             992
+`ubelt.ProgIter <https://ubelt.readthedocs.io/en/latest/ubelt.progiter.html#ubelt.progiter.ProgIter>`__                                                       544
+`ubelt.paragraph <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.paragraph>`__                                                     482
+`ubelt.take <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.take>`__                                                             387
+`ubelt.codeblock <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.codeblock>`__                                                     358
+`ubelt.expandpath <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.expandpath>`__                                                 331
+`ubelt.cmd <https://ubelt.readthedocs.io/en/latest/ubelt.util_cmd.html#ubelt.util_cmd.cmd>`__                                                                 302
+`ubelt.udict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.udict>`__                                                           271
+`ubelt.ensuredir <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.ensuredir>`__                                                   256
+`ubelt.odict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.odict>`__                                                           253
+`ubelt.iterable <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.iterable>`__                                                     252
+`ubelt.ddict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.ddict>`__                                                           238
+`ubelt.NiceRepr <https://ubelt.readthedocs.io/en/latest/ubelt.util_mixins.html#ubelt.util_mixins.NiceRepr>`__                                                 221
+`ubelt.NoParam <https://ubelt.readthedocs.io/en/latest/ubelt.util_const.html#ubelt.util_const.NoParam>`__                                                     216
+`ubelt.map_vals <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.map_vals>`__                                                     215
+`ubelt.flatten <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.flatten>`__                                                       214
+`ubelt.dzip <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dzip>`__                                                             200
+`ubelt.oset <https://ubelt.readthedocs.io/en/latest/ubelt.orderedset.html#ubelt.orderedset.oset>`__                                                           198
+`ubelt.peek <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.peek>`__                                                             196
+`ubelt.argflag <https://ubelt.readthedocs.io/en/latest/ubelt.util_arg.html#ubelt.util_arg.argflag>`__                                                         177
+`ubelt.group_items <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.group_items>`__                                               171
+`ubelt.hash_data <https://ubelt.readthedocs.io/en/latest/ubelt.util_hash.html#ubelt.util_hash.hash_data>`__                                                   165
 `ubelt.grabdata <https://ubelt.readthedocs.io/en/latest/ubelt.util_download.html#ubelt.util_download.grabdata>`__                                             131
+`ubelt.argval <https://ubelt.readthedocs.io/en/latest/ubelt.util_arg.html#ubelt.util_arg.argval>`__                                                           125
 `ubelt.Timer <https://ubelt.readthedocs.io/en/latest/ubelt.util_time.html#ubelt.util_time.Timer>`__                                                           120
 `ubelt.dict_isect <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dict_isect>`__                                                 113
-`ubelt.dict_hist <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dict_hist>`__                                                   112
-`ubelt.argval <https://ubelt.readthedocs.io/en/latest/ubelt.util_arg.html#ubelt.util_arg.argval>`__                                                           110
+`ubelt.dict_hist <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dict_hist>`__                                                   111
 `ubelt.augpath <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.augpath>`__                                                       106
-`ubelt.identity <https://ubelt.readthedocs.io/en/latest/ubelt.util_func.html#ubelt.util_func.identity>`__                                                     105
+`ubelt.identity <https://ubelt.readthedocs.io/en/latest/ubelt.util_func.html#ubelt.util_func.identity>`__                                                     106
 `ubelt.ensure_app_cache_dir <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.ensure_app_cache_dir>`__                     105
-`ubelt.allsame <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.allsame>`__                                                        98
-`ubelt.memoize <https://ubelt.readthedocs.io/en/latest/ubelt.util_memoize.html#ubelt.util_memoize.memoize>`__                                                  97
-`ubelt.color_text <https://ubelt.readthedocs.io/en/latest/ubelt.util_colors.html#ubelt.util_colors.color_text>`__                                              96
+`ubelt.allsame <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.allsame>`__                                                       102
+`ubelt.memoize <https://ubelt.readthedocs.io/en/latest/ubelt.util_memoize.html#ubelt.util_memoize.memoize>`__                                                  99
+`ubelt.color_text <https://ubelt.readthedocs.io/en/latest/ubelt.util_colors.html#ubelt.util_colors.color_text>`__                                              98
 `ubelt.dict_diff <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dict_diff>`__                                                    95
 `ubelt.delete <https://ubelt.readthedocs.io/en/latest/ubelt.util_io.html#ubelt.util_io.delete>`__                                                              89
+`ubelt.hzcat <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.hzcat>`__                                                              88
+`ubelt.schedule_deprecation <https://ubelt.readthedocs.io/en/latest/ubelt.util_deprecate.html#ubelt.util_deprecate.schedule_deprecation>`__                    87
 `ubelt.named_product <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.named_product>`__                                            85
-`ubelt.compress <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.compress>`__                                                      83
-`ubelt.schedule_deprecation <https://ubelt.readthedocs.io/en/latest/ubelt.util_deprecate.html#ubelt.util_deprecate.schedule_deprecation>`__                    77
-`ubelt.IndexableWalker <https://ubelt.readthedocs.io/en/latest/ubelt.util_indexable.html#ubelt.util_indexable.IndexableWalker>`__                              72
-`ubelt.hzcat <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.hzcat>`__                                                              68
+`ubelt.compress <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.compress>`__                                                      85
+`ubelt.IndexableWalker <https://ubelt.readthedocs.io/en/latest/ubelt.util_indexable.html#ubelt.util_indexable.IndexableWalker>`__                              74
 `ubelt.indent <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.indent>`__                                                            68
-`ubelt.JobPool <https://ubelt.readthedocs.io/en/latest/ubelt.util_futures.html#ubelt.util_futures.JobPool>`__                                                  65
+`ubelt.JobPool <https://ubelt.readthedocs.io/en/latest/ubelt.util_futures.html#ubelt.util_futures.JobPool>`__                                                  67
 `ubelt.unique <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.unique>`__                                                          63
 `ubelt.dict_union <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dict_union>`__                                                  57
 `ubelt.map_keys <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.map_keys>`__                                                      49
 `ubelt.invert_dict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.invert_dict>`__                                                48
+`ubelt.iter_window <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.iter_window>`__                                                46
 `ubelt.timestamp <https://ubelt.readthedocs.io/en/latest/ubelt.util_time.html#ubelt.util_time.timestamp>`__                                                    46
-`ubelt.iter_window <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.iter_window>`__                                                44
 `ubelt.argsort <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.argsort>`__                                                        44
 `ubelt.Cacher <https://ubelt.readthedocs.io/en/latest/ubelt.util_cache.html#ubelt.util_cache.Cacher>`__                                                        43
 `ubelt.find_exe <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.find_exe>`__                                              41
 `ubelt.symlink <https://ubelt.readthedocs.io/en/latest/ubelt.util_links.html#ubelt.util_links.symlink>`__                                                      41
 `ubelt.dict_subset <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.dict_subset>`__                                                41
 `ubelt.writeto <https://ubelt.readthedocs.io/en/latest/ubelt.util_io.html#ubelt.util_io.writeto>`__                                                            40
-`ubelt.chunks <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.chunks>`__                                                          39
+`ubelt.find_duplicates <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.find_duplicates>`__                                        39
+`ubelt.chunks <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.chunks>`__                                                          38
 `ubelt.hash_file <https://ubelt.readthedocs.io/en/latest/ubelt.util_hash.html#ubelt.util_hash.hash_file>`__                                                    37
 `ubelt.modname_to_modpath <https://ubelt.readthedocs.io/en/latest/ubelt.util_import.html#ubelt.util_import.modname_to_modpath>`__                              37
 `ubelt.ensure_unicode <https://ubelt.readthedocs.io/en/latest/ubelt.util_str.html#ubelt.util_str.ensure_unicode>`__                                            33
-`ubelt.sorted_vals <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.sorted_vals>`__                                                33
 `ubelt.memoize_property <https://ubelt.readthedocs.io/en/latest/ubelt.util_memoize.html#ubelt.util_memoize.memoize_property>`__                                33
-`ubelt.CacheStamp <https://ubelt.readthedocs.io/en/latest/ubelt.util_cache.html#ubelt.util_cache.CacheStamp>`__                                                32
-`ubelt.find_duplicates <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.find_duplicates>`__                                        32
-`ubelt.highlight_code <https://ubelt.readthedocs.io/en/latest/ubelt.util_colors.html#ubelt.util_colors.highlight_code>`__                                      31
+`ubelt.highlight_code <https://ubelt.readthedocs.io/en/latest/ubelt.util_colors.html#ubelt.util_colors.highlight_code>`__                                      33
+`ubelt.sorted_vals <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.sorted_vals>`__                                                32
+`ubelt.CacheStamp <https://ubelt.readthedocs.io/en/latest/ubelt.util_cache.html#ubelt.util_cache.CacheStamp>`__                                                30
 `ubelt.WIN32 <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.WIN32>`__                                                    28
 `ubelt.import_module_from_name <https://ubelt.readthedocs.io/en/latest/ubelt.util_import.html#ubelt.util_import.import_module_from_name>`__                    27
-`ubelt.argmax <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.argmax>`__                                                          26
-`ubelt.readfrom <https://ubelt.readthedocs.io/en/latest/ubelt.util_io.html#ubelt.util_io.readfrom>`__                                                          24
-`ubelt.import_module_from_path <https://ubelt.readthedocs.io/en/latest/ubelt.util_import.html#ubelt.util_import.import_module_from_path>`__                    21
+`ubelt.argmax <https://ubelt.readthedocs.io/en/latest/ubelt.util_list.html#ubelt.util_list.argmax>`__                                                          27
+`ubelt.readfrom <https://ubelt.readthedocs.io/en/latest/ubelt.util_io.html#ubelt.util_io.readfrom>`__                                                          23
+`ubelt.import_module_from_path <https://ubelt.readthedocs.io/en/latest/ubelt.util_import.html#ubelt.util_import.import_module_from_path>`__                    22
+`ubelt.compatible <https://ubelt.readthedocs.io/en/latest/ubelt.util_func.html#ubelt.util_func.compatible>`__                                                  17
 `ubelt.touch <https://ubelt.readthedocs.io/en/latest/ubelt.util_io.html#ubelt.util_io.touch>`__                                                                17
+`ubelt.Executor <https://ubelt.readthedocs.io/en/latest/ubelt.util_futures.html#ubelt.util_futures.Executor>`__                                                16
 `ubelt.memoize_method <https://ubelt.readthedocs.io/en/latest/ubelt.util_memoize.html#ubelt.util_memoize.memoize_method>`__                                    16
-`ubelt.Executor <https://ubelt.readthedocs.io/en/latest/ubelt.util_futures.html#ubelt.util_futures.Executor>`__                                                15
-`ubelt.compatible <https://ubelt.readthedocs.io/en/latest/ubelt.util_func.html#ubelt.util_func.compatible>`__                                                  15
 `ubelt.sorted_keys <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.sorted_keys>`__                                                14
+`ubelt.AutoDict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.AutoDict>`__                                                      11
 `ubelt.shrinkuser <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.shrinkuser>`__                                                  11
-`ubelt.AutoDict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.AutoDict>`__                                                      10
 `ubelt.inject_method <https://ubelt.readthedocs.io/en/latest/ubelt.util_func.html#ubelt.util_func.inject_method>`__                                            10
 `ubelt.varied_values <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.varied_values>`__                                             9
 `ubelt.split_modpath <https://ubelt.readthedocs.io/en/latest/ubelt.util_import.html#ubelt.util_import.split_modpath>`__                                         8
 `ubelt.modpath_to_modname <https://ubelt.readthedocs.io/en/latest/ubelt.util_import.html#ubelt.util_import.modpath_to_modname>`__                               8
 `ubelt.get_app_cache_dir <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.get_app_cache_dir>`__                             8
 `ubelt.zopen <https://ubelt.readthedocs.io/en/latest/ubelt.util_zip.html#ubelt.util_zip.zopen>`__                                                               7
 `ubelt.LINUX <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.LINUX>`__                                                     7
@@ -315,26 +294,26 @@
 `ubelt.get_app_data_dir <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.get_app_data_dir>`__                               0
 `ubelt.get_app_config_dir <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.get_app_config_dir>`__                           0
 `ubelt.ensure_app_data_dir <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.ensure_app_data_dir>`__                         0
 `ubelt.ensure_app_config_dir <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.ensure_app_config_dir>`__                     0
 `ubelt.TempDir <https://ubelt.readthedocs.io/en/latest/ubelt.util_path.html#ubelt.util_path.TempDir>`__                                                         0
 `ubelt.TeeStringIO <https://ubelt.readthedocs.io/en/latest/ubelt.util_stream.html#ubelt.util_stream.TeeStringIO>`__                                             0
 `ubelt.SetDict <https://ubelt.readthedocs.io/en/latest/ubelt.util_dict.html#ubelt.util_dict.SetDict>`__                                                         0
+`ubelt.ReprExtensions <https://ubelt.readthedocs.io/en/latest/ubelt.util_repr.html#ubelt.util_repr.ReprExtensions>`__                                           0
 `ubelt.POSIX <https://ubelt.readthedocs.io/en/latest/ubelt.util_platform.html#ubelt.util_platform.POSIX>`__                                                     0
 `ubelt.OrderedSet <https://ubelt.readthedocs.io/en/latest/ubelt.orderedset.html#ubelt.orderedset.OrderedSet>`__                                                 0
-`ubelt.FormatterExtensions <https://ubelt.readthedocs.io/en/latest/ubelt.util_format.html#ubelt.util_format.FormatterExtensions>`__                             0
 `ubelt.DownloadManager <https://ubelt.readthedocs.io/en/latest/ubelt.util_download_manager.html#ubelt.util_download_manager.DownloadManager>`__                 0
 `ubelt.CaptureStream <https://ubelt.readthedocs.io/en/latest/ubelt.util_stream.html#ubelt.util_stream.CaptureStream>`__                                         0
 ================================================================================================================================================ ================
 
 
 Examples
 ========
 
-The most up to date examples are the doctests. 
+The most up to date examples are the doctests.
 We also have a Jupyter notebook: https://github.com/Erotemic/ubelt/blob/main/docs/notebooks/Ubelt%20Demo.ipynb
 
 Here are some examples of some features inside ``ubelt``
 
 Paths
 -----
 
@@ -386,15 +365,15 @@
 usable and will become better integrated in the future. See
 ``ubelt/util_hash.py`` for details.
 
 Caching
 -------
 
 Cache intermediate results from blocks of code inside a script with minimal
-boilerplate or modification to the original code.  
+boilerplate or modification to the original code.
 
 For direct caching of data, use the ``Cacher`` class.  By default results will
 be written to the ubelt's appdir cache, but the exact location can be specified
 via ``dpath`` or the ``appname`` arguments.  Additionally, process dependencies
 can be specified via the ``depends`` argument, which allows for implicit cache
 invalidation.  As far as I can tell, this is the most concise way (4 lines of
 boilerplate) to cache a block of code with existing Python syntax (as of
@@ -430,61 +409,61 @@
     >>> params = {'params1': 1, 'param2': 2}
     >>> expected_fpath = dpath / 'file.txt'
     >>> stamp = ub.CacheStamp('name', dpath=dpath, depends=params,
     >>>                      hasher='sha256', product=expected_fpath,
     >>>                      expires='2101-01-01T000000Z', verbose=3)
     >>> # Start fresh
     >>> stamp.clear()
-    >>>     
+    >>>
     >>> for _ in range(2):
     >>>     if stamp.expired():
     >>>         expected_fpath.write_text('expensive process')
     >>>         stamp.renew()
 
 See `<https://ubelt.readthedocs.io/en/latest/ubelt.util_cache.html>`_ for more
 details about ``Cacher`` and ``CacheStamp``.
 
 Loop Progress
 -------------
 
 ``ProgIter`` is a no-threads attached Progress meter that writes to stdout.  It
 is a mostly drop-in alternative to `tqdm
-<https://pypi.python.org/pypi/tqdm>`__. 
+<https://pypi.python.org/pypi/tqdm>`__.
 *The advantage of ``ProgIter`` is that it does not use any python threading*,
 and therefore can be safer with code that makes heavy use of multiprocessing.
 
 Note: ``ProgIter`` is also defined in a standalone module: ``pip install progiter``)
 
 .. code:: python
 
     >>> import ubelt as ub
     >>> def is_prime(n):
     ...     return n >= 2 and not any(n % i == 0 for i in range(2, n))
     >>> for n in ub.ProgIter(range(1000), verbose=2):
     >>>     # do some work
     >>>     is_prime(n)
-        0/1000... rate=0.00 Hz, eta=?, total=0:00:00, wall=14:05 EST 
-        1/1000... rate=82241.25 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST 
-      257/1000... rate=177204.69 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST 
-      642/1000... rate=94099.22 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST 
-     1000/1000... rate=71886.74 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST 
+        0/1000... rate=0.00 Hz, eta=?, total=0:00:00, wall=14:05 EST
+        1/1000... rate=82241.25 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST
+      257/1000... rate=177204.69 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST
+      642/1000... rate=94099.22 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST
+     1000/1000... rate=71886.74 Hz, eta=0:00:00, total=0:00:00, wall=14:05 EST
 
 
 Command Line Interaction
 ------------------------
 
 The builtin Python ``subprocess.Popen`` module is great, but it can be a
 bit clunky at times. The ``os.system`` command is easy to use, but it
 doesn't have much flexibility. The ``ub.cmd`` function aims to fix this.
 It is as simple to run as ``os.system``, but it returns a dictionary
 containing the return code, standard out, standard error, and the
 ``Popen`` object used under the hood.
 
 This utility is designed to provide as consistent as possible behavior across
-different platforms.  We aim to support Windows, Linux, and OSX. 
+different platforms.  We aim to support Windows, Linux, and OSX.
 
 .. code:: python
 
     >>> import ubelt as ub
     >>> info = ub.cmd('gcc --version')
     >>> print(ub.urepr(info))
     {
@@ -522,15 +501,15 @@
 
 This allows you to easily run a command line executable as part of a
 python process, see what it is doing, and then do something based on its
 output, just as you would if you were interacting with the command line
 itself.
 
 The idea is that ``ub.cmd`` removes the need to think about if you need to pass
-a list of args, or a string. Both will work. 
+a list of args, or a string. Both will work.
 
 New in ``1.0.0``, a third variant with different consequences for executing
 shell commands. Using the ``system=True`` kwarg will directly use ``os.system``
 instead of ``Popen`` entirely. In this mode it is not possible to ``tee`` the
 output because the program is executing directly in the foreground. This is
 useful for doing things like spawning a vim session and returning if the user
 manages to quit vim.
@@ -568,25 +547,25 @@
 provided value. The ``hasher`` keyword argument can be used to change which
 hashing algorithm is used (it defaults to ``"sha512"``).
 
 Dictionary Set Operations
 -------------------------
 
 
-Dictionary operations that are analogous to set operations. 
+Dictionary operations that are analogous to set operations.
 See each funtions documentation for more details on the behavior of the values.
 Typically the last seen value is given priority.
 
-I hope Python decides to add these to the stdlib someday. 
+I hope Python decides to add these to the stdlib someday.
 
 * ``ubelt.dict_union`` corresponds to ``set.union``.
 * ``ubelt.dict_isect`` corresponds to ``set.intersection``.
 * ``ubelt.dict_diff`` corresponds to ``set.difference``.
 
-.. code:: python 
+.. code:: python
 
    >>> d1 = {'a': 1, 'b': 2, 'c': 3}
    >>> d2 = {'c': 10, 'e': 20, 'f': 30}
    >>> d3 = {'e': 10, 'f': 20, 'g': 30, 'a': 40}
    >>> ub.dict_union(d1, d2, d3)
    {'a': 40, 'b': 2, 'c': 10, 'e': 10, 'f': 20, 'g': 30}
 
@@ -594,19 +573,19 @@
    {'c': 3}
 
    >>> ub.dict_diff(d1, d2)
    {'a': 1, 'b': 2}
 
 
 New in Version 1.2.0: Ubelt now contains a dictionary subclass with set
-operations that can be invoked as ``ubelt.SetDict`` or ``ub.sdict``. 
+operations that can be invoked as ``ubelt.SetDict`` or ``ub.sdict``.
 Note that n-ary operations are supported.
 
 
-.. code:: python 
+.. code:: python
 
    >>> d1 = ub.sdict({'a': 1, 'b': 2, 'c': 3})
    >>> d2 = {'c': 10, 'e': 20, 'f': 30}
    >>> d3 = {'e': 10, 'f': 20, 'g': 30, 'a': 40}
    >>> d1 | d2 | d3
    {'a': 40, 'b': 2, 'c': 10, 'e': 10, 'f': 20, 'g': 30}
 
@@ -629,15 +608,15 @@
 id to a list of its corresponding items.  In other words, group a sequence of
 items of type ``VT`` and corresponding keys of type ``KT`` given by a function
 or corresponding list, group them into a ``Dict[KT, List[VT]`` such that each
 key maps to a list of the values associated with the key.  This is similar to
 `pandas.DataFrame.groupby <https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.groupby.html>`_.
 
 Group ids can be specified by a second list containing the id for
-each corresponding item. 
+each corresponding item.
 
 .. code:: python
 
     >>> import ubelt as ub
     >>> # Group via a corresonding list
     >>> item_list    = ['ham',     'jam',   'spam',     'eggs',    'cheese', 'bannana']
     >>> groupid_list = ['protein', 'fruit', 'protein',  'protein', 'dairy',  'fruit']
@@ -657,26 +636,26 @@
     ...     return item.count('a')
     >>> dict(ub.group_items(item_list, grouper))
     {1: ['ham', 'jam', 'spam'], 0: ['eggs', 'cheese'], 3: ['bannana']}
 
 Dictionary Histogram
 --------------------
 
-Find the frequency of items in a sequence. 
+Find the frequency of items in a sequence.
 Given a list or sequence of items, this returns a dictionary mapping each
 unique value in the sequence to the number of times it appeared.
 This is similar to `pandas.DataFrame.value_counts <https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.value_counts.html>`_.
 
 .. code:: python
 
     >>> import ubelt as ub
     >>> item_list = [1, 2, 39, 900, 1232, 900, 1232, 2, 2, 2, 900]
     >>> ub.dict_hist(item_list)
     {1232: 2, 1: 1, 2: 4, 900: 3, 39: 1}
-    
+
 
 Each item can also be given a weight
 
 .. code:: python
 
     >>> import ubelt as ub
     >>> item_list = [1, 2, 39, 900, 1232, 900, 1232, 2, 2, 2, 900]
@@ -752,15 +731,15 @@
     {0: {'A', 'a'}, 1: {'b'}, 2: {'C', 'c'}, 3: {'d'}}
 
 
 New in Version 1.2.0: Ubelt now contains a dictionary subclass ``ubelt.UDict``
 with these quality of life operations (and also inherits from
 ``ubelt.SetDict``). The alias ``ubelt.udict`` can be used for quicker access.
 
-.. code:: python 
+.. code:: python
 
    >>> import ubelt as ub
    >>> d1 = ub.udict({'a': 1, 'b': 2, 'c': 3})
    >>> d1 & {'a', 'c'}
    {'a': 1, 'c': 3}
 
    >>> d1.map_keys(ord)
@@ -778,49 +757,49 @@
 
 Next time you have a default configuration dictionary like and you allow the
 developer to pass keyword arguments to modify these behaviors, consider using
 dictionary intersection (&) to separate out only the relevant parts and
 dictionary union (|) to update those relevant parts.  You can also use
 dictionary differences (-) if you need to check for unused arguments.
 
-.. code:: python 
+.. code:: python
 
     import ubelt as ub
-    
+
     def run_multiple_algos(**kwargs):
         algo1_defaults = {'opt1': 10, 'opt2': 11}
         algo2_defaults = {'src': './here/', 'dst': './there'}
-    
+
         kwargs = ub.udict(kwargs)
-    
+
         algo1_specified = kwargs & algo1_defaults
         algo2_specified = kwargs & algo2_defaults
-    
+
         algo1_config = algo1_defaults | algo1_specified
         algo2_config = algo2_defaults | algo2_specified
-    
+
         unused_kwargs = kwargs - (algo1_defaults | algo2_defaults)
-    
+
         print('algo1_specified = {}'.format(ub.urepr(algo1_specified, nl=1)))
         print('algo2_specified = {}'.format(ub.urepr(algo2_specified, nl=1)))
         print(f'algo1_config={algo1_config}')
         print(f'algo2_config={algo2_config}')
         print(f'The following kwargs were unused {unused_kwargs}')
-    
+
     print(chr(10))
     print('-- Run with some specified --')
     run_multiple_algos(src='box', opt2='fox')
     print(chr(10))
     print('-- Run with extra unspecified --')
     run_multiple_algos(a=1, b=2)
 
 
-Produces: 
+Produces:
 
-.. code:: 
+.. code::
 
     -- Run with some specified --
     algo1_specified = {
         'opt2': 'fox',
     }
     algo2_specified = {
         'src': 'box',
@@ -832,15 +811,15 @@
 
     -- Run with extra unspecified --
     algo1_specified = {}
     algo2_specified = {}
     algo1_config={'opt1': 10, 'opt2': 11}
     algo2_config={'src': './here/', 'dst': './there'}
     The following kwargs were unused {'a': 1, 'b': 2}
-        
+
 
 
 Find Duplicates
 ---------------
 
 Find all duplicate items in a list. More specifically,
 ``ub.find_duplicates`` searches for items that appear more than ``k``
@@ -862,19 +841,19 @@
 the standard place to dump those files differs depending if you are on
 Windows, Linux, or Mac. Ubelt offers a unified functions for determining
 what these paths are.
 
 New in version 1.0.0: the ``ub.Path.appdir`` classmethod provides a way to
 achieve the above with a chainable object oriented interface.
 
-The ``ub.Path.appdir(..., type='cache')``, 
-``ub.Path.appdir(..., type='config')``, and 
+The ``ub.Path.appdir(..., type='cache')``,
+``ub.Path.appdir(..., type='config')``, and
 ``ub.Path.appdir(..., type='data')``
 functions find the correct platform-specific location for these files and
-calling ``ensuredir`` ensures that the directories exist. 
+calling ``ensuredir`` ensures that the directories exist.
 
 The config root directory is ``~/AppData/Roaming`` on Windows,
 ``~/.config`` on Linux and ``~/Library/Application Support`` on Mac. The
 cache root directory is ``~/AppData/Local`` on Windows, ``~/.config`` on
 Linux and ``~/Library/Caches`` on Mac.
 
 Example usage on Linux might look like this:
@@ -930,28 +909,28 @@
 
 Ubelt contains functions to import modules dynamically without using the
 python ``import`` statement. While ``importlib`` exists, the ``ubelt``
 implementation is simpler to user and does not have the disadvantage of
 breaking ``pytest``.
 
 Note ``ubelt`` simply provides an interface to this functionality, the
-core implementation is in ``xdoctest`` (over as of version ``0.7.0``, 
+core implementation is in ``xdoctest`` (over as of version ``0.7.0``,
 the code is statically copied into an autogenerated file such that ``ubelt``
 does not actually depend on ``xdoctest`` during runtime).
 
 .. code:: python
 
     >>> import ubelt as ub
     >>> try:
     >>>     # This is where I keep ubelt on my machine, so it is not expected to work elsewhere.
     >>>     module = ub.import_module_from_path(ub.expandpath('~/code/ubelt/ubelt'))
     >>>     print('module = {!r}'.format(module))
     >>> except OSError:
     >>>     pass
-    >>>         
+    >>>
     >>> module = ub.import_module_from_name('ubelt')
     >>> print('module = {!r}'.format(module))
     >>> #
     >>> try:
     >>>     module = ub.import_module_from_name('does-not-exist')
     >>>     raise AssertionError
     >>> except ModuleNotFoundError:
@@ -1016,16 +995,16 @@
 
 
 External tools
 --------------
 
 Some of the tools in ``ubelt`` also exist as standalone modules. I haven't
 decided if its best to statically copy them into ubelt or require on pypi to
-satisfy the dependency. There are some tools that are not used by default 
-unless you explicitly allow for them. 
+satisfy the dependency. There are some tools that are not used by default
+unless you explicitly allow for them.
 
 Code that is currently statically included (vendored):
 
 -  ProgIter - https://github.com/Erotemic/progiter
 -  OrderedSet - https://github.com/LuminosoInsight/ordered-set
 
 Code that is completely optional, and only used in specific cases:
@@ -1061,15 +1040,15 @@
 
 * Benedict: dictionary tools - https://pypi.org/project/python-benedict/
 * tqdm: progress bars - https://pypi.org/project/tqdm/
 * pooch: data downloading - https://pypi.org/project/pooch/
 * timerit: snippet timing for benchmarks - https://github.com/Erotemic/timerit
 
 
-Ubelt is included in the the [bestof-python list](https://github.com/ml-tooling/best-of-python), 
+Ubelt is included in the the [bestof-python list](https://github.com/ml-tooling/best-of-python),
 which contains many other tools that you should check out.
 
 
 History:
 ========
 
 Ubelt is a migration of the most useful parts of
@@ -1078,29 +1057,29 @@
 
 The ``utool`` library contains a number of useful utility functions, but it
 also contained non-useful functions, as well as the kitchen sink. A number of
 the functions were too specific or not well documented. The ``ubelt`` is a port
 of the simplest and most useful parts of ``utool``.
 
 Note that there are other cool things in ``utool`` that are not in ``ubelt``.
-Notably, the doctest harness ultimately became `xdoctest <https://github.com/Erotemic/xdoctest>`__. 
+Notably, the doctest harness ultimately became `xdoctest <https://github.com/Erotemic/xdoctest>`__.
 Code introspection and dynamic analysis tools were ported to `xinspect <https://github.com/Erotemic/xinspect>`__.
 The more IPython-y tools were ported to `xdev <https://github.com/Erotemic/xdev>`__.
 Parts of it made their way into `scriptconfig <https://gitlab.kitware.com/utils/scriptconfig>`__.
 The init-file generation was moved to `mkinit <https://github.com/Erotemic/mkinit>`__.
 Some vim and system-y things can be found in `vimtk <https://github.com/Erotemic/vimtk>`__.
 
 Development on ubelt started 2017-01-30 and development of utool mostly stopped
 on utool was stopped later that year, but received patches until about 2020.
 Ubelt achieved 1.0.0 and removed support for Python 2.7 and 3.5 on 2022-01-07.
 
 
 Notes.
 ------
-PRs are welcome. 
+PRs are welcome.
 
 Also check out my other projects which are powered by ubelt:
 
 -  xinspect https://github.com/Erotemic/xinspect
 -  xdev https://github.com/Erotemic/xdev
 -  vimtk https://github.com/Erotemic/vimtk
 -  graphid https://github.com/Erotemic/graphid
@@ -1112,15 +1091,15 @@
 And my projects related to ubelt:
 
 -  ProgIter https://github.com/Erotemic/progiter
 -  Timerit https://github.com/Erotemic/timerit
 -  mkinit https://github.com/Erotemic/mkinit
 -  xdoctest https://github.com/Erotemic/xdoctest
 
-  
+
 
 .. |CircleCI| image:: https://circleci.com/gh/Erotemic/ubelt.svg?style=svg
     :target: https://circleci.com/gh/Erotemic/ubelt
 .. |Travis| image:: https://img.shields.io/travis/Erotemic/ubelt/main.svg?label=Travis%20CI
    :target: https://travis-ci.org/Erotemic/ubelt?branch=main
 .. |Appveyor| image:: https://ci.appveyor.com/api/projects/status/github/Erotemic/ubelt?branch=main&svg=True
    :target: https://ci.appveyor.com/project/Erotemic/ubelt/branch/main
@@ -1128,15 +1107,13 @@
    :target: https://codecov.io/github/Erotemic/ubelt?branch=main
 .. |Pypi| image:: https://img.shields.io/pypi/v/ubelt.svg
    :target: https://pypi.python.org/pypi/ubelt
 .. |Downloads| image:: https://img.shields.io/pypi/dm/ubelt.svg
    :target: https://pypistats.org/packages/ubelt
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/ubelt/badge/?version=latest
     :target: http://ubelt.readthedocs.io/en/latest/
-.. |CodeQuality| image:: https://api.codacy.com/project/badge/Grade/4d815305fc014202ba7dea09c4676343   
+.. |CodeQuality| image:: https://api.codacy.com/project/badge/Grade/4d815305fc014202ba7dea09c4676343
     :target: https://www.codacy.com/manual/Erotemic/ubelt?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Erotemic/ubelt&amp;utm_campaign=Badge_Grade
 .. |GithubActions| image:: https://github.com/Erotemic/ubelt/actions/workflows/tests.yml/badge.svg?branch=main
     :target: https://github.com/Erotemic/ubelt/actions?query=branch%3Amain
 .. |TwitterFollow| image:: https://img.shields.io/twitter/follow/Erotemic.svg?style=social
     :target: https://twitter.com/Erotemic
-
-
```

### Comparing `ubelt-1.2.4/ubelt.egg-info/SOURCES.txt` & `ubelt-1.3.0/ubelt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,16 @@
 ubelt/util_memoize.pyi
 ubelt/util_mixins.py
 ubelt/util_mixins.pyi
 ubelt/util_path.py
 ubelt/util_path.pyi
 ubelt/util_platform.py
 ubelt/util_platform.pyi
+ubelt/util_repr.py
+ubelt/util_repr.pyi
 ubelt/util_str.py
 ubelt/util_str.pyi
 ubelt/util_stream.py
 ubelt/util_stream.pyi
 ubelt/util_time.py
 ubelt/util_time.pyi
 ubelt/util_zip.py
```

### Comparing `ubelt-1.2.4/ubelt.egg-info/requires.txt` & `ubelt-1.3.0/ubelt.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 
 [:platform_system == "Windows"]
 jaraco.windows
 
 [all]
 Pygments
-codecov
 pytest-timeout
 python_dateutil
 requests
 xdoctest
 
 [all-strict]
 Pygments==2.2.0
-codecov==2.0.15
 pytest-timeout==1.4.2
 python_dateutil==2.8.1
 requests==2.25.1
 xdoctest==0.14.0
 
 [all-strict:platform_system == "Windows"]
 colorama==0.4.3
@@ -292,21 +290,19 @@
 
 [runtime-strict]
 
 [runtime-strict:platform_system == "Windows"]
 jaraco.windows==3.9.1
 
 [tests]
-codecov
 pytest-timeout
 requests
 xdoctest
 
 [tests-strict]
-codecov==2.0.15
 pytest-timeout==1.4.2
 requests==2.25.1
 xdoctest==0.14.0
 
 [tests-strict:python_version < "2.7" and python_version >= "2.6"]
 coverage==4.5
```

